# Comparing `tmp/picodi-0.8.0.tar.gz` & `tmp/picodi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.8.0.tar", max compression
+gzip compressed data, was "picodi-0.9.0.tar", max compression
```

## Comparing `picodi-0.8.0.tar` & `picodi-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-05-25 21:08:34.311334 picodi-0.8.0/LICENSE
--rw-r--r--   0        0        0    16562 2024-05-25 21:08:34.311334 picodi-0.8.0/README.md
--rw-r--r--   0        0        0      252 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/_internal.py
--rw-r--r--   0        0        0    13996 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/_picodi.py
--rw-r--r--   0        0        0     1392 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/_scopes.py
--rw-r--r--   0        0        0     1625 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/helpers.py
--rw-r--r--   0        0        0        0 2024-05-25 21:08:34.311334 picodi-0.8.0/picodi/py.typed
--rw-r--r--   0        0        0     2680 2024-05-25 21:08:34.311334 picodi-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    17324 1970-01-01 00:00:00.000000 picodi-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-26 13:19:29.274986 picodi-0.9.0/LICENSE
+-rw-r--r--   0        0        0    16562 2024-05-26 13:19:29.274986 picodi-0.9.0/README.md
+-rw-r--r--   0        0        0      252 2024-05-26 13:19:29.274986 picodi-0.9.0/picodi/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-26 13:19:29.274986 picodi-0.9.0/picodi/_internal.py
+-rw-r--r--   0        0        0    14753 2024-05-26 13:19:29.274986 picodi-0.9.0/picodi/_picodi.py
+-rw-r--r--   0        0        0     4149 2024-05-26 13:19:29.274986 picodi-0.9.0/picodi/_scopes.py
+-rw-r--r--   0        0        0     1625 2024-05-26 13:19:29.274986 picodi-0.9.0/picodi/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-26 13:19:29.274986 picodi-0.9.0/picodi/py.typed
+-rw-r--r--   0        0        0     2680 2024-05-26 13:19:29.274986 picodi-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    17324 1970-01-01 00:00:00.000000 picodi-0.9.0/PKG-INFO
```

### Comparing `picodi-0.8.0/LICENSE` & `picodi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.8.0/README.md` & `picodi-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `picodi-0.8.0/picodi/_internal.py` & `picodi-0.9.0/picodi/_internal.py`

 * *Files identical despite different names*

### Comparing `picodi-0.8.0/picodi/_picodi.py` & `picodi-0.9.0/picodi/_picodi.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 import threading
 from collections.abc import Awaitable, Callable, Generator, Iterable, Iterator
 from contextlib import asynccontextmanager, contextmanager
 from dataclasses import asdict, dataclass
 from typing import TYPE_CHECKING, Any, NamedTuple, ParamSpec, TypeVar, cast
 
 from picodi._internal import DummyAwaitable
-from picodi._scopes import GlobalScope, NullScope, Scope, SingletonScope
+from picodi._scopes import (
+    GlobalScope,
+    NullScope,
+    ParentCallScope,
+    Scope,
+    SingletonScope,
+)
 
 if TYPE_CHECKING:
     from inspect import BoundArguments, Signature
 
 DependencyCallable = Callable[..., Any]
 T = TypeVar("T")
 P = ParamSpec("P")
@@ -156,14 +162,15 @@
 
 
 _registry_storage = RegistryStorage()
 _internal_registry = InternalRegistry(_registry_storage)
 registry = Registry(_registry_storage, _internal_registry)
 _scopes: dict[type[Scope], Scope] = {
     NullScope: NullScope(),
+    ParentCallScope: ParentCallScope(),
     SingletonScope: SingletonScope(),
 }
 _lock = threading.RLock()
 
 
 def Provide(dependency: DependencyCallable, /) -> Any:  # noqa: N802
     """
@@ -208,66 +215,84 @@
     ```
     """
     signature = inspect.signature(fn)
     if inspect.iscoroutinefunction(fn) or inspect.isasyncgenfunction(fn):
 
         @functools.wraps(fn)
         async def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+            for scope in _scopes.values():
+                scope.enter_decorator()
             bound, dep_arguments = _arguments_to_getters(
                 args, kwargs, signature, is_async=True
             )
             for name, get_value in dep_arguments.items():
                 bound.arguments[name] = await get_value()
 
             result_or_gen = fn(*bound.args, **bound.kwargs)
             if inspect.isasyncgen(result_or_gen):
                 result = result_or_gen
             else:
                 result = await result_or_gen  # type: ignore[misc]
 
             for scope in _scopes.values():
+                scope.exit_decorator()
                 coro = scope.close_local()
                 if coro is not None:
                     await coro
             return cast("T", result)
 
     else:
 
         @functools.wraps(fn)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+            for scope in _scopes.values():
+                scope.enter_decorator()
             bound, dep_arguments = _arguments_to_getters(
                 args, kwargs, signature, is_async=False
             )
             for name, get_value in dep_arguments.items():
                 bound.arguments[name] = get_value()
 
             result = fn(*bound.args, **bound.kwargs)
             for scope in _scopes.values():
+                scope.exit_decorator()
                 scope.close_local()
             return result
 
     return wrapper  # type: ignore[return-value]
 
 
+def dependency(*, scope_class: type[Scope] = NullScope) -> Callable[[TC], TC]:
+    """
+    Decorator to declare a dependency. You don't need to use it with default arguments,
+    use it only if you want to change the scope of the dependency.
+    """
+
+    if scope_class not in _scopes:
+        _scopes[scope_class] = scope_class()
+
+    def decorator(fn: TC) -> TC:
+        _internal_registry.add(
+            fn, scope_class=scope_class, in_use=False, override_scope=True
+        )
+        return fn
+
+    return decorator
+
+
 def resource(fn: TC) -> TC:
     """
     Decorator to declare a resource. Resource is a dependency that should be
     called only once, cached and shared across the application.
     On shutdown, all resources will be closed
     (you need to call `shutdown_resources` manually).
     Use it with a dependency generator function to declare a resource.
     Should be placed last in the decorator chain (on top).
     """
-    _internal_registry.add(
-        fn,
-        scope_class=SingletonScope,
-        in_use=False,
-        override_scope=True,
-    )
-    return fn
+    return dependency(scope_class=SingletonScope)(fn)
 
 
 def init_resources() -> Awaitable:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shutting down.
     """
```

### Comparing `picodi-0.8.0/picodi/helpers.py` & `picodi-0.9.0/picodi/helpers.py`

 * *Files identical despite different names*

### Comparing `picodi-0.8.0/pyproject.toml` & `picodi-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.8.0"
+version = "0.9.0"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
```

### Comparing `picodi-0.8.0/PKG-INFO` & `picodi-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.8.0
+Version: 0.9.0
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


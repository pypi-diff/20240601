# Comparing `tmp/graphene_django_query_optimizer-0.7.1.tar.gz` & `tmp/graphene_django_query_optimizer-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.7.1.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.7.2.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.7.1.tar` & `graphene_django_query_optimizer-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/LICENSE
--rw-r--r--   0        0        0     3151 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/README.md
--rw-r--r--   0        0        0     6906 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      579 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11972 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/ast.py
--rw-r--r--   0        0        0     8533 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/errors.py
--rw-r--r--   0        0        0    18399 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/filter.py
--rw-r--r--   0        0        0     5697 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    12422 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/py.typed
--rw-r--r--   0        0        0     3600 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/selections.py
--rw-r--r--   0        0        0     2520 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/settings.py
--rw-r--r--   0        0        0     3212 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/types.py
--rw-r--r--   0        0        0     4075 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/typing.py
--rw-r--r--   0        0        0     6842 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/utils.py
--rw-r--r--   0        0        0     3888 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3151 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/README.md
+-rw-r--r--   0        0        0     6906 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      579 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11972 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8533 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/errors.py
+-rw-r--r--   0        0        0    18399 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5697 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    13282 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/py.typed
+-rw-r--r--   0        0        0     3600 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/selections.py
+-rw-r--r--   0        0        0     2520 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/settings.py
+-rw-r--r--   0        0        0     3212 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/types.py
+-rw-r--r--   0        0        0     4075 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6842 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3888 2024-05-31 10:22:16.821170 graphene_django_query_optimizer-0.7.2/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.7.2/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.7.1/LICENSE` & `graphene_django_query_optimizer-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/README.md` & `graphene_django_query_optimizer-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/pyproject.toml` & `graphene_django_query_optimizer-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.7.1"
+version = "0.7.2"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
```

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/__init__.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/compiler.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/fields.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/filter_info.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 if TYPE_CHECKING:
     from .types import DjangoObjectType
     from .typing import (
         Any,
         ExpressionKind,
         GQLInfo,
         GraphQLFilterInfo,
+        Literal,
         Optional,
         QuerySetResolver,
         TModel,
         ToManyField,
     )
 
 __all__ = [
@@ -288,7 +289,29 @@
         if callable(getattr(object_type, "pre_compilation_hook", None)):
             object_type.pre_compilation_hook(self)
 
         # Run pre-compilation for all select related optimizers, since they might add annotations,
         # which would promote the select related to prefetch related.
         for optimizer in self.select_related.values():
             optimizer.pre_compilation()
+
+    def has_child_optimizer(self, name: str) -> bool:
+        return name in self.select_related or name in self.prefetch_related
+
+    def get_child_optimizer(self, name: str) -> QueryOptimizer | None:
+        return self.select_related.get(name) or self.prefetch_related.get(name)
+
+    def get_or_set_child_optimizer(
+        self,
+        name: str,
+        optimizer: QueryOptimizer,
+        *,
+        set_as: Literal["select_related", "prefetch_related"] = "select_related",
+    ) -> QueryOptimizer:
+        maybe_optimizer = self.select_related.get(name)
+        if maybe_optimizer is not None:
+            return maybe_optimizer
+        maybe_optimizer = self.prefetch_related.get(name)
+        if maybe_optimizer is not None:
+            return maybe_optimizer
+        getattr(self, set_as)[name] = optimizer
+        return optimizer
```

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/selections.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/selections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/types.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/typing.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.7.2/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.1/PKG-INFO` & `graphene_django_query_optimizer-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.7.1
+Version: 0.7.2
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```


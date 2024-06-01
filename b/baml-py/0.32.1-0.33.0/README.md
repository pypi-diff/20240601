# Comparing `tmp/baml_py-0.32.1-cp38-abi3-win_amd64.whl.zip` & `tmp/baml_py-0.33.0-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 4454154 bytes, number of entries: 13
--rw-r--r--  4.6 unx      354 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/WHEEL
--rw-r--r--  4.6 unx       54 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11556 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    11556 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx     3406 b- defN 24-May-31 09:54 baml_py/async_context_vars.py
--rw-r--r--  4.6 unx     4306 b- defN 24-May-31 09:54 baml_py/baml_py.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-May-31 09:54 baml_py/py.typed
--rw-r--r--  4.6 unx     2474 b- defN 24-May-31 09:54 baml_py/stream.py
--rw-r--r--  4.6 unx     4330 b- defN 24-May-31 09:54 baml_py/type_builder.py
--rw-r--r--  4.6 unx      506 b- defN 24-May-31 09:54 baml_py/__init__.py
--rwxr-xr-x  4.6 unx 11766272 b- defN 24-May-31 09:54 baml_py/baml_py.pyd
--rw-r--r--  4.6 unx     1053 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/RECORD
-13 files, 11805961 bytes uncompressed, 4452406 bytes compressed:  62.3%
+Zip file size: 4409893 bytes, number of entries: 13
+-rw-r--r--  4.6 unx      354 b- defN 24-Jun-01 02:37 baml_py-0.33.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-Jun-01 02:37 baml_py-0.33.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx       54 b- defN 24-Jun-01 02:37 baml_py-0.33.0.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11556 b- defN 24-Jun-01 02:37 baml_py-0.33.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    11556 b- defN 24-Jun-01 02:37 baml_py-0.33.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     3241 b- defN 24-Jun-01 02:37 baml_py/async_context_vars.py
+-rw-r--r--  4.6 unx     4151 b- defN 24-Jun-01 02:37 baml_py/baml_py.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-Jun-01 02:37 baml_py/py.typed
+-rw-r--r--  4.6 unx     2474 b- defN 24-Jun-01 02:37 baml_py/stream.py
+-rw-r--r--  4.6 unx     4330 b- defN 24-Jun-01 02:37 baml_py/type_builder.py
+-rw-r--r--  4.6 unx      506 b- defN 24-Jun-01 02:37 baml_py/__init__.py
+-rwxr-xr-x  4.6 unx 11628544 b- defN 24-Jun-01 02:37 baml_py/baml_py.pyd
+-rw-r--r--  4.6 unx     1053 b- defN 24-Jun-01 02:37 baml_py-0.33.0.dist-info/RECORD
+13 files, 11667913 bytes uncompressed, 4408145 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: baml_py-0.32.1.dist-info/METADATA
+Filename: baml_py-0.33.0.dist-info/METADATA
 Comment: 
 
-Filename: baml_py-0.32.1.dist-info/WHEEL
+Filename: baml_py-0.33.0.dist-info/WHEEL
 Comment: 
 
-Filename: baml_py-0.32.1.dist-info/entry_points.txt
+Filename: baml_py-0.33.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: baml_py-0.32.1.dist-info/license_files/LICENSE
+Filename: baml_py-0.33.0.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: baml_py-0.32.1.dist-info/license_files/LICENSE
+Filename: baml_py-0.33.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: baml_py/async_context_vars.py
 Comment: 
 
 Filename: baml_py/baml_py.pyi
 Comment: 
@@ -30,11 +30,11 @@
 
 Filename: baml_py/__init__.py
 Comment: 
 
 Filename: baml_py/baml_py.pyd
 Comment: 
 
-Filename: baml_py-0.32.1.dist-info/RECORD
+Filename: baml_py-0.33.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## baml_py/async_context_vars.py

```diff
@@ -37,19 +37,16 @@
         self, name: str, args: typing.Dict[str, typing.Any]
     ) -> BamlSpan:
         mng = self.ctx.get()
         cln = mng.deep_clone()
         self.ctx.set(cln)
         return BamlSpan.new(self.rt, name, args, cln)
 
-    async def end_trace(self, span: BamlSpan, response: typing.Any) -> None:
-        await span.finish(response, self.ctx.get())
-
-    def end_trace_sync(self, span: BamlSpan, response: typing.Any) -> None:
-        span.finish_sync(response, self.ctx.get())
+    def end_trace(self, span: BamlSpan, response: typing.Any) -> None:
+        span.finish(response, self.ctx.get())
 
     def flush(self) -> None:
         self.rt.flush()
 
     def trace_fn(self, func: F) -> F:
         func_name = func.__name__
         signature = inspect.signature(func).parameters
@@ -65,18 +62,18 @@
                     param_names[i] if i < len(param_names) else f"<arg:{i}>": arg
                     for i, arg in enumerate(args)
                 }
                 params.update(kwargs)
                 span = self.start_trace_async(func_name, params)
                 try:
                     response = await func(*args, **kwargs)
-                    await self.end_trace(span, response)
+                    self.end_trace(span, response)
                     return response
                 except Exception as e:
-                    await self.end_trace(span, e)
+                    self.end_trace(span, e)
                     raise e
 
             return typing.cast(F, async_wrapper)
 
         else:
 
             @functools.wraps(func)
@@ -85,14 +82,14 @@
                     param_names[i] if i < len(param_names) else f"<arg:{i}>": arg
                     for i, arg in enumerate(args)
                 }
                 params.update(kwargs)
                 span = self.start_trace_sync(func_name, params)
                 try:
                     response = func(*args, **kwargs)
-                    self.end_trace_sync(span, response)
+                    self.end_trace(span, response)
                     return response
                 except Exception as e:
-                    self.end_trace_sync(span, e)
+                    self.end_trace(span, e)
                     raise e
 
             return typing.cast(F, wrapper)
```

## baml_py/baml_py.pyi

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, Tuple
 
 class FunctionResult:
     """The result of a BAML function call.
 
     Represents any of:
 
         - a successful LLM call, with a successful type parse
@@ -28,24 +28,22 @@
     def __str__(self) -> str: ...
     def on_event(
         self, on_event: Callable[[FunctionResult], None]
     ) -> FunctionResultStream: ...
     async def done(self, ctx: RuntimeContextManager) -> FunctionResult: ...
 
 class BamlImagePy:
+    @staticmethod
     def from_url(url: str) -> BamlImagePy: ...
+    @staticmethod
     def from_base64(base64: str, media_type: str) -> BamlImagePy: ...
-    @property
-    def url(self) -> Optional[str]: ...
-    @url.setter
-    def url(self, value: Optional[str]) -> None: ...
-    @property
-    def base64(self) -> Optional[str]: ...
-    @base64.setter
-    def base64(self, value: Optional[str]) -> None: ...
+    def is_url(self) -> bool: ...
+    def is_base64(self) -> bool: ...
+    def as_url(self) -> str: ...
+    def as_base64(self) -> Tuple[str, str]: ...
 
 class RuntimeContextManager:
     def upsert_tags(self, tags: Dict[str, Any]) -> None: ...
     def deep_clone(self) -> RuntimeContextManager: ...
 
 class BamlRuntime:
     @staticmethod
@@ -76,16 +74,15 @@
     @staticmethod
     def new(
         runtime: BamlRuntime,
         function_name: str,
         args: Dict[str, Any],
         ctx: RuntimeContextManager,
     ) -> BamlSpan: ...
-    async def finish(self, result: Any, ctx: RuntimeContextManager) -> str | None: ...
-    def finish_sync(self, result: Any, ctx: RuntimeContextManager) -> str | None: ...
+    def finish(self, result: Any, ctx: RuntimeContextManager) -> str | None: ...
 
 class TypeBuilder:
     def __init__(self) -> None: ...
     def enum(self, name: str) -> EnumBuilder: ...
     def class_(self, name: str) -> ClassBuilder: ...
     def string(self) -> FieldType: ...
     def int(self) -> FieldType: ...
```

## Comparing `baml_py-0.32.1.dist-info/license_files/LICENSE` & `baml_py-0.33.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `baml_py-0.32.1.dist-info/RECORD` & `baml_py-0.33.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-baml_py-0.32.1.dist-info/METADATA,sha256=_a1mYpwUxJARHfPPxpSGY1nk6JPVxBMsYRtX2J6GVs4,354
-baml_py-0.32.1.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
-baml_py-0.32.1.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
-baml_py-0.32.1.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-baml_py-0.32.1.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-baml_py/async_context_vars.py,sha256=QfnNjQIT9MtpqbfuD4v0hWlZIdn2JmNu8U-iKpHjTrc,3406
-baml_py/baml_py.pyi,sha256=mDSpyFs8B8DeGJFucD5mjgDFmptTo5LAHTXBWAM5epU,4306
+baml_py-0.33.0.dist-info/METADATA,sha256=KiSCnV4tusElf3SvLqj5CzGSSj9PHgNPLIDXJJuvl5w,354
+baml_py-0.33.0.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
+baml_py-0.33.0.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
+baml_py-0.33.0.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py-0.33.0.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py/async_context_vars.py,sha256=lr2wJedu3TCNn62byJUAsIbuBB_Y0Dp7Qhf8O132tv4,3241
+baml_py/baml_py.pyi,sha256=xwq3CG1EONMS2g9PE51a_n9U2yzMvSK4IBGC398rDb8,4151
 baml_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 baml_py/stream.py,sha256=B4mpGnqAmU7DFHJPiAAAiNIeX5wgLJhXLZp9Pqb9-AY,2474
 baml_py/type_builder.py,sha256=v3yiY2VtGuCEECr0jh7OB3ueWSiSwj-8IETXQuSIYl0,4330
 baml_py/__init__.py,sha256=-y49naDuvHdmpkmUEqZBESlBNx6W4qsPOPu9KlrMT10,506
-baml_py/baml_py.pyd,sha256=VA59JVBmRUa8WvisjG8goUNZsj85Vc-LHme3B4XOya4,11766272
-baml_py-0.32.1.dist-info/RECORD,,
+baml_py/baml_py.pyd,sha256=-O0TP5mAZgsX4c8yywCgdzYgJPEqczrm5ytGBIBBOuM,11628544
+baml_py-0.33.0.dist-info/RECORD,,
```


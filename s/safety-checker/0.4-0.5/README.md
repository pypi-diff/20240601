# Comparing `tmp/safety_checker-0.4.tar.gz` & `tmp/safety_checker-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safety_checker-0.4.tar", last modified: Sun Dec  3 17:39:52 2023, max compression
+gzip compressed data, was "safety_checker-0.5.tar", last modified: Sat Jun  1 08:37:58 2024, max compression
```

## Comparing `safety_checker-0.4.tar` & `safety_checker-0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-11-29 13:58:31.394004 safety_checker-0.4/LICENSE
--rw-r--r--   0        0        0      622 2023-12-01 05:38:22.658900 safety_checker-0.4/README.md
--rw-r--r--   0        0        0      615 2023-12-03 17:39:52.611139 safety_checker-0.4/pyproject.toml
--rw-r--r--   0        0        0      235 2023-12-01 05:19:24.099102 safety_checker-0.4/safety_checker/__init__.py
--rw-r--r--   0        0        0     4331 2023-12-03 17:37:09.221157 safety_checker-0.4/safety_checker/sdhook.py
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 safety_checker-0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-29 13:58:31.394004 safety_checker-0.5/LICENSE
+-rw-r--r--   0        0        0      622 2023-12-01 05:38:22.658900 safety_checker-0.5/README.md
+-rw-r--r--   0        0        0      615 2024-06-01 08:37:58.237698 safety_checker-0.5/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-12-01 05:19:24.099102 safety_checker-0.5/safety_checker/__init__.py
+-rw-r--r--   0        0        0     4455 2024-06-01 08:26:44.357762 safety_checker-0.5/safety_checker/sdhook.py
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 safety_checker-0.5/PKG-INFO
```

### Comparing `safety_checker-0.4/LICENSE` & `safety_checker-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `safety_checker-0.4/README.md` & `safety_checker-0.5/README.md`

 * *Files identical despite different names*

### Comparing `safety_checker-0.4/pyproject.toml` & `safety_checker-0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "safety-checker"
-version = "0.4"
+version = "0.5"
 description = "Integrate stable diffusion safety checker / NSFW image detection into web service like FastAPI."
 authors = [
     { name = "iyume", email = "iyumelive@gmail.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = [
```

### Comparing `safety_checker-0.4/safety_checker/sdhook.py` & `safety_checker-0.5/safety_checker/sdhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,21 @@
         self.safety_checker = self.safety_checker.to(
             cast(Any, device),  # type shit from diffusers
         )
         return self
 
     def run(self, image: ImageInput) -> bool:
         """Run safety checker. Returns True if any input images have nsfw content."""
+        has_nsfw = self.run_batch(image)
+        return any(has_nsfw)
+
+    def run_batch(self, image: ImageInput) -> list[bool]:
         if not self.feature_extractor or not self.safety_checker:
             raise ValueError
         # No need to do input image normalization
         safety_checker_input = self.feature_extractor(image, return_tensors="pt")
         has_nsfw: list[bool]
         _, has_nsfw = self.safety_checker(
             images=safety_checker_input.pixel_values,  # dummy input
             clip_input=safety_checker_input.pixel_values.to(self.device),
         )
-        return any(has_nsfw)
+        return has_nsfw
```

### Comparing `safety_checker-0.4/PKG-INFO` & `safety_checker-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safety-checker
-Version: 0.4
+Version: 0.5
 Summary: Integrate stable diffusion safety checker / NSFW image detection into web service like FastAPI.
 Author-Email: iyume <iyumelive@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.8
 Requires-Dist: Pillow>=8.4.0
 Requires-Dist: transformers>=4.0; extra == "sdhook"
 Requires-Dist: diffusers[torch]>=0.20; extra == "sdhook"
```


# Comparing `tmp/lycoris_lora-3.0.0.dev6.tar.gz` & `tmp/lycoris_lora-3.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-3.0.0.dev6.tar", last modified: Thu May 30 16:56:04 2024, max compression
+gzip compressed data, was "lycoris_lora-3.0.0.dev7.tar", last modified: Sat Jun  1 11:34:31 2024, max compression
```

## Comparing `lycoris_lora-3.0.0.dev6.tar` & `lycoris_lora-3.0.0.dev7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 16:56:04.421377 lycoris_lora-3.0.0.dev6/
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-3.0.0.dev6/LICENSE.md
--rw-rw-rw-   0        0        0      465 2024-05-30 16:56:04.420377 lycoris_lora-3.0.0.dev6/PKG-INFO
--rw-rw-rw-   0        0        0    12433 2024-05-15 08:22:33.000000 lycoris_lora-3.0.0.dev6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 16:56:04.399356 lycoris_lora-3.0.0.dev6/lycoris/
--rw-rw-rw-   0        0        0      588 2024-05-18 10:27:24.000000 lycoris_lora-3.0.0.dev6/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev6/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:56:04.401356 lycoris_lora-3.0.0.dev6/lycoris/functional/
--rw-rw-rw-   0        0        0      251 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev6/lycoris/functional/__init__.py
--rw-rw-rw-   0        0        0     2499 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev6/lycoris/functional/general.py
--rw-rw-rw-   0        0        0     3186 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev6/lycoris/functional/locon.py
--rw-rw-rw-   0        0        0     6387 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev6/lycoris/functional/loha.py
--rw-rw-rw-   0        0        0    31398 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev6/lycoris/kohya.py
--rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-3.0.0.dev6/lycoris/logging.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:56:04.405861 lycoris_lora-3.0.0.dev6/lycoris/modules/
--rw-rw-rw-   0        0        0     4461 2024-05-30 12:50:16.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     9568 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/base.py
--rw-rw-rw-   0        0        0     8349 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/boft.py
--rw-rw-rw-   0        0        0     7743 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/diag_oft.py
--rw-rw-rw-   0        0        0     7032 2024-05-25 08:12:37.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0     6439 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/full.py
--rw-rw-rw-   0        0        0     9077 2024-05-25 03:28:17.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0     5963 2024-05-25 03:59:59.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    11595 2024-05-30 15:24:12.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    11372 2024-05-25 03:26:29.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    16571 2024-05-25 03:28:25.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0     3557 2024-05-18 09:12:34.000000 lycoris_lora-3.0.0.dev6/lycoris/modules/norms.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:56:04.408867 lycoris_lora-3.0.0.dev6/lycoris/utils/
--rw-rw-rw-   0        0        0    24042 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev6/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-3.0.0.dev6/lycoris/utils/bnb.py
--rw-rw-rw-   0        0        0      102 2024-05-25 08:12:37.000000 lycoris_lora-3.0.0.dev6/lycoris/utils/general.py
--rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev6/lycoris/utils/logger.py
--rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev6/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev6/lycoris/utils/xformers_utils.py
--rw-rw-rw-   0        0        0    18777 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev6/lycoris/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:56:04.420377 lycoris_lora-3.0.0.dev6/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      465 2024-05-30 16:56:04.000000 lycoris_lora-3.0.0.dev6/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      904 2024-05-30 16:56:04.000000 lycoris_lora-3.0.0.dev6/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 16:56:04.000000 lycoris_lora-3.0.0.dev6/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-3.0.0.dev6/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2024-05-30 16:56:04.000000 lycoris_lora-3.0.0.dev6/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-30 16:56:04.000000 lycoris_lora-3.0.0.dev6/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 16:56:04.421377 lycoris_lora-3.0.0.dev6/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-05-30 15:24:23.000000 lycoris_lora-3.0.0.dev6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:34:31.356703 lycoris_lora-3.0.0.dev7/
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-3.0.0.dev7/LICENSE.md
+-rw-rw-rw-   0        0        0      465 2024-06-01 11:34:31.356703 lycoris_lora-3.0.0.dev7/PKG-INFO
+-rw-rw-rw-   0        0        0    12433 2024-05-15 08:22:33.000000 lycoris_lora-3.0.0.dev7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 11:34:31.334676 lycoris_lora-3.0.0.dev7/lycoris/
+-rw-rw-rw-   0        0        0      588 2024-05-18 10:27:24.000000 lycoris_lora-3.0.0.dev7/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev7/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:34:31.336679 lycoris_lora-3.0.0.dev7/lycoris/functional/
+-rw-rw-rw-   0        0        0      251 2024-05-17 14:23:10.000000 lycoris_lora-3.0.0.dev7/lycoris/functional/__init__.py
+-rw-rw-rw-   0        0        0     2499 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev7/lycoris/functional/general.py
+-rw-rw-rw-   0        0        0     3186 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev7/lycoris/functional/locon.py
+-rw-rw-rw-   0        0        0     6387 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev7/lycoris/functional/loha.py
+-rw-rw-rw-   0        0        0    31378 2024-06-01 11:33:51.000000 lycoris_lora-3.0.0.dev7/lycoris/kohya.py
+-rw-rw-rw-   0        0        0     1053 2024-02-05 11:33:20.000000 lycoris_lora-3.0.0.dev7/lycoris/logging.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:34:31.341680 lycoris_lora-3.0.0.dev7/lycoris/modules/
+-rw-rw-rw-   0        0        0     4461 2024-05-30 12:50:16.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     9568 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/base.py
+-rw-rw-rw-   0        0        0     8349 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/boft.py
+-rw-rw-rw-   0        0        0     7743 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/diag_oft.py
+-rw-rw-rw-   0        0        0     7032 2024-05-25 08:12:37.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0     6439 2024-05-24 08:53:18.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/full.py
+-rw-rw-rw-   0        0        0     9077 2024-05-25 03:28:17.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0     5963 2024-05-25 03:59:59.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    11595 2024-05-30 15:24:12.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    11372 2024-05-25 03:26:29.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    16571 2024-05-25 03:28:25.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/lokr.py
+-rw-rw-rw-   0        0        0     3557 2024-05-18 09:12:34.000000 lycoris_lora-3.0.0.dev7/lycoris/modules/norms.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:34:31.343183 lycoris_lora-3.0.0.dev7/lycoris/utils/
+-rw-rw-rw-   0        0        0    24042 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev7/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-03-13 17:06:13.000000 lycoris_lora-3.0.0.dev7/lycoris/utils/bnb.py
+-rw-rw-rw-   0        0        0      102 2024-05-25 08:12:37.000000 lycoris_lora-3.0.0.dev7/lycoris/utils/general.py
+-rw-rw-rw-   0        0        0     1078 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev7/lycoris/utils/logger.py
+-rw-rw-rw-   0        0        0      190 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev7/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      251 2023-12-02 03:39:50.000000 lycoris_lora-3.0.0.dev7/lycoris/utils/xformers_utils.py
+-rw-rw-rw-   0        0        0    18777 2024-05-30 08:28:44.000000 lycoris_lora-3.0.0.dev7/lycoris/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:34:31.355702 lycoris_lora-3.0.0.dev7/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      465 2024-06-01 11:34:31.000000 lycoris_lora-3.0.0.dev7/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      904 2024-06-01 11:34:31.000000 lycoris_lora-3.0.0.dev7/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 11:34:31.000000 lycoris_lora-3.0.0.dev7/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-06 13:42:23.000000 lycoris_lora-3.0.0.dev7/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2024-06-01 11:34:31.000000 lycoris_lora-3.0.0.dev7/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 11:34:31.000000 lycoris_lora-3.0.0.dev7/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 11:34:31.356703 lycoris_lora-3.0.0.dev7/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-06-01 11:34:14.000000 lycoris_lora-3.0.0.dev7/setup.py
```

### Comparing `lycoris_lora-3.0.0.dev6/LICENSE.md` & `lycoris_lora-3.0.0.dev7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/README.md` & `lycoris_lora-3.0.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/__init__.py` & `lycoris_lora-3.0.0.dev7/lycoris/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/config.py` & `lycoris_lora-3.0.0.dev7/lycoris/config.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/functional/general.py` & `lycoris_lora-3.0.0.dev7/lycoris/functional/general.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/functional/locon.py` & `lycoris_lora-3.0.0.dev7/lycoris/functional/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/functional/loha.py` & `lycoris_lora-3.0.0.dev7/lycoris/functional/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/kohya.py` & `lycoris_lora-3.0.0.dev7/lycoris/kohya.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,15 +608,15 @@
         if os.path.splitext(file)[1] == ".safetensors":
             from safetensors.torch import save_file
 
             # Precalculate model hashes to save time on indexing
             if metadata is None:
                 metadata = {}
             model_hash, legacy_hash = precalculate_safetensors_hashes(
-                state_dict, metadata
+                state_dict
             )
             metadata["sshs_model_hash"] = model_hash
             metadata["sshs_legacy_hash"] = legacy_hash
 
             save_file(state_dict, file, metadata)
         else:
             torch.save(state_dict, file)
@@ -842,15 +842,15 @@
         if os.path.splitext(file)[1] == ".safetensors":
             from safetensors.torch import save_file
 
             # Precalculate model hashes to save time on indexing
             if metadata is None:
                 metadata = {}
             model_hash, legacy_hash = precalculate_safetensors_hashes(
-                state_dict, metadata
+                state_dict
             )
             metadata["sshs_model_hash"] = model_hash
             metadata["sshs_legacy_hash"] = legacy_hash
 
             save_file(state_dict, file, metadata)
         else:
             torch.save(state_dict, file)
```

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/logging.py` & `lycoris_lora-3.0.0.dev7/lycoris/logging.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/__init__.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/base.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/base.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/boft.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/boft.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/diag_oft.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/diag_oft.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/dylora.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/full.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/full.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/glora.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/ia3.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/locon.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/loha.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/lokr.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/modules/norms.py` & `lycoris_lora-3.0.0.dev7/lycoris/modules/norms.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/utils/__init__.py` & `lycoris_lora-3.0.0.dev7/lycoris/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/utils/logger.py` & `lycoris_lora-3.0.0.dev7/lycoris/utils/logger.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris/wrapper.py` & `lycoris_lora-3.0.0.dev7/lycoris/wrapper.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-3.0.0.dev7/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-3.0.0.dev6/setup.py` & `lycoris_lora-3.0.0.dev7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="lycoris_lora",
     packages=find_packages(),
-    version="3.0.0.dev6",
+    version="3.0.0.dev7",
     url="https://github.com/KohakuBlueleaf/LyCORIS",
     description="Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion",
     author="Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao",
     author_email="apolloyeh0123@gmail.com",
     zip_safe=False,
     install_requires=["torch", "einops", "toml", "tqdm"],
     python_requires=">=3.10",
```


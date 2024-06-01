# Comparing `tmp/nonebot_plugin_nsfw-0.8.tar.gz` & `tmp/nonebot_plugin_nsfw-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nsfw-0.8.tar", last modified: Sun Dec  3 07:52:15 2023, max compression
+gzip compressed data, was "nonebot_plugin_nsfw-0.9.tar", last modified: Wed Dec  6 09:36:30 2023, max compression
```

## Comparing `nonebot_plugin_nsfw-0.8.tar` & `nonebot_plugin_nsfw-0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-11-30 13:04:06.338564 nonebot_plugin_nsfw-0.8/LICENSE
--rw-r--r--   0        0        0     5094 2023-12-03 07:05:53.796852 nonebot_plugin_nsfw-0.8/README.md
--rw-r--r--   0        0        0     1767 2023-12-03 07:52:01.116796 nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/__init__.py
--rw-r--r--   0        0        0     1460 2023-12-03 07:27:37.706825 nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/config.py
--rw-r--r--   0        0        0     2238 2023-12-03 05:14:59.936993 nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/deps.py
--rw-r--r--   0        0        0     3586 2023-12-03 07:29:24.846822 nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/loader.py
--rw-r--r--   0        0        0     4273 2023-12-02 16:20:52.832945 nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/vendor_nsfw_model.py
--rw-r--r--   0        0        0      790 2023-12-03 07:52:15.946797 nonebot_plugin_nsfw-0.8/pyproject.toml
--rw-r--r--   0        0        0     5860 1970-01-01 00:00:00.000000 nonebot_plugin_nsfw-0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-30 13:04:06.338564 nonebot_plugin_nsfw-0.9/LICENSE
+-rw-r--r--   0        0        0     5312 2023-12-03 08:18:48.186769 nonebot_plugin_nsfw-0.9/README.md
+-rw-r--r--   0        0        0     1780 2023-12-06 09:35:38.797948 nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/__init__.py
+-rw-r--r--   0        0        0     1460 2023-12-06 09:35:51.137945 nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/config.py
+-rw-r--r--   0        0        0     2238 2023-12-03 05:14:59.936993 nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/deps.py
+-rw-r--r--   0        0        0     3586 2023-12-03 07:29:24.846822 nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/loader.py
+-rw-r--r--   0        0        0     4273 2023-12-02 16:20:52.832945 nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/vendor_nsfw_model.py
+-rw-r--r--   0        0        0      790 2023-12-06 09:36:30.637933 nonebot_plugin_nsfw-0.9/pyproject.toml
+-rw-r--r--   0        0        0     6078 1970-01-01 00:00:00.000000 nonebot_plugin_nsfw-0.9/PKG-INFO
```

### Comparing `nonebot_plugin_nsfw-0.8/LICENSE` & `nonebot_plugin_nsfw-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nsfw-0.8/README.md` & `nonebot_plugin_nsfw-0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,17 @@
+<p align="center">
+  <img src="logo/logo.png" width="200" height="200" alt="nonebot-plugin-nsfw">
+</p>
+
+<div align="center">
+
 # NoneBot Plugin NSFW
 
+</div>
+
 此插件是一个集成于 NoneBot 的、基于深度神经网络的 **群聊 NSFW 图片检测插件**，带有 **撤回、警告、禁言** 等功能。可选择使用 [Safety Checker](https://github.com/iyume/safety-checker)、[NSFW Model](https://github.com/GantMan/nsfw_model) 模型。
 
 **注意：** 目前插件仅在 matcha 完成测试，只能保证 OneBot V11 兼容。
 
 ## Safety Checker 对比 NSFW Model
 
 |                              | Safety Checker      | NSFW Model（默认） |
@@ -50,15 +58,15 @@
 pip install nonebot-plugin-nsfw[safety-checker]
 ```
 
 此过程会自动下载 torch GPU 版本，大约 2GB。
 
 > 如果你需要仅 CPU 的 torch，需要提前使用这条命令安装 torch：`pip install torch --index-url https://download.pytorch.org/whl/cpu`
 
-第一次加载插件时会从 huggingface 下载一个 600 MB 的模型文件，请确保网络连接通畅。
+第一次加载插件时会从 huggingface 下载一个 600 MB 的模型文件，请确保网络连接通畅。（模型缓存由 huggingface_lab 管理，位置在 `~/.cache/huggingface/hub`）
 
 载入 Safety Checker 需要 **至少 1.2 GB** 内存/显存。
 CPU (Ryzen 7 7840H) 每次调用大约耗时 0.5s，图像大小不影响调用耗时。
 
 ## 使用 NSFW Model（默认）
 
 NSFW Model 是基于 Inception V3 和 MobileNet V2 的传统视觉模型。
@@ -84,14 +92,14 @@
 
 |                          | 默认值                            | 可选值                         | 说明                                               |
 | ------------------------ | --------------------------------- | ------------------------------ | -------------------------------------------------- |
 | nsfw\_\_model            | "safety-checker"                  | "safety-checker", "nsfw-model" |                                                    |
 | nsfw\_\_device           | "cpu"                             | "cpu", "cuda", etc.            |                                                    |
 | nsfw\_\_withdraw         | True                              | True, False                    | 撤回检测到 NSFW 图片的消息                         |
 | nsfw\_\_nsfw_model_path  | cwd() / nsfw_mobilenet2_v1.2.0.h5 | .h5 or SavedModel path         | nsfw-model 模型路径，没配置则自动下载              |
-| nsfw\_\_warning_capacity | 3                                 | 正整数                         | 一天内警告 N 次后禁言，0 不警告，ban=True 直接禁言 |
+| nsfw\_\_warning_capacity | 3                                 | 非负整数                       | 一天内警告 N 次后禁言，0 不警告，ban=True 直接禁言 |
 | nsfw\_\_ban              | True                              | True, False                    | 是否启用禁言                                       |
 | nsfw\_\_ban_time         | 1800                              | 正整数                         | 禁言时长，单位为秒数                               |
 
 更多配置正在开发中...
 
 欢迎 issue 提出问题和想法。
```

### Comparing `nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/__init__.py` & `nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     try:
         get_run_model()
     except ValueError:
         return False
     return True
 
 
-nsfw_matcher = on_message(rule=check_model_available)
+nsfw_matcher = on_message(rule=check_model_available, block=False)
 
 
 @nsfw_matcher.handle()
 async def _(
     bot: Bot,
     event: GroupMessageEvent,
     has_nsfw: bool = Depends(detect_nsfw),
```

### Comparing `nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/config.py` & `nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Literal, Optional
 
 import nonebot
 from nonebot import logger
 from pydantic import BaseModel, NonNegativeInt, PositiveInt
 
 DEFAULT_NSFW_MODEL_PATH = str(Path.cwd() / "nsfw_mobilenet2_v1.2.0.h5")
-DEFAULT_NSFW_MODEL_URI = "https://github.com/iyume/nonebot-plugin-nsfw/releases/download/v0.1/nsfw_mobilenet2_v1.2.0.h5"
+DEFAULT_NSFW_MODEL_URI = "https://github.com/iyume/nonebot-plugin-nsfw/releases/download/v0.0/nsfw_mobilenet2_v1.2.0.h5"
 
 T_AVAILABLE_MODEL = Literal["safety-checker", "nsfw-model"]
 
 
 class PluginScopedConfig(BaseModel):
     model: T_AVAILABLE_MODEL = "nsfw-model"
     """要使用的模型。默认为 NSFW Model。"""
```

### Comparing `nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/deps.py` & `nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/deps.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/loader.py` & `nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/loader.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nsfw-0.8/nonebot_plugin_nsfw/vendor_nsfw_model.py` & `nonebot_plugin_nsfw-0.9/nonebot_plugin_nsfw/vendor_nsfw_model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nsfw-0.8/pyproject.toml` & `nonebot_plugin_nsfw-0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-nsfw"
-version = "0.8"
+version = "0.9"
 description = "群聊 NSFW 图片检测插件，带有撤回、警告、禁言等功能。使用 Safety Checker / NSFW Model。"
 authors = [
     { name = "iyume", email = "iyumelive@gmail.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = [
```

### Comparing `nonebot_plugin_nsfw-0.8/PKG-INFO` & `nonebot_plugin_nsfw-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nsfw
-Version: 0.8
+Version: 0.9
 Summary: 群聊 NSFW 图片检测插件，带有撤回、警告、禁言等功能。使用 Safety Checker / NSFW Model。
 Author-Email: iyume <iyumelive@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.0
 Requires-Dist: nonebot-adapter-onebot>=2.0
 Requires-Dist: Pillow>=8.4.0
@@ -14,16 +14,24 @@
 Requires-Dist: tensorflow>=2.2.0; extra == "nsfw-model"
 Requires-Dist: tensorflow-hub>=0.12; extra == "nsfw-model"
 Requires-Dist: numpy; extra == "nsfw-model"
 Provides-Extra: safety-checker
 Provides-Extra: nsfw-model
 Description-Content-Type: text/markdown
 
+<p align="center">
+  <img src="logo/logo.png" width="200" height="200" alt="nonebot-plugin-nsfw">
+</p>
+
+<div align="center">
+
 # NoneBot Plugin NSFW
 
+</div>
+
 此插件是一个集成于 NoneBot 的、基于深度神经网络的 **群聊 NSFW 图片检测插件**，带有 **撤回、警告、禁言** 等功能。可选择使用 [Safety Checker](https://github.com/iyume/safety-checker)、[NSFW Model](https://github.com/GantMan/nsfw_model) 模型。
 
 **注意：** 目前插件仅在 matcha 完成测试，只能保证 OneBot V11 兼容。
 
 ## Safety Checker 对比 NSFW Model
 
 |                              | Safety Checker      | NSFW Model（默认） |
@@ -70,15 +78,15 @@
 pip install nonebot-plugin-nsfw[safety-checker]
 ```
 
 此过程会自动下载 torch GPU 版本，大约 2GB。
 
 > 如果你需要仅 CPU 的 torch，需要提前使用这条命令安装 torch：`pip install torch --index-url https://download.pytorch.org/whl/cpu`
 
-第一次加载插件时会从 huggingface 下载一个 600 MB 的模型文件，请确保网络连接通畅。
+第一次加载插件时会从 huggingface 下载一个 600 MB 的模型文件，请确保网络连接通畅。（模型缓存由 huggingface_lab 管理，位置在 `~/.cache/huggingface/hub`）
 
 载入 Safety Checker 需要 **至少 1.2 GB** 内存/显存。
 CPU (Ryzen 7 7840H) 每次调用大约耗时 0.5s，图像大小不影响调用耗时。
 
 ## 使用 NSFW Model（默认）
 
 NSFW Model 是基于 Inception V3 和 MobileNet V2 的传统视觉模型。
@@ -104,14 +112,14 @@
 
 |                          | 默认值                            | 可选值                         | 说明                                               |
 | ------------------------ | --------------------------------- | ------------------------------ | -------------------------------------------------- |
 | nsfw\_\_model            | "safety-checker"                  | "safety-checker", "nsfw-model" |                                                    |
 | nsfw\_\_device           | "cpu"                             | "cpu", "cuda", etc.            |                                                    |
 | nsfw\_\_withdraw         | True                              | True, False                    | 撤回检测到 NSFW 图片的消息                         |
 | nsfw\_\_nsfw_model_path  | cwd() / nsfw_mobilenet2_v1.2.0.h5 | .h5 or SavedModel path         | nsfw-model 模型路径，没配置则自动下载              |
-| nsfw\_\_warning_capacity | 3                                 | 正整数                         | 一天内警告 N 次后禁言，0 不警告，ban=True 直接禁言 |
+| nsfw\_\_warning_capacity | 3                                 | 非负整数                       | 一天内警告 N 次后禁言，0 不警告，ban=True 直接禁言 |
 | nsfw\_\_ban              | True                              | True, False                    | 是否启用禁言                                       |
 | nsfw\_\_ban_time         | 1800                              | 正整数                         | 禁言时长，单位为秒数                               |
 
 更多配置正在开发中...
 
 欢迎 issue 提出问题和想法。
```


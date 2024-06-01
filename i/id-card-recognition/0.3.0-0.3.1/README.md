# Comparing `tmp/id_card_recognition-0.3.0.tar.gz` & `tmp/id_card_recognition-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_card_recognition-0.3.0.tar", last modified: Sat Jun  1 13:20:05 2024, max compression
+gzip compressed data, was "id_card_recognition-0.3.1.tar", last modified: Sat Jun  1 13:22:08 2024, max compression
```

## Comparing `id_card_recognition-0.3.0.tar` & `id_card_recognition-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:20:05.509343 id_card_recognition-0.3.0/
--rw-r--r--   0 wangligang   (501) staff       (20)     2061 2024-06-01 13:20:05.508803 id_card_recognition-0.3.0/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)     1543 2024-06-01 13:20:01.000000 id_card_recognition-0.3.0/README.md
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:20:05.505629 id_card_recognition-0.3.0/id_card_recognition/
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.3.0/id_card_recognition/__init__.py
--rw-r--r--   0 wangligang   (501) staff       (20)     5347 2024-06-01 12:52:04.000000 id_card_recognition-0.3.0/id_card_recognition/recognition.py
--rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.3.0/id_card_recognition/utils.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:20:05.508314 id_card_recognition-0.3.0/id_card_recognition.egg-info/
--rw-r--r--   0 wangligang   (501) staff       (20)     2061 2024-06-01 13:20:05.000000 id_card_recognition-0.3.0/id_card_recognition.egg-info/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 13:20:05.000000 id_card_recognition-0.3.0/id_card_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 13:20:05.000000 id_card_recognition-0.3.0/id_card_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 13:20:05.000000 id_card_recognition-0.3.0/id_card_recognition.egg-info/entry_points.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:20:05.000000 id_card_recognition-0.3.0/id_card_recognition.egg-info/requires.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 13:20:05.000000 id_card_recognition-0.3.0/id_card_recognition.egg-info/top_level.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:20:05.509487 id_card_recognition-0.3.0/setup.cfg
--rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 13:20:01.000000 id_card_recognition-0.3.0/setup.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:20:05.507922 id_card_recognition-0.3.0/tests/
--rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.3.0/tests/test_recognition.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:22:08.715147 id_card_recognition-0.3.1/
+-rw-r--r--   0 wangligang   (501) staff       (20)     2062 2024-06-01 13:22:08.714605 id_card_recognition-0.3.1/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)     1544 2024-06-01 13:22:06.000000 id_card_recognition-0.3.1/README.md
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:22:08.710066 id_card_recognition-0.3.1/id_card_recognition/
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.3.1/id_card_recognition/__init__.py
+-rw-r--r--   0 wangligang   (501) staff       (20)     5353 2024-06-01 13:22:06.000000 id_card_recognition-0.3.1/id_card_recognition/recognition.py
+-rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.3.1/id_card_recognition/utils.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:22:08.713952 id_card_recognition-0.3.1/id_card_recognition.egg-info/
+-rw-r--r--   0 wangligang   (501) staff       (20)     2062 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/entry_points.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/requires.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 13:22:08.000000 id_card_recognition-0.3.1/id_card_recognition.egg-info/top_level.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 13:22:08.715244 id_card_recognition-0.3.1/setup.cfg
+-rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 13:22:06.000000 id_card_recognition-0.3.1/setup.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 13:22:08.713297 id_card_recognition-0.3.1/tests/
+-rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.3.1/tests/test_recognition.py
```

### Comparing `id_card_recognition-0.3.0/PKG-INFO` & `id_card_recognition-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 ## 配置
 
 ### 创建 .env 文件
 
 在项目根目录下创建一个 `.env` 文件，并添加以下内容：
 
 ```env
-API_KEY= 你的moonshot AI 秘钥
+API_KEY= 你的 moonshot AI 秘钥
 IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images
 RESULT_FILE_NAME= 识别结果文件名称，默认为 result.txt
 CHOSEN_MODEL_NAME= 选择的模型名称，默认为 "moonshot-v1-8k"
 ```
 
 ### 示例 .env 文件
```

### Comparing `id_card_recognition-0.3.0/README.md` & `id_card_recognition-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## 配置
 
 ### 创建 .env 文件
 
 在项目根目录下创建一个 `.env` 文件，并添加以下内容：
 
 ```env
-API_KEY= 你的moonshot AI 秘钥
+API_KEY= 你的 moonshot AI 秘钥
 IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images
 RESULT_FILE_NAME= 识别结果文件名称，默认为 result.txt
 CHOSEN_MODEL_NAME= 选择的模型名称，默认为 "moonshot-v1-8k"
 ```
 
 ### 示例 .env 文件
```

### Comparing `id_card_recognition-0.3.0/id_card_recognition/recognition.py` & `id_card_recognition-0.3.1/id_card_recognition/recognition.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     total_tokens = 0
     results = []
 
     for image_file in image_files:
         try:
             start_time = time.time()
 
-            print(f"开始识别文件{image_file}......")
+            print(f"开始识别文件 {image_file} ......")
 
             file_object = client.files.create(file=image_file, purpose="file-extract")
             file_content = client.files.content(file_id=file_object.id).text
 
             result, tokens_used = process_id_card(image_file, file_content, chosen_model)
 
             if not result:
@@ -140,15 +140,15 @@
             total_tokens += tokens_used
 
             result["recognition_time"] = f"{recognition_time:.2f} 秒"
             result["cost"] = f"¥{cost_per_image:.6f}"
             result["tokens_used"] = tokens_used
 
             results.append(result)
-            print(f"文件{image_file}识别完成，耗时{recognition_time:.2f}秒。")
+            print(f"文件 {image_file} 识别完成，耗时 {recognition_time:.2f} 秒。")
 
         except Exception as e:
             error_result = {
                 "file": str(image_file),
                 "result": f"处理文件时出错: {e}"
             }
             results.append(error_result)
```

### Comparing `id_card_recognition-0.3.0/id_card_recognition/utils.py` & `id_card_recognition-0.3.1/id_card_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.3.0/id_card_recognition.egg-info/PKG-INFO` & `id_card_recognition-0.3.1/id_card_recognition.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 ## 配置
 
 ### 创建 .env 文件
 
 在项目根目录下创建一个 `.env` 文件，并添加以下内容：
 
 ```env
-API_KEY= 你的moonshot AI 秘钥
+API_KEY= 你的 moonshot AI 秘钥
 IMAGE_DIRECTORY= 需要识别的身份证照片存放路径，默认为 ./images
 RESULT_FILE_NAME= 识别结果文件名称，默认为 result.txt
 CHOSEN_MODEL_NAME= 选择的模型名称，默认为 "moonshot-v1-8k"
 ```
 
 ### 示例 .env 文件
```

### Comparing `id_card_recognition-0.3.0/setup.py` & `id_card_recognition-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='id_card_recognition',
-    version='0.3.0',
+    version='0.3.1',
     packages=find_packages(),
     install_requires=[
         'requests',
         'natsort',
         'openai',
         'python-dotenv',
     ],
```


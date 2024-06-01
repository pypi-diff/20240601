# Comparing `tmp/id_card_recognition-0.2.0.tar.gz` & `tmp/id_card_recognition-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_card_recognition-0.2.0.tar", last modified: Sat Jun  1 12:37:16 2024, max compression
+gzip compressed data, was "id_card_recognition-0.2.1.tar", last modified: Sat Jun  1 12:43:18 2024, max compression
```

## Comparing `id_card_recognition-0.2.0.tar` & `id_card_recognition-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:37:16.162663 id_card_recognition-0.2.0/
--rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:37:16.162153 id_card_recognition-0.2.0/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:18.000000 id_card_recognition-0.2.0/README.md
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:37:16.158551 id_card_recognition-0.2.0/id_card_recognition/
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.2.0/id_card_recognition/__init__.py
--rw-r--r--   0 wangligang   (501) staff       (20)     5391 2024-06-01 12:37:10.000000 id_card_recognition-0.2.0/id_card_recognition/recognition.py
--rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.2.0/id_card_recognition/utils.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:37:16.161709 id_card_recognition-0.2.0/id_card_recognition.egg-info/
--rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/entry_points.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/requires.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/top_level.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:37:16.162941 id_card_recognition-0.2.0/setup.cfg
--rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 12:37:10.000000 id_card_recognition-0.2.0/setup.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:37:16.161147 id_card_recognition-0.2.0/tests/
--rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.2.0/tests/test_recognition.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:43:18.272545 id_card_recognition-0.2.1/
+-rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:43:18.271963 id_card_recognition-0.2.1/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:18.000000 id_card_recognition-0.2.1/README.md
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:43:18.267429 id_card_recognition-0.2.1/id_card_recognition/
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.2.1/id_card_recognition/__init__.py
+-rw-r--r--   0 wangligang   (501) staff       (20)     5347 2024-06-01 12:43:13.000000 id_card_recognition-0.2.1/id_card_recognition/recognition.py
+-rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.2.1/id_card_recognition/utils.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:43:18.271252 id_card_recognition-0.2.1/id_card_recognition.egg-info/
+-rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/entry_points.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/requires.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/top_level.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:43:18.272637 id_card_recognition-0.2.1/setup.cfg
+-rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 12:43:13.000000 id_card_recognition-0.2.1/setup.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:43:18.270762 id_card_recognition-0.2.1/tests/
+-rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.2.1/tests/test_recognition.py
```

### Comparing `id_card_recognition-0.2.0/PKG-INFO` & `id_card_recognition-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.2.0/id_card_recognition/recognition.py` & `id_card_recognition-0.2.1/id_card_recognition/recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # 加载环境变量
 load_dotenv()
 
 # 从环境变量中获取API密钥
 api_key = os.getenv("API_KEY")
 
 # 指定使用的模型
-chosen_model = os.getenv('CHOSEN_MODEL_NAME', 'moonshot-v1-8k')
+chosen_model = os.getenv("CHOSEN_MODEL_NAME")
 
 # 指定图像目录
-image_directory = os.getenv('IMAGE_DIRECTORY', 'images/')  # 替换为实际的目录名
-result_file_name = os.getenv('RESULT_FILE_NAME', 'results.txt')
+image_directory = os.getenv("IMAGE_DIRECTORY")  # 替换为实际的目录名
+result_file_name = os.getenv("RESULT_FILE_NAME")
 
 # 初始化OpenAI客户端
 client = OpenAI(
     api_key=api_key,
     base_url="https://api.moonshot.cn/v1",
 )
```

### Comparing `id_card_recognition-0.2.0/id_card_recognition/utils.py` & `id_card_recognition-0.2.1/id_card_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.2.0/id_card_recognition.egg-info/PKG-INFO` & `id_card_recognition-0.2.1/id_card_recognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.2.0/setup.py` & `id_card_recognition-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='id_card_recognition',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         'requests',
         'natsort',
         'openai',
         'python-dotenv',
     ],
```


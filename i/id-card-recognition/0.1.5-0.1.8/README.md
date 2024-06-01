# Comparing `tmp/id_card_recognition-0.1.5.tar.gz` & `tmp/id_card_recognition-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_card_recognition-0.1.5.tar", last modified: Sat Jun  1 12:13:16 2024, max compression
+gzip compressed data, was "id_card_recognition-0.1.8.tar", last modified: Sat Jun  1 12:26:57 2024, max compression
```

## Comparing `id_card_recognition-0.1.5.tar` & `id_card_recognition-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:13:16.839811 id_card_recognition-0.1.5/
--rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:13:16.839129 id_card_recognition-0.1.5/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:18.000000 id_card_recognition-0.1.5/README.md
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:13:16.834929 id_card_recognition-0.1.5/id_card_recognition/
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.1.5/id_card_recognition/__init__.py
--rw-r--r--   0 wangligang   (501) staff       (20)     5094 2024-06-01 10:42:43.000000 id_card_recognition-0.1.5/id_card_recognition/recognition.py
--rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.1.5/id_card_recognition/utils.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:13:16.838366 id_card_recognition-0.1.5/id_card_recognition.egg-info/
--rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:13:16.000000 id_card_recognition-0.1.5/id_card_recognition.egg-info/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 12:13:16.000000 id_card_recognition-0.1.5/id_card_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 12:13:16.000000 id_card_recognition-0.1.5/id_card_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 12:13:16.000000 id_card_recognition-0.1.5/id_card_recognition.egg-info/entry_points.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:13:16.000000 id_card_recognition-0.1.5/id_card_recognition.egg-info/requires.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 12:13:16.000000 id_card_recognition-0.1.5/id_card_recognition.egg-info/top_level.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:13:16.840028 id_card_recognition-0.1.5/setup.cfg
--rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 11:43:56.000000 id_card_recognition-0.1.5/setup.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:13:16.837680 id_card_recognition-0.1.5/tests/
--rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.1.5/tests/test_recognition.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:26:57.499257 id_card_recognition-0.1.8/
+-rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:26:57.498649 id_card_recognition-0.1.8/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:18.000000 id_card_recognition-0.1.8/README.md
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:26:57.494551 id_card_recognition-0.1.8/id_card_recognition/
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.1.8/id_card_recognition/__init__.py
+-rw-r--r--   0 wangligang   (501) staff       (20)     5117 2024-06-01 12:23:48.000000 id_card_recognition-0.1.8/id_card_recognition/recognition.py
+-rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.1.8/id_card_recognition/utils.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:26:57.497807 id_card_recognition-0.1.8/id_card_recognition.egg-info/
+-rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/entry_points.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/requires.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/top_level.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:26:57.499386 id_card_recognition-0.1.8/setup.cfg
+-rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 12:26:53.000000 id_card_recognition-0.1.8/setup.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:26:57.497174 id_card_recognition-0.1.8/tests/
+-rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.1.8/tests/test_recognition.py
```

### Comparing `id_card_recognition-0.1.5/PKG-INFO` & `id_card_recognition-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.1.5
+Version: 0.1.8
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.1.5/id_card_recognition/recognition.py` & `id_card_recognition-0.1.8/id_card_recognition/recognition.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 加载环境变量
 load_dotenv()
 
 # 从环境变量中获取API密钥
 api_key = os.getenv("API_KEY")
 
 # 指定使用的模型
-chosen_model = "moonshot-v1-8k"
+chosen_model = os.getenv('CHOSEN_MODEL_NAME', 'moonshot-v1-8k')
 
 # 指定图像目录
 image_directory = os.getenv('IMAGE_DIRECTORY', 'images/')  # 替换为实际的目录名
 
 # 初始化OpenAI客户端
 client = OpenAI(
     api_key=api_key,
@@ -97,24 +97,22 @@
 
 def delete_all_files():
     file_list = client.files.list()
     for file in file_list.data:
         client.files.delete(file_id=file.id)
 
 
-def main():
+def do_recognition():
     model_prices = {
         "moonshot-v1-8k": 12.0,
         "moonshot-v1-32k": 24.0,
         "moonshot-v1-128k": 60.0
     }
     model_price_per_million_tokens = model_prices[chosen_model]
 
-    initial_balance_info = get_balance(api_key)
-
     image_files = natsorted([Path(image_directory) / file_name for file_name in os.listdir(image_directory) if
                              file_name.lower().endswith(('.png', '.jpg', '.jpeg', '.bmp', '.gif'))])
 
     total_start_time = time.time()
     total_cost = 0.0
     total_tokens = 0
     results = []
@@ -159,11 +157,13 @@
 
     final_balance_info = get_balance(api_key)
     results.append({"balance_info": final_balance_info})
 
     with open('results.txt', 'w', encoding='utf-8') as result_file:
         json.dump(results, result_file, ensure_ascii=False, indent=4)
 
+    return results
+
 
 if __name__ == "__main__":
     delete_all_files()
-    main()
+    do_recognition()
```

### Comparing `id_card_recognition-0.1.5/id_card_recognition/utils.py` & `id_card_recognition-0.1.8/id_card_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.1.5/id_card_recognition.egg-info/PKG-INFO` & `id_card_recognition-0.1.8/id_card_recognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.1.5
+Version: 0.1.8
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.1.5/setup.py` & `id_card_recognition-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='id_card_recognition',
-    version='0.1.5',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=[
         'requests',
         'natsort',
         'openai',
         'python-dotenv',
     ],
```


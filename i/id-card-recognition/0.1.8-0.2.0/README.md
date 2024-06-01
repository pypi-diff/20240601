# Comparing `tmp/id_card_recognition-0.1.8.tar.gz` & `tmp/id_card_recognition-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_card_recognition-0.1.8.tar", last modified: Sat Jun  1 12:26:57 2024, max compression
+gzip compressed data, was "id_card_recognition-0.2.0.tar", last modified: Sat Jun  1 12:37:16 2024, max compression
```

## Comparing `id_card_recognition-0.1.8.tar` & `id_card_recognition-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:26:57.499257 id_card_recognition-0.1.8/
--rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:26:57.498649 id_card_recognition-0.1.8/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:18.000000 id_card_recognition-0.1.8/README.md
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:26:57.494551 id_card_recognition-0.1.8/id_card_recognition/
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.1.8/id_card_recognition/__init__.py
--rw-r--r--   0 wangligang   (501) staff       (20)     5117 2024-06-01 12:23:48.000000 id_card_recognition-0.1.8/id_card_recognition/recognition.py
--rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.1.8/id_card_recognition/utils.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:26:57.497807 id_card_recognition-0.1.8/id_card_recognition.egg-info/
--rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/entry_points.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/requires.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 12:26:57.000000 id_card_recognition-0.1.8/id_card_recognition.egg-info/top_level.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:26:57.499386 id_card_recognition-0.1.8/setup.cfg
--rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 12:26:53.000000 id_card_recognition-0.1.8/setup.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:26:57.497174 id_card_recognition-0.1.8/tests/
--rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.1.8/tests/test_recognition.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:37:16.162663 id_card_recognition-0.2.0/
+-rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:37:16.162153 id_card_recognition-0.2.0/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:18.000000 id_card_recognition-0.2.0/README.md
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:37:16.158551 id_card_recognition-0.2.0/id_card_recognition/
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.2.0/id_card_recognition/__init__.py
+-rw-r--r--   0 wangligang   (501) staff       (20)     5391 2024-06-01 12:37:10.000000 id_card_recognition-0.2.0/id_card_recognition/recognition.py
+-rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.2.0/id_card_recognition/utils.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:37:16.161709 id_card_recognition-0.2.0/id_card_recognition.egg-info/
+-rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/entry_points.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/requires.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 12:37:16.000000 id_card_recognition-0.2.0/id_card_recognition.egg-info/top_level.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:37:16.162941 id_card_recognition-0.2.0/setup.cfg
+-rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 12:37:10.000000 id_card_recognition-0.2.0/setup.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:37:16.161147 id_card_recognition-0.2.0/tests/
+-rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.2.0/tests/test_recognition.py
```

### Comparing `id_card_recognition-0.1.8/PKG-INFO` & `id_card_recognition-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.1.8
+Version: 0.2.0
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.1.8/id_card_recognition/recognition.py` & `id_card_recognition-0.2.0/id_card_recognition/recognition.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 api_key = os.getenv("API_KEY")
 
 # 指定使用的模型
 chosen_model = os.getenv('CHOSEN_MODEL_NAME', 'moonshot-v1-8k')
 
 # 指定图像目录
 image_directory = os.getenv('IMAGE_DIRECTORY', 'images/')  # 替换为实际的目录名
+result_file_name = os.getenv('RESULT_FILE_NAME', 'results.txt')
 
 # 初始化OpenAI客户端
 client = OpenAI(
     api_key=api_key,
     base_url="https://api.moonshot.cn/v1",
 )
 
@@ -117,14 +118,16 @@
     total_tokens = 0
     results = []
 
     for image_file in image_files:
         try:
             start_time = time.time()
 
+            print(f"开始识别文件{image_file}......")
+
             file_object = client.files.create(file=image_file, purpose="file-extract")
             file_content = client.files.content(file_id=file_object.id).text
 
             result, tokens_used = process_id_card(image_file, file_content, chosen_model)
 
             if not result:
                 continue
@@ -137,32 +140,34 @@
             total_tokens += tokens_used
 
             result["recognition_time"] = f"{recognition_time:.2f} 秒"
             result["cost"] = f"¥{cost_per_image:.6f}"
             result["tokens_used"] = tokens_used
 
             results.append(result)
+            print(f"文件{image_file}识别完成，耗时{recognition_time:.2f}秒。")
 
         except Exception as e:
             error_result = {
                 "file": str(image_file),
                 "result": f"处理文件时出错: {e}"
             }
             results.append(error_result)
             continue
 
     total_end_time = time.time()
-    total_time_message = f"总处理时间: {total_end_time - total_start_time:.2f} 秒"
+    total_time_message = f"文件全部处理完成，总处理时间: {total_end_time - total_start_time:.2f} 秒"
+    print(total_time_message)
 
     results.append({"total_time": total_time_message, "total_cost": f"¥{total_cost:.6f}", "total_tokens": total_tokens})
 
     final_balance_info = get_balance(api_key)
     results.append({"balance_info": final_balance_info})
 
-    with open('results.txt', 'w', encoding='utf-8') as result_file:
+    with open(result_file_name, 'w', encoding='utf-8') as result_file:
         json.dump(results, result_file, ensure_ascii=False, indent=4)
 
     return results
 
 
 if __name__ == "__main__":
     delete_all_files()
```

### Comparing `id_card_recognition-0.1.8/id_card_recognition/utils.py` & `id_card_recognition-0.2.0/id_card_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.1.8/id_card_recognition.egg-info/PKG-INFO` & `id_card_recognition-0.2.0/id_card_recognition.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.1.8
+Version: 0.2.0
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.1.8/setup.py` & `id_card_recognition-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='id_card_recognition',
-    version='0.1.8',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         'requests',
         'natsort',
         'openai',
         'python-dotenv',
     ],
```


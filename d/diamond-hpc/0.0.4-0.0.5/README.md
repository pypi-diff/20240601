# Comparing `tmp/diamond-hpc-0.0.4.tar.gz` & `tmp/diamond-hpc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diamond-hpc-0.0.4.tar", last modified: Thu May 30 15:34:51 2024, max compression
+gzip compressed data, was "diamond-hpc-0.0.5.tar", last modified: Sat Jun  1 19:44:56 2024, max compression
```

## Comparing `diamond-hpc-0.0.4.tar` & `diamond-hpc-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.813279 diamond-hpc-0.0.4/
--rw-r--r--   0 haotianxie   (501) staff       (20)     1069 2024-04-04 14:31:34.000000 diamond-hpc-0.0.4/LICENSE
--rw-r--r--   0 haotianxie   (501) staff       (20)     1883 2024-05-30 15:34:51.813073 diamond-hpc-0.0.4/PKG-INFO
--rw-r--r--   0 haotianxie   (501) staff       (20)     1282 2024-05-30 15:34:12.000000 diamond-hpc-0.0.4/README.md
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.808732 diamond-hpc-0.0.4/diamond/
--rw-r--r--   0 haotianxie   (501) staff       (20)        0 2024-05-19 19:23:22.000000 diamond-hpc-0.0.4/diamond/__init__.py
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.808893 diamond-hpc-0.0.4/diamond/container/
--rw-r--r--   0 haotianxie   (501) staff       (20)        0 2024-05-22 16:33:58.000000 diamond-hpc-0.0.4/diamond/container/__init__.py
--rw-r--r--   0 haotianxie   (501) staff       (20)     7107 2024-05-18 17:12:27.000000 diamond-hpc-0.0.4/diamond/container/container.py
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.809408 diamond-hpc-0.0.4/diamond/container/custom_image_builder/
--rw-r--r--   0 haotianxie   (501) staff       (20)       55 2024-04-04 14:31:34.000000 diamond-hpc-0.0.4/diamond/container/custom_image_builder/__init__.py
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.810187 diamond-hpc-0.0.4/diamond/container/custom_image_builder/exception/
--rw-r--r--   0 haotianxie   (501) staff       (20)      142 2024-04-04 14:31:34.000000 diamond-hpc-0.0.4/diamond/container/custom_image_builder/exception/ImageBuilderException.py
--rw-r--r--   0 haotianxie   (501) staff       (20)      143 2024-04-04 14:31:34.000000 diamond-hpc-0.0.4/diamond/container/custom_image_builder/exception/RegisterImageException.py
--rw-r--r--   0 haotianxie   (501) staff       (20)        0 2024-04-04 14:31:34.000000 diamond-hpc-0.0.4/diamond/container/custom_image_builder/exception/__init__.py
--rw-r--r--   0 haotianxie   (501) staff       (20)     7174 2024-05-28 13:34:04.000000 diamond-hpc-0.0.4/diamond/container/custom_image_builder/image_builder.py
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.810418 diamond-hpc-0.0.4/diamond/diamond_client/
--rw-r--r--   0 haotianxie   (501) staff       (20)        0 2024-05-28 13:34:04.000000 diamond-hpc-0.0.4/diamond/diamond_client/__init__.py
--rw-r--r--   0 haotianxie   (501) staff       (20)     2788 2024-05-30 15:08:47.000000 diamond-hpc-0.0.4/diamond/diamond_client/diamond_client.py
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.810543 diamond-hpc-0.0.4/diamond/diamond_client/templates/
--rw-r--r--   0 haotianxie   (501) staff       (20)      772 2024-05-28 13:34:04.000000 diamond-hpc-0.0.4/diamond/diamond_client/templates/task_template
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.812083 diamond-hpc-0.0.4/diamond/wrapper/
--rw-r--r--   0 haotianxie   (501) staff       (20)        0 2024-05-22 16:33:58.000000 diamond-hpc-0.0.4/diamond/wrapper/__init__.py
--rw-r--r--   0 haotianxie   (501) staff       (20)     2210 2024-05-30 15:08:47.000000 diamond-hpc-0.0.4/diamond/wrapper/wrapper.py
-drwxr-xr-x   0 haotianxie   (501) staff       (20)        0 2024-05-30 15:34:51.812861 diamond-hpc-0.0.4/diamond_hpc.egg-info/
--rw-r--r--   0 haotianxie   (501) staff       (20)     1883 2024-05-30 15:34:51.000000 diamond-hpc-0.0.4/diamond_hpc.egg-info/PKG-INFO
--rw-r--r--   0 haotianxie   (501) staff       (20)      814 2024-05-30 15:34:51.000000 diamond-hpc-0.0.4/diamond_hpc.egg-info/SOURCES.txt
--rw-r--r--   0 haotianxie   (501) staff       (20)        1 2024-05-30 15:34:51.000000 diamond-hpc-0.0.4/diamond_hpc.egg-info/dependency_links.txt
--rw-r--r--   0 haotianxie   (501) staff       (20)       60 2024-05-30 15:34:51.000000 diamond-hpc-0.0.4/diamond_hpc.egg-info/entry_points.txt
--rw-r--r--   0 haotianxie   (501) staff       (20)       71 2024-05-30 15:34:51.000000 diamond-hpc-0.0.4/diamond_hpc.egg-info/requires.txt
--rw-r--r--   0 haotianxie   (501) staff       (20)        8 2024-05-30 15:34:51.000000 diamond-hpc-0.0.4/diamond_hpc.egg-info/top_level.txt
--rw-r--r--   0 haotianxie   (501) staff       (20)       38 2024-05-30 15:34:51.813318 diamond-hpc-0.0.4/setup.cfg
--rw-r--r--   0 haotianxie   (501) staff       (20)      971 2024-05-30 15:34:39.000000 diamond-hpc-0.0.4/setup.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1069 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/LICENSE
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1789 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/PKG-INFO
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1282 2024-05-31 19:26:48.000000 diamond-hpc-0.0.5/README.md
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/__init__.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/container/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     7107 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/container.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/container/custom_image_builder/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       55 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/__init__.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/container/custom_image_builder/exception/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      142 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/exception/ImageBuilderException.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      143 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/exception/RegisterImageException.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/exception/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     7174 2024-05-28 00:38:00.000000 diamond-hpc-0.0.5/diamond/container/custom_image_builder/image_builder.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/diamond_client/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-28 00:38:00.000000 diamond-hpc-0.0.5/diamond/diamond_client/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     3010 2024-06-01 19:44:07.000000 diamond-hpc-0.0.5/diamond/diamond_client/diamond_client.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/diamond_client/templates/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      772 2024-05-28 00:38:00.000000 diamond-hpc-0.0.5/diamond/diamond_client/templates/task_template
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond/wrapper/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        0 2024-05-21 23:35:15.000000 diamond-hpc-0.0.5/diamond/wrapper/__init__.py
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     2285 2024-06-01 19:43:36.000000 diamond-hpc-0.0.5/diamond/wrapper/wrapper.py
+drwxr-xr-x   0 hotine    (1000) hotine    (1000)        0 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/diamond_hpc.egg-info/
+-rw-r--r--   0 hotine    (1000) hotine    (1000)     1789 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/PKG-INFO
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      814 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/SOURCES.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        1 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/dependency_links.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       61 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/entry_points.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       71 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/requires.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)        8 2024-06-01 19:44:56.000000 diamond-hpc-0.0.5/diamond_hpc.egg-info/top_level.txt
+-rw-r--r--   0 hotine    (1000) hotine    (1000)       38 2024-06-01 19:44:56.023372 diamond-hpc-0.0.5/setup.cfg
+-rw-r--r--   0 hotine    (1000) hotine    (1000)      971 2024-06-01 19:44:25.000000 diamond-hpc-0.0.5/setup.py
```

### Comparing `diamond-hpc-0.0.4/LICENSE` & `diamond-hpc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.4/PKG-INFO` & `diamond-hpc-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: diamond-hpc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Diamond is a Python package for running tasks on HPC.
 Home-page: https://github.com/Diamond-Proj/Diamond
 Author: Haotian XIE, Gengcong YANG
 Author-email: hotinexie@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click>=8.1.3
-Requires-Dist: globus_compute_sdk>=2.20.0
-Requires-Dist: Jinja2>=3.1.4
-Requires-Dist: Requests>=2.32.2
 
 # Diamond
 
 ### Examples
 
 #### login
 Run
@@ -39,7 +37,9 @@
 
 #### submit task via script file
 1. create an container build endpoint by start endpoint in the globus endpoint server
 2. run the following command(substitude the relevent text with your config)
 ```
 diamond-hpc run-task-from-script --cmd_script /home/hotine/work/Diamond/example/sample_task/openfold_single_node_task --endpoint_id fb1ffeec-aa63-4136-8a49-f3f24608d36f --container_id a20b806c-29a8-44b4-97b6-591434ca9365 --log_path /work/09912/haotianxie/frontera/openfold_demo_single_node.log
 ```
+
+
```

### Comparing `diamond-hpc-0.0.4/README.md` & `diamond-hpc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.4/diamond/container/container.py` & `diamond-hpc-0.0.5/diamond/container/container.py`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.4/diamond/container/custom_image_builder/image_builder.py` & `diamond-hpc-0.0.5/diamond/container/custom_image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.4/diamond/diamond_client/diamond_client.py` & `diamond-hpc-0.0.5/diamond/diamond_client/diamond_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,15 +30,20 @@
 
     def get_oauth2_url(self, auth_client: NativeAppAuthClient):
         query_params = {"prompt": "login"}
         oauth2_url = auth_client.oauth2_get_authorize_url(query_params=query_params)
         return oauth2_url
     
     def oauth2_login_by_token(self, auth_client: NativeAppAuthClient, auth_code: str):
-        auth_client.oauth2_exchange_code_for_tokens(auth_code)
+        return auth_client.oauth2_exchange_code_for_tokens(auth_code)
+
+    def write_auth_token_to_db(self, oauth_token_response: str):
+        login_manager = LoginManager()
+        with login_manager._access_lock:
+            login_manager._token_storage.store(oauth_token_response)
 
     def generate_temp_file(self):
         return tempfile.mktemp()
 
     def generate_task_script(self, cmd: str, log_path: str, endpoint_id: str, container_id: str):
         task_template_filepath = pkg_resources.resource_filename(
             'diamond','diamond_client/templates/task_template')
```

### Comparing `diamond-hpc-0.0.4/diamond/diamond_client/templates/task_template` & `diamond-hpc-0.0.5/diamond/diamond_client/templates/task_template`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.4/diamond/wrapper/wrapper.py` & `diamond-hpc-0.0.5/diamond/wrapper/wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,13 +45,15 @@
 
 
 @cli.command()
 def get_oauth2_url_and_login():
     diamond = DiamondClient()
     auth_client = diamond.get_auth_client()
     click.echo(diamond.get_oauth2_url(auth_client))
-    auth_code = input("Please input the auth code: ")
-    click.echo(diamond.oauth2_login_by_token(auth_client, auth_code))
+    auth_code = input()
+    oauth_token_response = diamond.oauth2_login_by_token(auth_client, auth_code)
+    diamond.write_auth_token_to_db(oauth_token_response)
+    click.echo("Login successfully")
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `diamond-hpc-0.0.4/diamond_hpc.egg-info/PKG-INFO` & `diamond-hpc-0.0.5/diamond_hpc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: diamond-hpc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Diamond is a Python package for running tasks on HPC.
 Home-page: https://github.com/Diamond-Proj/Diamond
 Author: Haotian XIE, Gengcong YANG
 Author-email: hotinexie@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click>=8.1.3
-Requires-Dist: globus_compute_sdk>=2.20.0
-Requires-Dist: Jinja2>=3.1.4
-Requires-Dist: Requests>=2.32.2
 
 # Diamond
 
 ### Examples
 
 #### login
 Run
@@ -39,7 +37,9 @@
 
 #### submit task via script file
 1. create an container build endpoint by start endpoint in the globus endpoint server
 2. run the following command(substitude the relevent text with your config)
 ```
 diamond-hpc run-task-from-script --cmd_script /home/hotine/work/Diamond/example/sample_task/openfold_single_node_task --endpoint_id fb1ffeec-aa63-4136-8a49-f3f24608d36f --container_id a20b806c-29a8-44b4-97b6-591434ca9365 --log_path /work/09912/haotianxie/frontera/openfold_demo_single_node.log
 ```
+
+
```

### Comparing `diamond-hpc-0.0.4/diamond_hpc.egg-info/SOURCES.txt` & `diamond-hpc-0.0.5/diamond_hpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diamond-hpc-0.0.4/setup.py` & `diamond-hpc-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="diamond-hpc",
-    version="0.0.4",
+    version="0.0.5",
     author="Haotian XIE, Gengcong YANG",
     author_email="hotinexie@gmail.com",
     description="Diamond is a Python package for running tasks on HPC.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Diamond-Proj/Diamond",
     packages=find_packages(),
```


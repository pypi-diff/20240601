# Comparing `tmp/qlv-client-0.2.9.tar.gz` & `tmp/qlv-client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.2.9.tar", last modified: Wed May 15 03:18:00 2024, max compression
+gzip compressed data, was "qlv-client-0.3.0.tar", last modified: Sat Jun  1 04:19:56 2024, max compression
```

## Comparing `qlv-client-0.2.9.tar` & `qlv-client-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 03:18:00.805840 qlv-client-0.2.9/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      456 2024-05-15 03:18:00.805840 qlv-client-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 03:18:00.802363 qlv-client-0.2.9/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.2.9/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.2.9/qlv_client/api.py
--rw-rw-rw-   0        0        0     2076 2024-05-15 03:17:47.000000 qlv-client-0.2.9/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.2.9/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.2.9/qlv_client/http_client.py
--rw-rw-rw-   0        0        0    10708 2024-05-10 09:59:08.000000 qlv-client-0.2.9/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.2.9/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.2.9/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.2.9/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 03:18:00.805343 qlv-client-0.2.9/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-05-15 03:18:00.000000 qlv-client-0.2.9/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-15 03:18:00.000000 qlv-client-0.2.9/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 03:18:00.000000 qlv-client-0.2.9/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-15 03:18:00.000000 qlv-client-0.2.9/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 03:18:00.000000 qlv-client-0.2.9/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 03:18:00.806336 qlv-client-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-05-15 03:17:53.000000 qlv-client-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 04:19:56.198582 qlv-client-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-06-01 04:19:56.198086 qlv-client-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 04:19:56.195602 qlv-client-0.3.0/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.3.0/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.3.0/qlv_client/api.py
+-rw-rw-rw-   0        0        0     2225 2024-06-01 04:19:36.000000 qlv-client-0.3.0/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.3.0/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.3.0/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0    10708 2024-05-10 09:59:08.000000 qlv-client-0.3.0/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.3.0/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.3.0/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.3.0/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 04:19:56.198086 qlv-client-0.3.0/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-06-01 04:19:56.000000 qlv-client-0.3.0/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-06-01 04:19:56.000000 qlv-client-0.3.0/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 04:19:56.000000 qlv-client-0.3.0/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-06-01 04:19:56.000000 qlv-client-0.3.0/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 04:19:56.000000 qlv-client-0.3.0/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 04:19:56.198582 qlv-client-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-06-01 04:19:48.000000 qlv-client-0.3.0/setup.py
```

### Comparing `qlv-client-0.2.9/LICENSE` & `qlv-client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.9/qlv_client/api.py` & `qlv-client-0.3.0/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.9/qlv_client/config.py` & `qlv-client-0.3.0/qlv_client/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     "10002": {"code": 10002, "describe": "航班官方变价"},
     "10003": {"code": 10003, "describe": "乘客重复下单"},
     "10004": {"code": 10004, "describe": "添加乘客后点击下一步出现未知弹框"},
     "10005": {"code": 10005, "describe": "本地订单重复入库导致主键冲突"},
     "10006": {"code": 10006, "describe": "未成年人出行弹出提示框"},
     "10007": {"code": 10007, "describe": "api接口获取订单状态已取消"},
     "10008": {"code": 10008, "describe": "创建订单失败，请重试或拨打携程客服电，电话(95010)预订"},
-    "10009": {"code": 10009, "describe": "您预订的航班机票已售完，请重新查询预订"}
+    "10009": {"code": 10009, "describe": "您预订的航班机票已售完，请重新查询预订"},
+    "10010": {"code": 10010, "describe": "该价格余票不足，无法为该乘客预订该价格，请删除该乘机人或重新搜索航班"}
 }
 
 qvl_map = {
     "user_id": 186,
     "user_key": "9a68295ec90b1fc10ab94331c882bab9",
     "domain": "outsideapi.qlv88.com",
     "protocol": "http",
```

### Comparing `qlv-client-0.2.9/qlv_client/converter.py` & `qlv-client-0.3.0/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.9/qlv_client/http_client.py` & `qlv-client-0.3.0/qlv_client/http_client.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.9/qlv_client/proxy.py` & `qlv-client-0.3.0/qlv_client/proxy.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.9/qlv_client/repository.py` & `qlv-client-0.3.0/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.9/qlv_client/test.py` & `qlv-client-0.3.0/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.9/qlv_client/utils.py` & `qlv-client-0.3.0/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.2.9/setup.py` & `qlv-client-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.2.9',
+    version='0.3.0',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```


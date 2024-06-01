# Comparing `tmp/seldom-3.7.0.tar.gz` & `tmp/seldom-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldom-3.7.0.tar", max compression
+gzip compressed data, was "seldom-3.7.1.tar", max compression
```

## Comparing `seldom-3.7.0.tar` & `seldom-3.7.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    11565 2022-12-06 15:57:51.673402 seldom-3.7.0/LICENSE
--rw-r--r--   0        0        0     1483 2024-05-05 16:38:56.203308 seldom-3.7.0/pyproject.toml
--rw-r--r--   0        0        0     9999 2024-04-15 11:20:45.995202 seldom-3.7.0/README.md
--rw-r--r--   0        0        0     1305 2024-05-05 16:38:33.826783 seldom-3.7.0/seldom/__init__.py
--rw-r--r--   0        0        0     6413 2023-12-13 16:52:02.087773 seldom-3.7.0/seldom/appdriver.py
--rw-r--r--   0        0        0     1669 2022-12-06 15:57:51.730115 seldom-3.7.0/seldom/appium_lab/__init__.py
--rw-r--r--   0        0        0     3909 2023-03-13 16:12:23.693178 seldom-3.7.0/seldom/appium_lab/action.py
--rw-r--r--   0        0        0     7248 2023-12-13 00:18:29.166651 seldom-3.7.0/seldom/appium_lab/find.py
--rw-r--r--   0        0        0     3122 2023-12-20 00:17:05.579680 seldom-3.7.0/seldom/appium_lab/keyboard.py
--rw-r--r--   0        0        0      424 2023-12-25 15:36:49.142129 seldom-3.7.0/seldom/appium_lab/ocr_plugin.py
--rw-r--r--   0        0        0     1961 2023-12-25 15:34:24.464069 seldom-3.7.0/seldom/appium_lab/switch.py
--rw-r--r--   0        0        0    11736 2023-12-25 15:41:48.053185 seldom-3.7.0/seldom/case.py
--rw-r--r--   0        0        0    12379 2024-02-21 14:54:07.472569 seldom-3.7.0/seldom/cli.py
--rw-r--r--   0        0        0       64 2022-12-06 15:57:51.734123 seldom-3.7.0/seldom/db_operation/__init__.py
--rw-r--r--   0        0        0     1698 2022-12-06 15:57:51.734123 seldom-3.7.0/seldom/db_operation/base_db.py
--rw-r--r--   0        0        0      715 2022-12-06 15:57:51.734123 seldom-3.7.0/seldom/db_operation/mongo_db.py
--rw-r--r--   0        0        0     4084 2023-05-04 15:57:05.737940 seldom-3.7.0/seldom/db_operation/mssql_db.py
--rw-r--r--   0        0        0     4329 2023-05-04 15:55:58.648089 seldom-3.7.0/seldom/db_operation/mysql_db.py
--rw-r--r--   0        0        0     3773 2023-11-28 15:46:07.408523 seldom-3.7.0/seldom/db_operation/postgres_db.py
--rw-r--r--   0        0        0     3206 2023-05-04 15:54:53.581476 seldom-3.7.0/seldom/db_operation/sqlite_db.py
--rw-r--r--   0        0        0     4348 2024-05-05 15:56:27.392733 seldom-3.7.0/seldom/driver.py
--rw-r--r--   0        0        0      271 2024-01-04 17:28:13.391020 seldom-3.7.0/seldom/extend_lib/__init__.py
--rw-r--r--   0        0        0     1179 2023-10-18 16:11:35.953126 seldom-3.7.0/seldom/extend_lib/curlify.py
--rw-r--r--   0        0        0    10519 2023-10-18 16:11:35.948109 seldom-3.7.0/seldom/extend_lib/jsonpath.py
--rw-r--r--   0        0        0    26889 2023-10-18 16:11:35.942112 seldom-3.7.0/seldom/extend_lib/parameterized.py
--rw-r--r--   0        0        0     1607 2023-10-18 16:15:40.944034 seldom-3.7.0/seldom/extend_lib/tomorrow.py
--rw-r--r--   0        0        0        0 2022-12-06 15:57:51.737139 seldom-3.7.0/seldom/har2case/__init__.py
--rw-r--r--   0        0        0     4014 2023-10-18 15:53:26.993547 seldom-3.7.0/seldom/har2case/core.py
--rw-r--r--   0        0        0     3948 2022-12-06 15:57:51.738139 seldom-3.7.0/seldom/har2case/demo.har
--rw-r--r--   0        0        0     1171 2022-12-06 15:57:51.738139 seldom-3.7.0/seldom/har2case/utils.py
--rw-r--r--   0        0        0       48 2022-12-06 15:57:51.739133 seldom-3.7.0/seldom/logging/__init__.py
--rw-r--r--   0        0        0     1201 2024-02-03 10:35:36.064307 seldom-3.7.0/seldom/logging/exceptions.py
--rw-r--r--   0        0        0     2018 2023-07-16 13:48:12.015173 seldom-3.7.0/seldom/logging/log.py
--rw-r--r--   0        0        0    13534 2024-03-04 14:29:21.584809 seldom-3.7.0/seldom/request.py
--rw-r--r--   0        0        0      803 2022-12-06 15:57:51.741121 seldom-3.7.0/seldom/running/__init__.py
--rw-r--r--   0        0        0      732 2024-05-05 15:30:00.257749 seldom-3.7.0/seldom/running/config.py
--rw-r--r--   0        0        0     2477 2023-08-31 14:22:17.854138 seldom-3.7.0/seldom/running/DebugTestRunner.py
--rw-r--r--   0        0        0     7450 2022-12-15 14:14:22.344315 seldom-3.7.0/seldom/running/loader_extend.py
--rw-r--r--   0        0        0     1038 2023-07-16 13:48:12.018172 seldom-3.7.0/seldom/running/loader_hook.py
--rw-r--r--   0        0        0    15594 2024-05-05 15:40:42.575496 seldom-3.7.0/seldom/running/runner.py
--rw-r--r--   0        0        0     3119 2023-10-12 15:27:54.643152 seldom-3.7.0/seldom/skip.py
--rw-r--r--   0        0        0        0 2024-01-29 16:24:55.055502 seldom-3.7.0/seldom/swagger2case/__init__.py
--rw-r--r--   0        0        0     5280 2024-02-21 14:57:41.944522 seldom-3.7.0/seldom/swagger2case/core.py
--rw-r--r--   0        0        0    36088 2024-01-29 16:24:55.056506 seldom-3.7.0/seldom/swagger2case/swagger.json
--rw-r--r--   0        0        0       28 2022-12-06 15:57:51.743682 seldom-3.7.0/seldom/testdata/__init__.py
--rw-r--r--   0        0        0     4164 2024-04-11 13:52:00.191608 seldom-3.7.0/seldom/testdata/conversion.py
--rw-r--r--   0        0        0    11342 2024-04-11 13:18:49.359610 seldom-3.7.0/seldom/testdata/parameterization.py
--rw-r--r--   0        0        0    18847 2022-12-06 15:57:51.745728 seldom-3.7.0/seldom/testdata/random_data.py
--rw-r--r--   0        0        0    12547 2023-09-19 15:35:38.286847 seldom-3.7.0/seldom/testdata/random_func.py
--rw-r--r--   0        0        0      266 2024-01-04 17:28:24.650425 seldom-3.7.0/seldom/utils/__init__.py
--rw-r--r--   0        0        0     5599 2024-04-11 13:51:55.088380 seldom-3.7.0/seldom/utils/cache.py
--rw-r--r--   0        0        0        2 2022-12-06 15:57:51.747723 seldom-3.7.0/seldom/utils/cache_data.json
--rw-r--r--   0        0        0     1556 2024-04-11 13:51:55.089380 seldom-3.7.0/seldom/utils/dependence.py
--rw-r--r--   0        0        0     2817 2024-04-11 13:51:55.089380 seldom-3.7.0/seldom/utils/diff.py
--rw-r--r--   0        0        0     3280 2022-12-06 15:57:51.748714 seldom-3.7.0/seldom/utils/file_extend.py
--rw-r--r--   0        0        0      438 2022-12-06 15:57:51.748714 seldom-3.7.0/seldom/utils/genson.py
--rw-r--r--   0        0        0      243 2022-12-06 15:57:51.749711 seldom-3.7.0/seldom/utils/jmespath.py
--rw-r--r--   0        0        0     1500 2024-04-11 13:51:55.090367 seldom-3.7.0/seldom/utils/send_extend.py
--rw-r--r--   0        0        0     3967 2023-10-26 15:02:35.253349 seldom-3.7.0/seldom/utils/so_and_so.py
--rw-r--r--   0        0        0     1577 2022-12-06 15:57:51.750730 seldom-3.7.0/seldom/utils/thread_lab.py
--rw-r--r--   0        0        0      401 2024-01-04 17:29:14.316525 seldom-3.7.0/seldom/utils/timer.py
--rw-r--r--   0        0        0    34272 2024-04-13 15:25:54.214029 seldom-3.7.0/seldom/webdriver.py
--rw-r--r--   0        0        0    10364 2023-10-31 02:40:43.274505 seldom-3.7.0/seldom/webdriver_chaining.py
--rw-r--r--   0        0        0     2168 2024-04-11 13:32:22.825914 seldom-3.7.0/seldom/websocket_client.py
--rw-r--r--   0        0        0    11502 1970-01-01 00:00:00.000000 seldom-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11565 2022-12-06 15:57:51.673402 seldom-3.7.1/LICENSE
+-rw-r--r--   0        0        0     1534 2024-06-01 13:21:32.346565 seldom-3.7.1/pyproject.toml
+-rw-r--r--   0        0        0     9943 2024-05-13 16:38:14.422452 seldom-3.7.1/README.md
+-rw-r--r--   0        0        0     1305 2024-05-05 16:38:33.826783 seldom-3.7.1/seldom/__init__.py
+-rw-r--r--   0        0        0     6413 2023-12-13 16:52:02.087773 seldom-3.7.1/seldom/appdriver.py
+-rw-r--r--   0        0        0     1669 2022-12-06 15:57:51.730115 seldom-3.7.1/seldom/appium_lab/__init__.py
+-rw-r--r--   0        0        0     6100 2024-06-01 13:02:46.120715 seldom-3.7.1/seldom/appium_lab/action.py
+-rw-r--r--   0        0        0     7288 2024-05-30 10:29:34.337722 seldom-3.7.1/seldom/appium_lab/find.py
+-rw-r--r--   0        0        0     3120 2024-05-30 10:26:12.727673 seldom-3.7.1/seldom/appium_lab/keyboard.py
+-rw-r--r--   0        0        0      426 2024-05-30 10:25:57.359273 seldom-3.7.1/seldom/appium_lab/ocr_plugin.py
+-rw-r--r--   0        0        0     2224 2024-06-01 13:02:46.266736 seldom-3.7.1/seldom/appium_lab/switch.py
+-rw-r--r--   0        0        0    11736 2023-12-25 15:41:48.053185 seldom-3.7.1/seldom/case.py
+-rw-r--r--   0        0        0    12379 2024-02-21 14:54:07.472569 seldom-3.7.1/seldom/cli.py
+-rw-r--r--   0        0        0       64 2022-12-06 15:57:51.734123 seldom-3.7.1/seldom/db_operation/__init__.py
+-rw-r--r--   0        0        0     1698 2022-12-06 15:57:51.734123 seldom-3.7.1/seldom/db_operation/base_db.py
+-rw-r--r--   0        0        0      715 2022-12-06 15:57:51.734123 seldom-3.7.1/seldom/db_operation/mongo_db.py
+-rw-r--r--   0        0        0     4084 2023-05-04 15:57:05.737940 seldom-3.7.1/seldom/db_operation/mssql_db.py
+-rw-r--r--   0        0        0     4329 2023-05-04 15:55:58.648089 seldom-3.7.1/seldom/db_operation/mysql_db.py
+-rw-r--r--   0        0        0     3773 2023-11-28 15:46:07.408523 seldom-3.7.1/seldom/db_operation/postgres_db.py
+-rw-r--r--   0        0        0     3206 2024-06-01 12:56:26.577491 seldom-3.7.1/seldom/db_operation/sqlite_db.py
+-rw-r--r--   0        0        0     4348 2024-05-05 15:56:27.392733 seldom-3.7.1/seldom/driver.py
+-rw-r--r--   0        0        0      271 2024-01-04 17:28:13.391020 seldom-3.7.1/seldom/extend_lib/__init__.py
+-rw-r--r--   0        0        0     1179 2023-10-18 16:11:35.953126 seldom-3.7.1/seldom/extend_lib/curlify.py
+-rw-r--r--   0        0        0    10520 2024-05-29 16:59:26.806649 seldom-3.7.1/seldom/extend_lib/jsonpath.py
+-rw-r--r--   0        0        0    26889 2023-10-18 16:11:35.942112 seldom-3.7.1/seldom/extend_lib/parameterized.py
+-rw-r--r--   0        0        0     1607 2023-10-18 16:15:40.944034 seldom-3.7.1/seldom/extend_lib/tomorrow.py
+-rw-r--r--   0        0        0        0 2022-12-06 15:57:51.737139 seldom-3.7.1/seldom/har2case/__init__.py
+-rw-r--r--   0        0        0     4014 2023-10-18 15:53:26.993547 seldom-3.7.1/seldom/har2case/core.py
+-rw-r--r--   0        0        0     3948 2022-12-06 15:57:51.738139 seldom-3.7.1/seldom/har2case/demo.har
+-rw-r--r--   0        0        0     1171 2022-12-06 15:57:51.738139 seldom-3.7.1/seldom/har2case/utils.py
+-rw-r--r--   0        0        0       48 2022-12-06 15:57:51.739133 seldom-3.7.1/seldom/logging/__init__.py
+-rw-r--r--   0        0        0     1201 2024-02-03 10:35:36.064307 seldom-3.7.1/seldom/logging/exceptions.py
+-rw-r--r--   0        0        0     2018 2023-07-16 13:48:12.015173 seldom-3.7.1/seldom/logging/log.py
+-rw-r--r--   0        0        0    13534 2024-03-04 14:29:21.584809 seldom-3.7.1/seldom/request.py
+-rw-r--r--   0        0        0      803 2022-12-06 15:57:51.741121 seldom-3.7.1/seldom/running/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-05 15:30:00.257749 seldom-3.7.1/seldom/running/config.py
+-rw-r--r--   0        0        0     2477 2023-08-31 14:22:17.854138 seldom-3.7.1/seldom/running/DebugTestRunner.py
+-rw-r--r--   0        0        0     7450 2022-12-15 14:14:22.344315 seldom-3.7.1/seldom/running/loader_extend.py
+-rw-r--r--   0        0        0     1038 2023-07-16 13:48:12.018172 seldom-3.7.1/seldom/running/loader_hook.py
+-rw-r--r--   0        0        0    16099 2024-05-30 07:53:16.398182 seldom-3.7.1/seldom/running/runner.py
+-rw-r--r--   0        0        0     3119 2023-10-12 15:27:54.643152 seldom-3.7.1/seldom/skip.py
+-rw-r--r--   0        0        0        0 2024-01-29 16:24:55.055502 seldom-3.7.1/seldom/swagger2case/__init__.py
+-rw-r--r--   0        0        0     5280 2024-02-21 14:57:41.944522 seldom-3.7.1/seldom/swagger2case/core.py
+-rw-r--r--   0        0        0    36088 2024-01-29 16:24:55.056506 seldom-3.7.1/seldom/swagger2case/swagger.json
+-rw-r--r--   0        0        0       28 2022-12-06 15:57:51.743682 seldom-3.7.1/seldom/testdata/__init__.py
+-rw-r--r--   0        0        0     4164 2024-04-11 13:52:00.191608 seldom-3.7.1/seldom/testdata/conversion.py
+-rw-r--r--   0        0        0    11342 2024-05-30 07:56:38.879332 seldom-3.7.1/seldom/testdata/parameterization.py
+-rw-r--r--   0        0        0    18847 2022-12-06 15:57:51.745728 seldom-3.7.1/seldom/testdata/random_data.py
+-rw-r--r--   0        0        0    12547 2023-09-19 15:35:38.286847 seldom-3.7.1/seldom/testdata/random_func.py
+-rw-r--r--   0        0        0      266 2024-01-04 17:28:24.650425 seldom-3.7.1/seldom/utils/__init__.py
+-rw-r--r--   0        0        0     5599 2024-04-11 13:51:55.088380 seldom-3.7.1/seldom/utils/cache.py
+-rw-r--r--   0        0        0        2 2022-12-06 15:57:51.747723 seldom-3.7.1/seldom/utils/cache_data.json
+-rw-r--r--   0        0        0     1556 2024-04-11 13:51:55.089380 seldom-3.7.1/seldom/utils/dependence.py
+-rw-r--r--   0        0        0     2817 2024-04-11 13:51:55.089380 seldom-3.7.1/seldom/utils/diff.py
+-rw-r--r--   0        0        0     3280 2022-12-06 15:57:51.748714 seldom-3.7.1/seldom/utils/file_extend.py
+-rw-r--r--   0        0        0      438 2022-12-06 15:57:51.748714 seldom-3.7.1/seldom/utils/genson.py
+-rw-r--r--   0        0        0      243 2022-12-06 15:57:51.749711 seldom-3.7.1/seldom/utils/jmespath.py
+-rw-r--r--   0        0        0     1646 2024-05-30 09:54:41.856251 seldom-3.7.1/seldom/utils/send_extend.py
+-rw-r--r--   0        0        0     3967 2023-10-26 15:02:35.253349 seldom-3.7.1/seldom/utils/so_and_so.py
+-rw-r--r--   0        0        0     1577 2022-12-06 15:57:51.750730 seldom-3.7.1/seldom/utils/thread_lab.py
+-rw-r--r--   0        0        0      401 2024-01-04 17:29:14.316525 seldom-3.7.1/seldom/utils/timer.py
+-rw-r--r--   0        0        0    34272 2024-04-13 15:25:54.214029 seldom-3.7.1/seldom/webdriver.py
+-rw-r--r--   0        0        0    10364 2023-10-31 02:40:43.274505 seldom-3.7.1/seldom/webdriver_chaining.py
+-rw-r--r--   0        0        0     2168 2024-04-11 13:32:22.825914 seldom-3.7.1/seldom/websocket_client.py
+-rw-r--r--   0        0        0    11224 1970-01-01 00:00:00.000000 seldom-3.7.1/PKG-INFO
```

### Comparing `seldom-3.7.0/LICENSE` & `seldom-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/pyproject.toml` & `seldom-3.7.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seldom"
-version = "3.7.0"
+version = "3.7.1"
 description = "Seldom automation testing framework based on unittest."
 authors = ["bugmaster <fnngj@126.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 homepage = "https://seldomqa.github.io"
 repository = "https://github.com/SeldomQA/seldom"
@@ -17,26 +17,27 @@
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: Microsoft :: Windows',
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development :: Testing',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-Appium-Python-Client = "^3.1.0"
-XTestRunner = "^1.7.0"
-loguru = "~0.6.0"
+python = ">=3.8"
+Appium-Python-Client = ">=3.1.0"
+XTestRunner = ">=1.7.2"
+loguru = "~0.7.0"
 openpyxl = "^3.0.3"
 pyyaml = "^6.0"
-requests = "^2.22.0"
+requests = ">=2.22.0"
 jsonschema = "^4.10.0"
 jmespath = "^0.10.0"
 pymysql = "^1.0.0"
 genson = "~1.2.2"
 click = "^8.1.3"
 python-dateutil = "~2.8.2"
 websocket-client = "~1.7.0"
```

### Comparing `seldom-3.7.0/README.md` & `seldom-3.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 - [x] 提供丰富的断言
 - [x] 提供强大的`数据驱动`
 - [x] 平台化支持
 
 ### Install
 
 ```shell
-pip install seldom==3.6.0
+pip install seldom==3.7.0
 ```
 
 If you want to keep up with the latest version, you can install with github repository url:
 
 ```shell
 > pip install -U git+https://github.com/SeldomQA/seldom.git@master
 ```
@@ -228,32 +228,29 @@
 from appium.options.android import UiAutomator2Options
 
 import seldom
 from seldom.appium_lab.keyboard import KeyEvent
 
 
 class TestBingApp(seldom.TestCase):
-    """
-    Test Bing APP
-    """
 
     def start(self):
         self.ke = KeyEvent(self.driver)
 
     def test_bing_search(self):
         """
-        test bing bbs search
+        test bing App search
         """
         self.sleep(2)
         self.click(id_="com.microsoft.bing:id/sa_hp_header_search_box")
-        self.type(id_="com.microsoft.bing:id/sapphire_search_header_input", text="seldom")
+        self.type(id_="com.microsoft.bing:id/sapphire_search_header_input", text="seldomQA")
         self.ke.press_key("ENTER")
         self.sleep(1)
-        elem = self.get_element(xpath='//android.widget.TextView[@resource-id="count"]')
-        self.assertIn("个结果", elem.text.lower())
+        elem = self.get_elements(xpath='//android.widget.TextView')
+        self.assertIn("seldom", elem[0].text.lower())
 
 
 if __name__ == '__main__':
     capabilities = {
         'deviceName': 'ELS-AN00',
         'automationName': 'UiAutomator2',
         'platformName': 'Android',
```

### Comparing `seldom-3.7.0/seldom/__init__.py` & `seldom-3.7.1/seldom/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/appdriver.py` & `seldom-3.7.1/seldom/appdriver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/appium_lab/__init__.py` & `seldom-3.7.1/seldom/appium_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/appium_lab/action.py` & `seldom-3.7.1/seldom/appium_lab/action.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """
 appium action
 """
-from time import sleep
-from seldom.logging import log
-from seldom.appium_lab.switch import Switch
+
 from selenium.webdriver.common.action_chains import ActionChains
+from selenium.webdriver.common.actions import interaction
 from selenium.webdriver.common.actions.action_builder import ActionBuilder
 from selenium.webdriver.common.actions.pointer_input import PointerInput
-from selenium.webdriver.common.actions import interaction
+
+from seldom.appium_lab.switch import Switch
+from seldom.logging import log
 
 
 class Action(Switch):
     """
     Encapsulate basic actions: swipe, tap, etc
     """
 
-    def __init__(self, driver):
+    def __init__(self, driver=None):
         Switch.__init__(self, driver)
         self.switch_to_app()
         self._size = self.driver.get_window_size()
-        self.width = self._size.get("width")     # {'width': 1080, 'height': 2028}
-        self.height = self._size.get("height")   # {'width': 1080, 'height': 2028}
+        self.width = self._size.get("width")  # {'width': 1080, 'height': 2028}
+        self.height = self._size.get("height")  # {'width': 1080, 'height': 2028}
 
     def size(self) -> dict:
         """
         return screen resolution.
         """
         log.info(f"screen resolution: {self._size}")
         return self._size
@@ -41,25 +42,25 @@
         actions = ActionChains(self.driver)
         actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
         actions.w3c_actions.pointer_action.move_to_location(x, y)
         actions.w3c_actions.pointer_action.pointer_down()
         actions.w3c_actions.pointer_action.pause(0.1)
         actions.w3c_actions.pointer_action.release()
         actions.perform()
-        sleep(2)
+        self.sleep(2)
 
     def swipe_up(self, times: int = 1, upper: bool = False):
         """
         swipe up
         :param times: swipe times
         :param upper: Keyboard screen occlusion, swipe only the upper half of the area.
         :return:
         """
         self.switch_to_app()
-        log.info(f"swipe up {times} times")
+        log.info(f"⬆️ swipe up {times} times")
         x_start = int(self.width / 2)
         x_end = int(self.width / 2)
 
         if upper is True:
             self.height = (self.height / 2)
 
         y_start = int((self.height / 3) * 2)
@@ -69,25 +70,25 @@
             actions = ActionChains(self.driver)
             actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
             actions.w3c_actions.pointer_action.move_to_location(x_start, y_start)
             actions.w3c_actions.pointer_action.pointer_down()
             actions.w3c_actions.pointer_action.move_to_location(x_end, y_end)
             actions.w3c_actions.pointer_action.release()
             actions.perform()
-            sleep(1)
+            self.sleep(1)
 
     def swipe_down(self, times: int = 1, upper: bool = False) -> None:
         """
         swipe down
         :param times: swipe times
         :param upper: Keyboard screen occlusion, swipe only the upper half of the area.
         :return:
         """
         self.switch_to_app()
-        log.info(f"swipe down {times} times")
+        log.info(f"⬇️ swipe down {times} times")
         x_start = int(self.width / 2)
         x_end = int(self.width / 2)
 
         if upper is True:
             self.height = (self.height / 2)
 
         y_start = int((self.height / 3) * 1)
@@ -97,8 +98,58 @@
             actions = ActionChains(self.driver)
             actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
             actions.w3c_actions.pointer_action.move_to_location(x_start, y_start)
             actions.w3c_actions.pointer_action.pointer_down()
             actions.w3c_actions.pointer_action.move_to_location(x_end, y_end)
             actions.w3c_actions.pointer_action.release()
             actions.perform()
-            sleep(1)
+            self.sleep(1)
+
+    def swipe_left(self, times: int = 1, width_percentage: float = 0.8):
+        """
+        Swipe left
+        :param times: swipe times
+        :param width_percentage: Percentage of the screen width to swipe (default 80%)
+        :return:
+        """
+        self.switch_to_app()
+        log.info(f"⬅️ swipe left {times} times")
+
+        x_start = int(self.width * (1 - width_percentage / 2))
+        x_end = int(self.width * width_percentage / 2)
+        y_start = int(self.height / 2)
+        y_end = int(self.height / 2)
+
+        for _ in range(times):
+            actions = ActionChains(self.driver)
+            actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
+            actions.w3c_actions.pointer_action.move_to_location(x_start, y_start)
+            actions.w3c_actions.pointer_action.pointer_down()
+            actions.w3c_actions.pointer_action.move_to_location(x_end, y_end)
+            actions.w3c_actions.pointer_action.release()
+            actions.perform()
+            self.sleep(1)
+
+    def swipe_right(self, times: int = 1, width_percentage: float = 0.8):
+        """
+        Swipe right
+        :param times: swipe times
+        :param width_percentage: Percentage of the screen width to swipe (default 80%)
+        :return:
+        """
+        self.switch_to_app()
+        log.info(f"➡️ swipe right {times} times")
+
+        x_start = int(self.width * width_percentage / 2)
+        x_end = int(self.width * (1 - width_percentage / 2))
+        y_start = int(self.height / 2)
+        y_end = int(self.height / 2)
+
+        for _ in range(times):
+            actions = ActionChains(self.driver)
+            actions.w3c_actions = ActionBuilder(self.driver, mouse=PointerInput(interaction.POINTER_TOUCH, "touch"))
+            actions.w3c_actions.pointer_action.move_to_location(x_start, y_start)
+            actions.w3c_actions.pointer_action.pointer_down()
+            actions.w3c_actions.pointer_action.move_to_location(x_end, y_end)
+            actions.w3c_actions.pointer_action.release()
+            actions.perform()
+            self.sleep(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `seldom-3.7.0/seldom/appium_lab/find.py` & `seldom-3.7.1/seldom/appium_lab/find.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 find element by text
 """
-from time import sleep
+
 from appium.webdriver.common.appiumby import AppiumBy
-from seldom.logging import log
+
 from seldom.appium_lab.switch import Switch
+from seldom.logging import log
 
 
 class FindByText(Switch):
     """
     Find elements based on text
     """
 
@@ -28,15 +29,15 @@
         :param text: text
         :return:
         """
         elems = self.driver.find_elements(AppiumBy.CLASS_NAME, class_name)
         for _ in range(3):
             if len(elems) > 0:
                 break
-            sleep(1)
+            self.sleep(1)
 
         for elem in elems:
             if elem.get_attribute(attribute) is None:
                 continue
             attribute_text = self.__remove_unprintable_chars(elem.get_attribute(attribute))
             if text in attribute_text:
                 log.info(f'find -> {attribute_text}')
@@ -60,15 +61,15 @@
         else:
             raise ValueError("parameter error, setting text/content_desc")
 
         for _ in range(3):
             elem = self.__find(class_name="android.view.View", attribute=attribute, text=_text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_edit_text(self, text: str):
         """
@@ -77,15 +78,15 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="android.widget.EditText", attribute="text", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_button(self, text: str = None, content_desc: str = None):
         """
@@ -104,15 +105,15 @@
         else:
             raise ValueError("parameter error, setting text/content_desc")
 
         for _ in range(3):
             elem = self.__find(class_name="android.widget.Button", attribute=attribute, text=_text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_text_view(self, text: str):
         """
@@ -121,15 +122,15 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="android.widget.TextView", attribute="text", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_image_view(self, text: str):
         """
@@ -138,15 +139,15 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="android.widget.ImageView", attribute="content-desc", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_check_box(self, text: str):
         """
@@ -155,15 +156,15 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="android.widget.CheckBox", attribute="text", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_static_text(self, text: str):
         """
@@ -172,15 +173,15 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="XCUIElementTypeStaticText", attribute="name", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_other(self, text: str):
         """
@@ -189,15 +190,15 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="XCUIElementTypeOther", attribute="name", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_text_field(self, text: str):
         """
@@ -206,15 +207,15 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="XCUIElementTypeTextField", attribute="name", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_image(self, text: str):
         """
@@ -223,15 +224,15 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="XCUIElementTypeImage", attribute="name", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
 
     def find_ios_button(self, text: str):
         """
@@ -240,12 +241,12 @@
         :return:
         """
         self.switch_to_app()
         for _ in range(3):
             elem = self.__find(class_name="XCUIElementTypeButton", attribute="name", text=text)
             if elem is not None:
                 break
-            sleep(1)
+            self.sleep(1)
         else:
             raise ValueError(f"Unable to find -> {text}")
 
         return elem
```

### Comparing `seldom-3.7.0/seldom/appium_lab/keyboard.py` & `seldom-3.7.1/seldom/appium_lab/keyboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 App keyboard operation
 """
 from seldom.logging import log
 
-
 keycodes = {
     '0': 7,
     '1': 8,
     '2': 9,
     '3': 10,
     '4': 11,
     '5': 12,
```

### Comparing `seldom-3.7.0/seldom/appium_lab/switch.py` & `seldom-3.7.1/seldom/appium_lab/switch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """
 switch app context
 """
+import time
+
 from seldom.logging import log
+from seldom import Seldom
 
 
 class Switch:
     """
     switch context by appium
     """
 
-    def __init__(self, driver):
-        self.driver = driver
+    def __init__(self, driver=None):
+        self.driver = Seldom.driver
+        if driver is not None:
+            self.driver = driver
 
     def context(self):
         """
         Returns the current context of the current session.
         """
         current_context = self.driver.current_context
         all_context = self.driver.contexts
@@ -59,7 +64,15 @@
     def switch_to_ocr(self) -> None:
         """
         Switch to OCR app.
         help: https://github.com/jlipps/appium-ocr-plugin
         """
         log.info("🔀 switch to OCR.")
         self.driver.switch_to.context('OCR')
+
+    @staticmethod
+    def sleep(sec):
+        """
+        python time.sleep()
+        :param sec:
+        """
+        time.sleep(sec)
```

### Comparing `seldom-3.7.0/seldom/case.py` & `seldom-3.7.1/seldom/case.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/cli.py` & `seldom-3.7.1/seldom/cli.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/db_operation/base_db.py` & `seldom-3.7.1/seldom/db_operation/base_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/db_operation/mongo_db.py` & `seldom-3.7.1/seldom/db_operation/mongo_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/db_operation/mssql_db.py` & `seldom-3.7.1/seldom/db_operation/mssql_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/db_operation/mysql_db.py` & `seldom-3.7.1/seldom/db_operation/mysql_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/db_operation/postgres_db.py` & `seldom-3.7.1/seldom/db_operation/postgres_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/db_operation/sqlite_db.py` & `seldom-3.7.1/seldom/db_operation/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/driver.py` & `seldom-3.7.1/seldom/driver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/extend_lib/curlify.py` & `seldom-3.7.1/seldom/extend_lib/curlify.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/extend_lib/jsonpath.py` & `seldom-3.7.1/seldom/extend_lib/jsonpath.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         loc = loc.replace("&&", " and ").replace("||", " or ")
 
         # replace !@.name with 'name' not in obj
         # XXX handle !@.name.name.name....
         def notvar(m):
             return "'%s' not in __obj" % m.group(1)
 
-        loc = re.sub("!@\.([a-zA-Z@_0-9-]*)", notvar, loc)
+        loc = re.sub(r"!@\.([a-zA-Z@_0-9-]*)", notvar, loc)
 
         # replace @.name.... with __obj['name']....
         # handle @.name[.name...].length
         def varmatch(m):
             def brackets(elts):
                 ret = "__obj"
                 for e in elts:
```

### Comparing `seldom-3.7.0/seldom/extend_lib/parameterized.py` & `seldom-3.7.1/seldom/extend_lib/parameterized.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/extend_lib/tomorrow.py` & `seldom-3.7.1/seldom/extend_lib/tomorrow.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/har2case/core.py` & `seldom-3.7.1/seldom/har2case/core.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/har2case/demo.har` & `seldom-3.7.1/seldom/har2case/demo.har`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/har2case/utils.py` & `seldom-3.7.1/seldom/har2case/utils.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/logging/exceptions.py` & `seldom-3.7.1/seldom/logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/logging/log.py` & `seldom-3.7.1/seldom/logging/log.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/request.py` & `seldom-3.7.1/seldom/request.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/running/__init__.py` & `seldom-3.7.1/seldom/running/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/running/config.py` & `seldom-3.7.1/seldom/running/config.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/running/DebugTestRunner.py` & `seldom-3.7.1/seldom/running/DebugTestRunner.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/running/loader_extend.py` & `seldom-3.7.1/seldom/running/loader_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/running/loader_hook.py` & `seldom-3.7.1/seldom/running/loader_hook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/running/runner.py` & `seldom-3.7.1/seldom/running/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,34 +28,34 @@
 
 INIT_FILE = os.path.join(os.path.dirname(os.path.dirname(os.path.abspath(__file__))), "__init__.py")
 _version_re = re.compile(r'__version__\s+=\s+(.*)')
 with open(INIT_FILE, 'rb') as f:
     VERSION = str(ast.literal_eval(_version_re.search(
         f.read().decode('utf-8')).group(1)))
 
-SELDOM_STR = f"""
+SELDOM_STR = r"""
               __    __              
    ________  / /___/ /___  ____ ____ 
   / ___/ _ \/ / __  / __ \/ __ ` ___/
  (__  )  __/ / /_/ / /_/ / / / / / /
-/____/\___/_/\__,_/\____/_/ /_/ /_/  v{VERSION}
+/____/\___/_/\__,_/\____/_/ /_/ /_/  v""" + VERSION + """
 -----------------------------------------
                              @itest.info
 """
 
 
 class TestMain:
     """
     Reimplemented Seldom Runner, Support for Web and API
     """
     TestSuits = []
 
     def __init__(
             self,
-            path: str = None,
+            path: [str, list] = None,
             case: str = None,
             browser: [str or dict] = None,
             base_url: str = None,
             debug: bool = False,
             timeout: int = 10,
             app_server=None,
             app_info=None,
@@ -145,30 +145,43 @@
                 this_file = file_path.split("\\")[-1]
             elif "/" in file_path:
                 this_file = file_path.split("/")[-1]
             else:
                 this_file = file_path
             self.TestSuits = seldomTestLoader.discover(file_dir, this_file)
         else:
-            if len(self.path) > 3:
-                if self.path[-3:] == ".py":
-                    if "/" in self.path:
-                        path_list = self.path.split("/")
-                        path_dir = self.path.replace(path_list[-1], "")
-                        self.TestSuits = seldomTestLoader.discover(path_dir, pattern=path_list[-1])
-                    elif "\\" in self.path:
-                        path_list = self.path.split("\\")
-                        path_dir = self.path.replace(path_list[-1], "")
-                        self.TestSuits = seldomTestLoader.discover(path_dir, pattern=path_list[-1])
+            paths = []
+            if isinstance(self.path, str):
+                paths.append(self.path)
+            elif isinstance(self.path, list):
+                paths = self.path
+            else:
+                raise TypeError("The `path` type is incorrect. Only list or string is supported.")
+
+            self.TestSuits = unittest.TestSuite()
+            for path in paths:
+                log.info(f"TestLoader: {path}")
+                if len(path) > 3:
+                    if path[-3:] == ".py":
+                        if "/" in path:
+                            path_list = path.split("/")
+                            path_dir = path.replace(path_list[-1], "")
+                            test_suits = seldomTestLoader.discover(path_dir, pattern=path_list[-1])
+                        elif "\\" in path:
+                            path_list = path.split("\\")
+                            path_dir = path.replace(path_list[-1], "")
+                            test_suits = seldomTestLoader.discover(path_dir, pattern=path_list[-1])
+                        else:
+                            test_suits = seldomTestLoader.discover(os.getcwd(), pattern=path)
                     else:
-                        self.TestSuits = seldomTestLoader.discover(os.getcwd(), pattern=self.path)
+                        test_suits = seldomTestLoader.rediscover(path)
                 else:
-                    self.TestSuits = seldomTestLoader.rediscover(self.path)
-            else:
-                self.TestSuits = seldomTestLoader.discover(self.path)
+                    test_suits = seldomTestLoader.discover(path)
+
+                self.TestSuits.addTest(test_suits)
 
         if self.auto is True:
             self.run(self.TestSuits)
 
             # ----- Close browser globally -----
             self.close_browser()
```

### Comparing `seldom-3.7.0/seldom/skip.py` & `seldom-3.7.1/seldom/skip.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/swagger2case/core.py` & `seldom-3.7.1/seldom/swagger2case/core.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/swagger2case/swagger.json` & `seldom-3.7.1/seldom/swagger2case/swagger.json`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/testdata/conversion.py` & `seldom-3.7.1/seldom/testdata/conversion.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/testdata/parameterization.py` & `seldom-3.7.1/seldom/testdata/parameterization.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/testdata/random_data.py` & `seldom-3.7.1/seldom/testdata/random_data.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/testdata/random_func.py` & `seldom-3.7.1/seldom/testdata/random_func.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/utils/cache.py` & `seldom-3.7.1/seldom/utils/cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/utils/dependence.py` & `seldom-3.7.1/seldom/utils/dependence.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/utils/diff.py` & `seldom-3.7.1/seldom/utils/diff.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/utils/file_extend.py` & `seldom-3.7.1/seldom/utils/file_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/utils/send_extend.py` & `seldom-3.7.1/seldom/utils/send_extend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 send message file
 """
 import os
-from XTestRunner import SMTP as XSMTP
+
 from XTestRunner import DingTalk as XDingTalk
 from XTestRunner import FeiShu as XFeiShu
+from XTestRunner import SMTP as XSMTP
 from XTestRunner import Weinxin as XWeinxin
+from XTestRunner.config import RunResult as XRunResult
+
 from seldom.running.config import BrowserConfig
 from seldom.utils import file
 
 
 class SMTP(XSMTP):
     """send email class"""
 
@@ -47,7 +50,13 @@
     """
 
 
 class Weinxin(XWeinxin):
     """
     send weixin, Inherit XTestRunner weixin Class
     """
+
+
+class RunResult(XRunResult):
+    """
+    XTestRunner Test run results
+    """
```

### Comparing `seldom-3.7.0/seldom/utils/so_and_so.py` & `seldom-3.7.1/seldom/utils/so_and_so.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/utils/thread_lab.py` & `seldom-3.7.1/seldom/utils/thread_lab.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/webdriver.py` & `seldom-3.7.1/seldom/webdriver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/webdriver_chaining.py` & `seldom-3.7.1/seldom/webdriver_chaining.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/seldom/websocket_client.py` & `seldom-3.7.1/seldom/websocket_client.py`

 * *Files identical despite different names*

### Comparing `seldom-3.7.0/PKG-INFO` & `seldom-3.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 Metadata-Version: 2.1
 Name: seldom
-Version: 3.7.0
+Version: 3.7.1
 Summary: Seldom automation testing framework based on unittest.
 Home-page: https://seldomqa.github.io
 License: Apache-2.0
 Keywords: sedom,selenium,appium,requests
 Author: bugmaster
 Author-email: fnngj@126.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: Appium-Python-Client (>=3.1.0,<4.0.0)
-Requires-Dist: XTestRunner (>=1.7.0,<2.0.0)
+Requires-Dist: Appium-Python-Client (>=3.1.0)
+Requires-Dist: XTestRunner (>=1.7.2)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: genson (>=1.2.2,<1.3.0)
 Requires-Dist: jmespath (>=0.10.0,<0.11.0)
 Requires-Dist: jsonschema (>=4.10.0,<5.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openpyxl (>=3.0.3,<4.0.0)
 Requires-Dist: pymysql (>=1.0.0,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<2.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.22.0,<3.0.0)
+Requires-Dist: requests (>=2.22.0)
 Requires-Dist: websocket-client (>=1.7.0,<1.8.0)
 Project-URL: Documentation, https://seldomqa.github.io
 Project-URL: Repository, https://github.com/SeldomQA/seldom
 Description-Content-Type: text/markdown
 
 [GitHub](https://github.com/SeldomQA/seldom) | [Gitee](https://gitee.com/fnngj/seldom) |
 
@@ -59,15 +55,15 @@
 - [x] 提供丰富的断言
 - [x] 提供强大的`数据驱动`
 - [x] 平台化支持
 
 ### Install
 
 ```shell
-pip install seldom==3.6.0
+pip install seldom==3.7.0
 ```
 
 If you want to keep up with the latest version, you can install with github repository url:
 
 ```shell
 > pip install -U git+https://github.com/SeldomQA/seldom.git@master
 ```
@@ -271,32 +267,29 @@
 from appium.options.android import UiAutomator2Options
 
 import seldom
 from seldom.appium_lab.keyboard import KeyEvent
 
 
 class TestBingApp(seldom.TestCase):
-    """
-    Test Bing APP
-    """
 
     def start(self):
         self.ke = KeyEvent(self.driver)
 
     def test_bing_search(self):
         """
-        test bing bbs search
+        test bing App search
         """
         self.sleep(2)
         self.click(id_="com.microsoft.bing:id/sa_hp_header_search_box")
-        self.type(id_="com.microsoft.bing:id/sapphire_search_header_input", text="seldom")
+        self.type(id_="com.microsoft.bing:id/sapphire_search_header_input", text="seldomQA")
         self.ke.press_key("ENTER")
         self.sleep(1)
-        elem = self.get_element(xpath='//android.widget.TextView[@resource-id="count"]')
-        self.assertIn("个结果", elem.text.lower())
+        elem = self.get_elements(xpath='//android.widget.TextView')
+        self.assertIn("seldom", elem[0].text.lower())
 
 
 if __name__ == '__main__':
     capabilities = {
         'deviceName': 'ELS-AN00',
         'automationName': 'UiAutomator2',
         'platformName': 'Android',
```


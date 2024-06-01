# Comparing `tmp/NsparkleLog-1.0.2.tar.gz` & `tmp/NsparkleLog-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NsparkleLog-1.0.2.tar", last modified: Thu May 30 13:49:58 2024, max compression
+gzip compressed data, was "NsparkleLog-1.0.3.tar", last modified: Fri May 31 13:43:55 2024, max compression
```

## Comparing `NsparkleLog-1.0.2.tar` & `NsparkleLog-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.798913 NsparkleLog-1.0.2/
--rw-rw-rw-   0        0        0        0 2024-05-25 15:37:29.000000 NsparkleLog-1.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.553981 NsparkleLog-1.0.2/NsparkleLog/
--rw-rw-rw-   0        0        0      148 2024-05-26 13:00:49.000000 NsparkleLog-1.0.2/NsparkleLog/Interfaces.py
--rw-rw-rw-   0        0        0      265 2024-05-30 13:32:00.000000 NsparkleLog-1.0.2/NsparkleLog/__init__.py
--rw-rw-rw-   0        0        0      145 2024-05-30 13:22:36.000000 NsparkleLog-1.0.2/NsparkleLog/_env.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.768975 NsparkleLog-1.0.2/NsparkleLog/core/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 NsparkleLog-1.0.2/NsparkleLog/core/__init__.py
--rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 NsparkleLog-1.0.2/NsparkleLog/core/_excformat.py
--rw-rw-rw-   0        0        0     1467 2024-05-30 12:50:00.000000 NsparkleLog-1.0.2/NsparkleLog/core/_formatter.py
--rw-rw-rw-   0        0        0     4026 2024-05-30 13:37:07.000000 NsparkleLog-1.0.2/NsparkleLog/core/_handler.py
--rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 NsparkleLog-1.0.2/NsparkleLog/core/_level.py
--rw-rw-rw-   0        0        0     5799 2024-05-30 13:32:46.000000 NsparkleLog-1.0.2/NsparkleLog/core/_logger.py
--rw-rw-rw-   0        0        0     1337 2024-05-30 12:50:46.000000 NsparkleLog-1.0.2/NsparkleLog/core/_manager.py
--rw-rw-rw-   0        0        0      312 2024-05-26 14:43:06.000000 NsparkleLog-1.0.2/NsparkleLog/dependencies.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.770969 NsparkleLog-1.0.2/NsparkleLog/plugins/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.2/NsparkleLog/plugins/__init__.py
--rw-rw-rw-   0        0        0      824 2024-05-30 13:02:42.000000 NsparkleLog-1.0.2/NsparkleLog/plugins/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.774958 NsparkleLog-1.0.2/NsparkleLog/utils/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.2/NsparkleLog/utils/__init__.py
--rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 NsparkleLog-1.0.2/NsparkleLog/utils/_color.py
--rw-rw-rw-   0        0        0      178 2024-05-26 13:01:00.000000 NsparkleLog-1.0.2/NsparkleLog/utils/_types.py
-drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.775957 NsparkleLog-1.0.2/NsparkleLog.egg-info/
--rw-rw-rw-   0        0        0     3676 2024-05-30 13:49:55.000000 NsparkleLog-1.0.2/NsparkleLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2024-05-30 13:49:56.000000 NsparkleLog-1.0.2/NsparkleLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 13:49:55.000000 NsparkleLog-1.0.2/NsparkleLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-30 13:49:55.000000 NsparkleLog-1.0.2/NsparkleLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3676 2024-05-30 13:49:58.776954 NsparkleLog-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-30 13:49:58.798913 NsparkleLog-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-26 13:01:15.000000 NsparkleLog-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.158206 NsparkleLog-1.0.3/
+-rw-rw-rw-   0        0        0        0 2024-05-25 15:37:29.000000 NsparkleLog-1.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.105716 NsparkleLog-1.0.3/NsparkleLog/
+-rw-rw-rw-   0        0        0      148 2024-05-26 13:00:49.000000 NsparkleLog-1.0.3/NsparkleLog/Interfaces.py
+-rw-rw-rw-   0        0        0      265 2024-05-31 13:33:31.000000 NsparkleLog-1.0.3/NsparkleLog/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-05-31 09:30:54.000000 NsparkleLog-1.0.3/NsparkleLog/_env.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.147899 NsparkleLog-1.0.3/NsparkleLog/core/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 NsparkleLog-1.0.3/NsparkleLog/core/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 NsparkleLog-1.0.3/NsparkleLog/core/_excformat.py
+-rw-rw-rw-   0        0        0     1467 2024-05-30 12:50:00.000000 NsparkleLog-1.0.3/NsparkleLog/core/_formatter.py
+-rw-rw-rw-   0        0        0     4020 2024-05-31 13:36:13.000000 NsparkleLog-1.0.3/NsparkleLog/core/_handler.py
+-rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 NsparkleLog-1.0.3/NsparkleLog/core/_level.py
+-rw-rw-rw-   0        0        0     5799 2024-05-30 13:32:46.000000 NsparkleLog-1.0.3/NsparkleLog/core/_logger.py
+-rw-rw-rw-   0        0        0     1337 2024-05-30 12:50:46.000000 NsparkleLog-1.0.3/NsparkleLog/core/_manager.py
+-rw-rw-rw-   0        0        0      329 2024-05-31 09:32:27.000000 NsparkleLog-1.0.3/NsparkleLog/dependencies.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.149893 NsparkleLog-1.0.3/NsparkleLog/plugins/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.3/NsparkleLog/plugins/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-31 09:49:56.000000 NsparkleLog-1.0.3/NsparkleLog/plugins/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.153748 NsparkleLog-1.0.3/NsparkleLog/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.3/NsparkleLog/utils/__init__.py
+-rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 NsparkleLog-1.0.3/NsparkleLog/utils/_color.py
+-rw-rw-rw-   0        0        0      177 2024-05-31 09:42:52.000000 NsparkleLog-1.0.3/NsparkleLog/utils/_types.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:43:55.154749 NsparkleLog-1.0.3/NsparkleLog.egg-info/
+-rw-rw-rw-   0        0        0     3676 2024-05-31 13:43:54.000000 NsparkleLog-1.0.3/NsparkleLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2024-05-31 13:43:54.000000 NsparkleLog-1.0.3/NsparkleLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 13:43:54.000000 NsparkleLog-1.0.3/NsparkleLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-31 13:43:54.000000 NsparkleLog-1.0.3/NsparkleLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3676 2024-05-31 13:43:55.156211 NsparkleLog-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-31 13:43:55.158206 NsparkleLog-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-26 13:01:15.000000 NsparkleLog-1.0.3/setup.py
```

### Comparing `NsparkleLog-1.0.2/NsparkleLog/core/_excformat.py` & `NsparkleLog-1.0.3/NsparkleLog/core/_excformat.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.2/NsparkleLog/core/_formatter.py` & `NsparkleLog-1.0.3/NsparkleLog/core/_formatter.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.2/NsparkleLog/core/_handler.py` & `NsparkleLog-1.0.3/NsparkleLog/core/_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,28 +96,28 @@
         string = super().handle(name, threadName, filename, lineno, funcName, moduleName, message, level, color)
         if level >= self.level:
            self.queue.put(string)
         return
 
     def writeToFile(self) -> None:
         with open(self.filename, self.mode, encoding=self.encoding) as f:
-            while isMainThreadAlive():
+            while True:
                 try:
                     string = self.queue.get(timeout=1)  # 使用timeout来避免忙等
                     with self.lock:
-                        f.write(string + "\n")
+                        f.write(f"{string}\n")
                         f.flush()
                     self.queue.task_done()
                 except queue.Empty:
                     if  not isMainThreadAlive():
                         break
                     else:
                         continue
                 except Exception as e:
                     stderr.write(f"{e}\n")
         
 
-class RotatingFileHandler:
+class RotatingFileHandler(Handler):
     """
     日志文件按大小轮换写入器
     """
     pass
```

### Comparing `NsparkleLog-1.0.2/NsparkleLog/core/_logger.py` & `NsparkleLog-1.0.3/NsparkleLog/core/_logger.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.2/NsparkleLog/core/_manager.py` & `NsparkleLog-1.0.3/NsparkleLog/core/_manager.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.2/NsparkleLog/utils/_color.py` & `NsparkleLog-1.0.3/NsparkleLog/utils/_color.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.2/NsparkleLog.egg-info/PKG-INFO` & `NsparkleLog-1.0.3/NsparkleLog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsparkleLog
-Version: 1.0.2
+Version: 1.0.3
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NsparkleLog-1.0.2/NsparkleLog.egg-info/SOURCES.txt` & `NsparkleLog-1.0.3/NsparkleLog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.2/PKG-INFO` & `NsparkleLog-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsparkleLog
-Version: 1.0.2
+Version: 1.0.3
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NsparkleLog-1.0.2/setup.py` & `NsparkleLog-1.0.3/setup.py`

 * *Files identical despite different names*


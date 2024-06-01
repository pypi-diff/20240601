# Comparing `tmp/dalpha-0.5.5.tar.gz` & `tmp/dalpha-0.5.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.5.tar", max compression
+gzip compressed data, was "dalpha-0.5.5rc0.tar", max compression
```

## Comparing `dalpha-0.5.5.tar` & `dalpha-0.5.5rc0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.5/README.md
--rw-r--r--   0        0        0     2090 2024-05-22 02:06:09.763823 dalpha-0.5.5/dalpha/__init__.py
--rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.5/dalpha/agent.py
--rw-r--r--   0        0        0     7889 2024-05-22 02:06:09.763823 dalpha-0.5.5/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.5/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.5/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.5/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.5/dalpha/dto.py
--rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.5/dalpha/exception.py
--rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.5/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.5/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.5/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.5/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.5/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.5/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6689 2024-05-22 02:06:09.767823 dalpha-0.5.5/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.5/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.5/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.5/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.5/dalpha/request.py
--rw-r--r--   0        0        0     2673 2024-05-23 10:37:42.216823 dalpha-0.5.5/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.5/dalpha/signal_handler.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.5/dalpha/update_agent.py
--rw-r--r--   0        0        0      946 2024-05-23 10:37:42.216823 dalpha-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 dalpha-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.5rc0/README.md
+-rw-r--r--   0        0        0     2104 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/__init__.py
+-rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.5rc0/dalpha/agent.py
+-rw-r--r--   0        0        0     7889 2024-05-22 02:06:09.763823 dalpha-0.5.5rc0/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.5rc0/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/context.py
+-rw-r--r--   0        0        0     2970 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0     3087 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/data_update_consumer.py
+-rw-r--r--   0        0        0     1798 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/dto.py
+-rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.5rc0/dalpha/exception.py
+-rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.5rc0/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.5rc0/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.5rc0/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6689 2024-05-22 02:06:09.767823 dalpha-0.5.5rc0/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.5rc0/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.5rc0/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.5rc0/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.5rc0/dalpha/request.py
+-rw-r--r--   0        0        0     2673 2024-05-23 10:37:42.216823 dalpha-0.5.5rc0/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.5rc0/dalpha/signal_handler.py
+-rw-r--r--   0        0        0     4612 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-06-01 12:03:50.256168 dalpha-0.5.5rc0/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.5rc0/PKG-INFO
```

### Comparing `dalpha-0.5.5/README.md` & `dalpha-0.5.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/__init__.py` & `dalpha-0.5.5rc0/dalpha/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 __load_config(cfg_path)
 check_package_version("dalpha")
 
 from dalpha.signal_handler import get_shutdown_requested
 from dalpha.context import clear_context_evaluate, set_context, set_context_evaluate, get_context, Context
 from dalpha.logging.events import Event
 
-from dalpha.dto import InferenceResult
+from dalpha.dto import InferenceResult, UpdateResult
 from dalpha.exception import BaseStatusCode, ExpectedError, WaitException
 
 from dalpha.agent import Agent
 from dalpha.cobra_cls import Cobra
 from dalpha.data_update_cls import DalphaDataUpdater
 from dalpha.inference_cls import DalphaAI
 from dalpha.redis_cls import DalphaRedis
```

### Comparing `dalpha-0.5.5/dalpha/agent.py` & `dalpha-0.5.5rc0/dalpha/agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/backend_cli.py` & `dalpha-0.5.5rc0/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/cobra_cls.py` & `dalpha-0.5.5rc0/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/context.py` & `dalpha-0.5.5rc0/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/data_update_cls.py` & `dalpha-0.5.5rc0/dalpha/data_update_cls.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,90 @@
 import sys
 import time
 import traceback
 from typing import Callable, Dict
 
-from dalpha.dto import InferenceResult
+from dalpha.data_update_consumer import DataUpdateItem
+from dalpha.dto import UpdateResult
 from dalpha.logging import logger
-from dalpha.exception import ExpectedError
-from dalpha.agent import Agent
+from dalpha.exception import ExpectedError, WaitException
+from dalpha.update_agent import UpdateAgent
 
 class DalphaDataUpdater:
     def __init__(
         self,
-        kafka_topic: str,
-        inference: Callable[[Agent, Dict, int, int, bool], InferenceResult], # TODO: InferenceResult에 해당하는 UpdateResult가 있는지?
+        process: Callable[[Dict, DataUpdateItem, bool], UpdateResult],
         load_globals: Callable[[], Dict],
+        kafka_topic: str = "",
+        api_id: int = 0,
+        alert: bool = False
     ):
-        self.agent = Agent(api_id=0, kafka_topic=kafka_topic)
-        self.inference = inference
+        self.wait_flag = True
+
+        self.update_agent = UpdateAgent(kafka_topic, api_id=api_id)
+        self.process = process
         self.globals = load_globals()
+        self.api_id = api_id
+        self.alert = alert
 
     def _poll_input(self):
         try:
-            return self.agent.update_poll()
+            input_json =  self.update_agent.poll()
         except SystemExit:
             logger.info("SystemExit caught, exiting.")
             sys.exit(0)
         except Exception as e:
             logger.warning(f"Error during update_poll: {e}")
-            return None
+            input_json = None
+        
+        if input_json is None:
+            if self.wait_flag:
+                logger.info("waiting...")
+                self.wait_flag = False
+            raise WaitException("No input_json")
+        else:
+            return input_json
+
 
     def _pipeline(self):
-        input_json = self._poll_input()
-        if input_json is None:
-            logger.info("No input for update")
+        try:
+            input_json = self._poll_input()
+        except WaitException:
             return
         
         logger.info("processing...")
 
         try:
-            file = input_json["file"]
-            bucket, key, size = (
-                file["bucket"],
-                file["key"],
-                file["size"],
-            )
-        except KeyError as e:
-            error_message = f"input format is not correct!\n{e}"
-            logger.error(error_message)
-            error_json = {"reason": error_message}
-            self.agent.update_error(output=error_json)
-            return
-        
-        try:
-            download_path = 'temp'
-            self.agent.download_from_s3(
-                bucket, key, download_path
-            )
-        except Exception as e:
-            error_message = f"Error during download_from_s3: {e}\n{traceback.format_exc()}"
-            logger.error(error_message)
-            error_json = {"reason": error_message}
-            self.agent.update_error(output=error_json)
-            return
-        
-        try:
             logger.info("Data update starts...")
             update_start_time = time.time()
-            ## TODO : data update code
+            data_update_result: UpdateResult = self.process(
+                globals = self.globals,
+                data_update_item = input_json,
+                use_mock = False
+            )
             update_end_time = time.time()
             logger.info(f"Data update is done. Time taken: {update_end_time - update_start_time:.2f} sec")
         except ExpectedError as expected_error:
-            self.agent.update_error(output=expected_error.error_json)
+            self.update_agent.validate_error(output=expected_error.error_json, alert=self.alert)
+            self.update_agent.close()
+
             return
         except Exception as unexpected_error:
             error_message = f"Unexpected error occurred while data update : \033[31m{unexpected_error}\033[0m\n{traceback.format_exc()}\n"
             logger.error(error_message)
             error_json = {"reason": f"Unexpected error occurred while data update: {unexpected_error}"}
-            self.agent.update_error(output=error_json)
+            self.update_agent.validate_error(output=error_json, alert=self.alert)
+            self.update_agent.close()
+
             return
+        finally:
+            self.wait_flag = True
         
-        self.agent.update_complete(alert=False) # alert_data_update 채널에 알람 보내기
+        self.update_agent.validate(
+            output = data_update_result.output_json,
+            usage = data_update_result.usage,
+            alert = self.alert
+        )
+        self.update_agent.close()
 
     def run(self):
         self._pipeline()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dalpha-0.5.5/dalpha/dto.py` & `dalpha-0.5.5rc0/dalpha/dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,7 +15,25 @@
             error_message = f"Expected TypeError occured. \033[31moutput_json should be dictionary type\033[31m\n"
             logger.error(error_message)
             error_json = {"reason": f"TypeError; output_json should be dictionary type"}
             raise ExpectedError(error_json=error_json)
 
         self.usage = usage
         self.output_json = output_json
+
+class UpdateResult:
+    def __init__(self, usage: int, output_json: dict) -> None:
+        # validation
+        if not isinstance(usage, int) or usage <= 0:
+            error_message = f"Expected TypeError occured. \033[31musage should be positive integer\033[0m\n"
+            logger.error(error_message)
+            error_json = {"reason": f"TypeError; usage should be positive integer"}
+            raise ExpectedError(error_json=error_json)
+
+        if not isinstance(output_json, dict):
+            error_message = f"Expected TypeError occured. \033[31moutput_json should be dictionary type\033[31m\n"
+            logger.error(error_message)
+            error_json = {"reason": f"TypeError; output_json should be dictionary type"}
+            raise ExpectedError(error_json=error_json)
+
+        self.usage = usage
+        self.output_json = output_json
```

### Comparing `dalpha-0.5.5/dalpha/exception.py` & `dalpha-0.5.5rc0/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/inference_cls.py` & `dalpha-0.5.5rc0/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/logging/__init__.py` & `dalpha-0.5.5rc0/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/logging/log_formatter.py` & `dalpha-0.5.5rc0/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/logging/utils.py` & `dalpha-0.5.5rc0/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/message_consumer.py` & `dalpha-0.5.5rc0/dalpha/message_consumer.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/openai_cls.py` & `dalpha-0.5.5rc0/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/redis_cli.py` & `dalpha-0.5.5rc0/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/redis_cls.py` & `dalpha-0.5.5rc0/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/request.py` & `dalpha-0.5.5rc0/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/dalpha/s3.py` & `dalpha-0.5.5rc0/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.5/PKG-INFO` & `dalpha-0.5.5rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.5
+Version: 0.5.5rc0
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


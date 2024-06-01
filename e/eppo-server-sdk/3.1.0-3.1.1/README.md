# Comparing `tmp/eppo_server_sdk-3.1.0.tar.gz` & `tmp/eppo_server_sdk-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo_server_sdk-3.1.0.tar", last modified: Thu May 30 05:18:42 2024, max compression
+gzip compressed data, was "eppo_server_sdk-3.1.1.tar", last modified: Sat Jun  1 01:55:12 2024, max compression
```

## Comparing `eppo_server_sdk-3.1.0.tar` & `eppo_server_sdk-3.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:18:42.890961 eppo_server_sdk-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-30 05:18:42.886961 eppo_server_sdk-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:18:42.886961 eppo_server_sdk-3.1.0/eppo_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/assignment_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/configuration_requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/configuration_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/read_write_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/sharders.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/eppo_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 05:18:42.886961 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 05:18:42.000000 eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-30 05:18:39.000000 eppo_server_sdk-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-30 05:18:42.890961 eppo_server_sdk-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:55:12.238076 eppo_server_sdk-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-06-01 01:55:12.238076 eppo_server_sdk-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:55:12.234076 eppo_server_sdk-3.1.1/eppo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/assignment_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/configuration_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/configuration_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/read_write_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/sharders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/eppo_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:55:12.238076 eppo_server_sdk-3.1.1/eppo_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-06-01 01:55:12.000000 eppo_server_sdk-3.1.1/eppo_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-06-01 01:55:12.000000 eppo_server_sdk-3.1.1/eppo_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:55:12.000000 eppo_server_sdk-3.1.1/eppo_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 01:55:12.000000 eppo_server_sdk-3.1.1/eppo_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 01:55:12.000000 eppo_server_sdk-3.1.1/eppo_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-01 01:55:08.000000 eppo_server_sdk-3.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-01 01:55:12.238076 eppo_server_sdk-3.1.1/setup.cfg
```

### Comparing `eppo_server_sdk-3.1.0/LICENSE` & `eppo_server_sdk-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/PKG-INFO` & `eppo_server_sdk-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 3.1.0
+Version: 3.1.1
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo_server_sdk-3.1.0/README.md` & `eppo_server_sdk-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/__init__.py` & `eppo_server_sdk-3.1.1/eppo_client/__init__.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/bandit.py` & `eppo_server_sdk-3.1.1/eppo_client/bandit.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/client.py` & `eppo_server_sdk-3.1.1/eppo_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             logger.error("[Eppo SDK] Error logging assignment event: " + str(e))
         return result
 
     def get_bandit_action(
         self,
         flag_key: str,
         subject_key: str,
-        subject_attributes: Attributes,
+        subject_context: Attributes,
         actions_with_contexts: List[ActionContext],
         default: str,
     ) -> BanditResult:
         """
         Determines the bandit action for a given subject based on the provided bandit key and subject attributes.
 
         This method performs the following steps:
@@ -240,49 +240,49 @@
         4. Evaluates the bandit action using the bandit evaluator.
         5. Logs the bandit action event.
         6. Returns the BanditResult containing the selected action key and the assignment.
 
         Args:
             flag_key (str): The feature flag key that contains the bandit as one of the variations.
             subject_key (str): The key identifying the subject.
-            subject_attributes (Attributes): The attributes of the subject.
+            subject_context (Attributes): The subject context
             actions_with_contexts (List[ActionContext]): The list of actions with their contexts.
 
         Returns:
             BanditResult: The result containing either the bandit action if the subject is part of the bandit,
                           or the assignment if they are not. The BanditResult includes:
                           - variation (str): The assignment key indicating the subject's variation.
                           - action (str): The key of the selected action if the subject is part of the bandit.
         """
         try:
             return self.get_bandit_action_detail(
                 flag_key,
                 subject_key,
-                subject_attributes,
+                subject_context,
                 actions_with_contexts,
                 default,
             )
         except Exception as e:
             if self.__is_graceful_mode:
                 logger.error("[Eppo SDK] Error getting bandit action: " + str(e))
                 return BanditResult(default, None)
             raise e
 
     def get_bandit_action_detail(
         self,
         flag_key: str,
         subject_key: str,
-        subject_attributes: Attributes,
+        subject_context: Attributes,
         actions_with_contexts: List[ActionContext],
         default: str,
     ) -> BanditResult:
         # get experiment assignment
         # ignoring type because Dict[str, str] satisfies Dict[str, str | ...] but mypy does not understand
         variation = self.get_string_assignment(
-            flag_key, subject_key, subject_attributes.categorical_attributes, default  # type: ignore
+            flag_key, subject_key, subject_context.categorical_attributes, default  # type: ignore
         )
 
         # if the variation is not the bandit key, then the subject is not allocated in the bandit
         if variation not in self.get_bandit_keys():
             return BanditResult(variation, None)
 
         # for now, assume that the variation is equal to the bandit key
@@ -293,35 +293,35 @@
                 f"[Eppo SDK] No assigned action. Bandit not found for flag: {flag_key}"
             )
             return BanditResult(variation, None)
 
         evaluation = self.__bandit_evaluator.evaluate_bandit(
             flag_key,
             subject_key,
-            subject_attributes,
+            subject_context,
             actions_with_contexts,
             bandit_data.model_data,
         )
 
         # log bandit action
         bandit_event = {
             "flagKey": flag_key,
             "banditKey": bandit_data.bandit_key,
             "subject": subject_key,
             "action": evaluation.action_key if evaluation else None,
             "actionProbability": evaluation.action_weight if evaluation else None,
             "modelVersion": bandit_data.model_version if evaluation else None,
             "timestamp": datetime.datetime.utcnow().isoformat(),
             "subjectNumericAttributes": (
-                subject_attributes.numeric_attributes
+                subject_context.numeric_attributes
                 if evaluation.subject_attributes
                 else {}
             ),
             "subjectCategoricalAttributes": (
-                subject_attributes.categorical_attributes
+                subject_context.categorical_attributes
                 if evaluation.subject_attributes
                 else {}
             ),
             "actionNumericAttributes": (
                 evaluation.action_attributes.numeric_attributes
                 if evaluation.action_attributes
                 else {}
```

### Comparing `eppo_server_sdk-3.1.0/eppo_client/configuration_requestor.py` & `eppo_server_sdk-3.1.1/eppo_client/configuration_requestor.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/configuration_store.py` & `eppo_server_sdk-3.1.1/eppo_client/configuration_store.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/eval.py` & `eppo_server_sdk-3.1.1/eppo_client/eval.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/http_client.py` & `eppo_server_sdk-3.1.1/eppo_client/http_client.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/models.py` & `eppo_server_sdk-3.1.1/eppo_client/models.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/poller.py` & `eppo_server_sdk-3.1.1/eppo_client/poller.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/read_write_lock.py` & `eppo_server_sdk-3.1.1/eppo_client/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/rules.py` & `eppo_server_sdk-3.1.1/eppo_client/rules.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_client/sharders.py` & `eppo_server_sdk-3.1.1/eppo_client/sharders.py`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/PKG-INFO` & `eppo_server_sdk-3.1.1/eppo_server_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 3.1.0
+Version: 3.1.1
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo_server_sdk-3.1.0/eppo_server_sdk.egg-info/SOURCES.txt` & `eppo_server_sdk-3.1.1/eppo_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eppo_server_sdk-3.1.0/setup.cfg` & `eppo_server_sdk-3.1.1/setup.cfg`

 * *Files identical despite different names*


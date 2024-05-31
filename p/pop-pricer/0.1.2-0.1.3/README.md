# Comparing `tmp/pop_pricer-0.1.2.tar.gz` & `tmp/pop_pricer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop_pricer-0.1.2.tar", max compression
+gzip compressed data, was "pop_pricer-0.1.3.tar", max compression
```

## Comparing `pop_pricer-0.1.2.tar` & `pop_pricer-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34522 2024-05-29 16:55:10.865652 pop_pricer-0.1.2/LICENSE.md
--rw-r--r--   0        0        0       90 2024-05-29 17:14:35.796179 pop_pricer-0.1.2/README.md
--rw-r--r--   0        0        0      138 2024-05-31 17:16:57.938928 pop_pricer-0.1.2/pop_pricer/__init__.py
--rw-r--r--   0        0        0     2381 2024-05-31 20:45:15.301287 pop_pricer-0.1.2/pop_pricer/pricer.py
--rw-r--r--   0        0        0      360 2024-05-31 20:46:54.755751 pop_pricer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 pop_pricer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-05-29 16:55:10.865652 pop_pricer-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0       90 2024-05-29 17:14:35.796179 pop_pricer-0.1.3/README.md
+-rw-r--r--   0        0        0      138 2024-05-31 21:18:14.018828 pop_pricer-0.1.3/pop_pricer/__init__.py
+-rw-r--r--   0        0        0     2474 2024-05-31 21:11:23.283341 pop_pricer-0.1.3/pop_pricer/pricer.py
+-rw-r--r--   0        0        0      360 2024-05-31 21:18:27.936411 pop_pricer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 pop_pricer-0.1.3/PKG-INFO
```

### Comparing `pop_pricer-0.1.2/LICENSE.md` & `pop_pricer-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pop_pricer-0.1.2/pop_pricer/pricer.py` & `pop_pricer-0.1.3/pop_pricer/pricer.py`

 * *Files 15% similar despite different names*

```diff
@@ -73,11 +73,12 @@
       return json.dumps(data)
 
     @staticmethod
     def deserialize(str):
       try:
         data = json.loads(str)
         p = Pricer(data['_start_price'], data['_max_price'], data['_reset_rate'], data['_cost_weight'])
-        p._last_cost = data['_last_cost']
+        p._last_cost = data['_last_cost'] and datetime.fromisoformat(data['_last_cost'])
         p._cost = data['_cost']
-      except:
+        return p
+      except json.decoder.JSONDecodeError:
         return None
```

### Comparing `pop_pricer-0.1.2/PKG-INFO` & `pop_pricer-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-pricer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dynamic Pricing Algorithm
 License: AGPL-3.0-only
 Author: David LoBosco
 Author-email: 5651124+dqlobo@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```


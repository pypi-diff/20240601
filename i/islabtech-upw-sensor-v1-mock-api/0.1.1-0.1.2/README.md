# Comparing `tmp/islabtech_upw_sensor_v1_mock_api-0.1.1.tar.gz` & `tmp/islabtech_upw_sensor_v1_mock_api-0.1.2.tar.gz`

## Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1.tar` & `islabtech_upw_sensor_v1_mock_api-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/conftest.py
--rw-r--r--   0        0        0    67870 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/modbus-doc.pdf
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/modbus-doc.tex
--rw-r--r--   0        0        0    27510 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/openapi.yml
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/guides/measure.md
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/guides/system.md
--rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/guides/temperature calibration.md
--rw-r--r--   0        0        0    28028 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/islabtech_upw_sensor_v1_mock_api/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/islabtech_upw_sensor_v1_mock_api/__main__.py
--rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/islabtech_upw_sensor_v1_mock_api/tests/test_modbus.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/islabtech_upw_sensor_v1_mock_api/tests/test_units.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/.gitignore
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/README.md
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/conftest.py
+-rw-r--r--   0        0        0    67870 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/modbus-doc.pdf
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/modbus-doc.tex
+-rw-r--r--   0        0        0    27510 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/openapi.yml
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/guides/measure.md
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/guides/system.md
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/guides/temperature calibration.md
+-rw-r--r--   0        0        0    28028 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/islabtech_upw_sensor_v1_mock_api/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/islabtech_upw_sensor_v1_mock_api/__main__.py
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/islabtech_upw_sensor_v1_mock_api/tests/test_modbus.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/islabtech_upw_sensor_v1_mock_api/tests/test_units.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/README.md
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 islabtech_upw_sensor_v1_mock_api-0.1.2/PKG-INFO
```

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/.gitlab-ci.yml` & `islabtech_upw_sensor_v1_mock_api-0.1.2/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         - pip3 install pytest
         - pytest -v .
     # TODO: capture test results in GitLab
 
 test-version-consistency:
     stage: test
     image: debian:stable-slim
+    needs: []
     rules:
         - if: $CI_COMMIT_TAG
     script:
         - test "$CI_COMMIT_TAG"  = v"$(sed -n 's/^ *version *= *"\(.*\)" *$/\1/p' pyproject.toml)"
 
 publish:
     image: python:3
```

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/conftest.py` & `islabtech_upw_sensor_v1_mock_api-0.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/modbus-doc.pdf` & `islabtech_upw_sensor_v1_mock_api-0.1.2/modbus-doc.pdf`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/modbus-doc.tex` & `islabtech_upw_sensor_v1_mock_api-0.1.2/modbus-doc.tex`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/openapi.yml` & `islabtech_upw_sensor_v1_mock_api-0.1.2/openapi.yml`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/guides/measure.md` & `islabtech_upw_sensor_v1_mock_api-0.1.2/guides/measure.md`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/guides/system.md` & `islabtech_upw_sensor_v1_mock_api-0.1.2/guides/system.md`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/guides/temperature calibration.md` & `islabtech_upw_sensor_v1_mock_api-0.1.2/guides/temperature calibration.md`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/islabtech_upw_sensor_v1_mock_api/__init__.py` & `islabtech_upw_sensor_v1_mock_api-0.1.2/islabtech_upw_sensor_v1_mock_api/__init__.py`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/islabtech_upw_sensor_v1_mock_api/tests/test_modbus.py` & `islabtech_upw_sensor_v1_mock_api-0.1.2/islabtech_upw_sensor_v1_mock_api/tests/test_modbus.py`

 * *Files identical despite different names*

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/README.md` & `islabtech_upw_sensor_v1_mock_api-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## REST API
 [The entire REST API is documented in OpenAPI/Swagger.](openapi.yml).
 
 ## Modbus/TCP
 [The Modbus/TCP interface is documented in this PDF.](modbus-doc.pdf)
 
-## :snake: Mock API
+## 🐍 Mock API
 
 Run the mock API locally with Python:
 
 ```sh
 pip3 install islabtech_upw_sensor_v1_mock_api
 python3 -m islabtech_upw_sensor_v1_mock_api
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/pyproject.toml` & `islabtech_upw_sensor_v1_mock_api-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "islabtech_upw_sensor_v1_mock_api"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Ilka Schulz", email = "ilka@islabtech.com" }]
 description = "Mock API simulating the Rest+Modbus/TCP API of the ISLabTech UPW sensor"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Natural Language :: English",
```

### Comparing `islabtech_upw_sensor_v1_mock_api-0.1.1/PKG-INFO` & `islabtech_upw_sensor_v1_mock_api-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: islabtech_upw_sensor_v1_mock_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mock API simulating the Rest+Modbus/TCP API of the ISLabTech UPW sensor
 Project-URL: Bug Tracker, https://gitlab.com/islabtech/upw-sensor/api
 Author-email: Ilka Schulz <ilka@islabtech.com>
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
@@ -22,15 +22,15 @@
 
 ## REST API
 [The entire REST API is documented in OpenAPI/Swagger.](openapi.yml).
 
 ## Modbus/TCP
 [The Modbus/TCP interface is documented in this PDF.](modbus-doc.pdf)
 
-## :snake: Mock API
+## 🐍 Mock API
 
 Run the mock API locally with Python:
 
 ```sh
 pip3 install islabtech_upw_sensor_v1_mock_api
 python3 -m islabtech_upw_sensor_v1_mock_api
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


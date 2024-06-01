# Comparing `tmp/espy_pay-1.0.0.tar.gz` & `tmp/espy_pay-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_pay-1.0.0.tar", last modified: Sat Jun  1 01:59:47 2024, max compression
+gzip compressed data, was "espy_pay-1.0.1.tar", last modified: Sat Jun  1 07:01:44 2024, max compression
```

## Comparing `espy_pay-1.0.0.tar` & `espy_pay-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,41 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.537134 espy_pay-1.0.0/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-30 14:26:42.000000 espy_pay-1.0.0/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      533 2024-06-01 01:59:47.536945 espy_pay-1.0.0/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      119 2024-05-31 23:52:39.000000 espy_pay-1.0.0/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.527861 espy_pay-1.0.0/espy_pay/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:33:17.000000 espy_pay-1.0.0/espy_pay/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.531290 espy_pay-1.0.0/espy_pay/general/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-05-31 23:59:43.000000 espy_pay-1.0.0/espy_pay/general/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 15:06:04.000000 espy_pay-1.0.0/espy_pay/general/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-30 16:03:25.000000 espy_pay-1.0.0/espy_pay/general/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:42.000000 espy_pay-1.0.0/espy_pay/general/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:46.000000 espy_pay-1.0.0/espy_pay/general/model.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-30 15:09:25.000000 espy_pay-1.0.0/espy_pay/general/pg.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:50.000000 espy_pay-1.0.0/espy_pay/general/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:53.000000 espy_pay-1.0.0/espy_pay/general/util.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.531655 espy_pay-1.0.0/espy_pay/ng/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:35:16.000000 espy_pay-1.0.0/espy_pay/ng/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.531810 espy_pay-1.0.0/espy_pay/ng/paystack/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:37:46.000000 espy_pay-1.0.0/espy_pay/ng/paystack/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.532048 espy_pay-1.0.0/espy_pay/ng/paystack/schema/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:37:07.000000 espy_pay-1.0.0/espy_pay/ng/paystack/schema/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2033 2024-06-01 01:45:37.000000 espy_pay-1.0.0/espy_pay/ng/paystack/schema/schema.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.532573 espy_pay-1.0.0/espy_pay/ng/paystack/service/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 16:42:58.000000 espy_pay-1.0.0/espy_pay/ng/paystack/service/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3271 2024-05-31 23:46:54.000000 espy_pay-1.0.0/espy_pay/ng/paystack/service/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.535374 espy_pay-1.0.0/espy_pay/ng/paystack/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)     6430 2024-05-31 23:11:47.000000 espy_pay-1.0.0/espy_pay/ng/paystack/util/Bankcodes.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1062 2024-06-01 01:51:32.000000 espy_pay-1.0.0/espy_pay/ng/paystack/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 16:45:32.000000 espy_pay-1.0.0/espy_pay/ng/paystack/util/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.535499 espy_pay-1.0.0/espy_pay/us/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:35:42.000000 espy_pay-1.0.0/espy_pay/us/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.535613 espy_pay-1.0.0/espy_pay/us/stripe/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:36:34.000000 espy_pay-1.0.0/espy_pay/us/stripe/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.528674 espy_pay-1.0.0/espy_pay.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      533 2024-06-01 01:59:47.000000 espy_pay-1.0.0/espy_pay.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      860 2024-06-01 01:59:47.000000 espy_pay-1.0.0/espy_pay.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-06-01 01:59:47.000000 espy_pay-1.0.0/espy_pay.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)      115 2024-06-01 01:59:47.000000 espy_pay-1.0.0/espy_pay.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       15 2024-06-01 01:59:47.000000 espy_pay-1.0.0/espy_pay.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-06-01 01:59:47.537199 espy_pay-1.0.0/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      921 2024-06-01 01:59:44.000000 espy_pay-1.0.0/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 01:59:47.536325 espy_pay-1.0.0/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-31 22:58:06.000000 espy_pay-1.0.0/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      110 2024-05-31 19:50:27.000000 espy_pay-1.0.0/tests/config.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1483 2024-05-31 23:02:11.000000 espy_pay-1.0.0/tests/test_copyright.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.654873 espy_pay-1.0.1/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-30 14:26:42.000000 espy_pay-1.0.1/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      533 2024-06-01 07:01:44.654657 espy_pay-1.0.1/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      119 2024-05-31 23:52:39.000000 espy_pay-1.0.1/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.646791 espy_pay-1.0.1/espy_pay/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:33:17.000000 espy_pay-1.0.1/espy_pay/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.650256 espy_pay-1.0.1/espy_pay/general/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-05-31 23:59:43.000000 espy_pay-1.0.1/espy_pay/general/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 15:06:04.000000 espy_pay-1.0.1/espy_pay/general/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-30 16:03:25.000000 espy_pay-1.0.1/espy_pay/general/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:42.000000 espy_pay-1.0.1/espy_pay/general/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:46.000000 espy_pay-1.0.1/espy_pay/general/model.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-30 15:09:25.000000 espy_pay-1.0.1/espy_pay/general/pg.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:50.000000 espy_pay-1.0.1/espy_pay/general/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:53.000000 espy_pay-1.0.1/espy_pay/general/util.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.650704 espy_pay-1.0.1/espy_pay/ng/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:35:16.000000 espy_pay-1.0.1/espy_pay/ng/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.651335 espy_pay-1.0.1/espy_pay/ng/paystack/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:37:46.000000 espy_pay-1.0.1/espy_pay/ng/paystack/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2033 2024-06-01 01:45:37.000000 espy_pay-1.0.1/espy_pay/ng/paystack/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3263 2024-06-01 06:58:02.000000 espy_pay-1.0.1/espy_pay/ng/paystack/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.652597 espy_pay-1.0.1/espy_pay/ng/paystack/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     6430 2024-05-31 23:11:47.000000 espy_pay-1.0.1/espy_pay/ng/paystack/util/Bankcodes.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1062 2024-06-01 01:51:32.000000 espy_pay-1.0.1/espy_pay/ng/paystack/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 16:45:32.000000 espy_pay-1.0.1/espy_pay/ng/paystack/util/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.652837 espy_pay-1.0.1/espy_pay/us/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:35:42.000000 espy_pay-1.0.1/espy_pay/us/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.652957 espy_pay-1.0.1/espy_pay/us/stripe/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:36:34.000000 espy_pay-1.0.1/espy_pay/us/stripe/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.647495 espy_pay-1.0.1/espy_pay.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      533 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      764 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)      115 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       15 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-06-01 07:01:44.654927 espy_pay-1.0.1/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      921 2024-06-01 07:00:46.000000 espy_pay-1.0.1/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.654141 espy_pay-1.0.1/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-31 22:58:06.000000 espy_pay-1.0.1/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      110 2024-05-31 19:50:27.000000 espy_pay-1.0.1/tests/config.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1483 2024-05-31 23:02:11.000000 espy_pay-1.0.1/tests/test_copyright.py
```

### Comparing `espy_pay-1.0.0/LICENSE` & `espy_pay-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/PKG-INFO` & `espy_pay-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espy_pay
-Version: 1.0.0
+Version: 1.0.1
 Summary: Payment services aggregator for ESSL
 Home-page: UNKNOWN
 Author: Femi Adigun
 Author-email: femi.adigun@myeverlasting.net
 License: UNKNOWN
 Keywords: payment, essl, aggregator, paystack, stripe, interswitch, square, flutterwave, payant
 Platform: UNKNOWN
```

### Comparing `espy_pay-1.0.0/espy_pay/general/CONSTANTS.py` & `espy_pay-1.0.1/espy_pay/general/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/general/db.py` & `espy_pay-1.0.1/espy_pay/general/db.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/general/enums.py` & `espy_pay-1.0.1/espy_pay/general/enums.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/general/model.py` & `espy_pay-1.0.1/espy_pay/general/model.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/general/pg.py` & `espy_pay-1.0.1/espy_pay/general/pg.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/general/schema.py` & `espy_pay-1.0.1/espy_pay/general/schema.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/general/util.py` & `espy_pay-1.0.1/espy_pay/general/util.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/ng/paystack/schema/schema.py` & `espy_pay-1.0.1/espy_pay/ng/paystack/schema.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/ng/paystack/service/service.py` & `espy_pay-1.0.1/espy_pay/ng/paystack/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 office@myeverlasting.net
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 import requests
 from espy_pay.ng.paystack.util import CONSTANTS
-from espy_pay.ng.paystack.schema.schema import TranxRequest, Subaccount_Request
+from espy_pay.ng.paystack.schema import TranxRequest, Subaccount_Request
 
 def init_tranx(data: TranxRequest):
     url = f"{CONSTANTS.PAYSTACK_URL}initialize"
     data = {
         "email": data.email,
         "amount": data.amount
     }
     headers = {
         "Authorization": CONSTANTS.AUTH,
         "Content-Type": "application/json"
     }
-    response = requests.post(url, json=data, headers=headers)
+    response = requests.get(url, json=data, headers=headers)
     return response.json()
 def verify_tranx(reference: str):
     url = f"{CONSTANTS.PAYSTACK_URL}verify/{reference}"
     headers = {
         "Authorization": CONSTANTS.AUTH
     }
     response = requests.get(url, headers=headers)
```

### Comparing `espy_pay-1.0.0/espy_pay/ng/paystack/util/Bankcodes.py` & `espy_pay-1.0.1/espy_pay/ng/paystack/util/Bankcodes.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay/ng/paystack/util/CONSTANTS.py` & `espy_pay-1.0.1/espy_pay/ng/paystack/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.0/espy_pay.egg-info/PKG-INFO` & `espy_pay-1.0.1/espy_pay.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espy-pay
-Version: 1.0.0
+Version: 1.0.1
 Summary: Payment services aggregator for ESSL
 Home-page: UNKNOWN
 Author: Femi Adigun
 Author-email: femi.adigun@myeverlasting.net
 License: UNKNOWN
 Keywords: payment, essl, aggregator, paystack, stripe, interswitch, square, flutterwave, payant
 Platform: UNKNOWN
```

### Comparing `espy_pay-1.0.0/espy_pay.egg-info/SOURCES.txt` & `espy_pay-1.0.1/espy_pay.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,18 +13,16 @@
 espy_pay/general/enums.py
 espy_pay/general/model.py
 espy_pay/general/pg.py
 espy_pay/general/schema.py
 espy_pay/general/util.py
 espy_pay/ng/__init__.py
 espy_pay/ng/paystack/__init__.py
-espy_pay/ng/paystack/schema/__init__.py
-espy_pay/ng/paystack/schema/schema.py
-espy_pay/ng/paystack/service/__init__.py
-espy_pay/ng/paystack/service/service.py
+espy_pay/ng/paystack/schema.py
+espy_pay/ng/paystack/service.py
 espy_pay/ng/paystack/util/Bankcodes.py
 espy_pay/ng/paystack/util/CONSTANTS.py
 espy_pay/ng/paystack/util/__init__.py
 espy_pay/us/__init__.py
 espy_pay/us/stripe/__init__.py
 tests/__init__.py
 tests/config.py
```

### Comparing `espy_pay-1.0.0/setup.py` & `espy_pay-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 VERSION = '0.0.1'
 DESCRIPTION = 'ESSL Payments Aggregator'
 LONG_DESCRIPTION = 'Internal helper package for ESSL online payment'
 setup(
     name='espy_pay',
-    version='1.0.0',
+    version='1.0.1',
     author='Femi Adigun',
     author_email='femi.adigun@myeverlasting.net',
     description='Payment services aggregator for ESSL',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
```

### Comparing `espy_pay-1.0.0/tests/test_copyright.py` & `espy_pay-1.0.1/tests/test_copyright.py`

 * *Files identical despite different names*


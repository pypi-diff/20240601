# Comparing `tmp/espy_pay-1.0.1.tar.gz` & `tmp/espy_pay-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_pay-1.0.1.tar", last modified: Sat Jun  1 07:01:44 2024, max compression
+gzip compressed data, was "espy_pay-1.0.2.tar", last modified: Sat Jun  1 08:28:03 2024, max compression
```

## Comparing `espy_pay-1.0.1.tar` & `espy_pay-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.654873 espy_pay-1.0.1/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-30 14:26:42.000000 espy_pay-1.0.1/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      533 2024-06-01 07:01:44.654657 espy_pay-1.0.1/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      119 2024-05-31 23:52:39.000000 espy_pay-1.0.1/README.md
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.646791 espy_pay-1.0.1/espy_pay/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:33:17.000000 espy_pay-1.0.1/espy_pay/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.650256 espy_pay-1.0.1/espy_pay/general/
--rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-05-31 23:59:43.000000 espy_pay-1.0.1/espy_pay/general/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 15:06:04.000000 espy_pay-1.0.1/espy_pay/general/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-30 16:03:25.000000 espy_pay-1.0.1/espy_pay/general/db.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:42.000000 espy_pay-1.0.1/espy_pay/general/enums.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:46.000000 espy_pay-1.0.1/espy_pay/general/model.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-30 15:09:25.000000 espy_pay-1.0.1/espy_pay/general/pg.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:50.000000 espy_pay-1.0.1/espy_pay/general/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:53.000000 espy_pay-1.0.1/espy_pay/general/util.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.650704 espy_pay-1.0.1/espy_pay/ng/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:35:16.000000 espy_pay-1.0.1/espy_pay/ng/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.651335 espy_pay-1.0.1/espy_pay/ng/paystack/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:37:46.000000 espy_pay-1.0.1/espy_pay/ng/paystack/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     2033 2024-06-01 01:45:37.000000 espy_pay-1.0.1/espy_pay/ng/paystack/schema.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     3263 2024-06-01 06:58:02.000000 espy_pay-1.0.1/espy_pay/ng/paystack/service.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.652597 espy_pay-1.0.1/espy_pay/ng/paystack/util/
--rw-r--r--   0 philipadigun   (501) staff       (20)     6430 2024-05-31 23:11:47.000000 espy_pay-1.0.1/espy_pay/ng/paystack/util/Bankcodes.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1062 2024-06-01 01:51:32.000000 espy_pay-1.0.1/espy_pay/ng/paystack/util/CONSTANTS.py
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 16:45:32.000000 espy_pay-1.0.1/espy_pay/ng/paystack/util/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.652837 espy_pay-1.0.1/espy_pay/us/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:35:42.000000 espy_pay-1.0.1/espy_pay/us/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.652957 espy_pay-1.0.1/espy_pay/us/stripe/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:36:34.000000 espy_pay-1.0.1/espy_pay/us/stripe/__init__.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.647495 espy_pay-1.0.1/espy_pay.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      533 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      764 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)      115 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       15 2024-06-01 07:01:44.000000 espy_pay-1.0.1/espy_pay.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-06-01 07:01:44.654927 espy_pay-1.0.1/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      921 2024-06-01 07:00:46.000000 espy_pay-1.0.1/setup.py
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 07:01:44.654141 espy_pay-1.0.1/tests/
--rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-31 22:58:06.000000 espy_pay-1.0.1/tests/__init__.py
--rw-r--r--   0 philipadigun   (501) staff       (20)      110 2024-05-31 19:50:27.000000 espy_pay-1.0.1/tests/config.py
--rw-r--r--   0 philipadigun   (501) staff       (20)     1483 2024-05-31 23:02:11.000000 espy_pay-1.0.1/tests/test_copyright.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.583331 espy_pay-1.0.2/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-30 14:26:42.000000 espy_pay-1.0.2/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      533 2024-06-01 08:28:03.583177 espy_pay-1.0.2/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      119 2024-05-31 23:52:39.000000 espy_pay-1.0.2/README.md
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.577190 espy_pay-1.0.2/espy_pay/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:33:17.000000 espy_pay-1.0.2/espy_pay/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.580165 espy_pay-1.0.2/espy_pay/general/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      959 2024-05-31 23:59:43.000000 espy_pay-1.0.2/espy_pay/general/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 15:06:04.000000 espy_pay-1.0.2/espy_pay/general/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1055 2024-05-30 16:03:25.000000 espy_pay-1.0.2/espy_pay/general/db.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:42.000000 espy_pay-1.0.2/espy_pay/general/enums.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:46.000000 espy_pay-1.0.2/espy_pay/general/model.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     4353 2024-05-30 15:09:25.000000 espy_pay-1.0.2/espy_pay/general/pg.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:50.000000 espy_pay-1.0.2/espy_pay/general/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      870 2024-05-30 15:09:53.000000 espy_pay-1.0.2/espy_pay/general/util.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.580421 espy_pay-1.0.2/espy_pay/ng/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:35:16.000000 espy_pay-1.0.2/espy_pay/ng/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.580947 espy_pay-1.0.2/espy_pay/ng/paystack/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:37:46.000000 espy_pay-1.0.2/espy_pay/ng/paystack/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2033 2024-06-01 08:27:33.000000 espy_pay-1.0.2/espy_pay/ng/paystack/schema.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     3263 2024-06-01 06:58:02.000000 espy_pay-1.0.2/espy_pay/ng/paystack/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.582018 espy_pay-1.0.2/espy_pay/ng/paystack/util/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     6430 2024-05-31 23:11:47.000000 espy_pay-1.0.2/espy_pay/ng/paystack/util/Bankcodes.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1062 2024-06-01 01:51:32.000000 espy_pay-1.0.2/espy_pay/ng/paystack/util/CONSTANTS.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 16:45:32.000000 espy_pay-1.0.2/espy_pay/ng/paystack/util/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.582138 espy_pay-1.0.2/espy_pay/us/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:35:42.000000 espy_pay-1.0.2/espy_pay/us/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.582256 espy_pay-1.0.2/espy_pay/us/stripe/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-30 14:36:34.000000 espy_pay-1.0.2/espy_pay/us/stripe/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.577850 espy_pay-1.0.2/espy_pay.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      533 2024-06-01 08:28:03.000000 espy_pay-1.0.2/espy_pay.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      764 2024-06-01 08:28:03.000000 espy_pay-1.0.2/espy_pay.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-06-01 08:28:03.000000 espy_pay-1.0.2/espy_pay.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)      115 2024-06-01 08:28:03.000000 espy_pay-1.0.2/espy_pay.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       15 2024-06-01 08:28:03.000000 espy_pay-1.0.2/espy_pay.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-06-01 08:28:03.583389 espy_pay-1.0.2/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      921 2024-06-01 08:27:57.000000 espy_pay-1.0.2/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-06-01 08:28:03.582846 espy_pay-1.0.2/tests/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-31 22:58:06.000000 espy_pay-1.0.2/tests/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)      110 2024-05-31 19:50:27.000000 espy_pay-1.0.2/tests/config.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1483 2024-05-31 23:02:11.000000 espy_pay-1.0.2/tests/test_copyright.py
```

### Comparing `espy_pay-1.0.1/LICENSE` & `espy_pay-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/PKG-INFO` & `espy_pay-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espy_pay
-Version: 1.0.1
+Version: 1.0.2
 Summary: Payment services aggregator for ESSL
 Home-page: UNKNOWN
 Author: Femi Adigun
 Author-email: femi.adigun@myeverlasting.net
 License: UNKNOWN
 Keywords: payment, essl, aggregator, paystack, stripe, interswitch, square, flutterwave, payant
 Platform: UNKNOWN
```

### Comparing `espy_pay-1.0.1/espy_pay/general/CONSTANTS.py` & `espy_pay-1.0.2/espy_pay/general/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/general/db.py` & `espy_pay-1.0.2/espy_pay/general/db.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/general/enums.py` & `espy_pay-1.0.2/espy_pay/general/enums.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/general/model.py` & `espy_pay-1.0.2/espy_pay/general/model.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/general/pg.py` & `espy_pay-1.0.2/espy_pay/general/pg.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/general/schema.py` & `espy_pay-1.0.2/espy_pay/general/schema.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/general/util.py` & `espy_pay-1.0.2/espy_pay/general/util.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/ng/paystack/schema.py` & `espy_pay-1.0.2/espy_pay/ng/paystack/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     status: bool
     message: str
     data: object
 class TranxRequest(BaseModel):
     email: EmailStr
     amount: int = Field(..., gt=2500, description="Amount must be greater than 2500 kobo")
     authorization_code: Optional[str] = None
-    reference: Optional[str] = None
+    reference: Optional[int] = None
     currency: Optional[str] = None
     callback_url: Optional[AnyHttpUrl] = None
 class Subaccount(BaseModel):
     subaccount: str = Field(..., min_length=5, description="Subaccount charged code from Paystack")
     share: int
 class SplitRequest(BaseModel):
     name: str
```

### Comparing `espy_pay-1.0.1/espy_pay/ng/paystack/service.py` & `espy_pay-1.0.2/espy_pay/ng/paystack/service.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/ng/paystack/util/Bankcodes.py` & `espy_pay-1.0.2/espy_pay/ng/paystack/util/Bankcodes.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay/ng/paystack/util/CONSTANTS.py` & `espy_pay-1.0.2/espy_pay/ng/paystack/util/CONSTANTS.py`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/espy_pay.egg-info/PKG-INFO` & `espy_pay-1.0.2/espy_pay.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espy-pay
-Version: 1.0.1
+Version: 1.0.2
 Summary: Payment services aggregator for ESSL
 Home-page: UNKNOWN
 Author: Femi Adigun
 Author-email: femi.adigun@myeverlasting.net
 License: UNKNOWN
 Keywords: payment, essl, aggregator, paystack, stripe, interswitch, square, flutterwave, payant
 Platform: UNKNOWN
```

### Comparing `espy_pay-1.0.1/espy_pay.egg-info/SOURCES.txt` & `espy_pay-1.0.2/espy_pay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `espy_pay-1.0.1/setup.py` & `espy_pay-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 VERSION = '0.0.1'
 DESCRIPTION = 'ESSL Payments Aggregator'
 LONG_DESCRIPTION = 'Internal helper package for ESSL online payment'
 setup(
     name='espy_pay',
-    version='1.0.1',
+    version='1.0.2',
     author='Femi Adigun',
     author_email='femi.adigun@myeverlasting.net',
     description='Payment services aggregator for ESSL',
     packages=find_packages(),
     install_requires=[
         'bcrypt==4.1.2',
         'pytest==8.1.1',
```

### Comparing `espy_pay-1.0.1/tests/test_copyright.py` & `espy_pay-1.0.2/tests/test_copyright.py`

 * *Files identical despite different names*


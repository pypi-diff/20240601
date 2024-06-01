# Comparing `tmp/tuyul_sdk-0.1.0rc1.tar.gz` & `tmp/tuyul_sdk-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuyul_sdk-0.1.0rc1.tar", max compression
+gzip compressed data, was "tuyul_sdk-0.1.0rc2.tar", max compression
```

## Comparing `tuyul_sdk-0.1.0rc1.tar` & `tuyul_sdk-0.1.0rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      619 2024-05-31 04:03:29.472700 tuyul_sdk-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-31 02:26:37.717294 tuyul_sdk-0.1.0rc1/README.md
--rw-r--r--   0        0        0      125 2024-05-31 03:57:46.818106 tuyul_sdk-0.1.0rc1/tuyul_sdk/__init__.py
--rw-r--r--   0        0        0      303 2024-05-31 03:14:55.963434 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Cipher/__init__.py
--rw-r--r--   0        0        0     6029 2024-05-31 03:13:40.901253 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Cipher/AES.py
--rw-r--r--   0        0        0     1559 2024-05-31 02:38:39.120584 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Cipher/Password.py
--rw-r--r--   0        0        0      518 2024-05-31 02:45:58.639747 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Cipher/Salt.py
--rw-r--r--   0        0        0      101 2024-05-31 03:28:50.075893 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/_certificate/__init__.py
--rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/_certificate/cacert.pem
--rw-r--r--   0        0        0     1581 2024-05-31 03:28:19.129050 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/httpx.py
--rw-r--r--   0        0        0     1294 2024-05-31 03:28:24.109127 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/requests.py
--rw-r--r--   0        0        0     4286 2024-05-31 03:18:09.960902 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/utils.py
--rw-r--r--   0        0        0     2654 2024-05-30 03:57:45.352001 tuyul_sdk-0.1.0rc1/tuyul_sdk/_Database.py
--rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.1.0rc1/tuyul_sdk/sql.py
--rw-r--r--   0        0        0      366 2024-05-31 03:59:01.720591 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/__init__.py
--rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_Color.py
--rw-r--r--   0        0        0     3669 2024-05-31 02:45:00.849778 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_hexbytes.py
--rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_input.py
--rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_Line.py
--rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_Log.py
--rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_Progress.py
--rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_Reset.py
--rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_UserAgent.py
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0rc1/setup.py
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      628 2024-06-01 07:48:13.984868 tuyul_sdk-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 02:26:37.717294 tuyul_sdk-0.1.0rc2/README.md
+-rw-r--r--   0        0        0      125 2024-05-31 03:57:46.818106 tuyul_sdk-0.1.0rc2/tuyul_sdk/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-31 03:14:55.963434 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Cipher/__init__.py
+-rw-r--r--   0        0        0     6029 2024-05-31 05:48:34.784524 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Cipher/AES.py
+-rw-r--r--   0        0        0     1559 2024-05-31 02:38:39.120584 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Cipher/Password.py
+-rw-r--r--   0        0        0      526 2024-05-31 05:51:39.453523 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Cipher/Salt.py
+-rw-r--r--   0        0        0      101 2024-05-31 03:28:50.075893 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/_certificate/__init__.py
+-rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/_certificate/cacert.pem
+-rw-r--r--   0        0        0     1581 2024-05-31 03:28:19.129050 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/httpx.py
+-rw-r--r--   0        0        0     1294 2024-05-31 03:28:24.109127 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/requests.py
+-rw-r--r--   0        0        0     4286 2024-05-31 03:18:09.960902 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/utils.py
+-rw-r--r--   0        0        0     2654 2024-05-30 03:57:45.352001 tuyul_sdk-0.1.0rc2/tuyul_sdk/_Database.py
+-rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.1.0rc2/tuyul_sdk/sql.py
+-rw-r--r--   0        0        0      366 2024-05-31 03:59:01.720591 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/__init__.py
+-rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_Color.py
+-rw-r--r--   0        0        0     3669 2024-05-31 02:45:00.849778 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_hexbytes.py
+-rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_input.py
+-rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_Line.py
+-rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_Log.py
+-rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_Progress.py
+-rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_Reset.py
+-rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_UserAgent.py
+-rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0rc2/setup.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0rc2/PKG-INFO
```

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/_Cipher/AES.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/_Cipher/AES.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,26 +35,26 @@
             return data
     else:
         raise TypeError('Password must be a string or bytes') 
 
 def to_decode(PlainText: Union[str, bytes]):
     if isinstance(PlainText, str):
         try:
+            return HexBytes(PlainText)
+        except: pass
+        try:
             decode = base64.b64decode(PlainText)
             if PlainText == base64.b64encode(decode).decode():
                 return decode
         except: pass
         try:
             decode = base58.b58decode(PlainText)
             if PlainText == base58.b58encode(decode).decode():
                 return decode
         except: pass
-        try:
-            return HexBytes(PlainText)
-        except: pass
     elif isinstance(PlainText, (bytes, HexBytes, bytearray)):
         return PlainText
     else:
         raise TypeError('Data must be a string or bytes')
 
 def pad(PlainText: bytes):
     return PlainText + (SIZE - len(PlainText) % SIZE) * bytes(chr(0), encoding='utf-8')
```

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/_Cipher/Password.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/_Cipher/Password.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/_Cipher/Salt.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/_Cipher/Salt.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DEFAULT_SALT = HexBytes('0e25b3489775f493')
 
 class Salt:
 
     @classmethod
     def create(cls):
         return cls(get_random_bytes(8))
-    def __init__(self, keys: bytes = None) -> None:
+    def __init__(self, keys: bytes = DEFAULT_SALT) -> None:
         self.__k__ = self.create() if not keys else keys
     def __str__(self) -> str:
         return str(self.__k__)
     def __repr__(self) -> str:
         return str(self.__k__)
     def __bytes__(self):
         return self.__k__
```

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/_certificate/cacert.pem` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/_certificate/cacert.pem`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/httpx.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/httpx.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/requests.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/requests.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/_Connection/utils.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/_Connection/utils.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/_Database.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/_Database.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_hexbytes.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_hexbytes.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_Line.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_Line.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_Log.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_Log.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_Progress.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_Progress.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/tuyul_sdk/Utils/_UserAgent.py` & `tuyul_sdk-0.1.0rc2/tuyul_sdk/Utils/_UserAgent.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.1.0rc1/setup.py` & `tuyul_sdk-0.1.0rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['base58==2.1.1',
  'chardet==5.2.0',
  'colorama==0.4.6',
- 'httpx[socks]==0.27.0',
+ 'httpx[http2,socks]==0.27.0',
  'pycryptodomex==3.20.0',
  'random-user-agent==1.0.1',
  'requests-toolbelt==0.10.1',
- 'requests==2.32.3',
+ 'requests==2.31.0',
  'sqlalchemy-utils==0.41.2',
  'sqlalchemy==2.0.30',
  'urllib3==1.26.15']
 
 setup_kwargs = {
     'name': 'tuyul-sdk',
-    'version': '0.1.0rc1',
+    'version': '0.1.0rc2',
     'description': '',
     'long_description': '',
     'author': 'DesKaOne',
     'author_email': 'DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tuyul_sdk-0.1.0rc1/PKG-INFO` & `tuyul_sdk-0.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tuyul-sdk
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: 
 Author: DesKaOne
 Author-email: DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: base58 (==2.1.1)
 Requires-Dist: chardet (==5.2.0)
 Requires-Dist: colorama (==0.4.6)
-Requires-Dist: httpx[socks] (==0.27.0)
+Requires-Dist: httpx[http2,socks] (==0.27.0)
 Requires-Dist: pycryptodomex (==3.20.0)
 Requires-Dist: random-user-agent (==1.0.1)
-Requires-Dist: requests (==2.32.3)
+Requires-Dist: requests (==2.31.0)
 Requires-Dist: requests-toolbelt (==0.10.1)
 Requires-Dist: sqlalchemy (==2.0.30)
 Requires-Dist: sqlalchemy-utils (==0.41.2)
 Requires-Dist: urllib3 (==1.26.15)
 Description-Content-Type: text/markdown
```


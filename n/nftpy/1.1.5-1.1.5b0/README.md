# Comparing `tmp/nftpy-1.1.5.tar.gz` & `tmp/nftpy-1.1.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nftpy-1.1.5.tar", max compression
+gzip compressed data, was "nftpy-1.1.5b0.tar", max compression
```

## Comparing `nftpy-1.1.5.tar` & `nftpy-1.1.5b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1091 2024-05-28 18:17:49.643296 nftpy-1.1.5/LICENSE
--rw-r--r--   0        0        0      285 2024-06-01 05:36:12.515801 nftpy-1.1.5/nftpy/__init__.py
--rw-r--r--   0        0        0     2669 2024-06-01 05:25:48.705907 nftpy-1.1.5/nftpy/errors.py
--rw-r--r--   0        0        0      168 2024-06-01 05:36:12.514801 nftpy-1.1.5/nftpy/EVM/__init__.py
--rw-r--r--   0        0        0    14009 2024-05-28 18:17:49.644297 nftpy-1.1.5/nftpy/EVM/abi.py
--rw-r--r--   0        0        0     7094 2024-06-01 05:35:56.993423 nftpy-1.1.5/nftpy/EVM/chains.py
--rw-r--r--   0        0        0     6253 2024-06-01 05:35:56.994424 nftpy-1.1.5/nftpy/EVM/nft.py
--rw-r--r--   0        0        0    14387 2024-06-01 05:45:48.310250 nftpy-1.1.5/nftpy/EVM/wallet.py
--rw-r--r--   0        0        0    15051 2024-06-01 02:59:48.543399 nftpy-1.1.5/nftpy/opensea.py
--rw-r--r--   0        0        0      570 2024-06-01 05:36:12.515801 nftpy-1.1.5/pyproject.toml
--rw-r--r--   0        0        0    13725 2024-06-01 05:57:20.368338 nftpy-1.1.5/README.md
--rw-r--r--   0        0        0    14066 1970-01-01 00:00:00.000000 nftpy-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-28 18:17:49.643296 nftpy-1.1.5b0/LICENSE
+-rw-r--r--   0        0        0      286 2024-06-01 06:16:58.282863 nftpy-1.1.5b0/nftpy/__init__.py
+-rw-r--r--   0        0        0     2669 2024-06-01 05:25:48.705907 nftpy-1.1.5b0/nftpy/errors.py
+-rw-r--r--   0        0        0      168 2024-06-01 06:09:11.960373 nftpy-1.1.5b0/nftpy/EVM/__init__.py
+-rw-r--r--   0        0        0    14009 2024-05-28 18:17:49.644297 nftpy-1.1.5b0/nftpy/EVM/abi.py
+-rw-r--r--   0        0        0     7094 2024-06-01 05:35:56.993423 nftpy-1.1.5b0/nftpy/EVM/chains.py
+-rw-r--r--   0        0        0     6253 2024-06-01 05:35:56.994424 nftpy-1.1.5b0/nftpy/EVM/nft.py
+-rw-r--r--   0        0        0    14387 2024-06-01 06:09:11.961373 nftpy-1.1.5b0/nftpy/EVM/wallet.py
+-rw-r--r--   0        0        0    15051 2024-06-01 02:59:48.543399 nftpy-1.1.5b0/nftpy/opensea.py
+-rw-r--r--   0        0        0      570 2024-06-01 06:17:14.150934 nftpy-1.1.5b0/pyproject.toml
+-rw-r--r--   0        0        0    13870 2024-06-01 06:21:08.253423 nftpy-1.1.5b0/README.md
+-rw-r--r--   0        0        0    14361 1970-01-01 00:00:00.000000 nftpy-1.1.5b0/PKG-INFO
```

### Comparing `nftpy-1.1.5/LICENSE` & `nftpy-1.1.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.5/nftpy/errors.py` & `nftpy-1.1.5b0/nftpy/errors.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.5/nftpy/EVM/abi.py` & `nftpy-1.1.5b0/nftpy/EVM/abi.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.5/nftpy/EVM/chains.py` & `nftpy-1.1.5b0/nftpy/EVM/chains.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.5/nftpy/EVM/nft.py` & `nftpy-1.1.5b0/nftpy/EVM/nft.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.5/nftpy/EVM/wallet.py` & `nftpy-1.1.5b0/nftpy/EVM/wallet.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.5/nftpy/opensea.py` & `nftpy-1.1.5b0/nftpy/opensea.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.5/pyproject.toml` & `nftpy-1.1.5b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "nftpy"
-version = "1.1.5"
+version = "1.1.5b"
 description = "A NFT specific Python library for easy NFT integration in Python"
 authors = ["CoulterStutz <coultercash@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/coulterstutz/nftpy"
 repository = "https://github.com/coulterstutz/nftpy"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.9"
 web3 = "^6.2.0"
 requests = "^2.28.1"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^5.1.0"
 
 [build-system]
```

### Comparing `nftpy-1.1.5/README.md` & `nftpy-1.1.5b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # nftpy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1.5-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.5b-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
-### Changes in 1.1.5
+### Changes in 1.1.5b
 #### Threaded NFTWallet class for fast chain querying!
 If you are querying to multiple chains at once, fear no more as processing times are slashed for multichain querying!
+#### Adjusted to support Python ^3.9
+NFTPy has been adjusted to support earlier versions of python. Python 3.9-3.12 will now be supported!
+
 ## Features
 
 #### EVM Interaction with NFT Tokens
 ![Ethereum](https://img.shields.io/badge/Ethereum%20Based%20Networks-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white)
 
 nftpy enables interaction with the Ethereum Virtual Machine (EVM) through RPC to retrieve contract details and token holders. It provides a direct communication pathway between the client and the blockchain. Currently, transactional methods are not supported but will be implemented in future updates. The following methods are available:
```

### Comparing `nftpy-1.1.5/PKG-INFO` & `nftpy-1.1.5b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: nftpy
-Version: 1.1.5
+Version: 1.1.5b0
 Summary: A NFT specific Python library for easy NFT integration in Python
 Home-page: https://github.com/coulterstutz/nftpy
 License: MIT
 Author: CoulterStutz
 Author-email: coultercash@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: web3 (>=6.2.0,<7.0.0)
 Project-URL: Repository, https://github.com/coulterstutz/nftpy
 Description-Content-Type: text/markdown
 
 # nftpy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1.5-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.5b-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
-### Changes in 1.1.5
+### Changes in 1.1.5b
 #### Threaded NFTWallet class for fast chain querying!
 If you are querying to multiple chains at once, fear no more as processing times are slashed for multichain querying!
+#### Adjusted to support Python ^3.9
+NFTPy has been adjusted to support earlier versions of python. Python 3.9-3.12 will now be supported!
+
 ## Features
 
 #### EVM Interaction with NFT Tokens
 ![Ethereum](https://img.shields.io/badge/Ethereum%20Based%20Networks-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white)
 
 nftpy enables interaction with the Ethereum Virtual Machine (EVM) through RPC to retrieve contract details and token holders. It provides a direct communication pathway between the client and the blockchain. Currently, transactional methods are not supported but will be implemented in future updates. The following methods are available:
```


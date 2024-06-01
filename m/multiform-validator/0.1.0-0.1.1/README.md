# Comparing `tmp/multiform_validator-0.1.0.tar.gz` & `tmp/multiform_validator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiform_validator-0.1.0.tar", last modified: Wed May 15 08:21:30 2024, max compression
+gzip compressed data, was "multiform_validator-0.1.1.tar", last modified: Sat Jun  1 01:18:09 2024, max compression
```

## Comparing `multiform_validator-0.1.0.tar` & `multiform_validator-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:30.062606 multiform_validator-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-15 08:21:30.062606 multiform_validator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:21:30.062606 multiform_validator-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:30.058606 multiform_validator-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:30.062606 multiform_validator-0.1.0/src/multiform_validator/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/cnpjValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/cpfValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/getOnlyEmail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/identifyFlagCard.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/isCreditCardValid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/isEmail.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/isValidImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/passwordStrengthTester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 08:21:20.000000 multiform_validator-0.1.0/src/multiform_validator/validateBRPhoneNumber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:21:30.062606 multiform_validator-0.1.0/src/multiform_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-15 08:21:30.000000 multiform_validator-0.1.0/src/multiform_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-15 08:21:30.000000 multiform_validator-0.1.0/src/multiform_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:21:30.000000 multiform_validator-0.1.0/src/multiform_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 08:21:30.000000 multiform_validator-0.1.0/src/multiform_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:18:09.939833 multiform_validator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-06-01 01:18:09.939833 multiform_validator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:18:09.939833 multiform_validator-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:18:09.935833 multiform_validator-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:18:09.935833 multiform_validator-0.1.1/src/multiform_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/cnpjValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/cpfValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/getOnlyEmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/identifyFlagCard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/isCreditCardValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/isEmail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/isValidImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/passwordStrengthTester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-06-01 01:17:55.000000 multiform_validator-0.1.1/src/multiform_validator/validateBRPhoneNumber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:18:09.939833 multiform_validator-0.1.1/src/multiform_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-06-01 01:18:09.000000 multiform_validator-0.1.1/src/multiform_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-01 01:18:09.000000 multiform_validator-0.1.1/src/multiform_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:18:09.000000 multiform_validator-0.1.1/src/multiform_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-01 01:18:09.000000 multiform_validator-0.1.1/src/multiform_validator.egg-info/top_level.txt
```

### Comparing `multiform_validator-0.1.0/LICENSE` & `multiform_validator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/PKG-INFO` & `multiform_validator-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: multiform-validator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more.
 Author: Gabriel Logan
-Project-URL: Homepage, https://gabriel-logan.github.io/multiform-validator/documentation
+Project-URL: Homepage, https://multiform-validator.vercel.app/documentation
 Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
 Keywords: validator,multiform,validação,email-validator,image,multiform-validator,python,security,safe,pentest,security-tools,Validator,validate,cpf,cnpj,email validator,password,email,isEmail
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
 This package provides Python functions to validate various forms fields.
 
-Documentation: https://gabriel-logan.github.io/multiform-validator/documentation/py
+Documentation: https://multiform-validator.vercel.app/documentation/py
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
 
 <p align="center">
 	<a href="https://www.buymeacoffee.com/gabriellogan" target="_blank">
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: multiform-validator Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: multiform-validator Version: 0.1.1 Summary:
 Multilingual library made for validation, various form fields, such as: email,
 cpf, cnpj, credit card, and much more. Author: Gabriel Logan Project-URL:
-Homepage, https://gabriel-logan.github.io/multiform-validator/documentation
-Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/
-tree/main/packages/python Keywords: validator,multiform,validaÃ§Ã£o,email-
+Homepage, https://multiform-validator.vercel.app/documentation Project-URL: Bug
+Tracker, https://github.com/gabriel-logan/multiform-validator/tree/main/
+packages/python Keywords: validator,multiform,validaÃ§Ã£o,email-
 validator,image,multiform-validator,python,security,safe,pentest,security-
 tools,Validator,validate,cpf,cnpj,email validator,password,email,isEmail
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1 Description-Content-Type: text/markdown License-File:
 LICENSE # Multiform-validator [![PyPI version](https://badge.fury.io/py/
 multiform-validator.svg)](https://badge.fury.io/py/multiform-validator) [!
 [License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![PyPI downloads](https://img.shields.io/pypi/dm/
 multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/
 multiform-validator) This package provides Python functions to validate various
-forms fields. Documentation: https://gabriel-logan.github.io/multiform-
-validator/documentation/py Feel free to find bugs and report them to me. Your
-feedback is highly appreciated. Hugs from Gabriel Logan! If you want to help
-me, you can buy me a coffee (:
+forms fields. Documentation: https://multiform-validator.vercel.app/
+documentation/py Feel free to find bugs and report them to me. Your feedback is
+highly appreciated. Hugs from Gabriel Logan! If you want to help me, you can
+buy me a coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ### Installation ```bash pip install multiform-validator ``` # Data Validator
 This package contains various modules for validating different types of data.
 Below are the available validation modules: # Avaliable for while -
 **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
 **getOnlyEmail**: Extracts only the email or emails address from a string. -
 **identifyFlagCard**: Identifies the flag of a credit card. -
```

### Comparing `multiform_validator-0.1.0/README.md` & `multiform_validator-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
 This package provides Python functions to validate various forms fields.
 
-Documentation: https://gabriel-logan.github.io/multiform-validator/documentation/py
+Documentation: https://multiform-validator.vercel.app/documentation/py
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
 
 <p align="center">
 	<a href="https://www.buymeacoffee.com/gabriellogan" target="_blank">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 # Multiform-validator [![PyPI version](https://badge.fury.io/py/multiform-
 validator.svg)](https://badge.fury.io/py/multiform-validator) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
 licenses/MIT) [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-
 validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-
 validator) This package provides Python functions to validate various forms
-fields. Documentation: https://gabriel-logan.github.io/multiform-validator/
-documentation/py Feel free to find bugs and report them to me. Your feedback is
-highly appreciated. Hugs from Gabriel Logan! If you want to help me, you can
-buy me a coffee (:
+fields. Documentation: https://multiform-validator.vercel.app/documentation/py
+Feel free to find bugs and report them to me. Your feedback is highly
+appreciated. Hugs from Gabriel Logan! If you want to help me, you can buy me a
+coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ### Installation ```bash pip install multiform-validator ``` # Data Validator
 This package contains various modules for validating different types of data.
 Below are the available validation modules: # Avaliable for while -
 **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
 **getOnlyEmail**: Extracts only the email or emails address from a string. -
 **identifyFlagCard**: Identifies the flag of a credit card. -
```

### Comparing `multiform_validator-0.1.0/pyproject.toml` & `multiform_validator-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 requires = [
     "setuptools>=61"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "multiform-validator"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Gabriel Logan" },
 ]
 description = "Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more."
 readme = "README.md"
 keywords = ["validator", "multiform", "validação", "email-validator", "image", "multiform-validator", "python", "security", "safe", "pentest", "security-tools", "Validator", "validate", "cpf", "cnpj", "email validator", "password", "email", "isEmail"]
 requires-python = ">=3.1"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://gabriel-logan.github.io/multiform-validator/documentation"
+"Homepage" = "https://multiform-validator.vercel.app/documentation"
 "Bug Tracker" = "https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python"
```

### Comparing `multiform_validator-0.1.0/src/multiform_validator/cnpjValidator.py` & `multiform_validator-0.1.1/src/multiform_validator/cnpjValidator.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/src/multiform_validator/cpfValidator.py` & `multiform_validator-0.1.1/src/multiform_validator/cpfValidator.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/src/multiform_validator/getOnlyEmail.py` & `multiform_validator-0.1.1/src/multiform_validator/getOnlyEmail.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/src/multiform_validator/identifyFlagCard.py` & `multiform_validator-0.1.1/src/multiform_validator/identifyFlagCard.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/src/multiform_validator/isCreditCardValid.py` & `multiform_validator-0.1.1/src/multiform_validator/isCreditCardValid.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/src/multiform_validator/isEmail.py` & `multiform_validator-0.1.1/src/multiform_validator/isEmail.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/src/multiform_validator/passwordStrengthTester.py` & `multiform_validator-0.1.1/src/multiform_validator/passwordStrengthTester.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/src/multiform_validator/validateBRPhoneNumber.py` & `multiform_validator-0.1.1/src/multiform_validator/validateBRPhoneNumber.py`

 * *Files identical despite different names*

### Comparing `multiform_validator-0.1.0/src/multiform_validator.egg-info/PKG-INFO` & `multiform_validator-0.1.1/src/multiform_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: multiform-validator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more.
 Author: Gabriel Logan
-Project-URL: Homepage, https://gabriel-logan.github.io/multiform-validator/documentation
+Project-URL: Homepage, https://multiform-validator.vercel.app/documentation
 Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
 Keywords: validator,multiform,validação,email-validator,image,multiform-validator,python,security,safe,pentest,security-tools,Validator,validate,cpf,cnpj,email validator,password,email,isEmail
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
 This package provides Python functions to validate various forms fields.
 
-Documentation: https://gabriel-logan.github.io/multiform-validator/documentation/py
+Documentation: https://multiform-validator.vercel.app/documentation/py
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
 
 <p align="center">
 	<a href="https://www.buymeacoffee.com/gabriellogan" target="_blank">
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: multiform-validator Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: multiform-validator Version: 0.1.1 Summary:
 Multilingual library made for validation, various form fields, such as: email,
 cpf, cnpj, credit card, and much more. Author: Gabriel Logan Project-URL:
-Homepage, https://gabriel-logan.github.io/multiform-validator/documentation
-Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/
-tree/main/packages/python Keywords: validator,multiform,validaÃ§Ã£o,email-
+Homepage, https://multiform-validator.vercel.app/documentation Project-URL: Bug
+Tracker, https://github.com/gabriel-logan/multiform-validator/tree/main/
+packages/python Keywords: validator,multiform,validaÃ§Ã£o,email-
 validator,image,multiform-validator,python,security,safe,pentest,security-
 tools,Validator,validate,cpf,cnpj,email validator,password,email,isEmail
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1 Description-Content-Type: text/markdown License-File:
 LICENSE # Multiform-validator [![PyPI version](https://badge.fury.io/py/
 multiform-validator.svg)](https://badge.fury.io/py/multiform-validator) [!
 [License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 opensource.org/licenses/MIT) [![PyPI downloads](https://img.shields.io/pypi/dm/
 multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/
 multiform-validator) This package provides Python functions to validate various
-forms fields. Documentation: https://gabriel-logan.github.io/multiform-
-validator/documentation/py Feel free to find bugs and report them to me. Your
-feedback is highly appreciated. Hugs from Gabriel Logan! If you want to help
-me, you can buy me a coffee (:
+forms fields. Documentation: https://multiform-validator.vercel.app/
+documentation/py Feel free to find bugs and report them to me. Your feedback is
+highly appreciated. Hugs from Gabriel Logan! If you want to help me, you can
+buy me a coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ### Installation ```bash pip install multiform-validator ``` # Data Validator
 This package contains various modules for validating different types of data.
 Below are the available validation modules: # Avaliable for while -
 **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
 **getOnlyEmail**: Extracts only the email or emails address from a string. -
 **identifyFlagCard**: Identifies the flag of a credit card. -
```

### Comparing `multiform_validator-0.1.0/src/multiform_validator.egg-info/SOURCES.txt` & `multiform_validator-0.1.1/src/multiform_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/Flask-Inputs-0.3.0.tar.gz` & `tmp/flask_inputs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Inputs-0.3.0.tar", last modified: Tue Jul 31 19:53:51 2018, max compression
+gzip compressed data, was "flask_inputs-1.0.0.tar", last modified: Sat Jun  1 16:48:17 2024, max compression
```

## Comparing `Flask-Inputs-0.3.0.tar` & `flask_inputs-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxr-xr-x   0 nathancahill   (501) staff       (20)        0 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/
--rw-r--r--   0 nathancahill   (501) staff       (20)     1239 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/PKG-INFO
--rw-r--r--   0 nathancahill   (501) staff       (20)      681 2018-07-31 19:53:26.000000 Flask-Inputs-0.3.0/setup.py
-drwxr-xr-x   0 nathancahill   (501) staff       (20)        0 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/flask_inputs/
--rw-r--r--   0 nathancahill   (501) staff       (20)      749 2018-07-31 19:50:24.000000 Flask-Inputs-0.3.0/flask_inputs/validators.py
--rw-r--r--   0 nathancahill   (501) staff       (20)       28 2018-07-31 19:50:24.000000 Flask-Inputs-0.3.0/flask_inputs/__init__.py
--rw-r--r--   0 nathancahill   (501) staff       (20)     2580 2018-07-31 19:50:24.000000 Flask-Inputs-0.3.0/flask_inputs/inputs.py
--rw-r--r--   0 nathancahill   (501) staff       (20)       38 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/setup.cfg
--rw-r--r--   0 nathancahill   (501) staff       (20)      715 2018-07-31 19:50:24.000000 Flask-Inputs-0.3.0/README.rst
-drwxr-xr-x   0 nathancahill   (501) staff       (20)        0 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/Flask_Inputs.egg-info/
--rw-r--r--   0 nathancahill   (501) staff       (20)     1239 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/Flask_Inputs.egg-info/PKG-INFO
--rw-r--r--   0 nathancahill   (501) staff       (20)      273 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/Flask_Inputs.egg-info/SOURCES.txt
--rw-r--r--   0 nathancahill   (501) staff       (20)       21 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/Flask_Inputs.egg-info/requires.txt
--rw-r--r--   0 nathancahill   (501) staff       (20)       13 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/Flask_Inputs.egg-info/top_level.txt
--rw-r--r--   0 nathancahill   (501) staff       (20)        1 2018-07-31 19:53:51.000000 Flask-Inputs-0.3.0/Flask_Inputs.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:48:17.658813 flask_inputs-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-06-01 16:48:17.658813 flask_inputs-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-01 16:48:10.000000 flask_inputs-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:48:17.658813 flask_inputs-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:48:17.654813 flask_inputs-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:48:17.658813 flask_inputs-1.0.0/src/Flask_Inputs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-06-01 16:48:17.000000 flask_inputs-1.0.0/src/Flask_Inputs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-06-01 16:48:17.000000 flask_inputs-1.0.0/src/Flask_Inputs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:48:17.000000 flask_inputs-1.0.0/src/Flask_Inputs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 16:48:17.000000 flask_inputs-1.0.0/src/Flask_Inputs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 16:48:17.000000 flask_inputs-1.0.0/src/Flask_Inputs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:48:17.654813 flask_inputs-1.0.0/src/flask_inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/src/flask_inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/src/flask_inputs/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/src/flask_inputs/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:48:17.654813 flask_inputs-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/tests/test_jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/tests/test_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-06-01 16:48:04.000000 flask_inputs-1.0.0/tests/test_values.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-Inputs-0.3.0/setup.py` & `flask_inputs-1.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,43 @@
 
 from setuptools import setup
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
+if not path.exists('README.rst'):
+    import pypandoc
+    pypandoc.download_pandoc(targetfolder='~/bin/')
+    pypandoc.convert_file('README.md', 'rst', outputfile='README.rst')
+
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
+    python_requires='>=3.9',
     name='Flask-Inputs',
-    version='0.3.0',
+    version='1.0.0',
     description='Flask request data validation',
     long_description=long_description,
-    url='http://pythonhosted.org/Flask-Inputs/',
-    author='Nathan Cahill',
-    author_email='nathan@nathancahill.com',
+    url='http://pythonhosted.org/Flask-Inputs',
+    author='David Parker',
+    author_email='durera@gmail.com',
     license='MIT',
     keywords='flask validation wtforms',
+    package_dir={'': 'src'},
     packages=['flask_inputs'],
-    install_requires=['flask', 'wtforms', 'future'],
-    tests_require=['nose', 'coverage', 'jsonschema'],
+    install_requires=[
+        'flask >= 3',
+        'wtforms >= 3',
+        'future >= 1'
+    ],
+    extras_require={
+        'dev': [
+            'build',
+            'pytest',
+            'email_validator',
+            'jsonschema'
+        ]
+    },
 )
```

### Comparing `Flask-Inputs-0.3.0/flask_inputs/validators.py` & `flask_inputs-1.0.0/src/flask_inputs/validators.py`

 * *Files identical despite different names*

### Comparing `Flask-Inputs-0.3.0/flask_inputs/inputs.py` & `flask_inputs-1.0.0/src/flask_inputs/inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-import collections
+from collections.abc import Iterable
 from itertools import chain
 from future.utils import iteritems
 
 from werkzeug.datastructures import MultiDict
 
 from wtforms.form import BaseForm
 from wtforms.fields import Field
@@ -30,15 +30,15 @@
             if not name.startswith('_') and name not in ['errors', 'validate', 'valid_attrs']:
                 input = getattr(self, name)
                 fields = dict()
 
                 if isinstance(input, dict):
                     for field, validators in iteritems(input):
                         fields[field] = Field(validators=validators)
-                elif isinstance(input, collections.Iterable):
+                elif isinstance(input, Iterable):
                     fields['_input'] = Field(validators=input)
 
                 self._forms[name] = BaseForm(fields)
 
     def _get_values(self, attribute, coerse=True):
         """Compatability function to return MultiDict objects with values from
         a flask.Request object.
```


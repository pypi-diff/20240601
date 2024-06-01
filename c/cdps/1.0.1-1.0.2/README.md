# Comparing `tmp/cdps-1.0.1.tar.gz` & `tmp/cdps-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdps-1.0.1.tar", last modified: Sat Jun  1 15:05:13 2024, max compression
+gzip compressed data, was "cdps-1.0.2.tar", last modified: Sat Jun  1 15:11:23 2024, max compression
```

## Comparing `cdps-1.0.1.tar` & `cdps-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:05:13.474017 cdps-1.0.1/
--rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      755 2024-06-01 15:05:13.474017 cdps-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 15:05:13.473018 cdps-1.0.1/cdps.egg-info/
--rw-rw-rw-   0        0        0      755 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      218 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:05:13.000000 cdps-1.0.1/cdps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:05:13.474017 cdps-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1489 2024-06-01 15:04:37.000000 cdps-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:11:23.949931 cdps-1.0.2/
+-rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:11:23.949931 cdps-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:11:23.948947 cdps-1.0.2/cdps.egg-info/
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:11:23.000000 cdps-1.0.2/cdps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-06-01 15:11:23.000000 cdps-1.0.2/cdps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:11:23.000000 cdps-1.0.2/cdps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-06-01 15:11:23.000000 cdps-1.0.2/cdps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      218 2024-06-01 15:11:23.000000 cdps-1.0.2/cdps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:11:23.000000 cdps-1.0.2/cdps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:11:23.950930 cdps-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1715 2024-06-01 15:11:18.000000 cdps-1.0.2/setup.py
```

### Comparing `cdps-1.0.1/LICENSE` & `cdps-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdps-1.0.1/README.md` & `cdps-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cdps-1.0.1/setup.py` & `cdps-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,43 +6,48 @@
 NAME = core_constant.PACKAGE_NAME
 VERSION = core_constant.VERSION
 DESCRIPTION = 'Composite Disaster Prevention Server'
 AUTHOR = 'ExpTechTW'
 REQUIRES_PYTHON = '>=3.8'
 
 CLASSIFIERS = [
-	# https://pypi.org/classifiers/
-	'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-	'Operating System :: OS Independent',
-	'Programming Language :: Python',
-	'Programming Language :: Python :: 3',
-	'Programming Language :: Python :: 3.8',
-	'Programming Language :: Python :: 3.9',
-	'Programming Language :: Python :: 3.10',
-	'Programming Language :: Python :: 3.11',
-	'Programming Language :: Python :: 3.12',
+    # https://pypi.org/classifiers/
+    'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
+    'Operating System :: OS Independent',
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 
 ENTRY_POINTS = {
 	'console_scripts': [
 		'{} = {}.entrypoint:entrypoint'.format(core_constant.CLI_COMMAND, core_constant.PACKAGE_NAME)
 	]
 }
 print('ENTRY_POINTS = {}'.format(ENTRY_POINTS))
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'requirements.txt')) as f:
 	REQUIRED = list(filter(None, map(str.strip, f)))
 	print('REQUIRED = {}'.format(REQUIRED))
+	
+with open(os.path.join(here, 'README.md'), encoding='utf8') as f:
+	LONG_DESCRIPTION = f.read()
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
+	long_description=LONG_DESCRIPTION,
+	long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email='exptech.tw@gmail.com',
     packages=find_packages(exclude=['tests']),
     include_package_data=True,
 	python_requires=REQUIRES_PYTHON,
 	install_requires=REQUIRED,
 	classifiers=CLASSIFIERS,
```


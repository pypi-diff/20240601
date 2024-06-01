# Comparing `tmp/django-models-package-0.2.tar.gz` & `tmp/django-models-package-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-models-package-0.2.tar", last modified: Sat Jun  1 18:59:15 2024, max compression
+gzip compressed data, was "django-models-package-0.3.tar", last modified: Sat Jun  1 19:48:40 2024, max compression
```

## Comparing `django-models-package-0.2.tar` & `django-models-package-0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 18:59:15.341585 django-models-package-0.2/
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)       18 2024-06-01 18:52:14.000000 django-models-package-0.2/MANIFEST.in
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      561 2024-06-01 18:59:15.341585 django-models-package-0.2/PKG-INFO
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      117 2024-06-01 18:57:04.000000 django-models-package-0.2/README.md
-drwxrwxr-x   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 18:59:15.341585 django-models-package-0.2/django_models_package.egg-info/
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      561 2024-06-01 18:59:15.000000 django-models-package-0.2/django_models_package.egg-info/PKG-INFO
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      448 2024-06-01 18:59:15.000000 django-models-package-0.2/django_models_package.egg-info/SOURCES.txt
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)        1 2024-06-01 18:59:15.000000 django-models-package-0.2/django_models_package.egg-info/dependency_links.txt
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)       12 2024-06-01 18:59:15.000000 django-models-package-0.2/django_models_package.egg-info/requires.txt
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)       15 2024-06-01 18:59:15.000000 django-models-package-0.2/django_models_package.egg-info/top_level.txt
-drwxrwxr-x   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 18:59:15.341585 django-models-package-0.2/models_package/
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 18:49:30.000000 django-models-package-0.2/models_package/__init__.py
-drwxrwxr-x   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 18:59:15.341585 django-models-package-0.2/models_package/models/
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      120 2024-06-01 18:51:04.000000 django-models-package-0.2/models_package/models/__init__.py
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      798 2024-06-01 18:51:12.000000 django-models-package-0.2/models_package/models/booking.py
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      607 2024-06-01 18:51:18.000000 django-models-package-0.2/models_package/models/flight.py
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      263 2024-06-01 18:51:23.000000 django-models-package-0.2/models_package/models/notification.py
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      627 2024-06-01 18:51:29.000000 django-models-package-0.2/models_package/models/user.py
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)       38 2024-06-01 18:59:15.341585 django-models-package-0.2/setup.cfg
--rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      702 2024-06-01 18:58:32.000000 django-models-package-0.2/setup.py
+drwxrwxr-x   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 19:48:40.256925 django-models-package-0.3/
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)       18 2024-06-01 18:52:14.000000 django-models-package-0.3/MANIFEST.in
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      560 2024-06-01 19:48:40.256925 django-models-package-0.3/PKG-INFO
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      117 2024-06-01 18:57:04.000000 django-models-package-0.3/README.md
+drwxrwxr-x   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 19:48:40.256925 django-models-package-0.3/django_models_package.egg-info/
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      560 2024-06-01 19:48:40.000000 django-models-package-0.3/django_models_package.egg-info/PKG-INFO
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      471 2024-06-01 19:48:40.000000 django-models-package-0.3/django_models_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)        1 2024-06-01 19:48:40.000000 django-models-package-0.3/django_models_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)       12 2024-06-01 19:48:40.000000 django-models-package-0.3/django_models_package.egg-info/requires.txt
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)       15 2024-06-01 19:48:40.000000 django-models-package-0.3/django_models_package.egg-info/top_level.txt
+drwxrwxr-x   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 19:48:40.256925 django-models-package-0.3/models_package/
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 18:49:30.000000 django-models-package-0.3/models_package/__init__.py
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      100 2024-06-01 19:48:15.000000 django-models-package-0.3/models_package/apps.py
+drwxrwxr-x   0 sayrex    (1000) sayrex    (1000)        0 2024-06-01 19:48:40.256925 django-models-package-0.3/models_package/models/
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      120 2024-06-01 18:51:04.000000 django-models-package-0.3/models_package/models/__init__.py
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      798 2024-06-01 18:51:12.000000 django-models-package-0.3/models_package/models/booking.py
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      607 2024-06-01 18:51:18.000000 django-models-package-0.3/models_package/models/flight.py
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      263 2024-06-01 18:51:23.000000 django-models-package-0.3/models_package/models/notification.py
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      627 2024-06-01 18:51:29.000000 django-models-package-0.3/models_package/models/user.py
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)       38 2024-06-01 19:48:40.256925 django-models-package-0.3/setup.cfg
+-rw-rw-r--   0 sayrex    (1000) sayrex    (1000)      701 2024-06-01 19:48:38.000000 django-models-package-0.3/setup.py
```

### Comparing `django-models-package-0.2/models_package/models/booking.py` & `django-models-package-0.3/models_package/models/booking.py`

 * *Files identical despite different names*

### Comparing `django-models-package-0.2/models_package/models/flight.py` & `django-models-package-0.3/models_package/models/flight.py`

 * *Files identical despite different names*

### Comparing `django-models-package-0.2/models_package/models/user.py` & `django-models-package-0.3/models_package/models/user.py`

 * *Files identical despite different names*

### Comparing `django-models-package-0.2/setup.py` & `django-models-package-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 setup(
     name='django-models-package',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'Django>=3.0',
     ],
     include_package_data=True,
     description='A reusable Django models package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    author='Your Name',
-    author_email='your.email@example.com',
+    author='Sayrex',
+    author_email='reshetneff2013@gmail.com',
     url='https://github.com/yourusername/django-models-package',
     classifiers=[
         'Programming Language :: Python :: 3',
         'Framework :: Django',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```


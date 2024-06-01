# Comparing `tmp/gdmty_django_users-24.5.2.tar.gz` & `tmp/gdmty_django_users-24.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty_django_users-24.5.2.tar", last modified: Fri May 31 21:40:08 2024, max compression
+gzip compressed data, was "gdmty_django_users-24.5.3.tar", last modified: Sat Jun  1 02:25:09 2024, max compression
```

## Comparing `gdmty_django_users-24.5.2.tar` & `gdmty_django_users-24.5.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 21:40:08.992654 gdmty_django_users-24.5.2/
--rw-rw-rw-   0        0        0    35182 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.2/LICENSE
--rw-rw-rw-   0        0        0       51 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0    43714 2024-05-31 21:40:08.992654 gdmty_django_users-24.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/README.md
--rw-rw-rw-   0        0        0     1527 2024-05-31 21:39:52.000000 gdmty_django_users-24.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 21:40:08.992654 gdmty_django_users-24.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 21:40:08.961005 gdmty_django_users-24.5.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 21:40:08.977021 gdmty_django_users-24.5.2/src/gdmty_django_users/
--rw-rw-rw-   0        0        0     1367 2024-05-31 21:39:52.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/__init__.py
--rw-rw-rw-   0        0        0     2477 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/admin.py
--rw-rw-rw-   0        0        0     1048 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/apps.py
--rw-rw-rw-   0        0        0     1437 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/decorators.py
--rw-rw-rw-   0        0        0     2332 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/managers.py
-drwxrwxrwx   0        0        0        0 2024-05-31 21:40:08.977021 gdmty_django_users-24.5.2/src/gdmty_django_users/migrations/
--rw-rw-rw-   0        0        0     3284 2024-05-10 04:28:25.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1333 2024-05-10 04:29:08.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
--rw-rw-rw-   0        0        0        0 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/migrations/__init__.py
--rw-rw-rw-   0        0        0     3209 2024-05-31 21:39:31.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/models.py
--rw-rw-rw-   0        0        0     1819 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/permissions.py
--rw-rw-rw-   0        0        0     1763 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/serializers.py
--rw-rw-rw-   0        0        0     1065 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/settings.py
--rw-rw-rw-   0        0        0      910 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/tests.py
--rw-rw-rw-   0        0        0     1756 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/urls.py
--rw-rw-rw-   0        0        0     4811 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/viewsets.py
--rw-rw-rw-   0        0        0     1471 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.2/src/gdmty_django_users/wagtail_forms.py
-drwxrwxrwx   0        0        0        0 2024-05-31 21:40:08.977021 gdmty_django_users-24.5.2/src/gdmty_django_users.egg-info/
--rw-rw-rw-   0        0        0    43714 2024-05-31 21:40:08.000000 gdmty_django_users-24.5.2/src/gdmty_django_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-05-31 21:40:08.000000 gdmty_django_users-24.5.2/src/gdmty_django_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 21:40:08.000000 gdmty_django_users-24.5.2/src/gdmty_django_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2024-05-31 21:40:08.000000 gdmty_django_users-24.5.2/src/gdmty_django_users.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-31 21:40:08.000000 gdmty_django_users-24.5.2/src/gdmty_django_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 02:25:09.858991 gdmty_django_users-24.5.3/
+-rw-rw-rw-   0        0        0    35182 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.3/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    43714 2024-06-01 02:25:09.858991 gdmty_django_users-24.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/README.md
+-rw-rw-rw-   0        0        0     1527 2024-06-01 02:24:57.000000 gdmty_django_users-24.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 02:25:09.858991 gdmty_django_users-24.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 02:25:09.828289 gdmty_django_users-24.5.3/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 02:25:09.844485 gdmty_django_users-24.5.3/src/gdmty_django_users/
+-rw-rw-rw-   0        0        0     1367 2024-06-01 02:24:57.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/__init__.py
+-rw-rw-rw-   0        0        0     2477 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/admin.py
+-rw-rw-rw-   0        0        0     1048 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/apps.py
+-rw-rw-rw-   0        0        0     1437 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/decorators.py
+-rw-rw-rw-   0        0        0     2332 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/managers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:25:09.844485 gdmty_django_users-24.5.3/src/gdmty_django_users/migrations/
+-rw-rw-rw-   0        0        0     3284 2024-05-10 04:28:25.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1333 2024-05-10 04:29:08.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
+-rw-rw-rw-   0        0        0      819 2024-06-01 02:24:23.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/migrations/0003_alter_user_groups.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3209 2024-05-31 21:39:31.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/models.py
+-rw-rw-rw-   0        0        0     1819 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/permissions.py
+-rw-rw-rw-   0        0        0     1763 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/serializers.py
+-rw-rw-rw-   0        0        0     1065 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/settings.py
+-rw-rw-rw-   0        0        0      910 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/tests.py
+-rw-rw-rw-   0        0        0     1756 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/urls.py
+-rw-rw-rw-   0        0        0     4811 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/viewsets.py
+-rw-rw-rw-   0        0        0     1471 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.3/src/gdmty_django_users/wagtail_forms.py
+drwxrwxrwx   0        0        0        0 2024-06-01 02:25:09.858991 gdmty_django_users-24.5.3/src/gdmty_django_users.egg-info/
+-rw-rw-rw-   0        0        0    43714 2024-06-01 02:25:09.000000 gdmty_django_users-24.5.3/src/gdmty_django_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2024-06-01 02:25:09.000000 gdmty_django_users-24.5.3/src/gdmty_django_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 02:25:09.000000 gdmty_django_users-24.5.3/src/gdmty_django_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-06-01 02:25:09.000000 gdmty_django_users-24.5.3/src/gdmty_django_users.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-06-01 02:25:09.000000 gdmty_django_users-24.5.3/src/gdmty_django_users.egg-info/top_level.txt
```

### Comparing `gdmty_django_users-24.5.2/LICENSE` & `gdmty_django_users-24.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/PKG-INFO` & `gdmty_django_users-24.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.5.2
+Version: 24.5.3
 Summary: Extension of Django's AbstractBaseUser for user management, using email as user.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdmty_django_users-24.5.2/README.md` & `gdmty_django_users-24.5.3/README.md`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/pyproject.toml` & `gdmty_django_users-24.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-django-users"
-version = "24.5.2"
+version = "24.5.3"
 description = "Extension of Django's AbstractBaseUser for user management, using email as user."
 readme = "README.md"
 authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-users"
 "Bug Tracker" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues"
 
 [tool.bumpver]
-current_version = "24.5.2"
+current_version = "24.5.3"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/__init__.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 
 """
 
 __title__ = "gdmty_django_users"
-__version__ = "24.5.2"
+__version__ = "24.5.3"
 __description__ = "Django module for Users models and permission adding reCAPTCHA token verification."
 __url__ = "https://github.com/SIGAMty/gdmty-django-recaptcha-enterprise"
 __author__ = "César Benjamín"
 __author_email__ = "mathereall@gmail.com"
 __license__ = "GNU Affero General Public License v3 or later (AGPLv3+)"
 __keywords__ = ["django", "users"]
 VERSION = __version__
```

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/admin.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/admin.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/apps.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/apps.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/decorators.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/decorators.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/managers.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/managers.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/migrations/0001_initial.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/models.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/models.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/permissions.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/permissions.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/serializers.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/serializers.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/settings.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/settings.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/tests.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/tests.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/urls.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/urls.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/viewsets.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/viewsets.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users/wagtail_forms.py` & `gdmty_django_users-24.5.3/src/gdmty_django_users/wagtail_forms.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users.egg-info/PKG-INFO` & `gdmty_django_users-24.5.3/src/gdmty_django_users.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.5.2
+Version: 24.5.3
 Summary: Extension of Django's AbstractBaseUser for user management, using email as user.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdmty_django_users-24.5.2/src/gdmty_django_users.egg-info/SOURCES.txt` & `gdmty_django_users-24.5.3/src/gdmty_django_users.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 src/gdmty_django_users.egg-info/PKG-INFO
 src/gdmty_django_users.egg-info/SOURCES.txt
 src/gdmty_django_users.egg-info/dependency_links.txt
 src/gdmty_django_users.egg-info/requires.txt
 src/gdmty_django_users.egg-info/top_level.txt
 src/gdmty_django_users/migrations/0001_initial.py
 src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
+src/gdmty_django_users/migrations/0003_alter_user_groups.py
 src/gdmty_django_users/migrations/__init__.py
```


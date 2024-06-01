# Comparing `tmp/heaobject-1.6.2.tar.gz` & `tmp/heaobject-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.6.2.tar", last modified: Thu May 30 23:14:49 2024, max compression
+gzip compressed data, was "heaobject-1.6.3.tar", last modified: Sat Jun  1 05:05:29 2024, max compression
```

## Comparing `heaobject-1.6.2.tar` & `heaobject-1.6.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 23:14:49.893928 heaobject-1.6.2/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     6314 2024-05-30 23:14:49.892929 heaobject-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4808 2024-05-30 23:13:21.000000 heaobject-1.6.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-30 23:14:49.893928 heaobject-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     2603 2024-05-30 23:14:29.000000 heaobject-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 23:14:49.835929 heaobject-1.6.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 23:14:49.882929 heaobject-1.6.2/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0    11343 2024-05-30 23:08:07.000000 heaobject-1.6.2/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9988 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.6.2/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.6.2/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.6.2/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/error.py
--rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4566 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/mimetype.py
--rw-rw-rw-   0        0        0    11772 2024-05-23 21:44:05.000000 heaobject-1.6.2/src/heaobject/organization.py
--rw-rw-rw-   0        0        0    13108 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.6.2/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/record.py
--rw-rw-rw-   0        0        0    23400 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    80257 2024-04-24 17:43:21.000000 heaobject-1.6.2/src/heaobject/root.py
--rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.6.2/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/storage.py
--rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.6.2/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1217 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/util.py
--rw-rw-rw-   0        0        0     7290 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-05-30 23:14:49.890929 heaobject-1.6.2/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     6314 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 05:05:29.369945 heaobject-1.6.3/
+-rw-rw-rw-   0        0        0    11625 2023-06-22 19:55:16.000000 heaobject-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0     6492 2024-06-01 05:05:29.368901 heaobject-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2024-06-01 05:04:10.000000 heaobject-1.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 05:05:29.369945 heaobject-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-06-01 05:04:10.000000 heaobject-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:05:29.181307 heaobject-1.6.3/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 05:05:29.351263 heaobject-1.6.3/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0    11343 2024-05-31 23:54:03.000000 heaobject-1.6.3/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-11-27 15:51:20.000000 heaobject-1.6.3/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-12 22:05:30.000000 heaobject-1.6.3/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9988 2024-05-22 20:39:01.000000 heaobject-1.6.3/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2023-06-22 19:55:16.000000 heaobject-1.6.3/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2023-06-22 19:55:16.000000 heaobject-1.6.3/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2023-06-22 19:55:16.000000 heaobject-1.6.3/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4461 2024-06-01 05:04:10.000000 heaobject-1.6.3/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0    11772 2024-05-31 23:54:03.000000 heaobject-1.6.3/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0    13860 2024-06-01 05:04:10.000000 heaobject-1.6.3/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 19:55:16.000000 heaobject-1.6.3/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    23497 2024-06-01 05:04:10.000000 heaobject-1.6.3/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    80287 2024-06-01 05:04:10.000000 heaobject-1.6.3/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-04-09 19:10:11.000000 heaobject-1.6.3/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-07-10 22:02:52.000000 heaobject-1.6.3/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-16 21:52:49.000000 heaobject-1.6.3/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0    10289 2024-04-22 18:44:54.000000 heaobject-1.6.3/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1217 2024-05-22 20:38:15.000000 heaobject-1.6.3/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-10-30 17:37:04.000000 heaobject-1.6.3/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     7290 2024-05-22 20:39:01.000000 heaobject-1.6.3/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:05:29.367363 heaobject-1.6.3/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     6492 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 05:05:29.000000 heaobject-1.6.3/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.6.2/LICENSE` & `heaobject-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/PKG-INFO` & `heaobject-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.6.2
+Version: 1.6.3
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.3
+* credential's expiration type changed from str to datetime
+* registry in creator list no longer checks for NONE_USER
+* person now has access token object
+
 ## Version 1.6.2
 * Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
 
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
 
 ## Version 1.6.0
```

### Comparing `heaobject-1.6.2/README.md` & `heaobject-1.6.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.3
+* credential's expiration type changed from str to datetime
+* registry in creator list no longer checks for NONE_USER
+* person now has access token object
+
 ## Version 1.6.2
 * Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
 
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
 
 ## Version 1.6.0
```

### Comparing `heaobject-1.6.2/setup.py` & `heaobject-1.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.6.2',
+                 version='1.6.3',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.6.2/src/heaobject/__init__.py` & `heaobject-1.6.3/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/account.py` & `heaobject-1.6.3/src/heaobject/account.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/activity.py` & `heaobject-1.6.3/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/aws.py` & `heaobject-1.6.3/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/awss3key.py` & `heaobject-1.6.3/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/bucket.py` & `heaobject-1.6.3/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/data.py` & `heaobject-1.6.3/src/heaobject/data.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/dataadapter.py` & `heaobject-1.6.3/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/datamodel.py` & `heaobject-1.6.3/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/folder.py` & `heaobject-1.6.3/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/keychain.py` & `heaobject-1.6.3/src/heaobject/keychain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Classes supporting the management of user credentials and certificates.
 """
 from datetime import datetime, timezone
 from typing import Optional, Union, TypeVar
 from heaobject import root
+from dateutil import parser as dateparser
 
 
 class Credentials(root.AbstractDesktopObject):
     """
         Stores a user's secrets, passwords, and keys, and makes them available to applications.
     """
 
@@ -84,49 +85,51 @@
         return self.__session_token
 
     @session_token.setter  # type: ignore
     def session_token(self, session_token: Optional[str]):
         self.__session_token = str(session_token) if session_token is not None else None
 
     @property  # type: ignore
-    def expiration(self) -> Optional[str]:
+    def expiration(self) -> datetime | None:
         """
         The session's expiration time.
         """
         return self.__expiration
 
     @expiration.setter  # type: ignore
-    def expiration(self, expiration: Optional[Union[str, datetime]]) -> None:
-        exp_formatted = expiration
-        if type(exp_formatted) is datetime:
-            exp_formatted = exp_formatted.strftime("%Y-%m-%dT%H:%M:%S%z")
-        self.__expiration = str(exp_formatted) if exp_formatted is not None else None
+    def expiration(self, expiration: str | datetime | None) -> None:
+        date_obj = None
+        if type(expiration) is datetime:
+            date_obj = expiration.astimezone(timezone.utc)
+        elif type(expiration) is str:
+            date_obj = dateparser.isoparse(expiration).astimezone(timezone.utc)
+        elif expiration:
+            raise ValueError("Invalid Expiration type")
+
+        self.__expiration = date_obj
 
     @property
     def temporary(self) -> bool:
         """Whether or not to use AWS' temporary credentials generation mechanism. The default value is False."""
         return self.__temporary
 
     @temporary.setter
     def temporary(self, temporary: bool):
         self.__temporary = bool(temporary)
 
-    def has_expired(self, exp_diff: int = 0, parse_pattern: Optional[str] = None):
+    def has_expired(self, exp_diff: int = 0):
         """
         This function assumes time will be provided in UTC per aws documentation
         and that the expiration time is a datetime str.
         :param exp_diff: the difference between expiration and current time in minutes (default to zero)
-        :param parse_pattern: is the pattern to parse for the expiration field (optional)
         :return: a boolean whether the token has expired or not
         :raise Value Error if expiration field cannot be parsed
         """
-        parse_pattern = "%Y-%m-%dT%H:%M:%S%z" if not parse_pattern else parse_pattern
         if not self.expiration:
             #if not field not set allow credentials to generated to set it
             return True
-        exp = datetime.strptime(self.expiration, parse_pattern)
-        diff = exp - datetime.now(timezone.utc)
+        diff = self.expiration - datetime.now(timezone.utc)
         return (diff.total_seconds() / 60) < exp_diff
 
     @property
     def type_display_name(self) -> str:
         return "AWS Credentials"
```

### Comparing `heaobject-1.6.2/src/heaobject/mimetype.py` & `heaobject-1.6.3/src/heaobject/mimetype.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/organization.py` & `heaobject-1.6.3/src/heaobject/organization.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/person.py` & `heaobject-1.6.3/src/heaobject/person.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,14 +312,43 @@
     def group_type(self, group_type: GroupType):
         if group_type is None:
             self.__group_type = GroupType.ADMIN
         else:
             self.__group_type = group_type if isinstance(group_type, GroupType) else GroupType[group_type]
 
 
+class AccessToken(AbstractDesktopObject):
+    def __init__(self):
+        super().__init__()
+        self.__id: str | None = None
+        self.__auth_scheme: str | None = None
+
+    @property
+    def id(self) -> str | None:
+        """
+        The IDC token issued by keycloak.
+        """
+        return self.__id
+
+    @id.setter
+    def id(self, id_: str | None):
+        self.__id = id_
+
+    @property
+    def auth_scheme(self) -> str | None:
+        """
+         The auth_scheme precedes the id token typically Bearer
+        """
+        return self.__auth_scheme if self.__auth_scheme else 'Bearer'
+
+    @auth_scheme.setter
+    def auth_scheme(self, auth_scheme: str | None):
+        self.__auth_scheme = auth_scheme
+
+
 def encode_role(role: str) -> str:
     """
     Encodes a role string using the Base 64 URL- and filesystem-safe alphabet, which replaces '+' with '-' and '/' with
     '_' in the base 64 alphabet as described in the IETF RFC 4648 specification section 5.
 
     :param role: the role string (required).
     :returns: returns the encoded data as a utf-8 string.
```

### Comparing `heaobject-1.6.2/src/heaobject/project.py` & `heaobject-1.6.3/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/registry.py` & `heaobject-1.6.3/src/heaobject/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Desktop and member objects that compose the HEA registry.
 """
 
 from . import root
 import yarl
 import copy
 from typing import Optional, List, Mapping, Union, Sequence
+
+from .user import ALL_USERS, NONE_USER
 from .volume import DEFAULT_FILE_SYSTEM
 from heaobject.volume import MongoDBFileSystem
 from heaobject.data import DataObject
 import uritemplate
 from uritemplate.orderedset import OrderedSet
 
 
@@ -159,14 +161,16 @@
     def is_creator_user(self, sub: str) -> bool:
         """
         Returns whether the user is in the creator user list.
 
         :param sub: the user (required).
         :return: True or False.
         """
+        if sub == NONE_USER:
+            return True
         return sub in self.__creator_users
 
     @property
     def collection_accessor_users(self) -> list[str]:
         """
         Users who can access desktop objects managed by this resource via a Collection. An empty list means no one can
         access these objects via a Collection. Getting the users will return a de-duplicated list.
```

### Comparing `heaobject-1.6.2/src/heaobject/root.py` & `heaobject-1.6.3/src/heaobject/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A collection of classes and interfaces supporting the construction of data transfer objects for moving data between
 HEA microservices as well as between a HEA microservice and a web browser or other client. The HEAObject is the root
 interface for these data transfer objects, and AbstractHEAObject provides a root abstract implementation for them.
 See HEAObject's docstring for details.
 """
 
 import json
-from datetime import date, time
+from datetime import date, time, datetime
 
 from humanize import naturalsize
 
 from .error import DeserializeException
 from .util import parse_bool
 from . import user
 from enum import auto, Enum
@@ -22,17 +22,17 @@
 import logging
 import importlib
 from copy import deepcopy
 from dateutil import parser as dateparser
 
 from .user import ALL_USERS
 
-PRIMITIVE_ATTRIBUTE_TYPES = (int, float, str, bool, Enum, type(None), date, time)
+PRIMITIVE_ATTRIBUTE_TYPES = (int, float, str, bool, Enum, type(None), date, time, datetime)
 
-Primitive = Optional[Union[int, float, str, bool, Enum, date, time]]
+Primitive = Optional[Union[int, float, str, bool, Enum, date, time, datetime]]
 MemberObjectDict = Dict[str, Union[Primitive, List[Primitive]]]
 HEAObjectDictValueTypeVar = TypeVar('HEAObjectDictValueTypeVar', List[MemberObjectDict], MemberObjectDict,
                                     List[Primitive], Primitive)
 HEAObjectDictValue = Optional[Union[List[MemberObjectDict], MemberObjectDict, List[Primitive], Primitive]]
 DesktopObjectDict = Dict[str, HEAObjectDictValueTypeVar]
 HEAObjectDict = Union[DesktopObjectDict, MemberObjectDict]
```

### Comparing `heaobject-1.6.2/src/heaobject/settings.py` & `heaobject-1.6.3/src/heaobject/settings.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/source2target.py` & `heaobject-1.6.3/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/storage.py` & `heaobject-1.6.3/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/trash.py` & `heaobject-1.6.3/src/heaobject/trash.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/user.py` & `heaobject-1.6.3/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject/volume.py` & `heaobject-1.6.3/src/heaobject/volume.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.2/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.6.3/src/heaobject.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.6.2
+Version: 1.6.3
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,19 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.3
+* credential's expiration type changed from str to datetime
+* registry in creator list no longer checks for NONE_USER
+* person now has access token object
+
 ## Version 1.6.2
 * Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
 
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
 
 ## Version 1.6.0
```

### Comparing `heaobject-1.6.2/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.6.3/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/emailcompat32crlf-1.0.0.tar.gz` & `tmp/emailcompat32crlf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailcompat32crlf-1.0.0.tar", last modified: Fri May 31 14:57:14 2024, max compression
+gzip compressed data, was "emailcompat32crlf-1.0.1.tar", last modified: Fri May 31 22:35:48 2024, max compression
```

## Comparing `emailcompat32crlf-1.0.0.tar` & `emailcompat32crlf-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-31 14:57:14.845021 emailcompat32crlf-1.0.0/
--rw-rw-r--   0 ale       (1000) ale       (1000)       57 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/MANIFEST.in
--rw-r--r--   0 ale       (1000) ale       (1000)     1632 2024-05-31 14:57:14.845021 emailcompat32crlf-1.0.0/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)     1173 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/README.rst
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-31 14:57:14.844021 emailcompat32crlf-1.0.0/emailcompat32clrf/
--rw-rw-r--   0 ale       (1000) ale       (1000)       93 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/emailcompat32clrf/__init__.py
-drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2024-05-31 14:57:14.845021 emailcompat32crlf-1.0.0/emailcompat32crlf.egg-info/
--rw-r--r--   0 ale       (1000) ale       (1000)     1632 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/emailcompat32crlf.egg-info/PKG-INFO
--rw-rw-r--   0 ale       (1000) ale       (1000)      265 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/emailcompat32crlf.egg-info/SOURCES.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/emailcompat32crlf.egg-info/dependency_links.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)        1 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/emailcompat32crlf.egg-info/not-zip-safe
--rw-rw-r--   0 ale       (1000) ale       (1000)       18 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/emailcompat32crlf.egg-info/top_level.txt
--rw-rw-r--   0 ale       (1000) ale       (1000)       38 2024-05-31 14:57:14.845021 emailcompat32crlf-1.0.0/setup.cfg
--rw-rw-r--   0 ale       (1000) ale       (1000)      696 2024-05-31 14:57:14.000000 emailcompat32crlf-1.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-31 22:35:48.997630 emailcompat32crlf-1.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)       57 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     2879 2024-05-31 22:35:48.997299 emailcompat32crlf-1.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2128 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-31 22:35:48.994704 emailcompat32crlf-1.0.1/emailcompat32crlf/
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/emailcompat32crlf/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-31 22:35:48.996775 emailcompat32crlf-1.0.1/emailcompat32crlf.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     2879 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/emailcompat32crlf.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      265 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/emailcompat32crlf.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/emailcompat32crlf.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/emailcompat32crlf.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       18 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/emailcompat32crlf.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-31 22:35:48.997752 emailcompat32crlf-1.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1011 2024-05-31 22:35:48.000000 emailcompat32crlf-1.0.1/setup.py
```

### Comparing `emailcompat32crlf-1.0.0/PKG-INFO` & `emailcompat32crlf-1.0.1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: emailcompat32crlf
-Version: 1.0.0
-Summary: Patch stdlib email compat32 policy to default to CRLF line endings.
-Home-page: https://github.com/collective/emailcompat32crlf
-Author: Guido Stevens
-Author-email: guido.stevens@cosent.net
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Communications :: Email
-
 Default to CRLF policy for compat32 emails
 ==========================================
 
 This is a minimal package. It patches the standard lib, so that it defaults to using
 ``\r\n`` as line endings, instead of the standard lib default ``\n``.
 
 Doing so makes emitted emails standards compliant.
@@ -23,16 +10,28 @@
 outlook.com or office365.com.
 
 The problem this package fixes, shows up as quoted-printable soft line endings
 ``=\n`` getting transformed into encoded equals signs ``=3D`` plus the removal
 of the first character following the newline. If you have URLs straddling a newline,
 those will not be valid anymore. But also normal text gets broken.
 
+Email policies
+--------------
+
+We patch the ``Compat32`` policy class and its ``compat32`` instance.
+There are other policies, like the ``EmailPolicy`` class (using ``\n`` as line separator) and its `SMTP` instance (using ``\r\n`` as line separator).  We do not touch those.
+
+Quoting from the `email.policy documentation <https://docs.python.org/3/library/email.policy.html>`_:
+
+* There is a default policy used by all classes in the email package. For all of the parser classes and the related convenience functions, and for the Message class, this is the ``Compat32`` policy, via its corresponding pre-defined instance ``compat32``. This policy provides for complete backward compatibility (in some cases, including bug compatibility) with the pre-Python3.3 version of the email package.
+* The default value for the policy keyword to ``EmailMessage`` is the ``EmailPolicy`` policy, via its pre-defined instance ``default``.
+
+
 Why patch the standard lib, instead of fixing your own code?
 ------------------------------------------------------------
 
 Because to fix your own code, you'd have to ensure to override the default
 policy in every single instantiation of every ``Message`` or ``MIMEText`` or any
 of the other constructors which default to the ``compat32`` policy
 without carriage returns.
 
-Instead, you now can simply add ``emailcompat32crlf`` to your project. Done.
+Instead, you now can simply add ``emailcompat32crlf`` to your project dependencies and import it. Done.
```

### Comparing `emailcompat32crlf-1.0.0/emailcompat32crlf.egg-info/PKG-INFO` & `emailcompat32crlf-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 Metadata-Version: 2.1
 Name: emailcompat32crlf
-Version: 1.0.0
+Version: 1.0.1
 Summary: Patch stdlib email compat32 policy to default to CRLF line endings.
 Home-page: https://github.com/collective/emailcompat32crlf
 Author: Guido Stevens
 Author-email: guido.stevens@cosent.net
 License: MIT
+Keywords: email
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Email
+Requires-Python: >=3.8
 
 Default to CRLF policy for compat32 emails
 ==========================================
 
 This is a minimal package. It patches the standard lib, so that it defaults to using
 ``\r\n`` as line endings, instead of the standard lib default ``\n``.
 
@@ -23,16 +30,28 @@
 outlook.com or office365.com.
 
 The problem this package fixes, shows up as quoted-printable soft line endings
 ``=\n`` getting transformed into encoded equals signs ``=3D`` plus the removal
 of the first character following the newline. If you have URLs straddling a newline,
 those will not be valid anymore. But also normal text gets broken.
 
+Email policies
+--------------
+
+We patch the ``Compat32`` policy class and its ``compat32`` instance.
+There are other policies, like the ``EmailPolicy`` class (using ``\n`` as line separator) and its `SMTP` instance (using ``\r\n`` as line separator).  We do not touch those.
+
+Quoting from the `email.policy documentation <https://docs.python.org/3/library/email.policy.html>`_:
+
+* There is a default policy used by all classes in the email package. For all of the parser classes and the related convenience functions, and for the Message class, this is the ``Compat32`` policy, via its corresponding pre-defined instance ``compat32``. This policy provides for complete backward compatibility (in some cases, including bug compatibility) with the pre-Python3.3 version of the email package.
+* The default value for the policy keyword to ``EmailMessage`` is the ``EmailPolicy`` policy, via its pre-defined instance ``default``.
+
+
 Why patch the standard lib, instead of fixing your own code?
 ------------------------------------------------------------
 
 Because to fix your own code, you'd have to ensure to override the default
 policy in every single instantiation of every ``Message`` or ``MIMEText`` or any
 of the other constructors which default to the ``compat32`` policy
 without carriage returns.
 
-Instead, you now can simply add ``emailcompat32crlf`` to your project. Done.
+Instead, you now can simply add ``emailcompat32crlf`` to your project dependencies and import it. Done.
```


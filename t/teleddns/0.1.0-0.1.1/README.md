# Comparing `tmp/teleddns-0.1.0.tar.gz` & `tmp/teleddns-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teleddns-0.1.0.tar", max compression
+gzip compressed data, was "teleddns-0.1.1.tar", max compression
```

## Comparing `teleddns-0.1.0.tar` & `teleddns-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-11-30 01:06:54.929564 teleddns-0.1.0/LICENSE
--rw-r--r--   0        0        0     6060 2024-06-01 01:03:55.430084 teleddns-0.1.0/README.md
--rw-r--r--   0        0        0      470 2024-06-01 00:54:34.542764 teleddns-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11197 2023-12-08 02:00:08.285550 teleddns-0.1.0/src/teleddns/__init__.py
--rw-r--r--   0        0        0     6840 1970-01-01 00:00:00.000000 teleddns-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-30 01:06:54.929564 teleddns-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6060 2024-06-01 01:03:55.430084 teleddns-0.1.1/README.md
+-rw-r--r--   0        0        0      470 2024-06-01 01:24:05.864443 teleddns-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11276 2024-06-01 01:20:46.923042 teleddns-0.1.1/src/teleddns/__init__.py
+-rw-r--r--   0        0        0     6840 1970-01-01 00:00:00.000000 teleddns-0.1.1/PKG-INFO
```

### Comparing `teleddns-0.1.0/LICENSE` & `teleddns-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `teleddns-0.1.0/README.md` & `teleddns-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `teleddns-0.1.0/src/teleddns/__init__.py` & `teleddns-0.1.1/src/teleddns/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 #
-# DDNSM
-# (C) 2015-2023 Tomas Hlavacek (tmshlvck@gmail.com)
+# TeleDDNS
+# (C) 2015-2024 Tomas Hlavacek (tmshlvck@gmail.com)
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -251,23 +251,24 @@
                 oldip4, oldip6, known_ipaddrs = ddns_client(config, oldip4, oldip6)
                 ddns_trigger = False
                 since_refresh = 0
         time.sleep(min_period)
         since_refresh += min_period
 
 
-DEFAULT_CONFIG='/etc/ddnsm/ddnsm.yaml'
+DEFAULT_CONFIG='/etc/teleddns/teleddns.yaml'
 
 @click.command()
-@click.option('-c', '--config', 'config_file', default=DEFAULT_CONFIG, help=f'DDNSM config file ({DEFAULT_CONFIG})')
+@click.option('-c', '--config', 'config_file', default=os.environ.get('TELEDDNS_CONFIG',DEFAULT_CONFIG),
+              help=f"override TELEDDNS_CONFIG env or defult {DEFAULT_CONFIG}")
 @click.option('-d', '--debug', 'debug', is_flag=True, help='Enable debugging output.')
 @click.option('-n', '--noexit', 'daemon', is_flag=True, help='Run in loop and keep wating for new IPs. Best for systemd simple service.')
 @click.option('-h', '--hash', 'hash', help="Hash password and exit.")
 def main(config_file, debug, daemon, hash):
-    """DDNSM client that can become a daemon."""
+    """TeleDDNS client that can become a daemon."""
     
     if hash:
         from passlib.context import CryptContext
         pwd_context = CryptContext(schemes=["bcrypt"], deprecated="auto")
         print(pwd_context.hash(hash))
         return 0
```

### Comparing `teleddns-0.1.0/PKG-INFO` & `teleddns-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teleddns
-Version: 0.1.0
+Version: 0.1.1
 Summary: Telephant Linux DDNS client
 License: GPL-3.0-or-later
 Author: Tomas Hlavacek
 Author-email: tmshlvck@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```


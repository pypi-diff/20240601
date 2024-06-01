# Comparing `tmp/pucoti-0.1.0.tar.gz` & `tmp/pucoti-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pucoti-0.1.0.tar", max compression
+gzip compressed data, was "pucoti-0.1.2.tar", max compression
```

## Comparing `pucoti-0.1.0.tar` & `pucoti-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0      965 2024-06-01 02:12:51.679957 pucoti-0.1.0/README.md
--rwxr-xr-x   0        0        0    12158 2024-06-01 01:48:11.102166 pucoti-0.1.0/pucoti.py
--rw-r--r--   0        0        0      429 2024-06-01 02:11:54.560923 pucoti-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 pucoti-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.1.2/COPYING
+-rw-r--r--   0        0        0     1222 2024-06-01 02:40:08.335744 pucoti-0.1.2/README.md
+-rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.1.2/bell.mp3
+-rwxr-xr-x   0        0        0    12849 2024-06-01 02:26:57.467326 pucoti-0.1.2/pucoti.py
+-rw-r--r--   0        0        0      616 2024-06-01 02:47:47.675989 pucoti-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 pucoti-0.1.2/PKG-INFO
```

### Comparing `pucoti-0.1.0/pucoti.py` & `pucoti-0.1.2/pucoti.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 #!/usr/bin/env python
 
+"""
+PUCOTI - A Purposeful Countdown Timer
+Copyright (C) 2024  Diego Dorn
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+
+
 from dataclasses import dataclass
 from functools import lru_cache
 import json
 import os
 import subprocess
 import sys
 from time import time
@@ -50,16 +69,14 @@
 Press any key to dismiss this message.
 """.strip()
 
 
 PURPOSE_HISTORY_FILE.parent.mkdir(parents=True, exist_ok=True)
 
 
-
-
 def fmt_time(seconds):
     if seconds < 0:
         return "-" + fmt_time(-seconds)
     minutes, seconds = divmod(seconds, 60)
     hours, minutes = divmod(minutes, 60)
     if hours:
         return "%d:%02d:%02d" % (hours, minutes, seconds)
```


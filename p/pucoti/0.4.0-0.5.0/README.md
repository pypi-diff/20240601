# Comparing `tmp/pucoti-0.4.0.tar.gz` & `tmp/pucoti-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pucoti-0.4.0.tar", max compression
+gzip compressed data, was "pucoti-0.5.0.tar", max compression
```

## Comparing `pucoti-0.4.0.tar` & `pucoti-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.4.0/COPYING
--rw-r--r--   0        0        0     1388 2024-06-01 15:37:43.579912 pucoti-0.4.0/README.md
--rw-r--r--   0        0        0   116584 2023-08-25 17:51:24.000000 pucoti-0.4.0/assets/Bevan-Regular.ttf
--rw-r--r--   0        0        0     4481 2024-06-01 12:32:12.000000 pucoti-0.4.0/assets/OFL-Bevan.txt
--rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.4.0/assets/bell.mp3
--rwxr-xr-x   0        0        0    16332 2024-06-01 15:33:23.490050 pucoti-0.4.0/pucoti.py
--rw-r--r--   0        0        0      688 2024-06-01 15:41:05.679342 pucoti-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 pucoti-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.5.0/COPYING
+-rw-r--r--   0        0        0     1588 2024-06-01 18:16:07.399874 pucoti-0.5.0/README.md
+-rw-r--r--   0        0        0   116584 2023-08-25 17:51:24.000000 pucoti-0.5.0/assets/Bevan-Regular.ttf
+-rw-r--r--   0        0        0     4481 2024-06-01 12:32:12.000000 pucoti-0.5.0/assets/OFL-Bevan.txt
+-rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.5.0/assets/bell.mp3
+-rwxr-xr-x   0        0        0    23583 2024-06-01 18:12:25.196938 pucoti-0.5.0/pucoti.py
+-rw-r--r--   0        0        0      688 2024-06-01 18:10:41.497964 pucoti-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2202 1970-01-01 00:00:00.000000 pucoti-0.5.0/PKG-INFO
```

### Comparing `pucoti-0.4.0/COPYING` & `pucoti-0.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `pucoti-0.4.0/assets/Bevan-Regular.ttf` & `pucoti-0.5.0/assets/Bevan-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pucoti-0.4.0/assets/OFL-Bevan.txt` & `pucoti-0.5.0/assets/OFL-Bevan.txt`

 * *Files identical despite different names*

### Comparing `pucoti-0.4.0/assets/bell.mp3` & `pucoti-0.5.0/assets/bell.mp3`

 * *Files identical despite different names*

### Comparing `pucoti-0.4.0/pyproject.toml` & `pucoti-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pucoti"
-version = "0.4.0"
+version = "0.5.0"
 description = "A Purposeful Countdown Timer"
 authors = ["ddorn <diego.dorn@free.fr>"]
 readme = "README.md"
 license = "GPL-3.0"
 homepage = "https://github.com/ddorn/pucoti"
 repository = "https://github.com/ddorn/pucoti"
 keywords = ["timer", "countdown", "pygame"]
```

### Comparing `pucoti-0.4.0/PKG-INFO` & `pucoti-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pucoti
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Purposeful Countdown Timer
 Home-page: https://github.com/ddorn/pucoti
 License: GPL-3.0
 Keywords: timer,countdown,pygame
 Author: ddorn
 Author-email: diego.dorn@free.fr
 Requires-Python: >=3.12,<4.0
@@ -34,18 +34,20 @@
 - **Configurable**: Change the bell sound, waste time changing colors, and more.
 - **Basic Controls**: Add or subtract time, reset the timer, but not more.
 
 PUCOTI is straightforward and gets the job done. Give it a try.
 
 ## Screenshots
 
-![Screenshot](./assets/screenshot.webp)
-*Pucoti can be big...*
-![Screenshot](./assets/screenshot-small.webp)
-*... or stay in a corner*
+### *Pucoti can be big...*
+![Screenshot of PUCOTI full-screen](./assets/screenshot.webp)
+### *... or stay in a corner*
+![Screenshot of PUCOTI in the bottom right of a screen](./assets/screenshot-small.webp)
+### *Keep track of your intentions*
+![Screenshot of PUCOTI showing the history of intentions](./assets/screenshot-history.webp)
 
 ## Installation
 
 You can easily install PUCOTI using pip. Follow these steps:
 
 1. **Install PUCOTI:**
    ```sh
```


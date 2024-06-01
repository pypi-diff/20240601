# Comparing `tmp/CTkKeyboard-0.3.4.tar.gz` & `tmp/CTkKeyboard-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkKeyboard-0.3.4.tar", last modified: Sat Jun  1 15:28:44 2024, max compression
+gzip compressed data, was "CTkKeyboard-0.3.5.tar", last modified: Sat Jun  1 15:31:49 2024, max compression
```

## Comparing `CTkKeyboard-0.3.4.tar` & `CTkKeyboard-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:28:44.980553 CTkKeyboard-0.3.4/
-drwxrwxrwx   0        0        0        0 2024-06-01 15:28:44.952694 CTkKeyboard-0.3.4/CTkKeyboard/
--rw-rw-rw-   0        0        0       28 2024-06-01 15:28:31.000000 CTkKeyboard-0.3.4/CTkKeyboard/__init__.py
--rw-rw-rw-   0        0        0       78 2024-06-01 15:28:37.000000 CTkKeyboard-0.3.4/CTkKeyboard/main.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:28:44.977228 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/
--rw-rw-rw-   0        0        0      118 2024-06-01 15:28:44.000000 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-06-01 15:28:44.000000 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:28:44.000000 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 15:28:44.000000 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2024-06-01 15:28:44.977228 CTkKeyboard-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-06-01 15:28:40.000000 CTkKeyboard-0.3.4/Setup.py
--rw-rw-rw-   0        0        0       42 2024-06-01 15:28:44.980553 CTkKeyboard-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:49.738459 CTkKeyboard-0.3.5/
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:49.723334 CTkKeyboard-0.3.5/CTkKeyboard/
+-rw-rw-rw-   0        0        0       28 2024-06-01 15:31:42.000000 CTkKeyboard-0.3.5/CTkKeyboard/__init__.py
+-rw-rw-rw-   0        0        0     7142 2024-06-01 15:31:41.000000 CTkKeyboard-0.3.5/CTkKeyboard/main.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:31:49.735804 CTkKeyboard-0.3.5/CTkKeyboard.egg-info/
+-rw-rw-rw-   0        0        0      118 2024-06-01 15:31:49.000000 CTkKeyboard-0.3.5/CTkKeyboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-06-01 15:31:49.000000 CTkKeyboard-0.3.5/CTkKeyboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:31:49.000000 CTkKeyboard-0.3.5/CTkKeyboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 15:31:49.000000 CTkKeyboard-0.3.5/CTkKeyboard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2024-06-01 15:31:49.736860 CTkKeyboard-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-06-01 15:31:39.000000 CTkKeyboard-0.3.5/Setup.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:31:49.739107 CTkKeyboard-0.3.5/setup.cfg
```


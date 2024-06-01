# Comparing `tmp/CTkKeyboard-0.3.3.tar.gz` & `tmp/CTkKeyboard-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkKeyboard-0.3.3.tar", last modified: Sat Jun  1 15:22:52 2024, max compression
+gzip compressed data, was "CTkKeyboard-0.3.4.tar", last modified: Sat Jun  1 15:28:44 2024, max compression
```

## Comparing `CTkKeyboard-0.3.3.tar` & `CTkKeyboard-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:22:52.007014 CTkKeyboard-0.3.3/
-drwxrwxrwx   0        0        0        0 2024-06-01 15:22:51.995212 CTkKeyboard-0.3.3/CTkKeyboard/
--rw-rw-rw-   0        0        0       76 2024-06-01 15:11:14.000000 CTkKeyboard-0.3.3/CTkKeyboard/Name.py
--rw-rw-rw-   0        0        0       35 2024-06-01 15:19:06.000000 CTkKeyboard-0.3.3/CTkKeyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:22:52.004006 CTkKeyboard-0.3.3/CTkKeyboard.egg-info/
--rw-rw-rw-   0        0        0      118 2024-06-01 15:22:51.000000 CTkKeyboard-0.3.3/CTkKeyboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-06-01 15:22:51.000000 CTkKeyboard-0.3.3/CTkKeyboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:22:51.000000 CTkKeyboard-0.3.3/CTkKeyboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 15:22:51.000000 CTkKeyboard-0.3.3/CTkKeyboard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2024-06-01 15:22:52.004006 CTkKeyboard-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-06-01 15:22:16.000000 CTkKeyboard-0.3.3/Setup.py
--rw-rw-rw-   0        0        0       42 2024-06-01 15:22:52.007014 CTkKeyboard-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 15:28:44.980553 CTkKeyboard-0.3.4/
+drwxrwxrwx   0        0        0        0 2024-06-01 15:28:44.952694 CTkKeyboard-0.3.4/CTkKeyboard/
+-rw-rw-rw-   0        0        0       28 2024-06-01 15:28:31.000000 CTkKeyboard-0.3.4/CTkKeyboard/__init__.py
+-rw-rw-rw-   0        0        0       78 2024-06-01 15:28:37.000000 CTkKeyboard-0.3.4/CTkKeyboard/main.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:28:44.977228 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/
+-rw-rw-rw-   0        0        0      118 2024-06-01 15:28:44.000000 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-06-01 15:28:44.000000 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:28:44.000000 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 15:28:44.000000 CTkKeyboard-0.3.4/CTkKeyboard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2024-06-01 15:28:44.977228 CTkKeyboard-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-06-01 15:28:40.000000 CTkKeyboard-0.3.4/Setup.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:28:44.980553 CTkKeyboard-0.3.4/setup.cfg
```


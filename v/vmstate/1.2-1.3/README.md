# Comparing `tmp/vmstate-1.2.tar.gz` & `tmp/vmstate-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmstate-1.2.tar", last modified: Sat Jun  1 20:42:53 2024, max compression
+gzip compressed data, was "vmstate-1.3.tar", last modified: Sat Jun  1 21:00:05 2024, max compression
```

## Comparing `vmstate-1.2.tar` & `vmstate-1.3.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:42:53.259348 vmstate-1.2/
--rw-r--r--   0 root         (0) root         (0)      329 2024-06-01 20:42:53.259348 vmstate-1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 20:42:53.259348 vmstate-1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      325 2024-06-01 20:42:05.000000 vmstate-1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:42:53.259348 vmstate-1.2/vmstate.egg-info/
--rw-r--r--   0 root         (0) root         (0)      329 2024-06-01 20:42:53.000000 vmstate-1.2/vmstate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      132 2024-06-01 20:42:53.000000 vmstate-1.2/vmstate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 20:42:53.000000 vmstate-1.2/vmstate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 20:42:53.000000 vmstate-1.2/vmstate.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:00:05.269355 vmstate-1.3/
+-rw-r--r--   0 root         (0) root         (0)      467 2024-06-01 21:00:05.269355 vmstate-1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       34 2024-06-01 20:53:28.000000 vmstate-1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 21:00:05.269355 vmstate-1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      807 2024-06-01 21:00:02.000000 vmstate-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:00:05.269355 vmstate-1.3/vmstate/
+-rw-r--r--   0 root         (0) root         (0)     3445 2024-06-01 20:52:45.000000 vmstate-1.3/vmstate/vmstate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 21:00:05.269355 vmstate-1.3/vmstate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      467 2024-06-01 21:00:05.000000 vmstate-1.3/vmstate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      161 2024-06-01 21:00:05.000000 vmstate-1.3/vmstate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 21:00:05.000000 vmstate-1.3/vmstate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-06-01 21:00:05.000000 vmstate-1.3/vmstate.egg-info/top_level.txt
```


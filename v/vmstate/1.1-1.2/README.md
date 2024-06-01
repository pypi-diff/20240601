# Comparing `tmp/vmstate-1.1.tar.gz` & `tmp/vmstate-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmstate-1.1.tar", last modified: Sat Jun  1 20:04:48 2024, max compression
+gzip compressed data, was "vmstate-1.2.tar", last modified: Sat Jun  1 20:42:53 2024, max compression
```

## Comparing `vmstate-1.1.tar` & `vmstate-1.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:04:48.049335 vmstate-1.1/
--rw-r--r--   0 root         (0) root         (0)      472 2024-06-01 20:04:48.049335 vmstate-1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2024-06-01 20:04:37.000000 vmstate-1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 20:04:48.049335 vmstate-1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      708 2024-06-01 20:01:45.000000 vmstate-1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:04:48.049335 vmstate-1.1/vmstate.egg-info/
--rw-r--r--   0 root         (0) root         (0)      472 2024-06-01 20:04:48.000000 vmstate-1.1/vmstate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2024-06-01 20:04:48.000000 vmstate-1.1/vmstate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 20:04:48.000000 vmstate-1.1/vmstate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 20:04:48.000000 vmstate-1.1/vmstate.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:42:53.259348 vmstate-1.2/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-06-01 20:42:53.259348 vmstate-1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 20:42:53.259348 vmstate-1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      325 2024-06-01 20:42:05.000000 vmstate-1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 20:42:53.259348 vmstate-1.2/vmstate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-06-01 20:42:53.000000 vmstate-1.2/vmstate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      132 2024-06-01 20:42:53.000000 vmstate-1.2/vmstate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 20:42:53.000000 vmstate-1.2/vmstate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 20:42:53.000000 vmstate-1.2/vmstate.egg-info/top_level.txt
```


# Comparing `tmp/pyconfig_util-1.0.1.tar.gz` & `tmp/pyconfig_util-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconfig_util-1.0.1.tar", last modified: Sat Mar 16 08:09:30 2024, max compression
+gzip compressed data, was "pyconfig_util-1.0.2.tar", last modified: Wed May  1 13:41:32 2024, max compression
```

## Comparing `pyconfig_util-1.0.1.tar` & `pyconfig_util-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:09:30.150976 pyconfig_util-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-16 08:09:18.000000 pyconfig_util-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-16 08:09:30.150976 pyconfig_util-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-16 08:09:18.000000 pyconfig_util-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:09:30.146976 pyconfig_util-1.0.1/pyconfig_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 08:09:18.000000 pyconfig_util-1.0.1/pyconfig_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-16 08:09:18.000000 pyconfig_util-1.0.1/pyconfig_util/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:09:30.150976 pyconfig_util-1.0.1/pyconfig_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-16 08:09:30.000000 pyconfig_util-1.0.1/pyconfig_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-16 08:09:30.000000 pyconfig_util-1.0.1/pyconfig_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 08:09:30.000000 pyconfig_util-1.0.1/pyconfig_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-16 08:09:30.000000 pyconfig_util-1.0.1/pyconfig_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-16 08:09:30.000000 pyconfig_util-1.0.1/pyconfig_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 08:09:30.000000 pyconfig_util-1.0.1/pyconfig_util.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 08:09:30.150976 pyconfig_util-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-16 08:09:18.000000 pyconfig_util-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:41:32.341922 pyconfig_util-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-01 13:41:32.337922 pyconfig_util-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:41:32.337922 pyconfig_util-1.0.2/pyconfig_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/pyconfig_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/pyconfig_util/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:41:32.337922 pyconfig_util-1.0.2/pyconfig_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:41:32.000000 pyconfig_util-1.0.2/pyconfig_util.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:41:32.341922 pyconfig_util-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-01 13:41:24.000000 pyconfig_util-1.0.2/setup.py
```

### Comparing `pyconfig_util-1.0.1/LICENSE` & `pyconfig_util-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconfig_util-1.0.1/pyconfig_util/config_util.py` & `pyconfig_util-1.0.2/pyconfig_util/config_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,11 @@
                 # 如果值是字典，则处理字典中的键值对
                 for key, item_value in value.items():
                     attr_name = "{}_{}".format(section.upper(), key.upper())
                     setattr(self, attr_name, item_value)
             else:
                 # 如果值不是字典，则直接将该值作为属性添加到实例中
                 attr_name = section.upper()
-                setattr(self, attr_name, value)
+                setattr(self, attr_name, value)
+
+
+setting = Setting()
```

### Comparing `pyconfig_util-1.0.1/setup.py` & `pyconfig_util-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with io.open("requirements.txt", 'r') as f:
     install_requires = f.read().split(os.sep)
 
 
 setup(
     name='pyconfig_util',
-    version='1.0.1',
+    version='1.0.2',
     description='config助手',
     author='buyfakett',
     author_email='buyfakett@vip.qq.com',
     license='MIT',
     url="https://github.com/buyfakett",
     packages=find_packages(),  # packages=["pytest"],
     long_description=long_description,
```


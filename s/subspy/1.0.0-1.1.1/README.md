# Comparing `tmp/subspy-1.0.0.tar.gz` & `tmp/subspy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subspy-1.0.0.tar", last modified: Fri May 31 18:19:19 2024, max compression
+gzip compressed data, was "subspy-1.1.1.tar", last modified: Sat Jun  1 05:16:07 2024, max compression
```

## Comparing `subspy-1.0.0.tar` & `subspy-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 18:19:19.819714 subspy-1.0.0/
--rw-rw-rw-   0        0        0      706 2024-05-31 18:19:19.818713 subspy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       15 2024-05-31 18:19:08.000000 subspy-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-31 18:19:19.819714 subspy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1152 2024-05-31 18:13:22.000000 subspy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 18:19:19.774071 subspy-1.0.0/subspy/
--rw-rw-rw-   0        0        0       13 2024-05-31 18:15:46.000000 subspy-1.0.0/subspy/__init__.py
--rw-rw-rw-   0        0        0      286 2024-05-31 18:17:25.000000 subspy-1.0.0/subspy/banner.py
--rw-rw-rw-   0        0        0     1475 2024-05-31 18:14:56.000000 subspy-1.0.0/subspy/cli.py
--rw-rw-rw-   0        0        0       59 2024-05-31 18:15:19.000000 subspy-1.0.0/subspy/default_subdomains.txt
--rw-rw-rw-   0        0        0     1582 2024-05-31 18:14:29.000000 subspy-1.0.0/subspy/subdomain.py
-drwxrwxrwx   0        0        0        0 2024-05-31 18:19:19.817108 subspy-1.0.0/subspy.egg-info/
--rw-rw-rw-   0        0        0      706 2024-05-31 18:19:19.000000 subspy-1.0.0/subspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-05-31 18:19:19.000000 subspy-1.0.0/subspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 18:19:19.000000 subspy-1.0.0/subspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-31 18:19:19.000000 subspy-1.0.0/subspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 18:19:19.000000 subspy-1.0.0/subspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-31 18:19:19.000000 subspy-1.0.0/subspy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 05:16:07.450798 subspy-1.1.1/
+-rw-rw-rw-   0        0        0     2426 2024-06-01 05:16:07.450798 subspy-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1687 2024-06-01 05:10:53.000000 subspy-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 05:16:07.450798 subspy-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2024-06-01 05:15:18.000000 subspy-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:16:07.419552 subspy-1.1.1/subspy/
+-rw-rw-rw-   0        0        0      258 2024-06-01 05:10:53.000000 subspy-1.1.1/subspy/__init__.py
+-rw-rw-rw-   0        0        0     2176 2024-06-01 05:10:53.000000 subspy-1.1.1/subspy/cli.py
+-rw-rw-rw-   0        0        0       59 2024-06-01 05:10:53.000000 subspy-1.1.1/subspy/default_subdomains.txt
+-rw-rw-rw-   0        0        0     1458 2024-06-01 05:10:53.000000 subspy-1.1.1/subspy/subdomain.py
+drwxrwxrwx   0        0        0        0 2024-06-01 05:16:07.450798 subspy-1.1.1/subspy.egg-info/
+-rw-rw-rw-   0        0        0     2426 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 05:16:07.000000 subspy-1.1.1/subspy.egg-info/top_level.txt
```

### Comparing `subspy-1.0.0/setup.py` & `subspy-1.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r', encoding='utf-8') as readme_file:
+    long_description = readme_file.read()
+
 setup(
     name='subspy',
-    version='1.0.0',
+    version='1.1.1',
     description='SubSpy: A tool for subdomain enumeration.',
-    long_description=open('README.md').read(),
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/subspy',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `subspy-1.0.0/subspy/subdomain.py` & `subspy-1.1.1/subspy/subdomain.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     fixed_url = fix_url(url)
     for idx, subdomain in enumerate(subdomains, start=1):
         url_with_subdomain = f"https://{subdomain}.{fixed_url}"
         tried_subdomains.append(url_with_subdomain)
         available, status_code = is_subdomain_available(url_with_subdomain)
         if available:
             found_subdomains.append(subdomain)
-            print(f"\033[97m ({idx}/{len(subdomains)}) [\033[92m+\033[97m] \033[92mSubdomain found : {subdomain}.{fixed_url} \033[97m(\033[92mStatus Code : {status_code}\033[97m)")
+            print(f" ({idx}/{len(subdomains)}) Subdomain found : {subdomain}.{fixed_url} Status Code : {status_code}")
         else:
-            print(f"\033[97m ({idx}/{len(subdomains)}) [\033[91m+\033[97m] \033[91mWrong Subdomain : {subdomain}.{fixed_url} \033[97m(\033[91mStatus Code : {status_code}\033[97m)")
+            print(f" ({idx}/{len(subdomains)}) Wrong Subdomain : {subdomain}.{fixed_url} Status Code : {status_code}")
 
     return found_subdomains
 
 def get_default_subdomains():
     current_dir = os.path.dirname(__file__)
     default_subdomains_path = os.path.join(current_dir, "default_subdomains.txt")
     with open(default_subdomains_path, "r") as file:
```


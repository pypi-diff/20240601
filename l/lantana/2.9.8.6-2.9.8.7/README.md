# Comparing `tmp/lantana-2.9.8.6.tar.gz` & `tmp/lantana-2.9.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lantana-2.9.8.6.tar", last modified: Sun May 26 09:46:19 2024, max compression
+gzip compressed data, was "lantana-2.9.8.7.tar", last modified: Sat Jun  1 13:25:40 2024, max compression
```

## Comparing `lantana-2.9.8.6.tar` & `lantana-2.9.8.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:19.061536 lantana-2.9.8.6/
--rw-rw-rw-   0        0        0     1083 2022-10-28 14:22:28.000000 lantana-2.9.8.6/LICENCE.md
--rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.9.8.6/MANIFEST.in
--rw-rw-rw-   0        0        0      239 2024-05-26 09:46:19.060536 lantana-2.9.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.9.8.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:19.031169 lantana-2.9.8.6/lantana/
--rw-rw-rw-   0        0        0      829 2024-04-03 03:18:14.000000 lantana-2.9.8.6/lantana/404.html
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8.6/lantana/__init__.py
--rw-rw-rw-   0        0        0     2731 2024-03-07 12:04:46.000000 lantana-2.9.8.6/lantana/__main__.py
--rw-rw-rw-   0        0        0        0 2023-06-28 13:19:19.000000 lantana-2.9.8.6/lantana/after_header.html
--rw-rw-rw-   0        0        0        0 2024-05-26 09:17:07.000000 lantana-2.9.8.6/lantana/after_nav_tool.html
--rw-rw-rw-   0        0        0     9493 2024-04-19 06:39:06.000000 lantana-2.9.8.6/lantana/base.html
--rw-rw-rw-   0        0        0        0 2023-06-28 13:14:52.000000 lantana-2.9.8.6/lantana/before_header.html
--rw-rw-rw-   0        0        0      306 2023-08-26 17:00:51.000000 lantana-2.9.8.6/lantana/breadcrumb.html
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:19.042548 lantana-2.9.8.6/lantana/css/
--rw-rw-rw-   0        0        0    85883 2024-04-19 06:40:56.000000 lantana-2.9.8.6/lantana/css/bootstrap-icons.min.css
--rw-rw-rw-   0        0        0   224443 2024-03-18 09:06:45.000000 lantana-2.9.8.6/lantana/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     1152 2024-03-18 13:45:00.000000 lantana-2.9.8.6/lantana/css/default.min.css
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:19.044536 lantana-2.9.8.6/lantana/css/fonts/
--rw-rw-rw-   0        0        0   176032 2024-04-19 06:23:31.000000 lantana-2.9.8.6/lantana/css/fonts/bootstrap-icons.woff.css
--rw-rw-rw-   0        0        0   130396 2024-04-19 06:23:31.000000 lantana-2.9.8.6/lantana/css/fonts/bootstrap-icons.woff2.css
--rw-rw-rw-   0        0        0     3949 2024-05-06 12:45:53.000000 lantana-2.9.8.6/lantana/css/theme.css
--rw-rw-rw-   0        0        0     1927 2024-03-18 13:47:24.000000 lantana-2.9.8.6/lantana/css/vs.min.css
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:19.055535 lantana-2.9.8.6/lantana/extensions/
--rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8.6/lantana/extensions/__init__.py
--rw-rw-rw-   0        0        0     2714 2024-03-18 13:02:35.000000 lantana-2.9.8.6/lantana/extensions/accordion.py
--rw-rw-rw-   0        0        0     3930 2024-05-06 13:25:21.000000 lantana-2.9.8.6/lantana/extensions/alerts.py
--rw-rw-rw-   0        0        0     4704 2024-05-06 17:26:51.000000 lantana-2.9.8.6/lantana/extensions/alerts2.py
--rw-rw-rw-   0        0        0     4553 2024-04-03 02:58:18.000000 lantana-2.9.8.6/lantana/extensions/cards.py
--rw-rw-rw-   0        0        0     2116 2024-03-11 07:11:53.000000 lantana-2.9.8.6/lantana/extensions/codeblock_copybtn.py
--rw-rw-rw-   0        0        0     1889 2024-05-06 17:43:29.000000 lantana-2.9.8.6/lantana/extensions/lantana.py
--rw-rw-rw-   0        0        0      882 2024-03-11 07:41:11.000000 lantana-2.9.8.6/lantana/extensions/link_opennewtab.py
--rw-rw-rw-   0        0        0     1996 2024-05-06 10:05:23.000000 lantana-2.9.8.6/lantana/extensions/mdx_embedly.py
--rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.9.8.6/lantana/extensions/mdx_wsid.py
--rw-rw-rw-   0        0        0     1380 2024-03-11 05:31:11.000000 lantana-2.9.8.6/lantana/extensions/mermaid_precompile.py
--rw-rw-rw-   0        0        0     2021 2024-05-06 17:30:11.000000 lantana-2.9.8.6/lantana/extensions/selector.py
--rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.9.8.6/lantana/favicon.png
--rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.9.8.6/lantana/favicon.svg
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:19.060536 lantana-2.9.8.6/lantana/js/
--rw-rw-rw-   0        0        0    78749 2023-07-07 13:01:47.000000 lantana-2.9.8.6/lantana/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.9.8.6/lantana/js/highlight.min.js
--rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.9.8.6/lantana/js/jquery-3.6.1.slim.min.js
--rw-rw-rw-   0        0        0     3727 2024-03-11 07:44:04.000000 lantana-2.9.8.6/lantana/js/theme.js
--rw-rw-rw-   0        0        0     5678 2024-05-26 09:45:51.000000 lantana-2.9.8.6/lantana/main.html
--rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.9.8.6/lantana/mkdocs_theme.yml
--rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.9.8.6/lantana/nav.html
--rw-rw-rw-   0        0        0     1994 2024-04-19 06:45:51.000000 lantana-2.9.8.6/lantana/statics.html
--rw-rw-rw-   0        0        0      396 2024-04-03 03:19:38.000000 lantana-2.9.8.6/lantana/toc.html
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:19.037536 lantana-2.9.8.6/lantana.egg-info/
--rw-rw-rw-   0        0        0      239 2024-05-26 09:46:18.000000 lantana-2.9.8.6/lantana.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1317 2024-05-26 09:46:18.000000 lantana-2.9.8.6/lantana.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:46:18.000000 lantana-2.9.8.6/lantana.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      852 2024-05-26 09:46:18.000000 lantana-2.9.8.6/lantana.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-26 09:46:18.000000 lantana-2.9.8.6/lantana.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      275 2024-05-26 09:46:18.000000 lantana-2.9.8.6/lantana.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 09:46:18.000000 lantana-2.9.8.6/lantana.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 09:46:19.061536 lantana-2.9.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1877 2024-05-26 09:45:59.000000 lantana-2.9.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:25:40.525824 lantana-2.9.8.7/
+-rw-rw-rw-   0        0        0     1083 2022-10-28 14:22:28.000000 lantana-2.9.8.7/LICENCE.md
+-rw-rw-rw-   0        0        0      124 2022-10-28 12:09:36.000000 lantana-2.9.8.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      239 2024-06-01 13:25:40.525824 lantana-2.9.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-03-04 05:20:30.000000 lantana-2.9.8.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:25:40.463360 lantana-2.9.8.7/lantana/
+-rw-rw-rw-   0        0        0      829 2024-04-03 03:18:14.000000 lantana-2.9.8.7/lantana/404.html
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8.7/lantana/__init__.py
+-rw-rw-rw-   0        0        0     2731 2024-03-07 12:04:46.000000 lantana-2.9.8.7/lantana/__main__.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 13:19:19.000000 lantana-2.9.8.7/lantana/after_header.html
+-rw-rw-rw-   0        0        0        0 2024-05-26 09:17:07.000000 lantana-2.9.8.7/lantana/after_nav_tool.html
+-rw-rw-rw-   0        0        0     9458 2024-06-01 13:25:17.000000 lantana-2.9.8.7/lantana/base.html
+-rw-rw-rw-   0        0        0        0 2023-06-28 13:14:52.000000 lantana-2.9.8.7/lantana/before_header.html
+-rw-rw-rw-   0        0        0      306 2023-08-26 17:00:51.000000 lantana-2.9.8.7/lantana/breadcrumb.html
+drwxrwxrwx   0        0        0        0 2024-06-01 13:25:40.510199 lantana-2.9.8.7/lantana/css/
+-rw-rw-rw-   0        0        0    85883 2024-04-19 06:40:56.000000 lantana-2.9.8.7/lantana/css/bootstrap-icons.min.css
+-rw-rw-rw-   0        0        0   224443 2024-03-18 09:06:45.000000 lantana-2.9.8.7/lantana/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1152 2024-03-18 13:45:00.000000 lantana-2.9.8.7/lantana/css/default.min.css
+drwxrwxrwx   0        0        0        0 2024-06-01 13:25:40.510199 lantana-2.9.8.7/lantana/css/fonts/
+-rw-rw-rw-   0        0        0   176032 2024-04-19 06:23:31.000000 lantana-2.9.8.7/lantana/css/fonts/bootstrap-icons.woff.css
+-rw-rw-rw-   0        0        0   130396 2024-04-19 06:23:31.000000 lantana-2.9.8.7/lantana/css/fonts/bootstrap-icons.woff2.css
+-rw-rw-rw-   0        0        0     3949 2024-05-06 12:45:53.000000 lantana-2.9.8.7/lantana/css/theme.css
+-rw-rw-rw-   0        0        0     1927 2024-03-18 13:47:24.000000 lantana-2.9.8.7/lantana/css/vs.min.css
+drwxrwxrwx   0        0        0        0 2024-06-01 13:25:40.510199 lantana-2.9.8.7/lantana/extensions/
+-rw-rw-rw-   0        0        0        0 2022-10-28 12:09:36.000000 lantana-2.9.8.7/lantana/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2714 2024-03-18 13:02:35.000000 lantana-2.9.8.7/lantana/extensions/accordion.py
+-rw-rw-rw-   0        0        0     3930 2024-05-06 13:25:21.000000 lantana-2.9.8.7/lantana/extensions/alerts.py
+-rw-rw-rw-   0        0        0     4704 2024-05-06 17:26:51.000000 lantana-2.9.8.7/lantana/extensions/alerts2.py
+-rw-rw-rw-   0        0        0     4553 2024-04-03 02:58:18.000000 lantana-2.9.8.7/lantana/extensions/cards.py
+-rw-rw-rw-   0        0        0     2116 2024-03-11 07:11:53.000000 lantana-2.9.8.7/lantana/extensions/codeblock_copybtn.py
+-rw-rw-rw-   0        0        0     1889 2024-05-06 17:43:29.000000 lantana-2.9.8.7/lantana/extensions/lantana.py
+-rw-rw-rw-   0        0        0      882 2024-03-11 07:41:11.000000 lantana-2.9.8.7/lantana/extensions/link_opennewtab.py
+-rw-rw-rw-   0        0        0     1996 2024-05-06 10:05:23.000000 lantana-2.9.8.7/lantana/extensions/mdx_embedly.py
+-rw-rw-rw-   0        0        0     2138 2023-03-08 08:22:38.000000 lantana-2.9.8.7/lantana/extensions/mdx_wsid.py
+-rw-rw-rw-   0        0        0     1380 2024-03-11 05:31:11.000000 lantana-2.9.8.7/lantana/extensions/mermaid_precompile.py
+-rw-rw-rw-   0        0        0     2021 2024-05-06 17:30:11.000000 lantana-2.9.8.7/lantana/extensions/selector.py
+-rw-rw-rw-   0        0        0     1784 2022-10-28 12:09:36.000000 lantana-2.9.8.7/lantana/favicon.png
+-rw-rw-rw-   0        0        0     4486 2022-10-28 12:09:36.000000 lantana-2.9.8.7/lantana/favicon.svg
+drwxrwxrwx   0        0        0        0 2024-06-01 13:25:40.525824 lantana-2.9.8.7/lantana/js/
+-rw-rw-rw-   0        0        0    78749 2023-07-07 13:01:47.000000 lantana-2.9.8.7/lantana/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   126355 2023-05-21 06:59:30.000000 lantana-2.9.8.7/lantana/js/highlight.min.js
+-rw-rw-rw-   0        0        0    72535 2023-05-21 06:58:42.000000 lantana-2.9.8.7/lantana/js/jquery-3.6.1.slim.min.js
+-rw-rw-rw-   0        0        0     3727 2024-03-11 07:44:04.000000 lantana-2.9.8.7/lantana/js/theme.js
+-rw-rw-rw-   0        0        0     5678 2024-05-26 09:45:51.000000 lantana-2.9.8.7/lantana/main.html
+-rw-rw-rw-   0        0        0      360 2023-02-09 08:21:12.000000 lantana-2.9.8.7/lantana/mkdocs_theme.yml
+-rw-rw-rw-   0        0        0      843 2023-03-04 05:20:30.000000 lantana-2.9.8.7/lantana/nav.html
+-rw-rw-rw-   0        0        0     1994 2024-04-19 06:45:51.000000 lantana-2.9.8.7/lantana/statics.html
+-rw-rw-rw-   0        0        0      396 2024-04-03 03:19:38.000000 lantana-2.9.8.7/lantana/toc.html
+drwxrwxrwx   0        0        0        0 2024-06-01 13:25:40.494606 lantana-2.9.8.7/lantana.egg-info/
+-rw-rw-rw-   0        0        0      239 2024-06-01 13:25:40.000000 lantana-2.9.8.7/lantana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1317 2024-06-01 13:25:40.000000 lantana-2.9.8.7/lantana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:25:40.000000 lantana-2.9.8.7/lantana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      852 2024-06-01 13:25:40.000000 lantana-2.9.8.7/lantana.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-06-01 13:25:40.000000 lantana-2.9.8.7/lantana.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      275 2024-06-01 13:25:40.000000 lantana-2.9.8.7/lantana.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 13:25:40.000000 lantana-2.9.8.7/lantana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 13:25:40.525824 lantana-2.9.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1877 2024-06-01 13:25:29.000000 lantana-2.9.8.7/setup.py
```

### Comparing `lantana-2.9.8.6/LICENCE.md` & `lantana-2.9.8.7/LICENCE.md`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/README.md` & `lantana-2.9.8.7/README.md`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/404.html` & `lantana-2.9.8.7/lantana/404.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/__main__.py` & `lantana-2.9.8.7/lantana/__main__.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/base.html` & `lantana-2.9.8.7/lantana/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       <meta property="og:image" content="{{ page.meta.image|url }}" />
     {% else %}
       <meta property="og:image" content="{{ config.image|url }}" />
     {% endif %}
   {% endif %}
 
   {% if page and page.meta and page.meta.long_title %}
-    <title>{% if page.meta.long_title %}{{ page.title }} | {% endif %}{% if config.site_short_name %}{{ config.site_short_name }}{% else %}{{ config.site_name }}{% endif %}</title>
+    <title>{{ page.long_title }} | {% if config.site_short_name %}{{ config.site_short_name }}{% else %}{{ config.site_name }}{% endif %}</title>
   {% else %}
   <title>{% if page.title %}{{ page.title }} | {% endif %}{% if config.site_short_name %}{{ config.site_short_name }}{% else %}{{ config.site_name }}{% endif %}</title>
   {% endif %}
 
   {% if config.favicon %}
     <link rel="favicon" href="{{ config.favicon|url }}">
   {% endif %}
```

### Comparing `lantana-2.9.8.6/lantana/css/bootstrap-icons.min.css` & `lantana-2.9.8.7/lantana/css/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/css/bootstrap.min.css` & `lantana-2.9.8.7/lantana/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/css/default.min.css` & `lantana-2.9.8.7/lantana/css/default.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/css/fonts/bootstrap-icons.woff.css` & `lantana-2.9.8.7/lantana/css/fonts/bootstrap-icons.woff.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/css/fonts/bootstrap-icons.woff2.css` & `lantana-2.9.8.7/lantana/css/fonts/bootstrap-icons.woff2.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/css/theme.css` & `lantana-2.9.8.7/lantana/css/theme.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/css/vs.min.css` & `lantana-2.9.8.7/lantana/css/vs.min.css`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/accordion.py` & `lantana-2.9.8.7/lantana/extensions/accordion.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/alerts.py` & `lantana-2.9.8.7/lantana/extensions/alerts.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/alerts2.py` & `lantana-2.9.8.7/lantana/extensions/alerts2.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/cards.py` & `lantana-2.9.8.7/lantana/extensions/cards.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/codeblock_copybtn.py` & `lantana-2.9.8.7/lantana/extensions/codeblock_copybtn.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/lantana.py` & `lantana-2.9.8.7/lantana/extensions/lantana.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/link_opennewtab.py` & `lantana-2.9.8.7/lantana/extensions/link_opennewtab.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/mdx_embedly.py` & `lantana-2.9.8.7/lantana/extensions/mdx_embedly.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/mdx_wsid.py` & `lantana-2.9.8.7/lantana/extensions/mdx_wsid.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/mermaid_precompile.py` & `lantana-2.9.8.7/lantana/extensions/mermaid_precompile.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/extensions/selector.py` & `lantana-2.9.8.7/lantana/extensions/selector.py`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/favicon.png` & `lantana-2.9.8.7/lantana/favicon.png`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/favicon.svg` & `lantana-2.9.8.7/lantana/favicon.svg`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/js/bootstrap.bundle.min.js` & `lantana-2.9.8.7/lantana/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/js/highlight.min.js` & `lantana-2.9.8.7/lantana/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/js/jquery-3.6.1.slim.min.js` & `lantana-2.9.8.7/lantana/js/jquery-3.6.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/js/theme.js` & `lantana-2.9.8.7/lantana/js/theme.js`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/main.html` & `lantana-2.9.8.7/lantana/main.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/nav.html` & `lantana-2.9.8.7/lantana/nav.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana/statics.html` & `lantana-2.9.8.7/lantana/statics.html`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana.egg-info/SOURCES.txt` & `lantana-2.9.8.7/lantana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/lantana.egg-info/entry_points.txt` & `lantana-2.9.8.7/lantana.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lantana-2.9.8.6/setup.py` & `lantana-2.9.8.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.9.8.6'
+VERSION = '2.9.8.7'
 
 setup(
     name="lantana",
     version=VERSION,
     url='https://lantana.wsoft.ws/',
     license='MIT',
     description='Bootstrap theme for MkDocs',
```


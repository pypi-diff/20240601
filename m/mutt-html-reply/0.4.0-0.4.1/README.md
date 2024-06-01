# Comparing `tmp/mutt_html_reply-0.4.0.tar.gz` & `tmp/mutt_html_reply-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutt_html_reply-0.4.0.tar", last modified: Fri May 31 03:30:55 2024, max compression
+gzip compressed data, was "mutt_html_reply-0.4.1.tar", last modified: Sat Jun  1 00:53:46 2024, max compression
```

## Comparing `mutt_html_reply-0.4.0.tar` & `mutt_html_reply-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-31 03:30:55.044740 mutt_html_reply-0.4.0/
--rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.4.0/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-05-31 03:30:55.044740 mutt_html_reply-0.4.0/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      807 2024-05-30 03:23:26.000000 mutt_html_reply-0.4.0/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-05-31 03:30:06.000000 mutt_html_reply-0.4.0/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-31 03:30:55.044740 mutt_html_reply-0.4.0/setup.cfg
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-31 03:30:55.044740 mutt_html_reply-0.4.0/src/
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-31 03:30:55.044740 mutt_html_reply-0.4.0/src/mutt_html_reply/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.4.0/src/mutt_html_reply/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4519 2024-05-31 03:28:11.000000 mutt_html_reply-0.4.0/src/mutt_html_reply/mutt_html_reply.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-31 03:30:55.044740 mutt_html_reply-0.4.0/src/mutt_html_reply.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-05-31 03:30:55.000000 mutt_html_reply-0.4.0/src/mutt_html_reply.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-05-31 03:30:55.000000 mutt_html_reply-0.4.0/src/mutt_html_reply.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-31 03:30:55.000000 mutt_html_reply-0.4.0/src/mutt_html_reply.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-05-31 03:30:55.000000 mutt_html_reply-0.4.0/src/mutt_html_reply.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-05-31 03:30:55.000000 mutt_html_reply-0.4.0/src/mutt_html_reply.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-05-31 03:30:55.000000 mutt_html_reply-0.4.0/src/mutt_html_reply.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-01 00:53:46.792389 mutt_html_reply-0.4.1/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.4.1/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-06-01 00:53:46.792389 mutt_html_reply-0.4.1/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      807 2024-05-30 03:23:26.000000 mutt_html_reply-0.4.1/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-06-01 00:53:03.000000 mutt_html_reply-0.4.1/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-06-01 00:53:46.792389 mutt_html_reply-0.4.1/setup.cfg
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-01 00:53:46.792389 mutt_html_reply-0.4.1/src/
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-01 00:53:46.792389 mutt_html_reply-0.4.1/src/mutt_html_reply/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.4.1/src/mutt_html_reply/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4894 2024-05-31 20:11:54.000000 mutt_html_reply-0.4.1/src/mutt_html_reply/mutt_html_reply.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-06-01 00:53:46.792389 mutt_html_reply-0.4.1/src/mutt_html_reply.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2354 2024-06-01 00:53:46.000000 mutt_html_reply-0.4.1/src/mutt_html_reply.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-06-01 00:53:46.000000 mutt_html_reply-0.4.1/src/mutt_html_reply.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-06-01 00:53:46.000000 mutt_html_reply-0.4.1/src/mutt_html_reply.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-06-01 00:53:46.000000 mutt_html_reply-0.4.1/src/mutt_html_reply.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-06-01 00:53:46.000000 mutt_html_reply-0.4.1/src/mutt_html_reply.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-06-01 00:53:46.000000 mutt_html_reply-0.4.1/src/mutt_html_reply.egg-info/top_level.txt
```

### Comparing `mutt_html_reply-0.4.0/LICENSE` & `mutt_html_reply-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.4.0/PKG-INFO` & `mutt_html_reply-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutt-html-reply
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create an Outlook-style HTML reply
 Author-email: Erik Rogers <erik@rogers-family.net>
 Maintainer-email: Erik Rogers <erik@rogers-family.net>
 License: Copyright © 2024 Erik Rogers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `mutt_html_reply-0.4.0/README.md` & `mutt_html_reply-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.4.0/pyproject.toml` & `mutt_html_reply-0.4.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mutt-html-reply"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
 	"bs4",
 	"css_inline"
 ]
 authors = [
 	{name = "Erik Rogers", email = "erik@rogers-family.net"}
 ]
```

### Comparing `mutt_html_reply-0.4.0/src/mutt_html_reply/mutt_html_reply.py` & `mutt_html_reply-0.4.1/src/mutt_html_reply/mutt_html_reply.py`

 * *Files 26% similar despite different names*

```diff
@@ -62,28 +62,39 @@
     bs4_final.body.append(bs4_original_msg) #type: ignore
 
     # Write output
     args.output.write(str(bs4_final))
 
 
 def _get_header_html(message):
-    headers = ''
+    headers = '''\
+        <div>
+        <div style=&quot;border:none;border-top:solid;padding:3.0pt 0in 0in 0in&quot;>
+        <span style=font-size:11.0pt;font-family:&quot;Calibri&quot;,sans-serif>
+        '''
     if message['from'] is not None:
-        headers = '<b>From</b>: ' + html.escape(message['from']) + '<br></br>'
+        headers = headers + '<b>From:</b> ' + html.escape(message['from'].replace('"','')) + '<br></br>'
     if message['date'] is not None:
-        headers = headers + '<b>Date</b>: ' + html.escape(message['date']) + '<br></br>'
+        headers = headers + '<b>Sent:</b> ' + html.escape(message['date'].replace('"','')) + '<br></br>'
     if message['to'] is not None:
-        headers = headers + '<b>To</b>: ' + html.escape(message['to']) + '<br></br>'
+        headers = headers + '<b>To:</b> ' + html.escape(message['to'].replace('"','')) + '<br></br>'
     if message['cc'] is not None:
-        headers = headers + '<b>Cc</b>: ' + html.escape(message['cc']) + '<br></br>'
+        headers = headers + '<b>Cc:</b> ' + html.escape(message['cc'].replace('"','')) + '<br></br>'
     if message['subject'] is not None:
-        headers = headers + '<b>Subject</b>: ' + html.escape(message['subject']) + '<br></br>'
-    return headers
+        headers = headers + '<b>Subject:</b> ' + html.escape(message['subject'].replace('"','')) + '<br></br>'
+
+    headers = headers + '''\
+        </span>
+        </div>
+        </div>
+        '''
 
 
+    return headers
+
 def _get_message_html(message):
     body = ''
     first_part = True
     if message.is_multipart():
         for part in message.walk():
             ctype = part.get_content_type()
             cdispo = str(part.get('Content-Disposition'))
```

### Comparing `mutt_html_reply-0.4.0/src/mutt_html_reply.egg-info/PKG-INFO` & `mutt_html_reply-0.4.1/src/mutt_html_reply.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutt-html-reply
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create an Outlook-style HTML reply
 Author-email: Erik Rogers <erik@rogers-family.net>
 Maintainer-email: Erik Rogers <erik@rogers-family.net>
 License: Copyright © 2024 Erik Rogers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```


# Comparing `tmp/finitelycomputable_helloworld_flask_cherrypy-24.4.tar.gz` & `tmp/finitelycomputable_helloworld_flask_cherrypy-24.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable_helloworld_flask_cherrypy-24.4.tar", last modified: Tue Apr 30 04:46:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


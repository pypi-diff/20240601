# Comparing `tmp/diaspora-event-sdk-0.2.9.tar.gz` & `tmp/diaspora_event_sdk-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diaspora-event-sdk-0.2.9.tar", last modified: Mon May  6 18:03:09 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


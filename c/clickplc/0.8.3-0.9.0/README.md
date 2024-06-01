# Comparing `tmp/clickplc-0.8.3.tar.gz` & `tmp/clickplc-0.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickplc-0.8.3.tar", last modified: Sun May  5 17:02:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


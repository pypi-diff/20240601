# Comparing `tmp/log_writer-1.0.0.tar.gz` & `tmp/log_writer-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log_writer-1.0.0.tar", last modified: Sat Jun  1 18:42:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


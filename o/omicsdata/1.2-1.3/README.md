# Comparing `tmp/omicsdata-1.2.tar.gz` & `tmp/omicsdata-1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omicsdata-1.2.tar", last modified: Sat Jun  1 15:18:17 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


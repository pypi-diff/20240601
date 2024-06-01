# Comparing `tmp/SeqLbToolkit-0.4.6.tar.gz` & `tmp/SeqLbToolkit-0.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeqLbToolkit-0.4.6.tar", last modified: Sat Jan 13 23:55:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


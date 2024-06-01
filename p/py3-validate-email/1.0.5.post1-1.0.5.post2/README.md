# Comparing `tmp/py3-validate-email-1.0.5.post1.tar.gz` & `tmp/py3_validate_email-1.0.5.post2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3-validate-email-1.0.5.post1.tar", last modified: Mon Nov 21 16:10:19 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


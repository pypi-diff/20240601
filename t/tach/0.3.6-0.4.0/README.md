# Comparing `tmp/tach-0.3.6.tar.gz` & `tmp/tach-0.4.0-pp39-pypy39_pp73-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/cpi-1.0.9.dev1660391811.tar.gz` & `tmp/cpi-1.0.9.dev1660391812-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpi-1.0.9.dev1660391811.tar", last modified: Sat Aug 13 11:56:51 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


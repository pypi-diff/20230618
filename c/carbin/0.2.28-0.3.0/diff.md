# Comparing `tmp/carbin-0.2.28.tar.gz` & `tmp/carbin-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/carbin-0.2.28.tar", last modified: Mon Apr 20 11:13:47 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


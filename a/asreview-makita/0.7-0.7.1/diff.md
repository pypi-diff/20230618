# Comparing `tmp/asreview-makita-0.7.tar.gz` & `tmp/asreview_makita-0.7.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asreview-makita-0.7.tar", last modified: Tue Jun 13 07:15:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


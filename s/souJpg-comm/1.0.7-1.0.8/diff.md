# Comparing `tmp/souJpg-comm-1.0.7.tar.gz` & `tmp/souJpg_comm-1.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "souJpg-comm-1.0.7.tar", last modified: Sun Jun 11 07:37:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


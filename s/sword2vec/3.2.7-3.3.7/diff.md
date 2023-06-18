# Comparing `tmp/sword2vec-3.2.7.tar.gz` & `tmp/sword2vec-3.3.7-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sword2vec-3.2.7.tar", last modified: Sun May 28 13:30:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


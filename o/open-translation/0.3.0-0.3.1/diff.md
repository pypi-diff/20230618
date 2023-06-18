# Comparing `tmp/open_translation-0.3.0.tar.gz` & `tmp/open_translation-0.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_translation-0.3.0.tar", last modified: Sun Jun 18 15:18:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/pandoc-beamer-arrow-0.1.2.tar.gz` & `tmp/pandoc_beamer_arrow-1.0.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pandoc-beamer-arrow-0.1.2.tar", last modified: Thu Dec 12 19:55:04 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/pretext-1.6.1.dev20230617.tar.gz` & `tmp/pretext-1.6.1.dev20230618-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230617.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/experiment-scheduler-1.0.tar.gz` & `tmp/experiment_scheduler-1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-scheduler-1.0.tar", last modified: Thu May 11 11:36:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


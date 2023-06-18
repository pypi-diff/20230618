# Comparing `tmp/markmodule-0.1.0.tar.gz` & `tmp/markmodule-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markmodule-0.1.0.tar", max compression
+gzip compressed data, was "markmodule-0.2.0.tar", max compression
```

## Comparing `markmodule-0.1.0.tar` & `markmodule-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-18 16:55:12.319246 markmodule-0.1.0/LICENSE
--rw-r--r--   0        0        0      476 2023-06-18 16:55:12.327246 markmodule-0.1.0/README.md
--rw-r--r--   0        0        0      172 2023-06-18 16:55:12.327246 markmodule-0.1.0/markmodule/__init__.py
--rw-r--r--   0        0        0      200 2023-06-18 16:55:12.327246 markmodule-0.1.0/markmodule/class_source.py
--rw-r--r--   0        0        0     2062 2023-06-18 16:55:12.327246 markmodule-0.1.0/markmodule/import_string.py
--rw-r--r--   0        0        0     3822 2023-06-18 16:55:12.327246 markmodule-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2089 1970-01-01 00:00:00.000000 markmodule-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-18 17:44:37.980431 markmodule-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1795 2023-06-18 17:44:37.980431 markmodule-0.2.0/README.md
+-rw-r--r--   0        0        0      172 2023-06-18 17:44:37.980431 markmodule-0.2.0/markmodule/__init__.py
+-rw-r--r--   0        0        0      200 2023-06-18 17:44:37.980431 markmodule-0.2.0/markmodule/class_source.py
+-rw-r--r--   0        0        0     2062 2023-06-18 17:44:37.980431 markmodule-0.2.0/markmodule/import_string.py
+-rw-r--r--   0        0        0     3822 2023-06-18 17:44:37.980431 markmodule-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3408 1970-01-01 00:00:00.000000 markmodule-0.2.0/PKG-INFO
```

### Comparing `markmodule-0.1.0/LICENSE` & `markmodule-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markmodule-0.1.0/markmodule/import_string.py` & `markmodule-0.2.0/markmodule/import_string.py`

 * *Files identical despite different names*

### Comparing `markmodule-0.1.0/pyproject.toml` & `markmodule-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markmodule"
-version = "0.1.0"
+version = "0.2.0"
 description = "Import python code in markdown as module"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```


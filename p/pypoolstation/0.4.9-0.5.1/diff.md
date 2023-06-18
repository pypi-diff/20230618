# Comparing `tmp/PyPoolstation-0.4.9.tar.gz` & `tmp/pypoolstation-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPoolstation-0.4.9.tar", max compression
+gzip compressed data, was "pypoolstation-0.5.1.tar", max compression
```

## Comparing `PyPoolstation-0.4.9.tar` & `pypoolstation-0.5.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1055 2022-05-27 14:55:13.547093 PyPoolstation-0.4.9/LICENSE
--rw-r--r--   0        0        0     7382 2022-08-17 20:57:59.341277 PyPoolstation-0.4.9/pypoolstation/__init__.py
--rw-r--r--   0        0        0      443 2022-08-17 20:58:56.229047 PyPoolstation-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      715 2022-08-17 20:59:05.702071 PyPoolstation-0.4.9/setup.py
--rw-r--r--   0        0        0      572 2022-08-17 20:59:05.702197 PyPoolstation-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-05-27 14:55:13.547093 pypoolstation-0.5.1/LICENSE
+-rw-r--r--   0        0        0     8767 2023-06-18 09:10:00.063730 pypoolstation-0.5.1/pypoolstation/__init__.py
+-rw-r--r--   0        0        0      444 2023-06-18 09:10:45.855157 pypoolstation-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 pypoolstation-0.5.1/PKG-INFO
```

### Comparing `PyPoolstation-0.4.9/LICENSE` & `pypoolstation-0.5.1/LICENSE`

 * *Files identical despite different names*


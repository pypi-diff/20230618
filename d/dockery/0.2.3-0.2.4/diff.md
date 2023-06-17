# Comparing `tmp/dockery-0.2.3.tar.gz` & `tmp/dockery-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.2.3.tar", last modified: Mon Jun 12 18:15:28 2023, max compression
+gzip compressed data, was "dockery-0.2.4.tar", last modified: Sat Jun 17 22:26:01 2023, max compression
```

## Comparing `dockery-0.2.3.tar` & `dockery-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-06-12 18:15:11.476290 dockery-0.2.3/LICENSE
--rw-r--r--   0        0        0      665 2023-06-12 18:15:11.476290 dockery-0.2.3/README.md
--rw-r--r--   0        0        0      614 2023-06-12 18:15:28.744381 dockery-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-12 18:15:11.476290 dockery-0.2.3/src/dockery/__init__.py
--rw-r--r--   0        0        0     2489 2023-06-12 18:15:11.476290 dockery-0.2.3/src/dockery/dockery.py
--rw-r--r--   0        0        0     5022 2023-06-12 18:15:11.476290 dockery-0.2.3/src/dockery/gui.py
--rw-r--r--   0        0        0      322 2023-06-12 18:15:11.476290 dockery-0.2.3/src/dockery/style.css
--rw-r--r--   0        0        0      881 2023-06-12 18:15:11.476290 dockery-0.2.3/src/dockery/utils.py
--rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 dockery-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-17 22:25:53.894298 dockery-0.2.4/LICENSE
+-rw-r--r--   0        0        0      665 2023-06-17 22:25:53.894298 dockery-0.2.4/README.md
+-rw-r--r--   0        0        0      761 2023-06-17 22:26:01.970420 dockery-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/__init__.py
+-rw-r--r--   0        0        0     2489 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/dockery.py
+-rw-r--r--   0        0        0     5022 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/gui.py
+-rw-r--r--   0        0        0      322 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/style.css
+-rw-r--r--   0        0        0      881 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/utils.py
+-rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 dockery-0.2.4/PKG-INFO
```

### Comparing `dockery-0.2.3/LICENSE` & `dockery-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.2.3/README.md` & `dockery-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dockery-0.2.3/pyproject.toml` & `dockery-0.2.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.2.3"
+version = "0.2.4"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.27.0",
@@ -15,14 +15,18 @@
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 dockery = "dockery.dockery:main"
 
+[project.urls]
+"Bug Tracker" = "https://github.com/marianocarrazana/dockery/issues"
+"Source Code" = "https://github.com/marianocarrazana/dockery"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
```

### Comparing `dockery-0.2.3/src/dockery/dockery.py` & `dockery-0.2.4/src/dockery/dockery.py`

 * *Files identical despite different names*

### Comparing `dockery-0.2.3/src/dockery/gui.py` & `dockery-0.2.4/src/dockery/gui.py`

 * *Files identical despite different names*

### Comparing `dockery-0.2.3/src/dockery/utils.py` & `dockery-0.2.4/src/dockery/utils.py`

 * *Files identical despite different names*

### Comparing `dockery-0.2.3/PKG-INFO` & `dockery-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: dockery
-Version: 0.2.3
+Version: 0.2.4
 Summary: Graphical interface for Docker in your console
 Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
 License: MIT
+Project-URL: Bug tracker, https://github.com/marianocarrazana/dockery/issues
+Project-URL: Source code, https://github.com/marianocarrazana/dockery
 Requires-Python: >=3.9
 Requires-Dist: docker>=6.1.3
 Requires-Dist: textual>=0.27.0
 Requires-Dist: click>=8.1.3
 Description-Content-Type: text/markdown
 
 # dockery
```


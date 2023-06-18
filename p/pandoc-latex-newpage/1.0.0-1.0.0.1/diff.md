# Comparing `tmp/pandoc_latex_newpage-1.0.0.tar.gz` & `tmp/pandoc_latex_newpage-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_latex_newpage-1.0.0.tar", max compression
+gzip compressed data, was "pandoc_latex_newpage-1.0.0.1.tar", max compression
```

## Comparing `pandoc_latex_newpage-1.0.0.tar` & `pandoc_latex_newpage-1.0.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1521 2023-06-18 11:57:30.593497 pandoc_latex_newpage-1.0.0/LICENSE
--rw-r--r--   0        0        0     8462 2023-06-18 11:57:30.593497 pandoc_latex_newpage-1.0.0/README.md
--rw-r--r--   0        0        0     1561 2023-06-18 11:57:30.597497 pandoc_latex_newpage-1.0.0/pandoc_latex_newpage.py
--rw-r--r--   0        0        0     2929 2023-06-18 11:57:30.597497 pandoc_latex_newpage-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9579 1970-01-01 00:00:00.000000 pandoc_latex_newpage-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-06-18 12:29:51.023649 pandoc_latex_newpage-1.0.0.1/LICENSE
+-rw-r--r--   0        0        0     8462 2023-06-18 12:29:51.027649 pandoc_latex_newpage-1.0.0.1/README.md
+-rw-r--r--   0        0        0     1561 2023-06-18 12:29:51.027649 pandoc_latex_newpage-1.0.0.1/pandoc_latex_newpage.py
+-rw-r--r--   0        0        0     2936 2023-06-18 12:29:51.027649 pandoc_latex_newpage-1.0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9581 1970-01-01 00:00:00.000000 pandoc_latex_newpage-1.0.0.1/PKG-INFO
```

### Comparing `pandoc_latex_newpage-1.0.0/LICENSE` & `pandoc_latex_newpage-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_latex_newpage-1.0.0/README.md` & `pandoc_latex_newpage-1.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pandoc_latex_newpage-1.0.0/pandoc_latex_newpage.py` & `pandoc_latex_newpage-1.0.0.1/pandoc_latex_newpage.py`

 * *Files identical despite different names*

### Comparing `pandoc_latex_newpage-1.0.0/pyproject.toml` & `pandoc_latex_newpage-1.0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-    requires = ["poetry-core"]
+    requires = ["poetry-core>=1.2"]
     build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
     name = "pandoc-latex-newpage"
-    version = "1.0.0"
+    version = "1.0.0.1"
     description="A pandoc filter for converting horizontal rule to new page in LaTeX"
     authors = ["Christophe Demko <chdemko@gmail.com>"]
     license = "BSD-3-Clause"
     readme = "README.md"
     homepage="https://github.com/chdemko/pandoc-latex-newpage"
     keywords=["pandoc", "filters", "latex", "newpage"]
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `pandoc_latex_newpage-1.0.0/PKG-INFO` & `pandoc_latex_newpage-1.0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoc-latex-newpage
-Version: 1.0.0
+Version: 1.0.0.1
 Summary: A pandoc filter for converting horizontal rule to new page in LaTeX
 Home-page: https://github.com/chdemko/pandoc-latex-newpage
 License: BSD-3-Clause
 Keywords: pandoc,filters,latex,newpage
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
 Requires-Python: >=3.9,<4.0
```


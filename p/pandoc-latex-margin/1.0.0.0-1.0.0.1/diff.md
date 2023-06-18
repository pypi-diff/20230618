# Comparing `tmp/pandoc_latex_margin-1.0.0.0.tar.gz` & `tmp/pandoc_latex_margin-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_latex_margin-1.0.0.0.tar", max compression
+gzip compressed data, was "pandoc_latex_margin-1.0.0.1.tar", max compression
```

## Comparing `pandoc_latex_margin-1.0.0.0.tar` & `pandoc_latex_margin-1.0.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1521 2023-06-18 18:40:37.128913 pandoc_latex_margin-1.0.0.0/LICENSE
--rw-r--r--   0        0        0     3087 2023-06-18 18:40:37.128913 pandoc_latex_margin-1.0.0.0/README.md
--rw-r--r--   0        0        0     4986 2023-06-18 18:40:37.128913 pandoc_latex_margin-1.0.0.0/pandoc_latex_margin.py
--rw-r--r--   0        0        0     2916 2023-06-18 18:40:37.128913 pandoc_latex_margin-1.0.0.0/pyproject.toml
--rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 pandoc_latex_margin-1.0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-06-18 18:59:13.423937 pandoc_latex_margin-1.0.0.1/LICENSE
+-rw-r--r--   0        0        0     3087 2023-06-18 18:59:13.423937 pandoc_latex_margin-1.0.0.1/README.md
+-rw-r--r--   0        0        0     4986 2023-06-18 18:59:13.423937 pandoc_latex_margin-1.0.0.1/pandoc_latex_margin.py
+-rw-r--r--   0        0        0     2909 2023-06-18 18:59:13.423937 pandoc_latex_margin-1.0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 pandoc_latex_margin-1.0.0.1/PKG-INFO
```

### Comparing `pandoc_latex_margin-1.0.0.0/LICENSE` & `pandoc_latex_margin-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_latex_margin-1.0.0.0/README.md` & `pandoc_latex_margin-1.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pandoc_latex_margin-1.0.0.0/pandoc_latex_margin.py` & `pandoc_latex_margin-1.0.0.1/pandoc_latex_margin.py`

 * *Files identical despite different names*

### Comparing `pandoc_latex_margin-1.0.0.0/pyproject.toml` & `pandoc_latex_margin-1.0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
     requires = ["poetry-core>=1.2"]
     build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
     name = "pandoc-latex-margin"
-    version = "1.0.0.0"
+    version = "1.0.0.1"
     description="A pandoc filter for changing margins in LaTeX"
     authors = ["Christophe Demko <chdemko@gmail.com>"]
     license = "BSD-3-Clause"
     readme = "README.md"
-    homepage="https://github.com/chdemko/pandoc-latex-french-spaces"
+    homepage="https://github.com/chdemko/pandoc-latex-margin"
     keywords=["pandoc", "filters", "latex", "margins"]
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
```

### Comparing `pandoc_latex_margin-1.0.0.0/PKG-INFO` & `pandoc_latex_margin-1.0.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pandoc-latex-margin
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: A pandoc filter for changing margins in LaTeX
-Home-page: https://github.com/chdemko/pandoc-latex-french-spaces
+Home-page: https://github.com/chdemko/pandoc-latex-margin
 License: BSD-3-Clause
 Keywords: pandoc,filters,latex,margins
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```


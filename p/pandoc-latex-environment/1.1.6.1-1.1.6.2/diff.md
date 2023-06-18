# Comparing `tmp/pandoc_latex_environment-1.1.6.1.tar.gz` & `tmp/pandoc_latex_environment-1.1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_latex_environment-1.1.6.1.tar", max compression
+gzip compressed data, was "pandoc_latex_environment-1.1.6.2.tar", max compression
```

## Comparing `pandoc_latex_environment-1.1.6.1.tar` & `pandoc_latex_environment-1.1.6.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1521 2023-06-18 15:13:00.019788 pandoc_latex_environment-1.1.6.1/LICENSE
--rw-r--r--   0        0        0     2888 2023-06-18 15:13:00.019788 pandoc_latex_environment-1.1.6.1/README.md
--rwxr-xr-x   0        0        0     2601 2023-06-18 15:13:00.019788 pandoc_latex_environment-1.1.6.1/pandoc_latex_environment.py
--rw-r--r--   0        0        0     2956 2023-06-18 15:13:00.019788 pandoc_latex_environment-1.1.6.1/pyproject.toml
--rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 pandoc_latex_environment-1.1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-06-18 18:51:45.442446 pandoc_latex_environment-1.1.6.2/LICENSE
+-rw-r--r--   0        0        0     3149 2023-06-18 18:51:45.442446 pandoc_latex_environment-1.1.6.2/README.md
+-rwxr-xr-x   0        0        0     2601 2023-06-18 18:51:45.442446 pandoc_latex_environment-1.1.6.2/pandoc_latex_environment.py
+-rw-r--r--   0        0        0     2954 2023-06-18 18:51:45.442446 pandoc_latex_environment-1.1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4274 1970-01-01 00:00:00.000000 pandoc_latex_environment-1.1.6.2/PKG-INFO
```

### Comparing `pandoc_latex_environment-1.1.6.1/LICENSE` & `pandoc_latex_environment-1.1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_latex_environment-1.1.6.1/README.md` & `pandoc_latex_environment-1.1.6.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Installation
 
-![Python package](https://github.com/chdemko/pandoc-latex-environment/workflows/Python%20package/badge.svg?branch=develop)
+[![Python package](https://github.com/chdemko/pandoc-latex-environment/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-environment/actions/workflows/python-package.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-environment/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-environment?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-environment.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-environment/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
 [![License](https://img.shields.io/pypi/l/pandoc-latex-environment.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-environment/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
 [![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
 [![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-latex-environment.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-environment.readthedocs.io/en/latest/)
 
 *pandoc-latex-environment* is a [pandoc] filter for adding LaTeX environement on specific HTML `div` tags.
 
 [pandoc]: http://pandoc.org/
 
 Instructions
 ------------
```

### Comparing `pandoc_latex_environment-1.1.6.1/pandoc_latex_environment.py` & `pandoc_latex_environment-1.1.6.2/pandoc_latex_environment.py`

 * *Files identical despite different names*

### Comparing `pandoc_latex_environment-1.1.6.1/pyproject.toml` & `pandoc_latex_environment-1.1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
     requires = ["poetry-core>=1.2"]
     build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
     name = "pandoc-latex-environment"
-    version = "1.1.6.1"
+    version = "1.1.6.2"
     description="A pandoc filter for adding LaTeX environement on specific div"
     authors = ["Christophe Demko <chdemko@gmail.com>"]
     license = "BSD-3-Clause"
     readme = "README.md"
-    homepage="https://github.com/chdemko/pandoc-latex-french-spaces"
+    homepage="https://github.com/chdemko/pandoc-latex-environment"
     keywords=["pandoc", "filters", "latex", "environment"]
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
```

### Comparing `pandoc_latex_environment-1.1.6.1/PKG-INFO` & `pandoc_latex_environment-1.1.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pandoc-latex-environment
-Version: 1.1.6.1
+Version: 1.1.6.2
 Summary: A pandoc filter for adding LaTeX environement on specific div
-Home-page: https://github.com/chdemko/pandoc-latex-french-spaces
+Home-page: https://github.com/chdemko/pandoc-latex-environment
 License: BSD-3-Clause
 Keywords: pandoc,filters,latex,environment
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -23,24 +23,25 @@
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Filters
 Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Installation
 
-![Python package](https://github.com/chdemko/pandoc-latex-environment/workflows/Python%20package/badge.svg?branch=develop)
+[![Python package](https://github.com/chdemko/pandoc-latex-environment/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-environment/actions/workflows/python-package.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-environment/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-environment?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-environment.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-environment/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
 [![License](https://img.shields.io/pypi/l/pandoc-latex-environment.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-environment/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
 [![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
 [![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-latex-environment.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-environment.readthedocs.io/en/latest/)
 
 *pandoc-latex-environment* is a [pandoc] filter for adding LaTeX environement on specific HTML `div` tags.
 
 [pandoc]: http://pandoc.org/
 
 Instructions
 ------------
```


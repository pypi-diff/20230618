# Comparing `tmp/pandoc_beamer_block-1.0.0.0.tar.gz` & `tmp/pandoc_beamer_block-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_beamer_block-1.0.0.0.tar", max compression
+gzip compressed data, was "pandoc_beamer_block-1.0.0.1.tar", max compression
```

## Comparing `pandoc_beamer_block-1.0.0.0.tar` & `pandoc_beamer_block-1.0.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1521 2023-06-18 13:41:49.899906 pandoc_beamer_block-1.0.0.0/LICENSE
--rw-r--r--   0        0        0     8926 2023-06-18 13:41:49.899906 pandoc_beamer_block-1.0.0.0/README.md
--rw-r--r--   0        0        0     2792 2023-06-18 13:41:49.903906 pandoc_beamer_block-1.0.0.0/pandoc_beamer_block.py
--rw-r--r--   0        0        0     2935 2023-06-18 13:41:49.903906 pandoc_beamer_block-1.0.0.0/pyproject.toml
--rw-r--r--   0        0        0    10044 1970-01-01 00:00:00.000000 pandoc_beamer_block-1.0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-06-18 19:00:14.295724 pandoc_beamer_block-1.0.0.1/LICENSE
+-rw-r--r--   0        0        0     8992 2023-06-18 19:00:14.295724 pandoc_beamer_block-1.0.0.1/README.md
+-rw-r--r--   0        0        0     2792 2023-06-18 19:00:14.295724 pandoc_beamer_block-1.0.0.1/pandoc_beamer_block.py
+-rw-r--r--   0        0        0     2928 2023-06-18 19:00:14.295724 pandoc_beamer_block-1.0.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10103 1970-01-01 00:00:00.000000 pandoc_beamer_block-1.0.0.1/PKG-INFO
```

### Comparing `pandoc_beamer_block-1.0.0.0/LICENSE` & `pandoc_beamer_block-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_beamer_block-1.0.0.0/README.md` & `pandoc_beamer_block-1.0.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Installation
-![Python package](https://github.com/chdemko/pandoc-beamer-block/workflows/Python%20package/badge.svg?branch=develop)
+
+[![Python package](https://github.com/chdemko/pandoc-beamer-block/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-beamer-block/actions/workflows/python-package.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-block/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-block?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-beamer-block/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-beamer-block/)
 [![Code Beat](https://codebeat.co/badges/cb5538dc-f30b-4ac4-abf6-3c213682c54d)](https://codebeat.co/projects/github-com-chdemko-pandoc-beamer-block-develop/)
 [![Codacy](https://img.shields.io/codacy/grade/af5a670790264990811713280a8f8dcf.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-beamer-block)
 [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-block/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-block)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-beamer-block.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-block/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-block/)
@@ -42,15 +43,14 @@
 ~~~shell
 $ pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-block
 ~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
 ~~~shell
-$ sudo apt-get update
 $ sudo apt-get install python3-pip
 ~~~
 
 [python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
```

### Comparing `pandoc_beamer_block-1.0.0.0/pandoc_beamer_block.py` & `pandoc_beamer_block-1.0.0.1/pandoc_beamer_block.py`

 * *Files identical despite different names*

### Comparing `pandoc_beamer_block-1.0.0.0/pyproject.toml` & `pandoc_beamer_block-1.0.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
     requires = ["poetry-core>=1.2"]
     build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
     name = "pandoc-beamer-block"
-    version = "1.0.0.0"
+    version = "1.0.0.1"
     description="A pandoc filter for adding beamer block on specific div"
     authors = ["Christophe Demko <chdemko@gmail.com>"]
     license = "BSD-3-Clause"
     readme = "README.md"
-    homepage="https://github.com/chdemko/pandoc-latex-french-spaces"
+    homepage="https://github.com/chdemko/pandoc-beamer-block"
     keywords=["pandoc", "filters", "latex", "french", "spaces"]
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
```

### Comparing `pandoc_beamer_block-1.0.0.0/PKG-INFO` & `pandoc_beamer_block-1.0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pandoc-beamer-block
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: A pandoc filter for adding beamer block on specific div
-Home-page: https://github.com/chdemko/pandoc-latex-french-spaces
+Home-page: https://github.com/chdemko/pandoc-beamer-block
 License: BSD-3-Clause
 Keywords: pandoc,filters,latex,french,spaces
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -22,15 +22,16 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Filters
 Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Installation
-![Python package](https://github.com/chdemko/pandoc-beamer-block/workflows/Python%20package/badge.svg?branch=develop)
+
+[![Python package](https://github.com/chdemko/pandoc-beamer-block/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-beamer-block/actions/workflows/python-package.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-block/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-block?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-beamer-block/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-beamer-block/)
 [![Code Beat](https://codebeat.co/badges/cb5538dc-f30b-4ac4-abf6-3c213682c54d)](https://codebeat.co/projects/github-com-chdemko-pandoc-beamer-block-develop/)
 [![Codacy](https://img.shields.io/codacy/grade/af5a670790264990811713280a8f8dcf.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-beamer-block)
 [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-block/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-block)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-beamer-block.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-block/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-block/)
@@ -69,15 +70,14 @@
 ~~~shell
 $ pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-block
 ~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
 ~~~shell
-$ sudo apt-get update
 $ sudo apt-get install python3-pip
 ~~~
 
 [python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
```


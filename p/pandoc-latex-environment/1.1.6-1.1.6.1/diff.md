# Comparing `tmp/pandoc-latex-environment-1.1.6.tar.gz` & `tmp/pandoc_latex_environment-1.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-latex-environment-1.1.6.tar", last modified: Wed Feb 24 15:12:27 2021, max compression
+gzip compressed data, was "pandoc_latex_environment-1.1.6.1.tar", max compression
```

## Comparing `pandoc-latex-environment-1.1.6.tar` & `pandoc_latex_environment-1.1.6.1.tar`

### file list

```diff
@@ -1,14 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-24 15:12:27.462849 pandoc-latex-environment-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-02-24 15:12:15.000000 pandoc-latex-environment-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2021-02-24 15:12:27.462849 pandoc-latex-environment-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2021-02-24 15:12:15.000000 pandoc-latex-environment-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-24 15:12:27.462849 pandoc-latex-environment-1.1.6/pandoc_latex_environment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2021-02-24 15:12:27.000000 pandoc-latex-environment-1.1.6/pandoc_latex_environment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-02-24 15:12:27.000000 pandoc-latex-environment-1.1.6/pandoc_latex_environment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-24 15:12:27.000000 pandoc-latex-environment-1.1.6/pandoc_latex_environment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-02-24 15:12:27.000000 pandoc-latex-environment-1.1.6/pandoc_latex_environment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-02-24 15:12:27.000000 pandoc-latex-environment-1.1.6/pandoc_latex_environment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-02-24 15:12:27.000000 pandoc-latex-environment-1.1.6/pandoc_latex_environment.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     2077 2021-02-24 15:12:15.000000 pandoc-latex-environment-1.1.6/pandoc_latex_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-02-24 15:12:27.462849 pandoc-latex-environment-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4133 2021-02-24 15:12:15.000000 pandoc-latex-environment-1.1.6/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-18 15:13:00.019788 pandoc_latex_environment-1.1.6.1/LICENSE
+-rw-r--r--   0        0        0     2888 2023-06-18 15:13:00.019788 pandoc_latex_environment-1.1.6.1/README.md
+-rwxr-xr-x   0        0        0     2601 2023-06-18 15:13:00.019788 pandoc_latex_environment-1.1.6.1/pandoc_latex_environment.py
+-rw-r--r--   0        0        0     2956 2023-06-18 15:13:00.019788 pandoc_latex_environment-1.1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 pandoc_latex_environment-1.1.6.1/PKG-INFO
```

### Comparing `pandoc-latex-environment-1.1.6/PKG-INFO` & `pandoc_latex_environment-1.1.6.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,93 +1,85 @@
 Metadata-Version: 2.1
 Name: pandoc-latex-environment
-Version: 1.1.6
+Version: 1.1.6.1
 Summary: A pandoc filter for adding LaTeX environement on specific div
-Home-page: https://github.com/chdemko/pandoc-latex-environment
+Home-page: https://github.com/chdemko/pandoc-latex-french-spaces
+License: BSD-3-Clause
+Keywords: pandoc,filters,latex,environment
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
-Maintainer: Christophe Demko
-Maintainer-email: chdemko@gmail.com
-License: BSD-3-Clause
-Download-URL: https://github.com/chdemko/pandoc-latex-environment/archive/master.zip
-Description: # pandoc-latex-environment
-        ![Python package](https://github.com/chdemko/pandoc-latex-environment/workflows/Python%20package/badge.svg?branch=develop)
-        [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-environment/1.1.6.svg)](https://coveralls.io/github/chdemko/pandoc-latex-environment?branch=1.1.6)
-        [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-environment.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-environment/)
-        [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
-        [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
-        [![License](https://img.shields.io/pypi/l/pandoc-latex-environment.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-environment/1.1.6/LICENSE)
-        [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
-        [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
-        
-        *pandoc-latex-environment* is a [pandoc] filter for adding LaTeX environement on specific HTML `div` tags.
-        
-        [pandoc]: http://pandoc.org/
-        
-        Documentation
-        -------------
-        
-        See the [wiki pages](https://github.com/chdemko/pandoc-latex-environment/wiki).
-        
-        Usage
-        -----
-        
-        To apply the filter, use the following option with pandoc:
-        
-            --filter pandoc-latex-environment
-        
-        Installation
-        ------------
-        
-        *pandoc-latex-environment* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
-        
-        Install *pandoc-latex-environment* as root using the bash command
-        
-            pip install pandoc-latex-environment 
-        
-        To upgrade to the most recent release, use
-        
-            pip install --upgrade pandoc-latex-environment 
-        
-        To upgrade to the current code, use
-        
-            pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-environment
-        
-        `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
-        
-            apt-get update
-            apt-get install python-pip
-        
-        [python]: https://www.python.org/
-        [on Windows]: https://www.python.org/downloads/windows/
-        [PyPI]: https://pypi.python.org/pypi
-        
-        
-        Getting Help
-        ------------
-        
-        If you have any difficulties with *pandoc-latex-environment*, please feel welcome to [file an issue] on github so that we can help.
-        
-        [file an issue]: https://github.com/chdemko/pandoc-latex-environment/issues
-        
-Keywords: pandoc,filters,environment,latex
-Platform: UNKNOWN
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Filters
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Natural Language :: English
+Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
+
+# Installation
+
+![Python package](https://github.com/chdemko/pandoc-latex-environment/workflows/Python%20package/badge.svg?branch=develop)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-environment/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-environment?branch=develop)
+[![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-environment.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-environment/)
+[![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
+[![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
+[![License](https://img.shields.io/pypi/l/pandoc-latex-environment.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-environment/develop/LICENSE)
+[![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
+[![Development Status](https://img.shields.io/pypi/status/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
+
+*pandoc-latex-environment* is a [pandoc] filter for adding LaTeX environement on specific HTML `div` tags.
+
+[pandoc]: http://pandoc.org/
+
+Instructions
+------------
+
+*pandoc-latex-environment* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+
+Install *pandoc-latex-environment* using the bash command
+
+~~~shell
+$ pip install pandoc-latex-environment
+~~~
+
+To upgrade to the most recent release, use
+
+~~~shell
+$ pip install --upgrade pandoc-latex-environment 
+~~~
+
+To upgrade to the current code, use
+
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-environment
+~~~
+
+`pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
+
+~~~shell
+$ apt-get install python3-pip
+~~~
+
+[python]: https://www.python.org/
+[on Windows]: https://www.python.org/downloads/windows/
+[PyPI]: https://pypi.python.org/pypi
+
+
+Getting Help
+------------
+
+If you have any difficulties with *pandoc-latex-environment*, please feel welcome to [file an issue] on github so that we can help.
+
+[file an issue]: https://github.com/chdemko/pandoc-latex-environment/issues
+
```

### Comparing `pandoc-latex-environment-1.1.6/README.md` & `pandoc_latex_environment-1.1.6.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,52 @@
-# pandoc-latex-environment
+# Installation
+
 ![Python package](https://github.com/chdemko/pandoc-latex-environment/workflows/Python%20package/badge.svg?branch=develop)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-environment/1.1.6.svg)](https://coveralls.io/github/chdemko/pandoc-latex-environment?branch=1.1.6)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-environment/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-environment?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-environment.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-environment/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
-[![License](https://img.shields.io/pypi/l/pandoc-latex-environment.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-environment/1.1.6/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-latex-environment.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-environment/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-environment.svg)](https://pypi.org/project/pandoc-latex-environment/)
 
 *pandoc-latex-environment* is a [pandoc] filter for adding LaTeX environement on specific HTML `div` tags.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [wiki pages](https://github.com/chdemko/pandoc-latex-environment/wiki).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-latex-environment
-
-Installation
+Instructions
 ------------
 
-*pandoc-latex-environment* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
+*pandoc-latex-environment* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-latex-environment* as root using the bash command
+Install *pandoc-latex-environment* using the bash command
 
-    pip install pandoc-latex-environment 
+~~~shell
+$ pip install pandoc-latex-environment
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-latex-environment 
+~~~shell
+$ pip install --upgrade pandoc-latex-environment 
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-environment
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-environment
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ apt-get install python3-pip
+~~~
 
 [python]: https://www.python.org/
 [on Windows]: https://www.python.org/downloads/windows/
 [PyPI]: https://pypi.python.org/pypi
 
 
 Getting Help
```


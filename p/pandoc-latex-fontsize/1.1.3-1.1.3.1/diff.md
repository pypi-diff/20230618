# Comparing `tmp/pandoc-latex-fontsize-1.1.3.tar.gz` & `tmp/pandoc_latex_fontsize-1.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-latex-fontsize-1.1.3.tar", last modified: Tue Feb 23 15:59:33 2021, max compression
+gzip compressed data, was "pandoc_latex_fontsize-1.1.3.1.tar", max compression
```

## Comparing `pandoc-latex-fontsize-1.1.3.tar` & `pandoc_latex_fontsize-1.1.3.1.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 15:59:33.739855 pandoc-latex-fontsize-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2021-02-23 15:59:25.000000 pandoc-latex-fontsize-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-02-23 15:59:25.000000 pandoc-latex-fontsize-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2021-02-23 15:59:33.739855 pandoc-latex-fontsize-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2021-02-23 15:59:25.000000 pandoc-latex-fontsize-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 15:59:33.739855 pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2021-02-23 15:59:33.000000 pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      345 2021-02-23 15:59:33.000000 pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-23 15:59:33.000000 pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-02-23 15:59:33.000000 pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-02-23 15:59:33.000000 pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-02-23 15:59:33.000000 pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2021-02-23 15:59:25.000000 pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-02-23 15:59:33.739855 pandoc-latex-fontsize-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-02-23 15:59:25.000000 pandoc-latex-fontsize-1.1.3/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-18 20:03:52.518079 pandoc_latex_fontsize-1.1.3.1/LICENSE
+-rw-r--r--   0        0        0     3149 2023-06-18 20:03:52.518079 pandoc_latex_fontsize-1.1.3.1/README.md
+-rw-r--r--   0        0        0     4278 2023-06-18 20:03:52.522079 pandoc_latex_fontsize-1.1.3.1/pandoc_latex_fontsize.py
+-rw-r--r--   0        0        0     2920 2023-06-18 20:03:52.522079 pandoc_latex_fontsize-1.1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4249 1970-01-01 00:00:00.000000 pandoc_latex_fontsize-1.1.3.1/PKG-INFO
```

### Comparing `pandoc-latex-fontsize-1.1.3/LICENSE` & `pandoc_latex_fontsize-1.1.3.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2017-2018, Christophe Demko
+Copyright (c) 2017-2021, Christophe Demko
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pandoc-latex-fontsize-1.1.3/README.md` & `pandoc_latex_fontsize-1.1.3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-# pandoc-latex-fontsize
-![Python package](https://github.com/chdemko/pandoc-latex-fontsize/workflows/Python%20package/badge.svg?branch=develop)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-fontsize/1.1.3.svg)](https://coveralls.io/github/chdemko/pandoc-latex-fontsize?branch=1.1.3)
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-latex-fontsize/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-fontsize/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-fontsize/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-fontsize?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-fontsize.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-fontsize/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-fontsize.svg)](https://pypi.org/project/pandoc-latex-fontsize/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-fontsize.svg)](https://pypi.org/project/pandoc-latex-fontsize/)
-[![License](https://img.shields.io/pypi/l/pandoc-latex-fontsize.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-fontsize/1.1.3/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-latex-fontsize.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-fontsize/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-fontsize.svg)](https://pypi.org/project/pandoc-latex-fontsize/)
-[![Development Status](https://img.shields.io/pypi/status/pandoc-latex-fontsize.svg)](https://pypi.org/project/pandoc-latex-fontsize/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)[![Development Status](https://img.shields.io/pypi/status/pandoc-latex-fontsize.svg)](https://pypi.org/project/pandoc-latex-fontsize/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-latex-fontsize.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-fontsize.readthedocs.io/en/latest/)
 
 *pandoc-latex-fontsize* is a [pandoc] filter for modifying font size to `Code`, `CodeBlock`, `Span`, and `Div` that have speficied classes or `latex-fontsize` attribute.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [wiki pages](https://github.com/chdemko/pandoc-latex-fontsize/wiki).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-latex-fontsize
-
-Installation
+Instructions
 ------------
 
-*pandoc-latex-fontsize* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
+*pandoc-latex-fontsize* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-latex-fontsize* as root using the bash command
+Install *pandoc-latex-fontsize* using the bash command
 
-    pip install pandoc-latex-fontsize
+~~~shell
+$ pip install pandoc-latex-fontsize
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-latex-fontsize
+~~~shell
+$ pip install --upgrade pandoc-latex-fontsize
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-fontsize
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-fontsize
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get update
+$ sudo apt-get install python3-pip
+~~~
 
 [python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
 
 
 Getting Help
```

### Comparing `pandoc-latex-fontsize-1.1.3/pandoc_latex_fontsize.py` & `pandoc_latex_fontsize-1.1.3.1/pandoc_latex_fontsize.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,186 @@
 #!/usr/bin/env python
 
 """
-Pandoc filter for changing font size in LaTeX
+Pandoc filter for changing font size in LaTeX.
 """
 
 from panflute import (  # type: ignore
-    debug,
-    run_filter,
-    Span,
-    Div,
-    RawInline,
-    RawBlock,
     Code,
     CodeBlock,
+    Div,
+    RawBlock,
+    RawInline,
+    Span,
+    debug,
+    run_filter,
 )
 
 
 def latex_code(size):
     """
-    Get LaTeX code for size
+    Get LaTeX code for size.
+
+    Arguments
+    ---------
+    size
+        The size name.
+
+    Returns
+    -------
+        LaTeX code for size.
     """
     return "\\" + size + " "
 
 
 def get_correct_size(size):
     """
     Get correct size.
+
+    Arguments
+    ---------
+    size
+        The size name.
+
+    Returns
+    -------
+        The correct size.
     """
-    if size in [
+    if size in (
         "Huge",
         "huge",
         "LARGE",
         "Large",
         "large",
         "normalsize",
         "small",
         "footnotesize",
         "scriptsize",
         "tiny",
-    ]:
+    ):
         return size
     debug(
         "[WARNING] pandoc-latex-fontsize: "
         + size
         + " is not a correct LaTeX size; using normalsize"
     )
     return "normalsize"
 
 
 def add_latex(elem, latex):
     """
     Add LaTeX code to elem.
+
+    Arguments
+    ---------
+    elem
+        A pandoc element
+    latex
+        A LaTeX code
+
+    Returns
+    -------
+        A list of pandoc elements or None
     """
     # Is it a Span?
     if isinstance(elem, Span):
         elem.content.insert(0, RawInline(latex, "tex"))
 
     # Is it a Div?
     elif isinstance(elem, Div):
         elem.content.insert(0, RawBlock("{" + latex, "tex"))
         elem.content.append(RawBlock("}", "tex"))
 
     # Is it a Code?
-    elif isinstance(elem, Code):
+    elif isinstance(elem, Code):  # noqa: R505
         return [RawInline("{" + latex, "tex"), elem, RawInline("}", "tex")]
 
     # Is it a CodeBlock?
     elif isinstance(elem, CodeBlock):
         return [RawBlock("{" + latex, "tex"), elem, RawBlock("}", "tex")]
 
     return None
 
 
 def fontsize(elem, doc):
     """
     Generate fontsize for elem.
+
+    Arguments
+    ---------
+    elem
+        A pandoc element
+    doc
+        The pandoc document
+
+    Returns
+    -------
+        A list of pandoc elements or None
     """
     # Is it in the right format and is it a Span, Div, Code or CodeBlock?
-    if doc.format in ["latex", "beamer"] and elem.tag in [
+    if doc.format in ("latex", "beamer") and elem.tag in (
         "Span",
         "Div",
         "Code",
         "CodeBlock",
-    ]:
-
+    ):
         # Is there a latex-fontsize attribute?
         if "latex-fontsize" in elem.attributes:
             return add_latex(
                 elem, latex_code(get_correct_size(elem.attributes["latex-fontsize"]))
             )
         # Get the classes
         classes = set(elem.classes)
 
         # Loop on all fontsize definition
         for definition in doc.defined:
-
             # Are the classes correct?
             if classes >= definition["classes"]:
                 return add_latex(elem, definition["latex"])
 
     return None
 
 
 def prepare(doc):
     """
-    Prepare doc.
+    Prepare the doc.
+
+    Arguments
+    ---------
+    doc
+        The pandoc document
     """
     # Prepare the definitions
     doc.defined = []
 
     # Get the meta data
     meta = doc.get_metadata("pandoc-latex-fontsize")
 
     if isinstance(meta, list):
-
         # Loop on all definitions
         for definition in meta:
-
             # Verify the definition
             if (
                 isinstance(definition, dict)
                 and "classes" in definition
                 and isinstance(definition["classes"], list)
             ):
                 add_definition(doc.defined, definition)
 
 
 def add_definition(defined, definition):
     """
     Add definition to doc.
+
+    Arguments
+    ---------
+    defined
+        A list of definition
+    definition
+        A new definition
     """
     # Get the classes
     classes = definition["classes"]
 
     # Get the size
     if "size" in definition:
         size = get_correct_size(definition["size"])
@@ -142,14 +190,23 @@
 
     # Add a definition
     defined.append({"classes": set(classes), "latex": latex_code(size)})
 
 
 def main(doc=None):
     """
-    main function.
+    Convert the pandoc document.
+
+    Arguments
+    ---------
+    doc
+        The pandoc document.
+
+    Returns
+    -------
+        The modified document.
     """
     return run_filter(fontsize, prepare=prepare, doc=doc)
 
 
 if __name__ == "__main__":
     main()
```


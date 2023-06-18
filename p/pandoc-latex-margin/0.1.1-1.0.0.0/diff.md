# Comparing `tmp/pandoc-latex-margin-0.1.1.tar.gz` & `tmp/pandoc_latex_margin-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-latex-margin-0.1.1.tar", last modified: Tue Feb 23 16:56:00 2021, max compression
+gzip compressed data, was "pandoc_latex_margin-1.0.0.0.tar", max compression
```

## Comparing `pandoc-latex-margin-0.1.1.tar` & `pandoc_latex_margin-1.0.0.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 16:56:00.144042 pandoc-latex-margin-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2021-02-23 16:55:50.000000 pandoc-latex-margin-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-02-23 16:55:50.000000 pandoc-latex-margin-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4354 2021-02-23 16:56:00.144042 pandoc-latex-margin-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2021-02-23 16:55:50.000000 pandoc-latex-margin-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 16:56:00.140042 pandoc-latex-margin-0.1.1/pandoc_latex_margin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4354 2021-02-23 16:55:59.000000 pandoc-latex-margin-0.1.1/pandoc_latex_margin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-02-23 16:56:00.000000 pandoc-latex-margin-0.1.1/pandoc_latex_margin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-23 16:55:59.000000 pandoc-latex-margin-0.1.1/pandoc_latex_margin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-02-23 16:55:59.000000 pandoc-latex-margin-0.1.1/pandoc_latex_margin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-02-23 16:55:59.000000 pandoc-latex-margin-0.1.1/pandoc_latex_margin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-02-23 16:55:59.000000 pandoc-latex-margin-0.1.1/pandoc_latex_margin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4058 2021-02-23 16:55:50.000000 pandoc-latex-margin-0.1.1/pandoc_latex_margin.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-02-23 16:56:00.144042 pandoc-latex-margin-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3757 2021-02-23 16:55:50.000000 pandoc-latex-margin-0.1.1/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-18 18:40:37.128913 pandoc_latex_margin-1.0.0.0/LICENSE
+-rw-r--r--   0        0        0     3087 2023-06-18 18:40:37.128913 pandoc_latex_margin-1.0.0.0/README.md
+-rw-r--r--   0        0        0     4986 2023-06-18 18:40:37.128913 pandoc_latex_margin-1.0.0.0/pandoc_latex_margin.py
+-rw-r--r--   0        0        0     2916 2023-06-18 18:40:37.128913 pandoc_latex_margin-1.0.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 pandoc_latex_margin-1.0.0.0/PKG-INFO
```

### Comparing `pandoc-latex-margin-0.1.1/LICENSE` & `pandoc_latex_margin-1.0.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018-2021, Christophe Demko
+Copyright (c) 2018-2023, Christophe Demko
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pandoc-latex-margin-0.1.1/README.md` & `pandoc_latex_margin-1.0.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,52 @@
-# pandoc-latex-margin
-![Python package](https://github.com/chdemko/pandoc-latex-margin/workflows/Python%20package/badge.svg?branch=develop)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-margin/0.1.1.svg)](https://coveralls.io/github/chdemko/pandoc-latex-margin?branch=0.1.1)
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-latex-margin/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-margin/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-margin/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-margin?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-margin.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-margin/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-margin.svg)](https://pypi.org/project/pandoc-latex-margin/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-margin.svg)](https://pypi.org/project/pandoc-latex-margin/)
-[![License](https://img.shields.io/pypi/l/pandoc-latex-margin.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-margin/0.1.1/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-latex-margin.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-margin/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-margin.svg)](https://pypi.org/project/pandoc-latex-margin/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-margin.svg)](https://pypi.org/project/pandoc-latex-margin/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-latex-margin.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-margin.readthedocs.io/en/latest/)
 
 *pandoc-latex-margin* is a [pandoc] filter for changing margin size to `CodeBlock` and `Div` that have speficied classes or `latex-left-margin` and `latex-right-margin` attributes.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [wiki pages](https://github.com/chdemko/pandoc-latex-margin/wiki).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-latex-margin
-
-Installation
+Instructions
 ------------
 
-*pandoc-latex-margin* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
+*pandoc-latex-margin* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-latex-margin* as root using the bash command
+Install *pandoc-latex-margin* using the bash command
 
-    pip install pandoc-latex-margin
+~~~shell
+$ pip install pandoc-latex-margin
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-latex-margin
+~~~shell
+$ pip install --upgrade pandoc-latex-margin
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-margin
+~~~
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-margin
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
     apt-get update
-    apt-get install python-pip
+    apt-get install python3-pip
 
 [python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
 
 
 Getting Help
```

### Comparing `pandoc-latex-margin-0.1.1/pandoc_latex_margin.py` & `pandoc_latex_margin-1.0.0.0/pandoc_latex_margin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 #!/usr/bin/env python
 
 """
-Pandoc filter for changing margins in LaTeX
+Pandoc filter for changing margins in LaTeX.
 """
 
 import re
 
 from panflute import (  # type: ignore
-    RawBlock,
-    MetaList,
     MetaInlines,
+    MetaList,
+    RawBlock,
     RawInline,
     debug,
     run_filter,
 )
 
 
 # pylint:disable=line-too-long
 def get_correct_margin(length):
+    """
+    Get the margin.
+
+    Arguments
+    ---------
+    length
+        A margin in LaTeX notation.
+
+    Returns
+    -------
+        A correct margin.
+    """
     if (
         re.match(
             "^(-?([1-9][0-9]*)|0)(pt|mm|cm|in|ex|em|bp|pc|dd|cc|nd|nc|sp)$", length
         )
         is not None
     ):  # noqa: E501
         return length
@@ -31,26 +43,38 @@
         + " is not a correct LaTeX margin; using 0pt"
     )  # noqa: E501
     return "0pt"
 
 
 # pylint: disable=inconsistent-return-statements
 def margin(elem, doc):
-    # Is it in the right format and is it a Div or CodeBlock?
-    if doc.format in ["latex", "beamer"] and elem.tag in ["Div", "CodeBlock"]:
+    """
+    Add margin to element if needed.
 
+    Arguments
+    ---------
+    elem
+        A pandoc element
+    doc
+        The pandoc document
+
+    Returns
+    -------
+        A list of pandoc elements or None.
+    """
+    # Is it in the right format and is it a Div or CodeBlock?
+    if doc.format in ("latex", "beamer") and elem.tag in ("Div", "CodeBlock"):
         left = None
         right = None
 
         # Get the classes
         classes = set(elem.classes)
 
         # Loop on all fontsize definition
         for definition in doc.defined:
-
             # Are the classes correct?
             if classes >= definition["classes"]:
                 left = definition["left"]
                 right = definition["right"]
                 break
 
         # Is there a latex-margin-left attribute?
@@ -69,38 +93,55 @@
             return [
                 RawBlock(
                     "\\begin{pandocchangemargin}{" + left + "}{" + right + "}", "tex"
                 ),  # noqa: E501
                 elem,
                 RawBlock("\\end{pandocchangemargin}", "tex"),
             ]
+    return None
 
 
 def prepare(doc):
+    """
+    Prepare the document.
+
+    Arguments
+    ---------
+    doc
+        The pandoc document
+    """
     # Prepare the definitions
     doc.defined = []
 
     # Get the meta data
     meta = doc.get_metadata("pandoc-latex-margin")
 
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
             ):  # noqa: E501
                 add_definition(doc.defined, definition)
 
 
 def add_definition(defined, definition):
+    """
+    Add a definition.
+
+    Arguments
+    ---------
+    defined
+        A list of definition
+    definition
+        A new definition
+    """
     # Get the classes
     classes = definition["classes"]
 
     # Get the left margin
     if "left" in definition:
         left = get_correct_margin(definition["left"])
     else:
@@ -113,24 +154,32 @@
         right = "0pt"
 
     # Add a definition
     defined.append({"classes": set(classes), "left": left, "right": right})
 
 
 def finalize(doc):
+    """
+    Finalize the document.
+
+    Arguments
+    ---------
+    doc
+        The pandoc document
+    """
     # Add header-includes if necessary
     if "header-includes" not in doc.metadata:
         doc.metadata["header-includes"] = MetaList()
     # Convert header-includes to MetaList if necessary
     elif not isinstance(doc.metadata["header-includes"], MetaList):
         doc.metadata["header-includes"] = MetaList(
             doc.metadata["header-includes"]
         )  # noqa: E501
 
-    # Add usefull LaTex definition
+    # Add useful LaTex definition
     doc.metadata["header-includes"].append(
         MetaInlines(
             RawInline(
                 "\n".join(
                     [
                         "\\def\\pandocchangemargin#1#2{\\list{}{\\rightmargin#2\\leftmargin#1}\\item[]}",  # noqa: E501
                         "\\let\\endpandocchangemargin=\\endlist",
@@ -140,12 +189,24 @@
                 "tex",
             )
         )
     )
 
 
 def main(doc=None):
+    """
+    Process the transformation.
+
+    Arguments
+    ---------
+    doc
+        The pandoc document.
+
+    Returns
+    -------
+        The modified document.
+    """
     return run_filter(margin, prepare=prepare, doc=doc, finalize=finalize)
 
 
 if __name__ == "__main__":
     main()
```


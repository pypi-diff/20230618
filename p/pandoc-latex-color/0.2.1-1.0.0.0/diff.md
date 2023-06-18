# Comparing `tmp/pandoc-latex-color-0.2.1.tar.gz` & `tmp/pandoc_latex_color-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-latex-color-0.2.1.tar", last modified: Tue Feb 23 12:32:57 2021, max compression
+gzip compressed data, was "pandoc_latex_color-1.0.0.0.tar", max compression
```

## Comparing `pandoc-latex-color-0.2.1.tar` & `pandoc_latex_color-1.0.0.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 12:32:57.052971 pandoc-latex-color-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2021-02-23 12:32:45.000000 pandoc-latex-color-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-02-23 12:32:45.000000 pandoc-latex-color-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-02-23 12:32:57.052971 pandoc-latex-color-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2021-02-23 12:32:45.000000 pandoc-latex-color-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 12:32:57.052971 pandoc-latex-color-0.2.1/pandoc_latex_color.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4431 2021-02-23 12:32:56.000000 pandoc-latex-color-0.2.1/pandoc_latex_color.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      324 2021-02-23 12:32:56.000000 pandoc-latex-color-0.2.1/pandoc_latex_color.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-23 12:32:56.000000 pandoc-latex-color-0.2.1/pandoc_latex_color.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-02-23 12:32:56.000000 pandoc-latex-color-0.2.1/pandoc_latex_color.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-02-23 12:32:56.000000 pandoc-latex-color-0.2.1/pandoc_latex_color.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-02-23 12:32:56.000000 pandoc-latex-color-0.2.1/pandoc_latex_color.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9937 2021-02-23 12:32:45.000000 pandoc-latex-color-0.2.1/pandoc_latex_color.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-02-23 12:32:57.052971 pandoc-latex-color-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3808 2021-02-23 12:32:45.000000 pandoc-latex-color-0.2.1/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-18 20:38:34.130010 pandoc_latex_color-1.0.0.0/LICENSE
+-rw-r--r--   0        0        0     2830 2023-06-18 20:38:34.130010 pandoc_latex_color-1.0.0.0/README.md
+-rw-r--r--   0        0        0    11481 2023-06-18 20:38:34.134010 pandoc_latex_color-1.0.0.0/pandoc_latex_color.py
+-rw-r--r--   0        0        0     2900 2023-06-18 20:38:34.134010 pandoc_latex_color-1.0.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 pandoc_latex_color-1.0.0.0/PKG-INFO
```

### Comparing `pandoc-latex-color-0.2.1/LICENSE` & `pandoc_latex_color-1.0.0.0/LICENSE`

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

### Comparing `pandoc-latex-color-0.2.1/PKG-INFO` & `pandoc_latex_color-1.0.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,87 @@
 Metadata-Version: 2.1
 Name: pandoc-latex-color
-Version: 0.2.1
+Version: 1.0.0.0
 Summary: A pandoc filter for changing color in LaTeX
 Home-page: https://github.com/chdemko/pandoc-latex-color
+License: BSD-3-Clause
+Keywords: pandoc,filters,latex,color
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
-Maintainer: Christophe Demko
-Maintainer-email: chdemko@gmail.com
-License: BSD-3-Clause
-Download-URL: https://github.com/chdemko/pandoc-latex-color/archive/develop.zip
-Description: # pandoc-latex-color
-        ![Python package](https://github.com/chdemko/pandoc-latex-color/workflows/Python%20package/badge.svg?branch=0.2.1)
-        [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-color/0.2.1.svg)](https://coveralls.io/github/chdemko/pandoc-latex-color?branch=0.2.1)
-        [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-color.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-color/)
-        [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
-        [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
-        [![License](https://img.shields.io/pypi/l/pandoc-latex-color.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-color/0.2.1/LICENSE)
-        [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
-        [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
-        
-        *pandoc-latex-color* is a [pandoc] filter for setting the color to `Span`, and `Div` that have speficied classes or `latex-color` attribute.
-        
-        [pandoc]: http://pandoc.org/
-        
-        Documentation
-        -------------
-        
-        See the [wiki pages](https://github.com/chdemko/pandoc-latex-color/wiki).
-        
-        Usage
-        -----
-        
-        To apply the filter, use the following option with pandoc:
-        
-            --filter pandoc-latex-color
-        
-        Installation
-        ------------
-        
-        *pandoc-latex-color* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
-        
-        Install *pandoc-latex-color* as root using the bash command
-        
-            pip install pandoc-latex-color
-        
-        To upgrade to the most recent release, use
-        
-            pip install --upgrade pandoc-latex-color
-        
-        To upgrade to the current code, use
-        
-            pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-color
-        
-        `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
-        
-            apt-get update
-            apt-get install python-pip
-        
-        It uses the *xcolor* LaTeX package to handle correctly colors in spans and divs and the *soulutf8* package for highlighing the text.
-        
-        [python]: https://www.python.org
-        [on Windows]: https://www.python.org/downloads/windows
-        [PyPI]: https://pypi.org
-        
-        
-        Getting Help
-        ------------
-        
-        If you have any difficulties with *pandoc-latex-color*, please feel welcome to [file an issue] on github so that we can help.
-        
-        [file an issue]: https://github.com/chdemko/pandoc-latex-color/issues
-        
-        
-Keywords: pandoc filters latex color
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
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
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
+
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-latex-color/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-color/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-color/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-color?branch=develop)
+[![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-color.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-color/)
+[![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
+[![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
+[![License](https://img.shields.io/pypi/l/pandoc-latex-color.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-color/develop/LICENSE)
+[![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
+[![Development Status](https://img.shields.io/pypi/status/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-latex-color.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-color.readthedocs.io/en/latest/)
+
+*pandoc-latex-color* is a [pandoc] filter for setting the color to `Span`, and `Div` that have speficied classes or `latex-color` attribute.
+
+[pandoc]: http://pandoc.org/
+
+Instructions
+------------
+
+*pandoc-latex-color* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+
+Install *pandoc-latex-color* using the bash command
+
+~~~shell
+$ pip install pandoc-latex-color
+~~~
+
+To upgrade to the most recent release, use
+
+~~~shell
+$ pip install --upgrade pandoc-latex-color
+~~~
+
+To upgrade to the current code, use
+
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-color
+~~~
+
+`pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
+
+~~~shell
+$ sudo apt-get install python3-pip
+~~~
+
+It uses the *xcolor* LaTeX package to handle correctly colors in spans and divs and the *soulutf8* package for highlighing the text.
+
+[python]: https://www.python.org
+[on Windows]: https://www.python.org/downloads/windows
+[PyPI]: https://pypi.org
+
+
+Getting Help
+------------
+
+If you have any difficulties with *pandoc-latex-color*, please feel welcome to [file an issue] on github so that we can help.
+
+[file an issue]: https://github.com/chdemko/pandoc-latex-color/issues
+
+
```

### Comparing `pandoc-latex-color-0.2.1/README.md` & `pandoc_latex_color-1.0.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,51 @@
-# pandoc-latex-color
-![Python package](https://github.com/chdemko/pandoc-latex-color/workflows/Python%20package/badge.svg?branch=0.2.1)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-color/0.2.1.svg)](https://coveralls.io/github/chdemko/pandoc-latex-color?branch=0.2.1)
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-latex-color/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-latex-color/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-color/develop.svg)](https://coveralls.io/github/chdemko/pandoc-latex-color?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-color.svg)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-color/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
-[![License](https://img.shields.io/pypi/l/pandoc-latex-color.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-color/0.2.1/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-latex-color.svg)](https://raw.githubusercontent.com/chdemko/pandoc-latex-color/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-color.svg)](https://pypi.org/project/pandoc-latex-color/)
+[![Docs](https://img.shields.io/readthedocs/pandoc-latex-color.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-color.readthedocs.io/en/latest/)
 
 *pandoc-latex-color* is a [pandoc] filter for setting the color to `Span`, and `Div` that have speficied classes or `latex-color` attribute.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [wiki pages](https://github.com/chdemko/pandoc-latex-color/wiki).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-latex-color
-
-Installation
+Instructions
 ------------
 
-*pandoc-latex-color* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. Either python 2.7 or 3.x will do.
+*pandoc-latex-color* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-latex-color* as root using the bash command
+Install *pandoc-latex-color* using the bash command
 
-    pip install pandoc-latex-color
+~~~shell
+$ pip install pandoc-latex-color
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-latex-color
+~~~shell
+$ pip install --upgrade pandoc-latex-color
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-color
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-latex-color
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get install python3-pip
+~~~
 
 It uses the *xcolor* LaTeX package to handle correctly colors in spans and divs and the *soulutf8* package for highlighing the text.
 
 [python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
```

### Comparing `pandoc-latex-color-0.2.1/pandoc_latex_color.py` & `pandoc_latex_color-1.0.0.0/pandoc_latex_color.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 #!/usr/bin/env python
 
 """
-Pandoc filter for changing color in LaTeX
+Pandoc filter for changing color in LaTeX.
 """
 
 from panflute import (  # type: ignore
-    run_filter,
-    debug,
-    Span,
     Div,
-    RawInline,
     MetaInlines,
     MetaList,
     RawBlock,
+    RawInline,
+    Span,
+    debug,
+    run_filter,
 )
 
 
 def x11colors():
+    """
+    Get the x1 colors.
+
+    Returns
+    -------
+        A dictionary of colornames -> colorcode.
+    """
     # See https://www.w3.org/TR/css-color-3/#svg-color
     return {
         "aliceblue": "F0F8FF",
         "antiquewhite": "FAEBD7",
         "aqua": "00FFFF",
         "aquamarine": "7FFFD4",
         "azure": "F0FFFF",
@@ -166,37 +173,85 @@
         "whitesmoke": "F5F5F5",
         "yellow": "FFFF00",
         "yellowgreen": "9ACD32",
     }
 
 
 def color_code(color):
+    """
+    Get the LaTeX color code.
+
+    Arguments
+    ---------
+    color
+        X11 color name
+
+    Returns
+    -------
+        The LaTeX color code.
+    """
     return "\\color{" + color + "} "
 
 
 def bgcolor_code(color):
+    """
+    Get the LaTeX color code for the background.
+
+    Arguments
+    ---------
+    color
+        X11 color name
+
+    Returns
+    -------
+        The LaTeX color code for the background.
+    """
     if color:
         return "\\sethlcolor{" + color + "}"
     return False
 
 
 def get_correct_color(color):
+    """
+    Get a correct color name.
+
+    Arguments
+    ---------
+    color
+        Color name
+
+    Returns
+    -------
+        A X11 color name.
+    """
     if color in x11colors():
         return color
     if color:
         debug(
             "[WARNING] pandoc-latex-color: "
             + color
             + " is not a correct X11 color; using black"
         )
         return "black"
     return False
 
 
 def add_latex(elem, color, bgcolor):
+    """
+    Insert LaTeX code.
+
+    Arguments
+    ---------
+    elem
+        The pandoc element
+    color
+        The X11 color name
+    bgcolor
+        The X11 bgcolor name
+    """
     # Is it a Span?
     if isinstance(elem, Span):
         if bgcolor:
             elem.content.insert(0, RawInline(bgcolor + "\\hl{", "tex"))
             elem.content.append(RawInline("}", "tex"))
 
         elem.content.insert(0, RawInline(color, "tex"))
@@ -208,17 +263,30 @@
             elem.content.append(RawBlock("}", "tex"))
         else:
             elem.content.insert(0, RawBlock("{" + color, "tex"))
             elem.content.append(RawBlock("}", "tex"))
 
 
 def colorize(elem, doc):
-    # Is it in the right format and is it a Span, Div, Code or CodeBlock?
-    if doc.format in ["latex", "beamer"] and elem.tag in ["Span", "Div"]:
+    """
+    Colorize an element.
 
+    Arguments
+    ---------
+    elem
+        The pandoc element
+    doc
+        The pandoc document
+
+    Returns
+    -------
+        LaTeX code or None.
+    """
+    # Is it in the right format and is it a Span, Div, Code or CodeBlock?
+    if doc.format in ("latex", "beamer") and elem.tag in ("Span", "Div"):
         # Is there a latex-color attribute?
         if "latex-color" in elem.attributes or "latex-bgcolor" in elem.attributes:
             try:
                 color = elem.attributes["latex-color"]
             except KeyError:
                 color = "black"
 
@@ -234,44 +302,59 @@
             )
 
         # Get the classes
         classes = set(elem.classes)
 
         # Loop on all color definition
         for definition in doc.defined:
-
             # Are the classes correct?
             if classes >= definition["classes"]:
                 return add_latex(elem, definition["color"], definition["bgcolor"])
 
     return None
 
 
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
     meta = doc.get_metadata("pandoc-latex-color")
 
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
 
     # Get the color
     if "color" in definition:
         color = get_correct_color(definition["color"])
     else:
@@ -291,22 +374,30 @@
             "color": color_code(color),
             "bgcolor": bgcolor_code(bgcolor),
         }
     )
 
 
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
         doc.metadata["header-includes"] = MetaList(doc.metadata["header-includes"])
 
-    # Add usefull LaTexPackage
+    # Add useful LaTexPackage
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\\usepackage{xcolor}", "tex"))
     )
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\\usepackage{soulutf8,color}", "tex"))
     )
     doc.metadata["header-includes"].append(
@@ -337,12 +428,24 @@
             "\\makeatother",
         ]
         for line in special_beamer:
             doc.metadata["header-includes"].append(MetaInlines(RawInline(line, "tex")))
 
 
 def main(doc=None):
+    """
+    Convert the pandoc document.
+
+    Arguments
+    ---------
+    doc
+        The pandoc document
+
+    Returns
+    -------
+        The modified pandoc document
+    """
     return run_filter(colorize, prepare=prepare, finalize=finalize, doc=doc)
 
 
 if __name__ == "__main__":
     main()
```


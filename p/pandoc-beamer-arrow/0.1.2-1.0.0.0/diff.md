# Comparing `tmp/pandoc-beamer-arrow-0.1.2.tar.gz` & `tmp/pandoc_beamer_arrow-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pandoc-beamer-arrow-0.1.2.tar", last modified: Thu Dec 12 19:55:04 2019, max compression
+gzip compressed data, was "pandoc_beamer_arrow-1.0.0.0.tar", max compression
```

## Comparing `pandoc-beamer-arrow-0.1.2.tar` & `pandoc_beamer_arrow-1.0.0.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 chdemko   (1000) chdemko   (1000)        0 2019-12-12 19:55:04.000000 pandoc-beamer-arrow-0.1.2/
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)     3529 2019-12-12 19:53:58.000000 pandoc-beamer-arrow-0.1.2/setup.py
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)       55 2019-12-11 23:27:39.000000 pandoc-beamer-arrow-0.1.2/MANIFEST.in
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)      133 2019-12-12 19:55:04.000000 pandoc-beamer-arrow-0.1.2/setup.cfg
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)    11325 2019-12-12 19:49:33.000000 pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.py
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)    11432 2019-12-12 19:55:04.000000 pandoc-beamer-arrow-0.1.2/PKG-INFO
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)     9233 2019-12-12 19:54:52.000000 pandoc-beamer-arrow-0.1.2/README.md
-drwxr-xr-x   0 chdemko   (1000) chdemko   (1000)        0 2019-12-12 19:55:04.000000 pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.egg-info/
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)       20 2019-12-12 19:55:03.000000 pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.egg-info/top_level.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)      331 2019-12-12 19:55:04.000000 pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.egg-info/SOURCES.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)        1 2019-12-12 19:55:03.000000 pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.egg-info/dependency_links.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)       68 2019-12-12 19:55:03.000000 pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.egg-info/requires.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)       66 2019-12-12 19:55:03.000000 pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.egg-info/entry_points.txt
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)    11432 2019-12-12 19:55:03.000000 pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.egg-info/PKG-INFO
--rw-r--r--   0 chdemko   (1000) chdemko   (1000)     1516 2019-12-11 23:27:39.000000 pandoc-beamer-arrow-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1521 2023-06-18 18:02:19.466679 pandoc_beamer_arrow-1.0.0.0/LICENSE
+-rw-r--r--   0        0        0     9288 2023-06-18 18:02:19.466679 pandoc_beamer_arrow-1.0.0.0/README.md
+-rw-r--r--   0        0        0    11606 2023-06-18 18:02:19.466679 pandoc_beamer_arrow-1.0.0.0/pandoc_beamer_arrow.py
+-rw-r--r--   0        0        0     2920 2023-06-18 18:02:19.466679 pandoc_beamer_arrow-1.0.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10394 1970-01-01 00:00:00.000000 pandoc_beamer_arrow-1.0.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pandoc-beamer-arrow-0.1.2/pandoc_beamer_arrow.py` & `pandoc_beamer_arrow-1.0.0.0/pandoc_beamer_arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
 
-"""
-Pandoc filter for adding admonition in LaTeX
-"""
-from panflute import (
-    run_filter,
-    RawInline,
-    MetaList,
+"""Pandoc filter for adding admonition in LaTeX."""
+
+import contextlib
+
+from panflute import (  # type: ignore
     MetaInlines,
-    convert_text,
+    MetaList,
     Plain,
+    RawInline,
+    convert_text,
     debug,
+    run_filter,
 )
 
 
-def x11colors():
+def x11colors():  # noqa: CFQ001
     """
-    Get the x11 colors
+    Get the x11 colors.
 
     Returns
     -------
         The x11 colors
     """
     # See https://www.w3.org/TR/css-color-3/#svg-color
     return {
@@ -173,29 +174,29 @@
         "yellowgreen": "9ACD32",
     }
 
 
 # pylint: disable=inconsistent-return-statements,too-many-branches,too-many-statements
 def tikz(elem, doc):
     """
-    Add admonition to elem
+    Add admonition to elem.
 
     Arguments
     ---------
-        elem:
-            The current element
-        doc:
-            The pandoc document
+    elem
+        The current element
+    doc
+        The pandoc document
 
     Returns
     -------
-        The modified element
+        The modified element or None
     """
     # Is it in the right format and is it Div or a CodeBlock?
-    if doc.format in ["beamer"] and elem.tag in ["Span"]:
+    if doc.format in ("beamer") and elem.tag in ("Span"):
         # Is there a latex-admonition-color attribute?
         if "beamer-arrow-node" in elem.classes:
             text = convert_text(
                 Plain(*elem.content), input_format="panflute", output_format="latex"
             )
 
             options = ["anchor=base"]
@@ -265,19 +266,29 @@
                 f"({elem.attributes['src']}) "
                 f"edge "
                 f"[{','.join(angles)}] "
                 f"({elem.attributes['dest']});"
                 f"\\end{{tikzpicture}}",
                 format="tex",
             )
+    return None
 
 
 def get_range(elem, _):
     """
     Get the range of display for an element.
+
+    Arguments
+    ---------
+    elem
+        A pandoc element.
+
+    Returns
+    -------
+        A range represented by a couple.
     """
     from_value = elem.attributes.get("from", "")
     if bool(from_value):
         try:
             from_value = max(1, int(from_value))
         except ValueError:
             debug(f"pandoc-beamer-arrow: from value '{from_value}' is not " f"correct")
@@ -291,69 +302,78 @@
             to_value = max(1, int(to_value))
         except ValueError:
             debug(f"pandoc-beamer-arrow: to value '{to_value}' is not " f"correct")
             to_value = ""
     else:
         to_value = ""
 
-    try:
+    with contextlib.suppress(TypeError):
         if to_value < from_value:
             debug(
                 f"pandoc-beamer-arrow: from value '{from_value}' and "
                 f" to value '{to_value}' are incompatible"
             )
             from_value = ""
             to_value = ""
-    except TypeError:
-        pass
 
     return (from_value, to_value)
 
 
 def get_color(elem, doc):
     """
     Get the color of display for an element.
+
+    Arguments
+    ---------
+    elem
+        A pandoc element
+    doc
+        The pandoc document.
+
+    Returns
+    -------
+        The color.
     """
     if "color" in elem.attributes:
         color = elem.attributes["color"]
         if color in doc.x11colors:
             return color
         debug(f"pandoc-beamer-arrow: color '{color}' is not correct")
     return ""
 
 
 def prepare(doc):
     """
-    Prepare the document
+    Prepare the document.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
     """
     doc.x11colors = x11colors()
 
 
 def finalize(doc):
     """
-    Finalize the pandoc document
+    Finalize the pandoc document.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
     """
     # Add header-includes if necessary
     if "header-includes" not in doc.metadata:
         doc.metadata["header-includes"] = MetaList()
     # Convert header-includes to MetaList if necessary
     elif not isinstance(doc.metadata["header-includes"], MetaList):
         doc.metadata["header-includes"] = MetaList(doc.metadata["header-includes"])
 
-    # Add usefull LaTexPackage
+    # Add useful LaTexPackage
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\\usepackage{tikz}", "tex"))
     )
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\\tikzstyle{every picture}+=[remember picture]", "tex"))
     )
     doc.metadata["header-includes"].append(
@@ -365,30 +385,31 @@
                 "\\tikzset{onslide/.code args={<#1>#2}{\\only<#1>{\\pgfkeysalso{#2}}}}",
                 "tex",
             )
         )
     )
 
     # Define x11 colors
-    tex = []
-    for name, color in doc.x11colors.items():
-        tex.append("\\definecolor{" + name.lower() + "}{HTML}{" + color + "}")
+    tex = [
+        f"\\definecolor{{{name.lower()}}}{{HTML}}{{{color}}}"
+        for name, color in doc.x11colors.items()
+    ]
     doc.metadata["header-includes"].append(
         MetaInlines(RawInline("\n".join(tex), "tex"))
     )
 
 
 def main(doc=None):
     """
-    Main function called by the script.
+    Convert the document.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
 
     Returns
     -------
         The modified pandoc document
     """
     return run_filter(tikz, prepare=prepare, finalize=finalize, doc=doc)
```

### Comparing `pandoc-beamer-arrow-0.1.2/README.md` & `pandoc_beamer_arrow-1.0.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-# pandoc-beamer-arrow
-[![Build Status](https://img.shields.io/travis/chdemko/pandoc-beamer-arrow/0.1.2.svg?logo=travis)](https://travis-ci.org/chdemko/pandoc-beamer-arrow/branches)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-arrow/0.1.2.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-arrow?branch=0.1.2)
+# Installation
+
+[![Python package](https://github.com/chdemko/pandoc-beamer-arrow/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-beamer-arrow/actions/workflows/python-package.yml)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-arrow/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-arrow?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-beamer-arrow/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-beamer-arrow/)
 [![Code Beat](https://codebeat.co/badges/4d7e44d2-04ed-4c66-b8d2-ea1d28bc16ee)](https://codebeat.co/projects/github-com-chdemko-pandoc-beamer-arrow-develop/)
-[![Codacy](https://img.shields.io/codacy/grade/5e04e80fe4124ea18911026086fdafe9.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-beamer-arrow)
+[![Codacy](https://img.shields.io/codacy/grade/5e04e80fe4124ea18911026086fdafe9.svg?logo=codacy&logoColor=white)](https://app.codacy.com/gh/chdemko/pandoc-beamer-arrow/)
 [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-arrow/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-arrow)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-beamer-arrow.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-arrow/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-beamer-arrow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-arrow/)
-[![License](https://img.shields.io/pypi/l/pandoc-beamer-arrow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-arrow/0.1.2/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-beamer-arrow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-arrow/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-beamer-arrow.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-arrow/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Downloads](https://pepy.tech/badge/pandoc-beamer-arrow)](https://pepy.tech/project/pandoc-beamer-arrow)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-beamer-arrow.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-arrow/)
 [![Docs](https://img.shields.io/readthedocs/pandoc-beamer-arrow.svg?logo=read-the-docs&logoColor=white)](http://pandoc-beamer-arrow.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
-*pandoc-beamer-arrow* is a [pandoc] filter for adding admonition to `div`s or `codeblock`s elements.
-
-It uses the *tcolorbox* LaTeX package to generate admonitions and the *footnote* LaTeX package to handle correctly footnotes in admonition.
+*pandoc-beamer-arrow* is a [pandoc] filter for creating arrows between text
+elements for beamer presentation.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [Read the docs pages](http://pandoc-beamer-arrow.readthedocs.io/en/0.1.2/).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-beamer-arrow
-
-Installation
+Instructions
 ------------
 
-*pandoc-beamer-arrow* requires [python 3.6], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+*pandoc-beamer-arrow* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-beamer-arrow* as root using the bash command
+Install *pandoc-beamer-arrow* using the bash command
 
-    pip install pandoc-beamer-arrow
+~~~shell
+$ pip install pandoc-beamer-arrow
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-beamer-arrow
+~~~shell
+$ pip install --upgrade pandoc-beamer-arrow
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-arrow
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-arrow
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get install python3-pip
+~~~
 
 Make sure you have the
 
 * *xcolor*
 
 LaTeX packages. On linux you have to install some extra libraries **before** *pandoc-beamer-arrow*. On a Debian-based system (including Ubuntu), you can install it as root using
 
-	apt-get texlive-latex-extra
+~~~shell
+$ sudo apt-get texlive-latex-extra
+~~~
 
-[python 3.6]: https://www.python.org
+[python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
 
 
 Getting Help
 ------------
```

### Comparing `pandoc-beamer-arrow-0.1.2/LICENSE` & `pandoc_beamer_arrow-1.0.0.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2019, Christophe Demko
+Copyright (c) 2019-2023, Christophe Demko
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```


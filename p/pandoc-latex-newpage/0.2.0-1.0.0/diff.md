# Comparing `tmp/pandoc-latex-newpage-0.2.0.tar.gz` & `tmp/pandoc_latex_newpage-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-latex-newpage-0.2.0.tar", last modified: Tue Aug  2 14:13:07 2022, max compression
+gzip compressed data, was "pandoc_latex_newpage-1.0.0.tar", max compression
```

## Comparing `pandoc-latex-newpage-0.2.0.tar` & `pandoc_latex_newpage-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 14:13:07.550768 pandoc-latex-newpage-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-08-02 14:12:56.000000 pandoc-latex-newpage-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-02 14:12:56.000000 pandoc-latex-newpage-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3854 2022-08-02 14:13:07.550768 pandoc-latex-newpage-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2681 2022-08-02 14:12:56.000000 pandoc-latex-newpage-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 14:13:07.550768 pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3854 2022-08-02 14:13:07.000000 pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-08-02 14:13:07.000000 pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 14:13:07.000000 pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-02 14:13:07.000000 pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-02 14:13:07.000000 pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-02 14:13:07.000000 pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-08-02 14:12:56.000000 pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-08-02 14:13:07.550768 pandoc-latex-newpage-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3724 2022-08-02 14:12:56.000000 pandoc-latex-newpage-0.2.0/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-18 11:57:30.593497 pandoc_latex_newpage-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8462 2023-06-18 11:57:30.593497 pandoc_latex_newpage-1.0.0/README.md
+-rw-r--r--   0        0        0     1561 2023-06-18 11:57:30.597497 pandoc_latex_newpage-1.0.0/pandoc_latex_newpage.py
+-rw-r--r--   0        0        0     2929 2023-06-18 11:57:30.597497 pandoc_latex_newpage-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9579 1970-01-01 00:00:00.000000 pandoc_latex_newpage-1.0.0/PKG-INFO
```

### Comparing `pandoc-latex-newpage-0.2.0/LICENSE` & `pandoc_latex_newpage-1.0.0/LICENSE`

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

### Comparing `pandoc-latex-newpage-0.2.0/pandoc_latex_newpage.py` & `pandoc_latex_newpage-1.0.0/pandoc_latex_newpage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,36 @@
 #!/usr/bin/env python
 
 """
-Pandoc filter for converting horizontal rule to new page in LaTeX
+Pandoc filter for converting horizontal rule to new page in LaTeX.
 """
 
-from panflute import HorizontalRule, MetaBool, MetaMap, RawBlock, run_filter  # type: ignore
+from panflute import (  # type: ignore
+    HorizontalRule,
+    MetaBool,
+    MetaMap,
+    RawBlock,
+    run_filter,
+)
 
 
 def newpage(elem, doc):
-    """
-    Replace HorizontalRule by a \\clearpage or a \\cleardoublepage
+    r"""
+    Replace HorizontalRule by a \clearpage or a \cleardoublepage.
+
+    Arguments
+    ---------
+    elem
+        A pandoc element
+    doc
+        pandoc document
+
+    Returns
+    -------
+        A RawBlock or None.
     """
     # Is it in the right format and is it an HorizontalRule?
     if doc.format == "latex" and isinstance(elem, HorizontalRule):
         if doc.double:
             return RawBlock("\\cleardoublepage", "tex")
         return RawBlock("\\clearpage", "tex")
     return None
@@ -21,29 +38,39 @@
 
 def prepare(doc):
     """
     Prepare document.
 
     Arguments
     ---------
-        doc: pandoc document
+    doc
+        pandoc document
     """
     doc.double = True
 
-    if "pandoc-latex-newpage" in doc.metadata.content and isinstance(
-        doc.metadata.content["pandoc-latex-newpage"], MetaMap
+    if (
+        "pandoc-latex-newpage" in doc.metadata.content
+        and isinstance(doc.metadata.content["pandoc-latex-newpage"], MetaMap)
+        and "double" in doc.metadata.content["pandoc-latex-newpage"]
+        and isinstance(doc.metadata.content["pandoc-latex-newpage"]["double"], MetaBool)
     ):
-        if "double" in doc.metadata.content["pandoc-latex-newpage"] and isinstance(
-            doc.metadata.content["pandoc-latex-newpage"]["double"], MetaBool
-        ):
-            doc.double = doc.metadata.content["pandoc-latex-newpage"]["double"].boolean
+        doc.double = doc.metadata.content["pandoc-latex-newpage"]["double"].boolean
 
 
 def main(doc=None):
     """
-    main function
+    Convert the pandoc document.
+
+    Arguments
+    ---------
+    doc
+        pandoc document
+
+    Returns
+    -------
+        The modified document.
     """
     return run_filter(newpage, prepare=prepare, doc=doc)
 
 
 if __name__ == "__main__":
     main()
```


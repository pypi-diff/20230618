# Comparing `tmp/sans-1.2.2.tar.gz` & `tmp/sans-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sans-1.2.2.tar", last modified: Thu Jun  8 20:36:47 2023, max compression
+gzip compressed data, was "sans-1.2.3.tar", last modified: Sun Jun 18 21:46:15 2023, max compression
```

## Comparing `sans-1.2.2.tar` & `sans-1.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:36:47.516878 sans-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:36:47.508878 sans-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:36:47.512878 sans-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-08 20:36:31.000000 sans-1.2.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-08 20:36:31.000000 sans-1.2.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-08 20:36:31.000000 sans-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-08 20:36:31.000000 sans-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 20:36:31.000000 sans-1.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-08 20:36:31.000000 sans-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-08 20:36:47.516878 sans-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-08 20:36:31.000000 sans-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:36:47.512878 sans-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 20:36:31.000000 sans-1.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 20:36:31.000000 sans-1.2.2/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-08 20:36:31.000000 sans-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 20:36:31.000000 sans-1.2.2/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 20:36:31.000000 sans-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 20:36:31.000000 sans-1.2.2/docs/limiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 20:36:31.000000 sans-1.2.2/docs/lock.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 20:36:31.000000 sans-1.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 20:36:31.000000 sans-1.2.2/docs/response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 20:36:31.000000 sans-1.2.2/docs/url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 20:36:31.000000 sans-1.2.2/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-08 20:36:31.000000 sans-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-08 20:36:31.000000 sans-1.2.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:36:47.516878 sans-1.2.2/sans/
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-08 20:36:31.000000 sans-1.2.2/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-06-08 20:36:31.000000 sans-1.2.2/sans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-08 20:36:31.000000 sans-1.2.2/sans/_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-08 20:36:31.000000 sans-1.2.2/sans/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-08 20:36:31.000000 sans-1.2.2/sans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27979 2023-06-08 20:36:31.000000 sans-1.2.2/sans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-08 20:36:31.000000 sans-1.2.2/sans/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-08 20:36:31.000000 sans-1.2.2/sans/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-06-08 20:36:31.000000 sans-1.2.2/sans/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:36:31.000000 sans-1.2.2/sans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-08 20:36:31.000000 sans-1.2.2/sans/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-08 20:36:31.000000 sans-1.2.2/sans/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-08 20:36:31.000000 sans-1.2.2/sans/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:36:47.516878 sans-1.2.2/sans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-08 20:36:47.000000 sans-1.2.2/sans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-08 20:36:47.000000 sans-1.2.2/sans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:36:47.000000 sans-1.2.2/sans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 20:36:47.000000 sans-1.2.2/sans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 20:36:47.000000 sans-1.2.2/sans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 20:36:47.000000 sans-1.2.2/sans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:36:47.516878 sans-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-08 20:36:31.000000 sans-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:46:15.938080 sans-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:46:15.934080 sans-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:46:15.934080 sans-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-18 21:46:05.000000 sans-1.2.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-18 21:46:05.000000 sans-1.2.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-18 21:46:05.000000 sans-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-18 21:46:05.000000 sans-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-18 21:46:05.000000 sans-1.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-18 21:46:05.000000 sans-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-18 21:46:15.938080 sans-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-18 21:46:05.000000 sans-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:46:15.934080 sans-1.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 21:46:05.000000 sans-1.2.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-18 21:46:05.000000 sans-1.2.3/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-18 21:46:05.000000 sans-1.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-18 21:46:05.000000 sans-1.2.3/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-18 21:46:05.000000 sans-1.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-18 21:46:05.000000 sans-1.2.3/docs/limiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-18 21:46:05.000000 sans-1.2.3/docs/lock.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-18 21:46:05.000000 sans-1.2.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 21:46:05.000000 sans-1.2.3/docs/response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-18 21:46:05.000000 sans-1.2.3/docs/url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 21:46:05.000000 sans-1.2.3/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-18 21:46:05.000000 sans-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-18 21:46:05.000000 sans-1.2.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:46:15.938080 sans-1.2.3/sans/
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-18 21:46:05.000000 sans-1.2.3/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-18 21:46:05.000000 sans-1.2.3/sans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-18 21:46:05.000000 sans-1.2.3/sans/_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-18 21:46:05.000000 sans-1.2.3/sans/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-18 21:46:05.000000 sans-1.2.3/sans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27979 2023-06-18 21:46:05.000000 sans-1.2.3/sans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-18 21:46:05.000000 sans-1.2.3/sans/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-18 21:46:05.000000 sans-1.2.3/sans/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-06-18 21:46:05.000000 sans-1.2.3/sans/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 21:46:05.000000 sans-1.2.3/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-18 21:46:05.000000 sans-1.2.3/sans/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-18 21:46:05.000000 sans-1.2.3/sans/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-18 21:46:05.000000 sans-1.2.3/sans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:46:15.938080 sans-1.2.3/sans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-18 21:46:15.000000 sans-1.2.3/sans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-18 21:46:15.000000 sans-1.2.3/sans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:46:15.000000 sans-1.2.3/sans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-18 21:46:15.000000 sans-1.2.3/sans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-18 21:46:15.000000 sans-1.2.3/sans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 21:46:15.000000 sans-1.2.3/sans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 21:46:15.938080 sans-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-18 21:46:05.000000 sans-1.2.3/setup.py
```

### Comparing `sans-1.2.2/.github/workflows/codeql-analysis.yml` & `sans-1.2.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/.github/workflows/pythonpublish.yml` & `sans-1.2.3/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/.gitignore` & `sans-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/.pre-commit-config.yaml` & `sans-1.2.3/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     -   id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.313
+    rev: v1.1.314
     hooks:
     -   id: pyright
         additional_dependencies:
             # required dependencies
         -   httpx ~= 0.23
         -   importlib_metadata >= 1.4.0; python_version < "3.8"
```

### Comparing `sans-1.2.2/LICENSE` & `sans-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/PKG-INFO` & `sans-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.2.2
+Version: 1.2.3
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -118,15 +118,15 @@
    async with sans.AsyncClient() as client:
       request = sans.Nation(
          "darcania",
          "fullname population flag census",
          mode="score",
          scale="65 66",
       )
-      root = (await client.send(request)).xml
+      root = (await client.get(request)).xml
       sans.indent(root)
       print(ET.tostring(root, encoding="unicode"))
 
       async with client.stream("GET", sans.RegionsDump()) as response:
          async for region in response.aiter_xml():
             sans.indent(region)
             print(ET.tostring(region, encoding="unicode"))
```

### Comparing `sans-1.2.2/README.md` & `sans-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
    async with sans.AsyncClient() as client:
       request = sans.Nation(
          "darcania",
          "fullname population flag census",
          mode="score",
          scale="65 66",
       )
-      root = (await client.send(request)).xml
+      root = (await client.get(request)).xml
       sans.indent(root)
       print(ET.tostring(root, encoding="unicode"))
 
       async with client.stream("GET", sans.RegionsDump()) as response:
          async for region in response.aiter_xml():
             sans.indent(region)
             print(ET.tostring(region, encoding="unicode"))
```

### Comparing `sans-1.2.2/docs/Makefile` & `sans-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/docs/conf.py` & `sans-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/docs/make.bat` & `sans-1.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/pyproject.toml` & `sans-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/__init__.py` & `sans-1.2.3/sans/__init__.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/__main__.py` & `sans-1.2.3/sans/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
                     pretty_print(response.xml)
                 elif response.content_type.startswith("text/"):
                     print(
                         Syntax(
                             response.text,
                             response.content_type.partition("/")[2],
                             background_color="default",
+                            word_wrap=True,
                         )
                     )
                 else:
                     print(response.content)
                 if known.quit:
                     print("Exiting...", file=sys.stderr)
                     sys.exit(0)
@@ -205,14 +206,15 @@
     print(
         Syntax(
             ET.tostring(element, encoding="unicode").strip(),
             "xml",
             background_color="default",
             indent_guides=True,
             tab_size=len(space),
+            word_wrap=True,
         )
     )
 
 
 if __name__ == "__main__":
     logging.captureWarnings(True)
     sys.exit(main())
```

### Comparing `sans-1.2.2/sans/_lock.py` & `sans-1.2.3/sans/_lock.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/auth.py` & `sans-1.2.3/sans/auth.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/client.py` & `sans-1.2.3/sans/client.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/client.pyi` & `sans-1.2.3/sans/client.pyi`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/decoder.py` & `sans-1.2.3/sans/decoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,20 +71,34 @@
 
 
 try:
     from lxml.etree import (
         XMLParser as LXMLParser,
         _Element as LElement,
     )
+    from lxml.objectify import ObjectifiedElement, ObjectifyElementClassLookup
 except ImportError:
     pass
 else:
 
     class LXMLDecoder:
         def __init__(self, encoding: str | None = None) -> None:
             self._parser = LXMLParser(encoding=encoding)
 
         def decode(self, data: bytes) -> None:
             self._parser.feed(data)
 
         def flush(self) -> LElement:
             return self._parser.close()
+
+    class ObjectifyDecoder:
+        def __init__(self, encoding: str | None = None) -> None:
+            self._parser = parser = LXMLParser(
+                encoding=encoding, remove_blank_text=True
+            )
+            parser.set_element_class_lookup(ObjectifyElementClassLookup())
+
+        def decode(self, data: bytes) -> None:
+            self._parser.feed(data)
+
+        def flush(self) -> ObjectifiedElement:
+            return self._parser.close()  # type: ignore
```

### Comparing `sans-1.2.2/sans/errors.py` & `sans-1.2.3/sans/errors.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/limiter.py` & `sans-1.2.3/sans/limiter.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/response.py` & `sans-1.2.3/sans/response.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 
     HAS_XMLTODICT = True
 except ImportError:
     HAS_XMLTODICT = False
 
 try:
     from lxml.etree import _Element
+    from lxml.objectify import ObjectifiedElement
 
     HAS_LXML = True
 except ImportError:
     HAS_LXML = False
 else:
-    from .decoder import LXMLDecoder
+    from .decoder import LXMLDecoder, ObjectifyDecoder
 
 __all__ = ["Response"]
 
 
 class Response(httpx.Response):
     @property
     def content_type(self) -> str:
@@ -97,12 +98,21 @@
             if not hasattr(self, "_lxml"):
                 content = self.content
                 decoder = LXMLDecoder(self.encoding)
                 decoder.decode(content)
                 self._lxml = decoder.flush()
             return self._lxml
 
+        @property
+        def objectified(self) -> ObjectifiedElement:
+            if not hasattr(self, "_objectified"):
+                content = self.content
+                decoder = ObjectifyDecoder(self.encoding)
+                decoder.decode(content)
+                self._objectified = decoder.flush()
+            return self._objectified
+
     def raise_for_status(self) -> None:
         try:
             return super().raise_for_status()
         except httpx.HTTPStatusError as exc:
             raise narrow(exc).with_traceback(exc.__traceback__) from None
```

### Comparing `sans-1.2.2/sans/url.py` & `sans-1.2.3/sans/url.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans/utils.py` & `sans-1.2.3/sans/utils.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.2/sans.egg-info/PKG-INFO` & `sans-1.2.3/sans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.2.2
+Version: 1.2.3
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -118,15 +118,15 @@
    async with sans.AsyncClient() as client:
       request = sans.Nation(
          "darcania",
          "fullname population flag census",
          mode="score",
          scale="65 66",
       )
-      root = (await client.send(request)).xml
+      root = (await client.get(request)).xml
       sans.indent(root)
       print(ET.tostring(root, encoding="unicode"))
 
       async with client.stream("GET", sans.RegionsDump()) as response:
          async for region in response.aiter_xml():
             sans.indent(region)
             print(ET.tostring(region, encoding="unicode"))
```

### Comparing `sans-1.2.2/sans.egg-info/SOURCES.txt` & `sans-1.2.3/sans.egg-info/SOURCES.txt`

 * *Files identical despite different names*


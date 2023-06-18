# Comparing `tmp/strip-tags-0.4.tar.gz` & `tmp/strip-tags-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strip-tags-0.4.tar", last modified: Sun Jun 18 08:09:05 2023, max compression
+gzip compressed data, was "strip-tags-0.4.1.tar", last modified: Sun Jun 18 08:39:13 2023, max compression
```

## Comparing `strip-tags-0.4.tar` & `strip-tags-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:09:05.822164 strip-tags-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 08:08:47.000000 strip-tags-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-18 08:09:05.822164 strip-tags-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-18 08:08:47.000000 strip-tags-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 08:09:05.822164 strip-tags-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 08:08:47.000000 strip-tags-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:09:05.822164 strip-tags-0.4/strip_tags/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 08:08:47.000000 strip-tags-0.4/strip_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 08:08:47.000000 strip-tags-0.4/strip_tags/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-18 08:08:47.000000 strip-tags-0.4/strip_tags/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-18 08:08:47.000000 strip-tags-0.4/strip_tags/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:09:05.822164 strip-tags-0.4/strip_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:09:05.822164 strip-tags-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-18 08:08:47.000000 strip-tags-0.4/tests/test_strip_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:39:13.579093 strip-tags-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 08:38:56.000000 strip-tags-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-18 08:39:13.579093 strip-tags-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-18 08:38:56.000000 strip-tags-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 08:39:13.579093 strip-tags-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-18 08:38:56.000000 strip-tags-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:39:13.579093 strip-tags-0.4.1/strip_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 08:38:56.000000 strip-tags-0.4.1/strip_tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 08:38:56.000000 strip-tags-0.4.1/strip_tags/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-18 08:38:56.000000 strip-tags-0.4.1/strip_tags/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-18 08:38:56.000000 strip-tags-0.4.1/strip_tags/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:39:13.579093 strip-tags-0.4.1/strip_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 08:39:13.000000 strip-tags-0.4.1/strip_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:39:13.579093 strip-tags-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-18 08:38:56.000000 strip-tags-0.4.1/tests/test_strip_tags.py
```

### Comparing `strip-tags-0.4/LICENSE` & `strip-tags-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strip-tags-0.4/PKG-INFO` & `strip-tags-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strip-tags
-Version: 0.4
+Version: 0.4.1
 Summary: Strip tags from HTML, optionally from areas identified by CSS selectors
 Home-page: https://github.com/simonw/strip-tags
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/strip-tags/issues
 Project-URL: CI, https://github.com/simonw/strip-tags/actions
 Project-URL: Changelog, https://github.com/simonw/strip-tags/releases
@@ -119,17 +119,23 @@
 <div>
 <h1>This has tags</h1>
 
 <p>And whitespace too</p>
 </div>
 Ignore this bit.
 """
-stripped = strip_tags(html, ["div"], minify=True)
+stripped = strip_tags(html, ["div"], minify=True, keep_tags=["h1"])
 print(stripped)
 ```
+Output:
+```
+<h1>This has tags</h1>
+
+And whitespace too
+```
 
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 ```bash
 cd strip-tags
 python -m venv venv
```

### Comparing `strip-tags-0.4/README.md` & `strip-tags-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,23 @@
 <div>
 <h1>This has tags</h1>
 
 <p>And whitespace too</p>
 </div>
 Ignore this bit.
 """
-stripped = strip_tags(html, ["div"], minify=True)
+stripped = strip_tags(html, ["div"], minify=True, keep_tags=["h1"])
 print(stripped)
 ```
+Output:
+```
+<h1>This has tags</h1>
+
+And whitespace too
+```
 
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 ```bash
 cd strip-tags
 python -m venv venv
@@ -123,8 +129,8 @@
 Now install the dependencies and test dependencies:
 ```bash
 pip install -e '.[test]'
 ```
 To run the tests:
 ```bash
 pytest
-```
+```
```

### Comparing `strip-tags-0.4/setup.py` & `strip-tags-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.4"
+VERSION = "0.4.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `strip-tags-0.4/strip_tags/cli.py` & `strip-tags-0.4.1/strip_tags/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 @click.command()
 @click.version_option()
 @click.argument("selectors", nargs=-1)
 @click.option("-i", "--input", type=click.File("r"), default="-")
 @click.option("-m", "--minify", is_flag=True, help="Minify whitespace")
-# multiple -t
 @click.option("keep_tags", "-t", "--keep-tag", multiple=True, help="Keep these <tags>")
 @click.option("--all-attrs", is_flag=True, help="Include all attributes on kept tags")
 @click.option("--first", is_flag=True, help="First element matching the selectors")
 def cli(selectors, input, minify, keep_tags, all_attrs, first):
     """
     Strip tags from HTML, optionally from areas identified by CSS selectors
```

### Comparing `strip-tags-0.4/strip_tags/lib.py` & `strip-tags-0.4.1/strip_tags/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,23 +167,23 @@
             minified = _whitespace_re.sub(repl, node)
             if minified == "\n":
                 minified = " "
             return minified
         else:
             return node
     elif node.name == "pre":
-        # TODO: Handle 'pre' in keep_tags
-        return str(node.text)  # keep <pre> tags as-is
+        s = str(node.text)
+        if "pre" in keep_tags:
+            return tag_with_attributes(node, s, all_attrs)
+        else:
+            return s
     else:
         bits = [
             process_node(child, minify, keep_tags, all_attrs) for child in node.contents
         ]
-        # print(bits)
-        # if bits == ['', 'Uses', '', 'Examples', '', 'Plugins', '']:
-        #    breakpoint()
         s = "".join(bits)
         if node.name in keep_tags:
             s = tag_with_attributes(node, s, all_attrs)
         return s
 
 
 _whitespace_re = re.compile(r"\s+")
```

### Comparing `strip-tags-0.4/strip_tags.egg-info/PKG-INFO` & `strip-tags-0.4.1/strip_tags.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strip-tags
-Version: 0.4
+Version: 0.4.1
 Summary: Strip tags from HTML, optionally from areas identified by CSS selectors
 Home-page: https://github.com/simonw/strip-tags
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/strip-tags/issues
 Project-URL: CI, https://github.com/simonw/strip-tags/actions
 Project-URL: Changelog, https://github.com/simonw/strip-tags/releases
@@ -119,17 +119,23 @@
 <div>
 <h1>This has tags</h1>
 
 <p>And whitespace too</p>
 </div>
 Ignore this bit.
 """
-stripped = strip_tags(html, ["div"], minify=True)
+stripped = strip_tags(html, ["div"], minify=True, keep_tags=["h1"])
 print(stripped)
 ```
+Output:
+```
+<h1>This has tags</h1>
+
+And whitespace too
+```
 
 ## Development
 
 To contribute to this tool, first checkout the code. Then create a new virtual environment:
 ```bash
 cd strip-tags
 python -m venv venv
```

### Comparing `strip-tags-0.4/tests/test_strip_tags.py` & `strip-tags-0.4.1/tests/test_strip_tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,21 @@
     (
         """
         <h2 class="c" id="i" onclick="f">h2 with class and id</h2><p>Done</p>
         """,
         ["-t", "h2", "-m", "--all-attrs"],
         '<h2 class="c" id="i" onclick="f">h2 with class and id</h2>Done',
     ),
+    (
+        """
+        <pre class="foop" onclick="bar">This\nis    code</pre>
+        """,
+        ["-t", "pre", "-m"],
+        '<pre class="foop">This\nis    code</pre>',
+    ),
     # Keep a[href] and img[alt] and meta[name][value] even if not asked for
     (
         """
         Link: <a href="url" class="c" onclick="strip">URL</a>
         Image: <img alt="ALT">
         Meta: <meta name="metaname" value="metavalue" blah="blah">
         <p>No p tag</p>
```


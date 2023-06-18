# Comparing `tmp/markmoji-1.1.tar.gz` & `tmp/markmoji-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markmoji-1.1.tar", last modified: Sat Feb 25 18:28:53 2023, max compression
+gzip compressed data, was "markmoji-1.2.tar", last modified: Sun Jun 18 18:02:42 2023, max compression
```

## Comparing `markmoji-1.1.tar` & `markmoji-1.2.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 18:28:53.067000 markmoji-1.1/
--rw-rw-rw-   0        0        0     2826 2023-02-25 18:28:53.060000 markmoji-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2023-02-14 18:17:49.000000 markmoji-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 18:28:52.978000 markmoji-1.1/markmoji/
--rw-rw-rw-   0        0        0       73 2023-02-14 15:57:58.000000 markmoji-1.1/markmoji/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-02-14 15:14:13.000000 markmoji-1.1/markmoji/authors.py
-drwxrwxrwx   0        0        0        0 2023-02-25 18:28:53.054000 markmoji-1.1/markmoji/handlers/
--rw-rw-rw-   0        0        0       44 2022-12-29 13:03:12.000000 markmoji-1.1/markmoji/handlers/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-01-12 22:30:52.000000 markmoji-1.1/markmoji/handlers/base.py
--rw-rw-rw-   0        0        0     9640 2023-02-25 12:21:03.000000 markmoji-1.1/markmoji/handlers/handlers.py
--rw-rw-rw-   0        0        0      192 2022-12-29 12:55:29.000000 markmoji-1.1/markmoji/handlers/map.py
--rw-rw-rw-   0        0        0     2948 2023-02-15 15:55:29.000000 markmoji-1.1/markmoji/markmoji.py
-drwxrwxrwx   0        0        0        0 2023-02-25 18:28:53.022000 markmoji-1.1/markmoji.egg-info/
--rw-rw-rw-   0        0        0     2826 2023-02-25 18:28:52.000000 markmoji-1.1/markmoji.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-02-25 18:28:52.000000 markmoji-1.1/markmoji.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 18:28:52.000000 markmoji-1.1/markmoji.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-02-25 18:28:52.000000 markmoji-1.1/markmoji.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 18:28:52.000000 markmoji-1.1/markmoji.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-16 17:03:55.000000 markmoji-1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1134 2023-02-25 18:28:53.065000 markmoji-1.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-14 15:16:33.000000 markmoji-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:02:42.503569 markmoji-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-18 18:02:42.503569 markmoji-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-18 18:02:40.000000 markmoji-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:02:42.503569 markmoji-1.2/markmoji/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-18 18:02:40.000000 markmoji-1.2/markmoji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-18 18:02:40.000000 markmoji-1.2/markmoji/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-18 18:02:40.000000 markmoji-1.2/markmoji/markmoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:02:42.503569 markmoji-1.2/markmoji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-18 18:02:42.000000 markmoji-1.2/markmoji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-18 18:02:42.000000 markmoji-1.2/markmoji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:02:42.000000 markmoji-1.2/markmoji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-18 18:02:42.000000 markmoji-1.2/markmoji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 18:02:42.000000 markmoji-1.2/markmoji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 18:02:40.000000 markmoji-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-18 18:02:42.503569 markmoji-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 18:02:40.000000 markmoji-1.2/setup.py
```

### Comparing `markmoji-1.1/PKG-INFO` & `markmoji-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,56 @@
-Metadata-Version: 2.1
-Name: markmoji
-Version: 1.1
-Summary: Extends the basic markdown syntax using an easy to understand and quickly readable emoji-based syntax.
-Home-page: https://TEParsons.github.io/Markmoji
-Author: Todd Parsons
-Author-email: todd.e.parsons@gmail.com
-Maintainer-email: todd.e.parsons@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/TEParsons/Markmoji/archive/refs/tags/v1.1.tar.gz
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: suggested
-
-Markmoji extends the [basic markdown syntax](https://www.markdownguide.org/basic-syntax/) using an easy to understand and quickly readable emoji-based syntax, allowing you to create custom HTML elements from just an emoji, a label and a URL.
-
-## Installing
-Markmoji is on PyPi! To install, just copy the following into a terminal:
-
-```
-pip install markmoji
-```
-
-[Click here](https://datatofish.com/install-package-python-using-pip/) for more instructions on what installing from pip means.
-
-# The Syntax
-Similar to how basic markdown indicates an image using an exclamation point before a link (`![name](url)`), markmoji syntax uses an emoji beore a link (`🐦[name](url)`), with the emoji dictating the type of HTML element created.
-
-# Python function
-To parse markmoji syntax, just use the function `markmoji.markmoji()` with your markdown text as the input. It will return the same text but with any markmoji syntax returned as HTML objects.
-
-# Integration with [`python-markdown`](https://python-markdown.github.io/)
-Included in the package are the necessary classes to use markmoji as an extension to `markdown.Markdown`. Here's an example of how you might do it:
-```
-import markmoji
-import markdown as md
-
-# Define some dummy content
-content = "🏐[label1](link1)\n🏐[label2](link2)/n🐦[label3](link3)"
-# Create markdown processor with markmoji
-processor = md.Markdown(extensions=[markmoji.Markmoji()])
-# Do actual markdown conversion
-content = processor.convert(content)
-```
-
-# Contributing
-This is all designed with open source contribution in mind! To add your own handlers, check out the file `handlers/handlers.py` to see the existing implementations and some instructions on how to add your own. It's not all that hard to do, I promise!
-
+Metadata-Version: 2.1
+Name: markmoji
+Version: 1.2
+Summary: Extends the basic markdown syntax using an easy to understand and quickly readable emoji-based syntax.
+Home-page: https://TEParsons.github.io/Markmoji
+Download-URL: https://github.com/TEParsons/Markmoji/archive/refs/tags/v1.2.tar.gz
+Author: Todd Parsons
+Author-email: todd.e.parsons@gmail.com
+Maintainer-email: todd.e.parsons@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: suggested
+
+Markmoji extends the [basic markdown syntax](https://www.markdownguide.org/basic-syntax/) using an easy to understand and quickly readable emoji-based syntax, allowing you to create custom HTML elements from just an emoji, a label and a URL.
+
+## Installing
+Markmoji is on PyPi! To install, just copy the following into a terminal:
+
+```
+pip install markmoji
+```
+
+[Click here](https://datatofish.com/install-package-python-using-pip/) for more instructions on what installing from pip means.
+
+# The Syntax
+Similar to how basic markdown indicates an image using an exclamation point before a link (`![name](url)`), markmoji syntax uses an emoji beore a link (`🐦[name](url)`), with the emoji dictating the type of HTML element created.
+
+# Python function
+To parse markmoji syntax, just use the function `markmoji.markmoji()` with your markdown text as the input. It will return the same text but with any markmoji syntax returned as HTML objects.
+
+# Integration with [`python-markdown`](https://python-markdown.github.io/)
+Included in the package are the necessary classes to use markmoji as an extension to `markdown.Markdown`. Here's an example of how you might do it:
+```
+import markmoji
+import markdown as md
+
+# Define some dummy content
+content = "🏐[label1](link1)\n🏐[label2](link2)/n🐦[label3](link3)"
+# Create markdown processor with markmoji
+processor = md.Markdown(extensions=[markmoji.Markmoji()])
+# Do actual markdown conversion
+content = processor.convert(content)
+```
+
+# Contributing
+This is all designed with open source contribution in mind! To add your own handlers, check out the file `handlers/handlers.py` to see the existing implementations and some instructions on how to add your own. It's not all that hard to do, I promise!
```

### Comparing `markmoji-1.1/README.md` & `markmoji-1.2/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Markmoji extends the [basic markdown syntax](https://www.markdownguide.org/basic-syntax/) using an easy to understand and quickly readable emoji-based syntax, allowing you to create custom HTML elements from just an emoji, a label and a URL.
-
-## Installing
-Markmoji is on PyPi! To install, just copy the following into a terminal:
-
-```
-pip install markmoji
-```
-
-[Click here](https://datatofish.com/install-package-python-using-pip/) for more instructions on what installing from pip means.
-
-# The Syntax
-Similar to how basic markdown indicates an image using an exclamation point before a link (`![name](url)`), markmoji syntax uses an emoji beore a link (`🐦[name](url)`), with the emoji dictating the type of HTML element created.
-
-# Python function
-To parse markmoji syntax, just use the function `markmoji.markmoji()` with your markdown text as the input. It will return the same text but with any markmoji syntax returned as HTML objects.
-
-# Integration with [`python-markdown`](https://python-markdown.github.io/)
-Included in the package are the necessary classes to use markmoji as an extension to `markdown.Markdown`. Here's an example of how you might do it:
-```
-import markmoji
-import markdown as md
-
-# Define some dummy content
-content = "🏐[label1](link1)\n🏐[label2](link2)/n🐦[label3](link3)"
-# Create markdown processor with markmoji
-processor = md.Markdown(extensions=[markmoji.Markmoji()])
-# Do actual markdown conversion
-content = processor.convert(content)
-```
-
-# Contributing
+Markmoji extends the [basic markdown syntax](https://www.markdownguide.org/basic-syntax/) using an easy to understand and quickly readable emoji-based syntax, allowing you to create custom HTML elements from just an emoji, a label and a URL.
+
+## Installing
+Markmoji is on PyPi! To install, just copy the following into a terminal:
+
+```
+pip install markmoji
+```
+
+[Click here](https://datatofish.com/install-package-python-using-pip/) for more instructions on what installing from pip means.
+
+# The Syntax
+Similar to how basic markdown indicates an image using an exclamation point before a link (`![name](url)`), markmoji syntax uses an emoji beore a link (`🐦[name](url)`), with the emoji dictating the type of HTML element created.
+
+# Python function
+To parse markmoji syntax, just use the function `markmoji.markmoji()` with your markdown text as the input. It will return the same text but with any markmoji syntax returned as HTML objects.
+
+# Integration with [`python-markdown`](https://python-markdown.github.io/)
+Included in the package are the necessary classes to use markmoji as an extension to `markdown.Markdown`. Here's an example of how you might do it:
+```
+import markmoji
+import markdown as md
+
+# Define some dummy content
+content = "🏐[label1](link1)\n🏐[label2](link2)/n🐦[label3](link3)"
+# Create markdown processor with markmoji
+processor = md.Markdown(extensions=[markmoji.Markmoji()])
+# Do actual markdown conversion
+content = processor.convert(content)
+```
+
+# Contributing
 This is all designed with open source contribution in mind! To add your own handlers, check out the file `handlers/handlers.py` to see the existing implementations and some instructions on how to add your own. It's not all that hard to do, I promise!
```

### Comparing `markmoji-1.1/markmoji/authors.py` & `markmoji-1.2/markmoji/authors.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-try:
-    from pybtex.database import Person
-except ImportError:
-    class Person:
-        """
-        If Pybtex isn't installed, use this placeholder object which has enough attributes that 
-        markmoji doesn't break.
-        """
-        def __init__(self, string='', first='', middle='', prelast='', last='', lineage=''):
-            self.first_names = [first]
-            self.middle_names = [middle] + [prelast]
-            self.last_names = [last]
-            self.lineage = lineage
-
-# Emojis representing authors, pick something fun!
-authors = {
-    "🦊": Person(first="Todd", middle="Ethan", last="Parsons"),
-}
-
-def getCreditText():
-    from .handlers.map import map
-
-    # Array to store accreditations in
-    refs = {}
-    for handler in map.values():
-        # Get author object
-        author = handler.__author__
-        # Add author to accreditations list if not already present
-        if author not in refs:
-            refs[author] = " "
-        # Add credit
-        refs[author] += handler.emoji + " "
-    # Write preface
-    txt = (
-        "Markmoji by Todd Parsons.\n"
-        "\n"
-        "Handlers by:\n"
-    )
-    # Add credit for each handler
-    for author, credit in refs.items():
-        author = authors.get(author, authors["🦊"])
-        # Format name
-        name = f"{author.first_names[0]} {author.last_names[0]}"
-        # Construct line
-        line = f"{name} ({credit})\n"
-        # Append
-        txt += line
-    
-    return txt
+try:
+    from pybtex.database import Person
+except ImportError:
+    class Person:
+        """
+        If Pybtex isn't installed, use this placeholder object which has enough attributes that 
+        markmoji doesn't break.
+        """
+        def __init__(self, string='', first='', middle='', prelast='', last='', lineage=''):
+            self.first_names = [first]
+            self.middle_names = [middle] + [prelast]
+            self.last_names = [last]
+            self.lineage = lineage
+
+# Emojis representing authors, pick something fun!
+authors = {
+    "🦊": Person(first="Todd", middle="Ethan", last="Parsons"),
+}
+
+def getCreditText():
+    from .handlers.map import map
+
+    # Array to store accreditations in
+    refs = {}
+    for handler in map.values():
+        # Get author object
+        author = handler.__author__
+        # Add author to accreditations list if not already present
+        if author not in refs:
+            refs[author] = " "
+        # Add credit
+        refs[author] += handler.emoji + " "
+    # Write preface
+    txt = (
+        "Markmoji by Todd Parsons.\n"
+        "\n"
+        "Handlers by:\n"
+    )
+    # Add credit for each handler
+    for author, credit in refs.items():
+        author = authors.get(author, authors["🦊"])
+        # Format name
+        name = f"{author.first_names[0]} {author.last_names[0]}"
+        # Construct line
+        line = f"{name} ({credit})\n"
+        # Append
+        txt += line
+    
+    return txt
```

### Comparing `markmoji-1.1/markmoji.egg-info/PKG-INFO` & `markmoji-1.2/markmoji.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,56 @@
-Metadata-Version: 2.1
-Name: markmoji
-Version: 1.1
-Summary: Extends the basic markdown syntax using an easy to understand and quickly readable emoji-based syntax.
-Home-page: https://TEParsons.github.io/Markmoji
-Author: Todd Parsons
-Author-email: todd.e.parsons@gmail.com
-Maintainer-email: todd.e.parsons@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/TEParsons/Markmoji/archive/refs/tags/v1.1.tar.gz
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: suggested
-
-Markmoji extends the [basic markdown syntax](https://www.markdownguide.org/basic-syntax/) using an easy to understand and quickly readable emoji-based syntax, allowing you to create custom HTML elements from just an emoji, a label and a URL.
-
-## Installing
-Markmoji is on PyPi! To install, just copy the following into a terminal:
-
-```
-pip install markmoji
-```
-
-[Click here](https://datatofish.com/install-package-python-using-pip/) for more instructions on what installing from pip means.
-
-# The Syntax
-Similar to how basic markdown indicates an image using an exclamation point before a link (`![name](url)`), markmoji syntax uses an emoji beore a link (`🐦[name](url)`), with the emoji dictating the type of HTML element created.
-
-# Python function
-To parse markmoji syntax, just use the function `markmoji.markmoji()` with your markdown text as the input. It will return the same text but with any markmoji syntax returned as HTML objects.
-
-# Integration with [`python-markdown`](https://python-markdown.github.io/)
-Included in the package are the necessary classes to use markmoji as an extension to `markdown.Markdown`. Here's an example of how you might do it:
-```
-import markmoji
-import markdown as md
-
-# Define some dummy content
-content = "🏐[label1](link1)\n🏐[label2](link2)/n🐦[label3](link3)"
-# Create markdown processor with markmoji
-processor = md.Markdown(extensions=[markmoji.Markmoji()])
-# Do actual markdown conversion
-content = processor.convert(content)
-```
-
-# Contributing
-This is all designed with open source contribution in mind! To add your own handlers, check out the file `handlers/handlers.py` to see the existing implementations and some instructions on how to add your own. It's not all that hard to do, I promise!
-
+Metadata-Version: 2.1
+Name: markmoji
+Version: 1.2
+Summary: Extends the basic markdown syntax using an easy to understand and quickly readable emoji-based syntax.
+Home-page: https://TEParsons.github.io/Markmoji
+Download-URL: https://github.com/TEParsons/Markmoji/archive/refs/tags/v1.2.tar.gz
+Author: Todd Parsons
+Author-email: todd.e.parsons@gmail.com
+Maintainer-email: todd.e.parsons@gmail.com
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: suggested
+
+Markmoji extends the [basic markdown syntax](https://www.markdownguide.org/basic-syntax/) using an easy to understand and quickly readable emoji-based syntax, allowing you to create custom HTML elements from just an emoji, a label and a URL.
+
+## Installing
+Markmoji is on PyPi! To install, just copy the following into a terminal:
+
+```
+pip install markmoji
+```
+
+[Click here](https://datatofish.com/install-package-python-using-pip/) for more instructions on what installing from pip means.
+
+# The Syntax
+Similar to how basic markdown indicates an image using an exclamation point before a link (`![name](url)`), markmoji syntax uses an emoji beore a link (`🐦[name](url)`), with the emoji dictating the type of HTML element created.
+
+# Python function
+To parse markmoji syntax, just use the function `markmoji.markmoji()` with your markdown text as the input. It will return the same text but with any markmoji syntax returned as HTML objects.
+
+# Integration with [`python-markdown`](https://python-markdown.github.io/)
+Included in the package are the necessary classes to use markmoji as an extension to `markdown.Markdown`. Here's an example of how you might do it:
+```
+import markmoji
+import markdown as md
+
+# Define some dummy content
+content = "🏐[label1](link1)\n🏐[label2](link2)/n🐦[label3](link3)"
+# Create markdown processor with markmoji
+processor = md.Markdown(extensions=[markmoji.Markmoji()])
+# Do actual markdown conversion
+content = processor.convert(content)
+```
+
+# Contributing
+This is all designed with open source contribution in mind! To add your own handlers, check out the file `handlers/handlers.py` to see the existing implementations and some instructions on how to add your own. It's not all that hard to do, I promise!
```

### Comparing `markmoji-1.1/setup.cfg` & `markmoji-1.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,70 @@
-00000000: 5b62 6469 7374 5f77 6865 656c 5d0d 0a75  [bdist_wheel]..u
-00000010: 6e69 7665 7273 616c 203d 2031 0d0a 0d0a  niversal = 1....
-00000020: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000030: 203d 206d 6172 6b6d 6f6a 690d 0a76 6572   = markmoji..ver
-00000040: 7369 6f6e 203d 2031 2e31 0d0a 6c69 6365  sion = 1.1..lice
-00000050: 6e73 655f 6669 6c65 203d 204c 4943 454e  nse_file = LICEN
-00000060: 5345 0d0a 6175 7468 6f72 203d 2054 6f64  SE..author = Tod
-00000070: 6420 5061 7273 6f6e 730d 0a61 7574 686f  d Parsons..autho
-00000080: 725f 656d 6169 6c20 3d20 746f 6464 2e65  r_email = todd.e
-00000090: 2e70 6172 736f 6e73 4067 6d61 696c 2e63  .parsons@gmail.c
-000000a0: 6f6d 0d0a 6d61 696e 7461 696e 6572 5f65  om..maintainer_e
-000000b0: 6d61 696c 203d 2074 6f64 642e 652e 7061  mail = todd.e.pa
-000000c0: 7273 6f6e 7340 676d 6169 6c2e 636f 6d0d  rsons@gmail.com.
-000000d0: 0a75 726c 203d 2068 7474 7073 3a2f 2f54  .url = https://T
-000000e0: 4550 6172 736f 6e73 2e67 6974 6875 622e  EParsons.github.
-000000f0: 696f 2f4d 6172 6b6d 6f6a 690d 0a64 6f77  io/Markmoji..dow
-00000100: 6e6c 6f61 645f 7572 6c20 3d20 6874 7470  nload_url = http
-00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-00000120: 4550 6172 736f 6e73 2f4d 6172 6b6d 6f6a  EParsons/Markmoj
-00000130: 692f 6172 6368 6976 652f 7265 6673 2f74  i/archive/refs/t
-00000140: 6167 732f 7631 2e31 2e74 6172 2e67 7a0d  ags/v1.1.tar.gz.
-00000150: 0a64 6573 6372 6970 7469 6f6e 203d 2045  .description = E
-00000160: 7874 656e 6473 2074 6865 2062 6173 6963  xtends the basic
-00000170: 206d 6172 6b64 6f77 6e20 7379 6e74 6178   markdown syntax
-00000180: 2075 7369 6e67 2061 6e20 6561 7379 2074   using an easy t
-00000190: 6f20 756e 6465 7273 7461 6e64 2061 6e64  o understand and
-000001a0: 2071 7569 636b 6c79 2072 6561 6461 626c   quickly readabl
-000001b0: 6520 656d 6f6a 692d 6261 7365 6420 7379  e emoji-based sy
-000001c0: 6e74 6178 2e0d 0a6c 6f6e 675f 6465 7363  ntax...long_desc
-000001d0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-000001e0: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-000001f0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-00000200: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-00000210: 6d61 726b 646f 776e 0d0a 636c 6173 7369  markdown..classi
-00000220: 6669 6572 7320 3d20 0d0a 0944 6576 656c  fiers = ...Devel
-00000230: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000240: 2034 202d 2042 6574 610d 0a09 4f70 6572   4 - Beta...Oper
-00000250: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000260: 4d61 634f 5320 3a3a 204d 6163 4f53 2058  MacOS :: MacOS X
-00000270: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000280: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
-00000290: 203a 3a20 5769 6e64 6f77 730d 0a09 4f70   :: Windows...Op
-000002a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000002b0: 3a20 504f 5349 5820 3a3a 204c 696e 7578  : POSIX :: Linux
-000002c0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002e0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
-000002f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000300: 2050 7974 686f 6e20 3a3a 2033 2e36 0d0a   Python :: 3.6..
-00000310: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000320: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000330: 3a3a 2033 2e37 0d0a 0950 726f 6772 616d  :: 3.7...Program
-00000340: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000350: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
-00000360: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000370: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000380: 3a3a 2033 2e39 0d0a 0950 726f 6772 616d  :: 3.9...Program
-00000390: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000003a0: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
-000003b0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7079  ...[options]..py
-000003c0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-000003d0: 3e3d 332e 360d 0a69 6e73 7461 6c6c 5f72  >=3.6..install_r
-000003e0: 6571 7569 7265 7320 3d20 0d0a 096d 6172  equires = ...mar
-000003f0: 6b64 6f77 6e0d 0a09 7265 7175 6573 7473  kdown...requests
-00000400: 0d0a 0976 616c 6964 6174 6f72 730d 0a0d  ...validators...
-00000410: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
-00000420: 5f72 6571 7569 7265 5d0d 0a73 7567 6765  _require]..sugge
-00000430: 7374 6564 203d 200d 0a09 7079 6274 6578  sted = ...pybtex
-00000440: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000450: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000460: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000000: 5b62 6469 7374 5f77 6865 656c 5d0a 756e  [bdist_wheel].un
+00000010: 6976 6572 7361 6c20 3d20 310a 0a5b 6d65  iversal = 1..[me
+00000020: 7461 6461 7461 5d0a 6e61 6d65 203d 206d  tadata].name = m
+00000030: 6172 6b6d 6f6a 690a 7665 7273 696f 6e20  arkmoji.version 
+00000040: 3d20 312e 320a 6c69 6365 6e73 655f 6669  = 1.2.license_fi
+00000050: 6c65 203d 204c 4943 454e 5345 0a61 7574  le = LICENSE.aut
+00000060: 686f 7220 3d20 546f 6464 2050 6172 736f  hor = Todd Parso
+00000070: 6e73 0a61 7574 686f 725f 656d 6169 6c20  ns.author_email 
+00000080: 3d20 746f 6464 2e65 2e70 6172 736f 6e73  = todd.e.parsons
+00000090: 4067 6d61 696c 2e63 6f6d 0a6d 6169 6e74  @gmail.com.maint
+000000a0: 6169 6e65 725f 656d 6169 6c20 3d20 746f  ainer_email = to
+000000b0: 6464 2e65 2e70 6172 736f 6e73 4067 6d61  dd.e.parsons@gma
+000000c0: 696c 2e63 6f6d 0a75 726c 203d 2068 7474  il.com.url = htt
+000000d0: 7073 3a2f 2f54 4550 6172 736f 6e73 2e67  ps://TEParsons.g
+000000e0: 6974 6875 622e 696f 2f4d 6172 6b6d 6f6a  ithub.io/Markmoj
+000000f0: 690a 646f 776e 6c6f 6164 5f75 726c 203d  i.download_url =
+00000100: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000110: 636f 6d2f 5445 5061 7273 6f6e 732f 4d61  com/TEParsons/Ma
+00000120: 726b 6d6f 6a69 2f61 7263 6869 7665 2f72  rkmoji/archive/r
+00000130: 6566 732f 7461 6773 2f76 312e 322e 7461  efs/tags/v1.2.ta
+00000140: 722e 677a 0a64 6573 6372 6970 7469 6f6e  r.gz.description
+00000150: 203d 2045 7874 656e 6473 2074 6865 2062   = Extends the b
+00000160: 6173 6963 206d 6172 6b64 6f77 6e20 7379  asic markdown sy
+00000170: 6e74 6178 2075 7369 6e67 2061 6e20 6561  ntax using an ea
+00000180: 7379 2074 6f20 756e 6465 7273 7461 6e64  sy to understand
+00000190: 2061 6e64 2071 7569 636b 6c79 2072 6561   and quickly rea
+000001a0: 6461 626c 6520 656d 6f6a 692d 6261 7365  dable emoji-base
+000001b0: 6420 7379 6e74 6178 2e0a 6c6f 6e67 5f64  d syntax..long_d
+000001c0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000001d0: 653a 2052 4541 444d 452e 6d64 0a6c 6f6e  e: README.md.lon
+000001e0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000001f0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+00000200: 742f 6d61 726b 646f 776e 0a63 6c61 7373  t/markdown.class
+00000210: 6966 6965 7273 203d 200a 0944 6576 656c  ifiers = ..Devel
+00000220: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000230: 2034 202d 2042 6574 610a 094f 7065 7261   4 - Beta..Opera
+00000240: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
+00000250: 6163 4f53 203a 3a20 4d61 634f 5320 580a  acOS :: MacOS X.
+00000260: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000270: 6d20 3a3a 204d 6963 726f 736f 6674 203a  m :: Microsoft :
+00000280: 3a20 5769 6e64 6f77 730a 094f 7065 7261  : Windows..Opera
+00000290: 7469 6e67 2053 7973 7465 6d20 3a3a 2050  ting System :: P
+000002a0: 4f53 4958 203a 3a20 4c69 6e75 780a 0950  OSIX :: Linux..P
+000002b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002d0: 2033 0a09 5072 6f67 7261 6d6d 696e 6720   3..Programming 
+000002e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002f0: 6f6e 203a 3a20 332e 360a 0950 726f 6772  on :: 3.6..Progr
+00000300: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000310: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+00000320: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000330: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000340: 203a 3a20 332e 380a 0950 726f 6772 616d   :: 3.8..Program
+00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000360: 2050 7974 686f 6e20 3a3a 2033 2e39 0a09   Python :: 3.9..
+00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000390: 3a20 332e 3130 0a0a 5b6f 7074 696f 6e73  : 3.10..[options
+000003a0: 5d0a 7079 7468 6f6e 5f72 6571 7569 7265  ].python_require
+000003b0: 7320 3d20 3e3d 332e 360a 696e 7374 616c  s = >=3.6.instal
+000003c0: 6c5f 7265 7175 6972 6573 203d 200a 096d  l_requires = ..m
+000003d0: 6172 6b64 6f77 6e0a 0965 6d6f 6a69 0a09  arkdown..emoji..
+000003e0: 7265 7175 6573 7473 0a09 7661 6c69 6461  requests..valida
+000003f0: 746f 7273 0a09 656d 6f6a 690a 0a5b 6f70  tors..emoji..[op
+00000400: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+00000410: 7569 7265 5d0a 7375 6767 6573 7465 6420  uire].suggested 
+00000420: 3d20 0a09 7079 6274 6578 0a0a 5b65 6767  = ..pybtex..[egg
+00000430: 5f69 6e66 6f5d 0a74 6167 5f62 7569 6c64  _info].tag_build
+00000440: 203d 200a 7461 675f 6461 7465 203d 2030   = .tag_date = 0
+00000450: 0a0a                                     ..
```


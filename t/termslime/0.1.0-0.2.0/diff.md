# Comparing `tmp/termslime-0.1.0.tar.gz` & `tmp/termslime-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termslime-0.1.0.tar", max compression
+gzip compressed data, was "termslime-0.2.0.tar", max compression
```

## Comparing `termslime-0.1.0.tar` & `termslime-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-06-18 08:41:45.640249 termslime-0.1.0/LICENSE
--rw-r--r--   0        0        0      442 2023-06-18 09:04:54.067914 termslime-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-18 08:39:50.888877 termslime-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-18 08:39:50.888877 termslime-0.1.0/termslime/__init__.py
--rw-r--r--   0        0        0     5269 2023-06-18 09:02:54.963980 termslime-0.1.0/termslime/main.py
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 termslime-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-18 08:41:45.640249 termslime-0.2.0/LICENSE
+-rw-r--r--   0        0        0      715 2023-06-18 10:59:12.900708 termslime-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-18 08:39:50.888877 termslime-0.2.0/README.md
+-rw-r--r--   0        0        0       12 2023-06-18 09:15:03.198103 termslime-0.2.0/termslime/.gitignore
+-rw-r--r--   0        0        0     5409 2023-06-18 10:57:33.410810 termslime-0.2.0/termslime/main.py
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 termslime-0.2.0/PKG-INFO
```

### Comparing `termslime-0.1.0/LICENSE` & `termslime-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termslime-0.1.0/termslime/main.py` & `termslime-0.2.0/termslime/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,21 +79,28 @@
     # print the end padding
     print("\n" * endPadding, end="")
 
 # the entry point of the cli
 def main():
 
     # set up the argument parser
-    parser = argparse.ArgumentParser(prog="termslime", description="Display an image in your terminal with true colors.")
+    parser = argparse.ArgumentParser(
+        prog="tslime",
+        description="Termslime displays images in your terminal with true colors. Project home page: https://github.com/garyzbm/termslime",
+    )
+
+    # add arguments
     parser.add_argument("path", type=str, help="path to an image file or a directory containing image files")
     parser.add_argument("-hl", "--heightLimit", type=int, default=500, help="maximum number of lines of blocks to display the image in the terminal")
     parser.add_argument("-wl", "--widthLimit", type=int, default=1000, help="maximum number of blocks per line to display the image in the terminal")
     parser.add_argument("-bp", "--beginPadding", type=int, default=1, help="number of empty lines before the image")
     parser.add_argument("-ep", "--endPadding", type=int, default=0, help="number of empty lines after the image")
     parser.add_argument("-lp", "--leftPadding", type=int, default=1, help="number of empty spaces at the beginning of each line of the image")
+
+    # parse the arguments
     args = parser.parse_args()
 
     # get path from the arguments
     imgPath = args.path
     assert os.path.exists(imgPath), f"{imgPath} does not exist"
 
     # if imgPath is a path to a directory
```

### Comparing `termslime-0.1.0/PKG-INFO` & `termslime-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 Metadata-Version: 2.1
 Name: termslime
-Version: 0.1.0
+Version: 0.2.0
 Summary: Termslime displays images in your terminal with true colors.
+Home-page: https://github.com/garyzbm/termslime
+License: MIT
+Keywords: cli,image,terminal
 Author: Gary Zhang
 Author-email: garyzhang2002@hotmail.com
+Maintainer: Gary Zhang
+Maintainer-email: garyzhang2002@hotmail.com
 Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorful (>=0.5.5,<0.6.0)
 Requires-Dist: pillow (>=9.2.0,<10.0.0)
+Project-URL: Documentation, https://github.com/garyzbm/termslime
+Project-URL: Repository, https://github.com/garyzbm/termslime
 Description-Content-Type: text/markdown
```


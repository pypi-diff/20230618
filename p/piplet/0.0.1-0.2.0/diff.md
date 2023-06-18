# Comparing `tmp/piplet-0.0.1.tar.gz` & `tmp/piplet-0.2.0.tar.gz`

## Comparing `piplet-0.0.1.tar` & `piplet-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 piplet-0.0.1/piplet/__init__.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 piplet-0.0.1/.gitignore
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 piplet-0.0.1/LICENSE
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 piplet-0.0.1/README.md
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 piplet-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 piplet-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 piplet-0.2.0/piplet/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 piplet-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 piplet-0.2.0/LICENSE
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 piplet-0.2.0/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 piplet-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 piplet-0.2.0/PKG-INFO
```

### Comparing `piplet-0.0.1/piplet/__init__.py` & `piplet-0.2.0/piplet/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+import argparse
+
+from sys import stdlib_module_names
+
 from typing import Iterator, Dict, List, Union
+
 from colorama import Fore
 
 # imports for get_packges()
 from pip._internal.commands.show import search_packages_info
 from pkg_resources import working_set
 
 
@@ -44,19 +49,47 @@
                 )
             else:
                 print(
                     f"{Fore.BLUE}{package['name']}={package['version']}{Fore.RESET}",
                 )
 
 
-def main() -> None:
+def _list_stdlib():
+    """lists packages from the python standard library"""
+    modules = sorted(filter(str.isalpha, stdlib_module_names))
+
+    for i in modules:
+        print(i)
+
+def _list():
     packages = get_packages()
     try:
         from pip._internal.commands.show import _PackageInfo
     except ImportError:
         show_dependency_tree21(packages)
     else:
         show_dependency_tree(packages)
 
+def main():
+    parser = argparse.ArgumentParser(
+        prog = "piplet",
+        description = "for doing what pip can't yet do"
+    )
+
+    parser.add_argument(
+        "command",
+        choices=["list"]
+    )
+    parser.add_argument("--stdlib", action="store_true")
+
+    args = parser.parse_args()
+
+    if args.command == "list":
+        if args.stdlib is True:
+            _list_stdlib()
+        else:
+            _list()
+
 if __name__ == "__main__":
     main()
 
+
```

### Comparing `piplet-0.0.1/LICENSE` & `piplet-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piplet-0.0.1/pyproject.toml` & `piplet-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "piplet"
-version = "0.0.1"
+version = "0.2.0"
 description = "for doing what pip can't yet do"
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
 authors = [
     { name = "berkay-yalin", email = "66202981+berkay-yalin@users.noreply.github.com" },
 ]
```

### Comparing `piplet-0.0.1/PKG-INFO` & `piplet-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piplet
-Version: 0.0.1
+Version: 0.2.0
 Summary: for doing what pip can't yet do
 Project-URL: Documentation, https://github.com/berkay-yalin/omnicron#readme
 Project-URL: Issues, https://github.com/berkay-yalin/omnicron/issues
 Project-URL: Source, https://github.com/berkay-yalin/omnicron
 Author-email: berkay-yalin <66202981+berkay-yalin@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
```


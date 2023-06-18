# Comparing `tmp/cabinet-2023.6.17.3.tar.gz` & `tmp/cabinet-2023.6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.6.17.3.tar", last modified: Sun Jun 18 03:57:07 2023, max compression
+gzip compressed data, was "cabinet-2023.6.8.1.tar", last modified: Fri Jun  9 04:30:15 2023, max compression
```

## Comparing `cabinet-2023.6.17.3.tar` & `cabinet-2023.6.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-18 03:57:07.236868 cabinet-2023.6.17.3/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1090 2023-06-17 20:33:55.000000 cabinet-2023.6.17.3/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6583 2023-06-18 03:57:07.236868 cabinet-2023.6.17.3/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6231 2023-06-10 19:53:03.000000 cabinet-2023.6.17.3/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.6.17.3/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-06-18 03:57:07.236868 cabinet-2023.6.17.3/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-18 03:57:07.236868 cabinet-2023.6.17.3/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-18 03:57:07.236868 cabinet-2023.6.17.3/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-09 04:30:03.000000 cabinet-2023.6.17.3/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.6.17.3/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    27851 2023-06-18 03:56:56.000000 cabinet-2023.6.17.3/src/cabinet/cabinet.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.6.17.3/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-18 03:57:07.236868 cabinet-2023.6.17.3/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6583 2023-06-18 03:57:07.000000 cabinet-2023.6.17.3/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-06-18 03:57:07.000000 cabinet-2023.6.17.3/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-18 03:57:07.000000 cabinet-2023.6.17.3/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-06-18 03:57:07.000000 cabinet-2023.6.17.3/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-06-18 03:57:07.000000 cabinet-2023.6.17.3/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-18 03:57:07.236868 cabinet-2023.6.17.3/test/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.6.17.3/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.6.8.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.6.8.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-09 04:30:03.000000 cabinet-2023.6.8.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.6.8.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    26147 2023-06-09 04:29:47.000000 cabinet-2023.6.8.1/src/cabinet/cabinet.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.6.8.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/test/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/test/test___init__.py
```

### Comparing `cabinet-2023.6.17.3/PKG-INFO` & `cabinet-2023.6.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.6.17.3
+Version: 2023.6.8.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -237,19 +237,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.17.3/README.md` & `cabinet-2023.6.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -225,19 +225,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.17.3/setup.cfg` & `cabinet-2023.6.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.06.17.3
+version = 2023.06.08.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2023.6.17.3/src/cabinet/cabinet.py` & `cabinet-2023.6.8.1/src/cabinet/cabinet.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 """
 
 import os
 import json
 import pathlib
 import logging
 import sys
-import ast
 import argparse
 from datetime import date
 from typing import Optional
 import importlib.metadata
 from .mail import Mail
 
 
@@ -304,29 +303,18 @@
         file_handler.setFormatter(log_format)
 
         logger.addHandler(file_handler)
         return logger
 
     def _ifprint(self, message: str, is_print: bool):
         """
-        Prints the message if `print` is true.
+        Prints a string if `print` is true.
         """
-
-        # check for valid JSON
-        try:
-            json.loads(message)
-            if is_print:
-                print(json.dumps(message, indent=2))
-        except TypeError:
-            if is_print:
-                print(json.dumps(message, indent=2))
-        except json.JSONDecodeError:
-            if is_print:
-                print(message)
-            return message
+        if is_print:
+            print(message)
 
     def configure(self):
         """
         Configures the Cabinet instance based on command line arguments or user input.
         """
 
         message = f"""
@@ -456,76 +444,54 @@
                 File must be in the `path_cabinet` folder.
                 Default: 'settings.json'
 
         Returns:
             The value that was put into the property.
         """
 
-        def parse_arg(value):
-            """
-            Infer the value type (e.g. 2 will not be parsed as a string)
-            """
-            if value == "null":
-                return None
-            try:
-                return int(value)
-            except ValueError:
-                try:
-                    return float(value)
-                except ValueError:
-                    if value.lower() == 'true':
-                        return True
-                    if value.lower() == 'false':
-                        return False
-                    try:
-                        return ast.literal_eval(value)
-                    except (SyntaxError, ValueError):
-                        return value
-
         path_full = f"{self.path_cabinet}/{file_name}"
 
         maximum_attribute_index = 0
         attribute_max_attribute_index = attribute
 
         if not value:
-            value = parse_arg(attribute[-1])
+            value = attribute[-1]
             maximum_attribute_index = -1
             attribute_max_attribute_index = attribute[:maximum_attribute_index]
 
         _settings = self.settings_json if file_name == 'settings.json' else json.load(
             open(path_full, encoding="utf8"))
 
+        # iterate through entire JSON object and replace 2nd to last attribute with value
+
         partition = _settings
 
         for index, item in enumerate(attribute_max_attribute_index):
             if item not in partition:
                 try:
                     partition[item] = value if index == len(
                         attribute) + maximum_attribute_index - 1 else {}
                     partition = partition[item]
                     self.log(
-                        f"Adding key: {{'{item}': {partition}}} \
-to \"{attribute_max_attribute_index[index-1] if index > 0 else path_full}\"",
+                        f"Adding new key '{item}' to {partition if index > 0 else path_full}",
                         is_quiet=self.new_setup)
                 except TypeError as error:
                     self.log(f"{error}\n\n{attribute[index-1]} is currently a string, so it cannot \
 be treated as an object with multiple properties.", level="error")
             else:
                 if index == len(attribute) + maximum_attribute_index - 1:
                     partition[item] = value
                 else:
                     partition = partition[item]
 
         with open(path_full, 'w+', encoding="utf8") as file:
             json.dump(_settings, file, indent=4)
 
-        self.log(
-            f"{' -> '.join(attribute[:-1])} set to {value}",
-            level='info', is_quiet=not is_print)
-
+        self._ifprint(
+            f"{' -> '.join(attribute[:-1])} set to {value}", is_print)
         return value
 
     def get_file_as_array(self, item: str, file_path=None, strip: bool = True,
                           ignore_not_found: bool = False):
         """
         Reads a file and returns its contents as a list of lines.
         The file is assumed to be encoded in UTF-8.
@@ -659,43 +625,29 @@
         cabinet edit <file path/name, optional; default: settings.json>
     """
 
     cab = Cabinet()
     package_name = sys.modules[__name__].__package__.split('.')[0]
     version = importlib.metadata.version(package_name)
 
-    class ValidatePutArgs(argparse.Action):
-        """
-        Custom argparse action to validate the number of arguments for the --put option.
-        Ensures that a minimum of 2 arguments are provided.
-        """
-
-        def __call__(self, parser, namespace, values, option_string=None):
-            if len(values) < 2:
-                if len(values) == 1 and values[0] == 'ut':
-                    print("I think you meant to use '--put' or '-p'.\n")
-                parser.error(
-                    f"At least 2 arguments are required for {option_string}")
-            setattr(namespace, self.dest, values)
-
     parser = argparse.ArgumentParser(
         description=f"Cabinet ({version})")
 
     parser.add_argument('--configure', '-config', dest='configure',
                         action='store_true', help='Configure')
     parser.add_argument('--edit', '-e', dest='edit', action='store_true',
                         help='Edit the settings.json file')
     parser.add_argument('--edit-file', '-ef', type=str, dest='edit_file',
                         help='Edit a specific file')
     parser.add_argument('--no-create', dest='create',
                         action='store_false',
                         help='(for -ef) Do not create file if it does not exist')
     parser.add_argument('--get', '-g', dest='get', nargs='+',
                         help='Get a property from settings.json')
-    parser.add_argument('--put', '-p', dest='put', nargs='+', action=ValidatePutArgs,
+    parser.add_argument('--put', '-p', dest='put', nargs='+',
                         help='Put a property into settings.json')
     parser.add_argument('--get-file', dest='get_file',
                         type=str, help='Get file')
     parser.add_argument('--strip', dest='strip', action='store_false',
                         help='(for --get-file) Whether to strip file content whitespace')
     parser.add_argument('--log', '-l', type=str,
                         dest='log', help='Log a message to the default location')
```

### Comparing `cabinet-2023.6.17.3/src/cabinet/mail.py` & `cabinet-2023.6.8.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.6.17.3/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.6.17.3
+Version: 2023.6.8.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -237,19 +237,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.17.3/test/test___init__.py` & `cabinet-2023.6.8.1/test/test___init__.py`

 * *Files identical despite different names*


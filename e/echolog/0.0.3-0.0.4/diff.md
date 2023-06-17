# Comparing `tmp/echolog-0.0.3.tar.gz` & `tmp/echolog-0.0.4.tar.gz`

## Comparing `echolog-0.0.3.tar` & `echolog-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 echolog-0.0.3/src/echolog/__init__.py
--rw-r--r--   0        0        0    11837 2020-02-02 00:00:00.000000 echolog-0.0.3/src/echolog/echolog.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 echolog-0.0.3/LICENSE
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 echolog-0.0.3/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 echolog-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 echolog-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 echolog-0.0.4/src/echolog/__init__.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 echolog-0.0.4/src/echolog/demo.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 echolog-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 echolog-0.0.4/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 echolog-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 echolog-0.0.4/PKG-INFO
```

### Comparing `echolog-0.0.3/src/echolog/echolog.py` & `echolog-0.0.4/src/echolog/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -294,43 +294,14 @@
         logging.log(levelNum, message, *args, **kwargs)
 
     logging.addLevelName(levelNum, levelName)
     setattr(logging, levelName, levelNum)
     setattr(logging.getLoggerClass(), methodName, logForLevel)
     setattr(logging, methodName, logToRoot)
 
-
-if __name__ == "__main__":
-    
-    # runs a short demo if this file is called directly
-    
-    newline(3)
-    
-    for fmt in ['short-time', 'short', 'long-time', 'long']:
-        log = get_logger(level=logging.DEBUG, fmt=fmt)
-
-        echo(       f"Demo echo() call with   fmt={fmt}")
-        log.debug(  f'Demo debug message with fmt = {fmt}.')
-        log.debug(  f'Demo debug message with fmt = {fmt}.')
-        log.echo(   f'Demo echo message with  fmt = {fmt}.')
-        log.info(   f'Demo info message with  fmt = {fmt}.')
-        log.warning(f'Demo warn message with  fmt = {fmt}.')
-        log.error(  f'Demo error message with fmt = {fmt}.')
-        log.fatal(  f'Demo fatal message with fmt = {fmt}.')
-    
-        newline()
-    
-    a = 2
-    b = [3, 4]
-
-    echo('Example call to echo() with multiple arguments.', a, blah=b)
-    newline()
-
-
-
 # def dprint(*args):
 #     # Old debug printing function.
 #     # Uses dark magic (?) to print both name and value of passed arguments.
 #     frame = inspect.currentframe().f_back
 #     s = inspect.getframeinfo(frame).code_context[0]
 #     r = re.search(r"\((.*)\)", s).group(1)
 #     vnames = r.split(", ")
```

### Comparing `echolog-0.0.3/LICENSE` & `echolog-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `echolog-0.0.3/README.md` & `echolog-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,20 @@
 
     Adding 'bg_' to the start of any of these will get the background ANSI color.
     
     Finally, 'reset' contains the ANSI code to reset to default formatting.
 
 ## Example usage
 
-Running the main `echolog.py` project file directly the following test case:
+Running `demo.py` executes the following test case:
 
 ``` python
+    import logging
+    from echolog import echo, get_logger, newline
+    
     newline(3)
     
     for fmt in ['short-time', 'short', 'long-time', 'long']:
         log = get_logger(level=logging.DEBUG, fmt=fmt)
 
         echo(       f"Demo echo() call with   fmt={fmt}")
         log.debug(  f'Demo debug message with fmt = {fmt}.')
```

### Comparing `echolog-0.0.3/pyproject.toml` & `echolog-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "echolog"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="nerdpersonthing" },
 ]
 description = "A logging package that adds an echo() function to return both the input expression/variable and its results. Also sets up nicely-formatted logging."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `echolog-0.0.3/PKG-INFO` & `echolog-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolog
-Version: 0.0.3
+Version: 0.0.4
 Summary: A logging package that adds an echo() function to return both the input expression/variable and its results. Also sets up nicely-formatted logging.
 Project-URL: Homepage, https://github.com/nerdpersonthing/echolog
 Author: nerdpersonthing
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -72,17 +72,20 @@
 
     Adding 'bg_' to the start of any of these will get the background ANSI color.
     
     Finally, 'reset' contains the ANSI code to reset to default formatting.
 
 ## Example usage
 
-Running the main `echolog.py` project file directly the following test case:
+Running `demo.py` executes the following test case:
 
 ``` python
+    import logging
+    from echolog import echo, get_logger, newline
+    
     newline(3)
     
     for fmt in ['short-time', 'short', 'long-time', 'long']:
         log = get_logger(level=logging.DEBUG, fmt=fmt)
 
         echo(       f"Demo echo() call with   fmt={fmt}")
         log.debug(  f'Demo debug message with fmt = {fmt}.')
```


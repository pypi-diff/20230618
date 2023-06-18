# Comparing `tmp/consoleprint-1.3.6.tar.gz` & `tmp/consoleprint-1.3.9.tar.gz`

## Comparing `consoleprint-1.3.6.tar` & `consoleprint-1.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 consoleprint-1.3.6/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 consoleprint-1.3.6/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 consoleprint-1.3.6/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.6/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 consoleprint-1.3.6/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.6/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.6/LICENSE
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 consoleprint-1.3.6/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 consoleprint-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 consoleprint-1.3.9/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 consoleprint-1.3.9/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 consoleprint-1.3.9/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.3.9/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 consoleprint-1.3.9/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.3.9/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.3.9/LICENSE
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 consoleprint-1.3.9/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 consoleprint-1.3.9/PKG-INFO
```

### Comparing `consoleprint-1.3.6/src/ConsolePrint/animate.py` & `consoleprint-1.3.9/src/ConsolePrint/animate.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.6/src/ConsolePrint/console2file.py` & `consoleprint-1.3.9/src/ConsolePrint/console2file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 """This module  saves terminal output to file."""
 import sys
 import subprocess
 import time
 
 
-def __saving(t, text='Saving...', confirm=False):
+def __saving(t, text='Writing to file...', confirm=False):
     "Takes two arguments, time and text to display such as 'loading...'"
     load = ['-', '\\', '|', '/', '-'] * t
     print()
     for _ in load:
         print(f"  {_}  {text}", end='\r')
         time.sleep(0.4)
     if confirm:
-        print('Saved!!!         ')
+        print('Complete!!!             ')
 
-def startConsoleSave():
+def startConsoleSave(name:str=''):
     """Starts the process to save the output to file"""
     global filename
-    filename = input("\nEnter the output filename and extension:\n>>  ") # specified filename/path      
+    if name:
+        filename = name
+    else:
+        filename = 'terminal_output.txt'    
     sys.stdout = open(filename, 'a')  # redirects output to specified file
 
 
-def endConsoleSave():  
+def endConsoleSave(prompt=True):  
     """Ends the save to file process and returns output to console"""  
     sys.stdout.close()
     sys.stdout = sys.__stdout__   # redirects output from file back to terminal
     __saving(1, confirm=True)
-    print(f"Output has been saved to {filename}")
-    open_file = input("\nWould you like to open the file? y/n: ")
-    if open_file.strip().lower() == "y":
-        try:
-            subprocess.Popen(["start", "", filename], shell=True)
-        except FileNotFoundError:
-            print("File not found.")
-        except OSError:
-            print("Error opening file.")
+    print(f"Output has been saved to \033[36m{filename}\033[0m")
+    if prompt:
+        open_file = input("\nWould you like to open the file? y/n: ")
+        if open_file.strip().lower() == "y":
+            try:
+                subprocess.Popen(["start", "", filename], shell=True)
+            except FileNotFoundError:
+                print("File not found.")
+            except OSError:
+                print("Error opening file.")
 
 
 if __name__ == "__main__":
     print("Running module test")
     import calendar
     
-    startConsoleSave()
+    startConsoleSave() # Saves file to default terminal_output.txt 
     
     print("Printing Calendar")
     print(calendar.calendar(2023))
     
     endConsoleSave()
```

### Comparing `consoleprint-1.3.6/src/ConsolePrint/loading.py` & `consoleprint-1.3.9/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.6/tests/tests.py` & `consoleprint-1.3.9/tests/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # Test codes.  Ensure you have installed the module first using: pip install ConsolePrint
 
 # animate.py
 import ConsolePrint.animate as prt
 
-prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
+prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='double_under')
 prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
 prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
 prt.animate1("This text is animated with #", symbol="#", format='blue')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
 prt.star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 
 # console2file.py
-# import ConsolePrint.console2file as file
-# import calendar
+import ConsolePrint.console2file as file
+import calendar
 
-# file.startConsoleSave()
+file.startConsoleSave("my_output.txt")
 
-# print("Printing Calendar")
-# print(calendar.calendar(2023))
+print("Printing Calendar")
+print(calendar.calendar(2023))
 
-# file.endConsoleSave()  
-
-# # loading.py
-# import ConsolePrint.loading as load
-
-# load.countdown(5)
-# print()
-# load.loading1(20)  
-# print()
-# load.loading2(5, 'thinking...')
-# print()
-# load.loading3(5)
+file.endConsoleSave()  
+
+# loading.py
+import ConsolePrint.loading as load
+
+load.countdown(5)
+print()
+load.loading1(20)  
+print()
+load.loading2(5, 'thinking...')
+print()
+load.loading3(5)
```

### Comparing `consoleprint-1.3.6/LICENSE` & `consoleprint-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.3.6/README.md` & `consoleprint-1.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 `pip install ConsolePrint`
 
 # Test Cases
 1.  This permits output of programs to be saved in a file.  Run your code between the start and end console save functions to save the output to file.
 ```python
 import ConsolePrint.console2file as file  
 
-file.startConsoleSave()
-# Saves all output between the start and end functions to file
+file.startConsoleSave(name="my_output.txt", prompt=False)
+# Saves all output between the start and end functions to filename argument
 from calendar import calendar
 print(calendar(2023))
 file.endConsoleSave()
 ```
 2.  This module permits differnt colourful print animations to be output to file.  The format argument takes an ANSI escape sequences as a string.  You may also modify other arguments as desired.<br>
 <b>Preset string values for the format argument</b>
 <table>
@@ -68,25 +68,25 @@
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
 prt.animate1("This text is animated with #", symbol="#", format='magenta')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 prt.text_box("boxed in", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 ```
 
-3.  This adds loading animations to terminal program.  The load time argument is specified as an integer in seconds.
+<!-- 3.  This adds loading animations to terminal program.  The load time argument is specified as an integer in seconds.
 ```python
 import ConsolePrint.loading as load  
 
 load.countdown(5)
 load.loading1(10)
 print()
 load.loading2(5)
 print()
 load.loading3(5)
-```
+``` -->
 ## License
 This project is given free for use and download under the MIT license.
 
 ## Project Status
 Still undergoing enhancements.
 
 ## How to Contribute
```

### Comparing `consoleprint-1.3.6/pyproject.toml` & `consoleprint-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.3.6"
+version = "1.3.9"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `consoleprint-1.3.6/PKG-INFO` & `consoleprint-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.3.6
+Version: 1.3.9
 Summary: A package to animate and beautify print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,16 +23,16 @@
 `pip install ConsolePrint`
 
 # Test Cases
 1.  This permits output of programs to be saved in a file.  Run your code between the start and end console save functions to save the output to file.
 ```python
 import ConsolePrint.console2file as file  
 
-file.startConsoleSave()
-# Saves all output between the start and end functions to file
+file.startConsoleSave(name="my_output.txt", prompt=False)
+# Saves all output between the start and end functions to filename argument
 from calendar import calendar
 print(calendar(2023))
 file.endConsoleSave()
 ```
 2.  This module permits differnt colourful print animations to be output to file.  The format argument takes an ANSI escape sequences as a string.  You may also modify other arguments as desired.<br>
 <b>Preset string values for the format argument</b>
 <table>
@@ -82,25 +82,25 @@
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
 prt.animate1("This text is animated with #", symbol="#", format='magenta')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 prt.text_box("boxed in", symbol="#", padding=True, wall=True, align='right', format='\033[48;5;4m')
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 ```
 
-3.  This adds loading animations to terminal program.  The load time argument is specified as an integer in seconds.
+<!-- 3.  This adds loading animations to terminal program.  The load time argument is specified as an integer in seconds.
 ```python
 import ConsolePrint.loading as load  
 
 load.countdown(5)
 load.loading1(10)
 print()
 load.loading2(5)
 print()
 load.loading3(5)
-```
+``` -->
 ## License
 This project is given free for use and download under the MIT license.
 
 ## Project Status
 Still undergoing enhancements.
 
 ## How to Contribute
```


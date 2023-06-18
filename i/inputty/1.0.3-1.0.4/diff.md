# Comparing `tmp/inputty-1.0.3.tar.gz` & `tmp/inputty-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inputty-1.0.3.tar", last modified: Tue Jun  6 16:52:30 2023, max compression
+gzip compressed data, was "inputty-1.0.4.tar", last modified: Sun Jun 18 11:19:04 2023, max compression
```

## Comparing `inputty-1.0.3.tar` & `inputty-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.3/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1161 2023-06-06 16:52:30.119789 inputty-1.0.3/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.3/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/inputty/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.3/inputty/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-06 16:52:09.000000 inputty-1.0.3/inputty/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/inputty/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.3/inputty/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     8058 2023-06-06 16:52:25.000000 inputty-1.0.3/inputty/src/input.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/inputty/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.3/inputty/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3230 2023-05-30 11:09:18.000000 inputty-1.0.3/inputty/tests/test_input.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      339 2023-05-31 08:29:56.000000 inputty-1.0.3/inputty/xxx.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-06 16:52:30.119789 inputty-1.0.3/inputty.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1161 2023-06-06 16:52:29.000000 inputty-1.0.3/inputty.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      318 2023-06-06 16:52:30.000000 inputty-1.0.3/inputty.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-06 16:52:29.000000 inputty-1.0.3/inputty.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-06-06 16:52:29.000000 inputty-1.0.3/inputty.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-06 16:52:30.123123 inputty-1.0.3/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.3/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 inputty-1.0.4/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1242 2023-06-18 11:19:04.962110 inputty-1.0.4/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)       96 2023-05-09 13:23:03.000000 inputty-1.0.4/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/inputty/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      124 2023-05-09 13:45:56.000000 inputty-1.0.4/inputty/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-18 11:17:15.000000 inputty-1.0.4/inputty/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/inputty/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 inputty-1.0.4/inputty/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2129 2023-06-18 11:11:12.000000 inputty-1.0.4/inputty/src/colours.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9133 2023-06-18 10:50:30.000000 inputty-1.0.4/inputty/src/input.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/inputty/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-29 12:23:03.000000 inputty-1.0.4/inputty/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3219 2023-06-17 09:42:30.000000 inputty-1.0.4/inputty/tests/test_input.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      664 2023-06-18 11:15:07.000000 inputty-1.0.4/inputty/tests/test_prompt.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      551 2023-06-18 10:49:43.000000 inputty-1.0.4/inputty/xxx.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:19:04.962110 inputty-1.0.4/inputty.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1242 2023-06-18 11:19:04.000000 inputty-1.0.4/inputty.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      370 2023-06-18 11:19:04.000000 inputty-1.0.4/inputty.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-18 11:19:04.000000 inputty-1.0.4/inputty.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        8 2023-06-18 11:19:04.000000 inputty-1.0.4/inputty.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-18 11:19:04.965443 inputty-1.0.4/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1157 2023-05-09 13:25:02.000000 inputty-1.0.4/setup.py
```

### Comparing `inputty-1.0.3/LICENSE.txt` & `inputty-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inputty-1.0.3/PKG-INFO` & `inputty-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 1.0.3
+Version: 1.0.4
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
-Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
+Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # inputty
 
 A module to facilitate CLI inputs.
 
@@ -20,18 +21,27 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.4 18 June 2023
+
+1. Colour cues
+
+------
+
 Version 1.0.3 6 June 2023
 
 1. Actually make changes
 
+------
+
+
 Version 1.0.2 6 June 2023
 
 1. Allow the capture of a string
 2. Add extra args with INTEGERS
 3. Add space to end of prompt
 
 ------
@@ -75,7 +85,9 @@
 ------
 
 Version 0.0.0 9 May 2023
 
 1. Initial version
 
 ------
+
+
```

### Comparing `inputty-1.0.3/inputty/src/input.py` & `inputty-1.0.4/inputty/src/input.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Provide an Input class to handle CLI inputs."""
 
 from typing import List, Tuple
 from termcolor import cprint
-import colorama
 
-colorama.init()
+from .colours import get_colour_map
+
+__all__ = ['Input']
 
 MODULE_COLOUR = 'blue'
 ERROR_COLOUR = 'red'
 INVALID_SPEC_MSG = 'Invalid specification for process:'
 INVALID_INPUT_MSG = 'Invalid input.'
 USE_ONE_OF_MSG = 'Use one of'
 INTEGER_RANGE_MSG = 'Integer outside valid range:'
 
+DEFAULT_COLOURS = {
+    'text': ('black',),
+    'cues': ('green', 'bright'),
+}
+
 RETURN = '<RTN>'
 STRING = '<STRING>'
 INTEGER_SELECTION = '<INTEGERS>'
 INTEGER_BASE = 1
 
-__all__ = ['Input']
-
 
 class Input():
     """
     The class takes a prompt string and a list of processes that
     define allowed inputs and the relevant process to be called.
 
     Attributes
@@ -69,16 +73,17 @@
         Input(prompt, processes)()
     or,
         my_input = Input(prompt, processes)
         my_input()
     """
     def __init__(self, prompt: str,
                  processes: dict[str, Tuple[object, List[object]]],
-                 validation: dict[str, object] = {}):
-        self.prompt = prompt.strip() + ' '
+                 validation: dict[str, object] = {},
+                 colours: dict[str, str] = DEFAULT_COLOURS):
+        self.prompt = self.colorize_prompt(prompt, processes, colours)
         self.processes = self._generate_processes(processes)
         self.validation = validation
         self.message_list = self._get_message_list(processes)
         self .response = None
         self.error_colour = ERROR_COLOUR
         # Are valid inputs to be included in the error message?
         self.include_valid_in_error = True
@@ -225,9 +230,32 @@
         if self.include_valid_in_error:
             valid_responses_list = self.message_list
             valid_responses = ', '.join(valid_responses_list)
             if len(valid_responses_list) >= 1:
                 return f'{INVALID_INPUT_MSG} {USE_ONE_OF_MSG} {valid_responses}'
         return INVALID_INPUT_MSG
 
+    def colorize_prompt(self, prompt, processes, colours) -> str:
+        colours = get_colour_map(colours)
+        prompt = prompt.strip() + ' '
+        for key, item in processes.items():
+            if f"'{key}'" in prompt:
+                # prompt = prompt.replace(f"'{key}'", f"{Fore.BLUE}{key}{''}")
+                prompt = prompt.replace(f"'{key}'", self.colorize_key(key, colours))
+        return prompt
+
+    @staticmethod
+    def colorize_key(key: str, colours) -> str:
+        text_fore = colours['text-fore']
+        text_style = colours['text-style']
+        text_back = colours['text-back']
+        text_format = f'{text_fore}{text_style}{text_back}'
+
+        cues_fore = colours['cues-fore']
+        cues_style = colours['cues-style']
+        cues_back = colours['cues-back']
+        cues_format = f'{cues_fore}{cues_style}{cues_back}'
+
+        return f"{cues_format}{key}{text_format}"
+
     def __str__(self) -> str:
         return f'Input: {self.prompt} {[key for key in self.processes]}'
```

### Comparing `inputty-1.0.3/inputty/tests/test_input.py` & `inputty-1.0.4/inputty/tests/test_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,13 +100,13 @@
         'Y': (input_Y, ['Y input']),
         'Q': (sys.exit, ['user quit']),
     }
 
     for response in ['P', 'Q']:
         monkeypatch.setattr('builtins.input', lambda name: response)
         if response == 'P':
-            captured = capsys.readouterr()
+            capsys.readouterr()
             # assert captured.out.strip() == 'Invalid input'
         else:
             with pytest.raises(SystemExit) as excinfo:
                 Input(prompt, processes).invoke()
             assert excinfo.value.code == 'user quit'
```

### Comparing `inputty-1.0.3/inputty.egg-info/PKG-INFO` & `inputty-1.0.4/inputty.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: inputty
-Version: 1.0.3
+Version: 1.0.4
 Summary: """A collection of modules that supports cCLI inputs."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
-Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
+Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # inputty
 
 A module to facilitate CLI inputs.
 
@@ -20,18 +21,27 @@
 ```bash
 pip install inputty
 ```
 
 
 # Version History
 
+Version 1.0.4 18 June 2023
+
+1. Colour cues
+
+------
+
 Version 1.0.3 6 June 2023
 
 1. Actually make changes
 
+------
+
+
 Version 1.0.2 6 June 2023
 
 1. Allow the capture of a string
 2. Add extra args with INTEGERS
 3. Add space to end of prompt
 
 ------
@@ -75,7 +85,9 @@
 ------
 
 Version 0.0.0 9 May 2023
 
 1. Initial version
 
 ------
+
+
```

### Comparing `inputty-1.0.3/setup.py` & `inputty-1.0.4/setup.py`

 * *Files identical despite different names*


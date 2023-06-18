# Comparing `tmp/CallingGPT-0.0.0.2.tar.gz` & `tmp/CallingGPT-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CallingGPT-0.0.0.2.tar", last modified: Sat Jun 17 12:38:15 2023, max compression
+gzip compressed data, was "CallingGPT-0.0.0.3.tar", last modified: Sun Jun 18 03:03:20 2023, max compression
```

## Comparing `CallingGPT-0.0.0.2.tar` & `CallingGPT-0.0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.744107 CallingGPT-0.0.0.2/CallingGPT/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.748108 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3277 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      395 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.748108 CallingGPT-0.0.0.2/CallingGPT/cli/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      933 2023-06-17 08:44:54.000000 CallingGPT-0.0.0.2/CallingGPT/cli/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/CallingGPT/entities/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.2/CallingGPT/entities/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4420 2023-06-17 08:49:00.000000 CallingGPT-0.0.0.2/CallingGPT/entities/namespace.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/CallingGPT/session/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.2/CallingGPT/session/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2244 2023-06-17 08:49:49.000000 CallingGPT-0.0.0.2/CallingGPT/session/session.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3277 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2873 2023-06-17 12:37:52.000000 CallingGPT-0.0.0.2/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      748 2023-06-17 12:37:52.000000 CallingGPT-0.0.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.119381 CallingGPT-0.0.0.3/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.107380 CallingGPT-0.0.0.3/CallingGPT/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.115381 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3506 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      395 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-18 03:03:20.000000 CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.115381 CallingGPT-0.0.0.3/CallingGPT/cli/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1062 2023-06-18 03:02:45.000000 CallingGPT-0.0.0.3/CallingGPT/cli/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.115381 CallingGPT-0.0.0.3/CallingGPT/entities/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.3/CallingGPT/entities/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4420 2023-06-17 08:49:00.000000 CallingGPT-0.0.0.3/CallingGPT/entities/namespace.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-18 03:03:20.119381 CallingGPT-0.0.0.3/CallingGPT/session/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.3/CallingGPT/session/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2287 2023-06-18 02:57:27.000000 CallingGPT-0.0.0.3/CallingGPT/session/session.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3506 2023-06-18 03:03:20.119381 CallingGPT-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3102 2023-06-18 03:02:22.000000 CallingGPT-0.0.0.3/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-18 03:03:20.119381 CallingGPT-0.0.0.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      748 2023-06-18 03:03:07.000000 CallingGPT-0.0.0.3/setup.py
```

### Comparing `CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/PKG-INFO` & `CallingGPT-0.0.0.3/CallingGPT/CallingGPT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # CallingGPT
 
-GPT's Function Calling - the proof-of-concept.  
+[![PyPi](https://img.shields.io/pypi/v/CallingGPT.svg)](https://pypi.python.org/pypi/CallingGPT)
 
-> Read this guide before you start: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
+GPT's Function Calling Demo, a experiment of self-hosted ChatGPT-Plugins-like platform.
+
+> Recommend reading: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
 
 ## Abstract
 
 OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT-Plugins-like` tools. This repository is a proof-of-concept of the function calling feature.  
 In this experiment, we defined the `Plugin` as `Namespace` which contains a serial of functions. While user performing a conversation, the functions in `Namespace` will be called by the API and return the result to the user.
 
 ## Usage
@@ -62,14 +64,16 @@
 >>> say hello to Rock
 func<examples.greet.greet>: Hello, Rock!
 >>> and to Alice
 func<examples.greet.greet>: Hello, Alice!
 >>> 
 ```
 
+Type `help` to get help.
+
 ## For Code
 
 1. Install the package
 
     ```bash
     pip install --upgrade CallingGPT
     ```
@@ -84,15 +88,17 @@
 
         Args:
             prompt(str): The prompt of the function.
 
         Returns:
             The result of the function.
         """
-        # Google style docstring is REQUIRED, it will be split into `description` and `params`(required if there are args) and `returns`(optional), `\n\n` between each part.
+        # Google style docstring is REQUIRED, it will be split into
+        # `description` and `params`(required if there are args) and 
+        # `returns`(optional), `\n\n` between each part.
         return "func_a: " + prompt
     ```
 
     ```python
     # your_module_b.py
     def adder(a: int, b: int) -> int:
         """
@@ -109,16 +115,18 @@
         return a + b
     ```
 
 3. Call the wrapper
 
     ```python
     from CallingGPT.session.session import Session
-
     import your_module_a, your_module_b
+    import openai
+
+    openai.apikey = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
     session.ask("your prompt")
     ```
 
     `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.2/CallingGPT/cli/__init__.py` & `CallingGPT-0.0.0.3/CallingGPT/cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,19 @@
     cmd = input(">>> ")
 
     while cmd != "exit":
         if cmd == "help":
             print("help: print this message")
             print("exit: exit the program")
             print("lsf: list all functions")
+            print("msg: list all messages")
         elif cmd == "lsf":
             print(json.dumps(session.namespace.functions_list, indent=4))
+        elif cmd == "msg":
+            print(json.dumps(session.messages, indent=4))
         else:
             resp = session.ask(cmd)
 
             if resp['type'] == 'function_call':
                 print(
                     "func<{}>: {}".format(
                         resp['func'],
```

### Comparing `CallingGPT-0.0.0.2/CallingGPT/entities/namespace.py` & `CallingGPT-0.0.0.3/CallingGPT/entities/namespace.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.2/CallingGPT/session/session.py` & `CallingGPT-0.0.0.3/CallingGPT/session/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,17 @@
         ret = {}
 
         if 'function_call' in reply_msg:
             fc = reply_msg['function_call']
             args = json.loads(fc['arguments'])
             call_ret = self._call_function(fc['name'], args)
 
-            append_msg['content'] = "(Function: {} called, and returned: {})".format(
+            append_msg['role'] = 'system'
+
+            append_msg['content'] = "(Function {} called, returned: {})".format(
                 fc['name'],
                 call_ret
             )
 
             ret = {
                 "type": "function_call",
                 "func": fc['name'].replace('-', '.'),
@@ -82,8 +84,9 @@
 
         # get the function
         function = self.namespace.functions[module_name][function_name]['function']
 
         # call the function
         result = function(**args)
 
-        return result
+        return result
+
```

### Comparing `CallingGPT-0.0.0.2/PKG-INFO` & `CallingGPT-0.0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # CallingGPT
 
-GPT's Function Calling - the proof-of-concept.  
+[![PyPi](https://img.shields.io/pypi/v/CallingGPT.svg)](https://pypi.python.org/pypi/CallingGPT)
 
-> Read this guide before you start: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
+GPT's Function Calling Demo, a experiment of self-hosted ChatGPT-Plugins-like platform.
+
+> Recommend reading: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
 
 ## Abstract
 
 OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT-Plugins-like` tools. This repository is a proof-of-concept of the function calling feature.  
 In this experiment, we defined the `Plugin` as `Namespace` which contains a serial of functions. While user performing a conversation, the functions in `Namespace` will be called by the API and return the result to the user.
 
 ## Usage
@@ -62,14 +64,16 @@
 >>> say hello to Rock
 func<examples.greet.greet>: Hello, Rock!
 >>> and to Alice
 func<examples.greet.greet>: Hello, Alice!
 >>> 
 ```
 
+Type `help` to get help.
+
 ## For Code
 
 1. Install the package
 
     ```bash
     pip install --upgrade CallingGPT
     ```
@@ -84,15 +88,17 @@
 
         Args:
             prompt(str): The prompt of the function.
 
         Returns:
             The result of the function.
         """
-        # Google style docstring is REQUIRED, it will be split into `description` and `params`(required if there are args) and `returns`(optional), `\n\n` between each part.
+        # Google style docstring is REQUIRED, it will be split into
+        # `description` and `params`(required if there are args) and 
+        # `returns`(optional), `\n\n` between each part.
         return "func_a: " + prompt
     ```
 
     ```python
     # your_module_b.py
     def adder(a: int, b: int) -> int:
         """
@@ -109,16 +115,18 @@
         return a + b
     ```
 
 3. Call the wrapper
 
     ```python
     from CallingGPT.session.session import Session
-
     import your_module_a, your_module_b
+    import openai
+
+    openai.apikey = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
     session.ask("your prompt")
     ```
 
     `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.2/README.md` & `CallingGPT-0.0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # CallingGPT
 
-GPT's Function Calling - the proof-of-concept.  
+[![PyPi](https://img.shields.io/pypi/v/CallingGPT.svg)](https://pypi.python.org/pypi/CallingGPT)
 
-> Read this guide before you start: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
+GPT's Function Calling Demo, a experiment of self-hosted ChatGPT-Plugins-like platform.
+
+> Recommend reading: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
 
 ## Abstract
 
 OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT-Plugins-like` tools. This repository is a proof-of-concept of the function calling feature.  
 In this experiment, we defined the `Plugin` as `Namespace` which contains a serial of functions. While user performing a conversation, the functions in `Namespace` will be called by the API and return the result to the user.
 
 ## Usage
@@ -50,14 +52,16 @@
 >>> say hello to Rock
 func<examples.greet.greet>: Hello, Rock!
 >>> and to Alice
 func<examples.greet.greet>: Hello, Alice!
 >>> 
 ```
 
+Type `help` to get help.
+
 ## For Code
 
 1. Install the package
 
     ```bash
     pip install --upgrade CallingGPT
     ```
@@ -72,15 +76,17 @@
 
         Args:
             prompt(str): The prompt of the function.
 
         Returns:
             The result of the function.
         """
-        # Google style docstring is REQUIRED, it will be split into `description` and `params`(required if there are args) and `returns`(optional), `\n\n` between each part.
+        # Google style docstring is REQUIRED, it will be split into
+        # `description` and `params`(required if there are args) and 
+        # `returns`(optional), `\n\n` between each part.
         return "func_a: " + prompt
     ```
 
     ```python
     # your_module_b.py
     def adder(a: int, b: int) -> int:
         """
@@ -97,16 +103,18 @@
         return a + b
     ```
 
 3. Call the wrapper
 
     ```python
     from CallingGPT.session.session import Session
-
     import your_module_a, your_module_b
+    import openai
+
+    openai.apikey = 'your_openai_api_key'
 
     session = Session([your_module_a, your_module_b])
 
     session.ask("your prompt")
     ```
 
     `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.2/setup.py` & `CallingGPT-0.0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CallingGPT',
-    version='0.0.0.2',
+    version='0.0.0.3',
     description="GPT's function calling feature wrapper",
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     install_requires=[
         'openai',
     ],
     author='RockChinQ',
```


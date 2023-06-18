# Comparing `tmp/promptrix-0.2.4.tar.gz` & `tmp/promptrix-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.2.4.tar", last modified: Thu Jun 15 20:06:44 2023, max compression
+gzip compressed data, was "promptrix-0.2.5.tar", last modified: Sun Jun 18 19:19:27 2023, max compression
```

## Comparing `promptrix-0.2.4.tar` & `promptrix-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:06:44.845356 promptrix-0.2.4/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.4/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2225 2023-06-15 20:06:44.845356 promptrix-0.2.4/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1655 2023-06-14 03:06:34.000000 promptrix-0.2.4/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      777 2023-06-15 20:06:35.000000 promptrix-0.2.4/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-15 20:06:44.845356 promptrix-0.2.4/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:06:44.841356 promptrix-0.2.4/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:06:44.845356 promptrix-0.2.4/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      763 2023-06-12 20:40:27.000000 promptrix-0.2.4/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2900 2023-06-15 03:37:36.000000 promptrix-0.2.4/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.4/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.2.4/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.2.4/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.2.4/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.4/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2445 2023-06-15 17:06:28.000000 promptrix-0.2.4/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.4/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5738 2023-06-14 19:26:14.000000 promptrix-0.2.4/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.4/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.2.4/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-14 19:25:22.000000 promptrix-0.2.4/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-14 20:55:08.000000 promptrix-0.2.4/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.4/src/promptrix/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.4/src/promptrix/promptrixTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:06:44.845356 promptrix-0.2.4/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2225 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-15 20:06:44.000000 promptrix-0.2.4/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:19:27.511229 promptrix-0.2.5/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.2.5/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2177 2023-06-18 19:19:27.511229 promptrix-0.2.5/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.2.5/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      847 2023-06-18 19:19:17.000000 promptrix-0.2.5/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-18 19:19:27.511229 promptrix-0.2.5/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:19:27.511229 promptrix-0.2.5/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:19:27.511229 promptrix-0.2.5/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      763 2023-06-12 20:40:27.000000 promptrix-0.2.5/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2900 2023-06-15 03:37:36.000000 promptrix-0.2.5/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.2.5/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.2.5/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.2.5/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.2.5/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.2.5/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2445 2023-06-15 17:06:28.000000 promptrix-0.2.5/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.2.5/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5738 2023-06-14 19:26:14.000000 promptrix-0.2.5/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.2.5/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.2.5/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      985 2023-06-14 19:25:22.000000 promptrix-0.2.5/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-14 20:55:08.000000 promptrix-0.2.5/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.2.5/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.2.5/src/promptrix/promptrixTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:19:27.511229 promptrix-0.2.5/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2177 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-06-18 19:19:27.000000 promptrix-0.2.5/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.2.4/LICENSE` & `promptrix-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/PKG-INFO` & `promptrix-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.4
+Version: 0.2.5
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,14 @@
         msgs = []
         if not as_msgs.tooLong:
             msgs = as_msgs.output
         return msgs
 
     ### basic chat loop
     while True:
-        query = input('Hi, how can I help you?)
         memory.set('input', query)
         msgs = asyncio.run(render_messages_completion())
         response = ... your favorite llm api (model, msgs, ...)
         print(response)
         history = memory.get('history')
         history.append({'role':USER_PREFIX, 'content': query})
         history.append({'role': ASSISTANT_PREFIX, 'content': response})
```

### Comparing `promptrix-0.2.4/README.md` & `promptrix-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         msgs = []
         if not as_msgs.tooLong:
             msgs = as_msgs.output
         return msgs
 
     ### basic chat loop
     while True:
-        query = input('Hi, how can I help you?)
         memory.set('input', query)
         msgs = asyncio.run(render_messages_completion())
         response = ... your favorite llm api (model, msgs, ...)
         print(response)
         history = memory.get('history')
         history.append({'role':USER_PREFIX, 'content': query})
         history.append({'role': ASSISTANT_PREFIX, 'content': response})
```

### Comparing `promptrix-0.2.4/src/promptrix/AssistantMessage.py` & `promptrix-0.2.5/src/promptrix/AssistantMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/ConversationHistory.py` & `promptrix-0.2.5/src/promptrix/ConversationHistory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/FunctionRegistry.py` & `promptrix-0.2.5/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/GPT3Tokenizer.py` & `promptrix-0.2.5/src/promptrix/GPT3Tokenizer.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/GroupSection.py` & `promptrix-0.2.5/src/promptrix/GroupSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/LayoutEngine.py` & `promptrix-0.2.5/src/promptrix/LayoutEngine.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/PromptSectionBase.py` & `promptrix-0.2.5/src/promptrix/PromptSectionBase.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/TemplateSection.py` & `promptrix-0.2.5/src/promptrix/TemplateSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/TextSection.py` & `promptrix-0.2.5/src/promptrix/TextSection.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/UserMessage.py` & `promptrix-0.2.5/src/promptrix/UserMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/Utilities.py` & `promptrix-0.2.5/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/VolatileMemory.py` & `promptrix-0.2.5/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix/promptrixTypes.py` & `promptrix-0.2.5/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.2.4/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.2.5/src/promptrix.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.2.4
+Version: 0.2.5
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/promptrix-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,14 @@
         msgs = []
         if not as_msgs.tooLong:
             msgs = as_msgs.output
         return msgs
 
     ### basic chat loop
     while True:
-        query = input('Hi, how can I help you?)
         memory.set('input', query)
         msgs = asyncio.run(render_messages_completion())
         response = ... your favorite llm api (model, msgs, ...)
         print(response)
         history = memory.get('history')
         history.append({'role':USER_PREFIX, 'content': query})
         history.append({'role': ASSISTANT_PREFIX, 'content': response})
```

### Comparing `promptrix-0.2.4/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.2.5/src/promptrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/yid_langchain_extensions-0.4.6.tar.gz` & `tmp/yid_langchain_extensions-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yid_langchain_extensions-0.4.6.tar", last modified: Sat Jun 17 18:23:11 2023, max compression
+gzip compressed data, was "yid_langchain_extensions-0.4.7.tar", last modified: Sun Jun 18 07:15:35 2023, max compression
```

## Comparing `yid_langchain_extensions-0.4.6.tar` & `yid_langchain_extensions-0.4.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:23:11.357780 yid_langchain_extensions-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 18:23:11.357780 yid_langchain_extensions-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:23:11.357780 yid_langchain_extensions-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:23:11.357780 yid_langchain_extensions-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/tests/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:23:11.357780 yid_langchain_extensions-0.4.6/yid_langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:23:11.357780 yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/action_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/class_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/direct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/thoughts_json_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:23:11.357780 yid_langchain_extensions-0.4.6/yid_langchain_extensions/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/tools/agent_as_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 18:22:44.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:23:11.357780 yid_langchain_extensions-0.4.6/yid_langchain_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 18:23:11.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 18:23:11.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:23:11.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-17 18:23:11.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-17 18:23:11.000000 yid_langchain_extensions-0.4.6/yid_langchain_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.986989 yid_langchain_extensions-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.986989 yid_langchain_extensions-0.4.7/yid_langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/action_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/class_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/direct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/thoughts_json_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/agent_as_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/top_level.txt
```

### Comparing `yid_langchain_extensions-0.4.6/LICENSE` & `yid_langchain_extensions-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.6/PKG-INFO` & `yid_langchain_extensions-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid_langchain_extensions
-Version: 0.4.6
+Version: 0.4.7
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.4.6/setup.py` & `yid_langchain_extensions-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='yid_langchain_extensions',
-    version='0.4.6',
+    version='0.4.7',
     author='Dmitrii Rashchenko',
     author_email='dimitree54@gmail.com',
     packages=find_packages(),
     description='Useful classes extending langchain library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dimitree54/yid_langchain_extensions',
```

### Comparing `yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/action_parser.py` & `yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/action_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 from langchain.schema import AgentAction
 
 from yid_langchain_extensions.output_parser.thoughts_json_parser import Thought, ThoughtsJSONParser
 
 
 class ActionParser(ThoughtsJSONParser):
-    extra_thoughts: List[Thought] = []
-    action_thoughts: List[Thought] = [
-        Thought(name="action", description="The action to take. Must be one of [{tool_names}]"),
-        Thought(name="action_input", description="The input to the action")
-    ]
-
-    @property
-    def thoughts(self) -> List[Thought]:
-        return self.action_thoughts + self.extra_thoughts
+    @classmethod
+    def from_extra_thoughts(cls, extra_thoughts: List[Thought]):
+        action_thoughts: List[Thought] = [
+            Thought(name="action", description="The action to take. Must be one of [{tool_names}]"),
+            Thought(name="action_input", description="The input to the action")
+        ]
+        thoughts = extra_thoughts + action_thoughts
+        return cls(thoughts=thoughts)
 
     def parse(self, text: str) -> AgentAction:
         response = super().parse(text)
         return AgentAction(response["action"], response["action_input"], text)
```

### Comparing `yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/class_parser.py` & `yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/class_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,19 +18,18 @@
 
 
 def get_classes_summary(classes: List[Class]) -> str:
     return "; ".join([f"{class_index} ({_class.name})" for class_index, _class in enumerate(classes)])
 
 
 class ClassParser(ThoughtsJSONParser):
-    extra_thoughts: List[Thought] = []
-    action_thoughts: List[Thought] = [
-        Thought(name="class_index", type="int", description="The class chosen. Must be one of [{classes_summary}]"),
-    ]
-
-    @property
-    def thoughts(self) -> List[Thought]:
-        return self.action_thoughts + self.extra_thoughts
+    @classmethod
+    def from_extra_thoughts(cls, extra_thoughts: List[Thought]):
+        action_thoughts: List[Thought] = [
+            Thought(name="class_index", type="int", description="The class chosen. Must be one of [{classes_summary}]"),
+        ]
+        thoughts = extra_thoughts + action_thoughts
+        return cls(thoughts=thoughts)
 
     def parse(self, text: str) -> int:
         response = super().parse(text)
         return int(response["class_index"])
```

### Comparing `yid_langchain_extensions-0.4.6/yid_langchain_extensions/output_parser/thoughts_json_parser.py` & `yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/thoughts_json_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import List, Dict, Any
 
 from langchain import PromptTemplate
 from langchain.schema import BaseOutputParser
-from pydantic import BaseModel
+from pydantic import BaseModel, validator
 
 FORMAT_PROMPT = """FORMAT:
 ------
 You response should be in the following format:
 
 ```json
 {
@@ -22,14 +22,19 @@
     type: str = "string"
 
 
 class ThoughtsJSONParser(BaseOutputParser):
     stop_sequences: List[str] = ["}\n```", "}```"]
     thoughts: List[Thought] = []
 
+    @validator("thoughts")
+    def validate_thoughts(cls, v):
+        assert len(v) > 0, "You must have at least one thought"
+        return v
+
     def parse(self, text: str) -> Dict[str, Any]:
         text += self.stop_sequences[0]
         cleaned_output = text.strip()
         if "```json" in cleaned_output:
             _, cleaned_output = cleaned_output.split("```json")
         if "```" in cleaned_output:
             cleaned_output, _ = cleaned_output.split("```")
```

### Comparing `yid_langchain_extensions-0.4.6/yid_langchain_extensions/tools/agent_as_tool.py` & `yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/agent_as_tool.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.6/yid_langchain_extensions.egg-info/PKG-INFO` & `yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid-langchain-extensions
-Version: 0.4.6
+Version: 0.4.7
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.4.6/yid_langchain_extensions.egg-info/SOURCES.txt` & `yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*


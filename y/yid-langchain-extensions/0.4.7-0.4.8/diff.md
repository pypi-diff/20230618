# Comparing `tmp/yid_langchain_extensions-0.4.7.tar.gz` & `tmp/yid_langchain_extensions-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yid_langchain_extensions-0.4.7.tar", last modified: Sun Jun 18 07:15:35 2023, max compression
+gzip compressed data, was "yid_langchain_extensions-0.4.8.tar", last modified: Sun Jun 18 07:30:03 2023, max compression
```

## Comparing `yid_langchain_extensions-0.4.7.tar` & `yid_langchain_extensions-0.4.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.986989 yid_langchain_extensions-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/tests/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.986989 yid_langchain_extensions-0.4.7/yid_langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/action_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/class_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/direct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/thoughts_json_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/agent_as_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-18 07:15:13.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:15:35.990989 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 07:15:35.000000 yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/yid_langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/action_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/class_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/direct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/thoughts_json_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/agent_as_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-18 07:29:44.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:30:03.365272 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 07:30:03.000000 yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/top_level.txt
```

### Comparing `yid_langchain_extensions-0.4.7/LICENSE` & `yid_langchain_extensions-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.7/PKG-INFO` & `yid_langchain_extensions-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid_langchain_extensions
-Version: 0.4.7
+Version: 0.4.8
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.4.7/setup.py` & `yid_langchain_extensions-0.4.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='yid_langchain_extensions',
-    version='0.4.7',
+    version='0.4.8',
     author='Dmitrii Rashchenko',
     author_email='dimitree54@gmail.com',
     packages=find_packages(),
     description='Useful classes extending langchain library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dimitree54/yid_langchain_extensions',
```

### Comparing `yid_langchain_extensions-0.4.7/tests/test_parser.py` & `yid_langchain_extensions-0.4.8/tests/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import unittest
 
+from pydantic import ValidationError
+
 from yid_langchain_extensions.output_parser.action_parser import ActionParser
 from yid_langchain_extensions.output_parser.class_parser import Class, get_classes_description, get_classes_summary, \
     ClassParser
 from yid_langchain_extensions.output_parser.thoughts_json_parser import ThoughtsJSONParser, Thought
 
 
 class TestThoughtsJSONParser(unittest.TestCase):
     def test_parse(self):
         parser = ThoughtsJSONParser(
-            extra_thoughts=[
+            thoughts=[
                 Thought(name="thought1", description="Thought 1"),
                 Thought(name="thought2", type="int", description="Thought 2")
             ]
         )
         string_to_parse = """```json
 {
     "thought1": "thought 1",
@@ -41,14 +43,18 @@
             Thought(name="thought2", type="int", description="Thought 2")
         ]
         format_instructions = ThoughtsJSONParser(
             thoughts=thoughts
         ).get_format_instructions()
         self.assertTrue('"thought1": string [Thought 1]\n\t"thought2": int [Thought 2]' in format_instructions)
 
+    def test_raise_without_thoughts(self):
+        with self.assertRaises(ValidationError):
+            ThoughtsJSONParser(thoughts=[])
+
 
 class TestClassParser(unittest.TestCase):
     def setUp(self) -> None:
         self.classes = [
             Class(name="class1", description="description1"),
             Class(name="class2", description="description2"),
         ]
@@ -57,15 +63,15 @@
         self.assertEqual(get_classes_description(self.classes),
                          "> 0: class1. description1;\n> 1: class2. description2;\n")
 
     def test_get_classes_summary(self):
         self.assertEqual(get_classes_summary(self.classes), "0 (class1); 1 (class2)")
 
     def test_class_parser(self):
-        class_parser = ClassParser(extra_thoughts=[
+        class_parser = ClassParser.from_extra_thoughts(extra_thoughts=[
             Thought(name="thought1", description="Thought 1")
         ])
         string_to_parse = """```json
 {
     "thought1": "thought 1",
     "class_index": 0
 """
@@ -79,15 +85,15 @@
         class_parser = ClassParser.from_extra_thoughts(extra_thoughts=extra_thoughts)
         self.assertEqual(class_parser.thoughts[:2], extra_thoughts)
         self.assertEqual(class_parser.thoughts[2].name, "class_index")
 
 
 class TestActionParser(unittest.TestCase):
     def test_class_parser(self):
-        class_parser = ActionParser(extra_thoughts=[
+        class_parser = ActionParser.from_extra_thoughts(extra_thoughts=[
             Thought(name="thought1", description="Thought 1")
         ])
         string_to_parse = """```json
 {
     "thought1": "thought 1",
     "action": "action 1",
     "action_input": "action input"
```

### Comparing `yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/action_parser.py` & `yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/action_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from yid_langchain_extensions.output_parser.thoughts_json_parser import Thought, ThoughtsJSONParser
 
 
 class ActionParser(ThoughtsJSONParser):
     @classmethod
     def from_extra_thoughts(cls, extra_thoughts: List[Thought]):
         action_thoughts: List[Thought] = [
-            Thought(name="action", description="The action to take. Must be one of [{tool_names}]"),
+            Thought(name="action", description="The action to take. Must be one of [{{tool_names}}]"),
             Thought(name="action_input", description="The input to the action")
         ]
         thoughts = extra_thoughts + action_thoughts
         return cls(thoughts=thoughts)
 
     def parse(self, text: str) -> AgentAction:
         response = super().parse(text)
```

### Comparing `yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/class_parser.py` & `yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/class_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     return "; ".join([f"{class_index} ({_class.name})" for class_index, _class in enumerate(classes)])
 
 
 class ClassParser(ThoughtsJSONParser):
     @classmethod
     def from_extra_thoughts(cls, extra_thoughts: List[Thought]):
         action_thoughts: List[Thought] = [
-            Thought(name="class_index", type="int", description="The class chosen. Must be one of [{classes_summary}]"),
+            Thought(name="class_index", type="int",
+                    description="The class chosen. Must be one of [{{classes_summary}}]"),
         ]
         thoughts = extra_thoughts + action_thoughts
         return cls(thoughts=thoughts)
 
     def parse(self, text: str) -> int:
         response = super().parse(text)
         return int(response["class_index"])
```

### Comparing `yid_langchain_extensions-0.4.7/yid_langchain_extensions/output_parser/thoughts_json_parser.py` & `yid_langchain_extensions-0.4.8/yid_langchain_extensions/output_parser/thoughts_json_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 class Thought(BaseModel):
     name: str
     description: str
     type: str = "string"
 
 
 class ThoughtsJSONParser(BaseOutputParser):
+    thoughts: List[Thought]
     stop_sequences: List[str] = ["}\n```", "}```"]
-    thoughts: List[Thought] = []
 
     @validator("thoughts")
     def validate_thoughts(cls, v):
         assert len(v) > 0, "You must have at least one thought"
         return v
 
     def parse(self, text: str) -> Dict[str, Any]:
```

### Comparing `yid_langchain_extensions-0.4.7/yid_langchain_extensions/tools/agent_as_tool.py` & `yid_langchain_extensions-0.4.8/yid_langchain_extensions/tools/agent_as_tool.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/PKG-INFO` & `yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid-langchain-extensions
-Version: 0.4.7
+Version: 0.4.8
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.4.7/yid_langchain_extensions.egg-info/SOURCES.txt` & `yid_langchain_extensions-0.4.8/yid_langchain_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*


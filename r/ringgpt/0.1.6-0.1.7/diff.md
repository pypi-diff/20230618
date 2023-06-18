# Comparing `tmp/ringgpt-0.1.6.tar.gz` & `tmp/ringgpt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringgpt-0.1.6.tar", max compression
+gzip compressed data, was "ringgpt-0.1.7.tar", max compression
```

## Comparing `ringgpt-0.1.6.tar` & `ringgpt-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-18 16:40:56.662291 ringgpt-0.1.6/README.md
--rw-r--r--   0        0        0      597 2023-06-18 16:50:57.983373 ringgpt-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.6/ringgpt/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.6/ringgpt/dataloader.py
--rw-r--r--   0        0        0     5815 2023-06-18 16:50:13.265631 ringgpt-0.1.6/ringgpt/prompt.py
--rw-r--r--   0        0        0    10672 2023-06-18 15:50:57.342661 ringgpt-0.1.6/ringgpt/ring.py
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 ringgpt-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-18 16:40:56.662291 ringgpt-0.1.7/README.md
+-rw-r--r--   0        0        0      597 2023-06-18 16:56:10.777687 ringgpt-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.7/ringgpt/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.7/ringgpt/dataloader.py
+-rw-r--r--   0        0        0     5911 2023-06-18 16:55:51.675667 ringgpt-0.1.7/ringgpt/prompt.py
+-rw-r--r--   0        0        0    10672 2023-06-18 15:50:57.342661 ringgpt-0.1.7/ringgpt/ring.py
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 ringgpt-0.1.7/PKG-INFO
```

### Comparing `ringgpt-0.1.6/pyproject.toml` & `ringgpt-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ringgpt"
-version = "0.1.6"
+version = "0.1.7"
 description = "Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat"
 authors = ["Avinaash Anand K <avinaash96@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `ringgpt-0.1.6/ringgpt/dataloader.py` & `ringgpt-0.1.7/ringgpt/dataloader.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.6/ringgpt/prompt.py` & `ringgpt-0.1.7/ringgpt/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,48 +19,48 @@
         "Email": "Email addresses",
         "URL": "URLs to websites",
         "DateTime": "Dates and times of day in the format dd/mm/yyyy hh:mm:ss",
         "Quantity": "Numbers and numeric quantities"
     }
 
     instructions = {
-        Instruction.UNSTRUCTURED_TO_STRUCTURED: {
+        Instruction.UNSTRUCTURED_TO_STRUCTURED.value: {
             'prompt': '### INSTRUCTION ### Extract the below attributes based on the text in context below. Follow additional instructions when available for an attribute, mentioned after the colon. Use only "N/A" wherever the value for an attribute is unavailable in the context below.',
             'expected_output': '### DESIRED FORMAT OF OUTPUT ### \n<attribute_name>: <extracted_value>'
         },
-        Instruction.SUMMARISE: {
+        Instruction.SUMMARISE.value: {
             'prompt': '### INSTRUCTION ### I want you to act as an AI summariser. I will give you context, and you will provide a summary of that context. Your summary should be informative and factual, covering the most important aspects of the context.',
             'expected_output': '### DESIRED FORMAT OF OUTPUT ### \n<summary_text>'
         },
-        Instruction.CLASSIFICATION: {
+        Instruction.CLASSIFICATION.value: {
             'prompt': '### INSTRUCTION ### Classify the text in context below into one of the following categories. The output should be all applicable categories from the list below.',
             'expected_output': '### DESIRED FORMAT OF OUTPUT ### \n<comma_separated_list_of_category_names>'
         },
-        Instruction.NAMED_ENTITY_RECOGNITION: {
+        Instruction.NAMED_ENTITY_RECOGNITION.value: {
             'prompt': '### INSTRUCTION ### Classify the text in context below into one of the following categories. A substring of the input context can only belong to one of the categories from the list below.',
             'expected_output': '### DESIRED FORMAT OF OUTPUT ### \n<category_name>: <comma_separated_list_of_substrings_from_text>'
         }
     }
 
     def __init__(self, instruction, instruction_categories=None, example=None):
-        if instruction not in [Instruction.UNSTRUCTURED_TO_STRUCTURED, Instruction.CLASSIFICATION, Instruction.NAMED_ENTITY_RECOGNITION,Instruction.SUMMARISE]:
+        if instruction not in [Instruction.UNSTRUCTURED_TO_STRUCTURED.value, Instruction.CLASSIFICATION.value, Instruction.NAMED_ENTITY_RECOGNITION.value,Instruction.SUMMARISE.value]:
             raise ValueError("""Instruction not recognised. Ring can only take the following instructions:
             1. Unstructured to structured
             2. Summarise
             3. Classification
             4. Named Entity Recognition""")
 
         if instruction_categories:
             if not isinstance(instruction_categories, list) or not all(isinstance(cat, str) for cat in instruction_categories):
                 raise ValueError("Instruction categories must be a list of strings.")
 
-        if instruction in [Instruction.UNSTRUCTURED_TO_STRUCTURED, Instruction.CLASSIFICATION, Instruction.NAMED_ENTITY_RECOGNITION] and not instruction_categories:
+        if instruction in [Instruction.UNSTRUCTURED_TO_STRUCTURED.value, Instruction.CLASSIFICATION.value, Instruction.NAMED_ENTITY_RECOGNITION.value] and not instruction_categories:
             raise ValueError(f"Instruction categories is mandatory for '{instruction.value}' instruction.")
 
-        if instruction == Instruction.NAMED_ENTITY_RECOGNITION and instruction_categories:
+        if instruction == Instruction.NAMED_ENTITY_RECOGNITION.value and instruction_categories:
             unique_entity_names = set(self.entity.keys())
             if not set(instruction_categories).issubset(unique_entity_names):
                 raise ValueError(f"Instruction categories can only have values from the list of unique entity names for '{instruction.value}' task.")
 
         if example:
             if not isinstance(example, list) or not all(isinstance(e, dict) and 'input' in e and 'output' in e for e in example):
                 raise ValueError("""Examples is not in the expected format. Please pass examples in the format:
@@ -73,17 +73,17 @@
         self.instruction_categories = [e.value for e in Instruction]
         
         if example:
             self.instruction_prompt = self.instructions[instruction]['prompt'] + " Refer to the examples which define expected outputs for given contexts.\n"
         else:
             self.instruction_prompt = self.instructions[instruction]['prompt']
         
-        if instruction in [Instruction.UNSTRUCTURED_TO_STRUCTURED, Instruction.CLASSIFICATION, Instruction.NAMED_ENTITY_RECOGNITION]:
+        if instruction in [Instruction.UNSTRUCTURED_TO_STRUCTURED.value, Instruction.CLASSIFICATION.value, Instruction.NAMED_ENTITY_RECOGNITION.value]:
             self.instruction_prompt += "\n### CATEGORIES ###\n"
-            if instruction == Instruction.NAMED_ENTITY_RECOGNITION:
+            if instruction == Instruction.NAMED_ENTITY_RECOGNITION.value:
                 for category in instruction_categories:
                     self.instruction_prompt += f"{category}: {self.entity.get(category, 'N/A')}\n"
             else:
                 self.instruction_prompt += "\n".join(instruction_categories) + "\n"
 
     def get_instruction_prompt(self):
         return self.instruction_prompt
```

### Comparing `ringgpt-0.1.6/ringgpt/ring.py` & `ringgpt-0.1.7/ringgpt/ring.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.6/PKG-INFO` & `ringgpt-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ringgpt
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat
 License: Apache-2.0
 Author: Avinaash Anand K
 Author-email: avinaash96@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


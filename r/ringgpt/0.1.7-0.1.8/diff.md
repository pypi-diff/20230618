# Comparing `tmp/ringgpt-0.1.7.tar.gz` & `tmp/ringgpt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringgpt-0.1.7.tar", max compression
+gzip compressed data, was "ringgpt-0.1.8.tar", max compression
```

## Comparing `ringgpt-0.1.7.tar` & `ringgpt-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-18 16:40:56.662291 ringgpt-0.1.7/README.md
--rw-r--r--   0        0        0      597 2023-06-18 16:56:10.777687 ringgpt-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.7/ringgpt/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.7/ringgpt/dataloader.py
--rw-r--r--   0        0        0     5911 2023-06-18 16:55:51.675667 ringgpt-0.1.7/ringgpt/prompt.py
--rw-r--r--   0        0        0    10672 2023-06-18 15:50:57.342661 ringgpt-0.1.7/ringgpt/ring.py
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 ringgpt-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-18 16:40:56.662291 ringgpt-0.1.8/README.md
+-rw-r--r--   0        0        0      597 2023-06-18 17:00:49.254869 ringgpt-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.8/ringgpt/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.8/ringgpt/dataloader.py
+-rw-r--r--   0        0        0     5911 2023-06-18 16:55:51.675667 ringgpt-0.1.8/ringgpt/prompt.py
+-rw-r--r--   0        0        0    10671 2023-06-18 17:00:43.191611 ringgpt-0.1.8/ringgpt/ring.py
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 ringgpt-0.1.8/PKG-INFO
```

### Comparing `ringgpt-0.1.7/pyproject.toml` & `ringgpt-0.1.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ringgpt"
-version = "0.1.7"
+version = "0.1.8"
 description = "Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat"
 authors = ["Avinaash Anand K <avinaash96@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `ringgpt-0.1.7/ringgpt/dataloader.py` & `ringgpt-0.1.8/ringgpt/dataloader.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.7/ringgpt/prompt.py` & `ringgpt-0.1.8/ringgpt/prompt.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.7/ringgpt/ring.py` & `ringgpt-0.1.8/ringgpt/ring.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             chunk_size=350,
             chunk_overlap=20,
             length_function=self.tokenizer_len,
             separators=['\n\n', '\n', ' ', '']
         )
         self.tokenizer = tiktoken.get_encoding('cl100k_base')
 
-        self.instruction_prompt = self.prompt.get_instruction_prompt() + self.example_picker(self.prompt.get_examples())
+        self.instruction_prompt = self.prompt.get_instruction_prompt() + self.example_picker(self.prompt.get_example())
 
         self.data_column_name = self.data_loader.get_data_column_name()
         self.process_data(data_column_name=self.data_column_name) 
 
         self.instruction_categories = self.prompt.get_instruction_categories()
 
     def instruction_categories_picker(self, instruction_categories):
```

### Comparing `ringgpt-0.1.7/PKG-INFO` & `ringgpt-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ringgpt
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat
 License: Apache-2.0
 Author: Avinaash Anand K
 Author-email: avinaash96@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


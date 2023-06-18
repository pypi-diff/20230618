# Comparing `tmp/ringgpt-0.1.8.tar.gz` & `tmp/ringgpt-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringgpt-0.1.8.tar", max compression
+gzip compressed data, was "ringgpt-0.1.9.tar", max compression
```

## Comparing `ringgpt-0.1.8.tar` & `ringgpt-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-18 16:40:56.662291 ringgpt-0.1.8/README.md
--rw-r--r--   0        0        0      597 2023-06-18 17:00:49.254869 ringgpt-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.8/ringgpt/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.8/ringgpt/dataloader.py
--rw-r--r--   0        0        0     5911 2023-06-18 16:55:51.675667 ringgpt-0.1.8/ringgpt/prompt.py
--rw-r--r--   0        0        0    10671 2023-06-18 17:00:43.191611 ringgpt-0.1.8/ringgpt/ring.py
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 ringgpt-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-18 16:40:56.662291 ringgpt-0.1.9/README.md
+-rw-r--r--   0        0        0      597 2023-06-18 17:08:28.270440 ringgpt-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-17 17:25:10.567674 ringgpt-0.1.9/ringgpt/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 15:38:01.724785 ringgpt-0.1.9/ringgpt/dataloader.py
+-rw-r--r--   0        0        0     5911 2023-06-18 16:55:51.675667 ringgpt-0.1.9/ringgpt/prompt.py
+-rw-r--r--   0        0        0    11401 2023-06-18 17:08:16.455814 ringgpt-0.1.9/ringgpt/ring.py
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 ringgpt-0.1.9/PKG-INFO
```

### Comparing `ringgpt-0.1.8/pyproject.toml` & `ringgpt-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ringgpt"
-version = "0.1.8"
+version = "0.1.9"
 description = "Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat"
 authors = ["Avinaash Anand K <avinaash96@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `ringgpt-0.1.8/ringgpt/dataloader.py` & `ringgpt-0.1.9/ringgpt/dataloader.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.8/ringgpt/prompt.py` & `ringgpt-0.1.9/ringgpt/prompt.py`

 * *Files identical despite different names*

### Comparing `ringgpt-0.1.8/ringgpt/ring.py` & `ringgpt-0.1.9/ringgpt/ring.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,22 +113,32 @@
             disallowed_special=()
         )
         return len(tokens)
 
     def process_data(self, data_column_name=None):
         prompt_length = self.tokenizer_len(self.instruction_prompt)
         chunk_size = 2000 - prompt_length
-        self.output_dataframe['chunk'] = self.output_dataframe[data_column_name].apply(lambda x: self.text_chunker.split_text(x, chunk_size, 20))
-        self.output_dataframe = self.output_dataframe.explode('chunk')
-        self.output_dataframe.reset_index(drop=True, inplace=True)
+        if data_column_name:
+            self.output_dataframe['chunk'] = self.output_dataframe[data_column_name].apply(lambda x: self.text_chunker.split_text(x, chunk_size, 20))
+            self.output_dataframe = self.output_dataframe.explode('chunk')
+            self.output_dataframe.reset_index(drop=True, inplace=True)
 
-        # Repeat other columns for each row
-        self.output_dataframe = self.output_dataframe.reindex(self.output_dataframe.index.repeat(len(self.output_dataframe.columns) - 1)).reset_index(drop=True)
-        self.output_dataframe[data_column_name] = self.output_dataframe['chunk']
-        self.output_dataframe.drop(columns=['chunk'], inplace=True)
+            # Repeat other columns for each row
+            self.output_dataframe = self.output_dataframe.reindex(self.output_dataframe.index.repeat(len(self.output_dataframe.columns) - 1)).reset_index(drop=True)
+            self.output_dataframe[data_column_name] = self.output_dataframe['chunk']
+            self.output_dataframe.drop(columns=['chunk'], inplace=True)
+        else:
+            self.output_dataframe[0] = self.output_dataframe[0].apply(lambda x: self.text_chunker.split_text(x, chunk_size, 20))
+            self.output_dataframe = self.output_dataframe.explode(self.output_dataframe.columns[0])
+            self.output_dataframe.reset_index(drop=True, inplace=True)
+
+            # Repeat other columns for each row
+            self.output_dataframe = self.output_dataframe.reindex(self.output_dataframe.index.repeat(len(self.output_dataframe.columns) - 1)).reset_index(drop=True)
+            self.output_dataframe[data_column_name] = self.output_dataframe[0]
+            self.output_dataframe.drop(columns=[0], inplace=True)
 
     def BardChat(self, prompt, token):
         logging.info("Function BardChat called")
         try:
             chatbot = BardChatbot(token)
             response = chatbot.ask(prompt)
             response_raw = {
```

### Comparing `ringgpt-0.1.8/PKG-INFO` & `ringgpt-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ringgpt
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package enables users to iterate on a corpus to perform single shot completion tasks leveraging GPT-3.5, Bard and Bing Chat
 License: Apache-2.0
 Author: Avinaash Anand K
 Author-email: avinaash96@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


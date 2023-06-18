# Comparing `tmp/aifunc-0.5.7.tar.gz` & `tmp/aifunc-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.5.7.tar", max compression
+gzip compressed data, was "aifunc-0.5.8.tar", max compression
```

## Comparing `aifunc-0.5.7.tar` & `aifunc-0.5.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2023-06-17 22:58:36.361414 aifunc-0.5.7/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-17 15:48:26.010370 aifunc-0.5.7/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-17 15:48:26.010370 aifunc-0.5.7/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-17 15:48:26.010370 aifunc-0.5.7/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-17 15:48:26.010370 aifunc-0.5.7/aifunc/generate_question.py
--rw-r--r--   0        0        0    13590 2023-06-18 01:16:42.106401 aifunc-0.5.7/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-18 01:25:38.630754 aifunc-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-06-17 22:58:36.361414 aifunc-0.5.8/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-17 15:48:26.010370 aifunc-0.5.8/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-17 15:48:26.010370 aifunc-0.5.8/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-17 15:48:26.010370 aifunc-0.5.8/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-17 15:48:26.010370 aifunc-0.5.8/aifunc/generate_question.py
+-rw-r--r--   0        0        0    13586 2023-06-18 01:27:21.149250 aifunc-0.5.8/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-18 01:27:29.813123 aifunc-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.8/PKG-INFO
```

### Comparing `aifunc-0.5.7/aifunc/add_ai_function.py` & `aifunc-0.5.8/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.5.7/aifunc/utility.py` & `aifunc-0.5.8/aifunc/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     instruction = data["instruction"]
     instruction = "Instruction:" + instruction
     if "example_pairs" in data.keys():
         example_pairs = data["example_pairs"]
         # some examples
         instruction += " For example: " + str(example_pairs)
-        properties = data["properties"]
+    properties = data["properties"]
 
     def fixed_format_ai_wrapper(prompt) -> dict:
         message = [{"role": "system", "content": instruction}]
         message.append({"role": "user", "content": prompt})
         function_name = "print_parameters"
         function_description = "print the generated result from assistant, including "
         for prop in properties:
```


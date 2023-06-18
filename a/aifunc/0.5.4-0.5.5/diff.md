# Comparing `tmp/aifunc-0.5.4.tar.gz` & `tmp/aifunc-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.5.4.tar", max compression
+gzip compressed data, was "aifunc-0.5.5.tar", max compression
```

## Comparing `aifunc-0.5.4.tar` & `aifunc-0.5.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2023-06-17 22:58:36.361414 aifunc-0.5.4/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-17 15:48:26.010370 aifunc-0.5.4/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-17 15:48:26.010370 aifunc-0.5.4/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-17 15:48:26.010370 aifunc-0.5.4/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-17 15:48:26.010370 aifunc-0.5.4/aifunc/generate_question.py
--rw-r--r--   0        0        0    13626 2023-06-18 01:02:07.512755 aifunc-0.5.4/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-18 01:02:32.356354 aifunc-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-06-17 22:58:36.361414 aifunc-0.5.5/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-17 15:48:26.010370 aifunc-0.5.5/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-17 15:48:26.010370 aifunc-0.5.5/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-17 15:48:26.010370 aifunc-0.5.5/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-17 15:48:26.010370 aifunc-0.5.5/aifunc/generate_question.py
+-rw-r--r--   0        0        0    13613 2023-06-18 01:12:16.713927 aifunc-0.5.5/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-18 01:12:29.841759 aifunc-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.5/PKG-INFO
```

### Comparing `aifunc-0.5.4/aifunc/add_ai_function.py` & `aifunc-0.5.5/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.5.4/aifunc/utility.py` & `aifunc-0.5.5/aifunc/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,19 +133,20 @@
         yaml_data = response.text
         data = yaml.safe_load(yaml_data)
     else:
         print("Failed to load YAML file.")
         exit(0)
 
     instruction = data["instruction"]
-    instruction = "Here are the instructions and some examples of conversations between me and you." + instruction
-    example_pairs = data["example_pairs"]
-    # some examples
-    instruction += " For example: " + str(example_pairs) + "." + " Now, let's start!"
-    properties = data["properties"]
+    instruction = "Instruction:" + instruction
+    if "example_pairs" in data.keys():
+        example_pairs = data["example_pairs"]
+        # some examples
+        instruction += " For example: " + str(example_pairs) + "." + " Now, let's start!"
+        properties = data["properties"]
 
     def fixed_format_ai_wrapper(prompt) -> dict:
         message = [{"role": "system", "content": instruction}]
         message.append({"role": "user", "content": prompt})
         function_name = "print_parameters"
         function_description = "print the generated result from assistant, including "
         for prop in properties:
```


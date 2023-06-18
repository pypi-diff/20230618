# Comparing `tmp/aifunc-0.5.5.tar.gz` & `tmp/aifunc-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.5.5.tar", max compression
+gzip compressed data, was "aifunc-0.5.6.tar", max compression
```

## Comparing `aifunc-0.5.5.tar` & `aifunc-0.5.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2023-06-17 22:58:36.361414 aifunc-0.5.5/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-17 15:48:26.010370 aifunc-0.5.5/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-17 15:48:26.010370 aifunc-0.5.5/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-17 15:48:26.010370 aifunc-0.5.5/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-17 15:48:26.010370 aifunc-0.5.5/aifunc/generate_question.py
--rw-r--r--   0        0        0    13613 2023-06-18 01:12:16.713927 aifunc-0.5.5/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-18 01:12:29.841759 aifunc-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-06-17 22:58:36.361414 aifunc-0.5.6/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-17 15:48:26.010370 aifunc-0.5.6/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-17 15:48:26.010370 aifunc-0.5.6/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-17 15:48:26.010370 aifunc-0.5.6/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-17 15:48:26.010370 aifunc-0.5.6/aifunc/generate_question.py
+-rw-r--r--   0        0        0    13590 2023-06-18 01:16:42.106401 aifunc-0.5.6/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-18 01:16:58.258179 aifunc-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.6/PKG-INFO
```

### Comparing `aifunc-0.5.5/aifunc/add_ai_function.py` & `aifunc-0.5.6/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.5.5/aifunc/utility.py` & `aifunc-0.5.6/aifunc/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         exit(0)
 
     instruction = data["instruction"]
     instruction = "Instruction:" + instruction
     if "example_pairs" in data.keys():
         example_pairs = data["example_pairs"]
         # some examples
-        instruction += " For example: " + str(example_pairs) + "." + " Now, let's start!"
+        instruction += " For example: " + str(example_pairs)
         properties = data["properties"]
 
     def fixed_format_ai_wrapper(prompt) -> dict:
         message = [{"role": "system", "content": instruction}]
         message.append({"role": "user", "content": prompt})
         function_name = "print_parameters"
         function_description = "print the generated result from assistant, including "
@@ -182,15 +182,15 @@
                     return arguments
                 else:
                     # print(response)
                     raise Exception("No function call.")
             except Exception as e:
                 # print(e)
                 print(f"Attempt {i} failed, retrying in 1 seconds...")
-                time.sleep(1)  # wait for 5 seconds before next attempt
+                time.sleep(0.1)  # wait for 5 seconds before next attempt
                 continue
         raise Exception(
             "Unable to execute fixed_format_ai_wrapper after 5 attempts.")
 
     return fixed_format_ai_wrapper
 
 
@@ -245,15 +245,15 @@
                     return arguments["array"]
                 else:
                     # print(response)
                     raise Exception("No function call.")
             except Exception as e:
                 # print(e)
                 print(f"Attempt {i} failed, retrying in 1 seconds...")
-                time.sleep(1)  # wait for 5 seconds before next attempt
+                time.sleep(0.1)  # wait for 5 seconds before next attempt
                 continue
         raise Exception(
             "Unable to execute fixed_format_ai_wrapper after 5 attempts.")
 
     return fixed_format_ai_wrapper
 
 
@@ -309,13 +309,13 @@
                 else:
                     # print(response)
                     raise Exception("No function call.")
             except Exception as e:
                 # print(response)
                 # print(e)
                 print(f"Attempt {i} failed, retrying in 1 seconds...")
-                time.sleep(1)  # wait for 5 seconds before next attempt
+                time.sleep(0.1)  # wait for 5 seconds before next attempt
                 continue
         raise Exception(
             "Unable to execute fixed_format_ai_wrapper after 5 attempts.")
 
     return fixed_format_ai_wrapper
```


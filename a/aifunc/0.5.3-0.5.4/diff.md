# Comparing `tmp/aifunc-0.5.3.tar.gz` & `tmp/aifunc-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.5.3.tar", max compression
+gzip compressed data, was "aifunc-0.5.4.tar", max compression
```

## Comparing `aifunc-0.5.3.tar` & `aifunc-0.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2023-06-17 22:58:36.361414 aifunc-0.5.3/aifunc/__init__.py
--rw-r--r--   0        0        0      725 2023-06-17 15:48:26.010370 aifunc-0.5.3/aifunc/add_ai_function.py
--rw-r--r--   0        0        0      371 2023-06-17 15:48:26.010370 aifunc-0.5.3/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0      228 2023-06-17 15:48:26.010370 aifunc-0.5.3/aifunc/follow_up.py
--rw-r--r--   0        0        0      126 2023-06-17 15:48:26.010370 aifunc-0.5.3/aifunc/generate_question.py
--rw-r--r--   0        0        0    13622 2023-06-18 00:11:18.560030 aifunc-0.5.3/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-18 00:12:36.618906 aifunc-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-06-17 22:58:36.361414 aifunc-0.5.4/aifunc/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-17 15:48:26.010370 aifunc-0.5.4/aifunc/add_ai_function.py
+-rw-r--r--   0        0        0      371 2023-06-17 15:48:26.010370 aifunc-0.5.4/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0      228 2023-06-17 15:48:26.010370 aifunc-0.5.4/aifunc/follow_up.py
+-rw-r--r--   0        0        0      126 2023-06-17 15:48:26.010370 aifunc-0.5.4/aifunc/generate_question.py
+-rw-r--r--   0        0        0    13626 2023-06-18 01:02:07.512755 aifunc-0.5.4/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-18 01:02:32.356354 aifunc-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.5.4/PKG-INFO
```

### Comparing `aifunc-0.5.3/aifunc/add_ai_function.py` & `aifunc-0.5.4/aifunc/add_ai_function.py`

 * *Files identical despite different names*

### Comparing `aifunc-0.5.3/aifunc/utility.py` & `aifunc-0.5.4/aifunc/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,16 +305,16 @@
                         # remove space if any
                         arguments["array"][i] = arguments["array"][i].strip()
                     return arguments["array"]
                 else:
                     # print(response)
                     raise Exception("No function call.")
             except Exception as e:
-                print(response)
-                print(e)
+                # print(response)
+                # print(e)
                 print(f"Attempt {i} failed, retrying in 1 seconds...")
                 time.sleep(1)  # wait for 5 seconds before next attempt
                 continue
         raise Exception(
             "Unable to execute fixed_format_ai_wrapper after 5 attempts.")
 
     return fixed_format_ai_wrapper
```


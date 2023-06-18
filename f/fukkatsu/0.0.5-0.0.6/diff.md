# Comparing `tmp/fukkatsu-0.0.5.tar.gz` & `tmp/fukkatsu-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fukkatsu-0.0.5.tar", last modified: Wed Jun 14 23:47:14 2023, max compression
+gzip compressed data, was "fukkatsu-0.0.6.tar", last modified: Sun Jun 18 20:19:23 2023, max compression
```

## Comparing `fukkatsu-0.0.5.tar` & `fukkatsu-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.528207 fukkatsu-0.0.5/
--rw-rw-rw-   0        0        0     1085 2023-06-14 23:28:09.000000 fukkatsu-0.0.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    12171 2023-06-14 23:47:14.528207 fukkatsu-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    11530 2023-06-13 23:47:46.000000 fukkatsu-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.455854 fukkatsu-0.0.5/fukkatsu/
--rw-rw-rw-   0        0        0    10304 2023-06-14 23:46:10.000000 fukkatsu-0.0.5/fukkatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.497509 fukkatsu-0.0.5/fukkatsu/memory/
--rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.5/fukkatsu/memory/__init__.py
--rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.5/fukkatsu/memory/manage.py
--rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.5/fukkatsu/memory/short.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.512552 fukkatsu-0.0.5/fukkatsu/utils/
--rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.5/fukkatsu/utils/__init__.py
--rw-rw-rw-   0        0        0     4082 2023-06-12 22:53:43.000000 fukkatsu-0.0.5/fukkatsu/utils/helper.py
--rw-rw-rw-   0        0        0     3061 2023-06-14 23:46:10.000000 fukkatsu-0.0.5/fukkatsu/utils/medic.py
--rw-rw-rw-   0        0        0     2779 2023-06-14 23:23:55.000000 fukkatsu-0.0.5/fukkatsu/utils/prompt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:47:14.486758 fukkatsu-0.0.5/fukkatsu.egg-info/
--rw-rw-rw-   0        0        0    12171 2023-06-14 23:47:13.000000 fukkatsu-0.0.5/fukkatsu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-06-14 23:47:14.000000 fukkatsu-0.0.5/fukkatsu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:47:13.000000 fukkatsu-0.0.5/fukkatsu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-14 23:47:13.000000 fukkatsu-0.0.5/fukkatsu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 23:47:13.000000 fukkatsu-0.0.5/fukkatsu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 23:47:14.528207 fukkatsu-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-06-14 23:44:47.000000 fukkatsu-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.956079 fukkatsu-0.0.6/
+-rw-rw-rw-   0        0        0     1319 2023-06-18 20:16:23.000000 fukkatsu-0.0.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2023-04-28 00:39:24.000000 fukkatsu-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 fukkatsu-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    12171 2023-06-18 20:19:23.949512 fukkatsu-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11530 2023-06-13 23:47:46.000000 fukkatsu-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.855746 fukkatsu-0.0.6/fukkatsu/
+-rw-rw-rw-   0        0        0    10417 2023-06-18 19:57:30.000000 fukkatsu-0.0.6/fukkatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.905830 fukkatsu-0.0.6/fukkatsu/memory/
+-rw-rw-rw-   0        0        0       75 2023-05-20 04:07:03.000000 fukkatsu-0.0.6/fukkatsu/memory/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-05-20 04:07:01.000000 fukkatsu-0.0.6/fukkatsu/memory/manage.py
+-rw-rw-rw-   0        0        0       23 2023-05-20 04:07:01.000000 fukkatsu-0.0.6/fukkatsu/memory/short.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.917845 fukkatsu-0.0.6/fukkatsu/observer/
+-rw-rw-rw-   0        0        0       40 2023-06-15 23:48:34.000000 fukkatsu-0.0.6/fukkatsu/observer/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-06-18 20:00:23.000000 fukkatsu-0.0.6/fukkatsu/observer/tracker.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.938999 fukkatsu-0.0.6/fukkatsu/utils/
+-rw-rw-rw-   0        0        0      110 2023-05-18 05:17:09.000000 fukkatsu-0.0.6/fukkatsu/utils/__init__.py
+-rw-rw-rw-   0        0        0     4082 2023-06-12 22:53:43.000000 fukkatsu-0.0.6/fukkatsu/utils/helper.py
+-rw-rw-rw-   0        0        0     3242 2023-06-18 19:57:30.000000 fukkatsu-0.0.6/fukkatsu/utils/medic.py
+-rw-rw-rw-   0        0        0     2779 2023-06-14 23:23:55.000000 fukkatsu-0.0.6/fukkatsu/utils/prompt.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:23.888836 fukkatsu-0.0.6/fukkatsu.egg-info/
+-rw-rw-rw-   0        0        0    12171 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 20:19:23.000000 fukkatsu-0.0.6/fukkatsu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 20:19:23.956079 fukkatsu-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-06-17 23:20:33.000000 fukkatsu-0.0.6/setup.py
```

### Comparing `fukkatsu-0.0.5/CHANGELOG.md` & `fukkatsu-0.0.6/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -24,8 +24,16 @@
 - changed the name of `extract_text_between_backticks` to `extract_text_between_pipes`
 - added additional functions for response sanitation in LLM: `standardize_delimiters` and `add_delimiters`, which handle edge case answers from LLM
 
 ### 0.0.5
 
 - added control arguments for OpenAi model and temperature
 - added `twin` for review capabilities
-- improved prompt clarity on code indicator tags `|||`
+- improved prompt clarity on code indicator tags `|||`
+
+### 0.0.6
+
+- short-term-memory fix
+    - short-term-memory will now only save functions that executed successfully
+- live counter fix
+    - removed unintended extra live
+- logging formatting enhanced + api call logging added
```

### Comparing `fukkatsu-0.0.5/LICENSE` & `fukkatsu-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.5/PKG-INFO` & `fukkatsu-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fukkatsu-0.0.5/README.md` & `fukkatsu-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.5/fukkatsu/__init__.py` & `fukkatsu-0.0.6/fukkatsu/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 import copy
 import functools
-import logging
 import traceback
 
 from fukkatsu.memory import SHORT_TERM_MEMORY
+from fukkatsu.observer.tracker import track
 from fukkatsu.utils import (check_and_install_libraries, extract_imports,
                             extract_text_between_pipes,
                             insert_string_after_colon, remove_trace_lines,
                             remove_wrapper_name, return_input_arguments,
                             return_source_code)
 from fukkatsu.utils.medic import defibrillate, enhance, twin
 
@@ -31,146 +31,153 @@
                 args_copy = copy.deepcopy(args)
                 kwargs_copy = copy.deepcopy(kwargs)
                 result = func(*args_copy, **kwargs_copy)
 
                 return result
 
             except Exception as e:
-                logging.exception(e)
+                track.exception(e)
                 trace = traceback.format_exc()
                 trace = remove_trace_lines(trace)
 
                 source = return_source_code(func)
                 source = remove_wrapper_name(source)
 
-                logging.warning(f"Input arguments: {input_args}\n")
-                logging.warning(f"\nSource Code: \n {source}\n")
+                track.warning(f"Input arguments: {input_args}\n")
+                track.warning(f"\nSource Code: \n {source}\n")
 
                 if trace in SHORT_TERM_MEMORY.keys():
-                    logging.warning("Correction already in-memory\n")
+                    track.warning("Correction already in-memory\n")
                     suggested_code = SHORT_TERM_MEMORY[trace]
-                    logging.warning(
+                    track.warning(
                         f"Using in-memory saved correction:\n{suggested_code}\n"
                     )
 
                 else:
-                    logging.warning("Requesting INITIAL correction\n")
+                    track.warning("Requesting INITIAL correction - Attempt 1\n")
                     suggested_code = defibrillate(
                         inputs=input_args,
                         faulty_function=source,
                         error_trace=trace,
                         model=llm["primary"],
                         temperature=temperature["primary"],
                         additional_req=additional_req,
                     )
-                    logging.warning(
+                    track.warning(
                         f"Received INITIAL RAW suggestion:\n{suggested_code}\n"
                     )
                     if active_twin == True:
-                        logging.warning("Requesting TWIN review\n")
+                        track.warning("Requesting TWIN review\n")
                         suggested_code = twin(
                             inputs=input_args,
                             target_function=suggested_code,
                             model=llm["secondary"],
                             temperature=temperature["secondary"],
                         )
-                        logging.warning(f"TWIN review complete:\n{suggested_code}")
+                        track.warning(f"TWIN review complete:\n{suggested_code}")
                     suggested_code = extract_text_between_pipes(suggested_code)
-                    logging.warning(
+                    track.warning(
                         f"Received INITIAL CLEANED suggestion:\n{suggested_code}\n"
                     )
 
                     import_block = extract_imports(suggested_code)
                     if allow_installs == True:
                         check_and_install_libraries(import_statements=import_block)
 
                     suggested_code = insert_string_after_colon(
                         suggested_code, import_block
                     )
-                    logging.warning(
+                    track.warning(
                         f"Import block added to suggested code:\n {suggested_code}\n"
                     )
 
                 for i in range(lives):
-                    logging.warning(f"Attempt {i+1} to reanimate\n")
+
+                    if i != lives - 1:
+                        track.warning(f"Attempt {i+2} to reanimate\n")
 
                     try:
                         global_dict = globals()
                         local_dict = locals()
 
                         compiled_code = compile(suggested_code, "<string>", "exec")
 
                         exec(compiled_code, global_dict, local_dict)
                         new_function = local_dict[func.__name__]
 
-                        SHORT_TERM_MEMORY[trace] = suggested_code
-                        logging.warning(
-                            f"Reanimation successful, using:\n{suggested_code}\n"
-                        )
                         locals()[func.__name__] = new_function
 
                         args_copy = copy.deepcopy(args)
                         kwargs_copy = copy.deepcopy(kwargs)
 
-                        return new_function(*args_copy, **kwargs_copy)
+                        output = new_function(*args_copy, **kwargs_copy)
+
+                        SHORT_TERM_MEMORY[trace] = suggested_code
+                        track.warning(
+                            f"Reanimation successful, using:\n{suggested_code}\n"
+                        )
+
+                        return output
+
+                    except Exception as e:
+                        track.exception(e)
+
+                        if i == lives - 1:
+                            break
 
-                    except:
-                        logging.exception(e)
                         trace = traceback.format_exc()
                         trace = remove_trace_lines(trace)
-                        logging.warning(
-                            "Reanimation failed, requesting new correction\n"
-                        )
+                        track.warning("Reanimation failed, requesting new correction\n")
 
                         if trace in SHORT_TERM_MEMORY.keys():
-                            logging.warning("Correction already in-memory\n")
+                            track.warning("Correction already in-memory\n")
                             suggested_code = SHORT_TERM_MEMORY[trace]
-                            logging.warning(
+                            track.warning(
                                 f"Using in-memory saved correction:\n{suggested_code}\n"
                             )
 
                         else:
                             suggested_code = defibrillate(
                                 inputs=input_args,
                                 faulty_function=suggested_code,
                                 error_trace=trace,
                                 model=llm["primary"],
                                 temperature=temperature["primary"],
                                 additional_req=additional_req,
                             )
-                            logging.warning(
+                            track.warning(
                                 f"Received attempt RAW suggestion:\n{suggested_code}\n"
                             )
 
                             if active_twin == True:
-                                logging.warning("Requesting TWIN review\n")
+                                track.warning("Requesting TWIN review\n")
                                 suggested_code = twin(
                                     inputs=input_args,
                                     target_function=suggested_code,
                                     model=llm["secondary"],
                                     temperature=temperature["secondary"],
                                 )
-                                logging.warning(
+                                track.warning(
                                     f"TWIN review complete:\n{suggested_code}"
                                 )
                             suggested_code = extract_text_between_pipes(suggested_code)
-                            logging.warning(
+                            track.warning(
                                 f"Received attempt CLEANED suggestion:\n{suggested_code}\n"
                             )
 
                             import_block = extract_imports(suggested_code)
                             if allow_installs == True:
                                 check_and_install_libraries(
                                     import_statements=import_block
                                 )
 
                             suggested_code = insert_string_after_colon(
                                 suggested_code, import_block
                             )
-                            logging.warning(
+                            track.warning(
                                 f"Import block added to suggested code:\n {suggested_code}\n"
                             )
 
                 raise Exception(f"|__|__|______ {func.__name__} flatlined")
 
         return wrapper
 
@@ -188,57 +195,58 @@
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
 
             input_args = return_input_arguments(func, *args, **kwargs)
             source = return_source_code(func)
             source = remove_wrapper_name(source)
 
-            logging.warning(f"Input arguments: {input_args}\n")
-            logging.warning(f"\nSource Code: \n {source}\n")
+            track.warning(f"Input arguments: {input_args}\n")
+            track.warning(f"\nSource Code: \n {source}\n")
 
-            logging.warning("Requesting mutation\n")
+            track.warning("Requesting mutation\n")
             suggested_code = enhance(
                 inputs=input_args,
                 target_function=source,
                 model=llm["primary"],
                 temperature=temperature["primary"],
                 request=request,
             )
-            logging.warning(f"Received RAW suggestion mutation:\n{suggested_code}\n")
+            track.warning(f"Received RAW suggestion mutation:\n{suggested_code}\n")
 
             if active_twin == True:
-                logging.warning("Requesting TWIN review:\n")
+                track.warning("Requesting TWIN review:\n")
                 suggested_code = twin(
                     inputs=input_args,
                     target_function=suggested_code,
                     model=llm["secondary"],
                     temperature=temperature["secondary"],
                 )
-                logging.warning(f"TWIN review complete:\n{suggested_code}")
+                track.warning(f"TWIN review complete:\n{suggested_code}")
             suggested_code = extract_text_between_pipes(suggested_code)
-            logging.warning(f"Received CLEANED suggestion mutation: {suggested_code}\n")
+            track.warning(f"Received CLEANED suggestion mutation: {suggested_code}\n")
 
             global_dict = globals()
             local_dict = locals()
 
             import_block = extract_imports(suggested_code)
             if allow_installs == True:
                 check_and_install_libraries(import_statements=import_block)
 
             suggested_code = insert_string_after_colon(suggested_code, import_block)
-            logging.warning(
-                f"Import block added to suggested code:\n {suggested_code}\n"
-            )
+            track.warning(f"Import block added to suggested code:\n {suggested_code}\n")
 
             compiled_code = compile(suggested_code, "<string>", "exec")
 
             exec(compiled_code, global_dict, local_dict)
             new_function = local_dict[func.__name__]
 
-            logging.warning(f"Mutation successful, using {suggested_code}\n")
             locals()[func.__name__] = new_function
 
-            return new_function(*args, **kwargs)
+            output = new_function(*args, **kwargs)
+
+            track.warning(f"Mutation successful, using {suggested_code}\n")
+
+            return output
 
         return wrapper
 
     return _mutate
```

### Comparing `fukkatsu-0.0.5/fukkatsu/memory/manage.py` & `fukkatsu-0.0.6/fukkatsu/memory/manage.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.5/fukkatsu/utils/helper.py` & `fukkatsu-0.0.6/fukkatsu/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.5/fukkatsu/utils/medic.py` & `fukkatsu-0.0.6/fukkatsu/utils/medic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 import openai
 
+from fukkatsu.observer.tracker import track
 from fukkatsu.utils.prompt import (ADDITIONAL, CONTEXT, CONTEXT_MUTATE,
                                    CONTEXT_TWIN, OUTPUT_CONSTRAINTS,
                                    OUTPUT_CONSTRAINTS_MUTATE,
                                    OUTPUT_CONSTRAINTS_TWIN)
 
 try:
     openai.api_key = os.environ.get("OPENAI_API_KEY")
@@ -30,15 +31,15 @@
         )
     else:
         set_prompt = (
             f"{CONTEXT}\n\n{faulty_function}\n\nThe function received the following inputs:\n\n"
             f"{inputs}\n\nAnd returned the following error trace:\n\n{error_trace}\n\n{OUTPUT_CONSTRAINTS}\n"
             f"{ADDITIONAL}{additional_req}"
         )
-
+    track.warning(f"API REQUEST to {model}")
     response = openai.ChatCompletion.create(
         model=model,
         messages=[
             {"role": "system", "content": set_prompt},
         ],
         max_tokens=1024,
         n=1,
@@ -55,14 +56,15 @@
     inputs: str, target_function: str, model: str, temperature: float, request: str = ""
 ) -> str:
     set_prompt = (
         f"{CONTEXT_MUTATE}\n\n{target_function}\n\nThe function received the following inputs:\n\n"
         f"{inputs}\n\nThe user requests the following:\n{request}\n{OUTPUT_CONSTRAINTS_MUTATE}"
     )
 
+    track.warning(f"API REQUEST to {model}")
     response = openai.ChatCompletion.create(
         model=model,
         messages=[
             {"role": "system", "content": set_prompt},
         ],
         max_tokens=1024,
         n=1,
@@ -82,14 +84,15 @@
     temperature: float,
 ) -> str:
     set_prompt = (
         f"{CONTEXT_TWIN}\n\n{target_function}\n\nThe function received the following inputs:\n\n"
         f"{inputs}\n\n{OUTPUT_CONSTRAINTS_TWIN}"
     )
 
+    track.warning(f"API REQUEST to {model}")
     response = openai.ChatCompletion.create(
         model=model,
         messages=[
             {"role": "system", "content": set_prompt},
         ],
         max_tokens=1024,
         n=1,
```

### Comparing `fukkatsu-0.0.5/fukkatsu/utils/prompt.py` & `fukkatsu-0.0.6/fukkatsu/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `fukkatsu-0.0.5/fukkatsu.egg-info/PKG-INFO` & `fukkatsu-0.0.6/fukkatsu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fukkatsu
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python library for runtime LLM supported code corrections.
 Home-page: https://github.com/maxmekiska/fukkatsu
 Author: Maximilian Mekiska
 Author-email: maxmekiska@gmail.com
 Keywords: machinelearning,llm,runtime,codecorrection
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `fukkatsu-0.0.5/setup.py` & `fukkatsu-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/fukkatsu",
     description="A python library for runtime LLM supported code corrections.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="fukkatsu",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(include=["fukkatsu", "fukkatsu.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "openai >= 0.27.5, <= 0.28",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
```


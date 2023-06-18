# Comparing `tmp/heygptcli-0.1.1.tar.gz` & `tmp/heygptcli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heygptcli-0.1.1.tar", max compression
+gzip compressed data, was "heygptcli-0.1.2.tar", max compression
```

## Comparing `heygptcli-0.1.1.tar` & `heygptcli-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-16 18:46:16.771883 heygptcli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/__init__.py
--rw-r--r--   0        0        0      717 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/api.py
--rwxr-xr-x   0        0        0     4840 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/cli.py
--rw-r--r--   0        0        0     2249 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/constant.py
--rw-r--r--   0        0        0     2804 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/core.py
--rw-r--r--   0        0        0     1897 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/serve.py
--rw-r--r--   0        0        0      153 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/serve_prompts.py
--rw-r--r--   0        0        0      849 2023-06-16 18:46:16.771883 heygptcli-0.1.1/heygpt/utils.py
--rw-r--r--   0        0        0      677 2023-06-16 18:46:16.771883 heygptcli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-18 11:19:57.231599 heygptcli-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/__init__.py
+-rw-r--r--   0        0        0      717 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/api.py
+-rwxr-xr-x   0        0        0     4804 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/cli.py
+-rw-r--r--   0        0        0     2249 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/constant.py
+-rw-r--r--   0        0        0     2804 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/core.py
+-rw-r--r--   0        0        0     1897 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/serve.py
+-rw-r--r--   0        0        0      153 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/serve_prompts.py
+-rw-r--r--   0        0        0      849 2023-06-18 11:19:57.231599 heygptcli-0.1.2/heygpt/utils.py
+-rw-r--r--   0        0        0      677 2023-06-18 11:19:57.231599 heygptcli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.2/PKG-INFO
```

### Comparing `heygptcli-0.1.1/heygpt/api.py` & `heygptcli-0.1.2/heygpt/api.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.1/heygpt/cli.py` & `heygptcli-0.1.2/heygpt/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,25 +35,25 @@
     no_prompt: bool = typer.Option(
         False, "--no-prompt", "-n", help="Ask without anyprompt templates."
     ),
     text: str = typer.Option(
         str, help="Optional provide text query as an input argument."
     ),
     tag: Annotated[Optional[List[str]], typer.Option()] = [],
-    save: bool = typer.Option(
-        False, "--output", "-o", help="save output to file availabe formats: md"
+    save: str = typer.Option(
+        "", "--output", "-o", help="save output to file availabe formats: md"
     ),
 ):
     tags: str = " #".join(tag)
     command: str = ""
 
     # print(tags)
     # return
-    prompts = load_promps(prompt_items_url)
     if not no_prompt:
+        prompts = load_promps(prompt_items_url)
         log.debug(prompts)
         prompts_title = [i.Title for i in prompts]
         try:
             act = sh('echo "' + "\n".join(prompts_title) + '" | fzf -e').strip()
             if act == "":
                 raise Exception("maybe fzf not present on system")
         except Exception as e:
@@ -90,19 +90,18 @@
         content = completion_bard(command=command, text=text, _print=True)
     else:
         completion = completion_openai_gpt(command=command, text=text, _print=True)
         content = completion
 
     # typer.echo("\n---------- output ----------\n")
 
-    if save:
-        file_name = "output.md"
-        with open(f"{file_name}", "w") as f:
+    if save != "":
+        with open(f"{save}", "w") as f:
             f.write(content)
-        rich.print(f"\n\nINFO: Output saved to: {file_name}")
+        rich.print(f"\n\nINFO: Output saved to: {save}")
 
 
 @app.command(help="Generate new prompts.")
 def create_prompt(text):
     data = make_prompt(text)
 
     rich.print(data["generated_text"])
```

### Comparing `heygptcli-0.1.1/heygpt/constant.py` & `heygptcli-0.1.2/heygpt/constant.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.1/heygpt/core.py` & `heygptcli-0.1.2/heygpt/core.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.1/heygpt/serve.py` & `heygptcli-0.1.2/heygpt/serve.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.1/heygpt/utils.py` & `heygptcli-0.1.2/heygpt/utils.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.1/pyproject.toml` & `heygptcli-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "heygptcli"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Rishang <rishang@localhost.com>"]
 readme = "README.md"
 packages = [
   { include = "heygpt" }
 ]
 
 [tool.poetry.scripts]
 heygpt = "heygpt.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
-fastapi = "^0.95.2"
+fastapi = "^0.97.0"
 uvicorn = "^0.22.0"
 typer = "^0.9.0"
 python-dotenv = "^1.0.0"
 bardapi = "^0.1.11"
 openai = "^0.27.8"
 rich = "^13.4.1"
 prompt-toolkit = "^3.0.38"
```

### Comparing `heygptcli-0.1.1/PKG-INFO` & `heygptcli-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: heygptcli
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Rishang
 Author-email: rishang@localhost.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bardapi (>=0.1.11,<0.2.0)
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
+Requires-Dist: fastapi (>=0.97.0,<0.98.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: streamlit (>=1.23.1,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```


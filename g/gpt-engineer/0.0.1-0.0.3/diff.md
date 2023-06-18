# Comparing `tmp/gpt-engineer-0.0.1.tar.gz` & `tmp/gpt-engineer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-engineer-0.0.1.tar", last modified: Sun Jun 18 13:39:52 2023, max compression
+gzip compressed data, was "gpt-engineer-0.0.3.tar", last modified: Sun Jun 18 21:33:56 2023, max compression
```

## Comparing `gpt-engineer-0.0.1.tar` & `gpt-engineer-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:39:52.403164 gpt-engineer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-18 13:39:52.403164 gpt-engineer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:39:52.399164 gpt-engineer-0.0.1/gpt_engineer/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/gpt_engineer/ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/gpt_engineer/chat_to_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/gpt_engineer/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/gpt_engineer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/gpt_engineer/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:39:52.403164 gpt-engineer-0.0.1/gpt_engineer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-18 13:39:52.000000 gpt-engineer-0.0.1/gpt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-18 13:39:52.000000 gpt-engineer-0.0.1/gpt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:39:52.000000 gpt-engineer-0.0.1/gpt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 13:39:52.000000 gpt-engineer-0.0.1/gpt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-18 13:39:52.000000 gpt-engineer-0.0.1/gpt_engineer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 13:39:52.000000 gpt-engineer-0.0.1/gpt_engineer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 13:39:52.403164 gpt-engineer-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:39:52.403164 gpt-engineer-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/tests/test_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-18 13:39:42.000000 gpt-engineer-0.0.1/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:33:56.700646 gpt-engineer-0.0.3/gpt_engineer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/gpt_engineer/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/gpt_engineer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 21:33:56.000000 gpt-engineer-0.0.3/gpt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:33:56.704646 gpt-engineer-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/tests/test_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-18 21:33:43.000000 gpt-engineer-0.0.3/tests/test_db.py
```

### Comparing `gpt-engineer-0.0.1/LICENSE` & `gpt-engineer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.1/PKG-INFO` & `gpt-engineer-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-engineer
-Version: 0.0.1
-Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
-Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
-Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GPT Engineer
 **Specify what you want it to build, the AI asks for clarification, and then builds it.**
 
 GPT Engineer is made to be easy to adapt, extend, and make your agent learn how you want your code to look. It generates an entire codebase based on a prompt.
 
 [Demo](https://twitter.com/antonosika/status/1667641038104674306) 👶🤖
 
@@ -20,29 +10,43 @@
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-
 ## Usage
 
-**Setup**:
-- `pip install -r requirements.txt`
-- `export OPENAI_API_KEY=[your api key]` with a key that has GPT4 access
+Choose either **stable** or **development**.
+
+For **stable** release:
+
+- `pip install gpt-engineer`
+
+For **development**:
+- `git clone git@github.com:AntonOsika/gpt-engineer.git`
+- `cd gpt-engineer`
+- `make install`
+- `source venv/bin/activate`
+
+**Setup**
+
+With an api key that has GPT4 access run:
+
+- `export OPENAI_API_KEY=[your api key]`
+
 
 **Run**:
-- Create a new empty folder with a `main_prompt` file in the `projects` folder (or copy the example folder `cp -r projects/example/ projects/my-new-project`)
-- Fill in the `main_prompt` in your new folder
-- Run `python -m gpt_engineer.main my-new-project`
-  - Optionally pass in `true` to delete the working files before running
+- Create an empty folder. If inside the repo, you can run:
+  - `cp -r projects/example/ projects/my-new-project`
+- Fill in the `main_prompt` file in your new folder
+- Run: `gpt-engineer projects/my-new-project`
 
-**Results**:
-- Check the generated files in projects/my-new-project/workspace
+**Results**
+- Check the generated files in `projects/my-new-project/workspace`
 
 ### Limitations
 Implementing additional chain of thought prompting, e.g. [Reflexion](https://github.com/noahshinn024/reflexion), should be able to make it more reliable and not miss requested functionality in the main prompt.
 
 Contributors welcome! If you are unsure what to add, check out the ideas listed in the Projects tab in the GitHub repo.
```

### Comparing `gpt-engineer-0.0.1/README.md` & `gpt-engineer-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: gpt-engineer
+Version: 0.0.3
+Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
+Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
+Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # GPT Engineer
 **Specify what you want it to build, the AI asks for clarification, and then builds it.**
 
 GPT Engineer is made to be easy to adapt, extend, and make your agent learn how you want your code to look. It generates an entire codebase based on a prompt.
 
 [Demo](https://twitter.com/antonosika/status/1667641038104674306) 👶🤖
 
@@ -10,29 +20,43 @@
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-
 ## Usage
 
-**Setup**:
-- `pip install -r requirements.txt`
-- `export OPENAI_API_KEY=[your api key]` with a key that has GPT4 access
+Choose either **stable** or **development**.
+
+For **stable** release:
+
+- `pip install gpt-engineer`
+
+For **development**:
+- `git clone git@github.com:AntonOsika/gpt-engineer.git`
+- `cd gpt-engineer`
+- `make install`
+- `source venv/bin/activate`
+
+**Setup**
+
+With an api key that has GPT4 access run:
+
+- `export OPENAI_API_KEY=[your api key]`
+
 
 **Run**:
-- Create a new empty folder with a `main_prompt` file in the `projects` folder (or copy the example folder `cp -r projects/example/ projects/my-new-project`)
-- Fill in the `main_prompt` in your new folder
-- Run `python -m gpt_engineer.main my-new-project`
-  - Optionally pass in `true` to delete the working files before running
+- Create an empty folder. If inside the repo, you can run:
+  - `cp -r projects/example/ projects/my-new-project`
+- Fill in the `main_prompt` file in your new folder
+- Run: `gpt-engineer projects/my-new-project`
 
-**Results**:
-- Check the generated files in projects/my-new-project/workspace
+**Results**
+- Check the generated files in `projects/my-new-project/workspace`
 
 ### Limitations
 Implementing additional chain of thought prompting, e.g. [Reflexion](https://github.com/noahshinn024/reflexion), should be able to make it more reliable and not miss requested functionality in the main prompt.
 
 Contributors welcome! If you are unsure what to add, check out the ideas listed in the Projects tab in the GitHub repo.
```

### Comparing `gpt-engineer-0.0.1/gpt_engineer/ai.py` & `gpt-engineer-0.0.3/gpt_engineer/ai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+import logging
+
 import openai
 
+logger = logging.getLogger(__name__)
+
 
 class AI:
-    def __init__(self, **kwargs):
-        self.kwargs = kwargs
+    def __init__(self, model="gpt-4", temperature=0.1):
+        self.temperature = temperature
 
         try:
-            openai.Model.retrieve("gpt-4")
-        except openai.error.InvalidRequestError:
+            openai.Model.retrieve(model)
+            self.model = model
+        except openai.InvalidRequestError:
             print(
-                "Model gpt-4 not available for provided api key reverting "
-                "to gpt-3.5.turbo. Sign up for the gpt-4 wait list here: "
+                f"Model {model} not available for provided API key. Reverting "
+                "to gpt-3.5-turbo. Sign up for the GPT-4 wait list here: "
                 "https://openai.com/waitlist/gpt-4-api"
             )
-            self.kwargs["model"] = "gpt-3.5-turbo"
+            self.model = "gpt-3.5-turbo"
 
     def start(self, system, user):
         messages = [
             {"role": "system", "content": system},
             {"role": "user", "content": user},
         ]
 
@@ -32,18 +37,25 @@
     def fassistant(self, msg):
         return {"role": "assistant", "content": msg}
 
     def next(self, messages: list[dict[str, str]], prompt=None):
         if prompt:
             messages = messages + [{"role": "user", "content": prompt}]
 
+        logger.debug(f"Creating a new chat completion: {messages}")
         response = openai.ChatCompletion.create(
-            messages=messages, stream=True, **self.kwargs
+            messages=messages,
+            stream=True,
+            model=self.model,
+            temperature=self.temperature,
         )
 
         chat = []
         for chunk in response:
             delta = chunk["choices"][0]["delta"]
             msg = delta.get("content", "")
             print(msg, end="")
             chat.append(msg)
-        return messages + [{"role": "assistant", "content": "".join(chat)}]
+        print()
+        messages = messages + [{"role": "assistant", "content": "".join(chat)}]
+        logger.debug(f"Chat completion finished: {messages}")
+        return messages
```

### Comparing `gpt-engineer-0.0.1/gpt_engineer/main.py` & `gpt-engineer-0.0.3/gpt_engineer/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 import json
+import logging
 import os
-import pathlib
 import shutil
 
+from pathlib import Path
+
 import typer
 
 from gpt_engineer.ai import AI
 from gpt_engineer.db import DB, DBs
 from gpt_engineer.steps import STEPS
 
 app = typer.Typer()
 
 
 @app.command()
-def chat(
+def main(
     project_path: str = typer.Argument("example", help="path"),
-    delete_existing: str = typer.Argument(None, help="delete existing files"),
+    delete_existing: bool = typer.Argument(False, help="delete existing files"),
+    model: str = "gpt-4",
+    temperature: float = 0.1,
+    steps_config: str = "default",
+    verbose: bool = typer.Option(False, "--verbose", "-v"),
     run_prefix: str = typer.Option(
         "",
         help=(
             "run prefix, if you want to run multiple variants of the same project and "
             "later compare them"
         ),
     ),
-    model: str = "gpt-4",
-    temperature: float = 0.1,
-    steps_config: str = "default",
 ):
-    app_dir = pathlib.Path(os.path.curdir)
-    input_path = pathlib.Path(app_dir / "projects" / project_path)
+    logging.basicConfig(level=logging.DEBUG if verbose else logging.INFO)
+
+    input_path = Path(project_path).absolute()
     memory_path = input_path / (run_prefix + "memory")
     workspace_path = input_path / (run_prefix + "workspace")
 
-    if delete_existing == "true":
+    if delete_existing:
         # Delete files and subdirectories in paths
         shutil.rmtree(memory_path, ignore_errors=True)
         shutil.rmtree(workspace_path, ignore_errors=True)
 
     ai = AI(
         model=model,
         temperature=temperature,
     )
 
     dbs = DBs(
         memory=DB(memory_path),
         logs=DB(memory_path / "logs"),
         input=DB(input_path),
         workspace=DB(workspace_path),
-        identity=DB(app_dir / "identity"),
+        identity=DB(Path(os.path.curdir) / "identity"),
     )
 
     for step in STEPS[steps_config]:
         messages = step(ai, dbs)
         dbs.logs[step.__name__] = json.dumps(messages)
```

### Comparing `gpt-engineer-0.0.1/gpt_engineer/steps.py` & `gpt-engineer-0.0.3/gpt_engineer/steps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
+import re
 import subprocess
 
 from gpt_engineer.ai import AI
-from gpt_engineer.chat_to_files import parse_chat, to_files
+from gpt_engineer.chat_to_files import to_files
 from gpt_engineer.db import DBs
 
 
 def setup_sys_prompt(dbs):
     return dbs.identity["generate"] + "\nUseful to know:\n" + dbs.identity["philosophy"]
 
 
@@ -153,35 +154,29 @@
     return []
 
 
 def gen_entrypoint(ai, dbs):
     messages = ai.start(
         system=(
             "You will get information about a codebase that is currently on disk in "
-            f"the folder {dbs.workspace.path}.\n"
+            "the current folder.\n"
             "From this you will answer with code blocks that includes all the necessary "
-            "Windows, MacOS, and Linux terminal commands to "
+            "unix terminal commands to "
             "a) install dependencies "
             "b) run all necessary parts of the codebase (in parallell if necessary).\n"
             "Do not install globally. Do not use sudo.\n"
             "Do not explain the code, just give the commands.\n"
         ),
         user="Information about the codebase:\n\n" + dbs.workspace["all_output.txt"],
     )
     print()
 
-    blocks = parse_chat(messages[-1]["content"])
-    for lang, _ in blocks:
-        assert lang in [
-            "",
-            "bash",
-            "sh",
-        ], "Generated entrypoint command that was not bash"
-
-    dbs.workspace["run.sh"] = "\n".join(block for lang, block in blocks)
+    regex = r"```\S*\n(.+?)```"
+    matches = re.finditer(regex, messages[-1]["content"], re.DOTALL)
+    dbs.workspace["run.sh"] = "\n".join(match.group(1) for match in matches)
     return messages
 
 
 def use_feedback(ai: AI, dbs: DBs):
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
         ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
@@ -189,18 +184,31 @@
         ai.fsystem(dbs.identity["use_feedback"]),
     ]
     messages = ai.next(messages, dbs.memory["feedback"])
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
+def fix_code(ai: AI, dbs: DBs):
+    code_ouput = json.loads(dbs.logs[gen_code.__name__])[-1]["content"]
+    messages = [
+        ai.fsystem(setup_sys_prompt(dbs)),
+        ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
+        ai.fuser(code_ouput),
+        ai.fsystem(dbs.identity["fix_code"]),
+    ]
+    messages = ai.next(messages, "Please fix any errors in the code above.")
+    to_files(messages[-1]["content"], dbs.workspace)
+    return messages
+
+
 # Different configs of what steps to run
 STEPS = {
     "default": [gen_spec, gen_unit_tests, gen_code, gen_entrypoint, execute_entrypoint],
-    "benchmark": [gen_spec, gen_unit_tests, gen_code, gen_entrypoint],
+    "benchmark": [gen_spec, gen_unit_tests, gen_code, fix_code, gen_entrypoint],
     "simple": [simple_gen, gen_entrypoint, execute_entrypoint],
     "clarify": [clarify, gen_clarified_code, gen_entrypoint, execute_entrypoint],
     "respec": [
         gen_spec,
         respec,
         gen_unit_tests,
         gen_code,
```

### Comparing `gpt-engineer-0.0.1/gpt_engineer.egg-info/PKG-INFO` & `gpt-engineer-0.0.3/gpt_engineer.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.1
+Version: 0.0.3
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,29 +20,43 @@
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-
 ## Usage
 
-**Setup**:
-- `pip install -r requirements.txt`
-- `export OPENAI_API_KEY=[your api key]` with a key that has GPT4 access
+Choose either **stable** or **development**.
+
+For **stable** release:
+
+- `pip install gpt-engineer`
+
+For **development**:
+- `git clone git@github.com:AntonOsika/gpt-engineer.git`
+- `cd gpt-engineer`
+- `make install`
+- `source venv/bin/activate`
+
+**Setup**
+
+With an api key that has GPT4 access run:
+
+- `export OPENAI_API_KEY=[your api key]`
+
 
 **Run**:
-- Create a new empty folder with a `main_prompt` file in the `projects` folder (or copy the example folder `cp -r projects/example/ projects/my-new-project`)
-- Fill in the `main_prompt` in your new folder
-- Run `python -m gpt_engineer.main my-new-project`
-  - Optionally pass in `true` to delete the working files before running
+- Create an empty folder. If inside the repo, you can run:
+  - `cp -r projects/example/ projects/my-new-project`
+- Fill in the `main_prompt` file in your new folder
+- Run: `gpt-engineer projects/my-new-project`
 
-**Results**:
-- Check the generated files in projects/my-new-project/workspace
+**Results**
+- Check the generated files in `projects/my-new-project/workspace`
 
 ### Limitations
 Implementing additional chain of thought prompting, e.g. [Reflexion](https://github.com/noahshinn024/reflexion), should be able to make it more reliable and not miss requested functionality in the main prompt.
 
 Contributors welcome! If you are unsure what to add, check out the ideas listed in the Projects tab in the GitHub repo.
```

### Comparing `gpt-engineer-0.0.1/pyproject.toml` & `gpt-engineer-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "gpt-engineer"
-version = "0.0.1"
+version = "0.0.3"
 description = "Specify what you want it to build, the AI asks for clarification, and then builds it."
 readme = "README.md"
 requires-python = ">=3"
 dependencies = [
   'black == 23.3.0',
   'openai == 0.27.8',
   'ruff == 0.0.272',
```


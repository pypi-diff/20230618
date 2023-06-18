# Comparing `tmp/kube_copilot-0.1.8.tar.gz` & `tmp/kube_copilot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kube_copilot-0.1.8.tar", max compression
+gzip compressed data, was "kube_copilot-0.1.9.tar", max compression
```

## Comparing `kube_copilot-0.1.8.tar` & `kube_copilot-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-03-25 09:21:30.419382 kube_copilot-0.1.8/LICENSE
--rw-r--r--   0        0        0     3727 2023-05-15 12:57:51.606979 kube_copilot-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-25 09:21:38.259064 kube_copilot-0.1.8/kube_copilot/__init__.py
--rw-r--r--   0        0        0     2759 2023-05-15 12:57:51.607506 kube_copilot-0.1.8/kube_copilot/agent.py
--rw-r--r--   0        0        0     2275 2023-05-15 12:57:51.607927 kube_copilot-0.1.8/kube_copilot/cli.py
--rw-r--r--   0        0        0      671 2023-03-25 10:47:12.857795 kube_copilot-0.1.8/kube_copilot/llm.py
--rw-r--r--   0        0        0     3166 2023-05-15 12:57:51.608488 kube_copilot-0.1.8/kube_copilot/prompts.py
--rw-r--r--   0        0        0     2022 2023-03-30 03:11:54.460130 kube_copilot-0.1.8/kube_copilot/shell.py
--rw-r--r--   0        0        0      747 2023-05-15 12:57:51.610774 kube_copilot-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 kube_copilot-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-25 09:21:30.419382 kube_copilot-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3727 2023-05-15 12:57:51.606979 kube_copilot-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 09:21:38.259064 kube_copilot-0.1.9/kube_copilot/__init__.py
+-rw-r--r--   0        0        0     2846 2023-05-29 14:55:42.856683 kube_copilot-0.1.9/kube_copilot/agent.py
+-rw-r--r--   0        0        0     2275 2023-05-15 12:57:51.607927 kube_copilot-0.1.9/kube_copilot/cli.py
+-rw-r--r--   0        0        0      663 2023-05-29 14:24:09.414057 kube_copilot-0.1.9/kube_copilot/llm.py
+-rw-r--r--   0        0        0     4434 2023-05-29 14:55:14.059978 kube_copilot-0.1.9/kube_copilot/prompts.py
+-rw-r--r--   0        0        0     2022 2023-03-30 03:11:54.460130 kube_copilot-0.1.9/kube_copilot/shell.py
+-rw-r--r--   0        0        0      747 2023-05-29 15:02:04.837277 kube_copilot-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 kube_copilot-0.1.9/PKG-INFO
```

### Comparing `kube_copilot-0.1.8/LICENSE` & `kube_copilot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.8/README.md` & `kube_copilot-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.8/kube_copilot/agent.py` & `kube_copilot-0.1.9/kube_copilot/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import os
 from langchain.chat_models import ChatOpenAI
 from langchain.agents import Tool
 from langchain.utilities import GoogleSearchAPIWrapper
 from langchain.experimental.plan_and_execute import PlanAndExecute, load_agent_executor, load_chat_planner
 from kube_copilot.shell import KubeProcess
-
+from kube_copilot.prompts import get_planner_prompt
 
 class CopilotLLM:
     '''Wrapper for LLM chain.'''
 
     def __init__(self, verbose=True, model="gpt-4", additional_tools=None):
         '''Initialize the LLM chain.'''
         self.chain = get_chat_chain(
@@ -33,15 +33,15 @@
     if os.getenv("OPENAI_API_TYPE") == "azure":
         engine = model.replace(".", "")
         llm = ChatOpenAI(model_name=model, temperature=0,
                          model_kwargs={"engine": engine})
     else:
         llm = ChatOpenAI(model_name=model, temperature=0)
 
-    planner = load_chat_planner(llm=llm)
+    planner = load_chat_planner(llm=llm, system_prompt=get_planner_prompt())
     tools = [
         Tool(
             name="kubectl",
             description="Useful for executing kubectl command to query information from kubernetes cluster. Input: a kubectl get command. Output: the yaml for the resource.",
             func=KubeProcess(command="kubectl").run,
         ),
         Tool(
@@ -63,8 +63,8 @@
             )
         ]
 
     if additional_tools is not None:
         tools += additional_tools
 
     executor = load_agent_executor(llm, tools, verbose=verbose)
-    return PlanAndExecute(planner=planner, executer=executor, verbose=verbose)
+    return PlanAndExecute(planner=planner, executor=executor, verbose=verbose)
```

### Comparing `kube_copilot-0.1.8/kube_copilot/cli.py` & `kube_copilot-0.1.9/kube_copilot/cli.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.8/kube_copilot/llm.py` & `kube_copilot-0.1.9/kube_copilot/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,12 +10,12 @@
     """
     if os.getenv("OPENAI_API_KEY") == "":
         raise Exception("Please set OPENAI_API_KEY via environment variable")
 
     if os.getenv("OPENAI_API_TYPE") == "azure":
         openai.api_type = "azure"
         openai.api_base = os.getenv("OPENAI_API_BASE")
-        openai.api_version = "2023-03-15-preview"
+        openai.api_version = "2023-05-15"
         openai.api_key = os.getenv("OPENAI_API_KEY")
     else:
         openai.api_key = os.getenv("OPENAI_API_KEY")
         openai.api_base = "https://api.openai.com/v1"
```

### Comparing `kube_copilot-0.1.8/kube_copilot/shell.py` & `kube_copilot-0.1.9/kube_copilot/shell.py`

 * *Files identical despite different names*

### Comparing `kube_copilot-0.1.8/pyproject.toml` & `kube_copilot-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kube-copilot"
-version = "0.1.8"
+version = "0.1.9"
 description = "Kubernetes Copilot"
 authors = ["Pengfei Ni <feiskyer@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kube_copilot"}]
 homepage = "https://github.com/feiskyer/kube-copilot"
 repository = "https://github.com/feiskyer/kube-copilot"
 keywords = ["kubernetes", "copilot", "openai", "chatgpt"]
```

### Comparing `kube_copilot-0.1.8/PKG-INFO` & `kube_copilot-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-copilot
-Version: 0.1.8
+Version: 0.1.9
 Summary: Kubernetes Copilot
 Home-page: https://github.com/feiskyer/kube-copilot
 Keywords: kubernetes,copilot,openai,chatgpt
 Author: Pengfei Ni
 Author-email: feiskyer@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
```


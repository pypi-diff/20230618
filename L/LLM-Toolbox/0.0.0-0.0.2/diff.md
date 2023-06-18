# Comparing `tmp/llm-toolbox-0.0.0.tar.gz` & `tmp/LLM-Toolbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-toolbox-0.0.0.tar", last modified: Fri Jun 16 16:42:25 2023, max compression
+gzip compressed data, was "LLM-Toolbox-0.0.2.tar", last modified: Sun Jun 18 19:23:17 2023, max compression
```

## Comparing `llm-toolbox-0.0.0.tar` & `LLM-Toolbox-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,53 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-16 16:42:25.198938 llm-toolbox-0.0.0/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 llm-toolbox-0.0.0/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3381 2023-06-16 16:42:25.198938 llm-toolbox-0.0.0/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3248 2023-06-16 16:29:28.000000 llm-toolbox-0.0.0/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-16 16:42:25.198938 llm-toolbox-0.0.0/llm_toolbox.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3381 2023-06-16 16:42:25.000000 llm-toolbox-0.0.0/llm_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      166 2023-06-16 16:42:25.000000 llm-toolbox-0.0.0/llm_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-16 16:42:25.000000 llm-toolbox-0.0.0/llm_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-16 16:42:25.000000 llm-toolbox-0.0.0/llm_toolbox.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-16 16:42:25.198938 llm-toolbox-0.0.0/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      262 2023-06-16 16:34:28.000000 llm-toolbox-0.0.0/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 08:04:31.000000 LLM-Toolbox-0.0.2/LICENSE
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11013 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1547 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      670 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1026 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-18 19:23:17.000000 LLM-Toolbox-0.0.2/LLM_Toolbox.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11013 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10475 2023-06-18 18:54:17.000000 LLM-Toolbox-0.0.2/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/llm_toolbox/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10678 2023-06-18 19:17:13.000000 LLM-Toolbox-0.0.2/llm_toolbox/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/llm_toolbox/tools/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/common.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      368 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      594 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      854 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      576 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      270 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      332 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      748 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      533 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      423 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      453 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      393 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      818 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      248 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      364 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/templates/translate.yaml
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/llm_toolbox/tools/user_defined/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/user_defined/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/llm_toolbox/tools/user_defined/example_tool.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/prompt_templates/
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/prompt_templates/tools/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      368 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/cheermeup.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      594 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/codereview.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      854 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/commitgen.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      576 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/critique.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      270 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/define.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      332 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/explain.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      748 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/lessonize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      533 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/pathlearner.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      423 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/proofread.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      453 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/study.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      393 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/summarize.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      818 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/teachlib.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      248 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/thesaurus.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      364 2023-06-18 18:46:56.000000 LLM-Toolbox-0.0.2/prompt_templates/tools/translate.yaml
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-18 19:23:17.287164 LLM-Toolbox-0.0.2/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2924 2023-06-18 19:21:47.000000 LLM-Toolbox-0.0.2/setup.py
```

### Comparing `llm-toolbox-0.0.0/LICENSE` & `LLM-Toolbox-0.0.2/LICENSE`

 * *Files identical despite different names*


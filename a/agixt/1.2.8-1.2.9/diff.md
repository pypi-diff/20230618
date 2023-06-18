# Comparing `tmp/agixt-1.2.8.tar.gz` & `tmp/agixt-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.2.8.tar", last modified: Thu Jun 15 16:17:05 2023, max compression
+gzip compressed data, was "agixt-1.2.9.tar", last modified: Fri Jun 16 02:42:28 2023, max compression
```

## Comparing `agixt-1.2.8.tar` & `agixt-1.2.9.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 16:16:56.000000 agixt-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-15 16:16:56.000000 agixt-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-15 16:17:05.882562 agixt-1.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27135 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/Prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt/WORKSPACE/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/WORKSPACE/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.858561 agixt-1.2.8/agixt/agents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt/agents/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/agents/gpt4free/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt/chains/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate Smart Task Chain without Research.json
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate Smart Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate Task Chain without Research.json
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate and Run Smart Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Generate and Run Task Chain.json
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Smart Chat.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Smart Instruct.json
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Test_Commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/chains/Write a Poem.json
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.866562 agixt-1.2.8/agixt/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/agixt_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/agixt_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/briantts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/dalle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/gtts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/macostts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/microsoft_365.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/searxng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/sendgrid_email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/extensions/web_playwright.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Chat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Check-Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Create New Command.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Custom Input.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Get Task Description.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Get Task List.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Instruction.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/JSONFormatter.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Pick a Poem Subject.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Pick-a-Link.txt
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Prioritize.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Pseudo Code.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Score Response.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartChat-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartChat-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartChat-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartChat-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-Researcher.txt
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-Resolver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartInstruct-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartTask-CleanResponse.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartTask-Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/SmartTask-StepByStep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Task Execution.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Tell Me How.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Title a Chain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Title a Poem.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Validation.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/ValidationFailed.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/WebSearch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Write a Haiku.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/Write a Poem.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/gpt-3.5-turbo/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/gpt-3.5-turbo/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/gpt-4/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/gpt-4/instruct.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/starchat/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/starchat/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.870561 agixt-1.2.8/agixt/prompts/vicuna/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/prompts/vicuna/instruct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/llamacppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/poe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/runpod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 16:16:56.000000 agixt-1.2.8/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.862562 agixt-1.2.8/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 16:17:05.000000 agixt-1.2.8/agixt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/docs/1-Getting started/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/1-Getting started/Quick Start.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/1-Getting started/Screenshots.md
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/1-Getting started/Support.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/docs/2-Concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/0-Core Concepts.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Agents.md
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Chains.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Commands.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Instructions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Prompts.md
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Providers.md
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Smart Chat.md
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Smart Instruct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Smart Task.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/2-Concepts/Tasks.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.874561 agixt-1.2.8/docs/3-Providers/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Anthropic Claude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Azure OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/ChatGPT.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/FastChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/GPT4ALL-GPU.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/GPT4ALL.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/GPT4Free.md
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Google Bard.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Google Palm.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Hugging Face Transformers.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/HuggingChat.md
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Kobold.md
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Microsoft Bing.md
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Oobabooga Text Generation Web UI.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/OpenAI.md
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/Poe.md
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/llamacpp API.md
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/3-Providers/llamacpp.md
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.878561 agixt-1.2.8/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT-gradient-flat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT-gradient-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT.png
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXT_Original_PSD.psd
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/AGiXTwhiteborder.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Docker-desktop-win-setting-streamlit.png
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Smart Instruct.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Smart Instruct.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Smart Tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Smart Tasks.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-15 16:16:56.000000 agixt-1.2.8/docs/images/Untitled Diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 16:16:56.000000 agixt-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-15 16:16:56.000000 agixt-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:17:05.882562 agixt-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-15 16:16:56.000000 agixt-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.878561 agixt-1.2.8/streamlit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.878561 agixt-1.2.8/streamlit/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/Main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.878561 agixt-1.2.8/streamlit/auth_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/Cfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/Redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/Users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/streamlit/auth_libs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/pages/Login.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/pages/Profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/auth_libs/pages/Register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/components/verify_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/streamlit/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/pages/0-Agent_Settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/pages/1-Prompt_Templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/pages/2-Chain_Management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-15 16:16:56.000000 agixt-1.2.8/streamlit/pages/3-Interact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:17:05.882562 agixt-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-15 16:16:56.000000 agixt-1.2.8/tests/ApiClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-15 16:16:56.000000 agixt-1.2.8/tests/test-commands.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    57091 2023-06-15 16:16:56.000000 agixt-1.2.8/tests/tests.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.232481 agixt-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-16 02:42:18.000000 agixt-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-16 02:42:18.000000 agixt-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-16 02:42:28.232481 agixt-1.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.208480 agixt-1.2.9/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27140 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/Prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.208480 agixt-1.2.9/agixt/WORKSPACE/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/WORKSPACE/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.204481 agixt-1.2.9/agixt/agents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.208480 agixt-1.2.9/agixt/agents/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/agents/gpt4free/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16777 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.212481 agixt-1.2.9/agixt/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate Smart Task Chain without Research.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate Smart Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate Task Chain without Research.json
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate and Run Smart Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Generate and Run Task Chain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Smart Chat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Smart Instruct.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Test_Commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/chains/Write a Poem.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.212481 agixt-1.2.9/agixt/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/agixt_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/agixt_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/briantts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/dalle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/gtts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/macostts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/microsoft_365.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/searxng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/sendgrid_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/extensions/web_playwright.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Chat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Check-Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Create New Command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Custom Input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Get Task Description.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Get Task List.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Instruction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/JSONFormatter.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Pick a Poem Subject.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Pick-a-Link.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Prioritize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Pseudo Code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Score Response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartChat-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartChat-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartChat-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartChat-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-Researcher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-Resolver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartInstruct-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartTask-CleanResponse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartTask-Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/SmartTask-StepByStep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Task Execution.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Tell Me How.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Title a Chain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Title a Poem.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Validation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/ValidationFailed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/WebSearch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Write a Haiku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/Write a Poem.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/gpt-3.5-turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/gpt-3.5-turbo/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/gpt-4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/gpt-4/instruct.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/starchat/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/starchat/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.216481 agixt-1.2.9/agixt/prompts/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/prompts/vicuna/instruct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.220481 agixt-1.2.9/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/llamacppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/poe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 02:42:18.000000 agixt-1.2.9/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.208480 agixt-1.2.9/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 02:42:28.000000 agixt-1.2.9/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.220481 agixt-1.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.220481 agixt-1.2.9/docs/1-Getting started/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/1-Getting started/Quick Start.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/1-Getting started/Screenshots.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/1-Getting started/Support.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.220481 agixt-1.2.9/docs/2-Concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/0-Core Concepts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Agents.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Chains.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Instructions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Prompts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Providers.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Smart Chat.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Smart Instruct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Smart Task.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/2-Concepts/Tasks.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.224481 agixt-1.2.9/docs/3-Providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Anthropic Claude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Azure OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/ChatGPT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/FastChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/GPT4ALL-GPU.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/GPT4ALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/GPT4Free.md
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Google Bard.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Google Palm.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Hugging Face Transformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/HuggingChat.md
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Kobold.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Microsoft Bing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Oobabooga Text Generation Web UI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/OpenAI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/Poe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/llamacpp API.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/3-Providers/llamacpp.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT-gradient-flat.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT-gradient-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1707562 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXT_Original_PSD.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/AGiXTwhiteborder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Docker-desktop-win-setting-streamlit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Smart Instruct.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Smart Instruct.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Smart Tasks.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    22011 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Smart Tasks.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-16 02:42:18.000000 agixt-1.2.9/docs/images/Untitled Diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 02:42:18.000000 agixt-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 02:42:18.000000 agixt-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:42:28.232481 agixt-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-16 02:42:18.000000 agixt-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/Main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/auth_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/Cfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/Redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/Users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/auth_libs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/pages/Login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/pages/Profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/auth_libs/pages/Register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/components/verify_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.228481 agixt-1.2.9/streamlit/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/pages/0-Agent_Settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/pages/1-Prompt_Templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/pages/2-Chain_Management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-16 02:42:18.000000 agixt-1.2.9/streamlit/pages/3-Interact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:42:28.232481 agixt-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-06-16 02:42:18.000000 agixt-1.2.9/tests/ApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-16 02:42:18.000000 agixt-1.2.9/tests/test-commands.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    57091 2023-06-16 02:42:18.000000 agixt-1.2.9/tests/tests.ipynb
```

### Comparing `agixt-1.2.8/LICENSE` & `agixt-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/PKG-INFO` & `agixt-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.8
+Version: 1.2.9
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.8/agixt/Agent.py` & `agixt-1.2.9/agixt/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/Chain.py` & `agixt-1.2.9/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/Embedding.py` & `agixt-1.2.9/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/Extensions.py` & `agixt-1.2.9/agixt/Extensions.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/Interactions.py` & `agixt-1.2.9/agixt/Interactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
                 pass
             if prompt == "Chat":
                 self.agent.log_interaction(role="USER", message=user_input)
             else:
                 self.agent.log_interaction(role="USER", message=formatted_prompt)
             self.agent.log_interaction(role=self.agent_name, message=self.response)
 
-        if shots > 1:
+        if int(shots) > 1:
             responses = [self.response]
             for shot in range(shots - 1):
                 shot_response = await self.run(
                     user_input=user_input,
                     prompt=prompt,
                     context_results=context_results,
                     shots=shots - 1,
```

### Comparing `agixt-1.2.8/agixt/Memories.py` & `agixt-1.2.9/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/Prompts.py` & `agixt-1.2.9/agixt/Prompts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/app.py` & `agixt-1.2.9/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/chains/Generate Smart Task Chain without Research.json` & `agixt-1.2.9/agixt/chains/Smart Chat.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6690104166666666%*

 * *Differences: {"'chain_name'": "'Smart Chat'",*

 * * "'steps'": "{0: {'prompt': {'prompt_name': 'SmartChat-StepByStep', 'websearch': True, "*

 * *            "'websearch_depth': 3, 'shots': 3}}, 1: {'prompt': {'prompt_name': "*

 * *            "'SmartChat-Researcher', 'shots': '3', 'task': '{STEP1}'}}, 2: {'prompt': "*

 * *            "{'prompt_name': 'SmartChat-Resolver', 'shots': '3', 'task': '{STEP2}'}}, delete: [3]}"}*

```diff
@@ -1,43 +1,37 @@
 {
-    "chain_name": "Generate Smart Task Chain without Research",
+    "chain_name": "Smart Chat",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
-                "prompt_name": "Get Task List"
+                "prompt_name": "SmartChat-StepByStep",
+                "shots": 3,
+                "websearch": true,
+                "websearch_depth": 3
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "Get Task Description"
+                "prompt_name": "SmartChat-Researcher",
+                "shots": "3",
+                "task": "{STEP1}"
             },
             "prompt_type": "Prompt",
             "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "Title a Chain"
+                "prompt_name": "SmartChat-Resolver",
+                "shots": "3",
+                "task": "{STEP2}"
             },
             "prompt_type": "Prompt",
             "step": 3
-        },
-        {
-            "agent_name": "gpt4free",
-            "prompt": {
-                "agent": "gpt4free",
-                "command_name": "Create Smart Task Chain",
-                "numbered_list_of_tasks": "{STEP1}",
-                "primary_objective": "{user_input}",
-                "short_chain_description": "{STEP3}",
-                "short_task_description": "{STEP2}"
-            },
-            "prompt_type": "Command",
-            "step": 4
         }
     ]
 }
```

### Comparing `agixt-1.2.8/agixt/chains/Generate Smart Task Chain.json` & `agixt-1.2.9/agixt/chains/Generate Smart Task Chain.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.923828125%*

 * *Differences: {"'steps'": "{1: {'prompt': {'prompt_name': 'Title a Chain'}}, 2: {'step': 3, 'prompt': "*

 * *            "{'short_chain_description': '{STEP2}', delete: ['short_task_description']}}, delete: "*

 * *            '[2]}'}*

```diff
@@ -11,35 +11,26 @@
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "Get Task Description"
-            },
-            "prompt_type": "Prompt",
-            "step": 2
-        },
-        {
-            "agent_name": "gpt4free",
-            "prompt": {
                 "prompt_name": "Title a Chain"
             },
             "prompt_type": "Prompt",
-            "step": 3
+            "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "agent": "gpt4free",
                 "command_name": "Create Smart Task Chain",
                 "numbered_list_of_tasks": "{STEP1}",
                 "primary_objective": "{user_input}",
-                "short_chain_description": "{STEP3}",
-                "short_task_description": "{STEP2}"
+                "short_chain_description": "{STEP2}"
             },
             "prompt_type": "Command",
-            "step": 4
+            "step": 3
         }
     ]
 }
```

### Comparing `agixt-1.2.8/agixt/chains/Generate Task Chain without Research.json` & `agixt-1.2.9/agixt/chains/Generate and Run Smart Task Chain.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7109375%*

 * *Differences: {"'chain_name'": "'Generate and Run Smart Task Chain'",*

 * * "'steps'": "{0: {'prompt': {'websearch': True, 'websearch_depth': 3}}, 1: {'prompt': "*

 * *            "{'prompt_name': 'Title a Chain'}}, 2: {'prompt_type': 'Command', 'prompt': {replace: "*

 * *            "OrderedDict([('command_name', 'Create Smart Task Chain'), ('agent', 'gpt4free'), "*

 * *            "('primary_objective', '{user_input}'), ('numbered_list_of_tasks', '{STEP1}'), "*

 * *            "('short_chain_description', '{STEP2}')])}}, 3: {'prompt_type': 'Ch […]*

```diff
@@ -1,43 +1,45 @@
 {
-    "chain_name": "Generate Task Chain without Research",
+    "chain_name": "Generate and Run Smart Task Chain",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
-                "prompt_name": "Get Task List"
+                "prompt_name": "Get Task List",
+                "websearch": true,
+                "websearch_depth": 3
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "Get Task Description"
+                "prompt_name": "Title a Chain"
             },
             "prompt_type": "Prompt",
             "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "Title a Chain"
+                "agent": "gpt4free",
+                "command_name": "Create Smart Task Chain",
+                "numbered_list_of_tasks": "{STEP1}",
+                "primary_objective": "{user_input}",
+                "short_chain_description": "{STEP2}"
             },
-            "prompt_type": "Prompt",
+            "prompt_type": "Command",
             "step": 3
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "agent": "gpt4free",
-                "command_name": "Create Task Chain",
-                "numbered_list_of_tasks": "{STEP1}",
-                "primary_objective": "{user_input}",
-                "short_chain_description": "{STEP3}",
-                "short_task_description": "{STEP2}"
+                "chain": "{STEP4}",
+                "input": "{user_input}"
             },
-            "prompt_type": "Command",
+            "prompt_type": "Chain",
             "step": 4
         }
     ]
 }
```

### Comparing `agixt-1.2.8/agixt/chains/Generate Task Chain.json` & `agixt-1.2.9/agixt/chains/Generate Task Chain without Research.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.669921875%*

 * *Differences: {"'chain_name'": "'Generate Task Chain without Research'",*

 * * "'steps'": "{0: {'prompt': {delete: ['websearch', 'websearch_depth']}}, 1: {'prompt': "*

 * *            "{'prompt_name': 'Title a Chain'}}, 2: {'step': 3, 'prompt': "*

 * *            "{'short_chain_description': '{STEP2}', delete: ['short_task_description']}}, delete: "*

 * *            '[2]}'}*

```diff
@@ -1,45 +1,34 @@
 {
-    "chain_name": "Generate Task Chain",
+    "chain_name": "Generate Task Chain without Research",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
-                "prompt_name": "Get Task List",
-                "websearch": true,
-                "websearch_depth": 3
+                "prompt_name": "Get Task List"
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "Get Task Description"
-            },
-            "prompt_type": "Prompt",
-            "step": 2
-        },
-        {
-            "agent_name": "gpt4free",
-            "prompt": {
                 "prompt_name": "Title a Chain"
             },
             "prompt_type": "Prompt",
-            "step": 3
+            "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "agent": "gpt4free",
                 "command_name": "Create Task Chain",
                 "numbered_list_of_tasks": "{STEP1}",
                 "primary_objective": "{user_input}",
-                "short_chain_description": "{STEP3}",
-                "short_task_description": "{STEP2}"
+                "short_chain_description": "{STEP2}"
             },
             "prompt_type": "Command",
-            "step": 4
+            "step": 3
         }
     ]
 }
```

### Comparing `agixt-1.2.8/agixt/chains/Generate and Run Smart Task Chain.json` & `agixt-1.2.9/agixt/chains/Generate and Run Task Chain.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6822916666666666%*

 * *Differences: {"'chain_name'": "'Generate and Run Task Chain'",*

 * * "'steps'": "{1: {'prompt': {'prompt_name': 'Title a Chain'}}, 2: {'step': 3, 'prompt': "*

 * *            "{'command_name': 'Create Task Chain', 'short_chain_description': '{STEP2}', delete: "*

 * *            "['short_task_description']}}, 3: {'step': 4}, delete: [2]}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "chain_name": "Generate and Run Smart Task Chain",
+    "chain_name": "Generate and Run Task Chain",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
                 "prompt_name": "Get Task List",
                 "websearch": true,
@@ -11,44 +11,35 @@
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "Get Task Description"
-            },
-            "prompt_type": "Prompt",
-            "step": 2
-        },
-        {
-            "agent_name": "gpt4free",
-            "prompt": {
                 "prompt_name": "Title a Chain"
             },
             "prompt_type": "Prompt",
-            "step": 3
+            "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "agent": "gpt4free",
-                "command_name": "Create Smart Task Chain",
+                "command_name": "Create Task Chain",
                 "numbered_list_of_tasks": "{STEP1}",
                 "primary_objective": "{user_input}",
-                "short_chain_description": "{STEP3}",
-                "short_task_description": "{STEP2}"
+                "short_chain_description": "{STEP2}"
             },
             "prompt_type": "Command",
-            "step": 4
+            "step": 3
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "chain": "{STEP4}",
                 "input": "{user_input}"
             },
             "prompt_type": "Chain",
-            "step": 5
+            "step": 4
         }
     ]
 }
```

### Comparing `agixt-1.2.8/agixt/chains/Generate and Run Task Chain.json` & `agixt-1.2.9/agixt/chains/Generate Smart Task Chain without Research.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6354166666666666%*

 * *Differences: {"'chain_name'": "'Generate Smart Task Chain without Research'",*

 * * "'steps'": "{0: {'prompt': {delete: ['websearch', 'websearch_depth']}}, 1: {'prompt': "*

 * *            "{'prompt_name': 'Title a Chain'}}, 2: {'step': 3, 'prompt': {'command_name': 'Create "*

 * *            "Smart Task Chain', 'short_chain_description': '{STEP2}', delete: "*

 * *            "['short_task_description']}}, delete: [4, 2]}"}*

```diff
@@ -1,54 +1,34 @@
 {
-    "chain_name": "Generate and Run Task Chain",
+    "chain_name": "Generate Smart Task Chain without Research",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
-                "prompt_name": "Get Task List",
-                "websearch": true,
-                "websearch_depth": 3
+                "prompt_name": "Get Task List"
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "Get Task Description"
-            },
-            "prompt_type": "Prompt",
-            "step": 2
-        },
-        {
-            "agent_name": "gpt4free",
-            "prompt": {
                 "prompt_name": "Title a Chain"
             },
             "prompt_type": "Prompt",
-            "step": 3
+            "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "agent": "gpt4free",
-                "command_name": "Create Task Chain",
+                "command_name": "Create Smart Task Chain",
                 "numbered_list_of_tasks": "{STEP1}",
                 "primary_objective": "{user_input}",
-                "short_chain_description": "{STEP3}",
-                "short_task_description": "{STEP2}"
+                "short_chain_description": "{STEP2}"
             },
             "prompt_type": "Command",
-            "step": 4
-        },
-        {
-            "agent_name": "gpt4free",
-            "prompt": {
-                "chain": "{STEP4}",
-                "input": "{user_input}"
-            },
-            "prompt_type": "Chain",
-            "step": 5
+            "step": 3
         }
     ]
 }
```

### Comparing `agixt-1.2.8/agixt/chains/Smart Chat.json` & `agixt-1.2.9/agixt/chains/Smart Instruct.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7454861111111112%*

 * *Differences: {"'chain_name'": "'Smart Instruct'",*

 * * "'steps'": "{0: {'prompt': {'prompt_name': 'SmartInstruct-StepByStep'}}, 1: {'prompt': "*

 * *            "{'prompt_name': 'SmartInstruct-Researcher'}}, 2: {'prompt': {'prompt_name': "*

 * *            "'SmartInstruct-Resolver'}}}"}*

```diff
@@ -1,36 +1,36 @@
 {
-    "chain_name": "Smart Chat",
+    "chain_name": "Smart Instruct",
     "steps": [
         {
             "agent_name": "gpt4free",
             "prompt": {
                 "context_results": 5,
-                "prompt_name": "SmartChat-StepByStep",
+                "prompt_name": "SmartInstruct-StepByStep",
                 "shots": 3,
                 "websearch": true,
                 "websearch_depth": 3
             },
             "prompt_type": "Prompt",
             "step": 1
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "SmartChat-Researcher",
+                "prompt_name": "SmartInstruct-Researcher",
                 "shots": "3",
                 "task": "{STEP1}"
             },
             "prompt_type": "Prompt",
             "step": 2
         },
         {
             "agent_name": "gpt4free",
             "prompt": {
-                "prompt_name": "SmartChat-Resolver",
+                "prompt_name": "SmartInstruct-Resolver",
                 "shots": "3",
                 "task": "{STEP2}"
             },
             "prompt_type": "Prompt",
             "step": 3
         }
     ]
```

### Comparing `agixt-1.2.8/agixt/chains/Test_Commands.json` & `agixt-1.2.9/agixt/chains/Test_Commands.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/chains/Write a Poem.json` & `agixt-1.2.9/agixt/chains/Write a Poem.json`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/example.ipynb` & `agixt-1.2.9/agixt/example.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/agixt_agent.py` & `agixt-1.2.9/agixt/extensions/agixt_agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/agixt_chain.py` & `agixt-1.2.9/agixt/extensions/agixt_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from Chain import Chain
 from Extensions import Extensions
 from Interactions import Interactions
+import datetime
 
 
 class agixt_chain(Extensions):
     def __init__(self, **kwargs):
         self.chains = Chain().get_chains()
         self.commands = {
             "Create Task Chain": self.create_task_chain,
@@ -18,19 +19,17 @@
                     )
 
     async def create_task_chain(
         self,
         agent: str,
         primary_objective: str,
         numbered_list_of_tasks: str,
-        short_task_description: str,
         short_chain_description: str,
     ):
-        import datetime
-        now = datetime.datetime.now()  
+        now = datetime.datetime.now()
         timestamp = now.strftime("%Y-%m-%d_%H-%M-%S")
         task_list = numbered_list_of_tasks.split("\n")
         task_list = [
             task.lstrip("0123456789.")  # Strip leading digits and periods
             for task in task_list
             if task
             and task[0]
@@ -44,43 +43,44 @@
             chain.add_chain_step(
                 chain_name=chain_name,
                 agent_name=agent,
                 step_number=i,
                 prompt_type="Prompt",
                 prompt={
                     "prompt_name": "Task Execution",
-                    "user_input": primary_objective,
+                    "primary_objective": primary_objective,
                     "task": task,
                     "websearch": True,
                     "websearch_depth": 3,
                     "context_results": 5,
                 },
             )
             i += 1
         return chain_name
 
     async def create_smart_task_chain(
         self,
         agent: str,
         primary_objective: str,
         numbered_list_of_tasks: str,
-        short_task_description: str,
+        short_chain_description: str,
     ):
-        import datetime
-        now = datetime.datetime.now()  
+        now = datetime.datetime.now()
         timestamp = now.strftime("%Y-%m-%d_%H-%M-%S")
         task_list = numbered_list_of_tasks.split("\n")
         task_list = [
             task.lstrip("0123456789.")  # Strip leading digits and periods
             for task in task_list
             if task
             and task[0]
             in [str(i) for i in range(10)]  # Check for task starting with a digit (0-9)
         ]
-        chain_name = f"AI Generated Smart Task - {short_chain_description} - {timestamp}"
+        chain_name = (
+            f"AI Generated Smart Task - {short_chain_description} - {timestamp}"
+        )
         chain = Chain()
         chain.add_chain(chain_name=chain_name)
         i = 1
         for task in task_list:
             chain.add_chain_step(
                 chain_name=chain_name,
                 agent_name=agent,
```

### Comparing `agixt-1.2.8/agixt/extensions/briantts.py` & `agixt-1.2.9/agixt/extensions/briantts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/dalle.py` & `agixt-1.2.9/agixt/extensions/dalle.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/discord.py` & `agixt-1.2.9/agixt/extensions/discord.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/elevenlabs.py` & `agixt-1.2.9/agixt/extensions/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/file_system.py` & `agixt-1.2.9/agixt/extensions/file_system.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/github.py` & `agixt-1.2.9/agixt/extensions/github.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/google.py` & `agixt-1.2.9/agixt/extensions/google.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/gtts.py` & `agixt-1.2.9/agixt/extensions/gtts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/huggingface.py` & `agixt-1.2.9/agixt/extensions/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/macostts.py` & `agixt-1.2.9/agixt/extensions/macostts.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/microsoft_365.py` & `agixt-1.2.9/agixt/extensions/microsoft_365.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/searxng.py` & `agixt-1.2.9/agixt/extensions/searxng.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/sendgrid_email.py` & `agixt-1.2.9/agixt/extensions/sendgrid_email.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/twitter.py` & `agixt-1.2.9/agixt/extensions/twitter.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/extensions/web_playwright.py` & `agixt-1.2.9/agixt/extensions/web_playwright.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/Create New Command.txt` & `agixt-1.2.9/agixt/prompts/Create New Command.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/Execution.txt` & `agixt-1.2.9/agixt/prompts/Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/Get Task List.txt` & `agixt-1.2.9/agixt/prompts/Get Task List.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/Instruction.txt` & `agixt-1.2.9/agixt/prompts/Instruction.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/SmartInstruct-Execution.txt` & `agixt-1.2.9/agixt/prompts/SmartInstruct-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/SmartTask-Execution.txt` & `agixt-1.2.9/agixt/prompts/SmartTask-Execution.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/Task Execution.txt` & `agixt-1.2.9/agixt/prompts/Task Execution.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,9 +19,9 @@
             "arg1": "val1",
             "arg2": "val2",
             "argN": "valN"
         }
     }
 }
 ```
-Primary Objective: {user_input}
+Primary Objective: {primary_objective}
 Your task: {task}
```

### Comparing `agixt-1.2.8/agixt/prompts/Title a Chain.txt` & `agixt-1.2.9/agixt/prompts/Title a Chain.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/ValidationFailed.txt` & `agixt-1.2.9/agixt/prompts/ValidationFailed.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/gpt-3.5-turbo/instruct.txt` & `agixt-1.2.9/agixt/prompts/gpt-3.5-turbo/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/gpt-4/instruct.txt` & `agixt-1.2.9/agixt/prompts/gpt-4/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/instruct.txt` & `agixt-1.2.9/agixt/prompts/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/starchat/instruct.txt` & `agixt-1.2.9/agixt/prompts/starchat/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/prompts/vicuna/instruct.txt` & `agixt-1.2.9/agixt/prompts/vicuna/instruct.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/__init__.py` & `agixt-1.2.9/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/azure.py` & `agixt-1.2.9/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/bing.py` & `agixt-1.2.9/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/chatgpt.py` & `agixt-1.2.9/agixt/provider/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/claude.py` & `agixt-1.2.9/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/fastchat.py` & `agixt-1.2.9/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/gpt4all.py` & `agixt-1.2.9/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/gpt4free.py` & `agixt-1.2.9/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/gpugpt4all.py` & `agixt-1.2.9/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/huggingchat.py` & `agixt-1.2.9/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/huggingface.py` & `agixt-1.2.9/agixt/provider/huggingface.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/kobold.py` & `agixt-1.2.9/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/llamacpp.py` & `agixt-1.2.9/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/llamacppapi.py` & `agixt-1.2.9/agixt/provider/llamacppapi.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/oobabooga.py` & `agixt-1.2.9/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/openai.py` & `agixt-1.2.9/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/palm.py` & `agixt-1.2.9/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/poe.py` & `agixt-1.2.9/agixt/provider/poe.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/runpod.py` & `agixt-1.2.9/agixt/provider/runpod.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt/provider/transformer.py` & `agixt-1.2.9/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/agixt.egg-info/PKG-INFO` & `agixt-1.2.9/agixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.2.8
+Version: 1.2.9
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `agixt-1.2.8/agixt.egg-info/SOURCES.txt` & `agixt-1.2.9/agixt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/1-Getting started/Quick Start.md` & `agixt-1.2.9/docs/1-Getting started/Quick Start.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/1-Getting started/Screenshots.md` & `agixt-1.2.9/docs/1-Getting started/Screenshots.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/1-Getting started/Support.md` & `agixt-1.2.9/docs/1-Getting started/Support.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/0-Core Concepts.md` & `agixt-1.2.9/docs/2-Concepts/0-Core Concepts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Agents.md` & `agixt-1.2.9/docs/2-Concepts/Agents.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Chains.md` & `agixt-1.2.9/docs/2-Concepts/Chains.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Chat.md` & `agixt-1.2.9/docs/2-Concepts/Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Commands.md` & `agixt-1.2.9/docs/2-Concepts/Commands.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Instructions.md` & `agixt-1.2.9/docs/2-Concepts/Instructions.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Prompts.md` & `agixt-1.2.9/docs/2-Concepts/Prompts.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Smart Chat.md` & `agixt-1.2.9/docs/2-Concepts/Smart Chat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Smart Instruct.md` & `agixt-1.2.9/docs/2-Concepts/Smart Instruct.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/2-Concepts/Smart Task.md` & `agixt-1.2.9/docs/2-Concepts/Smart Task.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/Anthropic Claude.md` & `agixt-1.2.9/docs/3-Providers/Anthropic Claude.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/Azure OpenAI.md` & `agixt-1.2.9/docs/3-Providers/Azure OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/ChatGPT.md` & `agixt-1.2.9/docs/3-Providers/ChatGPT.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/FastChat.md` & `agixt-1.2.9/docs/3-Providers/FastChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/GPT4ALL-GPU.md` & `agixt-1.2.9/docs/3-Providers/GPT4ALL-GPU.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/GPT4ALL.md` & `agixt-1.2.9/docs/3-Providers/GPT4ALL.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/GPT4Free.md` & `agixt-1.2.9/docs/3-Providers/GPT4Free.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/Google Bard.md` & `agixt-1.2.9/docs/3-Providers/Google Bard.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/Hugging Face Transformers.md` & `agixt-1.2.9/docs/3-Providers/Hugging Face Transformers.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/HuggingChat.md` & `agixt-1.2.9/docs/3-Providers/HuggingChat.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/Microsoft Bing.md` & `agixt-1.2.9/docs/3-Providers/Microsoft Bing.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/Oobabooga Text Generation Web UI.md` & `agixt-1.2.9/docs/3-Providers/Oobabooga Text Generation Web UI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/OpenAI.md` & `agixt-1.2.9/docs/3-Providers/OpenAI.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/Poe.md` & `agixt-1.2.9/docs/3-Providers/Poe.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/llamacpp API.md` & `agixt-1.2.9/docs/3-Providers/llamacpp API.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/3-Providers/llamacpp.md` & `agixt-1.2.9/docs/3-Providers/llamacpp.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/README.md` & `agixt-1.2.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/AGiXT-gradient-flat.svg` & `agixt-1.2.9/docs/images/AGiXT-gradient-flat.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/AGiXT-gradient-light.svg` & `agixt-1.2.9/docs/images/AGiXT-gradient-light.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/AGiXT.png` & `agixt-1.2.9/docs/images/AGiXT.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/AGiXT.svg` & `agixt-1.2.9/docs/images/AGiXT.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/AGiXT_Original_PSD.psd` & `agixt-1.2.9/docs/images/AGiXT_Original_PSD.psd`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/AGiXTwhiteborder.svg` & `agixt-1.2.9/docs/images/AGiXTwhiteborder.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/Docker-desktop-win-setting-streamlit.png` & `agixt-1.2.9/docs/images/Docker-desktop-win-setting-streamlit.png`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/Smart Instruct.drawio` & `agixt-1.2.9/docs/images/Smart Instruct.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/Smart Instruct.drawio.svg` & `agixt-1.2.9/docs/images/Smart Instruct.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/Smart Tasks.drawio` & `agixt-1.2.9/docs/images/Smart Tasks.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/Smart Tasks.drawio.svg` & `agixt-1.2.9/docs/images/Smart Tasks.drawio.svg`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/docs/images/Untitled Diagram.drawio` & `agixt-1.2.9/docs/images/Untitled Diagram.drawio`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/setup.py` & `agixt-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/ApiClient.py` & `agixt-1.2.9/streamlit/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/Main.py` & `agixt-1.2.9/streamlit/Main.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/auth_libs/Cfig.py` & `agixt-1.2.9/streamlit/auth_libs/Cfig.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/auth_libs/Redirect.py` & `agixt-1.2.9/streamlit/auth_libs/Redirect.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/auth_libs/Users.py` & `agixt-1.2.9/streamlit/auth_libs/Users.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/auth_libs/pages/Login.py` & `agixt-1.2.9/streamlit/auth_libs/pages/Login.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/auth_libs/pages/Profile.py` & `agixt-1.2.9/streamlit/auth_libs/pages/Profile.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/auth_libs/pages/Register.py` & `agixt-1.2.9/streamlit/auth_libs/pages/Register.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/components/chain.py` & `agixt-1.2.9/streamlit/components/chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/components/docs.py` & `agixt-1.2.9/streamlit/components/docs.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/components/history.py` & `agixt-1.2.9/streamlit/components/history.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/components/learning.py` & `agixt-1.2.9/streamlit/components/learning.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/components/selectors.py` & `agixt-1.2.9/streamlit/components/selectors.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/components/verify_backend.py` & `agixt-1.2.9/streamlit/components/verify_backend.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/pages/0-Agent_Settings.py` & `agixt-1.2.9/streamlit/pages/0-Agent_Settings.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/pages/1-Prompt_Templates.py` & `agixt-1.2.9/streamlit/pages/1-Prompt_Templates.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/pages/2-Chain_Management.py` & `agixt-1.2.9/streamlit/pages/2-Chain_Management.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/streamlit/pages/3-Interact.py` & `agixt-1.2.9/streamlit/pages/3-Interact.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/tests/ApiClient.py` & `agixt-1.2.9/tests/ApiClient.py`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/tests/test-commands.ipynb` & `agixt-1.2.9/tests/test-commands.ipynb`

 * *Files identical despite different names*

### Comparing `agixt-1.2.8/tests/tests.ipynb` & `agixt-1.2.9/tests/tests.ipynb`

 * *Files identical despite different names*


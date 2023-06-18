# Comparing `tmp/alphawave-0.2.4.tar.gz` & `tmp/alphawave-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.4.tar", last modified: Thu Jun 15 20:03:28 2023, max compression
+gzip compressed data, was "alphawave-0.2.5.tar", last modified: Sun Jun 18 19:21:17 2023, max compression
```

## Comparing `alphawave-0.2.4.tar` & `alphawave-0.2.5.tar`

### file list

```diff
@@ -1,50 +1,57 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.4/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-15 20:03:28.144310 alphawave-0.2.4/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7129 2023-06-10 04:04:27.000000 alphawave-0.2.4/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-15 20:03:13.000000 alphawave-0.2.4/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-15 20:03:28.144310 alphawave-0.2.4/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.140310 alphawave-0.2.4/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9229 2023-06-15 03:36:54.000000 alphawave-0.2.4/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.4/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      723 2023-06-15 04:11:00.000000 alphawave-0.2.4/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5982 2023-06-15 20:01:04.000000 alphawave-0.2.4/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7236 2023-06-11 19:10:18.000000 alphawave-0.2.4/src/alphawave/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.4/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7966 2023-06-11 19:12:11.000000 alphawave-0.2.4/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8572 2023-06-11 18:41:22.000000 alphawave-0.2.4/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.4/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 04:11:51.000000 alphawave-0.2.4/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.4/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.4/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.4/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.4/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.4/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.4/src/alphawave/jsonParser.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.4/src/alphawave/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7742 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1350 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-15 20:03:28.000000 alphawave-0.2.4/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16240 2023-06-15 18:47:04.000000 alphawave-0.2.4/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.4/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2637 2023-06-15 18:44:50.000000 alphawave-0.2.4/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.4/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.4/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.4/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.4/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.4/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-15 19:13:49.000000 alphawave-0.2.4/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3553 2023-06-11 03:56:28.000000 alphawave-0.2.4/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.4/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.4/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.4/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-10 21:45:49.000000 alphawave-0.2.4/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-15 20:03:28.144310 alphawave-0.2.4/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.4/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14653 2023-06-07 04:29:45.000000 alphawave-0.2.4/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.4/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.5/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9472 2023-06-18 19:21:17.265798 alphawave-0.2.5/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.5/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      925 2023-06-18 19:21:09.000000 alphawave-0.2.5/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-18 19:21:17.265798 alphawave-0.2.5/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.261798 alphawave-0.2.5/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9228 2023-06-17 19:16:02.000000 alphawave-0.2.5/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.5/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.5/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5978 2023-06-17 19:12:44.000000 alphawave-0.2.5/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.5/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9094 2023-06-18 19:09:29.000000 alphawave-0.2.5/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8570 2023-06-18 03:50:01.000000 alphawave-0.2.5/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.5/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.5/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.5/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.5/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.5/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.5/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.5/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.5/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9472 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1585 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      125 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-18 19:21:17.000000 alphawave-0.2.5/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16065 2023-06-18 16:59:38.000000 alphawave-0.2.5/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.5/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2643 2023-06-18 02:59:07.000000 alphawave-0.2.5/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.5/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.5/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.5/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.5/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.5/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.5/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3547 2023-06-16 16:10:31.000000 alphawave-0.2.5/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.5/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.5/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.5/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-10 21:45:49.000000 alphawave-0.2.5/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3741 2023-06-18 18:11:10.000000 alphawave-0.2.5/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2515 2023-06-18 03:44:14.000000 alphawave-0.2.5/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    19050 2023-06-17 23:10:50.000000 alphawave-0.2.5/src/alphawave_pyexts/conversation.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13351 2023-06-18 03:42:44.000000 alphawave-0.2.5/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1032 2023-06-18 00:09:12.000000 alphawave-0.2.5/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1402 2023-06-16 20:15:32.000000 alphawave-0.2.5/src/alphawave_pyexts/searchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6615 2023-06-18 17:44:47.000000 alphawave-0.2.5/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-18 19:21:17.265798 alphawave-0.2.5/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.5/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.5/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.5/tests/testSchema.py
```

### Comparing `alphawave-0.2.4/LICENSE` & `alphawave-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/PKG-INFO` & `alphawave-0.2.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,17 @@
-Metadata-Version: 2.1
-Name: alphawave
-Version: 0.2.4
-Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
-Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
-Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
-Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AlphaWave
+minor bug fixes, OS Client now correctly handles host, port, temperature, top_p, max_tokens
+
+New: SearchCommand will search the web. You will need a google api key.
+See tests/SearchCommandAgentTest.py
+
 AlphaWave is a very opinionated client for interfacing with Large Language Models (LLM). It uses [Promptrix](https://github.com/Stevenic/promptrix) for prompt management and has the following features:
 
 - Supports calling OpenAI and Azure OpenAI hosted models out of the box but a simple plugin model lets you extend AlphaWave to support any LLM.
+- Supports OS LLMs through an OSClient. Currently assumes a server on port 5004, see details below.
 - Promptrix integration means that all prompts are universal and work with either Chat Completion or Text Completion API's.
 - Automatic history management. AlphaWave manages a prompts conversation history and all you have todo is tell it where to store it. It uses an in-memory store by default but a simple plugin interface (provided by Promptrix) lets you store short term memory, like conversation history, anywhere.
 - State-of-the-art response repair logic. AlphaWave lets you provide an optional "response validator" plugin which it will use to validate every response returned from an LLM. Should a response fail validation, AlphaWave will automatically try to get the model to correct its mistake. More below...
 
 ## Automatic Response Repair
 A key goal of AlphaWave is to be the most reliable mechanisms for talking to an LLM on the planet. If you lookup the wikipedia definition for Alpha Waves you see that it's believed that they may be used to help predict mistakes in the human brain. One of the key roles of the AlphaWave library is to help automatically correct for mistakes made by an LLM, leading to more reliable output. It can correct for everything from hallucinations to just malformed output. It does this by using a series of techniques.
 
@@ -106,27 +98,60 @@
 
 # Start chat session
 asyncio.run(chat("Hello, how can I help you?"))
 ```
 
 One of the key features of Promptrix is its ability to proportionally layout prompts, so this prompt has an overall budget of 2000 input tokens. It will give the `SystemMessage` up to 50 tokens, the `UserMessage` up to 450 tokens, and then the `ConversationHistory` gets 100% of the remaining tokens.
 
-Next we just need to call `completePrompt()` on the wave to process the users input (in typescript for now, sorry):
+Once the prompt is formed, we just need to call `completePrompt()` on the wave to process the users input
+
+The  parameter to wave.completePrompt is optional and the wave can also take input directly from memory, but you don't have to pass prompts input. You can see in the example that if the prompt doesn't reference the input via a `{{$input}}` template variable it won't use it anyway.
+
+# Logging
+if you want to see the traffic with the server, the Client constructors (OSClient and OpenAIClient) take a logRequests parameter - False by default, set it to True to see prompts and responses on the console.
+
+# OSClient
+the 'default' way to use Alphawave-py with OpenAI is to use the OpenAI client as in line 49 of the example above. 
+If you want to use your own LLM, you can use instead:
+
+```python
+client = OSClient(apiKey=None)
+```
+
+The current OSClient assumes a server exists on localhost port 5004, using my own unique protocol.
+Not very useful, I know.
+Short term plans include: 
+1. allow specification of the host and port in the client constructor
+2. allow FastChat-like specification of the conversation template (user/assistant/etc). Support for this is already in the OSClient, just need to bring it out to the Constructor
+3. Implementation of a FastChat compatible api. Again, this was running in a dev version of the code, just need to re-insert it now that basic port is stable.
 
-```typescript
-// Route users message to wave
-const result = await wave.completePrompt(input);
-switch (result.status) {
-    case 'success':
-        console.log((result.response as Message).content);
-        break;
-    default:
-        if (result.response) {
-            console.log(`${result.status}: ${result.response}`);
-        } else {
-            console.log(`A result status of '${result.status}' was returned.`);
-        }
-        break;
+## OSClient protocol
+### OSClient sends json to the server:
+```python
+        server_message = {'prompt':prompt, 'temp': temp, 'top_p':top_p, 'max_tokens':max_tokens}
+        smj = json.dumps(server_message)
+        client_socket.sendall(smj.encode('utf-8'))
+        client_socket.sendall(b'x00xff')
+```
+where prompt is a string containing the messages:
+```python
+{
+  "role": "system",
+  "content": "You are an AI assistant that is friendly, kind, and helpful"
+}{
+  "role": "user",
+  "content": "Hi. How are you today?"
 }
 ```
 
-The `input` parameter is optional and the wave can also take input directly from memory, but you don't have to pass prompts input. You can see in the example that if the prompt doesn't reference the input via a `{{$input}}` template variable it won't use it anyway.
+and the x00xff is the end of send message because I know nothing about sockets
+
+### OSClient expects to receive from the server:
+1. streaming or all at once, the text, followed by 'x00xff'
+2. that's it, no return code, no json wrapper, no {role: assistant, content: str), just the response.
+
+
+
+
+
+4. **the x00ff signals end of messages
+
```

### Comparing `alphawave-0.2.4/README.md` & `alphawave-0.2.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,31 @@
+Metadata-Version: 2.1
+Name: alphawave
+Version: 0.2.5
+Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
+Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
+Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
+Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AlphaWave
+minor bug fixes, OS Client now correctly handles host, port, temperature, top_p, max_tokens
+
+New: SearchCommand will search the web. You will need a google api key.
+See tests/SearchCommandAgentTest.py
+
 AlphaWave is a very opinionated client for interfacing with Large Language Models (LLM). It uses [Promptrix](https://github.com/Stevenic/promptrix) for prompt management and has the following features:
 
 - Supports calling OpenAI and Azure OpenAI hosted models out of the box but a simple plugin model lets you extend AlphaWave to support any LLM.
+- Supports OS LLMs through an OSClient. Currently assumes a server on port 5004, see details below.
 - Promptrix integration means that all prompts are universal and work with either Chat Completion or Text Completion API's.
 - Automatic history management. AlphaWave manages a prompts conversation history and all you have todo is tell it where to store it. It uses an in-memory store by default but a simple plugin interface (provided by Promptrix) lets you store short term memory, like conversation history, anywhere.
 - State-of-the-art response repair logic. AlphaWave lets you provide an optional "response validator" plugin which it will use to validate every response returned from an LLM. Should a response fail validation, AlphaWave will automatically try to get the model to correct its mistake. More below...
 
 ## Automatic Response Repair
 A key goal of AlphaWave is to be the most reliable mechanisms for talking to an LLM on the planet. If you lookup the wikipedia definition for Alpha Waves you see that it's believed that they may be used to help predict mistakes in the human brain. One of the key roles of the AlphaWave library is to help automatically correct for mistakes made by an LLM, leading to more reliable output. It can correct for everything from hallucinations to just malformed output. It does this by using a series of techniques.
 
@@ -92,27 +112,60 @@
 
 # Start chat session
 asyncio.run(chat("Hello, how can I help you?"))
 ```
 
 One of the key features of Promptrix is its ability to proportionally layout prompts, so this prompt has an overall budget of 2000 input tokens. It will give the `SystemMessage` up to 50 tokens, the `UserMessage` up to 450 tokens, and then the `ConversationHistory` gets 100% of the remaining tokens.
 
-Next we just need to call `completePrompt()` on the wave to process the users input (in typescript for now, sorry):
+Once the prompt is formed, we just need to call `completePrompt()` on the wave to process the users input
+
+The  parameter to wave.completePrompt is optional and the wave can also take input directly from memory, but you don't have to pass prompts input. You can see in the example that if the prompt doesn't reference the input via a `{{$input}}` template variable it won't use it anyway.
+
+# Logging
+if you want to see the traffic with the server, the Client constructors (OSClient and OpenAIClient) take a logRequests parameter - False by default, set it to True to see prompts and responses on the console.
+
+# OSClient
+the 'default' way to use Alphawave-py with OpenAI is to use the OpenAI client as in line 49 of the example above. 
+If you want to use your own LLM, you can use instead:
+
+```python
+client = OSClient(apiKey=None)
+```
+
+The current OSClient assumes a server exists on localhost port 5004, using my own unique protocol.
+Not very useful, I know.
+Short term plans include: 
+1. allow specification of the host and port in the client constructor
+2. allow FastChat-like specification of the conversation template (user/assistant/etc). Support for this is already in the OSClient, just need to bring it out to the Constructor
+3. Implementation of a FastChat compatible api. Again, this was running in a dev version of the code, just need to re-insert it now that basic port is stable.
 
-```typescript
-// Route users message to wave
-const result = await wave.completePrompt(input);
-switch (result.status) {
-    case 'success':
-        console.log((result.response as Message).content);
-        break;
-    default:
-        if (result.response) {
-            console.log(`${result.status}: ${result.response}`);
-        } else {
-            console.log(`A result status of '${result.status}' was returned.`);
-        }
-        break;
+## OSClient protocol
+### OSClient sends json to the server:
+```python
+        server_message = {'prompt':prompt, 'temp': temp, 'top_p':top_p, 'max_tokens':max_tokens}
+        smj = json.dumps(server_message)
+        client_socket.sendall(smj.encode('utf-8'))
+        client_socket.sendall(b'x00xff')
+```
+where prompt is a string containing the messages:
+```python
+{
+  "role": "system",
+  "content": "You are an AI assistant that is friendly, kind, and helpful"
+}{
+  "role": "user",
+  "content": "Hi. How are you today?"
 }
 ```
 
-The `input` parameter is optional and the wave can also take input directly from memory, but you don't have to pass prompts input. You can see in the example that if the prompt doesn't reference the input via a `{{$input}}` template variable it won't use it anyway.
+and the x00xff is the end of send message because I know nothing about sockets
+
+### OSClient expects to receive from the server:
+1. streaming or all at once, the text, followed by 'x00xff'
+2. that's it, no return code, no json wrapper, no {role: assistant, content: str), just the response.
+
+
+
+
+
+4. **the x00ff signals end of messages
+
```

### Comparing `alphawave-0.2.4/pyproject.toml` & `alphawave-0.2.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
 
+
 readme = "README.md"
 
 requires-python = ">=3.8"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -24,14 +25,19 @@
 
 dependencies = [
     "promptrix",
     "requests",
     "tiktoken",
     "pyyaml",
     "pyee",
+    "selenium",
+    "wordfreq",
+    "tenacity",	
+    "openai",
+    "nltk",
     'importlib-metadata; python_version<"3.9"',
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/Stevenic/alphawave-py"
 "Bug Tracker" = "https://github.com/Stevenic/alphawave-py/issues"
```

### Comparing `alphawave-0.2.4/src/alphawave/AlphaWave.py` & `alphawave-0.2.5/src/alphawave/AlphaWave.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         elif not input:
             input = ''
 
         try:
             self.emit('beforePrompt', memory, functions, tokenizer, prompt, prompt_options)
             response = await client.completePrompt(memory, functions, tokenizer, prompt, prompt_options)
             self.emit('afterPrompt', memory, functions, tokenizer, prompt, prompt_options, response)
-
             if response['status'] != 'success':
                 return response
 
             if not isinstance(response['message'], dict):
                 response['message'] = {'role': 'assistant', 'content': response['message'] or ''}
 
             self.emit('beforeValidation', memory, functions, tokenizer, response, max_repair_attempts)
```

### Comparing `alphawave-0.2.4/src/alphawave/Colorize.py` & `alphawave-0.2.5/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.5/src/alphawave/DefaultResponseValidator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, Tokenizer
 from alphawave.alphawaveTypes import PromptResponse, Validation, PromptResponseValidator
 import json
+import traceback
 
 class DefaultResponseValidator(PromptResponseValidator):
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: PromptResponse, remaining_attempts) -> Validation:
         self.feedback = response['message']['content'] if isinstance(response['message'], dict) else response.message
         return {
             'type': 'Validation',
             'valid': True,
```

### Comparing `alphawave-0.2.4/src/alphawave/JSONResponseValidator.py` & `alphawave-0.2.5/src/alphawave/JSONResponseValidator.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,22 +104,22 @@
                     path = str(list(e.relative_schema_path)[1:-1]).replace('[','').replace(']',"").replace(', ', ':')
                     if not errors:
                         errors = e
                     template = extract_json_template(self.schema)
                     return {
                         'type': 'Validation',
                         'valid': False,
-                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(errors)}.'# respond using this template: {template}'
+                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(errors)}'#. respond using this template: {template}'
                     }
                 except Exception as e:
                     template = extract_json_template(self.schema)
                     return {
                         'type': 'Validation',
                         'valid': False,
-                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(e)}.'# respond using this template: {template}'
+                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(e)}'#spond using this template: {template}'
                     }      
     
         else:
             # Return the last object
             return {
                 'type': 'Validation',
                 'valid': True,
```

### Comparing `alphawave-0.2.4/src/alphawave/MemoryFork.py` & `alphawave-0.2.5/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave/OSClient.py` & `alphawave-0.2.5/src/alphawave/OSClient.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,69 +8,88 @@
 from promptrix.SystemMessage import SystemMessage
 from promptrix.ConversationHistory import ConversationHistory
 from promptrix.AssistantMessage import AssistantMessage
 
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse
 from alphawave.internalTypes import ChatCompletionRequestMessage, CreateChatCompletionRequest, CreateChatCompletionResponse, CreateCompletionRequest, CreateCompletionResponse
 from alphawave.Colorize import Colorize
-import alphawave.utilityV2 as ut
-import alphawave.LLMClient as client
+import alphawave_pyexts.utilityV2 as ut
+import alphawave_pyexts.LLMClient as client
 
 @dataclass
 class OSClientOptions(PromptCompletionOptions):
-    def __init__(self, apiKey, organization = None, endpoint = None, logRequests = None):
+    def __init__(self, apiKey, model='wizardLM', organization = None, endpoint ='127.0.0.1', port=5004,logRequests =False):
         self.apiKey = apiKey
         self.organization = organization
         self.endpoint = endpoint
+        self.port = port
         self.logRequests = logRequests
-
+        self.model = model
+        
 def update_dataclass(instance, **kwargs):
     for key, value in kwargs.items():
         if hasattr(instance, key):
             setattr(instance, key, value)
+    return instance
 
 def get_values(instance, keys):
     values = []
     for key in keys:
         if hasattr(instance, key):
             values.append(getattr(instance, key))
         else:
             values.append(None)
     return values
 
-        
+def display_options(options):
+    options_dict = options.__dict__
+    print()
+    for item in options_dict.keys():
+        print(item, options_dict[item])
+    print()
+    
 @dataclass
 class Response:
     status_code: int
     text: str
     headers: Dict[str,str] = None
     reason: str = ''
     
 class OSClient(PromptCompletionClient):
     DefaultEndpoint = 'https://api.openai.com'
     UserAgent = 'AlphaWave'
 
     def __init__(self, **kwargs):
-        self.options = OSClientOptions(apiKey=None, organization=None, endpoint= '127.0.0.1', logRequests=False)
+        self.options = OSClientOptions(apiKey=None, organization=None, endpoint= '127.0.0.1', port = 5004, logRequests=False)
         update_dataclass(self.options, **kwargs)
         if self.options.endpoint:
             self.options.endpoint = self.options.endpoint.strip()
             if self.options.endpoint.endswith('/'):
                 self.options.endpoint = self.options.endpoint[:-1]
 
         self._session = requests.Session()
 
     async def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
         if isinstance(options, dict):
             argoptions = options
-            options = PromptCompletionOptions(completion_type = argoptions['completion_type'], model = argoptions['model'])
+            options = PromptCompletionOptions(completion_type = argoptions['completion_type'],
+                                              model = argoptions['model'],
+                                              max_input_tokens = argoptions['max_input_tokens'],
+                                              temperature = argoptions['temperature'],
+                                              top_p = argoptions['top_p'],
+                                              max_tokens = argoptions['max_tokens'],
+                                              stop = argoptions['stop'],
+                                              presence_penalty = argoptions['presence_penalty'],
+                                              frequency_penalty = argoptions['frequency_penalty']
+                                              )
         startTime = time.time()
-        max_input_tokens = 2048
+        max_input_tokens = 1500
         if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
             max_input_tokens = options.max_input_tokens
+        
         if hasattr(options, 'completion_type') and options.completion_type == 'text':
             result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
         if hasattr(options, 'completion_type') and options.completion_type == 'text':
             result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated text completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
             if self.options.logRequests:
@@ -83,43 +102,41 @@
             request = self.copyOptionsToRequest(CreateCompletionRequest({
                 'model': optionsmodel,
                 'prompt': result.output,
             }), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createCompletion(request)
             if self.options.logRequests:
                 print(Colorize.title('RESPONSE:'))
-                print(Colorize.value('statuse', response.status))
+                print(Colorize.value('status', response.status))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
                 print(Colorize.output(response.message))
 
             if response.status == 'success':
                 completion = response.message
                 return {'status': 'success', 'message': completion}
             else:
                 return {'status': 'error', 'message': f"The text completion API returned an error status of {response.status}: {response.message}"}
         else:
             result = await prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
-            self.options.logRequests = True
             if self.options.logRequests:
                 print(Colorize.title('CHAT PROMPT:'))
                 for msg in result.output:
                     if not isinstance(msg, dict):
                         msg = msg.__dict__
                     print(Colorize.output(json.dumps(msg, indent=2)), end='')
                 print()
             request = self.copyOptionsToRequest(CreateChatCompletionRequest(model = options.model, messages =  result.output), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createChatCompletion(request)
-            self.options.logRequests = True
             if self.options.logRequests:
                 print(Colorize.title('CHAT RESPONSE:'))
                 print(Colorize.value('status', response.status))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
-                print(Colorize.output(response))
+                print(Colorize.output(response.message))
 
             if response.status == 'success':
                 completion = response.message
                 return {'status': 'success', 'message': completion}
             else:
                 return {'status': 'error', 'message': f"The chat completion API returned an error status of {response.status}: {response.message}"}
 
@@ -145,14 +162,18 @@
     def post(self, url: str, body: object) -> requests.Response:
         requestHeaders = {
             'Content-Type': 'application/json',
             'User-Agent': self.UserAgent
         }
         result = ''
         try:
-            result = ut.ask_LLM(ut.MODEL, body.messages)
-            runon_idx = result.find(client.USER)
-            if runon_idx > 0:
-                result = result[:runon_idx]
+            result = ut.ask_LLM(self.options.model,
+                                body.messages,
+                                self.options.max_tokens,
+                                self.options.temperature,
+                                self.options.top_p,
+                                self.options.endpoint,
+                                self.options.port
+                                )
         except Exception as e:
             return PromptResponse(status='error',message=str(e))
-        return PromptResponse(status='success', message = {'role':'assistant', 'content': result})
+        return PromptResponse(status='success', message=result)
```

### Comparing `alphawave-0.2.4/src/alphawave/OpenAIClient.py` & `alphawave-0.2.5/src/alphawave/OpenAIClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 print()
 
             request = self.copyOptionsToRequest(CreateChatCompletionRequest(model=options.model, messages=result.output), options,
                                                     ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createChatCompletion(request)
             if self.options['logRequests']:
                 print(Colorize.title('CHAT RESPONSE:'))
-                print(Colorize.value('statuse', response.status_code))
+                print(Colorize.value('status', response.status_code))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
                 print(Colorize.output(response.json()))
 
             if response.status_code < 300:
                 completion = response.json().get('choices')[0]
                 return {'status': 'success', 'message': completion.get('message', {'role': 'assistant', 'content': ''})}
             elif response.status_code == 429:
@@ -148,10 +148,9 @@
         keys = list(jsonbody.keys())
         for key in keys:
             if jsonbody[key] is None:
                 del jsonbody[key]
         result = self._session.post(url, json=jsonbody, headers=requestHeaders)
         if result.status_code < 300:
             completion = result.json().get('choices')[0]
-
         return result
```

### Comparing `alphawave-0.2.4/src/alphawave/RepairTestClient.py` & `alphawave-0.2.5/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave/Response.py` & `alphawave-0.2.5/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave/TestClient.py` & `alphawave-0.2.5/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave/TestClientTest.py` & `alphawave-0.2.5/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.5/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave/internalTypes.py` & `alphawave-0.2.5/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave/jsonParser.py` & `alphawave-0.2.5/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.5/src/alphawave.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.4
+Version: 0.2.5
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AlphaWave
+minor bug fixes, OS Client now correctly handles host, port, temperature, top_p, max_tokens
+
+New: SearchCommand will search the web. You will need a google api key.
+See tests/SearchCommandAgentTest.py
+
 AlphaWave is a very opinionated client for interfacing with Large Language Models (LLM). It uses [Promptrix](https://github.com/Stevenic/promptrix) for prompt management and has the following features:
 
 - Supports calling OpenAI and Azure OpenAI hosted models out of the box but a simple plugin model lets you extend AlphaWave to support any LLM.
+- Supports OS LLMs through an OSClient. Currently assumes a server on port 5004, see details below.
 - Promptrix integration means that all prompts are universal and work with either Chat Completion or Text Completion API's.
 - Automatic history management. AlphaWave manages a prompts conversation history and all you have todo is tell it where to store it. It uses an in-memory store by default but a simple plugin interface (provided by Promptrix) lets you store short term memory, like conversation history, anywhere.
 - State-of-the-art response repair logic. AlphaWave lets you provide an optional "response validator" plugin which it will use to validate every response returned from an LLM. Should a response fail validation, AlphaWave will automatically try to get the model to correct its mistake. More below...
 
 ## Automatic Response Repair
 A key goal of AlphaWave is to be the most reliable mechanisms for talking to an LLM on the planet. If you lookup the wikipedia definition for Alpha Waves you see that it's believed that they may be used to help predict mistakes in the human brain. One of the key roles of the AlphaWave library is to help automatically correct for mistakes made by an LLM, leading to more reliable output. It can correct for everything from hallucinations to just malformed output. It does this by using a series of techniques.
 
@@ -106,27 +112,60 @@
 
 # Start chat session
 asyncio.run(chat("Hello, how can I help you?"))
 ```
 
 One of the key features of Promptrix is its ability to proportionally layout prompts, so this prompt has an overall budget of 2000 input tokens. It will give the `SystemMessage` up to 50 tokens, the `UserMessage` up to 450 tokens, and then the `ConversationHistory` gets 100% of the remaining tokens.
 
-Next we just need to call `completePrompt()` on the wave to process the users input (in typescript for now, sorry):
+Once the prompt is formed, we just need to call `completePrompt()` on the wave to process the users input
+
+The  parameter to wave.completePrompt is optional and the wave can also take input directly from memory, but you don't have to pass prompts input. You can see in the example that if the prompt doesn't reference the input via a `{{$input}}` template variable it won't use it anyway.
+
+# Logging
+if you want to see the traffic with the server, the Client constructors (OSClient and OpenAIClient) take a logRequests parameter - False by default, set it to True to see prompts and responses on the console.
+
+# OSClient
+the 'default' way to use Alphawave-py with OpenAI is to use the OpenAI client as in line 49 of the example above. 
+If you want to use your own LLM, you can use instead:
+
+```python
+client = OSClient(apiKey=None)
+```
+
+The current OSClient assumes a server exists on localhost port 5004, using my own unique protocol.
+Not very useful, I know.
+Short term plans include: 
+1. allow specification of the host and port in the client constructor
+2. allow FastChat-like specification of the conversation template (user/assistant/etc). Support for this is already in the OSClient, just need to bring it out to the Constructor
+3. Implementation of a FastChat compatible api. Again, this was running in a dev version of the code, just need to re-insert it now that basic port is stable.
 
-```typescript
-// Route users message to wave
-const result = await wave.completePrompt(input);
-switch (result.status) {
-    case 'success':
-        console.log((result.response as Message).content);
-        break;
-    default:
-        if (result.response) {
-            console.log(`${result.status}: ${result.response}`);
-        } else {
-            console.log(`A result status of '${result.status}' was returned.`);
-        }
-        break;
+## OSClient protocol
+### OSClient sends json to the server:
+```python
+        server_message = {'prompt':prompt, 'temp': temp, 'top_p':top_p, 'max_tokens':max_tokens}
+        smj = json.dumps(server_message)
+        client_socket.sendall(smj.encode('utf-8'))
+        client_socket.sendall(b'x00xff')
+```
+where prompt is a string containing the messages:
+```python
+{
+  "role": "system",
+  "content": "You are an AI assistant that is friendly, kind, and helpful"
+}{
+  "role": "user",
+  "content": "Hi. How are you today?"
 }
 ```
 
-The `input` parameter is optional and the wave can also take input directly from memory, but you don't have to pass prompts input. You can see in the example that if the prompt doesn't reference the input via a `{{$input}}` template variable it won't use it anyway.
+and the x00xff is the end of send message because I know nothing about sockets
+
+### OSClient expects to receive from the server:
+1. streaming or all at once, the text, followed by 'x00xff'
+2. that's it, no return code, no json wrapper, no {role: assistant, content: str), just the response.
+
+
+
+
+
+4. **the x00ff signals end of messages
+
```

### Comparing `alphawave-0.2.4/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.5/src/alphawave.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 src/alphawave/AlphaWave.py
 src/alphawave/Colorize.py
 src/alphawave/DefaultResponseValidator.py
 src/alphawave/JSONResponseValidator.py
-src/alphawave/LLMClient.py
 src/alphawave/MemoryFork.py
 src/alphawave/OSClient.py
 src/alphawave/OpenAIClient.py
 src/alphawave/RepairTestClient.py
 src/alphawave/Response.py
 src/alphawave/TestClient.py
 src/alphawave/TestClientTest.py
 src/alphawave/__init__.py
 src/alphawave/alphawaveTypes.py
 src/alphawave/internalTypes.py
 src/alphawave/jsonParser.py
-src/alphawave/utilityV2.py
 src/alphawave.egg-info/PKG-INFO
 src/alphawave.egg-info/SOURCES.txt
 src/alphawave.egg-info/dependency_links.txt
 src/alphawave.egg-info/requires.txt
 src/alphawave.egg-info/top_level.txt
 src/alphawave_agents/Agent.py
 src/alphawave_agents/AgentCommandSection.py
@@ -33,10 +31,17 @@
 src/alphawave_agents/MathCommand.py
 src/alphawave_agents/PromptCommand.py
 src/alphawave_agents/SchemaBasedCommand.py
 src/alphawave_agents/SentimentAnalysis.py
 src/alphawave_agents/SetPropertyCommand.py
 src/alphawave_agents/__init__.py
 src/alphawave_agents/agentTypes.py
+src/alphawave_pyexts/LLMClient.py
+src/alphawave_pyexts/SearchCommand.py
+src/alphawave_pyexts/conversation.py
+src/alphawave_pyexts/searchCommand.py
+src/alphawave_pyexts/utilityV2.py
+src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+src/alphawave_pyexts/llmsearch/search_service.py
 tests/testOSClient.py
 tests/testOpenAiClient.py
 tests/testSchema.py
```

### Comparing `alphawave-0.2.4/src/alphawave_agents/Agent.py` & `alphawave-0.2.5/src/alphawave_agents/Agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,14 @@
                     history.append(message)
                     self.memory.set(history_variable, history)
 
                 # Create command validator
                 validator = AgentCommandValidator(self._commands)
 
                 # Create a wave for the prompt
-                #wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.options.prompt_options, memory=memory, functions=functions, tokenizer=tokenizer)
                 wave = AlphaWave(
                     client = self._options['client'],
                     prompt = prompt,
                     prompt_options = self._options['prompt_options'],
                     functions = self._options['functions'],
                     history_variable = history_variable,
                     input_variable = self._options['input_variable'],
```

### Comparing `alphawave-0.2.4/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.5/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.5/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
           command_name = thought['command']['input']['name'] if thought['command']['name'] == 'character' else thought['command']['name']
           #command_name = thought['command']['name']
           if command_name not in self._commands:
               return {
                   'type': 'Validation',
                   'valid': False,
-                  'feedback': 'The command '+thought['command']['name']+f' does not exist. The only commands you have are {self._commands.keys()}'
+                  'feedback': 'The command '+thought['command']['name']+f' does not exist. The only commands you have are {list(self._commands.keys())}'
               }
           
           # Validate that the command input is valid
           command = self._commands[command_name]
           command_validation_result = await command.validate(thought['command']['input'] or {}, memory, functions, tokenizer)
           if not command_validation_result['valid']:
               return command_validation_result
```

### Comparing `alphawave-0.2.4/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.5/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.5/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.5/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.5/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.5/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.5/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.5/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def description(self) -> str:
         return self._description or self._schema.description
 
     @property
     def inputs(self) -> Optional[str]:
         if self._schema.properties:
             properties = self._schema.properties or {}
-            inputs = [f'"{key}":"<{property.get("description", property.get("type", "any"))} value>"' for key, property in properties.items()]
+            inputs = [f'"{key}":"<{property.get("description", property.get("type", "any"))}>"' for key, property in properties.items()]
             return ",".join(inputs)
         else:
             return None
 
     @property
     def output(self) -> Optional[str]:
         return self._schema.returns
```

### Comparing `alphawave-0.2.4/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.5/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.5/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.5/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/tests/testOSClient.py` & `alphawave-0.2.5/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.4/tests/testOpenAiClient.py` & `alphawave-0.2.5/tests/testOpenAiClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         assert_that(str(response['message']).startswith("{ 'role': 'assistant', 'content':"))
         history = self.memory.get('history')
         assert_that(str(history).startswith("[{ 'role': 'user', 'content': 'Hi' },{ 'role': 'assistant', 'content':"))
         input = self.memory.get('input')
         assert_that(input).is_equal_to('Hi')
         self.memory.clear()
         self.memory.set('history', [])
-    """
+
 
     async def test_prompt_completion_with_validation(self):
         wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.prompt_options, memory=self.memory, functions=self.functions, tokenizer=self.tokenizer, validator=self.validator)
         
         self.client.response = 'Hello'
         self.validator.repairAttempts = 1
         response = await wave.completePrompt('Hi')
@@ -259,10 +259,10 @@
         response = await wave.completePrompt('Hi')
         assert_that(response['status']).is_equal_to('success')
         assert_that(str(response['message']).startswith("{ 'role': 'assistant', 'content': {"))
         history = self.memory.get('history')
         assert_that(str(history).startswith("[{ 'role': 'user', 'content': 'Hi' },{ 'role': 'assistant', 'content': {"))
         self.memory.clear()
         self.memory.set('history', [])
-    """
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `alphawave-0.2.4/tests/testSchema.py` & `alphawave-0.2.5/tests/testSchema.py`

 * *Files identical despite different names*


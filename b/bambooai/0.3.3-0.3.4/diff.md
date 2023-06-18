# Comparing `tmp/bambooai-0.3.3.tar.gz` & `tmp/bambooai-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.3.3.tar", last modified: Sun Jun 11 03:18:22 2023, max compression
+gzip compressed data, was "bambooai-0.3.4.tar", last modified: Sun Jun 18 06:48:38 2023, max compression
```

## Comparing `bambooai-0.3.3.tar` & `bambooai-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 03:18:22.286844 bambooai-0.3.3/
--rw-rw-rw-   0        0        0     8017 2023-06-11 03:18:22.286844 bambooai-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     7483 2023-06-11 02:09:10.000000 bambooai-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 03:18:22.254845 bambooai-0.3.3/bambooai/
--rw-rw-rw-   0        0        0       53 2023-06-11 03:03:44.000000 bambooai-0.3.3/bambooai/__init__.py
--rw-rw-rw-   0        0        0    25067 2023-06-11 03:10:50.000000 bambooai-0.3.3/bambooai/bambooai.py
--rw-rw-rw-   0        0        0     8600 2023-06-11 00:55:58.000000 bambooai-0.3.3/bambooai/prompts.py
-drwxrwxrwx   0        0        0        0 2023-06-11 03:18:22.284843 bambooai-0.3.3/bambooai.egg-info/
--rw-rw-rw-   0        0        0     8017 2023-06-11 03:18:22.000000 bambooai-0.3.3/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-06-11 03:18:22.000000 bambooai-0.3.3/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 03:18:22.000000 bambooai-0.3.3/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-11 03:18:22.000000 bambooai-0.3.3/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-11 03:18:22.000000 bambooai-0.3.3/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 03:18:22.287845 bambooai-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      702 2023-06-11 02:48:50.000000 bambooai-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:48:38.720979 bambooai-0.3.4/
+-rw-rw-rw-   0        0        0     7966 2023-06-18 06:48:38.719975 bambooai-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7430 2023-06-18 06:44:01.000000 bambooai-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 06:48:38.686757 bambooai-0.3.4/bambooai/
+-rw-rw-rw-   0        0        0       79 2023-06-18 06:42:14.000000 bambooai-0.3.4/bambooai/__init__.py
+-rw-rw-rw-   0        0        0    26085 2023-06-18 06:39:28.000000 bambooai-0.3.4/bambooai/bambooai.py
+-rw-rw-rw-   0        0        0     1340 2023-06-17 08:09:42.000000 bambooai-0.3.4/bambooai/func_calls.py
+-rw-rw-rw-   0        0        0     6692 2023-06-18 02:03:23.000000 bambooai-0.3.4/bambooai/prompts.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:48:38.718705 bambooai-0.3.4/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     7966 2023-06-18 06:48:38.000000 bambooai-0.3.4/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-18 06:48:38.000000 bambooai-0.3.4/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 06:48:38.000000 bambooai-0.3.4/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-18 06:48:38.000000 bambooai-0.3.4/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 06:48:38.000000 bambooai-0.3.4/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 06:48:38.720979 bambooai-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-06-18 06:43:04.000000 bambooai-0.3.4/setup.py
```

### Comparing `bambooai-0.3.3/PKG-INFO` & `bambooai-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.3.3
+Version: 0.3.4
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,18 @@
 - The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
   - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
 - The received code is then executed to generate an answer or a visualization:
   - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
   - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
 - The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
 - Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+ 
+**Flow chart:**
+
+![](images/flow_chart_3.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -67,18 +71,16 @@
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
 rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
 
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
-flow_diagram: bool - If True, a mermaid diagram will be generated and displayed to complement the answer.
-
 
-e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True, flow_diagram=False)
+e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -101,20 +103,20 @@
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
-
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
-- Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
+- Be sure to monitor your token usage. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
+- Supported models: gpt-3.5-turbo, gpt-3.5-turbo-613, gpt-3.5-turbo-16k, gpt-4, gpt-4-0613.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
```

### Comparing `bambooai-0.3.3/README.md` & `bambooai-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 - The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
   - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
 - The received code is then executed to generate an answer or a visualization:
   - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
   - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
 - The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
 - Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+ 
+**Flow chart:**
+
+![](images/flow_chart_3.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -54,18 +58,16 @@
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
 rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
 
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
-flow_diagram: bool - If True, a mermaid diagram will be generated and displayed to complement the answer.
-
 
-e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True, flow_diagram=False)
+e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -88,20 +90,20 @@
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
-
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
-- Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
+- Be sure to monitor your token usage. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
+- Supported models: gpt-3.5-turbo, gpt-3.5-turbo-613, gpt-3.5-turbo-16k, gpt-4, gpt-4-0613.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
```

### Comparing `bambooai-0.3.3/bambooai/bambooai.py` & `bambooai-0.3.4/bambooai/bambooai.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1567 +1,1631 @@
 00000000: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
 00000010: 6f72 7420 7265 0d0a 696d 706f 7274 2073  ort re..import s
 00000020: 7973 0d0a 696d 706f 7274 2062 6173 6536  ys..import base6
-00000030: 340d 0a66 726f 6d20 636f 6e74 6578 746c  4..from contextl
-00000040: 6962 2069 6d70 6f72 7420 7265 6469 7265  ib import redire
-00000050: 6374 5f73 7464 6f75 740d 0a69 6d70 6f72  ct_stdout..impor
-00000060: 7420 696f 0d0a 696d 706f 7274 2074 696d  t io..import tim
-00000070: 650d 0a69 6d70 6f72 7420 6f70 656e 6169  e..import openai
-00000080: 0d0a 696d 706f 7274 2070 616e 6461 7320  ..import pandas 
-00000090: 6173 2070 640d 0a66 726f 6d20 7465 726d  as pd..from term
-000000a0: 636f 6c6f 7220 696d 706f 7274 2063 6f6c  color import col
-000000b0: 6f72 6564 2c20 6370 7269 6e74 0d0a 6672  ored, cprint..fr
-000000c0: 6f6d 2049 5079 7468 6f6e 2e64 6973 706c  om IPython.displ
-000000d0: 6179 2069 6d70 6f72 7420 6469 7370 6c61  ay import displa
-000000e0: 792c 2049 6d61 6765 2c20 4854 4d4c 0d0a  y, Image, HTML..
-000000f0: 696d 706f 7274 2077 6172 6e69 6e67 730d  import warnings.
-00000100: 0a77 6172 6e69 6e67 732e 6669 6c74 6572  .warnings.filter
-00000110: 7761 726e 696e 6773 2827 6967 6e6f 7265  warnings('ignore
-00000120: 2729 0d0a 6672 6f6d 202e 2069 6d70 6f72  ')..from . impor
-00000130: 7420 7072 6f6d 7074 730d 0a0d 0a63 6c61  t prompts....cla
-00000140: 7373 2042 616d 626f 6f41 493a 0d0a 2020  ss BambooAI:..  
-00000150: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000160: 656c 662c 2064 663a 2070 642e 4461 7461  elf, df: pd.Data
-00000170: 4672 616d 652c 0d0a 2020 2020 2020 2020  Frame,..        
-00000180: 2020 2020 2020 2020 206d 6178 5f63 6f6e           max_con
-00000190: 7665 7273 6174 696f 6e73 3a20 696e 7420  versations: int 
-000001a0: 3d20 3220 2c0d 0a20 2020 2020 2020 2020  = 2 ,..         
-000001b0: 2020 2020 2020 2020 6c6c 6d3a 2073 7472          llm: str
-000001c0: 203d 2027 6770 742d 332e 352d 7475 7262   = 'gpt-3.5-turb
-000001d0: 6f27 2c0d 0a20 2020 2020 2020 2020 2020  o',..           
-000001e0: 2020 2020 2020 6465 6275 673a 2062 6f6f        debug: boo
-000001f0: 6c20 3d20 4661 6c73 652c 200d 0a20 2020  l = False, ..   
-00000200: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00000210: 6e6b 3a20 626f 6f6c 203d 2046 616c 7365  nk: bool = False
-00000220: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-00000230: 2020 2020 206c 6c6d 5f73 7769 7463 683a       llm_switch:
-00000240: 2062 6f6f 6c20 3d20 4661 6c73 652c 200d   bool = False, .
-00000250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000260: 2020 6578 706c 6f72 6174 6f72 793a 2062    exploratory: b
-00000270: 6f6f 6c20 3d20 5472 7565 2c20 0d0a 2020  ool = True, ..  
-00000280: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00000290: 6c6f 775f 6469 6167 7261 6d3a 2062 6f6f  low_diagram: boo
-000002a0: 6c20 3d20 4661 6c73 650d 0a20 2020 2020  l = False..     
-000002b0: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
-000002c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e41  ..        self.A
-000002d0: 5049 5f4b 4559 203d 206f 732e 656e 7669  PI_KEY = os.envi
-000002e0: 726f 6e2e 6765 7428 274f 5045 4e41 495f  ron.get('OPENAI_
-000002f0: 4150 495f 4b45 5927 290d 0a20 2020 2020  API_KEY')..     
-00000300: 2020 2073 656c 662e 4d41 585f 4552 524f     self.MAX_ERRO
-00000310: 525f 434f 5252 4543 5449 4f4e 5320 3d20  R_CORRECTIONS = 
-00000320: 350d 0a20 2020 2020 2020 2023 2053 6574  5..        # Set
-00000330: 2074 6865 206d 6178 696d 756d 206e 756d   the maximum num
-00000340: 6265 7220 6f66 2071 7565 7374 696f 6e2f  ber of question/
-00000350: 616e 7377 6572 2070 6169 7273 2074 6f20  answer pairs to 
-00000360: 6265 206b 6570 7420 696e 2074 6865 2063  be kept in the c
-00000370: 6f6e 7665 7273 6174 696f 6e20 6d65 6d6d  onversation memm
-00000380: 6f72 790d 0a20 2020 2020 2020 2073 656c  ory..        sel
-00000390: 662e 4d41 585f 434f 4e56 4552 5341 5449  f.MAX_CONVERSATI
-000003a0: 4f4e 5320 3d20 286d 6178 5f63 6f6e 7665  ONS = (max_conve
-000003b0: 7273 6174 696f 6e73 2a32 2920 2d20 310d  rsations*2) - 1.
-000003c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000003d0: 2020 2023 2053 746f 7265 2074 6865 206f     # Store the o
-000003e0: 7269 6769 6e61 6c20 6461 7461 6672 616d  riginal datafram
-000003f0: 652e 2054 6869 7320 7769 6c6c 2062 6520  e. This will be 
-00000400: 7573 6564 2074 6f20 7265 7365 7420 7468  used to reset th
-00000410: 6520 6461 7461 6672 616d 6520 6265 666f  e dataframe befo
-00000420: 7265 2065 7865 6375 7469 6e67 2074 6865  re executing the
-00000430: 2063 6f64 650d 0a20 2020 2020 2020 2073   code..        s
-00000440: 656c 662e 6f72 6967 696e 616c 5f64 6620  elf.original_df 
-00000450: 3d20 6466 0d0a 2020 2020 2020 2020 7365  = df..        se
-00000460: 6c66 2e64 6620 3d20 6466 2e63 6f70 7928  lf.df = df.copy(
-00000470: 2920 2023 206d 616b 6520 6120 636f 7079  )  # make a copy
-00000480: 206f 6620 7468 6520 6461 7461 6672 616d   of the datafram
-00000490: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-000004a0: 6466 5f68 6561 6420 3d20 7365 6c66 2e6f  df_head = self.o
-000004b0: 7269 6769 6e61 6c5f 6466 2e68 6561 6428  riginal_df.head(
-000004c0: 3129 0d0a 2020 2020 0d0a 2020 2020 2020  1)..    ..      
-000004d0: 2020 7365 6c66 2e6c 6c6d 203d 206c 6c6d    self.llm = llm
-000004e0: 0d0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
-000004f0: 7468 6520 6465 6275 6720 6d6f 6465 2e20  the debug mode. 
-00000500: 5468 6973 206d 6f64 6520 6973 2054 7275  This mode is Tru
-00000510: 6520 7768 656e 2079 6f75 2077 616e 7420  e when you want 
-00000520: 7468 6520 6d6f 6465 6c20 746f 2064 6562  the model to deb
-00000530: 7567 2074 6865 2063 6f64 6520 616e 6420  ug the code and 
-00000540: 636f 7272 6563 7420 6974 2e0d 0a20 2020  correct it...   
-00000550: 2020 2020 2073 656c 662e 6465 6275 6720       self.debug 
-00000560: 3d20 6465 6275 670d 0a20 2020 2020 2020  = debug..       
-00000570: 2023 2053 6574 2074 6865 206c 6c6d 5f73   # Set the llm_s
-00000580: 7769 7463 6820 6d6f 6465 2e20 5468 6973  witch mode. This
-00000590: 206d 6f64 6520 6973 2054 7275 6520 7768   mode is True wh
-000005a0: 656e 2079 6f75 2077 616e 7420 7468 6520  en you want the 
-000005b0: 6d6f 6465 6c20 746f 2073 7769 7463 6820  model to switch 
-000005c0: 746f 2067 7074 2d34 2066 6f72 2064 6562  to gpt-4 for deb
-000005d0: 7567 6769 6e67 2c20 6572 726f 7220 636f  ugging, error co
-000005e0: 7272 6563 7469 6f6e 2061 6e64 2072 616e  rrection and ran
-000005f0: 6b69 6e67 2e0d 0a20 2020 2020 2020 2073  king...        s
-00000600: 656c 662e 6c6c 6d5f 7377 6974 6368 203d  elf.llm_switch =
-00000610: 206c 6c6d 5f73 7769 7463 680d 0a20 2020   llm_switch..   
-00000620: 2020 2020 2023 2053 6574 2074 6865 2072       # Set the r
-00000630: 616e 6b20 6d6f 6465 2e20 5468 6973 206d  ank mode. This m
-00000640: 6f64 6520 6973 2054 7275 6520 7768 656e  ode is True when
-00000650: 2079 6f75 2077 616e 7420 7468 6520 6d6f   you want the mo
-00000660: 6465 6c20 746f 2072 616e 6b20 7468 6520  del to rank the 
-00000670: 6765 6e65 7261 7465 6420 636f 6465 2e0d  generated code..
-00000680: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
-00000690: 6e6b 203d 2072 616e 6b0d 0a0d 0a20 2020  nk = rank....   
-000006a0: 2020 2020 2023 2053 6574 2074 6865 2065       # Set the e
-000006b0: 7870 6c6f 7261 746f 7279 206d 6f64 652e  xploratory mode.
-000006c0: 2054 6869 7320 6d6f 6465 2069 7320 5472   This mode is Tr
-000006d0: 7565 2077 6865 6e20 796f 7520 7761 6e74  ue when you want
-000006e0: 2074 6865 206d 6f64 656c 2074 6f20 6576   the model to ev
-000006f0: 616c 7561 7465 2074 6865 206f 7269 6769  aluate the origi
-00000700: 6e61 6c20 7072 6f6d 7074 2061 6e64 2062  nal prompt and b
-00000710: 7265 616b 2069 7420 646f 776e 2069 6e20  reak it down in 
-00000720: 6865 7572 6973 7469 6320 616c 676f 7269  heuristic algori
-00000730: 7468 6d2e 0d0a 2020 2020 2020 2020 7365  thm...        se
-00000740: 6c66 2e65 7870 6c6f 7261 746f 7279 203d  lf.exploratory =
-00000750: 2065 7870 6c6f 7261 746f 7279 0d0a 0d0a   exploratory....
-00000760: 2020 2020 2020 2020 2320 5365 7420 7468          # Set th
-00000770: 6520 666c 6f77 5f64 6961 6772 616d 206d  e flow_diagram m
-00000780: 6f64 652e 2054 6869 7320 6d6f 6465 2069  ode. This mode i
-00000790: 7320 5472 7565 2077 6865 6e20 796f 7520  s True when you 
-000007a0: 7761 6e74 2074 6865 206d 6f64 656c 2074  want the model t
-000007b0: 6f20 6765 6e65 7261 7465 2061 2066 6c6f  o generate a flo
-000007c0: 7720 6469 6167 7261 6d2e 0d0a 2020 2020  w diagram...    
-000007d0: 2020 2020 7365 6c66 2e66 6c6f 775f 6469      self.flow_di
-000007e0: 6167 7261 6d20 3d20 666c 6f77 5f64 6961  agram = flow_dia
-000007f0: 6772 616d 0d0a 2020 2020 2020 2020 0d0a  gram..        ..
-00000800: 2020 2020 2020 2020 2320 5072 6f6d 7074          # Prompt
-00000810: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-00000820: 7461 736b 5f65 7661 6c75 6174 696f 6e20  task_evaluation 
-00000830: 3d20 7072 6f6d 7074 732e 7461 736b 5f65  = prompts.task_e
-00000840: 7661 6c75 6174 696f 6e0d 0a20 2020 2020  valuation..     
-00000850: 2020 2073 656c 662e 7379 7374 656d 5f74     self.system_t
-00000860: 6173 6b20 3d20 7072 6f6d 7074 732e 7379  ask = prompts.sy
-00000870: 7374 656d 5f74 6173 6b0d 0a20 2020 2020  stem_task..     
-00000880: 2020 2073 656c 662e 7461 736b 203d 2070     self.task = p
-00000890: 726f 6d70 7473 2e74 6173 6b0d 0a20 2020  rompts.task..   
-000008a0: 2020 2020 2073 656c 662e 6572 726f 725f       self.error_
-000008b0: 636f 7272 6563 745f 7461 736b 203d 2070  correct_task = p
-000008c0: 726f 6d70 7473 2e65 7272 6f72 5f63 6f72  rompts.error_cor
-000008d0: 7265 6374 5f74 6173 6b0d 0a20 2020 2020  rect_task..     
-000008e0: 2020 2073 656c 662e 6465 6275 675f 636f     self.debug_co
-000008f0: 6465 5f74 6173 6b20 3d20 7072 6f6d 7074  de_task = prompt
-00000900: 732e 6465 6275 675f 636f 6465 5f74 6173  s.debug_code_tas
-00000910: 6b20 200d 0a20 2020 2020 2020 2073 656c  k  ..        sel
-00000920: 662e 7261 6e6b 5f61 6e73 7765 7220 3d20  f.rank_answer = 
-00000930: 7072 6f6d 7074 732e 7261 6e6b 5f61 6e73  prompts.rank_ans
-00000940: 7765 720d 0a20 2020 2020 2020 200d 0a20  wer..        .. 
-00000950: 2020 2020 2020 206f 7065 6e61 692e 6170         openai.ap
-00000960: 695f 6b65 7920 3d20 7365 6c66 2e41 5049  i_key = self.API
-00000970: 5f4b 4559 0d0a 2020 2020 2020 2020 2320  _KEY..        # 
-00000980: 496e 6974 6961 6c69 7a65 2074 6865 2074  Initialize the t
-00000990: 6f74 616c 2074 6f6b 656e 7320 7573 6564  otal tokens used
-000009a0: 206c 6973 742e 2054 6869 7320 6c69 7374   list. This list
-000009b0: 2077 696c 6c20 6265 2075 7365 6420 746f   will be used to
-000009c0: 206b 6565 7020 7472 6163 6b20 6f66 2074   keep track of t
-000009d0: 6865 2074 6f74 616c 2074 6f6b 656e 7320  he total tokens 
-000009e0: 7573 6564 2062 7920 7468 6520 6d6f 6465  used by the mode
-000009f0: 6c0d 0a20 2020 2020 2020 2073 656c 662e  l..        self.
-00000a00: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-00000a10: 6420 3d20 5b5d 0d0a 0d0a 2020 2020 6465  d = []....    de
-00000a20: 6620 6d6d 2873 656c 662c 2067 7261 7068  f mm(self, graph
-00000a30: 293a 0d0a 2020 2020 2020 2020 6772 6170  ):..        grap
-00000a40: 6862 7974 6573 203d 2067 7261 7068 2e65  hbytes = graph.e
-00000a50: 6e63 6f64 6528 2261 7363 6969 2229 0d0a  ncode("ascii")..
-00000a60: 2020 2020 2020 2020 6261 7365 3634 5f62          base64_b
-00000a70: 7974 6573 203d 2062 6173 6536 342e 6236  ytes = base64.b6
-00000a80: 3465 6e63 6f64 6528 6772 6170 6862 7974  4encode(graphbyt
-00000a90: 6573 290d 0a20 2020 2020 2020 2062 6173  es)..        bas
-00000aa0: 6536 345f 7374 7269 6e67 203d 2062 6173  e64_string = bas
-00000ab0: 6536 345f 6279 7465 732e 6465 636f 6465  e64_bytes.decode
-00000ac0: 2822 6173 6369 6922 290d 0a20 2020 2020  ("ascii")..     
-00000ad0: 2020 2069 6d67 5f75 726c 203d 2022 6874     img_url = "ht
-00000ae0: 7470 733a 2f2f 6d65 726d 6169 642e 696e  tps://mermaid.in
-00000af0: 6b2f 696d 672f 2220 2b20 6261 7365 3634  k/img/" + base64
-00000b00: 5f73 7472 696e 670d 0a20 2020 2020 2020  _string..       
-00000b10: 2072 6574 7572 6e20 696d 675f 7572 6c0d   return img_url.
-00000b20: 0a0d 0a20 2020 2064 6566 206c 6c6d 5f63  ...    def llm_c
-00000b30: 616c 6c28 7365 6c66 2c20 6d65 7373 6167  all(self, messag
-00000b40: 6573 3a20 7374 722c 2074 656d 7065 7261  es: str, tempera
-00000b50: 7475 7265 3a20 666c 6f61 7420 3d20 302c  ture: float = 0,
-00000b60: 206d 6178 5f74 6f6b 656e 733a 2069 6e74   max_tokens: int
-00000b70: 203d 2032 3030 3029 3a0d 0a20 2020 2020   = 2000):..     
-00000b80: 2020 2072 6573 706f 6e73 6520 3d20 6f70     response = op
-00000b90: 656e 6169 2e43 6861 7443 6f6d 706c 6574  enai.ChatComplet
-00000ba0: 696f 6e2e 6372 6561 7465 280d 0a20 2020  ion.create(..   
-00000bb0: 2020 2020 2020 2020 206d 6f64 656c 3d73           model=s
-00000bc0: 656c 662e 6c6c 6d2c 0d0a 2020 2020 2020  elf.llm,..      
-00000bd0: 2020 2020 2020 6d65 7373 6167 6573 3d6d        messages=m
-00000be0: 6573 7361 6765 732c 0d0a 2020 2020 2020  essages,..      
-00000bf0: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
-00000c00: 653d 7465 6d70 6572 6174 7572 652c 0d0a  e=temperature,..
-00000c10: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-00000c20: 746f 6b65 6e73 3d6d 6178 5f74 6f6b 656e  tokens=max_token
-00000c30: 732c 0d0a 2020 2020 2020 2020 290d 0a0d  s,..        )...
-00000c40: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
-00000c50: 203d 2072 6573 706f 6e73 652e 6368 6f69   = response.choi
-00000c60: 6365 735b 305d 2e6d 6573 7361 6765 2e63  ces[0].message.c
-00000c70: 6f6e 7465 6e74 2e73 7472 6970 2829 0d0a  ontent.strip()..
-00000c80: 2020 2020 2020 2020 746f 6b65 6e73 5f75          tokens_u
-00000c90: 7365 6420 3d20 7265 7370 6f6e 7365 2e75  sed = response.u
-00000ca0: 7361 6765 2e74 6f74 616c 5f74 6f6b 656e  sage.total_token
-00000cb0: 730d 0a0d 0a20 2020 2020 2020 2072 6574  s....        ret
-00000cc0: 7572 6e20 636f 6e74 656e 742c 2074 6f6b  urn content, tok
-00000cd0: 656e 735f 7573 6564 0d0a 2020 2020 0d0a  ens_used..    ..
-00000ce0: 2020 2020 2320 4675 6e63 7469 6f6e 7320      # Functions 
-00000cf0: 746f 2073 616e 6974 697a 6520 7468 6520  to sanitize the 
-00000d00: 6f75 7470 7574 2066 726f 6d20 7468 6520  output from the 
-00000d10: 4c4c 4d0d 0a20 2020 2064 6566 205f 6578  LLM..    def _ex
-00000d20: 7472 6163 745f 636f 6465 2873 656c 662c  tract_code(self,
-00000d30: 7265 7370 6f6e 7365 3a20 7374 722c 2073  response: str, s
-00000d40: 6570 6172 6174 6f72 3a20 7374 7220 3d20  eparator: str = 
-00000d50: 2260 6060 2229 202d 3e20 7374 723a 0d0a  "```") -> str:..
-00000d60: 0d0a 2020 2020 2020 2020 2320 4465 6669  ..        # Defi
-00000d70: 6e65 2061 2062 6c61 636b 6c69 7374 206f  ne a blacklist o
-00000d80: 6620 5079 7468 6f6e 206b 6579 776f 7264  f Python keyword
-00000d90: 7320 616e 6420 6675 6e63 7469 6f6e 7320  s and functions 
-00000da0: 7468 6174 2061 7265 206e 6f74 2061 6c6c  that are not all
-00000db0: 6f77 6564 0d0a 2020 2020 2020 2020 626c  owed..        bl
-00000dc0: 6163 6b6c 6973 7420 3d20 5b27 6f73 272c  acklist = ['os',
-00000dd0: 2773 7562 7072 6f63 6573 7327 2c27 7379  'subprocess','sy
-00000de0: 7327 2c27 6576 616c 272c 2765 7865 6327  s','eval','exec'
-00000df0: 2c27 6669 6c65 272c 2773 6f63 6b65 7427  ,'file','socket'
-00000e00: 2c27 7572 6c6c 6962 272c 0d0a 2020 2020  ,'urllib',..    
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2773 6875 7469 6c27 2c27 7069 636b 6c65  'shutil','pickle
-00000e30: 272c 2763 7479 7065 7327 2c27 6d75 6c74  ','ctypes','mult
-00000e40: 6970 726f 6365 7373 696e 6727 2c27 7465  iprocessing','te
-00000e50: 6d70 6669 6c65 272c 2767 6c6f 6227 2c27  mpfile','glob','
-00000e60: 636f 6465 272c 2770 7479 272c 2763 6f6d  code','pty','com
-00000e70: 6d61 6e64 7327 2c0d 0a20 2020 2020 2020  mands',..       
-00000e80: 2020 2020 2020 2020 2020 2020 2027 7265               're
-00000e90: 7175 6573 7473 272c 2763 6769 272c 2763  quests','cgi','c
-00000ea0: 6769 7462 272c 2778 6d6c 2e65 7472 6565  gitb','xml.etree
-00000eb0: 2e45 6c65 6d65 6e74 5472 6565 272c 2762  .ElementTree','b
-00000ec0: 7569 6c74 696e 7327 0d0a 2020 2020 2020  uiltins'..      
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 5d0d                ].
-00000ee0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000ef0: 2020 2023 2053 6561 7263 6820 666f 7220     # Search for 
-00000f00: 6120 7061 7474 6572 6e20 6265 7477 6565  a pattern betwee
-00000f10: 6e20 3c72 6566 6c65 6374 696f 6e3e 2061  n <reflection> a
-00000f20: 6e64 203c 2f72 6566 6c65 6374 696f 6e3e  nd </reflection>
-00000f30: 2069 6e20 7468 6520 7265 7370 6f6e 7365   in the response
-00000f40: 0d0a 2020 2020 2020 2020 6d61 7463 6820  ..        match 
-00000f50: 3d20 7265 2e73 6561 7263 6828 7222 3c72  = re.search(r"<r
-00000f60: 6566 6c65 6374 696f 6e3e 282e 2a29 3c2f  eflection>(.*)</
-00000f70: 7265 666c 6563 7469 6f6e 3e22 2c20 7265  reflection>", re
-00000f80: 7370 6f6e 7365 2c20 7265 2e44 4f54 414c  sponse, re.DOTAL
-00000f90: 4c29 0d0a 2020 2020 2020 2020 6966 206d  L)..        if m
-00000fa0: 6174 6368 3a0d 0a20 2020 2020 2020 2020  atch:..         
-00000fb0: 2020 2023 2049 6620 6120 6d61 7463 6820     # If a match 
-00000fc0: 6973 2066 6f75 6e64 2c20 6578 7472 6163  is found, extrac
-00000fd0: 7420 7468 6520 7265 666c 6563 7469 6f6e  t the reflection
-00000fe0: 2062 6574 7765 656e 203c 7265 666c 6563   between <reflec
-00000ff0: 7469 6f6e 3e20 616e 6420 3c2f 7265 666c  tion> and </refl
-00001000: 6563 7469 6f6e 3e0d 0a20 2020 2020 2020  ection>..       
-00001010: 2020 2020 2072 6566 6c65 6374 696f 6e20       reflection 
-00001020: 3d20 6d61 7463 682e 6772 6f75 7028 3129  = match.group(1)
-00001030: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00001040: 0a20 2020 2020 2020 2020 2020 2072 6566  .            ref
-00001050: 6c65 6374 696f 6e20 3d20 2222 0d0a 0d0a  lection = ""....
-00001060: 2020 2020 2020 2020 2320 5365 6172 6368          # Search
-00001070: 2066 6f72 2061 2070 6174 7465 726e 2062   for a pattern b
-00001080: 6574 7765 656e 203c 666c 6f77 3e20 616e  etween <flow> an
-00001090: 6420 3c2f 666c 6f77 3e20 696e 2074 6865  d </flow> in the
-000010a0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-000010b0: 2020 206d 6174 6368 203d 2072 652e 7365     match = re.se
-000010c0: 6172 6368 2872 223c 666c 6f77 3e28 2e2a  arch(r"<flow>(.*
-000010d0: 293c 2f66 6c6f 773e 222c 2072 6573 706f  )</flow>", respo
-000010e0: 6e73 652c 2072 652e 444f 5441 4c4c 290d  nse, re.DOTALL).
-000010f0: 0a20 2020 2020 2020 2069 6620 6d61 7463  .        if matc
-00001100: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-00001110: 2320 4966 2061 206d 6174 6368 2069 7320  # If a match is 
-00001120: 666f 756e 642c 2065 7874 7261 6374 2074  found, extract t
-00001130: 6865 2072 6566 6c65 6374 696f 6e20 6265  he reflection be
-00001140: 7477 6565 6e20 3c66 6c6f 773e 2061 6e64  tween <flow> and
-00001150: 203c 2f66 6c6f 773e 0d0a 2020 2020 2020   </flow>..      
-00001160: 2020 2020 2020 666c 6f77 203d 206d 6174        flow = mat
-00001170: 6368 2e67 726f 7570 2831 290d 0a20 2020  ch.group(1)..   
-00001180: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00001190: 2020 2020 2020 2020 666c 6f77 203d 2022          flow = "
-000011a0: 220d 0a0d 0a20 2020 2020 2020 2023 2053  "....        # S
-000011b0: 6561 7263 6820 666f 7220 6120 7061 7474  earch for a patt
-000011c0: 6572 6e20 6265 7477 6565 6e20 3c72 616e  ern between <ran
-000011d0: 6b3e 2061 6e64 203c 2f72 616e 6b3e 2069  k> and </rank> i
-000011e0: 6e20 7468 6520 7265 7370 6f6e 7365 0d0a  n the response..
-000011f0: 2020 2020 2020 2020 6d61 7463 6820 3d20          match = 
-00001200: 7265 2e73 6561 7263 6828 7222 3c72 616e  re.search(r"<ran
-00001210: 6b3e 282e 2a29 3c2f 7261 6e6b 3e22 2c20  k>(.*)</rank>", 
-00001220: 7265 7370 6f6e 7365 290d 0a20 2020 2020  response)..     
-00001230: 2020 2069 6620 6d61 7463 683a 0d0a 2020     if match:..  
-00001240: 2020 2020 2020 2020 2020 2320 4966 2061            # If a
-00001250: 206d 6174 6368 2069 7320 666f 756e 642c   match is found,
-00001260: 2065 7874 7261 6374 2074 6865 2072 6566   extract the ref
-00001270: 6c65 6374 696f 6e20 6265 7477 6565 6e20  lection between 
-00001280: 3c72 616e 6b3e 2061 6e64 203c 2f72 616e  <rank> and </ran
-00001290: 6b3e 0d0a 2020 2020 2020 2020 2020 2020  k>..            
-000012a0: 7261 6e6b 203d 206d 6174 6368 2e67 726f  rank = match.gro
-000012b0: 7570 2831 290d 0a20 2020 2020 2020 2065  up(1)..        e
-000012c0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000012d0: 2020 7261 6e6b 203d 2022 220d 0a0d 0a20    rank = "".... 
-000012e0: 2020 2020 2020 2023 2053 6561 7263 6820         # Search 
-000012f0: 666f 7220 6120 7061 7474 6572 6e20 6265  for a pattern be
-00001300: 7477 6565 6e20 3c63 6f64 653e 2061 6e64  tween <code> and
-00001310: 203c 2f63 6f64 653e 2069 6e20 7468 6520   </code> in the 
-00001320: 6578 7472 6163 7465 6420 636f 6465 0d0a  extracted code..
-00001330: 2020 2020 2020 2020 6d61 7463 6820 3d20          match = 
-00001340: 7265 2e73 6561 7263 6828 7222 3c63 6f64  re.search(r"<cod
-00001350: 653e 282e 2a29 3c2f 636f 6465 3e22 2c20  e>(.*)</code>", 
-00001360: 7265 7370 6f6e 7365 2c20 7265 2e44 4f54  response, re.DOT
-00001370: 414c 4c29 0d0a 2020 2020 2020 2020 6966  ALL)..        if
-00001380: 206d 6174 6368 3a0d 0a20 2020 2020 2020   match:..       
-00001390: 2020 2020 2023 2049 6620 6120 6d61 7463       # If a matc
-000013a0: 6820 6973 2066 6f75 6e64 2c20 6578 7472  h is found, extr
-000013b0: 6163 7420 7468 6520 636f 6465 2062 6574  act the code bet
-000013c0: 7765 656e 203c 636f 6465 3e20 616e 6420  ween <code> and 
-000013d0: 3c2f 636f 6465 3e0d 0a20 2020 2020 2020  </code>..       
-000013e0: 2020 2020 2063 6f64 6520 3d20 6d61 7463       code = matc
-000013f0: 682e 6772 6f75 7028 3129 0d0a 2020 2020  h.group(1)..    
-00001400: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
-00001410: 2072 6573 706f 6e73 6520 636f 6e74 6169   response contai
-00001420: 6e73 2074 6865 2073 6570 6172 6174 6f72  ns the separator
-00001430: 2c20 6578 7472 6163 7420 7468 6520 636f  , extract the co
-00001440: 6465 2062 6c6f 636b 2062 6574 7765 656e  de block between
-00001450: 2074 6865 2073 6570 6172 6174 6f72 730d   the separators.
-00001460: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00001470: 6c65 6e28 636f 6465 2e73 706c 6974 2873  len(code.split(s
-00001480: 6570 6172 6174 6f72 2929 203e 2031 3a0d  eparator)) > 1:.
-00001490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014a0: 2063 6f64 6520 3d20 636f 6465 2e73 706c   code = code.spl
-000014b0: 6974 2873 6570 6172 6174 6f72 295b 315d  it(separator)[1]
-000014c0: 0d0a 0d0a 2020 2020 2020 2020 2320 4966  ....        # If
-000014d0: 2074 6865 2072 6573 706f 6e73 6520 636f   the response co
-000014e0: 6e74 6169 6e73 2074 6865 2073 6570 6172  ntains the separ
-000014f0: 6174 6f72 2c20 6578 7472 6163 7420 7468  ator, extract th
-00001500: 6520 636f 6465 2062 6c6f 636b 2062 6574  e code block bet
-00001510: 7765 656e 2074 6865 2073 6570 6172 6174  ween the separat
-00001520: 6f72 730d 0a20 2020 2020 2020 2069 6620  ors..        if 
-00001530: 6c65 6e28 7265 7370 6f6e 7365 2e73 706c  len(response.spl
-00001540: 6974 2873 6570 6172 6174 6f72 2929 203e  it(separator)) >
-00001550: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-00001560: 2063 6f64 6520 3d20 7265 7370 6f6e 7365   code = response
-00001570: 2e73 706c 6974 2873 6570 6172 6174 6f72  .split(separator
-00001580: 295b 315d 0d0a 2020 2020 2020 2020 2020  )[1]..          
-00001590: 2020 0d0a 2020 2020 2020 2020 2320 5265    ..        # Re
-000015a0: 6d6f 7665 2074 6865 2022 7079 7468 6f6e  move the "python
-000015b0: 2220 6f72 2022 7079 2220 7072 6566 6978  " or "py" prefix
-000015c0: 2069 6620 7072 6573 656e 740d 0a20 2020   if present..   
-000015d0: 2020 2020 2069 6620 7265 2e6d 6174 6368       if re.match
-000015e0: 2872 225e 2870 7974 686f 6e7c 7079 2922  (r"^(python|py)"
-000015f0: 2c20 636f 6465 293a 0d0a 2020 2020 2020  , code):..      
-00001600: 2020 2020 2020 636f 6465 203d 2072 652e        code = re.
-00001610: 7375 6228 7222 5e28 7079 7468 6f6e 7c70  sub(r"^(python|p
-00001620: 7929 222c 2022 222c 2063 6f64 6529 0d0a  y)", "", code)..
-00001630: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
-00001640: 2063 6f64 6520 6973 2062 6574 7765 656e   code is between
-00001650: 2073 696e 676c 6520 6261 636b 7469 636b   single backtick
-00001660: 732c 2065 7874 7261 6374 2074 6865 2063  s, extract the c
-00001670: 6f64 6520 6265 7477 6565 6e20 7468 656d  ode between them
-00001680: 0d0a 2020 2020 2020 2020 6966 2072 652e  ..        if re.
-00001690: 6d61 7463 6828 7222 5e60 2e2a 6024 222c  match(r"^`.*`$",
-000016a0: 2063 6f64 6529 3a0d 0a20 2020 2020 2020   code):..       
-000016b0: 2020 2020 2063 6f64 6520 3d20 7265 2e73       code = re.s
-000016c0: 7562 2872 225e 6028 2e2a 2960 2422 2c20  ub(r"^`(.*)`$", 
-000016d0: 7222 5c31 222c 2063 6f64 6529 0d0a 0d0a  r"\1", code)....
-000016e0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-000016f0: 2061 6e79 2069 6e73 7461 6e63 6573 206f   any instances o
-00001700: 6620 2264 6620 3d20 7064 2e72 6561 645f  f "df = pd.read_
-00001710: 6373 7628 2766 696c 656e 616d 652e 6373  csv('filename.cs
-00001720: 7627 2922 2066 726f 6d20 7468 6520 636f  v')" from the co
-00001730: 6465 0d0a 2020 2020 2020 2020 636f 6465  de..        code
-00001740: 203d 2072 652e 7375 6228 7222 6466 5c73   = re.sub(r"df\s
-00001750: 2a3d 5c73 2a70 645c 2e72 6561 645f 6373  *=\s*pd\.read_cs
-00001760: 765c 2827 2e2a 3f27 282c 2e2a 293f 5c29  v\('.*?'(,.*)?\)
-00001770: 222c 2022 222c 2063 6f64 6529 0d0a 0d0a  ", "", code)....
-00001780: 2020 2020 2020 2020 2320 4465 6669 6e65          # Define
-00001790: 2074 6865 2072 6567 756c 6172 2065 7870   the regular exp
-000017a0: 7265 7373 696f 6e20 7061 7474 6572 6e20  ression pattern 
-000017b0: 746f 206d 6174 6368 2074 6865 2062 6c61  to match the bla
-000017c0: 636b 6c69 7374 2069 7465 6d73 0d0a 2020  cklist items..  
-000017d0: 2020 2020 2020 7061 7474 6572 6e20 3d20        pattern = 
-000017e0: 7222 5e28 2e2a 5c62 2822 202b 2022 7c22  r"^(.*\b(" + "|"
-000017f0: 2e6a 6f69 6e28 626c 6163 6b6c 6973 7429  .join(blacklist)
-00001800: 202b 2072 2229 5c62 2e2a 2924 220d 0a0d   + r")\b.*)$"...
-00001810: 0a20 2020 2020 2020 2023 2052 6570 6c61  .        # Repla
-00001820: 6365 2074 6865 2062 6c61 636b 6c69 7374  ce the blacklist
-00001830: 2069 7465 6d73 2077 6974 6820 636f 6d6d   items with comm
-00001840: 656e 7473 0d0a 2020 2020 2020 2020 636f  ents..        co
-00001850: 6465 203d 2072 652e 7375 6228 7061 7474  de = re.sub(patt
-00001860: 6572 6e2c 2072 2223 206e 6f74 2061 6c6c  ern, r"# not all
-00001870: 6f77 6564 205c 3122 2c20 636f 6465 2c20  owed \1", code, 
-00001880: 666c 6167 733d 7265 2e4d 554c 5449 4c49  flags=re.MULTILI
-00001890: 4e45 290d 0a0d 0a20 2020 2020 2020 2023  NE)....        #
-000018a0: 2052 6574 7572 6e20 7468 6520 636c 6561   Return the clea
-000018b0: 6e65 6420 616e 6420 6578 7472 6163 7465  ned and extracte
-000018c0: 6420 636f 6465 0d0a 2020 2020 2020 2020  d code..        
-000018d0: 7265 7475 726e 2063 6f64 652e 7374 7269  return code.stri
-000018e0: 7028 292c 2072 6566 6c65 6374 696f 6e2e  p(), reflection.
-000018f0: 7374 7269 7028 292c 2066 6c6f 772e 7374  strip(), flow.st
-00001900: 7269 7028 290d 0a20 2020 200d 0a20 2020  rip()..    ..   
-00001910: 2064 6566 205f 6578 7472 6163 745f 7261   def _extract_ra
-00001920: 6e6b 2873 656c 662c 7265 7370 6f6e 7365  nk(self,response
-00001930: 3a20 7374 7229 202d 3e20 7374 723a 0d0a  : str) -> str:..
-00001940: 0d0a 2020 2020 2020 2020 2320 5365 6172  ..        # Sear
-00001950: 6368 2066 6f72 2061 2070 6174 7465 726e  ch for a pattern
-00001960: 2062 6574 7765 656e 203c 7261 6e6b 3e20   between <rank> 
-00001970: 616e 6420 3c2f 7261 6e6b 3e20 696e 2074  and </rank> in t
-00001980: 6865 2072 6573 706f 6e73 650d 0a20 2020  he response..   
-00001990: 2020 2020 206d 6174 6368 203d 2072 652e       match = re.
-000019a0: 7365 6172 6368 2872 223c 7261 6e6b 3e28  search(r"<rank>(
-000019b0: 2e2a 293c 2f72 616e 6b3e 222c 2072 6573  .*)</rank>", res
-000019c0: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
-000019d0: 6966 206d 6174 6368 3a0d 0a20 2020 2020  if match:..     
-000019e0: 2020 2020 2020 2023 2049 6620 6120 6d61         # If a ma
-000019f0: 7463 6820 6973 2066 6f75 6e64 2c20 6578  tch is found, ex
-00001a00: 7472 6163 7420 7468 6520 7265 666c 6563  tract the reflec
-00001a10: 7469 6f6e 2062 6574 7765 656e 203c 7261  tion between <ra
-00001a20: 6e6b 3e20 616e 6420 3c2f 7261 6e6b 3e0d  nk> and </rank>.
-00001a30: 0a20 2020 2020 2020 2020 2020 2072 616e  .            ran
-00001a40: 6b20 3d20 6d61 7463 682e 6772 6f75 7028  k = match.group(
-00001a50: 3129 0d0a 2020 2020 2020 2020 656c 7365  1)..        else
-00001a60: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00001a70: 616e 6b20 3d20 2222 0d0a 0d0a 2020 2020  ank = ""....    
-00001a80: 2020 2020 2320 5265 7475 726e 2074 6865      # Return the
-00001a90: 2063 6c65 616e 6564 2061 6e64 2065 7874   cleaned and ext
-00001aa0: 7261 6374 6564 2063 6f64 650d 0a20 2020  racted code..   
-00001ab0: 2020 2020 2072 6574 7572 6e20 7261 6e6b       return rank
-00001ac0: 2e73 7472 6970 2829 0d0a 2020 2020 0d0a  .strip()..    ..
-00001ad0: 2020 2020 6465 6620 7461 736b 5f65 7661      def task_eva
-00001ae0: 6c28 7365 6c66 2c20 7175 6573 7469 6f6e  l(self, question
-00001af0: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
-00001b00: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
-00001b10: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
-00001b20: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
-00001b30: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
-00001b40: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
-00001b50: 0d0a 2020 2020 2020 2020 6576 616c 5f6d  ..        eval_m
-00001b60: 6573 7361 6765 7320 3d20 5b7b 2272 6f6c  essages = [{"rol
-00001b70: 6522 3a20 2273 7973 7465 6d22 2c20 2263  e": "system", "c
-00001b80: 6f6e 7465 6e74 223a 2073 656c 662e 7461  ontent": self.ta
-00001b90: 736b 5f65 7661 6c75 6174 696f 6e2e 666f  sk_evaluation.fo
-00001ba0: 726d 6174 2871 7565 7374 696f 6e2c 2073  rmat(question, s
-00001bb0: 656c 662e 6466 5f68 6561 642c 297d 5d0d  elf.df_head,)}].
-00001bc0: 0a0d 0a20 2020 2020 2020 2069 6620 2769  ...        if 'i
-00001bd0: 7079 6b65 726e 656c 2720 696e 2073 7973  pykernel' in sys
-00001be0: 2e6d 6f64 756c 6573 3a0d 0a20 2020 2020  .modules:..     
-00001bf0: 2020 2020 2020 2023 204a 7570 7974 6572         # Jupyter
-00001c00: 206e 6f74 6562 6f6f 6b20 6f72 2069 7079   notebook or ipy
-00001c10: 7468 6f6e 0d0a 2020 2020 2020 2020 2020  thon..          
-00001c20: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
-00001c30: 273c 7020 7374 796c 653d 2263 6f6c 6f72  '<p style="color
-00001c40: 3a6d 6167 656e 7461 3b22 3e5c 6e43 616c  :magenta;">\nCal
-00001c50: 6c69 6e67 204d 6f64 656c 3a20 7b73 656c  ling Model: {sel
-00001c60: 662e 6c6c 6d7d 3c2f 703e 2729 290d 0a20  f.llm}</p>')).. 
-00001c70: 2020 2020 2020 2020 2020 2064 6973 706c             displ
-00001c80: 6179 2848 544d 4c28 6627 3c70 3e3c 6220  ay(HTML(f'<p><b 
-00001c90: 7374 796c 653d 2263 6f6c 6f72 3a6d 6167  style="color:mag
-00001ca0: 656e 7461 3b22 3e54 7279 696e 6720 746f  enta;">Trying to
-00001cb0: 2064 6574 6572 6d69 6e65 2074 6865 2062   determine the b
-00001cc0: 6573 7420 6d65 7468 6f64 2074 6f20 616e  est method to an
-00001cd0: 616c 7973 6520 796f 7572 2064 6174 612c  alyse your data,
-00001ce0: 2070 6c65 6173 6520 7761 6974 2e2e 2e3c   please wait...<
-00001cf0: 2f62 3e3c 2f70 3e3c 6272 3e27 2929 0d0a  /b></p><br>'))..
-00001d00: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00001d10: 2020 2020 2020 2020 2020 2023 204f 7468             # Oth
-00001d20: 6572 2065 6e76 6972 6f6e 6d65 6e74 2028  er environment (
-00001d30: 6c69 6b65 2074 6572 6d69 6e61 6c29 0d0a  like terminal)..
-00001d40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00001d50: 7428 636f 6c6f 7265 6428 6622 5c6e 3e20  t(colored(f"\n> 
-00001d60: 4361 6c6c 696e 6720 4d6f 6465 6c3a 207b  Calling Model: {
-00001d70: 7365 6c66 2e6c 6c6d 7d22 2c20 226d 6167  self.llm}", "mag
-00001d80: 656e 7461 2229 290d 0a20 2020 2020 2020  enta"))..       
-00001d90: 2020 2020 2063 7072 696e 7428 6622 5c6e       cprint(f"\n
-00001da0: 3e20 5472 7969 6e67 2074 6f20 6465 7465  > Trying to dete
-00001db0: 726d 696e 6520 7468 6520 6265 7374 206d  rmine the best m
-00001dc0: 6574 686f 6420 746f 2061 6e61 6c79 7365  ethod to analyse
-00001dd0: 2079 6f75 7220 6461 7461 2c20 706c 6561   your data, plea
-00001de0: 7365 2077 6169 742e 2e2e 5c6e 222c 2027  se wait...\n", '
-00001df0: 6d61 6765 6e74 6127 2c20 6174 7472 733d  magenta', attrs=
-00001e00: 5b27 626f 6c64 275d 290d 0a0d 0a20 2020  ['bold'])....   
-00001e10: 2020 2020 2023 2046 756e 6374 696f 6e20       # Function 
-00001e20: 746f 2064 6973 706c 6179 2072 6573 756c  to display resul
-00001e30: 7473 206e 6963 656c 790d 0a20 2020 2020  ts nicely..     
-00001e40: 2020 2064 6566 2064 6973 706c 6179 5f74     def display_t
-00001e50: 6173 6b28 7461 736b 293a 0d0a 2020 2020  ask(task):..    
-00001e60: 2020 2020 2020 2020 6966 2027 6970 796b          if 'ipyk
-00001e70: 6572 6e65 6c27 2069 6e20 7379 732e 6d6f  ernel' in sys.mo
-00001e80: 6475 6c65 733a 0d0a 2020 2020 2020 2020  dules:..        
-00001e90: 2020 2020 2020 2020 2320 4a75 7079 7465          # Jupyte
-00001ea0: 7220 6e6f 7465 626f 6f6b 206f 7220 6970  r notebook or ip
-00001eb0: 7974 686f 6e0d 0a20 2020 2020 2020 2020  ython..         
-00001ec0: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
-00001ed0: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
-00001ee0: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
-00001ef0: 4920 6861 7665 2063 7265 6174 6564 2074  I have created t
-00001f00: 6865 2066 6f6c 6c6f 7769 6e67 2074 6173  he following tas
-00001f10: 6b20 6c69 7374 2c20 616e 6420 7769 6c6c  k list, and will
-00001f20: 206e 6f77 2074 7279 2074 6f20 6578 7072   now try to expr
-00001f30: 6573 7320 6974 2069 6e20 636f 6465 3a3c  ess it in code:<
-00001f40: 2f62 3e3c 6272 3e3c 7072 6520 7374 796c  /b><br><pre styl
-00001f50: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b22  e="color:black;"
-00001f60: 3e3c 623e 7b74 6173 6b7d 3c2f 623e 3c2f  ><b>{task}</b></
-00001f70: 7072 653e 3c2f 703e 3c62 723e 2729 290d  pre></p><br>')).
-00001f80: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00001f90: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001fa0: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
-00001fb0: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
-00001fc0: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
-00001fd0: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
-00001fe0: 6622 5c6e 5461 736b 3a5c 6e7b 7461 736b  f"\nTask:\n{task
-00001ff0: 7d5c 6e22 2c20 276d 6167 656e 7461 272c  }\n", 'magenta',
-00002000: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
-00002010: 0d0a 0d0a 2020 2020 2020 2020 2320 4361  ....        # Ca
-00002020: 6c6c 2074 6865 204f 7065 6e41 4920 4150  ll the OpenAI AP
-00002030: 4920 616e 6420 6861 6e64 6c65 2072 6174  I and handle rat
-00002040: 6520 6c69 6d69 7420 6572 726f 7273 0d0a  e limit errors..
-00002050: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00002060: 2020 2020 2020 2020 2020 6c6c 6d5f 7265            llm_re
-00002070: 7370 6f6e 7365 2c20 746f 6b65 6e73 5f75  sponse, tokens_u
-00002080: 7365 6420 3d20 7365 6c66 2e6c 6c6d 5f63  sed = self.llm_c
-00002090: 616c 6c28 6576 616c 5f6d 6573 7361 6765  all(eval_message
-000020a0: 732c 7465 6d70 6572 6174 7572 653d 3029  s,temperature=0)
-000020b0: 2023 2068 6967 6865 7220 7465 6d70 6572   # higher temper
-000020c0: 6174 7572 6520 7265 7375 6c74 7320 696e  ature results in
-000020d0: 206d 6f72 6520 2263 7265 6174 6976 6522   more "creative"
-000020e0: 2061 6e73 7765 7273 2028 736f 6d65 7469   answers (someti
-000020f0: 6d65 7320 746f 6f20 6372 6561 7469 7665  mes too creative
-00002100: 203a 2d29 290d 0a20 2020 2020 2020 2020   :-))..         
-00002110: 2020 200d 0a20 2020 2020 2020 2065 7863     ..        exc
-00002120: 6570 7420 6f70 656e 6169 2e65 7272 6f72  ept openai.error
-00002130: 2e52 6174 654c 696d 6974 4572 726f 723a  .RateLimitError:
-00002140: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00002150: 696e 7428 0d0a 2020 2020 2020 2020 2020  int(..          
-00002160: 2020 2020 2020 2254 6865 204f 7065 6e41        "The OpenA
-00002170: 4920 4150 4920 7261 7465 206c 696d 6974  I API rate limit
-00002180: 2068 6173 2062 6565 6e20 6578 6365 6564   has been exceed
-00002190: 6564 2e20 5761 6974 696e 6720 3130 2073  ed. Waiting 10 s
-000021a0: 6563 6f6e 6473 2061 6e64 2074 7279 696e  econds and tryin
-000021b0: 6720 6167 6169 6e2e 220d 0a20 2020 2020  g again."..     
-000021c0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000021d0: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-000021e0: 2831 3029 0d0a 2020 2020 2020 2020 2020  (10)..          
-000021f0: 2020 6c6c 6d5f 7265 7370 6f6e 7365 2c20    llm_response, 
-00002200: 746f 6b65 6e73 5f75 7365 6420 3d20 7365  tokens_used = se
-00002210: 6c66 2e6c 6c6d 5f63 616c 6c28 6576 616c  lf.llm_call(eval
-00002220: 5f6d 6573 7361 6765 7329 0d0a 0d0a 2020  _messages)....  
-00002230: 2020 2020 2020 7461 736b 203d 206c 6c6d        task = llm
-00002240: 5f72 6573 706f 6e73 650d 0a20 2020 2020  _response..     
-00002250: 2020 200d 0a20 2020 2020 2020 2064 6973     ..        dis
-00002260: 706c 6179 5f74 6173 6b28 7461 736b 290d  play_task(task).
-00002270: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00002280: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-00002290: 642e 6170 7065 6e64 2874 6f6b 656e 735f  d.append(tokens_
-000022a0: 7573 6564 290d 0a0d 0a20 2020 2020 2020  used)....       
-000022b0: 2072 6574 7572 6e20 7461 736b 0d0a 0d0a   return task....
-000022c0: 2020 2020 6465 6620 6465 6275 675f 636f      def debug_co
-000022d0: 6465 2873 656c 662c 636f 6465 2c71 7565  de(self,code,que
-000022e0: 7374 696f 6e29 3a0d 0a20 2020 2020 2020  stion):..       
-000022f0: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
-00002300: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
-00002310: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
-00002320: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
-00002330: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
-00002340: 0d0a 2020 2020 2020 2020 6465 6275 675f  ..        debug_
-00002350: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
-00002360: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
-00002370: 636f 6e74 656e 7422 3a20 7365 6c66 2e64  content": self.d
-00002380: 6562 7567 5f63 6f64 655f 7461 736b 2e66  ebug_code_task.f
-00002390: 6f72 6d61 7428 636f 6465 2c71 7565 7374  ormat(code,quest
-000023a0: 696f 6e29 7d5d 0d0a 0d0a 2020 2020 2020  ion)}]....      
-000023b0: 2020 6966 2027 6970 796b 6572 6e65 6c27    if 'ipykernel'
-000023c0: 2069 6e20 7379 732e 6d6f 6475 6c65 733a   in sys.modules:
-000023d0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000023e0: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
-000023f0: 206f 7220 6970 7974 686f 6e0d 0a20 2020   or ipython..   
-00002400: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00002410: 2848 544d 4c28 6627 3c70 2073 7479 6c65  (HTML(f'<p style
-00002420: 3d22 636f 6c6f 723a 6d61 6765 6e74 613b  ="color:magenta;
-00002430: 223e 5c6e 4361 6c6c 696e 6720 4d6f 6465  ">\nCalling Mode
-00002440: 6c3a 207b 7365 6c66 2e6c 6c6d 7d3c 2f70  l: {self.llm}</p
-00002450: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
-00002460: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
-00002470: 273c 703e 3c62 2073 7479 6c65 3d22 636f  '<p><b style="co
-00002480: 6c6f 723a 6d61 6765 6e74 613b 223e 4920  lor:magenta;">I 
-00002490: 6861 7665 2072 6563 6569 7665 6420 7468  have received th
-000024a0: 6520 6669 7273 7420 7665 7273 696f 6e20  e first version 
-000024b0: 6f66 2074 6865 2063 6f64 652e 2049 2061  of the code. I a
-000024c0: 6d20 7365 6e64 696e 6720 6974 2062 6163  m sending it bac
-000024d0: 6b20 746f 204c 4c4d 2074 6f20 6765 7420  k to LLM to get 
-000024e0: 6974 2063 6865 636b 6564 2066 6f72 2061  it checked for a
-000024f0: 6e79 2065 7272 6f72 732c 2062 7567 7320  ny errors, bugs 
-00002500: 6f72 2069 6e63 6f6e 7369 7374 656e 6369  or inconsistenci
-00002510: 6573 2c20 616e 6420 636f 7272 6563 7469  es, and correcti
-00002520: 6f6e 2069 6620 6e65 6365 7373 6172 792e  on if necessary.
-00002530: 2050 6c65 6173 6520 7761 6974 2e2e 2e3c   Please wait...<
-00002540: 2f62 3e3c 2f70 3e3c 6272 3e27 2929 0d0a  /b></p><br>'))..
-00002550: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00002560: 2020 2020 2020 2020 2020 2023 204f 7468             # Oth
-00002570: 6572 2065 6e76 6972 6f6e 6d65 6e74 2028  er environment (
-00002580: 6c69 6b65 2074 6572 6d69 6e61 6c29 0d0a  like terminal)..
-00002590: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000025a0: 7428 636f 6c6f 7265 6428 6622 5c6e 3e20  t(colored(f"\n> 
-000025b0: 4361 6c6c 696e 6720 4d6f 6465 6c3a 207b  Calling Model: {
-000025c0: 7365 6c66 2e6c 6c6d 7d22 2c20 226d 6167  self.llm}", "mag
-000025d0: 656e 7461 2229 290d 0a20 2020 2020 2020  enta"))..       
-000025e0: 2020 2020 2063 7072 696e 7428 6622 5c6e       cprint(f"\n
-000025f0: 3e20 4920 6861 7665 2072 6563 6569 7665  > I have receive
-00002600: 6420 7468 6520 6669 7273 7420 7665 7273  d the first vers
-00002610: 696f 6e20 6f66 2074 6865 2063 6f64 652e  ion of the code.
-00002620: 2049 2061 6d20 7365 6e64 696e 6720 6974   I am sending it
-00002630: 2062 6163 6b20 746f 204c 4c4d 2074 6f20   back to LLM to 
-00002640: 6765 7420 6974 2063 6865 636b 6564 2066  get it checked f
-00002650: 6f72 2061 6e79 2065 7272 6f72 732c 2062  or any errors, b
-00002660: 7567 7320 6f72 2069 6e63 6f6e 7369 7374  ugs or inconsist
-00002670: 656e 6369 6573 2c20 616e 6420 636f 7272  encies, and corr
-00002680: 6563 7469 6f6e 2069 6620 6e65 6365 7373  ection if necess
-00002690: 6172 792e 2050 6c65 6173 6520 7761 6974  ary. Please wait
-000026a0: 2e2e 2e5c 6e22 2c20 276d 6167 656e 7461  ...\n", 'magenta
-000026b0: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
-000026c0: 5d29 0d0a 0d0a 2020 2020 2020 2020 2320  ])....        # 
-000026d0: 4675 6e63 7469 6f6e 2074 6f20 6469 7370  Function to disp
-000026e0: 6c61 7920 7265 7375 6c74 7320 6e69 6365  lay results nice
-000026f0: 6c79 0d0a 2020 2020 2020 2020 6465 6620  ly..        def 
-00002700: 6469 7370 6c61 795f 7461 736b 2864 6562  display_task(deb
-00002710: 7567 5f69 6e73 6967 6874 293a 0d0a 2020  ug_insight):..  
-00002720: 2020 2020 2020 2020 2020 6966 2027 6970            if 'ip
-00002730: 796b 6572 6e65 6c27 2069 6e20 7379 732e  ykernel' in sys.
-00002740: 6d6f 6475 6c65 733a 0d0a 2020 2020 2020  modules:..      
-00002750: 2020 2020 2020 2020 2020 2320 4a75 7079            # Jupy
-00002760: 7465 7220 6e6f 7465 626f 6f6b 206f 7220  ter notebook or 
-00002770: 6970 7974 686f 6e0d 0a20 2020 2020 2020  ipython..       
-00002780: 2020 2020 2020 2020 2064 6973 706c 6179           display
-00002790: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
-000027a0: 796c 653d 2263 6f6c 6f72 3a62 6c75 653b  yle="color:blue;
-000027b0: 223e 4920 6861 7665 2066 696e 6973 6865  ">I have finishe
-000027c0: 6420 6465 6275 6767 696e 6720 7468 6520  d debugging the 
-000027d0: 636f 6465 2c20 6265 6c6f 7720 6172 6520  code, below are 
-000027e0: 6d79 2074 686f 7567 6874 733a 3c2f 623e  my thoughts:</b>
-000027f0: 3c62 723e 3c70 7265 2073 7479 6c65 3d22  <br><pre style="
-00002800: 636f 6c6f 723a 626c 6163 6b3b 2077 6869  color:black; whi
-00002810: 7465 2d73 7061 6365 3a20 7072 652d 7772  te-space: pre-wr
-00002820: 6170 3b20 666f 6e74 2d77 6569 6768 743a  ap; font-weight:
-00002830: 2062 6f6c 643b 223e 7b64 6562 7567 5f69   bold;">{debug_i
-00002840: 6e73 6967 6874 7d3c 2f70 7265 3e3c 2f70  nsight}</pre></p
-00002850: 3e3c 6272 3e27 2929 0d0a 2020 2020 2020  ><br>'))..      
-00002860: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
-00002870: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
-00002880: 7479 6c65 3d22 636f 6c6f 723a 6d61 6765  tyle="color:mage
-00002890: 6e74 613b 223e 4920 616d 2070 726f 6365  nta;">I am proce
-000028a0: 6564 696e 6720 746f 2074 6865 2065 7865  eding to the exe
-000028b0: 6375 7469 6f6e 2e2e 2e3c 2f62 3e3c 2f70  cution...</b></p
-000028c0: 3e3c 6272 3e27 2929 0d0a 2020 2020 2020  ><br>'))..      
-000028d0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000028e0: 2020 2020 2020 2020 2020 2020 2023 204f               # O
-000028f0: 7468 6572 2065 6e76 6972 6f6e 6d65 6e74  ther environment
-00002900: 2028 6c69 6b65 2074 6572 6d69 6e61 6c29   (like terminal)
-00002910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002920: 2020 6370 7269 6e74 2866 225c 6e3e 2049    cprint(f"\n> I
-00002930: 2068 6176 6520 6669 6e69 7368 6564 2064   have finished d
-00002940: 6562 7567 6769 6e67 2074 6865 2063 6f64  ebugging the cod
-00002950: 652c 2062 656c 6f77 2061 7265 206d 7920  e, below are my 
-00002960: 7468 6f75 6768 7473 3a5c 6e7b 6465 6275  thoughts:\n{debu
-00002970: 675f 696e 7369 6768 747d 5c6e 222c 2027  g_insight}\n", '
-00002980: 6d61 6765 6e74 6127 2c20 6174 7472 733d  magenta', attrs=
-00002990: 5b27 626f 6c64 275d 290d 0a20 2020 2020  ['bold'])..     
-000029a0: 2020 2020 2020 2020 2020 2063 7072 696e             cprin
-000029b0: 7428 6622 5c6e 3e20 4920 616d 2070 726f  t(f"\n> I am pro
-000029c0: 6365 6564 696e 6720 746f 2074 6865 2065  ceeding to the e
-000029d0: 7865 6375 7469 6f6e 2e2e 2e5c 6e22 2c20  xecution...\n", 
-000029e0: 276d 6167 656e 7461 272c 2061 7474 7273  'magenta', attrs
-000029f0: 3d5b 2762 6f6c 6427 5d29 0d0a 0d0a 2020  =['bold'])....  
-00002a00: 2020 2020 2020 2320 4361 6c6c 2074 6865        # Call the
-00002a10: 204f 7065 6e41 4920 4150 4920 616e 6420   OpenAI API and 
-00002a20: 6861 6e64 6c65 2072 6174 6520 6c69 6d69  handle rate limi
-00002a30: 7420 6572 726f 7273 0d0a 2020 2020 2020  t errors..      
-00002a40: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00002a50: 2020 2020 6c6c 6d5f 7265 7370 6f6e 7365      llm_response
-00002a60: 2c20 746f 6b65 6e73 5f75 7365 6420 3d20  , tokens_used = 
-00002a70: 7365 6c66 2e6c 6c6d 5f63 616c 6c28 6465  self.llm_call(de
-00002a80: 6275 675f 6d65 7373 6167 6573 2c74 656d  bug_messages,tem
-00002a90: 7065 7261 7475 7265 3d30 2920 2320 6869  perature=0) # hi
-00002aa0: 6768 6572 2074 656d 7065 7261 7475 7265  gher temperature
-00002ab0: 2072 6573 756c 7473 2069 6e20 6d6f 7265   results in more
-00002ac0: 2022 6372 6561 7469 7665 2220 616e 7377   "creative" answ
-00002ad0: 6572 7320 2873 6f6d 6574 696d 6573 2074  ers (sometimes t
-00002ae0: 6f6f 2063 7265 6174 6976 6520 3a2d 2929  oo creative :-))
-00002af0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00002b00: 2020 2020 2020 2020 6578 6365 7074 206f          except o
-00002b10: 7065 6e61 692e 6572 726f 722e 5261 7465  penai.error.Rate
-00002b20: 4c69 6d69 7445 7272 6f72 3a0d 0a20 2020  LimitError:..   
-00002b30: 2020 2020 2020 2020 2070 7269 6e74 280d           print(.
-00002b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b50: 2022 5468 6520 4f70 656e 4149 2041 5049   "The OpenAI API
-00002b60: 2072 6174 6520 6c69 6d69 7420 6861 7320   rate limit has 
-00002b70: 6265 656e 2065 7863 6565 6465 642e 2057  been exceeded. W
-00002b80: 6169 7469 6e67 2031 3020 7365 636f 6e64  aiting 10 second
-00002b90: 7320 616e 6420 7472 7969 6e67 2061 6761  s and trying aga
-00002ba0: 696e 2e22 0d0a 2020 2020 2020 2020 2020  in."..          
-00002bb0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00002bc0: 2074 696d 652e 736c 6565 7028 3130 290d   time.sleep(10).
-00002bd0: 0a20 2020 2020 2020 2020 2020 206c 6c6d  .            llm
-00002be0: 5f72 6573 706f 6e73 652c 2074 6f6b 656e  _response, token
-00002bf0: 735f 7573 6564 203d 2073 656c 662e 6c6c  s_used = self.ll
-00002c00: 6d5f 6361 6c6c 2864 6562 7567 5f6d 6573  m_call(debug_mes
-00002c10: 7361 6765 7329 0d0a 2020 2020 2020 2020  sages)..        
-00002c20: 0d0a 2020 2020 2020 2020 2320 4578 7472  ..        # Extr
-00002c30: 6163 7420 7468 6520 636f 6465 2066 726f  act the code fro
-00002c40: 6d20 7468 6520 4150 4920 7265 7370 6f6e  m the API respon
-00002c50: 7365 0d0a 2020 2020 2020 2020 6465 6275  se..        debu
-00002c60: 6767 6564 5f63 6f64 652c 6465 6275 675f  gged_code,debug_
-00002c70: 696e 7369 6768 742c 666c 6f77 203d 2073  insight,flow = s
-00002c80: 656c 662e 5f65 7874 7261 6374 5f63 6f64  elf._extract_cod
-00002c90: 6528 6c6c 6d5f 7265 7370 6f6e 7365 2920  e(llm_response) 
-00002ca0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002cb0: 6469 7370 6c61 795f 7461 736b 2864 6562  display_task(deb
-00002cc0: 7567 5f69 6e73 6967 6874 290d 0a0d 0a20  ug_insight).... 
-00002cd0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-00002ce0: 6c5f 746f 6b65 6e73 5f75 7365 642e 6170  l_tokens_used.ap
-00002cf0: 7065 6e64 2874 6f6b 656e 735f 7573 6564  pend(tokens_used
-00002d00: 290d 0a0d 0a20 2020 2020 2020 2072 6574  )....        ret
-00002d10: 7572 6e20 6465 6275 6767 6564 5f63 6f64  urn debugged_cod
-00002d20: 650d 0a0d 0a20 2020 2064 6566 2072 616e  e....    def ran
-00002d30: 6b5f 636f 6465 2873 656c 662c 636f 6465  k_code(self,code
-00002d40: 2c71 7565 7374 696f 6e29 3a0d 0a20 2020  ,question):..   
-00002d50: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
-00002d60: 6520 7468 6520 6d65 7373 6167 6573 206c  e the messages l
-00002d70: 6973 7420 7769 7468 2061 2073 7973 7465  ist with a syste
-00002d80: 6d20 6d65 7373 6167 6520 636f 6e74 6169  m message contai
-00002d90: 6e69 6e67 2074 6865 2074 6173 6b20 7072  ning the task pr
-00002da0: 6f6d 7074 0d0a 2020 2020 2020 2020 7261  ompt..        ra
-00002db0: 6e6b 5f6d 6573 7361 6765 7320 3d20 5b7b  nk_messages = [{
-00002dc0: 2272 6f6c 6522 3a20 2273 7973 7465 6d22  "role": "system"
-00002dd0: 2c20 2263 6f6e 7465 6e74 223a 2073 656c  , "content": sel
-00002de0: 662e 7261 6e6b 5f61 6e73 7765 722e 666f  f.rank_answer.fo
-00002df0: 726d 6174 2863 6f64 652c 7175 6573 7469  rmat(code,questi
-00002e00: 6f6e 297d 5d0d 0a0d 0a20 2020 2020 2020  on)}]....       
-00002e10: 2069 6620 2769 7079 6b65 726e 656c 2720   if 'ipykernel' 
-00002e20: 696e 2073 7973 2e6d 6f64 756c 6573 3a0d  in sys.modules:.
-00002e30: 0a20 2020 2020 2020 2020 2020 2023 204a  .            # J
-00002e40: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
-00002e50: 6f72 2069 7079 7468 6f6e 0d0a 2020 2020  or ipython..    
-00002e60: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-00002e70: 4854 4d4c 2866 273c 7020 7374 796c 653d  HTML(f'<p style=
-00002e80: 2263 6f6c 6f72 3a6d 6167 656e 7461 3b22  "color:magenta;"
-00002e90: 3e5c 6e43 616c 6c69 6e67 204d 6f64 656c  >\nCalling Model
-00002ea0: 3a20 7b73 656c 662e 6c6c 6d7d 3c2f 703e  : {self.llm}</p>
-00002eb0: 2729 290d 0a20 2020 2020 2020 2020 2020  '))..           
-00002ec0: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
-00002ed0: 3c70 3e3c 6220 7374 796c 653d 2263 6f6c  <p><b style="col
-00002ee0: 6f72 3a6d 6167 656e 7461 3b22 3e49 2061  or:magenta;">I a
-00002ef0: 6d20 676f 696e 6720 746f 2065 7661 6c75  m going to evalu
-00002f00: 6174 6520 616e 6420 7261 6e6b 2074 6865  ate and rank the
-00002f10: 2061 6e73 7765 722e 2050 6c65 6173 6520   answer. Please 
-00002f20: 7761 6974 2e2e 2e3c 2f62 3e3c 2f70 3e3c  wait...</b></p><
-00002f30: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
-00002f40: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00002f50: 2020 2023 204f 7468 6572 2065 6e76 6972     # Other envir
-00002f60: 6f6e 6d65 6e74 2028 6c69 6b65 2074 6572  onment (like ter
-00002f70: 6d69 6e61 6c29 0d0a 2020 2020 2020 2020  minal)..        
-00002f80: 2020 2020 7072 696e 7428 636f 6c6f 7265      print(colore
-00002f90: 6428 6622 5c6e 3e20 4361 6c6c 696e 6720  d(f"\n> Calling 
-00002fa0: 4d6f 6465 6c3a 207b 7365 6c66 2e6c 6c6d  Model: {self.llm
-00002fb0: 7d22 2c20 226d 6167 656e 7461 2229 290d  }", "magenta")).
-00002fc0: 0a20 2020 2020 2020 2020 2020 2063 7072  .            cpr
-00002fd0: 696e 7428 6622 5c6e 3e20 4920 616d 2067  int(f"\n> I am g
-00002fe0: 6f69 6e67 2074 6f20 6576 616c 7561 7465  oing to evaluate
-00002ff0: 2061 6e64 2072 616e 6b20 7468 6520 616e   and rank the an
-00003000: 7377 6572 2e20 506c 6561 7365 2077 6169  swer. Please wai
-00003010: 742e 2e5c 6e22 2c20 276d 6167 656e 7461  t..\n", 'magenta
-00003020: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
-00003030: 5d29 0d0a 0d0a 2020 2020 2020 2020 2320  ])....        # 
-00003040: 4361 6c6c 2074 6865 204f 7065 6e41 4920  Call the OpenAI 
-00003050: 4150 4920 616e 6420 6861 6e64 6c65 2072  API and handle r
-00003060: 6174 6520 6c69 6d69 7420 6572 726f 7273  ate limit errors
-00003070: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00003080: 2020 2020 2020 2020 2020 2020 6c6c 6d5f              llm_
-00003090: 7265 7370 6f6e 7365 2c20 746f 6b65 6e73  response, tokens
-000030a0: 5f75 7365 6420 3d20 7365 6c66 2e6c 6c6d  _used = self.llm
-000030b0: 5f63 616c 6c28 7261 6e6b 5f6d 6573 7361  _call(rank_messa
-000030c0: 6765 7329 0d0a 2020 2020 2020 2020 2020  ges)..          
-000030d0: 2020 0d0a 2020 2020 2020 2020 6578 6365    ..        exce
-000030e0: 7074 206f 7065 6e61 692e 6572 726f 722e  pt openai.error.
-000030f0: 5261 7465 4c69 6d69 7445 7272 6f72 3a0d  RateLimitError:.
-00003100: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00003110: 6e74 280d 0a20 2020 2020 2020 2020 2020  nt(..           
-00003120: 2020 2020 2022 5468 6520 4f70 656e 4149       "The OpenAI
-00003130: 2041 5049 2072 6174 6520 6c69 6d69 7420   API rate limit 
-00003140: 6861 7320 6265 656e 2065 7863 6565 6465  has been exceede
-00003150: 642e 2057 6169 7469 6e67 2031 3020 7365  d. Waiting 10 se
-00003160: 636f 6e64 7320 616e 6420 7472 7969 6e67  conds and trying
-00003170: 2061 6761 696e 2e22 0d0a 2020 2020 2020   again."..      
-00003180: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00003190: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-000031a0: 3130 290d 0a20 2020 2020 2020 2020 2020  10)..           
-000031b0: 206c 6c6d 5f72 6573 706f 6e73 652c 2074   llm_response, t
-000031c0: 6f6b 656e 735f 7573 6564 203d 2073 656c  okens_used = sel
-000031d0: 662e 6c6c 6d5f 6361 6c6c 2872 616e 6b5f  f.llm_call(rank_
-000031e0: 6d65 7373 6167 6573 290d 0a20 2020 2020  messages)..     
-000031f0: 2020 200d 0a20 2020 2020 2020 2023 2045     ..        # E
-00003200: 7874 7261 6374 2074 6865 2063 6f64 6520  xtract the code 
-00003210: 6672 6f6d 2074 6865 2041 5049 2072 6573  from the API res
-00003220: 706f 6e73 650d 0a20 2020 2020 2020 2072  ponse..        r
-00003230: 616e 6b20 3d20 7365 6c66 2e5f 6578 7472  ank = self._extr
-00003240: 6163 745f 7261 6e6b 286c 6c6d 5f72 6573  act_rank(llm_res
-00003250: 706f 6e73 6529 2020 2020 2020 200d 0a0d  ponse)       ...
-00003260: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
-00003270: 7461 6c5f 746f 6b65 6e73 5f75 7365 642e  tal_tokens_used.
-00003280: 6170 7065 6e64 2874 6f6b 656e 735f 7573  append(tokens_us
-00003290: 6564 290d 0a0d 0a20 2020 2020 2020 2072  ed)....        r
-000032a0: 6574 7572 6e20 7261 6e6b 0d0a 0d0a 2020  eturn rank....  
-000032b0: 2020 6465 6620 7064 5f61 6765 6e74 5f63    def pd_agent_c
-000032c0: 6f6e 7665 7273 6528 7365 6c66 2c20 7175  onverse(self, qu
-000032d0: 6573 7469 6f6e 3d4e 6f6e 6529 3a0d 0a20  estion=None):.. 
-000032e0: 2020 2020 2020 2023 2046 756e 6374 696f         # Functio
-000032f0: 6e20 746f 2064 6973 706c 6179 2072 6573  n to display res
-00003300: 756c 7473 206e 6963 656c 790d 0a20 2020  ults nicely..   
-00003310: 2020 2020 2064 6566 2064 6973 706c 6179       def display
-00003320: 5f72 6573 756c 7473 2861 6e73 7765 722c  _results(answer,
-00003330: 2063 6f64 652c 2072 6566 6c65 6374 696f   code, reflectio
-00003340: 6e2c 2066 6c6f 772c 2072 616e 6b2c 2074  n, flow, rank, t
-00003350: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
-00003360: 5f73 756d 293a 0d0a 2020 2020 2020 2020  _sum):..        
-00003370: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
-00003380: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
-00003390: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000033a0: 2020 2020 2320 4a75 7079 7465 7220 6e6f      # Jupyter no
-000033b0: 7465 626f 6f6b 206f 7220 6970 7974 686f  tebook or ipytho
-000033c0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-000033d0: 2020 2064 6973 706c 6179 2848 544d 4c28     display(HTML(
-000033e0: 6627 3c70 3e3c 6220 7374 796c 653d 2263  f'<p><b style="c
-000033f0: 6f6c 6f72 3a62 6c75 653b 223e 416e 7377  olor:blue;">Answ
-00003400: 6572 3a3c 2f62 3e3c 6272 3e3c 7072 6520  er:</b><br><pre 
-00003410: 7374 796c 653d 2263 6f6c 6f72 3a62 6c61  style="color:bla
-00003420: 636b 3b22 3e3c 623e 7b61 6e73 7765 727d  ck;"><b>{answer}
-00003430: 3c2f 623e 3c2f 7072 653e 3c2f 703e 3c62  </b></pre></p><b
-00003440: 723e 2729 290d 0a20 2020 2020 2020 2020  r>'))..         
-00003450: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
-00003460: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
-00003470: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
-00003480: 4865 7265 2069 7320 7468 6520 6669 6e61  Here is the fina
-00003490: 6c20 636f 6465 2074 6861 7420 6163 636f  l code that acco
-000034a0: 6d70 6c69 7368 6573 2074 6865 2074 6173  mplishes the tas
-000034b0: 6b3a 3c2f 623e 3c62 723e 3c70 7265 2073  k:</b><br><pre s
-000034c0: 7479 6c65 3d22 636f 6c6f 723a 2335 3535  tyle="color:#555
-000034d0: 3535 353b 223e 7b63 6f64 657d 3c2f 7072  555;">{code}</pr
-000034e0: 653e 3c2f 703e 3c62 723e 2729 290d 0a20  e></p><br>')).. 
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00003500: 6973 706c 6179 2848 544d 4c28 6627 3c70  isplay(HTML(f'<p
-00003510: 3e3c 6220 7374 796c 653d 2263 6f6c 6f72  ><b style="color
-00003520: 3a62 6c75 653b 223e 4669 6e61 6c20 5468  :blue;">Final Th
-00003530: 6f75 6768 7473 3a3c 2f62 3e3c 6272 3e3c  oughts:</b><br><
-00003540: 7072 6520 7374 796c 653d 2263 6f6c 6f72  pre style="color
-00003550: 3a62 6c61 636b 3b20 7768 6974 652d 7370  :black; white-sp
-00003560: 6163 653a 2070 7265 2d77 7261 703b 2066  ace: pre-wrap; f
-00003570: 6f6e 742d 7765 6967 6874 3a20 626f 6c64  ont-weight: bold
-00003580: 3b22 3e7b 7265 666c 6563 7469 6f6e 7d3c  ;">{reflection}<
-00003590: 2f70 7265 3e3c 2f70 3e3c 6272 3e27 2929  /pre></p><br>'))
-000035a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000035b0: 2020 6966 2073 656c 662e 666c 6f77 5f64    if self.flow_d
-000035c0: 6961 6772 616d 3a0d 0a20 2020 2020 2020  iagram:..       
-000035d0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-000035e0: 706c 6179 2848 544d 4c28 6627 3c70 3e3c  play(HTML(f'<p><
-000035f0: 6220 7374 796c 653d 2263 6f6c 6f72 3a62  b style="color:b
-00003600: 6c75 653b 223e 4265 6c6f 7720 6973 206d  lue;">Below is m
-00003610: 7920 6170 7072 6f63 6820 6173 2061 2046  y approch as a F
-00003620: 6c6f 7720 6368 6172 743a 3c2f 623e 3c62  low chart:</b><b
-00003630: 723e 3c69 6d67 2073 7263 3d22 7b73 656c  r><img src="{sel
-00003640: 662e 6d6d 2866 6c6f 7729 7d22 2061 6c74  f.mm(flow)}" alt
-00003650: 3d22 416e 616c 7973 6973 2046 6c6f 7722  ="Analysis Flow"
-00003660: 3e3c 2f69 6d67 3e3c 2f70 3e3c 6272 3e27  ></img></p><br>'
-00003670: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00003680: 2020 2020 6966 2073 656c 662e 7261 6e6b      if self.rank
-00003690: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000036a0: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
-000036b0: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
-000036c0: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
-000036d0: 5261 6e6b 3a3c 2f62 3e3c 6272 3e3c 7370  Rank:</b><br><sp
-000036e0: 616e 2073 7479 6c65 3d22 636f 6c6f 723a  an style="color:
-000036f0: 626c 6163 6b3b 223e 7b72 616e 6b7d 3c2f  black;">{rank}</
-00003700: 7370 616e 3e3c 2f70 3e3c 6272 3e27 2929  span></p><br>'))
-00003710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003720: 2020 6469 7370 6c61 7928 4854 4d4c 2866    display(HTML(f
-00003730: 273c 703e 3c62 2073 7479 6c65 3d22 636f  '<p><b style="co
-00003740: 6c6f 723a 626c 7565 3b22 3e54 6f74 616c  lor:blue;">Total
-00003750: 2054 6f6b 656e 7320 5573 6564 3a3c 2f62   Tokens Used:</b
-00003760: 3e3c 6272 3e3c 7370 616e 2073 7479 6c65  ><br><span style
-00003770: 3d22 636f 6c6f 723a 626c 6163 6b3b 223e  ="color:black;">
-00003780: 7b74 6f74 616c 5f74 6f6b 656e 735f 7573  {total_tokens_us
-00003790: 6564 5f73 756d 7d3c 2f73 7061 6e3e 3c2f  ed_sum}</span></
-000037a0: 703e 3c62 723e 2729 290d 0a20 2020 2020  p><br>'))..     
-000037b0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000037d0: 4f74 6865 7220 656e 7669 726f 6e6d 656e  Other environmen
-000037e0: 7420 286c 696b 6520 7465 726d 696e 616c  t (like terminal
-000037f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003800: 2020 2063 7072 696e 7428 6622 5c6e 3e20     cprint(f"\n> 
-00003810: 416e 7377 6572 3a5c 6e7b 616e 7377 6572  Answer:\n{answer
-00003820: 7d5c 6e22 2c20 2767 7265 656e 272c 2061  }\n", 'green', a
-00003830: 7474 7273 3d5b 2762 6f6c 6427 5d29 0d0a  ttrs=['bold'])..
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 6370 7269 6e74 2866 223e 2048 6572 6520  cprint(f"> Here 
-00003860: 6973 2074 6865 2066 696e 616c 2063 6f64  is the final cod
-00003870: 6520 7468 6174 2061 6363 6f6d 706c 6973  e that accomplis
-00003880: 6865 7320 7468 6520 7461 736b 3a5c 6e7b  hes the task:\n{
-00003890: 636f 6465 7d5c 6e22 2c20 2767 7265 656e  code}\n", 'green
-000038a0: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
-000038b0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000038c0: 2020 2020 6370 7269 6e74 2866 223e 2046      cprint(f"> F
-000038d0: 696e 616c 2054 686f 7567 6874 733a 5c6e  inal Thoughts:\n
-000038e0: 7b72 6566 6c65 6374 696f 6e7d 5c6e 222c  {reflection}\n",
-000038f0: 2027 6772 6565 6e27 2c20 6174 7472 733d   'green', attrs=
-00003900: 5b27 626f 6c64 275d 290d 0a20 2020 2020  ['bold'])..     
-00003910: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00003920: 6c66 2e72 616e 6b3a 0d0a 2020 2020 2020  lf.rank:..      
-00003930: 2020 2020 2020 2020 2020 2020 2020 6370                cp
-00003940: 7269 6e74 2866 223e 2052 616e 6b3a 5c6e  rint(f"> Rank:\n
-00003950: 7b72 616e 6b7d 5c6e 222c 2027 6772 6565  {rank}\n", 'gree
-00003960: 6e27 2c20 6174 7472 733d 5b27 626f 6c64  n', attrs=['bold
-00003970: 275d 290d 0a20 2020 2020 2020 2020 2020  '])..           
-00003980: 2020 2020 2063 7072 696e 7428 6622 3e20       cprint(f"> 
-00003990: 546f 7461 6c20 746f 6b65 6e73 2075 7365  Total tokens use
-000039a0: 643a 5c6e 7b74 6f74 616c 5f74 6f6b 656e  d:\n{total_token
-000039b0: 735f 7573 6564 5f73 756d 7d5c 6e22 2c20  s_used_sum}\n", 
-000039c0: 2779 656c 6c6f 7727 2c20 6174 7472 733d  'yellow', attrs=
-000039d0: 5b27 626f 6c64 275d 290d 0a20 2020 2020  ['bold'])..     
-000039e0: 2020 200d 0a20 2020 2020 2020 2023 2049     ..        # I
-000039f0: 6620 6120 7175 6573 7469 6f6e 2069 7320  f a question is 
-00003a00: 7072 6f76 6964 6564 2c20 736b 6970 2074  provided, skip t
-00003a10: 6865 2069 6e70 7574 2070 726f 6d70 740d  he input prompt.
-00003a20: 0a20 2020 2020 2020 2069 6620 7175 6573  .        if ques
-00003a30: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
-00003a40: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00003a50: 2049 6e69 7469 616c 697a 6520 7468 6520   Initialize the 
-00003a60: 6d65 7373 6167 6573 206c 6973 7420 7769  messages list wi
-00003a70: 7468 2061 2073 7973 7465 6d20 6d65 7373  th a system mess
-00003a80: 6167 6520 636f 6e74 6169 6e69 6e67 2074  age containing t
-00003a90: 6865 2074 6173 6b20 7072 6f6d 7074 0d0a  he task prompt..
-00003aa0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00003ab0: 6167 6573 203d 205b 7b22 726f 6c65 223a  ages = [{"role":
-00003ac0: 2022 7379 7374 656d 222c 2022 636f 6e74   "system", "cont
-00003ad0: 656e 7422 3a20 7365 6c66 2e73 7973 7465  ent": self.syste
-00003ae0: 6d5f 7461 736b 2e66 6f72 6d61 7428 7175  m_task.format(qu
-00003af0: 6573 7469 6f6e 297d 5d0d 0a20 2020 2020  estion)}]..     
-00003b00: 2020 2020 2020 2023 2043 616c 6c20 7468         # Call th
-00003b10: 6520 7461 736b 5f65 7661 6c20 6d65 7468  e task_eval meth
-00003b20: 6f64 2077 6974 6820 7468 6520 7573 6572  od with the user
-00003b30: 2773 2071 7565 7374 696f 6e20 6966 2074  's question if t
-00003b40: 6865 2065 7870 6c6f 7261 746f 7279 206d  he exploratory m
-00003b50: 6f64 6520 6973 2054 7275 650d 0a20 2020  ode is True..   
-00003b60: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00003b70: 2e65 7870 6c6f 7261 746f 7279 2069 7320  .exploratory is 
-00003b80: 5472 7565 3a0d 0a20 2020 2020 2020 2020  True:..         
-00003b90: 2020 2020 2020 2074 6173 6b20 3d20 7365         task = se
-00003ba0: 6c66 2e74 6173 6b5f 6576 616c 2871 7565  lf.task_eval(que
-00003bb0: 7374 696f 6e29 0d0a 2020 2020 2020 2020  stion)..        
-00003bc0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00003bd0: 2020 2020 2020 2020 2020 2074 6173 6b20             task 
-00003be0: 3d20 7175 6573 7469 6f6e 0d0a 2020 2020  = question..    
-00003bf0: 2020 2020 2020 2020 2320 4361 6c6c 2074          # Call t
-00003c00: 6865 2070 645f 6167 656e 7420 6d65 7468  he pd_agent meth
-00003c10: 6f64 2077 6974 6820 7468 6520 7573 6572  od with the user
-00003c20: 2773 2071 7565 7374 696f 6e2c 2074 6865  's question, the
-00003c30: 206d 6573 7361 6765 7320 6c69 7374 2c20   messages list, 
-00003c40: 616e 6420 7468 6520 6461 7461 6672 616d  and the datafram
-00003c50: 650d 0a20 2020 2020 2020 2020 2020 2061  e..            a
-00003c60: 6e73 7765 722c 2063 6f64 652c 2072 6566  nswer, code, ref
-00003c70: 6c65 6374 696f 6e2c 2066 6c6f 772c 2074  lection, flow, t
-00003c80: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
-00003c90: 5f73 756d 203d 2073 656c 662e 7064 5f61  _sum = self.pd_a
-00003ca0: 6765 6e74 2874 6173 6b2c 206d 6573 7361  gent(task, messa
-00003cb0: 6765 732c 2073 656c 662e 6466 290d 0a0d  ges, self.df)...
-00003cc0: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-00003cd0: 746f 7265 2074 6865 206f 7269 6769 6e61  tore the origina
-00003ce0: 6c20 6c6c 6d20 7661 6c75 650d 0a20 2020  l llm value..   
-00003cf0: 2020 2020 2020 2020 206f 7269 6769 6e61           origina
-00003d00: 6c5f 6c6c 6d20 3d20 7365 6c66 2e6c 6c6d  l_llm = self.llm
-00003d10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00003d20: 2320 5261 6e6b 2074 6865 204c 4c4d 2072  # Rank the LLM r
-00003d30: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-00003d40: 2020 2020 2069 6620 7365 6c66 2e72 616e       if self.ran
-00003d50: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
-00003d60: 2020 2020 2320 5377 6974 6368 2074 6f20      # Switch to 
-00003d70: 6770 742d 3420 6966 206c 6c6d 5f73 7769  gpt-4 if llm_swi
-00003d80: 7463 6820 7061 7261 6d65 7465 7220 6973  tch parameter is
-00003d90: 2073 6574 2074 6f20 5472 7565 2e20 5468   set to True. Th
-00003da0: 6973 2077 696c 6c20 696e 6372 6561 7365  is will increase
-00003db0: 2074 6865 2070 726f 6365 7373 696e 6720   the processing 
-00003dc0: 7469 6d65 2061 6e64 2063 6f73 740d 0a20  time and cost.. 
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003de0: 6620 7365 6c66 2e6c 6c6d 5f73 7769 7463  f self.llm_switc
-00003df0: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-00003e00: 2020 2020 2020 2020 7365 6c66 2e6c 6c6d          self.llm
-00003e10: 203d 2027 6770 742d 3427 0d0a 2020 2020   = 'gpt-4'..    
-00003e20: 2020 2020 2020 2020 2020 2020 7261 6e6b              rank
-00003e30: 203d 2073 656c 662e 7261 6e6b 5f63 6f64   = self.rank_cod
-00003e40: 6528 636f 6465 2c71 7565 7374 696f 6e29  e(code,question)
-00003e50: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00003e60: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00003e70: 2020 2020 2072 616e 6b20 3d20 2222 0d0a       rank = ""..
-00003e80: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00003e90: 5377 6974 6368 2062 6163 6b20 746f 2074  Switch back to t
-00003ea0: 6865 206f 7269 6769 6e61 6c20 6c6c 6d20  he original llm 
-00003eb0: 6265 666f 7265 2074 6865 2066 756e 6374  before the funct
-00003ec0: 696f 6e20 6669 6e69 7368 6573 0d0a 2020  ion finishes..  
-00003ed0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-00003ee0: 6c6d 203d 206f 7269 6769 6e61 6c5f 6c6c  lm = original_ll
-00003ef0: 6d0d 0a0d 0a20 2020 2020 2020 2020 2020  m....           
-00003f00: 2064 6973 706c 6179 5f72 6573 756c 7473   display_results
-00003f10: 2861 6e73 7765 722c 2063 6f64 652c 2072  (answer, code, r
-00003f20: 6566 6c65 6374 696f 6e2c 2066 6c6f 772c  eflection, flow,
-00003f30: 2072 616e 6b2c 2074 6f74 616c 5f74 6f6b   rank, total_tok
-00003f40: 656e 735f 7573 6564 5f73 756d 290d 0a20  ens_used_sum).. 
-00003f50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003f60: 6e0d 0a0d 0a20 2020 2020 2020 2023 2053  n....        # S
-00003f70: 7461 7274 2061 6e20 696e 6669 6e69 7465  tart an infinite
-00003f80: 206c 6f6f 7020 746f 206b 6565 7020 6173   loop to keep as
-00003f90: 6b69 6e67 2074 6865 2075 7365 7220 666f  king the user fo
-00003fa0: 7220 7175 6573 7469 6f6e 730d 0a20 2020  r questions..   
-00003fb0: 2020 2020 2066 6972 7374 5f69 7465 7261       first_itera
-00003fc0: 7469 6f6e 203d 2054 7275 6520 2023 2046  tion = True  # F
-00003fd0: 6c61 6720 666f 7220 7468 6520 6669 7273  lag for the firs
-00003fe0: 7420 6974 6572 6174 696f 6e20 6f66 2074  t iteration of t
-00003ff0: 6865 206c 6f6f 700d 0a20 2020 2020 2020  he loop..       
-00004000: 2077 6869 6c65 2054 7275 653a 0d0a 2020   while True:..  
-00004010: 2020 2020 2020 2020 2020 2320 5072 6f6d            # Prom
-00004020: 7074 2074 6865 2075 7365 7220 746f 2065  pt the user to e
-00004030: 6e74 6572 2061 2071 7565 7374 696f 6e20  nter a question 
-00004040: 6f72 2074 7970 6520 2765 7869 7427 2074  or type 'exit' t
-00004050: 6f20 7175 6974 0d0a 2020 2020 2020 2020  o quit..        
-00004060: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
-00004070: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
-00004080: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00004090: 2020 2020 6469 7370 6c61 7928 4854 4d4c      display(HTML
-000040a0: 2827 3c62 2073 7479 6c65 3d22 636f 6c6f  ('<b style="colo
-000040b0: 723a 626c 7565 3b22 3e45 6e74 6572 2079  r:blue;">Enter y
-000040c0: 6f75 7220 7175 6573 7469 6f6e 206f 7220  our question or 
-000040d0: 7479 7065 205c 2765 7869 745c 2720 746f  type \'exit\' to
-000040e0: 2071 7569 743a 3c2f 623e 2729 290d 0a20   quit:</b>')).. 
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2071                 q
-00004100: 7565 7374 696f 6e20 3d20 696e 7075 7428  uestion = input(
-00004110: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00004120: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00004130: 2020 2020 2020 6370 7269 6e74 2822 5c6e        cprint("\n
-00004140: 456e 7465 7220 796f 7572 2071 7565 7374  Enter your quest
-00004150: 696f 6e20 6f72 2074 7970 6520 2765 7869  ion or type 'exi
-00004160: 7427 2074 6f20 7175 6974 3a22 2c20 2762  t' to quit:", 'b
-00004170: 6c75 6527 2c20 6174 7472 733d 5b27 626f  lue', attrs=['bo
-00004180: 6c64 275d 290d 0a20 2020 2020 2020 2020  ld'])..         
-00004190: 2020 2020 2020 2071 7565 7374 696f 6e20         question 
-000041a0: 3d20 696e 7075 7428 290d 0a0d 0a20 2020  = input()....   
-000041b0: 2020 2020 2020 2020 2023 2052 656d 656d           # Remem
-000041c0: 6265 7274 2074 6865 206f 7269 6769 6e61  bert the origina
-000041d0: 6c20 7175 6573 7469 6f6e 2066 6f72 2072  l question for r
-000041e0: 616e 6b69 6e67 0d0a 2020 2020 2020 2020  anking..        
-000041f0: 2020 2020 6f72 6967 696e 616c 5f71 7565      original_que
-00004200: 7374 696f 6e20 3d20 7175 6573 7469 6f6e  stion = question
-00004210: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00004220: 2320 4966 2074 6865 2075 7365 7220 7479  # If the user ty
-00004230: 7065 7320 2765 7869 7427 2c20 6272 6561  pes 'exit', brea
-00004240: 6b20 6f75 7420 6f66 2074 6865 206c 6f6f  k out of the loo
-00004250: 700d 0a20 2020 2020 2020 2020 2020 2069  p..            i
-00004260: 6620 7175 6573 7469 6f6e 2e73 7472 6970  f question.strip
-00004270: 2829 2e6c 6f77 6572 2829 203d 3d20 2765  ().lower() == 'e
-00004280: 7869 7427 3a0d 0a20 2020 2020 2020 2020  xit':..         
-00004290: 2020 2020 2020 2062 7265 616b 0d0a 0d0a         break....
-000042a0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-000042b0: 6972 7374 5f69 7465 7261 7469 6f6e 3a0d  irst_iteration:.
-000042c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000042d0: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
-000042e0: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
-000042f0: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
-00004300: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
-00004310: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
-00004320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004330: 2020 6d65 7373 6167 6573 203d 205b 7b22    messages = [{"
-00004340: 726f 6c65 223a 2022 7379 7374 656d 222c  role": "system",
-00004350: 2022 636f 6e74 656e 7422 3a20 7365 6c66   "content": self
-00004360: 2e73 7973 7465 6d5f 7461 736b 2e66 6f72  .system_task.for
-00004370: 6d61 7428 7175 6573 7469 6f6e 2c71 7565  mat(question,que
-00004380: 7374 696f 6e29 7d5d 0d0a 2020 2020 2020  stion)}]..      
-00004390: 2020 2020 2020 2020 2020 2320 4361 6c6c            # Call
-000043a0: 2074 6865 2074 6173 6b5f 6576 616c 206d   the task_eval m
-000043b0: 6574 686f 6420 7769 7468 2074 6865 2075  ethod with the u
-000043c0: 7365 7227 7320 7175 6573 7469 6f6e 2069  ser's question i
-000043d0: 6620 7468 6520 6578 706c 6f72 6174 6f72  f the explorator
-000043e0: 7920 6d6f 6465 2069 7320 5472 7565 0d0a  y mode is True..
-000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004400: 6966 2073 656c 662e 6578 706c 6f72 6174  if self.explorat
-00004410: 6f72 7920 6973 2054 7275 653a 0d0a 2020  ory is True:..  
-00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 2020 7461 736b 203d 2073 656c 662e 7461    task = self.ta
-00004440: 736b 5f65 7661 6c28 7175 6573 7469 6f6e  sk_eval(question
-00004450: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004460: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00004470: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-00004480: 736b 203d 2071 7565 7374 696f 6e0d 0a20  sk = question.. 
-00004490: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000044a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000044b0: 2020 7461 736b 203d 2071 7565 7374 696f    task = questio
-000044c0: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
-000044d0: 2023 2043 616c 6c20 7468 6520 7064 5f61   # Call the pd_a
-000044e0: 6765 6e74 206d 6574 686f 6420 7769 7468  gent method with
-000044f0: 2074 6865 2075 7365 7227 7320 7175 6573   the user's ques
-00004500: 7469 6f6e 2c20 7468 6520 6d65 7373 6167  tion, the messag
-00004510: 6573 206c 6973 742c 2061 6e64 2074 6865  es list, and the
-00004520: 2064 6174 6166 7261 6d65 0d0a 2020 2020   dataframe..    
-00004530: 2020 2020 2020 2020 616e 7377 6572 2c20          answer, 
-00004540: 636f 6465 2c20 7265 666c 6563 7469 6f6e  code, reflection
-00004550: 2c20 666c 6f77 2c20 746f 7461 6c5f 746f  , flow, total_to
-00004560: 6b65 6e73 5f75 7365 645f 7375 6d20 3d20  kens_used_sum = 
-00004570: 7365 6c66 2e70 645f 6167 656e 7428 7461  self.pd_agent(ta
-00004580: 736b 2c20 6d65 7373 6167 6573 2c20 7365  sk, messages, se
-00004590: 6c66 2e64 6629 0d0a 0d0a 2020 2020 2020  lf.df)....      
-000045a0: 2020 2020 2020 2320 5374 6f72 6520 7468        # Store th
-000045b0: 6520 6f72 6967 696e 616c 206c 6c6d 2076  e original llm v
-000045c0: 616c 7565 0d0a 2020 2020 2020 2020 2020  alue..          
-000045d0: 2020 6f72 6967 696e 616c 5f6c 6c6d 203d    original_llm =
-000045e0: 2073 656c 662e 6c6c 6d0d 0a0d 0a20 2020   self.llm....   
-000045f0: 2020 2020 2020 2020 2023 2052 616e 6b20           # Rank 
-00004600: 7468 6520 4c4c 4d20 7265 7370 6f6e 7365  the LLM response
-00004610: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00004620: 2073 656c 662e 7261 6e6b 3a0d 0a20 2020   self.rank:..   
-00004630: 2020 2020 2020 2020 2020 2020 2023 2053               # S
-00004640: 7769 7463 6820 746f 2067 7074 2d34 2069  witch to gpt-4 i
-00004650: 6620 6c6c 6d5f 7377 6974 6368 2070 6172  f llm_switch par
-00004660: 616d 6574 6572 2069 7320 7365 7420 746f  ameter is set to
-00004670: 2054 7275 652e 2054 6869 7320 7769 6c6c   True. This will
-00004680: 2069 6e63 7265 6173 6520 7468 6520 7072   increase the pr
-00004690: 6f63 6573 7369 6e67 2074 696d 6520 616e  ocessing time an
-000046a0: 6420 636f 7374 0d0a 2020 2020 2020 2020  d cost..        
-000046b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000046c0: 6c6c 6d5f 7377 6974 6368 3a0d 0a20 2020  llm_switch:..   
-000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046e0: 2073 656c 662e 6c6c 6d20 3d20 2767 7074   self.llm = 'gpt
-000046f0: 2d34 270d 0a20 2020 2020 2020 2020 2020  -4'..           
-00004700: 2020 2020 2072 616e 6b20 3d20 7365 6c66       rank = self
-00004710: 2e72 616e 6b5f 636f 6465 2863 6f64 652c  .rank_code(code,
-00004720: 6f72 6967 696e 616c 5f71 7565 7374 696f  original_questio
-00004730: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
-00004740: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00004750: 2020 2020 2020 2072 616e 6b20 3d20 2222         rank = ""
-00004760: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00004770: 2320 5377 6974 6368 2062 6163 6b20 746f  # Switch back to
-00004780: 2074 6865 206f 7269 6769 6e61 6c20 6c6c   the original ll
-00004790: 6d20 6265 666f 7265 2074 6865 2066 756e  m before the fun
-000047a0: 6374 696f 6e20 6669 6e69 7368 6573 0d0a  ction finishes..
-000047b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000047c0: 2e6c 6c6d 203d 206f 7269 6769 6e61 6c5f  .llm = original_
-000047d0: 6c6c 6d0d 0a0d 0a20 2020 2020 2020 2020  llm....         
-000047e0: 2020 2064 6973 706c 6179 5f72 6573 756c     display_resul
-000047f0: 7473 2861 6e73 7765 722c 2063 6f64 652c  ts(answer, code,
-00004800: 2072 6566 6c65 6374 696f 6e2c 666c 6f77   reflection,flow
-00004810: 2c72 616e 6b2c 746f 7461 6c5f 746f 6b65  ,rank,total_toke
-00004820: 6e73 5f75 7365 645f 7375 6d29 0d0a 0d0a  ns_used_sum)....
-00004830: 2020 2020 2020 2020 2020 2020 2320 4166              # Af
-00004840: 7465 7220 7468 6520 6669 7273 7420 6974  ter the first it
-00004850: 6572 6174 696f 6e2c 2073 6574 2074 6865  eration, set the
-00004860: 2066 6c61 6720 746f 2046 616c 7365 0d0a   flag to False..
-00004870: 2020 2020 2020 2020 2020 2020 6669 7273              firs
-00004880: 745f 6974 6572 6174 696f 6e20 3d20 4661  t_iteration = Fa
-00004890: 6c73 650d 0a0d 0a20 2020 2064 6566 2070  lse....    def p
-000048a0: 645f 6167 656e 7428 7365 6c66 2c20 7175  d_agent(self, qu
-000048b0: 6573 7469 6f6e 2c20 6d65 7373 6167 6573  estion, messages
-000048c0: 2c20 6466 3d4e 6f6e 6529 3a0d 0a20 2020  , df=None):..   
-000048d0: 2020 2020 2023 2041 6464 2061 2075 7365       # Add a use
-000048e0: 7220 6d65 7373 6167 6520 7769 7468 2074  r message with t
-000048f0: 6865 2075 7064 6174 6564 2074 6173 6b20  he updated task 
-00004900: 7072 6f6d 7074 2074 6f20 7468 6520 6d65  prompt to the me
-00004910: 7373 6167 6573 206c 6973 740d 0a20 2020  ssages list..   
-00004920: 2020 2020 206d 6573 7361 6765 732e 6170       messages.ap
-00004930: 7065 6e64 287b 2272 6f6c 6522 3a20 2275  pend({"role": "u
-00004940: 7365 7222 2c20 2263 6f6e 7465 6e74 223a  ser", "content":
-00004950: 2073 656c 662e 7461 736b 2e66 6f72 6d61   self.task.forma
-00004960: 7428 7365 6c66 2e64 665f 6865 6164 2c20  t(self.df_head, 
-00004970: 7175 6573 7469 6f6e 297d 290d 0a0d 0a20  question)}).... 
-00004980: 2020 2020 2020 2069 6620 2769 7079 6b65         if 'ipyke
-00004990: 726e 656c 2720 696e 2073 7973 2e6d 6f64  rnel' in sys.mod
-000049a0: 756c 6573 3a0d 0a20 2020 2020 2020 2020  ules:..         
-000049b0: 2020 2023 204a 7570 7974 6572 206e 6f74     # Jupyter not
-000049c0: 6562 6f6f 6b20 6f72 2069 7079 7468 6f6e  ebook or ipython
-000049d0: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
-000049e0: 7370 6c61 7928 4854 4d4c 2866 273c 7020  splay(HTML(f'<p 
-000049f0: 7374 796c 653d 2263 6f6c 6f72 3a6d 6167  style="color:mag
-00004a00: 656e 7461 3b22 3e5c 6e43 616c 6c69 6e67  enta;">\nCalling
-00004a10: 204d 6f64 656c 3a20 7b73 656c 662e 6c6c   Model: {self.ll
-00004a20: 6d7d 3c2f 703e 2729 290d 0a20 2020 2020  m}</p>'))..     
-00004a30: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
-00004a40: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
-00004a50: 653d 2263 6f6c 6f72 3a6d 6167 656e 7461  e="color:magenta
-00004a60: 3b22 3e49 2068 6176 6520 7365 6e74 2079  ;">I have sent y
-00004a70: 6f75 7220 7265 7175 6573 7420 746f 2074  our request to t
-00004a80: 6865 204c 4c4d 2061 6e64 2061 7761 6974  he LLM and await
-00004a90: 696e 6720 7265 7370 6f6e 7365 2c20 706c  ing response, pl
-00004aa0: 6561 7365 2077 6169 742e 2e2e 3c2f 623e  ease wait...</b>
-00004ab0: 3c2f 703e 3c62 723e 2729 290d 0a20 2020  </p><br>'))..   
-00004ac0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00004ad0: 2020 2020 2020 2020 2320 4f74 6865 7220          # Other 
-00004ae0: 656e 7669 726f 6e6d 656e 7420 286c 696b  environment (lik
-00004af0: 6520 7465 726d 696e 616c 290d 0a20 2020  e terminal)..   
-00004b00: 2020 2020 2020 2020 2070 7269 6e74 2863           print(c
-00004b10: 6f6c 6f72 6564 2866 225c 6e3e 2043 616c  olored(f"\n> Cal
-00004b20: 6c69 6e67 204d 6f64 656c 3a20 7b73 656c  ling Model: {sel
-00004b30: 662e 6c6c 6d7d 222c 2022 6d61 6765 6e74  f.llm}", "magent
-00004b40: 6122 2929 0d0a 2020 2020 2020 2020 2020  a"))..          
-00004b50: 2020 6370 7269 6e74 2866 225c 6e3e 2049    cprint(f"\n> I
-00004b60: 2068 6176 6520 7365 6e74 2079 6f75 7220   have sent your 
-00004b70: 7265 7175 6573 7420 746f 2074 6865 204c  request to the L
-00004b80: 4c4d 2061 6e64 2061 7761 6974 696e 6720  LM and awaiting 
-00004b90: 7265 7370 6f6e 7365 2c20 706c 6561 7365  response, please
-00004ba0: 2077 6169 742e 2e2e 5c6e 222c 2027 6d61   wait...\n", 'ma
-00004bb0: 6765 6e74 6127 2c20 6174 7472 733d 5b27  genta', attrs=['
-00004bc0: 626f 6c64 275d 290d 0a0d 0a20 2020 2020  bold'])....     
-00004bd0: 2020 2023 2043 616c 6c20 7468 6520 4f70     # Call the Op
-00004be0: 656e 4149 2041 5049 2061 6e64 2068 616e  enAI API and han
-00004bf0: 646c 6520 7261 7465 206c 696d 6974 2065  dle rate limit e
-00004c00: 7272 6f72 730d 0a20 2020 2020 2020 2074  rrors..        t
-00004c10: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
-00004c20: 206c 6c6d 5f72 6573 706f 6e73 652c 2074   llm_response, t
-00004c30: 6f6b 656e 735f 7573 6564 203d 2073 656c  okens_used = sel
-00004c40: 662e 6c6c 6d5f 6361 6c6c 286d 6573 7361  f.llm_call(messa
-00004c50: 6765 7329 0d0a 0d0a 2020 2020 2020 2020  ges)....        
-00004c60: 6578 6365 7074 206f 7065 6e61 692e 6572  except openai.er
-00004c70: 726f 722e 5261 7465 4c69 6d69 7445 7272  ror.RateLimitErr
-00004c80: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00004c90: 2070 7269 6e74 280d 0a20 2020 2020 2020   print(..       
-00004ca0: 2020 2020 2020 2020 2022 5468 6520 4f70           "The Op
-00004cb0: 656e 4149 2041 5049 2072 6174 6520 6c69  enAI API rate li
-00004cc0: 6d69 7420 6861 7320 6265 656e 2065 7863  mit has been exc
-00004cd0: 6565 6465 642e 2057 6169 7469 6e67 2031  eeded. Waiting 1
-00004ce0: 3020 7365 636f 6e64 7320 616e 6420 7472  0 seconds and tr
-00004cf0: 7969 6e67 2061 6761 696e 2e22 0d0a 2020  ying again."..  
-00004d00: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00004d10: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
-00004d20: 6565 7028 3130 290d 0a20 2020 2020 2020  eep(10)..       
-00004d30: 2020 2020 206c 6c6d 5f72 6573 706f 6e73       llm_respons
-00004d40: 652c 2074 6f6b 656e 735f 7573 6564 203d  e, tokens_used =
-00004d50: 2073 656c 662e 6c6c 6d5f 6361 6c6c 286d   self.llm_call(m
-00004d60: 6573 7361 6765 7329 0d0a 0d0a 2020 2020  essages)....    
-00004d70: 2020 2020 2320 4578 7472 6163 7420 7468      # Extract th
-00004d80: 6520 636f 6465 2066 726f 6d20 7468 6520  e code from the 
-00004d90: 4150 4920 7265 7370 6f6e 7365 0d0a 2020  API response..  
-00004da0: 2020 2020 2020 636f 6465 2c72 6566 6c65        code,refle
-00004db0: 6374 696f 6e2c 666c 6f77 3d20 7365 6c66  ction,flow= self
-00004dc0: 2e5f 6578 7472 6163 745f 636f 6465 286c  ._extract_code(l
-00004dd0: 6c6d 5f72 6573 706f 6e73 6529 0d0a 0d0a  lm_response)....
-00004de0: 2020 2020 2020 2020 2320 5570 6461 7465          # Update
-00004df0: 2074 6865 2074 6f74 616c 2074 6f6b 656e   the total token
-00004e00: 7320 7573 6564 0d0a 2020 2020 2020 2020  s used..        
-00004e10: 7365 6c66 2e74 6f74 616c 5f74 6f6b 656e  self.total_token
-00004e20: 735f 7573 6564 2e61 7070 656e 6428 746f  s_used.append(to
-00004e30: 6b65 6e73 5f75 7365 6429 0d0a 2020 2020  kens_used)..    
-00004e40: 2020 2020 746f 7461 6c5f 746f 6b65 6e73      total_tokens
-00004e50: 5f75 7365 645f 7375 6d20 3d20 7375 6d28  _used_sum = sum(
-00004e60: 7365 6c66 2e74 6f74 616c 5f74 6f6b 656e  self.total_token
-00004e70: 735f 7573 6564 290d 0a0d 0a20 2020 2020  s_used)....     
-00004e80: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
-00004e90: 6572 726f 7220 636f 7272 6563 7469 6f6e  error correction
-00004ea0: 2063 6f75 6e74 6572 0d0a 2020 2020 2020   counter..      
-00004eb0: 2020 6572 726f 725f 636f 7272 6563 7469    error_correcti
-00004ec0: 6f6e 7320 3d20 300d 0a0d 0a20 2020 2020  ons = 0....     
-00004ed0: 2020 2023 2053 746f 7265 2074 6865 206f     # Store the o
-00004ee0: 7269 6769 6e61 6c20 6c6c 6d20 7661 6c75  riginal llm valu
-00004ef0: 650d 0a20 2020 2020 2020 206f 7269 6769  e..        origi
-00004f00: 6e61 6c5f 6c6c 6d20 3d20 7365 6c66 2e6c  nal_llm = self.l
-00004f10: 6c6d 0d0a 0d0a 2020 2020 2020 2020 2320  lm....        # 
-00004f20: 4465 6275 6720 636f 6465 2069 6620 6465  Debug code if de
-00004f30: 6275 6720 7061 7261 6d65 7465 7220 6973  bug parameter is
-00004f40: 2073 6574 2074 6f20 5472 7565 0d0a 2020   set to True..  
-00004f50: 2020 2020 2020 6966 2073 656c 662e 6465        if self.de
-00004f60: 6275 673a 0d0a 2020 2020 2020 2020 2020  bug:..          
-00004f70: 2020 2320 5377 6974 6368 2074 6f20 6770    # Switch to gp
-00004f80: 742d 3420 6966 206c 6c6d 5f73 7769 7463  t-4 if llm_switc
-00004f90: 6820 7061 7261 6d65 7465 7220 6973 2073  h parameter is s
-00004fa0: 6574 2074 6f20 5472 7565 2e20 5468 6973  et to True. This
-00004fb0: 2077 696c 6c20 696e 6372 6561 7365 2074   will increase t
-00004fc0: 6865 2070 726f 6365 7373 696e 6720 7469  he processing ti
-00004fd0: 6d65 2061 6e64 2063 6f73 740d 0a20 2020  me and cost..   
-00004fe0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00004ff0: 2e6c 6c6d 5f73 7769 7463 683a 0d0a 2020  .llm_switch:..  
-00005000: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005010: 6c66 2e6c 6c6d 203d 2027 6770 742d 3427  lf.llm = 'gpt-4'
-00005020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005030: 2020 6966 2027 6970 796b 6572 6e65 6c27    if 'ipykernel'
-00005040: 2069 6e20 7379 732e 6d6f 6475 6c65 733a   in sys.modules:
-00005050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005060: 2020 2020 2020 2320 4a75 7079 7465 7220        # Jupyter 
-00005070: 6e6f 7465 626f 6f6b 0d0a 2020 2020 2020  notebook..      
-00005080: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00005090: 7370 6c61 7928 4854 4d4c 2827 3c73 7061  splay(HTML('<spa
-000050a0: 6e20 7374 796c 653d 2263 6f6c 6f72 3a20  n style="color: 
-000050b0: 6d61 6765 6e74 613b 223e 5377 6974 6368  magenta;">Switch
-000050c0: 696e 6720 6d6f 6465 6c20 746f 2067 7074  ing model to gpt
-000050d0: 2d34 2074 6f20 6465 6275 6720 7468 6520  -4 to debug the 
-000050e0: 636f 6465 2e3c 2f73 7061 6e3e 2729 290d  code.</span>')).
-000050f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005100: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00005110: 2020 2020 2020 2020 2020 2020 2320 434c              # CL
-00005120: 490d 0a20 2020 2020 2020 2020 2020 2020  I..             
-00005130: 2020 2020 2020 2070 7269 6e74 2863 6f6c         print(col
-00005140: 6f72 6564 2822 5c6e 3e20 5377 6974 6368  ored("\n> Switch
-00005150: 696e 6720 6d6f 6465 6c20 746f 2047 5054  ing model to GPT
-00005160: 2d34 2074 6f20 6465 6275 6720 7468 6520  -4 to debug the 
-00005170: 636f 6465 2e22 2c20 226d 6167 656e 7461  code.", "magenta
-00005180: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
-00005190: 2063 6f64 6520 3d20 7365 6c66 2e64 6562   code = self.deb
-000051a0: 7567 5f63 6f64 6528 636f 6465 2c20 7175  ug_code(code, qu
-000051b0: 6573 7469 6f6e 290d 0a0d 0a20 2020 2020  estion)....     
-000051c0: 2020 2020 2020 2023 2053 7769 7463 6820         # Switch 
-000051d0: 6261 636b 2074 6f20 7468 6520 6f72 6967  back to the orig
-000051e0: 696e 616c 206c 6c6d 2062 6566 6f72 6520  inal llm before 
-000051f0: 7468 6520 6675 6e63 7469 6f6e 2066 696e  the function fin
-00005200: 6973 6865 730d 0a20 2020 2020 2020 2020  ishes..         
-00005210: 2020 2073 656c 662e 6c6c 6d20 3d20 6f72     self.llm = or
-00005220: 6967 696e 616c 5f6c 6c6d 0d0a 0d0a 2020  iginal_llm....  
-00005230: 2020 2020 2020 2320 5265 6469 7265 6374        # Redirect
-00005240: 2073 7461 6e64 6172 6420 6f75 7470 7574   standard output
-00005250: 2074 6f20 6120 5374 7269 6e67 494f 2062   to a StringIO b
-00005260: 7566 6665 720d 0a20 2020 2020 2020 2077  uffer..        w
-00005270: 6974 6820 7265 6469 7265 6374 5f73 7464  ith redirect_std
-00005280: 6f75 7428 696f 2e53 7472 696e 6749 4f28  out(io.StringIO(
-00005290: 2929 2061 7320 6f75 7470 7574 3a0d 0a20  )) as output:.. 
-000052a0: 2020 2020 2020 2020 2020 2023 2054 7279             # Try
-000052b0: 2074 6f20 6578 6563 7574 6520 7468 6520   to execute the 
-000052c0: 636f 6465 2061 6e64 2068 616e 646c 6520  code and handle 
-000052d0: 6572 726f 7273 0d0a 2020 2020 2020 2020  errors..        
-000052e0: 2020 2020 7768 696c 6520 6572 726f 725f      while error_
-000052f0: 636f 7272 6563 7469 6f6e 7320 3c20 7365  corrections < se
-00005300: 6c66 2e4d 4158 5f45 5252 4f52 5f43 4f52  lf.MAX_ERROR_COR
-00005310: 5245 4354 494f 4e53 3a0d 0a20 2020 2020  RECTIONS:..     
-00005320: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00005330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005340: 2020 2020 206d 6573 7361 6765 732e 6170       messages.ap
-00005350: 7065 6e64 287b 2272 6f6c 6522 3a20 2261  pend({"role": "a
-00005360: 7373 6973 7461 6e74 222c 2022 636f 6e74  ssistant", "cont
-00005370: 656e 7422 3a20 6c6c 6d5f 7265 7370 6f6e  ent": llm_respon
-00005380: 7365 7d29 0d0a 2020 2020 2020 2020 2020  se})..          
-00005390: 2020 2020 2020 2020 2020 2320 5265 6d6f            # Remo
-000053a0: 7665 2074 6865 206f 6c64 6573 7420 636f  ve the oldest co
-000053b0: 6e76 6572 7361 7469 6f6e 2066 726f 6d20  nversation from 
-000053c0: 7468 6520 6d65 7373 6167 6573 206c 6973  the messages lis
-000053d0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-000053e0: 2020 2020 2020 2069 6620 6c65 6e28 6d65         if len(me
-000053f0: 7373 6167 6573 2920 3e20 7365 6c66 2e4d  ssages) > self.M
-00005400: 4158 5f43 4f4e 5645 5253 4154 494f 4e53  AX_CONVERSATIONS
-00005410: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005420: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00005430: 6765 732e 706f 7028 3129 0d0a 2020 2020  ges.pop(1)..    
-00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2020 6d65 7373 6167 6573 2e70 6f70      messages.pop
-00005460: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
-00005470: 2020 2020 2020 2020 2023 2052 6573 6574           # Reset
-00005480: 2064 6620 746f 2074 6865 206f 7269 6769   df to the origi
-00005490: 6e61 6c20 7374 6174 6520 6265 666f 7265  nal state before
-000054a0: 2065 7865 6375 7469 6e67 2074 6865 2063   executing the c
-000054b0: 6f64 650d 0a20 2020 2020 2020 2020 2020  ode..           
-000054c0: 2020 2020 2020 2020 2073 656c 662e 6466           self.df
-000054d0: 203d 2073 656c 662e 6f72 6967 696e 616c   = self.original
-000054e0: 5f64 662e 636f 7079 2829 0d0a 2020 2020  _df.copy()..    
-000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005500: 2320 4578 6563 7574 6520 7468 6520 636f  # Execute the co
-00005510: 6465 0d0a 2020 2020 2020 2020 2020 2020  de..            
-00005520: 2020 2020 2020 2020 6966 2063 6f64 6520          if code 
-00005530: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 2020 2020 2020 6578 6563 2863 6f64 652c        exec(code,
-00005560: 207b 2764 6627 3a20 7365 6c66 2e64 667d   {'df': self.df}
-00005570: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005580: 2020 2020 2020 2062 7265 616b 0d0a 2020         break..  
-00005590: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000055a0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-000055b0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
-000055c0: 2020 2020 2020 2020 2020 2320 5072 696e            # Prin
-000055d0: 7420 7468 6520 6572 726f 7220 6d65 7373  t the error mess
-000055e0: 6167 650d 0a20 2020 2020 2020 2020 2020  age..           
-000055f0: 2020 2020 2020 2020 2069 6620 2769 7079           if 'ipy
-00005600: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
-00005610: 6f64 756c 6573 3a0d 0a20 2020 2020 2020  odules:..       
-00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005630: 2023 204a 7570 7974 6572 206e 6f74 6562   # Jupyter noteb
-00005640: 6f6f 6b0d 0a20 2020 2020 2020 2020 2020  ook..           
-00005650: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00005660: 706c 6179 2848 544d 4c28 6627 3c62 723e  play(HTML(f'<br>
-00005670: 3c62 3e3c 7370 616e 2073 7479 6c65 3d22  <b><span style="
-00005680: 636f 6c6f 723a 2023 6438 3663 3030 3b22  color: #d86c00;"
-00005690: 3e49 2072 616e 2069 6e74 6f20 616e 2069  >I ran into an i
-000056a0: 7373 7565 3a3c 2f73 7061 6e3e 3c2f 623e  ssue:</span></b>
-000056b0: 3c62 723e 3c70 7265 2073 7479 6c65 3d22  <br><pre style="
-000056c0: 636f 6c6f 723a 2023 6438 3663 3030 3b22  color: #d86c00;"
-000056d0: 3e7b 657d 3c2f 7072 653e 3c62 723e 3c62  >{e}</pre><br><b
-000056e0: 3e3c 7370 616e 2073 7479 6c65 3d22 636f  ><span style="co
-000056f0: 6c6f 723a 2023 6438 3663 3030 3b22 3e49  lor: #d86c00;">I
-00005700: 2077 696c 6c20 6578 616d 696e 6520 6974   will examine it
-00005710: 2c20 616e 6420 7472 7920 6167 6169 6e20  , and try again 
-00005720: 7769 7468 2061 6e20 6164 6a75 7374 6564  with an adjusted
-00005730: 2063 6f64 652e 3c2f 7370 616e 3e3c 2f62   code.</span></b
-00005740: 3e3c 6272 3e27 2929 0d0a 2020 2020 2020  ><br>'))..      
-00005750: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005760: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00005770: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-00005780: 4c49 0d0a 2020 2020 2020 2020 2020 2020  LI..            
-00005790: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
-000057a0: 6e74 2863 6f6c 6f72 6564 2866 2749 2072  nt(colored(f'I r
-000057b0: 616e 2069 6e74 6f20 616e 2069 7373 7565  an into an issue
-000057c0: 3a20 7b65 7d2e 203e 2049 2077 696c 6c20  : {e}. > I will 
-000057d0: 6578 616d 696e 6520 6974 2c20 616e 6420  examine it, and 
-000057e0: 7472 7920 6167 6169 6e20 7769 7468 2061  try again with a
-000057f0: 6e20 6164 6a75 7374 6564 2063 6f64 652e  n adjusted code.
-00005800: 272c 2027 7265 6427 2929 0d0a 2020 2020  ', 'red'))..    
-00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 2020 7379 732e 7374 6465 7272 2e77      sys.stderr.w
-00005830: 7269 7465 2827 5c30 3333 5b33 316d 2720  rite('\033[31m' 
-00005840: 2b20 6627 3e20 4920 7261 6e20 696e 746f  + f'> I ran into
-00005850: 2061 6e20 6973 7375 653a 207b 657d 2e20   an issue: {e}. 
-00005860: 5c6e 3e20 4920 7769 6c6c 2065 7861 6d69  \n> I will exami
-00005870: 6e65 2069 742c 2061 6e64 2074 7279 2061  ne it, and try a
-00005880: 6761 696e 2077 6974 6820 616e 2061 646a  gain with an adj
-00005890: 7573 7465 6420 636f 6465 2e27 202b 2027  usted code.' + '
-000058a0: 5c30 3333 5b30 6d27 202b 2027 5c6e 2729  \033[0m' + '\n')
-000058b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000058c0: 2020 2020 2020 2020 2020 7379 732e 7374            sys.st
-000058d0: 6465 7272 2e66 6c75 7368 2829 0d0a 0d0a  derr.flush()....
-000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 2020 2020 2320 496e 6372 656d 656e 7420      # Increment 
-00005900: 7468 6520 6572 726f 7220 636f 7272 6563  the error correc
-00005910: 7469 6f6e 2063 6f75 6e74 6572 2061 6e64  tion counter and
-00005920: 2075 7064 6174 6520 7468 6520 6d65 7373   update the mess
-00005930: 6167 6573 206c 6973 7420 7769 7468 2074  ages list with t
-00005940: 6865 2065 7272 6f72 0d0a 2020 2020 2020  he error..      
-00005950: 2020 2020 2020 2020 2020 2020 2020 6572                er
-00005960: 726f 725f 636f 7272 6563 7469 6f6e 7320  ror_corrections 
-00005970: 2b3d 2031 0d0a 2020 2020 2020 2020 2020  += 1..          
-00005980: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00005990: 6573 2e61 7070 656e 6428 7b22 726f 6c65  es.append({"role
-000059a0: 223a 2022 7573 6572 222c 2022 636f 6e74  ": "user", "cont
-000059b0: 656e 7422 3a20 7365 6c66 2e65 7272 6f72  ent": self.error
-000059c0: 5f63 6f72 7265 6374 5f74 6173 6b2e 666f  _correct_task.fo
-000059d0: 726d 6174 2865 297d 290d 0a0d 0a20 2020  rmat(e)})....   
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059f0: 2023 2053 7769 7463 6820 746f 2067 7074   # Switch to gpt
-00005a00: 2d34 2069 6620 6c6c 6d5f 7377 6974 6368  -4 if llm_switch
-00005a10: 2070 6172 616d 6574 6572 2069 7320 7365   parameter is se
-00005a20: 7420 746f 2054 7275 652e 2054 6869 7320  t to True. This 
-00005a30: 7769 6c6c 2069 6e63 7265 6173 6520 7468  will increase th
-00005a40: 6520 7072 6f63 6573 7369 6e67 2074 696d  e processing tim
-00005a50: 6520 616e 6420 636f 7374 2e0d 0a20 2020  e and cost...   
-00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a70: 2069 6620 7365 6c66 2e6c 6c6d 5f73 7769   if self.llm_swi
-00005a80: 7463 683a 0d0a 2020 2020 2020 2020 2020  tch:..          
-00005a90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005aa0: 6c66 2e6c 6c6d 203d 2027 6770 742d 3427  lf.llm = 'gpt-4'
-00005ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005ac0: 2020 2020 2020 2020 2020 6966 2027 6970            if 'ip
-00005ad0: 796b 6572 6e65 6c27 2069 6e20 7379 732e  ykernel' in sys.
-00005ae0: 6d6f 6475 6c65 733a 0d0a 2020 2020 2020  modules:..      
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2020 2020 2320 4a75 7079 7465 7220        # Jupyter 
-00005b10: 6e6f 7465 626f 6f6b 0d0a 2020 2020 2020  notebook..      
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b30: 2020 2020 2020 6469 7370 6c61 7928 4854        display(HT
-00005b40: 4d4c 2827 3c73 7061 6e20 7374 796c 653d  ML('<span style=
-00005b50: 2263 6f6c 6f72 3a20 2364 3836 6330 303b  "color: #d86c00;
-00005b60: 223e 5377 6974 6368 696e 6720 6d6f 6465  ">Switching mode
-00005b70: 6c20 746f 2067 7074 2d34 2074 6f20 7472  l to gpt-4 to tr
-00005b80: 7920 746f 2069 6d70 726f 7665 2074 6865  y to improve the
-00005b90: 206f 7574 636f 6d65 2e3c 2f73 7061 6e3e   outcome.</span>
-00005ba0: 2729 290d 0a20 2020 2020 2020 2020 2020  '))..           
-00005bb0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00005bc0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005be0: 2320 434c 490d 0a20 2020 2020 2020 2020  # CLI..         
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2020 2073 7973 2e73 7464 6572 722e 7772     sys.stderr.wr
-00005c10: 6974 6528 275c 3033 335b 3331 6d27 202b  ite('\033[31m' +
-00005c20: 2066 273e 2053 7769 7463 6869 6e67 206d   f'> Switching m
-00005c30: 6f64 656c 2074 6f20 6770 742d 3420 746f  odel to gpt-4 to
-00005c40: 2074 7279 2074 6f20 696d 7072 6f76 6520   try to improve 
-00005c50: 7468 6520 6f75 7463 6f6d 652e 2720 2b20  the outcome.' + 
-00005c60: 275c 3033 335b 306d 2720 2b20 275c 6e27  '\033[0m' + '\n'
-00005c70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005c90: 7973 2e73 7464 6572 722e 666c 7573 6828  ys.stderr.flush(
-00005ca0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00005cb0: 2020 2020 2020 2020 2023 2041 7474 656d           # Attem
-00005cc0: 7074 2074 6f20 636f 7272 6563 7420 7468  pt to correct th
-00005cd0: 6520 636f 6465 2061 6e64 2068 616e 646c  e code and handl
-00005ce0: 6520 7261 7465 206c 696d 6974 2065 7272  e rate limit err
-00005cf0: 6f72 730d 0a20 2020 2020 2020 2020 2020  ors..           
-00005d00: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2020 206c 6c6d 5f72 6573 706f         llm_respo
-00005d30: 6e73 652c 2074 6f6b 656e 735f 7573 6564  nse, tokens_used
-00005d40: 203d 2073 656c 662e 6c6c 6d5f 6361 6c6c   = self.llm_call
-00005d50: 286d 6573 7361 6765 7329 0d0a 2020 2020  (messages)..    
-00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d70: 2020 2020 636f 6465 2c72 6566 6c65 6374      code,reflect
-00005d80: 696f 6e2c 666c 6f77 203d 2073 656c 662e  ion,flow = self.
-00005d90: 5f65 7874 7261 6374 5f63 6f64 6528 6c6c  _extract_code(ll
-00005da0: 6d5f 7265 7370 6f6e 7365 290d 0a20 2020  m_response)..   
+00000030: 340d 0a69 6d70 6f72 7420 6a73 6f6e 0d0a  4..import json..
+00000040: 6672 6f6d 2063 6f6e 7465 7874 6c69 6220  from contextlib 
+00000050: 696d 706f 7274 2072 6564 6972 6563 745f  import redirect_
+00000060: 7374 646f 7574 0d0a 696d 706f 7274 2069  stdout..import i
+00000070: 6f0d 0a69 6d70 6f72 7420 7469 6d65 0d0a  o..import time..
+00000080: 696d 706f 7274 206f 7065 6e61 690d 0a69  import openai..i
+00000090: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
+000000a0: 7064 0d0a 6672 6f6d 2074 6572 6d63 6f6c  pd..from termcol
+000000b0: 6f72 2069 6d70 6f72 7420 636f 6c6f 7265  or import colore
+000000c0: 642c 2063 7072 696e 740d 0a66 726f 6d20  d, cprint..from 
+000000d0: 4950 7974 686f 6e2e 6469 7370 6c61 7920  IPython.display 
+000000e0: 696d 706f 7274 2064 6973 706c 6179 2c20  import display, 
+000000f0: 496d 6167 652c 2048 544d 4c0d 0a69 6d70  Image, HTML..imp
+00000100: 6f72 7420 7761 726e 696e 6773 0d0a 7761  ort warnings..wa
+00000110: 726e 696e 6773 2e66 696c 7465 7277 6172  rnings.filterwar
+00000120: 6e69 6e67 7328 2769 676e 6f72 6527 290d  nings('ignore').
+00000130: 0a23 5275 6e6e 696e 6720 6173 2061 2073  .#Running as a s
+00000140: 6372 6970 740d 0a23 696d 706f 7274 2070  cript..#import p
+00000150: 726f 6d70 7473 0d0a 2369 6d70 6f72 7420  rompts..#import 
+00000160: 6675 6e63 5f63 616c 6c73 0d0a 2352 756e  func_calls..#Run
+00000170: 6e69 6e67 2061 7320 6120 7061 636b 6167  ning as a packag
+00000180: 650d 0a66 726f 6d20 2e20 696d 706f 7274  e..from . import
+00000190: 2070 726f 6d70 7473 0d0a 6672 6f6d 202e   prompts..from .
+000001a0: 2069 6d70 6f72 7420 6675 6e63 5f63 616c   import func_cal
+000001b0: 6c73 0d0a 0d0a 636c 6173 7320 4261 6d62  ls....class Bamb
+000001c0: 6f6f 4149 3a0d 0a20 2020 2064 6566 205f  ooAI:..    def _
+000001d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6466  _init__(self, df
+000001e0: 3a20 7064 2e44 6174 6146 7261 6d65 2c0d  : pd.DataFrame,.
+000001f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000200: 2020 6d61 785f 636f 6e76 6572 7361 7469    max_conversati
+00000210: 6f6e 733a 2069 6e74 203d 2034 2c0d 0a20  ons: int = 4,.. 
+00000220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000230: 6c6c 6d3a 2073 7472 203d 2027 6770 742d  llm: str = 'gpt-
+00000240: 332e 352d 7475 7262 6f2d 3036 3133 272c  3.5-turbo-0613',
+00000250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000260: 2020 206c 6c6d 5f66 756e 633a 2073 7472     llm_func: str
+00000270: 203d 2027 6770 742d 332e 352d 7475 7262   = 'gpt-3.5-turb
+00000280: 6f2d 3036 3133 272c 0d0a 2020 2020 2020  o-0613',..      
+00000290: 2020 2020 2020 2020 2020 206c 6c6d 5f31             llm_1
+000002a0: 366b 3a20 7374 7220 3d20 2767 7074 2d33  6k: str = 'gpt-3
+000002b0: 2e35 2d74 7572 626f 2d31 366b 272c 0d0a  .5-turbo-16k',..
+000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002d0: 206c 6c6d 5f67 7074 343a 2073 7472 203d   llm_gpt4: str =
+000002e0: 2027 6770 742d 342d 3036 3133 272c 0d0a   'gpt-4-0613',..
+000002f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000300: 2064 6562 7567 3a20 626f 6f6c 203d 2046   debug: bool = F
+00000310: 616c 7365 2c20 0d0a 2020 2020 2020 2020  alse, ..        
+00000320: 2020 2020 2020 2020 2072 616e 6b3a 2062           rank: b
+00000330: 6f6f 6c20 3d20 4661 6c73 652c 200d 0a20  ool = False, .. 
+00000340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000350: 6c6c 6d5f 7377 6974 6368 3a20 626f 6f6c  llm_switch: bool
+00000360: 203d 2046 616c 7365 2c20 0d0a 2020 2020   = False, ..    
+00000370: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+00000380: 6c6f 7261 746f 7279 3a20 626f 6f6c 203d  loratory: bool =
+00000390: 2054 7275 652c 200d 0a20 2020 2020 2020   True, ..       
+000003a0: 2020 2020 2020 2020 2020 293a 0d0a 0d0a            ):....
+000003b0: 2020 2020 2020 2020 7365 6c66 2e41 5049          self.API
+000003c0: 5f4b 4559 203d 206f 732e 656e 7669 726f  _KEY = os.enviro
+000003d0: 6e2e 6765 7428 274f 5045 4e41 495f 4150  n.get('OPENAI_AP
+000003e0: 495f 4b45 5927 290d 0a20 2020 2020 2020  I_KEY')..       
+000003f0: 2073 656c 662e 4d41 585f 4552 524f 525f   self.MAX_ERROR_
+00000400: 434f 5252 4543 5449 4f4e 5320 3d20 350d  CORRECTIONS = 5.
+00000410: 0a20 2020 2020 2020 2023 2053 6574 2074  .        # Set t
+00000420: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
+00000430: 7220 6f66 2071 7565 7374 696f 6e2f 616e  r of question/an
+00000440: 7377 6572 2070 6169 7273 2074 6f20 6265  swer pairs to be
+00000450: 206b 6570 7420 696e 2074 6865 2063 6f6e   kept in the con
+00000460: 7665 7273 6174 696f 6e20 6d65 6d6d 6f72  versation memmor
+00000470: 790d 0a20 2020 2020 2020 2073 656c 662e  y..        self.
+00000480: 4d41 585f 434f 4e56 4552 5341 5449 4f4e  MAX_CONVERSATION
+00000490: 5320 3d20 286d 6178 5f63 6f6e 7665 7273  S = (max_convers
+000004a0: 6174 696f 6e73 2a32 2920 2d20 310d 0a20  ations*2) - 1.. 
+000004b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000004c0: 2023 2053 746f 7265 2074 6865 206f 7269   # Store the ori
+000004d0: 6769 6e61 6c20 6461 7461 6672 616d 652e  ginal dataframe.
+000004e0: 2054 6869 7320 7769 6c6c 2062 6520 7573   This will be us
+000004f0: 6564 2074 6f20 7265 7365 7420 7468 6520  ed to reset the 
+00000500: 6461 7461 6672 616d 6520 6265 666f 7265  dataframe before
+00000510: 2065 7865 6375 7469 6e67 2074 6865 2063   executing the c
+00000520: 6f64 650d 0a20 2020 2020 2020 2073 656c  ode..        sel
+00000530: 662e 6f72 6967 696e 616c 5f64 6620 3d20  f.original_df = 
+00000540: 6466 0d0a 2020 2020 2020 2020 7365 6c66  df..        self
+00000550: 2e64 6620 3d20 6466 2e63 6f70 7928 2920  .df = df.copy() 
+00000560: 2023 206d 616b 6520 6120 636f 7079 206f   # make a copy o
+00000570: 6620 7468 6520 6461 7461 6672 616d 650d  f the dataframe.
+00000580: 0a20 2020 2020 2020 2073 656c 662e 6466  .        self.df
+00000590: 5f68 6561 6420 3d20 7365 6c66 2e6f 7269  _head = self.ori
+000005a0: 6769 6e61 6c5f 6466 2e68 6561 6428 3129  ginal_df.head(1)
+000005b0: 0d0a 0d0a 2020 2020 2020 2020 2320 4c4c  ....        # LL
+000005c0: 4d73 0d0a 2020 2020 2020 2020 7365 6c66  Ms..        self
+000005d0: 2e6c 6c6d 203d 206c 6c6d 0d0a 2020 2020  .llm = llm..    
+000005e0: 2020 2020 7365 6c66 2e6c 6c6d 5f66 756e      self.llm_fun
+000005f0: 6320 3d20 6c6c 6d5f 6675 6e63 0d0a 2020  c = llm_func..  
+00000600: 2020 2020 2020 7365 6c66 2e6c 6c6d 5f31        self.llm_1
+00000610: 366b 203d 206c 6c6d 5f31 366b 0d0a 2020  6k = llm_16k..  
+00000620: 2020 2020 2020 7365 6c66 2e6c 6c6d 5f67        self.llm_g
+00000630: 7074 3420 3d20 6c6c 6d5f 6770 7434 0d0a  pt4 = llm_gpt4..
+00000640: 0d0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
+00000650: 7468 6520 6465 6275 6720 6d6f 6465 2e20  the debug mode. 
+00000660: 5468 6973 206d 6f64 6520 6973 2054 7275  This mode is Tru
+00000670: 6520 7768 656e 2079 6f75 2077 616e 7420  e when you want 
+00000680: 7468 6520 6d6f 6465 6c20 746f 2064 6562  the model to deb
+00000690: 7567 2074 6865 2063 6f64 6520 616e 6420  ug the code and 
+000006a0: 636f 7272 6563 7420 6974 2e0d 0a20 2020  correct it...   
+000006b0: 2020 2020 2073 656c 662e 6465 6275 6720       self.debug 
+000006c0: 3d20 6465 6275 670d 0a20 2020 2020 2020  = debug..       
+000006d0: 2023 2053 6574 2074 6865 206c 6c6d 5f73   # Set the llm_s
+000006e0: 7769 7463 6820 6d6f 6465 2e20 5468 6973  witch mode. This
+000006f0: 206d 6f64 6520 6973 2054 7275 6520 7768   mode is True wh
+00000700: 656e 2079 6f75 2077 616e 7420 7468 6520  en you want the 
+00000710: 6d6f 6465 6c20 746f 2073 7769 7463 6820  model to switch 
+00000720: 746f 2067 7074 2d34 2066 6f72 2064 6562  to gpt-4 for deb
+00000730: 7567 6769 6e67 2c20 6572 726f 7220 636f  ugging, error co
+00000740: 7272 6563 7469 6f6e 2061 6e64 2072 616e  rrection and ran
+00000750: 6b69 6e67 2e0d 0a20 2020 2020 2020 2073  king...        s
+00000760: 656c 662e 6c6c 6d5f 7377 6974 6368 203d  elf.llm_switch =
+00000770: 206c 6c6d 5f73 7769 7463 680d 0a20 2020   llm_switch..   
+00000780: 2020 2020 2023 2053 6574 2074 6865 2072       # Set the r
+00000790: 616e 6b20 6d6f 6465 2e20 5468 6973 206d  ank mode. This m
+000007a0: 6f64 6520 6973 2054 7275 6520 7768 656e  ode is True when
+000007b0: 2079 6f75 2077 616e 7420 7468 6520 6d6f   you want the mo
+000007c0: 6465 6c20 746f 2072 616e 6b20 7468 6520  del to rank the 
+000007d0: 6765 6e65 7261 7465 6420 636f 6465 2e0d  generated code..
+000007e0: 0a20 2020 2020 2020 2073 656c 662e 7261  .        self.ra
+000007f0: 6e6b 203d 2072 616e 6b0d 0a0d 0a20 2020  nk = rank....   
+00000800: 2020 2020 2023 2053 6574 2074 6865 2065       # Set the e
+00000810: 7870 6c6f 7261 746f 7279 206d 6f64 652e  xploratory mode.
+00000820: 2054 6869 7320 6d6f 6465 2069 7320 5472   This mode is Tr
+00000830: 7565 2077 6865 6e20 796f 7520 7761 6e74  ue when you want
+00000840: 2074 6865 206d 6f64 656c 2074 6f20 6576   the model to ev
+00000850: 616c 7561 7465 2074 6865 206f 7269 6769  aluate the origi
+00000860: 6e61 6c20 7072 6f6d 7074 2061 6e64 2062  nal prompt and b
+00000870: 7265 616b 2069 7420 646f 776e 2069 6e20  reak it down in 
+00000880: 6865 7572 6973 7469 6320 616c 676f 7269  heuristic algori
+00000890: 7468 6d2e 0d0a 2020 2020 2020 2020 7365  thm...        se
+000008a0: 6c66 2e65 7870 6c6f 7261 746f 7279 203d  lf.exploratory =
+000008b0: 2065 7870 6c6f 7261 746f 7279 0d0a 2020   exploratory..  
+000008c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000008d0: 2320 5072 6f6d 7074 730d 0a20 2020 2020  # Prompts..     
+000008e0: 2020 2073 656c 662e 7461 736b 5f65 7661     self.task_eva
+000008f0: 6c75 6174 696f 6e20 3d20 7072 6f6d 7074  luation = prompt
+00000900: 732e 7461 736b 5f65 7661 6c75 6174 696f  s.task_evaluatio
+00000910: 6e0d 0a20 2020 2020 2020 2073 656c 662e  n..        self.
+00000920: 7379 7374 656d 5f74 6173 6b20 3d20 7072  system_task = pr
+00000930: 6f6d 7074 732e 7379 7374 656d 5f74 6173  ompts.system_tas
+00000940: 6b0d 0a20 2020 2020 2020 2073 656c 662e  k..        self.
+00000950: 7461 736b 203d 2070 726f 6d70 7473 2e74  task = prompts.t
+00000960: 6173 6b0d 0a20 2020 2020 2020 2073 656c  ask..        sel
+00000970: 662e 6572 726f 725f 636f 7272 6563 745f  f.error_correct_
+00000980: 7461 736b 203d 2070 726f 6d70 7473 2e65  task = prompts.e
+00000990: 7272 6f72 5f63 6f72 7265 6374 5f74 6173  rror_correct_tas
+000009a0: 6b0d 0a20 2020 2020 2020 2073 656c 662e  k..        self.
+000009b0: 6465 6275 675f 636f 6465 5f74 6173 6b20  debug_code_task 
+000009c0: 3d20 7072 6f6d 7074 732e 6465 6275 675f  = prompts.debug_
+000009d0: 636f 6465 5f74 6173 6b20 200d 0a20 2020  code_task  ..   
+000009e0: 2020 2020 2073 656c 662e 7261 6e6b 5f61       self.rank_a
+000009f0: 6e73 7765 7220 3d20 7072 6f6d 7074 732e  nswer = prompts.
+00000a00: 7261 6e6b 5f61 6e73 7765 720d 0a20 2020  rank_answer..   
+00000a10: 2020 2020 2073 656c 662e 736f 6c75 7469       self.soluti
+00000a20: 6f6e 5f69 6e73 6967 6874 7320 3d20 7072  on_insights = pr
+00000a30: 6f6d 7074 732e 736f 6c75 7469 6f6e 5f69  ompts.solution_i
+00000a40: 6e73 6967 6874 730d 0a0d 0a20 2020 2020  nsights....     
+00000a50: 2020 2023 2046 756e 6374 696f 6e73 0d0a     # Functions..
+00000a60: 2020 2020 2020 2020 7365 6c66 2e74 6173          self.tas
+00000a70: 6b5f 6576 616c 5f66 756e 6374 696f 6e20  k_eval_function 
+00000a80: 3d20 6675 6e63 5f63 616c 6c73 2e74 6173  = func_calls.tas
+00000a90: 6b5f 6576 616c 5f66 756e 6374 696f 6e0d  k_eval_function.
+00000aa0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00000ab0: 7369 6768 7473 5f66 756e 6374 696f 6e20  sights_function 
+00000ac0: 3d20 6675 6e63 5f63 616c 6c73 2e73 6f6c  = func_calls.sol
+00000ad0: 7574 696f 6e5f 696e 7369 6768 7473 5f66  ution_insights_f
+00000ae0: 756e 6374 696f 6e0d 0a20 2020 2020 2020  unction..       
+00000af0: 200d 0a20 2020 2020 2020 206f 7065 6e61   ..        opena
+00000b00: 692e 6170 695f 6b65 7920 3d20 7365 6c66  i.api_key = self
+00000b10: 2e41 5049 5f4b 4559 0d0a 0d0a 2020 2020  .API_KEY....    
+00000b20: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
+00000b30: 2074 6865 2074 6f74 616c 2074 6f6b 656e   the total token
+00000b40: 7320 7573 6564 206c 6973 742e 2054 6869  s used list. Thi
+00000b50: 7320 6c69 7374 2077 696c 6c20 6265 2075  s list will be u
+00000b60: 7365 6420 746f 206b 6565 7020 7472 6163  sed to keep trac
+00000b70: 6b20 6f66 2074 6865 2074 6f74 616c 2074  k of the total t
+00000b80: 6f6b 656e 7320 7573 6564 2062 7920 7468  okens used by th
+00000b90: 6520 6d6f 6465 6c0d 0a20 2020 2020 2020  e model..       
+00000ba0: 2073 656c 662e 746f 7461 6c5f 746f 6b65   self.total_toke
+00000bb0: 6e73 5f75 7365 6420 3d20 5b5d 0d0a 0d0a  ns_used = []....
+00000bc0: 2020 2020 6465 6620 6c6c 6d5f 6361 6c6c      def llm_call
+00000bd0: 2873 656c 662c 206d 6573 7361 6765 733a  (self, messages:
+00000be0: 2073 7472 2c20 7465 6d70 6572 6174 7572   str, temperatur
+00000bf0: 653a 2066 6c6f 6174 203d 2030 2c20 6d61  e: float = 0, ma
+00000c00: 785f 746f 6b65 6e73 3a20 696e 7420 3d20  x_tokens: int = 
+00000c10: 3130 3030 2c20 6c6c 6d5f 6361 7363 6164  1000, llm_cascad
+00000c20: 653a 2062 6f6f 6c20 3d20 4661 6c73 6529  e: bool = False)
+00000c30: 3a0d 0a20 2020 2020 2020 206d 6f64 656c  :..        model
+00000c40: 203d 2073 656c 662e 6c6c 6d0d 0a20 2020   = self.llm..   
+00000c50: 2020 2020 2069 6620 6c6c 6d5f 6361 7363       if llm_casc
+00000c60: 6164 653a 0d0a 2020 2020 2020 2020 2020  ade:..          
+00000c70: 2020 6d6f 6465 6c20 3d20 7365 6c66 2e6c    model = self.l
+00000c80: 6c6d 5f67 7074 340d 0a20 2020 2020 2020  lm_gpt4..       
+00000c90: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00000ca0: 2020 2072 6573 706f 6e73 6520 3d20 6f70     response = op
+00000cb0: 656e 6169 2e43 6861 7443 6f6d 706c 6574  enai.ChatComplet
+00000cc0: 696f 6e2e 6372 6561 7465 280d 0a20 2020  ion.create(..   
+00000cd0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+00000ce0: 656c 3d6d 6f64 656c 2c0d 0a20 2020 2020  el=model,..     
+00000cf0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00000d00: 6765 733d 6d65 7373 6167 6573 2c0d 0a20  ges=messages,.. 
+00000d10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00000d20: 656d 7065 7261 7475 7265 3d74 656d 7065  emperature=tempe
+00000d30: 7261 7475 7265 2c0d 0a20 2020 2020 2020  rature,..       
+00000d40: 2020 2020 2020 2020 206d 6178 5f74 6f6b           max_tok
+00000d50: 656e 733d 6d61 785f 746f 6b65 6e73 2c0d  ens=max_tokens,.
+00000d60: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00000d70: 2020 2020 2020 2020 6578 6365 7074 206f          except o
+00000d80: 7065 6e61 692e 6572 726f 722e 5261 7465  penai.error.Rate
+00000d90: 4c69 6d69 7445 7272 6f72 3a0d 0a20 2020  LimitError:..   
+00000da0: 2020 2020 2020 2020 2070 7269 6e74 280d           print(.
+00000db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000dc0: 2022 5468 6520 4f70 656e 4149 2041 5049   "The OpenAI API
+00000dd0: 2072 6174 6520 6c69 6d69 7420 6861 7320   rate limit has 
+00000de0: 6265 656e 2065 7863 6565 6465 642e 2057  been exceeded. W
+00000df0: 6169 7469 6e67 2031 3020 7365 636f 6e64  aiting 10 second
+00000e00: 7320 616e 6420 7472 7969 6e67 2061 6761  s and trying aga
+00000e10: 696e 2e22 0d0a 2020 2020 2020 2020 2020  in."..          
+00000e20: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00000e30: 2074 696d 652e 736c 6565 7028 3130 290d   time.sleep(10).
+00000e40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00000e50: 706f 6e73 6520 3d20 6f70 656e 6169 2e43  ponse = openai.C
+00000e60: 6861 7443 6f6d 706c 6574 696f 6e2e 6372  hatCompletion.cr
+00000e70: 6561 7465 280d 0a20 2020 2020 2020 2020  eate(..         
+00000e80: 2020 2020 2020 206d 6f64 656c 3d6d 6f64         model=mod
+00000e90: 656c 2c0d 0a20 2020 2020 2020 2020 2020  el,..           
+00000ea0: 2020 2020 206d 6573 7361 6765 733d 6d65       messages=me
+00000eb0: 7373 6167 6573 2c0d 0a20 2020 2020 2020  ssages,..       
+00000ec0: 2020 2020 2020 2020 2074 656d 7065 7261           tempera
+00000ed0: 7475 7265 3d74 656d 7065 7261 7475 7265  ture=temperature
+00000ee0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000ef0: 2020 206d 6178 5f74 6f6b 656e 733d 6d61     max_tokens=ma
+00000f00: 785f 746f 6b65 6e73 2c0d 0a20 2020 2020  x_tokens,..     
+00000f10: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00000f20: 2020 2320 4578 6365 6564 6564 2074 6865    # Exceeded the
+00000f30: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
+00000f40: 6f66 2074 6f6b 656e 7320 616c 6c6f 7765  of tokens allowe
+00000f50: 6420 6279 2074 6865 2041 5049 0d0a 2020  d by the API..  
+00000f60: 2020 2020 2020 6578 6365 7074 206f 7065        except ope
+00000f70: 6e61 692e 6572 726f 722e 496e 7661 6c69  nai.error.Invali
+00000f80: 6452 6571 7565 7374 4572 726f 723a 0d0a  dRequestError:..
+00000f90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000fa0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00000fb0: 2020 2020 2254 6865 204f 7065 6e41 4920      "The OpenAI 
+00000fc0: 4150 4920 6d61 7869 6d75 6d20 746f 6b65  API maximum toke
+00000fd0: 6e73 206c 696d 6974 2068 6173 2062 6565  ns limit has bee
+00000fe0: 6e20 6578 6365 6564 6564 2e20 5377 6974  n exceeded. Swit
+00000ff0: 6368 696e 6720 746f 2061 2031 364b 206d  ching to a 16K m
+00001000: 6f64 656c 2e22 0d0a 2020 2020 2020 2020  odel."..        
+00001010: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00001020: 2020 2072 6573 706f 6e73 6520 3d20 6f70     response = op
+00001030: 656e 6169 2e43 6861 7443 6f6d 706c 6574  enai.ChatComplet
+00001040: 696f 6e2e 6372 6561 7465 280d 0a20 2020  ion.create(..   
+00001050: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+00001060: 656c 3d73 656c 662e 6c6c 6d5f 3136 6b2c  el=self.llm_16k,
+00001070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001080: 2020 6d65 7373 6167 6573 3d6d 6573 7361    messages=messa
+00001090: 6765 732c 0d0a 2020 2020 2020 2020 2020  ges,..          
+000010a0: 2020 2020 2020 7465 6d70 6572 6174 7572        temperatur
+000010b0: 653d 7465 6d70 6572 6174 7572 652c 0d0a  e=temperature,..
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010d0: 6d61 785f 746f 6b65 6e73 3d6d 6178 5f74  max_tokens=max_t
+000010e0: 6f6b 656e 732c 0d0a 2020 2020 2020 2020  okens,..        
+000010f0: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+00001100: 2063 6f6e 7465 6e74 203d 2072 6573 706f   content = respo
+00001110: 6e73 652e 6368 6f69 6365 735b 305d 2e6d  nse.choices[0].m
+00001120: 6573 7361 6765 2e63 6f6e 7465 6e74 2e73  essage.content.s
+00001130: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
+00001140: 746f 6b65 6e73 5f75 7365 6420 3d20 7265  tokens_used = re
+00001150: 7370 6f6e 7365 2e75 7361 6765 2e74 6f74  sponse.usage.tot
+00001160: 616c 5f74 6f6b 656e 730d 0a0d 0a20 2020  al_tokens....   
+00001170: 2020 2020 2072 6574 7572 6e20 636f 6e74       return cont
+00001180: 656e 742c 2074 6f6b 656e 735f 7573 6564  ent, tokens_used
+00001190: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+000011a0: 6c6c 6d5f 6675 6e63 5f63 616c 6c28 7365  llm_func_call(se
+000011b0: 6c66 2c20 6d65 7373 6167 6573 2c20 6675  lf, messages, fu
+000011c0: 6e63 7469 6f6e 732c 2066 756e 6374 696f  nctions, functio
+000011d0: 6e5f 6e61 6d65 293a 0d0a 2020 2020 2020  n_name):..      
+000011e0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+000011f0: 2020 2020 7265 7370 6f6e 7365 203d 206f      response = o
+00001200: 7065 6e61 692e 4368 6174 436f 6d70 6c65  penai.ChatComple
+00001210: 7469 6f6e 2e63 7265 6174 6528 0d0a 2020  tion.create(..  
+00001220: 2020 2020 2020 2020 2020 6d6f 6465 6c20            model 
+00001230: 3d20 7365 6c66 2e6c 6c6d 5f66 756e 632c  = self.llm_func,
+00001240: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
+00001250: 7373 6167 6573 3d6d 6573 7361 6765 732c  ssages=messages,
+00001260: 0d0a 2020 2020 2020 2020 2020 2020 6675  ..            fu
+00001270: 6e63 7469 6f6e 733d 6675 6e63 7469 6f6e  nctions=function
+00001280: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+00001290: 6675 6e63 7469 6f6e 5f63 616c 6c20 3d20  function_call = 
+000012a0: 6675 6e63 7469 6f6e 5f6e 616d 652c 0d0a  function_name,..
+000012b0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+000012c0: 6572 6174 7572 653d 302c 0d0a 2020 2020  erature=0,..    
+000012d0: 2020 2020 2020 2020 6d61 785f 746f 6b65          max_toke
+000012e0: 6e73 203d 2037 3030 2c20 0d0a 2020 2020  ns = 700, ..    
+000012f0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00001300: 2020 2065 7863 6570 7420 6f70 656e 6169     except openai
+00001310: 2e65 7272 6f72 2e52 6174 654c 696d 6974  .error.RateLimit
+00001320: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
+00001330: 2020 2020 7072 696e 7428 0d0a 2020 2020      print(..    
+00001340: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+00001350: 204f 7065 6e41 4920 4150 4920 7261 7465   OpenAI API rate
+00001360: 206c 696d 6974 2068 6173 2062 6565 6e20   limit has been 
+00001370: 6578 6365 6564 6564 2e20 5761 6974 696e  exceeded. Waitin
+00001380: 6720 3130 2073 6563 6f6e 6473 2061 6e64  g 10 seconds and
+00001390: 2074 7279 696e 6720 6167 6169 6e2e 220d   trying again.".
+000013a0: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+000013b0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+000013c0: 2e73 6c65 6570 2831 3029 0d0a 2020 2020  .sleep(10)..    
+000013d0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+000013e0: 203d 206f 7065 6e61 692e 4368 6174 436f   = openai.ChatCo
+000013f0: 6d70 6c65 7469 6f6e 2e63 7265 6174 6528  mpletion.create(
+00001400: 0d0a 2020 2020 2020 2020 2020 2020 6d6f  ..            mo
+00001410: 6465 6c20 3d20 7365 6c66 2e6c 6c6d 5f66  del = self.llm_f
+00001420: 756e 632c 0d0a 2020 2020 2020 2020 2020  unc,..          
+00001430: 2020 6d65 7373 6167 6573 3d6d 6573 7361    messages=messa
+00001440: 6765 732c 0d0a 2020 2020 2020 2020 2020  ges,..          
+00001450: 2020 6675 6e63 7469 6f6e 733d 6675 6e63    functions=func
+00001460: 7469 6f6e 732c 0d0a 2020 2020 2020 2020  tions,..        
+00001470: 2020 2020 6675 6e63 7469 6f6e 5f63 616c      function_cal
+00001480: 6c20 3d20 6675 6e63 7469 6f6e 5f6e 616d  l = function_nam
+00001490: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000014a0: 7465 6d70 6572 6174 7572 653d 302c 0d0a  temperature=0,..
+000014b0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+000014c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000014d0: 2066 6e5f 6e61 6d65 203d 2072 6573 706f   fn_name = respo
+000014e0: 6e73 652e 6368 6f69 6365 735b 305d 2e6d  nse.choices[0].m
+000014f0: 6573 7361 6765 5b22 6675 6e63 7469 6f6e  essage["function
+00001500: 5f63 616c 6c22 5d2e 6e61 6d65 0d0a 2020  _call"].name..  
+00001510: 2020 2020 2020 6172 6775 6d65 6e74 7320        arguments 
+00001520: 3d20 7265 7370 6f6e 7365 2e63 686f 6963  = response.choic
+00001530: 6573 5b30 5d2e 6d65 7373 6167 655b 2266  es[0].message["f
+00001540: 756e 6374 696f 6e5f 6361 6c6c 225d 2e61  unction_call"].a
+00001550: 7267 756d 656e 7473 0d0a 2020 2020 2020  rguments..      
+00001560: 2020 746f 6b65 6e73 5f75 7365 6420 3d20    tokens_used = 
+00001570: 7265 7370 6f6e 7365 2e75 7361 6765 2e74  response.usage.t
+00001580: 6f74 616c 5f74 6f6b 656e 730d 0a0d 0a20  otal_tokens.... 
+00001590: 2020 2020 2020 2072 6574 7572 6e20 666e         return fn
+000015a0: 5f6e 616d 652c 6172 6775 6d65 6e74 732c  _name,arguments,
+000015b0: 746f 6b65 6e73 5f75 7365 640d 0a0d 0a20  tokens_used.... 
+000015c0: 2020 200d 0a20 2020 2023 2046 756e 6374     ..    # Funct
+000015d0: 696f 6e73 2074 6f20 7361 6e69 7469 7a65  ions to sanitize
+000015e0: 2074 6865 206f 7574 7075 7420 6672 6f6d   the output from
+000015f0: 2074 6865 204c 4c4d 0d0a 2020 2020 6465   the LLM..    de
+00001600: 6620 5f65 7874 7261 6374 5f63 6f64 6528  f _extract_code(
+00001610: 7365 6c66 2c72 6573 706f 6e73 653a 2073  self,response: s
+00001620: 7472 2c20 7365 7061 7261 746f 723a 2073  tr, separator: s
+00001630: 7472 203d 2022 6060 6022 2920 2d3e 2073  tr = "```") -> s
+00001640: 7472 3a0d 0a0d 0a20 2020 2020 2020 2023  tr:....        #
+00001650: 2044 6566 696e 6520 6120 626c 6163 6b6c   Define a blackl
+00001660: 6973 7420 6f66 2050 7974 686f 6e20 6b65  ist of Python ke
+00001670: 7977 6f72 6473 2061 6e64 2066 756e 6374  ywords and funct
+00001680: 696f 6e73 2074 6861 7420 6172 6520 6e6f  ions that are no
+00001690: 7420 616c 6c6f 7765 640d 0a20 2020 2020  t allowed..     
+000016a0: 2020 2062 6c61 636b 6c69 7374 203d 205b     blacklist = [
+000016b0: 276f 7327 2c27 7375 6270 726f 6365 7373  'os','subprocess
+000016c0: 272c 2773 7973 272c 2765 7661 6c27 2c27  ','sys','eval','
+000016d0: 6578 6563 272c 2766 696c 6527 2c27 736f  exec','file','so
+000016e0: 636b 6574 272c 2775 726c 6c69 6227 2c0d  cket','urllib',.
+000016f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001700: 2020 2020 2027 7368 7574 696c 272c 2770       'shutil','p
+00001710: 6963 6b6c 6527 2c27 6374 7970 6573 272c  ickle','ctypes',
+00001720: 276d 756c 7469 7072 6f63 6573 7369 6e67  'multiprocessing
+00001730: 272c 2774 656d 7066 696c 6527 2c27 676c  ','tempfile','gl
+00001740: 6f62 272c 2763 6f64 6527 2c27 7074 7927  ob','code','pty'
+00001750: 2c27 636f 6d6d 616e 6473 272c 0d0a 2020  ,'commands',..  
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2020 2772 6571 7565 7374 7327 2c27 6367    'requests','cg
+00001780: 6927 2c27 6367 6974 6227 2c27 786d 6c2e  i','cgitb','xml.
+00001790: 6574 7265 652e 456c 656d 656e 7454 7265  etree.ElementTre
+000017a0: 6527 2c27 6275 696c 7469 6e73 270d 0a20  e','builtins'.. 
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017c0: 2020 205d 0d0a 0d0a 2020 2020 2020 2020     ]....        
+000017d0: 2320 5365 6172 6368 2066 6f72 2061 2070  # Search for a p
+000017e0: 6174 7465 726e 2062 6574 7765 656e 203c  attern between <
+000017f0: 636f 6465 3e20 616e 6420 3c2f 636f 6465  code> and </code
+00001800: 3e20 696e 2074 6865 2065 7874 7261 6374  > in the extract
+00001810: 6564 2063 6f64 650d 0a20 2020 2020 2020  ed code..       
+00001820: 206d 6174 6368 203d 2072 652e 7365 6172   match = re.sear
+00001830: 6368 2872 223c 636f 6465 3e28 2e2a 293c  ch(r"<code>(.*)<
+00001840: 2f63 6f64 653e 222c 2072 6573 706f 6e73  /code>", respons
+00001850: 652c 2072 652e 444f 5441 4c4c 290d 0a20  e, re.DOTALL).. 
+00001860: 2020 2020 2020 2069 6620 6d61 7463 683a         if match:
+00001870: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00001880: 4966 2061 206d 6174 6368 2069 7320 666f  If a match is fo
+00001890: 756e 642c 2065 7874 7261 6374 2074 6865  und, extract the
+000018a0: 2063 6f64 6520 6265 7477 6565 6e20 3c63   code between <c
+000018b0: 6f64 653e 2061 6e64 203c 2f63 6f64 653e  ode> and </code>
+000018c0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+000018d0: 6465 203d 206d 6174 6368 2e67 726f 7570  de = match.group
+000018e0: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
+000018f0: 2023 2049 6620 7468 6520 7265 7370 6f6e   # If the respon
+00001900: 7365 2063 6f6e 7461 696e 7320 7468 6520  se contains the 
+00001910: 7365 7061 7261 746f 722c 2065 7874 7261  separator, extra
+00001920: 6374 2074 6865 2063 6f64 6520 626c 6f63  ct the code bloc
+00001930: 6b20 6265 7477 6565 6e20 7468 6520 7365  k between the se
+00001940: 7061 7261 746f 7273 0d0a 2020 2020 2020  parators..      
+00001950: 2020 2020 2020 6966 206c 656e 2863 6f64        if len(cod
+00001960: 652e 7370 6c69 7428 7365 7061 7261 746f  e.split(separato
+00001970: 7229 2920 3e20 313a 0d0a 2020 2020 2020  r)) > 1:..      
+00001980: 2020 2020 2020 2020 2020 636f 6465 203d            code =
+00001990: 2063 6f64 652e 7370 6c69 7428 7365 7061   code.split(sepa
+000019a0: 7261 746f 7229 5b31 5d0d 0a0d 0a20 2020  rator)[1]....   
+000019b0: 2020 2020 2023 2049 6620 7468 6520 7265       # If the re
+000019c0: 7370 6f6e 7365 2063 6f6e 7461 696e 7320  sponse contains 
+000019d0: 7468 6520 7365 7061 7261 746f 722c 2065  the separator, e
+000019e0: 7874 7261 6374 2074 6865 2063 6f64 6520  xtract the code 
+000019f0: 626c 6f63 6b20 6265 7477 6565 6e20 7468  block between th
+00001a00: 6520 7365 7061 7261 746f 7273 0d0a 2020  e separators..  
+00001a10: 2020 2020 2020 6966 206c 656e 2872 6573        if len(res
+00001a20: 706f 6e73 652e 7370 6c69 7428 7365 7061  ponse.split(sepa
+00001a30: 7261 746f 7229 2920 3e20 313a 0d0a 2020  rator)) > 1:..  
+00001a40: 2020 2020 2020 2020 2020 636f 6465 203d            code =
+00001a50: 2072 6573 706f 6e73 652e 7370 6c69 7428   response.split(
+00001a60: 7365 7061 7261 746f 7229 5b31 5d0d 0a20  separator)[1].. 
+00001a70: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00001a80: 2020 2020 2023 2052 656d 6f76 6520 7468       # Remove th
+00001a90: 6520 2270 7974 686f 6e22 206f 7220 2270  e "python" or "p
+00001aa0: 7922 2070 7265 6669 7820 6966 2070 7265  y" prefix if pre
+00001ab0: 7365 6e74 0d0a 2020 2020 2020 2020 6966  sent..        if
+00001ac0: 2072 652e 6d61 7463 6828 7222 5e28 7079   re.match(r"^(py
+00001ad0: 7468 6f6e 7c70 7929 222c 2063 6f64 6529  thon|py)", code)
+00001ae0: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00001af0: 6f64 6520 3d20 7265 2e73 7562 2872 225e  ode = re.sub(r"^
+00001b00: 2870 7974 686f 6e7c 7079 2922 2c20 2222  (python|py)", ""
+00001b10: 2c20 636f 6465 290d 0a20 2020 2020 2020  , code)..       
+00001b20: 2023 2049 6620 7468 6520 636f 6465 2069   # If the code i
+00001b30: 7320 6265 7477 6565 6e20 7369 6e67 6c65  s between single
+00001b40: 2062 6163 6b74 6963 6b73 2c20 6578 7472   backticks, extr
+00001b50: 6163 7420 7468 6520 636f 6465 2062 6574  act the code bet
+00001b60: 7765 656e 2074 6865 6d0d 0a20 2020 2020  ween them..     
+00001b70: 2020 2069 6620 7265 2e6d 6174 6368 2872     if re.match(r
+00001b80: 225e 602e 2a60 2422 2c20 636f 6465 293a  "^`.*`$", code):
+00001b90: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00001ba0: 6465 203d 2072 652e 7375 6228 7222 5e60  de = re.sub(r"^`
+00001bb0: 282e 2a29 6024 222c 2072 225c 3122 2c20  (.*)`$", r"\1", 
+00001bc0: 636f 6465 290d 0a0d 0a20 2020 2020 2020  code)....       
+00001bd0: 2023 2052 656d 6f76 6520 616e 7920 696e   # Remove any in
+00001be0: 7374 616e 6365 7320 6f66 2022 6466 203d  stances of "df =
+00001bf0: 2070 642e 7265 6164 5f63 7376 2827 6669   pd.read_csv('fi
+00001c00: 6c65 6e61 6d65 2e63 7376 2729 2220 6672  lename.csv')" fr
+00001c10: 6f6d 2074 6865 2063 6f64 650d 0a20 2020  om the code..   
+00001c20: 2020 2020 2063 6f64 6520 3d20 7265 2e73       code = re.s
+00001c30: 7562 2872 2264 665c 732a 3d5c 732a 7064  ub(r"df\s*=\s*pd
+00001c40: 5c2e 7265 6164 5f63 7376 5c28 272e 2a3f  \.read_csv\('.*?
+00001c50: 2728 2c2e 2a29 3f5c 2922 2c20 2222 2c20  '(,.*)?\)", "", 
+00001c60: 636f 6465 290d 0a0d 0a20 2020 2020 2020  code)....       
+00001c70: 2023 2044 6566 696e 6520 7468 6520 7265   # Define the re
+00001c80: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+00001c90: 2070 6174 7465 726e 2074 6f20 6d61 7463   pattern to matc
+00001ca0: 6820 7468 6520 626c 6163 6b6c 6973 7420  h the blacklist 
+00001cb0: 6974 656d 730d 0a20 2020 2020 2020 2070  items..        p
+00001cc0: 6174 7465 726e 203d 2072 225e 282e 2a5c  attern = r"^(.*\
+00001cd0: 6228 2220 2b20 227c 222e 6a6f 696e 2862  b(" + "|".join(b
+00001ce0: 6c61 636b 6c69 7374 2920 2b20 7222 295c  lacklist) + r")\
+00001cf0: 622e 2a29 2422 0d0a 0d0a 2020 2020 2020  b.*)$"....      
+00001d00: 2020 2320 5265 706c 6163 6520 7468 6520    # Replace the 
+00001d10: 626c 6163 6b6c 6973 7420 6974 656d 7320  blacklist items 
+00001d20: 7769 7468 2063 6f6d 6d65 6e74 730d 0a20  with comments.. 
+00001d30: 2020 2020 2020 2063 6f64 6520 3d20 7265         code = re
+00001d40: 2e73 7562 2870 6174 7465 726e 2c20 7222  .sub(pattern, r"
+00001d50: 2320 6e6f 7420 616c 6c6f 7765 6420 5c31  # not allowed \1
+00001d60: 222c 2063 6f64 652c 2066 6c61 6773 3d72  ", code, flags=r
+00001d70: 652e 4d55 4c54 494c 494e 4529 0d0a 0d0a  e.MULTILINE)....
+00001d80: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+00001d90: 2074 6865 2063 6c65 616e 6564 2061 6e64   the cleaned and
+00001da0: 2065 7874 7261 6374 6564 2063 6f64 650d   extracted code.
+00001db0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001dc0: 636f 6465 2e73 7472 6970 2829 0d0a 2020  code.strip()..  
+00001dd0: 2020 0d0a 2020 2020 6465 6620 5f65 7874    ..    def _ext
+00001de0: 7261 6374 5f72 616e 6b28 7365 6c66 2c72  ract_rank(self,r
+00001df0: 6573 706f 6e73 653a 2073 7472 2920 2d3e  esponse: str) ->
+00001e00: 2073 7472 3a0d 0a0d 0a20 2020 2020 2020   str:....       
+00001e10: 2023 2053 6561 7263 6820 666f 7220 6120   # Search for a 
+00001e20: 7061 7474 6572 6e20 6265 7477 6565 6e20  pattern between 
+00001e30: 3c72 616e 6b3e 2061 6e64 203c 2f72 616e  <rank> and </ran
+00001e40: 6b3e 2069 6e20 7468 6520 7265 7370 6f6e  k> in the respon
+00001e50: 7365 0d0a 2020 2020 2020 2020 6d61 7463  se..        matc
+00001e60: 6820 3d20 7265 2e73 6561 7263 6828 7222  h = re.search(r"
+00001e70: 3c72 616e 6b3e 282e 2a29 3c2f 7261 6e6b  <rank>(.*)</rank
+00001e80: 3e22 2c20 7265 7370 6f6e 7365 290d 0a20  >", response).. 
+00001e90: 2020 2020 2020 2069 6620 6d61 7463 683a         if match:
+00001ea0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00001eb0: 4966 2061 206d 6174 6368 2069 7320 666f  If a match is fo
+00001ec0: 756e 642c 2065 7874 7261 6374 2074 6865  und, extract the
+00001ed0: 2072 616e 6b20 6265 7477 6565 6e20 3c72   rank between <r
+00001ee0: 616e 6b3e 2061 6e64 203c 2f72 616e 6b3e  ank> and </rank>
+00001ef0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00001f00: 6e6b 203d 206d 6174 6368 2e67 726f 7570  nk = match.group
+00001f10: 2831 290d 0a20 2020 2020 2020 2065 6c73  (1)..        els
+00001f20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001f30: 7261 6e6b 203d 2022 220d 0a0d 0a20 2020  rank = ""....   
+00001f40: 2020 2020 2023 2052 6574 7572 6e20 7468       # Return th
+00001f50: 6520 636c 6561 6e65 6420 616e 6420 6578  e cleaned and ex
+00001f60: 7472 6163 7465 6420 636f 6465 0d0a 2020  tracted code..  
+00001f70: 2020 2020 2020 7265 7475 726e 2072 616e        return ran
+00001f80: 6b2e 7374 7269 7028 290d 0a20 2020 200d  k.strip()..    .
+00001f90: 0a20 2020 2064 6566 2074 6173 6b5f 6576  .    def task_ev
+00001fa0: 616c 2873 656c 662c 2065 7661 6c5f 6d65  al(self, eval_me
+00001fb0: 7373 6167 6573 293a 0d0a 0d0a 2020 2020  ssages):....    
+00001fc0: 2020 2020 6966 2027 6970 796b 6572 6e65      if 'ipykerne
+00001fd0: 6c27 2069 6e20 7379 732e 6d6f 6475 6c65  l' in sys.module
+00001fe0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00001ff0: 2320 4a75 7079 7465 7220 6e6f 7465 626f  # Jupyter notebo
+00002000: 6f6b 206f 7220 6970 7974 686f 6e0d 0a20  ok or ipython.. 
+00002010: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00002020: 6179 2848 544d 4c28 6627 3c70 2073 7479  ay(HTML(f'<p sty
+00002030: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
+00002040: 613b 223e 5c6e 4361 6c6c 696e 6720 4d6f  a;">\nCalling Mo
+00002050: 6465 6c3a 207b 7365 6c66 2e6c 6c6d 5f66  del: {self.llm_f
+00002060: 756e 637d 3c2f 703e 2729 290d 0a20 2020  unc}</p>'))..   
+00002070: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00002080: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
+00002090: 796c 653d 2263 6f6c 6f72 3a6d 6167 656e  yle="color:magen
+000020a0: 7461 3b22 3e54 7279 696e 6720 746f 2064  ta;">Trying to d
+000020b0: 6574 6572 6d69 6e65 2074 6865 2062 6573  etermine the bes
+000020c0: 7420 6d65 7468 6f64 2074 6f20 616e 7377  t method to answ
+000020d0: 6572 2079 6f75 7220 7175 6573 7469 6f6e  er your question
+000020e0: 2c20 706c 6561 7365 2077 6169 742e 2e2e  , please wait...
+000020f0: 3c2f 623e 3c2f 703e 3c62 723e 2729 290d  </b></p><br>')).
+00002100: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00002110: 2020 2020 2020 2020 2020 2020 2320 4f74              # Ot
+00002120: 6865 7220 656e 7669 726f 6e6d 656e 7420  her environment 
+00002130: 286c 696b 6520 7465 726d 696e 616c 290d  (like terminal).
+00002140: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00002150: 6e74 2863 6f6c 6f72 6564 2866 225c 6e3e  nt(colored(f"\n>
+00002160: 3e20 4361 6c6c 696e 6720 4d6f 6465 6c3a  > Calling Model:
+00002170: 207b 7365 6c66 2e6c 6c6d 5f66 756e 637d   {self.llm_func}
+00002180: 222c 2022 6d61 6765 6e74 6122 2929 0d0a  ", "magenta"))..
+00002190: 2020 2020 2020 2020 2020 2020 6370 7269              cpri
+000021a0: 6e74 2866 225c 6e3e 3e20 5472 7969 6e67  nt(f"\n>> Trying
+000021b0: 2074 6f20 6465 7465 726d 696e 6520 7468   to determine th
+000021c0: 6520 6265 7374 206d 6574 686f 6420 746f  e best method to
+000021d0: 2061 6e73 7765 7220 796f 7572 2071 7565   answer your que
+000021e0: 7374 696f 6e2c 2070 6c65 6173 6520 7761  stion, please wa
+000021f0: 6974 2e2e 2e5c 6e22 2c20 276d 6167 656e  it...\n", 'magen
+00002200: 7461 272c 2061 7474 7273 3d5b 2762 6f6c  ta', attrs=['bol
+00002210: 6427 5d29 0d0a 0d0a 2020 2020 2020 2020  d'])....        
+00002220: 2320 4361 6c6c 204f 7065 6e41 4920 4150  # Call OpenAI AP
+00002230: 490d 0a20 2020 2020 2020 2066 756e 6374  I..        funct
+00002240: 696f 6e5f 6e61 6d65 203d 207b 226e 616d  ion_name = {"nam
+00002250: 6522 3a20 2251 415f 5265 7370 6f6e 7365  e": "QA_Response
+00002260: 227d 0d0a 2020 2020 2020 2020 666e 5f6e  "}..        fn_n
+00002270: 616d 652c 2061 7267 756d 656e 7473 2c20  ame, arguments, 
+00002280: 746f 6b65 6e73 5f75 7365 6420 3d20 7365  tokens_used = se
+00002290: 6c66 2e6c 6c6d 5f66 756e 635f 6361 6c6c  lf.llm_func_call
+000022a0: 2865 7661 6c5f 6d65 7373 6167 6573 2c73  (eval_messages,s
+000022b0: 656c 662e 7461 736b 5f65 7661 6c5f 6675  elf.task_eval_fu
+000022c0: 6e63 7469 6f6e 2c20 6675 6e63 7469 6f6e  nction, function
+000022d0: 5f6e 616d 6529 0d0a 0d0a 2020 2020 2020  _name)....      
+000022e0: 2020 2320 5061 7273 6520 7468 6520 4a53    # Parse the JS
+000022f0: 4f4e 2073 7472 696e 6720 746f 2061 2050  ON string to a P
+00002300: 7974 686f 6e20 6469 6374 0d0a 2020 2020  ython dict..    
+00002310: 2020 2020 6172 6775 6d65 6e74 735f 6469      arguments_di
+00002320: 6374 203d 206a 736f 6e2e 6c6f 6164 7328  ct = json.loads(
+00002330: 6172 6775 6d65 6e74 732c 2073 7472 6963  arguments, stric
+00002340: 743d 4661 6c73 6529 0d0a 0d0a 2020 2020  t=False)....    
+00002350: 2020 2020 2320 5265 7472 6965 7665 2076      # Retrieve v
+00002360: 616c 7565 730d 0a20 2020 2020 2020 2065  alues..        e
+00002370: 7661 6c5f 616e 7377 6572 203d 2061 7267  val_answer = arg
+00002380: 756d 656e 7473 5f64 6963 745b 2261 6e73  uments_dict["ans
+00002390: 7765 7222 5d0d 0a20 2020 2020 2020 2065  wer"]..        e
+000023a0: 7661 6c5f 616e 7377 6572 5f74 7970 6520  val_answer_type 
+000023b0: 3d20 6172 6775 6d65 6e74 735f 6469 6374  = arguments_dict
+000023c0: 5b22 616e 7377 6572 5f74 7970 6522 5d0d  ["answer_type"].
+000023d0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+000023e0: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
+000023f0: 642e 6170 7065 6e64 2874 6f6b 656e 735f  d.append(tokens_
+00002400: 7573 6564 290d 0a0d 0a20 2020 2020 2020  used)....       
+00002410: 2072 6574 7572 6e20 6172 6775 6d65 6e74   return argument
+00002420: 732c 2066 6e5f 6e61 6d65 2c20 6576 616c  s, fn_name, eval
+00002430: 5f61 6e73 7765 722c 2065 7661 6c5f 616e  _answer, eval_an
+00002440: 7377 6572 5f74 7970 650d 0a0d 0a20 2020  swer_type....   
+00002450: 2064 6566 2064 6562 7567 5f63 6f64 6528   def debug_code(
+00002460: 7365 6c66 2c63 6f64 652c 7175 6573 7469  self,code,questi
+00002470: 6f6e 2c20 6c6c 6d5f 6361 7363 6164 653d  on, llm_cascade=
+00002480: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00002490: 2023 2049 6e69 7469 616c 697a 6520 7468   # Initialize th
+000024a0: 6520 6d65 7373 6167 6573 206c 6973 7420  e messages list 
+000024b0: 7769 7468 2061 2073 7973 7465 6d20 6d65  with a system me
+000024c0: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
+000024d0: 2074 6865 2074 6173 6b20 7072 6f6d 7074   the task prompt
+000024e0: 0d0a 2020 2020 2020 2020 6465 6275 675f  ..        debug_
+000024f0: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
+00002500: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
+00002510: 636f 6e74 656e 7422 3a20 7365 6c66 2e64  content": self.d
+00002520: 6562 7567 5f63 6f64 655f 7461 736b 2e66  ebug_code_task.f
+00002530: 6f72 6d61 7428 636f 6465 2c71 7565 7374  ormat(code,quest
+00002540: 696f 6e29 7d5d 0d0a 0d0a 2020 2020 2020  ion)}]....      
+00002550: 2020 7573 696e 675f 6d6f 6465 6c20 3d20    using_model = 
+00002560: 7365 6c66 2e6c 6c6d 0d0a 2020 2020 2020  self.llm..      
+00002570: 2020 6966 206c 6c6d 5f63 6173 6361 6465    if llm_cascade
+00002580: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
+00002590: 7369 6e67 5f6d 6f64 656c 203d 2073 656c  sing_model = sel
+000025a0: 662e 6c6c 6d5f 6770 7434 0d0a 0d0a 2020  f.llm_gpt4....  
+000025b0: 2020 2020 2020 6966 2027 6970 796b 6572        if 'ipyker
+000025c0: 6e65 6c27 2069 6e20 7379 732e 6d6f 6475  nel' in sys.modu
+000025d0: 6c65 733a 0d0a 2020 2020 2020 2020 2020  les:..          
+000025e0: 2020 2320 4a75 7079 7465 7220 6e6f 7465    # Jupyter note
+000025f0: 626f 6f6b 206f 7220 6970 7974 686f 6e0d  book or ipython.
+00002600: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00002610: 706c 6179 2848 544d 4c28 6627 3c70 2073  play(HTML(f'<p s
+00002620: 7479 6c65 3d22 636f 6c6f 723a 6d61 6765  tyle="color:mage
+00002630: 6e74 613b 223e 5c6e 4361 6c6c 696e 6720  nta;">\nCalling 
+00002640: 4d6f 6465 6c3a 207b 7573 696e 675f 6d6f  Model: {using_mo
+00002650: 6465 6c7d 3c2f 703e 2729 290d 0a20 2020  del}</p>'))..   
+00002660: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00002670: 2848 544d 4c28 6627 3c70 3e3c 6220 7374  (HTML(f'<p><b st
+00002680: 796c 653d 2263 6f6c 6f72 3a6d 6167 656e  yle="color:magen
+00002690: 7461 3b22 3e49 2068 6176 6520 7265 6365  ta;">I have rece
+000026a0: 6976 6564 2074 6865 2066 6972 7374 2076  ived the first v
+000026b0: 6572 7369 6f6e 206f 6620 7468 6520 636f  ersion of the co
+000026c0: 6465 2e20 4920 616d 2073 656e 6469 6e67  de. I am sending
+000026d0: 2069 7420 6261 636b 2074 6f20 4c4c 4d20   it back to LLM 
+000026e0: 746f 2067 6574 2069 7420 6368 6563 6b65  to get it checke
+000026f0: 6420 666f 7220 616e 7920 6572 726f 7273  d for any errors
+00002700: 2c20 6275 6773 206f 7220 696e 636f 6e73  , bugs or incons
+00002710: 6973 7465 6e63 6965 732c 2061 6e64 2063  istencies, and c
+00002720: 6f72 7265 6374 696f 6e20 6966 206e 6563  orrection if nec
+00002730: 6573 7361 7279 2e20 506c 6561 7365 2077  essary. Please w
+00002740: 6169 742e 2e2e 3c2f 623e 3c2f 703e 3c62  ait...</b></p><b
+00002750: 723e 2729 290d 0a20 2020 2020 2020 2065  r>'))..        e
+00002760: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00002770: 2020 2320 4f74 6865 7220 656e 7669 726f    # Other enviro
+00002780: 6e6d 656e 7420 286c 696b 6520 7465 726d  nment (like term
+00002790: 696e 616c 290d 0a20 2020 2020 2020 2020  inal)..         
+000027a0: 2020 2070 7269 6e74 2863 6f6c 6f72 6564     print(colored
+000027b0: 2866 225c 6e3e 3e20 4361 6c6c 696e 6720  (f"\n>> Calling 
+000027c0: 4d6f 6465 6c3a 207b 7573 696e 675f 6d6f  Model: {using_mo
+000027d0: 6465 6c7d 222c 2022 6d61 6765 6e74 6122  del}", "magenta"
+000027e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000027f0: 6370 7269 6e74 2866 225c 6e3e 3e20 4920  cprint(f"\n>> I 
+00002800: 6861 7665 2072 6563 6569 7665 6420 7468  have received th
+00002810: 6520 6669 7273 7420 7665 7273 696f 6e20  e first version 
+00002820: 6f66 2074 6865 2063 6f64 652e 2049 2061  of the code. I a
+00002830: 6d20 7365 6e64 696e 6720 6974 2062 6163  m sending it bac
+00002840: 6b20 746f 204c 4c4d 2074 6f20 6765 7420  k to LLM to get 
+00002850: 6974 2063 6865 636b 6564 2066 6f72 2061  it checked for a
+00002860: 6e79 2065 7272 6f72 732c 2062 7567 7320  ny errors, bugs 
+00002870: 6f72 2069 6e63 6f6e 7369 7374 656e 6369  or inconsistenci
+00002880: 6573 2c20 616e 6420 636f 7272 6563 7469  es, and correcti
+00002890: 6f6e 2069 6620 6e65 6365 7373 6172 792e  on if necessary.
+000028a0: 2050 6c65 6173 6520 7761 6974 2e2e 2e5c   Please wait...\
+000028b0: 6e22 2c20 276d 6167 656e 7461 272c 2061  n", 'magenta', a
+000028c0: 7474 7273 3d5b 2762 6f6c 6427 5d29 0d0a  ttrs=['bold'])..
+000028d0: 0d0a 2020 2020 2020 2020 2320 4675 6e63  ..        # Func
+000028e0: 7469 6f6e 2074 6f20 6469 7370 6c61 7920  tion to display 
+000028f0: 7265 7375 6c74 7320 6e69 6365 6c79 0d0a  results nicely..
+00002900: 2020 2020 2020 2020 6465 6620 6469 7370          def disp
+00002910: 6c61 795f 7461 736b 2829 3a0d 0a20 2020  lay_task():..   
+00002920: 2020 2020 2020 2020 2069 6620 2769 7079           if 'ipy
+00002930: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
+00002940: 6f64 756c 6573 3a0d 0a20 2020 2020 2020  odules:..       
+00002950: 2020 2020 2020 2020 2023 204a 7570 7974           # Jupyt
+00002960: 6572 206e 6f74 6562 6f6f 6b20 6f72 2069  er notebook or i
+00002970: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
+00002980: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
+00002990: 4854 4d4c 2866 273c 703e 3c62 2073 7479  HTML(f'<p><b sty
+000029a0: 6c65 3d22 636f 6c6f 723a 6d61 6765 6e74  le="color:magent
+000029b0: 613b 223e 4920 6861 7665 2066 696e 6973  a;">I have finis
+000029c0: 6865 6420 6465 6275 6767 696e 6720 7468  hed debugging th
+000029d0: 6520 636f 6465 2c20 616e 6420 7769 6c6c  e code, and will
+000029e0: 206e 6f77 2070 726f 6365 6564 2074 6f20   now proceed to 
+000029f0: 7468 6520 6578 6563 7574 696f 6e2e 2e2e  the execution...
+00002a00: 3c2f 623e 3c2f 703e 3c62 723e 2729 290d  </b></p><br>')).
+00002a10: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00002a20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002a30: 2020 2020 2320 4f74 6865 7220 656e 7669      # Other envi
+00002a40: 726f 6e6d 656e 7420 286c 696b 6520 7465  ronment (like te
+00002a50: 726d 696e 616c 290d 0a20 2020 2020 2020  rminal)..       
+00002a60: 2020 2020 2020 2020 2063 7072 696e 7428           cprint(
+00002a70: 6622 5c6e 3e3e 2049 2068 6176 6520 6669  f"\n>> I have fi
+00002a80: 6e69 7368 6564 2064 6562 7567 6769 6e67  nished debugging
+00002a90: 2074 6865 2063 6f64 652c 2061 6e64 2077   the code, and w
+00002aa0: 696c 6c20 6e6f 7720 7072 6f63 6565 6420  ill now proceed 
+00002ab0: 746f 2074 6865 2065 7865 6375 7469 6f6e  to the execution
+00002ac0: 2e2e 2e5c 6e22 2c20 276d 6167 656e 7461  ...\n", 'magenta
+00002ad0: 272c 2061 7474 7273 3d5b 2762 6f6c 6427  ', attrs=['bold'
+00002ae0: 5d29 0d0a 0d0a 2020 2020 2020 2020 2320  ])....        # 
+00002af0: 4361 6c6c 2074 6865 204f 7065 6e41 4920  Call the OpenAI 
+00002b00: 4150 490d 0a20 2020 2020 2020 206c 6c6d  API..        llm
+00002b10: 5f72 6573 706f 6e73 652c 2074 6f6b 656e  _response, token
+00002b20: 735f 7573 6564 203d 2073 656c 662e 6c6c  s_used = self.ll
+00002b30: 6d5f 6361 6c6c 2864 6562 7567 5f6d 6573  m_call(debug_mes
+00002b40: 7361 6765 732c 7465 6d70 6572 6174 7572  sages,temperatur
+00002b50: 653d 302c 6c6c 6d5f 6361 7363 6164 653d  e=0,llm_cascade=
+00002b60: 6c6c 6d5f 6361 7363 6164 6529 2023 2068  llm_cascade) # h
+00002b70: 6967 6865 7220 7465 6d70 6572 6174 7572  igher temperatur
+00002b80: 6520 7265 7375 6c74 7320 696e 206d 6f72  e results in mor
+00002b90: 6520 2263 7265 6174 6976 6522 2061 6e73  e "creative" ans
+00002ba0: 7765 7273 2028 736f 6d65 7469 6d65 7320  wers (sometimes 
+00002bb0: 746f 6f20 6372 6561 7469 7665 203a 2d29  too creative :-)
+00002bc0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00002bd0: 2020 2020 2023 2045 7874 7261 6374 2074       # Extract t
+00002be0: 6865 2063 6f64 6520 6672 6f6d 2074 6865  he code from the
+00002bf0: 2041 5049 2072 6573 706f 6e73 650d 0a20   API response.. 
+00002c00: 2020 2020 2020 2064 6562 7567 6765 645f         debugged_
+00002c10: 636f 6465 203d 2073 656c 662e 5f65 7874  code = self._ext
+00002c20: 7261 6374 5f63 6f64 6528 6c6c 6d5f 7265  ract_code(llm_re
+00002c30: 7370 6f6e 7365 2920 2020 2020 2020 0d0a  sponse)       ..
+00002c40: 2020 2020 2020 2020 6469 7370 6c61 795f          display_
+00002c50: 7461 736b 2829 0d0a 0d0a 2020 2020 2020  task()....      
+00002c60: 2020 7365 6c66 2e74 6f74 616c 5f74 6f6b    self.total_tok
+00002c70: 656e 735f 7573 6564 2e61 7070 656e 6428  ens_used.append(
+00002c80: 746f 6b65 6e73 5f75 7365 6429 0d0a 0d0a  tokens_used)....
+00002c90: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00002ca0: 6562 7567 6765 645f 636f 6465 0d0a 0d0a  ebugged_code....
+00002cb0: 2020 2020 6465 6620 7261 6e6b 5f63 6f64      def rank_cod
+00002cc0: 6528 7365 6c66 2c63 6f64 652c 7175 6573  e(self,code,ques
+00002cd0: 7469 6f6e 2c6c 6c6d 5f63 6173 6361 6465  tion,llm_cascade
+00002ce0: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
+00002cf0: 2020 2320 496e 6974 6961 6c69 7a65 2074    # Initialize t
+00002d00: 6865 206d 6573 7361 6765 7320 6c69 7374  he messages list
+00002d10: 2077 6974 6820 6120 7379 7374 656d 206d   with a system m
+00002d20: 6573 7361 6765 2063 6f6e 7461 696e 696e  essage containin
+00002d30: 6720 7468 6520 7461 736b 2070 726f 6d70  g the task promp
+00002d40: 740d 0a20 2020 2020 2020 2072 616e 6b5f  t..        rank_
+00002d50: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
+00002d60: 6c65 223a 2022 7379 7374 656d 222c 2022  le": "system", "
+00002d70: 636f 6e74 656e 7422 3a20 7365 6c66 2e72  content": self.r
+00002d80: 616e 6b5f 616e 7377 6572 2e66 6f72 6d61  ank_answer.forma
+00002d90: 7428 636f 6465 2c71 7565 7374 696f 6e29  t(code,question)
+00002da0: 7d5d 0d0a 0d0a 2020 2020 2020 2020 7573  }]....        us
+00002db0: 696e 675f 6d6f 6465 6c20 3d20 7365 6c66  ing_model = self
+00002dc0: 2e6c 6c6d 0d0a 2020 2020 2020 2020 6966  .llm..        if
+00002dd0: 206c 6c6d 5f63 6173 6361 6465 3a0d 0a20   llm_cascade:.. 
+00002de0: 2020 2020 2020 2020 2020 2075 7369 6e67             using
+00002df0: 5f6d 6f64 656c 203d 2073 656c 662e 6c6c  _model = self.ll
+00002e00: 6d5f 6770 7434 0d0a 0d0a 2020 2020 2020  m_gpt4....      
+00002e10: 2020 6966 2027 6970 796b 6572 6e65 6c27    if 'ipykernel'
+00002e20: 2069 6e20 7379 732e 6d6f 6475 6c65 733a   in sys.modules:
+00002e30: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00002e40: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
+00002e50: 206f 7220 6970 7974 686f 6e0d 0a20 2020   or ipython..   
+00002e60: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00002e70: 2848 544d 4c28 6627 3c70 2073 7479 6c65  (HTML(f'<p style
+00002e80: 3d22 636f 6c6f 723a 6d61 6765 6e74 613b  ="color:magenta;
+00002e90: 223e 5c6e 4361 6c6c 696e 6720 4d6f 6465  ">\nCalling Mode
+00002ea0: 6c3a 207b 7573 696e 675f 6d6f 6465 6c7d  l: {using_model}
+00002eb0: 3c2f 703e 2729 290d 0a20 2020 2020 2020  </p>'))..       
+00002ec0: 2020 2020 2064 6973 706c 6179 2848 544d       display(HTM
+00002ed0: 4c28 6627 3c70 3e3c 6220 7374 796c 653d  L(f'<p><b style=
+00002ee0: 2263 6f6c 6f72 3a6d 6167 656e 7461 3b22  "color:magenta;"
+00002ef0: 3e49 2061 6d20 676f 696e 6720 746f 2065  >I am going to e
+00002f00: 7661 6c75 6174 6520 616e 6420 7261 6e6b  valuate and rank
+00002f10: 2074 6865 2061 6e73 7765 722e 2050 6c65   the answer. Ple
+00002f20: 6173 6520 7761 6974 2e2e 2e3c 2f62 3e3c  ase wait...</b><
+00002f30: 2f70 3e3c 6272 3e27 2929 0d0a 2020 2020  /p><br>'))..    
+00002f40: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002f50: 2020 2020 2020 2023 204f 7468 6572 2065         # Other e
+00002f60: 6e76 6972 6f6e 6d65 6e74 2028 6c69 6b65  nvironment (like
+00002f70: 2074 6572 6d69 6e61 6c29 0d0a 2020 2020   terminal)..    
+00002f80: 2020 2020 2020 2020 7072 696e 7428 636f          print(co
+00002f90: 6c6f 7265 6428 6622 5c6e 3e3e 2043 616c  lored(f"\n>> Cal
+00002fa0: 6c69 6e67 204d 6f64 656c 3a20 7b75 7369  ling Model: {usi
+00002fb0: 6e67 5f6d 6f64 656c 7d22 2c20 226d 6167  ng_model}", "mag
+00002fc0: 656e 7461 2229 290d 0a20 2020 2020 2020  enta"))..       
+00002fd0: 2020 2020 2063 7072 696e 7428 6622 5c6e       cprint(f"\n
+00002fe0: 3e3e 2049 2061 6d20 676f 696e 6720 746f  >> I am going to
+00002ff0: 2065 7661 6c75 6174 6520 616e 6420 7261   evaluate and ra
+00003000: 6e6b 2074 6865 2061 6e73 7765 722e 2050  nk the answer. P
+00003010: 6c65 6173 6520 7761 6974 2e2e 5c6e 222c  lease wait..\n",
+00003020: 2027 6d61 6765 6e74 6127 2c20 6174 7472   'magenta', attr
+00003030: 733d 5b27 626f 6c64 275d 290d 0a0d 0a20  s=['bold']).... 
+00003040: 2020 2020 2020 2023 2043 616c 6c20 7468         # Call th
+00003050: 6520 4f70 656e 4149 2041 5049 200d 0a20  e OpenAI API .. 
+00003060: 2020 2020 2020 206c 6c6d 5f72 6573 706f         llm_respo
+00003070: 6e73 652c 2074 6f6b 656e 735f 7573 6564  nse, tokens_used
+00003080: 203d 2073 656c 662e 6c6c 6d5f 6361 6c6c   = self.llm_call
+00003090: 2872 616e 6b5f 6d65 7373 6167 6573 2c6c  (rank_messages,l
+000030a0: 6c6d 5f63 6173 6361 6465 3d6c 6c6d 5f63  lm_cascade=llm_c
+000030b0: 6173 6361 6465 290d 0a0d 0a20 2020 2020  ascade)....     
+000030c0: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
+000030d0: 2063 6f64 6520 6672 6f6d 2074 6865 2041   code from the A
+000030e0: 5049 2072 6573 706f 6e73 650d 0a20 2020  PI response..   
+000030f0: 2020 2020 2072 616e 6b20 3d20 7365 6c66       rank = self
+00003100: 2e5f 6578 7472 6163 745f 7261 6e6b 286c  ._extract_rank(l
+00003110: 6c6d 5f72 6573 706f 6e73 6529 2020 2020  lm_response)    
+00003120: 2020 200d 0a0d 0a20 2020 2020 2020 2073     ....        s
+00003130: 656c 662e 746f 7461 6c5f 746f 6b65 6e73  elf.total_tokens
+00003140: 5f75 7365 642e 6170 7065 6e64 2874 6f6b  _used.append(tok
+00003150: 656e 735f 7573 6564 290d 0a0d 0a20 2020  ens_used)....   
+00003160: 2020 2020 2072 6574 7572 6e20 7261 6e6b       return rank
+00003170: 0d0a 0d0a 2020 2020 6465 6620 7064 5f61  ....    def pd_a
+00003180: 6765 6e74 5f63 6f6e 7665 7273 6528 7365  gent_converse(se
+00003190: 6c66 2c20 7175 6573 7469 6f6e 3d4e 6f6e  lf, question=Non
+000031a0: 6529 3a0d 0a20 2020 2020 2020 2023 2046  e):..        # F
+000031b0: 756e 6374 696f 6e73 2074 6f20 6469 7370  unctions to disp
+000031c0: 6c61 7920 7265 7375 6c74 7320 6e69 6365  lay results nice
+000031d0: 6c79 0d0a 2020 2020 2020 2020 6465 6620  ly..        def 
+000031e0: 6469 7370 6c61 795f 7265 7375 6c74 7328  display_results(
+000031f0: 616e 7377 6572 2c20 636f 6465 2c20 7261  answer, code, ra
+00003200: 6e6b 2c20 746f 7461 6c5f 746f 6b65 6e73  nk, total_tokens
+00003210: 5f75 7365 645f 7375 6d29 3a0d 0a20 2020  _used_sum):..   
+00003220: 2020 2020 2020 2020 2069 6620 2769 7079           if 'ipy
+00003230: 6b65 726e 656c 2720 696e 2073 7973 2e6d  kernel' in sys.m
+00003240: 6f64 756c 6573 3a20 2020 2020 0d0a 2020  odules:     ..  
+00003250: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003260: 2061 6e73 7765 7220 6973 206e 6f74 204e   answer is not N
+00003270: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00003280: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00003290: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
+000032a0: 7479 6c65 3d22 636f 6c6f 723a 626c 7565  tyle="color:blue
+000032b0: 3b22 3e49 206e 6f77 2068 6176 6520 7468  ;">I now have th
+000032c0: 6520 6669 6e61 6c20 616e 7377 6572 3a3c  e final answer:<
+000032d0: 2f62 3e3c 6272 3e3c 7072 6520 7374 796c  /b><br><pre styl
+000032e0: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b20  e="color:black; 
+000032f0: 7768 6974 652d 7370 6163 653a 2070 7265  white-space: pre
+00003300: 2d77 7261 703b 2066 6f6e 742d 7765 6967  -wrap; font-weig
+00003310: 6874 3a20 626f 6c64 3b22 3e7b 616e 7377  ht: bold;">{answ
+00003320: 6572 7d3c 2f70 7265 3e3c 2f70 3e3c 6272  er}</pre></p><br
+00003330: 3e27 2929 0d0a 2020 2020 2020 2020 2020  >'))..          
+00003340: 2020 2020 2020 6966 2063 6f64 6520 6973        if code is
+00003350: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003370: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+00003380: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
+00003390: 723a 626c 7565 3b22 3e48 6572 6520 6973  r:blue;">Here is
+000033a0: 2074 6865 2066 696e 616c 2063 6f64 6520   the final code 
+000033b0: 7468 6174 2061 6363 6f6d 706c 6973 6865  that accomplishe
+000033c0: 7320 7468 6520 7461 736b 3a3c 2f62 3e3c  s the task:</b><
+000033d0: 6272 3e3c 7072 6520 7374 796c 653d 2263  br><pre style="c
+000033e0: 6f6c 6f72 3a23 3535 3535 3535 3b22 3e7b  olor:#555555;">{
+000033f0: 636f 6465 7d3c 2f70 7265 3e3c 2f70 3e3c  code}</pre></p><
+00003400: 6272 3e27 2929 0d0a 2020 2020 2020 2020  br>'))..        
+00003410: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003420: 7261 6e6b 2061 6e64 2072 616e 6b20 6973  rank and rank is
+00003430: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003450: 6469 7370 6c61 7928 4854 4d4c 2866 273c  display(HTML(f'<
+00003460: 703e 3c62 2073 7479 6c65 3d22 636f 6c6f  p><b style="colo
+00003470: 723a 626c 7565 3b22 3e52 616e 6b3a 3c2f  r:blue;">Rank:</
+00003480: 623e 3c62 723e 3c73 7061 6e20 7374 796c  b><br><span styl
+00003490: 653d 2263 6f6c 6f72 3a62 6c61 636b 3b22  e="color:black;"
+000034a0: 3e7b 7261 6e6b 7d3c 2f73 7061 6e3e 3c2f  >{rank}</span></
+000034b0: 703e 3c62 723e 2729 290d 0a20 2020 2020  p><br>'))..     
+000034c0: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+000034d0: 6179 2848 544d 4c28 6627 3c70 3e3c 6220  ay(HTML(f'<p><b 
+000034e0: 7374 796c 653d 2263 6f6c 6f72 3a62 6c75  style="color:blu
+000034f0: 653b 223e 546f 7461 6c20 546f 6b65 6e73  e;">Total Tokens
+00003500: 2055 7365 643a 3c2f 623e 3c62 723e 3c73   Used:</b><br><s
+00003510: 7061 6e20 7374 796c 653d 2263 6f6c 6f72  pan style="color
+00003520: 3a62 6c61 636b 3b22 3e7b 746f 7461 6c5f  :black;">{total_
+00003530: 746f 6b65 6e73 5f75 7365 645f 7375 6d7d  tokens_used_sum}
+00003540: 3c2f 7370 616e 3e3c 2f70 3e3c 6272 3e27  </span></p><br>'
+00003550: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00003560: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00003570: 2020 2020 2020 2069 6620 616e 7377 6572         if answer
+00003580: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035a0: 2020 2063 7072 696e 7428 6622 5c6e 3e3e     cprint(f"\n>>
+000035b0: 2049 206e 6f77 2068 6176 6520 7468 6520   I now have the 
+000035c0: 6669 6e61 6c20 616e 7377 6572 3a5c 6e7b  final answer:\n{
+000035d0: 616e 7377 6572 7d5c 6e22 2c20 2767 7265  answer}\n", 'gre
+000035e0: 656e 272c 2061 7474 7273 3d5b 2762 6f6c  en', attrs=['bol
+000035f0: 6427 5d29 0d0a 2020 2020 2020 2020 2020  d'])..          
+00003600: 2020 2020 2020 6966 2063 6f64 6520 6973        if code is
+00003610: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003630: 6370 7269 6e74 2866 223e 3e20 4865 7265  cprint(f">> Here
+00003640: 2069 7320 7468 6520 6669 6e61 6c20 636f   is the final co
+00003650: 6465 2074 6861 7420 6163 636f 6d70 6c69  de that accompli
+00003660: 7368 6573 2074 6865 2074 6173 6b3a 5c6e  shes the task:\n
+00003670: 7b63 6f64 657d 5c6e 222c 2027 6772 6565  {code}\n", 'gree
+00003680: 6e27 2c20 6174 7472 733d 5b27 626f 6c64  n', attrs=['bold
+00003690: 275d 290d 0a20 2020 2020 2020 2020 2020  '])..           
+000036a0: 2020 2020 2069 6620 7365 6c66 2e72 616e       if self.ran
+000036b0: 6b20 616e 6420 7261 6e6b 2069 7320 6e6f  k and rank is no
+000036c0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+000036d0: 2020 2020 2020 2020 2020 2020 2063 7072               cpr
+000036e0: 696e 7428 6622 3e3e 2052 616e 6b3a 5c6e  int(f">> Rank:\n
+000036f0: 7b72 616e 6b7d 5c6e 222c 2027 6772 6565  {rank}\n", 'gree
+00003700: 6e27 2c20 6174 7472 733d 5b27 626f 6c64  n', attrs=['bold
+00003710: 275d 290d 0a20 2020 2020 2020 2020 2020  '])..           
+00003720: 2020 2020 2063 7072 696e 7428 6622 3e3e       cprint(f">>
+00003730: 2054 6f74 616c 2074 6f6b 656e 7320 7573   Total tokens us
+00003740: 6564 3a5c 6e7b 746f 7461 6c5f 746f 6b65  ed:\n{total_toke
+00003750: 6e73 5f75 7365 645f 7375 6d7d 5c6e 222c  ns_used_sum}\n",
+00003760: 2027 7965 6c6c 6f77 272c 2061 7474 7273   'yellow', attrs
+00003770: 3d5b 2762 6f6c 6427 5d29 0d0a 0d0a 2020  =['bold'])....  
+00003780: 2020 2020 2020 6465 6620 6469 7370 6c61        def displa
+00003790: 795f 6576 616c 2874 6173 6b5f 6576 616c  y_eval(task_eval
+000037a0: 2c20 7469 746c 652c 2074 6f74 616c 5f74  , title, total_t
+000037b0: 6f6b 656e 735f 7573 6564 5f73 756d 293a  okens_used_sum):
+000037c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000037d0: 2027 6970 796b 6572 6e65 6c27 2069 6e20   'ipykernel' in 
+000037e0: 7379 732e 6d6f 6475 6c65 733a 0d0a 2020  sys.modules:..  
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003800: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
+00003810: 206f 7220 6970 7974 686f 6e0d 0a20 2020   or ipython..   
+00003820: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00003830: 706c 6179 2848 544d 4c28 6627 3c70 3e3c  play(HTML(f'<p><
+00003840: 6220 7374 796c 653d 2263 6f6c 6f72 3a62  b style="color:b
+00003850: 6c75 653b 223e 7b74 6974 6c65 7d3c 2f62  lue;">{title}</b
+00003860: 3e3c 6272 3e3c 7072 6520 7374 796c 653d  ><br><pre style=
+00003870: 2263 6f6c 6f72 3a62 6c61 636b 3b20 7768  "color:black; wh
+00003880: 6974 652d 7370 6163 653a 2070 7265 2d77  ite-space: pre-w
+00003890: 7261 703b 2066 6f6e 742d 7765 6967 6874  rap; font-weight
+000038a0: 3a20 626f 6c64 3b22 3e7b 7461 736b 5f65  : bold;">{task_e
+000038b0: 7661 6c7d 3c2f 7072 653e 3c2f 703e 3c62  val}</pre></p><b
+000038c0: 723e 2729 290d 0a20 2020 2020 2020 2020  r>'))..         
+000038d0: 2020 2020 2020 2064 6973 706c 6179 2848         display(H
+000038e0: 544d 4c28 6627 3c70 3e3c 6220 7374 796c  TML(f'<p><b styl
+000038f0: 653d 2263 6f6c 6f72 3a62 6c75 653b 223e  e="color:blue;">
+00003900: 546f 7461 6c20 546f 6b65 6e73 2055 7365  Total Tokens Use
+00003910: 643a 3c2f 623e 3c62 723e 3c73 7061 6e20  d:</b><br><span 
+00003920: 7374 796c 653d 2263 6f6c 6f72 3a62 6c61  style="color:bla
+00003930: 636b 3b22 3e7b 746f 7461 6c5f 746f 6b65  ck;">{total_toke
+00003940: 6e73 5f75 7365 645f 7375 6d7d 3c2f 7370  ns_used_sum}</sp
+00003950: 616e 3e3c 2f70 3e3c 6272 3e27 2929 0d0a  an></p><br>'))..
+00003960: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00003970: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003980: 2020 2023 204f 7468 6572 2065 6e76 6972     # Other envir
+00003990: 6f6e 6d65 6e74 2028 6c69 6b65 2074 6572  onment (like ter
+000039a0: 6d69 6e61 6c29 0d0a 2020 2020 2020 2020  minal)..        
+000039b0: 2020 2020 2020 2020 6370 7269 6e74 2866          cprint(f
+000039c0: 225c 6e3e 3e20 7b74 6974 6c65 7d5c 6e7b  "\n>> {title}\n{
+000039d0: 7461 736b 5f65 7661 6c7d 5c6e 222c 2027  task_eval}\n", '
+000039e0: 6d61 6765 6e74 6127 2c20 6174 7472 733d  magenta', attrs=
+000039f0: 5b27 626f 6c64 275d 290d 0a20 2020 2020  ['bold'])..     
+00003a00: 2020 2020 2020 2020 2020 2063 7072 696e             cprin
+00003a10: 7428 6622 3e3e 2054 6f74 616c 2074 6f6b  t(f">> Total tok
+00003a20: 656e 7320 7573 6564 3a5c 6e7b 746f 7461  ens used:\n{tota
+00003a30: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
+00003a40: 6d7d 5c6e 222c 2027 7965 6c6c 6f77 272c  m}\n", 'yellow',
+00003a50: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
+00003a60: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00003a70: 2020 2020 2320 4966 2061 2071 7565 7374      # If a quest
+00003a80: 696f 6e20 6973 2070 726f 7669 6465 642c  ion is provided,
+00003a90: 2073 6b69 7020 7468 6520 696e 7075 7420   skip the input 
+00003aa0: 7072 6f6d 7074 0d0a 2020 2020 2020 2020  prompt..        
+00003ab0: 6966 2071 7565 7374 696f 6e20 6973 206e  if question is n
+00003ac0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00003ad0: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
+00003ae0: 7a65 2074 6865 206d 6573 7361 6765 7320  ze the messages 
+00003af0: 6c69 7374 2077 6974 6820 6120 7379 7374  list with a syst
+00003b00: 656d 206d 6573 7361 6765 2063 6f6e 7461  em message conta
+00003b10: 696e 696e 6720 7468 6520 7461 736b 2070  ining the task p
+00003b20: 726f 6d70 740d 0a20 2020 2020 2020 2020  rompt..         
+00003b30: 2020 206d 6573 7361 6765 7320 3d20 5b7b     messages = [{
+00003b40: 2272 6f6c 6522 3a20 2273 7973 7465 6d22  "role": "system"
+00003b50: 2c20 2263 6f6e 7465 6e74 223a 2073 656c  , "content": sel
+00003b60: 662e 7379 7374 656d 5f74 6173 6b2e 666f  f.system_task.fo
+00003b70: 726d 6174 2871 7565 7374 696f 6e29 7d5d  rmat(question)}]
+00003b80: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00003b90: 496e 6974 6961 6c69 7a65 2074 6865 206d  Initialize the m
+00003ba0: 6573 7361 6765 7320 6c69 7374 2077 6974  essages list wit
+00003bb0: 6820 6120 7379 7374 656d 206d 6573 7361  h a system messa
+00003bc0: 6765 2063 6f6e 7461 696e 696e 6720 7468  ge containing th
+00003bd0: 6520 7461 736b 2070 726f 6d70 740d 0a20  e task prompt.. 
+00003be0: 2020 2020 2020 2020 2020 2065 7661 6c5f             eval_
+00003bf0: 6d65 7373 6167 6573 203d 205b 7b22 726f  messages = [{"ro
+00003c00: 6c65 223a 2022 7573 6572 222c 2022 636f  le": "user", "co
+00003c10: 6e74 656e 7422 3a20 7365 6c66 2e74 6173  ntent": self.tas
+00003c20: 6b5f 6576 616c 7561 7469 6f6e 2e66 6f72  k_evaluation.for
+00003c30: 6d61 7428 7175 6573 7469 6f6e 2c20 7365  mat(question, se
+00003c40: 6c66 2e64 665f 6865 6164 297d 5d0d 0a0d  lf.df_head)}]...
+00003c50: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+00003c60: 616c 6c20 7468 6520 7461 736b 5f65 7661  all the task_eva
+00003c70: 6c20 6d65 7468 6f64 2077 6974 6820 7468  l method with th
+00003c80: 6520 7573 6572 2773 2071 7565 7374 696f  e user's questio
+00003c90: 6e20 6966 2074 6865 2065 7870 6c6f 7261  n if the explora
+00003ca0: 746f 7279 206d 6f64 6520 6973 2054 7275  tory mode is Tru
+00003cb0: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00003cc0: 6620 7365 6c66 2e65 7870 6c6f 7261 746f  f self.explorato
+00003cd0: 7279 2069 7320 5472 7565 3a0d 0a20 2020  ry is True:..   
+00003ce0: 2020 2020 2020 2020 2020 2020 2061 7267               arg
+00003cf0: 756d 656e 7473 2c20 666e 5f6e 616d 652c  uments, fn_name,
+00003d00: 2074 6173 6b5f 6576 616c 2c20 7461 736b   task_eval, task
+00003d10: 5f74 7970 6520 3d20 7365 6c66 2e74 6173  _type = self.tas
+00003d20: 6b5f 6576 616c 2865 7661 6c5f 6d65 7373  k_eval(eval_mess
+00003d30: 6167 6573 290d 0a20 2020 2020 2020 2020  ages)..         
+00003d40: 2020 2020 2020 2074 6f74 616c 5f74 6f6b         total_tok
+00003d50: 656e 735f 7573 6564 5f73 756d 203d 2073  ens_used_sum = s
+00003d60: 756d 2873 656c 662e 746f 7461 6c5f 746f  um(self.total_to
+00003d70: 6b65 6e73 5f75 7365 6429 0d0a 2020 2020  kens_used)..    
+00003d80: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00003d90: 6173 6b5f 7479 7065 203d 3d20 276e 6174  ask_type == 'nat
+00003da0: 7572 616c 5f6c 616e 6775 6167 6527 3a0d  ural_language':.
+00003db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003dc0: 2020 2020 2074 6974 6c65 203d 2027 4865       title = 'He
+00003dd0: 7265 2069 7320 616e 2061 6e73 7765 7220  re is an answer 
+00003de0: 746f 2079 6f75 7220 7175 6573 7469 6f6e  to your question
+00003df0: 3a27 2020 2020 2020 2020 2020 2020 2020  :'              
+00003e00: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00003e10: 2020 2020 2020 2020 2020 2064 6973 706c             displ
+00003e20: 6179 5f65 7661 6c28 7461 736b 5f65 7661  ay_eval(task_eva
+00003e30: 6c2c 2074 6974 6c65 2c20 746f 7461 6c5f  l, title, total_
+00003e40: 746f 6b65 6e73 5f75 7365 645f 7375 6d29  tokens_used_sum)
+00003e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003e60: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+00003e70: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00003e80: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00003e90: 2020 2020 2020 2020 2074 6974 6c65 203d           title =
+00003ea0: 2027 4865 7265 2069 7320 6120 7365 7175   'Here is a sequ
+00003eb0: 656e 6365 206f 6620 7374 6570 7320 7265  ence of steps re
+00003ec0: 7175 6972 6564 2074 6f20 636f 6d70 6c65  quired to comple
+00003ed0: 7465 2074 6865 2074 6173 6b3a 270d 0a20  te the task:'.. 
+00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ef0: 2020 2074 6173 6b20 3d20 7461 736b 5f65     task = task_e
+00003f00: 7661 6c0d 0a20 2020 2020 2020 2020 2020  val..           
+00003f10: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00003f20: 5f65 7661 6c28 7461 736b 5f65 7661 6c2c  _eval(task_eval,
+00003f30: 2074 6974 6c65 2c20 746f 7461 6c5f 746f   title, total_to
+00003f40: 6b65 6e73 5f75 7365 645f 7375 6d29 0d0a  kens_used_sum)..
+00003f50: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00003f60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003f70: 2020 2074 6173 6b20 3d20 7175 6573 7469     task = questi
+00003f80: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
+00003f90: 2020 2320 4361 6c6c 2074 6865 2070 645f    # Call the pd_
+00003fa0: 6167 656e 7420 6d65 7468 6f64 2077 6974  agent method wit
+00003fb0: 6820 7468 6520 7573 6572 2773 2071 7565  h the user's que
+00003fc0: 7374 696f 6e2c 2074 6865 206d 6573 7361  stion, the messa
+00003fd0: 6765 7320 6c69 7374 2c20 616e 6420 7468  ges list, and th
+00003fe0: 6520 6461 7461 6672 616d 650d 0a20 2020  e dataframe..   
+00003ff0: 2020 2020 2020 2020 2061 6e73 7765 722c           answer,
+00004000: 2063 6f64 652c 2074 6f74 616c 5f74 6f6b   code, total_tok
+00004010: 656e 735f 7573 6564 5f73 756d 203d 2073  ens_used_sum = s
+00004020: 656c 662e 7064 5f61 6765 6e74 2874 6173  elf.pd_agent(tas
+00004030: 6b2c 206d 6573 7361 6765 732c 2073 656c  k, messages, sel
+00004040: 662e 6466 290d 0a0d 0a20 2020 2020 2020  f.df)....       
+00004050: 2020 2020 2023 2052 616e 6b20 7468 6520       # Rank the 
+00004060: 4c4c 4d20 7265 7370 6f6e 7365 0d0a 2020  LLM response..  
+00004070: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00004080: 662e 7261 6e6b 3a0d 0a20 2020 2020 2020  f.rank:..       
+00004090: 2020 2020 2020 2020 2023 2053 7769 7463           # Switc
+000040a0: 6820 746f 2067 7074 2d34 2069 6620 6c6c  h to gpt-4 if ll
+000040b0: 6d5f 7377 6974 6368 2070 6172 616d 6574  m_switch paramet
+000040c0: 6572 2069 7320 7365 7420 746f 2054 7275  er is set to Tru
+000040d0: 652e 2054 6869 7320 7769 6c6c 2069 6e63  e. This will inc
+000040e0: 7265 6173 6520 7468 6520 7072 6f63 6573  rease the proces
+000040f0: 7369 6e67 2074 696d 6520 616e 6420 636f  sing time and co
+00004100: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
+00004110: 2020 2020 6966 2073 656c 662e 6c6c 6d5f      if self.llm_
+00004120: 7377 6974 6368 3a0d 0a20 2020 2020 2020  switch:..       
+00004130: 2020 2020 2020 2020 2020 2020 206c 6c6d               llm
+00004140: 5f63 6173 6361 6465 203d 2054 7275 650d  _cascade = True.
+00004150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004160: 2072 616e 6b20 3d20 7365 6c66 2e72 616e   rank = self.ran
+00004170: 6b5f 636f 6465 2863 6f64 652c 7461 736b  k_code(code,task
+00004180: 2c6c 6c6d 5f63 6173 6361 6465 3d6c 6c6d  ,llm_cascade=llm
+00004190: 5f63 6173 6361 6465 290d 0a20 2020 2020  _cascade)..     
+000041a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000041b0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000041c0: 6e6b 203d 2022 220d 0a0d 0a20 2020 2020  nk = ""....     
+000041d0: 2020 2020 2020 2064 6973 706c 6179 5f72         display_r
+000041e0: 6573 756c 7473 2861 6e73 7765 722c 2063  esults(answer, c
+000041f0: 6f64 652c 2072 616e 6b2c 2074 6f74 616c  ode, rank, total
+00004200: 5f74 6f6b 656e 735f 7573 6564 5f73 756d  _tokens_used_sum
+00004210: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+00004220: 6574 7572 6e0d 0a20 2020 2020 2020 200d  eturn..        .
+00004230: 0a20 2020 2020 2020 2023 2053 7461 7274  .        # Start
+00004240: 2061 6e20 696e 6669 6e69 7465 206c 6f6f   an infinite loo
+00004250: 7020 746f 206b 6565 7020 6173 6b69 6e67  p to keep asking
+00004260: 2074 6865 2075 7365 7220 666f 7220 7175   the user for qu
+00004270: 6573 7469 6f6e 730d 0a20 2020 2020 2020  estions..       
+00004280: 2066 6972 7374 5f69 7465 7261 7469 6f6e   first_iteration
+00004290: 203d 2054 7275 6520 2023 2046 6c61 6720   = True  # Flag 
+000042a0: 666f 7220 7468 6520 6669 7273 7420 6974  for the first it
+000042b0: 6572 6174 696f 6e20 6f66 2074 6865 206c  eration of the l
+000042c0: 6f6f 700d 0a20 2020 2020 2020 2077 6869  oop..        whi
+000042d0: 6c65 2054 7275 653a 0d0a 2020 2020 2020  le True:..      
+000042e0: 2020 2020 2020 2320 5072 6f6d 7074 2074        # Prompt t
+000042f0: 6865 2075 7365 7220 746f 2065 6e74 6572  he user to enter
+00004300: 2061 2071 7565 7374 696f 6e20 6f72 2074   a question or t
+00004310: 7970 6520 2765 7869 7427 2074 6f20 7175  ype 'exit' to qu
+00004320: 6974 0d0a 2020 2020 2020 2020 2020 2020  it..            
+00004330: 6966 2027 6970 796b 6572 6e65 6c27 2069  if 'ipykernel' i
+00004340: 6e20 7379 732e 6d6f 6475 6c65 733a 0d0a  n sys.modules:..
+00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004360: 6469 7370 6c61 7928 4854 4d4c 2827 3c62  display(HTML('<b
+00004370: 2073 7479 6c65 3d22 636f 6c6f 723a 626c   style="color:bl
+00004380: 7565 3b22 3e45 6e74 6572 2079 6f75 7220  ue;">Enter your 
+00004390: 7175 6573 7469 6f6e 206f 7220 7479 7065  question or type
+000043a0: 205c 2765 7869 745c 2720 746f 2071 7569   \'exit\' to qui
+000043b0: 743a 3c2f 623e 2729 290d 0a20 2020 2020  t:</b>'))..     
+000043c0: 2020 2020 2020 2020 2020 2074 696d 652e             time.
+000043d0: 736c 6565 7028 3129 0d0a 2020 2020 2020  sleep(1)..      
+000043e0: 2020 2020 2020 2020 2020 7175 6573 7469            questi
+000043f0: 6f6e 203d 2069 6e70 7574 2829 0d0a 2020  on = input()..  
+00004400: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00004410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004420: 2063 7072 696e 7428 225c 6e45 6e74 6572   cprint("\nEnter
+00004430: 2079 6f75 7220 7175 6573 7469 6f6e 206f   your question o
+00004440: 7220 7479 7065 2027 6578 6974 2720 746f  r type 'exit' to
+00004450: 2071 7569 743a 222c 2027 626c 7565 272c   quit:", 'blue',
+00004460: 2061 7474 7273 3d5b 2762 6f6c 6427 5d29   attrs=['bold'])
+00004470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004480: 2020 7175 6573 7469 6f6e 203d 2069 6e70    question = inp
+00004490: 7574 2829 0d0a 0d0a 2020 2020 2020 2020  ut()....        
+000044a0: 2020 2020 2320 4966 2074 6865 2075 7365      # If the use
+000044b0: 7220 7479 7065 7320 2765 7869 7427 2c20  r types 'exit', 
+000044c0: 6272 6561 6b20 6f75 7420 6f66 2074 6865  break out of the
+000044d0: 206c 6f6f 700d 0a20 2020 2020 2020 2020   loop..         
+000044e0: 2020 2069 6620 7175 6573 7469 6f6e 2e73     if question.s
+000044f0: 7472 6970 2829 2e6c 6f77 6572 2829 203d  trip().lower() =
+00004500: 3d20 2765 7869 7427 3a0d 0a20 2020 2020  = 'exit':..     
+00004510: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00004520: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00004530: 6966 2066 6972 7374 5f69 7465 7261 7469  if first_iterati
+00004540: 6f6e 3a0d 0a20 2020 2020 2020 2020 2020  on:..           
+00004550: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
+00004560: 6520 7468 6520 6d65 7373 6167 6573 206c  e the messages l
+00004570: 6973 7420 7769 7468 2061 2073 7973 7465  ist with a syste
+00004580: 6d20 6d65 7373 6167 6520 636f 6e74 6169  m message contai
+00004590: 6e69 6e67 2074 6865 2074 6173 6b20 7072  ning the task pr
+000045a0: 6f6d 7074 0d0a 2020 2020 2020 2020 2020  ompt..          
+000045b0: 2020 2020 2020 6d65 7373 6167 6573 203d        messages =
+000045c0: 205b 7b22 726f 6c65 223a 2022 7379 7374   [{"role": "syst
+000045d0: 656d 222c 2022 636f 6e74 656e 7422 3a20  em", "content": 
+000045e0: 7365 6c66 2e73 7973 7465 6d5f 7461 736b  self.system_task
+000045f0: 2e66 6f72 6d61 7428 7175 6573 7469 6f6e  .format(question
+00004600: 297d 5d0d 0a20 2020 2020 2020 2020 2020  )}]..           
+00004610: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
+00004620: 6520 7468 6520 6576 616c 5f6d 6573 7361  e the eval_messa
+00004630: 6765 7320 6c69 7374 0d0a 2020 2020 2020  ges list..      
+00004640: 2020 2020 2020 2020 2020 6576 616c 5f6d            eval_m
+00004650: 6573 7361 6765 7320 3d20 5b5d 0d0a 2020  essages = []..  
+00004660: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00004670: 7273 745f 6974 6572 6174 696f 6e20 3d20  rst_iteration = 
+00004680: 4661 6c73 6520 200d 0a20 2020 2020 2020  False  ..       
+00004690: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000046a0: 2020 2020 2020 2023 2043 616c 6c20 7468         # Call th
+000046b0: 6520 7461 736b 5f65 7661 6c20 6d65 7468  e task_eval meth
+000046c0: 6f64 2077 6974 6820 7468 6520 7573 6572  od with the user
+000046d0: 2773 2071 7565 7374 696f 6e20 6966 2074  's question if t
+000046e0: 6865 2065 7870 6c6f 7261 746f 7279 206d  he exploratory m
+000046f0: 6f64 6520 6973 2054 7275 650d 0a20 2020  ode is True..   
+00004700: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00004710: 2e65 7870 6c6f 7261 746f 7279 2069 7320  .exploratory is 
+00004720: 5472 7565 3a0d 0a20 2020 2020 2020 2020  True:..         
+00004730: 2020 2020 2020 2065 7661 6c5f 6d65 7373         eval_mess
+00004740: 6167 6573 2e61 7070 656e 6428 7b22 726f  ages.append({"ro
+00004750: 6c65 223a 2022 7573 6572 222c 2022 636f  le": "user", "co
+00004760: 6e74 656e 7422 3a20 7365 6c66 2e74 6173  ntent": self.tas
+00004770: 6b5f 6576 616c 7561 7469 6f6e 2e66 6f72  k_evaluation.for
+00004780: 6d61 7428 7175 6573 7469 6f6e 2c20 7365  mat(question, se
+00004790: 6c66 2e64 665f 6865 6164 297d 290d 0a20  lf.df_head)}).. 
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000047b0: 7267 756d 656e 7473 2c20 666e 5f6e 616d  rguments, fn_nam
+000047c0: 652c 2074 6173 6b5f 6576 616c 2c20 7461  e, task_eval, ta
+000047d0: 736b 5f74 7970 6520 3d20 7365 6c66 2e74  sk_type = self.t
+000047e0: 6173 6b5f 6576 616c 2865 7661 6c5f 6d65  ask_eval(eval_me
+000047f0: 7373 6167 6573 290d 0a20 2020 2020 2020  ssages)..       
+00004800: 2020 2020 2020 2020 2065 7661 6c5f 6d65           eval_me
+00004810: 7373 6167 6573 2e61 7070 656e 6428 0d0a  ssages.append(..
+00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004830: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+00004840: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004850: 726f 6c65 223a 2022 6173 7369 7374 616e  role": "assistan
+00004860: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
+00004870: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+00004880: 6e74 656e 7422 3a20 4e6f 6e65 2c0d 0a20  ntent": None,.. 
+00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048a0: 2020 2020 2020 2022 6675 6e63 7469 6f6e         "function
+000048b0: 5f63 616c 6c22 3a20 7b0d 0a20 2020 2020  _call": {..     
+000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048d0: 2020 2020 2020 2022 6e61 6d65 223a 2066         "name": f
+000048e0: 6e5f 6e61 6d65 2c0d 0a20 2020 2020 2020  n_name,..       
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
+00004910: 3a20 6172 6775 6d65 6e74 732c 0d0a 2020  : arguments,..  
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2020 2020 7d2c 0d0a 2020 2020 2020        },..      
+00004940: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
+00004950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004960: 2029 0d0a 0d0a 2020 2020 2020 2020 2020   )....          
+00004970: 2020 2020 2020 2320 5265 6d6f 7665 2074        # Remove t
+00004980: 6865 206f 6c64 6573 7420 636f 6e76 6572  he oldest conver
+00004990: 7361 7469 6f6e 2066 726f 6d20 7468 6520  sation from the 
+000049a0: 6d65 7373 6167 6573 206c 6973 740d 0a20  messages list.. 
+000049b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000049c0: 6620 6c65 6e28 6576 616c 5f6d 6573 7361  f len(eval_messa
+000049d0: 6765 7329 203e 2073 656c 662e 4d41 585f  ges) > self.MAX_
+000049e0: 434f 4e56 4552 5341 5449 4f4e 533a 0d0a  CONVERSATIONS:..
+000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a00: 2020 2020 6576 616c 5f6d 6573 7361 6765      eval_message
+00004a10: 732e 706f 7028 3129 0d0a 2020 2020 2020  s.pop(1)..      
+00004a20: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+00004a30: 616c 5f6d 6573 7361 6765 732e 706f 7028  al_messages.pop(
+00004a40: 3129 0d0a 0d0a 2020 2020 2020 2020 2020  1)....          
+00004a50: 2020 2020 2020 746f 7461 6c5f 746f 6b65        total_toke
+00004a60: 6e73 5f75 7365 645f 7375 6d20 3d20 7375  ns_used_sum = su
+00004a70: 6d28 7365 6c66 2e74 6f74 616c 5f74 6f6b  m(self.total_tok
+00004a80: 656e 735f 7573 6564 290d 0a0d 0a20 2020  ens_used)....   
+00004a90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004aa0: 7461 736b 5f74 7970 6520 3d3d 2027 6e61  task_type == 'na
+00004ab0: 7475 7261 6c5f 6c61 6e67 7561 6765 273a  tural_language':
+00004ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004ad0: 2020 2020 2020 7469 746c 6520 3d20 2748        title = 'H
+00004ae0: 6572 6520 6973 2061 6e20 616e 7377 6572  ere is an answer
+00004af0: 2074 6f20 796f 7572 2071 7565 7374 696f   to your questio
+00004b00: 6e3a 2720 2020 2020 2020 2020 2020 2020  n:'             
+00004b10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00004b20: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+00004b30: 6c61 795f 6576 616c 2874 6173 6b5f 6576  lay_eval(task_ev
+00004b40: 616c 2c20 7469 746c 652c 2074 6f74 616c  al, title, total
+00004b50: 5f74 6f6b 656e 735f 7573 6564 5f73 756d  _tokens_used_sum
+00004b60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00004b70: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00004b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b90: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00004ba0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+00004bb0: 6520 3d20 2748 6572 6520 6973 2061 2073  e = 'Here is a s
+00004bc0: 6571 7565 6e63 6520 6f66 2073 7465 7073  equence of steps
+00004bd0: 2072 6571 7569 7265 6420 746f 2063 6f6d   required to com
+00004be0: 706c 6574 6520 7468 6520 7461 736b 3a27  plete the task:'
+00004bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004c00: 2020 2020 2020 7461 736b 203d 2074 6173        task = tas
+00004c10: 6b5f 6576 616c 0d0a 2020 2020 2020 2020  k_eval..        
+00004c20: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+00004c30: 6c61 795f 6576 616c 2874 6173 6b5f 6576  lay_eval(task_ev
+00004c40: 616c 2c20 7469 746c 652c 2074 6f74 616c  al, title, total
+00004c50: 5f74 6f6b 656e 735f 7573 6564 5f73 756d  _tokens_used_sum
+00004c60: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00004c70: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00004c80: 2020 2020 2020 7461 736b 203d 2071 7565        task = que
+00004c90: 7374 696f 6e0d 0a0d 0a20 2020 2020 2020  stion....       
+00004ca0: 2020 2020 2023 2043 616c 6c20 7468 6520       # Call the 
+00004cb0: 7064 5f61 6765 6e74 206d 6574 686f 6420  pd_agent method 
+00004cc0: 7769 7468 2074 6865 2075 7365 7227 7320  with the user's 
+00004cd0: 7175 6573 7469 6f6e 2c20 7468 6520 6d65  question, the me
+00004ce0: 7373 6167 6573 206c 6973 742c 2061 6e64  ssages list, and
+00004cf0: 2074 6865 2064 6174 6166 7261 6d65 0d0a   the dataframe..
+00004d00: 2020 2020 2020 2020 2020 2020 616e 7377              answ
+00004d10: 6572 2c20 636f 6465 2c20 746f 7461 6c5f  er, code, total_
+00004d20: 746f 6b65 6e73 5f75 7365 645f 7375 6d20  tokens_used_sum 
+00004d30: 3d20 7365 6c66 2e70 645f 6167 656e 7428  = self.pd_agent(
+00004d40: 7461 736b 2c20 6d65 7373 6167 6573 2c20  task, messages, 
+00004d50: 7365 6c66 2e64 6629 0d0a 0d0a 2020 2020  self.df)....    
+00004d60: 2020 2020 2020 2020 2320 5261 6e6b 2074          # Rank t
+00004d70: 6865 204c 4c4d 2072 6573 706f 6e73 650d  he LLM response.
+00004d80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004d90: 7365 6c66 2e72 616e 6b3a 0d0a 2020 2020  self.rank:..    
+00004da0: 2020 2020 2020 2020 2020 2020 2320 5377              # Sw
+00004db0: 6974 6368 2074 6f20 6770 742d 3420 6966  itch to gpt-4 if
+00004dc0: 206c 6c6d 5f73 7769 7463 6820 7061 7261   llm_switch para
+00004dd0: 6d65 7465 7220 6973 2073 6574 2074 6f20  meter is set to 
+00004de0: 5472 7565 2e20 5468 6973 2077 696c 6c20  True. This will 
+00004df0: 696e 6372 6561 7365 2074 6865 2070 726f  increase the pro
+00004e00: 6365 7373 696e 6720 7469 6d65 2061 6e64  cessing time and
+00004e10: 2063 6f73 740d 0a20 2020 2020 2020 2020   cost..         
+00004e20: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+00004e30: 6c6d 5f73 7769 7463 683a 0d0a 2020 2020  lm_switch:..    
+00004e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e50: 6c6c 6d5f 6361 7363 6164 6520 3d20 5472  llm_cascade = Tr
+00004e60: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00004e70: 2020 2020 7261 6e6b 203d 2073 656c 662e      rank = self.
+00004e80: 7261 6e6b 5f63 6f64 6528 636f 6465 2c74  rank_code(code,t
+00004e90: 6173 6b2c 6c6c 6d5f 6361 7363 6164 653d  ask,llm_cascade=
+00004ea0: 6c6c 6d5f 6361 7363 6164 6529 0d0a 2020  llm_cascade)..  
+00004eb0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00004ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ed0: 2072 616e 6b20 3d20 2222 0d0a 0d0a 2020   rank = ""....  
+00004ee0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00004ef0: 795f 7265 7375 6c74 7328 616e 7377 6572  y_results(answer
+00004f00: 2c20 636f 6465 2c20 7261 6e6b 2c20 746f  , code, rank, to
+00004f10: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
+00004f20: 7375 6d29 0d0a 0d0a 0d0a 2020 2020 6465  sum)......    de
+00004f30: 6620 7064 5f61 6765 6e74 2873 656c 662c  f pd_agent(self,
+00004f40: 2071 7565 7374 696f 6e2c 206d 6573 7361   question, messa
+00004f50: 6765 732c 2064 663d 4e6f 6e65 293a 0d0a  ges, df=None):..
+00004f60: 2020 2020 2020 2020 2320 4164 6420 6120          # Add a 
+00004f70: 7573 6572 206d 6573 7361 6765 2077 6974  user message wit
+00004f80: 6820 7468 6520 7570 6461 7465 6420 7461  h the updated ta
+00004f90: 736b 2070 726f 6d70 7420 746f 2074 6865  sk prompt to the
+00004fa0: 206d 6573 7361 6765 7320 6c69 7374 0d0a   messages list..
+00004fb0: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
+00004fc0: 2e61 7070 656e 6428 7b22 726f 6c65 223a  .append({"role":
+00004fd0: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
+00004fe0: 7422 3a20 7365 6c66 2e74 6173 6b2e 666f  t": self.task.fo
+00004ff0: 726d 6174 2873 656c 662e 6466 5f68 6561  rmat(self.df_hea
+00005000: 642c 2071 7565 7374 696f 6e29 7d29 0d0a  d, question)})..
+00005010: 0d0a 2020 2020 2020 2020 6966 2027 6970  ..        if 'ip
+00005020: 796b 6572 6e65 6c27 2069 6e20 7379 732e  ykernel' in sys.
+00005030: 6d6f 6475 6c65 733a 0d0a 2020 2020 2020  modules:..      
+00005040: 2020 2020 2020 2320 4a75 7079 7465 7220        # Jupyter 
+00005050: 6e6f 7465 626f 6f6b 206f 7220 6970 7974  notebook or ipyt
+00005060: 686f 6e0d 0a20 2020 2020 2020 2020 2020  hon..           
+00005070: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
+00005080: 3c70 2073 7479 6c65 3d22 636f 6c6f 723a  <p style="color:
+00005090: 6d61 6765 6e74 613b 223e 5c6e 4361 6c6c  magenta;">\nCall
+000050a0: 696e 6720 4d6f 6465 6c3a 207b 7365 6c66  ing Model: {self
+000050b0: 2e6c 6c6d 7d3c 2f70 3e27 2929 0d0a 2020  .llm}</p>'))..  
+000050c0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+000050d0: 7928 4854 4d4c 2866 273c 703e 3c62 2073  y(HTML(f'<p><b s
+000050e0: 7479 6c65 3d22 636f 6c6f 723a 6d61 6765  tyle="color:mage
+000050f0: 6e74 613b 223e 4920 6861 7665 2073 656e  nta;">I have sen
+00005100: 7420 796f 7572 2072 6571 7565 7374 2074  t your request t
+00005110: 6f20 7468 6520 4c4c 4d20 616e 6420 6177  o the LLM and aw
+00005120: 6169 7469 6e67 2072 6573 706f 6e73 652c  aiting response,
+00005130: 2070 6c65 6173 6520 7761 6974 2e2e 2e3c   please wait...<
+00005140: 2f62 3e3c 2f70 3e3c 6272 3e27 2929 0d0a  /b></p><br>'))..
+00005150: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00005160: 2020 2020 2020 2020 2020 2023 204f 7468             # Oth
+00005170: 6572 2065 6e76 6972 6f6e 6d65 6e74 2028  er environment (
+00005180: 6c69 6b65 2074 6572 6d69 6e61 6c29 0d0a  like terminal)..
+00005190: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000051a0: 7428 636f 6c6f 7265 6428 6622 5c6e 3e3e  t(colored(f"\n>>
+000051b0: 2043 616c 6c69 6e67 204d 6f64 656c 3a20   Calling Model: 
+000051c0: 7b73 656c 662e 6c6c 6d7d 222c 2022 6d61  {self.llm}", "ma
+000051d0: 6765 6e74 6122 2929 0d0a 2020 2020 2020  genta"))..      
+000051e0: 2020 2020 2020 6370 7269 6e74 2866 225c        cprint(f"\
+000051f0: 6e3e 3e20 4920 6861 7665 2073 656e 7420  n>> I have sent 
+00005200: 796f 7572 2072 6571 7565 7374 2074 6f20  your request to 
+00005210: 7468 6520 4c4c 4d20 616e 6420 6177 6169  the LLM and awai
+00005220: 7469 6e67 2072 6573 706f 6e73 652c 2070  ting response, p
+00005230: 6c65 6173 6520 7761 6974 2e2e 2e5c 6e22  lease wait...\n"
+00005240: 2c20 276d 6167 656e 7461 272c 2061 7474  , 'magenta', att
+00005250: 7273 3d5b 2762 6f6c 6427 5d29 0d0a 0d0a  rs=['bold'])....
+00005260: 2020 2020 2020 2020 2320 4361 6c6c 2074          # Call t
+00005270: 6865 204f 7065 6e41 4920 4150 490d 0a20  he OpenAI API.. 
+00005280: 2020 2020 2020 206c 6c6d 5f72 6573 706f         llm_respo
+00005290: 6e73 652c 2074 6f6b 656e 735f 7573 6564  nse, tokens_used
+000052a0: 203d 2073 656c 662e 6c6c 6d5f 6361 6c6c   = self.llm_call
+000052b0: 286d 6573 7361 6765 7329 0d0a 0d0a 2020  (messages)....  
+000052c0: 2020 2020 2020 2320 4578 7472 6163 7420        # Extract 
+000052d0: 7468 6520 636f 6465 2066 726f 6d20 7468  the code from th
+000052e0: 6520 4150 4920 7265 7370 6f6e 7365 0d0a  e API response..
+000052f0: 2020 2020 2020 2020 636f 6465 203d 2073          code = s
+00005300: 656c 662e 5f65 7874 7261 6374 5f63 6f64  elf._extract_cod
+00005310: 6528 6c6c 6d5f 7265 7370 6f6e 7365 290d  e(llm_response).
+00005320: 0a0d 0a20 2020 2020 2020 2023 2055 7064  ...        # Upd
+00005330: 6174 6520 7468 6520 746f 7461 6c20 746f  ate the total to
+00005340: 6b65 6e73 2075 7365 640d 0a20 2020 2020  kens used..     
+00005350: 2020 2073 656c 662e 746f 7461 6c5f 746f     self.total_to
+00005360: 6b65 6e73 5f75 7365 642e 6170 7065 6e64  kens_used.append
+00005370: 2874 6f6b 656e 735f 7573 6564 290d 0a0d  (tokens_used)...
+00005380: 0a20 2020 2020 2020 2023 2049 6e69 7469  .        # Initi
+00005390: 616c 697a 6520 6572 726f 7220 636f 7272  alize error corr
+000053a0: 6563 7469 6f6e 2063 6f75 6e74 6572 0d0a  ection counter..
+000053b0: 2020 2020 2020 2020 6572 726f 725f 636f          error_co
+000053c0: 7272 6563 7469 6f6e 7320 3d20 300d 0a0d  rrections = 0...
+000053d0: 0a20 2020 2020 2020 2023 2044 6562 7567  .        # Debug
+000053e0: 2063 6f64 6520 6966 2064 6562 7567 2070   code if debug p
+000053f0: 6172 616d 6574 6572 2069 7320 7365 7420  arameter is set 
+00005400: 746f 2054 7275 650d 0a20 2020 2020 2020  to True..       
+00005410: 2069 6620 7365 6c66 2e64 6562 7567 3a0d   if self.debug:.
+00005420: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
+00005430: 7769 7463 6820 746f 2067 7074 2d34 2069  witch to gpt-4 i
+00005440: 6620 6c6c 6d5f 7377 6974 6368 2070 6172  f llm_switch par
+00005450: 616d 6574 6572 2069 7320 7365 7420 746f  ameter is set to
+00005460: 2054 7275 652e 2054 6869 7320 7769 6c6c   True. This will
+00005470: 2069 6e63 7265 6173 6520 7468 6520 7072   increase the pr
+00005480: 6f63 6573 7369 6e67 2074 696d 6520 616e  ocessing time an
+00005490: 6420 636f 7374 0d0a 2020 2020 2020 2020  d cost..        
+000054a0: 2020 2020 6966 2073 656c 662e 6c6c 6d5f      if self.llm_
+000054b0: 7377 6974 6368 3a0d 0a20 2020 2020 2020  switch:..       
+000054c0: 2020 2020 2020 2020 206c 6c6d 5f63 6173           llm_cas
+000054d0: 6361 6465 203d 2054 7275 650d 0a20 2020  cade = True..   
+000054e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000054f0: 2769 7079 6b65 726e 656c 2720 696e 2073  'ipykernel' in s
+00005500: 7973 2e6d 6f64 756c 6573 3a0d 0a20 2020  ys.modules:..   
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2023 204a 7570 7974 6572 206e 6f74 6562   # Jupyter noteb
+00005530: 6f6f 6b0d 0a20 2020 2020 2020 2020 2020  ook..           
+00005540: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00005550: 2848 544d 4c28 273c 7370 616e 2073 7479  (HTML('<span sty
+00005560: 6c65 3d22 636f 6c6f 723a 206d 6167 656e  le="color: magen
+00005570: 7461 3b22 3e53 7769 7463 6869 6e67 206d  ta;">Switching m
+00005580: 6f64 656c 2074 6f20 6770 742d 3420 746f  odel to gpt-4 to
+00005590: 2064 6562 7567 2074 6865 2063 6f64 652e   debug the code.
+000055a0: 3c2f 7370 616e 3e27 2929 0d0a 2020 2020  </span>'))..    
+000055b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000055c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000055d0: 2020 2020 2020 2023 2043 4c49 0d0a 2020         # CLI..  
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 7072 696e 7428 636f 6c6f 7265 6428    print(colored(
+00005600: 225c 6e3e 3e20 5377 6974 6368 696e 6720  "\n>> Switching 
+00005610: 6d6f 6465 6c20 746f 2047 5054 2d34 2074  model to GPT-4 t
+00005620: 6f20 6465 6275 6720 7468 6520 636f 6465  o debug the code
+00005630: 2e22 2c20 226d 6167 656e 7461 2229 290d  .", "magenta")).
+00005640: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
+00005650: 6520 3d20 7365 6c66 2e64 6562 7567 5f63  e = self.debug_c
+00005660: 6f64 6528 636f 6465 2c20 7175 6573 7469  ode(code, questi
+00005670: 6f6e 2c20 6c6c 6d5f 6361 7363 6164 653d  on, llm_cascade=
+00005680: 6c6c 6d5f 6361 7363 6164 6529 0d0a 0d0a  llm_cascade)....
+00005690: 2020 2020 2020 2020 2320 5265 6469 7265          # Redire
+000056a0: 6374 2073 7461 6e64 6172 6420 6f75 7470  ct standard outp
+000056b0: 7574 2074 6f20 6120 5374 7269 6e67 494f  ut to a StringIO
+000056c0: 2062 7566 6665 720d 0a20 2020 2020 2020   buffer..       
+000056d0: 2077 6974 6820 7265 6469 7265 6374 5f73   with redirect_s
+000056e0: 7464 6f75 7428 696f 2e53 7472 696e 6749  tdout(io.StringI
+000056f0: 4f28 2929 2061 7320 6f75 7470 7574 3a0d  O()) as output:.
+00005700: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00005710: 7279 2074 6f20 6578 6563 7574 6520 7468  ry to execute th
+00005720: 6520 636f 6465 2061 6e64 2068 616e 646c  e code and handl
+00005730: 6520 6572 726f 7273 0d0a 2020 2020 2020  e errors..      
+00005740: 2020 2020 2020 7768 696c 6520 6572 726f        while erro
+00005750: 725f 636f 7272 6563 7469 6f6e 7320 3c20  r_corrections < 
+00005760: 7365 6c66 2e4d 4158 5f45 5252 4f52 5f43  self.MAX_ERROR_C
+00005770: 4f52 5245 4354 494f 4e53 3a0d 0a20 2020  ORRECTIONS:..   
+00005780: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00005790: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000057a0: 2020 2020 2020 206d 6573 7361 6765 732e         messages.
+000057b0: 6170 7065 6e64 287b 2272 6f6c 6522 3a20  append({"role": 
+000057c0: 2261 7373 6973 7461 6e74 222c 2022 636f  "assistant", "co
+000057d0: 6e74 656e 7422 3a20 6c6c 6d5f 7265 7370  ntent": llm_resp
+000057e0: 6f6e 7365 7d29 0d0a 2020 2020 2020 2020  onse})..        
+000057f0: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
+00005800: 6d6f 7665 2074 6865 206f 6c64 6573 7420  move the oldest 
+00005810: 636f 6e76 6572 7361 7469 6f6e 2066 726f  conversation fro
+00005820: 6d20 7468 6520 6d65 7373 6167 6573 206c  m the messages l
+00005830: 6973 740d 0a20 2020 2020 2020 2020 2020  ist..           
+00005840: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00005850: 6d65 7373 6167 6573 2920 3e20 7365 6c66  messages) > self
+00005860: 2e4d 4158 5f43 4f4e 5645 5253 4154 494f  .MAX_CONVERSATIO
+00005870: 4e53 3a0d 0a20 2020 2020 2020 2020 2020  NS:..           
+00005880: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+00005890: 7361 6765 732e 706f 7028 3129 0d0a 2020  sages.pop(1)..  
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058b0: 2020 2020 2020 6d65 7373 6167 6573 2e70        messages.p
+000058c0: 6f70 2831 290d 0a20 2020 2020 2020 2020  op(1)..         
+000058d0: 2020 2020 2020 2020 2020 2023 2052 6573             # Res
+000058e0: 6574 2064 6620 746f 2074 6865 206f 7269  et df to the ori
+000058f0: 6769 6e61 6c20 7374 6174 6520 6265 666f  ginal state befo
+00005900: 7265 2065 7865 6375 7469 6e67 2074 6865  re executing the
+00005910: 2063 6f64 650d 0a20 2020 2020 2020 2020   code..         
+00005920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005930: 6466 203d 2073 656c 662e 6f72 6967 696e  df = self.origin
+00005940: 616c 5f64 662e 636f 7079 2829 0d0a 2020  al_df.copy()..  
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 2320 4578 6563 7574 6520 7468 6520    # Execute the 
+00005970: 636f 6465 0d0a 2020 2020 2020 2020 2020  code..          
+00005980: 2020 2020 2020 2020 2020 6966 2063 6f64            if cod
+00005990: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059b0: 2020 2020 2020 2020 6578 6563 2863 6f64          exec(cod
+000059c0: 652c 207b 2764 6627 3a20 7365 6c66 2e64  e, {'df': self.d
+000059d0: 667d 290d 0a20 2020 2020 2020 2020 2020  f})..           
+000059e0: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
+000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a00: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00005a10: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00005a20: 2020 2020 2020 2020 2020 2020 2320 5072              # Pr
+00005a30: 696e 7420 7468 6520 6572 726f 7220 6d65  int the error me
+00005a40: 7373 6167 650d 0a20 2020 2020 2020 2020  ssage..         
+00005a50: 2020 2020 2020 2020 2020 2069 6620 2769             if 'i
+00005a60: 7079 6b65 726e 656c 2720 696e 2073 7973  pykernel' in sys
+00005a70: 2e6d 6f64 756c 6573 3a0d 0a20 2020 2020  .modules:..     
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2023 204a 7570 7974 6572 206e 6f74     # Jupyter not
+00005aa0: 6562 6f6f 6b0d 0a20 2020 2020 2020 2020  ebook..         
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00005ac0: 6973 706c 6179 2848 544d 4c28 6627 3c62  isplay(HTML(f'<b
+00005ad0: 723e 3c62 3e3c 7370 616e 2073 7479 6c65  r><b><span style
+00005ae0: 3d22 636f 6c6f 723a 2023 6438 3663 3030  ="color: #d86c00
+00005af0: 3b22 3e49 2072 616e 2069 6e74 6f20 616e  ;">I ran into an
+00005b00: 2069 7373 7565 3a3c 2f73 7061 6e3e 3c2f   issue:</span></
+00005b10: 623e 3c62 723e 3c70 7265 2073 7479 6c65  b><br><pre style
+00005b20: 3d22 636f 6c6f 723a 2023 6438 3663 3030  ="color: #d86c00
+00005b30: 3b22 3e7b 657d 3c2f 7072 653e 3c62 723e  ;">{e}</pre><br>
+00005b40: 3c62 3e3c 7370 616e 2073 7479 6c65 3d22  <b><span style="
+00005b50: 636f 6c6f 723a 2023 6438 3663 3030 3b22  color: #d86c00;"
+00005b60: 3e49 2077 696c 6c20 6578 616d 696e 6520  >I will examine 
+00005b70: 6974 2c20 616e 6420 7472 7920 6167 6169  it, and try agai
+00005b80: 6e20 7769 7468 2061 6e20 6164 6a75 7374  n with an adjust
+00005b90: 6564 2063 6f64 652e 3c2f 7370 616e 3e3c  ed code.</span><
+00005ba0: 2f62 3e3c 6272 3e27 2929 0d0a 2020 2020  /b><br>'))..    
+00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bc0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00005bd0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00005be0: 2043 4c49 0d0a 2020 2020 2020 2020 2020   CLI..          
+00005bf0: 2020 2020 2020 2020 2020 2020 2020 2370                #p
+00005c00: 7269 6e74 2863 6f6c 6f72 6564 2866 2749  rint(colored(f'I
+00005c10: 2072 616e 2069 6e74 6f20 616e 2069 7373   ran into an iss
+00005c20: 7565 3a20 7b65 7d2e 203e 2049 2077 696c  ue: {e}. > I wil
+00005c30: 6c20 6578 616d 696e 6520 6974 2c20 616e  l examine it, an
+00005c40: 6420 7472 7920 6167 6169 6e20 7769 7468  d try again with
+00005c50: 2061 6e20 6164 6a75 7374 6564 2063 6f64   an adjusted cod
+00005c60: 652e 272c 2027 7265 6427 2929 0d0a 2020  e.', 'red'))..  
+00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c80: 2020 2020 2020 7379 732e 7374 6465 7272        sys.stderr
+00005c90: 2e77 7269 7465 2827 5c30 3333 5b33 316d  .write('\033[31m
+00005ca0: 2720 2b20 6627 3e3e 2049 2072 616e 2069  ' + f'>> I ran i
+00005cb0: 6e74 6f20 616e 2069 7373 7565 3a20 7b65  nto an issue: {e
+00005cc0: 7d2e 205c 6e3e 2049 2077 696c 6c20 6578  }. \n> I will ex
+00005cd0: 616d 696e 6520 6974 2c20 616e 6420 7472  amine it, and tr
+00005ce0: 7920 6167 6169 6e20 7769 7468 2061 6e20  y again with an 
+00005cf0: 6164 6a75 7374 6564 2063 6f64 652e 2720  adjusted code.' 
+00005d00: 2b20 275c 3033 335b 306d 2720 2b20 275c  + '\033[0m' + '\
+00005d10: 6e27 290d 0a20 2020 2020 2020 2020 2020  n')..           
+00005d20: 2020 2020 2020 2020 2020 2020 2073 7973               sys
+00005d30: 2e73 7464 6572 722e 666c 7573 6828 290d  .stderr.flush().
+00005d40: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00005d50: 2020 2020 2020 2023 2049 6e63 7265 6d65         # Increme
+00005d60: 6e74 2074 6865 2065 7272 6f72 2063 6f72  nt the error cor
+00005d70: 7265 6374 696f 6e20 636f 756e 7465 7220  rection counter 
+00005d80: 616e 6420 7570 6461 7465 2074 6865 206d  and update the m
+00005d90: 6573 7361 6765 7320 6c69 7374 2077 6974  essages list wit
+00005da0: 6820 7468 6520 6572 726f 720d 0a20 2020  h the error..   
 00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
-00005dd0: 746f 6b65 6e73 5f75 7365 642e 6170 7065  tokens_used.appe
-00005de0: 6e64 2874 6f6b 656e 735f 7573 6564 290d  nd(tokens_used).
-00005df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005e00: 2020 2020 2020 2020 2074 6f74 616c 5f74           total_t
-00005e10: 6f6b 656e 735f 7573 6564 5f73 756d 203d  okens_used_sum =
-00005e20: 2073 756d 2873 656c 662e 746f 7461 6c5f   sum(self.total_
-00005e30: 746f 6b65 6e73 5f75 7365 6429 0d0a 2020  tokens_used)..  
+00005dc0: 2065 7272 6f72 5f63 6f72 7265 6374 696f   error_correctio
+00005dd0: 6e73 202b 3d20 310d 0a20 2020 2020 2020  ns += 1..       
+00005de0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+00005df0: 7361 6765 732e 6170 7065 6e64 287b 2272  sages.append({"r
+00005e00: 6f6c 6522 3a20 2275 7365 7222 2c20 2263  ole": "user", "c
+00005e10: 6f6e 7465 6e74 223a 2073 656c 662e 6572  ontent": self.er
+00005e20: 726f 725f 636f 7272 6563 745f 7461 736b  ror_correct_task
+00005e30: 2e66 6f72 6d61 7428 6529 7d29 0d0a 0d0a  .format(e)})....
 00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e50: 2020 6578 6365 7074 206f 7065 6e61 692e    except openai.
-00005e60: 6572 726f 722e 5261 7465 4c69 6d69 7445  error.RateLimitE
-00005e70: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00005e90: 7269 6e74 280d 0a20 2020 2020 2020 2020  rint(..         
-00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005eb0: 2020 2022 5468 6520 4f70 656e 4149 2041     "The OpenAI A
-00005ec0: 5049 2072 6174 6520 6c69 6d69 7420 6861  PI rate limit ha
-00005ed0: 7320 6265 656e 2065 7863 6565 6465 642e  s been exceeded.
-00005ee0: 2057 6169 7469 6e67 2031 3020 7365 636f   Waiting 10 seco
-00005ef0: 6e64 7320 616e 6420 7472 7969 6e67 2061  nds and trying a
-00005f00: 6761 696e 2e22 0d0a 2020 2020 2020 2020  gain."..        
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005f30: 2020 2020 2020 2020 2020 2074 696d 652e             time.
-00005f40: 736c 6565 7028 3130 290d 0a20 2020 2020  sleep(10)..     
+00005e50: 2020 2020 2320 5377 6974 6368 2074 6f20      # Switch to 
+00005e60: 6770 742d 3420 6966 206c 6c6d 5f73 7769  gpt-4 if llm_swi
+00005e70: 7463 6820 7061 7261 6d65 7465 7220 6973  tch parameter is
+00005e80: 2073 6574 2074 6f20 5472 7565 2e20 5468   set to True. Th
+00005e90: 6973 2077 696c 6c20 696e 6372 6561 7365  is will increase
+00005ea0: 2074 6865 2070 726f 6365 7373 696e 6720   the processing 
+00005eb0: 7469 6d65 2061 6e64 2063 6f73 742e 0d0a  time and cost...
+00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ed0: 2020 2020 6966 2073 656c 662e 6c6c 6d5f      if self.llm_
+00005ee0: 7377 6974 6368 3a0d 0a20 2020 2020 2020  switch:..       
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f00: 206c 6c6d 5f63 6173 6361 6465 203d 2054   llm_cascade = T
+00005f10: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
+00005f20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00005f30: 2769 7079 6b65 726e 656c 2720 696e 2073  'ipykernel' in s
+00005f40: 7973 2e6d 6f64 756c 6573 3a0d 0a20 2020  ys.modules:..   
 00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 206c 6c6d 5f72 6573 706f 6e73 652c     llm_response,
-00005f70: 2074 6f6b 656e 735f 7573 6564 203d 2073   tokens_used = s
-00005f80: 656c 662e 6c6c 6d5f 6361 6c6c 286d 6573  elf.llm_call(mes
-00005f90: 7361 6765 7329 0d0a 2020 2020 2020 2020  sages)..        
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fb0: 636f 6465 2c72 6566 6c65 6374 696f 6e2c  code,reflection,
-00005fc0: 666c 6f77 203d 2073 656c 662e 5f65 7874  flow = self._ext
-00005fd0: 7261 6374 5f63 6f64 6528 6c6c 6d5f 7265  ract_code(llm_re
-00005fe0: 7370 6f6e 7365 290d 0a20 2020 2020 2020  sponse)..       
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2073 656c 662e 746f 7461 6c5f 746f 6b65   self.total_toke
-00006010: 6e73 5f75 7365 642e 6170 7065 6e64 2874  ns_used.append(t
-00006020: 6f6b 656e 735f 7573 6564 290d 0a20 2020  okens_used)..   
+00005f60: 2020 2020 2020 2020 2023 204a 7570 7974           # Jupyt
+00005f70: 6572 206e 6f74 6562 6f6f 6b0d 0a20 2020  er notebook..   
+00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f90: 2020 2020 2020 2020 2064 6973 706c 6179           display
+00005fa0: 2848 544d 4c28 273c 7370 616e 2073 7479  (HTML('<span sty
+00005fb0: 6c65 3d22 636f 6c6f 723a 2023 6438 3663  le="color: #d86c
+00005fc0: 3030 3b22 3e53 7769 7463 6869 6e67 206d  00;">Switching m
+00005fd0: 6f64 656c 2074 6f20 6770 742d 3420 746f  odel to gpt-4 to
+00005fe0: 2074 7279 2074 6f20 696d 7072 6f76 6520   try to improve 
+00005ff0: 7468 6520 6f75 7463 6f6d 652e 3c2f 7370  the outcome.</sp
+00006000: 616e 3e27 2929 0d0a 2020 2020 2020 2020  an>'))..        
+00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006020: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
 00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 2020 2074 6f74 616c 5f74 6f6b 656e       total_token
-00006050: 735f 7573 6564 5f73 756d 203d 2073 756d  s_used_sum = sum
-00006060: 2873 656c 662e 746f 7461 6c5f 746f 6b65  (self.total_toke
-00006070: 6e73 5f75 7365 6429 0d0a 0d0a 2020 2020  ns_used)....    
-00006080: 2020 2020 2020 2020 2320 5377 6974 6368          # Switch
-00006090: 2062 6163 6b20 746f 2074 6865 206f 7269   back to the ori
-000060a0: 6769 6e61 6c20 6c6c 6d20 6265 666f 7265  ginal llm before
-000060b0: 2074 6865 2066 756e 6374 696f 6e20 6669   the function fi
-000060c0: 6e69 7368 6573 0d0a 2020 2020 2020 2020  nishes..        
-000060d0: 2020 2020 7365 6c66 2e6c 6c6d 203d 206f      self.llm = o
-000060e0: 7269 6769 6e61 6c5f 6c6c 6d0d 0a0d 0a20  riginal_llm.... 
-000060f0: 2020 2020 2020 2023 2047 6574 2074 6865         # Get the
-00006100: 206f 7574 7075 7420 6672 6f6d 2074 6865   output from the
-00006110: 2065 7865 6375 7465 6420 636f 6465 0d0a   executed code..
-00006120: 2020 2020 2020 2020 616e 7377 6572 203d          answer =
-00006130: 206f 7574 7075 742e 6765 7476 616c 7565   output.getvalue
-00006140: 2829 0d0a 0d0a 2020 2020 2020 2020 2320  ()....        # 
-00006150: 5265 7365 7420 7468 6520 5374 7269 6e67  Reset the String
-00006160: 494f 2062 7566 6665 720d 0a20 2020 2020  IO buffer..     
-00006170: 2020 206f 7574 7075 742e 7472 756e 6361     output.trunca
-00006180: 7465 2830 290d 0a20 2020 2020 2020 206f  te(0)..        o
-00006190: 7574 7075 742e 7365 656b 2830 290d 0a0d  utput.seek(0)...
-000061a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000061b0: 616e 7377 6572 2c20 636f 6465 2c20 7265  answer, code, re
-000061c0: 666c 6563 7469 6f6e 2c20 666c 6f77 2c20  flection, flow, 
-000061d0: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
-000061e0: 645f 7375 6d0d 0a20 2020 20              d_sum..    
+00006040: 2020 2023 2043 4c49 0d0a 2020 2020 2020     # CLI..      
+00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006060: 2020 2020 2020 7379 732e 7374 6465 7272        sys.stderr
+00006070: 2e77 7269 7465 2827 5c30 3333 5b33 316d  .write('\033[31m
+00006080: 2720 2b20 6627 3e3e 2053 7769 7463 6869  ' + f'>> Switchi
+00006090: 6e67 206d 6f64 656c 2074 6f20 6770 742d  ng model to gpt-
+000060a0: 3420 746f 2074 7279 2074 6f20 696d 7072  4 to try to impr
+000060b0: 6f76 6520 7468 6520 6f75 7463 6f6d 652e  ove the outcome.
+000060c0: 2720 2b20 275c 3033 335b 306d 2720 2b20  ' + '\033[0m' + 
+000060d0: 275c 6e27 290d 0a20 2020 2020 2020 2020  '\n')..         
+000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060f0: 2020 2073 7973 2e73 7464 6572 722e 666c     sys.stderr.fl
+00006100: 7573 6828 290d 0a0d 0a20 2020 2020 2020  ush()....       
+00006110: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+00006120: 616c 6c20 4f70 656e 4149 2041 5049 2074  all OpenAI API t
+00006130: 6f20 6765 7420 616e 2075 7064 6174 6564  o get an updated
+00006140: 2063 6f64 650d 0a20 2020 2020 2020 2020   code..         
+00006150: 2020 2020 2020 2020 2020 206c 6c6d 5f72             llm_r
+00006160: 6573 706f 6e73 652c 2074 6f6b 656e 735f  esponse, tokens_
+00006170: 7573 6564 203d 2073 656c 662e 6c6c 6d5f  used = self.llm_
+00006180: 6361 6c6c 286d 6573 7361 6765 732c 6c6c  call(messages,ll
+00006190: 6d5f 6361 7363 6164 653d 6c6c 6d5f 6361  m_cascade=llm_ca
+000061a0: 7363 6164 6529 0d0a 2020 2020 2020 2020  scade)..        
+000061b0: 2020 2020 2020 2020 2020 2020 636f 6465              code
+000061c0: 203d 2073 656c 662e 5f65 7874 7261 6374   = self._extract
+000061d0: 5f63 6f64 6528 6c6c 6d5f 7265 7370 6f6e  _code(llm_respon
+000061e0: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
+000061f0: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
+00006200: 7461 6c5f 746f 6b65 6e73 5f75 7365 642e  tal_tokens_used.
+00006210: 6170 7065 6e64 2874 6f6b 656e 735f 7573  append(tokens_us
+00006220: 6564 290d 0a20 2020 2020 2020 2020 2020  ed)..           
+00006230: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00006240: 2020 2020 2023 2047 6574 2074 6865 206f       # Get the o
+00006250: 7574 7075 7420 6672 6f6d 2074 6865 2065  utput from the e
+00006260: 7865 6375 7465 6420 636f 6465 0d0a 2020  xecuted code..  
+00006270: 2020 2020 2020 616e 7377 6572 203d 206f        answer = o
+00006280: 7574 7075 742e 6765 7476 616c 7565 2829  utput.getvalue()
+00006290: 0d0a 0d0a 2020 2020 2020 2020 2320 4361  ....        # Ca
+000062a0: 6c6c 204f 7065 6e41 4920 4150 490d 0a20  ll OpenAI API.. 
+000062b0: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
+000062c0: 697a 6520 7468 6520 6d65 7373 6167 6573  ize the messages
+000062d0: 206c 6973 7420 7769 7468 2061 2073 7973   list with a sys
+000062e0: 7465 6d20 6d65 7373 6167 6520 636f 6e74  tem message cont
+000062f0: 6169 6e69 6e67 2074 6865 2074 6173 6b20  aining the task 
+00006300: 7072 6f6d 7074 0d0a 2020 2020 2020 2020  prompt..        
+00006310: 696e 7369 6768 7473 5f6d 6573 7361 6765  insights_message
+00006320: 7320 3d20 5b7b 2272 6f6c 6522 3a20 2275  s = [{"role": "u
+00006330: 7365 7222 2c20 2263 6f6e 7465 6e74 223a  ser", "content":
+00006340: 2073 656c 662e 736f 6c75 7469 6f6e 5f69   self.solution_i
+00006350: 6e73 6967 6874 732e 666f 726d 6174 2871  nsights.format(q
+00006360: 7565 7374 696f 6e2c 2061 6e73 7765 7229  uestion, answer)
+00006370: 7d5d 0d0a 2020 2020 2020 2020 6675 6e63  }]..        func
+00006380: 7469 6f6e 5f6e 616d 6520 3d20 7b22 6e61  tion_name = {"na
+00006390: 6d65 223a 2022 536f 6c75 7469 6f6e 5f49  me": "Solution_I
+000063a0: 6e73 6967 6874 7322 7d0d 0a20 2020 2020  nsights"}..     
+000063b0: 2020 2066 6e5f 6e61 6d65 2c20 6172 6775     fn_name, argu
+000063c0: 6d65 6e74 732c 2074 6f6b 656e 735f 7573  ments, tokens_us
+000063d0: 6564 203d 2073 656c 662e 6c6c 6d5f 6675  ed = self.llm_fu
+000063e0: 6e63 5f63 616c 6c28 696e 7369 6768 7473  nc_call(insights
+000063f0: 5f6d 6573 7361 6765 732c 2073 656c 662e  _messages, self.
+00006400: 696e 7369 6768 7473 5f66 756e 6374 696f  insights_functio
+00006410: 6e2c 2066 756e 6374 696f 6e5f 6e61 6d65  n, function_name
+00006420: 290d 0a0d 0a20 2020 2020 2020 2023 2050  )....        # P
+00006430: 6172 7365 2074 6865 204a 534f 4e20 7374  arse the JSON st
+00006440: 7269 6e67 2074 6f20 6120 5079 7468 6f6e  ring to a Python
+00006450: 2064 6963 740d 0a20 2020 2020 2020 2061   dict..        a
+00006460: 7267 756d 656e 7473 5f64 6963 7420 3d20  rguments_dict = 
+00006470: 6a73 6f6e 2e6c 6f61 6473 2861 7267 756d  json.loads(argum
+00006480: 656e 7473 2c73 7472 6963 743d 4661 6c73  ents,strict=Fals
+00006490: 6529 0d0a 0d0a 2020 2020 2020 2020 2320  e)....        # 
+000064a0: 5265 7472 6965 7665 2076 616c 7565 730d  Retrieve values.
+000064b0: 0a20 2020 2020 2020 2061 6e73 7765 7220  .        answer 
+000064c0: 3d20 6172 6775 6d65 6e74 735f 6469 6374  = arguments_dict
+000064d0: 5b22 696e 7369 6768 7422 5d0d 0a0d 0a20  ["insight"].... 
+000064e0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
+000064f0: 6c5f 746f 6b65 6e73 5f75 7365 642e 6170  l_tokens_used.ap
+00006500: 7065 6e64 2874 6f6b 656e 735f 7573 6564  pend(tokens_used
+00006510: 290d 0a20 2020 2020 2020 2074 6f74 616c  )..        total
+00006520: 5f74 6f6b 656e 735f 7573 6564 5f73 756d  _tokens_used_sum
+00006530: 203d 2073 756d 2873 656c 662e 746f 7461   = sum(self.tota
+00006540: 6c5f 746f 6b65 6e73 5f75 7365 6429 0d0a  l_tokens_used)..
+00006550: 0d0a 2020 2020 2020 2020 2320 5265 7365  ..        # Rese
+00006560: 7420 7468 6520 5374 7269 6e67 494f 2062  t the StringIO b
+00006570: 7566 6665 720d 0a20 2020 2020 2020 206f  uffer..        o
+00006580: 7574 7075 742e 7472 756e 6361 7465 2830  utput.truncate(0
+00006590: 290d 0a20 2020 2020 2020 206f 7574 7075  )..        outpu
+000065a0: 742e 7365 656b 2830 290d 0a0d 0a20 2020  t.seek(0)....   
+000065b0: 2020 2020 2072 6574 7572 6e20 616e 7377       return answ
+000065c0: 6572 2c20 636f 6465 2c20 746f 7461 6c5f  er, code, total_
+000065d0: 746f 6b65 6e73 5f75 7365 645f 7375 6d0d  tokens_used_sum.
+000065e0: 0a20 2020 20                             .
```

### Comparing `bambooai-0.3.3/bambooai.egg-info/PKG-INFO` & `bambooai-0.3.4/bambooai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.3.3
+Version: 0.3.4
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 Author: Palo Galko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,18 @@
 - The response from the API, containing the corresponding Python code, is received, checked and sanitised if necessary.
   - If the debug parameter is set to "True", the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking, debugging and sanitization of any harmful elements..
 - The received code is then executed to generate an answer or a visualization:
   - If the code executes successfully, it displays the answer or visualization and subsequently prompts for another question. This new question could be related to the previous question or could be on an entirely new topic.
   - If an error occurs during code execution, the program requests a corrected version of the code from the OpenAI API by providing the error message, and then attempts to execute the corrected code. *In cases where the "llm_switch" argument is set to "True" (indicating LLM cascading), the program will switch from the base model to the more powerful GPT-4 model for a retry. After successful execution, it will revert to the base model.*
 - The program then displays the total token usage at each step, thereby providing insights into the resources consumed during the process.
 - Lastly, the final answer is evaluated and given a score between 1-10. The answers that receive a rank above the threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
+ 
+**Flow chart:**
+
+![](images/flow_chart_3.png)
 
 ## How to use
 
 **Installation**
 
 ```
 pip install bambooai
@@ -67,18 +71,16 @@
 
 debug: bool - If True, the received code is sent back to the Language Learning Model (LLM) for an evaluation of its relevance to the user's question, along with code error checking and debugging.
 
 rank: bool - If True, the final version of the code is sent back to the Language Learning Model (LLM) ro ranking from on a scale from 1 to 10.The answers that receive a rank higher than the given threshold are exceptionally well-composed and are utilized to build the knowledge base for future references.
 
 exploratory: bool - If True, the LLM will assess the user's question and create a task list outlining the steps, which will be sent to the LLM as a prompt. This approach is effective for vague user prompts, but may not perform as well with more defined prompts. The default setting is True.
 
-flow_diagram: bool - If True, a mermaid diagram will be generated and displayed to complement the answer.
-
 
-e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True, flow_diagram=False)
+e.g. bamboo = BambooAI(df, debug=True, rank=True, llm_switch=True, exploratory=True)
 ```
 
 Run in a loop
 
 ```
 # Run in a loop remembering the conversation history
 import pandas as pd
@@ -101,20 +103,20 @@
 Visualize the data (Uses Matplotlib). Works with both Loop and Single execution
 
 **Environment Variables**
 
 The library requires an OpenAI API account and the API key to connect to an OpenAI LLMs. The OpenAI API key needs to be stored in a 'OPENAI_API_KEY' environment variable.
 The key can be obtained from here: https://platform.openai.com/account/api-keys
 
-
 ## Notes
 
 - The library currently supports only OpenAI Chat models. It has been tested with both gpt-3.5-turbo and gpt-4. The gpt-3.5-turbo seems to perform well and is the preferred option due to its 10x lower cost.
 - The library executes LLM generated Python code, this can be bad if the LLM generated Python code is harmful. Use cautiously.
-- Be sure to monitor your token usage, as each execution of BambooAI uses an average of 400-600 tokens. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
+- Be sure to monitor your token usage. At the time of writing, the cost per 1K tokens is $0.03 USD for GPT-4 and $0.002 USD for GPT-3.5-turbo. It's important to keep these costs in mind when using the library, particularly when using the more expensive models.
+- Supported models: gpt-3.5-turbo, gpt-3.5-turbo-613, gpt-3.5-turbo-16k, gpt-4, gpt-4-0613.
 
 ## Contributing
 
 Contributions are welcome; please feel free to open a pull request. Keep in mind that our goal is to maintain a concise codebase with high readability.
 
 ## ToDo
```

### Comparing `bambooai-0.3.3/setup.py` & `bambooai-0.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='bambooai',
-    version='0.3.3',
+    version='0.3.4',
     description='A lightweight library for working with pandas dataframes using natural language queries',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Palo Galko',
     packages=find_packages(),
     install_requires=[
         'openai',
```


# Comparing `tmp/ProTaska-GPT-0.0.8.tar.gz` & `tmp/ProTaska-GPT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProTaska-GPT-0.0.8.tar", last modified: Sat Jun 17 16:57:49 2023, max compression
+gzip compressed data, was "ProTaska-GPT-0.0.9.tar", last modified: Sat Jun 17 17:03:07 2023, max compression
```

## Comparing `ProTaska-GPT-0.0.8.tar` & `ProTaska-GPT-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:57:49.734953 ProTaska-GPT-0.0.8/
--rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2167 2023-06-17 16:57:49.734953 ProTaska-GPT-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 16:57:49.718547 ProTaska-GPT-0.0.8/ProTaska/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.8/ProTaska/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:57:49.721425 ProTaska-GPT-0.0.8/ProTaska/data/
--rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.8/ProTaska/data/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.8/ProTaska/data/data_utils.py
--rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.8/ProTaska/data/ingestion.py
--rw-rw-rw-   0        0        0     5357 2023-06-17 16:57:15.000000 ProTaska-GPT-0.0.8/ProTaska/data/loader.py
--rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.8/ProTaska/describer.py
--rw-rw-rw-   0        0        0     3323 2023-06-17 16:48:44.000000 ProTaska-GPT-0.0.8/ProTaska/ideate.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:57:49.734953 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/
--rw-rw-rw-   0        0        0     2167 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 16:57:49.000000 ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 16:57:49.734953 ProTaska-GPT-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-06-17 16:57:21.000000 ProTaska-GPT-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 17:03:07.803465 ProTaska-GPT-0.0.9/
+-rw-rw-rw-   0        0        0     1092 2023-06-14 10:32:13.000000 ProTaska-GPT-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2167 2023-06-17 17:03:07.803465 ProTaska-GPT-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 17:03:07.782390 ProTaska-GPT-0.0.9/ProTaska/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:39:28.000000 ProTaska-GPT-0.0.9/ProTaska/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 17:03:07.787461 ProTaska-GPT-0.0.9/ProTaska/data/
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:36:56.000000 ProTaska-GPT-0.0.9/ProTaska/data/__init__.py
+-rw-rw-rw-   0        0        0     4396 2023-06-14 23:22:05.000000 ProTaska-GPT-0.0.9/ProTaska/data/data_utils.py
+-rw-rw-rw-   0        0        0     2327 2023-06-15 20:26:38.000000 ProTaska-GPT-0.0.9/ProTaska/data/ingestion.py
+-rw-rw-rw-   0        0        0     5357 2023-06-17 16:57:15.000000 ProTaska-GPT-0.0.9/ProTaska/data/loader.py
+-rw-rw-rw-   0        0        0     2009 2023-06-17 15:29:17.000000 ProTaska-GPT-0.0.9/ProTaska/describer.py
+-rw-rw-rw-   0        0        0     3373 2023-06-17 17:02:38.000000 ProTaska-GPT-0.0.9/ProTaska/ideate.py
+drwxrwxrwx   0        0        0        0 2023-06-17 17:03:07.797283 ProTaska-GPT-0.0.9/ProTaska_GPT.egg-info/
+-rw-rw-rw-   0        0        0     2167 2023-06-17 17:03:07.000000 ProTaska-GPT-0.0.9/ProTaska_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-17 17:03:07.000000 ProTaska-GPT-0.0.9/ProTaska_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 17:03:07.000000 ProTaska-GPT-0.0.9/ProTaska_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-17 17:03:07.000000 ProTaska-GPT-0.0.9/ProTaska_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 17:03:07.000000 ProTaska-GPT-0.0.9/ProTaska_GPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1445 2023-06-17 16:24:08.000000 ProTaska-GPT-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 17:03:07.803465 ProTaska-GPT-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-06-17 17:02:46.000000 ProTaska-GPT-0.0.9/setup.py
```

### Comparing `ProTaska-GPT-0.0.8/LICENSE` & `ProTaska-GPT-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.8/PKG-INFO` & `ProTaska-GPT-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.8/ProTaska/data/data_utils.py` & `ProTaska-GPT-0.0.9/ProTaska/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.8/ProTaska/data/ingestion.py` & `ProTaska-GPT-0.0.9/ProTaska/data/ingestion.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.8/ProTaska/data/loader.py` & `ProTaska-GPT-0.0.9/ProTaska/data/loader.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.8/ProTaska/describer.py` & `ProTaska-GPT-0.0.9/ProTaska/describer.py`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.8/ProTaska/ideate.py` & `ProTaska-GPT-0.0.9/ProTaska/ideate.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,16 @@
         )
         self.second_output = self.agent_chain.run(self.first_output+"\n\nFind relevant sources from Wikipedia from the above techniques and advances. Also include some TLDRs in front of those links. Be specific to the ML techniques previously mentioned.")
 
     def __call__(self, human_input):
         output = self.agent_chain.run(human_input)
         return output
 
-def main(openai_key, dataset_description):
-    chat_bot = ChatBotWrapper(openai_key, dataset_description)
+def main(openai_key, dataset_description, agent_verbose=False):
+    chat_bot = ChatBotWrapper(openai_key, dataset_description, agent_verbose=agent_verbose)
     print("ProTaska:\t", chat_bot.first_output)
     print("ProTaska-Source:\t", chat_bot.second_output)
     print()
     while True:
         human_input = input("Human (input 'break' or 'exit' to stop the loop):\t")
         if human_input=='exit' or human_input=='break':
             print("ProTaska:\tStopping Execution!")
```

### Comparing `ProTaska-GPT-0.0.8/ProTaska_GPT.egg-info/PKG-INFO` & `ProTaska-GPT-0.0.9/ProTaska_GPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProTaska-GPT
-Version: 0.0.8
+Version: 0.0.9
 Summary: Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.
 Home-page: https://github.com/AmanPriyanshu/protaska-gpt
 Author: Aman Priyanshu, Supriti Vijay
 Author-email: amanpriyanshusms2001@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProTaska-GPT-0.0.8/README.md` & `ProTaska-GPT-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ProTaska-GPT-0.0.8/setup.py` & `ProTaska-GPT-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ProTaska-GPT',
-    version='0.0.8',
+    version='0.0.9',
     description='Unleash the Potential of Datasets with Intelligent Tasks, Tutorials, and Algorithm Recommendations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Aman Priyanshu, Supriti Vijay',
     author_email='amanpriyanshusms2001@gmail.com',
     packages=find_packages(exclude=["notebooks", "docs"]),
     url='https://github.com/AmanPriyanshu/protaska-gpt',
```


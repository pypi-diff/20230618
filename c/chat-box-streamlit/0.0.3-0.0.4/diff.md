# Comparing `tmp/chat-box-streamlit-0.0.3.tar.gz` & `tmp/chat-box-streamlit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.3.tar", last modified: Tue Jun 13 15:32:24 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.4.tar", last modified: Sun Jun 18 09:37:08 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.3.tar` & `chat-box-streamlit-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:32:24.707426 chat-box-streamlit-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 15:32:09.000000 chat-box-streamlit-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 15:32:09.000000 chat-box-streamlit-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-13 15:32:24.707426 chat-box-streamlit-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-13 15:32:09.000000 chat-box-streamlit-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:32:24.703426 chat-box-streamlit-0.0.3/chat_box/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-13 15:32:09.000000 chat-box-streamlit-0.0.3/chat_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:32:24.707426 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 15:32:24.000000 chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:32:24.707426 chat-box-streamlit-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-13 15:32:11.000000 chat-box-streamlit-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-18 09:36:57.000000 chat-box-streamlit-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-18 09:36:57.000000 chat-box-streamlit-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-18 09:36:57.000000 chat-box-streamlit-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/chat_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-18 09:36:57.000000 chat-box-streamlit-0.0.4/chat_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 09:36:59.000000 chat-box-streamlit-0.0.4/setup.py
```

### Comparing `chat-box-streamlit-0.0.3/LICENSE` & `chat-box-streamlit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.3/PKG-INFO` & `chat-box-streamlit-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,54 +26,42 @@
 1. Install the necessary dependencies by running the following command:
 ```
 pip install chat-box-streamlit
 ```
 
 2. Import the ChatBox component in your Streamlit application:
 ```
-from chat-box-streamlit import display_chat
+from chat_box import display_chat
+from chat_box import input
+from chat_box import message
 ```
 
 ## How to use 
 
 1. Input Box
 ![Input Box](./assets/Input-Box.png)
 To display an input box where users can enter their messages, use the following code:
 ```python
-response = display_chat(component="input", placeholder="This is the input component", rows=1)
+response = input(placeholder="This is the input component", rows=1)
 st.write(response)
 ```
 To display with loading:
 ```python
-response = display_chat(component="input", loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
+response = input(loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
 st.write(response)
 ```
 
 2. Left and Right Messages
 ![Left and Right Messages](./assets/Message.png)
 You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
 ```
-display_chat(component="message", isLeft=True, message="Hi, I am the left message component")
-display_chat(component="message", isLeft=False, message="Hello, I am the right message component")
+message(isLeft=True, message="Hi, I am the left message component")
+message(isLeft=False, message="Hello, I am the right message component")
 ```
 
-3. Complete Chat Component
-![Complete Chat Component](./assets/Complete-Chat.png)
-For a complete chat component with multiple messages, loading and scrollable content, use the following code:
-```python
-response = display_chat(
-    message=["What is your name?", "I am the chat component", "How are you different from others?", "I am a complete chat box with scroll"],
-    placeholder="Enter your input",
-    height=600
-)
-st.write(response)
-```
-For loading you can pass parameters
-```loading=True and loadingText="Fetching the message..."```
-
 ## Enjoy Conversational UI! 🗣️💬
 Feel free to experiment with different messages, components, and settings to create your unique chatbox experience. Happy coding! 💻🎉
 
 ## Contributing 🤝
 Contributions to the Streamlit Chat Box project are welcome! If you encounter any issues, have suggestions for improvements, or would like to contribute new features, please open an issue or submit a pull request on the GitHub repository.
 
 ## How to Contribute 👨‍💻
```

### Comparing `chat-box-streamlit-0.0.3/README.md` & `chat-box-streamlit-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,54 +15,42 @@
 1. Install the necessary dependencies by running the following command:
 ```
 pip install chat-box-streamlit
 ```
 
 2. Import the ChatBox component in your Streamlit application:
 ```
-from chat-box-streamlit import display_chat
+from chat_box import display_chat
+from chat_box import input
+from chat_box import message
 ```
 
 ## How to use 
 
 1. Input Box
 ![Input Box](./assets/Input-Box.png)
 To display an input box where users can enter their messages, use the following code:
 ```python
-response = display_chat(component="input", placeholder="This is the input component", rows=1)
+response = input(placeholder="This is the input component", rows=1)
 st.write(response)
 ```
 To display with loading:
 ```python
-response = display_chat(component="input", loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
+response = input(loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
 st.write(response)
 ```
 
 2. Left and Right Messages
 ![Left and Right Messages](./assets/Message.png)
 You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
 ```
-display_chat(component="message", isLeft=True, message="Hi, I am the left message component")
-display_chat(component="message", isLeft=False, message="Hello, I am the right message component")
+message(isLeft=True, message="Hi, I am the left message component")
+message(isLeft=False, message="Hello, I am the right message component")
 ```
 
-3. Complete Chat Component
-![Complete Chat Component](./assets/Complete-Chat.png)
-For a complete chat component with multiple messages, loading and scrollable content, use the following code:
-```python
-response = display_chat(
-    message=["What is your name?", "I am the chat component", "How are you different from others?", "I am a complete chat box with scroll"],
-    placeholder="Enter your input",
-    height=600
-)
-st.write(response)
-```
-For loading you can pass parameters
-```loading=True and loadingText="Fetching the message..."```
-
 ## Enjoy Conversational UI! 🗣️💬
 Feel free to experiment with different messages, components, and settings to create your unique chatbox experience. Happy coding! 💻🎉
 
 ## Contributing 🤝
 Contributions to the Streamlit Chat Box project are welcome! If you encounter any issues, have suggestions for improvements, or would like to contribute new features, please open an issue or submit a pull request on the GitHub repository.
 
 ## How to Contribute 👨‍💻
```

### Comparing `chat-box-streamlit-0.0.3/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,54 +26,42 @@
 1. Install the necessary dependencies by running the following command:
 ```
 pip install chat-box-streamlit
 ```
 
 2. Import the ChatBox component in your Streamlit application:
 ```
-from chat-box-streamlit import display_chat
+from chat_box import display_chat
+from chat_box import input
+from chat_box import message
 ```
 
 ## How to use 
 
 1. Input Box
 ![Input Box](./assets/Input-Box.png)
 To display an input box where users can enter their messages, use the following code:
 ```python
-response = display_chat(component="input", placeholder="This is the input component", rows=1)
+response = input(placeholder="This is the input component", rows=1)
 st.write(response)
 ```
 To display with loading:
 ```python
-response = display_chat(component="input", loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
+response = input(loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
 st.write(response)
 ```
 
 2. Left and Right Messages
 ![Left and Right Messages](./assets/Message.png)
 You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
 ```
-display_chat(component="message", isLeft=True, message="Hi, I am the left message component")
-display_chat(component="message", isLeft=False, message="Hello, I am the right message component")
+message(isLeft=True, message="Hi, I am the left message component")
+message(isLeft=False, message="Hello, I am the right message component")
 ```
 
-3. Complete Chat Component
-![Complete Chat Component](./assets/Complete-Chat.png)
-For a complete chat component with multiple messages, loading and scrollable content, use the following code:
-```python
-response = display_chat(
-    message=["What is your name?", "I am the chat component", "How are you different from others?", "I am a complete chat box with scroll"],
-    placeholder="Enter your input",
-    height=600
-)
-st.write(response)
-```
-For loading you can pass parameters
-```loading=True and loadingText="Fetching the message..."```
-
 ## Enjoy Conversational UI! 🗣️💬
 Feel free to experiment with different messages, components, and settings to create your unique chatbox experience. Happy coding! 💻🎉
 
 ## Contributing 🤝
 Contributions to the Streamlit Chat Box project are welcome! If you encounter any issues, have suggestions for improvements, or would like to contribute new features, please open an issue or submit a pull request on the GitHub repository.
 
 ## How to Contribute 👨‍💻
```

### Comparing `chat-box-streamlit-0.0.3/setup.py` & `chat-box-streamlit-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.3",
+    version="0.0.4",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
```


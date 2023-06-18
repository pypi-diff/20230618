# Comparing `tmp/GmailBox-0.0.2.tar.gz` & `tmp/GmailBox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GmailBox-0.0.2.tar", last modified: Fri Jun 16 13:42:44 2023, max compression
+gzip compressed data, was "GmailBox-0.0.3.tar", last modified: Sun Jun 18 05:18:24 2023, max compression
```

## Comparing `GmailBox-0.0.2.tar` & `GmailBox-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 13:42:44.301563 GmailBox-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-16 13:42:44.250603 GmailBox-0.0.2/GmailBox/
--rw-rw-rw-   0        0        0     5608 2023-06-15 15:08:43.000000 GmailBox-0.0.2/GmailBox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 13:42:44.296560 GmailBox-0.0.2/GmailBox.egg-info/
--rw-rw-rw-   0        0        0     1409 2023-06-16 13:42:44.000000 GmailBox-0.0.2/GmailBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-06-16 13:42:44.000000 GmailBox-0.0.2/GmailBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 13:42:44.000000 GmailBox-0.0.2/GmailBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-16 13:42:44.000000 GmailBox-0.0.2/GmailBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 13:42:44.000000 GmailBox-0.0.2/GmailBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1409 2023-06-16 13:42:44.299581 GmailBox-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      838 2023-06-16 13:09:56.000000 GmailBox-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 13:42:44.301563 GmailBox-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-16 13:42:21.000000 GmailBox-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:18:24.692305 GmailBox-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-18 05:18:24.636148 GmailBox-0.0.3/GmailBox/
+-rw-rw-rw-   0        0        0     5708 2023-06-18 05:04:32.000000 GmailBox-0.0.3/GmailBox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:18:24.685311 GmailBox-0.0.3/GmailBox.egg-info/
+-rw-rw-rw-   0        0        0     1409 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 05:18:24.000000 GmailBox-0.0.3/GmailBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1409 2023-06-18 05:18:24.688308 GmailBox-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      838 2023-06-16 13:09:56.000000 GmailBox-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-18 05:18:24.692305 GmailBox-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-18 05:17:01.000000 GmailBox-0.0.3/setup.py
```

### Comparing `GmailBox-0.0.2/GmailBox/__init__.py` & `GmailBox-0.0.3/GmailBox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,13 +108,16 @@
                 'messageID': f'{messageID}',
             }
 
             text = self.request.post('https://www.emailnator.com/message-list', headers=headers, json=json_data).text
             soup = BeautifulSoup(text, 'html.parser')
             sender = hamoo['from']
             emaill = re.findall(r'<(.*?)>', sender)[0]
-            sender = re.findall(r'"(.*?)"', sender)[0]
+            try:
+                sender = re.findall(r'"(.*?)"', sender)[0]
+            except:
+                sender = sender.split(f'<{emaill}>')[0]
             subject = hamoo['subject']
             timee = hamoo['time']
             message = '\n'.join([p.text for p in soup.find_all('p')])
             end.append({'from':sender,'email':emaill,'subject':subject,'message':message,'time':timee})
         return end
```

### Comparing `GmailBox-0.0.2/GmailBox.egg-info/PKG-INFO` & `GmailBox-0.0.3/GmailBox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GmailBox
-Version: 0.0.2
+Version: 0.0.3
 Summary: With this library, you can create random Gmail and receive messages
 Author: Hamo
 License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GmailBox Version: 0.0.2 Summary: With this library,
+Metadata-Version: 2.1 Name: GmailBox Version: 0.0.3 Summary: With this library,
 you can create random Gmail and receive messages Author: Hamo License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                                     [Hamo]
```

### Comparing `GmailBox-0.0.2/PKG-INFO` & `GmailBox-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GmailBox
-Version: 0.0.2
+Version: 0.0.3
 Summary: With this library, you can create random Gmail and receive messages
 Author: Hamo
 License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GmailBox Version: 0.0.2 Summary: With this library,
+Metadata-Version: 2.1 Name: GmailBox Version: 0.0.3 Summary: With this library,
 you can create random Gmail and receive messages Author: Hamo License: LGPLv3
 Keywords: gmail,mail,GmailBox,inbox Classifier: Development Status :: 1 -
 Planning Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: Unix Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
 :: Windows Description-Content-Type: text/markdown
                                     [Hamo]
```

### Comparing `GmailBox-0.0.2/README.md` & `GmailBox-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `GmailBox-0.0.2/setup.py` & `GmailBox-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
 	name= "GmailBox",
-	version= "0.0.2",
+	version= "0.0.3",
 	author= "Hamo",
     keywords=["gmail","mail","GmailBox","inbox"],
     install_requires=['requests','beautifulsoup4'],
     long_description=readme,
     long_description_content_type="text/markdown",
 	description= "With this library, you can create random Gmail and receive messages",
 	packages=setuptools.find_packages(),
```


# Comparing `tmp/AshCrypt-1.1.5.tar.gz` & `tmp/AshCrypt-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.1.5.tar", last modified: Sat Jun 17 16:35:05 2023, max compression
+gzip compressed data, was "AshCrypt-1.1.6.tar", last modified: Sun Jun 18 16:05:00 2023, max compression
```

## Comparing `AshCrypt-1.1.5.tar` & `AshCrypt-1.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:35:05.076210 AshCrypt-1.1.5/
-drwxrwxrwx   0        0        0        0 2023-06-17 16:35:05.050500 AshCrypt-1.1.5/AshCrypt/
--rw-rw-rw-   0        0        0     5157 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0     4387 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     7922 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/AshDatabase.py
--rw-rw-rw-   0        0        0     3001 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/AshFileCrypt.py
--rw-rw-rw-   0        0        0     2074 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/AshTextCrypt.py
--rw-rw-rw-   0        0        0     6000 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0    14403 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/README.md
--rw-rw-rw-   0        0        0       91 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:35:05.064049 AshCrypt-1.1.5/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    15322 2023-06-17 16:35:04.000000 AshCrypt-1.1.5/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-06-17 16:35:04.000000 AshCrypt-1.1.5/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:35:04.000000 AshCrypt-1.1.5/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-17 16:35:04.000000 AshCrypt-1.1.5/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-17 16:35:04.000000 AshCrypt-1.1.5/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/LICENSE
--rw-rw-rw-   0        0        0    15322 2023-06-17 16:35:05.075212 AshCrypt-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    17338 2023-06-17 16:22:19.000000 AshCrypt-1.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 16:35:05.076210 AshCrypt-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:35:05.071210 AshCrypt-1.1.5/unittestsAC/
--rw-rw-rw-   0        0        0       25 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/unittestsAC/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-06-17 16:19:54.000000 AshCrypt-1.1.5/unittestsAC/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:00.145609 AshCrypt-1.1.6/
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:00.041630 AshCrypt-1.1.6/AshCrypt/
+-rw-rw-rw-   0        0        0     5157 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0     4407 2023-06-18 16:01:05.000000 AshCrypt-1.1.6/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     7922 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/AshDatabase.py
+-rw-rw-rw-   0        0        0     3001 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/AshFileCrypt.py
+-rw-rw-rw-   0        0        0     2074 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/AshTextCrypt.py
+-rw-rw-rw-   0        0        0     6000 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0    14610 2023-06-18 15:58:49.000000 AshCrypt-1.1.6/AshCrypt/README.md
+-rw-rw-rw-   0        0        0       91 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:00.064401 AshCrypt-1.1.6/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    15529 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-18 16:04:59.000000 AshCrypt-1.1.6/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-17 16:19:54.000000 AshCrypt-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0    15529 2023-06-18 16:05:00.144600 AshCrypt-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    17580 2023-06-18 15:58:49.000000 AshCrypt-1.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:05:00.146604 AshCrypt-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-06-18 16:04:28.000000 AshCrypt-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:05:00.136233 AshCrypt-1.1.6/unittestsAC/
+-rw-rw-rw-   0        0        0       25 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/unittestsAC/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-06-17 18:15:01.000000 AshCrypt-1.1.6/unittestsAC/unittestAsh.py
```

### Comparing `AshCrypt-1.1.5/AshCrypt/Ash.py` & `AshCrypt-1.1.6/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.5/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.1.6/AshCrypt/AshCryptGUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ttkbootstrap as tk
 from AshCrypt.AshTextCrypt import *
-import qr
+import AshCrypt.qr as qr
 
 key = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
 
 def encryption():
     m = inputfield1_1.get()
     if len(m) > 200 :
         outputvar1.set('Too Long')
@@ -42,15 +42,15 @@
         label2.config(text='QR OFF')
 
 
 
 
 object = tk.Window(themename='vapor')
 object.resizable(False ,False)
-object.title('src')
+object.title('AshCrypt')
 object.geometry('500x540')
 
 frame1 = tk.Frame(master=object , width=500 , height=250)
 frame1.place(x=0 , y=0)
 frame2 = tk.Frame(master=object , width=500 , height=250)
 frame2.place(x=0 , y=250)
```

### Comparing `AshCrypt-1.1.5/AshCrypt/AshDatabase.py` & `AshCrypt-1.1.6/AshCrypt/AshDatabase.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.5/AshCrypt/AshFileCrypt.py` & `AshCrypt-1.1.6/AshCrypt/AshFileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.5/AshCrypt/AshTextCrypt.py` & `AshCrypt-1.1.6/AshCrypt/AshTextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.5/AshCrypt/CliCrypt.py` & `AshCrypt-1.1.6/AshCrypt/CliCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.5/AshCrypt/README.md` & `AshCrypt-1.1.6/AshCrypt/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Cryptography w/ AES-256
+# Cryptography Library : AES-256
 ##  Objective ## 
-#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
+#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
 ## Overview ## 
 **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
 <br>The library incorporates a base cryptography mdoule called **Ash** 
 
 <br>A simple, secure, and developer-oriented module for
 encryption and decryption with AES-256 (CBC) . It offers an intuitive
 interface, seamless integration with precompiled 
@@ -23,14 +23,24 @@
 <br>check **GUI**  for more info.
 
 While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
+**After the library is installed**
+<br>to run the GUI 
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+To run the CLI
+```shell
+python -m AshCrypt.CliCrypt
+```
+
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
 ## Ash Module ##
 The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers.
```

### Comparing `AshCrypt-1.1.5/AshCrypt/qr.py` & `AshCrypt-1.1.6/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.5/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.1.6/AshCrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cryptography w/ AES-256
+# Cryptography Library : AES-256
 ##  Objective ## 
-#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
+#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
 ## Overview ## 
 **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
 <br>The library incorporates a base cryptography mdoule called **Ash** 
 
 <br>A simple, secure, and developer-oriented module for
 encryption and decryption with AES-256 (CBC) . It offers an intuitive
 interface, seamless integration with precompiled 
@@ -44,14 +44,24 @@
 <br>check **GUI**  for more info.
 
 While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
+**After the library is installed**
+<br>to run the GUI 
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+To run the CLI
+```shell
+python -m AshCrypt.CliCrypt
+```
+
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
 ## Ash Module ##
 The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers.
```

### Comparing `AshCrypt-1.1.5/LICENSE` & `AshCrypt-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.5/PKG-INFO` & `AshCrypt-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.1.5
+Version: 1.1.6
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Cryptography w/ AES-256
+# Cryptography Library : AES-256
 ##  Objective ## 
-#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
+#### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256 With No Unnecessary Complications.
 ## Overview ## 
 **Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
 <br>The library incorporates a base cryptography mdoule called **Ash** 
 
 <br>A simple, secure, and developer-oriented module for
 encryption and decryption with AES-256 (CBC) . It offers an intuitive
 interface, seamless integration with precompiled 
@@ -44,14 +44,24 @@
 <br>check **GUI**  for more info.
 
 While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
+**After the library is installed**
+<br>to run the GUI 
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+To run the CLI
+```shell
+python -m AshCrypt.CliCrypt
+```
+
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
 ## Ash Module ##
 The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers.
```

### Comparing `AshCrypt-1.1.5/README.md` & `AshCrypt-1.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,23 @@
 <br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
 <br>It also has a qr module associated with it to display the message.
 <br>check [GUI](https://github.com/AshGw/AES-256/src#ashcryptgui) header for more info.
 
 
 While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints.
 
+**After the library is installed** 
+<br>To run the GUI 
+```shell
+python -m AshCrypt.AshCryptGUI
+```
+To run the CLI 
+```shell
+python -m AshCrypt.CliCrypt
+```
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [AshDatabase](https://github.com/AshGw/CryptographyAES-256#ashdatabase) header to learn more.
 
 ## Installation ##
@@ -246,14 +255,18 @@
 ```python
 import ttkbootstrap as tk
 from AshTextCrypt import *
 import qr
 
 key = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
 ```
+<br>To run the GUI anywhere
+```shell
+python -m AshCrypt.AshCryptGUI
+```
 ### QR ## 
 The `qr.py` module is used to display a qr code of the encrypted/decrypted messages to be quickly scanned and transmitted , you can use qr versions from `1` to `40` , although I recommend using `40` since it can take the maximum number of characters for small files , and `10` if you're working with the GUI which is intended for text/short messages,
 
 ## AshDatabase ##
 To support efficient content management, I have integrated this database module to enable the storage and retrieval of encrypted content in a safe and secure manner using an sqlite3 database
 
 Ensuring that the encrypted data remains organized and readily accessible to anyone with the right key. Any content going in must be encrypted with a key that you must keep off grid.
```

### Comparing `AshCrypt-1.1.5/setup.py` & `AshCrypt-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('AshCrypt/README.md','r') as f :
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.1.5',
+    version='1.1.6',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography library equipped with a file handling module along with"
                 " a text module w/ a user-friendly GUI and a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

### Comparing `AshCrypt-1.1.5/unittestsAC/unittestAsh.py` & `AshCrypt-1.1.6/unittestsAC/unittestAsh.py`

 * *Files identical despite different names*


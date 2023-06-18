# Comparing `tmp/qvatel_sms_api-1.0.tar.gz` & `tmp/qvatel_sms_api-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvatel_sms_api-1.0.tar", last modified: Sat Jun 17 23:54:16 2023, max compression
+gzip compressed data, was "qvatel_sms_api-1.0.5.tar", last modified: Sun Jun 18 01:19:26 2023, max compression
```

## Comparing `qvatel_sms_api-1.0.tar` & `qvatel_sms_api-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yoandysse   (501) staff       (20)        0 2023-06-17 23:54:16.132541 qvatel_sms_api-1.0/
--rw-r--r--   0 yoandysse   (501) staff       (20)     1542 2023-06-17 23:54:16.132432 qvatel_sms_api-1.0/PKG-INFO
--rw-r--r--   0 yoandysse   (501) staff       (20)     1204 2023-06-17 23:16:13.000000 qvatel_sms_api-1.0/README.md
-drwxr-xr-x   0 yoandysse   (501) staff       (20)        0 2023-06-17 23:54:16.131716 qvatel_sms_api-1.0/qvatel/
--rw-r--r--   0 yoandysse   (501) staff       (20)        0 2023-06-17 22:34:47.000000 qvatel_sms_api-1.0/qvatel/__init__.py
--rw-r--r--   0 yoandysse   (501) staff       (20)      993 2023-06-17 22:35:13.000000 qvatel_sms_api-1.0/qvatel/client.py
-drwxr-xr-x   0 yoandysse   (501) staff       (20)        0 2023-06-17 23:54:16.132257 qvatel_sms_api-1.0/qvatel_sms_api.egg-info/
--rw-r--r--   0 yoandysse   (501) staff       (20)     1542 2023-06-17 23:54:16.000000 qvatel_sms_api-1.0/qvatel_sms_api.egg-info/PKG-INFO
--rw-r--r--   0 yoandysse   (501) staff       (20)      243 2023-06-17 23:54:16.000000 qvatel_sms_api-1.0/qvatel_sms_api.egg-info/SOURCES.txt
--rw-r--r--   0 yoandysse   (501) staff       (20)        1 2023-06-17 23:54:16.000000 qvatel_sms_api-1.0/qvatel_sms_api.egg-info/dependency_links.txt
--rw-r--r--   0 yoandysse   (501) staff       (20)       24 2023-06-17 23:54:16.000000 qvatel_sms_api-1.0/qvatel_sms_api.egg-info/requires.txt
--rw-r--r--   0 yoandysse   (501) staff       (20)        7 2023-06-17 23:54:16.000000 qvatel_sms_api-1.0/qvatel_sms_api.egg-info/top_level.txt
--rw-r--r--   0 yoandysse   (501) staff       (20)       38 2023-06-17 23:54:16.132579 qvatel_sms_api-1.0/setup.cfg
--rw-r--r--   0 yoandysse   (501) staff       (20)      572 2023-06-17 23:45:03.000000 qvatel_sms_api-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:19:26.472817 qvatel_sms_api-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-18 01:19:26.472817 qvatel_sms_api-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-18 01:19:16.000000 qvatel_sms_api-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:19:26.468817 qvatel_sms_api-1.0.5/qvatel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 01:19:16.000000 qvatel_sms_api-1.0.5/qvatel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-18 01:19:16.000000 qvatel_sms_api-1.0.5/qvatel/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:19:26.472817 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:19:26.472817 qvatel_sms_api-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-18 01:19:16.000000 qvatel_sms_api-1.0.5/setup.py
```

### Comparing `qvatel_sms_api-1.0/PKG-INFO` & `qvatel_sms_api-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: qvatel_sms_api
-Version: 1.0
+Version: 1.0.5
 Summary: Una librería de Python para enviar SMS a través de QvaTel.com
-Home-page: 
+Home-page: https://github.com/yoandysse/qvatel_sms_api.git
 Author: Yoandy Isse
 Author-email: yoandysse@gmail.com
 License: MIT
 Keywords: sms,qvatel,api,python,enviar sms,sms masivos,sms marketing,sms api,sms gateway
 Description-Content-Type: text/markdown
 
 # QvaTel Python Library
@@ -25,15 +25,15 @@
 - Una cuenta de QvaTel con un API token de SMS.
 
 ## Instalación
 
 Instala la librería usando pip:
 
 ```
-pip install qvatelSMS
+pip install qvatel-sms-api
 
 ```
 
 ## Uso
 
 Aquí hay un ejemplo básico de cómo usar la librería para enviar un SMS, obtener el estado de un mensaje y consultar el balance de la cuenta:
```

### Comparing `qvatel_sms_api-1.0/README.md` & `qvatel_sms_api-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - Una cuenta de QvaTel con un API token de SMS.
 
 ## Instalación
 
 Instala la librería usando pip:
 
 ```
-pip install qvatelSMS
+pip install qvatel-sms-api
 
 ```
 
 ## Uso
 
 Aquí hay un ejemplo básico de cómo usar la librería para enviar un SMS, obtener el estado de un mensaje y consultar el balance de la cuenta:
```

### Comparing `qvatel_sms_api-1.0/qvatel_sms_api.egg-info/PKG-INFO` & `qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: qvatel-sms-api
-Version: 1.0
+Version: 1.0.5
 Summary: Una librería de Python para enviar SMS a través de QvaTel.com
-Home-page: 
+Home-page: https://github.com/yoandysse/qvatel_sms_api.git
 Author: Yoandy Isse
 Author-email: yoandysse@gmail.com
 License: MIT
 Keywords: sms,qvatel,api,python,enviar sms,sms masivos,sms marketing,sms api,sms gateway
 Description-Content-Type: text/markdown
 
 # QvaTel Python Library
@@ -25,15 +25,15 @@
 - Una cuenta de QvaTel con un API token de SMS.
 
 ## Instalación
 
 Instala la librería usando pip:
 
 ```
-pip install qvatelSMS
+pip install qvatel-sms-api
 
 ```
 
 ## Uso
 
 Aquí hay un ejemplo básico de cómo usar la librería para enviar un SMS, obtener el estado de un mensaje y consultar el balance de la cuenta:
```

### Comparing `qvatel_sms_api-1.0/setup.py` & `qvatel_sms_api-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='qvatel_sms_api',
-    version='1.0',
+    version='1.0.5',
     packages=['qvatel'],
-    url='',
+    url='https://github.com/yoandysse/qvatel_sms_api.git',
     license='MIT',
     author='Yoandy Isse',
     author_email='yoandysse@gmail.com',
     description='Una librería de Python para enviar SMS a través de QvaTel.com',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords=['sms', 'qvatel', 'api', 'python', 'enviar sms', 'sms masivos', 'sms marketing', 'sms api', 'sms gateway'],
```


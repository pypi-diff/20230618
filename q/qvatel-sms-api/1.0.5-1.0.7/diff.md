# Comparing `tmp/qvatel_sms_api-1.0.5.tar.gz` & `tmp/qvatel_sms_api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qvatel_sms_api-1.0.5.tar", last modified: Sun Jun 18 01:19:26 2023, max compression
+gzip compressed data, was "qvatel_sms_api-1.0.7.tar", last modified: Sun Jun 18 02:03:19 2023, max compression
```

## Comparing `qvatel_sms_api-1.0.5.tar` & `qvatel_sms_api-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:19:26.472817 qvatel_sms_api-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-18 01:19:26.472817 qvatel_sms_api-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-18 01:19:16.000000 qvatel_sms_api-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:19:26.468817 qvatel_sms_api-1.0.5/qvatel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 01:19:16.000000 qvatel_sms_api-1.0.5/qvatel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-18 01:19:16.000000 qvatel_sms_api-1.0.5/qvatel/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:19:26.472817 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 01:19:26.000000 qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:19:26.472817 qvatel_sms_api-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-18 01:19:16.000000 qvatel_sms_api-1.0.5/setup.py
+drwxr-xr-x   0 yoandysse   (501) staff       (20)        0 2023-06-18 02:03:19.746363 qvatel_sms_api-1.0.7/
+-rw-r--r--   0 yoandysse   (501) staff       (20)     1681 2023-06-18 02:03:19.746256 qvatel_sms_api-1.0.7/PKG-INFO
+-rw-r--r--   0 yoandysse   (501) staff       (20)     1293 2023-06-18 02:01:08.000000 qvatel_sms_api-1.0.7/README.md
+drwxr-xr-x   0 yoandysse   (501) staff       (20)        0 2023-06-18 02:03:19.745552 qvatel_sms_api-1.0.7/qvatel/
+-rw-r--r--   0 yoandysse   (501) staff       (20)        0 2023-06-17 22:34:47.000000 qvatel_sms_api-1.0.7/qvatel/__init__.py
+-rw-r--r--   0 yoandysse   (501) staff       (20)     1919 2023-06-18 01:45:35.000000 qvatel_sms_api-1.0.7/qvatel/client.py
+drwxr-xr-x   0 yoandysse   (501) staff       (20)        0 2023-06-18 02:03:19.746081 qvatel_sms_api-1.0.7/qvatel_sms_api.egg-info/
+-rw-r--r--   0 yoandysse   (501) staff       (20)     1681 2023-06-18 02:03:19.000000 qvatel_sms_api-1.0.7/qvatel_sms_api.egg-info/PKG-INFO
+-rw-r--r--   0 yoandysse   (501) staff       (20)      243 2023-06-18 02:03:19.000000 qvatel_sms_api-1.0.7/qvatel_sms_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yoandysse   (501) staff       (20)        1 2023-06-18 02:03:19.000000 qvatel_sms_api-1.0.7/qvatel_sms_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yoandysse   (501) staff       (20)       24 2023-06-18 02:03:19.000000 qvatel_sms_api-1.0.7/qvatel_sms_api.egg-info/requires.txt
+-rw-r--r--   0 yoandysse   (501) staff       (20)        7 2023-06-18 02:03:19.000000 qvatel_sms_api-1.0.7/qvatel_sms_api.egg-info/top_level.txt
+-rw-r--r--   0 yoandysse   (501) staff       (20)       38 2023-06-18 02:03:19.746404 qvatel_sms_api-1.0.7/setup.cfg
+-rw-r--r--   0 yoandysse   (501) staff       (20)      621 2023-06-18 02:03:02.000000 qvatel_sms_api-1.0.7/setup.py
```

### Comparing `qvatel_sms_api-1.0.5/PKG-INFO` & `qvatel_sms_api-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: qvatel_sms_api
-Version: 1.0.5
+Version: 1.0.7
 Summary: Una librería de Python para enviar SMS a través de QvaTel.com
 Home-page: https://github.com/yoandysse/qvatel_sms_api.git
 Author: Yoandy Isse
 Author-email: yoandysse@gmail.com
 License: MIT
 Keywords: sms,qvatel,api,python,enviar sms,sms masivos,sms marketing,sms api,sms gateway
 Description-Content-Type: text/markdown
 
+
 # QvaTel Python Library
 
 Esta librería proporciona una interfaz de Python para interactuar con la API de SMS de QvaTel
 
 ## Funciones
 
 * Enviar mensajes SMS.
@@ -58,7 +59,9 @@
 balance = client.get_account_balance()
 print(balance)
 ```
 
 ## Contribuciones
 
 Las contribuciones son bienvenidas. Por favor, abre un issue si encuentras un bug o tienes una solicitud de función.
+
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/G2G4MDF91)
```

### Comparing `qvatel_sms_api-1.0.5/README.md` & `qvatel_sms_api-1.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # QvaTel Python Library
 
 Esta librería proporciona una interfaz de Python para interactuar con la API de SMS de QvaTel
 
 ## Funciones
 
 * Enviar mensajes SMS.
@@ -47,7 +48,9 @@
 balance = client.get_account_balance()
 print(balance)
 ```
 
 ## Contribuciones
 
 Las contribuciones son bienvenidas. Por favor, abre un issue si encuentras un bug o tienes una solicitud de función.
+
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/G2G4MDF91)
```

### Comparing `qvatel_sms_api-1.0.5/qvatel_sms_api.egg-info/PKG-INFO` & `qvatel_sms_api-1.0.7/qvatel_sms_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: qvatel-sms-api
-Version: 1.0.5
+Version: 1.0.7
 Summary: Una librería de Python para enviar SMS a través de QvaTel.com
 Home-page: https://github.com/yoandysse/qvatel_sms_api.git
 Author: Yoandy Isse
 Author-email: yoandysse@gmail.com
 License: MIT
 Keywords: sms,qvatel,api,python,enviar sms,sms masivos,sms marketing,sms api,sms gateway
 Description-Content-Type: text/markdown
 
+
 # QvaTel Python Library
 
 Esta librería proporciona una interfaz de Python para interactuar con la API de SMS de QvaTel
 
 ## Funciones
 
 * Enviar mensajes SMS.
@@ -58,7 +59,9 @@
 balance = client.get_account_balance()
 print(balance)
 ```
 
 ## Contribuciones
 
 Las contribuciones son bienvenidas. Por favor, abre un issue si encuentras un bug o tienes una solicitud de función.
+
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/G2G4MDF91)
```

### Comparing `qvatel_sms_api-1.0.5/setup.py` & `qvatel_sms_api-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='qvatel_sms_api',
-    version='1.0.5',
+    version='1.0.7',
     packages=['qvatel'],
     url='https://github.com/yoandysse/qvatel_sms_api.git',
     license='MIT',
     author='Yoandy Isse',
     author_email='yoandysse@gmail.com',
     description='Una librería de Python para enviar SMS a través de QvaTel.com',
     long_description=open('README.md').read(),
```


# Comparing `tmp/vaultpass-1.0.8.tar.gz` & `tmp/vaultpass-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vaultpass-1.0.8.tar", last modified: Fri Jun 16 19:19:06 2023, max compression
+gzip compressed data, was "dist/vaultpass-1.0.9.tar", last modified: Fri Jun 16 19:33:12 2023, max compression
```

## Comparing `vaultpass-1.0.8.tar` & `vaultpass-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:19:06.000000 vaultpass-1.0.8/
--rw-------   0 mjstew   (99386308) mcomm      (985)      731 2023-06-16 19:19:06.000000 vaultpass-1.0.8/PKG-INFO
-drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:19:06.000000 vaultpass-1.0.8/scripts/
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     9372 2023-04-15 17:06:35.000000 vaultpass-1.0.8/scripts/vaultpass.py
--rw-------   0 mjstew   (99386308) mcomm      (985)       38 2023-06-16 19:19:06.000000 vaultpass-1.0.8/setup.cfg
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     1105 2023-06-16 19:19:03.000000 vaultpass-1.0.8/setup.py
-drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass/
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)      322 2023-06-16 19:19:03.000000 vaultpass-1.0.8/vaultpass/__init__.py
--rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     9492 2023-04-04 23:50:11.000000 vaultpass-1.0.8/vaultpass/vaultpass.py
-drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/
--rw-------   0 mjstew   (99386308) mcomm      (985)      731 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/PKG-INFO
--rw-------   0 mjstew   (99386308) mcomm      (985)      238 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/SOURCES.txt
--rw-------   0 mjstew   (99386308) mcomm      (985)        1 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/dependency_links.txt
--rw-------   0 mjstew   (99386308) mcomm      (985)      142 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/requires.txt
--rw-------   0 mjstew   (99386308) mcomm      (985)       10 2023-06-16 19:19:06.000000 vaultpass-1.0.8/vaultpass.egg-info/top_level.txt
+drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:33:12.000000 vaultpass-1.0.9/
+-rw-------   0 mjstew   (99386308) mcomm      (985)      731 2023-06-16 19:33:12.000000 vaultpass-1.0.9/PKG-INFO
+drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:33:12.000000 vaultpass-1.0.9/scripts/
+-rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     9372 2023-04-15 17:06:35.000000 vaultpass-1.0.9/scripts/vaultpass.py
+-rw-------   0 mjstew   (99386308) mcomm      (985)       38 2023-06-16 19:33:12.000000 vaultpass-1.0.9/setup.cfg
+-rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     1078 2023-06-16 19:33:09.000000 vaultpass-1.0.9/setup.py
+drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:33:12.000000 vaultpass-1.0.9/vaultpass/
+-rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)      322 2023-06-16 19:33:09.000000 vaultpass-1.0.9/vaultpass/__init__.py
+-rwxr-xr-x   0 mjstew   (99386308) mcomm      (985)     9492 2023-04-04 23:50:11.000000 vaultpass-1.0.9/vaultpass/vaultpass.py
+drwx------   0 mjstew   (99386308) mcomm      (985)        0 2023-06-16 19:33:12.000000 vaultpass-1.0.9/vaultpass.egg-info/
+-rw-------   0 mjstew   (99386308) mcomm      (985)      731 2023-06-16 19:33:12.000000 vaultpass-1.0.9/vaultpass.egg-info/PKG-INFO
+-rw-------   0 mjstew   (99386308) mcomm      (985)      238 2023-06-16 19:33:12.000000 vaultpass-1.0.9/vaultpass.egg-info/SOURCES.txt
+-rw-------   0 mjstew   (99386308) mcomm      (985)        1 2023-06-16 19:33:12.000000 vaultpass-1.0.9/vaultpass.egg-info/dependency_links.txt
+-rw-------   0 mjstew   (99386308) mcomm      (985)      123 2023-06-16 19:33:12.000000 vaultpass-1.0.9/vaultpass.egg-info/requires.txt
+-rw-------   0 mjstew   (99386308) mcomm      (985)       10 2023-06-16 19:33:12.000000 vaultpass-1.0.9/vaultpass.egg-info/top_level.txt
```

### Comparing `vaultpass-1.0.8/PKG-INFO` & `vaultpass-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vaultpass
-Version: 1.0.8
+Version: 1.0.9
 Summary: VaultPass: A CyberArk search CLI. Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.
 Home-page: https://github.com/mjackstewart/vaultpass
 Author: Jack Stewart
 Author-email: mjackstewart@gmail.com
 License: Unilicense
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `vaultpass-1.0.8/scripts/vaultpass.py` & `vaultpass-1.0.9/scripts/vaultpass.py`

 * *Files identical despite different names*

### Comparing `vaultpass-1.0.8/setup.py` & `vaultpass-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,20 @@
 	'enum34',
 	'idna',
 	'pexpect',
 	'ptyprocess',
 	'pypass',
 	'typing_extensions',
 	'urllib3==1.26.6',
-	'rich==12.0.0',
-	'twine',
 	'requests',
 ]
 
 setup(
 	name='vaultpass',
-    	version='1.0.8',    
+    	version='1.0.9',    
     	description='VaultPass: A CyberArk search CLI. Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.',
     	url='https://github.com/mjackstewart/vaultpass',
     	author='Jack Stewart',
     	author_email='mjackstewart@gmail.com',
     	license='Unilicense',
     	packages=['vaultpass'],
 	setup_requires=requirements_list,
```

### Comparing `vaultpass-1.0.8/vaultpass/vaultpass.py` & `vaultpass-1.0.9/vaultpass/vaultpass.py`

 * *Files identical despite different names*

### Comparing `vaultpass-1.0.8/vaultpass.egg-info/PKG-INFO` & `vaultpass-1.0.9/vaultpass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vaultpass
-Version: 1.0.8
+Version: 1.0.9
 Summary: VaultPass: A CyberArk search CLI. Search for accounts and retrieve their passwords in the CyberArk elevated access management application. You can only retrieve accounts that you are able to view.
 Home-page: https://github.com/mjackstewart/vaultpass
 Author: Jack Stewart
 Author-email: mjackstewart@gmail.com
 License: Unilicense
 Description: UNKNOWN
 Platform: UNKNOWN
```


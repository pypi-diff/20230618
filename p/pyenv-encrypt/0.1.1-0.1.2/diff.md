# Comparing `tmp/pyenv-encrypt-0.1.1.tar.gz` & `tmp/pyenv-encrypt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenv-encrypt-0.1.1.tar", last modified: Thu Jun 15 17:14:40 2023, max compression
+gzip compressed data, was "pyenv-encrypt-0.1.2.tar", last modified: Sun Jun 18 21:56:57 2023, max compression
```

## Comparing `pyenv-encrypt-0.1.1.tar` & `pyenv-encrypt-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:14:40.873376 pyenv-encrypt-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-15 17:14:28.000000 pyenv-encrypt-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-15 17:14:40.873376 pyenv-encrypt-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-15 17:14:28.000000 pyenv-encrypt-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:14:40.869377 pyenv-encrypt-0.1.1/pyenv_enc/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 17:14:29.000000 pyenv-encrypt-0.1.1/pyenv_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-15 17:14:29.000000 pyenv-encrypt-0.1.1/pyenv_enc/enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:14:40.873376 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 17:14:40.000000 pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 17:14:29.000000 pyenv-encrypt-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:14:40.873376 pyenv-encrypt-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:56:57.402146 pyenv-encrypt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-18 21:56:44.000000 pyenv-encrypt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-18 21:56:57.402146 pyenv-encrypt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-18 21:56:44.000000 pyenv-encrypt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:56:57.402146 pyenv-encrypt-0.1.2/pyenv_enc/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-18 21:56:44.000000 pyenv-encrypt-0.1.2/pyenv_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-18 21:56:44.000000 pyenv-encrypt-0.1.2/pyenv_enc/enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:56:57.402146 pyenv-encrypt-0.1.2/pyenv_encrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-18 21:56:57.000000 pyenv-encrypt-0.1.2/pyenv_encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-18 21:56:57.000000 pyenv-encrypt-0.1.2/pyenv_encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:56:57.000000 pyenv-encrypt-0.1.2/pyenv_encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 21:56:57.000000 pyenv-encrypt-0.1.2/pyenv_encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 21:56:57.000000 pyenv-encrypt-0.1.2/pyenv_encrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 21:56:57.000000 pyenv-encrypt-0.1.2/pyenv_encrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-18 21:56:44.000000 pyenv-encrypt-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 21:56:57.402146 pyenv-encrypt-0.1.2/setup.cfg
```

### Comparing `pyenv-encrypt-0.1.1/LICENSE` & `pyenv-encrypt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenv-encrypt-0.1.1/PKG-INFO` & `pyenv-encrypt-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenv-encrypt
-Version: 0.1.1
+Version: 0.1.2
 Summary: GPG based env file encryptor utility.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/pyenv-encrypt
 Project-URL: Bug Tracker, https://github.com/akhlakm/pyenv-encrypt/issues
 Keywords: encryption,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyenv-encrypt-0.1.1/README.md` & `pyenv-encrypt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyenv-encrypt-0.1.1/pyenv_enc/enc.py` & `pyenv-encrypt-0.1.2/pyenv_enc/enc.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,27 +74,37 @@
         return True
     else:
         print("Error - no public key found:", userid)
         return False
 
 
 def read_file(file: str) -> dict:
+    """
+    Read an env variable file into a dict object.
+    File format is auto detected based on its extension.
+
+    """
     with open(file, 'r') as fp:
         if file.endswith(".yaml") or file.endswith(".yml"):
             # print("Loading YAML file:", file)
             return yaml.safe_load(fp)
         elif file.endswith(".json"):
             # print("Loading JSON file:", file)
             return json.load(fp)
         else:
             # print("Loading ENV file:", file)
             return dotenv_values(stream=fp)
 
 
 def save_file(file: str, data: dict):
+    """
+    Save a dict object as a file.
+    File format is auto detected based on its extension.
+
+    """
     with open(file, 'w+') as fp:
         if file.endswith(".yaml") or file.endswith(".yml"):
             yaml.dump(data, fp, indent=4)
         elif file.endswith(".json"):
             json.dump(data, fp, indent=4)
         else:
             for key, val in data.items():
@@ -133,14 +143,15 @@
     value = value + "-----END PGP MESSAGE-----"
     command = f"gpg -d"
     encvalue = exec(command, stdin=value).stdout
     return str(encvalue, encoding="utf-8")
 
 
 def encrypted(value : str) -> bool:
+    """ Returns True if the given string is encrypted."""
     return type(value) == str and value.startswith(_MARKUP)
 
 
 def encrypt_data(userid: str, data: dict) -> dict:
     """
     Recursively loop over a dictionary and encrypt all string fields.
```

### Comparing `pyenv-encrypt-0.1.1/pyenv_encrypt.egg-info/PKG-INFO` & `pyenv-encrypt-0.1.2/pyenv_encrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenv-encrypt
-Version: 0.1.1
+Version: 0.1.2
 Summary: GPG based env file encryptor utility.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/pyenv-encrypt
 Project-URL: Bug Tracker, https://github.com/akhlakm/pyenv-encrypt/issues
 Keywords: encryption,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyenv-encrypt-0.1.1/pyproject.toml` & `pyenv-encrypt-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyenv-encrypt"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="Akhlak Mahmood", email="akhlakm@gatech.edu" },
 ]
 description = "GPG based env file encryptor utility."
 readme = "README.md"
 requires-python = ">=3.0"
```


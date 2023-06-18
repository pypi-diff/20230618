# Comparing `tmp/configration-2.0.3.tar.gz` & `tmp/configration-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configration-2.0.3.tar", last modified: Mon Jun 12 13:01:34 2023, max compression
+gzip compressed data, was "configration-2.0.4.tar", last modified: Sun Jun 18 11:48:33 2023, max compression
```

## Comparing `configration-2.0.3.tar` & `configration-2.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.114670 configration-2.0.3/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.3/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1019 2023-06-12 13:01:34.114670 configration-2.0.3/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.3/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.108003 configration-2.0.3/configration/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.3/configration/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-09 06:22:46.000000 configration-2.0.3/configration/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.114670 configration-2.0.3/configration/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.3/configration/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2228 2023-06-09 11:25:05.000000 configration-2.0.3/configration/src/config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.3/configration/src/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1509 2023-06-09 14:31:15.000000 configration-2.0.3/configration/src/json_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2779 2023-06-09 11:37:05.000000 configration-2.0.3/configration/src/toml_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.114670 configration-2.0.3/configration/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.3/configration/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2848 2023-06-09 14:35:21.000000 configration-2.0.3/configration/tests/test_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-12 13:01:34.108003 configration-2.0.3/configration.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1019 2023-06-12 13:01:34.000000 configration-2.0.3/configration.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      449 2023-06-12 13:01:34.000000 configration-2.0.3/configration.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-12 13:01:34.000000 configration-2.0.3/configration.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-06-12 13:01:34.000000 configration-2.0.3/configration.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-12 13:01:34.114670 configration-2.0.3/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.3/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.176785 configration-2.0.4/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.4/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1121 2023-06-18 11:48:33.176785 configration-2.0.4/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.4/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.173452 configration-2.0.4/configration/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.4/configration/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-18 11:41:45.000000 configration-2.0.4/configration/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.176785 configration-2.0.4/configration/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.4/configration/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2228 2023-06-09 11:25:05.000000 configration-2.0.4/configration/src/config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.4/configration/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1509 2023-06-09 14:31:15.000000 configration-2.0.4/configration/src/json_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2779 2023-06-18 11:40:32.000000 configration-2.0.4/configration/src/toml_config.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.176785 configration-2.0.4/configration/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.4/configration/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2852 2023-06-18 11:39:33.000000 configration-2.0.4/configration/tests/test_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      229 2023-06-18 11:34:14.000000 configration-2.0.4/configration/xxx.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.173452 configration-2.0.4/configration.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1121 2023-06-18 11:48:33.000000 configration-2.0.4/configration.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      469 2023-06-18 11:48:33.000000 configration-2.0.4/configration.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-18 11:48:33.000000 configration-2.0.4/configration.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-06-18 11:48:33.000000 configration-2.0.4/configration.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-18 11:48:33.176785 configration-2.0.4/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.4/setup.py
```

### Comparing `configration-2.0.3/LICENSE.txt` & `configration-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.3/PKG-INFO` & `configration-2.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.3
+Version: 2.0.4
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
@@ -21,22 +21,30 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.4 18 June 2023
+
+1. Invalid toml test corrected
+2. Add tomli to requirements.txt
+
+------
+
 Version 2.0.3 9 June 2023
 
 1. Implement create()
 2. Implement save()
 3. Consolidated testing into one file
 
 ------
 
+
 Version 1.0.2 29 May 2023
 
 1. Provide __repr__
 
 ------
```

### Comparing `configration-2.0.3/configration/src/config.py` & `configration-2.0.4/configration/src/config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.3/configration/src/json_config.py` & `configration-2.0.4/configration/src/json_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.3/configration/src/toml_config.py` & `configration-2.0.4/configration/src/toml_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.3/configration/tests/test_config.py` & `configration-2.0.4/configration/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def test_all(capsys):
     for index, config_class in enumerate([JsonConfig, TomlConfig]):
         extension = ['json', 'toml'][index]
         config_structure(config_class, extension)
         config_missing(capsys, config_class, extension)
         config_invalid_attrs(capsys, config_class, extension)
-        config_invalid_json(capsys, config_class, extension)
+        config_invalid_format(capsys, config_class, extension)
         config_missing_attr(capsys, config_class, extension)
         config_create(config_class, extension)
 
 
 def config_structure(config_class, extension):
     path = Path('tests', 'test_data', f'config.{extension}')
     config = config_class(path)
@@ -45,15 +45,15 @@
     path = Path('tests', 'test_data', f'config_invalid_attrs.{extension}')
     err_msg = "Corrupt config file. month not of type [<class 'int'>]"
     config_class(path, CONFIG_ATTRS)
     captured = capsys.readouterr()
     assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
 
 
-def config_invalid_json(capsys, config_class, extension):
+def config_invalid_format(capsys, config_class, extension):
     path = Path('tests', 'test_data', f'config_invalid_{extension}.{extension}')
     err_msg = f"Invalid {extension} format in {path}"
     config_class(path)
     captured = capsys.readouterr()
     assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
```

### Comparing `configration-2.0.3/configration.egg-info/PKG-INFO` & `configration-2.0.4/configration.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.3
+Version: 2.0.4
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
@@ -21,22 +21,30 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.4 18 June 2023
+
+1. Invalid toml test corrected
+2. Add tomli to requirements.txt
+
+------
+
 Version 2.0.3 9 June 2023
 
 1. Implement create()
 2. Implement save()
 3. Consolidated testing into one file
 
 ------
 
+
 Version 1.0.2 29 May 2023
 
 1. Provide __repr__
 
 ------
```

### Comparing `configration-2.0.3/setup.py` & `configration-2.0.4/setup.py`

 * *Files identical despite different names*


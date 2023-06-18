# Comparing `tmp/caddo-file-parser-0.45.1.tar.gz` & `tmp/caddo-file-parser-0.46.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caddo-file-parser-0.45.1.tar", last modified: Mon May 15 17:17:56 2023, max compression
+gzip compressed data, was "caddo-file-parser-0.46.1.tar", last modified: Sun Jun 18 20:00:01 2023, max compression
```

## Comparing `caddo-file-parser-0.45.1.tar` & `caddo-file-parser-0.46.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:56.547115 caddo-file-parser-0.45.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/src/caddo_file_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/caddo_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/src/caddo_file_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/models/caddo_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/models/index_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/models/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/src/caddo_file_parser/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/settings/generation_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/settings/generation_settings_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/src/caddo_file_parser/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/test/file_reading_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/test/file_saving_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/test/settings_loader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/src/caddo_file_parser/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/validation/caddo_file_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-15 17:17:42.000000 caddo-file-parser-0.45.1/src/caddo_file_parser/validation/settings_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:17:56.551115 caddo-file-parser-0.45.1/src/caddo_file_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 17:17:56.000000 caddo-file-parser-0.45.1/src/caddo_file_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-15 17:17:56.000000 caddo-file-parser-0.45.1/src/caddo_file_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:17:56.000000 caddo-file-parser-0.45.1/src/caddo_file_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 17:17:56.000000 caddo-file-parser-0.45.1/src/caddo_file_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 17:17:56.000000 caddo-file-parser-0.45.1/src/caddo_file_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:00:01.127969 caddo-file-parser-0.46.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-18 20:00:01.127969 caddo-file-parser-0.46.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 20:00:01.127969 caddo-file-parser-0.46.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:00:01.123969 caddo-file-parser-0.46.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:00:01.123969 caddo-file-parser-0.46.1/src/caddo_file_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/caddo_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:00:01.123969 caddo-file-parser-0.46.1/src/caddo_file_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/models/caddo_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/models/index_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/models/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:00:01.123969 caddo-file-parser-0.46.1/src/caddo_file_parser/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/settings/generation_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/settings/generation_settings_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:00:01.127969 caddo-file-parser-0.46.1/src/caddo_file_parser/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/test/file_reading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/test/file_saving_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/test/settings_loader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:00:01.127969 caddo-file-parser-0.46.1/src/caddo_file_parser/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/validation/caddo_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-18 19:59:51.000000 caddo-file-parser-0.46.1/src/caddo_file_parser/validation/settings_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:00:01.123969 caddo-file-parser-0.46.1/src/caddo_file_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-18 20:00:01.000000 caddo-file-parser-0.46.1/src/caddo_file_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-18 20:00:01.000000 caddo-file-parser-0.46.1/src/caddo_file_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:00:01.000000 caddo-file-parser-0.46.1/src/caddo_file_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 20:00:01.000000 caddo-file-parser-0.46.1/src/caddo_file_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 20:00:01.000000 caddo-file-parser-0.46.1/src/caddo_file_parser.egg-info/top_level.txt
```

### Comparing `caddo-file-parser-0.45.1/src/caddo_file_parser/caddo_file_parser.py` & `caddo-file-parser-0.46.1/src/caddo_file_parser/caddo_file_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         settings_file = zf.read("settings.yaml").decode(encoding="utf-8")
         settings_yaml = yaml.load(settings_file, Loader=SafeLoader)
         return GenerationSettingsLoader().load_settings_object(settings_yaml)
 
     def read_csv_data(self, zf, generation_settings):
         separator = generation_settings.data_output_file_separator
         data_csv = zf.read("data.csv").decode(encoding="utf-8")
-        return pd.read_csv(io.StringIO(data_csv), sep=separator)
+        return pd.read_csv(io.StringIO(data_csv), sep=separator,  engine='python', on_bad_lines='skip')
 
     def read_runs(self, zf, generation_settings):
         runs = []
         total_runs_number = generation_settings.data_splitting_runs
         total_index_sets_in_run = self._get_total_index_sets_in_run(generation_settings)
         for run_number in range(total_runs_number):
             index_sets = []
```

### Comparing `caddo-file-parser-0.45.1/src/caddo_file_parser/models/index_set.py` & `caddo-file-parser-0.46.1/src/caddo_file_parser/models/index_set.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.45.1/src/caddo_file_parser/settings/generation_settings.py` & `caddo-file-parser-0.46.1/src/caddo_file_parser/settings/generation_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     data_input_path = ''
     data_input_separator = ''
     data_extraction_function_path = ''
     data_splitting_folding_number = 0
     data_splitting_runs = 0
     data_output_file_name = ''
     data_splitting_folding_method = ''
+    data_splitting_folding_seeds_auto_generate = False
     data_splitting_folding_seeds_from_list = []
     data_splitting_folding_seeds_file_path = ''
     data_output_file_separator = ''
 
 # SAMPLE FILE
 # data:
 #   input:
```

### Comparing `caddo-file-parser-0.45.1/src/caddo_file_parser/settings/generation_settings_loader.py` & `caddo-file-parser-0.46.1/src/caddo_file_parser/settings/generation_settings_loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,17 @@
         settings_data.data_input_path = settings_file["data"]["input"]["path"]
         settings_data.data_input_separator = settings_file["data"]["input"]["separator"]
         settings_data.data_extraction_function_path = settings_file["data"]['extraction']['function']['path']
         settings_data.data_splitting_folding_number = settings_file["data"]['splitting']['folding']['number']
         settings_data.data_splitting_runs = settings_file["data"]['splitting']['runs']
         settings_data.data_output_file_name = settings_file["data"]['output']['file']['name']
         settings_data.data_splitting_folding_method = settings_file["data"]['splitting']['folding']['method']
-        if settings_file["data"]['splitting']['folding']['seeds']['from_list'] is not None:
-            settings_data.data_splitting_folding_seeds_from_list = settings_file["data"]['splitting']['folding']['seeds']['from_list']
-        if settings_file["data"]['splitting']['folding']['seeds']['from_file'] is not None:
-            settings_data.data_splitting_folding_seeds_file_path = settings_file["data"]['splitting']['folding']['seeds']['from_file']
+        if settings_file["data"]['splitting']['folding']['seeds']['auto_generate'] is False:
+            if settings_file["data"]['splitting']['folding']['seeds']['from_list'] is not None:
+                settings_data.data_splitting_folding_seeds_from_list = settings_file["data"]['splitting']['folding']['seeds']['from_list']
+            if settings_file["data"]['splitting']['folding']['seeds']['from_file'] is not None:
+                settings_data.data_splitting_folding_seeds_file_path = settings_file["data"]['splitting']['folding']['seeds']['from_file']
+        else:
+            settings_data.data_splitting_folding_seeds_from_list = [x + 1 for x in range(settings_data.data_splitting_runs * settings_data.data_splitting_folding_number)]
         settings_data.data_output_file_separator = settings_file["data"]['output']['file']['separator']
         SettingsValidator().validate(settings_data)
         return settings_data
```

### Comparing `caddo-file-parser-0.45.1/src/caddo_file_parser/test/file_saving_test.py` & `caddo-file-parser-0.46.1/src/caddo_file_parser/test/file_saving_test.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.45.1/src/caddo_file_parser/validation/caddo_file_validator.py` & `caddo-file-parser-0.46.1/src/caddo_file_parser/validation/caddo_file_validator.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.45.1/src/caddo_file_parser/validation/settings_validator.py` & `caddo-file-parser-0.46.1/src/caddo_file_parser/validation/settings_validator.py`

 * *Files identical despite different names*

### Comparing `caddo-file-parser-0.45.1/src/caddo_file_parser.egg-info/SOURCES.txt` & `caddo-file-parser-0.46.1/src/caddo_file_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*


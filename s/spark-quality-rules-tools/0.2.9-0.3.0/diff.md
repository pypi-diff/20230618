# Comparing `tmp/spark_quality_rules_tools-0.2.9.tar.gz` & `tmp/spark_quality_rules_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.2.9.tar", last modified: Sat Jun 17 21:37:32 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.3.0.tar", last modified: Sun Jun 18 12:51:49 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.2.9.tar` & `spark_quality_rules_tools-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 21:37:32.197585 spark_quality_rules_tools-0.2.9/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.9/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-06-17 21:37:32.197585 spark_quality_rules_tools-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.2.9/README.md
--rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-17 21:37:32.201586 spark_quality_rules_tools-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-06-17 21:37:20.000000 spark_quality_rules_tools-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 21:37:32.179581 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     1477 2023-06-14 13:37:36.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 21:37:32.193584 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    21200 2023-06-17 21:37:20.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-17 21:37:32.195584 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-06-17 21:37:32.196585 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-06-17 21:37:32.192584 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-06-17 21:37:32.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-06-17 21:37:32.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 21:37:32.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-06-17 21:37:32.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-17 21:37:32.000000 spark_quality_rules_tools-0.2.9/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.523546 spark_quality_rules_tools-0.3.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-06-18 12:51:49.523546 spark_quality_rules_tools-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.0/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-18 12:51:49.524546 spark_quality_rules_tools-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-06-18 12:10:00.000000 spark_quality_rules_tools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.507542 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     1477 2023-06-14 13:37:36.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.519545 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    21150 2023-06-18 03:08:52.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.521545 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.523546 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/resolve.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-06-18 12:51:49.518544 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-18 12:51:49.000000 spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.2.9/LICENSE` & `spark_quality_rules_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.9/PKG-INFO` & `spark_quality_rules_tools-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.2.9
+Version: 0.3.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.2.9/README.md` & `spark_quality_rules_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.9/pyproject.toml` & `spark_quality_rules_tools-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.9/setup.py` & `spark_quality_rules_tools-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.2.9',
+    version='0.3.0',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,18 +221,18 @@
 
     with open(dir_confs_filename) as f:
         hammurabi_conf = f.read()
 
     variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
     variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
     variables_list = list(set(variables_1 + variables_2))
-    print(variables_list)
+
     variables_dict = {variables: "" for variables in variables_list if
                       variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY")}
-    print(variables_dict)
+
     parameter_dict = dict()
     parameter_dict[uuaa_name] = list()
     parameter_dict[uuaa_name].append({"table": url_conf_name,
                                       "conf_name": url_conf_extension,
                                       "parameters": variables_dict})
 
     with open(f"{dir_confs_filename_parameters}", "w") as f:
```

### Comparing `spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/resource/resolve.conf` & `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/resolve.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.9/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.9/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.2.9
+Version: 0.3.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.2.9/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.3.0/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


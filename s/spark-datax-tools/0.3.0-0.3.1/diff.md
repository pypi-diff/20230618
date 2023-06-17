# Comparing `tmp/spark_datax_tools-0.3.0.tar.gz` & `tmp/spark_datax_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_datax_tools-0.3.0.tar", last modified: Mon Jun 12 04:29:49 2023, max compression
+gzip compressed data, was "spark_datax_tools-0.3.1.tar", last modified: Sat Jun 17 22:17:42 2023, max compression
```

## Comparing `spark_datax_tools-0.3.0.tar` & `spark_datax_tools-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 04:29:49.633324 spark_datax_tools-0.3.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       43 2023-06-12 03:39:06.000000 spark_datax_tools-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4266 2023-06-12 04:29:49.633324 spark_datax_tools-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3507 2023-06-12 03:37:30.000000 spark_datax_tools-0.3.0/README.md
--rw-rw-rw-   0        0        0      616 2023-06-12 03:41:29.000000 spark_datax_tools-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-12 04:29:49.638326 spark_datax_tools-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-12 04:29:34.000000 spark_datax_tools-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:29:49.614321 spark_datax_tools-0.3.0/spark_datax_tools/
--rw-rw-rw-   0        0        0     1441 2023-06-11 03:43:44.000000 spark_datax_tools-0.3.0/spark_datax_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:29:49.630324 spark_datax_tools-0.3.0/spark_datax_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.0/spark_datax_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    50446 2023-06-12 02:43:01.000000 spark_datax_tools-0.3.0/spark_datax_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:29:49.632324 spark_datax_tools-0.3.0/spark_datax_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.0/spark_datax_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_datax_tools-0.3.0/spark_datax_tools/utils/color.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:29:49.633324 spark_datax_tools-0.3.0/spark_datax_tools/utils/files/
--rw-rw-rw-   0        0        0     1911 2023-06-08 10:10:52.000000 spark_datax_tools-0.3.0/spark_datax_tools/utils/files/ns.csv
--rw-rw-rw-   0        0        0     3472 2023-06-05 07:39:00.000000 spark_datax_tools-0.3.0/spark_datax_tools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 04:29:49.629323 spark_datax_tools-0.3.0/spark_datax_tools.egg-info/
--rw-rw-rw-   0        0        0     4266 2023-06-12 04:29:49.000000 spark_datax_tools-0.3.0/spark_datax_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-06-12 04:29:49.000000 spark_datax_tools-0.3.0/spark_datax_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 04:29:49.000000 spark_datax_tools-0.3.0/spark_datax_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2023-06-12 04:29:49.000000 spark_datax_tools-0.3.0/spark_datax_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-12 04:29:49.000000 spark_datax_tools-0.3.0/spark_datax_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.156921 spark_datax_tools-0.3.1/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-06-12 03:39:06.000000 spark_datax_tools-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4266 2023-06-17 22:17:42.157922 spark_datax_tools-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3507 2023-06-12 03:37:30.000000 spark_datax_tools-0.3.1/README.md
+-rw-rw-rw-   0        0        0      616 2023-06-12 03:41:29.000000 spark_datax_tools-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-17 22:17:42.158923 spark_datax_tools-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-17 22:17:26.000000 spark_datax_tools-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.114911 spark_datax_tools-0.3.1/spark_datax_tools/
+-rw-rw-rw-   0        0        0     1441 2023-06-11 03:43:44.000000 spark_datax_tools-0.3.1/spark_datax_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.134916 spark_datax_tools-0.3.1/spark_datax_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.1/spark_datax_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    50486 2023-06-17 22:17:00.000000 spark_datax_tools-0.3.1/spark_datax_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.150920 spark_datax_tools-0.3.1/spark_datax_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:42:47.000000 spark_datax_tools-0.3.1/spark_datax_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-06-04 03:38:46.000000 spark_datax_tools-0.3.1/spark_datax_tools/utils/color.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.156921 spark_datax_tools-0.3.1/spark_datax_tools/utils/files/
+-rw-rw-rw-   0        0        0     1911 2023-06-08 10:10:52.000000 spark_datax_tools-0.3.1/spark_datax_tools/utils/files/ns.csv
+-rw-rw-rw-   0        0        0     3472 2023-06-05 07:39:00.000000 spark_datax_tools-0.3.1/spark_datax_tools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-17 22:17:42.133916 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/
+-rw-rw-rw-   0        0        0     4266 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-17 22:17:42.000000 spark_datax_tools-0.3.1/spark_datax_tools.egg-info/top_level.txt
```

### Comparing `spark_datax_tools-0.3.0/LICENSE` & `spark_datax_tools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.0/PKG-INFO` & `spark_datax_tools-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_datax_tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: spark_datax_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_datax_tools-0.3.0/README.md` & `spark_datax_tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.0/pyproject.toml` & `spark_datax_tools-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.0/setup.py` & `spark_datax_tools-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_datax_tools',
     packages=find_packages(),
-    version='0.3.0',
+    version='0.3.1',
     description='spark_datax_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_datax_tools/',
     download_url='https://github.com/jonaqp/spark_datax_tools/archive/main.zip',
```

### Comparing `spark_datax_tools-0.3.0/spark_datax_tools/__init__.py` & `spark_datax_tools-0.3.1/spark_datax_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.0/spark_datax_tools/functions/generator.py` & `spark_datax_tools-0.3.1/spark_datax_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,23 +455,24 @@
             ** {color:#0747a6}{key_do_out}{color}
 
             * {color:#0747a6}*Transfer_ID:*{color}  {key_transfer_id}
             ** {color:#0747a6}*Folder Control-M:*{color} {key_folder}
             ** {color:#0747a6}*JOB:*{color}  {key_job}
             ** {color:#0747a6}*PERIODICIDAD:*{color}  {key_periodicity}
             ** {color:#0747a6}*HORA:*{color}  {key_hour}
-            ** {color:#0747a6}*PESO:*{color}  {key_Weight}
+            ** {color:#0747a6}*PESO:*{color}  {key_weight}
             ** {color:#0747a6}*ORIGEN:*{color}  {key_origen}
             ** {color:#0747a6}*DESTINO:*{color}  {key_destination}
             ** {color:#0747a6}*CRQ:*{color}  {key_crq}
 
             {color:#0747a6}*Motivo modificación:*{color}  Promoción de transferencia
             ----
             """)
         ticket = ticket.replace('{key_uuaa}', uuaa) \
+            .replace('{key_ns}', ns) \
             .replace('{key_schema_in}', schema_in_id) \
             .replace('{key_schema_out}', schema_out_id) \
             .replace('{key_do_in}', do_read_id) \
             .replace('{key_do_out}', do_write_id) \
             .replace('{key_transfer_id}', transfer_id) \
             .replace('{key_folder}', folder) \
             .replace('{key_job}', job_name) \
```

### Comparing `spark_datax_tools-0.3.0/spark_datax_tools/utils/files/ns.csv` & `spark_datax_tools-0.3.1/spark_datax_tools/utils/files/ns.csv`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.0/spark_datax_tools/utils/utils.py` & `spark_datax_tools-0.3.1/spark_datax_tools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `spark_datax_tools-0.3.0/spark_datax_tools.egg-info/PKG-INFO` & `spark_datax_tools-0.3.1/spark_datax_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-datax-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: spark_datax_tools
 Home-page: https://github.com/jonaqp/spark_datax_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_datax_tools/archive/main.zip
 Keywords: spark,datax,schema
```

### Comparing `spark_datax_tools-0.3.0/spark_datax_tools.egg-info/SOURCES.txt` & `spark_datax_tools-0.3.1/spark_datax_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


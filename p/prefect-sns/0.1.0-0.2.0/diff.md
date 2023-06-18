# Comparing `tmp/prefect-sns-0.1.0.tar.gz` & `tmp/prefect-sns-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-sns/prefect-sns/dist/.tmp-03bdujej/prefect-sns-0.1.0.tar", last modified: Sun Jun 18 20:08:55 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-sns/prefect-sns/dist/.tmp-sooumthz/prefect-sns-0.2.0.tar", last modified: Sun Jun 18 20:35:13 2023, max compression
```

## Comparing `prefect-sns-0.1.0.tar` & `prefect-sns-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/prefect_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/prefect_sns/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/prefect_sns/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/prefect_sns/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/prefect_sns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:08:55.000000 prefect-sns-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-18 20:07:05.000000 prefect-sns-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/prefect_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/prefect_sns/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/prefect_sns/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/prefect_sns/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/prefect_sns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:35:13.000000 prefect-sns-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-18 20:32:56.000000 prefect-sns-0.2.0/versioneer.py
```

### Comparing `prefect-sns-0.1.0/LICENSE` & `prefect-sns-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-sns-0.1.0/PKG-INFO` & `prefect-sns-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-sns
-Version: 0.1.0
+Version: 0.2.0
 Summary: Prefect block for integration with AWS SNS
 Home-page: https://github.com/danielhstahl/prefect-sns
 Author: Daniel Stahl
 Author-email: danstahl1138@gmail.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-sns Version: 0.1.0 Summary: Prefect block
+Metadata-Version: 2.1 Name: prefect-sns Version: 0.2.0 Summary: Prefect block
 for integration with AWS SNS Home-page: https://github.com/danielhstahl/
 prefect-sns Author: Daniel Stahl Author-email: danstahl1138@gmail.com License:
 Apache License 2.0 Keywords: prefect Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `prefect-sns-0.1.0/README.md` & `prefect-sns-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prefect-sns-0.1.0/prefect_sns/blocks.py` & `prefect-sns-0.2.0/prefect_sns/blocks.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,18 @@
         block = SnsBlock.load("BLOCK_NAME")
         block.publish("my subject", "my message")
         ```
     """
 
     _block_type_name = "sns"
     # replace this with a relevant logo; defaults to Prefect logo
-    _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/08yCE6xpJMX9Kjl5VArDS/c2ede674c20f90b9b6edeab71feffac9/prefect-200x200.png?h=250"  # noqa
-    _documentation_url = "https://danielhstahl.github.io/prefect-sns/blocks/#prefect-sns.blocks.SnsBlock"  # noqa
+    _logo_url = "https://raw.githubusercontent.com/danielhstahl/prefect-sns/main/docs/img/aws-sns-simple-notification-service.svg"  # noqa
+    _documentation_url = (
+        "https://danielhstahl.github.io/prefect-sns/blocks_catalog/"  # noqa
+    )
 
     sns_arn: str
     aws_region: str = "us-east-1"
     aws_access_key_id: Optional[str] = None
     aws_secret_access_key: Optional[str] = None
 
     @classmethod
```

### Comparing `prefect-sns-0.1.0/prefect_sns/flows.py` & `prefect-sns-0.2.0/prefect_sns/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-sns-0.1.0/prefect_sns.egg-info/PKG-INFO` & `prefect-sns-0.2.0/prefect_sns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-sns
-Version: 0.1.0
+Version: 0.2.0
 Summary: Prefect block for integration with AWS SNS
 Home-page: https://github.com/danielhstahl/prefect-sns
 Author: Daniel Stahl
 Author-email: danstahl1138@gmail.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-sns Version: 0.1.0 Summary: Prefect block
+Metadata-Version: 2.1 Name: prefect-sns Version: 0.2.0 Summary: Prefect block
 for integration with AWS SNS Home-page: https://github.com/danielhstahl/
 prefect-sns Author: Daniel Stahl Author-email: danstahl1138@gmail.com License:
 Apache License 2.0 Keywords: prefect Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
```

### Comparing `prefect-sns-0.1.0/setup.cfg` & `prefect-sns-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-sns-0.1.0/setup.py` & `prefect-sns-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-sns-0.1.0/tests/test_block_standards.py` & `prefect-sns-0.2.0/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-sns-0.1.0/versioneer.py` & `prefect-sns-0.2.0/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/denormalize-0.0.1.tar.gz` & `tmp/denormalize-0.0.2.tar.gz`

## Comparing `denormalize-0.0.1.tar` & `denormalize-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 denormalize-0.0.1/src/denormalize/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 denormalize-0.0.1/src/denormalize/denormalize.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 denormalize-0.0.1/LICENSE
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 denormalize-0.0.1/README.md
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 denormalize-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 denormalize-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 denormalize-0.0.2/src/denormalize/denormalize.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 denormalize-0.0.2/LICENSE
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 denormalize-0.0.2/README.md
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 denormalize-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 denormalize-0.0.2/PKG-INFO
```

### Comparing `denormalize-0.0.1/src/denormalize/denormalize.py` & `denormalize-0.0.2/src/denormalize/denormalize.py`

 * *Files identical despite different names*

### Comparing `denormalize-0.0.1/LICENSE` & `denormalize-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `denormalize-0.0.1/PKG-INFO` & `denormalize-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: denormalize
-Version: 0.0.1
+Version: 0.0.2
 Summary: A single-cell denormalization tool
-Author-email: Lirong Yang <chichaumiau@gmail.com>
+Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```


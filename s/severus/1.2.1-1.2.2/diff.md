# Comparing `tmp/severus-1.2.1.tar.gz` & `tmp/severus-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "severus-1.2.1.tar", max compression
+gzip compressed data, was "severus-1.2.2.tar", max compression
```

## Comparing `severus-1.2.1.tar` & `severus-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      332 2023-03-14 13:21:33.652823 severus-1.2.1/CHANGES.md
--rw-r--r--   0        0        0     1486 2023-03-14 13:21:33.652823 severus-1.2.1/LICENSE
--rw-r--r--   0        0        0      724 2023-03-14 13:21:33.652823 severus-1.2.1/README.md
--rw-r--r--   0        0        0      252 2023-03-14 13:21:33.652823 severus-1.2.1/docs/README.md
--rw-r--r--   0        0        0     2105 2023-03-14 13:21:33.652823 severus-1.2.1/docs/installation.md
--rw-r--r--   0        0        0     5273 2023-03-14 13:21:33.652823 severus-1.2.1/docs/quickstart.md
--rw-r--r--   0        0        0       39 2023-03-14 13:21:33.652823 severus-1.2.1/docs/tree.yml
--rw-r--r--   0        0        0     1415 2023-03-14 13:21:33.652823 severus-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       52 2023-03-14 13:21:33.652823 severus-1.2.1/severus/__init__.py
--rw-r--r--   0        0        0       22 2023-03-14 13:21:33.652823 severus-1.2.1/severus/__version__.py
--rw-r--r--   0        0        0      834 2023-03-14 13:21:33.652823 severus-1.2.1/severus/apis.py
--rw-r--r--   0        0        0     1043 2023-03-14 13:21:33.652823 severus-1.2.1/severus/ctx.py
--rw-r--r--   0        0        0     2314 2023-03-14 13:21:33.652823 severus-1.2.1/severus/datastructures.py
--rw-r--r--   0        0        0     3695 2023-03-14 13:21:33.652823 severus-1.2.1/severus/language.py
--rw-r--r--   0        0        0        0 2023-03-14 13:21:33.652823 severus-1.2.1/severus/py.typed
--rw-r--r--   0        0        0     3440 2023-03-14 13:21:33.652823 severus-1.2.1/severus/translator.py
--rw-r--r--   0        0        0      433 2023-03-14 13:21:33.652823 severus-1.2.1/tests/conftest.py
--rw-r--r--   0        0        0      167 2023-03-14 13:21:33.652823 severus-1.2.1/tests/lang1/en.json
--rw-r--r--   0        0        0      290 2023-03-14 13:21:33.652823 severus-1.2.1/tests/lang1/it.yml
--rw-r--r--   0        0        0       69 2023-03-14 13:21:33.652823 severus-1.2.1/tests/lang1/ru.json
--rw-r--r--   0        0        0      372 2023-03-14 13:21:33.652823 severus-1.2.1/tests/lang2/en.json
--rw-r--r--   0        0        0      249 2023-03-14 13:21:33.652823 severus-1.2.1/tests/lang2/it/like.json
--rw-r--r--   0        0        0       40 2023-03-14 13:21:33.652823 severus-1.2.1/tests/lang2/it/weather.yml
--rw-r--r--   0        0        0       73 2023-03-14 13:21:33.652823 severus-1.2.1/tests/lang2/ru.yml
--rw-r--r--   0        0        0     1518 2023-03-14 13:21:33.652823 severus-1.2.1/tests/test_language.py
--rw-r--r--   0        0        0     4633 2023-03-14 13:21:33.652823 severus-1.2.1/tests/test_translator.py
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 severus-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      332 2023-06-18 12:12:59.464294 severus-1.2.2/CHANGES.md
+-rw-r--r--   0        0        0     1486 2023-06-18 12:12:59.468294 severus-1.2.2/LICENSE
+-rw-r--r--   0        0        0      724 2023-06-18 12:12:59.468294 severus-1.2.2/README.md
+-rw-r--r--   0        0        0      252 2023-06-18 12:12:59.468294 severus-1.2.2/docs/README.md
+-rw-r--r--   0        0        0     2105 2023-06-18 12:12:59.468294 severus-1.2.2/docs/installation.md
+-rw-r--r--   0        0        0     5273 2023-06-18 12:12:59.468294 severus-1.2.2/docs/quickstart.md
+-rw-r--r--   0        0        0       39 2023-06-18 12:12:59.468294 severus-1.2.2/docs/tree.yml
+-rw-r--r--   0        0        0     1415 2023-06-18 12:12:59.468294 severus-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-06-18 12:12:59.468294 severus-1.2.2/severus/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-18 12:12:59.468294 severus-1.2.2/severus/__version__.py
+-rw-r--r--   0        0        0      834 2023-06-18 12:12:59.468294 severus-1.2.2/severus/apis.py
+-rw-r--r--   0        0        0     1043 2023-06-18 12:12:59.468294 severus-1.2.2/severus/ctx.py
+-rw-r--r--   0        0        0     2314 2023-06-18 12:12:59.468294 severus-1.2.2/severus/datastructures.py
+-rw-r--r--   0        0        0     3697 2023-06-18 12:12:59.468294 severus-1.2.2/severus/language.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:12:59.468294 severus-1.2.2/severus/py.typed
+-rw-r--r--   0        0        0     3440 2023-06-18 12:12:59.468294 severus-1.2.2/severus/translator.py
+-rw-r--r--   0        0        0      433 2023-06-18 12:12:59.468294 severus-1.2.2/tests/conftest.py
+-rw-r--r--   0        0        0      167 2023-06-18 12:12:59.468294 severus-1.2.2/tests/lang1/en.json
+-rw-r--r--   0        0        0      290 2023-06-18 12:12:59.468294 severus-1.2.2/tests/lang1/it.yml
+-rw-r--r--   0        0        0       69 2023-06-18 12:12:59.468294 severus-1.2.2/tests/lang1/ru.json
+-rw-r--r--   0        0        0      372 2023-06-18 12:12:59.468294 severus-1.2.2/tests/lang2/en.json
+-rw-r--r--   0        0        0      249 2023-06-18 12:12:59.468294 severus-1.2.2/tests/lang2/it/like.json
+-rw-r--r--   0        0        0       40 2023-06-18 12:12:59.468294 severus-1.2.2/tests/lang2/it/weather.yml
+-rw-r--r--   0        0        0       73 2023-06-18 12:12:59.468294 severus-1.2.2/tests/lang2/ru.yml
+-rw-r--r--   0        0        0     1518 2023-06-18 12:12:59.468294 severus-1.2.2/tests/test_language.py
+-rw-r--r--   0        0        0     4633 2023-06-18 12:12:59.468294 severus-1.2.2/tests/test_translator.py
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 severus-1.2.2/PKG-INFO
```

### Comparing `severus-1.2.1/LICENSE` & `severus-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/README.md` & `severus-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/docs/installation.md` & `severus-1.2.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/docs/quickstart.md` & `severus-1.2.2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/pyproject.toml` & `severus-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "severus"
-version = "1.2.1"
+version = "1.2.2"
 description = "An internationalization engine designed with simplicity in mind"
 authors = ["Giovanni Barillari <gi0baro@d4net.org>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/severus"
 repository = "https://github.com/emmett-framework/severus"
```

### Comparing `severus-1.2.1/severus/apis.py` & `severus-1.2.2/severus/apis.py`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/severus/ctx.py` & `severus-1.2.2/severus/ctx.py`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/severus/datastructures.py` & `severus-1.2.2/severus/datastructures.py`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/severus/language.py` & `severus-1.2.2/severus/language.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 self._load_data(val, self._build_key(key, prefix))
 
     def _ensure_updated_sources(self):
         for source in self._sources:
             mtime = source['path'].stat().st_mtime
             if mtime != source['mtime']:
                 source['mtime'] = mtime
-                self._load_data(source['path'], source['prefix'])
+                self._load_source(source['path'], source['prefix'])
 
     def _get_reload(self, text: str) -> Tuple[str, Dict[int, str]]:
         self._ensure_updated_sources()
         return self._strings.get(text, text), self._groups.get(text, {})
 
     def _get_static(self, text: str) -> Tuple[str, Dict[int, str]]:
         return self._strings.get(text, text), self._groups.get(text, {})
```

### Comparing `severus-1.2.1/severus/translator.py` & `severus-1.2.2/severus/translator.py`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/tests/test_language.py` & `severus-1.2.2/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/tests/test_translator.py` & `severus-1.2.2/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `severus-1.2.1/PKG-INFO` & `severus-1.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: severus
-Version: 1.2.1
+Version: 1.2.2
 Summary: An internationalization engine designed with simplicity in mind
 Home-page: https://github.com/emmett-framework/severus
 License: BSD-3-Clause
 Keywords: internationalization
 Author: Giovanni Barillari
 Author-email: gi0baro@d4net.org
 Requires-Python: >=3.7,<4.0
@@ -14,20 +14,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Issue Tracker, https://github.com/emmett-framework/severus/issues
 Project-URL: Repository, https://github.com/emmett-framework/severus
 Description-Content-Type: text/markdown
```


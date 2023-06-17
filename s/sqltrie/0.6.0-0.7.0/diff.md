# Comparing `tmp/sqltrie-0.6.0.tar.gz` & `tmp/sqltrie-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqltrie-0.6.0.tar", last modified: Sun Jun 11 19:31:21 2023, max compression
+gzip compressed data, was "sqltrie-0.7.0.tar", last modified: Sat Jun 17 22:57:45 2023, max compression
```

## Comparing `sqltrie-0.6.0.tar` & `sqltrie-0.7.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.359420 sqltrie-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-11 19:30:58.000000 sqltrie-0.6.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 19:30:58.000000 sqltrie-0.6.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.351420 sqltrie-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-11 19:30:58.000000 sqltrie-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.351420 sqltrie-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-11 19:30:58.000000 sqltrie-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-11 19:30:58.000000 sqltrie-0.6.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-11 19:30:58.000000 sqltrie-0.6.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-11 19:30:58.000000 sqltrie-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-11 19:30:58.000000 sqltrie-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-11 19:30:58.000000 sqltrie-0.6.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-11 19:30:58.000000 sqltrie-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-11 19:30:58.000000 sqltrie-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-11 19:30:58.000000 sqltrie-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-11 19:31:21.359420 sqltrie-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-11 19:30:58.000000 sqltrie-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-11 19:30:58.000000 sqltrie-0.6.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-11 19:30:58.000000 sqltrie-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-11 19:31:21.359420 sqltrie-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.347419 sqltrie-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.351420 sqltrie-0.6.0/src/sqltrie/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.355419 sqltrie-0.6.0/src/sqltrie/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/__pyinstaller/hook-sqltrie.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/__pyinstaller/test_hook-sqltrie.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/pygtrie.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/serialized.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.355419 sqltrie-0.6.0/src/sqltrie/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/sqlite/diff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/sqlite/init.sql
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/sqlite/items.sql
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/sqlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/sqlite/steps.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-11 19:30:58.000000 sqltrie-0.6.0/src/sqltrie/trie.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.355419 sqltrie-0.6.0/src/sqltrie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-11 19:31:21.000000 sqltrie-0.6.0/src/sqltrie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-11 19:31:21.000000 sqltrie-0.6.0/src/sqltrie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:31:21.000000 sqltrie-0.6.0/src/sqltrie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-11 19:31:21.000000 sqltrie-0.6.0/src/sqltrie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:31:20.000000 sqltrie-0.6.0/src/sqltrie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-11 19:31:21.000000 sqltrie-0.6.0/src/sqltrie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 19:31:21.000000 sqltrie-0.6.0/src/sqltrie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.359420 sqltrie-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-11 19:30:58.000000 sqltrie-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:31:21.359420 sqltrie-0.6.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-11 19:30:58.000000 sqltrie-0.6.0/tests/benchmarks/test_sqltrie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-11 19:30:58.000000 sqltrie-0.6.0/tests/test_sqltrie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.518587 sqltrie-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-17 22:57:22.000000 sqltrie-0.7.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 22:57:22.000000 sqltrie-0.7.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.514587 sqltrie-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-17 22:57:22.000000 sqltrie-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.514587 sqltrie-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-17 22:57:22.000000 sqltrie-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-17 22:57:22.000000 sqltrie-0.7.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-17 22:57:22.000000 sqltrie-0.7.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-17 22:57:22.000000 sqltrie-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-17 22:57:22.000000 sqltrie-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-06-17 22:57:22.000000 sqltrie-0.7.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-17 22:57:22.000000 sqltrie-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-17 22:57:22.000000 sqltrie-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 22:57:22.000000 sqltrie-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-17 22:57:45.518587 sqltrie-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-17 22:57:22.000000 sqltrie-0.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-17 22:57:22.000000 sqltrie-0.7.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-17 22:57:22.000000 sqltrie-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-17 22:57:45.518587 sqltrie-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.514587 sqltrie-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.514587 sqltrie-0.7.0/src/sqltrie/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.518587 sqltrie-0.7.0/src/sqltrie/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/__pyinstaller/hook-sqltrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/__pyinstaller/test_hook-sqltrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/pygtrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/serialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.518587 sqltrie-0.7.0/src/sqltrie/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/sqlite/diff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/sqlite/init.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/sqlite/items.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/sqlite/steps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-17 22:57:22.000000 sqltrie-0.7.0/src/sqltrie/trie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.518587 sqltrie-0.7.0/src/sqltrie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-17 22:57:45.000000 sqltrie-0.7.0/src/sqltrie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-17 22:57:45.000000 sqltrie-0.7.0/src/sqltrie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:57:45.000000 sqltrie-0.7.0/src/sqltrie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-17 22:57:45.000000 sqltrie-0.7.0/src/sqltrie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:57:45.000000 sqltrie-0.7.0/src/sqltrie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-17 22:57:45.000000 sqltrie-0.7.0/src/sqltrie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 22:57:45.000000 sqltrie-0.7.0/src/sqltrie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.518587 sqltrie-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 22:57:22.000000 sqltrie-0.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:57:45.518587 sqltrie-0.7.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-17 22:57:22.000000 sqltrie-0.7.0/tests/benchmarks/test_sqltrie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-17 22:57:22.000000 sqltrie-0.7.0/tests/test_sqltrie.py
```

### Comparing `sqltrie-0.6.0/.cruft.json` & `sqltrie-0.7.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/.github/dependabot.yml` & `sqltrie-0.7.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/.github/workflows/release.yml` & `sqltrie-0.7.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/.github/workflows/tests.yml` & `sqltrie-0.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/.gitignore` & `sqltrie-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/.pre-commit-config.yaml` & `sqltrie-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/CODE_OF_CONDUCT.rst` & `sqltrie-0.7.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/CONTRIBUTING.rst` & `sqltrie-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/LICENSE` & `sqltrie-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/PKG-INFO` & `sqltrie-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqltrie
-Version: 0.6.0
+Version: 0.7.0
 Summary: SQL-based prefix tree inspired by pygtrie and python-diskcache
 Home-page: https://github.com/iterative/sqltrie
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Keywords: sqlite,sqlite3,sql,trie,prefix tree,data-science,diskcache
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqltrie-0.6.0/README.rst` & `sqltrie-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/noxfile.py` & `sqltrie-0.7.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/pyproject.toml` & `sqltrie-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/setup.cfg` & `sqltrie-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/src/sqltrie/__pyinstaller/test_hook-sqltrie.py` & `sqltrie-0.7.0/src/sqltrie/__pyinstaller/test_hook-sqltrie.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/src/sqltrie/pygtrie.py` & `sqltrie-0.7.0/src/sqltrie/pygtrie.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/src/sqltrie/serialized.py` & `sqltrie-0.7.0/src/sqltrie/serialized.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/src/sqltrie/sqlite/diff.sql` & `sqltrie-0.7.0/src/sqltrie/sqlite/diff.sql`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/src/sqltrie/sqlite/items.sql` & `sqltrie-0.7.0/src/sqltrie/sqlite/items.sql`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/src/sqltrie/sqlite/sqlite.py` & `sqltrie-0.7.0/src/sqltrie/sqlite/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,17 @@
             """
             UPDATE nodes SET has_value = 0, value = NULL WHERE id == ?
             """,
             (node["id"],),
         )
 
     def __len__(self):
-        self._conn.executescript(ITEMS_SQL.format(root=self._root_id, shallow=False))
+        self._conn.executescript(
+            ITEMS_SQL.format(root=self._root_id, shallow=int(False))
+        )
         return self._conn.execute(  # nosec
             f"""
             SELECT COUNT(*) AS count FROM {ITEMS_TABLE}
             """
         ).fetchone()["count"]
 
     def prefixes(self, key: TrieKey) -> Iterator[TrieStep]:
@@ -270,15 +272,15 @@
         pid = node["id"]
         has_value = node["has_value"]
         value = node["value"]
 
         if has_value:
             yield prefix, value
 
-        self._conn.executescript(ITEMS_SQL.format(root=pid, shallow=shallow))
+        self._conn.executescript(ITEMS_SQL.format(root=pid, shallow=int(shallow)))
         rows = self._conn.execute(f"SELECT * FROM {ITEMS_TABLE}")  # nosec
 
         yield from (((*prefix, *row["path"].split("/")), row["value"]) for row in rows)
 
     def clear(self):
         self._conn.execute("DELETE FROM nodes")
 
@@ -325,15 +327,15 @@
         old_id = self._get_node(old)["id"]
         new_id = self._get_node(new)["id"]
 
         self._conn.executescript(
             DIFF_SQL.format(
                 old_root=old_id,
                 new_root=new_id,
-                with_unchanged=with_unchanged,
+                with_unchanged=int(with_unchanged),
             )
         )
 
         rows = self._conn.execute(f"SELECT * FROM {DIFF_TABLE}")  # nosec
         yield from (
             Change(
                 row["type"],
```

### Comparing `sqltrie-0.6.0/src/sqltrie/sqlite/steps.sql` & `sqltrie-0.7.0/src/sqltrie/sqlite/steps.sql`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/src/sqltrie/trie.py` & `sqltrie-0.7.0/src/sqltrie/trie.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/src/sqltrie.egg-info/PKG-INFO` & `sqltrie-0.7.0/src/sqltrie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqltrie
-Version: 0.6.0
+Version: 0.7.0
 Summary: SQL-based prefix tree inspired by pygtrie and python-diskcache
 Home-page: https://github.com/iterative/sqltrie
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Keywords: sqlite,sqlite3,sql,trie,prefix tree,data-science,diskcache
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqltrie-0.6.0/src/sqltrie.egg-info/SOURCES.txt` & `sqltrie-0.7.0/src/sqltrie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/tests/benchmarks/test_sqltrie.py` & `sqltrie-0.7.0/tests/benchmarks/test_sqltrie.py`

 * *Files identical despite different names*

### Comparing `sqltrie-0.6.0/tests/test_sqltrie.py` & `sqltrie-0.7.0/tests/test_sqltrie.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 def test_set_get_root(cls):
     trie = cls()
 
     trie[()] = b"root"
     assert trie[()] == b"root"
     del trie[()]
     with pytest.raises(KeyError):
-        trie[()]
+        trie[()]  # pylint: disable=pointless-statement
 
 
 @pytest.mark.parametrize("cls", [SQLiteTrie, PyGTrie])
 def test_has_node(cls):
     trie = cls()
 
     trie[("foo", "bar")] = b"1"
```


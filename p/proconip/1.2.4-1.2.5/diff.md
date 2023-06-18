# Comparing `tmp/proconip-1.2.4.tar.gz` & `tmp/proconip-1.2.5.tar.gz`

## Comparing `proconip-1.2.4.tar` & `proconip-1.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.4/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.4/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.4/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.4/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.4/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.4/src/proconip/__init__.py
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 proconip-1.2.4/src/proconip/api.py
--rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.4/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.4/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.4/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.4/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.4/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.4/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.4/LICENSE
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.4/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.5/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.5/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.5/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.5/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.5/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.5/src/proconip/__init__.py
+-rw-r--r--   0        0        0    10015 2020-02-02 00:00:00.000000 proconip-1.2.5/src/proconip/api.py
+-rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.5/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.5/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.5/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.5/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.5/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.5/LICENSE
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.5/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.5/PKG-INFO
```

### Comparing `proconip-1.2.4/CODE_OF_CONDUCT.md` & `proconip-1.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/CONTRIBUTING.md` & `proconip-1.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/.github/workflows/pylint.yml` & `proconip-1.2.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/.github/workflows/python-publish.yml` & `proconip-1.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/.github/workflows/unittest.yml` & `proconip-1.2.5/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/src/proconip/api.py` & `proconip-1.2.5/src/proconip/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
             dosage_target=DosageTarget.PH_MINUS,
             dosage_duration=dosage_duration
         )
 
     async def async_ph_plus_dosage(
         self,
         dosage_duration: int,
-    ) -> None:
+    ) -> str:
         """Start manual pH plus dosage."""
         await async_start_dosage(
             client_session=self.client_session,
             config=self.config,
             dosage_target=DosageTarget.PH_PLUS,
             dosage_duration=dosage_duration
         )
```

### Comparing `proconip-1.2.4/src/proconip/definitions.py` & `proconip-1.2.5/src/proconip/definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/tests/helper.py` & `proconip-1.2.5/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/tests/test_definitions.py` & `proconip-1.2.5/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/.gitignore` & `proconip-1.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/LICENSE` & `proconip-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/README.md` & `proconip-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.4/pyproject.toml` & `proconip-1.2.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-1.2.4/PKG-INFO` & `proconip-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconip
-Version: 1.2.4
+Version: 1.2.5
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```


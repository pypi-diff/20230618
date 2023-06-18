# Comparing `tmp/berlin-0.3.7.tar.gz` & `tmp/berlin-0.3.8.tar.gz`

## Comparing `berlin-0.3.7.tar` & `berlin-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 berlin-0.3.7/Cargo.toml
--rw-r--r--   0     1001      123        7 2023-05-19 12:42:43.000000 berlin-0.3.7/.dockerignore
--rw-r--r--   0     1001      123     2833 2023-05-19 12:42:43.000000 berlin-0.3.7/.github/workflows/publish.yml
--rw-r--r--   0     1001      123      202 2023-05-19 12:42:43.000000 berlin-0.3.7/.github/workflows/python-static-ci.yml
--rw-r--r--   0     1001      123     1919 2023-05-19 12:42:43.000000 berlin-0.3.7/.github/workflows/rust-ci.yml
--rw-r--r--   0     1001      123       69 2023-05-19 12:42:43.000000 berlin-0.3.7/.gitignore
--rw-r--r--   0     1001      123      917 2023-05-19 12:42:43.000000 berlin-0.3.7/.gitlab-ci.yml
--rw-r--r--   0     1001      123      185 2023-05-19 12:42:43.000000 berlin-0.3.7/Dockerfile
--rw-r--r--   0     1001      123     2434 2023-05-19 12:42:43.000000 berlin-0.3.7/LICENSE.md
--rw-r--r--   0     1001      123      859 2023-05-19 12:42:43.000000 berlin-0.3.7/Makefile
--rw-r--r--   0     1001      123     4635 2023-05-19 12:42:43.000000 berlin-0.3.7/README.md
--rw-r--r--   0     1001      123       10 2023-05-19 12:44:30.000000 berlin-0.3.7/dist/berlin-0.3.7.tar.gz
--rw-r--r--   0     1001      123      695 2023-05-19 12:42:43.000000 berlin-0.3.7/pyproject.toml
--rw-r--r--   0     1001      123       97 2023-05-19 12:42:43.000000 berlin-0.3.7/python/berlin/__init__.py
--rw-r--r--   0     1001      123      307 2023-05-19 12:42:43.000000 berlin-0.3.7/python/berlin/_utils.py
--rw-r--r--   0     1001      123      155 2023-05-19 12:42:43.000000 berlin-0.3.7/scripts/test.py
--rw-r--r--   0     1001      123     7986 2023-05-19 12:42:43.000000 berlin-0.3.7/src/lib.rs
--rw-r--r--   0     1001      123      742 2023-05-19 12:42:43.000000 berlin-0.3.7/tests/conftest.py
--rw-r--r--   0     1001      123      480 2023-05-19 12:42:43.000000 berlin-0.3.7/tests/data/test-code-list.csv
--rw-r--r--   0     1001      123     3627 2023-05-19 12:42:43.000000 berlin-0.3.7/tests/data/test-codes.json
--rw-r--r--   0     1001      123      367 2023-05-19 12:42:43.000000 berlin-0.3.7/tests/test_berlin.py
--rw-r--r--   0     1001      123    24100 2023-05-19 12:42:43.000000 berlin-0.3.7/Cargo.lock
--rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 berlin-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 berlin-0.3.8/Cargo.toml
+-rw-r--r--   0     1001      123        7 2023-06-18 01:20:25.000000 berlin-0.3.8/.dockerignore
+-rw-r--r--   0     1001      123     2833 2023-06-18 01:20:25.000000 berlin-0.3.8/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123      202 2023-06-18 01:20:25.000000 berlin-0.3.8/.github/workflows/python-static-ci.yml
+-rw-r--r--   0     1001      123     1919 2023-06-18 01:20:25.000000 berlin-0.3.8/.github/workflows/rust-ci.yml
+-rw-r--r--   0     1001      123       69 2023-06-18 01:20:25.000000 berlin-0.3.8/.gitignore
+-rw-r--r--   0     1001      123      917 2023-06-18 01:20:25.000000 berlin-0.3.8/.gitlab-ci.yml
+-rw-r--r--   0     1001      123      185 2023-06-18 01:20:25.000000 berlin-0.3.8/Dockerfile
+-rw-r--r--   0     1001      123     2434 2023-06-18 01:20:25.000000 berlin-0.3.8/LICENSE.md
+-rw-r--r--   0     1001      123      859 2023-06-18 01:20:25.000000 berlin-0.3.8/Makefile
+-rw-r--r--   0     1001      123     4635 2023-06-18 01:20:25.000000 berlin-0.3.8/README.md
+-rw-r--r--   0     1001      123       10 2023-06-18 01:20:33.000000 berlin-0.3.8/dist/berlin-0.3.8.tar.gz
+-rw-r--r--   0     1001      123      695 2023-06-18 01:20:25.000000 berlin-0.3.8/pyproject.toml
+-rw-r--r--   0     1001      123      135 2023-06-18 01:20:25.000000 berlin-0.3.8/python/berlin/__init__.py
+-rw-r--r--   0     1001      123      307 2023-06-18 01:20:25.000000 berlin-0.3.8/python/berlin/_utils.py
+-rw-r--r--   0     1001      123      155 2023-06-18 01:20:25.000000 berlin-0.3.8/scripts/test.py
+-rw-r--r--   0     1001      123     8463 2023-06-18 01:20:25.000000 berlin-0.3.8/src/lib.rs
+-rw-r--r--   0     1001      123      742 2023-06-18 01:20:25.000000 berlin-0.3.8/tests/conftest.py
+-rw-r--r--   0     1001      123      480 2023-06-18 01:20:25.000000 berlin-0.3.8/tests/data/test-code-list.csv
+-rw-r--r--   0     1001      123     3627 2023-06-18 01:20:25.000000 berlin-0.3.8/tests/data/test-codes.json
+-rw-r--r--   0     1001      123      657 2023-06-18 01:20:25.000000 berlin-0.3.8/tests/test_berlin.py
+-rw-r--r--   0     1001      123    24100 2023-06-18 01:20:25.000000 berlin-0.3.8/Cargo.lock
+-rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 berlin-0.3.8/PKG-INFO
```

### Comparing `berlin-0.3.7/Cargo.toml` & `berlin-0.3.8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 name = "_berlin"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.18.3", features = ["extension-module"] }
 serde = { version = "1.0.133", features = ["derive"] }
 serde_json = "1.0.74"
-berlin-core = "0.2.1"
+berlin-core = "0.2.2"
 
 # Logging
 tracing = "0.1.29"
 tracing-futures = "0.2.5"
 tracing-log = "0.1.2"
 tracing-subscriber = "0.3.1"
 rayon = "1.7.0"
```

### Comparing `berlin-0.3.7/.github/workflows/publish.yml` & `berlin-0.3.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `berlin-0.3.7/.github/workflows/rust-ci.yml` & `berlin-0.3.8/.github/workflows/rust-ci.yml`

 * *Files identical despite different names*

### Comparing `berlin-0.3.7/.gitlab-ci.yml` & `berlin-0.3.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `berlin-0.3.7/LICENSE.md` & `berlin-0.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `berlin-0.3.7/Makefile` & `berlin-0.3.8/Makefile`

 * *Files identical despite different names*

### Comparing `berlin-0.3.7/README.md` & `berlin-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `berlin-0.3.7/pyproject.toml` & `berlin-0.3.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "berlin"
 authors = [
     {name = "Metin Akat", email = "metin.akat@flaxandteal.co.uk"},
     {name = "Phil Weir", email = "phil.weir@flaxandteal.co.uk"}
 ]
-version = "0.3.7"
+version = "0.3.8"
 description = "Identify locations and tag them with UN-LOCODEs and ISO-3166-2 subdivisions."
 readme = "README.md"
 license = {file = "LICENSE.md"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `berlin-0.3.7/src/lib.rs` & `berlin-0.3.8/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use std::collections::HashMap;
 use std::path::PathBuf;
 
-use pyo3::exceptions::PyTypeError;
+use pyo3::exceptions::{PyAttributeError, PyKeyError, PyTypeError};
 use pyo3::prelude::*;
 use rayon::iter::{
     IndexedParallelIterator, IntoParallelIterator, IntoParallelRefIterator, ParallelIterator,
 };
 
 use berlin_core::location::{CsvLocode, Location};
 use berlin_core::locations_db::{
@@ -14,21 +14,31 @@
 use berlin_core::search::SearchTerm;
 
 #[pyclass]
 struct LocationsDbProxy {
     _db: LocationsDb,
 }
 
-#[pyclass]
+#[pyclass(name = "Location")]
 struct LocationProxy {
     _loc: Location,
 }
 
 #[pymethods]
 impl LocationsDbProxy {
+    fn retrieve(&self, term: String) -> PyResult<LocationProxy> {
+        match self._db.retrieve(term.as_str()) {
+            Some(loc) => Python::with_gil(|_py| Ok(LocationProxy { _loc: loc })),
+            None => {
+                let err = PyKeyError::new_err(format!["{} not found", term.as_str()]);
+                Err(err)
+            }
+        }
+    }
+
     fn query(
         &self,
         query: String,
         limit: usize,
         lev_distance: u32,
         state: Option<String>,
     ) -> PyResult<Vec<LocationProxy>> {
@@ -64,15 +74,15 @@
                     ._loc
                     .words
                     .iter()
                     .map(|word| word.to_string())
                     .collect::<Vec<_>>()
                     .to_object(py),
                 _ => {
-                    let err = PyTypeError::new_err("AttributeError");
+                    let err = PyAttributeError::new_err(format!["{} not found", attr.as_str()]);
                     return Err(err);
                 }
             };
             Ok(val)
         });
         Ok(val.unwrap())
     }
@@ -228,11 +238,12 @@
     Ok(db_proxy)
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 #[pyo3(name = "_berlin")]
 fn berlin(_py: Python, m: &PyModule) -> PyResult<()> {
+    m.add_class::<LocationProxy>()?;
     m.add_function(wrap_pyfunction!(load, m)?)?;
     m.add_function(wrap_pyfunction!(load_from_json, m)?)?;
     Ok(())
 }
```

### Comparing `berlin-0.3.7/tests/conftest.py` & `berlin-0.3.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `berlin-0.3.7/tests/data/test-codes.json` & `berlin-0.3.8/tests/data/test-codes.json`

 * *Files identical despite different names*

### Comparing `berlin-0.3.7/Cargo.lock` & `berlin-0.3.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "berlin-core"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7cd9adfd3d711e1292aabfda7ebaf128b806e426d02815d49311dfb6d2d7cf7"
+checksum = "59971a182c17e7e3fce85b0be2a80b78a5fd77c35ae7057dca7af655ce8e3ab8"
 dependencies = [
  "ahash",
  "csv",
  "deunicode",
  "fst",
  "nom",
  "petgraph",
```

### Comparing `berlin-0.3.7/PKG-INFO` & `berlin-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin
-Version: 0.3.7
+Version: 0.3.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Summary: Identify locations and tag them with UN-LOCODEs and ISO-3166-2 subdivisions.
 Keywords: geospatial,nlp,search
 Author-email: Metin Akat <metin.akat@flaxandteal.co.uk>, Phil Weir <phil.weir@flaxandteal.co.uk>
```


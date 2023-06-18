# Comparing `tmp/tile_coder_rs-0.1.0.tar.gz` & `tmp/tile_coder_rs-0.3.1.tar.gz`

## Comparing `tile_coder_rs-0.1.0.tar` & `tile_coder_rs-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 tile_coder_rs-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2789 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123       35 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/.gitignore
--rw-r--r--   0     1001      123       10 2023-05-24 03:29:42.000000 tile_coder_rs-0.1.0/dist/tile_coder_rs-0.1.0.tar.gz
--rw-r--r--   0     1001      123      235 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123       56 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/requirements.txt
--rw-r--r--   0     1001      123     1760 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     3481 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/src/tc.rs
--rw-r--r--   0     1001      123      747 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/tests/perf.py
--rw-r--r--   0     1001      123     2590 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/tests/tc.py
--rw-r--r--   0     1001      123      473 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/tests/test.py
--rw-r--r--   0     1001      123       55 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/tile_coder_rs/__init__.py
--rw-r--r--   0     1001      123        0 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/tile_coder_rs/py.typed
--rw-r--r--   0     1001      123      218 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/tile_coder_rs/tile_coder_rs.pyi
--rw-r--r--   0     1001      123     9589 2023-05-24 03:27:55.000000 tile_coder_rs-0.1.0/Cargo.lock
--rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 tile_coder_rs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 tile_coder_rs-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      123     2789 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123       35 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/.gitignore
+-rw-r--r--   0     1001      123       10 2023-06-18 04:34:50.000000 tile_coder_rs-0.3.1/dist/tile_coder_rs-0.3.1.tar.gz
+-rw-r--r--   0     1001      123      235 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/pyproject.toml
+-rw-r--r--   0     1001      123       56 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/requirements.txt
+-rw-r--r--   0     1001      123     1760 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/src/lib.rs
+-rw-r--r--   0     1001      123     3469 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/src/tc.rs
+-rw-r--r--   0     1001      123      747 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tests/perf.py
+-rw-r--r--   0     1001      123     2590 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tests/tc.py
+-rw-r--r--   0     1001      123      473 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tests/test.py
+-rw-r--r--   0     1001      123       55 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tile_coder_rs/__init__.py
+-rw-r--r--   0     1001      123        0 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tile_coder_rs/py.typed
+-rw-r--r--   0     1001      123      187 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/tile_coder_rs/tile_coder_rs.pyi
+-rw-r--r--   0     1001      123     9589 2023-06-18 04:34:42.000000 tile_coder_rs-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0       57 1970-01-01 00:00:00.000000 tile_coder_rs-0.3.1/PKG-INFO
```

### Comparing `tile_coder_rs-0.1.0/.github/workflows/CI.yml` & `tile_coder_rs-0.3.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `tile_coder_rs-0.1.0/src/lib.rs` & `tile_coder_rs-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tile_coder_rs-0.1.0/src/tc.rs` & `tile_coder_rs-0.3.1/src/tc.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         let tiles = *tiles_per_dim.get(idx).expect("Index out-of-bounds");
 
         let axis = get_axis_cell(x, tiles);
         ind += axis * already_seen;
         already_seen *= tiles;
     }
 
-    ind.clamp(0, tiles_per_tiling - 1)
+    ind % tiles_per_tiling
 }
 
 pub fn get_tc_indices(dims: u32, tiles: &ArrayView1<u32>, tilings: u32, offsets: &ArrayView2<f64>, pos: &Array1<f64>) -> Array1<u32> {
     let tiles_per_tiling = tiles.product();
     let mut index = Array1::zeros(tilings as usize);
 
     for ntl in 0..tilings {
```

### Comparing `tile_coder_rs-0.1.0/tests/perf.py` & `tile_coder_rs-0.3.1/tests/perf.py`

 * *Files identical despite different names*

### Comparing `tile_coder_rs-0.1.0/tests/tc.py` & `tile_coder_rs-0.3.1/tests/tc.py`

 * *Files identical despite different names*

### Comparing `tile_coder_rs-0.1.0/Cargo.lock` & `tile_coder_rs-0.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tile-coder-rs"
-version = "0.1.0"
+version = "0.3.1"
 dependencies = [
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "unicode-ident"
```


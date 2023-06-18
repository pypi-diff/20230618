# Comparing `tmp/issue_db_api-0.9.3.tar.gz` & `tmp/issue_db_api-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.9.3.tar", last modified: Sun May 21 10:06:37 2023, max compression
+gzip compressed data, was "issue_db_api-0.9.4.tar", last modified: Tue May 23 13:09:20 2023, max compression
```

## Comparing `issue_db_api-0.9.3.tar` & `issue_db_api-0.9.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.9.3/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.382626 issue_db_api-0.9.3/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-21 10:01:40.000000 issue_db_api-0.9.3/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.9.3/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     9333 2023-05-21 09:55:20.000000 issue_db_api-0.9.3/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    47215 2023-05-21 10:01:27.000000 issue_db_api-0.9.3/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.9.3/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.9.3/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.9.3/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-12 10:30:49.000000 issue_db_api-0.9.3/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1622 2023-05-15 10:43:58.000000 issue_db_api-0.9.3/issue_db_api/src/files.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.9.3/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    41834 2023-05-15 11:58:40.000000 issue_db_api-0.9.3/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.9.3/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.9.3/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     7669 2023-05-15 11:58:40.000000 issue_db_api-0.9.3/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.9.3/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.9.3/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.382626 issue_db_api-0.9.3/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-21 10:06:37.000000 issue_db_api-0.9.3/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      774 2023-05-21 10:06:37.000000 issue_db_api-0.9.3/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-21 10:06:37.000000 issue_db_api-0.9.3/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.9.3/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-21 10:06:37.000000 issue_db_api-0.9.3/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-21 10:01:40.000000 issue_db_api-0.9.3/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-23 13:09:20.179716 issue_db_api-0.9.4/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.9.4/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.9.4/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.9.4/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-23 13:09:20.179716 issue_db_api-0.9.4/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.9.4/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-23 13:09:20.179716 issue_db_api-0.9.4/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-23 13:08:47.000000 issue_db_api-0.9.4/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.9.4/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     9333 2023-05-21 09:55:20.000000 issue_db_api-0.9.4/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-23 13:09:20.179716 issue_db_api-0.9.4/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    47368 2023-05-23 13:08:19.000000 issue_db_api-0.9.4/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.9.4/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.9.4/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.9.4/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-12 10:30:49.000000 issue_db_api-0.9.4/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1622 2023-05-15 10:43:58.000000 issue_db_api-0.9.4/issue_db_api/src/files.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.9.4/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.9.4/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41834 2023-05-15 11:58:40.000000 issue_db_api-0.9.4/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.9.4/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.9.4/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     7669 2023-05-15 11:58:40.000000 issue_db_api-0.9.4/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-23 13:09:20.179716 issue_db_api-0.9.4/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.9.4/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.9.4/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.9.4/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.9.4/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-23 13:09:20.179716 issue_db_api-0.9.4/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-23 13:09:20.000000 issue_db_api-0.9.4/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      774 2023-05-23 13:09:20.000000 issue_db_api-0.9.4/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-23 13:09:20.000000 issue_db_api-0.9.4/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.9.4/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-23 13:09:20.000000 issue_db_api-0.9.4/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-23 13:08:47.000000 issue_db_api-0.9.4/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-23 13:09:20.179716 issue_db_api-0.9.4/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.9.4/setup.py
```

### Comparing `issue_db_api-0.9.3/LICENSE` & `issue_db_api-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/PKG-INFO` & `issue_db_api-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.9.3
+Version: 0.9.4
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.9.3/issue_db_api/Cargo.toml` & `issue_db_api-0.9.4/issue_db_api/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.9.2"
+version = "0.9.3"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.9.3/issue_db_api/issue_api.pyi` & `issue_db_api-0.9.4/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/api_core.rs` & `issue_db_api-0.9.4/issue_db_api/src/api_core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -811,18 +811,22 @@
     pub(crate) fn create_embedding(&self,
                             name: String,
                             config: HashMap<String, Value>) -> APIResult<String> {
         let mut map = Map::new();
         map.insert("name".to_string(), Value::String(name));
         map.insert("config".to_string(),
                    Value::Object(Map::from_iter(config.into_iter())));
-        let result = self.call_endpoint_json::<_, String>(
+        #[derive(Debug, serde::Deserialize)]
+        struct NewEmbeddingResponse {
+            embedding_id: String
+        }
+        let result = self.call_endpoint_json::<_, NewEmbeddingResponse>(
             "embeddings", Verb::Post, Value::Object(map)
         )?;
-        Ok(result)
+        Ok(result.embedding_id)
     }
 
     pub(crate) fn get_embedding(&self, id: String) -> APIResult<UnboundEmbedding> {
         let endpoint = format!("embeddings/{}", id);
         self.call_endpoint_json::<_, UnboundEmbedding>(
             endpoint.as_str(), Verb::Get, Value::Object(Map::new())
         )
```

### Comparing `issue_db_api-0.9.3/issue_db_api/src/comments.rs` & `issue_db_api-0.9.4/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/config.rs` & `issue_db_api-0.9.4/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/embedding.rs` & `issue_db_api-0.9.4/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/errors.rs` & `issue_db_api-0.9.4/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/files.rs` & `issue_db_api-0.9.4/issue_db_api/src/files.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/issues.rs` & `issue_db_api-0.9.4/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/labels.rs` & `issue_db_api-0.9.4/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/lib.rs` & `issue_db_api-0.9.4/issue_db_api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/models.rs` & `issue_db_api-0.9.4/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/query.rs` & `issue_db_api-0.9.4/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/repository.rs` & `issue_db_api-0.9.4/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.9.4/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/tags.rs` & `issue_db_api-0.9.4/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api/src/util.rs` & `issue_db_api-0.9.4/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.9.4/issue_db_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.9.3
+Version: 0.9.4
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.9.3/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.9.4/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.3/pyproject.toml` & `issue_db_api-0.9.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.9.3"
+version = "0.9.4"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```


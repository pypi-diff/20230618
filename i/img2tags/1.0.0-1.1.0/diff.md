# Comparing `tmp/img2tags-1.0.0.tar.gz` & `tmp/img2tags-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img2tags-1.0.0.tar", max compression
+gzip compressed data, was "img2tags-1.1.0.tar", max compression
```

## Comparing `img2tags-1.0.0.tar` & `img2tags-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11342 2023-06-18 12:23:44.766767 img2tags-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      613 2023-06-18 12:23:44.766767 img2tags-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-18 12:23:44.766767 img2tags-1.0.0/img2tags/__init__.py
--rw-r--r--   0        0        0     7378 2023-06-18 12:23:44.766767 img2tags-1.0.0/img2tags/cli.py
--rw-r--r--   0        0        0     3085 2023-06-18 12:23:44.766767 img2tags-1.0.0/img2tags/tagger.py
--rw-r--r--   0        0        0     1318 2023-06-18 12:29:33.814331 img2tags-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1617 1970-01-01 00:00:00.000000 img2tags-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-18 12:23:44.766767 img2tags-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1788 2023-06-18 13:00:34.408478 img2tags-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 12:23:44.766767 img2tags-1.1.0/img2tags/__init__.py
+-rw-r--r--   0        0        0     7326 2023-06-18 12:59:53.016518 img2tags-1.1.0/img2tags/cli.py
+-rw-r--r--   0        0        0     3085 2023-06-18 12:23:44.766767 img2tags-1.1.0/img2tags/tagger.py
+-rw-r--r--   0        0        0     1318 2023-06-18 13:02:07.336388 img2tags-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 img2tags-1.1.0/PKG-INFO
```

### Comparing `img2tags-1.0.0/LICENSE.txt` & `img2tags-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2tags-1.0.0/img2tags/cli.py` & `img2tags-1.1.0/img2tags/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,23 +84,23 @@
 
     if path_out is None:
         path_out = path_in
     else:
         path_out.mkdir(exist_ok=True, parents=True)
 
     path_config: Path
-    session_infer_path = Path(path_or_name_model)
-    if session_infer_path.exists():
-        path_config = session_infer_path.joinpath("config.json")
-        session_infer_path = session_infer_path.joinpath("model.onnx")
+    path_model = Path(path_or_name_model)
+    if path_model.exists():
+        path_config = path_model.joinpath("config.json")
+        path_model = path_model.joinpath("model.onnx")
     else:
         items: list[str] = path_or_name_model.split("/")
         assert len(items) >= 2
         repo_id: str = "/".join(items[:2])
-        session_infer_path = hf_hub_download(
+        path_model = hf_hub_download(
             repo_id=repo_id,
             filename="/".join(items[2:]) + f"/{MODEL_FILE_NAME}",
         )
         path_config = Path(
             hf_hub_download(
                 repo_id=repo_id,
                 filename="/".join(items[2:]) + f"/{CONFIG_FILE_NAME}",
@@ -109,15 +109,15 @@
     config: ImageTaggerConfig = ImageTaggerConfig.parse_file(path_config)
 
     providers: list[str] = ["CPUExecutionProvider"]
     if not force_cpu and "CUDAExecutionProvider" in rt.get_available_providers():
         providers = ["CUDAExecutionProvider"]
 
     model: rt.InferenceSession = rt.InferenceSession(
-        session_infer_path,
+        path_model,
         providers=providers,
     )
 
     image_paths = list(glob_images(path_in, "**/*"))
 
     rconv = ResultConverter(path_or_name_model=path_or_name_model)
     is_json: bool = ext.lower() == "json"
@@ -215,15 +215,15 @@
         "--output",
         type=Path,
     )
     parser.add_argument(
         "--model",
         "-m",
         type=str,
-        default="shirayu/img2tags/SmilingWolf__wd-v1-4-moat-tagger-v2",
+        default="shirayu/img2tags/SmilingWolf__wd-v1-4-convnext-tagger-v2",
     )
     parser.add_argument(
         "--batch_size",
         type=int,
         default=1,
     )
     parser.add_argument(
```

### Comparing `img2tags-1.0.0/img2tags/tagger.py` & `img2tags-1.1.0/img2tags/tagger.py`

 * *Files identical despite different names*

### Comparing `img2tags-1.0.0/pyproject.toml` & `img2tags-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "img2tags"
-version = "1.0.0"
+version = "1.1.0"
 description = "Tag images"
 authors = ["Yuta Hayashibe <yuta@hayashibe.jp>"]
 readme = "README.md"
 homepage = "https://github.com/shirayu/img2tags"
 repository = "https://github.com/shirayu/img2tags"
 packages = [{include = "img2tags"}]
```

### Comparing `img2tags-1.0.0/PKG-INFO` & `img2tags-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2tags
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tag images
 Home-page: https://github.com/shirayu/img2tags
 Author: Yuta Hayashibe
 Author-email: yuta@hayashibe.jp
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -24,14 +24,26 @@
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/shirayu/img2tags
 Description-Content-Type: text/markdown
 
 
 # img2tags
 
+[![PyPI version](https://badge.fury.io/py/img2tags.svg)](https://badge.fury.io/py/img2tags)
+[![Python Versions](https://img.shields.io/pypi/pyversions/img2tags.svg)](https://pypi.org/project/img2tags/)
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Downloads](https://pepy.tech/badge/img2tags/week)](https://pepy.tech/project/img2tags)
+
+[![CI](https://github.com/shirayu/img2tags/actions/workflows/ci.yml/badge.svg)](https://github.com/shirayu/img2tags/actions/workflows/ci.yml)
+[![Typos](https://github.com/shirayu/img2tags/actions/workflows/typos.yml/badge.svg)](https://github.com/shirayu/img2tags/actions/workflows/typos.yml)
+
+Tag images by using onnxruntime.
+The current default model is the converted ``WD 1.4 ConvNext Tagger V2`` on <https://huggingface.co/shirayu/img2tags>.
+It works fine for anime images.
+
 ## Setup
 
 ```bash
 # For CPU
 pip install 'img2tags[cpu]'
 
 # For GPU
@@ -41,27 +53,30 @@
 ## Run
 
 ```bash
 # Generate .txt file
 img2tags -i input_dir
 
 # Generate .json file in another directory with CPU
-img2tags --model shirayu/img2tags/SmilingWolf__wd-v1-4-moat-tagger-v2 \
+img2tags --model shirayu/img2tags/SmilingWolf__wd-v1-4-convnext-tagger-v2 \
     --batch 4 \
     --ext json \
     --cpu \
     -i input_dir \
     -o output_dir
 ```
 
+The default threshold is used the values stored in ``config.json`` like [this](https://huggingface.co/shirayu/img2tags/blob/main/SmilingWolf__wd-v1-4-moat-tagger-v2/config.json).
+You can set the value in JSON format like ``--th {"0": 0.3, "4":0.2, "9":0.3}``.
+
 ## LICENSE
 
 Apache 2.0
 
 Some codes are based on codes in the following project.
 
 - <https://github.com/kohya-ss/sd-scripts>
 
 ## References
 
-- [Convert onnx models](https://github.com/onnx/onnx/issues/2182#issuecomment-881752539)
+- [Convert onnx models to change batch size](https://github.com/onnx/onnx/issues/2182#issuecomment-881752539)
```


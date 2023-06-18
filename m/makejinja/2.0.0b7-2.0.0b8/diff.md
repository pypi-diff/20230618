# Comparing `tmp/makejinja-2.0.0b7.tar.gz` & `tmp/makejinja-2.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makejinja-2.0.0b7.tar", max compression
+gzip compressed data, was "makejinja-2.0.0b8.tar", max compression
```

## Comparing `makejinja-2.0.0b7.tar` & `makejinja-2.0.0b8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/LICENSE
--rw-r--r--   0        0        0    16708 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/README.md
--rw-r--r--   0        0        0      101 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/__init__.py
--rw-r--r--   0        0        0       48 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/__main__.py
--rw-r--r--   0        0        0     6785 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/app.py
--rw-r--r--   0        0        0     1211 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/cli.py
--rw-r--r--   0        0        0    12243 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/config.py
--rw-r--r--   0        0        0     1060 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/loader.py
--rw-r--r--   0        0        0        0 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/py.typed
--rw-r--r--   0        0        0      813 2023-06-13 08:12:52.049161 makejinja-2.0.0b7/pyproject.toml
--rw-r--r--   0        0        0    17570 1970-01-01 00:00:00.000000 makejinja-2.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-13 09:18:32.642220 makejinja-2.0.0b8/LICENSE
+-rw-r--r--   0        0        0    17374 2023-06-13 09:18:32.642220 makejinja-2.0.0b8/README.md
+-rw-r--r--   0        0        0      101 2023-06-13 09:18:32.642220 makejinja-2.0.0b8/makejinja/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-13 09:18:32.642220 makejinja-2.0.0b8/makejinja/__main__.py
+-rw-r--r--   0        0        0     6872 2023-06-13 09:18:32.642220 makejinja-2.0.0b8/makejinja/app.py
+-rw-r--r--   0        0        0     1207 2023-06-13 09:18:32.646220 makejinja-2.0.0b8/makejinja/cli.py
+-rw-r--r--   0        0        0    12364 2023-06-13 09:18:32.646220 makejinja-2.0.0b8/makejinja/config.py
+-rw-r--r--   0        0        0     1060 2023-06-13 09:18:32.646220 makejinja-2.0.0b8/makejinja/loader.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:18:32.646220 makejinja-2.0.0b8/makejinja/py.typed
+-rw-r--r--   0        0        0      813 2023-06-13 09:19:27.122533 makejinja-2.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0    18236 1970-01-01 00:00:00.000000 makejinja-2.0.0b8/PKG-INFO
```

### Comparing `makejinja-2.0.0b7/LICENSE` & `makejinja-2.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `makejinja-2.0.0b7/README.md` & `makejinja-2.0.0b8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,41 +59,41 @@
 In its default configuration, makejinja searches the input folder recursively for files ending in `.jinja`.
 Also, we copy all contents (except raw template files) of the input folder to the output folder and remove the `.jinja` ending during the render process.
 To get an overview of the remaining options, we advise you to run `makejinja --help`:
 
 <!-- echo -e "\n```txt\n$(COLUMNS=120 poetry run makejinja --help)\n```" >> README.md -->
 
 ```txt
-
- Usage: makejinja [OPTIONS]
-
- makejinja can be used to automatically generate files from Jinja templates.
- Instead of passing CLI options, you can also write them to a file called .makejinja.toml in your working directory.
- Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual
- names. You will also find an example here: makejinja/tests/data/.makejinja.toml.
-
+                                                                                                                        
+ Usage: makejinja [OPTIONS]                                                                                             
+                                                                                                                        
+ makejinja can be used to automatically generate files from Jinja templates.                                            
+ Instead of passing CLI options, you can also write them to a file called makejinja.toml in your working directory.     
+ Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual 
+ names. You will also find an example here: makejinja/tests/data/makejinja.toml.                                        
+                                                                                                                        
 ╭─ Input/Output ───────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --input                DIRECTORY  Path to a folder containing template files. It is passed to Jinja's             │
 │                                      FileSystemLoader when creating the environment. Note: This option may be passed │
 │                                      multiple times to pass a list of values. If a template exists in multiple       │
 │                                      inputs, the last value with be used.                                            │
 │                                      [required]                                                                      │
 │ *  --output               DIRECTORY  Path to a folder where the rendered templates are stored. makejinja preserves   │
 │                                      the relative paths in the process, meaning that you can even use it on nested   │
 │                                      directories.                                                                    │
 │                                      [required]                                                                      │
-│    --input-pattern        TEXT       Glob pattern to search for files in input_folder. Accepts all pattern supported │
-│                                      by fnmatch. If a file is matched by this pattern and does not end with the      │
-│                                      specified jinja-suffix, it is copied over to the output_folder. Note: Do not    │
-│                                      add a special suffix used by your template files here, instead use the          │
-│                                      jinja-suffix option.                                                            │
+│    --include-pattern      TEXT       Glob patterns to search for files in inputs. Accepts all pattern supported by   │
+│                                      fnmatch. If a file is matched by this pattern and does not end with the         │
+│                                      specified jinja-suffix, it is copied over to the output_folder. Multiple can be │
+│                                      provided. Note: Do not add a special suffix used by your template files here,   │
+│                                      instead use the jinja-suffix option.                                            │
 │                                      [default: **/*]                                                                 │
 │    --exclude-pattern      TEXT       Glob patterns pattern to exclude files matched. Applied against files           │
-│                                      discovered by the input glob. Multiple can be provided.                         │
-│    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in input_folder │
+│                                      discovered through include_patterns. Multiple can be provided.                  │
+│    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in inputs       │
 │                                      matched by pattern are passed to the Jinja renderer. Note: Should be provided   │
 │                                      with the leading dot.                                                           │
 │                                      [default: .jinja]                                                               │
 │    --keep-jinja-suffix               Decide whether the specified jinja-suffix is removed from the file after        │
 │                                      rendering.                                                                      │
 │    --keep-empty                      Some Jinja template files may be empty after rendering (e.g., if they only      │
 │                                      contain macros that are imported by other templates). By default, we do not     │
@@ -151,10 +151,11 @@
 │                                     [default: }}]                                                                    │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Jinja Prefixes ─────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --prefix-line-statement    TEXT  If given and a string, this will be used as prefix for line based statements.       │
 │ --prefix-line-comment      TEXT  If given and a string, this will be used as prefix for line based comments.         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --help      Show this message and exit.                                                                              │
+│ --version      Show the version and exit.                                                                            │
+│ --help         Show this message and exit.                                                                           │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
```

### Comparing `makejinja-2.0.0b7/makejinja/app.py` & `makejinja-2.0.0b8/makejinja/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import shutil
 import sys
 import typing as t
 from inspect import signature
 from pathlib import Path
 
 import yaml
@@ -40,16 +41,18 @@
 
     for loader in config.loaders:
         process_loader(loader, env, data)
 
     rendered_files: set[Path] = set()
     rendered_folders: dict[Path, Path] = {}
 
-    for input_dir in config.inputs:
-        for input_path in sorted(input_dir.glob(config.input_pattern)):
+    for input_dir, include_pattern in itertools.product(
+        config.inputs, config.include_patterns
+    ):
+        for input_path in sorted(input_dir.glob(include_pattern)):
             relative_path = input_path.relative_to(input_dir)
             output_path = generate_output_path(config, relative_path)
 
             if any(input_path.match(x) for x in config.exclude_patterns):
                 print(f"Skip excluded '{input_path}'")
 
             elif input_path.is_file() and output_path not in rendered_files:
```

### Comparing `makejinja-2.0.0b7/makejinja/cli.py` & `makejinja-2.0.0b8/makejinja/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 __all__ = ["makejinja_cli"]
 
 click.rich_click.USE_MARKDOWN = True
 click.rich_click.OPTION_GROUPS = OPTION_GROUPS
 
 _loader = ts.default_loaders(
-    appname="makejinja", config_files=(Path(".makejinja.toml"),)
+    appname="makejinja", config_files=(Path("makejinja.toml"),)
 )
 
 
 @click.command("makejinja")
 @click.version_option()
 @ts.click_options(Config, _loader)
 def makejinja_cli(config: Config):
     """makejinja can be used to automatically generate files from [Jinja templates](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
-    Instead of passing CLI options, you can also write them to a file called `.makejinja.toml` in your working directory.
+    Instead of passing CLI options, you can also write them to a file called `makejinja.toml` in your working directory.
     **Note**: In this file, options may be named differently.
     Please refer to the file [`makejinja/config.py`](https://github.com/mirkolenz/makejinja/blob/main/makejinja/config.py) to see their actual names.
-    You will also find an example here: [`makejinja/tests/data/.makejinja.toml`](https://github.com/mirkolenz/makejinja/blob/main/tests/data/.makejinja.toml).
+    You will also find an example here: [`makejinja/tests/data/makejinja.toml`](https://github.com/mirkolenz/makejinja/blob/main/tests/data/makejinja.toml).
     """
 
     makejinja(config)
 
 
 if __name__ == "__main__":
     makejinja_cli()
```

### Comparing `makejinja-2.0.0b7/makejinja/config.py` & `makejinja-2.0.0b8/makejinja/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,36 +162,39 @@
     output: Path = ts.option(
         click={"type": click.Path(file_okay=False, writable=True, path_type=Path)},
         help="""
             Path to a folder where the rendered templates are stored.
             makejinja preserves the relative paths in the process, meaning that you can even use it on nested directories.
         """,
     )
-    input_pattern: str = ts.option(
-        default="**/*",
+    include_patterns: list[str] = ts.option(
+        factory=lambda: ["**/*"],
+        click={"param_decls": "--include-pattern"},
         help="""
-            Glob pattern to search for files in `input_folder`.
+            Glob patterns to search for files in `inputs`.
             Accepts all pattern supported by [`fnmatch`](https://docs.python.org/3/library/fnmatch.html#module-fnmatch).
             If a file is matched by this pattern and does not end with the specified `jinja-suffix`, it is copied over to the `output_folder`.
+            Multiple can be provided.
             **Note:** Do not add a special suffix used by your template files here, instead use the `jinja-suffix` option.
         """,
     )
     exclude_patterns: list[str] = ts.option(
         factory=list,
         click={"param_decls": "--exclude-pattern"},
         help="""
-            Glob patterns pattern to exclude files matched. Applied against files discovered by the input glob.
+            Glob patterns pattern to exclude files matched.
+            Applied against files discovered through `include_patterns`.
             Multiple can be provided.
         """,
     )
     jinja_suffix: str = ts.option(
         default=".jinja",
         help="""
             File ending of Jinja template files.
-            All files with this suffix in `input_folder` matched by `pattern` are passed to the Jinja renderer.
+            All files with this suffix in `inputs` matched by `pattern` are passed to the Jinja renderer.
             **Note:** Should be provided *with* the leading dot.
         """,
     )
     keep_jinja_suffix: bool = ts.option(
         default=False,
         click={"param_decls": "--keep-jinja-suffix"},
         help="""
@@ -274,15 +277,15 @@
 OPTION_GROUPS = {
     "makejinja": [
         {
             "name": "Input/Output",
             "options": [
                 "--input",
                 "--output",
-                "--input-pattern",
+                "--include-pattern",
                 "--exclude-pattern",
                 "--jinja-suffix",
                 "--keep-jinja-suffix",
                 "--keep-empty",
                 "--copy-metadata",
             ],
         },
```

### Comparing `makejinja-2.0.0b7/makejinja/loader.py` & `makejinja-2.0.0b8/makejinja/loader.py`

 * *Files identical despite different names*

### Comparing `makejinja-2.0.0b7/pyproject.toml` & `makejinja-2.0.0b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makejinja"
-version = "2.0.0b7"
+version = "2.0.0b8"
 description = "Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!"
 authors = ["Mirko Lenz <mirko@mirkolenz.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mirkolenz/makejinja"
 
 [tool.poetry.scripts]
```

### Comparing `makejinja-2.0.0b7/PKG-INFO` & `makejinja-2.0.0b8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makejinja
-Version: 2.0.0b7
+Version: 2.0.0b8
 Summary: Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!
 Home-page: https://github.com/mirkolenz/makejinja
 License: MIT
 Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -80,41 +80,41 @@
 In its default configuration, makejinja searches the input folder recursively for files ending in `.jinja`.
 Also, we copy all contents (except raw template files) of the input folder to the output folder and remove the `.jinja` ending during the render process.
 To get an overview of the remaining options, we advise you to run `makejinja --help`:
 
 <!-- echo -e "\n```txt\n$(COLUMNS=120 poetry run makejinja --help)\n```" >> README.md -->
 
 ```txt
-
- Usage: makejinja [OPTIONS]
-
- makejinja can be used to automatically generate files from Jinja templates.
- Instead of passing CLI options, you can also write them to a file called .makejinja.toml in your working directory.
- Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual
- names. You will also find an example here: makejinja/tests/data/.makejinja.toml.
-
+                                                                                                                        
+ Usage: makejinja [OPTIONS]                                                                                             
+                                                                                                                        
+ makejinja can be used to automatically generate files from Jinja templates.                                            
+ Instead of passing CLI options, you can also write them to a file called makejinja.toml in your working directory.     
+ Note: In this file, options may be named differently. Please refer to the file makejinja/config.py to see their actual 
+ names. You will also find an example here: makejinja/tests/data/makejinja.toml.                                        
+                                                                                                                        
 ╭─ Input/Output ───────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --input                DIRECTORY  Path to a folder containing template files. It is passed to Jinja's             │
 │                                      FileSystemLoader when creating the environment. Note: This option may be passed │
 │                                      multiple times to pass a list of values. If a template exists in multiple       │
 │                                      inputs, the last value with be used.                                            │
 │                                      [required]                                                                      │
 │ *  --output               DIRECTORY  Path to a folder where the rendered templates are stored. makejinja preserves   │
 │                                      the relative paths in the process, meaning that you can even use it on nested   │
 │                                      directories.                                                                    │
 │                                      [required]                                                                      │
-│    --input-pattern        TEXT       Glob pattern to search for files in input_folder. Accepts all pattern supported │
-│                                      by fnmatch. If a file is matched by this pattern and does not end with the      │
-│                                      specified jinja-suffix, it is copied over to the output_folder. Note: Do not    │
-│                                      add a special suffix used by your template files here, instead use the          │
-│                                      jinja-suffix option.                                                            │
+│    --include-pattern      TEXT       Glob patterns to search for files in inputs. Accepts all pattern supported by   │
+│                                      fnmatch. If a file is matched by this pattern and does not end with the         │
+│                                      specified jinja-suffix, it is copied over to the output_folder. Multiple can be │
+│                                      provided. Note: Do not add a special suffix used by your template files here,   │
+│                                      instead use the jinja-suffix option.                                            │
 │                                      [default: **/*]                                                                 │
 │    --exclude-pattern      TEXT       Glob patterns pattern to exclude files matched. Applied against files           │
-│                                      discovered by the input glob. Multiple can be provided.                         │
-│    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in input_folder │
+│                                      discovered through include_patterns. Multiple can be provided.                  │
+│    --jinja-suffix         TEXT       File ending of Jinja template files. All files with this suffix in inputs       │
 │                                      matched by pattern are passed to the Jinja renderer. Note: Should be provided   │
 │                                      with the leading dot.                                                           │
 │                                      [default: .jinja]                                                               │
 │    --keep-jinja-suffix               Decide whether the specified jinja-suffix is removed from the file after        │
 │                                      rendering.                                                                      │
 │    --keep-empty                      Some Jinja template files may be empty after rendering (e.g., if they only      │
 │                                      contain macros that are imported by other templates). By default, we do not     │
@@ -172,11 +172,12 @@
 │                                     [default: }}]                                                                    │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Jinja Prefixes ─────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --prefix-line-statement    TEXT  If given and a string, this will be used as prefix for line based statements.       │
 │ --prefix-line-comment      TEXT  If given and a string, this will be used as prefix for line based comments.         │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --help      Show this message and exit.                                                                              │
+│ --version      Show the version and exit.                                                                            │
+│ --help         Show this message and exit.                                                                           │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
```


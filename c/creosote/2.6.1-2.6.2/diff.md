# Comparing `tmp/creosote-2.6.1-py3-none-any.whl.zip` & `tmp/creosote-2.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14112 bytes, number of entries: 12
+Zip file size: 14224 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 creosote/__about__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 creosote/__init__.py
 -rw-r--r--  2.0 unx     6597 b- defN 20-Feb-02 00:00 creosote/cli.py
 -rw-r--r--  2.0 unx     1109 b- defN 20-Feb-02 00:00 creosote/formatters.py
 -rw-r--r--  2.0 unx      523 b- defN 20-Feb-02 00:00 creosote/models.py
--rw-r--r--  2.0 unx     8558 b- defN 20-Feb-02 00:00 creosote/parsers.py
+-rw-r--r--  2.0 unx     8488 b- defN 20-Feb-02 00:00 creosote/parsers.py
 -rw-r--r--  2.0 unx     9413 b- defN 20-Feb-02 00:00 creosote/resolvers.py
-?rw-r--r--  2.0 unx    13013 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      933 b- defN 20-Feb-02 00:00 creosote-2.6.1.dist-info/RECORD
-12 files, 41374 bytes uncompressed, 12554 bytes compressed:  69.7%
+?rw-r--r--  2.0 unx    13421 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      933 b- defN 20-Feb-02 00:00 creosote-2.6.2.dist-info/RECORD
+12 files, 41712 bytes uncompressed, 12666 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: creosote/parsers.py
 Comment: 
 
 Filename: creosote/resolvers.py
 Comment: 
 
-Filename: creosote-2.6.1.dist-info/METADATA
+Filename: creosote-2.6.2.dist-info/METADATA
 Comment: 
 
-Filename: creosote-2.6.1.dist-info/WHEEL
+Filename: creosote-2.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: creosote-2.6.1.dist-info/entry_points.txt
+Filename: creosote-2.6.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: creosote-2.6.1.dist-info/licenses/LICENSE
+Filename: creosote-2.6.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: creosote-2.6.1.dist-info/RECORD
+Filename: creosote-2.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## creosote/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "2.6.1"
+__version__ = "2.6.2"
```

## creosote/parsers.py

```diff
@@ -205,17 +205,16 @@
     for imp in imports_with_dupes_removed:
         logger.debug(f"- {imp}")
 
     return imports_with_dupes_removed
 
 
 def get_installed_dependency_names(venv: str) -> List[str]:
-    site_packages = Path(venv).glob("**/site-packages").__next__()
     dep_names = []
-    for path in site_packages.glob("**/*.dist-info"):
+    for path in Path(venv).glob("**/*.dist-info"):
         dep_names.append(path.name.split("-")[0])
     return dep_names
 
 
 def get_excluded_deps_which_are_not_installed(
     excluded_deps: List[str], venvs: List[str]
 ) -> List[str]:
```

## Comparing `creosote-2.6.1.dist-info/METADATA` & `creosote-2.6.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creosote
-Version: 2.6.1
+Version: 2.6.2
 Summary: Identify unused dependencies and avoid a bloated virtual environment.
 Project-URL: Source, https://github.com/fredrikaverpil/creosote
 Project-URL: Tracker, https://github.com/fredrikaverpil/creosote/issues
 Author-email: Fredrik Averpil <fredrik.averpil@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -112,25 +112,33 @@
 
 ## 🤨 FAQ
 
 ### Which dependency specification tooling/standards are supported?
 
 | Tool/standard                                                                                                               | Supported | `--deps-file` value | Example `--sections` values                                                                                         |
 | --------------------------------------------------------------------------------------------------------------------------- | :-------: | ------------------- | ------------------------------------------------------------------------------------------------------------------- |
-| [PDM](https://pdm.fming.dev/latest/)                                                                                        |     ✅     | `pyproject.toml`    | `project.dependencies`,<br>`project.optional-dependencies.<GROUP>`,<br>`tool.pdm.dev-dependencies`                  |
+| [PDM](https://pdm.fming.dev/latest/) and [PEP-582](https://peps.python.org/pep-0582/)                                                                                        |     ✅     | `pyproject.toml`    | `project.dependencies`,<br>`project.optional-dependencies.<GROUP>`,<br>`tool.pdm.dev-dependencies`                  |
 | [Pipenv](https://pipenv.pypa.io/en/latest/)                                                                                 |     ✅     | `pyproject.toml`    | `packages`,<br>`dev-packages`                                                                                       |
 | [Poetry](https://python-poetry.org/)                                                                                        |     ✅     | `pyproject.toml`    | `tool.poetry.dependencies`,<br>`tool.poetry.dev-dependencies` (legacy),<br>`tool.poetry.group.<GROUP>.dependencies` |
 | Legacy Setuptools (`setup.py`)                                                                                              |     ❌     |                     |                                                                                                                     |
 | [PEP-508](https://peps.python.org/pep-0508/) (`requirements.txt`, [pip-tools](https://pip-tools.readthedocs.io/en/latest/)) |     ✅     | `*.[txt\|in]`       | N/A                                                                                                                 |
 | [PEP-621](https://peps.python.org/pep-0621/)                                                                                |     ✅     | `pyproject.toml`    | `project.dependencies`,<br>`project.optional-dependencies.<GROUP>`                                                  |
 
 #### 📔 Notes on [PEP-508](https://peps.python.org/pep-0508) (`requirements.txt`)
 
 When using `requirements.txt` files to specify dependencies, there is no way to tell which part of `requirements.txt` specifies production vs developer dependencies. Therefore, you have to break your `requirements.txt` file into e.g. `requirements-prod.txt` and `requirements-dev.txt` and use any of them as input. When using [pip-tools](https://pip-tools.readthedocs.io/en/latest/), you likely want to point Creosote to scan your `*.in` file(s).
 
+#### 📓 Notes on [PEP-582](https://peps.python.org/pep-0582/) (`__pypackages__`)
+
+Creosote supports the `__pypackages__` folder, although PEP-582 was rejected. There is no reason to remove support for this today, but in case supporting this becomes cumbersome in the future, supporting PEP-582 might be dropped.
+
+```bash
+creosote --venv __pypackages__
+```
+
 ### Can I specify multiple toml sections?
 
 Yes, you can specify a list of sections after the `--sections` argument. It all depends on what your setup looks like and what you set out to achieve.
 
 ```bash
 $ creosote --sections project.dependencies project.optional-dependencies.lint project.optional-dependencies.test
 ```
```

## Comparing `creosote-2.6.1.dist-info/licenses/LICENSE` & `creosote-2.6.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*


# Comparing `tmp/theme-material-darcula-1.0.4.tar.gz` & `tmp/theme-material-darcula-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theme-material-darcula-1.0.4.tar", last modified: Mon Feb 20 17:12:05 2023, max compression
+gzip compressed data, was "theme-material-darcula-1.0.5.tar", last modified: Sun Jun 18 14:10:13 2023, max compression
```

## Comparing `theme-material-darcula-1.0.4.tar` & `theme-material-darcula-1.0.5.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.432465 theme-material-darcula-1.0.4/
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     1528 2022-06-15 01:18:09.000000 theme-material-darcula-1.0.4/LICENSE
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      441 2022-06-15 01:18:48.000000 theme-material-darcula-1.0.4/MANIFEST.in
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     3075 2023-02-20 17:12:05.432106 theme-material-darcula-1.0.4/PKG-INFO
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     2268 2023-02-20 17:03:58.000000 theme-material-darcula-1.0.4/README.md
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      205 2022-06-15 01:17:39.000000 theme-material-darcula-1.0.4/install.json
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     2418 2023-02-20 17:05:41.000000 theme-material-darcula-1.0.4/package.json
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      147 2022-11-20 08:02:05.000000 theme-material-darcula-1.0.4/pyproject.toml
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)       38 2023-02-20 17:12:05.432608 theme-material-darcula-1.0.4/setup.cfg
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     2575 2022-11-24 09:26:55.000000 theme-material-darcula-1.0.4/setup.py
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.418917 theme-material-darcula-1.0.4/src/
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      827 2022-06-15 01:25:29.000000 theme-material-darcula-1.0.4/src/index.ts
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.424002 theme-material-darcula-1.0.4/style/
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     3830 2023-01-03 08:26:44.000000 theme-material-darcula-1.0.4/style/base.css
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     2771 2022-06-15 01:15:40.000000 theme-material-darcula-1.0.4/style/codemirror-darcula.css
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      596 2022-07-14 16:32:11.000000 theme-material-darcula-1.0.4/style/index.css
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     2595 2022-06-15 01:15:40.000000 theme-material-darcula-1.0.4/style/scrollbars.css
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     2300 2022-11-22 13:12:30.000000 theme-material-darcula-1.0.4/style/tabs.css
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)    18646 2022-11-20 06:21:33.000000 theme-material-darcula-1.0.4/style/variables.css
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.425197 theme-material-darcula-1.0.4/theme-material-darcula/
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      324 2022-06-15 01:04:46.000000 theme-material-darcula-1.0.4/theme-material-darcula/__init__.py
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      458 2022-06-15 01:04:46.000000 theme-material-darcula-1.0.4/theme-material-darcula/_version.py
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.425677 theme-material-darcula-1.0.4/theme-material-darcula/labextension/
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     2534 2023-02-20 17:12:03.000000 theme-material-darcula-1.0.4/theme-material-darcula/labextension/package.json
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.427492 theme-material-darcula-1.0.4/theme-material-darcula/labextension/static/
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      499 2023-02-20 17:12:03.000000 theme-material-darcula-1.0.4/theme-material-darcula/labextension/static/568.42f66d09bcb7adc081da.js
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     6053 2023-02-20 17:12:03.000000 theme-material-darcula-1.0.4/theme-material-darcula/labextension/static/remoteEntry.07b544582ccd32c2f8af.js
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      118 2023-02-20 17:12:03.000000 theme-material-darcula-1.0.4/theme-material-darcula/labextension/static/style.js
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)       20 2023-02-20 17:12:03.000000 theme-material-darcula-1.0.4/theme-material-darcula/labextension/static/third-party-licenses.json
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.412563 theme-material-darcula-1.0.4/theme-material-darcula/labextension/themes/
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.412794 theme-material-darcula-1.0.4/theme-material-darcula/labextension/themes/@adhadse/
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.428407 theme-material-darcula-1.0.4/theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)    28040 2023-02-20 17:12:03.000000 theme-material-darcula-1.0.4/theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/index.css
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:03.000000 theme-material-darcula-1.0.4/theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/index.js
-drwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        0 2023-02-20 17:12:05.430965 theme-material-darcula-1.0.4/theme_material_darcula.egg-info/
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     3075 2023-02-20 17:12:05.000000 theme-material-darcula-1.0.4/theme_material_darcula.egg-info/PKG-INFO
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)     1055 2023-02-20 17:12:05.000000 theme-material-darcula-1.0.4/theme_material_darcula.egg-info/SOURCES.txt
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        1 2023-02-20 17:12:05.000000 theme-material-darcula-1.0.4/theme_material_darcula.egg-info/dependency_links.txt
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)        1 2022-07-13 13:41:28.000000 theme-material-darcula-1.0.4/theme_material_darcula.egg-info/not-zip-safe
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)       18 2023-02-20 17:12:05.000000 theme-material-darcula-1.0.4/theme_material_darcula.egg-info/requires.txt
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)       23 2023-02-20 17:12:05.000000 theme-material-darcula-1.0.4/theme_material_darcula.egg-info/top_level.txt
--rwxrwxrwx   0 nfsnobody (65534) nfsnobody (65534)      520 2022-06-15 01:04:46.000000 theme-material-darcula-1.0.4/tsconfig.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.834679 theme-material-darcula-1.0.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1528 2022-06-15 01:18:09.000000 theme-material-darcula-1.0.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      441 2022-06-15 01:18:48.000000 theme-material-darcula-1.0.5/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     3075 2023-06-18 14:10:13.834284 theme-material-darcula-1.0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2268 2023-02-20 17:03:58.000000 theme-material-darcula-1.0.5/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      205 2022-06-15 01:17:39.000000 theme-material-darcula-1.0.5/install.json
+-rwxrwxrwx   0 root         (0) root         (0)     2418 2023-06-18 12:14:25.000000 theme-material-darcula-1.0.5/package.json
+-rwxrwxrwx   0 root         (0) root         (0)      147 2022-11-20 08:02:05.000000 theme-material-darcula-1.0.5/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-18 14:10:13.834814 theme-material-darcula-1.0.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2529 2023-06-18 12:06:34.000000 theme-material-darcula-1.0.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.822809 theme-material-darcula-1.0.5/src/
+-rwxrwxrwx   0 root         (0) root         (0)      827 2022-06-15 01:25:29.000000 theme-material-darcula-1.0.5/src/index.ts
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.825810 theme-material-darcula-1.0.5/style/
+-rwxrwxrwx   0 root         (0) root         (0)     3830 2023-01-03 08:26:44.000000 theme-material-darcula-1.0.5/style/base.css
+-rwxrwxrwx   0 root         (0) root         (0)     2771 2022-06-15 01:15:40.000000 theme-material-darcula-1.0.5/style/codemirror-darcula.css
+-rwxrwxrwx   0 root         (0) root         (0)      596 2022-07-14 16:32:11.000000 theme-material-darcula-1.0.5/style/index.css
+-rwxrwxrwx   0 root         (0) root         (0)     2595 2022-06-15 01:15:40.000000 theme-material-darcula-1.0.5/style/scrollbars.css
+-rwxrwxrwx   0 root         (0) root         (0)     2300 2022-11-22 13:12:30.000000 theme-material-darcula-1.0.5/style/tabs.css
+-rwxrwxrwx   0 root         (0) root         (0)    18646 2022-11-20 06:21:33.000000 theme-material-darcula-1.0.5/style/variables.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.826978 theme-material-darcula-1.0.5/theme-material-darcula/
+-rwxrwxrwx   0 root         (0) root         (0)      324 2022-06-15 01:04:46.000000 theme-material-darcula-1.0.5/theme-material-darcula/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      458 2022-06-15 01:04:46.000000 theme-material-darcula-1.0.5/theme-material-darcula/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.827510 theme-material-darcula-1.0.5/theme-material-darcula/labextension/
+-rwxrwxrwx   0 root         (0) root         (0)     2534 2023-06-18 14:10:11.000000 theme-material-darcula-1.0.5/theme-material-darcula/labextension/package.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.829705 theme-material-darcula-1.0.5/theme-material-darcula/labextension/static/
+-rwxrwxrwx   0 root         (0) root         (0)      499 2023-06-18 14:10:11.000000 theme-material-darcula-1.0.5/theme-material-darcula/labextension/static/568.42f66d09bcb7adc081da.js
+-rwxrwxrwx   0 root         (0) root         (0)     6053 2023-06-18 14:10:11.000000 theme-material-darcula-1.0.5/theme-material-darcula/labextension/static/remoteEntry.29639ad0c8cd91440625.js
+-rwxrwxrwx   0 root         (0) root         (0)      118 2023-06-18 14:10:10.000000 theme-material-darcula-1.0.5/theme-material-darcula/labextension/static/style.js
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-06-18 14:10:11.000000 theme-material-darcula-1.0.5/theme-material-darcula/labextension/static/third-party-licenses.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.818123 theme-material-darcula-1.0.5/theme-material-darcula/labextension/themes/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.818211 theme-material-darcula-1.0.5/theme-material-darcula/labextension/themes/@adhadse/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.830935 theme-material-darcula-1.0.5/theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/
+-rwxrwxrwx   0 root         (0) root         (0)    28040 2023-06-18 14:10:11.000000 theme-material-darcula-1.0.5/theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/index.css
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:11.000000 theme-material-darcula-1.0.5/theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/index.js
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 14:10:13.833614 theme-material-darcula-1.0.5/theme_material_darcula.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3075 2023-06-18 14:10:13.000000 theme-material-darcula-1.0.5/theme_material_darcula.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1010 2023-06-18 14:10:13.000000 theme-material-darcula-1.0.5/theme_material_darcula.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-18 14:10:13.000000 theme-material-darcula-1.0.5/theme_material_darcula.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-06-18 14:10:13.000000 theme-material-darcula-1.0.5/theme_material_darcula.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       23 2023-06-18 14:10:13.000000 theme-material-darcula-1.0.5/theme_material_darcula.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      520 2022-06-15 01:04:46.000000 theme-material-darcula-1.0.5/tsconfig.json
```

### Comparing `theme-material-darcula-1.0.4/LICENSE` & `theme-material-darcula-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/PKG-INFO` & `theme-material-darcula-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theme-material-darcula
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Jupyterlab theme inspired by JetBrains IDE's Darcula scheme and Material Design.
 Home-page: https://github.com/adhadse/theme-material-darcula
 Author: Anurag Dhadse
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `theme-material-darcula-1.0.4/README.md` & `theme-material-darcula-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/package.json` & `theme-material-darcula-1.0.5/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'1.0.5'"}*

```diff
@@ -60,9 +60,9 @@
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "1.0.4"
+    "version": "1.0.5"
 }
```

### Comparing `theme-material-darcula-1.0.4/setup.py` & `theme-material-darcula-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,83 @@
 """
 theme-material-darcula setup
 """
 import json
-from pathlib import Path
-# import conda_build.bdist_conda
+import os	
 
 
 from jupyter_packaging import (
     create_cmdclass, 
     install_npm, 
     ensure_targets,
     combine_commands,
     skip_if_exists
 )
 import setuptools
 
-HERE = Path(__file__).parent.resolve()
+HERE = os.path.abspath(os.path.dirname(__file__))
 
 # The name of the project
 name = "theme-material-darcula"
 
 # Get our version
-with (HERE / "package.json").open() as f:
+with open(os.path.join(HERE, 'package.json')) as f:
     version = json.load(f)['version']
 
-lab_path = HERE / name / "labextension"
+lab_path = os.path.join(HERE, name, "labextension")	
 
 # Representative files that should exist after a successful build
 jstargets = [
-    str(HERE / "lib" / "index.js"),
-    str(lab_path / "package.json"),
+    os.path.join(HERE, "lib", "index.js"),	
+    os.path.join(lab_path, "package.json"),
 ]
 
 package_data_spec = {
     name: [
         "*"
     ]
 }
 
 labext_name = "@adhadse/theme-material-darcula"
 
 data_files_spec = [
-    ("share/jupyter/labextensions/%s" % labext_name, str(lab_path), "**"),
-    ("share/jupyter/labextensions/%s" % labext_name, str(HERE), "install.json"),
+    ("share/jupyter/labextensions/%s" % labext_name, lab_path, "**"),
+    ("share/jupyter/labextensions/%s" % labext_name, HERE, "install.json"),
 ]
 
 cmdclass = create_cmdclass(
     "jsdeps",
     package_data_spec=package_data_spec,
     data_files_spec=data_files_spec
 )
 
-js_command = combine_commands(
+cmdclass["jsdeps"] = combine_commands(
     install_npm(HERE, build_cmd="build:prod", npm=["jlpm"]),
     ensure_targets(jstargets),
 )
 
-is_repo = (HERE / ".git").exists()
-if is_repo:
-    cmdclass["jsdeps"] = js_command
-else:
-    cmdclass["jsdeps"] = skip_if_exists(jstargets, js_command)
+# is_repo = (HERE / ".git").exists()
+# if is_repo:
+#     cmdclass["jsdeps"] = js_command
+# else:
+#     cmdclass["jsdeps"] = skip_if_exists(jstargets, js_command)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_args = dict(
     name=name,
     version=version,
     url="https://github.com/adhadse/theme-material-darcula",
     author="Anurag Dhadse",
     description="A Jupyterlab theme inspired by JetBrains IDE's Darcula scheme and Material Design.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     cmdclass=cmdclass,
-    zip_safe=False,
-    # distclass=conda_build.bdist_conda.CondaDistribution,
+    # zip_safe=False,
     packages=setuptools.find_packages(),
     install_requires=[
         "jupyterlab>=3.0.0"
     ],
     include_package_data=True,
     python_requires=">=3.6",
     license="BSD-3-Clause",
```

### Comparing `theme-material-darcula-1.0.4/src/index.ts` & `theme-material-darcula-1.0.5/src/index.ts`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/style/base.css` & `theme-material-darcula-1.0.5/style/base.css`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/style/codemirror-darcula.css` & `theme-material-darcula-1.0.5/style/codemirror-darcula.css`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/style/index.css` & `theme-material-darcula-1.0.5/style/index.css`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/style/scrollbars.css` & `theme-material-darcula-1.0.5/style/scrollbars.css`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/style/tabs.css` & `theme-material-darcula-1.0.5/style/tabs.css`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/style/variables.css` & `theme-material-darcula-1.0.5/style/variables.css`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/theme-material-darcula/labextension/package.json` & `theme-material-darcula-1.0.5/theme-material-darcula/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9696691176470589%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.29639ad0c8cd91440625.js'}}",*

 * * "'version'": "'1.0.5'"}*

```diff
@@ -24,15 +24,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/adhadse/theme-material-darcula",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.07b544582ccd32c2f8af.js"
+            "load": "static/remoteEntry.29639ad0c8cd91440625.js"
         },
         "extension": true,
         "outputDir": "theme-material-darcula/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
@@ -64,9 +64,9 @@
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "1.0.4"
+    "version": "1.0.5"
 }
```

### Comparing `theme-material-darcula-1.0.4/theme-material-darcula/labextension/static/remoteEntry.07b544582ccd32c2f8af.js` & `theme-material-darcula-1.0.5/theme-material-darcula/labextension/static/remoteEntry.29639ad0c8cd91440625.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -87,15 +87,15 @@
                     var n = o[e] = o[e] || {},
                         u = n[r];
                     (!u || !u.loaded && (1 != !u.eager ? a : i > u.from)) && (n[r] = {
                         get: () => g.e(568).then((() => () => g(568))),
                         from: i,
                         eager: !1
                     })
-                })("@adhadse/theme-material-darcula", "1.0.4"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@adhadse/theme-material-darcula", "1.0.5"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `theme-material-darcula-1.0.4/theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/index.css` & `theme-material-darcula-1.0.5/theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/index.css`

 * *Files identical despite different names*

### Comparing `theme-material-darcula-1.0.4/theme_material_darcula.egg-info/PKG-INFO` & `theme-material-darcula-1.0.5/theme_material_darcula.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theme-material-darcula
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Jupyterlab theme inspired by JetBrains IDE's Darcula scheme and Material Design.
 Home-page: https://github.com/adhadse/theme-material-darcula
 Author: Anurag Dhadse
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `theme-material-darcula-1.0.4/theme_material_darcula.egg-info/SOURCES.txt` & `theme-material-darcula-1.0.5/theme_material_darcula.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 style/scrollbars.css
 style/tabs.css
 style/variables.css
 theme-material-darcula/__init__.py
 theme-material-darcula/_version.py
 theme-material-darcula/labextension/package.json
 theme-material-darcula/labextension/static/568.42f66d09bcb7adc081da.js
-theme-material-darcula/labextension/static/remoteEntry.07b544582ccd32c2f8af.js
+theme-material-darcula/labextension/static/remoteEntry.29639ad0c8cd91440625.js
 theme-material-darcula/labextension/static/style.js
 theme-material-darcula/labextension/static/third-party-licenses.json
 theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/index.css
 theme-material-darcula/labextension/themes/@adhadse/theme-material-darcula/index.js
 theme_material_darcula.egg-info/PKG-INFO
 theme_material_darcula.egg-info/SOURCES.txt
 theme_material_darcula.egg-info/dependency_links.txt
-theme_material_darcula.egg-info/not-zip-safe
 theme_material_darcula.egg-info/requires.txt
 theme_material_darcula.egg-info/top_level.txt
```

### Comparing `theme-material-darcula-1.0.4/tsconfig.json` & `theme-material-darcula-1.0.5/tsconfig.json`

 * *Files identical despite different names*


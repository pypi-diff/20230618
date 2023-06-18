# Comparing `tmp/pyvolsuggester-1.0.0.tar.gz` & `tmp/pyvolsuggester-1.0.1.tar.gz`

## Comparing `pyvolsuggester-1.0.0.tar` & `pyvolsuggester-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/License.txt
--rw-r--r--   0        0        0     9597 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/README.md
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/License.txt
+-rw-r--r--   0        0        0     9989 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/README.md
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/PKG-INFO
```

### Comparing `pyvolsuggester-1.0.0/License.txt` & `pyvolsuggester-1.0.1/License.txt`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-1.0.0/README.md` & `pyvolsuggester-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## ✔ PyVolSuggester Package
 - A Python package to provide suggestion on volume at which the music audio file needs to be played for better experience and feeling.
 - In backend, it extracts various generic features for particular audio and analyze among them and provide feedback on volumne on it.  
-- This tools helps in maintaining goob vibes along the music playout.
+- This tools helps in maintaining good vibes along the music playout.
 
 <p align = "center">
 	<img src = "https://img.shields.io/badge/Pypi Package-PyVolSuggester-green?style=plastic&logo=appveyor", alt = "PyVolSuggester">
 	<img src = "https://img.shields.io/badge/PyPi-Python Package Index-green?style=plastic&logo=appveyor", alt = "PyPi">
 </p>
 <p align = "center">
 	<img src = "https://img.shields.io/github/stars/akash-rajak/PyVolSuggester?style=social", alt = "GitHub Repo stars">
@@ -191,15 +191,21 @@
 pip install PyVolSuggester
 ```
 
 ****
 
 
 ### 🌟Stargazers Over Time:
+[![Stargazers repo roster for @akash-rajak/PyVolSuggester](https://reporoster.com/stars/akash-rajak/PyVolSuggester)](https://github.com/akash-rajak/PyVolSuggester/stargazers)
 [![Stargazers over time](https://starchart.cc/akash-rajak/PyVolSuggester.svg)](https://starchart.cc/akash-rajak/PyVolSuggester)
 
 ****
 
+### 🌟Forkers Over Time:
+[![Forkers repo roster for @akash-rajak/PyVolSuggester](https://reporoster.com/forks/akash-rajak/PyVolSuggester)](https://github.com/akash-rajak/PyVolSuggester/network/members)
+
+****
+
 ### 📌Contributors:
 <a href="https://github.com/akash-rajak/PyVolSuggester/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=akash-rajak/PyVolSuggester" />
 </a>
```

### Comparing `pyvolsuggester-1.0.0/pyproject.toml` & `pyvolsuggester-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 name = "PyVolSuggester"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.0"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
+version = "1.0.1"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is an optional longer description of your project that represents
```

### Comparing `pyvolsuggester-1.0.0/PKG-INFO` & `pyvolsuggester-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVolSuggester
-Version: 1.0.0
+Version: 1.0.1
 Summary: Does audio feature extraction and suggest the feasible volumne for better feeling and experience.
 Project-URL: Homepage, https://github.com/akash-rajak/PyVolSuggester
 Project-URL: Bug Reports, https://github.com/akash-rajak/PyVolSuggester/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Source, https://github.com/akash-rajak/PyVolSuggester
 Author-email: Akash Rajak <aakashrajak02@gmail.com>
 Maintainer-email: Akash Rajak <aakashrajak02@gmail.com>
@@ -43,15 +43,15 @@
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## ✔ PyVolSuggester Package
 - A Python package to provide suggestion on volume at which the music audio file needs to be played for better experience and feeling.
 - In backend, it extracts various generic features for particular audio and analyze among them and provide feedback on volumne on it.  
-- This tools helps in maintaining goob vibes along the music playout.
+- This tools helps in maintaining good vibes along the music playout.
 
 <p align = "center">
 	<img src = "https://img.shields.io/badge/Pypi Package-PyVolSuggester-green?style=plastic&logo=appveyor", alt = "PyVolSuggester">
 	<img src = "https://img.shields.io/badge/PyPi-Python Package Index-green?style=plastic&logo=appveyor", alt = "PyPi">
 </p>
 <p align = "center">
 	<img src = "https://img.shields.io/github/stars/akash-rajak/PyVolSuggester?style=social", alt = "GitHub Repo stars">
@@ -237,15 +237,21 @@
 pip install PyVolSuggester
 ```
 
 ****
 
 
 ### 🌟Stargazers Over Time:
+[![Stargazers repo roster for @akash-rajak/PyVolSuggester](https://reporoster.com/stars/akash-rajak/PyVolSuggester)](https://github.com/akash-rajak/PyVolSuggester/stargazers)
 [![Stargazers over time](https://starchart.cc/akash-rajak/PyVolSuggester.svg)](https://starchart.cc/akash-rajak/PyVolSuggester)
 
 ****
 
+### 🌟Forkers Over Time:
+[![Forkers repo roster for @akash-rajak/PyVolSuggester](https://reporoster.com/forks/akash-rajak/PyVolSuggester)](https://github.com/akash-rajak/PyVolSuggester/network/members)
+
+****
+
 ### 📌Contributors:
 <a href="https://github.com/akash-rajak/PyVolSuggester/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=akash-rajak/PyVolSuggester" />
 </a>
```


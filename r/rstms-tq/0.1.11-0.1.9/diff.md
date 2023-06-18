# Comparing `tmp/rstms_tq-0.1.11.tar.gz` & `tmp/rstms-tq-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_tq-0.1.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms-tq-0.1.9.tar", last modified: Thu Jan 12 04:39:07 2023, max compression
```

## Comparing `rstms_tq-0.1.11.tar` & `rstms-tq-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      266 2023-06-18 02:47:51.282419 rstms_tq-0.1.11/.bumpversion.cfg
--rw-r--r--   0        0        0     1238 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/.gitignore
--rw-r--r--   0        0        0     1071 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/LICENSE
--rw-r--r--   0        0        0      547 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/Makefile
--rw-r--r--   0        0        0      753 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/README.md
--rw-r--r--   0        0        0        7 2023-06-18 02:47:51.282419 rstms_tq-0.1.11/VERSION
--rw-r--r--   0        0        0      289 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/browser.mk
--rw-r--r--   0        0        0      608 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/clean.mk
--rw-r--r--   0        0        0     3334 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/common.mk
--rw-r--r--   0        0        0      931 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/docker.mk
--rw-r--r--   0        0        0      278 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/lint.mk
--rw-r--r--   0        0        0     1010 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/publish.mk
--rw-r--r--   0        0        0     1518 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/release.mk
--rw-r--r--   0        0        0      952 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/requirements.mk
--rw-r--r--   0        0        0     1089 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/test.mk
--rw-r--r--   0        0        0     1348 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/make.include/version.mk
--rw-r--r--   0        0        0     1049 2023-06-18 02:45:14.120270 rstms_tq-0.1.11/pyproject.toml
--rw-r--r--   0        0        0      231 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/pytest.ini
--rw-r--r--   0        0        0       77 2023-06-18 02:47:23.410734 rstms_tq-0.1.11/requirements-dev.txt
--rw-r--r--   0        0        0       42 2023-06-18 02:47:23.410734 rstms_tq-0.1.11/requirements-docs.txt
--rw-r--r--   0        0        0       11 2023-06-18 02:47:23.410734 rstms_tq-0.1.11/requirements.txt
--rw-r--r--   0        0        0      206 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/rstms_tq/__init__.py
--rw-r--r--   0        0        0       86 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/rstms_tq/__main__.py
--rw-r--r--   0        0        0      892 2023-06-18 02:44:54.992505 rstms_tq-0.1.11/rstms_tq/tq.py
--rw-r--r--   0        0        0      128 2023-06-18 02:47:51.282419 rstms_tq-0.1.11/rstms_tq/version.py
--rw-r--r--   0        0        0       32 2023-06-18 02:44:54.996505 rstms_tq-0.1.11/tests/__init__.py
--rw-r--r--   0        0        0      142 2023-06-18 02:44:54.996505 rstms_tq-0.1.11/tests/test_cli.py
--rw-r--r--   0        0        0      424 2023-06-18 02:44:54.996505 rstms_tq-0.1.11/tox.ini
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 rstms_tq-0.1.11/PKG-INFO
+-rw-r--r--   0        0        0      265 2023-01-12 04:38:23.740000 rstms-tq-0.1.9/.bumpversion.cfg
+-rw-r--r--   0        0        0     1238 2023-01-12 03:42:36.820000 rstms-tq-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1071 2023-01-12 03:42:36.830000 rstms-tq-0.1.9/LICENSE
+-rw-r--r--   0        0        0      547 2023-01-12 03:42:36.840000 rstms-tq-0.1.9/Makefile
+-rw-r--r--   0        0        0      753 2023-01-12 03:42:36.830000 rstms-tq-0.1.9/README.md
+-rw-r--r--   0        0        0        6 2023-01-12 04:38:23.740000 rstms-tq-0.1.9/VERSION
+-rw-r--r--   0        0        0      289 2023-01-12 03:42:36.880000 rstms-tq-0.1.9/make.include/browser.mk
+-rw-r--r--   0        0        0      608 2023-01-12 03:42:36.870000 rstms-tq-0.1.9/make.include/clean.mk
+-rw-r--r--   0        0        0     3334 2023-01-12 03:42:36.880000 rstms-tq-0.1.9/make.include/common.mk
+-rw-r--r--   0        0        0      931 2023-01-12 03:42:36.870000 rstms-tq-0.1.9/make.include/docker.mk
+-rw-r--r--   0        0        0      278 2023-01-12 04:35:11.590000 rstms-tq-0.1.9/make.include/lint.mk
+-rw-r--r--   0        0        0     1010 2023-01-12 03:42:36.880000 rstms-tq-0.1.9/make.include/publish.mk
+-rw-r--r--   0        0        0     1518 2023-01-12 04:38:02.080000 rstms-tq-0.1.9/make.include/release.mk
+-rw-r--r--   0        0        0      952 2023-01-12 03:42:36.880000 rstms-tq-0.1.9/make.include/requirements.mk
+-rw-r--r--   0        0        0     1089 2023-01-12 03:42:36.880000 rstms-tq-0.1.9/make.include/test.mk
+-rw-r--r--   0        0        0     1348 2023-01-12 03:42:36.880000 rstms-tq-0.1.9/make.include/version.mk
+-rw-r--r--   0        0        0     1049 2023-01-12 04:34:14.650000 rstms-tq-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-01-12 03:42:36.840000 rstms-tq-0.1.9/pytest.ini
+-rw-r--r--   0        0        0       82 2023-01-12 04:36:40.760000 rstms-tq-0.1.9/requirements-dev.txt
+-rw-r--r--   0        0        0       42 2023-01-12 04:36:40.760000 rstms-tq-0.1.9/requirements-docs.txt
+-rw-r--r--   0        0        0        6 2023-01-12 04:36:40.760000 rstms-tq-0.1.9/requirements.txt
+-rw-r--r--   0        0        0      206 2023-01-12 04:02:58.440000 rstms-tq-0.1.9/rstms_tq/__init__.py
+-rw-r--r--   0        0        0       86 2023-01-12 04:02:58.440000 rstms-tq-0.1.9/rstms_tq/__main__.py
+-rw-r--r--   0        0        0      892 2023-01-12 04:02:58.460000 rstms-tq-0.1.9/rstms_tq/tq.py
+-rw-r--r--   0        0        0      127 2023-01-12 04:38:23.740000 rstms-tq-0.1.9/rstms_tq/version.py
+-rw-r--r--   0        0        0       32 2023-01-12 03:42:36.860000 rstms-tq-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      142 2023-01-12 04:02:58.440000 rstms-tq-0.1.9/tests/test_cli.py
+-rw-r--r--   0        0        0      424 2023-01-12 04:36:14.540000 rstms-tq-0.1.9/tox.ini
+-rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 rstms-tq-0.1.9/PKG-INFO
```

### Comparing `rstms_tq-0.1.11/.gitignore` & `rstms-tq-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/LICENSE` & `rstms-tq-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/Makefile` & `rstms-tq-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/README.md` & `rstms-tq-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/make.include/clean.mk` & `rstms-tq-0.1.9/make.include/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/make.include/common.mk` & `rstms-tq-0.1.9/make.include/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/make.include/docker.mk` & `rstms-tq-0.1.9/make.include/docker.mk`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/make.include/publish.mk` & `rstms-tq-0.1.9/make.include/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/make.include/release.mk` & `rstms-tq-0.1.9/make.include/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/make.include/requirements.mk` & `rstms-tq-0.1.9/make.include/requirements.mk`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/make.include/test.mk` & `rstms-tq-0.1.9/make.include/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/make.include/version.mk` & `rstms-tq-0.1.9/make.include/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/pyproject.toml` & `rstms-tq-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,15 @@
   "Natural Language :: English", 
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10"
 ]
 dynamic = ["version", "description"] 
 
 dependencies = [
-  "tomli",
-  "toml"
+  "tomli"
 ]
 
 [tool.flit.module]
 name = "rstms_tq"
 
 [project.optional-dependencies]
 dev = [
@@ -34,14 +33,15 @@
   "bump2version",
   "coverage",
   "isort",
   "flake8",
   "flake8-length",
   "pytest",
   "python-box",
+  "toml",
   "tox"
 ]
 docs = [
   "m2r2",
   "sphinx",
   "sphinx-click",
   "sphinx-rtd-theme"
```

### Comparing `rstms_tq-0.1.11/rstms_tq/tq.py` & `rstms-tq-0.1.9/rstms_tq/tq.py`

 * *Files identical despite different names*

### Comparing `rstms_tq-0.1.11/PKG-INFO` & `rstms-tq-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: rstms-tq
-Version: 0.1.11
+Version: 0.1.9
 Summary: Top-level package for rstms-tq.
 Keywords: tq
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: tomli
-Requires-Dist: toml
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
 Requires-Dist: coverage ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: flake8-length ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: python-box ; extra == "dev"
+Requires-Dist: toml ; extra == "dev"
 Requires-Dist: tox ; extra == "dev"
 Requires-Dist: m2r2 ; extra == "docs"
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-click ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
 Project-URL: Home, https://github.com/rstms/rstms-tq
 Provides-Extra: dev
```


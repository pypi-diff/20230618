# Comparing `tmp/stochastic_matching-0.2.1.tar.gz` & `tmp/stochastic_matching-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stochastic_matching-0.2.1.tar", last modified: Thu Feb  3 15:46:40 2022, max compression
+gzip compressed data, was "stochastic_matching-0.2.2.tar", last modified: Sun Jun 18 07:37:20 2023, max compression
```

## Comparing `stochastic_matching-0.2.1.tar` & `stochastic_matching-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:40.221357 stochastic_matching-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6272 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9721 2022-02-03 15:46:40.221357 stochastic_matching-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:40.217357 stochastic_matching-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5825 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:40.217357 stochastic_matching-0.2.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/reference/common.rst
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/reference/display.rst
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/reference/graphs.rst
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/reference/model.rst
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/reference/simulator.rst
--rw-r--r--   0 runner    (1001) docker     (121)   224070 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/sm_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)   175903 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/sm_logo_short.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:40.217357 stochastic_matching-0.2.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-02-03 15:46:40.221357 stochastic_matching-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:40.221357 stochastic_matching-0.2.1/stochastic_matching/
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12396 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    22380 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/display.py
--rw-r--r--   0 runner    (1001) docker     (121)    23335 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)    53054 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:40.221357 stochastic_matching-0.2.1/stochastic_matching/simulator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13937 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/simulator/age_based.py
--rw-r--r--   0 runner    (1001) docker     (121)     9583 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/simulator/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    30758 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/simulator/size_based.py
--rw-r--r--   0 runner    (1001) docker     (121)     7980 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/stochastic_matching/simulator/virtual_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:40.221357 stochastic_matching-0.2.1/stochastic_matching.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9721 2022-02-03 15:46:40.000000 stochastic_matching-0.2.1/stochastic_matching.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-02-03 15:46:40.000000 stochastic_matching-0.2.1/stochastic_matching.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 15:46:40.000000 stochastic_matching-0.2.1/stochastic_matching.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 15:46:40.000000 stochastic_matching-0.2.1/stochastic_matching.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-03 15:46:40.000000 stochastic_matching-0.2.1/stochastic_matching.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-02-03 15:46:40.000000 stochastic_matching-0.2.1/stochastic_matching.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 15:46:40.221357 stochastic_matching-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-02-03 15:46:25.000000 stochastic_matching-0.2.1/tests/test_stochastic_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:20.414640 stochastic_matching-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-06-18 07:37:20.414640 stochastic_matching-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:20.410640 stochastic_matching-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:20.410640 stochastic_matching-0.2.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/reference/common.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/reference/display.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/reference/graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/reference/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/reference/simulator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   224070 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/sm_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   175903 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/sm_logo_short.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:20.410640 stochastic_matching-0.2.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-18 07:37:20.414640 stochastic_matching-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:20.410640 stochastic_matching-0.2.2/stochastic_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23335 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53054 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:20.414640 stochastic_matching-0.2.2/stochastic_matching/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13937 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/simulator/age_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/simulator/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/simulator/size_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/stochastic_matching/simulator/virtual_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:20.410640 stochastic_matching-0.2.2/stochastic_matching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-06-18 07:37:20.000000 stochastic_matching-0.2.2/stochastic_matching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-18 07:37:20.000000 stochastic_matching-0.2.2/stochastic_matching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:37:20.000000 stochastic_matching-0.2.2/stochastic_matching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 07:37:20.000000 stochastic_matching-0.2.2/stochastic_matching.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-18 07:37:20.000000 stochastic_matching-0.2.2/stochastic_matching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 07:37:20.000000 stochastic_matching-0.2.2/stochastic_matching.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 07:37:20.414640 stochastic_matching-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-18 07:37:08.000000 stochastic_matching-0.2.2/tests/test_stochastic_matching.py
```

### Comparing `stochastic_matching-0.2.1/CONTRIBUTING.rst` & `stochastic_matching-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/HISTORY.rst` & `stochastic_matching-0.2.2/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 =======
 History
 =======
 
 ------------------------------------------------
+0.2.2 (2023-06-18): Improved CCDF
+------------------------------------------------
+
+* Add a function to draw the (discrete) CCDFs piecewise
+* New range of officially supported Python versions: 3.6 -> 3.11
+
+------------------------------------------------
 0.2.1 (2022-02-03): Big little update
 ------------------------------------------------
 
 * New optimize_rates for Model. Outputs a flow that optimizes the rates according to some reward weights.
 * Refactoring: policies formerly called semi-greedy are now called (semi)-filtering.
 * New option weights for filtering policies. Auto-computes the forbidden edges to optimize the reward according to weights.
 * Default model tolerance raised to 1e-7 for better detection of null edges.
```

### Comparing `stochastic_matching-0.2.1/LICENSE` & `stochastic_matching-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/PKG-INFO` & `stochastic_matching-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: stochastic_matching
-Version: 0.2.1
+Version: 0.2.2
 Summary: Stochastic Matching provides tools to analyze the behavior of stochastic matching problems.
 Home-page: https://github.com/balouf/stochastic_matching
 Author: Fabien Mathieu
 Author-email: fabien.mathieu@normalesup.org
 License: GNU General Public License v3
 Keywords: stochastic_matching
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -45,15 +44,14 @@
 
 
 .. image:: https://codecov.io/gh/balouf/stochastic_matching/branch/master/graphs/badge.svg
         :target: https://codecov.io/gh/balouf/stochastic_matching/tree/master/stochastic_matching
         :alt: Code Coverage
 
 
-
 Stochastic Matching provides tools to analyze the behavior of stochastic matching problems.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://balouf.github.io/stochastic_matching/.
 
 
@@ -66,23 +64,36 @@
     * Injectivity/surjectivity of the graph, kernel description.
     * Polytope description of positive solutions.
 * Fast simulator.
     * Provided with a large set of greedy / non-greedy policies.
     * Adding new policies is feasible out-of-the-box.
 * Lot of display features, including `Vis JS Network`_.
 
+
+---------------------
+Installation
+---------------------
+
+To install Stochastic Matching, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install stochastic_matching
+
+This is the preferred method to install Stochastic Matching, as it will always install the most recent stable release.
+
+
 ---------------------------
 Acknowledging package
 ---------------------------
 
 If you publish results based on `Stochastic Matching`_, **please acknowledge** the usage of the package by quoting the following paper.
 
 * Céline Comte, Fabien Mathieu, Ana Bušić. `Stochastic dynamic matching: A mixed graph-theory and linear-algebra approach <https://hal.archives-ouvertes.fr/hal-03502084>`_. 2022.
 
-
 -------
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `francois-durand/package_helper_2`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -93,14 +104,21 @@
 
 
 =======
 History
 =======
 
 ------------------------------------------------
+0.2.2 (2023-06-18): Improved CCDF
+------------------------------------------------
+
+* Add a function to draw the (discrete) CCDFs piecewise
+* New range of officially supported Python versions: 3.6 -> 3.11
+
+------------------------------------------------
 0.2.1 (2022-02-03): Big little update
 ------------------------------------------------
 
 * New optimize_rates for Model. Outputs a flow that optimizes the rates according to some reward weights.
 * Refactoring: policies formerly called semi-greedy are now called (semi)-filtering.
 * New option weights for filtering policies. Auto-computes the forbidden edges to optimize the reward according to weights.
 * Default model tolerance raised to 1e-7 for better detection of null edges.
@@ -213,9 +231,7 @@
     * When displayed, flows are checked by default. Conservation law issues gives red nodes, negative edges are red,
       null edges are orange (can be disabled).
     * SIMULATION ENGINE NOT AVAILABLE IN 0.0.2, as there are a lot of things to change. It will return in 0.0.3.
 * Misc:
     * Tutorials (simulation apart) have been updated. Enjoy the double degenerated fan!
     * Local coverage computation. Enforcing 100% coverage on all 0.0.2+ code.
     * Minor changes in the display module to cope with the new graph API.
-
-
```

### Comparing `stochastic_matching-0.2.1/README.rst` & `stochastic_matching-0.2.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 
 .. image:: https://codecov.io/gh/balouf/stochastic_matching/branch/master/graphs/badge.svg
         :target: https://codecov.io/gh/balouf/stochastic_matching/tree/master/stochastic_matching
         :alt: Code Coverage
 
 
-
 Stochastic Matching provides tools to analyze the behavior of stochastic matching problems.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://balouf.github.io/stochastic_matching/.
 
 
@@ -43,23 +42,36 @@
     * Injectivity/surjectivity of the graph, kernel description.
     * Polytope description of positive solutions.
 * Fast simulator.
     * Provided with a large set of greedy / non-greedy policies.
     * Adding new policies is feasible out-of-the-box.
 * Lot of display features, including `Vis JS Network`_.
 
+
+---------------------
+Installation
+---------------------
+
+To install Stochastic Matching, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install stochastic_matching
+
+This is the preferred method to install Stochastic Matching, as it will always install the most recent stable release.
+
+
 ---------------------------
 Acknowledging package
 ---------------------------
 
 If you publish results based on `Stochastic Matching`_, **please acknowledge** the usage of the package by quoting the following paper.
 
 * Céline Comte, Fabien Mathieu, Ana Bušić. `Stochastic dynamic matching: A mixed graph-theory and linear-algebra approach <https://hal.archives-ouvertes.fr/hal-03502084>`_. 2022.
 
-
 -------
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `francois-durand/package_helper_2`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
```

### Comparing `stochastic_matching-0.2.1/docs/Makefile` & `stochastic_matching-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/docs/conf.py` & `stochastic_matching-0.2.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode', 'sphinx.ext.napoleon', 'sphinx.ext.githubpages',
-              'sphinx.ext.intersphinx', 'nbsphinx', 'IPython.sphinxext.ipython_console_highlighting']
+              'sphinx.ext.intersphinx', 'nbsphinx', 'IPython.sphinxext.ipython_console_highlighting',
+              'sphinx.ext.imgconverter']
 
 # Add the possibility to access python documentation.
 intersphinx_mapping = {'python':('https://docs.python.org/3', None),
                        'sklearn':('https://scikit-learn.org/stable', None),
                        'ipython':('https://ipython.readthedocs.io/en/stable/', None),
                        'numpy': ('https://docs.scipy.org/doc/numpy/', None),
                        'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
@@ -78,15 +79,15 @@
 release = stochastic_matching.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `stochastic_matching-0.2.1/docs/installation.rst` & `stochastic_matching-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/docs/make.bat` & `stochastic_matching-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/docs/sm_logo.png` & `stochastic_matching-0.2.2/docs/sm_logo.png`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/docs/sm_logo_short.png` & `stochastic_matching-0.2.2/docs/sm_logo_short.png`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/setup.py` & `stochastic_matching-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     keywords='stochastic_matching',
     name='stochastic_matching',
     packages=find_packages(),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/balouf/stochastic_matching',
-    version='0.2.1',
+    version='0.2.2',
     zip_safe=False,
 )
```

### Comparing `stochastic_matching-0.2.1/stochastic_matching/__init__.py` & `stochastic_matching-0.2.2/stochastic_matching/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Stochastic Matching."""
 
 __author__ = """Fabien Mathieu"""
 __email__ = 'fabien.mathieu@normalesup.org'
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 from stochastic_matching.model import Model
 from stochastic_matching.graphs import Path, Star, Cycle, Codomino, CycleChain, Complete, Pyramid, HyperPaddle, \
     KayakPaddle, Lollipop, Tadpole, Barbell, Fan, concatenate
 from stochastic_matching.simulator.age_based import FCFM
 from stochastic_matching.simulator.virtual_queue import VQSimulator
 from stochastic_matching.simulator.size_based import LongestSimulator, PrioritySimulator, QueueSizeSimulator, \
```

### Comparing `stochastic_matching-0.2.1/stochastic_matching/common.py` & `stochastic_matching-0.2.2/stochastic_matching/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,31 +204,31 @@
     >>> incidence = np.array([[1, 1, 1],
     ...                       [1, 0, 1],
     ...                       [0, 1, 1],
     ...                       [0, 0, 1]])
 
     Edges of node 0:
 
-    >>> neighbors(0, csr_matrix(incidence))
-    array([0, 1, 2], dtype=int32)
+    >>> neighbors(0, csr_matrix(incidence)) # doctest: +ELLIPSIS
+    array([0, 1, 2]...)
 
     Egde of node 3:
 
-    >>> neighbors(3, csr_matrix(incidence))
-    array([2], dtype=int32)
+    >>> neighbors(3, csr_matrix(incidence)) # doctest: +ELLIPSIS
+    array([2]...)
 
     Nodes of edge 0:
 
-    >>> neighbors(0, csc_matrix(incidence))
-    array([0, 1], dtype=int32)
+    >>> neighbors(0, csc_matrix(incidence)) # doctest: +ELLIPSIS
+    array([0, 1]...)
 
     Nodes of hyperedge 2:
 
-    >>> neighbors(2, csc_matrix(incidence))
-    array([0, 1, 2, 3], dtype=int32)
+    >>> neighbors(2, csc_matrix(incidence)) # doctest: +ELLIPSIS
+    array([0, 1, 2, 3]...)
     """
     return compressed_incidence.indices[compressed_incidence.indptr[i]:compressed_incidence.indptr[i + 1]]
 
 
 @njit
 def set_seed(value):
     """
```

### Comparing `stochastic_matching-0.2.1/stochastic_matching/display.py` & `stochastic_matching-0.2.2/stochastic_matching/display.py`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/stochastic_matching/graphs.py` & `stochastic_matching-0.2.2/stochastic_matching/graphs.py`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/stochastic_matching/model.py` & `stochastic_matching-0.2.2/stochastic_matching/model.py`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/stochastic_matching/simulator/age_based.py` & `stochastic_matching-0.2.2/stochastic_matching/simulator/age_based.py`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/stochastic_matching/simulator/generic.py` & `stochastic_matching-0.2.2/stochastic_matching/simulator/generic.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     >>> fig #doctest: +ELLIPSIS
     <Figure size ...x... with 1 Axes>
 
     >>> fig = sim.show_ccdf()
     >>> fig #doctest: +ELLIPSIS
     <Figure size ...x... with 1 Axes>
 
-    >>> fig = sim.show_ccdf(indices=[0, 3, 2], sort=True)
+    >>> fig = sim.show_ccdf(indices=[0, 3, 2], sort=True, strict=True)
     >>> fig #doctest: +ELLIPSIS
     <Figure size ...x... with 1 Axes>
     """
 
     name = None
     """
     Name that can be used to list all non-abstract classes.
@@ -265,22 +265,24 @@
         None
         """
         # noinspection PyUnresolvedReferences
         tot_mu = np.sum(self.model.rates)
         steps = self.logs['steps_done']
         return self.logs['trafic']*tot_mu/steps
 
-    def show_ccdf(self, indices=None, sort=None):
+    def show_ccdf(self, indices=None, sort=None, strict=False):
         """
         Parameters
         ----------
         indices: :class:`list`, optional
             Indices of the nodes to display
         sort: :class:`bool`, optional
             If True, order the nodes by decreasing average queue size
+        strict: :class:`bool`, default = False
+            Draws the curves as a true piece-wise function
 
         Returns
         -------
         :class:`~matplotlib.figure.Figure`
             A figure of the CCDFs of the queues.
         """
         ccdf = self.compute_ccdf()
@@ -294,15 +296,26 @@
             averages = self.compute_average_queues()
             if indices is not None:
                 averages = averages[indices]
             ind = np.argsort(-averages)
             ccdf = ccdf[ind, :]
             names = [names[i] for i in ind]
         for i, name in enumerate(names):
-            plt.semilogy(ccdf[i, ccdf[i, :] > 0], label=name)
+            if strict:
+                data = ccdf[i, ccdf[i, :] > 0]
+                n_d = len(data)
+                x = np.zeros(2*n_d-1)
+                x[::2] = np.arange(n_d)
+                x[1::2] = np.arange(n_d-1)
+                y = np.zeros(2 * n_d - 1)
+                y[::2] = data
+                y[1::2] = data[1:]
+                plt.semilogy(x, y, label=name)
+            else:
+                plt.semilogy(ccdf[i, ccdf[i, :] > 0], label=name)
         plt.legend()
         plt.xlim([0, None])
         plt.ylim([None, 1])
         plt.ylabel("CCDF")
         plt.xlabel("Queue occupancy")
         return plt.gcf()
```

### Comparing `stochastic_matching-0.2.1/stochastic_matching/simulator/size_based.py` & `stochastic_matching-0.2.2/stochastic_matching/simulator/size_based.py`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/stochastic_matching/simulator/virtual_queue.py` & `stochastic_matching-0.2.2/stochastic_matching/simulator/virtual_queue.py`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/stochastic_matching.egg-info/PKG-INFO` & `stochastic_matching-0.2.2/stochastic_matching.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: stochastic-matching
-Version: 0.2.1
+Version: 0.2.2
 Summary: Stochastic Matching provides tools to analyze the behavior of stochastic matching problems.
 Home-page: https://github.com/balouf/stochastic_matching
 Author: Fabien Mathieu
 Author-email: fabien.mathieu@normalesup.org
 License: GNU General Public License v3
 Keywords: stochastic_matching
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -45,15 +44,14 @@
 
 
 .. image:: https://codecov.io/gh/balouf/stochastic_matching/branch/master/graphs/badge.svg
         :target: https://codecov.io/gh/balouf/stochastic_matching/tree/master/stochastic_matching
         :alt: Code Coverage
 
 
-
 Stochastic Matching provides tools to analyze the behavior of stochastic matching problems.
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://balouf.github.io/stochastic_matching/.
 
 
@@ -66,23 +64,36 @@
     * Injectivity/surjectivity of the graph, kernel description.
     * Polytope description of positive solutions.
 * Fast simulator.
     * Provided with a large set of greedy / non-greedy policies.
     * Adding new policies is feasible out-of-the-box.
 * Lot of display features, including `Vis JS Network`_.
 
+
+---------------------
+Installation
+---------------------
+
+To install Stochastic Matching, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install stochastic_matching
+
+This is the preferred method to install Stochastic Matching, as it will always install the most recent stable release.
+
+
 ---------------------------
 Acknowledging package
 ---------------------------
 
 If you publish results based on `Stochastic Matching`_, **please acknowledge** the usage of the package by quoting the following paper.
 
 * Céline Comte, Fabien Mathieu, Ana Bušić. `Stochastic dynamic matching: A mixed graph-theory and linear-algebra approach <https://hal.archives-ouvertes.fr/hal-03502084>`_. 2022.
 
-
 -------
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `francois-durand/package_helper_2`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
@@ -93,14 +104,21 @@
 
 
 =======
 History
 =======
 
 ------------------------------------------------
+0.2.2 (2023-06-18): Improved CCDF
+------------------------------------------------
+
+* Add a function to draw the (discrete) CCDFs piecewise
+* New range of officially supported Python versions: 3.6 -> 3.11
+
+------------------------------------------------
 0.2.1 (2022-02-03): Big little update
 ------------------------------------------------
 
 * New optimize_rates for Model. Outputs a flow that optimizes the rates according to some reward weights.
 * Refactoring: policies formerly called semi-greedy are now called (semi)-filtering.
 * New option weights for filtering policies. Auto-computes the forbidden edges to optimize the reward according to weights.
 * Default model tolerance raised to 1e-7 for better detection of null edges.
@@ -213,9 +231,7 @@
     * When displayed, flows are checked by default. Conservation law issues gives red nodes, negative edges are red,
       null edges are orange (can be disabled).
     * SIMULATION ENGINE NOT AVAILABLE IN 0.0.2, as there are a lot of things to change. It will return in 0.0.3.
 * Misc:
     * Tutorials (simulation apart) have been updated. Enjoy the double degenerated fan!
     * Local coverage computation. Enforcing 100% coverage on all 0.0.2+ code.
     * Minor changes in the display module to cope with the new graph API.
-
-
```

### Comparing `stochastic_matching-0.2.1/stochastic_matching.egg-info/SOURCES.txt` & `stochastic_matching-0.2.2/stochastic_matching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stochastic_matching-0.2.1/tests/test_stochastic_matching.py` & `stochastic_matching-0.2.2/tests/test_stochastic_matching.py`

 * *Files identical despite different names*


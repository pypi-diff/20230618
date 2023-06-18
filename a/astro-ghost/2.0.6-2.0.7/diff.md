# Comparing `tmp/astro_ghost-2.0.6.tar.gz` & `tmp/astro_ghost-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.0.6.tar", last modified: Sat Jun 17 20:43:58 2023, max compression
+gzip compressed data, was "astro_ghost-2.0.7.tar", last modified: Sun Jun 18 19:30:13 2023, max compression
```

## Comparing `astro_ghost-2.0.6.tar` & `astro_ghost-2.0.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.797822 astro_ghost-2.0.6/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.723746 astro_ghost-2.0.6/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.729524 astro_ghost-2.0.6/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      587 2023-05-24 04:50:38.000000 astro_ghost-2.0.6/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-17 20:43:58.798078 astro_ghost-2.0.6/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.6/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.775485 astro_ghost-2.0.6/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    23411 2023-06-17 20:43:17.000000 astro_ghost-2.0.6/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.6/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.6/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.6/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.6/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.6/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.6/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-17 20:43:41.000000 astro_ghost-2.0.6/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.6/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    42487 2023-06-17 15:47:53.000000 astro_ghost-2.0.6/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.6/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.6/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.6/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-06-06 16:38:06.000000 astro_ghost-2.0.6/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.6/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.6/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.6/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.778467 astro_ghost-2.0.6/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-17 20:43:58.000000 astro_ghost-2.0.6/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-17 20:43:58.000000 astro_ghost-2.0.6/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-17 20:43:58.000000 astro_ghost-2.0.6/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-17 20:43:58.000000 astro_ghost-2.0.6/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-17 20:43:58.000000 astro_ghost-2.0.6/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-17 20:43:58.000000 astro_ghost-2.0.6/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.782316 astro_ghost-2.0.6/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.6/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.6/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.791663 astro_ghost-2.0.6/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.6/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.6/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.6/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.6/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.6/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.6/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.6/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.6/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.794086 astro_ghost-2.0.6/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.6/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-17 20:43:58.799372 astro_ghost-2.0.6/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-17 20:43:48.000000 astro_ghost-2.0.6/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 20:43:58.796818 astro_ghost-2.0.6/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.6/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.6/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.6/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.6/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.6/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.815736 astro_ghost-2.0.7/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.756559 astro_ghost-2.0.7/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.761514 astro_ghost-2.0.7/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      601 2023-06-17 21:52:31.000000 astro_ghost-2.0.7/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-18 19:30:13.815900 astro_ghost-2.0.7/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.7/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.802836 astro_ghost-2.0.7/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    23495 2023-06-18 19:28:46.000000 astro_ghost-2.0.7/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.7/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.7/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.7/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.7/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.7/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.7/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-18 19:29:34.000000 astro_ghost-2.0.7/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.7/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    42487 2023-06-17 15:47:53.000000 astro_ghost-2.0.7/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.7/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.7/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17703 2023-06-18 19:28:46.000000 astro_ghost-2.0.7/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-06-06 16:38:06.000000 astro_ghost-2.0.7/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.7/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.7/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.7/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.804889 astro_ghost-2.0.7/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.806837 astro_ghost-2.0.7/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.7/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.7/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.812021 astro_ghost-2.0.7/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.7/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.7/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.7/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.7/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.7/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.7/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.7/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.7/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.813759 astro_ghost-2.0.7/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-18 19:30:13.816603 astro_ghost-2.0.7/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-18 19:29:47.000000 astro_ghost-2.0.7/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.815485 astro_ghost-2.0.7/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.7/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.7/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.7/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4492 2023-06-18 19:28:46.000000 astro_ghost-2.0.7/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.7/tox.ini
```

### Comparing `astro_ghost-2.0.6/.github/workflows/tests.yml` & `astro_ghost-2.0.7/.github/workflows/tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: unit tests
 
-on: [push]
+on: [push, pull_request]
 
 jobs:
   build:
     runs-on: [macos-latest]
 
     steps:
     - uses: actions/checkout@v1
```

### Comparing `astro_ghost-2.0.6/.gitignore` & `astro_ghost-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/PKG-INFO` & `astro_ghost-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 2.0.6
+Version: 2.0.7
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.6/README.rst` & `astro_ghost-2.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/DLR.py` & `astro_ghost-2.0.7/astro_ghost/DLR.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,16 +414,18 @@
 
         #query the glade catalog
         Vizier.ROW_LIMIT = -1
         Vizier.TIMEOUT = 500
         result = Vizier.query_region(SkyCoord(ra=ra_SN, dec=dec_SN,unit=(u.deg, u.deg),frame='icrs'),radius=Angle(1.0, "deg"), catalog=["VII/275/glade1"])
         if result:
             hosts = result[0].to_pandas()
+        else:
+            hosts = pd.DataFrame({'a_b':[np.nan], 'maj':[np.nan], 'min':[np.nan]})
         
-        #NEW (06/14) - query NED for GLADE sources and get their radius
+        # query NED for GLADE sources and get their radius
         GLADE_rad = hosts.dropna(subset=['a_b', 'maj', 'min'])
         GLADE_norad = hosts[~hosts.index.isin(GLADE_rad.index)]
 
         from astroquery.ipac.ned import Ned
         badRadCount = 0
         for idx, row in GLADE_norad.iterrows():
             try:
```

### Comparing `astro_ghost-2.0.6/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.0.7/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.0.7/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.0.7/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.0.7/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.0.7/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/conftest.py` & `astro_ghost-2.0.7/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.0.7/astro_ghost/ghostHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/gradientAscent.py` & `astro_ghost-2.0.7/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/hostMatching.py` & `astro_ghost-2.0.7/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/photoz_helper.py` & `astro_ghost-2.0.7/astro_ghost/photoz_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,21 +96,21 @@
 
     for i in range(len(data_list)):
         data_list[i]['objID'] = objID[i]
 
     urls = []
     datas = []
     for i in range(len(objID)):
-        url, data = ps1search(table=table,release=release,format=format,columns=columns,
+        data = ps1search(table=table,release=release,format=format,columns=columns,
                     baseurl=baseurl, verbose=verbose, **data_list[i])
 
-        urls.append(url)
+        #urls.append(url)
         datas.append(data)
 
-    return urls, datas
+    return datas
 
 def fetch_information_serially(url, data, verbose=False, format='csv'):
     """A helper function called by serial_objID_search-- Queries PanStarrs API for data.
     
     :param url: Remote PS1 url.
     :type url: str
     :param data: List of objIDs requesting
@@ -198,16 +198,16 @@
     :param \\*\\*constraints: Keyword dictionary with an additional constraints for the PS1 query
     :type \\*\\*constraints: dict
     :return: list of pd.DataFrame objects. If a match was found, then the Dataframe contains data, else it only contains a local integer.
     :rtype: pd.DataFrame
     """
 
     constrains=constraints.copy()
-    URLS, DATAS = ps1objIDsearch(objID=objIDs,table='forced_mean',release=release,columns=columns,verbose=verbose,**constraints)
-    Return = fetch_information_serially(URLS,DATAS)
+    Return = ps1objIDsearch(objID=objIDs,table='forced_mean',release=release,columns=columns,verbose=verbose,**constraints)
+    #Return = fetch_information_serially(URLS,DATAS)
     DFs=[]
     for i in range(len(Return)):
         DFs.append(post_url_serial(Return[i],i))
 
     return DFs
 
 def post_url_parallel(results,YSE_ID):
@@ -354,14 +354,15 @@
         OUTPUT = tf.keras.layers.Dense(360,activation=tf.keras.activations.softmax)(DENSE4)
 
         model = tf.keras.Model(INPUT,OUTPUT)
 
         return model
     mymodel = model()
     mymodel.load_weights(model_path)
+    
 
     NB_BINS = 360
     ZMIN = 0.0
     ZMAX = 1.0
     BIN_SIZE = (ZMAX - ZMIN) / NB_BINS
     range_z = np.linspace(ZMIN, ZMAX, NB_BINS + 1)[:NB_BINS]
 
@@ -382,15 +383,15 @@
     :rtype: numpy ndarray shape of (df.shape[0], n)
     :return: Means
     :rtype: numpy ndarray shape of (df.shape[0],)
     :return: Standard deviations
     :rtype: numpy ndarray shape of (df.shape[0],)
     """
 
-    posteriors = mymodel(X,training=False).numpy()
+    posteriors = mymodel.predict(X)
     point_estimates = np.sum(posteriors*range_z,axis=1)
     for i in range(len(posteriors)):
         posteriors[i,:] /= np.sum(posteriors[i,:])
     errors=np.ones(len(posteriors))
     for i in range(len(posteriors)):
         errors[i] = (np.std(np.random.choice(a=range_z,size=1000,p=posteriors[i,:],replace=True)))
```

### Comparing `astro_ghost-2.0.6/astro_ghost/sourceCleaning.py` & `astro_ghost-2.0.7/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/starSeparation.py` & `astro_ghost-2.0.7/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost/stellarLocus.py` & `astro_ghost-2.0.7/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.0.7/astro_ghost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 2.0.6
+Version: 2.0.7
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.6/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.0.7/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/Makefile` & `astro_ghost-2.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/conf.py` & `astro_ghost-2.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/index.rst` & `astro_ghost-2.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/make.bat` & `astro_ghost-2.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/source/associationmodules.rst` & `astro_ghost-2.0.7/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/source/basicusage.rst` & `astro_ghost-2.0.7/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/source/catalogmodules.rst` & `astro_ghost-2.0.7/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/source/installation.rst` & `astro_ghost-2.0.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/docs/source/preprocessingmodules.rst` & `astro_ghost-2.0.7/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/licenses/LICENSE.rst` & `astro_ghost-2.0.7/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/setup.cfg` & `astro_ghost-2.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/setup.py` & `astro_ghost-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "2.0.6"
+version = "2.0.7"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-2.0.6/tests/debug.py` & `astro_ghost-2.0.7/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.6/tests/test_tutorial.py` & `astro_ghost-2.0.7/tests/test_tutorial.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import sys
 from astro_ghost.PS1QueryFunctions import *
 from astro_ghost.TNSQueryFunctions import *
 from astro_ghost.NEDQueryFunctions import *
 from astro_ghost.ghostHelperFunctions import *
 from astro_ghost.starSeparation import *
 from astro_ghost.stellarLocus import *
+from astro_ghost.photoz_helper import calc_photoz
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 import pandas as pd
 from datetime import datetime
 
+
 #we want to include print statements so we know what the algorithm is doing
 verbose = 1
 
 def test_getGHOST():
     #Download the GHOST database.
     #note: real=False creates an empty database, which
     #allows you to use the association methods without
@@ -96,7 +98,12 @@
     assert hosts['NED_name'].values[0] == 'ESO 184- G 042'
 
 def test_resolve():
     coords = resolve('M100')
     c1 = SkyCoord(coords[0]*u.deg, coords[1]*u.deg, frame='icrs')
     c2 = SkyCoord(185.7288750*u.deg, 15.82230*u.deg, frame='icrs')
     assert c2.separation(c2).arcsec < 0.1
+    
+def test_photoz():
+    DF_test = pd.DataFrame({'raMean':[258.026087],'decMean':[40.344349,],'objID':[156412580262833857],})
+    DF_test = calc_photoz(DF_test)
+    assert np.abs(DF_test['photo_z'].iloc[0] - 0.260683) < 0.01
```

### Comparing `astro_ghost-2.0.6/tox.ini` & `astro_ghost-2.0.7/tox.ini`

 * *Files identical despite different names*


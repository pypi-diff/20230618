# Comparing `tmp/astro_ghost-2.0.7.tar.gz` & `tmp/astro_ghost-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.0.7.tar", last modified: Sun Jun 18 19:30:13 2023, max compression
+gzip compressed data, was "astro_ghost-2.0.8.tar", last modified: Sun Jun 18 20:32:44 2023, max compression
```

## Comparing `astro_ghost-2.0.7.tar` & `astro_ghost-2.0.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.815736 astro_ghost-2.0.7/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.756559 astro_ghost-2.0.7/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.761514 astro_ghost-2.0.7/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      601 2023-06-17 21:52:31.000000 astro_ghost-2.0.7/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-18 19:30:13.815900 astro_ghost-2.0.7/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.7/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.802836 astro_ghost-2.0.7/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    23495 2023-06-18 19:28:46.000000 astro_ghost-2.0.7/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.7/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.7/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.7/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.7/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.7/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.7/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-18 19:29:34.000000 astro_ghost-2.0.7/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.7/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    42487 2023-06-17 15:47:53.000000 astro_ghost-2.0.7/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.7/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.7/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17703 2023-06-18 19:28:46.000000 astro_ghost-2.0.7/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-06-06 16:38:06.000000 astro_ghost-2.0.7/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.7/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.7/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.7/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.804889 astro_ghost-2.0.7/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-18 19:30:13.000000 astro_ghost-2.0.7/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.806837 astro_ghost-2.0.7/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.7/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.7/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.812021 astro_ghost-2.0.7/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.7/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.7/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.7/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.7/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.7/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.7/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.7/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.7/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.813759 astro_ghost-2.0.7/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.7/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-18 19:30:13.816603 astro_ghost-2.0.7/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-18 19:29:47.000000 astro_ghost-2.0.7/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 19:30:13.815485 astro_ghost-2.0.7/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.7/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.7/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.7/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4492 2023-06-18 19:28:46.000000 astro_ghost-2.0.7/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.7/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.823954 astro_ghost-2.0.8/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.748112 astro_ghost-2.0.8/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.753527 astro_ghost-2.0.8/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      601 2023-06-17 21:52:31.000000 astro_ghost-2.0.8/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-18 20:32:44.824143 astro_ghost-2.0.8/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.8/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.806973 astro_ghost-2.0.8/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    23495 2023-06-18 19:28:46.000000 astro_ghost-2.0.8/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.8/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.8/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.8/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.8/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.8/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.8/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-18 20:32:27.000000 astro_ghost-2.0.8/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.8/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    42652 2023-06-18 20:31:32.000000 astro_ghost-2.0.8/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.8/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.8/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17703 2023-06-18 19:28:46.000000 astro_ghost-2.0.8/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-06-06 16:38:06.000000 astro_ghost-2.0.8/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.8/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.8/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.8/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.809674 astro_ghost-2.0.8/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-18 20:32:44.000000 astro_ghost-2.0.8/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.812856 astro_ghost-2.0.8/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.8/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.8/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.819597 astro_ghost-2.0.8/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.8/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.8/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.8/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.8/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.8/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.8/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.8/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.8/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.821409 astro_ghost-2.0.8/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.8/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-18 20:32:44.824883 astro_ghost-2.0.8/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-18 20:32:18.000000 astro_ghost-2.0.8/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-18 20:32:44.823607 astro_ghost-2.0.8/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.8/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.8/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.8/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4492 2023-06-18 19:28:46.000000 astro_ghost-2.0.8/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.8/tox.ini
```

### Comparing `astro_ghost-2.0.7/.github/workflows/tests.yml` & `astro_ghost-2.0.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/.gitignore` & `astro_ghost-2.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/PKG-INFO` & `astro_ghost-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 2.0.7
+Version: 2.0.8
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.7/README.rst` & `astro_ghost-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/DLR.py` & `astro_ghost-2.0.8/astro_ghost/DLR.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.0.8/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.0.8/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.0.8/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.0.8/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.0.8/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/conftest.py` & `astro_ghost-2.0.8/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.0.8/astro_ghost/ghostHelperFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,17 +229,22 @@
         FROM (SELECT oid, id FROM basic JOIN ident ON oidref = oid WHERE
         CONTAINS(POINT('ICRS',ra,dec),CIRCLE('ICRS',{0},{1},0.000556))=1 ) AS cluster, basic
         JOIN h_link ON basic.oid = h_link.parent WHERE h_link.child = cluster.oid ORDER BY dist ASC;
         """.format(row.raMean, row.decMean)
         result = tap_simbad.search(query)
         tap_pandas = result.to_table().to_pandas().reset_index(drop=True)
         if ((not tap_pandas.empty) and (tap_pandas.loc[0, 'membership'] > 50)):
+            tap_pandas.drop_duplicates(subset=['main_id'], inplace=True)
+            tap_pandas.reset_index(drop=True, inplace=True)
+ 
+            if tap_pandas['main_id'].values[0].startswith("VIRTUAL PARENT"):
+                continue
+
             if verbose:
                 print("Warning! Host of %s is the hierarchical child of another object in Simbad, choosing parent as host instead..." % row.TransientName)
-            tap_pandas.drop_duplicates(subset=['main_id'], inplace=True)
 
             # query PS1 for correct host
             a = ps1cone(tap_pandas.loc[0, 'ra'], tap_pandas.loc[0, 'dec'], 10./3600)
             if a:
                 a = ascii.read(a)
                 a = a.to_pandas()
                 parent = a.iloc[[0]]
```

### Comparing `astro_ghost-2.0.7/astro_ghost/gradientAscent.py` & `astro_ghost-2.0.8/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/hostMatching.py` & `astro_ghost-2.0.8/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/photoz_helper.py` & `astro_ghost-2.0.8/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/sourceCleaning.py` & `astro_ghost-2.0.8/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/starSeparation.py` & `astro_ghost-2.0.8/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost/stellarLocus.py` & `astro_ghost-2.0.8/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.0.8/astro_ghost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 2.0.7
+Version: 2.0.8
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.7/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.0.8/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/Makefile` & `astro_ghost-2.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/conf.py` & `astro_ghost-2.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/index.rst` & `astro_ghost-2.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/make.bat` & `astro_ghost-2.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/source/associationmodules.rst` & `astro_ghost-2.0.8/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/source/basicusage.rst` & `astro_ghost-2.0.8/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/source/catalogmodules.rst` & `astro_ghost-2.0.8/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/source/installation.rst` & `astro_ghost-2.0.8/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/docs/source/preprocessingmodules.rst` & `astro_ghost-2.0.8/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/licenses/LICENSE.rst` & `astro_ghost-2.0.8/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/setup.cfg` & `astro_ghost-2.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/setup.py` & `astro_ghost-2.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "2.0.7"
+version = "2.0.8"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-2.0.7/tests/debug.py` & `astro_ghost-2.0.8/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/tests/test_tutorial.py` & `astro_ghost-2.0.8/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.7/tox.ini` & `astro_ghost-2.0.8/tox.ini`

 * *Files identical despite different names*


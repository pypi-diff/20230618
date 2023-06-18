# Comparing `tmp/nrh-lotr-0.0.2.tar.gz` & `tmp/nrh-lotr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrh-lotr-0.0.2.tar", last modified: Sun Jun 18 04:02:03 2023, max compression
+gzip compressed data, was "nrh-lotr-0.0.3.tar", last modified: Sun Jun 18 04:32:39 2023, max compression
```

## Comparing `nrh-lotr-0.0.2.tar` & `nrh-lotr-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.782823 nrh-lotr-0.0.2/
--rw-r--r--   0 nhapeman   (501) staff       (20)     1069 2023-06-18 02:23:37.000000 nrh-lotr-0.0.2/LICENSE.txt
--rw-r--r--   0 nhapeman   (501) staff       (20)     3008 2023-06-18 04:02:03.782710 nrh-lotr-0.0.2/PKG-INFO
--rw-r--r--   0 nhapeman   (501) staff       (20)     1537 2023-06-18 04:00:09.000000 nrh-lotr-0.0.2/README.md
--rw-r--r--   0 nhapeman   (501) staff       (20)      390 2023-06-18 04:01:13.000000 nrh-lotr-0.0.2/pyproject.toml
--rw-r--r--   0 nhapeman   (501) staff       (20)       38 2023-06-18 04:02:03.782853 nrh-lotr-0.0.2/setup.cfg
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.781180 nrh-lotr-0.0.2/src/
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.781903 nrh-lotr-0.0.2/src/lotr/
--rw-r--r--   0 nhapeman   (501) staff       (20)       37 2023-06-18 02:53:17.000000 nrh-lotr-0.0.2/src/lotr/__init__.py
--rw-r--r--   0 nhapeman   (501) staff       (20)     2216 2023-06-18 03:53:13.000000 nrh-lotr-0.0.2/src/lotr/lotr.py
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.782453 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/
--rw-r--r--   0 nhapeman   (501) staff       (20)     3008 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/PKG-INFO
--rw-r--r--   0 nhapeman   (501) staff       (20)      271 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/SOURCES.txt
--rw-r--r--   0 nhapeman   (501) staff       (20)        1 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/dependency_links.txt
--rw-r--r--   0 nhapeman   (501) staff       (20)       18 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/requires.txt
--rw-r--r--   0 nhapeman   (501) staff       (20)        5 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/top_level.txt
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.782564 nrh-lotr-0.0.2/tests/
--rw-r--r--   0 nhapeman   (501) staff       (20)     1095 2023-06-18 03:02:32.000000 nrh-lotr-0.0.2/tests/test_sdk.py
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:32:39.517867 nrh-lotr-0.0.3/
+-rw-r--r--   0 nhapeman   (501) staff       (20)     1069 2023-06-18 02:23:37.000000 nrh-lotr-0.0.3/LICENSE.txt
+-rw-r--r--   0 nhapeman   (501) staff       (20)     3253 2023-06-18 04:32:39.517761 nrh-lotr-0.0.3/PKG-INFO
+-rw-r--r--   0 nhapeman   (501) staff       (20)     1782 2023-06-18 04:28:05.000000 nrh-lotr-0.0.3/README.md
+-rw-r--r--   0 nhapeman   (501) staff       (20)      404 2023-06-18 04:31:26.000000 nrh-lotr-0.0.3/pyproject.toml
+-rw-r--r--   0 nhapeman   (501) staff       (20)       38 2023-06-18 04:32:39.517897 nrh-lotr-0.0.3/setup.cfg
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:32:39.516387 nrh-lotr-0.0.3/src/
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:32:39.516967 nrh-lotr-0.0.3/src/lotr/
+-rw-r--r--   0 nhapeman   (501) staff       (20)       37 2023-06-18 02:53:17.000000 nrh-lotr-0.0.3/src/lotr/__init__.py
+-rw-r--r--   0 nhapeman   (501) staff       (20)     2216 2023-06-18 03:53:13.000000 nrh-lotr-0.0.3/src/lotr/lotr.py
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:32:39.517502 nrh-lotr-0.0.3/src/nrh_lotr.egg-info/
+-rw-r--r--   0 nhapeman   (501) staff       (20)     3253 2023-06-18 04:32:39.000000 nrh-lotr-0.0.3/src/nrh_lotr.egg-info/PKG-INFO
+-rw-r--r--   0 nhapeman   (501) staff       (20)      271 2023-06-18 04:32:39.000000 nrh-lotr-0.0.3/src/nrh_lotr.egg-info/SOURCES.txt
+-rw-r--r--   0 nhapeman   (501) staff       (20)        1 2023-06-18 04:32:39.000000 nrh-lotr-0.0.3/src/nrh_lotr.egg-info/dependency_links.txt
+-rw-r--r--   0 nhapeman   (501) staff       (20)       25 2023-06-18 04:32:39.000000 nrh-lotr-0.0.3/src/nrh_lotr.egg-info/requires.txt
+-rw-r--r--   0 nhapeman   (501) staff       (20)        5 2023-06-18 04:32:39.000000 nrh-lotr-0.0.3/src/nrh_lotr.egg-info/top_level.txt
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:32:39.517615 nrh-lotr-0.0.3/tests/
+-rw-r--r--   0 nhapeman   (501) staff       (20)     1095 2023-06-18 03:02:32.000000 nrh-lotr-0.0.3/tests/test_sdk.py
```

### Comparing `nrh-lotr-0.0.2/LICENSE.txt` & `nrh-lotr-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nrh-lotr-0.0.2/PKG-INFO` & `nrh-lotr-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrh-lotr
-Version: 0.0.2
+Version: 0.0.3
 Summary: lotR SDK for movies and quotes
 Author-email: Nathan Hapeman <nhapeman@gmail.com>
 License: MIT License
         
         Copyright 2023 Nathanial Hapeman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,18 +49,22 @@
 ## Installation
 
 Using python>=3.9: `pip install nrh-lotr`
 
 ## Usage
 
 ```py
+# First grab an api key from: https://the-one-api.dev/documentation#3
+# Then put it in an env var like: `export API_KEY=SOME_API_KEY`
+# Or insert it directly into the LOTR class as depicted below
 from lotr import LOTR, Movie, Quote
 
 # Movie basics.
-lotr = LOTR()
+lotr = LOTR("YOUR_API_KEY")
+# lotr = LOTR() # if using env var
 movies = lotr.movies(limit=5)
 assert len(movies) == 5
 movie_3 = movies[3]
 assert lotr.movies(id=movie_3.id)[0] == movie_3
 
 # Quote basics.
 lotr = LOTR()
```

### Comparing `nrh-lotr-0.0.2/README.md` & `nrh-lotr-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,22 @@
 ## Installation
 
 Using python>=3.9: `pip install nrh-lotr`
 
 ## Usage
 
 ```py
+# First grab an api key from: https://the-one-api.dev/documentation#3
+# Then put it in an env var like: `export API_KEY=SOME_API_KEY`
+# Or insert it directly into the LOTR class as depicted below
 from lotr import LOTR, Movie, Quote
 
 # Movie basics.
-lotr = LOTR()
+lotr = LOTR("YOUR_API_KEY")
+# lotr = LOTR() # if using env var
 movies = lotr.movies(limit=5)
 assert len(movies) == 5
 movie_3 = movies[3]
 assert lotr.movies(id=movie_3.id)[0] == movie_3
 
 # Quote basics.
 lotr = LOTR()
```

### Comparing `nrh-lotr-0.0.2/src/lotr/lotr.py` & `nrh-lotr-0.0.3/src/lotr/lotr.py`

 * *Files identical despite different names*

### Comparing `nrh-lotr-0.0.2/src/nrh_lotr.egg-info/PKG-INFO` & `nrh-lotr-0.0.3/src/nrh_lotr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrh-lotr
-Version: 0.0.2
+Version: 0.0.3
 Summary: lotR SDK for movies and quotes
 Author-email: Nathan Hapeman <nhapeman@gmail.com>
 License: MIT License
         
         Copyright 2023 Nathanial Hapeman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,18 +49,22 @@
 ## Installation
 
 Using python>=3.9: `pip install nrh-lotr`
 
 ## Usage
 
 ```py
+# First grab an api key from: https://the-one-api.dev/documentation#3
+# Then put it in an env var like: `export API_KEY=SOME_API_KEY`
+# Or insert it directly into the LOTR class as depicted below
 from lotr import LOTR, Movie, Quote
 
 # Movie basics.
-lotr = LOTR()
+lotr = LOTR("YOUR_API_KEY")
+# lotr = LOTR() # if using env var
 movies = lotr.movies(limit=5)
 assert len(movies) == 5
 movie_3 = movies[3]
 assert lotr.movies(id=movie_3.id)[0] == movie_3
 
 # Quote basics.
 lotr = LOTR()
```

### Comparing `nrh-lotr-0.0.2/tests/test_sdk.py` & `nrh-lotr-0.0.3/tests/test_sdk.py`

 * *Files identical despite different names*


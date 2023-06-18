# Comparing `tmp/nrh-lotr-0.0.1.tar.gz` & `tmp/nrh-lotr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrh-lotr-0.0.1.tar", last modified: Sun Jun 18 03:15:30 2023, max compression
+gzip compressed data, was "nrh-lotr-0.0.2.tar", last modified: Sun Jun 18 04:02:03 2023, max compression
```

## Comparing `nrh-lotr-0.0.1.tar` & `nrh-lotr-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 03:15:30.621839 nrh-lotr-0.0.1/
--rw-r--r--   0 nhapeman   (501) staff       (20)     1069 2023-06-18 02:23:37.000000 nrh-lotr-0.0.1/LICENSE.txt
--rw-r--r--   0 nhapeman   (501) staff       (20)     1887 2023-06-18 03:15:30.621733 nrh-lotr-0.0.1/PKG-INFO
--rw-r--r--   0 nhapeman   (501) staff       (20)      416 2023-06-18 03:07:10.000000 nrh-lotr-0.0.1/README.md
--rw-r--r--   0 nhapeman   (501) staff       (20)      390 2023-06-18 02:35:38.000000 nrh-lotr-0.0.1/pyproject.toml
--rw-r--r--   0 nhapeman   (501) staff       (20)       38 2023-06-18 03:15:30.621870 nrh-lotr-0.0.1/setup.cfg
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 03:15:30.620182 nrh-lotr-0.0.1/src/
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 03:15:30.620819 nrh-lotr-0.0.1/src/lotr/
--rw-r--r--   0 nhapeman   (501) staff       (20)       37 2023-06-18 02:53:17.000000 nrh-lotr-0.0.1/src/lotr/__init__.py
--rw-r--r--   0 nhapeman   (501) staff       (20)     3005 2023-06-18 01:00:20.000000 nrh-lotr-0.0.1/src/lotr/lotr.py
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 03:15:30.621462 nrh-lotr-0.0.1/src/nrh_lotr.egg-info/
--rw-r--r--   0 nhapeman   (501) staff       (20)     1887 2023-06-18 03:15:30.000000 nrh-lotr-0.0.1/src/nrh_lotr.egg-info/PKG-INFO
--rw-r--r--   0 nhapeman   (501) staff       (20)      271 2023-06-18 03:15:30.000000 nrh-lotr-0.0.1/src/nrh_lotr.egg-info/SOURCES.txt
--rw-r--r--   0 nhapeman   (501) staff       (20)        1 2023-06-18 03:15:30.000000 nrh-lotr-0.0.1/src/nrh_lotr.egg-info/dependency_links.txt
--rw-r--r--   0 nhapeman   (501) staff       (20)       18 2023-06-18 03:15:30.000000 nrh-lotr-0.0.1/src/nrh_lotr.egg-info/requires.txt
--rw-r--r--   0 nhapeman   (501) staff       (20)        5 2023-06-18 03:15:30.000000 nrh-lotr-0.0.1/src/nrh_lotr.egg-info/top_level.txt
-drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 03:15:30.621581 nrh-lotr-0.0.1/tests/
--rw-r--r--   0 nhapeman   (501) staff       (20)     1095 2023-06-18 03:02:32.000000 nrh-lotr-0.0.1/tests/test_sdk.py
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.782823 nrh-lotr-0.0.2/
+-rw-r--r--   0 nhapeman   (501) staff       (20)     1069 2023-06-18 02:23:37.000000 nrh-lotr-0.0.2/LICENSE.txt
+-rw-r--r--   0 nhapeman   (501) staff       (20)     3008 2023-06-18 04:02:03.782710 nrh-lotr-0.0.2/PKG-INFO
+-rw-r--r--   0 nhapeman   (501) staff       (20)     1537 2023-06-18 04:00:09.000000 nrh-lotr-0.0.2/README.md
+-rw-r--r--   0 nhapeman   (501) staff       (20)      390 2023-06-18 04:01:13.000000 nrh-lotr-0.0.2/pyproject.toml
+-rw-r--r--   0 nhapeman   (501) staff       (20)       38 2023-06-18 04:02:03.782853 nrh-lotr-0.0.2/setup.cfg
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.781180 nrh-lotr-0.0.2/src/
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.781903 nrh-lotr-0.0.2/src/lotr/
+-rw-r--r--   0 nhapeman   (501) staff       (20)       37 2023-06-18 02:53:17.000000 nrh-lotr-0.0.2/src/lotr/__init__.py
+-rw-r--r--   0 nhapeman   (501) staff       (20)     2216 2023-06-18 03:53:13.000000 nrh-lotr-0.0.2/src/lotr/lotr.py
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.782453 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/
+-rw-r--r--   0 nhapeman   (501) staff       (20)     3008 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/PKG-INFO
+-rw-r--r--   0 nhapeman   (501) staff       (20)      271 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/SOURCES.txt
+-rw-r--r--   0 nhapeman   (501) staff       (20)        1 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/dependency_links.txt
+-rw-r--r--   0 nhapeman   (501) staff       (20)       18 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/requires.txt
+-rw-r--r--   0 nhapeman   (501) staff       (20)        5 2023-06-18 04:02:03.000000 nrh-lotr-0.0.2/src/nrh_lotr.egg-info/top_level.txt
+drwxr-xr-x   0 nhapeman   (501) staff       (20)        0 2023-06-18 04:02:03.782564 nrh-lotr-0.0.2/tests/
+-rw-r--r--   0 nhapeman   (501) staff       (20)     1095 2023-06-18 03:02:32.000000 nrh-lotr-0.0.2/tests/test_sdk.py
```

### Comparing `nrh-lotr-0.0.1/LICENSE.txt` & `nrh-lotr-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nrh-lotr-0.0.1/src/lotr/lotr.py` & `nrh-lotr-0.0.2/src/lotr/lotr.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,36 +62,7 @@
         """Helper for querying api."""
         headers = {"Authorization": f"Bearer {self.api_key}"}
         params = {"limit": limit, "offset": offset}
         url = f"https://the-one-api.dev/v2/{endpoint}"
         resp = requests.get(url, params=params, headers=headers)
         resp.raise_for_status()
         return resp.json()
-
-
-if __name__ == "__main__":
-    # Basic endpoints:
-    # /movie
-    # /movie/{id}
-    # /movie/{id}/{quote}
-    # /quote
-    # /quote/{id}
-
-    # Movie basics.
-    lotr = LOTR()
-    movies = lotr.movies(limit=5)
-    assert len(movies) == 5
-    movie_3 = movies[3]
-    assert lotr.movies(id=movie_3.id)[0] == movie_3
-
-    # Quote basics.
-    quotes = lotr.quotes(limit=7)
-    assert len(quotes) == 7
-    quote_6 = quotes[6]
-    assert lotr.quotes(id=quote_6.id)[0] == quote_6
-
-    # Movie quotes (only works on original 3).
-    all_movies = lotr.movies()
-    two_towers = next(m for m in all_movies if m.name == "The Two Towers")
-    movie_quotes = lotr.movie_quotes(id=two_towers.id, limit=11)
-    assert len(movie_quotes) == 11
-    assert all(isinstance(q, Quote) for q in movie_quotes)
```

### Comparing `nrh-lotr-0.0.1/tests/test_sdk.py` & `nrh-lotr-0.0.2/tests/test_sdk.py`

 * *Files identical despite different names*


# Comparing `tmp/geotribu-0.9.0.tar.gz` & `tmp/geotribu-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotribu-0.9.0.tar", last modified: Fri Jan 13 15:16:31 2023, max compression
+gzip compressed data, was "geotribu-0.9.1.tar", last modified: Fri Jan 13 15:47:56 2023, max compression
```

## Comparing `geotribu-0.9.0.tar` & `geotribu-0.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:16:31.109531 geotribu-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-13 15:16:13.000000 geotribu-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-13 15:16:31.113532 geotribu-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-13 15:16:13.000000 geotribu-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:16:31.109531 geotribu-0.9.0/geotribu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-13 15:16:31.000000 geotribu-0.9.0/geotribu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-13 15:16:31.000000 geotribu-0.9.0/geotribu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 15:16:31.000000 geotribu-0.9.0/geotribu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-13 15:16:31.000000 geotribu-0.9.0/geotribu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-13 15:16:31.000000 geotribu-0.9.0/geotribu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-13 15:16:31.000000 geotribu-0.9.0/geotribu.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:16:31.109531 geotribu-0.9.0/geotribu_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:16:31.109531 geotribu-0.9.0/geotribu_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/subcommands/rss_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/subcommands/search_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/subcommands/search_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:16:31.109531 geotribu-0.9.0/geotribu_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/utils/check_image_size.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8280 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/utils/check_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/utils/file_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/utils/file_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/utils/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/utils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-13 15:16:13.000000 geotribu-0.9.0/geotribu_cli/utils/slugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-13 15:16:31.113532 geotribu-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-01-13 15:16:13.000000 geotribu-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:47:56.993473 geotribu-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-13 15:47:30.000000 geotribu-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-13 15:47:56.993473 geotribu-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-13 15:47:30.000000 geotribu-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:47:56.989473 geotribu-0.9.1/geotribu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-01-13 15:47:56.000000 geotribu-0.9.1/geotribu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-01-13 15:47:56.000000 geotribu-0.9.1/geotribu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 15:47:56.000000 geotribu-0.9.1/geotribu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-13 15:47:56.000000 geotribu-0.9.1/geotribu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-13 15:47:56.000000 geotribu-0.9.1/geotribu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-13 15:47:56.000000 geotribu-0.9.1/geotribu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:47:56.989473 geotribu-0.9.1/geotribu_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:47:56.989473 geotribu-0.9.1/geotribu_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/subcommands/rss_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/subcommands/search_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/subcommands/search_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 15:47:56.993473 geotribu-0.9.1/geotribu_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/utils/check_image_size.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8280 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/utils/check_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/utils/file_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/utils/file_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/utils/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/utils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-13 15:47:30.000000 geotribu-0.9.1/geotribu_cli/utils/slugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-13 15:47:56.993473 geotribu-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-01-13 15:47:30.000000 geotribu-0.9.1/setup.py
```

### Comparing `geotribu-0.9.0/LICENSE` & `geotribu-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/PKG-INFO` & `geotribu-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotribu
-Version: 0.9.0
+Version: 0.9.1
 Summary: Des outils pour faciliter les tâches récurrentes des contributeur/ices de Geotribu.
 Home-page: https://github.com/geotribu/cli/
 Author: Julien Moura (Geotribu)
 Author-email: geotribu@gmail.com
 Keywords: cli, Geotribu, GIS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `geotribu-0.9.0/README.md` & `geotribu-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu.egg-info/PKG-INFO` & `geotribu-0.9.1/geotribu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotribu
-Version: 0.9.0
+Version: 0.9.1
 Summary: Des outils pour faciliter les tâches récurrentes des contributeur/ices de Geotribu.
 Home-page: https://github.com/geotribu/cli/
 Author: Julien Moura (Geotribu)
 Author-email: geotribu@gmail.com
 Keywords: cli, Geotribu, GIS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `geotribu-0.9.0/geotribu.egg-info/SOURCES.txt` & `geotribu-0.9.1/geotribu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/__about__.py` & `geotribu-0.9.1/geotribu_cli/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri_homepage__ = "https://cli.geotribu.fr/"
 __uri_repository__ = "https://github.com/geotribu/cli/"
 __uri_tracker__ = f"{__uri_repository__}issues/"
 
 __uri__ = __uri_repository__
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 __version_info__ = tuple(
     [
         int(num) if num.isdigit() else num
         for num in __version__.replace("-", ".", 1).split(".")
     ]
 )
```

### Comparing `geotribu-0.9.0/geotribu_cli/cli.py` & `geotribu-0.9.1/geotribu_cli/cli.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/constants.py` & `geotribu-0.9.1/geotribu_cli/constants.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/subcommands/rss_reader.py` & `geotribu-0.9.1/geotribu_cli/subcommands/rss_reader.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/subcommands/search_content.py` & `geotribu-0.9.1/geotribu_cli/subcommands/search_content.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,17 +57,19 @@
             title=f"Recherche de contenus - {len(result)} résultats "
             f"avec le terme : {search_term}",
             show_lines=True,
             highlight=True,
             caption=f"{__title__} {__version__}",
         )
 
-        # determine row from first item
-        for k in result[0].keys():
-            table.add_column(header=k.title(), justify="right")
+        # columns
+        table.add_column(header="Titre", justify="left", style="default")
+        table.add_column(header="Type", justify="center", style="bright_black")
+        table.add_column(header="Score", style="magenta")
+        table.add_column(header="URL", justify="right", style="blue")
 
         # iterate over results
         for r in result[:count]:
 
             table.add_row(
                 r.get("titre"),
                 r.get("type"),
@@ -155,14 +157,23 @@
         "--filter-type",
         choices=["article", "rdp"],
         default=None,
         help="Filtrer sur un type de contenu en particulier.",
     )
 
     subparser.add_argument(
+        "-n",
+        "--results-number",
+        type=int,
+        default=5,
+        help="Nombre de résultats à retourner.",
+        dest="results_number",
+    )
+
+    subparser.add_argument(
         "-x",
         "--expiration-rotating-hours",
         help="Nombre d'heures à partir duquel considérer le fichier local comme périmé.",
         default=24 * 7,
         type=int,
         dest="expiration_rotating_hours",
     )
```

### Comparing `geotribu-0.9.0/geotribu_cli/subcommands/search_image.py` & `geotribu-0.9.1/geotribu_cli/subcommands/search_image.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/utils/check_image_size.py` & `geotribu-0.9.1/geotribu_cli/utils/check_image_size.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/utils/check_path.py` & `geotribu-0.9.1/geotribu_cli/utils/check_path.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/utils/file_downloader.py` & `geotribu-0.9.1/geotribu_cli/utils/file_downloader.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/utils/file_stats.py` & `geotribu-0.9.1/geotribu_cli/utils/file_stats.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/utils/formatters.py` & `geotribu-0.9.1/geotribu_cli/utils/formatters.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/utils/proxies.py` & `geotribu-0.9.1/geotribu_cli/utils/proxies.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/geotribu_cli/utils/slugger.py` & `geotribu-0.9.1/geotribu_cli/utils/slugger.py`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/setup.cfg` & `geotribu-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `geotribu-0.9.0/setup.py` & `geotribu-0.9.1/setup.py`

 * *Files identical despite different names*


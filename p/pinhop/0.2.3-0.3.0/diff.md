# Comparing `tmp/pinhop-0.2.3.tar.gz` & `tmp/pinhop-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinhop-0.2.3.tar", last modified: Wed Jan 12 05:28:31 2022, max compression
+gzip compressed data, was "pinhop-0.3.0.tar", last modified: Sun Jun 18 17:23:06 2023, max compression
```

## Comparing `pinhop-0.2.3.tar` & `pinhop-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 05:28:31.679720 pinhop-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-01-12 05:28:31.679720 pinhop-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-01-12 05:28:23.000000 pinhop-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-01-12 05:28:23.000000 pinhop-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-01-12 05:28:31.683720 pinhop-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 05:28:31.679720 pinhop-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 05:28:31.679720 pinhop-0.2.3/src/pinhop/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 05:28:23.000000 pinhop-0.2.3/src/pinhop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13032 2022-01-12 05:28:23.000000 pinhop-0.2.3/src/pinhop/css.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5522 2022-01-12 05:28:23.000000 pinhop-0.2.3/src/pinhop/pinhop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 05:28:31.679720 pinhop-0.2.3/src/pinhop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-01-12 05:28:31.000000 pinhop-0.2.3/src/pinhop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-01-12 05:28:31.000000 pinhop-0.2.3/src/pinhop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 05:28:31.000000 pinhop-0.2.3/src/pinhop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-12 05:28:31.000000 pinhop-0.2.3/src/pinhop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-12 05:28:31.000000 pinhop-0.2.3/src/pinhop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-12 05:28:31.000000 pinhop-0.2.3/src/pinhop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:23:06.571037 pinhop-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-18 17:23:06.571037 pinhop-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-18 17:22:57.000000 pinhop-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-18 17:22:57.000000 pinhop-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-18 17:23:06.571037 pinhop-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:23:06.571037 pinhop-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:23:06.571037 pinhop-0.3.0/src/pinhop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:22:57.000000 pinhop-0.3.0/src/pinhop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-06-18 17:22:57.000000 pinhop-0.3.0/src/pinhop/css.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-06-18 17:22:57.000000 pinhop-0.3.0/src/pinhop/pinhop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:23:06.571037 pinhop-0.3.0/src/pinhop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-18 17:23:06.000000 pinhop-0.3.0/src/pinhop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-18 17:23:06.000000 pinhop-0.3.0/src/pinhop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:23:06.000000 pinhop-0.3.0/src/pinhop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-18 17:23:06.000000 pinhop-0.3.0/src/pinhop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 17:23:06.000000 pinhop-0.3.0/src/pinhop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 17:23:06.000000 pinhop-0.3.0/src/pinhop.egg-info/top_level.txt
```

### Comparing `pinhop-0.2.3/PKG-INFO` & `pinhop-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: pinhop
-Version: 0.2.3
+Version: 0.3.0
 Summary: Timehop for Pinboard
 Home-page: https://github.com/mikepqr/pinhop
 Author: Mike Lee Williams
 Author-email: mike@mike.place
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mikepqr/pinhop/issues
 Project-URL: Source, https://github.com/mikepqr/pinhop
 Keywords: twitter
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Pinhop
 
 Timehop for Pinboard.
 
 Get pinboard posts from a previous month or day as a pinboard-style web page.
@@ -58,9 +55,7 @@
   --install-completion [bash|zsh|fish|powershell|pwsh]
                                   Install completion for the specified shell.
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
                                   copy it or customize the installation.
   --help                          Show this message and exit.
 ```
-
-
```

### Comparing `pinhop-0.2.3/README.md` & `pinhop-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pinhop-0.2.3/setup.cfg` & `pinhop-0.3.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 [metadata]
 name = pinhop
-version = 0.2.3
+version = 0.3.0
 description = Timehop for Pinboard
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mikepqr/pinhop
 author = Mike Lee Williams
 author_email = mike@mike.place
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: End Users/Desktop
 	Topic :: Utilities
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 keywords = twitter
 project_urls = 
 	Bug Reports=https://github.com/mikepqr/pinhop/issues
 	Source=https://github.com/mikepqr/pinhop
 
 [options]
 package_dir = =src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.9
 install_requires = 
 	tqdm
 	typer
 
 [options.packages.find]
 where = src
```

### Comparing `pinhop-0.2.3/src/pinhop/css.py` & `pinhop-0.3.0/src/pinhop/css.py`

 * *Files identical despite different names*

### Comparing `pinhop-0.2.3/src/pinhop/pinhop.py` & `pinhop-0.3.0/src/pinhop/pinhop.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from urllib.request import urlopen
 
 import typer
 from tqdm import tqdm
 
 from pinhop.css import css
 
+auth_token: str
+
 
 def add_auth(params):
     global auth_token
     if not auth_token:
         raise ValueError(
             "Auth token unset. Configure PINBOARD_TOKEN "
             "environment variable or provide --token command line "
@@ -23,23 +25,20 @@
 
 
 def days_of_month(year, month):
     """
     Return list of YYYY-MM-DD strings for all days in year-month.
     """
     days_in_month = calendar.monthrange(year, month)[1]
-    return [
-        "{year}-{month:02d}-{day:02d}".format(year=year, month=month, day=day)
-        for day in range(1, days_in_month + 1)
-    ]
+    return [f"{year}-{month:02d}-{day:02d}" for day in range(1, days_in_month + 1)]
 
 
 def get_day(day):
     params = add_auth({"dt": day})
-    url = "https://api.pinboard.in/v1/posts/get?{}".format(urlencode(params))
+    url = f"https://api.pinboard.in/v1/posts/get?{urlencode(params)}"
     r = urlopen(url)
     return json.loads(r.read())
 
 
 def get_posts_days(days):
     """
     Returns list of posts for list of days (where each day is a YYYY-MM-DD
@@ -56,16 +55,15 @@
     return "<br />".join(extended.strip().split("\n"))
 
 
 def format_tags(post):
     tags = post["tags"].split()
     urls = ["https://pinboard.in/u:{}/t:".format(post["user"]) + tag for tag in tags]
     return "&nbsp;".join(
-        '<a class="tag" href="{url}">{tag}</a>'.format(url=url, tag=tag)
-        for tag, url in zip(tags, urls)
+        f'<a class="tag" href="{url}">{tag}</a>' for tag, url in zip(tags, urls)
     )
 
 
 def format_time(isotime):
     return isotime[:10]
```

### Comparing `pinhop-0.2.3/src/pinhop.egg-info/PKG-INFO` & `pinhop-0.3.0/src/pinhop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: pinhop
-Version: 0.2.3
+Version: 0.3.0
 Summary: Timehop for Pinboard
 Home-page: https://github.com/mikepqr/pinhop
 Author: Mike Lee Williams
 Author-email: mike@mike.place
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mikepqr/pinhop/issues
 Project-URL: Source, https://github.com/mikepqr/pinhop
 Keywords: twitter
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Pinhop
 
 Timehop for Pinboard.
 
 Get pinboard posts from a previous month or day as a pinboard-style web page.
@@ -58,9 +55,7 @@
   --install-completion [bash|zsh|fish|powershell|pwsh]
                                   Install completion for the specified shell.
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
                                   copy it or customize the installation.
   --help                          Show this message and exit.
 ```
-
-
```


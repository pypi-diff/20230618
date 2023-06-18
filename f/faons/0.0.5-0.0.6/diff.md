# Comparing `tmp/faons-0.0.5.tar.gz` & `tmp/faons-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faons-0.0.5.tar", last modified: Sun Jun 18 08:53:54 2023, max compression
+gzip compressed data, was "faons-0.0.6.tar", last modified: Sun Jun 18 10:20:24 2023, max compression
```

## Comparing `faons-0.0.5.tar` & `faons-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-18 08:53:54.333751 faons-0.0.5/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2344 2023-06-18 08:53:54.330754 faons-0.0.5/PKG-INFO
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2240 2023-06-18 08:53:32.000000 faons-0.0.5/README.md
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-18 08:53:54.194041 faons-0.0.5/faons/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 04:50:06.000000 faons-0.0.5/faons/__init__.py
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)    14636 2023-06-18 08:49:00.000000 faons-0.0.5/faons/cli.py
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-18 08:53:54.310492 faons-0.0.5/faons.egg-info/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2344 2023-06-18 08:53:53.000000 faons-0.0.5/faons.egg-info/PKG-INFO
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)      225 2023-06-18 08:53:54.000000 faons-0.0.5/faons.egg-info/SOURCES.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        1 2023-06-18 08:53:53.000000 faons-0.0.5/faons.egg-info/dependency_links.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       42 2023-06-18 08:53:53.000000 faons-0.0.5/faons.egg-info/entry_points.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       61 2023-06-18 08:53:53.000000 faons-0.0.5/faons.egg-info/requires.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        6 2023-06-18 08:53:53.000000 faons-0.0.5/faons.egg-info/top_level.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       38 2023-06-18 08:53:54.334886 faons-0.0.5/setup.cfg
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)      585 2023-06-10 03:59:22.000000 faons-0.0.5/setup.py
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-18 10:20:24.835323 faons-0.0.6/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2741 2023-06-18 10:20:24.829243 faons-0.0.6/PKG-INFO
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2641 2023-06-18 10:20:19.000000 faons-0.0.6/README.md
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-18 10:20:24.466139 faons-0.0.6/faons/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 04:50:06.000000 faons-0.0.6/faons/__init__.py
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)    22065 2023-06-18 10:13:19.000000 faons-0.0.6/faons/cli.py
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-18 10:20:24.770753 faons-0.0.6/faons.egg-info/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2741 2023-06-18 10:20:23.000000 faons-0.0.6/faons.egg-info/PKG-INFO
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)      225 2023-06-18 10:20:24.000000 faons-0.0.6/faons.egg-info/SOURCES.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        1 2023-06-18 10:20:23.000000 faons-0.0.6/faons.egg-info/dependency_links.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       42 2023-06-18 10:20:23.000000 faons-0.0.6/faons.egg-info/entry_points.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       61 2023-06-18 10:20:23.000000 faons-0.0.6/faons.egg-info/requires.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        6 2023-06-18 10:20:23.000000 faons-0.0.6/faons.egg-info/top_level.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       38 2023-06-18 10:20:24.838184 faons-0.0.6/setup.cfg
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)      585 2023-06-18 10:12:27.000000 faons-0.0.6/setup.py
```

### Comparing `faons-0.0.5/PKG-INFO` & `faons-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faons
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Welcome to Fast API on Steroids(FAONS)!
 
@@ -42,9 +42,13 @@
 
 ## Creating you first app for your project
 
 FAONS inherit the idea of creating apps from Django. We will be creating different apps to separate different modules in our application. We can create apps by using the command `faons startapp <app_name>` . Once done the app folder will be created inside the `src/core` folder.
 
 ## Updating your schema to the DB
 
-One useful feature that we missed while coming from django to fastapi was that it lacked the feature to migrate the schema to its db easily. With faons v 0.0.4 we included a function do exactly the same thing. You can use the command `faons updateschema` which will create, alter or drop tables based on the changes that you make to the `schema.py` in the apps. From faons v 0.0.5 we started to create an additional table faons_schema which will be used to track the table names. This table was included to avoid issues due to an upcoming feature to export models to db like exporting schema.
+One useful feature that we missed while coming from django to fastapi was that it lacked the feature to migrate the schema to its db easily. With faons v 0.0.4 we included a function do exactly the same thing. You can use the command `faons updateschema` which will create, alter or drop tables based on the changes that you make to the `schema.py` in the apps. From faons v 0.0.5 we started to create an additional table faons_schema which will be used to track the table names. This table was included to avoid issues like deleting tables exported from models file.
+
+## Migrating models to DB
+
+Just like exporting schema to DB the ability to export models directly to you DB has been added to faons from v 0.0.6. You can use the command `faons updatemodels` which will create, alter or drop tables based on the changes that you make to the `models.py` in the apps. This command also creates a table called faons_models which will be used to track the table names created from the models.
```

### Comparing `faons-0.0.5/README.md` & `faons-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,8 +34,12 @@
 
 ## Creating you first app for your project
 
 FAONS inherit the idea of creating apps from Django. We will be creating different apps to separate different modules in our application. We can create apps by using the command `faons startapp <app_name>` . Once done the app folder will be created inside the `src/core` folder.
 
 ## Updating your schema to the DB
 
-One useful feature that we missed while coming from django to fastapi was that it lacked the feature to migrate the schema to its db easily. With faons v 0.0.4 we included a function do exactly the same thing. You can use the command `faons updateschema` which will create, alter or drop tables based on the changes that you make to the `schema.py` in the apps. From faons v 0.0.5 we started to create an additional table faons_schema which will be used to track the table names. This table was included to avoid issues due to an upcoming feature to export models to db like exporting schema.
+One useful feature that we missed while coming from django to fastapi was that it lacked the feature to migrate the schema to its db easily. With faons v 0.0.4 we included a function do exactly the same thing. You can use the command `faons updateschema` which will create, alter or drop tables based on the changes that you make to the `schema.py` in the apps. From faons v 0.0.5 we started to create an additional table faons_schema which will be used to track the table names. This table was included to avoid issues like deleting tables exported from models file.
+
+## Migrating models to DB
+
+Just like exporting schema to DB the ability to export models directly to you DB has been added to faons from v 0.0.6. You can use the command `faons updatemodels` which will create, alter or drop tables based on the changes that you make to the `models.py` in the apps. This command also creates a table called faons_models which will be used to track the table names created from the models.
```

### Comparing `faons-0.0.5/faons.egg-info/PKG-INFO` & `faons-0.0.6/faons.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faons
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Welcome to Fast API on Steroids(FAONS)!
 
@@ -42,9 +42,13 @@
 
 ## Creating you first app for your project
 
 FAONS inherit the idea of creating apps from Django. We will be creating different apps to separate different modules in our application. We can create apps by using the command `faons startapp <app_name>` . Once done the app folder will be created inside the `src/core` folder.
 
 ## Updating your schema to the DB
 
-One useful feature that we missed while coming from django to fastapi was that it lacked the feature to migrate the schema to its db easily. With faons v 0.0.4 we included a function do exactly the same thing. You can use the command `faons updateschema` which will create, alter or drop tables based on the changes that you make to the `schema.py` in the apps. From faons v 0.0.5 we started to create an additional table faons_schema which will be used to track the table names. This table was included to avoid issues due to an upcoming feature to export models to db like exporting schema.
+One useful feature that we missed while coming from django to fastapi was that it lacked the feature to migrate the schema to its db easily. With faons v 0.0.4 we included a function do exactly the same thing. You can use the command `faons updateschema` which will create, alter or drop tables based on the changes that you make to the `schema.py` in the apps. From faons v 0.0.5 we started to create an additional table faons_schema which will be used to track the table names. This table was included to avoid issues like deleting tables exported from models file.
+
+## Migrating models to DB
+
+Just like exporting schema to DB the ability to export models directly to you DB has been added to faons from v 0.0.6. You can use the command `faons updatemodels` which will create, alter or drop tables based on the changes that you make to the `models.py` in the apps. This command also creates a table called faons_models which will be used to track the table names created from the models.
```

### Comparing `faons-0.0.5/setup.py` & `faons-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faons',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             'faons = faons.cli:faons'
         ]
```


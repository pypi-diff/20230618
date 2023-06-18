# Comparing `tmp/openapi-core-0.8.0.tar.gz` & `tmp/openapi-core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openapi-core-0.8.0.tar", last modified: Thu Feb 28 14:22:42 2019, max compression
+gzip compressed data, was "dist/openapi-core-0.9.0.tar", last modified: Fri Mar 22 14:57:32 2019, max compression
```

## Comparing `openapi-core-0.8.0.tar` & `openapi-core-0.9.0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1501 2019-02-28 14:21:57.000000 openapi-core-0.8.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2019-02-28 14:21:57.000000 openapi-core-0.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     6599 2019-02-28 14:22:42.000000 openapi-core-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4540 2019-02-28 14:21:57.000000 openapi-core-0.8.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/
--rw-rw-r--   0 travis    (2000) travis    (2000)      423 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      340 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/compat.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/extensions/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/extensions/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/extensions/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/extensions/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      656 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/extensions/models/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/extensions/models/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/components/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      457 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/components/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/content/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/content/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      384 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/content/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      505 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/content/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/infos/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/infos/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      409 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/infos/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/infos/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/media_types/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/media_types/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/media_types/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      938 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/media_types/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1575 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/media_types/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/operations/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/operations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/operations/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/operations/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1281 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/operations/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/parameters/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/parameters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      508 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/parameters/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      919 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/parameters/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1162 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/parameters/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      997 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/parameters/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3890 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/parameters/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/paths/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/paths/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      846 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/paths/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      295 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/paths/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/properties/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/properties/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      589 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/properties/generators.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/request_bodies/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/request_bodies/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      295 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/request_bodies/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      929 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/request_bodies/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      848 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/request_bodies/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/responses/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      503 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/responses/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1519 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/responses/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1115 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/responses/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      494 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1941 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3518 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      588 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21534 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      895 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/registries.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      574 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      601 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/schemas/validators.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/servers/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/servers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      329 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/servers/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/servers/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      829 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/servers/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/schema/specs/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/specs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/specs/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1827 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/schema/specs/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2265 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/shortcuts.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/validation/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      235 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/models.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/validation/request/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/request/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      961 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/request/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2893 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/request/validators.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/validation/response/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/response/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/response/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/response/validators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/validation/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core/wrappers/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/wrappers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1276 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/wrappers/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1342 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/wrappers/flask.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2019-02-28 14:21:57.000000 openapi-core-0.8.0/openapi_core/wrappers/mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6599 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3277 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-02-28 14:22:42.000000 openapi-core-0.8.0/openapi_core.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-02-28 14:21:57.000000 openapi-core-0.8.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2019-02-28 14:21:57.000000 openapi-core-0.8.0/requirements_2.7.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2019-02-28 14:21:57.000000 openapi-core-0.8.0/requirements_dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-02-28 14:22:42.000000 openapi-core-0.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2693 2019-02-28 14:21:57.000000 openapi-core-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1501 2019-03-22 14:56:49.000000 openapi-core-0.9.0/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      118 2019-03-22 14:56:49.000000 openapi-core-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6599 2019-03-22 14:57:32.000000 openapi-core-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4540 2019-03-22 14:56:49.000000 openapi-core-0.9.0/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      423 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      340 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/compat.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/extensions/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/extensions/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/extensions/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/extensions/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      656 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/extensions/models/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/extensions/models/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/components/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      457 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/components/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/content/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/content/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      384 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/content/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      505 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/content/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      138 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/infos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/infos/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      409 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/infos/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/infos/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/media_types/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/media_types/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      520 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/media_types/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      938 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/media_types/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1575 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/media_types/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/operations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/operations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      392 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/operations/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/operations/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1281 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/operations/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/parameters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/parameters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      508 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/parameters/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      919 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/parameters/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1162 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/parameters/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      997 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/parameters/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3967 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/parameters/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/paths/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/paths/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      846 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/paths/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      295 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/paths/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/properties/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/properties/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      589 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/properties/generators.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/request_bodies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/request_bodies/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      295 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/request_bodies/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      929 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/request_bodies/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      848 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/request_bodies/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/responses/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      503 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/responses/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1519 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/responses/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1115 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/responses/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/schemas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      494 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1941 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3618 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      588 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23085 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      895 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/registries.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      830 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      601 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/schemas/validators.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/servers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/servers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      329 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/servers/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1458 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/servers/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      829 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/servers/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/schema/specs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/specs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2141 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/specs/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1827 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/schema/specs/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2265 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/shortcuts.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/validation/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      235 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/models.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/validation/request/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/request/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      961 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/request/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2893 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/request/validators.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/validation/response/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/response/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      350 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/response/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2542 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/response/validators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/validation/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core/wrappers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/wrappers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1276 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/wrappers/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1342 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/wrappers/flask.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1042 2019-03-22 14:56:49.000000 openapi-core-0.9.0/openapi_core/wrappers/mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6599 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3277 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2019-03-22 14:57:32.000000 openapi-core-0.9.0/openapi_core.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-22 14:56:49.000000 openapi-core-0.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      137 2019-03-22 14:56:49.000000 openapi-core-0.9.0/requirements_2.7.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2019-03-22 14:56:49.000000 openapi-core-0.9.0/requirements_dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-22 14:57:32.000000 openapi-core-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2693 2019-03-22 14:56:49.000000 openapi-core-0.9.0/setup.py
```

### Comparing `openapi-core-0.8.0/LICENSE` & `openapi-core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/PKG-INFO` & `openapi-core-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/p1c2u/openapi-core
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 License: UNKNOWN
 Description: openapi-core
         ************
```

### Comparing `openapi-core-0.8.0/README.rst` & `openapi-core-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/extensions/models/factories.py` & `openapi-core-0.9.0/openapi_core/extensions/models/factories.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/extensions/models/models.py` & `openapi-core-0.9.0/openapi_core/extensions/models/models.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/components/factories.py` & `openapi-core-0.9.0/openapi_core/schema/components/factories.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/media_types/exceptions.py` & `openapi-core-0.9.0/openapi_core/schema/media_types/exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/media_types/generators.py` & `openapi-core-0.9.0/openapi_core/schema/media_types/generators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/media_types/models.py` & `openapi-core-0.9.0/openapi_core/schema/media_types/models.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/operations/generators.py` & `openapi-core-0.9.0/openapi_core/schema/operations/generators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/operations/models.py` & `openapi-core-0.9.0/openapi_core/schema/operations/models.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/parameters/exceptions.py` & `openapi-core-0.9.0/openapi_core/schema/parameters/exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/parameters/factories.py` & `openapi-core-0.9.0/openapi_core/schema/parameters/factories.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/parameters/generators.py` & `openapi-core-0.9.0/openapi_core/schema/parameters/generators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/parameters/models.py` & `openapi-core-0.9.0/openapi_core/schema/parameters/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,19 @@
 
         try:
             deserialized = self.deserialize(value)
         except (ValueError, AttributeError) as exc:
             raise InvalidParameterValue(self.name, exc)
 
         try:
-            unmarshalled = self.schema.unmarshal(deserialized, custom_formatters=custom_formatters)
+            unmarshalled = self.schema.unmarshal(
+                deserialized,
+                custom_formatters=custom_formatters,
+                strict=False,
+            )
         except OpenAPISchemaError as exc:
             raise InvalidParameterValue(self.name, exc)
 
         try:
             return self.schema.validate(unmarshalled, custom_formatters=custom_formatters)
         except OpenAPISchemaError as exc:
             raise InvalidParameterValue(self.name, exc)
```

### Comparing `openapi-core-0.8.0/openapi_core/schema/paths/generators.py` & `openapi-core-0.9.0/openapi_core/schema/paths/generators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/properties/generators.py` & `openapi-core-0.9.0/openapi_core/schema/properties/generators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/request_bodies/factories.py` & `openapi-core-0.9.0/openapi_core/schema/request_bodies/factories.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/request_bodies/models.py` & `openapi-core-0.9.0/openapi_core/schema/request_bodies/models.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/responses/generators.py` & `openapi-core-0.9.0/openapi_core/schema/responses/generators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/responses/models.py` & `openapi-core-0.9.0/openapi_core/schema/responses/models.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/schemas/exceptions.py` & `openapi-core-0.9.0/openapi_core/schema/schemas/exceptions.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/schemas/factories.py` & `openapi-core-0.9.0/openapi_core/schema/schemas/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
         properties_spec = schema_deref.get('properties', None)
         items_spec = schema_deref.get('items', None)
         nullable = schema_deref.get('nullable', False)
         enum = schema_deref.get('enum', None)
         deprecated = schema_deref.get('deprecated', False)
         all_of_spec = schema_deref.get('allOf', None)
         one_of_spec = schema_deref.get('oneOf', None)
-        additional_properties_spec = schema_deref.get('additionalProperties')
+        additional_properties_spec = schema_deref.get('additionalProperties',
+                                                      True)
         min_items = schema_deref.get('minItems', None)
         max_items = schema_deref.get('maxItems', None)
         min_length = schema_deref.get('minLength', None)
         max_length = schema_deref.get('maxLength', None)
         pattern = schema_deref.get('pattern', None)
         unique_items = schema_deref.get('uniqueItems', None)
         minimum = schema_deref.get('minimum', None)
@@ -55,16 +56,16 @@
         if one_of_spec:
             one_of = map(self.create, one_of_spec)
 
         items = None
         if items_spec:
             items = self._create_items(items_spec)
 
-        additional_properties = None
-        if additional_properties_spec:
+        additional_properties = additional_properties_spec
+        if isinstance(additional_properties_spec, dict):
             additional_properties = self.create(additional_properties_spec)
 
         return Schema(
             schema_type=schema_type, model=model, properties=properties,
             items=items, schema_format=schema_format, required=required,
             default=default, nullable=nullable, enum=enum,
             deprecated=deprecated, all_of=all_of, one_of=one_of,
```

### Comparing `openapi-core-0.8.0/openapi_core/schema/schemas/generators.py` & `openapi-core-0.9.0/openapi_core/schema/schemas/generators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/schemas/models.py` & `openapi-core-0.9.0/openapi_core/schema/schemas/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from openapi_core.schema.schemas.enums import SchemaFormat, SchemaType
 from openapi_core.schema.schemas.exceptions import (
     InvalidSchemaValue, UndefinedSchemaProperty, MissingSchemaProperty,
     OpenAPISchemaError, NoOneOfSchema, MultipleOneOfSchema, NoValidSchema,
     UndefinedItemsSchema, InvalidCustomFormatSchemaValue, InvalidSchemaProperty,
 )
 from openapi_core.schema.schemas.util import (
-    forcebool, format_date, format_datetime,
+    forcebool, format_date, format_datetime, format_byte, format_uuid,
 )
 from openapi_core.schema.schemas.validators import (
     TypeValidator, AttributeValidator,
 )
 
 log = logging.getLogger(__name__)
 
@@ -34,27 +34,24 @@
     validate = attr.ib()
 
 
 class Schema(object):
     """Represents an OpenAPI Schema."""
 
     DEFAULT_CAST_CALLABLE_GETTER = {
-        SchemaType.INTEGER: int,
-        SchemaType.NUMBER: float,
-        SchemaType.BOOLEAN: forcebool,
     }
 
     STRING_FORMAT_CALLABLE_GETTER = {
         SchemaFormat.NONE: Format(text_type, TypeValidator(text_type)),
         SchemaFormat.DATE: Format(
             format_date, TypeValidator(date, exclude=datetime)),
         SchemaFormat.DATETIME: Format(format_datetime, TypeValidator(datetime)),
         SchemaFormat.BINARY: Format(binary_type, TypeValidator(binary_type)),
-        SchemaFormat.UUID: Format(UUID, TypeValidator(UUID)),
-        SchemaFormat.BYTE: Format(b64decode, TypeValidator(binary_type)),
+        SchemaFormat.UUID: Format(format_uuid, TypeValidator(UUID)),
+        SchemaFormat.BYTE: Format(format_byte, TypeValidator(text_type)),
     }
 
     TYPE_VALIDATOR_CALLABLE_GETTER = {
         SchemaType.ANY: lambda x: True,
         SchemaType.BOOLEAN: TypeValidator(bool),
         SchemaType.INTEGER: TypeValidator(integer_types, exclude=bool),
         SchemaType.NUMBER: TypeValidator(integer_types, float, exclude=bool),
@@ -64,15 +61,15 @@
         SchemaType.OBJECT: AttributeValidator('__dict__'),
     }
 
     def __init__(
             self, schema_type=None, model=None, properties=None, items=None,
             schema_format=None, required=None, default=None, nullable=False,
             enum=None, deprecated=False, all_of=None, one_of=None,
-            additional_properties=None, min_items=None, max_items=None,
+            additional_properties=True, min_items=None, max_items=None,
             min_length=None, max_length=None, pattern=None, unique_items=False,
             minimum=None, maximum=None, multiple_of=None,
             exclusive_minimum=False, exclusive_maximum=False,
             min_properties=None, max_properties=None):
         self.type = SchemaType(schema_type)
         self.model = model
         self.properties = properties and dict(properties) or {}
@@ -144,63 +141,70 @@
 
         for subschema in self.all_of:
             subschema_req = subschema.get_all_required_properties()
             required += subschema_req
 
         return set(required)
 
-    def get_cast_mapping(self, custom_formatters=None):
+    def get_cast_mapping(self, custom_formatters=None, strict=True):
         pass_defaults = lambda f: functools.partial(
-          f, custom_formatters=custom_formatters)
+          f, custom_formatters=custom_formatters, strict=strict)
         mapping = self.DEFAULT_CAST_CALLABLE_GETTER.copy()
         mapping.update({
             SchemaType.STRING: pass_defaults(self._unmarshal_string),
+            SchemaType.BOOLEAN: pass_defaults(self._unmarshal_boolean),
+            SchemaType.INTEGER: pass_defaults(self._unmarshal_integer),
+            SchemaType.NUMBER: pass_defaults(self._unmarshal_number),
             SchemaType.ANY: pass_defaults(self._unmarshal_any),
             SchemaType.ARRAY: pass_defaults(self._unmarshal_collection),
             SchemaType.OBJECT: pass_defaults(self._unmarshal_object),
         })
 
         return defaultdict(lambda: lambda x: x, mapping)
 
-    def cast(self, value, custom_formatters=None):
+    def cast(self, value, custom_formatters=None, strict=True):
         """Cast value to schema type"""
         if value is None:
             if not self.nullable:
                 raise InvalidSchemaValue("Null value for non-nullable schema", value, self.type)
             return self.default
 
-        cast_mapping = self.get_cast_mapping(custom_formatters=custom_formatters)
+        cast_mapping = self.get_cast_mapping(
+            custom_formatters=custom_formatters, strict=strict)
 
         if self.type is not SchemaType.STRING and value == '':
             return None
 
         cast_callable = cast_mapping[self.type]
         try:
             return cast_callable(value)
         except ValueError:
             raise InvalidSchemaValue(
                 "Failed to cast value {value} to type {type}", value, self.type)
 
-    def unmarshal(self, value, custom_formatters=None):
+    def unmarshal(self, value, custom_formatters=None, strict=True):
         """Unmarshal parameter from the value."""
         if self.deprecated:
             warnings.warn("The schema is deprecated", DeprecationWarning)
 
-        casted = self.cast(value, custom_formatters=custom_formatters)
+        casted = self.cast(value, custom_formatters=custom_formatters, strict=strict)
 
         if casted is None and not self.required:
             return None
 
         if self.enum and casted not in self.enum:
             raise InvalidSchemaValue(
                 "Value {value} not in enum choices: {type}", value, self.enum)
 
         return casted
 
-    def _unmarshal_string(self, value, custom_formatters=None):
+    def _unmarshal_string(self, value, custom_formatters=None, strict=True):
+        if strict and not isinstance(value, (text_type, binary_type)):
+            raise InvalidSchemaValue("Value {value} is not of type {type}", value, self.type)
+
         try:
             schema_format = SchemaFormat(self.format)
         except ValueError:
             msg = "Unsupported format {type} unmarshalling for value {value}"
             if custom_formatters is not None:
                 formatstring = custom_formatters.get(self.format)
                 if formatstring is None:
@@ -212,15 +216,33 @@
 
         try:
             return formatstring.unmarshal(value)
         except ValueError as exc:
             raise InvalidCustomFormatSchemaValue(
                 "Failed to format value {value} to format {type}: {exception}", value, self.format, exc)
 
-    def _unmarshal_any(self, value, custom_formatters=None):
+    def _unmarshal_integer(self, value, custom_formatters=None, strict=True):
+        if strict and not isinstance(value, (integer_types, )):
+            raise InvalidSchemaValue("Value {value} is not of type {type}", value, self.type)
+
+        return int(value)
+
+    def _unmarshal_number(self, value, custom_formatters=None, strict=True):
+        if strict and not isinstance(value, (float, )):
+            raise InvalidSchemaValue("Value {value} is not of type {type}", value, self.type)
+
+        return float(value)
+
+    def _unmarshal_boolean(self, value, custom_formatters=None, strict=True):
+        if strict and not isinstance(value, (bool, )):
+            raise InvalidSchemaValue("Value {value} is not of type {type}", value, self.type)
+
+        return forcebool(value)
+
+    def _unmarshal_any(self, value, custom_formatters=None, strict=True):
         types_resolve_order = [
             SchemaType.OBJECT, SchemaType.ARRAY, SchemaType.BOOLEAN,
             SchemaType.INTEGER, SchemaType.NUMBER, SchemaType.STRING,
         ]
         cast_mapping = self.get_cast_mapping()
         for schema_type in types_resolve_order:
             cast_callable = cast_mapping[schema_type]
@@ -228,24 +250,29 @@
                 return cast_callable(value)
             # @todo: remove ValueError when validation separated
             except (OpenAPISchemaError, TypeError, ValueError):
                 continue
 
         raise NoValidSchema(value)
 
-    def _unmarshal_collection(self, value, custom_formatters=None):
+    def _unmarshal_collection(self, value, custom_formatters=None, strict=True):
+        if not isinstance(value, (list, tuple)):
+            raise InvalidSchemaValue("Value {value} is not of type {type}", value, self.type)
+
         if self.items is None:
             raise UndefinedItemsSchema(self.type)
 
-        f = functools.partial(self.items.unmarshal,
-                              custom_formatters=custom_formatters)
+        f = functools.partial(
+            self.items.unmarshal,
+            custom_formatters=custom_formatters, strict=strict,
+        )
         return list(map(f, value))
 
     def _unmarshal_object(self, value, model_factory=None,
-                          custom_formatters=None):
+                          custom_formatters=None, strict=True):
         if not isinstance(value, (dict, )):
             raise InvalidSchemaValue("Value {value} is not of type {type}", value, self.type)
 
         model_factory = model_factory or ModelFactory()
 
         if self.one_of:
             properties = None
@@ -266,36 +293,37 @@
         else:
             properties = self._unmarshal_properties(
               value, custom_formatters=custom_formatters)
 
         return model_factory.create(properties, name=self.model)
 
     def _unmarshal_properties(self, value, one_of_schema=None,
-                              custom_formatters=None):
+                              custom_formatters=None, strict=True):
         all_props = self.get_all_properties()
         all_props_names = self.get_all_properties_names()
         all_req_props_names = self.get_all_required_properties_names()
 
         if one_of_schema is not None:
             all_props.update(one_of_schema.get_all_properties())
             all_props_names |= one_of_schema.\
                 get_all_properties_names()
             all_req_props_names |= one_of_schema.\
                 get_all_required_properties_names()
 
         value_props_names = value.keys()
         extra_props = set(value_props_names) - set(all_props_names)
-        if extra_props and self.additional_properties is None:
+        if extra_props and self.additional_properties is False:
             raise UndefinedSchemaProperty(extra_props)
 
         properties = {}
-        for prop_name in extra_props:
-            prop_value = value[prop_name]
-            properties[prop_name] = self.additional_properties.unmarshal(
-                prop_value, custom_formatters=custom_formatters)
+        if self.additional_properties is not True:
+            for prop_name in extra_props:
+                prop_value = value[prop_name]
+                properties[prop_name] = self.additional_properties.unmarshal(
+                    prop_value, custom_formatters=custom_formatters)
 
         for prop_name, prop in iteritems(all_props):
             try:
                 prop_value = value[prop_name]
             except KeyError:
                 if prop_name in all_req_props_names:
                     raise MissingSchemaProperty(prop_name)
@@ -511,21 +539,22 @@
             all_props_names |= one_of_schema.\
                 get_all_properties_names()
             all_req_props_names |= one_of_schema.\
                 get_all_required_properties_names()
 
         value_props_names = value.keys()
         extra_props = set(value_props_names) - set(all_props_names)
-        if extra_props and self.additional_properties is None:
+        if extra_props and self.additional_properties is False:
             raise UndefinedSchemaProperty(extra_props)
 
-        for prop_name in extra_props:
-            prop_value = value[prop_name]
-            self.additional_properties.validate(
-                prop_value, custom_formatters=custom_formatters)
+        if self.additional_properties is not True:
+            for prop_name in extra_props:
+                prop_value = value[prop_name]
+                self.additional_properties.validate(
+                    prop_value, custom_formatters=custom_formatters)
 
         for prop_name, prop in iteritems(all_props):
             try:
                 prop_value = value[prop_name]
             except KeyError:
                 if prop_name in all_req_props_names:
                     raise MissingSchemaProperty(prop_name)
```

### Comparing `openapi-core-0.8.0/openapi_core/schema/schemas/registries.py` & `openapi-core-0.9.0/openapi_core/schema/schemas/registries.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/schemas/validators.py` & `openapi-core-0.9.0/openapi_core/schema/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/servers/generators.py` & `openapi-core-0.9.0/openapi_core/schema/servers/generators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/servers/models.py` & `openapi-core-0.9.0/openapi_core/schema/servers/models.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/specs/factories.py` & `openapi-core-0.9.0/openapi_core/schema/specs/factories.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/schema/specs/models.py` & `openapi-core-0.9.0/openapi_core/schema/specs/models.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/shortcuts.py` & `openapi-core-0.9.0/openapi_core/shortcuts.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/validation/request/models.py` & `openapi-core-0.9.0/openapi_core/validation/request/models.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/validation/request/validators.py` & `openapi-core-0.9.0/openapi_core/validation/request/validators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/validation/response/validators.py` & `openapi-core-0.9.0/openapi_core/validation/response/validators.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/validation/util.py` & `openapi-core-0.9.0/openapi_core/validation/util.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/wrappers/base.py` & `openapi-core-0.9.0/openapi_core/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/wrappers/flask.py` & `openapi-core-0.9.0/openapi_core/wrappers/flask.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core/wrappers/mock.py` & `openapi-core-0.9.0/openapi_core/wrappers/mock.py`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/openapi_core.egg-info/PKG-INFO` & `openapi-core-0.9.0/openapi_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/p1c2u/openapi-core
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
 License: UNKNOWN
 Description: openapi-core
         ************
```

### Comparing `openapi-core-0.8.0/openapi_core.egg-info/SOURCES.txt` & `openapi-core-0.9.0/openapi_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapi-core-0.8.0/setup.py` & `openapi-core-0.9.0/setup.py`

 * *Files identical despite different names*


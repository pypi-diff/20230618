# Comparing `tmp/polyfactory-2.3.1.tar.gz` & `tmp/polyfactory-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.3.1.tar", max compression
+gzip compressed data, was "polyfactory-2.3.2.tar", max compression
```

## Comparing `polyfactory-2.3.1.tar` & `polyfactory-2.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1092 2023-06-18 10:58:40.409414 polyfactory-2.3.1/LICENSE
--rw-r--r--   0        0        0     9446 2023-06-18 10:58:40.409414 polyfactory-2.3.1/README.md
--rw-r--r--   0        0        0      425 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/__init__.py
--rw-r--r--   0        0        0      825 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    32143 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1876 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     6873 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2217 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    10876 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1516 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     7410 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3329 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/py.typed
--rw-r--r--   0        0        0     2891 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3402 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     2834 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1880 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13607 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      522 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      529 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      535 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3636 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6186 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6257 2023-06-18 10:58:40.417415 polyfactory-2.3.1/pyproject.toml
--rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 polyfactory-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-18 19:05:35.362617 polyfactory-2.3.2/LICENSE
+-rw-r--r--   0        0        0     9446 2023-06-18 19:05:35.362617 polyfactory-2.3.2/README.md
+-rw-r--r--   0        0        0      425 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/__init__.py
+-rw-r--r--   0        0        0      825 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    32143 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1876 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     6873 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2217 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    10876 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1516 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     7410 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3329 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/py.typed
+-rw-r--r--   0        0        0     2891 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3402 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1880 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13607 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      522 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      529 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      535 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3636 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6186 2023-06-18 19:05:35.366617 polyfactory-2.3.2/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6257 2023-06-18 19:05:35.366617 polyfactory-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 polyfactory-2.3.2/PKG-INFO
```

### Comparing `polyfactory-2.3.1/LICENSE` & `polyfactory-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/README.md` & `polyfactory-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/constants.py` & `polyfactory-2.3.2/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/decorators.py` & `polyfactory-2.3.2/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/exceptions.py` & `polyfactory-2.3.2/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/factories/base.py` & `polyfactory-2.3.2/polyfactory/factories/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
 
         :returns: An arbitrary value.
 
         """
         if cls.is_ignored_type(field_meta.annotation):
             return None
 
-        if field_meta.constraints and field_meta.constraints.get("constant", False):
+        if field_meta.constraints and field_meta.constraints.pop("constant", False):
             return field_meta.default
 
         if cls.should_set_none_value(field_meta=field_meta):
             return None
 
         unwrapped_annotation = unwrap_annotation(field_meta.annotation, random=cls.__random__)
```

### Comparing `polyfactory-2.3.1/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.3.2/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.3.2/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.3.2/polyfactory/factories/msgspec_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.3.2/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.3.2/polyfactory/factories/pydantic_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.3.2/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/field_meta.py` & `polyfactory-2.3.2/polyfactory/field_meta.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/fields.py` & `polyfactory-2.3.2/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/persistence.py` & `polyfactory-2.3.2/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/pytest_plugin.py` & `polyfactory-2.3.2/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/utils/helpers.py` & `polyfactory-2.3.2/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/utils/predicates.py` & `polyfactory-2.3.2/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/complex_types.py` & `polyfactory-2.3.2/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.3.2/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.3.2/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.3.2/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/constrained_path.py` & `polyfactory-2.3.2/polyfactory/value_generators/constrained_path.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.3.2/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/constrained_url.py` & `polyfactory-2.3.2/polyfactory/value_generators/constrained_url.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/constrained_uuid.py` & `polyfactory-2.3.2/polyfactory/value_generators/constrained_uuid.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/primitives.py` & `polyfactory-2.3.2/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/polyfactory/value_generators/regex.py` & `polyfactory-2.3.2/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.1/pyproject.toml` & `polyfactory-2.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.3.1"
+version = "2.3.2"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
```

### Comparing `polyfactory-2.3.1/PKG-INFO` & `polyfactory-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.3.1
+Version: 2.3.2
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
```


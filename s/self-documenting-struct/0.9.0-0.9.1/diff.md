# Comparing `tmp/self_documenting_struct-0.9.0.tar.gz` & `tmp/self_documenting_struct-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "self_documenting_struct-0.9.0.tar", last modified: Sun Jun 18 00:16:29 2023, max compression
+gzip compressed data, was "self_documenting_struct-0.9.1.tar", last modified: Sun Jun 18 01:39:34 2023, max compression
```

## Comparing `self_documenting_struct-0.9.0.tar` & `self_documenting_struct-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 developer   (501) staff       (20)        0 2023-06-18 00:16:29.049731 self_documenting_struct-0.9.0/
--rw-r--r--   0 developer   (501) staff       (20)     1073 2022-10-05 02:49:16.000000 self_documenting_struct-0.9.0/LICENSE
--rw-r--r--   0 developer   (501) staff       (20)     5390 2023-06-18 00:16:29.048179 self_documenting_struct-0.9.0/PKG-INFO
--rw-r--r--   0 developer   (501) staff       (20)     3644 2023-06-17 20:42:14.000000 self_documenting_struct-0.9.0/README.md
--rw-r--r--   0 developer   (501) staff       (20)      628 2023-06-18 00:15:16.000000 self_documenting_struct-0.9.0/pyproject.toml
-drwxr-xr-x   0 developer   (501) staff       (20)        0 2023-06-18 00:16:29.029194 self_documenting_struct-0.9.0/self_documenting_struct/
--rw-r--r--   0 developer   (501) staff       (20)      357 2022-10-07 02:22:11.000000 self_documenting_struct-0.9.0/self_documenting_struct/__init__.py
--rw-r--r--   0 developer   (501) staff       (20)     3102 2023-03-15 11:50:20.000000 self_documenting_struct-0.9.0/self_documenting_struct/data_types.py
--rw-r--r--   0 developer   (501) staff       (20)     3143 2023-03-27 22:29:58.000000 self_documenting_struct-0.9.0/self_documenting_struct/pack.py
--rw-r--r--   0 developer   (501) staff       (20)     1627 2023-03-15 11:50:26.000000 self_documenting_struct-0.9.0/self_documenting_struct/unpack.py
-drwxr-xr-x   0 developer   (501) staff       (20)        0 2023-06-18 00:16:29.046821 self_documenting_struct-0.9.0/self_documenting_struct.egg-info/
--rw-r--r--   0 developer   (501) staff       (20)     5390 2023-06-18 00:16:28.000000 self_documenting_struct-0.9.0/self_documenting_struct.egg-info/PKG-INFO
--rw-r--r--   0 developer   (501) staff       (20)      369 2023-06-18 00:16:28.000000 self_documenting_struct-0.9.0/self_documenting_struct.egg-info/SOURCES.txt
--rw-r--r--   0 developer   (501) staff       (20)        1 2023-06-18 00:16:28.000000 self_documenting_struct-0.9.0/self_documenting_struct.egg-info/dependency_links.txt
--rw-r--r--   0 developer   (501) staff       (20)       24 2023-06-18 00:16:28.000000 self_documenting_struct-0.9.0/self_documenting_struct.egg-info/top_level.txt
--rw-r--r--   0 developer   (501) staff       (20)       38 2023-06-18 00:16:29.049944 self_documenting_struct-0.9.0/setup.cfg
--rw-r--r--   0 developer   (501) staff       (20)       38 2023-06-17 20:37:32.000000 self_documenting_struct-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:39:34.941397 self_documenting_struct-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 01:39:22.000000 self_documenting_struct-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-18 01:39:34.941397 self_documenting_struct-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-18 01:39:22.000000 self_documenting_struct-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-18 01:39:22.000000 self_documenting_struct-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:39:34.941397 self_documenting_struct-0.9.1/self_documenting_struct/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-18 01:39:22.000000 self_documenting_struct-0.9.1/self_documenting_struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-18 01:39:22.000000 self_documenting_struct-0.9.1/self_documenting_struct/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-18 01:39:22.000000 self_documenting_struct-0.9.1/self_documenting_struct/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-18 01:39:22.000000 self_documenting_struct-0.9.1/self_documenting_struct/unpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:39:34.941397 self_documenting_struct-0.9.1/self_documenting_struct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-18 01:39:34.000000 self_documenting_struct-0.9.1/self_documenting_struct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-18 01:39:34.000000 self_documenting_struct-0.9.1/self_documenting_struct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:39:34.000000 self_documenting_struct-0.9.1/self_documenting_struct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-18 01:39:34.000000 self_documenting_struct-0.9.1/self_documenting_struct.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:39:34.941397 self_documenting_struct-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:39:22.000000 self_documenting_struct-0.9.1/setup.py
```

### Comparing `self_documenting_struct-0.9.0/LICENSE` & `self_documenting_struct-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `self_documenting_struct-0.9.0/PKG-INFO` & `self_documenting_struct-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self_documenting_struct
-Version: 0.9.0
+Version: 0.9.1
 Summary: Makes the Python struct library more self-documenting.
 Author: npjg
 License: MIT License
         
         Copyright (c) 2022 Nathanael Gentry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# self-documenting-struct
 Most projects that use the [`struct` library](https://docs.python.org/3/library/struct.html) use raw format strings, which are difficult to understand and remember. This library intuitively wraps the `struct` library to address this issue. provides dataclasses that define the various `struct` format string elements, which can then be combined into format strings in a far more consistent and self-documenting manner than they could otherwise.
 
 I wrote this library to aid my reverse engineering efforts.
  - On a practical level, I grew tired of copy-pasting unintuitive `struct` format strings for common data types like integers and C strings. 
  - On a philosophical level, I believe read-time convenience should be favored above write-time convenience - especially for code that documents file formats.
 
 | Old-style `struct` format string     | Self-documenting `struct`  |
```

### Comparing `self_documenting_struct-0.9.0/README.md` & `self_documenting_struct-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# self-documenting-struct
 Most projects that use the [`struct` library](https://docs.python.org/3/library/struct.html) use raw format strings, which are difficult to understand and remember. This library intuitively wraps the `struct` library to address this issue. provides dataclasses that define the various `struct` format string elements, which can then be combined into format strings in a far more consistent and self-documenting manner than they could otherwise.
 
 I wrote this library to aid my reverse engineering efforts.
  - On a practical level, I grew tired of copy-pasting unintuitive `struct` format strings for common data types like integers and C strings. 
  - On a philosophical level, I believe read-time convenience should be favored above write-time convenience - especially for code that documents file formats.
 
 | Old-style `struct` format string     | Self-documenting `struct`  |
```

### Comparing `self_documenting_struct-0.9.0/pyproject.toml` & `self_documenting_struct-0.9.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "self_documenting_struct"
-version = "0.9.0"
+version = "0.9.1"
 description = "Makes the Python struct library more self-documenting."
 readme = "README.md"
 authors = [{ name = "npjg" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `self_documenting_struct-0.9.0/self_documenting_struct/data_types.py` & `self_documenting_struct-0.9.1/self_documenting_struct/data_types.py`

 * *Files identical despite different names*

### Comparing `self_documenting_struct-0.9.0/self_documenting_struct/pack.py` & `self_documenting_struct-0.9.1/self_documenting_struct/pack.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,14 @@
 
 import struct
 from struct import pack as raw
 from struct import pack_into as raw_into
 
 from .data_types import Type
 
-## Creates a 
-## \param[in] into - If provided, the encoded value is written to this
-##                   binary stream rather than being returned.
-def from_list(values_list, into = None) -> bytes:
-    # BUILD THE FORMAT STRING.
-    format_string = ''.join([entry[0] for entry in values_list]).replace('<', '')
-
-    if into is None:
-        return struct.pack(format_string, *[entry[1] for entry in values_list])
-    else:
-        into.write(struct.pack(format_string, *[entry[1] for entry in values_list]))
-        # struct.pack_into(format_string, into, into.tell(), *[entry[1] for entry in values_list])
-
 ## The following methods encode Python objects in binary data types.
 ## All these methods are "atomic": They write only one item each.
 ## \param[in] value - The value to encode. This value must fit in the
 ##                    space provided in the target data type.
 ## \param[in] into - If provided, the encoded value is written to this
 ##                   binary stream rather than being returned.
 ## \return The value encoded in the target binary data type,
@@ -44,39 +31,39 @@
     else:
         struct.pack_into(Type.uint16_le, into, into.tell(), value)
 
 def int16_le(value: int, into = None) -> bytes:
     if into is None:
         return struct.pack(Type.int16_le, value)
     else:
-        into.write(struct.pack(Type.int16_le, value))
+        struct.pack_into(Type.int16_le, into, into.tell(), value)
 
 def uint16_be(value: int, into = None) -> bytes:
     if into is None:
         return struct.pack(Type.uint16_be, value)
     else:
-        into.write(struct.pack(Type.uint16_be, value))
+        struct.pack_into(Type.uint16_be, into, into.tell(), value)
 
 def int16_be(value: int, into = None) -> bytes:
     if into is None:
         return struct.pack(Type.int16_be, value)
     else:
         struct.pack_into(Type.int16_be, into, into.tell(), value)
     
 def uint32_le(value: int, into = None) -> bytes:
     if into is None:
         return struct.pack(Type.uint32_le, value)
     else:
-        into.write(struct.pack(Type.uint32_le, value))
+        struct.pack_into(Type.uint32_le, into, into.tell(), value)
 
 def int32_le(value: int, into = None) -> bytes:
     if into is None:
         return struct.pack(Type.int32_le, value)
     else:
-        into.write(struct.pack(Type.int32_le, value))
+        struct.pack_into(Type.int32_le, into, into.tell(), value)
 
 def uint32_be(value: int, into = None) -> bytes:
     if into is None:
         return struct.pack(Type.uint32_be, value)
     else:
         struct.pack_into(Type.uint32_be, into, into.tell(), value)
```

### Comparing `self_documenting_struct-0.9.0/self_documenting_struct/unpack.py` & `self_documenting_struct-0.9.1/self_documenting_struct/unpack.py`

 * *Files identical despite different names*

### Comparing `self_documenting_struct-0.9.0/self_documenting_struct.egg-info/PKG-INFO` & `self_documenting_struct-0.9.1/self_documenting_struct.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: self-documenting-struct
-Version: 0.9.0
+Version: 0.9.1
 Summary: Makes the Python struct library more self-documenting.
 Author: npjg
 License: MIT License
         
         Copyright (c) 2022 Nathanael Gentry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# self-documenting-struct
 Most projects that use the [`struct` library](https://docs.python.org/3/library/struct.html) use raw format strings, which are difficult to understand and remember. This library intuitively wraps the `struct` library to address this issue. provides dataclasses that define the various `struct` format string elements, which can then be combined into format strings in a far more consistent and self-documenting manner than they could otherwise.
 
 I wrote this library to aid my reverse engineering efforts.
  - On a practical level, I grew tired of copy-pasting unintuitive `struct` format strings for common data types like integers and C strings. 
  - On a philosophical level, I believe read-time convenience should be favored above write-time convenience - especially for code that documents file formats.
 
 | Old-style `struct` format string     | Self-documenting `struct`  |
```


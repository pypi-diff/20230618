# Comparing `tmp/htdb-py-0.2.0.tar.gz` & `tmp/htdb-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htdb-py-0.2.0.tar", last modified: Sat Jun 17 09:37:08 2023, max compression
+gzip compressed data, was "htdb-py-0.3.0.tar", last modified: Sun Jun 18 10:00:04 2023, max compression
```

## Comparing `htdb-py-0.2.0.tar` & `htdb-py-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 09:37:08.000000 htdb-py-0.2.0/
--rw-rw-rw-   0        0        0    11558 2023-06-17 09:16:02.000000 htdb-py-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       18 2023-06-17 09:35:40.000000 htdb-py-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      123 2023-06-17 09:37:10.000000 htdb-py-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 09:37:08.000000 htdb-py-0.2.0/htdb/
--rw-rw-rw-   0        0        0    13094 2023-06-17 08:31:04.000000 htdb-py-0.2.0/htdb/dict.c
--rw-rw-rw-   0        0        0     2705 2023-06-17 08:31:04.000000 htdb-py-0.2.0/htdb/dict.h
--rw-rw-rw-   0        0        0     8110 2023-06-17 08:31:04.000000 htdb-py-0.2.0/htdb/htdb.c
--rw-rw-rw-   0        0        0     1672 2023-06-17 08:31:04.000000 htdb-py-0.2.0/htdb/htdb.h
--rw-rw-rw-   0        0        0    14397 2023-06-14 11:09:50.000000 htdb-py-0.2.0/htdb/siphash.c
--rw-rw-rw-   0        0        0      254 2023-06-15 13:51:52.000000 htdb-py-0.2.0/htdb/siphash.h
-drwxrwxrwx   0        0        0        0 2023-06-17 09:37:08.000000 htdb-py-0.2.0/htdb_py.egg-info/
--rw-rw-rw-   0        0        0      123 2023-06-17 09:37:08.000000 htdb-py-0.2.0/htdb_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-17 09:37:08.000000 htdb-py-0.2.0/htdb_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 09:37:08.000000 htdb-py-0.2.0/htdb_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 09:04:40.000000 htdb-py-0.2.0/htdb_py.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-06-17 09:37:08.000000 htdb-py-0.2.0/htdb_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-17 09:37:08.000000 htdb-py-0.2.0/htdb_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-06-17 09:30:36.000000 htdb-py-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-17 09:37:10.000000 htdb-py-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      548 2023-06-17 08:37:24.000000 htdb-py-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 09:37:08.000000 htdb-py-0.2.0/src/
--rw-rw-rw-   0        0        0     4765 2023-06-17 08:31:32.000000 htdb-py-0.2.0/src/bindings.cpp
+drwxrwxrwx   0        0        0        0 2023-06-18 10:00:04.000000 htdb-py-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-17 09:16:02.000000 htdb-py-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-06-17 09:35:40.000000 htdb-py-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      123 2023-06-18 10:00:06.000000 htdb-py-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb/
+-rw-rw-rw-   0        0        0    13080 2023-06-18 09:39:28.000000 htdb-py-0.3.0/htdb/dict.c
+-rw-rw-rw-   0        0        0     2705 2023-06-17 08:31:04.000000 htdb-py-0.3.0/htdb/dict.h
+-rw-rw-rw-   0        0        0     8088 2023-06-18 09:55:42.000000 htdb-py-0.3.0/htdb/htdb.c
+-rw-rw-rw-   0        0        0     1672 2023-06-17 08:31:04.000000 htdb-py-0.3.0/htdb/htdb.h
+-rw-rw-rw-   0        0        0    14397 2023-06-14 11:09:50.000000 htdb-py-0.3.0/htdb/siphash.c
+-rw-rw-rw-   0        0        0      254 2023-06-15 13:51:52.000000 htdb-py-0.3.0/htdb/siphash.h
+drwxrwxrwx   0        0        0        0 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/
+-rw-rw-rw-   0        0        0      123 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 09:04:40.000000 htdb-py-0.3.0/htdb_py.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-18 10:00:04.000000 htdb-py-0.3.0/htdb_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-06-17 09:30:36.000000 htdb-py-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 10:00:06.000000 htdb-py-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      548 2023-06-18 09:59:02.000000 htdb-py-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 10:00:04.000000 htdb-py-0.3.0/src/
+-rw-rw-rw-   0        0        0     5278 2023-06-18 08:08:34.000000 htdb-py-0.3.0/src/bindings.cpp
```

### Comparing `htdb-py-0.2.0/LICENSE` & `htdb-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htdb-py-0.2.0/htdb/dict.c` & `htdb-py-0.3.0/htdb/dict.c`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,16 @@
 dictDel(Dict* mp, DictKeyType key) {
     DictKeys* dk = mp->keys;
     ix_t ix = _DictKeys_Lookup(dk, key, dk->keyHashFunc(key), true);
     if (ix >= 0) {
         // Delete Key
         size_t hashpos = _DictKeys_GetHashPosition(dk, dk->keyHashFunc(key), ix);
 
-        DictKeyEntry ep = DK_ENTRIES(dk)[ix];
-        ep.hash = 0;
+        DictKeyEntry *ep = &DK_ENTRIES(dk)[ix];
+        ep->hash = 0;
 
         _DictKeys_SetIndex(dk, hashpos, DKIX_DUMMY);
         mp->used--;
     } else {
         // do nothing
     }
     return 0;
@@ -161,19 +161,19 @@
 }
 
 extern bool
 dictIterNext(DictIter *iter, DictKeyType *key_, DictValueType *val_) {
     DictKeys* dk = iter->mp->keys;
     DictKeyEntry* entries = DK_ENTRIES(dk);
     size_t i = iter->pos;
-    for (; i < dk->dk_nentries; i++, iter->pos++) {
+    for (; i < dk->dk_nentries; i++) {
+        ++iter->pos;
         if (entries[i].hash != 0) {
             *key_ = entries[i].key;
             *val_ = entries[i].value;
-            iter->pos++;
             return 1;
         }
     }
     return 0;
 }
 
 static uint8_t
```

### Comparing `htdb-py-0.2.0/htdb/dict.h` & `htdb-py-0.3.0/htdb/dict.h`

 * *Files identical despite different names*

### Comparing `htdb-py-0.2.0/htdb/htdb.c` & `htdb-py-0.3.0/htdb/htdb.c`

 * *Files 0% similar despite different names*

```diff
@@ -84,24 +84,23 @@
 void xdbLoad(xdb *db, FILE *stream) {
     char start_mark;
     uint8_t key_type, value_type;
     xobjlen_t key_len, value_len;
     char *data_buffer = (char *)malloc(65535);  // the max size of xobjlen_t
 
     while (fgetc(stream) == RECORD_START_MARK) {
-        // assert();
 
         fread(&key_type, sizeof(uint8_t), 1, stream);
         fread(&value_type, sizeof(uint8_t), 1, stream);
         fread(&key_len, sizeof(xobjlen_t), 1, stream);
         fread(&value_len, sizeof(xobjlen_t), 1, stream);
 
         fread(data_buffer, key_len, 1, stream);
-        fread(data_buffer, value_len, 1, stream);
         xobj *keyobj = xobjNew(key_type, data_buffer, key_len);
+        fread(data_buffer, value_len, 1, stream);
         xobj *valobj = xobjNew(value_type, data_buffer, value_len);
 
         dictSet(db->table, keyobj, valobj);
     }
     free(data_buffer);
 }
```

### Comparing `htdb-py-0.2.0/htdb/htdb.h` & `htdb-py-0.3.0/htdb/htdb.h`

 * *Files identical despite different names*

### Comparing `htdb-py-0.2.0/htdb/siphash.c` & `htdb-py-0.3.0/htdb/siphash.c`

 * *Files identical despite different names*

### Comparing `htdb-py-0.2.0/setup.py` & `htdb-py-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import glob
 
 from setuptools import setup
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 
 ext_modules=[
     Pybind11Extension(
         name="htdb",
         sources=sorted(glob.glob("htdb/*.c")) + sorted(glob.glob("src/*.cpp")),
         include_dirs=["htdb/"],
```

### Comparing `htdb-py-0.2.0/src/bindings.cpp` & `htdb-py-0.3.0/src/bindings.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include <pybind11/pybind11.h>
+#include <pybind11/stl/filesystem.h>
 #include "htdb.h"
 #include <iostream>
 #include <stdio.h>
 
 namespace py = pybind11;
 using namespace pybind11::literals;
 
@@ -116,29 +117,39 @@
             return;
         }
         FILE *fp = fopen(filename.c_str(), "wb");
         xdbDump(_db, fp);
         fclose(fp);
     }
 
+    auto dump(std::filesystem::path filename) -> void {
+        dump(filename.string());
+    }
+
     auto load(std::string filename) -> void {
         FILE *fp = fopen(filename.c_str(), "rb");
         xdbLoad(_db, fp);
         fclose(fp);
     }
+
+    auto load(std::filesystem::path filename) -> void {
+        load(filename.string());
+    }
 private:
     xdb *_db;
 };
 
 PYBIND11_MODULE(htdb, m) {
     py::class_<Htdb>(m, "Htdb")
         .def(py::init<>())
         .def("set", &Htdb::set)
         .def("get", &Htdb::get)
         .def("has", &Htdb::has)
         .def("remove", &Htdb::remove)
-        .def("dump", &Htdb::dump, "filename"_a = std::string())
-        .def("load", &Htdb::load, "filename"_a)
+        .def("dump", static_cast<void (Htdb::*)(std::string)>(&Htdb::dump), "filename"_a = "")
+        .def("dump", static_cast<void (Htdb::*)(std::filesystem::path)>(&Htdb::dump), "filename"_a)
+        .def("load", static_cast<void (Htdb::*)(std::string)>(&Htdb::load), "filename"_a)
+        .def("load", static_cast<void (Htdb::*)(std::filesystem::path)>(&Htdb::load), "filename"_a)
         .def("__len__", &Htdb::getSize)
         .def("__contains__", &Htdb::has)
     ;
 }
```


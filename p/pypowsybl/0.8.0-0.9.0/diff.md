# Comparing `tmp/pypowsybl-0.8.0.tar.gz` & `tmp/pypowsybl-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypowsybl-0.8.0.tar", last modified: Sun Jun 13 20:56:24 2021, max compression
+gzip compressed data, was "pypowsybl-0.9.0.tar", last modified: Fri Aug 20 15:57:18 2021, max compression
```

## Comparing `pypowsybl-0.8.0.tar` & `pypowsybl-0.9.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.588041 pypowsybl-0.8.0/
--rw-r--r--   0 runner     (501) staff       (20)    16727 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     9262 2021-06-13 20:56:24.588299 pypowsybl-0.8.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6773 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.547073 pypowsybl-0.8.0/cpp/
--rw-r--r--   0 runner     (501) staff       (20)     2870 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/cpp/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.542929 pypowsybl-0.8.0/cpp/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.547675 pypowsybl-0.8.0/cpp/lib/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)     9996 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.543273 pypowsybl-0.8.0/cpp/lib/pybind11/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.559039 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    21396 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner     (501) staff       (20)     6118 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner     (501) staff       (20)    93952 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner     (501) staff       (20)     8185 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)      120 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2037 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.562316 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner     (501) staff       (20)    27803 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner     (501) staff       (20)    39917 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner     (501) staff       (20)     3602 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner     (501) staff       (20)    16397 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner     (501) staff       (20)    16373 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner     (501) staff       (20)     1486 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner     (501) staff       (20)    29087 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner     (501) staff       (20)     7843 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner     (501) staff       (20)     5079 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner     (501) staff       (20)     3709 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner     (501) staff       (20)     5991 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner     (501) staff       (20)    69312 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner     (501) staff       (20)     9085 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner     (501) staff       (20)     2049 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner     (501) staff       (20)   107755 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner     (501) staff       (20)    65764 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 runner     (501) staff       (20)    14136 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner     (501) staff       (20)    23356 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.577707 pypowsybl-0.8.0/cpp/lib/pybind11/tools/
--rw-r--r--   0 runner     (501) staff       (20)     2295 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner     (501) staff       (20)     3031 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner     (501) staff       (20)     9942 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner     (501) staff       (20)    14003 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner     (501) staff       (20)     8187 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner     (501) staff       (20)     6592 2021-06-13 20:47:06.000000 pypowsybl-0.8.0/cpp/lib/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.579100 pypowsybl-0.8.0/cpp/src/
--rw-r--r--   0 runner     (501) staff       (20)    23422 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/cpp/src/bindings.cpp
--rw-r--r--   0 runner     (501) staff       (20)    15921 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/cpp/src/pypowsybl.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6416 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/cpp/src/pypowsybl.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.579536 pypowsybl-0.8.0/java/
--rw-r--r--   0 runner     (501) staff       (20)     9072 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/java/pom.xml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.544345 pypowsybl-0.8.0/java/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.544470 pypowsybl-0.8.0/java/src/main/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.580321 pypowsybl-0.8.0/java/src/main/resources/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.544801 pypowsybl-0.8.0/java/src/main/resources/META-INF/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.581957 pypowsybl-0.8.0/java/src/main/resources/META-INF/native-image/
--rw-r--r--   0 runner     (501) staff       (20)      423 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/java/src/main/resources/META-INF/native-image/jni-config.json
--rw-r--r--   0 runner     (501) staff       (20)      400 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/java/src/main/resources/META-INF/native-image/proxy-config.json
--rw-r--r--   0 runner     (501) staff       (20)     5636 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/java/src/main/resources/META-INF/native-image/reflect-config.json
--rw-r--r--   0 runner     (501) staff       (20)      347 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/java/src/main/resources/META-INF/native-image/resource-config.json
--rwxr-xr-x   0 runner     (501) staff       (20)      459 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/java/src/main/resources/logback.xml
--rw-r--r--   0 runner     (501) staff       (20)     2425 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/java/src/main/resources/pypowsybl-api.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.585137 pypowsybl-0.8.0/pypowsybl/
--rw-r--r--   0 runner     (501) staff       (20)      984 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/pypowsybl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2972 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/pypowsybl/loadflow.py
--rw-r--r--   0 runner     (501) staff       (20)    14483 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/pypowsybl/network.py
--rw-r--r--   0 runner     (501) staff       (20)     4227 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/pypowsybl/security.py
--rw-r--r--   0 runner     (501) staff       (20)    14181 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/pypowsybl/sensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)     1944 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/pypowsybl/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-06-13 20:56:24.587717 pypowsybl-0.8.0/pypowsybl.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     9262 2021-06-13 20:56:24.000000 pypowsybl-0.8.0/pypowsybl.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2165 2021-06-13 20:56:24.000000 pypowsybl-0.8.0/pypowsybl.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2021-06-13 20:56:24.000000 pypowsybl-0.8.0/pypowsybl.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2021-06-13 20:56:19.000000 pypowsybl-0.8.0/pypowsybl.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       19 2021-06-13 20:56:24.000000 pypowsybl-0.8.0/pypowsybl.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       21 2021-06-13 20:56:24.000000 pypowsybl-0.8.0/pypowsybl.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       88 2021-06-13 20:56:24.589049 pypowsybl-0.8.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     8803 2021-06-13 20:47:05.000000 pypowsybl-0.8.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.766861 pypowsybl-0.9.0/
+-rw-r--r--   0 runner     (501) staff       (20)    16727 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     9812 2021-08-20 15:57:18.767138 pypowsybl-0.9.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     7291 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.734245 pypowsybl-0.9.0/cpp/
+-rw-r--r--   0 runner     (501) staff       (20)     2876 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/cpp/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.728188 pypowsybl-0.9.0/cpp/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.734979 pypowsybl-0.9.0/cpp/lib/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)     9996 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.728645 pypowsybl-0.9.0/cpp/lib/pybind11/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.746841 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    21396 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner     (501) staff       (20)     6118 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner     (501) staff       (20)    93952 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner     (501) staff       (20)     8185 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner     (501) staff       (20)      120 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     2037 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.750917 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner     (501) staff       (20)    27803 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner     (501) staff       (20)    39917 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     3602 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner     (501) staff       (20)    16397 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner     (501) staff       (20)    16373 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner     (501) staff       (20)     1486 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner     (501) staff       (20)    29087 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner     (501) staff       (20)     7843 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner     (501) staff       (20)     5079 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner     (501) staff       (20)     3709 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner     (501) staff       (20)     5991 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner     (501) staff       (20)    69312 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner     (501) staff       (20)     9085 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner     (501) staff       (20)     2049 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner     (501) staff       (20)   107755 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner     (501) staff       (20)    65764 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0 runner     (501) staff       (20)    14136 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner     (501) staff       (20)    23356 2021-08-20 15:47:09.000000 pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.754516 pypowsybl-0.9.0/cpp/lib/pybind11/tools/
+-rw-r--r--   0 runner     (501) staff       (20)     2295 2021-08-20 15:47:10.000000 pypowsybl-0.9.0/cpp/lib/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     3031 2021-08-20 15:47:10.000000 pypowsybl-0.9.0/cpp/lib/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     9942 2021-08-20 15:47:10.000000 pypowsybl-0.9.0/cpp/lib/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner     (501) staff       (20)    14003 2021-08-20 15:47:10.000000 pypowsybl-0.9.0/cpp/lib/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     8187 2021-08-20 15:47:10.000000 pypowsybl-0.9.0/cpp/lib/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     6592 2021-08-20 15:47:10.000000 pypowsybl-0.9.0/cpp/lib/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.755777 pypowsybl-0.9.0/cpp/src/
+-rw-r--r--   0 runner     (501) staff       (20)    29183 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/cpp/src/bindings.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    22576 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/cpp/src/pypowsybl.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     9066 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/cpp/src/pypowsybl.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.756159 pypowsybl-0.9.0/java/
+-rw-r--r--   0 runner     (501) staff       (20)     9341 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/java/pom.xml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.730142 pypowsybl-0.9.0/java/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.730303 pypowsybl-0.9.0/java/src/main/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.756893 pypowsybl-0.9.0/java/src/main/resources/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.730769 pypowsybl-0.9.0/java/src/main/resources/META-INF/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.759341 pypowsybl-0.9.0/java/src/main/resources/META-INF/native-image/
+-rw-r--r--   0 runner     (501) staff       (20)      423 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/java/src/main/resources/META-INF/native-image/jni-config.json
+-rw-r--r--   0 runner     (501) staff       (20)      400 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/java/src/main/resources/META-INF/native-image/proxy-config.json
+-rw-r--r--   0 runner     (501) staff       (20)     5636 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/java/src/main/resources/META-INF/native-image/reflect-config.json
+-rw-r--r--   0 runner     (501) staff       (20)      347 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/java/src/main/resources/META-INF/native-image/resource-config.json
+-rwxr-xr-x   0 runner     (501) staff       (20)      459 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/java/src/main/resources/logback.xml
+-rw-r--r--   0 runner     (501) staff       (20)     2819 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/java/src/main/resources/pypowsybl-api.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.763121 pypowsybl-0.9.0/pypowsybl/
+-rw-r--r--   0 runner     (501) staff       (20)     1263 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/pypowsybl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3084 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/pypowsybl/loadflow.py
+-rw-r--r--   0 runner     (501) staff       (20)    25845 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/pypowsybl/network.py
+-rw-r--r--   0 runner     (501) staff       (20)    11779 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/pypowsybl/security.py
+-rw-r--r--   0 runner     (501) staff       (20)    13995 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/pypowsybl/sensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)     1876 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/pypowsybl/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-08-20 15:57:18.766410 pypowsybl-0.9.0/pypowsybl.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     9812 2021-08-20 15:57:18.000000 pypowsybl-0.9.0/pypowsybl.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2165 2021-08-20 15:57:18.000000 pypowsybl-0.9.0/pypowsybl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2021-08-20 15:57:18.000000 pypowsybl-0.9.0/pypowsybl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2021-08-20 15:57:13.000000 pypowsybl-0.9.0/pypowsybl.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       28 2021-08-20 15:57:18.000000 pypowsybl-0.9.0/pypowsybl.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       21 2021-08-20 15:57:18.000000 pypowsybl-0.9.0/pypowsybl.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       88 2021-08-20 15:57:18.767776 pypowsybl-0.9.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     8823 2021-08-20 15:47:06.000000 pypowsybl-0.9.0/setup.py
```

### Comparing `pypowsybl-0.8.0/LICENSE` & `pypowsybl-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/PKG-INFO` & `pypowsybl-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: pypowsybl
-Version: 0.8.0
+Version: 0.9.0
 Summary: A PowSyBl Python API
 Home-page: https://github.com/powsybl/pypowsybl
 Author: Geoffroy Jamgotchian
 Author-email: geoffroy.jamgotchian@gmail.com
 License: UNKNOWN
 Description: # PyPowSyBl
         
         [![Actions Status](https://github.com/powsybl/pypowsybl/workflows/CI/badge.svg)](https://github.com/powsybl/pypowsybl/actions)
+        [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=powsybl_pypowsybl&metric=alert_status)](https://sonarcloud.io/dashboard?id=powsybl_pypowsybl)
+        [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=powsybl_pypowsybl&metric=coverage)](https://sonarcloud.io/dashboard?id=powsybl_pypowsybl)
         [![PyPI Latest Release](https://img.shields.io/pypi/v/pypowsybl.svg)](https://pypi.org/project/pypowsybl/)
         [![Documentation Status](https://readthedocs.org/projects/pypowsybl/badge/?version=latest)](https://pypowsybl.readthedocs.io/en/latest/?badge=latest)
         [![MPL-2.0 License](https://img.shields.io/badge/license-MPL_2.0-blue.svg)](https://www.mozilla.org/en-US/MPL/2.0/)
         [![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/powsybl)
+        [![Slack](https://img.shields.io/badge/slack-powsybl-blueviolet.svg?logo=slack)](https://join.slack.com/t/powsybl/shared_invite/zt-rzvbuzjk-nxi0boim1RKPS5PjieI0rA)
         
-        The PyPowSyBl project gives access PowSyBl Java framework to Python developers. This Python integration relies on 
+        
+        The PyPowSyBl project gives access PowSyBl Java framework to Python developers. This Python integration relies on
         GraalVM to compile Java code to a native library.
         
         ## Installation
         
         PyPowSyBl is released on [PyPi](https://pypi.org/project/pypowsybl/).
         
         First, make sure you have an up-to-date version of pip and setuptools:
@@ -33,29 +37,29 @@
         
         ## Build from sources
         
         Requirements:
         
         - Maven >= 3.1
         - Cmake >= 3.14
-        - C++11 compiler 
+        - C++11 compiler
         - Python >= 3.7
-        - [GraalVM 20.3.0](https://github.com/graalvm/graalvm-ce-builds/releases/tag/vm-20.3.0) with [native image](https://www.graalvm.org/reference-manual/native-image/#install-native-image)
+        - [GraalVM 21.2.0](https://github.com/graalvm/graalvm-ce-builds/releases/tag/vm-21.2.0) with [native image](https://www.graalvm.org/reference-manual/native-image/#install-native-image)
         
         To build from sources and install PyPowSyBl package:
         ```bash
         git clone --recursive https://github.com/powsybl/pypowsybl.git
         export JAVA_HOME=<path to GraalVM>
         pip3 install --upgrade setuptools pip --user
         pip3 install . --user
         ```
         
         To run unit tests:
         ```bash
-        python3 -m unittest tests/test.py
+        python3 -m unittest discover --start-directory tests
         ```
         
         ## Usage
         
         First, we have to import pypowsybl:
         ```python
         import pypowsybl as pp
@@ -90,18 +94,18 @@
         ```
         
         We can re-run the load flow computation in DC mode:
         ```python
         results = pp.loadflow.run_dc(n)
         ```
         
-        Or with different parameters:
+        By default, the application read configs from `${HOME}/.itools/config.yml`
+        We can disable this with command :
         ```python
-        parameters = pp.loadflow.Parameters(distributed_slack=False)
-        results = pp.loadflow.run_ac(n, parameters)
+        pp.set_config_read(False)
         ```
         
         We can now get buses data (like any other network elements) as a [Pandas](https://pandas.pydata.org/) dataframe:
         ```python
         buses = n.get_buses()
         print(buses)
         ```
```

### Comparing `pypowsybl-0.8.0/README.md` & `pypowsybl-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # PyPowSyBl
 
 [![Actions Status](https://github.com/powsybl/pypowsybl/workflows/CI/badge.svg)](https://github.com/powsybl/pypowsybl/actions)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=powsybl_pypowsybl&metric=alert_status)](https://sonarcloud.io/dashboard?id=powsybl_pypowsybl)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=powsybl_pypowsybl&metric=coverage)](https://sonarcloud.io/dashboard?id=powsybl_pypowsybl)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pypowsybl.svg)](https://pypi.org/project/pypowsybl/)
 [![Documentation Status](https://readthedocs.org/projects/pypowsybl/badge/?version=latest)](https://pypowsybl.readthedocs.io/en/latest/?badge=latest)
 [![MPL-2.0 License](https://img.shields.io/badge/license-MPL_2.0-blue.svg)](https://www.mozilla.org/en-US/MPL/2.0/)
 [![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/powsybl)
+[![Slack](https://img.shields.io/badge/slack-powsybl-blueviolet.svg?logo=slack)](https://join.slack.com/t/powsybl/shared_invite/zt-rzvbuzjk-nxi0boim1RKPS5PjieI0rA)
 
-The PyPowSyBl project gives access PowSyBl Java framework to Python developers. This Python integration relies on 
+
+The PyPowSyBl project gives access PowSyBl Java framework to Python developers. This Python integration relies on
 GraalVM to compile Java code to a native library.
 
 ## Installation
 
 PyPowSyBl is released on [PyPi](https://pypi.org/project/pypowsybl/).
 
 First, make sure you have an up-to-date version of pip and setuptools:
@@ -25,29 +29,29 @@
 
 ## Build from sources
 
 Requirements:
 
 - Maven >= 3.1
 - Cmake >= 3.14
-- C++11 compiler 
+- C++11 compiler
 - Python >= 3.7
-- [GraalVM 20.3.0](https://github.com/graalvm/graalvm-ce-builds/releases/tag/vm-20.3.0) with [native image](https://www.graalvm.org/reference-manual/native-image/#install-native-image)
+- [GraalVM 21.2.0](https://github.com/graalvm/graalvm-ce-builds/releases/tag/vm-21.2.0) with [native image](https://www.graalvm.org/reference-manual/native-image/#install-native-image)
 
 To build from sources and install PyPowSyBl package:
 ```bash
 git clone --recursive https://github.com/powsybl/pypowsybl.git
 export JAVA_HOME=<path to GraalVM>
 pip3 install --upgrade setuptools pip --user
 pip3 install . --user
 ```
 
 To run unit tests:
 ```bash
-python3 -m unittest tests/test.py
+python3 -m unittest discover --start-directory tests
 ```
 
 ## Usage
 
 First, we have to import pypowsybl:
 ```python
 import pypowsybl as pp
@@ -82,18 +86,18 @@
 ```
 
 We can re-run the load flow computation in DC mode:
 ```python
 results = pp.loadflow.run_dc(n)
 ```
 
-Or with different parameters:
+By default, the application read configs from `${HOME}/.itools/config.yml`
+We can disable this with command :
 ```python
-parameters = pp.loadflow.Parameters(distributed_slack=False)
-results = pp.loadflow.run_ac(n, parameters)
+pp.set_config_read(False)
 ```
 
 We can now get buses data (like any other network elements) as a [Pandas](https://pandas.pydata.org/) dataframe:
 ```python
 buses = n.get_buses()
 print(buses)
 ```
```

### Comparing `pypowsybl-0.8.0/cpp/CMakeLists.txt` & `pypowsybl-0.9.0/cpp/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # linking with our shared library
 if(${CMAKE_SYSTEM_NAME} STREQUAL "Darwin")
     set(INSTALL_EXTRA_COMMAND COMMAND install_name_tool -id @loader_path/${PYPOWSYBL_JAVA_LIB} ${PYPOWSYBL_JAVA_BIN_DIR}/${PYPOWSYBL_JAVA_LIB})
 endif()
 
 ExternalProject_Add(mvn
     SOURCE_DIR ${PYPOWSYBL_JAVA_SRC_DIR}
-    PATCH_COMMAND mvn --batch-mode package
+    PATCH_COMMAND mvn --batch-mode clean package
     CONFIGURE_COMMAND ""
     BUILD_COMMAND ""
     INSTALL_COMMAND ""
 )
 
 # as GraalVm does not follow same library naming convention (lib prefix is missing on Linux and MacOS) we need to rename
 # it in the install command step
```

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/CMakeLists.txt` & `pypowsybl-0.9.0/cpp/lib/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/attr.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/buffer_info.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/cast.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/chrono.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/complex.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/class.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/common.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/descr.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/init.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/internals.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/detail/typeid.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/eigen.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/embed.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/eval.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/functional.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/iostream.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/numpy.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/operators.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/options.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/pybind11.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/pytypes.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/stl.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/include/pybind11/stl_bind.h` & `pypowsybl-0.9.0/cpp/lib/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/tools/FindCatch.cmake` & `pypowsybl-0.9.0/cpp/lib/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/tools/FindEigen3.cmake` & `pypowsybl-0.9.0/cpp/lib/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/tools/FindPythonLibsNew.cmake` & `pypowsybl-0.9.0/cpp/lib/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/tools/pybind11Common.cmake` & `pypowsybl-0.9.0/cpp/lib/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/tools/pybind11NewTools.cmake` & `pypowsybl-0.9.0/cpp/lib/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/lib/pybind11/tools/pybind11Tools.cmake` & `pypowsybl-0.9.0/cpp/lib/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/cpp/src/bindings.cpp` & `pypowsybl-0.9.0/cpp/src/bindings.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,14 @@
  * License, v. 2.0. If a copy of the MPL was not distributed with this
  * file, You can obtain one at http://mozilla.org/MPL/2.0/.
  */
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>
 
-#include <limits>
 #include "pypowsybl.h"
 
 namespace py = pybind11;
 
 template<typename T>
 void bindArray(py::module_& m, const std::string& className) {
     py::class_<T>(m, className.c_str())
@@ -26,58 +25,96 @@
 
 template<typename T>
 py::array seriesAsNumpyArray(const series& series) {
 	//Last argument is to bind lifetime of series to the returned array
     return py::array(py::dtype::of<T>(), series.data.length, series.data.ptr, py::cast(series));
 }
 
+// Reads parameters from config (if not disabled), then updates it with provided optional values
+std::shared_ptr<load_flow_parameters> initLoadFlowParameters(py::object voltageInitMode, py::object transformerVoltageControlOn, py::object noGeneratorReactiveLimits,
+                             py::object phaseShifterRegulationOn, py::object twtSplitShuntAdmittance, py::object simulShunt, py::object readSlackBus, py::object writeSlackBus,
+                             py::object distributedSlack, py::object balanceType, py::object dcUseTransformerRatio, py::object countriesToBalance,
+                             py::object connectedComponentMode) {
+        load_flow_parameters* parameters = new load_flow_parameters();
+        std::shared_ptr<load_flow_parameters> config_params = pypowsybl::createLoadFlowParameters();
+        parameters->voltage_init_mode = voltageInitMode.is_none() ? config_params->voltage_init_mode : voltageInitMode.cast<pypowsybl::VoltageInitMode>();
+        parameters->transformer_voltage_control_on = transformerVoltageControlOn.is_none() ? config_params->transformer_voltage_control_on : transformerVoltageControlOn.cast<bool>();
+        parameters->no_generator_reactive_limits = noGeneratorReactiveLimits.is_none() ? config_params->no_generator_reactive_limits : noGeneratorReactiveLimits.cast<bool>();
+        parameters->phase_shifter_regulation_on = phaseShifterRegulationOn.is_none() ? config_params->phase_shifter_regulation_on : phaseShifterRegulationOn.cast<bool>();
+        parameters->twt_split_shunt_admittance = twtSplitShuntAdmittance.is_none() ? config_params->twt_split_shunt_admittance : twtSplitShuntAdmittance.cast<bool>();
+        parameters->simul_shunt = simulShunt.is_none() ? config_params->simul_shunt : simulShunt.cast<bool>();
+        parameters->read_slack_bus = readSlackBus.is_none() ? config_params->read_slack_bus : readSlackBus.cast<bool>();
+        parameters->write_slack_bus = writeSlackBus.is_none() ? config_params->write_slack_bus : writeSlackBus.cast<bool>();
+        parameters->distributed_slack = distributedSlack.is_none() ? config_params->distributed_slack : distributedSlack.cast<bool>();
+        parameters->balance_type = balanceType.is_none() ? config_params->balance_type : balanceType.cast<pypowsybl::BalanceType>();
+        parameters->dc_use_transformer_ratio = dcUseTransformerRatio.is_none() ? config_params->dc_use_transformer_ratio : dcUseTransformerRatio.cast<bool>();
+        if (countriesToBalance.is_none()) {
+            //copy from config so that ownership is not transferred
+            std::vector<std::string> configCountries(config_params->countries_to_balance, config_params->countries_to_balance + config_params->countries_to_balance_count);
+            parameters->countries_to_balance = pypowsybl::copyVectorStringToCharPtrPtr(configCountries);
+            parameters->countries_to_balance_count = configCountries.size();
+        } else {
+            std::vector<std::string> countries = countriesToBalance.cast<std::vector<std::string>>();
+            parameters->countries_to_balance = pypowsybl::copyVectorStringToCharPtrPtr(countries);
+            parameters->countries_to_balance_count = countries.size();
+        }
+        parameters->connected_component_mode = connectedComponentMode.is_none() ? config_params->connected_component_mode : connectedComponentMode.cast<pypowsybl::ConnectedComponentMode>();
+    return std::shared_ptr<load_flow_parameters>(parameters, [](load_flow_parameters* ptr){
+        pypowsybl::deleteCharPtrPtr(ptr->countries_to_balance, ptr->countries_to_balance_count);
+        delete ptr;
+    });
+}
+
 PYBIND11_MODULE(_pypowsybl, m) {
     pypowsybl::init();
 
     m.doc() = "PowSyBl Python API";
 
     py::register_exception<pypowsybl::PyPowsyblError>(m, "PyPowsyblError");
 
-    m.def("set_debug_mode", &pypowsybl::setDebugMode, "Set debug mode");
+    py::class_<pypowsybl::JavaHandle>(m, "JavaHandle");
 
-    m.def("get_version_table", &pypowsybl::getVersionTable, "Get an ASCII table with all PowSybBl modules version");
+    m.def("set_debug_mode", &pypowsybl::setDebugMode, "Set debug mode");
 
-    m.def("create_empty_network", &pypowsybl::createEmptyNetwork, "Create an empty network",
-          py::arg("id"));
+    m.def("set_config_read", &pypowsybl::setConfigRead, "Set config read mode");
 
-    m.def("create_ieee_network", &pypowsybl::createIeeeNetwork, "Create an IEEE network", py::arg("bus_count"));
+    m.def("is_config_read", &pypowsybl::isConfigRead, "Get config read mode");
 
-    m.def("create_eurostag_tutorial_example1_network", &pypowsybl::createEurostagTutorialExample1Network, "Create an Eurostag tutorial example 1 network");
+    m.def("get_version_table", &pypowsybl::getVersionTable, "Get an ASCII table with all PowSybBl modules version");
 
-    m.def("create_four_substations_node_breaker_network", &pypowsybl::createFourSubstationsNodeBreakerNetwork, "Create an 4-substation example network");
+    m.def("create_network", &pypowsybl::createNetwork, "Create an example network", py::arg("name"), py::arg("id"));
 
     m.def("update_switch_position", &pypowsybl::updateSwitchPosition, "Update a switch position");
 
     m.def("update_connectable_status", &pypowsybl::updateConnectableStatus, "Update a connectable (branch or injection) status");
 
     py::enum_<element_type>(m, "ElementType")
             .value("BUS", element_type::BUS)
             .value("LINE", element_type::LINE)
             .value("TWO_WINDINGS_TRANSFORMER", element_type::TWO_WINDINGS_TRANSFORMER)
             .value("THREE_WINDINGS_TRANSFORMER", element_type::THREE_WINDINGS_TRANSFORMER)
             .value("GENERATOR", element_type::GENERATOR)
             .value("LOAD", element_type::LOAD)
             .value("BATTERY", element_type::BATTERY)
             .value("SHUNT_COMPENSATOR", element_type::SHUNT_COMPENSATOR)
+            .value("NON_LINEAR_SHUNT_COMPENSATOR_SECTION", element_type::NON_LINEAR_SHUNT_COMPENSATOR_SECTION)
             .value("DANGLING_LINE", element_type::DANGLING_LINE)
             .value("LCC_CONVERTER_STATION", element_type::LCC_CONVERTER_STATION)
             .value("VSC_CONVERTER_STATION", element_type::VSC_CONVERTER_STATION)
             .value("STATIC_VAR_COMPENSATOR", element_type::STATIC_VAR_COMPENSATOR)
             .value("SWITCH", element_type::SWITCH)
             .value("VOLTAGE_LEVEL", element_type::VOLTAGE_LEVEL)
             .value("SUBSTATION", element_type::SUBSTATION)
             .value("BUSBAR_SECTION", element_type::BUSBAR_SECTION)
             .value("HVDC_LINE", element_type::HVDC_LINE)
             .value("RATIO_TAP_CHANGER_STEP", element_type::RATIO_TAP_CHANGER_STEP)
             .value("PHASE_TAP_CHANGER_STEP", element_type::PHASE_TAP_CHANGER_STEP)
+            .value("RATIO_TAP_CHANGER", element_type::RATIO_TAP_CHANGER)
+            .value("PHASE_TAP_CHANGER", element_type::PHASE_TAP_CHANGER)
+            .value("REACTIVE_CAPABILITY_CURVE_POINT", element_type::REACTIVE_CAPABILITY_CURVE_POINT)
             .export_values();
 
     m.def("get_network_elements_ids", &pypowsybl::getNetworkElementsIds, "Get network elements ids for a given element type",
           py::arg("network"), py::arg("element_type"), py::arg("nominal_voltages"),
           py::arg("countries"), py::arg("main_connected_component"), py::arg("main_synchronous_component"),
           py::arg("not_connected_to_same_bus_at_both_sides"));
 
@@ -86,16 +123,22 @@
 
     m.def("create_importer_parameters_series_array", &pypowsybl::createImporterParametersSeriesArray, "Create a parameters series array for a given import format",
           py::arg("format"));
 
     m.def("load_network", &pypowsybl::loadNetwork, "Load a network from a file", py::arg("file"),
           py::arg("parameters"));
 
-    m.def("dump_network", &pypowsybl::dumpNetwork, "Dump network to a file in a given format", py::arg("file"),
-          py::arg("format"), py::arg("parameters"), py::arg("parameters"));
+    m.def("load_network_from_string", &pypowsybl::loadNetworkFromString, "Load a network from a string",
+          py::arg("file_name"), py::arg("file_content"),py::arg("parameters"));
+
+    m.def("dump_network", &pypowsybl::dumpNetwork, "Dump network to a file in a given format", py::arg("network"),
+          py::arg("file"),py::arg("format"), py::arg("parameters"));
+
+    m.def("dump_network_to_string", &pypowsybl::dumpNetworkToString, "Dump network in a given format",
+          py::arg("network"), py::arg("format"), py::arg("parameters"));
 
     m.def("reduce_network", &pypowsybl::reduceNetwork, "Reduce network", py::arg("network"), py::arg("v_min"), py::arg("v_max"),
           py::arg("ids"), py::arg("vls"), py::arg("depths"), py::arg("with_dangling_lines"));
 
     py::enum_<pypowsybl::LoadFlowComponentStatus>(m, "LoadFlowComponentStatus")
             .value("CONVERGED", pypowsybl::LoadFlowComponentStatus::CONVERGED)
             .value("FAILED", pypowsybl::LoadFlowComponentStatus::FAILED)
@@ -139,45 +182,25 @@
             .export_values();
 
     py::enum_<pypowsybl::ConnectedComponentMode>(m, "ConnectedComponentMode")
             .value("ALL", pypowsybl::ConnectedComponentMode::ALL)
             .value("MAIN", pypowsybl::ConnectedComponentMode::MAIN)
             .export_values();
 
+
+
     py::class_<load_flow_parameters, std::shared_ptr<load_flow_parameters>>(m, "LoadFlowParameters")
-            .def(py::init([](pypowsybl::VoltageInitMode voltageInitMode, bool transformerVoltageControlOn, bool noGeneratorReactiveLimits,
-                             bool phaseShifterRegulationOn, bool twtSplitShuntAdmittance, bool simulShunt, bool readSlackBus, bool writeSlackBus,
-                             bool distributedSlack, pypowsybl::BalanceType balanceType, bool dcUseTransformerRatio, const std::vector<std::string>& countriesToBalance,
-                             pypowsybl::ConnectedComponentMode connectedComponentMode) {
-                auto parameters = new load_flow_parameters();
-                parameters->voltage_init_mode = voltageInitMode;
-                parameters->transformer_voltage_control_on = transformerVoltageControlOn;
-                parameters->no_generator_reactive_limits = noGeneratorReactiveLimits;
-                parameters->phase_shifter_regulation_on = phaseShifterRegulationOn;
-                parameters->twt_split_shunt_admittance = twtSplitShuntAdmittance;
-                parameters->simul_shunt = simulShunt;
-                parameters->read_slack_bus = readSlackBus;
-                parameters->write_slack_bus = writeSlackBus;
-                parameters->distributed_slack = distributedSlack;
-                parameters->balance_type = balanceType;
-                parameters->dc_use_transformer_ratio = dcUseTransformerRatio;
-                parameters->countries_to_balance = pypowsybl::copyVectorStringToCharPtrPtr(countriesToBalance);
-                parameters->countries_to_balance_count = countriesToBalance.size();
-                parameters->connected_component_mode = connectedComponentMode;
-                return std::shared_ptr<load_flow_parameters>(parameters, [](load_flow_parameters* ptr){
-                    pypowsybl::deleteCharPtrPtr(ptr->countries_to_balance, ptr->countries_to_balance_count);
-                    delete ptr;
-                });
-            }), py::arg("voltage_init_mode") = pypowsybl::VoltageInitMode::UNIFORM_VALUES, py::arg("transformer_voltage_control_on") = false,
-                 py::arg("no_generator_reactive_limits") = false, py::arg("phase_shifter_regulation_on") = false,
-                 py::arg("twt_split_shunt_admittance") = false, py::arg("simul_shunt") = false,
-                 py::arg("read_slack_bus") = false, py::arg("write_slack_bus") = false,
-                 py::arg("distributed_slack") = true, py::arg("balance_type") = pypowsybl::BalanceType::PROPORTIONAL_TO_GENERATION_P_MAX,
-                 py::arg("dc_use_transformer_ratio") = true, py::arg("countries_to_balance") = std::vector<std::string>(),
-                 py::arg("connected_component_mode") = pypowsybl::ConnectedComponentMode::MAIN)
+            .def(py::init(&initLoadFlowParameters),
+                py::arg("voltage_init_mode") = py::none(), py::arg("transformer_voltage_control_on") = py::none(),
+                py::arg("no_generator_reactive_limits") = py::none(), py::arg("phase_shifter_regulation_on") = py::none(),
+                py::arg("twt_split_shunt_admittance") = py::none(), py::arg("simul_shunt") = py::none(),
+                py::arg("read_slack_bus") = py::none(), py::arg("write_slack_bus") = py::none(),
+                py::arg("distributed_slack") = py::none(), py::arg("balance_type") = py::none(),
+                py::arg("dc_use_transformer_ratio") = py::none(), py::arg("countries_to_balance") = py::none(),
+                py::arg("connected_component_mode") = py::none())
             .def_property("voltage_init_mode", [](const load_flow_parameters& p) {
                 return static_cast<pypowsybl::VoltageInitMode>(p.voltage_init_mode);
             }, [](load_flow_parameters& p, pypowsybl::VoltageInitMode voltageInitMode) {
                 p.voltage_init_mode = voltageInitMode;
             })
             .def_property("transformer_voltage_control_on", [](const load_flow_parameters& p) {
                 return (bool) p.transformer_voltage_control_on;
@@ -244,14 +267,17 @@
 
     m.def("run_load_flow", &pypowsybl::runLoadFlow, "Run a load flow", py::arg("network"),
           py::arg("dc"), py::arg("parameters"), py::arg("provider"));
 
     m.def("write_single_line_diagram_svg", &pypowsybl::writeSingleLineDiagramSvg, "Write single line diagram SVG",
           py::arg("network"), py::arg("container_id"), py::arg("svg_file"));
 
+    m.def("get_single_line_diagram_svg", &pypowsybl::getSingleLineDiagramSvg, "Get single line diagram SVG as a string",
+          py::arg("network"), py::arg("container_id"));
+
     m.def("create_security_analysis", &pypowsybl::createSecurityAnalysis, "Create a security analysis");
 
     m.def("add_contingency", &pypowsybl::addContingency, "Add a contingency to a security analysis or sensitivity analysis",
           py::arg("analysis_context"), py::arg("contingency_id"), py::arg("elements_ids"));
 
     py::enum_<pypowsybl::LimitType>(m, "LimitType")
             .value("CURRENT", pypowsybl::LimitType::CURRENT)
@@ -261,14 +287,31 @@
 
     py::enum_<pypowsybl::Side>(m, "Side")
             .value("NONE", pypowsybl::Side::NONE)
             .value("ONE", pypowsybl::Side::ONE)
             .value("TWO", pypowsybl::Side::TWO)
             .export_values();
 
+    py::class_<network_metadata, std::shared_ptr<network_metadata>>(m, "NetworkMetadata")
+            .def_property_readonly("id", [](const network_metadata& att) {
+                return att.id;
+            })
+            .def_property_readonly("name", [](const network_metadata& att) {
+                return att.name;
+            })
+            .def_property_readonly("source_format", [](const network_metadata& att) {
+                return att.source_format;
+            })
+            .def_property_readonly("forecast_distance", [](const network_metadata& att) {
+                return att.forecast_distance;
+            })
+            .def_property_readonly("case_date", [](const network_metadata& att) {
+                return att.case_date;
+            });
+
     py::class_<limit_violation>(m, "LimitViolation")
             .def_property_readonly("subject_id", [](const limit_violation& v) {
                 return v.subject_id;
             })
             .def_property_readonly("subject_name", [](const limit_violation& v) {
                 return v.subject_name;
             })
@@ -391,10 +434,37 @@
     m.def("update_network_elements_with_double_series", &pypowsybl::updateNetworkElementsWithDoubleSeries, "Update network elements for a given element type with a double series",
           py::arg("network"), py::arg("element_type"), py::arg("series_name"), py::arg("ids"), py::arg("values"),
           py::arg("element_count"));
 
     m.def("update_network_elements_with_string_series", &pypowsybl::updateNetworkElementsWithStringSeries, "Update network elements for a given element type with a string series",
           py::arg("network"), py::arg("element_type"), py::arg("series_name"), py::arg("ids"), py::arg("values"),
           py::arg("element_count"));
+    m.def("get_network_metadata", &pypowsybl::getNetworkMetadata, "get attributes", py::arg("network"));
+    m.def("get_working_variant_id", &pypowsybl::getWorkingVariantId, "get the current working variant id", py::arg("network"));
+    m.def("set_working_variant", &pypowsybl::setWorkingVariant, "set working variant", py::arg("network"), py::arg("variant"));
+    m.def("remove_variant", &pypowsybl::removeVariant, "remove a variant", py::arg("network"), py::arg("variant"));
+    m.def("clone_variant", &pypowsybl::cloneVariant, "clone a variant", py::arg("network"), py::arg("src"), py::arg("variant"), py::arg("may_overwrite"));
+    m.def("get_variant_ids", &pypowsybl::getVariantsIds, "get all variant ids from a network", py::arg("network"));
+    m.def("add_monitored_elements", &pypowsybl::addMonitoredElements, "Add monitors to get specific results on network after security analysis process", py::arg("security_analysis_context"),
+          py::arg("contingency_context_type"), py::arg("branch_ids"), py::arg("voltage_level_ids"), py::arg("three_windings_transformer_ids"),
+          py::arg("contingency_ids"));
+
+    py::enum_<contingency_context_type>(m, "ContingencyContextType")
+            .value("ALL", contingency_context_type::ALL)
+            .value("NONE", contingency_context_type::NONE)
+            .value("SPECIFIC", contingency_context_type::SPECIFIC)
+            .export_values();
 
-    m.def("destroy_object_handle", &pypowsybl::destroyObjectHandle, "Destroy Java object handle", py::arg("object_handle"));
+    m.def("get_security_analysis_result", &pypowsybl::getSecurityAnalysisResult, "get result of a security analysis", py::arg("result"));
+    m.def("get_node_breaker_view_nodes", &pypowsybl::getNodeBreakerViewNodes, "get all nodes for a voltage level", py::arg("network"), py::arg("voltage_level"));
+    m.def("get_node_breaker_view_internal_connections", &pypowsybl::getNodeBreakerViewInternalConnections,
+    "get all internal connections for a voltage level", py::arg("network"), py::arg("voltage_level"));
+    m.def("get_node_breaker_view_switches", &pypowsybl::getNodeBreakerViewSwitches, "get all switches for a voltage level", py::arg("network"), py::arg("voltage_level"));
+    m.def("get_limit_violations", &pypowsybl::getLimitViolations, "get limit violations of a security analysis", py::arg("result"));
+
+    m.def("get_branch_results", &pypowsybl::getBranchResults, "create a table with all branch results computed after security analysis",
+          py::arg("result"));
+    m.def("get_bus_results", &pypowsybl::getBusResults, "create a table with all bus results computed after security analysis",
+          py::arg("result"));
+    m.def("get_three_windings_transformer_results", &pypowsybl::getThreeWindingsTransformerResults,
+          "create a table with all three windings transformer results computed after security analysis", py::arg("result"));
 }
```

### Comparing `pypowsybl-0.8.0/cpp/src/pypowsybl.cpp` & `pypowsybl-0.9.0/cpp/src/pypowsybl.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -22,54 +22,73 @@
 
 class GraalVmGuard {
 public:
     GraalVmGuard() {
         if (!isolate) {
             throw std::runtime_error("isolate has not been created");
         }
-        if (graal_attach_thread(isolate, &thread_) != 0) {
-            throw std::runtime_error("graal_create_isolate error");
-        }
+        //if thread already attached to the isolate,
+        //we assume it's a nested call --> do nothing
+
+        thread_ = graal_get_current_thread(isolate);
+        if (thread_ == nullptr) {
+            if (graal_attach_thread(isolate, &thread_) != 0) {
+                throw std::runtime_error("graal_create_isolate error");
+            }
+            shouldDetach = true;
+       }
     }
 
     ~GraalVmGuard() noexcept(false) {
-        if (graal_detach_thread(thread_) != 0) {
+        if (shouldDetach && graal_detach_thread(thread_) != 0) {
             throw std::runtime_error("graal_detach_thread error");
         }
     }
 
     graal_isolatethread_t * thread() const {
         return thread_;
     }
 
 private:
+    bool shouldDetach = false;
     graal_isolatethread_t* thread_ = nullptr;
 };
 
+//copies to string and frees memory allocated by java
+std::string toString(char* cstring);
+
 template<typename F, typename... ARGS>
 void callJava(F f, ARGS... args) {
     GraalVmGuard guard;
     exception_handler exc;
     f(guard.thread(), args..., &exc);
     if (exc.message) {
-        throw PyPowsyblError(exc.message);
+        throw PyPowsyblError(toString(exc.message));
     }
 }
 
 template<typename T, typename F, typename... ARGS>
 T callJava(F f, ARGS... args) {
     GraalVmGuard guard;
     exception_handler exc;
     auto r = f(guard.thread(), args..., &exc);
     if (exc.message) {
-        throw PyPowsyblError(exc.message);
+        throw PyPowsyblError(toString(exc.message));
     }
     return r;
 }
 
+//Destruction of java object when the shared_ptr has no more references
+JavaHandle::JavaHandle(void* handle):
+    handle_(handle, [](void* to_be_deleted) {
+        callJava<>(::destroyObjectHandle, to_be_deleted);
+    })
+{
+}
+
 template<>
 Array<load_flow_component_result>::~Array() {
     callJava<>(::freeLoadFlowComponentResultPointer, delegate_);
 }
 
 template<>
 Array<contingency_result>::~Array() {
@@ -186,36 +205,43 @@
 void deleteCharPtrPtr(char** charPtrPtr, int length) {
     for (int i = 0; i < length; i++) {
         delete charPtrPtr[i];
     }
     delete charPtrPtr;
 }
 
-void setDebugMode(bool debug) {
-    callJava<>(::setDebugMode, debug);
+void freeCString(char* str) {
+    callJava<>(::freeString, str);
 }
 
-std::string getVersionTable() {
-    return std::string(callJava<char*>(::getVersionTable));
+//copies to string and frees memory allocated by java
+std::string toString(char* cstring) {
+    std::string res = cstring;
+    freeCString(cstring);
+    return res;
+}
+
+void setDebugMode(bool debug) {
+    callJava<>(::setDebugMode, debug);
 }
 
-void* createEmptyNetwork(const std::string& id) {
-    return callJava<void*>(::createEmptyNetwork, (char*) id.data());
+void setConfigRead(bool configRead) {
+    callJava<>(::setConfigRead, configRead);
 }
 
-void* createIeeeNetwork(int busCount) {
-    return callJava<void*>(::createIeeeNetwork, busCount);
+bool isConfigRead() {
+    return callJava<bool>(::isConfigRead);
 }
 
-void* createEurostagTutorialExample1Network() {
-    return callJava<void*>(::createEurostagTutorialExample1Network);
+std::string getVersionTable() {
+    return toString(callJava<char*>(::getVersionTable));
 }
 
-void* createFourSubstationsNodeBreakerNetwork() {
-    return callJava<void*>(::createFourSubstationsNodeBreakerNetwork);
+JavaHandle createNetwork(const std::string& name, const std::string& id) {
+    return callJava<JavaHandle>(::createNetwork, (char*) name.data(), (char*) id.data());
 }
 
 std::vector<std::string> getNetworkImportFormats() {
     auto formatsArrayPtr = callJava<array*>(::getNetworkImportFormats);
     ToStringVector formats(formatsArrayPtr);
     return formats.get();
 }
@@ -226,100 +252,148 @@
     return formats.get();
 }
 
 SeriesArray* createImporterParametersSeriesArray(const std::string& format) {
     return new SeriesArray(callJava<array*>(::createImporterParametersSeriesArray, (char*) format.data()));
 }
 
-void* loadNetwork(const std::string& file, const std::map<std::string, std::string>& parameters) {
+std::shared_ptr<network_metadata> getNetworkMetadata(const JavaHandle& network) {
+    network_metadata* attributes = callJava<network_metadata*>(::getNetworkMetadata, network);
+    return std::shared_ptr<network_metadata>(attributes, [](network_metadata* ptr){
+        callJava(::freeNetworkMetadata, ptr);
+    });
+}
+
+JavaHandle loadNetwork(const std::string& file, const std::map<std::string, std::string>& parameters) {
     std::vector<std::string> parameterNames;
     std::vector<std::string> parameterValues;
     parameterNames.reserve(parameters.size());
     parameterValues.reserve(parameters.size());
     for (std::pair<std::string, std::string> p : parameters) {
         parameterNames.push_back(p.first);
         parameterValues.push_back(p.second);
     }
     ToCharPtrPtr parameterNamesPtr(parameterNames);
     ToCharPtrPtr parameterValuesPtr(parameterValues);
-    return callJava<void*>(::loadNetwork, (char*) file.data(), parameterNamesPtr.get(), parameterNames.size(),
+    return callJava<JavaHandle>(::loadNetwork, (char*) file.data(), parameterNamesPtr.get(), parameterNames.size(),
                               parameterValuesPtr.get(), parameterValues.size());
 }
 
-void dumpNetwork(void* network, const std::string& file, const std::string& format, const std::map<std::string, std::string>& parameters) {
+JavaHandle loadNetworkFromString(const std::string& fileName, const std::string& fileContent, const std::map<std::string, std::string>& parameters) {
+    std::vector<std::string> parameterNames;
+    std::vector<std::string> parameterValues;
+    parameterNames.reserve(parameters.size());
+    parameterValues.reserve(parameters.size());
+    for (std::pair<std::string, std::string> p : parameters) {
+        parameterNames.push_back(p.first);
+        parameterValues.push_back(p.second);
+    }
+    ToCharPtrPtr parameterNamesPtr(parameterNames);
+    ToCharPtrPtr parameterValuesPtr(parameterValues);
+    return callJava<JavaHandle>(::loadNetworkFromString, (char*) fileName.data(), (char*) fileContent.data(),
+                           parameterNamesPtr.get(), parameterNames.size(),
+                           parameterValuesPtr.get(), parameterValues.size());
+}
+
+void dumpNetwork(const JavaHandle& network, const std::string& file, const std::string& format, const std::map<std::string, std::string>& parameters) {
     std::vector<std::string> parameterNames;
     std::vector<std::string> parameterValues;
     parameterNames.reserve(parameters.size());
     parameterValues.reserve(parameters.size());
     for (std::pair<std::string, std::string> p : parameters) {
         parameterNames.push_back(p.first);
         parameterValues.push_back(p.second);
     }
     ToCharPtrPtr parameterNamesPtr(parameterNames);
     ToCharPtrPtr parameterValuesPtr(parameterValues);
     callJava(::dumpNetwork, network, (char*) file.data(), (char*) format.data(), parameterNamesPtr.get(), parameterNames.size(),
                 parameterValuesPtr.get(), parameterValues.size());
 }
 
-void reduceNetwork(void* network, double v_min, double v_max, const std::vector<std::string>& ids,
+std::string dumpNetworkToString(const JavaHandle& network, const std::string& format, const std::map<std::string, std::string>& parameters) {
+    std::vector<std::string> parameterNames;
+    std::vector<std::string> parameterValues;
+    parameterNames.reserve(parameters.size());
+    parameterValues.reserve(parameters.size());
+    for (std::pair<std::string, std::string> p : parameters) {
+        parameterNames.push_back(p.first);
+        parameterValues.push_back(p.second);
+    }
+    ToCharPtrPtr parameterNamesPtr(parameterNames);
+    ToCharPtrPtr parameterValuesPtr(parameterValues);
+    return toString(callJava<char*>(::dumpNetworkToString, network, (char*) format.data(), parameterNamesPtr.get(), parameterNames.size(),
+             parameterValuesPtr.get(), parameterValues.size()));
+}
+
+void reduceNetwork(const JavaHandle& network, double v_min, double v_max, const std::vector<std::string>& ids,
                    const std::vector<std::string>& vls, const std::vector<int>& depths, bool withDangLingLines) {
     ToCharPtrPtr elementIdPtr(ids);
     ToCharPtrPtr vlsPtr(vls);
     ToIntPtr depthsPtr(depths);
     callJava(::reduceNetwork, network, v_min, v_max, elementIdPtr.get(), ids.size(), vlsPtr.get(), vls.size(), depthsPtr.get(), depths.size(), withDangLingLines);
 }
 
-bool updateSwitchPosition(void* network, const std::string& id, bool open) {
+bool updateSwitchPosition(const JavaHandle& network, const std::string& id, bool open) {
     return callJava<bool>(::updateSwitchPosition, network, (char*) id.data(), open);
 }
 
-bool updateConnectableStatus(void* network, const std::string& id, bool connected) {
+bool updateConnectableStatus(const JavaHandle& network, const std::string& id, bool connected) {
     return callJava<bool>(::updateConnectableStatus, network, (char*) id.data(), connected);
 }
 
-std::vector<std::string> getNetworkElementsIds(void* network, element_type elementType, const std::vector<double>& nominalVoltages,
+std::vector<std::string> getNetworkElementsIds(const JavaHandle& network, element_type elementType, const std::vector<double>& nominalVoltages,
                                                const std::vector<std::string>& countries, bool mainCc, bool mainSc,
                                                bool notConnectedToSameBusAtBothSides) {
     ToDoublePtr nominalVoltagePtr(nominalVoltages);
     ToCharPtrPtr countryPtr(countries);
     auto elementsIdsArrayPtr = callJava<array*>(::getNetworkElementsIds, network, elementType,
                                                        nominalVoltagePtr.get(), nominalVoltages.size(),
                                                        countryPtr.get(), countries.size(), mainCc, mainSc,
                                                        notConnectedToSameBusAtBothSides);
     ToStringVector elementsIds(elementsIdsArrayPtr);
     return elementsIds.get();
 }
 
-LoadFlowComponentResultArray* runLoadFlow(void* network, bool dc, const std::shared_ptr<load_flow_parameters>& parameters,
+std::shared_ptr<load_flow_parameters> createLoadFlowParameters() {
+    load_flow_parameters* parameters = callJava<load_flow_parameters*>(::createLoadFlowParameters);
+    return std::shared_ptr<load_flow_parameters>(parameters, [](load_flow_parameters* ptr){
+        callJava(::freeLoadFlowParameters, ptr);
+    });
+}
+
+LoadFlowComponentResultArray* runLoadFlow(const JavaHandle& network, bool dc, const std::shared_ptr<load_flow_parameters>& parameters,
                                           const std::string& provider) {
     return new LoadFlowComponentResultArray(
             callJava<array*>(::runLoadFlow, network, dc, parameters.get(), (char *) provider.data()));
 }
 
-void writeSingleLineDiagramSvg(void* network, const std::string& containerId, const std::string& svgFile) {
+void writeSingleLineDiagramSvg(const JavaHandle& network, const std::string& containerId, const std::string& svgFile) {
     callJava(::writeSingleLineDiagramSvg, network, (char*) containerId.data(), (char*) svgFile.data());
 }
 
-void* createSecurityAnalysis() {
-    return callJava<void*>(::createSecurityAnalysis);
+std::string getSingleLineDiagramSvg(const JavaHandle& network, const std::string& containerId) {
+    return toString(callJava<char*>(::getSingleLineDiagramSvg, network, (char*) containerId.data()));
+}
+
+JavaHandle createSecurityAnalysis() {
+    return callJava<JavaHandle>(::createSecurityAnalysis);
 }
 
-void addContingency(void* analysisContext, const std::string& contingencyId, const std::vector<std::string>& elementsIds) {
+void addContingency(const JavaHandle& analysisContext, const std::string& contingencyId, const std::vector<std::string>& elementsIds) {
     ToCharPtrPtr elementIdPtr(elementsIds);
     callJava(::addContingency, analysisContext, (char*) contingencyId.data(), elementIdPtr.get(), elementsIds.size());
 }
 
-ContingencyResultArray* runSecurityAnalysis(void* securityAnalysisContext, void* network, load_flow_parameters& parameters,
+JavaHandle runSecurityAnalysis(const JavaHandle& securityAnalysisContext, const JavaHandle& network, load_flow_parameters& parameters,
                                             const std::string& provider) {
-    return new ContingencyResultArray(callJava<array*>(::runSecurityAnalysis, securityAnalysisContext, network,
-                                                          &parameters, (char *) provider.data()));
+    return callJava<JavaHandle>(::runSecurityAnalysis, securityAnalysisContext, network, &parameters, (char *) provider.data());
 }
 
-void* createSensitivityAnalysis() {
-    return callJava<void*>(::createSensitivityAnalysis);
+JavaHandle createSensitivityAnalysis() {
+    return callJava<JavaHandle>(::createSensitivityAnalysis);
 }
 
 ::zone* createZone(const std::string& id, const std::vector<std::string>& injectionsIds, const std::vector<double>& injectionsShiftKeys) {
     auto z = new ::zone;
     z->id = copyStringToCharPtr(id);
     z->length = injectionsIds.size();
     z->injections_ids = new char*[injectionsIds.size()];
@@ -358,89 +432,150 @@
         return (::zone**) &vector_[0];
     }
 
 private:
     const std::vector<::zone*>& vector_;
 };
 
-void setZones(void* sensitivityAnalysisContext, const std::vector<::zone*>& zones) {
+void setZones(const JavaHandle& sensitivityAnalysisContext, const std::vector<::zone*>& zones) {
     ZonesPtr zonesPtr(zones);
     callJava(::setZones, sensitivityAnalysisContext, zonesPtr.get(), zones.size());
 }
 
-void setBranchFlowFactorMatrix(void* sensitivityAnalysisContext, const std::vector<std::string>& branchesIds,
+void setBranchFlowFactorMatrix(const JavaHandle& sensitivityAnalysisContext, const std::vector<std::string>& branchesIds,
                                const std::vector<std::string>& variablesIds) {
     ToCharPtrPtr branchIdPtr(branchesIds);
     ToCharPtrPtr variableIdPtr(variablesIds);
     callJava(::setBranchFlowFactorMatrix, sensitivityAnalysisContext, branchIdPtr.get(), branchesIds.size(),
                 variableIdPtr.get(), variablesIds.size());
 }
 
-void setBusVoltageFactorMatrix(void* sensitivityAnalysisContext, const std::vector<std::string>& busIds,
+void setBusVoltageFactorMatrix(const JavaHandle& sensitivityAnalysisContext, const std::vector<std::string>& busIds,
                                const std::vector<std::string>& targetVoltageIds) {
     ToCharPtrPtr busVoltageIdPtr(busIds);
     ToCharPtrPtr targetVoltageIdPtr(targetVoltageIds);
     callJava(::setBusVoltageFactorMatrix, sensitivityAnalysisContext, busVoltageIdPtr.get(),
                 busIds.size(), targetVoltageIdPtr.get(), targetVoltageIds.size());
 }
 
-void* runSensitivityAnalysis(void* sensitivityAnalysisContext, void* network, bool dc, load_flow_parameters& parameters, const std::string& provider) {
-    return callJava<void*>(::runSensitivityAnalysis, sensitivityAnalysisContext, network, dc, &parameters, (char *) provider.data());
+JavaHandle runSensitivityAnalysis(const JavaHandle& sensitivityAnalysisContext, const JavaHandle& network, bool dc, load_flow_parameters& parameters, const std::string& provider) {
+    return callJava<JavaHandle>(::runSensitivityAnalysis, sensitivityAnalysisContext, network, dc, &parameters, (char *) provider.data());
 }
 
-matrix* getBranchFlowsSensitivityMatrix(void* sensitivityAnalysisResultContext, const std::string& contingencyId) {
+matrix* getBranchFlowsSensitivityMatrix(const JavaHandle& sensitivityAnalysisResultContext, const std::string& contingencyId) {
     return callJava<matrix*>(::getBranchFlowsSensitivityMatrix, sensitivityAnalysisResultContext,
                                 (char*) contingencyId.c_str());
 }
 
-matrix* getBusVoltagesSensitivityMatrix(void* sensitivityAnalysisResultContext, const std::string& contingencyId) {
+matrix* getBusVoltagesSensitivityMatrix(const JavaHandle& sensitivityAnalysisResultContext, const std::string& contingencyId) {
     return callJava<matrix*>(::getBusVoltagesSensitivityMatrix, sensitivityAnalysisResultContext,
                                 (char*) contingencyId.c_str());
 }
 
-matrix* getReferenceFlows(void* sensitivityAnalysisResultContext, const std::string& contingencyId) {
+matrix* getReferenceFlows(const JavaHandle& sensitivityAnalysisResultContext, const std::string& contingencyId) {
     return callJava<matrix*>(::getReferenceFlows, sensitivityAnalysisResultContext,
                                 (char*) contingencyId.c_str());
 }
 
-matrix* getReferenceVoltages(void* sensitivityAnalysisResultContext, const std::string& contingencyId) {
+matrix* getReferenceVoltages(const JavaHandle& sensitivityAnalysisResultContext, const std::string& contingencyId) {
     return callJava<matrix*>(::getReferenceVoltages, sensitivityAnalysisResultContext,
                                 (char*) contingencyId.c_str());
 }
 
-SeriesArray* createNetworkElementsSeriesArray(void* network, element_type elementType) {
+SeriesArray* createNetworkElementsSeriesArray(const JavaHandle& network, element_type elementType) {
     return new SeriesArray(callJava<array*>(::createNetworkElementsSeriesArray, network, elementType));
 }
 
 int getSeriesType(element_type elementType, const std::string& seriesName) {
     return callJava<int>(::getSeriesType, elementType, (char *) seriesName.c_str());
 }
 
-void updateNetworkElementsWithIntSeries(void* network, element_type elementType, const std::string& seriesName, const std::vector<std::string>& ids,
+void updateNetworkElementsWithIntSeries(const JavaHandle& network, element_type elementType, const std::string& seriesName, const std::vector<std::string>& ids,
                                         const std::vector<int>& values, int elementCount) {
     ToCharPtrPtr idPtr(ids);
     ToIntPtr valuePtr(values);
     callJava(::updateNetworkElementsWithIntSeries, network, elementType, (char *) seriesName.c_str(),
                     idPtr.get(), valuePtr.get(), elementCount);
 }
 
-void updateNetworkElementsWithDoubleSeries(void* network, element_type elementType, const std::string& seriesName, const std::vector<std::string>& ids,
+void updateNetworkElementsWithDoubleSeries(const JavaHandle& network, element_type elementType, const std::string& seriesName, const std::vector<std::string>& ids,
                                            const std::vector<double>& values, int elementCount) {
     ToCharPtrPtr idPtr(ids);
     ToDoublePtr valuePtr(values);
     callJava(::updateNetworkElementsWithDoubleSeries, network, elementType, (char *) seriesName.c_str(),
                     idPtr.get(), valuePtr.get(), elementCount);
 }
 
-void updateNetworkElementsWithStringSeries(void* network, element_type elementType, const std::string& seriesName, const std::vector<std::string>& ids,
+void updateNetworkElementsWithStringSeries(const JavaHandle& network, element_type elementType, const std::string& seriesName, const std::vector<std::string>& ids,
                                            const std::vector<std::string>& values, int elementCount) {
     ToCharPtrPtr idPtr(ids);
     ToCharPtrPtr valuePtr(values);
     callJava<>(::updateNetworkElementsWithStringSeries, network, elementType, (char *) seriesName.c_str(),
                 idPtr.get(), valuePtr.get(), elementCount);
 }
 
-void destroyObjectHandle(void* objectHandle) {
-    callJava<>(::destroyObjectHandle, objectHandle);
+std::string getWorkingVariantId(const JavaHandle& network) {
+    return toString(callJava<char*>(::getWorkingVariantId, network));
+}
+
+void setWorkingVariant(const JavaHandle& network, std::string& variant) {
+    callJava<>(::setWorkingVariant, network, (char*) variant.c_str());
+}
+
+void removeVariant(const JavaHandle& network, std::string& variant) {
+    callJava<>(::removeVariant, network, (char*) variant.c_str());
+}
+
+void cloneVariant(const JavaHandle& network, std::string& src, std::string& variant, bool mayOverwrite) {
+    callJava<>(::cloneVariant, network, (char*) src.c_str(), (char*) variant.c_str(), mayOverwrite);
+}
+
+std::vector<std::string> getVariantsIds(const JavaHandle& network) {
+    auto formatsArrayPtr = callJava<array*>(::getVariantsIds, network);
+    ToStringVector formats(formatsArrayPtr);
+    return formats.get();
+}
+void addMonitoredElements(const JavaHandle& securityAnalysisContext, contingency_context_type contingencyContextType, const std::vector<std::string>& branchIds,
+                      const std::vector<std::string>& voltageLevelIds, const std::vector<std::string>& threeWindingsTransformerIds,
+                      const std::vector<std::string>& contingencyIds) {
+    ToCharPtrPtr branchIdsPtr(branchIds);
+    ToCharPtrPtr voltageLevelIdsPtr(voltageLevelIds);
+    ToCharPtrPtr threeWindingsTransformerIdsPtr(threeWindingsTransformerIds);
+    ToCharPtrPtr contingencyIdsPtr(contingencyIds);
+    callJava<>(::addMonitoredElements, securityAnalysisContext, contingencyContextType, branchIdsPtr.get(), branchIds.size(),
+    voltageLevelIdsPtr.get(), voltageLevelIds.size(), threeWindingsTransformerIdsPtr.get(),
+    threeWindingsTransformerIds.size(), contingencyIdsPtr.get(), contingencyIds.size());
+}
+
+ContingencyResultArray* getSecurityAnalysisResult(const JavaHandle& securityAnalysisResult) {
+    return new ContingencyResultArray(callJava<array*>(::getSecurityAnalysisResult, securityAnalysisResult));
+}
+
+SeriesArray* getLimitViolations(const JavaHandle& securityAnalysisResult) {
+    return new SeriesArray(callJava<array*>(::getLimitViolations, securityAnalysisResult));
+}
+
+SeriesArray* getBranchResults(const JavaHandle& securityAnalysisResult) {
+    return new SeriesArray(callJava<array*>(::getBranchResults, securityAnalysisResult));
+}
+
+SeriesArray* getBusResults(const JavaHandle& securityAnalysisResult) {
+    return new SeriesArray(callJava<array*>(::getBusResults, securityAnalysisResult));
+}
+
+SeriesArray* getThreeWindingsTransformerResults(const JavaHandle& securityAnalysisResult) {
+    return new SeriesArray(callJava<array*>(::getThreeWindingsTransformerResults, securityAnalysisResult));
+}
+
+SeriesArray* getNodeBreakerViewSwitches(const JavaHandle& network, std::string& voltageLevel) {
+    return new SeriesArray(callJava<array*>(::getNodeBreakerViewSwitches, network, (char*) voltageLevel.c_str()));
+}
+
+SeriesArray* getNodeBreakerViewNodes(const JavaHandle& network, std::string& voltageLevel) {
+    return new SeriesArray(callJava<array*>(::getNodeBreakerViewNodes, network, (char*) voltageLevel.c_str()));
+}
+
+SeriesArray* getNodeBreakerViewInternalConnections(const JavaHandle& network, std::string& voltageLevel) {
+    return new SeriesArray(callJava<array*>(::getNodeBreakerViewInternalConnections, network, (char*) voltageLevel.c_str()));
 }
 
 }
```

### Comparing `pypowsybl-0.8.0/java/pom.xml` & `pypowsybl-0.9.0/java/pom.xml`

 * *Files 1% similar despite different names*

#### Comparing `pypowsybl-0.8.0/java/pom.xml` & `pypowsybl-0.9.0/java/pom.xml`

```diff
@@ -15,25 +15,26 @@
     <version>4</version>
     <relativePath/>
   </parent>
   <artifactId>pypowsybl</artifactId>
   <version>1.0.0-SNAPSHOT</version>
   <properties>
     <java.version>11</java.version>
-    <graalvm.version>20.3.0</graalvm.version>
+    <graalvm.version>21.2.0</graalvm.version>
     <janino.version>3.1.0</janino.version>
     <junit-jupiter.version>5.5.2</junit-jupiter.version>
     <logback.version>1.2.3</logback.version>
     <mapdb.version>3.0.8</mapdb.version>
     <maven-shade-plugin.version>3.2.4</maven-shade-plugin.version>
     <slf4j.version>1.7.30</slf4j.version>
-    <powsybl-core.version>4.2.0</powsybl-core.version>
-    <powsybl-rte-core.version>3.2.0</powsybl-rte-core.version>
-    <powsybl-single-line-diagram.version>2.2.0</powsybl-single-line-diagram.version>
-    <powsybl-open-load-flow.version>0.11.0</powsybl-open-load-flow.version>
+    <powsybl-core.version>4.3.1</powsybl-core.version>
+    <powsybl-rte-core.version>3.3.1</powsybl-rte-core.version>
+    <powsybl-single-line-diagram.version>2.3.0</powsybl-single-line-diagram.version>
+    <powsybl-open-load-flow.version>0.12.0</powsybl-open-load-flow.version>
+    <assertj.version>3.11.0</assertj.version>
   </properties>
   <build>
     <plugins>
       <plugin>
         <groupId>org.apache.maven.plugins</groupId>
         <artifactId>maven-shade-plugin</artifactId>
         <version>${maven-shade-plugin.version}</version>
@@ -206,9 +207,15 @@
     <!-- test -->
     <dependency>
       <groupId>org.junit.jupiter</groupId>
       <artifactId>junit-jupiter-engine</artifactId>
       <version>${junit-jupiter.version}</version>
       <scope>test</scope>
     </dependency>
+    <dependency>
+      <groupId>org.assertj</groupId>
+      <artifactId>assertj-core</artifactId>
+      <version>${assertj.version}</version>
+      <scope>test</scope>
+    </dependency>
   </dependencies>
 </project>
```

### Comparing `pypowsybl-0.8.0/java/src/main/resources/META-INF/native-image/reflect-config.json` & `pypowsybl-0.9.0/java/src/main/resources/META-INF/native-image/reflect-config.json`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/java/src/main/resources/pypowsybl-api.h` & `pypowsybl-0.9.0/java/src/main/resources/pypowsybl-api.h`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,22 @@
 } exception_handler;
 
 typedef struct array_struct {
     void* ptr;
     int length;
 } array;
 
+typedef struct network_metadata_struct {
+    char* id;
+    char* name;
+    double case_date; //seconds since epoch
+    char* source_format;
+    int forecast_distance;
+} network_metadata;
+
 typedef struct load_flow_component_result_struct {
     int connected_component_num;
     int synchronous_component_num;
     int status;
     int iteration_count;
     char* slack_bus_id;
     double slack_bus_active_power_mismatch;
@@ -63,27 +71,37 @@
     LINE,
     TWO_WINDINGS_TRANSFORMER,
     THREE_WINDINGS_TRANSFORMER,
     GENERATOR,
     LOAD,
     BATTERY,
     SHUNT_COMPENSATOR,
+    NON_LINEAR_SHUNT_COMPENSATOR_SECTION,
     DANGLING_LINE,
     LCC_CONVERTER_STATION,
     VSC_CONVERTER_STATION,
     STATIC_VAR_COMPENSATOR,
     SWITCH,
     VOLTAGE_LEVEL,
     SUBSTATION,
     BUSBAR_SECTION,
     HVDC_LINE,
     RATIO_TAP_CHANGER_STEP,
     PHASE_TAP_CHANGER_STEP,
+    RATIO_TAP_CHANGER,
+    PHASE_TAP_CHANGER,
+    REACTIVE_CAPABILITY_CURVE_POINT,
 } element_type;
 
+typedef enum {
+    ALL = 0,
+    NONE,
+    SPECIFIC,
+} contingency_context_type;
+
 typedef struct matrix_struct {
     int row_count;
     int column_count;
     double* values;
 } matrix;
 
 typedef struct series_struct {
```

### Comparing `pypowsybl-0.8.0/pypowsybl/loadflow.py` & `pypowsybl-0.9.0/pypowsybl/loadflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,13 +36,19 @@
                                         f", status={self.status.name}"\
                                         f", iteration_count={self.iteration_count!r}"\
                                         f", slack_bus_id={self.slack_bus_id!r}"\
                                         f", slack_bus_active_power_mismatch={self.slack_bus_active_power_mismatch!r}"\
                                         f")"
 
 
-def run_ac(network: Network, parameters: Parameters = Parameters(), provider = 'OpenLoadFlow'):
-    return _pypowsybl.run_load_flow(network.ptr, False, parameters, provider)
+def run_ac(network: Network, parameters: Parameters = None, provider='OpenLoadFlow'):
+    p = parameters
+    if parameters is None:
+        p = Parameters()
+    return _pypowsybl.run_load_flow(network._handle, False, p, provider)
 
 
-def run_dc(network: Network, parameters: Parameters = Parameters(), provider = 'OpenLoadFlow'):
-    return _pypowsybl.run_load_flow(network.ptr, True, parameters, provider)
+def run_dc(network: Network, parameters: Parameters = None, provider='OpenLoadFlow'):
+    p = parameters
+    if parameters is None:
+        p = Parameters()
+    return _pypowsybl.run_load_flow(network._handle, True, p, provider)
```

### Comparing `pypowsybl-0.8.0/pypowsybl/sensitivity.py` & `pypowsybl-0.9.0/pypowsybl/sensitivity.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,44 +7,40 @@
 from __future__ import annotations
 
 import _pypowsybl
 
 from pypowsybl.loadflow import Parameters
 from pypowsybl.network import Network
 from pypowsybl.util import ContingencyContainer
-from pypowsybl.util import ObjectHandle
 from _pypowsybl import PyPowsyblError
 from typing import List, Optional, Dict, Tuple
 from enum import Enum
 import numpy as np
 import pandas as pd
 
 TO_REMOVE='TO_REMOVE'
 
+
 class Zone:
-    def __init__(self, id: str, shift_keys_by_injections_ids: Dict[str, float] = {}):
+    def __init__(self, id: str, shift_keys_by_injections_ids: Dict[str, float] = None):
         self._id = id
-        self._shift_keys_by_injections_ids = shift_keys_by_injections_ids
+        self._shift_keys_by_injections_ids = {} if shift_keys_by_injections_ids is None else shift_keys_by_injections_ids
 
     @property
     def id(self):
         return self._id
 
     @property
     def shift_keys_by_injections_ids(self):
         return self._shift_keys_by_injections_ids
 
     @property
     def injections_ids(self):
         return list(self._shift_keys_by_injections_ids.keys())
 
-    @property
-    def shift_keys_by_injections_ids(self):
-        return self._shift_keys_by_injections_ids
-
     def get_shift_key(self, injection_id: str):
         shift_key = self._shift_keys_by_injections_ids.get(injection_id)
         if shift_key is None:
             raise PyPowsyblError(f'Injection {injection_id} not found')
         return shift_key
 
     def add_injection(self, id: str, key: float = 1):
@@ -95,22 +91,22 @@
         shift_keys_by_id = dict(zip(filtered_loads.index, filtered_loads.p0))
     else:
         raise PyPowsyblError(f'Unknown key type {key_type}')
 
     return Zone(country, shift_keys_by_id)
 
 
-class DcSensitivityAnalysisResult(ObjectHandle):
+class DcSensitivityAnalysisResult(object):
     """ Represents the result of a DC sensitivity analysis.
     The result contains computed values (so called "reference" values) and sensitivity values
     of requested factors, on the base case and on post contingency states.
     """
 
     def __init__(self, result_context_ptr, branches_ids: List[str], branch_data_frame_index: List[str]):
-        ObjectHandle.__init__(self, result_context_ptr)
+        self._handle = result_context_ptr
         self.result_context_ptr = result_context_ptr
         self.branches_ids = branches_ids
         self.branch_data_frame_index = branch_data_frame_index
 
     def get_branch_flows_sensitivity_matrix(self, contingency_id: str = None) -> Optional[pd.DataFrame]:
         """ Get the matrix of branch flows sensitivities on the base case or on the post contingency state depending if
         a contingency ID has been provided.
@@ -198,34 +194,29 @@
         else:
             data = np.array(m, copy=False)
             return pd.DataFrame(data=data, columns=self.bus_ids, index=['reference_voltages'])
 
 
 class SensitivityAnalysis(ContingencyContainer):
     """ Base class for sensitivity analysis. Do not instantiate it directly!"""
-    def __init__(self, ptr):
-        ContingencyContainer.__init__(self, ptr)
+    def __init__(self, handle):
+        ContingencyContainer.__init__(self, handle)
         self.branches_ids = None
         self.branch_data_frame_index = None
 
-    @staticmethod
-    def __create_cpp_zone(zone: Zone) -> _pypowsybl.Zone:
-        return _pypowsybl.Zone(zone.id, list(zone.shift_keys_by_injections_ids.keys()),
-                               list(zone.shift_keys_by_injections_ids.values()))
-
     def set_zones(self, zones: List[Zone]):
         """ Define zones that will be used in branch flow factor matrix.
         Args:
             zones: a list of zones
         """
         _zones = []
         for zone in zones:
             _zones.append(_pypowsybl.Zone(zone.id, list(zone.shift_keys_by_injections_ids.keys()),
                                           list(zone.shift_keys_by_injections_ids.values())))
-        _pypowsybl.set_zones(self.ptr, _zones)
+        _pypowsybl.set_zones(self._handle, _zones)
 
     def set_branch_flow_factor_matrix(self, branches_ids: List[str], variables_ids: List):
         """ Defines branch active power flow factor matrix, with a list of branches IDs and a list of variables.
         A variable could be:
          - a network element ID: injections, PSTs, dangling lines and HVDC lines are supported
          - a zone ID
          - a couple of zone ID to define a transfer between 2 zones
@@ -246,70 +237,76 @@
                 flatten_variables_ids.append(variable_id[0])
                 flatten_variables_ids.append(variable_id[1])
                 branch_data_frame_index.append(variable_id[0] + ' -> ' + variable_id[1])
                 branch_data_frame_index.append(TO_REMOVE)
             else:
                 raise PyPowsyblError(f'Unsupported factor variable type {type(variable_id)}')
 
-        _pypowsybl.set_branch_flow_factor_matrix(self.ptr, branches_ids, flatten_variables_ids)
+        _pypowsybl.set_branch_flow_factor_matrix(self._handle, branches_ids, flatten_variables_ids)
         self.branches_ids = branches_ids
         self.branch_data_frame_index = branch_data_frame_index
 
 
 class DcSensitivityAnalysis(SensitivityAnalysis):
     """ Represents a DC sensitivity analysis."""
-    def __init__(self, ptr):
-        SensitivityAnalysis.__init__(self, ptr)
+    def __init__(self, handle):
+        SensitivityAnalysis.__init__(self, handle)
 
-    def run(self, network: Network, parameters: Parameters = Parameters(), provider: str = 'OpenSensitivityAnalysis') -> DcSensitivityAnalysisResult:
+    def run(self, network: Network, parameters: Parameters = None, provider: str = 'OpenSensitivityAnalysis') -> DcSensitivityAnalysisResult:
         """ Runs the sensitivity analysis
 
         Args:
             network (Network): The network
             parameters (Parameters, optional): The load flow parameters
             provider (str, optional): Name of the sensitivity analysis provider
 
         Returns:
             a sensitivity analysis result
         """
-        return DcSensitivityAnalysisResult(_pypowsybl.run_sensitivity_analysis(self.ptr, network.ptr, True, parameters, provider),
+        p = parameters
+        if parameters is None:
+            p = Parameters()
+        return DcSensitivityAnalysisResult(_pypowsybl.run_sensitivity_analysis(self._handle, network._handle, True, p, provider),
                                            branches_ids=self.branches_ids, branch_data_frame_index=self.branch_data_frame_index)
 
 
 class AcSensitivityAnalysis(SensitivityAnalysis):
     """ Represents an AC sensitivity analysis."""
-    def __init__(self, ptr):
-        SensitivityAnalysis.__init__(self, ptr)
+    def __init__(self, handle):
+        SensitivityAnalysis.__init__(self, handle)
         self.bus_voltage_ids = None
         self.target_voltage_ids = None
 
     def set_bus_voltage_factor_matrix(self, bus_ids: List[str], target_voltage_ids: List[str]):
         """ Defines buses for which voltage sensitivities should be computed,
         and to which regulating equipments.
 
         Args:
             bus_ids: IDs of buses for which voltage sensitivities should be computed
             target_voltage_ids: IDs of regulating equipments to which we should compute sensitivities
         """
-        _pypowsybl.set_bus_voltage_factor_matrix(self.ptr, bus_ids, target_voltage_ids)
+        _pypowsybl.set_bus_voltage_factor_matrix(self._handle, bus_ids, target_voltage_ids)
         self.bus_voltage_ids = bus_ids
         self.target_voltage_ids = target_voltage_ids
 
-    def run(self, network: Network, parameters: Parameters = Parameters(), provider: str = 'OpenSensitivityAnalysis') -> AcSensitivityAnalysisResult:
+    def run(self, network: Network, parameters: Parameters = None, provider: str = 'OpenSensitivityAnalysis') -> AcSensitivityAnalysisResult:
         """ Runs the sensitivity analysis
 
         Args:
             network (Network): The network
             parameters (Parameters, optional): The load flow parameters
             provider (str, optional): Name of the sensitivity analysis provider
 
         Returns:
             a sensitivity analysis result
         """
-        return AcSensitivityAnalysisResult(_pypowsybl.run_sensitivity_analysis(self.ptr, network.ptr, False, parameters, provider),
+        p = parameters
+        if parameters is None:
+            p = Parameters()
+        return AcSensitivityAnalysisResult(_pypowsybl.run_sensitivity_analysis(self._handle, network._handle, False, p, provider),
                                            branches_ids=self.branches_ids, branch_data_frame_index=self.branch_data_frame_index,
                                            bus_ids=self.bus_voltage_ids, target_voltage_ids=self.target_voltage_ids)
 
 
 def create_dc_analysis() -> DcSensitivityAnalysis:
     """ Creates a new DC sensitivity analysis.
```

### Comparing `pypowsybl-0.8.0/pypowsybl/util.py` & `pypowsybl-0.9.0/pypowsybl/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,47 +7,41 @@
 import _pypowsybl
 from typing import List
 from typing import Callable
 import pandas as pd
 from _pypowsybl import PyPowsyblError
 
 
-class ObjectHandle:
-    def __init__(self, ptr):
-        self.ptr = ptr
-
-    def __del__(self):
-        _pypowsybl.destroy_object_handle(self.ptr)
-
-
-class ContingencyContainer(ObjectHandle):
-    def __init__(self, ptr):
-        ObjectHandle.__init__(self, ptr)
+class ContingencyContainer(object):
+    def __init__(self, handle):
+        self._handle = handle
 
     def add_single_element_contingency(self, element_id: str, contingency_id: str = None):
-        _pypowsybl.add_contingency(self.ptr, contingency_id if contingency_id else element_id, [element_id])
+        _pypowsybl.add_contingency(self._handle, contingency_id if contingency_id else element_id, [element_id])
 
     def add_multiple_elements_contingency(self, elements_ids: List[str], contingency_id: str):
-        _pypowsybl.add_contingency(self.ptr, contingency_id, elements_ids)
+        _pypowsybl.add_contingency(self._handle, contingency_id, elements_ids)
 
     def add_single_element_contingencies(self, elements_ids: List[str], contingency_id_provider: Callable[[str], str] = None):
         for element_id in elements_ids:
             contingency_id = contingency_id_provider(element_id) if contingency_id_provider else element_id
-            _pypowsybl.add_contingency(self.ptr, contingency_id, [element_id])
+            _pypowsybl.add_contingency(self._handle, contingency_id, [element_id])
 
 
 def create_data_frame_from_series_array(series_array):
     series_dict = {}
     index_data = []
     index_names = []
     for series in series_array:
         if series.index:
             index_data.append(series.data)
             index_names.append(series.name)
         else:
             series_dict[series.name] = series.data
     index = None
+    if not index_names:
+        raise ValueError('No index in returned dataframe')
     if len(index_names) == 1:
         index = pd.Index(index_data[0], name=index_names[0])
     else:
         index = pd.MultiIndex.from_arrays(index_data, names=index_names)
     return pd.DataFrame(series_dict, index=index)
```

### Comparing `pypowsybl-0.8.0/pypowsybl.egg-info/PKG-INFO` & `pypowsybl-0.9.0/pypowsybl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: pypowsybl
-Version: 0.8.0
+Version: 0.9.0
 Summary: A PowSyBl Python API
 Home-page: https://github.com/powsybl/pypowsybl
 Author: Geoffroy Jamgotchian
 Author-email: geoffroy.jamgotchian@gmail.com
 License: UNKNOWN
 Description: # PyPowSyBl
         
         [![Actions Status](https://github.com/powsybl/pypowsybl/workflows/CI/badge.svg)](https://github.com/powsybl/pypowsybl/actions)
+        [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=powsybl_pypowsybl&metric=alert_status)](https://sonarcloud.io/dashboard?id=powsybl_pypowsybl)
+        [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=powsybl_pypowsybl&metric=coverage)](https://sonarcloud.io/dashboard?id=powsybl_pypowsybl)
         [![PyPI Latest Release](https://img.shields.io/pypi/v/pypowsybl.svg)](https://pypi.org/project/pypowsybl/)
         [![Documentation Status](https://readthedocs.org/projects/pypowsybl/badge/?version=latest)](https://pypowsybl.readthedocs.io/en/latest/?badge=latest)
         [![MPL-2.0 License](https://img.shields.io/badge/license-MPL_2.0-blue.svg)](https://www.mozilla.org/en-US/MPL/2.0/)
         [![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/powsybl)
+        [![Slack](https://img.shields.io/badge/slack-powsybl-blueviolet.svg?logo=slack)](https://join.slack.com/t/powsybl/shared_invite/zt-rzvbuzjk-nxi0boim1RKPS5PjieI0rA)
         
-        The PyPowSyBl project gives access PowSyBl Java framework to Python developers. This Python integration relies on 
+        
+        The PyPowSyBl project gives access PowSyBl Java framework to Python developers. This Python integration relies on
         GraalVM to compile Java code to a native library.
         
         ## Installation
         
         PyPowSyBl is released on [PyPi](https://pypi.org/project/pypowsybl/).
         
         First, make sure you have an up-to-date version of pip and setuptools:
@@ -33,29 +37,29 @@
         
         ## Build from sources
         
         Requirements:
         
         - Maven >= 3.1
         - Cmake >= 3.14
-        - C++11 compiler 
+        - C++11 compiler
         - Python >= 3.7
-        - [GraalVM 20.3.0](https://github.com/graalvm/graalvm-ce-builds/releases/tag/vm-20.3.0) with [native image](https://www.graalvm.org/reference-manual/native-image/#install-native-image)
+        - [GraalVM 21.2.0](https://github.com/graalvm/graalvm-ce-builds/releases/tag/vm-21.2.0) with [native image](https://www.graalvm.org/reference-manual/native-image/#install-native-image)
         
         To build from sources and install PyPowSyBl package:
         ```bash
         git clone --recursive https://github.com/powsybl/pypowsybl.git
         export JAVA_HOME=<path to GraalVM>
         pip3 install --upgrade setuptools pip --user
         pip3 install . --user
         ```
         
         To run unit tests:
         ```bash
-        python3 -m unittest tests/test.py
+        python3 -m unittest discover --start-directory tests
         ```
         
         ## Usage
         
         First, we have to import pypowsybl:
         ```python
         import pypowsybl as pp
@@ -90,18 +94,18 @@
         ```
         
         We can re-run the load flow computation in DC mode:
         ```python
         results = pp.loadflow.run_dc(n)
         ```
         
-        Or with different parameters:
+        By default, the application read configs from `${HOME}/.itools/config.yml`
+        We can disable this with command :
         ```python
-        parameters = pp.loadflow.Parameters(distributed_slack=False)
-        results = pp.loadflow.run_ac(n, parameters)
+        pp.set_config_read(False)
         ```
         
         We can now get buses data (like any other network elements) as a [Pandas](https://pandas.pydata.org/) dataframe:
         ```python
         buses = n.get_buses()
         print(buses)
         ```
```

### Comparing `pypowsybl-0.8.0/pypowsybl.egg-info/SOURCES.txt` & `pypowsybl-0.9.0/pypowsybl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypowsybl-0.8.0/setup.py` & `pypowsybl-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,10 +163,11 @@
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
     ],
     python_requires='>=3.7',
     install_requires=[
         'prettytable',
-        'pandas'
+        'pandas',
+        'networkx'
     ],
 )
```


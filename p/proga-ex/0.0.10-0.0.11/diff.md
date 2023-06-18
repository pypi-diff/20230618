# Comparing `tmp/proga_ex-0.0.10.tar.gz` & `tmp/proga_ex-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proga_ex-0.0.10.tar", last modified: Sun Jun 18 18:04:38 2023, max compression
+gzip compressed data, was "proga_ex-0.0.11.tar", last modified: Sun Jun 18 18:10:19 2023, max compression
```

## Comparing `proga_ex-0.0.10.tar` & `proga_ex-0.0.11.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 18:04:38.208549 proga_ex-0.0.10/
--rw-rw-rw-   0        0        0      125 2023-06-18 18:04:38.208549 proga_ex-0.0.10/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 18:04:38.192924 proga_ex-0.0.10/proga_ex/
--rw-rw-rw-   0        0        0       19 2023-06-18 17:53:08.000000 proga_ex-0.0.10/proga_ex/__init__.py
--rw-rw-rw-   0        0        0   389778 2023-06-18 17:51:34.000000 proga_ex-0.0.10/proga_ex/exam.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:04:38.208549 proga_ex-0.0.10/proga_ex.egg-info/
--rw-rw-rw-   0        0        0      125 2023-06-18 18:04:38.000000 proga_ex-0.0.10/proga_ex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-06-18 18:04:38.000000 proga_ex-0.0.10/proga_ex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 18:04:38.000000 proga_ex-0.0.10/proga_ex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-18 18:04:38.000000 proga_ex-0.0.10/proga_ex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-06-18 18:04:38.208549 proga_ex-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0      256 2023-06-18 18:04:29.000000 proga_ex-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:10:19.230031 proga_ex-0.0.11/
+-rw-rw-rw-   0        0        0      125 2023-06-18 18:10:19.230031 proga_ex-0.0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 18:10:19.214404 proga_ex-0.0.11/proga_ex/
+-rw-rw-rw-   0        0        0       19 2023-06-18 17:53:08.000000 proga_ex-0.0.11/proga_ex/__init__.py
+-rw-rw-rw-   0        0        0   389745 2023-06-18 18:09:18.000000 proga_ex-0.0.11/proga_ex/exam.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:10:19.230031 proga_ex-0.0.11/proga_ex.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-06-18 18:10:19.000000 proga_ex-0.0.11/proga_ex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-06-18 18:10:19.000000 proga_ex-0.0.11/proga_ex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 18:10:19.000000 proga_ex-0.0.11/proga_ex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-18 18:10:19.000000 proga_ex-0.0.11/proga_ex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-06-18 18:10:19.230031 proga_ex-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      256 2023-06-18 18:09:31.000000 proga_ex-0.0.11/setup.py
```

### Comparing `proga_ex-0.0.10/proga_ex/exam.py` & `proga_ex-0.0.11/proga_ex/exam.py`

 * *Files 0% similar despite different names*

```diff
@@ -7557,11 +7557,7 @@
 
 print(r1 == r2) # False
 print(r1 == r3) # True
 
 '''
         }
         print(sklad[n])
-
-
-prog.list_()
-prog.pract27(3)
```


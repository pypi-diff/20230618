# Comparing `tmp/creditagricole_particuliers-0.8.0.tar.gz` & `tmp/creditagricole_particuliers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creditagricole_particuliers-0.8.0.tar", last modified: Fri Dec 30 21:16:32 2022, max compression
+gzip compressed data, was "creditagricole_particuliers-0.9.0.tar", last modified: Sun Jan  8 08:49:55 2023, max compression
```

## Comparing `creditagricole_particuliers-0.8.0.tar` & `creditagricole_particuliers-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 21:16:32.748776 creditagricole_particuliers-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2022-12-30 21:16:32.748776 creditagricole_particuliers-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 21:16:32.748776 creditagricole_particuliers-0.8.0/creditagricole_particuliers/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers/iban.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2022-12-30 21:16:23.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers/regionalbanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 21:16:32.748776 creditagricole_particuliers-0.8.0/creditagricole_particuliers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2022-12-30 21:16:32.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-30 21:16:32.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 21:16:32.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-30 21:16:32.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-30 21:16:32.000000 creditagricole_particuliers-0.8.0/creditagricole_particuliers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-30 21:16:32.748776 creditagricole_particuliers-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2022-12-30 21:16:31.000000 creditagricole_particuliers-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 08:49:55.202728 creditagricole_particuliers-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-01-08 08:49:55.202728 creditagricole_particuliers-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 08:49:55.202728 creditagricole_particuliers-0.9.0/creditagricole_particuliers/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers/iban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-08 08:49:44.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers/regionalbanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 08:49:55.202728 creditagricole_particuliers-0.9.0/creditagricole_particuliers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-01-08 08:49:55.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-08 08:49:55.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 08:49:55.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-08 08:49:55.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-08 08:49:55.000000 creditagricole_particuliers-0.9.0/creditagricole_particuliers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 08:49:55.202728 creditagricole_particuliers-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-01-08 08:49:53.000000 creditagricole_particuliers-0.9.0/setup.py
```

### Comparing `creditagricole_particuliers-0.8.0/LICENSE` & `creditagricole_particuliers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/PKG-INFO` & `creditagricole_particuliers-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creditagricole_particuliers
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client pour la banque Crédit Agricole
 Home-page: https://github.com/dmachard/creditagricole-particuliers
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: credit agricole api banking banque
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `creditagricole_particuliers-0.8.0/README.md` & `creditagricole_particuliers-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers/accounts.py` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers/accounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,8 +109,22 @@
                 self.accounts_list.append( Account(self.session, descr) )
 
     def get_solde(self):
         """get global solde"""
         solde = 0
         for acc in self.accounts_list:
             solde += acc.get_solde()
-        return round(solde, 2)
+        return round(solde, 2)
+
+    def get_solde_per_products(self):
+        """get solde per products"""
+        ret_soldes = {}
+        for f in FAMILLE_PRODUITS:
+            ret_soldes[f["familleProduit"]] = 0.0
+
+        for f in FAMILLE_PRODUITS:
+            for acc in self.accounts_list:
+                if int(acc.grandeFamilleCode) == f["code"]:
+                    ret_soldes[f["familleProduit"]] += acc.get_solde()
+            ret_soldes[f["familleProduit"]] = round(ret_soldes[f["familleProduit"]], 2)
+
+        return ret_soldes
```

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers/authenticator.py` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers/authenticator.py`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers/cards.py` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers/cards.py`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers/iban.py` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers/iban.py`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers/logout.py` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers/logout.py`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers/operations.py` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers/operations.py`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers/regionalbanks.py` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers/regionalbanks.py`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers.egg-info/PKG-INFO` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creditagricole-particuliers
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client pour la banque Crédit Agricole
 Home-page: https://github.com/dmachard/creditagricole-particuliers
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: credit agricole api banking banque
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `creditagricole_particuliers-0.8.0/creditagricole_particuliers.egg-info/SOURCES.txt` & `creditagricole_particuliers-0.9.0/creditagricole_particuliers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creditagricole_particuliers-0.8.0/setup.py` & `creditagricole_particuliers-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
     
 KEYWORDS = ('credit agricole api banking banque')
 
 setuptools.setup(
     name="creditagricole_particuliers",
-    version="0.8.0",
+    version="0.9.0",
     author="Denis MACHARD",
     author_email="d.machard@gmail.com",
     description="Python client pour la banque Crédit Agricole",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/dmachard/creditagricole-particuliers",
     packages=['creditagricole_particuliers'],
```


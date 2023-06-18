# Comparing `tmp/homelab_node_red_backup-1.1.1.tar.gz` & `tmp/homelab_node_red_backup-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homelab_node_red_backup-1.1.1.tar", max compression
+gzip compressed data, was "homelab_node_red_backup-1.3.0.tar", max compression
```

## Comparing `homelab_node_red_backup-1.1.1.tar` & `homelab_node_red_backup-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1133 2023-06-18 11:29:30.133506 homelab_node_red_backup-1.1.1/LICENSE.md
--rw-r--r--   0        0        0     3042 2023-06-18 11:59:20.788562 homelab_node_red_backup-1.1.1/README.md
--rw-r--r--   0        0        0       46 2023-06-18 09:42:36.942073 homelab_node_red_backup-1.1.1/homelab_node_red_backup/__init__.py
--rw-r--r--   0        0        0     2186 2023-06-18 11:15:31.290878 homelab_node_red_backup-1.1.1/homelab_node_red_backup/__main__.py
--rw-r--r--   0        0        0       35 2023-06-18 10:37:38.701060 homelab_node_red_backup-1.1.1/homelab_node_red_backup/handler/__init__.py
--rw-r--r--   0        0        0     1658 2023-06-18 11:18:54.546243 homelab_node_red_backup-1.1.1/homelab_node_red_backup/handler/backup.py
--rw-r--r--   0        0        0      444 2023-06-18 11:03:46.745376 homelab_node_red_backup-1.1.1/homelab_node_red_backup/handler/check.py
--rw-r--r--   0        0        0      705 2023-06-18 11:10:59.339512 homelab_node_red_backup-1.1.1/homelab_node_red_backup/handler/flows.py
--rw-r--r--   0        0        0      565 2023-06-18 11:16:24.604019 homelab_node_red_backup-1.1.1/homelab_node_red_backup/handler/restore.py
--rw-r--r--   0        0        0     2395 2023-06-18 12:01:49.043907 homelab_node_red_backup-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 homelab_node_red_backup-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     3042 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/README.md
+-rw-r--r--   0        0        0       46 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/__init__.py
+-rw-r--r--   0        0        0     2186 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/__main__.py
+-rw-r--r--   0        0        0       35 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/__init__.py
+-rw-r--r--   0        0        0     1658 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/backup.py
+-rw-r--r--   0        0        0      444 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/check.py
+-rw-r--r--   0        0        0      705 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/flows.py
+-rw-r--r--   0        0        0      565 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/restore.py
+-rw-r--r--   0        0        0     2152 2023-06-18 13:05:44.937843 homelab_node_red_backup-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 homelab_node_red_backup-1.3.0/PKG-INFO
```

### Comparing `homelab_node_red_backup-1.1.1/LICENSE.md` & `homelab_node_red_backup-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.1.1/README.md` & `homelab_node_red_backup-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.1.1/homelab_node_red_backup/__main__.py` & `homelab_node_red_backup-1.3.0/homelab_node_red_backup/__main__.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.1.1/homelab_node_red_backup/handler/backup.py` & `homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/backup.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.1.1/homelab_node_red_backup/handler/flows.py` & `homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/flows.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.1.1/homelab_node_red_backup/handler/restore.py` & `homelab_node_red_backup-1.3.0/homelab_node_red_backup/handler/restore.py`

 * *Files identical despite different names*

### Comparing `homelab_node_red_backup-1.1.1/PKG-INFO` & `homelab_node_red_backup-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homelab-node-red-backup
-Version: 1.1.1
+Version: 1.3.0
 Summary: Backup and Restore for Node-RED.
 Home-page: https://github.com/muhlba91/onyx-client
 License: MIT
 Keywords: node-red,homelab
 Author: Daniel Muehlbachler-Pietrzykowski
 Author-email: daniel.muehlbachler@niftyside.io
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: homelab-node-red-backup Version: 1.1.1 Summary:
+Metadata-Version: 2.1 Name: homelab-node-red-backup Version: 1.3.0 Summary:
 Backup and Restore for Node-RED. Home-page: https://github.com/muhlba91/onyx-
 client License: MIT Keywords: node-red,homelab Author: Daniel Muehlbachler-
 Pietrzykowski Author-email: daniel.muehlbachler@niftyside.io Requires-Python:
 >=3.11,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/gardena_bluetooth-0.3.0.tar.gz` & `tmp/gardena_bluetooth-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardena_bluetooth-0.3.0.tar", max compression
+gzip compressed data, was "gardena_bluetooth-0.3.1.tar", max compression
```

## Comparing `gardena_bluetooth-0.3.0.tar` & `gardena_bluetooth-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2023-06-16 23:12:41.851169 gardena_bluetooth-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      704 2023-06-16 23:12:41.851169 gardena_bluetooth-0.3.0/README.rst
--rw-r--r--   0        0        0     3007 2023-06-16 23:12:41.851169 gardena_bluetooth-0.3.0/gardena_bluetooth/__init__.py
--rw-r--r--   0        0        0     2234 2023-06-16 23:12:41.851169 gardena_bluetooth-0.3.0/gardena_bluetooth/__main__.py
--rw-r--r--   0        0        0     4938 2023-06-16 23:12:41.851169 gardena_bluetooth-0.3.0/gardena_bluetooth/const.py
--rw-r--r--   0        0        0      186 2023-06-16 23:12:41.851169 gardena_bluetooth-0.3.0/gardena_bluetooth/exceptions.py
--rw-r--r--   0        0        0     5094 2023-06-16 23:12:41.851169 gardena_bluetooth-0.3.0/gardena_bluetooth/parse.py
--rw-r--r--   0        0        0      739 2023-06-16 23:12:41.855169 gardena_bluetooth-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 gardena_bluetooth-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      704 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/README.rst
+-rw-r--r--   0        0        0     3013 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/__init__.py
+-rw-r--r--   0        0        0     2234 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/__main__.py
+-rw-r--r--   0        0        0     4938 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/const.py
+-rw-r--r--   0        0        0      186 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/exceptions.py
+-rw-r--r--   0        0        0     5094 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/gardena_bluetooth/parse.py
+-rw-r--r--   0        0        0      739 2023-06-18 20:28:36.022564 gardena_bluetooth-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 gardena_bluetooth-0.3.1/PKG-INFO
```

### Comparing `gardena_bluetooth-0.3.0/LICENSE.txt` & `gardena_bluetooth-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.0/README.rst` & `gardena_bluetooth-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.0/gardena_bluetooth/__init__.py` & `gardena_bluetooth-0.3.1/gardena_bluetooth/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     client: BleakClient,
     char: Characteristic[CharacteristicType],
     value: CharacteristicType,
     response=True,
 ) -> None:
     """Write data to a characteristic."""
     data = char.encode(value)
-    write_char_raw(client, char.uuid, data, response)
+    await write_char_raw(client, char.uuid, data, response)
 
 
 async def update_timestamp(client: BleakClient, now: datetime):
     timestamp = await read_char(client, DeviceConfiguration.unix_timestamp)
     timestamp = timestamp.replace(tzinfo=now.tzinfo)
     delta = timestamp - now
     if abs(delta.total_seconds()) > 60:
```

### Comparing `gardena_bluetooth-0.3.0/gardena_bluetooth/__main__.py` & `gardena_bluetooth-0.3.1/gardena_bluetooth/__main__.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.0/gardena_bluetooth/const.py` & `gardena_bluetooth-0.3.1/gardena_bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.0/gardena_bluetooth/parse.py` & `gardena_bluetooth-0.3.1/gardena_bluetooth/parse.py`

 * *Files identical despite different names*

### Comparing `gardena_bluetooth-0.3.0/pyproject.toml` & `gardena_bluetooth-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gardena-bluetooth"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Joakim Plate <elupus@ecce.se>"]
 readme = "README.rst"
 packages = [{include = "gardena_bluetooth"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gardena_bluetooth-0.3.0/PKG-INFO` & `gardena_bluetooth-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gardena-bluetooth
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Joakim Plate
 Author-email: elupus@ecce.se
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/serial_packets-0.1.1.tar.gz` & `tmp/serial_packets-0.1.2.tar.gz`

## Comparing `serial_packets-0.1.1.tar` & `serial_packets-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/__init__.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/_interval_tracker.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/_packet_decoder.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/_packet_encoder.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/client.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.1/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.1/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.1/LICENSE
--rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 serial_packets-0.1.1/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    16624 2020-02-02 00:00:00.000000 serial_packets-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/_interval_tracker.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/_packet_decoder.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/_packet_encoder.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/client.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.1.2/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.1.2/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.1.2/LICENSE
+-rw-r--r--   0        0        0    16077 2020-02-02 00:00:00.000000 serial_packets-0.1.2/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 serial_packets-0.1.2/PKG-INFO
```

### Comparing `serial_packets-0.1.1/src/serial_packets/_interval_tracker.py` & `serial_packets-0.1.2/src/serial_packets/_interval_tracker.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.1/src/serial_packets/_packet_decoder.py` & `serial_packets-0.1.2/src/serial_packets/_packet_decoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.1/src/serial_packets/_packet_encoder.py` & `serial_packets-0.1.2/src/serial_packets/_packet_encoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.1/src/serial_packets/_packets.py` & `serial_packets-0.1.2/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.1/src/serial_packets/client.py` & `serial_packets-0.1.2/src/serial_packets/client.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.1/src/serial_packets/packets.py` & `serial_packets-0.1.2/src/serial_packets/packets.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,17 +63,20 @@
 
     def __init__(self):
         """ Constructs a PacketData with given initial data."""
         self.__data: bytearray = bytearray()
         self.__bytes_read: int = 0
         self.__read_error: bool = False
 
-    def hex_str(self) -> str:
+    def hex_str(self, max_bytes=None) -> str:
         """Returns a string with a hex dump fo the bytes. Can be long."""
-        return self.__data.hex(sep=' ')
+        if (max_bytes is None) or (self.size() <= max_bytes):
+            return  self.__data.hex(sep=' ')
+        prefix = self.__data[:max_bytes].hex(sep=" ")
+        return f"{prefix} ... ({self.size() - max_bytes} more)"
 
     def data_bytes(self) -> bytearray:
         """Return a copy of the data bytes."""
         return self.__data.copy()
 
     def _internal_bytes_buffer(self) -> bytearray:
         """Package private. Returns a reference to the internal bytearray. Do not mutate."""
@@ -151,31 +154,45 @@
             self.__read_error = True
             return None
         result = self.__data[self.__bytes_read]
         self.__bytes_read += 1
         return result
 
     def read_uint16(self) -> int | None:
-        """Decods the next 2 bytes as a 16 bits unsigned big endian value.
-        Returns the 16 bit numbmer and advances the reading location by 2 bytes,
-        or returns None if insuffient number of bytes to read.
+        """Decodes the next 2 bytes as a 16 bits unsigned big endian value.
+        Returns the 16 bit number and advances the reading location by 2 bytes,
+        or returns None if insufficient number of bytes to read.
         """
         if self.__read_error or self.__bytes_read + 2 > len(self.__data):
             self.__read_error = True
             return None
         result = int.from_bytes(self.__data[self.__bytes_read:self.__bytes_read + 2],
                                 byteorder='big',
                                 signed=False)
         self.__bytes_read += 2
         return result
+      
+    def read_int24(self) -> int | None:
+        """Decodes the next 3 bytes as a 24 bits signed big endian value.
+        Returns the 24 bit number and advances the reading location by 3 bytes,
+        or returns None if insufficient number of bytes to read.
+        """
+        if self.__read_error or self.__bytes_read + 3 > len(self.__data):
+            self.__read_error = True
+            return None
+        result = int.from_bytes(self.__data[self.__bytes_read:self.__bytes_read + 3],
+                                byteorder='big',
+                                signed=True)
+        self.__bytes_read += 3
+        return result
 
     def read_uint32(self) -> int | None:
-        """Decods the next 4 bytes as am unsigned  32 bits big endian value.
-        Returns the 32 bit numbmer and advances the reading location by 4 bytes,
-        or returns None if insuffient number of bytes to read.
+        """Decodes the next 4 bytes as am unsigned  32 bits big endian value.
+        Returns the 32 bit number and advances the reading location by 4 bytes,
+        or returns None if insufficient number of bytes to read.
         """
         if self.__read_error or self.__bytes_read + 4 > len(self.__data):
             self.__read_error = True
             return None
         result = int.from_bytes(self.__data[self.__bytes_read:self.__bytes_read + 4],
                                 byteorder='big',
                                 signed=False)
```

### Comparing `serial_packets-0.1.1/LICENSE` & `serial_packets-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.1.1/README.md` & `serial_packets-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -297,17 +297,14 @@
 | 7 - 99       | Reserved         | For future protocol definitions.     |
 | 100-255      | Custom           | For user's application specific use. |
 
 ## Endpoints
 
 Endpoints represent the destinations of commands and messages on the receiving node and allows the application to distinguish between command and message types. End points are identified by a single byte, where the values 0-199 are available for the application, and the values 200-255 are reserved for future expansions of the protocol.
 
-## Data
-
-Commands, responses and messages pass  data which is a sequence of zero to 1024 bytes. These bytes are opaque to the protocol which treat them as a blob. It's up to the application to determine the semantic of these bytes and to encode and decode them as needed.
 
 ## Application Example
 
 The repository contains and example with two main programs that communicate between them via serial port. One program called 'master' periodically sends a command and waits for a response and the other one called 'slave' sends a message periodically. To run the example, use two USB/Serial adapters and connect the TX of the first to the RX of the second and vice versa. Also, make sure to connect the gwo grounds. Then run each of the two program, providing the respective port in the command line. Make sure to replace the serial port ids in the example below with the actual port id of your system.
 
 <https://github.com/zapta/serial_packets_py/tree/main/src/examples>
```

### Comparing `serial_packets-0.1.1/pyproject.toml` & `serial_packets-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.1.1/PKG-INFO` & `serial_packets-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
@@ -313,17 +313,14 @@
 | 7 - 99       | Reserved         | For future protocol definitions.     |
 | 100-255      | Custom           | For user's application specific use. |
 
 ## Endpoints
 
 Endpoints represent the destinations of commands and messages on the receiving node and allows the application to distinguish between command and message types. End points are identified by a single byte, where the values 0-199 are available for the application, and the values 200-255 are reserved for future expansions of the protocol.
 
-## Data
-
-Commands, responses and messages pass  data which is a sequence of zero to 1024 bytes. These bytes are opaque to the protocol which treat them as a blob. It's up to the application to determine the semantic of these bytes and to encode and decode them as needed.
 
 ## Application Example
 
 The repository contains and example with two main programs that communicate between them via serial port. One program called 'master' periodically sends a command and waits for a response and the other one called 'slave' sends a message periodically. To run the example, use two USB/Serial adapters and connect the TX of the first to the RX of the second and vice versa. Also, make sure to connect the gwo grounds. Then run each of the two program, providing the respective port in the command line. Make sure to replace the serial port ids in the example below with the actual port id of your system.
 
 <https://github.com/zapta/serial_packets_py/tree/main/src/examples>
```


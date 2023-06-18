# Comparing `tmp/electrickiwi-api-0.8.4.tar.gz` & `tmp/electrickiwi-api-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrickiwi-api-0.8.4.tar", last modified: Tue Apr 25 09:48:11 2023, max compression
+gzip compressed data, was "electrickiwi-api-0.8.5.tar", last modified: Sun Jun 18 21:40:12 2023, max compression
```

## Comparing `electrickiwi-api-0.8.4.tar` & `electrickiwi-api-0.8.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:48:11.501531 electrickiwi-api-0.8.4/
--rw-rw-r--   0 michael   (1000) michael   (1000)    35149 2022-10-20 08:35:26.000000 electrickiwi-api-0.8.4/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-04-25 09:48:11.501531 electrickiwi-api-0.8.4/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     1678 2023-04-25 09:47:44.000000 electrickiwi-api-0.8.4/README.md
--rw-rw-r--   0 michael   (1000) michael   (1000)      976 2023-04-25 09:47:44.000000 electrickiwi-api-0.8.4/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      177 2023-04-25 09:48:11.502530 electrickiwi-api-0.8.4/setup.cfg
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:48:11.493531 electrickiwi-api-0.8.4/src/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:48:11.498530 electrickiwi-api-0.8.4/src/electrickiwi_api/
--rw-rw-r--   0 michael   (1000) michael   (1000)      428 2023-04-25 09:47:44.000000 electrickiwi-api-0.8.4/src/electrickiwi_api/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9031 2023-04-17 05:33:03.000000 electrickiwi-api-0.8.4/src/electrickiwi_api/api.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1588 2023-04-25 08:16:42.000000 electrickiwi-api-0.8.4/src/electrickiwi_api/auth.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      483 2023-03-22 18:50:16.000000 electrickiwi-api-0.8.4/src/electrickiwi_api/exceptions.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    21334 2023-04-17 05:26:30.000000 electrickiwi-api-0.8.4/src/electrickiwi_api/model.py
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-04-25 09:17:55.000000 electrickiwi-api-0.8.4/src/electrickiwi_api/py.typed
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:48:11.500531 electrickiwi-api-0.8.4/src/electrickiwi_api.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-04-25 09:48:11.000000 electrickiwi-api-0.8.4/src/electrickiwi_api.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      469 2023-04-25 09:48:11.000000 electrickiwi-api-0.8.4/src/electrickiwi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-25 09:48:11.000000 electrickiwi-api-0.8.4/src/electrickiwi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       15 2023-04-25 09:48:11.000000 electrickiwi-api-0.8.4/src/electrickiwi_api.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       17 2023-04-25 09:48:11.000000 electrickiwi-api-0.8.4/src/electrickiwi_api.egg-info/top_level.txt
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-25 09:48:11.500531 electrickiwi-api-0.8.4/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1382 2022-12-16 23:22:54.000000 electrickiwi-api-0.8.4/tests/test_instance.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-18 21:40:12.113804 electrickiwi-api-0.8.5/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    35149 2022-10-20 08:35:26.000000 electrickiwi-api-0.8.5/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-06-18 21:40:12.113804 electrickiwi-api-0.8.5/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1678 2023-06-18 21:39:57.000000 electrickiwi-api-0.8.5/README.md
+-rw-rw-r--   0 michael   (1000) michael   (1000)      976 2023-06-18 21:39:57.000000 electrickiwi-api-0.8.5/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      177 2023-06-18 21:40:12.113804 electrickiwi-api-0.8.5/setup.cfg
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-18 21:40:12.109804 electrickiwi-api-0.8.5/src/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-18 21:40:12.112804 electrickiwi-api-0.8.5/src/electrickiwi_api/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      428 2023-06-18 21:39:57.000000 electrickiwi-api-0.8.5/src/electrickiwi_api/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9031 2023-04-17 05:33:03.000000 electrickiwi-api-0.8.5/src/electrickiwi_api/api.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1588 2023-04-25 08:16:42.000000 electrickiwi-api-0.8.5/src/electrickiwi_api/auth.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      483 2023-03-22 18:50:16.000000 electrickiwi-api-0.8.5/src/electrickiwi_api/exceptions.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    21537 2023-06-18 21:38:29.000000 electrickiwi-api-0.8.5/src/electrickiwi_api/model.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-04-25 09:17:55.000000 electrickiwi-api-0.8.5/src/electrickiwi_api/py.typed
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-18 21:40:12.112804 electrickiwi-api-0.8.5/src/electrickiwi_api.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1899 2023-06-18 21:40:11.000000 electrickiwi-api-0.8.5/src/electrickiwi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      469 2023-06-18 21:40:12.000000 electrickiwi-api-0.8.5/src/electrickiwi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-06-18 21:40:11.000000 electrickiwi-api-0.8.5/src/electrickiwi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       15 2023-06-18 21:40:11.000000 electrickiwi-api-0.8.5/src/electrickiwi_api.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       17 2023-06-18 21:40:11.000000 electrickiwi-api-0.8.5/src/electrickiwi_api.egg-info/top_level.txt
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-18 21:40:12.113804 electrickiwi-api-0.8.5/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1382 2022-12-16 23:22:54.000000 electrickiwi-api-0.8.5/tests/test_instance.py
```

### Comparing `electrickiwi-api-0.8.4/LICENSE` & `electrickiwi-api-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.4/PKG-INFO` & `electrickiwi-api-0.8.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: electrickiwi-api
-Version: 0.8.4
+Version: 0.8.5
 Author-email: Michael Arthur <michael@jumblesoft.co.nz>
 License: GNU-3.0
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Electric Kiwi Python API
 
-[![SemVer 0.8.4][img_version]][url_version]
+[![SemVer 0.8.5][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
 
-[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.4&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.5&color=blue
 [url_version]: https://pypi.org/project/electrickiwi-api/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/electrickiwi-api/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/electrickiwi-api.svg
 [url_pyversions]: https://pypi.python.org/pypi/electrickiwi-api
```

### Comparing `electrickiwi-api-0.8.4/README.md` & `electrickiwi-api-0.8.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Electric Kiwi Python API
 
-[![SemVer 0.8.4][img_version]][url_version]
+[![SemVer 0.8.5][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
 
-[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.4&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.5&color=blue
 [url_version]: https://pypi.org/project/electrickiwi-api/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/electrickiwi-api/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/electrickiwi-api.svg
 [url_pyversions]: https://pypi.python.org/pypi/electrickiwi-api
```

### Comparing `electrickiwi-api-0.8.4/pyproject.toml` & `electrickiwi-api-0.8.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "electrickiwi-api"
-version     = "0.8.4"
+version     = "0.8.5"
 license     = {text = "GNU-3.0"}
 description = ""
 readme      = "README.md"
 authors     = [
     {name = "Michael Arthur", email = "michael@jumblesoft.co.nz"}
 ]
 
 
 requires-python = ">=3.9.0"
 dependencies    = [
     "aiohttp>=3.8.1"
     ]
 
 [tool.bumpver]
-current_version = "0.8.4"
+current_version = "0.8.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
```

### Comparing `electrickiwi-api-0.8.4/src/electrickiwi_api/api.py` & `electrickiwi-api-0.8.5/src/electrickiwi_api/api.py`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.4/src/electrickiwi_api/auth.py` & `electrickiwi-api-0.8.5/src/electrickiwi_api/auth.py`

 * *Files identical despite different names*

### Comparing `electrickiwi-api-0.8.4/src/electrickiwi_api/model.py` & `electrickiwi-api-0.8.5/src/electrickiwi_api/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,52 +143,53 @@
             _gender,
             _is_active,
             _medically_dependent_customer,
         )
 
 
 @dataclass
-class Hop:
+class ConnectionHop:
+    """Individual Hop start or end on customer connection"""
     start_time: str
     end_time: str
     interval_start: str
     interval_end: str
 
     @staticmethod
     def from_dict(obj: Any) -> "Hop":
         _start_time = str(obj.get("start_time"))
         _end_time = str(obj.get("end_time"))
         _interval_start = str(obj.get("interval_start"))
         _interval_end = str(obj.get("interval_end"))
-        return Hop(_start_time, _end_time, _interval_start, _interval_end)
+        return ConnectionHop(_start_time, _end_time, _interval_start, _interval_end)
 
 
 @dataclass
 class CustomerConnection:
     type: str
     id: int
     customer_number: int
     identifier: str
     address: str
     is_active: str
-    hop: Hop
+    hop: ConnectionHop
     start_date: str
     end_date: str
 
     @staticmethod
     def from_dict(customer_connection_data: Any) -> "CustomerConnection":
         customer_connection = customer_connection_data.get("data")
 
         _type = str(customer_connection.get("type"))
         _id = int(customer_connection.get("id"))
         _customer_number = int(customer_connection.get("customer_number"))
         _identifier = str(customer_connection.get("identifier"))
         _address = str(customer_connection.get("address"))
         _is_active = str(customer_connection.get("is_active"))
-        _hop = Hop.from_dict(customer_connection.get("hop"))
+        _hop = ConnectionHop.from_dict(customer_connection.get("hop"))
         _start_date = str(customer_connection.get("start_date"))
         _end_date = str(customer_connection.get("end_date"))
         return CustomerConnection(
             _type,
             _id,
             _customer_number,
             _identifier,
@@ -372,23 +373,23 @@
         _file_name = str(bill_file.get("file_name"))
         _id = int(bill_file.get("id"))
         _type = str(bill_file.get("type"))
         return BillFile(_file_base64, _file_name, _id, _type)
 
 
 @dataclass
-class Range:
+class ConsumptionRange:
     end_date: str
     start_date: str
 
     @staticmethod
-    def from_dict(obj: Any) -> "Range":
+    def from_dict(obj: Any) -> "ConsumptionRange":
         _end_date = str(obj.get("end_date"))
         _start_date = str(obj.get("start_date"))
-        return Range(_end_date, _start_date)
+        return ConsumptionRange(_end_date, _start_date)
 
 
 @dataclass
 class UsageCharge:
     end_date: str
     fixed_rate_incl_gst: str
     hop_saving: str
@@ -423,22 +424,22 @@
             _total_variable_charges_incl_gst,
             _variable_rate_incl_gst,
         )
 
 
 @dataclass
 class ConsumptionSummary:
-    range: Range
+    range: ConsumptionRange
     usage_charges: List[UsageCharge]
     type: str
 
     @staticmethod
     def from_dict(consumption_summary_data: Any) -> "ConsumptionSummary":
         consumption_summary = consumption_summary_data.get("data")
-        _range = Range.from_dict(consumption_summary.get("range"))
+        _range = ConsumptionRange.from_dict(consumption_summary.get("range"))
         _usage_charges = [
             UsageCharge.from_dict(y) for y in consumption_summary.get("usage_charges")
         ]
         _type = str(consumption_summary.get("type"))
         return ConsumptionSummary(_range, _usage_charges, _type)
 
 
@@ -456,24 +457,38 @@
         _consumption = str(obj.get("consumption"))
         _hop_best = int(obj.get("hop_best"))
         _time = str(obj.get("time"))
         return Interval(_consumption, _hop_best, _time)
 
 
 @dataclass
+class UsageRange:
+    end_date: str
+    start_date: str
+    group_by: str
+
+    @staticmethod
+    def from_dict(obj: Any) -> "UsageRange":
+        _end_date = str(obj.get("end_date"))
+        _start_date = str(obj.get("start_date"))
+        _group_by = str(obj.get("group_by"))
+        return UsageRange(_end_date, _start_date, _group_by)
+
+
+@dataclass
 class Usage:
     adjustment_charges_incl_gst: str
     bill_consumption: str
     consumption: str
     consumption_adjustment: str
     fixed_charges_excl_gst: str
     fixed_charges_incl_gst: str
     intervals: List[dict]
     percent_consumption_adjustment: str
-    range: Range
+    range: UsageRange
     status: str
     total_charges_incl_gst: str
     type: str
     variable_charges_excl_gst: str
     variable_charges_incl_gst: str
 
     @staticmethod
@@ -487,15 +502,15 @@
         _intervals = [
             {y: [Usage.from_dict(usage.get("intervals").get(y))]}
             for y in usage.get("usage").keys()
         ]
         _percent_consumption_adjustment = str(
             usage.get("percent_consumption_adjustment")
         )
-        _range = Range.from_dict(usage.get("range"))
+        _range = UsageRange.from_dict(usage.get("range"))
         _status = str(usage.get("status"))
         _total_charges_incl_gst = str(usage.get("total_charges_incl_gst"))
         _type = str(usage.get("type"))
         _variable_charges_excl_gst = str(usage.get("variable_charges_excl_gst"))
         _variable_charges_incl_gst = str(usage.get("variable_charges_incl_gst"))
         return Usage(
             _adjustment_charges_incl_gst,
@@ -512,39 +527,25 @@
             _type,
             _variable_charges_excl_gst,
             _variable_charges_incl_gst,
         )
 
 
 @dataclass
-class Range:
-    end_date: str
-    start_date: str
-    group_by: str
-
-    @staticmethod
-    def from_dict(obj: Any) -> "Range":
-        _end_date = str(obj.get("end_date"))
-        _start_date = str(obj.get("start_date"))
-        _group_by = str(obj.get("group_by"))
-        return Range(_end_date, _start_date, _group_by)
-
-
-@dataclass
 class ConsumptionAverage:
     group_breakdown: List[str]
-    range: Range
+    range: ConsumptionRange
     type: str
     usage: List[dict]
 
     @staticmethod
     def from_dict(consumption_average_data: dict) -> "ConsumptionAverage":
         consumption_average = consumption_average_data.get("data")
         _group_breakdown = consumption_average.get("group_breakdown")
-        _range = Range.from_dict(consumption_average.get("range"))
+        _range = ConsumptionRange.from_dict(consumption_average.get("range"))
         _type = str(consumption_average.get("type"))
         _usage = [
             {y: [Usage.from_dict(consumption_average.get("usage").get(y))]}
             for y in consumption_average.get("usage").keys()
         ]
         return ConsumptionAverage(_group_breakdown, _range, _type, _usage)
```

### Comparing `electrickiwi-api-0.8.4/src/electrickiwi_api.egg-info/PKG-INFO` & `electrickiwi-api-0.8.5/src/electrickiwi_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: electrickiwi-api
-Version: 0.8.4
+Version: 0.8.5
 Author-email: Michael Arthur <michael@jumblesoft.co.nz>
 License: GNU-3.0
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Electric Kiwi Python API
 
-[![SemVer 0.8.4][img_version]][url_version]
+[![SemVer 0.8.5][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
 
-[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.4&color=blue
+[img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.8.5&color=blue
 [url_version]: https://pypi.org/project/electrickiwi-api/
 
 [img_pypi]: https://img.shields.io/badge/PyPI-wheels-green.svg
 [url_pypi]: https://pypi.org/project/electrickiwi-api/#files
 
 [img_pyversions]: https://img.shields.io/pypi/pyversions/electrickiwi-api.svg
 [url_pyversions]: https://pypi.python.org/pypi/electrickiwi-api
```

### Comparing `electrickiwi-api-0.8.4/tests/test_instance.py` & `electrickiwi-api-0.8.5/tests/test_instance.py`

 * *Files identical despite different names*


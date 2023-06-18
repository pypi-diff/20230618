# Comparing `tmp/ifctester-0.0.230523.tar.gz` & `tmp/ifctester-0.0.230618.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifctester-0.0.230523.tar", last modified: Tue May 23 06:29:46 2023, max compression
+gzip compressed data, was "ifctester-0.0.230618.tar", last modified: Sun Jun 18 01:55:22 2023, max compression
```

## Comparing `ifctester-0.0.230523.tar` & `ifctester-0.0.230618.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:29:46.733398 ifctester-0.0.230523/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-23 06:29:46.733398 ifctester-0.0.230523/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-23 06:29:35.000000 ifctester-0.0.230523/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:29:46.729398 ifctester-0.0.230523/ifctester/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-23 06:29:35.000000 ifctester-0.0.230523/ifctester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-23 06:29:35.000000 ifctester-0.0.230523/ifctester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40890 2023-05-23 06:29:35.000000 ifctester-0.0.230523/ifctester/facet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-05-23 06:29:35.000000 ifctester-0.0.230523/ifctester/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-05-23 06:29:35.000000 ifctester-0.0.230523/ifctester/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:29:46.733398 ifctester-0.0.230523/ifctester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-23 06:29:46.000000 ifctester-0.0.230523/ifctester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-23 06:29:46.000000 ifctester-0.0.230523/ifctester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:29:46.000000 ifctester-0.0.230523/ifctester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 06:29:46.000000 ifctester-0.0.230523/ifctester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 06:29:46.000000 ifctester-0.0.230523/ifctester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-23 06:29:37.000000 ifctester-0.0.230523/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:29:46.733398 ifctester-0.0.230523/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:29:46.733398 ifctester-0.0.230523/test/
--rw-r--r--   0 runner    (1001) docker     (123)    88513 2023-05-23 06:29:35.000000 ifctester-0.0.230523/test/test_facet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-23 06:29:35.000000 ifctester-0.0.230523/test/test_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:55:22.835736 ifctester-0.0.230618/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-18 01:55:22.835736 ifctester-0.0.230618/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-18 01:55:13.000000 ifctester-0.0.230618/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:55:22.835736 ifctester-0.0.230618/ifctester/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40966 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-06-18 01:55:13.000000 ifctester-0.0.230618/ifctester/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:55:22.835736 ifctester-0.0.230618/ifctester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 01:55:22.000000 ifctester-0.0.230618/ifctester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-18 01:55:15.000000 ifctester-0.0.230618/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:55:22.835736 ifctester-0.0.230618/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:55:22.835736 ifctester-0.0.230618/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    88513 2023-06-18 01:55:13.000000 ifctester-0.0.230618/test/test_facet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-18 01:55:13.000000 ifctester-0.0.230618/test/test_ids.py
```

### Comparing `ifctester-0.0.230523/PKG-INFO` & `ifctester-0.0.230618/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.230523
+Version: 0.0.230618
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -29,15 +29,17 @@
 my_spec.applicability.append(ids.Entity(name="IFCWALL"))
 property = ids.Property(
     name="IsExternal", 
     value="TRUE", 
     propertySet="Pset_WallCommon", 
     measure="IfcBoolean",
     uri="https://identifier.buildingsmart.org/uri/.../prop/LoadBearing", 
-    instructions="Walls need to be load bearing.")
+    instructions="Walls need to be load bearing.",
+    minOccurs=1,
+    maxOccurs="unbounded")
 my_spec.requirements.append(property)
 my_ids.specifications.append(my_spec)
 
 # Save such IDS to file
 result = my_ids.to_xml("SampleIDS.xml")
 
 # open  IFC file:
```

### Comparing `ifctester-0.0.230523/README.md` & `ifctester-0.0.230618/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 my_spec.applicability.append(ids.Entity(name="IFCWALL"))
 property = ids.Property(
     name="IsExternal", 
     value="TRUE", 
     propertySet="Pset_WallCommon", 
     measure="IfcBoolean",
     uri="https://identifier.buildingsmart.org/uri/.../prop/LoadBearing", 
-    instructions="Walls need to be load bearing.")
+    instructions="Walls need to be load bearing.",
+    minOccurs=1,
+    maxOccurs="unbounded")
 my_spec.requirements.append(property)
 my_ids.specifications.append(my_spec)
 
 # Save such IDS to file
 result = my_ids.to_xml("SampleIDS.xml")
 
 # open  IFC file:
```

### Comparing `ifctester-0.0.230523/ifctester/__init__.py` & `ifctester-0.0.230618/ifctester/__init__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230523/ifctester/__main__.py` & `ifctester-0.0.230618/ifctester/__main__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230523/ifctester/facet.py` & `ifctester-0.0.230618/ifctester/facet.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         for name in self.parameters:
             value = getattr(self, name.replace("@", ""))
             if value is not None:
                 results[name] = value if "@" in name else self.to_ids_value(value)
         return results
 
     def parse(self, xml):
+        setattr(self, "minOccurs", 1)
+        setattr(self, "maxOccurs", 1)
         for name, value in xml.items():
             name = name.replace("@", "")
             if isinstance(value, dict) and "simpleValue" in value.keys():
                 setattr(self, name, value["simpleValue"])
             elif isinstance(value, dict) and "restriction" in value.keys():
                 setattr(self, name, Restriction().parse(value["restriction"][0]))
                 # TODO handle more than one restriction: return [restriction(r) for r in v["restriction"]]
@@ -889,15 +891,15 @@
 
 class ClassificationResult(Result):
     def to_string(self):
         if self.reason["type"] == "NOVALUE":
             return "The entity has no classification"
         elif self.reason["type"] == "VALUE":
             return f"The references \"{str(self.reason['actual'])}\" do not match the requirements"
-        elif self.reason["type"] == "system":
+        elif self.reason["type"] == "SYSTEM":
             return f"The systems \"{str(self.reason['actual'])}\" do not match the requirements"
         elif self.reason["type"] == "PROHIBITED":
             return f"The classification should not have met the requirement"
 
 
 class PartOfResult(Result):
     def to_string(self):
```

### Comparing `ifctester-0.0.230523/ifctester/ids.py` & `ifctester-0.0.230618/ifctester/ids.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230523/ifctester/reporter.py` & `ifctester-0.0.230618/ifctester/reporter.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230523/ifctester.egg-info/PKG-INFO` & `ifctester-0.0.230618/ifctester.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.230523
+Version: 0.0.230618
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Bug Tracker, https://github.com/ifcopenshell/ifcopenshell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -29,15 +29,17 @@
 my_spec.applicability.append(ids.Entity(name="IFCWALL"))
 property = ids.Property(
     name="IsExternal", 
     value="TRUE", 
     propertySet="Pset_WallCommon", 
     measure="IfcBoolean",
     uri="https://identifier.buildingsmart.org/uri/.../prop/LoadBearing", 
-    instructions="Walls need to be load bearing.")
+    instructions="Walls need to be load bearing.",
+    minOccurs=1,
+    maxOccurs="unbounded")
 my_spec.requirements.append(property)
 my_ids.specifications.append(my_spec)
 
 # Save such IDS to file
 result = my_ids.to_xml("SampleIDS.xml")
 
 # open  IFC file:
```

### Comparing `ifctester-0.0.230523/pyproject.toml` & `ifctester-0.0.230618/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ifctester"
-version = "0.0.230523"
+version = "0.0.230618"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC model auditing tool with support for IDS"
 readme = "README.md"
 keywords = ["IFC", "IDS", "BIM"]
 classifiers = [
```

### Comparing `ifctester-0.0.230523/test/test_facet.py` & `ifctester-0.0.230618/test/test_facet.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.230523/test/test_ids.py` & `ifctester-0.0.230618/test/test_ids.py`

 * *Files identical despite different names*


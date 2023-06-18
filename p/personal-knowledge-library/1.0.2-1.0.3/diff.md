# Comparing `tmp/personal_knowledge_library-1.0.2.tar.gz` & `tmp/personal_knowledge_library-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-1.0.2.tar", last modified: Fri Jun 16 10:48:54 2023, max compression
+gzip compressed data, was "personal_knowledge_library-1.0.3.tar", last modified: Sun Jun 18 18:20:38 2023, max compression
```

## Comparing `personal_knowledge_library-1.0.2.tar` & `personal_knowledge_library-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43992 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43122 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    79642 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/base/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/knowledge/ontomapping/
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/ontomapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/ontomapping/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/public/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/public/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/public/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    51852 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/utils/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 10:48:54.377348 personal_knowledge_library-1.0.2/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43992 2023-06-16 10:48:54.000000 personal_knowledge_library-1.0.2/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 10:48:54.000000 personal_knowledge_library-1.0.2/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 10:48:54.000000 personal_knowledge_library-1.0.2/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-16 10:48:54.000000 personal_knowledge_library-1.0.2/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 10:48:54.000000 personal_knowledge_library-1.0.2/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 10:48:54.381348 personal_knowledge_library-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-16 10:48:41.000000 personal_knowledge_library-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79715 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/base/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/ontomapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/ontomapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/ontomapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52672 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/utils/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-18 18:20:38.988197 personal_knowledge_library-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/setup.py
```

### Comparing `personal_knowledge_library-1.0.2/LICENSE` & `personal_knowledge_library-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/PKG-INFO` & `personal_knowledge_library-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_knowledge_library
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
@@ -830,15 +830,16 @@
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 
 ### Export entities script
 
 Dump all entities of a user to a ndjson file. 
 
 ```bash
->> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
+>> python export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP]
+                              [-c CONCEPT_TYPE] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
                         knowledge.wacom.com)
 - _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge
```

### Comparing `personal_knowledge_library-1.0.2/README.md` & `personal_knowledge_library-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -808,15 +808,16 @@
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 
 ### Export entities script
 
 Dump all entities of a user to a ndjson file. 
 
 ```bash
->> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
+>> python export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP]
+                              [-c CONCEPT_TYPE] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
                         knowledge.wacom.com)
 - _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge
```

### Comparing `personal_knowledge_library-1.0.2/knowledge/__init__.py` & `personal_knowledge_library-1.0.3/knowledge/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __author__ = "Markus Weber"
 __copyright__ = "Copyright 2021-2023 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 # Create the Logger
 logger: Union[logging.Logger, None] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
```

### Comparing `personal_knowledge_library-1.0.2/knowledge/base/__init__.py` & `personal_knowledge_library-1.0.3/knowledge/base/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/base/access.py` & `personal_knowledge_library-1.0.3/knowledge/base/access.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/base/entity.py` & `personal_knowledge_library-1.0.3/knowledge/base/entity.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/base/ontology.py` & `personal_knowledge_library-1.0.3/knowledge/base/ontology.py`

 * *Files 0% similar despite different names*

```diff
@@ -2146,14 +2146,16 @@
         if OBJECT_PROPERTIES_TAG in state:
             for object_property in state[OBJECT_PROPERTIES_TAG].values():
                 _, obj = ObjectProperty.create_from_dict(object_property)
                 self.add_relation(obj)
         # Finally, retrieve rights
         if TENANT_RIGHTS_TAG in state:
             self.tenant_access_right = TenantAccessRight.parse(state[TENANT_RIGHTS_TAG])
+        else:
+            self.tenant_access_right = TenantAccessRight()
 
     def __hash__(self):
         return 0
 
     def __eq__(self, other):
         # another object is equal to self, iff
         # it is an instance of MyClass
```

### Comparing `personal_knowledge_library-1.0.2/knowledge/nel/base.py` & `personal_knowledge_library-1.0.3/knowledge/nel/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/nel/engine.py` & `personal_knowledge_library-1.0.3/knowledge/nel/engine.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/ontomapping/__init__.py` & `personal_knowledge_library-1.0.3/knowledge/ontomapping/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/ontomapping/manager.py` & `personal_knowledge_library-1.0.3/knowledge/ontomapping/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,16 @@
             return value
         elif structure_type == 'monolingualtext' and isinstance(value, dict):
             if LOCALE_LANGUAGE_MAPPING.get(locale) == value['language']:
                 return value['text']
             return None
         elif structure_type == 'globe-coordinate' and isinstance(value, dict):
             return f'{value["latitude"]},{value["longitude"]}'
+        elif structure_type == 'url' and isinstance(value, str):
+            return value
     raise NotImplementedError()
 
 
 def wikidata_to_thing(wikidata_thing: WikidataThing, all_relations: Dict[str, Any], supported_locales: List[str],
                       all_wikidata_objects: Dict[str, WikidataThing], pull_wikipedia: bool = False)\
         -> Tuple[ThingObject, List[Dict[str, Any]]]:
     """
@@ -184,23 +186,26 @@
     relation_props: Dict[OntologyPropertyReference, List[str]] = {}
     for pid, cl in wikidata_thing.claims.items():
         prop: Optional[PropertyConfiguration] = get_mapping_configuration().guess_property(pid, thing.concept_type)
         if prop and prop.type == PropertyType.DATA_PROPERTY:
             property_type: OntologyPropertyReference = OntologyPropertyReference.parse(prop.iri)
             for locale in supported_locales:
                 for c in cl.literals:
-                    if isinstance(c, dict):
-                        content: Optional[str] = convert_dict(c, locale)
-                        if get_mapping_configuration().check_data_property_range(property_type, content):
-                            thing.add_data_property(DataProperty(content=content,
-                                                                 property_ref=property_type,
+                    try:
+                        if isinstance(c, dict):
+                            content: Optional[str] = convert_dict(c, locale)
+                            if get_mapping_configuration().check_data_property_range(property_type, content):
+                                thing.add_data_property(DataProperty(content=content,
+                                                                     property_ref=property_type,
+                                                                     language_code=LanguageCode(locale)))
+                        elif isinstance(c, (str, float, int)):
+                            thing.add_data_property(DataProperty(content=c, property_ref=property_type,
                                                                  language_code=LanguageCode(locale)))
-                    elif isinstance(c, (str, float, int)):
-                        thing.add_data_property(DataProperty(content=c, property_ref=property_type,
-                                                             language_code=LanguageCode(locale)))
+                    except NotImplementedError as e:
+                        import_warnings.append({'qid': qid, 'pid': pid, 'error': str(e)})
     for relation in all_relations.get(qid, []):
         prop: Optional[PropertyConfiguration] = get_mapping_configuration().guess_property(relation['predicate']['pid'],
                                                                                            thing.concept_type)
         target_thing: Optional[WikidataThing] = all_wikidata_objects.get(relation['target']['qid'])
         if target_thing:
             if prop and prop.type == PropertyType.OBJECT_PROPERTY:
                 class_types: List[str] = [c.qid for c in target_thing.instance_of]
```

### Comparing `personal_knowledge_library-1.0.2/knowledge/public/__init__.py` & `personal_knowledge_library-1.0.3/knowledge/public/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/public/cache.py` & `personal_knowledge_library-1.0.3/knowledge/public/cache.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/public/helper.py` & `personal_knowledge_library-1.0.3/knowledge/public/helper.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/public/relations.py` & `personal_knowledge_library-1.0.3/knowledge/public/relations.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/public/wikidata.py` & `personal_knowledge_library-1.0.3/knowledge/public/wikidata.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/services/__init__.py` & `personal_knowledge_library-1.0.3/knowledge/services/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/services/base.py` & `personal_knowledge_library-1.0.3/knowledge/services/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/services/graph.py` & `personal_knowledge_library-1.0.3/knowledge/services/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -851,41 +851,53 @@
                         thing.status_flag = EntityStatus.SYNCED
                         entities.append(thing)
                 return entities, estimated_total_number, next_page_id
 
         raise WacomServiceException(f'Failed to list the entities (since:= {page_id}, limit:={limit}). '
                                     f'Response code:={response.status_code}, exception:= {response.content}')
 
-    def ontology_update(self, auth_key: str):
+    def ontology_update(self, auth_key: str, fix: bool = False, max_retries: int = 3, backoff_factor: float = 0.1):
         """
         Update the ontology.
 
         **Remark:**
         Works for users with role 'TenantAdmin'.
 
         Parameters
         ----------
         auth_key: str
             Auth key from user
+        fix: bool [default:=False]
+            Fix the ontology if tenant is in inconsistent state.
+        max_retries: int
+            Maximum number of retries
+        backoff_factor: float
+            A backoff factor to apply between attempts after the second try (most errors are resolved immediately by a.
 
         Raises
         ------
         WacomServiceException
             If the graph service returns an error code and commit failed.
         """
-        url: str = f'{self.service_base_url}{WacomKnowledgeService.ONTOLOGY_UPDATE_ENDPOINT}'
+        url: str = f'{self.service_base_url}{WacomKnowledgeService.ONTOLOGY_UPDATE_ENDPOINT}{"/fix" if fix else ""}'
         # Header with auth token
         headers: dict = {
             USER_AGENT_HEADER_FLAG: USER_AGENT_STR,
             AUTHORIZATION_HEADER_FLAG: f'Bearer {auth_key}'
         }
-        response: Response = requests.patch(url, headers=headers, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
-        if not response.ok:
-            raise WacomServiceException(f'Ontology update fails. '
-                                        f'Response code:={response.status_code}, exception:= {response.content}')
+        mount_point: str = 'https://' if self.service_url.startswith('https') else 'http://'
+        with requests.Session() as session:
+            retries: Retry = Retry(total=max_retries,
+                                   backoff_factor=backoff_factor,
+                                   status_forcelist=[502, 503, 504])
+            session.mount(mount_point, HTTPAdapter(max_retries=retries))
+            response: Response = session.patch(url, headers=headers, timeout=DEFAULT_TIMEOUT, verify=self.verify_calls)
+            if not response.ok:
+                raise WacomServiceException(f'Ontology update fails. '
+                                            f'Response code:={response.status_code}, exception:= {response.content}')
 
     def search_all(self, auth_key: str, search_term: str, language_code: LanguageCode,
                    types: List[OntologyClassReference], limit: int = 30, next_page_id: str = None) \
             -> Tuple[List[ThingObject], str]:
         """Search term in labels, literals and description.
 
         Parameters
```

### Comparing `personal_knowledge_library-1.0.2/knowledge/services/group.py` & `personal_knowledge_library-1.0.3/knowledge/services/group.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/services/ontology.py` & `personal_knowledge_library-1.0.3/knowledge/services/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/services/tenant.py` & `personal_knowledge_library-1.0.3/knowledge/services/tenant.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/services/users.py` & `personal_knowledge_library-1.0.3/knowledge/services/users.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/utils/rdf.py` & `personal_knowledge_library-1.0.3/knowledge/utils/rdf.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/knowledge/utils/wikipedia.py` & `personal_knowledge_library-1.0.3/knowledge/utils/wikipedia.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
@@ -830,15 +830,16 @@
 - _-r, --relations (optional)_ -  Requesting the relations for each entity
 
 ### Export entities script
 
 Dump all entities of a user to a ndjson file. 
 
 ```bash
->> python  export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP] [-i INSTANCE]
+>> python export_entities.py [-h] -u USER -t TENANT [-r] [-a] [-p] [-d DUMP]
+                              [-c CONCEPT_TYPE] [-i INSTANCE]
 ```
 
 **Parameters:**
 
 - _-i INSTANCE, --instance INSTANCE_ - URL of instance. (default:=https://private-
                         knowledge.wacom.com)
 - _-u USER, --user USER_ - External ID to identify user of the Wacom Private Knowledge
```

### Comparing `personal_knowledge_library-1.0.2/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.2/setup.py` & `personal_knowledge_library-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 an older version of knowledge-service-lib :
     $ python -m pip install personal-knowledge-library
 """)
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
```


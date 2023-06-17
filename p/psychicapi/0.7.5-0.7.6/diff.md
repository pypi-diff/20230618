# Comparing `tmp/psychicapi-0.7.5.tar.gz` & `tmp/psychicapi-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psychicapi-0.7.5.tar", last modified: Sat Jun 17 07:29:42 2023, max compression
+gzip compressed data, was "dist/psychicapi-0.7.6.tar", last modified: Sat Jun 17 23:04:05 2023, max compression
```

## Comparing `psychicapi-0.7.5.tar` & `psychicapi-0.7.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 07:29:42.000000 psychicapi-0.7.5/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4412 2023-06-17 07:29:42.000000 psychicapi-0.7.5/PKG-INFO
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.7.5/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     6477 2023-06-16 23:11:57.000000 psychicapi-0.7.5/psychicapi/psychic.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3399 2023-06-12 19:04:35.000000 psychicapi-0.7.5/README.md
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-16 23:25:17.000000 psychicapi-0.7.5/setup.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4412 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-17 07:29:42.000000 psychicapi-0.7.5/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-17 07:29:42.000000 psychicapi-0.7.5/setup.cfg
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 23:04:05.000000 psychicapi-0.7.6/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-17 23:04:05.000000 psychicapi-0.7.6/PKG-INFO
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.7.6/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     7272 2023-06-17 22:29:02.000000 psychicapi-0.7.6/psychicapi/psychic.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3726 2023-06-17 23:03:51.000000 psychicapi-0.7.6/README.md
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-17 23:03:36.000000 psychicapi-0.7.6/setup.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-17 23:04:05.000000 psychicapi-0.7.6/setup.cfg
```

### Comparing `psychicapi-0.7.5/PKG-INFO` & `psychicapi-0.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.5
+Version: 0.7.6
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 License: UNKNOWN
 Description: # Psychic
         
@@ -35,15 +35,25 @@
         # Get all active connections and optionally filter by connector id and/or account id
         connections = psychic.get_connections(account_id="account_id")
         ```
         
         ### Retrieve documents from a connection
         
         ```
-        docs = psychic.get_documents(account_id="account_id")
+        page_cursor = None
+        all_docs = []
+        while True:
+            docs_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor, page_size=100)
+            if docs_response is None:
+                break
+            all_docs.extend(docs_response.documents)
+            page_cursor = docs_response.next_page_cursor
+            if page_cursor is None:
+                break
+        print(all_docs)
         ```
         
         ## Advanced Filtering
         
         ### Filtering by section(s)
         
         Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
```

### Comparing `psychicapi-0.7.5/psychicapi/psychic.py` & `psychicapi-0.7.6/psychicapi/psychic.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,44 +53,66 @@
         self.connector_id = connector_id
         self.metadata = metadata
         self.section_filters = section_filters
         self.sections = sections
         self.credential = credential
         self.config = config
 
+class GetDocumentsResponse:
+    documents: List[Dict]
+    next_page_cursor: Optional[str] = None
+
+    def __init__(self, documents: List[Dict], next_page_cursor: Optional[str] = None) -> None:
+        self.documents = documents
+        self.next_page_cursor = next_page_cursor
+
 class ChunkingOptions:
     min_chunk_size: Optional[int] = None
     max_chunk_size: Optional[int] = None
 
 class Psychic:
     def __init__(self, secret_key: str):
         self.api_url = "https://api.psychic.dev/"
         self.secret_key = secret_key
 
-    def get_documents(self, *, account_id: str, connector_id: Optional[ConnectorId] = None, section_filter_id: Optional[str] = None, uris: Optional[List[str]] = None, chunked: Optional[bool] = False, min_chunk_size: Optional[int] = None, max_chunk_size: Optional[int] = None):
+    def get_documents(self, 
+                      *, 
+                      account_id: str, 
+                      connector_id: Optional[ConnectorId] = None, 
+                      section_filter_id: Optional[str] = None, 
+                      uris: Optional[List[str]] = None, 
+                      chunked: Optional[bool] = False, 
+                      min_chunk_size: Optional[int] = None, 
+                      max_chunk_size: Optional[int] = None,
+                      page_cursor: Optional[str] = None,
+                      page_size: Optional[int] = 100):
         body = {
             "account_id": account_id,
             "connector_id": connector_id.value if connector_id is not None else None,
             "section_filter_id": section_filter_id,
             "uris": uris,
             "chunked": chunked,
             "min_chunk_size": min_chunk_size,
             "max_chunk_size": max_chunk_size,
+            "page_cursor": page_cursor,
+            "page_size": page_size
         }
         response = requests.post(
             self.api_url + "get-documents",
             json=body,
             headers={
                 'Authorization': 'Bearer ' + self.secret_key,
                 'Accept': 'application/json'
             }
         )
         if response.status_code == 200:
-            documents = response.json()["documents"]
-            return documents
+            data = response.json()
+            documents = data["documents"]
+            next_page_cursor = data["next_page_cursor"]
+            return GetDocumentsResponse(documents=documents, next_page_cursor=next_page_cursor)
         else:
             return None
         
     def get_connections(self, *, connector_id: Optional[ConnectorId] = None, account_id: Optional[str] = None):
         filter = {
             "connector_id": connector_id.value if connector_id is not None else None,
             "account_id": account_id
```

### Comparing `psychicapi-0.7.5/README.md` & `psychicapi-0.7.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,25 @@
 # Get all active connections and optionally filter by connector id and/or account id
 connections = psychic.get_connections(account_id="account_id")
 ```
 
 ### Retrieve documents from a connection
 
 ```
-docs = psychic.get_documents(account_id="account_id")
+page_cursor = None
+all_docs = []
+while True:
+    docs_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor, page_size=100)
+    if docs_response is None:
+        break
+    all_docs.extend(docs_response.documents)
+    page_cursor = docs_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_docs)
 ```
 
 ## Advanced Filtering
 
 ### Filtering by section(s)
 
 Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
```

### Comparing `psychicapi-0.7.5/setup.py` & `psychicapi-0.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.7.5',
+    version='0.7.6',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

### Comparing `psychicapi-0.7.5/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.7.6/psychicapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.5
+Version: 0.7.6
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 License: UNKNOWN
 Description: # Psychic
         
@@ -35,15 +35,25 @@
         # Get all active connections and optionally filter by connector id and/or account id
         connections = psychic.get_connections(account_id="account_id")
         ```
         
         ### Retrieve documents from a connection
         
         ```
-        docs = psychic.get_documents(account_id="account_id")
+        page_cursor = None
+        all_docs = []
+        while True:
+            docs_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor, page_size=100)
+            if docs_response is None:
+                break
+            all_docs.extend(docs_response.documents)
+            page_cursor = docs_response.next_page_cursor
+            if page_cursor is None:
+                break
+        print(all_docs)
         ```
         
         ## Advanced Filtering
         
         ### Filtering by section(s)
         
         Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
```


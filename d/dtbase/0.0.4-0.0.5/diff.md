# Comparing `tmp/dtbase-0.0.4.tar.gz` & `tmp/dtbase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtbase-0.0.4.tar", max compression
+gzip compressed data, was "dtbase-0.0.5.tar", max compression
```

## Comparing `dtbase-0.0.4.tar` & `dtbase-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2023-05-26 23:58:37.938978 dtbase-0.0.4/dtbase/__init__.py
--rw-r--r--   0        0        0     5281 2023-05-26 23:45:18.887306 dtbase-0.0.4/dtbase/config.py
--rw-r--r--   0        0        0     6359 2023-05-30 02:16:18.130747 dtbase-0.0.4/dtbase/engine.py
--rw-r--r--   0        0        0      352 2023-05-30 02:20:57.830457 dtbase-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      609 2023-05-30 02:21:13.006971 dtbase-0.0.4/setup.py
--rw-r--r--   0        0        0      374 2023-05-30 02:21:13.007151 dtbase-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-05-26 23:58:37.938978 dtbase-0.0.5/dtbase/__init__.py
+-rw-r--r--   0        0        0     5281 2023-05-26 23:45:18.887306 dtbase-0.0.5/dtbase/config.py
+-rw-r--r--   0        0        0     6616 2023-06-18 01:48:38.160256 dtbase-0.0.5/dtbase/engine.py
+-rw-r--r--   0        0        0      352 2023-06-18 01:42:57.463395 dtbase-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      609 2023-06-18 01:48:41.729501 dtbase-0.0.5/setup.py
+-rw-r--r--   0        0        0      374 2023-06-18 01:48:41.729701 dtbase-0.0.5/PKG-INFO
```

### Comparing `dtbase-0.0.4/dtbase/config.py` & `dtbase-0.0.5/dtbase/config.py`

 * *Files identical despite different names*

### Comparing `dtbase-0.0.4/dtbase/engine.py` & `dtbase-0.0.5/dtbase/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -177,14 +177,21 @@
 	async def get(self, key: str) -> Optional[dict]:
 		base = self.async_base()
 		try:
 			return await base.get(key)
 		finally:
 			await base.close()
 			
+	async def keys(self, query: DetaQuery = None) -> list[str]:
+		return [i['key'] for i in await self.fetch_all(query)]
+	
+	async def tabledata(self, query: DetaQuery = None) -> dict[str, dict]:
+		return {i['key']: i for i in await self.fetch_all(query)}
+
+			
 	async def get_first(self, query: DetaQuery = None) -> Optional[dict]:
 		result = await self.fetch(limit=1, query=query)
 		data = None
 		try:
 			data = result.items[0]
 		finally:
 			return data
```

### Comparing `dtbase-0.0.4/setup.py` & `dtbase-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['dtbase']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['deta[async]==1.1.0a2', 'starlette>=0.27.0,<0.28.0']
+['deta[async]==1.1.0a2', 'starlette>=0.28.0,<0.29.0']
 
 setup_kwargs = {
     'name': 'dtbase',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```


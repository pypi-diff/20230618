# Comparing `tmp/dtfield-0.2.2.tar.gz` & `tmp/dtfield-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.2.2.tar", max compression
+gzip compressed data, was "dtfield-0.2.3.tar", max compression
```

## Comparing `dtfield-0.2.2.tar` & `dtfield-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.2.2/dtfield/__init__.py
--rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.2.2/dtfield/_imports.py
--rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.2.2/dtfield/base_enum.py
--rw-r--r--   0        0        0    23631 2023-06-17 00:02:42.064522 dtfield-0.2.2/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.2.2/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.2.2/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.2.2/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.2.2/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.2.2/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.2.2/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.2.2/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.2.2/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.2.2/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.2.2/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.2.2/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.2.2/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.2.2/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.2.2/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.2.2/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.2.2/dtfield/parse/string.py
--rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.2.2/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      457 2023-06-17 00:25:40.076770 dtfield-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      806 2023-06-17 00:25:44.005888 dtfield-0.2.2/setup.py
--rw-r--r--   0        0        0      636 2023-06-17 00:25:44.006130 dtfield-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.2.3/dtfield/__init__.py
+-rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.2.3/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.2.3/dtfield/base_enum.py
+-rw-r--r--   0        0        0    25546 2023-06-17 23:30:27.745672 dtfield-0.2.3/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.2.3/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.2.3/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.2.3/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.2.3/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.2.3/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.2.3/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.2.3/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.2.3/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.2.3/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.2.3/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.2.3/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.2.3/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.2.3/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.2.3/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.2.3/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.2.3/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.2.3/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      457 2023-06-17 23:30:27.747997 dtfield-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      806 2023-06-17 23:30:32.733698 dtfield-0.2.3/setup.py
+-rw-r--r--   0        0        0      636 2023-06-17 23:30:32.734095 dtfield-0.2.3/PKG-INFO
```

### Comparing `dtfield-0.2.2/dtfield/_imports.py` & `dtfield-0.2.3/dtfield/_imports.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/base_enum.py` & `dtfield-0.2.3/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/engine.py` & `dtfield-0.2.3/dtfield/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,32 +223,37 @@
     TABLE: ClassVar[Optional[str]] = None
     ITEM_NAME: ClassVar[Optional[str]] = None
     DISPLAY_PROPERTIES: ClassVar[Optional[list[str]]] = None
     SINGULAR: ClassVar[Optional[str]] = None
     PLURAL: ClassVar[Optional[str]] = None
     EXIST_PARAMS: ClassVar[DetaQuery] = None
     DELETABLE: ClassVar[bool] = True
+    TABLEDATA: ClassVar[dict[str, dict]] = None
     
     async def delete(self):
         if self.DELETABLE:
             return await DetaBase(self.table()).delete(getattr(self, 'key'))
         print(f'{self.clsname()}.FROZEN is True and cannot be deleted')
         return
     
     @classmethod
     def exist_params(cls):
         return cls.EXIST_PARAMS
     
+    @classmethod
+    async def update_tabledata(cls, query: DetaQuery = None):
+        cls.TABLEDATA = {key(i): i for i in await cls.fetch_all(query or cls.DETA_QUERY)}
+    
     async def exist_response(self):
         return await DetaBase(self.table()).fetch(exist_query(self))
     
     async def save(self):
         new = await DetaBase(self.table()).insert(self.asjson_to_db())
         if new:
-            await self.update_context()
+            await self.update_tabledata()
             return self.safe_create(**new)
         return None
     
     async def save_new(self):
         exist = await self.exist_response()
         if exist.count == 0:
             return await self.save()
@@ -258,15 +263,15 @@
             return None
         
     async def update_instance(self, **kwargs):
         current = self.asjson()
         current.update(exclude_keys_from_dict(kwargs, exclude=['key']))
         key = current.pop('key')
         await DetaBase(self.table()).put(data=current, key=key)
-        await self.update_context()
+        await self.update_tabledata()
         return self.from_context(key)
         
     
     @classmethod
     def singular(cls):
         return cls.SINGULAR or cls.clsname()
     
@@ -287,82 +292,116 @@
         return cls.TABLE or cls.clsname()
     
     @classmethod
     def dependant_descriptors(cls):
         return {d.public_name: d for d in cls.descriptorsmap().values() if d.has_dependants is True}
     
     @classmethod
-    def model_dependants(cls, collection: list = None):
+    def model_dependants(cls, collection: list = None) -> list[type[ContextBase]]:
         return model_dependants(cls, collection or list())
 
     @classmethod
     def from_context(cls, key: str = None) -> Self:
         if key is None:
             return None
         data = cls.get_context().get(key, None)
         if data:
             return cls.safe_create(**data)
         return None
     
+    # @classmethod
+    # def from_tabledata(cls, key: str = None) -> Self:
+    #     if key is None:
+    #         return None
+    #     data = cls.TABLEDATA.get(key, None)
+    #     if data:
+    #         return cls.safe_create(**data)
+    #     return None
+    
     @classmethod
-    async def set_context(cls):
-        context.run(cls.CTXVAR.set, make_dict(await cls.fetch_all()))
-        
+    async def set_context(cls, data: Optional[dict[str, dict]] = None):
+        if not data:
+            context.run(cls.CTXVAR.set, make_dict(await cls.fetch_all()))
+        else:
+            context.run(cls.CTXVAR.set, data)
+
+    
     @classmethod
     def get_context(cls):
-        return context.get(cls.CTXVAR)
+        return cls.TABLEDATA or context.get(cls.CTXVAR)
 
     @classmethod
     async def fetch_all(cls, query: DetaQuery = None) -> list[dict[str, Jsonable]]:
         return await DetaBase(cls.table()).fetch_all(query or cls.DETA_QUERY)
     
     @classmethod
     async def fetch(cls, query: DetaQuery = None, last: Optional[str] = None, limit: int = 1000) -> FetchResponse:
         return await DetaBase(cls.table()).fetch(query or cls.DETA_QUERY, last, limit)
     
     @classmethod
     async def update_context(cls):
         async with create_task_group() as tks:
             for item in cls.model_dependants():
-                tks.start_soon(item.set_context)
+                tks.start_soon(item.set_context, item.TABLEDATA)
                 
     def __lt__(self, other):
         return normalize_lower(str(self)) < normalize_lower(str(other))
     
     @classmethod
-    async def instances_list(cls) -> list[Self]:
+    async def instances_list(cls, query: Optional[dict[str, Any]] = None) -> list[Self]:
         await cls.update_context()
-        return [cls.from_context(i) for i in cls.get_context().keys()]
+        instances = [cls.from_context(i) for i in cls.get_context().keys()]
+        if query:
+            print(query)
+            return [i for i in instances if all([*[getter(i, k) == v for k, v in query.items() if v]])]
+        return instances
+    
+    @classmethod
+    async def instances_list_contains(cls, query: Optional[dict[str, str]] = None) -> list[Self]:
+        await cls.update_context()
+        instances = [cls.from_context(i) for i in cls.get_context().keys()]
+        if query:
+            print(query)
+            return [i for i in instances if all([*[normalize_lower(str(getter(i, k))).__contains__(normalize_lower(str(v))) for k, v in query.items() if v]])]
+        return instances
+    
+    @classmethod
+    async def sorted_instances_list(cls, query: dict[str, Any] = None) -> list[Self]:
+        return sorted(await cls.instances_list(query=query))
+    
+    @classmethod
+    async def sorted_instances_list_contains(cls, query: dict[str, str] = None) -> list[Self]:
+        return sorted(await cls.instances_list_contains(query=query))
     
     @classmethod
-    async def sorted_instances_list(cls) -> list[Self]:
-        return sorted(await cls.instances_list())
+    async def ordered_instances_list(cls, query: dict[str, Any] = None) -> list[Self]:
+        return ordered(await cls.instances_list(query=query))
     
     @classmethod
-    async def ordered_instances_list(cls) -> list[Self]:
-        return ordered(await cls.instances_list())
+    async def ordered_instances_lis_containst(cls, query: dict[str, Any] = None) -> list[Self]:
+        return ordered(await cls.instances_list_contains(query=query))
     
     @classmethod
     async def html_list(cls, request: Request):
         return TEMPLATES.TemplateResponse(
                 '/partial/instances_list.jj',
                 {
                         'request': request,
-                        'instances': await cls.sorted_instances_list(),
+                        'instances': await cls.sorted_instances_list({'patient_key': request.path_params.get('patient_key')}),
                         'model': cls
                 }
         )
     
     @classmethod
     async def html_datalist(cls, request: Request):
         return TEMPLATES.TemplateResponse(
                 '/partial/datalist.jj',
                 {
                         'request': request,
-                        'instances': await cls.sorted_instances_list(),
+                        'instances': await cls.sorted_instances_list({'patient_key': request.path_params.get('patient_key')}),
                         'model': cls
                 }
         )
         
     
 
 def model_dependants(obj: type[ContextBase], collection: list = None):
```

### Comparing `dtfield-0.2.2/dtfield/functions.py` & `dtfield-0.2.3/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.2.3/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.2.3/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.2.3/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.2.3/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.2.3/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.2.3/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/dates.py` & `dtfield-0.2.3/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/json_encoder.py` & `dtfield-0.2.3/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/number.py` & `dtfield-0.2.3/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/string.py` & `dtfield-0.2.3/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/dtfield/parse/type_hint.py` & `dtfield-0.2.3/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.2/setup.py` & `dtfield-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'itsdangerous>=2.1.2,<3.0.0',
  'python-multipart>=0.0.6,<0.0.7',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dtfield-0.2.2/PKG-INFO` & `dtfield-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfield
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```


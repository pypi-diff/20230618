# Comparing `tmp/django_ninja_crud-0.1.1.tar.gz` & `tmp/django_ninja_crud-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_crud-0.1.1.tar", max compression
+gzip compressed data, was "django_ninja_crud-0.1.2.tar", max compression
```

## Comparing `django_ninja_crud-0.1.1.tar` & `django_ninja_crud-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1069 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/LICENSE
--rw-r--r--   0        0        0     4083 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/ninja_crud/__init__.py
--rw-r--r--   0        0        0      151 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/ninja_crud/apps.py
--rw-r--r--   0        0        0      574 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/ninja_crud/tests/__init__.py
--rw-r--r--   0        0        0     5225 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_abstract.py
--rw-r--r--   0        0        0     4637 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_create.py
--rw-r--r--   0        0        0     2593 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_delete.py
--rw-r--r--   0        0        0     3300 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_list.py
--rw-r--r--   0        0        0     3064 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_retrieve.py
--rw-r--r--   0        0        0     4515 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_update.py
--rw-r--r--   0        0        0      303 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/utils.py
--rw-r--r--   0        0        0      397 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/utils.py
--rw-r--r--   0        0        0      409 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/__init__.py
--rw-r--r--   0        0        0      796 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/abstract.py
--rw-r--r--   0        0        0     3876 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/create.py
--rw-r--r--   0        0        0     1551 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/delete.py
--rw-r--r--   0        0        0     3975 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/list.py
--rw-r--r--   0        0        0     1548 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/retrieve.py
--rw-r--r--   0        0        0     1959 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/update.py
--rw-r--r--   0        0        0     1611 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5739 1970-01-01 00:00:00.000000 django_ninja_crud-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4163 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/apps.py
+-rw-r--r--   0        0        0      239 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/schemas.py
+-rw-r--r--   0        0        0      574 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/__init__.py
+-rw-r--r--   0        0        0     5334 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_abstract.py
+-rw-r--r--   0        0        0     4548 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_create.py
+-rw-r--r--   0        0        0     2535 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_delete.py
+-rw-r--r--   0        0        0     4240 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_list.py
+-rw-r--r--   0        0        0     3006 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_retrieve.py
+-rw-r--r--   0        0        0     4446 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_update.py
+-rw-r--r--   0        0        0      303 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/utils.py
+-rw-r--r--   0        0        0      397 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/utils.py
+-rw-r--r--   0        0        0      409 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/abstract.py
+-rw-r--r--   0        0        0     3836 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/create.py
+-rw-r--r--   0        0        0     1551 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/delete.py
+-rw-r--r--   0        0        0     3947 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/list.py
+-rw-r--r--   0        0        0     1548 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/retrieve.py
+-rw-r--r--   0        0        0     1959 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/update.py
+-rw-r--r--   0        0        0     1611 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 django_ninja_crud-0.1.2/PKG-INFO
```

### Comparing `django_ninja_crud-0.1.1/LICENSE` & `django_ninja_crud-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.1/README.md` & `django_ninja_crud-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,45 +39,53 @@
 
 class DepartmentOut(Schema):
     id: int
     title: str
 ```
 
 Here is a brief example of how to use django-ninja-crud:
+
 ```python
 # views.py
-from examples.models import Department
-from examples.schemas import DepartmentIn, DepartmentOut
-from ninja_crud.views import ModelViewSet, ListModelView, CreateModelView, \
+from example.models import Department
+from example.schemas import DepartmentIn, DepartmentOut
+from ninja import Router
+from ninja_crud.views import ModelViewSet, ListModelView, CreateModelView,
     RetrieveModelView, UpdateModelView, DeleteModelView
 
 
 class DepartmentViewSet(ModelViewSet):
     model = Department
     input_schema = DepartmentIn
     output_schema = DepartmentOut
 
     list = ListModelView(output_schema=output_schema)
     create = CreateModelView(input_schema=input_schema, output_schema=output_schema)
     retrieve = RetrieveModelView(output_schema=output_schema)
     update = UpdateModelView(input_schema=input_schema, output_schema=output_schema)
     delete = DeleteModelView()
+
+
+router = Router()
+DepartmentViewSet.register_routes(router)
 ```
 
 ## Testing
 You can then write the associated tests like so:
+
 ```python
 # tests.py
 from django.test import TestCase
-from examples.models import Department
-from examples.views.view_department import DepartmentViewSet
-from ninja_crud.tests import CreateModelViewTest, DeleteModelViewTest, \
-    ListModelViewTest, ModelViewSetTest, Payloads, RetrieveModelViewTest, \
+from example.models import Department
+from example.views.view_department import DepartmentViewSet
+from ninja_crud.tests import CreateModelViewTest, DeleteModelViewTest,
+    ListModelViewTest, ModelViewSetTest, Payloads, RetrieveModelViewTest,
     UpdateModelViewTest
 
+
 class DepartmentViewSetTest(ModelViewSetTest, TestCase):
     model_view_set = DepartmentViewSet
 
     @classmethod
     def setUpTestData(cls):
         super().setUpTestData()
         cls.department_1 = Department.objects.create(title="department-1")
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/tests/__init__.py` & `django_ninja_crud-0.1.2/ninja_crud/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.1/ninja_crud/tests/test_abstract.py` & `django_ninja_crud-0.1.2/ninja_crud/tests/test_abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,33 @@
 
 class Payloads(NamedTuple):
     ok: dict
     bad_request: Optional[dict] = None
     conflict: Optional[dict] = None
 
 
+def default_credentials_getter(_: TestCase) -> Credentials:
+    return Credentials(ok={})
+
+
 class AbstractModelViewTest:
     model_view_set: ModelViewSet
     test_case: TestCase
     client: Client
     model_view: Type[AbstractModelView]
     name: str
 
     def __init__(
         self,
         instance_getter: Callable[[TestCase], Model],
-        credentials_getter: Callable[[TestCase], Credentials],
+        credentials_getter: Callable[[TestCase], Credentials] = None,
     ) -> None:
         self.get_instance = instance_getter
+        if credentials_getter is None:
+            credentials_getter = default_credentials_getter
         self.get_credentials = credentials_getter
 
     def get_tests(self) -> List[Tuple[str, Callable]]:
         return [
             (name, method)
             for name, method in inspect.getmembers(self, predicate=inspect.ismethod)
             if name.startswith("test")
@@ -99,18 +105,15 @@
         self.test_case.assertIsInstance(count, int)
         self.test_case.assertEqual(count, queryset.count())
 
         self.test_case.assertIn("items", content)
         items = content["items"]
         self.test_case.assertIsInstance(items, list)
 
-        if limit >= 0:
-            queryset_items = queryset[offset : offset + limit]
-        else:
-            queryset_items = queryset
+        queryset_items = queryset[offset : offset + limit]
         self.test_case.assertEqual(len(items), queryset_items.count())
 
         for item in items:
             self.assert_content_equals_schema(item, queryset, output_schema)
 
     def assert_response_is_bad_request(
         self, response: HttpResponse, status_code: HTTPStatus
@@ -136,15 +139,15 @@
                 attr_value.client = new_cls.client_class()
                 attr_value.name = attr_name
                 for test_name, test_func in attr_value.get_tests():
                     method = attr_value.get_model_view()
                     model_name = new_cls.model_view_set.model.__name__.lower()
                     substring_replace = model_name
                     if isinstance(method, (ListModelView, CreateModelView)):
-                        if method.is_instance_view:
+                        if method.detail:
                             related_model_name = method.related_model.__name__.lower()
                             substring_replace = f"{model_name}_{related_model_name}"
                     new_test_name = test_name.replace("model", substring_replace)
                     setattr(new_cls, new_test_name, test_func)
         return new_cls
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/tests/test_create.py` & `django_ninja_crud-0.1.2/ninja_crud/tests/test_create.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from http import HTTPStatus
-from typing import Callable, Optional
+from typing import Callable
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.test import TestCase
 from django.urls import reverse
 
@@ -16,30 +16,25 @@
 class CreateModelViewTest(AbstractModelViewTest):
     model_view = CreateModelView
 
     def __init__(
         self,
         payloads: Payloads,
         instance_getter: Callable[[TestCase], Model],
-        credentials_getter: Callable[[TestCase], Credentials],
+        credentials_getter: Callable[[TestCase], Credentials] = None,
     ) -> None:
         super().__init__(
             instance_getter=instance_getter, credentials_getter=credentials_getter
         )
         self.payloads = payloads
 
-    def create_model(
-        self, id: UUID, data: dict, credentials: Optional[dict]
-    ) -> HttpResponse:
-        if credentials is None:
-            credentials = {}
-
+    def create_model(self, id: UUID, data: dict, credentials: dict) -> HttpResponse:
         model_view: CreateModelView = self.get_model_view()
         model_name = utils.to_snake_case(self.model_view_set.model.__name__)
-        if model_view.is_instance_view:
+        if model_view.detail:
             related_model_name = utils.to_snake_case(model_view.related_model.__name__)
             url_name = f"{model_name}_{related_model_name}s"
             kwargs = {"id": id}
         else:
             url_name = f"{model_name}s"
             kwargs = {}
 
@@ -51,15 +46,15 @@
         )
 
     def assert_response_is_ok(self, response: HttpResponse):
         self.test_case.assertEqual(response.status_code, HTTPStatus.CREATED)
         content = json.loads(response.content)
 
         model_view: CreateModelView = self.get_model_view()
-        if model_view.is_instance_view:
+        if model_view.detail:
             model = model_view.related_model
         else:
             model = self.model_view_set.model
         self.assert_content_equals_schema(
             content,
             queryset=model.objects.get_queryset(),
             output_schema=model_view.output_schema,
@@ -97,15 +92,15 @@
 
     def test_create_model_unauthorized(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.unauthorized is None:
             self.test_case.skipTest("No unauthorized credentials provided")
         instance: Model = self.get_instance(self.test_case)
         response = self.create_model(
-            id=instance.pk, data=self.payloads.ok, credentials=None
+            id=instance.pk, data=self.payloads.ok, credentials=credentials.unauthorized
         )
         self.assert_response_is_bad_request(
             response, status_code=HTTPStatus.UNAUTHORIZED
         )
 
     def test_create_model_forbidden(self):
         credentials: Credentials = self.get_credentials(self.test_case)
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/tests/test_delete.py` & `django_ninja_crud-0.1.2/ninja_crud/tests/test_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import uuid
 from http import HTTPStatus
-from typing import Optional
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.urls import reverse
 
 from ninja_crud import utils
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
 from ninja_crud.views.delete import DeleteModelView
 
 
 class DeleteModelViewTest(AbstractModelViewTest):
     model_view = DeleteModelView
 
-    def delete_model(self, id: UUID, credentials: Optional[dict]) -> HttpResponse:
-        if credentials is None:
-            credentials = {}
-
+    def delete_model(self, id: UUID, credentials: dict) -> HttpResponse:
         kwargs = {"id": id}
         url_name = utils.to_snake_case(self.model_view_set.model.__name__)
         return self.client.delete(
             reverse(f"api:{url_name}", kwargs=kwargs),
             content_type="application/json",
             **credentials,
         )
@@ -38,15 +34,17 @@
         self.assert_response_is_ok(response)
 
     def test_delete_model_unauthorized(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.unauthorized is None:
             self.test_case.skipTest("No unauthorized credentials provided")
         instance: Model = self.get_instance(self.test_case)
-        response = self.delete_model(id=instance.pk, credentials=None)
+        response = self.delete_model(
+            id=instance.pk, credentials=credentials.unauthorized
+        )
         self.assert_response_is_bad_request(
             response, status_code=HTTPStatus.UNAUTHORIZED
         )
 
     def test_delete_model_not_found(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         response = self.delete_model(id=uuid.uuid4(), credentials=credentials.ok)
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/tests/test_list.py` & `django_ninja_crud-0.1.2/ninja_crud/tests/test_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,105 @@
 import json
 from http import HTTPStatus
-from typing import Optional
+from typing import Callable, List
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
+from django.test import TestCase
 from django.urls import reverse
 
 from ninja_crud import utils
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
 from ninja_crud.views.list import ListModelView
 
 
 class ListModelViewTest(AbstractModelViewTest):
     model_view = ListModelView
 
-    def list_model(self, id: UUID, credentials: Optional[dict]) -> HttpResponse:
-        if credentials is None:
-            credentials = {}
-
+    def __init__(
+        self,
+        instance_getter: Callable[[TestCase], Model],
+        credentials_getter: Callable[[TestCase], Credentials] = None,
+        filters: List[dict] = None,
+    ) -> None:
+        super().__init__(
+            instance_getter=instance_getter, credentials_getter=credentials_getter
+        )
+        if filters is None:
+            filters = []
+        self.filters = filters
+
+    def list_model(
+        self, id: UUID, credentials: dict, data: dict = None
+    ) -> HttpResponse:
         model_view: ListModelView = self.get_model_view()
         model_name = utils.to_snake_case(self.model_view_set.model.__name__)
-        if model_view.is_instance_view:
+        if model_view.detail:
             related_model_name = utils.to_snake_case(model_view.related_model.__name__)
             url_name = f"{model_name}_{related_model_name}s"
             kwargs = {"id": id}
         else:
             url_name = f"{model_name}s"
             kwargs = {}
 
         response = self.client.get(
             reverse(f"api:{url_name}", kwargs=kwargs),
+            data=data,
             content_type="application/json",
             **credentials,
         )
         return response
 
-    def assert_response_is_ok(self, response: HttpResponse, id: UUID):
+    def assert_response_is_ok(
+        self, response: HttpResponse, id: UUID, data: dict = None
+    ):
         self.test_case.assertEqual(response.status_code, HTTPStatus.OK)
         content = json.loads(response.content)
 
         model_view: ListModelView = self.get_model_view()
 
-        if model_view.is_instance_view:
+        if model_view.detail:
             if model_view.get_queryset is not None:
                 queryset = model_view.get_queryset(id)
             else:
                 queryset = model_view.related_model.objects.get_queryset()
         else:
             if model_view.get_queryset is not None:
                 queryset = model_view.get_queryset()
             else:
                 queryset = self.model_view_set.model.objects.get_queryset()
 
+        if data is not None:
+            filter_instance = model_view.filter_schema(**data)
+            queryset = model_view.filter_queryset(queryset, filter_instance)
+
         self.assert_content_equals_schema_list(
             content, queryset=queryset, output_schema=model_view.output_schema
         )
 
     def test_list_model_ok(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         instance: Model = self.get_instance(self.test_case)
         response = self.list_model(id=instance.pk, credentials=credentials.ok)
         self.assert_response_is_ok(response, id=instance.pk)
 
+        for data in self.filters:
+            with self.test_case.subTest(data=data):
+                response = self.list_model(
+                    id=instance.pk, credentials=credentials.ok, data=data
+                )
+                self.assert_response_is_ok(response, id=instance.pk, data=data)
+
     def test_list_model_unauthorized(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.unauthorized is None:
             self.test_case.skipTest("No unauthorized credentials provided")
         instance: Model = self.get_instance(self.test_case)
-        response = self.list_model(id=instance.pk, credentials=None)
+        response = self.list_model(id=instance.pk, credentials=credentials.unauthorized)
         self.assert_response_is_bad_request(
             response, status_code=HTTPStatus.UNAUTHORIZED
         )
 
     def test_list_model_forbidden(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.forbidden is None:
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/tests/test_retrieve.py` & `django_ninja_crud-0.1.2/ninja_crud/tests/test_retrieve.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import json
 import uuid
 from http import HTTPStatus
-from typing import Optional
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.urls import reverse
 
 from ninja_crud import utils
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
 from ninja_crud.views.retrieve import RetrieveModelView
 
 
 class RetrieveModelViewTest(AbstractModelViewTest):
     model_view = RetrieveModelView
 
-    def retrieve_model(self, id: UUID, credentials: Optional[dict]) -> HttpResponse:
-        if credentials is None:
-            credentials = {}
-
+    def retrieve_model(self, id: UUID, credentials: dict) -> HttpResponse:
         kwargs = {"id": id}
         url_name = utils.to_snake_case(self.model_view_set.model.__name__)
         return self.client.get(
             reverse(f"api:{url_name}", kwargs=kwargs),
             content_type="application/json",
             **credentials,
         )
@@ -52,15 +48,17 @@
         self.assert_response_is_ok(response, id=instance.pk)
 
     def test_retrieve_model_unauthorized(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.unauthorized is None:
             self.test_case.skipTest("No unauthorized credentials provided")
         instance: Model = self.get_instance(self.test_case)
-        response = self.retrieve_model(id=instance.pk, credentials=None)
+        response = self.retrieve_model(
+            id=instance.pk, credentials=credentials.unauthorized
+        )
         self.assert_response_is_bad_request(
             response, status_code=HTTPStatus.UNAUTHORIZED
         )
 
     def test_retrieve_model_not_found(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         response = self.retrieve_model(id=uuid.uuid4(), credentials=credentials.ok)
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/tests/test_update.py` & `django_ninja_crud-0.1.2/ninja_crud/tests/test_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import uuid
 from http import HTTPStatus
-from typing import Callable, Optional
+from typing import Callable
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.test import TestCase
 from django.urls import reverse
 
@@ -17,27 +17,22 @@
 class UpdateModelViewTest(AbstractModelViewTest):
     model_view = UpdateModelView
 
     def __init__(
         self,
         payloads: Payloads,
         instance_getter: Callable[[TestCase], Model],
-        credentials_getter: Callable[[TestCase], Credentials],
+        credentials_getter: Callable[[TestCase], Credentials] = None,
     ) -> None:
         super().__init__(
             instance_getter=instance_getter, credentials_getter=credentials_getter
         )
         self.payloads = payloads
 
-    def update_model(
-        self, id: UUID, data: dict, credentials: Optional[dict]
-    ) -> HttpResponse:
-        if credentials is None:
-            credentials = {}
-
+    def update_model(self, id: UUID, data: dict, credentials: dict) -> HttpResponse:
         kwargs = {"id": id}
         url_name = utils.to_snake_case(self.model_view_set.model.__name__)
         return self.client.put(
             reverse(f"api:{url_name}", kwargs=kwargs),
             data=data,
             content_type="application/json",
             **credentials,
@@ -86,15 +81,15 @@
 
     def test_update_model_unauthorized(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.unauthorized is None:
             self.test_case.skipTest("No unauthorized credentials provided")
         instance: Model = self.get_instance(self.test_case)
         response = self.update_model(
-            id=instance.pk, data=self.payloads.ok, credentials=None
+            id=instance.pk, data=self.payloads.ok, credentials=credentials.unauthorized
         )
         self.assert_response_is_bad_request(
             response, status_code=HTTPStatus.UNAUTHORIZED
         )
 
     def test_update_model_not_found(self):
         credentials: Credentials = self.get_credentials(self.test_case)
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/views/abstract.py` & `django_ninja_crud-0.1.2/ninja_crud/views/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 class AbstractModelView(ABC):
     def __init__(self, decorators: List[Callable] = None) -> None:
         if decorators is None:
             decorators = []
         self.decorators = decorators
 
     @abstractmethod
-    def register_route(self, router: Router, model: Type[Model]) -> None:
+    def register_route(
+        self, router: Router, model: Type[Model]
+    ) -> None:  # pragma: no cover
         pass
 
 
 class ModelViewSet:
     model: Type[Model]
 
     @classmethod
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/views/create.py` & `django_ninja_crud-0.1.2/ninja_crud/views/create.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,35 +13,35 @@
 
 class CreateModelView(AbstractModelView):
     def __init__(
         self,
         input_schema: Type[Schema],
         output_schema: Type[Schema],
         decorators: List[Callable] = None,
-        is_instance_view: bool = False,
+        detail: bool = False,
         related_model: Type[Model] = None,
         pre_save: Union[
             Callable[[HttpRequest, Model], None],
             Callable[[HttpRequest, UUID, Model], None],
         ] = None,
         post_save: Union[
             Callable[[HttpRequest, Model], None],
             Callable[[HttpRequest, UUID, Model], None],
         ] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.input_schema = input_schema
         self.output_schema = output_schema
-        self.is_instance_view = is_instance_view
+        self.detail = detail
         self.related_model = related_model
         self.pre_save = pre_save
         self.post_save = post_save
 
     def register_route(self, router: Router, model: Type[Model]) -> None:
-        if self.is_instance_view:
+        if self.detail:
             self.register_instance_route(router, model)
         else:
             self.register_collection_route(router, model)
 
     def register_collection_route(self, router: Router, model: Type[Model]) -> None:
         model_name = utils.to_snake_case(model.__name__)
         operation_id = f"create_{model_name}"
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/views/delete.py` & `django_ninja_crud-0.1.2/ninja_crud/views/delete.py`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.1/ninja_crud/views/list.py` & `django_ninja_crud-0.1.2/ninja_crud/views/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,26 @@
         self,
         output_schema: Type[Schema],
         filter_schema: Type[FilterSchema] = None,
         queryset_getter: Union[
             Callable[[], QuerySet[Model]], Callable[[UUID], QuerySet[Model]]
         ] = None,
         related_model: Type[Model] = None,
-        is_instance_view: bool = False,
+        detail: bool = False,
         decorators: List[Callable] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.output_schema = output_schema
         self.filter_schema = filter_schema
         self.get_queryset = queryset_getter
         self.related_model = related_model
-        self.is_instance_view = is_instance_view
+        self.detail = detail
 
     def register_route(self, router: Router, model: Type[Model]) -> None:
-        if self.is_instance_view:
+        if self.detail:
             self.register_instance_route(router, model)
         else:
             self.register_collection_route(router, model)
 
     def register_collection_route(self, router: Router, model: Type[Model]) -> None:
         model_name = utils.to_snake_case(model.__name__)
         operation_id = f"list_{model_name}s"
@@ -57,15 +57,15 @@
         def list_models(
             request: HttpRequest, filters: filter_schema = Query(default=FilterSchema())
         ):
             if self.get_queryset is not None:
                 queryset = self.get_queryset()
             else:
                 queryset = model.objects.get_queryset()
-            return self.list_models(queryset=queryset, filters=filters)
+            return self.filter_queryset(queryset=queryset, filters=filters)
 
     def register_instance_route(self, router: Router, model: Type[Model]) -> None:
         parent_model_name = utils.to_snake_case(model.__name__)
         model_name = utils.to_snake_case(self.related_model.__name__)
         plural_model_name = f"{model_name}s"
         url = "/{id}/" + plural_model_name
         operation_id = f"list_{parent_model_name}_{plural_model_name}"
@@ -88,17 +88,17 @@
             id: UUID,
             filters: filter_schema = Query(default=FilterSchema()),
         ):
             if self.get_queryset is not None:
                 queryset = self.get_queryset(id)
             else:
                 queryset = self.related_model.objects.get_queryset()
-            return self.list_models(queryset=queryset, filters=filters)
+            return self.filter_queryset(queryset=queryset, filters=filters)
 
     @staticmethod
-    def list_models(queryset: QuerySet[Model], filters: FilterSchema):
+    def filter_queryset(queryset: QuerySet[Model], filters: FilterSchema):
         filters_dict = filters.dict()
         if "order_by" in filters_dict and filters_dict["order_by"] is not None:
             queryset = queryset.order_by(*filters_dict.pop("order_by"))
 
         queryset = filters.filter(queryset)
         return queryset
```

### Comparing `django_ninja_crud-0.1.1/ninja_crud/views/retrieve.py` & `django_ninja_crud-0.1.2/ninja_crud/views/retrieve.py`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.1/ninja_crud/views/update.py` & `django_ninja_crud-0.1.2/ninja_crud/views/update.py`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.1/pyproject.toml` & `django_ninja_crud-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 src_paths = ["ninja_crud", "tests", "examples"]
 
 [tool.pycln]
 all = true
 
 [tool.poetry]
 name = "django-ninja-crud"
-version = "0.1.1"
+version = "0.1.2"
 description = "Django Ninja CRUD is a library that allows you to create CRUD APIs in a few lines of code."
 authors = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 maintainers = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/hbakri/django-ninja-crud"
 license = "MIT"
 classifiers = [
```

### Comparing `django_ninja_crud-0.1.1/PKG-INFO` & `django_ninja_crud-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ninja-crud
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django Ninja CRUD is a library that allows you to create CRUD APIs in a few lines of code.
 Home-page: https://github.com/hbakri/django-ninja-crud
 License: MIT
 Author: Hicham Bakri
 Author-email: hicham.bakri76@gmail.com
 Maintainer: Hicham Bakri
 Maintainer-email: hicham.bakri76@gmail.com
@@ -78,45 +78,53 @@
 
 class DepartmentOut(Schema):
     id: int
     title: str
 ```
 
 Here is a brief example of how to use django-ninja-crud:
+
 ```python
 # views.py
-from examples.models import Department
-from examples.schemas import DepartmentIn, DepartmentOut
-from ninja_crud.views import ModelViewSet, ListModelView, CreateModelView, \
+from example.models import Department
+from example.schemas import DepartmentIn, DepartmentOut
+from ninja import Router
+from ninja_crud.views import ModelViewSet, ListModelView, CreateModelView,
     RetrieveModelView, UpdateModelView, DeleteModelView
 
 
 class DepartmentViewSet(ModelViewSet):
     model = Department
     input_schema = DepartmentIn
     output_schema = DepartmentOut
 
     list = ListModelView(output_schema=output_schema)
     create = CreateModelView(input_schema=input_schema, output_schema=output_schema)
     retrieve = RetrieveModelView(output_schema=output_schema)
     update = UpdateModelView(input_schema=input_schema, output_schema=output_schema)
     delete = DeleteModelView()
+
+
+router = Router()
+DepartmentViewSet.register_routes(router)
 ```
 
 ## Testing
 You can then write the associated tests like so:
+
 ```python
 # tests.py
 from django.test import TestCase
-from examples.models import Department
-from examples.views.view_department import DepartmentViewSet
-from ninja_crud.tests import CreateModelViewTest, DeleteModelViewTest, \
-    ListModelViewTest, ModelViewSetTest, Payloads, RetrieveModelViewTest, \
+from example.models import Department
+from example.views.view_department import DepartmentViewSet
+from ninja_crud.tests import CreateModelViewTest, DeleteModelViewTest,
+    ListModelViewTest, ModelViewSetTest, Payloads, RetrieveModelViewTest,
     UpdateModelViewTest
 
+
 class DepartmentViewSetTest(ModelViewSetTest, TestCase):
     model_view_set = DepartmentViewSet
 
     @classmethod
     def setUpTestData(cls):
         super().setUpTestData()
         cls.department_1 = Department.objects.create(title="department-1")
```


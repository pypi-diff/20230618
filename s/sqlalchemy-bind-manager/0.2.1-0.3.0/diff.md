# Comparing `tmp/sqlalchemy_bind_manager-0.2.1.tar.gz` & `tmp/sqlalchemy_bind_manager-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_bind_manager-0.2.1.tar", max compression
+gzip compressed data, was "sqlalchemy_bind_manager-0.3.0.tar", max compression
```

## Comparing `sqlalchemy_bind_manager-0.2.1.tar` & `sqlalchemy_bind_manager-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/LICENSE
--rw-r--r--   0        0        0    11748 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/README.md
--rw-r--r--   0        0        0     1957 2023-04-25 17:00:09.547293 sqlalchemy_bind_manager-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      301 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/__init__.py
--rw-r--r--   0        0        0     5221 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_bind_manager.py
--rw-r--r--   0        0        0      136 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/__init__.py
--rw-r--r--   0        0        0     5959 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/async_.py
--rw-r--r--   0        0        0     6296 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/common.py
--rw-r--r--   0        0        0     5521 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/sync.py
--rw-r--r--   0        0        0     3125 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_transaction_handler.py
--rw-r--r--   0        0        0     1698 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_unit_of_work.py
--rw-r--r--   0        0        0      310 2023-04-25 16:59:54.450825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/exceptions.py
--rw-r--r--   0        0        0     1995 2023-04-25 16:59:54.454825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/protocols.py
--rw-r--r--   0        0        0        0 2023-04-25 16:59:54.454825 sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/py.typed
--rw-r--r--   0        0        0    13392 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/LICENSE
+-rw-r--r--   0        0        0    12017 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/README.md
+-rw-r--r--   0        0        0     2103 2023-06-18 17:43:39.487600 sqlalchemy_bind_manager-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/__init__.py
+-rw-r--r--   0        0        0     5241 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_bind_manager.py
+-rw-r--r--   0        0        0      204 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/__init__.py
+-rw-r--r--   0        0        0     5734 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/async_.py
+-rw-r--r--   0        0        0     8738 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/base_repository.py
+-rw-r--r--   0        0        0      937 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/common.py
+-rw-r--r--   0        0        0     7429 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/result_presenters.py
+-rw-r--r--   0        0        0     5731 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/sync.py
+-rw-r--r--   0        0        0     3125 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_transaction_handler.py
+-rw-r--r--   0        0        0     1722 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_unit_of_work.py
+-rw-r--r--   0        0        0      310 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/exceptions.py
+-rw-r--r--   0        0        0    10354 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/protocols.py
+-rw-r--r--   0        0        0        0 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/py.typed
+-rw-r--r--   0        0        0      242 2023-06-18 17:43:22.895494 sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/repository.py
+-rw-r--r--   0        0        0    13411 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.3.0/PKG-INFO
```

### Comparing `sqlalchemy_bind_manager-0.2.1/LICENSE` & `sqlalchemy_bind_manager-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.2.1/README.md` & `sqlalchemy_bind_manager-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 [![Python 3.10](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.10.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.10.yml)
 [![Python 3.11](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.11.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.11.yml)
 
 [![Maintainability](https://api.codeclimate.com/v1/badges/0140f7f4e559ae806887/maintainability)](https://codeclimate.com/github/febus982/sqlalchemy-bind-manager/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/0140f7f4e559ae806887/test_coverage)](https://codeclimate.com/github/febus982/sqlalchemy-bind-manager/test_coverage)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 This package provides an easy way to configure and use SQLAlchemy engines and sessions
 without depending on frameworks.
 
 It is composed by two main components:
 
 * A manager class for SQLAlchemy engine configuration
@@ -173,15 +174,15 @@
 to check [SQLAlchemy asyncio documentation](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html)
 
 ## Repository / Unit of work
 
 The `SQLAlchemyRepository` and `SQLAlchemyAsyncRepository` class can be used simply by extending them.
 
 ```python
-from sqlalchemy_bind_manager import SQLAlchemyRepository
+from sqlalchemy_bind_manager.repository import SQLAlchemyRepository
 
 
 class MyModel(model_declarative_base):
     pass
 
 
 class ModelRepository(SQLAlchemyRepository[MyModel]):
@@ -195,14 +196,15 @@
 
 * `get`: Retrieve a model by identifier
 * `save`: Persist a model
 * `save_many`: Persist multiple models in a single transaction
 * `delete`: Delete a model
 * `find`: Search for a list of models (basically an adapter for SELECT queries)
 * `paginated_find`: Search for a list of models, with pagination support
+* `cursor_paginated_find`: Search for a list of models, with cursor based pagination support
 
 ### Session lifecycle in repositories
 
 [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/20/orm/session_basics.html#when-do-i-construct-a-session-when-do-i-commit-it-and-when-do-i-close-it)
 recommends we create `Session` object at the beginning of a logical operation where
 database access is potentially anticipated.
```

### Comparing `sqlalchemy_bind_manager-0.2.1/pyproject.toml` & `sqlalchemy_bind_manager-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-bind-manager"
-version = "0.2.1"
+version = "0.3.0"
 description = "A manager to easily handle multiple SQLAlchemy configurations"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/sqlalchemy-bind-manager"
 readme = "README.md"
 packages = [{include = "sqlalchemy_bind_manager"}]
 keywords = ["sqlalchemy", "config", "manager"]
@@ -44,25 +44,33 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "~0.18.0"
 coverage = "~6.5.0"
 black = "~22.10.0"
-flake8 = "~5.0.4"
 mypy = "~0.990"
 pytest = "~7.2.0"
 pytest-asyncio = "~0.20.3"
 pytest-cov = "~4.0.0"
 pytest-factoryboy = "~2.5.0"
 pytest-xdist = "~3.0.2"
+ruff = "~0.0.263"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 minversion = "6.0"
 addopts = "-n auto --cov-report=term-missing"
 testpaths = [
     "tests",
 ]
 
 [tool.mypy]
 files = "sqlalchemy_bind_manager"
+plugins = "pydantic.mypy"
+
+[tool.ruff]
+select = ["E", "F", "I"]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+"repository.py" = ["F401"]
```

### Comparing `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_bind_manager.py` & `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_bind_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Union, Mapping, MutableMapping
+from typing import Mapping, MutableMapping, Union
 
 from pydantic import BaseModel
-from sqlalchemy import create_engine, MetaData
+from sqlalchemy import MetaData, create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.asyncio import (
-    AsyncSession,
-    create_async_engine,
     AsyncEngine,
+    AsyncSession,
     async_sessionmaker,
+    create_async_engine,
 )
-from sqlalchemy.orm import sessionmaker, Session
+from sqlalchemy.orm import Session, sessionmaker
 from sqlalchemy.orm.decl_api import registry
 
 from sqlalchemy_bind_manager.exceptions import (
-    NotInitializedBind,
     InvalidConfig,
+    NotInitializedBind,
 )
 
 
 class SQLAlchemyConfig(BaseModel):
     engine_options: Union[dict, None]
     engine_url: str
     session_options: Union[dict, None]
@@ -78,15 +78,16 @@
         if not any(
             [
                 isinstance(config, SQLAlchemyConfig),
                 isinstance(config, SQLAlchemyAsyncConfig),
             ]
         ):
             raise InvalidConfig(
-                f"Config for bind `{name}` is not a SQLAlchemyConfig or SQLAlchemyAsyncConfig object"
+                f"Config for bind `{name}` is not a SQLAlchemyConfig"
+                f" or SQLAlchemyAsyncConfig object"
             )
 
         engine_options: dict = config.engine_options or {}
         engine_options.setdefault("echo", False)
         engine_options.setdefault("future", True)
 
         session_options: dict = config.session_options or {}
```

### Comparing `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/async_.py` & `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/async_.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 from abc import ABC
 from contextlib import asynccontextmanager
 from typing import (
-    Union,
+    Any,
+    AsyncIterator,
     Generic,
-    Tuple,
     Iterable,
     List,
-    AsyncIterator,
-    Any,
     Mapping,
+    Tuple,
     Type,
+    Union,
 )
 
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from .._bind_manager import SQLAlchemyAsyncBind
 from .._transaction_handler import AsyncSessionHandler
-from ..exceptions import ModelNotFound, InvalidConfig
-from .common import MODEL, PRIMARY_KEY, SortDirection, BaseRepository, PaginatedResult
+from ..exceptions import InvalidConfig, ModelNotFound
+from .base_repository import (
+    BaseRepository,
+    SortDirection,
+)
+from .common import (
+    MODEL,
+    PRIMARY_KEY,
+    CursorPaginatedResult,
+    CursorReference,
+    PaginatedResult,
+)
+from .result_presenters import CursorPaginatedResultPresenter, PaginatedResultPresenter
 
 
 class SQLAlchemyAsyncRepository(Generic[MODEL], BaseRepository[MODEL], ABC):
     _session_handler: AsyncSessionHandler
     _external_session: Union[AsyncSession, None]
 
     def __init__(
@@ -50,122 +61,104 @@
         if not self._external_session:
             async with self._session_handler.get_session(not commit) as _session:
                 yield _session
         else:
             yield self._external_session
 
     async def save(self, instance: MODEL) -> MODEL:
-        """Persist a model.
-
-        :param instance: A mapped object instance to be persisted
-        :return: The model instance after being persisted (e.g. with primary key populated)
-        """
         async with self._get_session() as session:
             session.add(instance)
         return instance
 
     async def save_many(
         self,
         instances: Iterable[MODEL],
     ) -> Iterable[MODEL]:
-        """Persist many models in a single database get_session.
-
-        :param instances: A list of mapped objects to be persisted
-        :type instances: Iterable
-        :return: The model instances after being persisted (e.g. with primary keys populated)
-        """
         async with self._get_session() as session:
             session.add_all(instances)
         return instances
 
     async def get(self, identifier: PRIMARY_KEY) -> MODEL:
-        """Get a model by primary key.
-
-        :param identifier: The primary key
-        :return: A model instance
-        :raises ModelNotFound: No model has been found using the primary key
-        """
-        # TODO: implement get_many()
         async with self._get_session(commit=False) as session:
             model = await session.get(self._model, identifier)
         if model is None:
             raise ModelNotFound("No rows found for provided primary key.")
         return model
 
     async def delete(
         self,
         entity: Union[MODEL, PRIMARY_KEY],
     ) -> None:
-        """Deletes a model.
-
-        :param entity: The model instance or the primary key
-        :type entity: Union[MODEL, PRIMARY_KEY]
-        """
         # TODO: delete without loading the model
-        obj = entity if isinstance(entity, self._model) else await self.get(entity)  # type: ignore
+        if isinstance(entity, self._model):
+            obj = entity
+        else:
+            obj = await self.get(entity)  # type: ignore
         async with self._get_session() as session:
             await session.delete(obj)
 
     async def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
     ) -> List[MODEL]:
-        """Find models using filters
-
-        E.g.
-        find(search_params={"name": "John"}) finds all models with name = John
-
-        :param order_by:
-        :param search_params: A dictionary containing equality filters
-        :param limit: Number of models to retrieve
-        :type limit: int
-        :param offset: Number of models to skip
-        :type offset: int
-        :return: A collection of models
-        :rtype: List
-        """
         stmt = self._find_query(search_params, order_by)
 
         async with self._get_session() as session:
             result = await session.execute(stmt)
             return [x for x in result.scalars()]
 
     async def paginated_find(
         self,
-        per_page: int,
-        page: int,
+        items_per_page: int,
+        page: int = 1,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
     ) -> PaginatedResult[MODEL]:
-        """Find models using filters and pagination
-
-        E.g.
-        find(name="John") finds all models with name = John
-
-        :param per_page: Number of models to retrieve
-        :type per_page: int
-        :param page: Page to retrieve
-        :type page: int
-        :param search_params: A dictionary containing equality filters
-        :param order_by:
-        :return: A collection of models
-        :rtype: List
-        """
-
         find_stmt = self._find_query(search_params, order_by)
-        paginated_stmt = self._paginate_query(find_stmt, page, per_page)
+        paginated_stmt = self._paginate_query_by_page(find_stmt, page, items_per_page)
 
         async with self._get_session() as session:
             total_items_count = (
                 await session.execute(self._count_query(find_stmt))
             ).scalar() or 0
             result_items = [
                 x for x in (await session.execute(paginated_stmt)).scalars()
             ]
 
-            return self._build_paginated_result(
+            return PaginatedResultPresenter.build_result(
                 result_items=result_items,
                 total_items_count=total_items_count,
                 page=page,
-                per_page=per_page,
+                items_per_page=self._sanitised_query_limit(items_per_page),
+            )
+
+    async def cursor_paginated_find(
+        self,
+        items_per_page: int,
+        cursor_reference: Union[CursorReference, None] = None,
+        is_before_cursor: bool = False,
+        search_params: Union[None, Mapping[str, Any]] = None,
+    ) -> CursorPaginatedResult[MODEL]:
+        find_stmt = self._find_query(search_params)
+        paginated_stmt = self._cursor_paginated_query(
+            find_stmt,
+            cursor_reference=cursor_reference,
+            is_before_cursor=is_before_cursor,
+            items_per_page=items_per_page,
+        )
+
+        async with self._get_session() as session:
+            total_items_count = (
+                await session.execute(self._count_query(find_stmt))
+            ).scalar() or 0
+            result_items = [
+                x for x in (await session.execute(paginated_stmt)).scalars()
+            ] or []
+
+            return CursorPaginatedResultPresenter.build_result(
+                result_items=result_items,
+                total_items_count=total_items_count,
+                items_per_page=self._sanitised_query_limit(items_per_page),
+                cursor_reference=cursor_reference,
+                is_before_cursor=is_before_cursor,
             )
```

### Comparing `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/common.py` & `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/base_repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,52 @@
 from abc import ABC
 from enum import Enum
 from functools import partial
-from math import ceil
 from typing import (
-    TypeVar,
-    Union,
+    Any,
     Generic,
-    Type,
-    Tuple,
     Iterable,
-    Any,
     Mapping,
-    List,
-    Collection,
+    Tuple,
+    Type,
+    Union,
 )
 
-from pydantic.generics import GenericModel
-from sqlalchemy import asc, desc, select, func
-from sqlalchemy.orm import class_mapper, Mapper, lazyload
+from sqlalchemy import asc, desc, func, inspect, select
+from sqlalchemy.orm import Mapper, aliased, class_mapper, lazyload
 from sqlalchemy.orm.exc import UnmappedClassError
 from sqlalchemy.sql import Select
 
 from sqlalchemy_bind_manager.exceptions import InvalidModel, UnmappedProperty
 
-MODEL = TypeVar("MODEL")
-PRIMARY_KEY = Union[str, int, tuple, dict]
+from .common import (
+    MODEL,
+    CursorReference,
+)
 
 
 class SortDirection(Enum):
     ASC = partial(asc)
     DESC = partial(desc)
 
 
-class PaginatedResult(GenericModel, Generic[MODEL]):
-    items: List[MODEL]
-    page: int
-    per_page: int
-    total_pages: int
-    total_items: int
-
-
 class BaseRepository(Generic[MODEL], ABC):
     _max_query_limit: int = 50
     _model: Type[MODEL]
 
     def __init__(self, model_class: Union[Type[MODEL], None] = None) -> None:
         if getattr(self, "_model", None) is None and model_class is not None:
             self._model = model_class
 
         if getattr(self, "_model", None) is None or not self._is_mapped_class(
             self._model
         ):
             raise InvalidModel(
-                "You need to supply a valid model class either in the `model_class` parameter"
+                "You need to supply a valid model class"
+                " either in the `model_class` parameter"
                 " or in the `_model` class property."
             )
 
     def _is_mapped_class(self, class_: Type[MODEL]) -> bool:
         """Checks if the class is mapped in SQLAlchemy.
 
         :param class_: the model class
@@ -75,15 +65,16 @@
         :param property_name: The name of the property to be evaluated.
         :type property_name: str
         :raises UnmappedProperty: When the property is not mapped.
         """
         m: Mapper = class_mapper(self._model)
         if property_name not in m.column_attrs:
             raise UnmappedProperty(
-                f"Property `{property_name}` is not mapped in the ORM for model `{self._model}`"
+                f"Property `{property_name}` is not mapped"
+                f" in the ORM for model `{self._model}`"
             )
 
     def _filter_select(self, stmt: Select, search_params: Mapping[str, Any]) -> Select:
         """Build the query filtering clauses from submitted parameters.
 
         E.g.
         _filter_select(stmt, name="John") adds a `WHERE name = John` statement
@@ -106,16 +97,19 @@
 
     def _filter_order_by(
         self, stmt: Select, order_by: Iterable[Union[str, Tuple[str, SortDirection]]]
     ) -> Select:
         """Build the query ordering clauses from submitted parameters.
 
         E.g.
-        _filter_order_by(stmt, ['name']) adds a `ORDER BY name` statement
-        _filter_order_by(stmt, [('name', SortDirection.ASC)]) adds a `ORDER BY name ASC` statement
+        `_filter_order_by(stmt, ['name'])`
+            adds a `ORDER BY name` statement
+
+        `_filter_order_by(stmt, [('name', SortDirection.ASC)])`
+            adds a `ORDER BY name ASC` statement
 
         :param stmt: a Select statement
         :type stmt: Select
         :param order_by: a list of columns, or tuples (column, direction)
         :return: The filtered query
         """
         for value in order_by:
@@ -143,59 +137,130 @@
         return stmt
 
     def _count_query(
         self,
         query: Select,
     ) -> Select:
         return select(func.count()).select_from(
-            query.options(lazyload("*")).order_by(None).subquery()  # type: ignore
+            query.options(lazyload("*")).subquery()  # type: ignore
         )
 
-    def _paginate_query(
+    def _paginate_query_by_page(
         self,
         stmt: Select,
         page: int,
-        per_page: int,
+        items_per_page: int,
     ) -> Select:
         """Build the query offset and limit clauses from submitted parameters.
 
         :param stmt: a Select statement
         :type stmt: Select
         :param page: Number of models to skip
         :type page: int
-        :param per_page: Number of models to retrieve
-        :type per_page: int
+        :param items_per_page: Number of models to retrieve
+        :type items_per_page: int
         :return: The filtered query
         """
 
-        _offset = max((page - 1) * per_page, 0)
+        _offset = max((page - 1) * items_per_page, 0)
         if _offset > 0:
             stmt = stmt.offset(_offset)
 
-        _limit = max(min(per_page, self._max_query_limit), 0)
+        _limit = self._sanitised_query_limit(items_per_page)
         stmt = stmt.limit(_limit)
 
         return stmt
 
-    def _build_paginated_result(
+    def _cursor_paginated_query(
         self,
-        result_items: Collection[MODEL],
-        total_items_count: int,
-        page: int,
-        per_page: int,
-    ) -> PaginatedResult:
+        stmt: Select,
+        cursor_reference: Union[CursorReference, None],
+        is_before_cursor: bool = False,
+        items_per_page: int = _max_query_limit,
+    ) -> Select:
+        """Build the query offset and limit clauses from submitted parameters.
 
-        _per_page = max(min(per_page, self._max_query_limit), 0)
-        total_pages = (
-            0
-            if total_items_count == 0 or total_items_count is None
-            else ceil(total_items_count / _per_page)
-        )
-        _page = 0 if len(result_items) == 0 else min(page, total_pages)
+        :param stmt: a Select statement
+        :type stmt: Select
+        :param before: Identifier of the last node to skip
+        :type before: Union[int, str]
+        :param after: Identifier of the last node to skip
+        :type after: Union[int, str]
+        :param items_per_page: Number of models to retrieve
+        :type items_per_page: int
+        :return: The filtered query
+        """
+
+        forward_limit = self._sanitised_query_limit(items_per_page) + 1
+
+        if not cursor_reference:
+            return stmt.limit(forward_limit).order_by(  # type: ignore
+                asc(self._model_pk())
+            )
+
+        # TODO: Use window functions
+        if not is_before_cursor:
+            previous_query = stmt.where(
+                getattr(self._model, cursor_reference.column) <= cursor_reference.value
+            )
+            previous_query = (
+                self._filter_order_by(
+                    previous_query, [(cursor_reference.column, SortDirection.DESC)]
+                )
+                .limit(1)
+                .subquery("previous")  # type: ignore
+            )
+
+            page_query = stmt.where(
+                getattr(self._model, cursor_reference.column) > cursor_reference.value
+            )
+            page_query = (
+                self._filter_order_by(
+                    page_query, [(cursor_reference.column, SortDirection.ASC)]
+                )
+                .limit(forward_limit)
+                .subquery("page")  # type: ignore
+            )
+        else:
+            previous_query = stmt.where(
+                getattr(self._model, cursor_reference.column) >= cursor_reference.value
+            )
+            previous_query = (
+                self._filter_order_by(
+                    previous_query, [(cursor_reference.column, SortDirection.ASC)]
+                )
+                .limit(1)
+                .subquery("previous")  # type: ignore
+            )
+
+            page_query = stmt.where(
+                getattr(self._model, cursor_reference.column) < cursor_reference.value
+            )
+            page_query = (
+                self._filter_order_by(
+                    page_query, [(cursor_reference.column, SortDirection.DESC)]
+                )
+                .limit(forward_limit)
+                .subquery("page")  # type: ignore
+            )
 
-        return PaginatedResult(
-            items=result_items,
-            page=_page,
-            per_page=_per_page,
-            total_items=total_items_count,
-            total_pages=total_pages,
+        query = select(
+            aliased(
+                self._model,
+                select(previous_query)
+                .union(select(page_query))
+                .order_by(cursor_reference.column)
+                .subquery(),  # type: ignore
+            )
         )
+
+        return query
+
+    def _sanitised_query_limit(self, limit):
+        return max(min(limit, self._max_query_limit), 0)
+
+    def _model_pk(self) -> str:
+        primary_keys = inspect(self._model).primary_key  # type: ignore
+        if len(primary_keys) > 1:
+            raise NotImplementedError("Composite primary keys are not supported.")
+
+        return primary_keys[0].name
```

### Comparing `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_repository/sync.py` & `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_repository/sync.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 from abc import ABC
 from contextlib import contextmanager
-from math import ceil
 from typing import (
-    Union,
+    Any,
     Generic,
     Iterable,
-    Tuple,
-    List,
     Iterator,
-    Any,
+    List,
     Mapping,
+    Tuple,
     Type,
+    Union,
 )
 
 from sqlalchemy.orm import Session
 
 from .._bind_manager import SQLAlchemyBind
 from .._transaction_handler import SessionHandler
-from ..exceptions import ModelNotFound, InvalidConfig
-from .common import MODEL, PRIMARY_KEY, SortDirection, BaseRepository, PaginatedResult
+from ..exceptions import InvalidConfig, ModelNotFound
+from .base_repository import (
+    BaseRepository,
+    SortDirection,
+)
+from .common import (
+    MODEL,
+    PRIMARY_KEY,
+    CursorPaginatedResult,
+    CursorReference,
+    PaginatedResult,
+)
+from .result_presenters import CursorPaginatedResultPresenter, PaginatedResultPresenter
 
 
 class SQLAlchemyRepository(Generic[MODEL], BaseRepository[MODEL], ABC):
     _session_handler: SessionHandler
     _external_session: Union[Session, None]
 
     def __init__(
         self,
         bind: Union[SQLAlchemyBind, None] = None,
         session: Union[Session, None] = None,
         model_class: Union[Type[MODEL], None] = None,
     ) -> None:
-        """
-        :param bind: A configured instance of SQLAlchemyBind
-        :type bind: Union[SQLAlchemyBind, None]
-        :param session: An externally managed session
-        :type session: Union[Session, None]
-        :param model_class: A mapped SQLAlchemy model
-        :type model_class: Union[Type[MODEL], None]
-        """
         super().__init__(model_class=model_class)
         if not (bool(bind) ^ bool(session)):
             raise InvalidConfig("Either `bind` or `session` have to be used, not both")
         self._external_session = session
         if bind:
             self._session_handler = SessionHandler(bind)
 
@@ -51,110 +53,112 @@
         if not self._external_session:
             with self._session_handler.get_session(not commit) as _session:
                 yield _session
         else:
             yield self._external_session
 
     def save(self, instance: MODEL) -> MODEL:
-        """Persist a model.
-
-        :param instance: A mapped object instance to be persisted
-        :return: The model instance after being persisted (e.g. with primary key populated)
-        """
         with self._get_session() as session:
             session.add(instance)
         return instance
 
     def save_many(self, instances: Iterable[MODEL]) -> Iterable[MODEL]:
-        """Persist many models in a single database get_session.
-
-        :param instances: A list of mapped objects to be persisted
-        :type instances: Iterable
-        :return: The model instances after being persisted (e.g. with primary keys populated)
-        """
         with self._get_session() as session:
             session.add_all(instances)
         return instances
 
     def get(self, identifier: PRIMARY_KEY) -> MODEL:
-        """Get a model by primary key.
-
-        :param identifier: The primary key
-        :return: A model instance
-        :raises ModelNotFound: No model has been found using the primary key
-        """
-        # TODO: implement get_many()
         with self._get_session(commit=False) as session:
             model = session.get(self._model, identifier)
         if model is None:
             raise ModelNotFound("No rows found for provided primary key.")
         return model
 
     def delete(self, entity: Union[MODEL, PRIMARY_KEY]) -> None:
-        """Deletes a model.
-
-        :param entity: The model instance or the primary key
-        :type entity: Union[MODEL, PRIMARY_KEY]
-        """
         # TODO: delete without loading the model
-        obj = entity if isinstance(entity, self._model) else self.get(entity)  # type: ignore
+        if isinstance(entity, self._model):
+            obj = entity
+        else:
+            obj = self.get(entity)  # type: ignore
         with self._get_session() as session:
             session.delete(obj)
 
     def find(
         self,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
     ) -> List[MODEL]:
-        """Find models using filters
-
-        E.g.
-        find(name="John") finds all models with name = John
-
-        :param search_params: A dictionary containing equality filters
-        :param order_by:
-        :return: A collection of models
-        :rtype: List
-        """
         stmt = self._find_query(search_params, order_by)
 
         with self._get_session() as session:
             result = session.execute(stmt)
             return [x for x in result.scalars()]
 
     def paginated_find(
         self,
-        per_page: int,
-        page: int,
+        items_per_page: int,
+        page: int = 1,
         search_params: Union[None, Mapping[str, Any]] = None,
         order_by: Union[None, Iterable[Union[str, Tuple[str, SortDirection]]]] = None,
     ) -> PaginatedResult[MODEL]:
-        """Find models using filters and pagination
+        find_stmt = self._find_query(search_params, order_by)
+        paginated_stmt = self._paginate_query_by_page(find_stmt, page, items_per_page)
+
+        with self._get_session() as session:
+            total_items_count = (
+                session.execute(self._count_query(find_stmt)).scalar() or 0
+            )
+            result_items = [x for x in session.execute(paginated_stmt).scalars()]
+
+            return PaginatedResultPresenter.build_result(
+                result_items=result_items,
+                total_items_count=total_items_count,
+                page=page,
+                items_per_page=self._sanitised_query_limit(items_per_page),
+            )
+
+    def cursor_paginated_find(
+        self,
+        items_per_page: int,
+        cursor_reference: Union[CursorReference, None] = None,
+        is_before_cursor: bool = False,
+        search_params: Union[None, Mapping[str, Any]] = None,
+    ) -> CursorPaginatedResult[MODEL]:
+        """Find models using filters and cursor based pagination
 
         E.g.
         find(name="John") finds all models with name = John
 
-        :param per_page: Number of models to retrieve
-        :type per_page: int
-        :param page: Page to retrieve
-        :type page: int
+        :param items_per_page: Number of models to retrieve
+        :type items_per_page: int
+        :param order_by: Model property to use for ordering and before/after evaluation
+        :type order_by: str
+        :param before: Identifier of the last node to skip
+        :type before: Union[int, str]
+        :param after: Identifier of the last node to skip
+        :type after: Union[int, str]
         :param search_params: A dictionary containing equality filters
-        :param order_by:
         :return: A collection of models
         :rtype: List
         """
+        find_stmt = self._find_query(search_params)
 
-        find_stmt = self._find_query(search_params, order_by)
-        paginated_stmt = self._paginate_query(find_stmt, page, per_page)
+        paginated_stmt = self._cursor_paginated_query(
+            find_stmt,
+            cursor_reference=cursor_reference,
+            is_before_cursor=is_before_cursor,
+            items_per_page=items_per_page,
+        )
 
         with self._get_session() as session:
             total_items_count = (
                 session.execute(self._count_query(find_stmt)).scalar() or 0
             )
             result_items = [x for x in session.execute(paginated_stmt).scalars()]
 
-            return self._build_paginated_result(
+            return CursorPaginatedResultPresenter.build_result(
                 result_items=result_items,
                 total_items_count=total_items_count,
-                page=page,
-                per_page=per_page,
+                items_per_page=self._sanitised_query_limit(items_per_page),
+                cursor_reference=cursor_reference,
+                is_before_cursor=is_before_cursor,
             )
```

### Comparing `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_transaction_handler.py` & `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_transaction_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from asyncio import get_event_loop
-from typing import Iterator, AsyncIterator
-from contextlib import contextmanager, asynccontextmanager
+from contextlib import asynccontextmanager, contextmanager
+from typing import AsyncIterator, Iterator
 from uuid import uuid4
 
 from sqlalchemy.ext.asyncio import (
-    async_scoped_session,
     AsyncSession,
+    async_scoped_session,
 )
-from sqlalchemy.orm import scoped_session, Session
+from sqlalchemy.orm import Session, scoped_session
 
 from sqlalchemy_bind_manager._bind_manager import (
-    SQLAlchemyBind,
     SQLAlchemyAsyncBind,
+    SQLAlchemyBind,
 )
 from sqlalchemy_bind_manager.exceptions import UnsupportedBind
 
 
 class SessionHandler:
     _session_class: scoped_session
     session: Session
```

### Comparing `sqlalchemy_bind_manager-0.2.1/sqlalchemy_bind_manager/_unit_of_work.py` & `sqlalchemy_bind_manager-0.3.0/sqlalchemy_bind_manager/_unit_of_work.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from contextlib import contextmanager, asynccontextmanager
-from typing import Iterable, Type, Iterator, AsyncIterator
+from contextlib import asynccontextmanager, contextmanager
+from typing import AsyncIterator, Iterable, Iterator, Type
 
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import Session
 
-from sqlalchemy_bind_manager import SQLAlchemyRepository, SQLAlchemyAsyncRepository
-from sqlalchemy_bind_manager._bind_manager import SQLAlchemyBind, SQLAlchemyAsyncBind
+from sqlalchemy_bind_manager._bind_manager import SQLAlchemyAsyncBind, SQLAlchemyBind
 from sqlalchemy_bind_manager._transaction_handler import (
-    SessionHandler,
     AsyncSessionHandler,
+    SessionHandler,
+)
+from sqlalchemy_bind_manager.repository import (
+    SQLAlchemyAsyncRepository,
+    SQLAlchemyRepository,
 )
 
 
 class UnitOfWork:
     _transaction_handler: SessionHandler
 
     def __init__(
```

### Comparing `sqlalchemy_bind_manager-0.2.1/PKG-INFO` & `sqlalchemy_bind_manager-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bind-manager
-Version: 0.2.1
+Version: 0.3.0
 Summary: A manager to easily handle multiple SQLAlchemy configurations
 Home-page: https://github.com/febus982/sqlalchemy-bind-manager
 License: MIT
 Keywords: sqlalchemy,config,manager
 Author: Federico Busetti
 Author-email: 729029+febus982@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
@@ -17,20 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: SQLAlchemy[asyncio,mypy] (>=2.0.0,<2.1.0)
 Requires-Dist: pydantic (>=1.10.2,<1.11.0)
 Project-URL: Repository, https://github.com/febus982/sqlalchemy-bind-manager
@@ -45,14 +40,15 @@
 [![Python 3.10](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.10.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.10.yml)
 [![Python 3.11](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.11.yml/badge.svg?event=push)](https://github.com/febus982/sqlalchemy-bind-manager/actions/workflows/python-3.11.yml)
 
 [![Maintainability](https://api.codeclimate.com/v1/badges/0140f7f4e559ae806887/maintainability)](https://codeclimate.com/github/febus982/sqlalchemy-bind-manager/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/0140f7f4e559ae806887/test_coverage)](https://codeclimate.com/github/febus982/sqlalchemy-bind-manager/test_coverage)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 This package provides an easy way to configure and use SQLAlchemy engines and sessions
 without depending on frameworks.
 
 It is composed by two main components:
 
 * A manager class for SQLAlchemy engine configuration
@@ -211,15 +207,15 @@
 to check [SQLAlchemy asyncio documentation](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html)
 
 ## Repository / Unit of work
 
 The `SQLAlchemyRepository` and `SQLAlchemyAsyncRepository` class can be used simply by extending them.
 
 ```python
-from sqlalchemy_bind_manager import SQLAlchemyRepository
+from sqlalchemy_bind_manager.repository import SQLAlchemyRepository
 
 
 class MyModel(model_declarative_base):
     pass
 
 
 class ModelRepository(SQLAlchemyRepository[MyModel]):
@@ -233,14 +229,15 @@
 
 * `get`: Retrieve a model by identifier
 * `save`: Persist a model
 * `save_many`: Persist multiple models in a single transaction
 * `delete`: Delete a model
 * `find`: Search for a list of models (basically an adapter for SELECT queries)
 * `paginated_find`: Search for a list of models, with pagination support
+* `cursor_paginated_find`: Search for a list of models, with cursor based pagination support
 
 ### Session lifecycle in repositories
 
 [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/20/orm/session_basics.html#when-do-i-construct-a-session-when-do-i-commit-it-and-when-do-i-close-it)
 recommends we create `Session` object at the beginning of a logical operation where
 database access is potentially anticipated.
```


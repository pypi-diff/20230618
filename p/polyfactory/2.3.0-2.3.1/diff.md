# Comparing `tmp/polyfactory-2.3.0.tar.gz` & `tmp/polyfactory-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.3.0.tar", max compression
+gzip compressed data, was "polyfactory-2.3.1.tar", max compression
```

## Comparing `polyfactory-2.3.0.tar` & `polyfactory-2.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1092 2023-06-18 06:33:12.919477 polyfactory-2.3.0/LICENSE
--rw-r--r--   0        0        0     9446 2023-06-18 06:33:12.919477 polyfactory-2.3.0/README.md
--rw-r--r--   0        0        0      425 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/__init__.py
--rw-r--r--   0        0        0      772 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    32184 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2757 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1876 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     6873 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2193 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    10875 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1514 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     7413 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3328 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/fields.py
--rw-r--r--   0        0        0     1191 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/py.typed
--rw-r--r--   0        0        0     2890 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3940 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3401 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     2834 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1879 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13607 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      522 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3845 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      529 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      535 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3635 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6216 2023-06-18 06:33:12.923477 polyfactory-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 polyfactory-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-18 10:58:40.409414 polyfactory-2.3.1/LICENSE
+-rw-r--r--   0        0        0     9446 2023-06-18 10:58:40.409414 polyfactory-2.3.1/README.md
+-rw-r--r--   0        0        0      425 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/__init__.py
+-rw-r--r--   0        0        0      825 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    32143 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1876 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     6873 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2217 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    10876 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1516 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     7410 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3329 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/py.typed
+-rw-r--r--   0        0        0     2891 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-18 10:58:40.413415 polyfactory-2.3.1/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3402 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1880 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13607 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      522 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      529 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      535 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3636 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6186 2023-06-18 10:58:40.417415 polyfactory-2.3.1/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6257 2023-06-18 10:58:40.417415 polyfactory-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 polyfactory-2.3.1/PKG-INFO
```

### Comparing `polyfactory-2.3.0/LICENSE` & `polyfactory-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.0/README.md` & `polyfactory-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.0/polyfactory/constants.py` & `polyfactory-2.3.1/polyfactory/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import abc, defaultdict, deque
+from random import Random
 from typing import (
     DefaultDict,
     Deque,
     Dict,
     FrozenSet,
     Iterable,
     List,
@@ -35,7 +36,9 @@
     abc.Mapping: dict,
     abc.Sequence: list,
     abc.Set: set,
     UnionType: Union,
 }
 
 IGNORED_TYPE_ARGS: Set = {Ellipsis}
+
+DEFAULT_RANDOM = Random()
```

### Comparing `polyfactory-2.3.0/polyfactory/decorators.py` & `polyfactory-2.3.1/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.0/polyfactory/exceptions.py` & `polyfactory-2.3.1/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.0/polyfactory/factories/base.py` & `polyfactory-2.3.1/polyfactory/factories/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from collections import Counter, deque, abc
+from collections import Counter, abc, deque
 from contextlib import suppress
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from enum import EnumMeta
 from functools import partial
 from importlib import import_module
 from inspect import isclass
@@ -12,16 +13,16 @@
     IPv4Address,
     IPv4Interface,
     IPv4Network,
     IPv6Address,
     IPv6Interface,
     IPv6Network,
     ip_address,
-    ip_network,
     ip_interface,
+    ip_network,
 )
 from os.path import realpath
 from pathlib import Path
 from random import Random
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -30,55 +31,55 @@
     Generic,
     Mapping,
     Sequence,
     Type,
     TypeVar,
     cast,
 )
-from uuid import UUID, NAMESPACE_DNS, uuid3, uuid5, uuid1
+from uuid import NAMESPACE_DNS, UUID, uuid1, uuid3, uuid5
 
 from faker import Faker
 from typing_extensions import get_args
 
 from polyfactory.exceptions import (
     ConfigurationException,
     MissingBuildKwargException,
     ParameterException,
 )
 from polyfactory.fields import Fixture, Ignore, PostGenerated, Require, Use
-
 from polyfactory.utils.helpers import unwrap_annotation, unwrap_args, unwrap_optional
 from polyfactory.utils.predicates import (
     get_type_origin,
     is_literal,
     is_optional_union,
     is_safe_subclass,
 )
 from polyfactory.value_generators.complex_types import handle_complex_type
 from polyfactory.value_generators.constrained_collections import handle_constrained_collection
 from polyfactory.value_generators.constrained_dates import handle_constrained_date
 from polyfactory.value_generators.constrained_numbers import (
+    handle_constrained_decimal,
     handle_constrained_float,
     handle_constrained_int,
-    handle_constrained_decimal,
 )
 from polyfactory.value_generators.constrained_path import handle_constrained_path
 from polyfactory.value_generators.constrained_strings import handle_constrained_string_or_bytes
 from polyfactory.value_generators.constrained_url import handle_constrained_url
 from polyfactory.value_generators.constrained_uuid import handle_constrained_uuid
 from polyfactory.value_generators.primitives import (
     create_random_boolean,
     create_random_bytes,
 )
 
 if TYPE_CHECKING:
-    from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
-    from polyfactory.field_meta import FieldMeta, Constraints
     from typing_extensions import TypeGuard
 
+    from polyfactory.field_meta import Constraints, FieldMeta
+    from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
+
 
 def _create_pydantic_type_map(cls: "type[BaseFactory]") -> dict[type, Callable[[], Any]]:
     """Creates a mapping of pydantic types to mock data functions.
 
     :param cls: The base factory class.
     :return: A dict mapping types to callables.
     """
@@ -115,31 +116,28 @@
         }
 
     except ImportError:
         mapping = {}
 
     try:
         # v1 only values - these will raise an exception in v2
-        from pydantic import (
-            PyObject,
-        )
-
         # in pydantic v2 these are all aliases for Annotated with a constraint.
         # we therefore do not need them in v2
         from pydantic import (
-            AmqpDsn,
-            KafkaDsn,
-            PostgresDsn,
-            RedisDsn,
             UUID1,
             UUID3,
             UUID4,
             UUID5,
-            FilePath,
+            AmqpDsn,
             DirectoryPath,
+            FilePath,
+            KafkaDsn,
+            PostgresDsn,
+            PyObject,
+            RedisDsn,
         )
 
         mapping.update(
             {  # pyright: ignore
                 PyObject: lambda: "decimal.Decimal",
                 AmqpDsn: lambda: "amqps://example.com",
                 KafkaDsn: lambda: "kafka://localhost:9092",
```

### Comparing `polyfactory-2.3.0/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.3.1/polyfactory/factories/beanie_odm_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 from typing_extensions import get_args
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.pydantic_factory import ModelFactory
 from polyfactory.persistence import AsyncPersistenceProtocol
```

### Comparing `polyfactory-2.3.0/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.3.1/polyfactory/factories/dataclass_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
-from dataclasses import is_dataclass, fields, MISSING
+
+from dataclasses import MISSING, fields, is_dataclass
 from inspect import isclass
-from typing import Generic, Any, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Generic
 
 from typing_extensions import get_type_hints
 
-from polyfactory.factories.base import T, BaseFactory
+from polyfactory.factories.base import BaseFactory, T
 from polyfactory.field_meta import FieldMeta, Null
 
-
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
 
 class DataclassFactory(Generic[T], BaseFactory[T]):
     """Dataclass base factory"""
```

### Comparing `polyfactory-2.3.0/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.3.1/polyfactory/factories/msgspec_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime as dt
 from decimal import Decimal
 from inspect import isclass
-from typing import Any, Callable, Dict, FrozenSet, Generic, Iterable, List, Set, Tuple, TypeVar, Type, cast
+from typing import Any, Callable, Dict, FrozenSet, Generic, Iterable, List, Set, Tuple, Type, TypeVar, cast
 from uuid import UUID
 
 from typing_extensions import TypeGuard
 
 from polyfactory.exceptions import MissingDependencyException, ParameterException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import Constraints, FieldMeta
```

### Comparing `polyfactory-2.3.0/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.3.1/polyfactory/factories/odmantic_odm_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.pydantic_factory import ModelFactory
 from polyfactory.utils.predicates import is_safe_subclass
 from polyfactory.value_generators.primitives import create_random_bytes
 
 try:
     from bson.decimal128 import Decimal128, create_decimal128_context
-    from odmantic import EmbeddedModel, Model, bson as odbson
+    from odmantic import EmbeddedModel, Model
+    from odmantic import bson as odbson
 
 except ImportError as e:
     raise MissingDependencyException("odmantic is not installed") from e
 
 T = TypeVar("T", bound=Union[Model, EmbeddedModel])
 
 if TYPE_CHECKING:
```

### Comparing `polyfactory-2.3.0/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.3.1/polyfactory/factories/pydantic_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from contextlib import suppress
 from inspect import isclass
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Generic,
+    Literal,
     Mapping,
     TypeVar,
     cast,
-    Literal,
 )
 
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
-from polyfactory.field_meta import FieldMeta, Null, Constraints
+from polyfactory.field_meta import Constraints, FieldMeta, Null
 from polyfactory.utils.helpers import unwrap_new_type
 
 try:
     from pydantic import BaseModel
 
 except ImportError as e:
     raise MissingDependencyException("pydantic is not installed") from e
@@ -32,16 +32,17 @@
     pydantic_version = 2
 
     ModelField = Any
     from pydantic._internal._fields import Undefined
 
 if TYPE_CHECKING:
     from random import Random
-    from typing_extensions import TypeGuard
+
     from pydantic.fields import FieldInfo
+    from typing_extensions import TypeGuard
 
 T = TypeVar("T", bound=BaseModel)
 
 
 def is_pydantic_model(value: Any) -> "TypeGuard[type[BaseModel]]":
     """Determine whether the given value is a subclass of BaseModel.
 
@@ -116,16 +117,16 @@
 
         :param model_field: A pydantic ModelField.
         :param use_alias: Whether to use the field alias.
 
         :returns: A PydanticFieldMeta instance.
 
         """
+        from pydantic import AmqpDsn, AnyHttpUrl, AnyUrl, HttpUrl, KafkaDsn, PostgresDsn, RedisDsn
         from pydantic.fields import DeferredType, Undefined  # type: ignore
-        from pydantic import AnyUrl, HttpUrl, KafkaDsn, PostgresDsn, RedisDsn, AmqpDsn, AnyHttpUrl
 
         if callable(model_field.default_factory):
             default_value = model_field.default_factory()
         else:
             default_value = model_field.default if model_field.default is not Undefined else Null
 
         name = model_field.alias if model_field.alias and use_alias else model_field.name
```

### Comparing `polyfactory-2.3.0/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.3.1/polyfactory/factories/typed_dict_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
-from typing import TypeVar, Generic, Any
-from typing_extensions import TypeGuard, is_typeddict, _TypedDictMeta  # type: ignore[attr-defined]
+
+from typing import Any, Generic, TypeVar
+
+from typing_extensions import TypeGuard, _TypedDictMeta, is_typeddict  # type: ignore[attr-defined]
 
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import FieldMeta, Null
 
 TypedDictT = TypeVar("TypedDictT", bound=_TypedDictMeta)
```

### Comparing `polyfactory-2.3.0/polyfactory/field_meta.py` & `polyfactory-2.3.1/polyfactory/field_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING, Any, Literal, Pattern, TypedDict, cast
 
-from typing import Any, TypedDict, Pattern, TYPE_CHECKING, Literal, cast
-
-from polyfactory.constants import TYPE_MAPPING, IGNORED_TYPE_ARGS
-from polyfactory.utils.helpers import unwrap_args, unwrap_new_type, unwrap_annotated, normalize_annotation
+from polyfactory.constants import DEFAULT_RANDOM, IGNORED_TYPE_ARGS, TYPE_MAPPING
+from polyfactory.utils.helpers import normalize_annotation, unwrap_annotated, unwrap_args, unwrap_new_type
 from polyfactory.utils.predicates import is_annotated
 
 if TYPE_CHECKING:
     from random import Random
+
     from _pydecimal import Decimal
     from typing_extensions import NotRequired, Self
 
 
 class Null:
     """Sentinel class for empty values"""
 
@@ -62,15 +62,15 @@
     constraints: Constraints | None
 
     def __init__(
         self,
         *,
         name: str,
         annotation: type,
-        random: Random,
+        random: Random = DEFAULT_RANDOM,
         default: Any = Null,
         children: list[FieldMeta] | None = None,
         constraints: Constraints | None = None,
     ):
         """Create a factory field metadata instance."""
         self.annotation = annotation
         self.random = random
@@ -79,24 +79,23 @@
         self.name = name
         self.constraints = constraints
 
     @property
     def type_args(self) -> tuple[Any, ...]:
         """Return the normalized type args of the annotation, if any.
 
-        :param random: An instance of random.Random.
         :returns: a tuple of types.
         """
         return tuple(arg for arg in unwrap_args(self.annotation, random=self.random) if arg not in IGNORED_TYPE_ARGS)
 
     @classmethod
     def from_type(
         cls,
         annotation: Any,
-        random: Random,
+        random: Random = DEFAULT_RANDOM,
         name: str = "",
         default: Any = Null,
         constraints: Constraints | None = None,
     ) -> Self:
         """Builder method to create a FieldMeta from a type annotation.
 
         :param annotation: A type annotation.
@@ -147,16 +146,16 @@
                 ("max_items", (annotated_types.MaxLen, annotated_types.Len)),
             ]
         except ImportError:
             annotated_types_meta_data = []
 
         try:
             from pydantic import UrlConstraints
-            from pydantic.types import UuidVersion, PathType
             from pydantic._internal._fields import PydanticGeneralMetadata
+            from pydantic.types import PathType, UuidVersion
 
             pydantic_annotated_meta_data = [
                 ("pattern", PydanticGeneralMetadata),
                 ("max_digits", PydanticGeneralMetadata),
                 ("decimal_places", PydanticGeneralMetadata),
                 # pydantic 2 only constraints
                 ("strict", PydanticGeneralMetadata),
```

### Comparing `polyfactory-2.3.0/polyfactory/fields.py` & `polyfactory-2.3.1/polyfactory/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
-from typing import Any, Callable, Generic, TypeVar, cast, TypedDict
+
+from typing import Any, Callable, Generic, TypedDict, TypeVar, cast
 
 from typing_extensions import ParamSpec
 
 from polyfactory.exceptions import ParameterException
 
 T = TypeVar("T")
 P = ParamSpec("P")
```

### Comparing `polyfactory-2.3.0/polyfactory/persistence.py` & `polyfactory-2.3.1/polyfactory/persistence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from typing import Protocol, TypeVar, runtime_checkable
 
 T = TypeVar("T")
 
 
 @runtime_checkable
 class SyncPersistenceProtocol(Protocol[T]):
```

### Comparing `polyfactory-2.3.0/polyfactory/pytest_plugin.py` & `polyfactory-2.3.1/polyfactory/pytest_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 import re
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Literal,
```

### Comparing `polyfactory-2.3.0/polyfactory/utils/helpers.py` & `polyfactory-2.3.1/polyfactory/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import sys
-from typing import Any, get_args, TYPE_CHECKING, get_origin
+from typing import TYPE_CHECKING, Any, get_args, get_origin
+
 from polyfactory.constants import TYPE_MAPPING
 from polyfactory.utils.predicates import (
     is_annotated,
     is_new_type,
     is_optional_union,
     is_union,
 )
```

### Comparing `polyfactory-2.3.0/polyfactory/utils/predicates.py` & `polyfactory-2.3.1/polyfactory/utils/predicates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 import sys
 from inspect import isclass
 from typing import Any, Literal, NewType, Optional, TypeVar, Union, get_args
 
 from typing_extensions import (
     Annotated,
     NotRequired,
```

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/complex_types.py` & `polyfactory-2.3.1/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.3.1/polyfactory/value_generators/constrained_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from typing import TYPE_CHECKING, Any, Callable, TypeVar
 
 from polyfactory.exceptions import ParameterException
 
 if TYPE_CHECKING:
     from polyfactory.factories.base import BaseFactory
     from polyfactory.field_meta import FieldMeta
```

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.3.1/polyfactory/value_generators/constrained_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
-from datetime import date, timedelta, datetime, timezone
-from typing import TYPE_CHECKING, cast
 
+from datetime import date, datetime, timedelta, timezone
+from typing import TYPE_CHECKING, cast
 
 if TYPE_CHECKING:
     from faker import Faker
 
 
 def handle_constrained_date(
     faker: Faker,
```

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.3.1/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/constrained_path.py` & `polyfactory-2.3.1/polyfactory/value_generators/constrained_path.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.3.1/polyfactory/value_generators/constrained_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from typing import TYPE_CHECKING, Callable, Pattern, TypeVar, Union, cast
 
 from polyfactory.exceptions import ParameterException
 from polyfactory.value_generators.primitives import create_random_bytes, create_random_string
 from polyfactory.value_generators.regex import RegexFactory
 
 T = TypeVar("T", bound=Union[bytes, str])
```

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/constrained_url.py` & `polyfactory-2.3.1/polyfactory/value_generators/constrained_url.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/constrained_uuid.py` & `polyfactory-2.3.1/polyfactory/value_generators/constrained_uuid.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Literal, cast
-from uuid import uuid1, uuid3, NAMESPACE_DNS, uuid5, UUID
+from uuid import NAMESPACE_DNS, UUID, uuid1, uuid3, uuid5
 
 from faker import Faker
 
 
 # FIXME: remove the pragma when switching to pydantic v2 permanently
 def handle_constrained_uuid(uuid_version: Literal[1, 3, 4, 5], faker: Faker) -> UUID:  # pragma: no cover
     if uuid_version == 1:
```

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/primitives.py` & `polyfactory-2.3.1/polyfactory/value_generators/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from binascii import hexlify
 from decimal import Decimal
 from os import urandom
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from random import Random
```

### Comparing `polyfactory-2.3.0/polyfactory/value_generators/regex.py` & `polyfactory-2.3.1/polyfactory/value_generators/regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 from __future__ import annotations
+
 from itertools import chain
 from string import (
     ascii_letters,
     ascii_lowercase,
     ascii_uppercase,
     digits,
     printable,
```

### Comparing `polyfactory-2.3.0/pyproject.toml` & `polyfactory-2.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.3.0"
+version = "2.3.1"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -122,46 +122,48 @@
     'except ImportError as e:',
     '\.\.\.'
 ]
 
 [tool.ruff]
 select = [
     "A", # flake8-builtins
-    "B", # flake8-bugbear
+    "B",   # flake8-bugbear
     "BLE", # flake8-blind-except
-    "C4", # flake8-comprehensions
-    "D", # pydocstyle
-    "DJ", # flake8-django
+    "C4",  # flake8-comprehensions
+    "D",   # pydocstyle
+    "DJ",  # flake8-django
     "DTZ", # flake8-datetimez
-    "E", # pycodestyle errors
+    "E",   # pycodestyle errors
     "ERA", # eradicate
     "EXE", # flake8-executable
-    "F", # pyflakes
-    "G", # flake8-logging-format
+    "F",   # pyflakes
+    "G",   # flake8-logging-format
+    "I",   # isort
     "ICN", # flake8-import-conventions
     "ISC", # flake8-implicit-str-concat
-    "N", # pep8-naming
+    "N",   # pep8-naming
     "PIE", # flake8-pie
     "PLC", # pylint - convention
     "PLE", # pylint - error
     "PLW", # pylint - warning
     "PTH", # flake8-use-pathlib
-    "Q", # flake8-quotes
+    "Q",   # flake8-quotes
     "RET", # flake8-return
     "RUF", # Ruff-specific rules
-    "S", # flake8-bandit
+    "S",   # flake8-bandit
     "SIM", # flake8-simplify
     "T10", # flake8-debugger
     "T20", # flake8-print
     "TCH", # flake8-type-checking
     "TID", # flake8-tidy-imports
-    "UP", # pyupgrade
-    "W", # pycodestyle - warning
+    "UP",  # pyupgrade
+    "W",   # pycodestyle - warning
     "YTT", # flake8-2020
 ]
+
 ignore = [
     "A003", # flake8-builtins - class attribute {name} is shadowing a python builtin
     "B010", # flake8-bugbear - do not call setattr with a constant attribute value
     "D100", # pydocstyle - missing docstring in public module
     "D101", # pydocstyle - missing docstring in public class
     "D102", # pydocstyle - missing docstring in public method
     "D103", # pydocstyle - missing docstring in public function
```

### Comparing `polyfactory-2.3.0/PKG-INFO` & `polyfactory-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.3.0
+Version: 2.3.1
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
```


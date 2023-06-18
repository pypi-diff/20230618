# Comparing `tmp/polyfactory-2.2.0.tar.gz` & `tmp/polyfactory-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.2.0.tar", max compression
+gzip compressed data, was "polyfactory-2.3.0.tar", max compression
```

## Comparing `polyfactory-2.2.0.tar` & `polyfactory-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0     1092 2023-05-29 16:14:20.435754 polyfactory-2.2.0/LICENSE
--rw-r--r--   0        0        0     9446 2023-05-29 16:14:20.435754 polyfactory-2.2.0/README.md
--rw-r--r--   0        0        0      425 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/__init__.py
--rw-r--r--   0        0        0      642 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    30734 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2757 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1603 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     6812 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2193 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0     7552 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1471 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     2939 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3328 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/fields.py
--rw-r--r--   0        0        0     1191 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/py.typed
--rw-r--r--   0        0        0     2890 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3401 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     2807 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1838 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13431 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0     3845 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0     3635 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6177 2023-05-29 16:14:20.439754 polyfactory-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 polyfactory-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-18 06:33:12.919477 polyfactory-2.3.0/LICENSE
+-rw-r--r--   0        0        0     9446 2023-06-18 06:33:12.919477 polyfactory-2.3.0/README.md
+-rw-r--r--   0        0        0      425 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/__init__.py
+-rw-r--r--   0        0        0      772 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    32184 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2757 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1876 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     6873 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2193 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    10875 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1514 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     7413 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3328 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/fields.py
+-rw-r--r--   0        0        0     1191 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/py.typed
+-rw-r--r--   0        0        0     2890 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3940 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3401 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1879 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13607 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      522 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3845 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      529 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      535 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3635 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6185 2023-06-18 06:33:12.923477 polyfactory-2.3.0/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6216 2023-06-18 06:33:12.923477 polyfactory-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 polyfactory-2.3.0/PKG-INFO
```

### Comparing `polyfactory-2.2.0/LICENSE` & `polyfactory-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/README.md` & `polyfactory-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/constants.py` & `polyfactory-2.3.0/polyfactory/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,16 +6,23 @@
     FrozenSet,
     Iterable,
     List,
     Mapping,
     Sequence,
     Set,
     Tuple,
+    Union,
 )
 
+try:
+    from types import UnionType
+except ImportError:
+    UnionType = Union  # type: ignore
+
+
 # Mapping of type annotations into concrete types. This is used to normalize python <= 3.9 annotations.
 TYPE_MAPPING = {
     DefaultDict: defaultdict,
     Deque: deque,
     Dict: dict,
     FrozenSet: frozenset,
     Iterable: list,
@@ -24,10 +31,11 @@
     Sequence: list,
     Set: set,
     Tuple: tuple,
     abc.Iterable: list,
     abc.Mapping: dict,
     abc.Sequence: list,
     abc.Set: set,
+    UnionType: Union,
 }
 
 IGNORED_TYPE_ARGS: Set = {Ellipsis}
```

### Comparing `polyfactory-2.2.0/polyfactory/decorators.py` & `polyfactory-2.3.0/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/exceptions.py` & `polyfactory-2.3.0/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/factories/base.py` & `polyfactory-2.3.0/polyfactory/factories/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from collections import Counter, deque
+from collections import Counter, deque, abc
 from contextlib import suppress
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from enum import EnumMeta
 from functools import partial
 from importlib import import_module
 from inspect import isclass
@@ -30,15 +30,15 @@
     Generic,
     Mapping,
     Sequence,
     Type,
     TypeVar,
     cast,
 )
-from uuid import NAMESPACE_DNS, UUID, uuid1, uuid3, uuid5
+from uuid import UUID, NAMESPACE_DNS, uuid3, uuid5, uuid1
 
 from faker import Faker
 from typing_extensions import get_args
 
 from polyfactory.exceptions import (
     ConfigurationException,
     MissingBuildKwargException,
@@ -57,15 +57,18 @@
 from polyfactory.value_generators.constrained_collections import handle_constrained_collection
 from polyfactory.value_generators.constrained_dates import handle_constrained_date
 from polyfactory.value_generators.constrained_numbers import (
     handle_constrained_float,
     handle_constrained_int,
     handle_constrained_decimal,
 )
+from polyfactory.value_generators.constrained_path import handle_constrained_path
 from polyfactory.value_generators.constrained_strings import handle_constrained_string_or_bytes
+from polyfactory.value_generators.constrained_url import handle_constrained_url
+from polyfactory.value_generators.constrained_uuid import handle_constrained_uuid
 from polyfactory.value_generators.primitives import (
     create_random_boolean,
     create_random_bytes,
 )
 
 if TYPE_CHECKING:
     from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
@@ -78,56 +81,95 @@
 
     :param cls: The base factory class.
     :return: A dict mapping types to callables.
     """
     try:
         import pydantic
 
-        return {
+        mapping = {
             pydantic.ByteSize: cls.__faker__.pyint,
             pydantic.PositiveInt: cls.__faker__.pyint,
-            pydantic.FilePath: lambda: Path(realpath(__file__)),
             pydantic.NegativeFloat: lambda: cls.__random__.uniform(-100, -1),
             pydantic.NegativeInt: lambda: cls.__faker__.pyint() * -1,
             pydantic.PositiveFloat: cls.__faker__.pyint,
             pydantic.NonPositiveFloat: lambda: cls.__random__.uniform(-100, 0),
             pydantic.NonNegativeInt: cls.__faker__.pyint,
             pydantic.StrictInt: cls.__faker__.pyint,
             pydantic.StrictBool: cls.__faker__.pybool,
             pydantic.StrictBytes: partial(create_random_bytes, cls.__random__),
             pydantic.StrictFloat: cls.__faker__.pyfloat,
             pydantic.StrictStr: cls.__faker__.pystr,
-            pydantic.DirectoryPath: lambda: Path(realpath(__file__)).parent,
             pydantic.EmailStr: cls.__faker__.free_email,
             pydantic.NameEmail: cls.__faker__.free_email,
-            pydantic.PyObject: lambda: "decimal.Decimal",  # type: ignore[dict-item]
-            pydantic.color.Color: cls.__faker__.hex_color,  # pyright: ignore
             pydantic.Json: cls.__faker__.json,
             pydantic.PaymentCardNumber: cls.__faker__.credit_card_number,
             pydantic.AnyUrl: cls.__faker__.url,
             pydantic.AnyHttpUrl: cls.__faker__.url,
             pydantic.HttpUrl: cls.__faker__.url,
-            pydantic.PostgresDsn: lambda: "postgresql://user:secret@localhost",
-            pydantic.RedisDsn: lambda: "redis://localhost:6379",
-            pydantic.UUID1: uuid1,
-            pydantic.UUID3: lambda: uuid3(NAMESPACE_DNS, cls.__faker__.pystr()),
-            pydantic.UUID4: cls.__faker__.uuid4,
-            pydantic.UUID5: lambda: uuid5(NAMESPACE_DNS, cls.__faker__.pystr()),
             pydantic.SecretBytes: partial(create_random_bytes, cls.__random__),
             pydantic.SecretStr: cls.__faker__.pystr,
             pydantic.IPvAnyAddress: cls.__faker__.ipv4,
             pydantic.IPvAnyInterface: cls.__faker__.ipv4,
             pydantic.IPvAnyNetwork: lambda: cls.__faker__.ipv4(network=True),
-            pydantic.AmqpDsn: lambda: "amqps://",
-            pydantic.KafkaDsn: lambda: "kafka://",
             pydantic.PastDate: cls.__faker__.past_date,
             pydantic.FutureDate: cls.__faker__.future_date,
         }
+
+    except ImportError:
+        mapping = {}
+
+    try:
+        # v1 only values - these will raise an exception in v2
+        from pydantic import (
+            PyObject,
+        )
+
+        # in pydantic v2 these are all aliases for Annotated with a constraint.
+        # we therefore do not need them in v2
+        from pydantic import (
+            AmqpDsn,
+            KafkaDsn,
+            PostgresDsn,
+            RedisDsn,
+            UUID1,
+            UUID3,
+            UUID4,
+            UUID5,
+            FilePath,
+            DirectoryPath,
+        )
+
+        mapping.update(
+            {  # pyright: ignore
+                PyObject: lambda: "decimal.Decimal",
+                AmqpDsn: lambda: "amqps://example.com",
+                KafkaDsn: lambda: "kafka://localhost:9092",
+                PostgresDsn: lambda: "postgresql://user:secret@localhost",
+                RedisDsn: lambda: "redis://localhost:6379/0",
+                FilePath: lambda: Path(realpath(__file__)),
+                DirectoryPath: lambda: Path(realpath(__file__)).parent,
+                UUID1: uuid1,
+                UUID3: lambda: uuid3(NAMESPACE_DNS, cls.__faker__.pystr()),
+                UUID4: cls.__faker__.uuid4,
+                UUID5: lambda: uuid5(NAMESPACE_DNS, cls.__faker__.pystr()),
+            }
+        )
+
     except ImportError:
-        return {}
+        pass
+
+    try:
+        # this might be removed by pydantic 2
+        from pydantic import color
+
+        mapping[color.Color] = cls.__faker__.hex_color  # pyright: ignore
+    except ImportError:
+        pass
+
+    return mapping
 
 
 T = TypeVar("T")
 
 
 def is_factory(value: Any) -> "TypeGuard[type[BaseFactory]]":
     """Determine if a given value is a subclass of ModelFactory.
@@ -312,15 +354,15 @@
     def is_batch_factory_type(cls, annotation: Any) -> bool:
         """Determine whether a given field is annotated with a sequence of supported factory types.
 
         :param annotation: A type annotation.
         :returns: Boolean dictating whether the annotation is a batch factory type
         """
         origin = get_type_origin(annotation) or annotation
-        if is_safe_subclass(origin, Sequence) and (args := unwrap_args(annotation)):  # type: ignore
+        if is_safe_subclass(origin, Sequence) and (args := unwrap_args(annotation, random=cls.__random__)):  # type: ignore
             return len(args) == 1 and BaseFactory.is_factory_type(annotation=args[0])
         return False
 
     @classmethod
     def extract_field_build_parameters(cls, field_meta: FieldMeta, build_args: dict[str, Any]) -> Any:
         """Extract from the build kwargs any build parameters passed for a given field meta - if it is a factory type.
 
@@ -426,14 +468,15 @@
             IPv4Interface: lambda: ip_interface(cls.__faker__.ipv4()),
             IPv4Network: lambda: ip_network(cls.__faker__.ipv4(network=True)),
             IPv6Address: lambda: ip_address(cls.__faker__.ipv6()),
             IPv6Interface: lambda: ip_interface(cls.__faker__.ipv6()),
             IPv6Network: lambda: ip_network(cls.__faker__.ipv6(network=True)),
             # types
             Callable: _create_generic_fn,
+            abc.Callable: _create_generic_fn,
             Counter: lambda: Counter(cls.__faker__.pystr()),
             **_create_pydantic_type_map(cls),
         }
 
     @classmethod
     def get_mock_value(cls, annotation: type) -> Any:
         """Return a mock value for a given type.
@@ -513,14 +556,17 @@
                 multiple_of=cast("Any", constraints.get("multiple_of")),
                 gt=cast("Any", constraints.get("gt")),
                 ge=cast("Any", constraints.get("ge")),
                 lt=cast("Any", constraints.get("lt")),
                 le=cast("Any", constraints.get("le")),
             )
 
+        if url_constraints := constraints.get("url"):
+            return handle_constrained_url(constraints=url_constraints)
+
         if is_safe_subclass(annotation, str) or is_safe_subclass(annotation, bytes):
             return handle_constrained_string_or_bytes(
                 random=cls.__random__,
                 t_type=str if is_safe_subclass(annotation, str) else bytes,
                 lower_case=constraints.get("lower_case") or False,
                 upper_case=constraints.get("upper_case") or False,
                 min_length=constraints.get("min_length"),
@@ -559,14 +605,23 @@
                 faker=cls.__faker__,
                 ge=cast("Any", constraints.get("ge")),
                 gt=cast("Any", constraints.get("gt")),
                 le=cast("Any", constraints.get("le")),
                 lt=cast("Any", constraints.get("lt")),
             )
 
+        if is_safe_subclass(annotation, UUID) and (uuid_version := constraints.get("uuid_version")):
+            return handle_constrained_uuid(
+                uuid_version=uuid_version,
+                faker=cls.__faker__,
+            )
+
+        if is_safe_subclass(annotation, Path) and (path_constraint := constraints.get("path_type")):
+            return handle_constrained_path(constraint=path_constraint, faker=cls.__faker__)
+
         raise ParameterException(f"received constraints for unsupported type {annotation}")
 
     @classmethod
     def get_field_value(cls, field_meta: FieldMeta, field_build_parameters: Any | None = None) -> Any:
         """Return a field value on the subclass if existing, otherwise returns a mock value.
 
         :param field_meta: FieldMeta instance.
@@ -580,26 +635,23 @@
 
         if field_meta.constraints and field_meta.constraints.get("constant", False):
             return field_meta.default
 
         if cls.should_set_none_value(field_meta=field_meta):
             return None
 
-        unwrapped_annotation = unwrap_annotation(field_meta.annotation)
+        unwrapped_annotation = unwrap_annotation(field_meta.annotation, random=cls.__random__)
 
         if is_literal(annotation=unwrapped_annotation) and (literal_args := get_args(unwrapped_annotation)):
             return cls.__random__.choice(literal_args)
 
         if isinstance(unwrapped_annotation, EnumMeta):
             return cls.__random__.choice(list(unwrapped_annotation))  # pyright: ignore
 
-        if field_meta.constraints and (
-            unwrapped_annotation in (float, int, Decimal, bytes, str, list, tuple, set, frozenset, date)
-            or unwrapped_annotation not in cls.get_provider_map()
-        ):
+        if field_meta.constraints:
             return cls.get_constrained_field_value(annotation=unwrapped_annotation, field_meta=field_meta)
 
         if BaseFactory.is_factory_type(annotation=unwrapped_annotation):
             return cls._get_or_create_factory(model=unwrapped_annotation).build(
                 **(field_build_parameters if isinstance(field_build_parameters, Mapping) else {})
             )
```

### Comparing `polyfactory-2.2.0/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.3.0/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.3.0/polyfactory/factories/dataclass_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from dataclasses import is_dataclass, fields, MISSING
 from inspect import isclass
 from typing import Generic, Any, TYPE_CHECKING
 
+from typing_extensions import get_type_hints
 
 from polyfactory.factories.base import T, BaseFactory
 from polyfactory.field_meta import FieldMeta, Null
 
 
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
@@ -35,18 +36,27 @@
 
 
         :returns: A list of field MetaData instances.
 
         """
         fields_meta: list["FieldMeta"] = []
 
+        model_type_hints = get_type_hints(cls.__model__)
+
         for field in fields(cls.__model__):  # type: ignore[arg-type]
             if field.default_factory and field.default_factory is not MISSING:
                 default_value = field.default_factory()
             elif field.default is not MISSING:
                 default_value = field.default
             else:
                 default_value = Null
 
-            fields_meta.append(FieldMeta.from_type(annotation=field.type, name=field.name, default=default_value))
+            fields_meta.append(
+                FieldMeta.from_type(
+                    annotation=model_type_hints[field.name],
+                    name=field.name,
+                    default=default_value,
+                    random=cls.__random__,
+                )
+            )
 
         return fields_meta
```

### Comparing `polyfactory-2.2.0/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.3.0/polyfactory/factories/msgspec_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,17 @@
             if isinstance(field_type, inspect.StrType):
                 constraint_names.append("pattern")
             constraints = cls.get_constraints(field_type, constraint_names)
 
         if isinstance(field_type, (inspect.DateTimeType, inspect.TimeType)) and field_type.tz is not None:
             raise ParameterException(f"received constraints for unsupported type {annotation}")
 
-        return FieldMeta.from_type(annotation, field.name, constraints=constraints)
+        return FieldMeta.from_type(
+            annotation=annotation, name=field.name, constraints=constraints, random=cls.__random__
+        )
 
     @classmethod
     def get_provider_map(cls) -> Dict[Any, Callable[[], Any]]:
         def get_msgpack_ext() -> msgspec.msgpack.Ext:
             code = handle_constrained_int(cls.__random__, ge=-128, le=127)
             data = create_random_bytes(cls.__random__)
             return msgspec.msgpack.Ext(code, data)
```

### Comparing `polyfactory-2.2.0/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.3.0/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.3.0/polyfactory/factories/typed_dict_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,12 +35,13 @@
         """
         fields_meta: list["FieldMeta"] = []
 
         for field_name, annotation in cls.__model__.__annotations__.items():
             fields_meta.append(
                 FieldMeta.from_type(
                     annotation=annotation,
+                    random=cls.__random__,
                     name=field_name,
                     default=getattr(cls.__model__, field_name, Null),
                 )
             )
         return fields_meta
```

### Comparing `polyfactory-2.2.0/polyfactory/fields.py` & `polyfactory-2.3.0/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/persistence.py` & `polyfactory-2.3.0/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/pytest_plugin.py` & `polyfactory-2.3.0/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/utils/predicates.py` & `polyfactory-2.3.0/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/value_generators/complex_types.py` & `polyfactory-2.3.0/polyfactory/value_generators/complex_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     of pydantic field_metas.
 
     :param field_meta: A field meta instance.
     :param factory: A factory.
 
     :returns: A built result.
     """
-    if origin := get_type_origin(unwrap_annotation(field_meta.annotation)):
+    if origin := get_type_origin(unwrap_annotation(field_meta.annotation, random=factory.__random__)):
         if issubclass(origin, Collection):
             return handle_collection_type(field_meta, origin, factory)
         return factory.get_mock_value(origin)
 
     if is_union(field_meta.annotation) and field_meta.children:
         return factory.get_field_value(factory.__random__.choice(field_meta.children))
```

### Comparing `polyfactory-2.2.0/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.3.0/polyfactory/value_generators/constrained_collections.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,24 +27,25 @@
     :param item_type: Type of the collection items.
     :param max_items: Maximal number of items.
     :param min_items: Minimal number of items.
     :param unique_items: Whether the items should be unique.
 
     :returns: A collection value.
     """
-    min_items = min_items if min_items is not None else (max_items or 0)
-    max_items = max_items if max_items is not None else min_items + 1
+    min_items = abs(min_items if min_items is not None else (max_items or 0))
+    max_items = abs(max_items if max_items is not None else min_items + 1)
 
     if max_items < min_items:
         raise ParameterException("max_items must be larger or equal to min_items")
 
-    collection: set[T] | list[T] = set() if collection_type in (frozenset, set) or unique_items else []
+    collection: set[T] | list[T] = set() if (collection_type in (frozenset, set) or unique_items) else []
 
     try:
-        while len(collection) < factory.__random__.randint(min_items, max_items):
+        length = factory.__random__.randint(min_items, max_items) or 1
+        while len(collection) < length:
             value = factory.get_field_value(field_meta)
             if isinstance(collection, set):
                 collection.add(value)
             else:
                 collection.append(value)
         return collection_type(collection)
     except TypeError as e:
```

### Comparing `polyfactory-2.2.0/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.3.0/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.3.0/polyfactory/value_generators/constrained_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
+
 from decimal import Decimal
 from sys import float_info
 from typing import TYPE_CHECKING, Any, Protocol, TypeVar, cast
 
 from polyfactory.exceptions import ParameterException
 from polyfactory.value_generators.primitives import create_random_decimal, create_random_float, create_random_integer
 
 if TYPE_CHECKING:
     from random import Random
 
-
 T = TypeVar("T", Decimal, int, float)
 
 
 class NumberGeneratorProtocol(Protocol[T]):
     """Protocol for custom callables used to generate numerical values"""
 
     def __call__(self, random: "Random", minimum: T | None = None, maximum: T | None = None) -> T:
@@ -125,28 +125,43 @@
         int: 1,
         float: float_info.epsilon,
         Decimal: Decimal("0.001"),
     }
     return cast("T", values[t_type])
 
 
-def get_value_or_none(equal_value: T | None, constrained: T | None, increment: T) -> T | None:
+def get_value_or_none(
+    t_type: type[T],
+    lt: T | None = None,
+    le: T | None = None,
+    gt: T | None = None,
+    ge: T | None = None,
+) -> tuple[T | None, T | None]:
     """Return an optional value.
 
     :param equal_value: An GE/LE value.
     :param constrained: An GT/LT value.
     :param increment: increment
 
     :returns: Optional T.
     """
-    if equal_value is not None:
-        return equal_value
-    if constrained is not None:
-        return constrained + increment
-    return None
+    if ge is not None:
+        minimum_value = ge
+    elif gt is not None:
+        minimum_value = gt + get_increment(t_type)
+    else:
+        minimum_value = None
+
+    if le is not None:
+        maximum_value = le
+    elif lt is not None:
+        maximum_value = lt - get_increment(t_type)
+    else:
+        maximum_value = None
+    return minimum_value, maximum_value
 
 
 def get_constrained_number_range(
     t_type: type[T],
     random: Random,
     lt: T | None = None,
     le: T | None = None,
@@ -163,16 +178,15 @@
     :param gt: Greater than value.
     :param ge: Greater than or equal value.
     :param multiple_of: Multiple of value.
 
     :returns: a tuple of optional minimum and maximum values.
     """
     seed = t_type(random.random() * 10)
-    minimum = get_value_or_none(equal_value=ge, constrained=gt, increment=get_increment(t_type))
-    maximum = get_value_or_none(equal_value=le, constrained=lt, increment=-get_increment(t_type))  # pyright: ignore
+    minimum, maximum = get_value_or_none(lt=lt, le=le, gt=gt, ge=ge, t_type=t_type)
 
     if minimum is not None and maximum is not None and maximum < minimum:
         raise ParameterException("maximum value must be greater than minimum value")
 
     if multiple_of is None:
         if minimum is not None and maximum is None:
             if minimum == 0:
```

### Comparing `polyfactory-2.2.0/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.3.0/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/value_generators/primitives.py` & `polyfactory-2.3.0/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/polyfactory/value_generators/regex.py` & `polyfactory-2.3.0/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.2.0/pyproject.toml` & `polyfactory-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.2.0"
+version = "2.3.0"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -191,10 +191,11 @@
     "sqlalchemy.ext.declarative.declared_attr",
 ]
 
 [tool.ruff.isort]
 known-first-party = ["polyfactory", "tests"]
 
 [tool.ruff.per-file-ignores]
+"polyfactory/field_meta.py" = ["N806"]
 "tests/**/*.*" = ["S101", "D", "ARG", "PGH", "B", "FBT", "PTH", "A", "TCH", "DTZ", "TRY", "EM", "S", "N", "SIM", "PLR", "BLE", "RSE", "C901", "PLW", "G", "PIE"]
 "docs/examples/tests/**/*.*" = ["S101", "D", "ARG", "PGH", "B", "FBT", "PTH", "A", "TCH", "DTZ", "TRY", "EM", "S", "N", "SIM", "PLR", "BLE", "RSE", "C901", "PLW", "G", "PIE"]
 "docs/**/*.*" = ["S", "B", "DTZ", "A", "TCH", "ERA", "D", "RET", "E731"]
```

### Comparing `polyfactory-2.2.0/PKG-INFO` & `polyfactory-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.2.0
+Version: 2.3.0
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
```


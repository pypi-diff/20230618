# Comparing `tmp/dup_fmt-0.0.3.tar.gz` & `tmp/dup_fmt-0.0.3.post1.tar.gz`

## Comparing `dup_fmt-0.0.3.tar` & `dup_fmt-0.0.3.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/.bumpversion.cfg
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/__about__.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/cli.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/exceptions.py
--rw-r--r--   0        0        0    74758 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/formatter.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_errors.py
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_datetime.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_group.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_naming.py
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_order.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_serial.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_version.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_ralativeserial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/examples/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/examples/test_formatter_datetime.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/examples/test_formatter_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/perfs/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/perfs/perf_fomatter_datetime.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/LICENSE
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/README.md
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/CONTRIBUTING.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/dup_fmt/__about__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/dup_fmt/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/dup_fmt/cli.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/dup_fmt/exceptions.py
+-rw-r--r--   0        0        0    76983 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/dup_fmt/formatter.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/dup_fmt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_errors.py
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_formatter.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_formatter_datetime.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_formatter_group.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_formatter_naming.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_formatter_order.py
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_formatter_serial.py
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_formatter_version.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/test_ralativeserial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/examples/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/examples/test_formatter_datetime.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/examples/test_formatter_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/perfs/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/tests/perfs/perf_fomatter_datetime.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/LICENSE
+-rw-r--r--   0        0        0     9531 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/README.md
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/pyproject.toml
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 dup_fmt-0.0.3.post1/PKG-INFO
```

### Comparing `dup_fmt-0.0.3/.bumpversion.cfg` & `dup_fmt-0.0.3.post1/.bumpversion.cfg`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/CONTRIBUTING.md` & `dup_fmt-0.0.3.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/dup_fmt/exceptions.py` & `dup_fmt-0.0.3.post1/dup_fmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/dup_fmt/formatter.py` & `dup_fmt-0.0.3.post1/dup_fmt/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # --------------------------------------------------------------------------
+# mypy: disable-error-code="attr-defined"
 """
 The main object of formatter is able to format every thing you want by less
 config when inherit base class.
 """
 from __future__ import annotations
 
 import re
+from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from functools import lru_cache, partial, reduce, total_ordering
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Literal,
     Optional,
     Tuple,
     Type,
     TypedDict,
-    TypeVar,
     Union,
 )
 
 # TODO: Review ``semver`` package instead ``packaging``.
 #  docs: https://pypi.org/project/semver/
 import packaging.version as pck_version
 from dateutil.relativedelta import relativedelta
@@ -36,14 +37,45 @@
     FormatterArgumentError,
     FormatterKeyError,
     FormatterTypeError,
     FormatterValueError,
 )
 from dup_fmt.utils import caller, concat, itself, remove_pad
 
+FormatterType = Type["Formatter"]
+PriorityCallable = Union[Callable[[Any], Any], Callable[[], Any], partial]
+FormatterCallable = Union[Callable[[], Any], partial]
+
+ConstantType = Type["__BaseConstant"]
+
+
+class PriorityValue(TypedDict):
+    """Type Dictionary for value of mapping of ``cls.priorities``"""
+
+    value: PriorityCallable
+    level: Optional[Union[int, Tuple[int, ...]]]
+
+
+class CRegexValue(TypedDict):
+    """Type Dictionary for value of mapping of ``cls.formatter``"""
+
+    value: Union[FormatterCallable, str]
+    cregex: str
+
+
+class RegexValue(TypedDict):
+    """Type Dictionary for value of mapping of ``cls.formatter``"""
+
+    value: Union[FormatterCallable, str]
+    regex: str
+
+
+PropPrioritiesType = Dict[str, PriorityValue]
+PropFormattersType = Dict[str, Union[CRegexValue, RegexValue]]
+
 
 @total_ordering
 class SlotLevel:
     """Slot level object for order priority values. This was mean if
     you implement this slot level object to attribute on your class
     and update level to an instance when it has some action, it will
     be make the level more than another instance.
@@ -63,15 +95,15 @@
     """
 
     __slots__ = (
         "level",
         "slot",
     )
 
-    def __init__(self, level: int):
+    def __init__(self, level: int) -> None:
         """Main initialize of the slot object that define a slot list
         with level input value length of False.
         """
         self.level: int = level
         self.slot: List[bool] = [False] * level
 
     def __repr__(self) -> str:
@@ -106,30 +138,33 @@
         :rtype: int
         :return: a sum of weighted value from a True value in any slot
             position.
         """
         return sum(x[0] * int(x[1]) for x in enumerate(self.slot, start=1))
 
     def update(
-        self, numbers: Union[int, Tuple[int, ...]], strict: bool = True
+        self,
+        numbers: Optional[Union[int, Tuple[int, ...]]] = None,
+        strict: bool = True,
     ) -> SlotLevel:
         """Update value in slot from False to True
 
         :param numbers: updated numbers of this SlotLevel object.
         :type numbers: Union[int, tuple]
         :param strict: a strict flag for raise error when pass out of
             range numbers.
         :type strict: bool(=True)
 
         :raises ValueError: if updated number does not exist in range.
 
         :rtype: SlotLevel
         :return: Self that was updated level
         """
-        for num in SlotLevel.make_tuple(numbers):
+        _numbers: Union[int, Tuple[int, ...]] = numbers or (0,)
+        for num in SlotLevel.make_tuple(_numbers):
             if num == 0:
                 continue
             elif 0 <= (_num := (num - 1)) <= (self.level - 1):
                 self.slot[_num] = True
                 continue
             if strict:
                 raise FormatterValueError(
@@ -147,26 +182,32 @@
         :type value: Union[int, tuple]
 
         :rtype: tuple
         """
         return (value,) if isinstance(value, int) else value
 
 
-@dataclass
+@dataclass(frozen=True)
 class PriorityData:
     """Priority Data class"""
 
-    value: Callable = field(default=itself, repr=False)
-    level: Union[int, Tuple[int, ...]] = field(default=(0,))
+    value: PriorityCallable = field(default=itself, repr=False)
+    level: Optional[Union[int, Tuple[int, ...]]] = field(default=(0,))
+
+
+class MetaFormatter(metaclass=ABCMeta):
+    """Metaclass Formatter object"""
+
+    __slots__: Tuple[str, ...] = ()
 
 
 @total_ordering
-class BaseFormatter:
-    """Base formatter object for inherit to any formatter subclass that define
-    format and parse method. The bese class will implement necessary
+class Formatter(MetaFormatter):
+    """Formatter object for inherit to any formatter subclass that define
+    format and parse method. The base class will implement necessary
     properties and method for subclass that should implement or enhance such
     as `the cls.formatter()` method or the `cls.priorities` property.
 
     :param formats: A mapping value of attributes
     :type formats: Optional[dict](=None)
 
     .. class attributes::
@@ -194,51 +235,55 @@
 
         This class is abstract class for any formatter object. It will raise
     `NotImplementedError` when the necessary attributes and methods does not
     implement from subclass.
     """
 
     # This value must reassign from child class
-    base_fmt: str = NotImplementedError(
+    base_fmt: Union[str, NotImplementedError] = NotImplementedError(
         "Please implement base_fmt class property "
         "for this sub-formatter class"
     )
 
     # This value must reassign from child class
     base_attr_prefix: str = ""
 
     # This value must reassign from child class
     base_level: int = 1
 
     class Config:
         """Base Configuration"""
 
-        base_config_value = None
+        base_config_value: Optional[Any] = None
 
     @classmethod
-    def parse(cls, value: str, fmt: Optional[str] = None) -> BaseFormatter:
+    def parse(
+        cls,
+        value: str,
+        fmt: Optional[str] = None,
+    ) -> Formatter:
         """Parse string value with its format to subclass of base formatter
         object.
 
         :param value: a string value that match with fmt.
         :type value: str
         :param fmt: a format value will use `cls.base_fmt` if it does not pass
             from input argument.
         :type fmt: Optional[str](=None)
 
         :raises NotImplementedError: if fmt value parameter does not pass form
             input, or `cls.base_fmt` does not implement.
         :raises ValueError: if value does not match with regular expression
             format string.
 
-        :rtype: BaseFormatter
-        :return: an instance of BaseFormatter that parse from string value by
+        :rtype: Formatter
+        :return: an instance of Formatter that parse from string value by
             format string.
         """
-        _fmt: str = fmt or cls.base_fmt
+        _fmt: Union[str, NotImplementedError] = fmt or cls.base_fmt
 
         if not _fmt or isinstance(_fmt, NotImplementedError):
             raise NotImplementedError("This class does not set default format")
 
         _fmt = reduce(
             lambda x, y: x.replace(y, cls.regex()[y]),
             re.findall(r"(%[-+!*]?\w)", _fmt),
@@ -260,29 +305,31 @@
 
         :rtype: Dict[str, str]
         :return: a mapping of format, and it's regular expression string
         """
         results: Dict[str, str] = {}
         pre_results: Dict[str, str] = {}
         for f, props in cls.formatter().items():
+            # issue: https://github.com/python/mypy/issues/8887
+            # docs: https://mypy.readthedocs.io/en/stable/literal_types.html#tagged-unions
             if "regex" in props:
-                results[f] = props["regex"]
+                results[f] = props["regex"]  # type: ignore[typeddict-item]
             elif "cregex" in props:
                 pre_results[f] = props["cregex"]
             else:
                 raise FormatterValueError(
                     "formatter does not contain `regex` or `cregex` "
                     "in dict value"
                 )
         for f, cr in pre_results.items():
             # TODO: improve pref of this line when `results` was large
             #  of mapping regex values
             for rf in results:
                 if rf in cr:
-                    cr: str = cr.replace(rf, results[rf])
+                    cr = cr.replace(rf, results[rf])
             results[f] = cr
         return results
 
     def format(self, fmt: str) -> str:
         """Return string value that was filled by the input format pattern
         argument.
 
@@ -291,39 +338,45 @@
 
         :raises KeyError: if it has any format pattern does not found in
             `cls.formatter`.
 
         :rtype: str
         :return: a formatted string value
         """
-        _formatter: Dict[str, dict] = self.formatter(self.value)
+        _formatter: PropFormattersType = self.formatter(self.value)
         fmt = fmt.replace("%%", "[ESCAPE]")
         for _sup_fmt in re.findall(r"(%[-+!*]?\w)", fmt):
             try:
-                _value: Union[Callable, str] = _formatter[_sup_fmt]["value"]
+                _value: Union[FormatterCallable, str] = _formatter[_sup_fmt][
+                    "value"
+                ]
                 # FIXME: There shouldn't be any duplicate replaces to the
                 #  previous value
                 fmt = fmt.replace(
-                    _sup_fmt, (_value() if callable(_value) else _value)
+                    _sup_fmt,
+                    (_value() if callable(_value) else _value),
                 )
             except KeyError as err:
                 raise FormatterKeyError(
                     f"the format: {_sup_fmt!r} does not support for "
                     f"{self.__class__.__name__!r}"
                 ) from err
         return fmt.replace("[ESCAPE]", "%")
 
-    def __init__(self, formats: Optional[Dict] = None):
+    def __init__(
+        self,
+        formats: Optional[Dict[str, Any]] = None,
+    ) -> None:
         """Main initialization get the format mapping from input argument
         and generate the necessary attributes for define the value of this
         base formatter object.
 
             The setter of attribute does not do anything to __slot__ variable.
         """
-        _formats: Dict = formats or {}
+        _formats: Dict[str, Any] = formats or {}
 
         # Set level of SlotLevel object that set from `base_level` and pass this
         # value to _level variable for update process in priorities loop.
         setattr(
             self,
             f"_{self.base_attr_prefix}_level",
             SlotLevel(level=self.base_level),
@@ -336,30 +389,30 @@
                 f"_{self.base_attr_prefix}_{self.__class__.__name__.lower()}"
             ):
                 setattr(self, attr, None)
 
         for name, props in self.__priorities.items():
             # Split name of key of priorities property value.
             # From: <prefix>_<body> -> TO: [<prefix>, <body>]
-            attr: str = name.split("_", maxsplit=1)[0]
+            attr = name.split("_", maxsplit=1)[0]
 
             # Set attr condition
             # FIXME: the value in properties should defined input type!!!
             if getattr(self, f"_{self.base_attr_prefix}_{attr}"):
                 continue
             elif any(name.endswith(i) for i in {"_default", "_fix"}):
-                setattr(self, f"_{self.base_attr_prefix}_{attr}", props.value())
+                setattr(self, f"_{self.base_attr_prefix}_{attr}", props.value())  # type: ignore[call-arg]
 
                 # Update level by default it will update at first level
                 _level.update(props.level)
             elif name in _formats:
                 setattr(
                     self,
                     f"_{self.base_attr_prefix}_{attr}",
-                    props.value(_formats[name]),
+                    props.value(_formats[name]),  # type: ignore[call-arg]
                 )
 
                 # Update level by default it will update at first level
                 _level.update(props.level)
 
         # Set standard property by default is string value or `self.string`
         setattr(
@@ -370,14 +423,17 @@
 
         # Run validate method.
         if not self.validate:
             raise FormatterValueError(
                 "Parsing value does not valid from validator"
             )
 
+    def __setattr__(self, name: str, value: Any) -> None:
+        super().__setattr__(name, value)
+
     def __hash__(self) -> int:
         """Return hashed string value of str property"""
         return hash(self.string)
 
     def __str__(self) -> str:
         """Return string value of str property"""
         return self.string
@@ -386,92 +442,100 @@
         """Return represent string"""
         return (
             f"<{self.__class__.__name__}"
             f".parse('{self.string}', "
             f"'{self.base_fmt}')>"
         )
 
-    def __eq__(self, other) -> bool:
+    def __eq__(self, other: Union[Formatter, Any]) -> bool:
         return isinstance(other, self.__class__) and self.value == other.value
 
-    def __lt__(self, other) -> bool:
-        return self.value < other.value
+    def __lt__(self, other: Formatter) -> bool:
+        return self.value.__lt__(other.value)  # type: ignore[no-any-return]
 
     @property
+    @abstractmethod
     def value(self) -> Any:  # pragma: no cover
         """Return the value object that define by any subclass."""
         raise NotImplementedError(
             "Please implement value property for this sub-formatter class"
         )
 
     @property
+    @abstractmethod
     def string(self) -> str:  # pragma: no cover
         """Return standard string value that define by any subclass."""
         raise NotImplementedError(
             "Please implement string property for this sub-formatter class"
         )
 
     @property
     def validate(self) -> bool:
         """Validate method that will run after setup all attributes"""
         return True
 
-    def valid(self, string: str, fmt: str) -> bool:
+    def valid(
+        self,
+        string: str,
+        fmt: str,
+    ) -> bool:
         """Return true if the value attribute from parser of string and
         fmt is valid with self.value.
         """
-        return self.value == self.__class__.parse(string, fmt).value
+        return self.value.__eq__(self.__class__.parse(string, fmt).value)  # type: ignore[no-any-return]
 
     @property
     def level(self) -> SlotLevel:
         """Return the slot level object of any subclass."""
-        return getattr(self, f"_{self.base_attr_prefix}_level")
+        return getattr(self, f"_{self.base_attr_prefix}_level")  # type: ignore[no-any-return]
 
     @property
     def __priorities(self) -> Dict[str, PriorityData]:
         """Return private property of extracted mapping from
         `self.priorities` value.
         """
         return {k: PriorityData(**v) for k, v in self.priorities.items()}
 
     @property
+    @abstractmethod
     def priorities(
         self,
-    ) -> Dict[str, Dict[str, Union[Callable, Tuple[int, ...], int]]]:
+    ) -> PropPrioritiesType:
         """"""
         raise NotImplementedError(
             "Please implement priorities property for this sub-formatter class"
         )
 
     @staticmethod
+    @abstractmethod
     def formatter(
-        value: Optional = None,
-    ) -> Dict[str, Dict[str, Union[Callable, str]]]:
+        value: Optional[Any] = None,
+    ) -> PropFormattersType:
         """"""
         raise NotImplementedError(
             "Please implement formatter static method for this "
             "sub-formatter class"
         )
 
     @staticmethod
-    def default(value: str) -> Callable:
+    def default(value: str) -> Callable[[], str]:
         """Return wrapper function of value"""
         return lambda: value
 
 
-class Serial(BaseFormatter):
+class Serial(Formatter):
     """Serial object for register process that implement formatter and
     parser.
     """
 
     base_fmt: str = "%n"
 
     base_attr_prefix: str = "sr"
 
-    class Config(BaseFormatter.Config):
+    class Config(Formatter.Config):
         """Configuration of Serial object"""
 
         serial_max_padding: int = 3
         serial_max_binary: int = 8
 
     __slots__ = (
         "_sr_number",
@@ -480,20 +544,20 @@
 
     @property
     def value(self) -> int:
         return int(self.string)
 
     @property
     def string(self) -> str:
-        return self._sr_number
+        return self._sr_number  # type: ignore[no-any-return]
 
     @property
     def priorities(
         self,
-    ) -> Dict[str, Dict[str, Union[Callable, Tuple[int, ...], int]]]:
+    ) -> PropPrioritiesType:
         return {
             "number": {
                 "value": lambda x: x,
                 "level": 1,
             },
             "number_pad": {
                 "value": lambda x: remove_pad(x),
@@ -505,38 +569,38 @@
             },
             "number_default": {"value": self.default("0"), "level": 0},
         }
 
     @staticmethod
     def formatter(
         serial: Optional[int] = None,
-    ) -> Dict[str, Dict[str, Union[Callable, str]]]:
+    ) -> PropFormattersType:
         """Generate formatter that support mapping formatter,
             %n  : Normal format
             %p  : Padding number
             %b  : Binary number
 
         :param serial: the serial value that pars to generate all format
         :type serial: Optional[int](=None)
 
         :rtype: Dict[str, Dict[str, Union[Callable, str]]]
         :return: the generated mapping values of all format strings
         """
         _value: str = str(serial or 0)
         return {
-            "%n": {"value": _value, "regex": r"(?P<number>[0-9]*)"},
+            "%n": {"value": lambda: _value, "regex": r"(?P<number>[0-9]*)"},
             "%p": {
-                "value": Serial.to_padding(_value),
+                "value": partial(Serial.to_padding, _value),
                 "regex": (
                     r"(?P<number_pad>"
                     rf"[0-9]{{{str(Serial.Config.serial_max_padding)}}})"
                 ),
             },
             "%b": {
-                "value": Serial.to_binary(_value),
+                "value": partial(Serial.to_binary, _value),
                 "regex": r"(?P<number_binary>[0-1]*)",
             },
         }
 
     @staticmethod
     def to_padding(value: str) -> str:
         """Return padding string result with zero value"""
@@ -576,15 +640,15 @@
     "Tue": "3",
     "Fri": "4",
     "Sat": "5",
     "Sun": "6",
 }
 
 
-class Datetime(BaseFormatter):
+class Datetime(Formatter):
     """Datetime object for register process that implement formatter and
     parser.
     """
 
     base_fmt: str = "%Y-%m-%d %H:%M:%S.%f"
 
     base_attr_prefix: str = "dt"
@@ -631,15 +695,15 @@
     @property
     def validate(self) -> bool:  # no cov
         return True
 
     @property
     def priorities(
         self,
-    ) -> Dict[str, Dict[str, Union[Callable, Tuple[int, ...], int]]]:
+    ) -> PropPrioritiesType:
         """Priority Properties of the datetime object
 
         :rtype: Dict[str, Dict[str, Union[Callable, Tuple[int, ...], int]]]
         :returns: a priority properties of the datetime object
         """
         # TODO: Check about week value should keep first and validate if
         #  date value does not match with common sense.
@@ -813,15 +877,15 @@
                 "level": 0,
             },
         }
 
     @staticmethod
     def formatter(
         dt: Optional[datetime] = None,
-    ) -> Dict[str, Dict[str, Union[Callable, str]]]:
+    ) -> PropFormattersType:
         """Generate formatter that support mapping formatter,
             %n  : Normal format with `%Y%m%d_%H%M%S`
             %Y  : Year with century as a decimal number.
             %y  : Year without century as a zero-padded decimal number.
             %-y : Year without century as a decimal number.
             %m  : Month as a zero-padded decimal number.
             %-m : Month as a decimal number.
@@ -989,45 +1053,46 @@
                 "value": partial(_dt.strftime, "%f"),
                 "regex": r"(?P<microsecond_pad>\d{6})",
             },
         }
 
     def _from_day_year(self, value: str) -> str:
         """Return date of year"""
-        _this_year = datetime.strptime(self._dt_year, "%Y") + timedelta(
-            days=int(value)
-        )
+        _this_year: datetime = datetime.strptime(
+            self._dt_year, "%Y"
+        ) + timedelta(days=int(value))
         self._dt_month = _this_year.strftime("%m")
         return _this_year.strftime("%d")
 
     def _from_week_year_mon(self, value: str) -> str:
-        _this_week = (
+        _this_week: str = (
             str(((int(self._dt_week) - 1) % 7) + 1) if self._dt_week else "1"
         )
-        _this_year = datetime.strptime(
+        _this_year: datetime = datetime.strptime(
             f"{self._dt_year}-W{value}-{_this_week}", "%G-W%V-%u"
         )
         self._dt_month = _this_year.strftime("%m")
         self._dt_day = _this_year.strftime("%d")
         return _this_year.strftime("%w")
 
     def _from_week_year_sun(self, value: str) -> str:
-        _this_year = datetime.strptime(
+        _this_year: datetime = datetime.strptime(
             f"{self._dt_year}-W{value}-{self._dt_week or '0'}", "%Y-W%U-%w"
         )
         self._dt_month = _this_year.strftime("%m")
         self._dt_day = _this_year.strftime("%d")
         return _this_year.strftime("%w")
 
     @staticmethod
-    def remove_pad_dt(_dt: datetime, fmt: str):
+    def remove_pad_dt(_dt: datetime, fmt: str) -> str:
+        """Return padded datetime string that was formatted"""
         return remove_pad(_dt.strftime(fmt))
 
 
-class Version(BaseFormatter):
+class Version(Formatter):
     """Version object for register process that implement formatter and
     parser.
 
         Version segments reference from Hatch:
         - release	        1.0.0
         - major	            2.0.0
         - minor	            1.1.0
@@ -1063,51 +1128,51 @@
         "_vs_dev",
         "_vs_local",
     )
 
     def __repr__(self) -> str:
         _fmt: str = "v%m.%n.%c"
         if self._vs_epoch != "0":
-            _fmt: str = f"%e{_fmt[1:]}"
+            _fmt = f"%e{_fmt[1:]}"
         if self._vs_pre:
-            _fmt: str = f"{_fmt}%q"
+            _fmt = f"{_fmt}%q"
         if self._vs_post:
-            _fmt: str = f"{_fmt}%p"
+            _fmt = f"{_fmt}%p"
         if self._vs_dev:
-            _fmt: str = f"{_fmt}%d"
+            _fmt = f"{_fmt}%d"
         if self._vs_local:
-            _fmt: str = f"{_fmt}%l"
+            _fmt = f"{_fmt}%l"
         return (
             f"<{self.__class__.__name__}.parse(" f"'{self.string}', '{_fmt}')>"
         )
 
     @property
     def value(self) -> pck_version.Version:
         """"""
         return pck_version.parse(self.string)
 
     @property
     def string(self) -> str:
         _release: str = f"v{self._vs_major}.{self._vs_minor}.{self._vs_micro}"
         if self._vs_epoch != "0":
-            _release: str = f"{self._vs_epoch}!{_release[1:]}"
+            _release = f"{self._vs_epoch}!{_release[1:]}"
         if self._vs_pre:
-            _release: str = f"{_release}{self._vs_pre}"
+            _release = f"{_release}{self._vs_pre}"
         if self._vs_post:
-            _release: str = f"{_release}{self._vs_post}"
+            _release = f"{_release}{self._vs_post}"
         if self._vs_dev:
-            _release: str = f"{_release}.{self._vs_dev}"
+            _release = f"{_release}.{self._vs_dev}"
         if self._vs_local:
-            _release: str = f"{_release}+{self._vs_local}"
+            _release = f"{_release}+{self._vs_local}"
         return _release
 
     @property
     def priorities(
         self,
-    ) -> Dict[str, Dict[str, Union[Callable, Tuple[int, ...], int]]]:
+    ) -> PropPrioritiesType:
         return {
             "epoch": {
                 "value": lambda x: x.rstrip("!"),
                 "level": 3,
             },
             "epoch_num": {
                 "value": lambda x: x,
@@ -1166,15 +1231,15 @@
                 "level": 0,
             },
         }
 
     @staticmethod
     def formatter(
         version: Optional[pck_version.Version] = None,
-    ) -> Dict[str, Dict[str, str]]:
+    ) -> PropFormattersType:
         """Generate formatter that support mapping formatter,
             %f  : full version format with `%m_%n_%c`
             %-f : full version format with `%m-%n-%c`
             %m  : major number
             %n  : minor number
             %c  : micro number
             %e  : epoch release
@@ -1276,15 +1341,15 @@
                 elif re.match(rf"{rep}[-_.]?[0-9]+", value):
                     return value
         raise FormatterValueError(
             f"Convert prefix dose not valid for value `{value}`"
         )
 
 
-class Naming(BaseFormatter):
+class Naming(Formatter):
     """Naming object for register process that implement formatter and parser.
 
     note: A name value that parsing to this class should not contain any
     special characters, this will keep only.
     """
 
     base_fmt: str = "%n"
@@ -1306,25 +1371,25 @@
         return self.string
 
     @property
     def string(self) -> str:
         if self._nm_strings:
             return " ".join(self._nm_strings)
         elif self._nm_flats:
-            return self._nm_flats[0]
+            return self._nm_flats[0]  # type: ignore[no-any-return]
         elif self._nm_shorts:
             return " ".join(self._nm_shorts)
         elif self._nm_vowels:
-            return self._nm_vowels[0]
+            return self._nm_vowels[0]  # type: ignore[no-any-return]
         return ""
 
     @property
     def priorities(
         self,
-    ) -> Dict[str, Dict[str, Union[Callable, Tuple[int, ...], int]]]:
+    ) -> PropPrioritiesType:
         return {
             "strings": {"value": lambda x: x.split(), "level": 5},
             "strings_upper": {
                 "value": lambda x: x.lower().split(),
                 "level": 5,
             },
             "strings_title": {
@@ -1388,16 +1453,16 @@
                 "value": lambda x: [x.lower()],
                 "level": 1,
             },
         }
 
     @staticmethod
     def formatter(
-        value: Optional[Union[str, list]] = None
-    ) -> Dict[str, Dict[str, Union[Callable, str]]]:
+        value: Optional[Union[str, List[str]]] = None,
+    ) -> PropFormattersType:
         """Generate formatter that support mapping formatter,
 
             %n  : Normal name format
             %N  : Normal name upper case format
             %-N : Normal name title case format
             %u  : Upper case format
             %l  : Lower case format
@@ -1425,15 +1490,15 @@
             %v  : normal name removed vowel
             %V  : normal name removed vowel with upper case
 
         :param value:
 
         docs: https://gist.github.com/SuppieRK/a6fb471cf600271230c8c7e532bdae4b
         """
-        _value: list = (
+        _value: List[str] = (
             Naming.__prepare_value(value)
             if isinstance(value, str)
             else (value or [])
         )
         return {
             "%n": {
                 "value": partial(Naming.__join_with, " ", _value),
@@ -1574,88 +1639,99 @@
     def camel_case(snake_case: str) -> str:
         """Return a string value with camel case with lower case first
         letter.
         """
         return snake_case[0].lower() + Naming.pascal_case(snake_case)[1:]
 
     @staticmethod
-    def __join_with(by: str, values: list, func: Optional[Callable] = None):
+    def __join_with(
+        by: str, values: List[str], func: Optional[Callable[[str], str]] = None
+    ) -> str:
         return by.join(map(func, values)) if func else by.join(values)
 
     @staticmethod
-    def __prepare_value(value: str) -> list:
+    def __prepare_value(value: str) -> List[str]:
         """Return list of word that split from input value string"""
         result = re.sub(r"[^\-.\w\s]+", "", value)
         return re.sub(r"[\-._\s]]", " ", result).strip().split()
 
     @staticmethod
-    def __split_pascal_case(value: str) -> list:
+    def __split_pascal_case(value: str) -> List[str]:
         return (
             "".join([f" {c.lower()}" if c.isupper() else c for c in value])
             .strip()
             .split()
         )
 
 
-ConstantType = Type["BaseConstant"]
-
-
-class BaseConstant(BaseFormatter):
+class __BaseConstant(Formatter):
     """Constant object for register process that implement formatter and
     parser.
     """
 
     base_attr_prefix: str = "ct"
 
-    base_formatter: Optional[dict] = None
+    base_formatter: Optional[PropFormattersType] = None
 
     __slots__ = (
         "_ct_string",
         "_ct_constant",
     )
 
     @classmethod
-    def create(cls, formatter: dict) -> ConstantType:
+    def create(cls, formatter: Dict[str, str]) -> ConstantType:
         """Set formatter"""
-        cls.base_formatter: dict = {
+        cls.base_formatter = {
             fmt: {
                 "regex": f"(?P<constant>{formatter[fmt]})",
                 "value": formatter[fmt],
             }
             for fmt in formatter.copy()
         }
         return cls
 
     @property
     def priorities(
         self,
-    ) -> Dict[str, Dict[str, Union[Callable, Tuple[int, ...], int]]]:
+    ) -> PropPrioritiesType:
         return {
             "constant": {
                 "value": lambda x: x,
                 "level": 1,
             },
         }
 
+    def __init__(
+        self,
+        formats: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        if not self.base_formatter:
+            raise NotImplementedError(
+                "The Constant object should define the `cls.base_formatter` "
+                "before make a instance."
+            )
+        super().__init__(formats=formats)
+
     @property
     def value(self) -> str:
         return self.string
 
     @property
     def string(self) -> str:
         return str(self.base_formatter)
 
     @classmethod
-    def formatter(
-        cls, value: Optional[str] = None
-    ) -> Dict[str, Dict[str, Union[Callable, str]]]:
+    def formatter(  # type: ignore[override]
+        cls,
+        value: Optional[str] = None,
+    ) -> Optional[PropFormattersType]:
         return cls.base_formatter
 
 
-Constant = BaseConstant.create
+Constant = __BaseConstant.create
 
 EnvConstant: ConstantType = Constant(
     {
         "%d": "development",
         "%-d": "dev",
         "%s": "sit",
         "%-s": "sit",
@@ -1667,17 +1743,14 @@
         "%-t": "test",
         "%b": "sandbox",
         "%-b": "box",
         "%c": "poc",
     }
 )
 
-Formatter = TypeVar("Formatter", bound=BaseFormatter)
-
-FormatterType = Type[Formatter]
 
 FORMATTERS: Dict[str, Type[BaseFormatter]] = {
     "timestamp": Datetime,
     "version": Version,
     "serial": Serial,
     "naming": Naming,
     "envconst": EnvConstant,
@@ -1691,30 +1764,32 @@
 
 class ExpectRegexValue(TypedDict):
     regex: str
     value: Callable[[], Any]
 
 
 def extract_regex_with_value(
-    fmt: FormatterType, value: Optional[Any] = None, called: bool = False
-) -> Dict[str, ExpectRegexValue]:
+    fmt: FormatterType,
+    value: Optional[Any] = None,
+    called: bool = False,
+) -> Dict[str, RegexValue]:
     """Return extract data from `cls.regex` method and `cls.formatter`
 
     :param fmt: a formatter object
     :type fmt: FormatterType
     :param value:
     :type value: Optional[Any]
     :param called: a called flag for extract value if it callable
     :type called: bool(=False)
 
     :rtype: Dict[str, dict]
     :return: an extract data from `cls.regex` method and `cls.formatter`
     """
     regex: Dict[str, str] = fmt.regex()
-    formatter: Dict[str, Dict[str, Union[Callable, str]]] = fmt.formatter(value)
+    formatter: PropFormattersType = fmt.formatter(value)
     return {
         i: {
             "regex": regex[i],
             "value": (
                 caller(formatter[i]["value"])
                 if called
                 else formatter[i]["value"]
@@ -1749,46 +1824,54 @@
         -3
 
         >>> -relativeserial(**{"number": 5})
         <relativeserial(number=-5)>
 
     """
 
-    def __init__(self, number: int = 0):
-        self.number = number
+    def __init__(self, number: int = 0) -> None:
+        self.number: int = number
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self.number)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(number={self.number})>"
 
-    def __eq__(self, other: Union[int, relativeserial]):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, int):
             return self.number == other
-        return self.number == other.number
+        if isinstance(other, relativeserial):
+            return self.number == other.number
+        raise NotImplementedError
 
-    def __lt__(self, other):
+    def __lt__(self, other: relativeserial) -> bool:
         return self.number < other.number
 
-    def __neg__(self):
+    def __neg__(self) -> relativeserial:
         return self.__class__(number=-self.number)
 
-    def __rsub__(self, other: Union[int, relativeserial]):
+    def __rsub__(self, other: int) -> int:
         return other - self.number
 
-    def __sub__(self, other: Union[int, relativeserial]):
+    def __sub__(
+        self,
+        other: Union[int, relativeserial],
+    ) -> Union[int, relativeserial]:
         if isinstance(other, int):
             return self.number - other
         return self.__class__(number=(self.number - other.number))
 
-    def __radd__(self, other: Union[int, relativeserial]):
+    def __radd__(self, other: int) -> int:
         return other + self.number
 
-    def __add__(self, other: Union[int, relativeserial]):
+    def __add__(
+        self,
+        other: Union[int, relativeserial],
+    ) -> Union[int, relativeserial]:
         if isinstance(other, int):
             return self.__radd__(other)
         return self.__class__(number=(self.number + other.number))
 
 
 # TODO: create relativeversion
 # @total_ordering
@@ -1811,34 +1894,34 @@
         self.alpha: Optional[int] = alpha
         self.beta: Optional[int] = beta
         self.pre: Optional[int] = pre
         self.post: Optional[int] = post
         self.dev: Optional[int] = dev
         self.local: Optional[str] = local
 
-    def __hash__(self) -> str:
-        return ...
+    def __hash__(self) -> int:
+        return ...  # type: ignore
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}()>"
 
     def __eq__(self, other) -> bool:  # type: ignore
-        return ...
+        return ...  # type: ignore
 
     def __neg__(self) -> relativeversion:
-        return ...
+        return ...  # type: ignore
 
     def __add__(self, other):  # type: ignore
         return ...
 
     def __sub__(self, other):  # type: ignore
         return ...
 
     def __lt__(self, other) -> bool:  # type: ignore
-        return ...
+        return ...  # type: ignore
 
 
 def adjust_datetime(
     self: OrderFormatter, metrics: Optional[Dict[str, int]] = None
 ) -> OrderFormatter:
     """
     :param self: a OrderFormatter instance that want to adjust
@@ -1850,26 +1933,27 @@
     """
     _metrics: Dict[str, int] = metrics or {}
     if "timestamp" not in self.data:
         raise FormatterArgumentError(
             "timestamp",
             "order file object does not have `timestamp` in name " "formatter",
         )
-    _replace: List[BaseFormatter] = [
+    _replace: List[Formatter] = [
         FORMATTERS["timestamp"].parse(
             **{
-                "value": (time_data.value - relativedelta(**_metrics)).strftime(
-                    "%Y%m%d %H%M%S"
-                ),
+                "value": (
+                    time_data.value
+                    - relativedelta(**_metrics)  # type: ignore[arg-type]
+                ).strftime("%Y%m%d %H%M%S"),
                 "fmt": "%Y%m%d %H%M%S",
             }
         )
         for time_data in self.data["timestamp"]
     ]
-    self.data["timestamp"]: List[BaseFormatter] = _replace
+    self.data["timestamp"] = _replace
     return self
 
 
 def adjust_serial(
     self: OrderFormatter, metrics: Optional[Dict[str, int]] = None
 ) -> OrderFormatter:
     """
@@ -1882,15 +1966,15 @@
     """
     _metrics: Dict[str, int] = metrics or {}
     if "serial" not in self.data:
         raise FormatterArgumentError(
             "serial",
             "order file object does not have `serial` in name " "formatter",
         )
-    _replace: List[BaseFormatter] = [
+    _replace: List[Formatter] = [
         FORMATTERS["serial"].parse(
             **{
                 "value": (str(serial.value - relativeserial(**_metrics))),
                 "fmt": "%n",
             }
         )
         for serial in self.data["serial"]
@@ -1910,43 +1994,41 @@
 class OrderFormatter:
     """Order formatter object from mapping dictionary.
 
     :param formatters: a mapping value
     :type formatters: dict
 
     :raises TypeError: if value of mapping does not match with dict or
-        BaseFormatter type.
+        Formatter type.
     """
 
     __slots__ = ("data",)
 
-    def __init__(
-        self, formatters: Dict[str, Union[BaseFormatter, Dict[str, Any]]]
-    ):
+    def __init__(self, formatters: Dict[str, Union[Formatter, Dict[str, Any]]]):
         """Main initialize process of the ordering formatter object."""
-        self.data: Dict[str, List[BaseFormatter]] = {}
+        self.data: Dict[str, List[Formatter]] = {}
         # TODO: add merge_dict function to mapping by {'serial': ...}
         #  before for-loop process
-        for name in formatters:
+        for name, value in formatters.items():
             _name: str = re.sub(r"(_\d+)$", "", name)
 
             if _name not in FORMATTERS:
                 raise FormatterValueError(
                     f"value of key {_name} does not support"
                 )
 
-            name_value: List[BaseFormatter] = self.data.setdefault(_name, [])
-            if isinstance(formatters[name], dict):
-                name_value.append(FORMATTERS[_name].parse(**formatters[name]))
-            elif isinstance(formatters[name], BaseFormatter):
-                name_value.append(formatters[name])
+            name_value: List[Formatter] = self.data.setdefault(_name, [])
+            if isinstance(value, Formatter):
+                name_value.append(value)
+            elif isinstance(value, dict):
+                name_value.append(FORMATTERS[_name].parse(**value))
             else:
                 raise FormatterTypeError(
                     f"value of key {_name} does not support for type "
-                    f"{type(formatters[name])}"
+                    f"{type(value)}"
                 )
 
     def adjust(self, fmt: str, value: int):  # type: ignore  # no cov
         # TODO: merge adjust methods to dynamic method
         if fmt not in self.data:
             raise FormatterArgumentError(
                 fmt,
@@ -1970,15 +2052,15 @@
         """
         if "version" not in self.data:
             raise FormatterArgumentError(
                 "version",
                 "order file object does not have `version` "
                 "in name formatter",
             )
-        _replace: List[BaseFormatter] = []
+        _replace: List[Formatter] = []
         for version_data in self.data["version"]:
             # `versioning` must have 3 length of tuple
             versioning: Tuple[int, ...] = version_data.value.release
             _values: List[int] = [
                 -99 if v == "*" else int(v) for v in value.split(".")
             ]
             _results: List[str] = []
@@ -2035,15 +2117,15 @@
                 if (name in self.data and name in other.data)
             ),
             self.__eq__(other),
         )
 
 
 class FormatterGroupParseArgs(TypedDict):
-    fmt: FormatterType[Any]
+    fmt: FormatterType
     value: Optional[str]
 
 
 @dataclass
 class FormatterGroupData:
     """Formatter Data"""
 
@@ -2107,15 +2189,15 @@
             for k, v in formatters.items()
         }
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({', '.join(self.formatters)})"
 
     @property
-    def groups(self) -> Dict[str, Dict[str, ExpectRegexValue]]:
+    def groups(self) -> Dict[str, Dict[str, RegexValue]]:
         """Return the groups of format value and extract Formatter
         values.
         """
         return {
             k: extract_regex_with_value(v.fmt, v.value)
             for k, v in self.formatters.items()
         }
@@ -2292,15 +2374,15 @@
             was duplicated from string formatter.
         """
         return f"__{str(index - 1)}" if index > 1 else ""
 
     @staticmethod
     def __loop_sub_fmt(
         search: re.Match[str],
-        mapping: Dict[str, ExpectRegexValue],
+        mapping: Dict[str, RegexValue],
         key: Literal["regex", "value"],
         index: int = 1,
     ) -> str:
         """Loop method for find any sub-format from search input argument.
 
         :param search: a Match object from searching process.
         :type search: re.Match
@@ -2345,19 +2427,18 @@
                 ) from err
         return _search_re
 
 
 __all__ = (
     "FORMATTERS",
     "FORMATTERS_ADJUST",
-    "BaseFormatter",
+    "Formatter",
     "Serial",
     "Datetime",
     "Version",
     "Naming",
     "ConstantType",
     "Constant",
     "EnvConstant",
-    "Formatter",
     "FormatterGroup",
     "OrderFormatter",
 )
```

### Comparing `dup_fmt-0.0.3/dup_fmt/utils.py` & `dup_fmt-0.0.3.post1/dup_fmt/utils.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/tests/test_errors.py` & `dup_fmt-0.0.3.post1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/tests/test_formatter.py` & `dup_fmt-0.0.3.post1/tests/test_formatter.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
 Test the formatter object.
 """
 import unittest
+from abc import ABC
 from typing import Dict, Optional, Type
 
 import dup_fmt.formatter as fmt
 from dup_fmt.exceptions import FormatterValueError
 
 
 class SlotLevelTestCase(unittest.TestCase):
@@ -58,17 +59,17 @@
     def test_init_data(self):
         self.assertEqual(
             "PriorityData(level=5)",
             fmt.PriorityData(**{"value": self.caller, "level": 5}).__repr__(),
         )
 
 
-class BaseFormatterTestCase(unittest.TestCase):
+class FormatterTestCase(unittest.TestCase):
     def setUp(self) -> None:
-        class WrongFormatter(fmt.BaseFormatter):
+        class WrongFormatter(fmt.Formatter):
             base_fmt: str = "%n"
 
             base_attr_prefix: str = "sr"
 
             __slots__ = (
                 "_sr_number",
                 "_sr_serial",
@@ -94,43 +95,85 @@
                 return {
                     "%n": {
                         "value": _value,
                         "wrong_regex": r"(?P<number>[0-9]*)",
                     },
                 }
 
+        class NotImpPriority(fmt.Formatter, ABC):
+            base_fmt: str = "%n"
+
+            base_attr_prefix: str = "sr"
+
+            __slots__ = (
+                "_sr_number",
+                "_sr_serial",
+            )
+
+            @property
+            def value(self) -> int:  # pragma: no cover
+                return 1
+
+            @property
+            def string(self) -> str:  # pragma: no cover
+                return "Demo"
+
+            @staticmethod
+            def formatter(
+                serial: Optional[int] = None,
+            ) -> Dict[str, Dict[str, str]]:
+                _value: str = str(serial or 0)
+                return {
+                    "%n": {
+                        "value": _value,
+                        "wrong_regex": r"(?P<number>[0-9]*)",
+                    },
+                }
+
         class ValidateFormatter(fmt.Naming):
             @property
             def validate(self) -> bool:
                 return False
 
         self.wrong_fmt_cls = WrongFormatter
+        self.not_imp_priority_cls = NotImpPriority
         self.validate_fmt_cls = ValidateFormatter
 
     def test_base_formatter_properties(self):
-        with self.assertRaises(NotImplementedError) as context:
-            fmt.BaseFormatter()
+        with self.assertRaises(TypeError) as context:
+            fmt.Formatter()
         self.assertTrue(
             (
-                "Please implement priorities property "
-                "for this sub-formatter class"
+                "Can't instantiate abstract class Formatter with abstract "
+                "methods formatter, priorities, string, value"
+            )
+            in str(context.exception)
+        )
+
+    def test_base_formatter_init_with_fmt(self):
+        with self.assertRaises(TypeError) as context:
+            fmt.Formatter({"month": 1})
+        self.assertTrue(
+            (
+                "Can't instantiate abstract class Formatter with abstract "
+                "methods formatter, priorities, string, value"
             )
             in str(context.exception)
         )
 
     def test_base_formatter_parse_without_fmt(self):
         with self.assertRaises(NotImplementedError) as context:
-            fmt.BaseFormatter.parse("dummy")
+            fmt.Formatter.parse("dummy")
         self.assertTrue(
             "This class does not set default format" in str(context.exception)
         )
 
     def test_base_formatter_parse_with_fmt(self):
         with self.assertRaises(NotImplementedError) as context:
-            fmt.BaseFormatter.parse("dummy", "%Z")
+            fmt.Formatter.parse("dummy", "%Z")
         self.assertTrue(
             (
                 "Please implement formatter static method "
                 "for this sub-formatter class"
             )
             in str(context.exception)
         )
@@ -139,14 +182,23 @@
         with self.assertRaises(FormatterValueError) as context:
             self.wrong_fmt_cls.regex()
         self.assertTrue(
             "formatter does not contain `regex` or `cregex` "
             "in dict value" in str(context.exception)
         )
 
+    def test_new_format_without_priorities(self):
+        with self.assertRaises(TypeError) as context:
+            self.not_imp_priority_cls()
+        self.assertTrue(
+            "Can't instantiate abstract class NotImpPriority "
+            "with abstract method" in str(context.exception)
+        )
+        self.assertTrue("priorities" in str(context.exception))
+
     def test_new_validate_error(self):
         with self.assertRaises(FormatterValueError) as context:
             self.validate_fmt_cls()
         self.assertTrue(
             "Parsing value does not valid from validator"
             in str(context.exception)
         )
```

### Comparing `dup_fmt-0.0.3/tests/test_formatter_datetime.py` & `dup_fmt-0.0.3.post1/tests/test_formatter_datetime.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/tests/test_formatter_group.py` & `dup_fmt-0.0.3.post1/tests/test_formatter_group.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/tests/test_formatter_naming.py` & `dup_fmt-0.0.3.post1/tests/test_formatter_naming.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/tests/test_formatter_order.py` & `dup_fmt-0.0.3.post1/tests/test_formatter_order.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/tests/test_formatter_serial.py` & `dup_fmt-0.0.3.post1/tests/test_formatter_serial.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,29 @@
                 "%n": "(?P<number>[0-9]*)",
                 "%p": "(?P<number_pad>[0-9]{3})",
                 "%b": "(?P<number_binary>[0-1]*)",
             },
             fmt.Serial.regex(),
         )
 
+    def test_serial_formatter(self):
+        self.assertDictEqual(
+            {
+                "%b": {
+                    "regex": "(?P<number_binary>[0-1]*)",
+                    "value": "1000000000",
+                },
+                "%n": {"regex": "(?P<number>[0-9]*)", "value": "512"},
+                "%p": {"regex": "(?P<number_pad>[0-9]{3})", "value": "512"},
+            },
+            fmt.extract_regex_with_value(
+                fmt=fmt.Serial, value=512, called=True
+            ),
+        )
+
     def test_serial_properties(self):
         self.assertEqual("<Serial.parse('781', '%n')>", self.sr.__repr__())
         self.assertEqual(hash(self.sr.string), self.sr.__hash__())
 
         self.assertEqual(9, self.sr_p.value)
         self.assertEqual("9", self.sr_p.string)
```

### Comparing `dup_fmt-0.0.3/tests/test_formatter_version.py` & `dup_fmt-0.0.3.post1/tests/test_formatter_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
                     "value": "+None",
                 },
             },
             fmt.extract_regex_with_value(
                 fmt=fmt.Version, value=Version(version="0.5.6"), called=True
             ),
         )
-        ...
 
     def test_version_properties(self):
         self.assertEqual(
             "<Version.parse('v8.1.0post2+local1.0', 'v%m.%n.%c%p%l')>",
             self.vs.__repr__(),
         )
         self.assertEqual(
```

### Comparing `dup_fmt-0.0.3/tests/test_ralativeserial.py` & `dup_fmt-0.0.3.post1/tests/test_ralativeserial.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/tests/examples/test_formatter_datetime.py` & `dup_fmt-0.0.3.post1/tests/examples/test_formatter_datetime.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/tests/examples/test_formatter_version.py` & `dup_fmt-0.0.3.post1/tests/examples/test_formatter_version.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/.gitignore` & `dup_fmt-0.0.3.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/LICENSE` & `dup_fmt-0.0.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.3/README.md` & `dup_fmt-0.0.3.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 
 **Install from PyPI**:
 
 ```shell
 pip install dup-fmt
 ```
 
-First objective of this project is include necessary formatter objects for data
-components of the framework engine pakage. We can use `parse` any filename on source
+:dart: First objective of this project is include necessary formatter objects for data
+components of the framework engine package. We can use `parse` any filename on source
 server machine and ingest the right filename to target landing zone.
 
 For example, we want to get filename with the format like, `filename_20220101.csv`, on
-the file system storage, and we want to incremental ingest latest file with date **2022-03-25**
+the file system storage, and we want to incremental ingest the latest file with date **2022-03-25**
 date. So we will implement `Datetime` object and parse that filename to it,
 
 ```python
 Datetime.parse('filename_20220101.csv', 'filename_%Y%m%d.csv').value == datetime.today()
 ```
 
-The above example is **NOT SURPRISE!!!** for us because Python already provide build-in package
+The above example is :yawning_face: **NOT SURPRISE!!!** for us because Python already provide build-in package
 `datetime` to parse by `.strptime` and format by `.strftime` with any string datetime value.
 This package will the special thing when we combine more than one formatter objects such as `Naming`,
 `Version`, or `Constant` together.
 
 **For complex filename format like**:
 
 ```text
@@ -67,16 +67,16 @@
 
 - [Datetime](#datetime)
 - [Version](#version)
 - [Serial](#serial)
 - [Naming](#naming)
 - [Constant](#constant)
 
-The main component is **Formatter Objects** for `parse` and `format` with string
-value, such as `Datetime`, `Version`, and `Serial` formatter objects. This objects
+The main purpose is **Formatter Objects** for `parse` and `format` with string
+value, such as `Datetime`, `Version`, and `Serial` formatter objects. These objects
 were used for parse any filename with put the format string value. The formatter
 able to enhancement any format value from sting value, like in `Datetime`, for `%B`
 value that was designed for month shortname (`Jan`, `Feb`, etc.) that does not
 support in build-in `datetime` package.
 
 > **Note**: \
 > The main usage of this formatter object is `parse` and `format` method.
@@ -93,14 +93,16 @@
 datetime.format('This_datetime_format_%Y%b-%-d_%H:%M:%S')
 ```
 
 ```text
 >>> 'This_datetime_format_2022Jan-1_00:01:01'
 ```
 
+[Supported Datetime formats](/docs/en/docs/API.md#datetime)
+
 ### Version
 
 ```python
 from dup_fmt import Version
 
 version = Version.parse(
     value='This_is_version_2_0_1',
@@ -109,14 +111,16 @@
 version.format('New_version_%m%n%c')
 ```
 
 ```text
 >>> 'New_version_201'
 ```
 
+[Supported Version formats](/docs/en/docs/API.md#version)
+
 ### Serial
 
 ```python
 from dup_fmt import Serial
 
 serial = Serial.parse(
     value='This_is_serial_62130',
@@ -125,14 +129,16 @@
 serial.format('Convert to binary: %b')
 ```
 
 ```text
 >>> 'Convert to binary: 1111001010110010'
 ```
 
+[Supported Serial formats](/docs/en/docs/API.md#serial)
+
 ### Naming
 
 ```python
 from dup_fmt import Naming
 
 naming = Naming.parse(
     value='de is data engineer',
@@ -141,14 +147,16 @@
 naming.format('Camel case is %c')
 ```
 
 ```text
 >>> 'Camel case is dataEngineer'
 ```
 
+[Supported Naming formats](/docs/en/docs/API.md#naming)
+
 ### Constant
 
 ```python
 from dup_fmt import Constant
 from dup_fmt.exceptions import FormatterError
 
 const = Constant({
@@ -170,17 +178,17 @@
 ```
 
 > **Note**: \
 > This package already implement environment constant object, `dup_fmt.EnvConstant`.
 
 ## Ordered Formatter
 
-The Formatter object already implement the `OrderFormatter` object that combine
-all formatter objects together and can use order properties with other
-`OrderFormatter` object.
+The **Ordered Formatter** object, `OrderFormatter`, that will combine some of all
+formatter objects together. The use-case of this object is make **order principle**
+to formatter objects.
 
 ```python
 from dup_fmt import OrderFormatter, Datetime, Version
 
 ordered_1 = OrderFormatter({
     'timestamp': Datetime.parse("20220101", "%Y%m%d"),
     'version': Version.parse("202", "%m%n%c"),
@@ -195,17 +203,17 @@
 > **Warning**: \
 > This object support for any formatter object only in `FORMATTERS` mapping constant,
 > this mapping constant contain; `Datetime` - timestamp, `Serial` - serial,
 > `Version` - version, `Naming` - naming, and `EnvConstant` - envconst.
 
 ## Formatter Group
 
-The formatter group object, `FormatterGroup`, that is the grouping of needed
-mapping formatter object and name together. You can define a name of formatter
-like `name` as Naming object, or `timestamp` as Datetime object.
+The **Formatter Group** object, `FormatterGroup`, which is the grouping of needed
+mapping formatter objects and its name together. You can define a name of formatter
+that you want, like `name` for `Naming` object, or `timestamp` for `Datetime` object.
 
 **Parse**:
 
 ```python
 from dup_fmt import FormatterGroup, Naming, Datetime
 
 group = FormatterGroup({'name': Naming, 'datetime': Datetime})
@@ -241,28 +249,32 @@
 group.format('{name:%c}_{timestamp:%Y_%m_%d}_{name}')
 ```
 
 ```text
 >>> dataEngineer_2022_01_01
 ```
 
+> **Warning**: \
+> This formatter group object does not good enough for implement order principle.
+> If you want it, you can use `OrderFormatter` together with `FormatterGroup`.
+
 ## Make your Formatter Object
 
 If this implemented formatter objects in this package does not help you all scenario
 of a formatted value, you can create your formatter object by yourself.
 
-This package provide the base abstract class, `BaseFormatter`, for this use-case. You
+This package provide the base abstract class, `Formatter`, for this use-case. You
 can create your formatter object like,
 
 ```python
 from typing import Optional, Dict, Union, Callable, Tuple
-from dup_fmt import BaseFormatter
+from dup_fmt import Formatter
 
 
-class Storage(BaseFormatter):
+class Storage(Formatter):
 
     base_fmt = '%b'
 
     base_attr_prefix = "st"
 
     __slots__ = (
         "_st_bit",
```

### Comparing `dup_fmt-0.0.3/pyproject.toml` & `dup_fmt-0.0.3.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 relative_files = true
 
 [tool.coverage.report]
 exclude_lines = [
     "no cov",
     "if __name__ == __main__:",
     "if TYPE_CHECKING:",
+    "raise NotImplementedError",
 ]
 
 [tool.hatch.version]
 scheme = "standard"
 source = "code"
 path = "dup_fmt/__about__.py"
```

### Comparing `dup_fmt-0.0.3/PKG-INFO` & `dup_fmt-0.0.3.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dup-fmt
-Version: 0.0.3
+Version: 0.0.3.post1
 Summary: The utility formatter objects for the data engine package
 Project-URL: Homepage, https://github.com/korawica/dup-fmt/
 Project-URL: Source Code, https://github.com/korawica/dup-fmt/
 Author-email: korawica <korawich.anu@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: data,formatter
@@ -60,27 +60,27 @@
 
 **Install from PyPI**:
 
 ```shell
 pip install dup-fmt
 ```
 
-First objective of this project is include necessary formatter objects for data
-components of the framework engine pakage. We can use `parse` any filename on source
+:dart: First objective of this project is include necessary formatter objects for data
+components of the framework engine package. We can use `parse` any filename on source
 server machine and ingest the right filename to target landing zone.
 
 For example, we want to get filename with the format like, `filename_20220101.csv`, on
-the file system storage, and we want to incremental ingest latest file with date **2022-03-25**
+the file system storage, and we want to incremental ingest the latest file with date **2022-03-25**
 date. So we will implement `Datetime` object and parse that filename to it,
 
 ```python
 Datetime.parse('filename_20220101.csv', 'filename_%Y%m%d.csv').value == datetime.today()
 ```
 
-The above example is **NOT SURPRISE!!!** for us because Python already provide build-in package
+The above example is :yawning_face: **NOT SURPRISE!!!** for us because Python already provide build-in package
 `datetime` to parse by `.strptime` and format by `.strftime` with any string datetime value.
 This package will the special thing when we combine more than one formatter objects such as `Naming`,
 `Version`, or `Constant` together.
 
 **For complex filename format like**:
 
 ```text
@@ -102,16 +102,16 @@
 
 - [Datetime](#datetime)
 - [Version](#version)
 - [Serial](#serial)
 - [Naming](#naming)
 - [Constant](#constant)
 
-The main component is **Formatter Objects** for `parse` and `format` with string
-value, such as `Datetime`, `Version`, and `Serial` formatter objects. This objects
+The main purpose is **Formatter Objects** for `parse` and `format` with string
+value, such as `Datetime`, `Version`, and `Serial` formatter objects. These objects
 were used for parse any filename with put the format string value. The formatter
 able to enhancement any format value from sting value, like in `Datetime`, for `%B`
 value that was designed for month shortname (`Jan`, `Feb`, etc.) that does not
 support in build-in `datetime` package.
 
 > **Note**: \
 > The main usage of this formatter object is `parse` and `format` method.
@@ -128,14 +128,16 @@
 datetime.format('This_datetime_format_%Y%b-%-d_%H:%M:%S')
 ```
 
 ```text
 >>> 'This_datetime_format_2022Jan-1_00:01:01'
 ```
 
+[Supported Datetime formats](/docs/en/docs/API.md#datetime)
+
 ### Version
 
 ```python
 from dup_fmt import Version
 
 version = Version.parse(
     value='This_is_version_2_0_1',
@@ -144,14 +146,16 @@
 version.format('New_version_%m%n%c')
 ```
 
 ```text
 >>> 'New_version_201'
 ```
 
+[Supported Version formats](/docs/en/docs/API.md#version)
+
 ### Serial
 
 ```python
 from dup_fmt import Serial
 
 serial = Serial.parse(
     value='This_is_serial_62130',
@@ -160,14 +164,16 @@
 serial.format('Convert to binary: %b')
 ```
 
 ```text
 >>> 'Convert to binary: 1111001010110010'
 ```
 
+[Supported Serial formats](/docs/en/docs/API.md#serial)
+
 ### Naming
 
 ```python
 from dup_fmt import Naming
 
 naming = Naming.parse(
     value='de is data engineer',
@@ -176,14 +182,16 @@
 naming.format('Camel case is %c')
 ```
 
 ```text
 >>> 'Camel case is dataEngineer'
 ```
 
+[Supported Naming formats](/docs/en/docs/API.md#naming)
+
 ### Constant
 
 ```python
 from dup_fmt import Constant
 from dup_fmt.exceptions import FormatterError
 
 const = Constant({
@@ -205,17 +213,17 @@
 ```
 
 > **Note**: \
 > This package already implement environment constant object, `dup_fmt.EnvConstant`.
 
 ## Ordered Formatter
 
-The Formatter object already implement the `OrderFormatter` object that combine
-all formatter objects together and can use order properties with other
-`OrderFormatter` object.
+The **Ordered Formatter** object, `OrderFormatter`, that will combine some of all
+formatter objects together. The use-case of this object is make **order principle**
+to formatter objects.
 
 ```python
 from dup_fmt import OrderFormatter, Datetime, Version
 
 ordered_1 = OrderFormatter({
     'timestamp': Datetime.parse("20220101", "%Y%m%d"),
     'version': Version.parse("202", "%m%n%c"),
@@ -230,17 +238,17 @@
 > **Warning**: \
 > This object support for any formatter object only in `FORMATTERS` mapping constant,
 > this mapping constant contain; `Datetime` - timestamp, `Serial` - serial,
 > `Version` - version, `Naming` - naming, and `EnvConstant` - envconst.
 
 ## Formatter Group
 
-The formatter group object, `FormatterGroup`, that is the grouping of needed
-mapping formatter object and name together. You can define a name of formatter
-like `name` as Naming object, or `timestamp` as Datetime object.
+The **Formatter Group** object, `FormatterGroup`, which is the grouping of needed
+mapping formatter objects and its name together. You can define a name of formatter
+that you want, like `name` for `Naming` object, or `timestamp` for `Datetime` object.
 
 **Parse**:
 
 ```python
 from dup_fmt import FormatterGroup, Naming, Datetime
 
 group = FormatterGroup({'name': Naming, 'datetime': Datetime})
@@ -276,28 +284,32 @@
 group.format('{name:%c}_{timestamp:%Y_%m_%d}_{name}')
 ```
 
 ```text
 >>> dataEngineer_2022_01_01
 ```
 
+> **Warning**: \
+> This formatter group object does not good enough for implement order principle.
+> If you want it, you can use `OrderFormatter` together with `FormatterGroup`.
+
 ## Make your Formatter Object
 
 If this implemented formatter objects in this package does not help you all scenario
 of a formatted value, you can create your formatter object by yourself.
 
-This package provide the base abstract class, `BaseFormatter`, for this use-case. You
+This package provide the base abstract class, `Formatter`, for this use-case. You
 can create your formatter object like,
 
 ```python
 from typing import Optional, Dict, Union, Callable, Tuple
-from dup_fmt import BaseFormatter
+from dup_fmt import Formatter
 
 
-class Storage(BaseFormatter):
+class Storage(Formatter):
 
     base_fmt = '%b'
 
     base_attr_prefix = "st"
 
     __slots__ = (
         "_st_bit",
```


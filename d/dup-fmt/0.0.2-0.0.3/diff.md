# Comparing `tmp/dup_fmt-0.0.2.tar.gz` & `tmp/dup_fmt-0.0.3.tar.gz`

## Comparing `dup_fmt-0.0.2.tar` & `dup_fmt-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/dup_fmt/__about__.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/dup_fmt/__init__.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/dup_fmt/errors.py
--rw-r--r--   0        0        0    72951 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/dup_fmt/formatter.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/dup_fmt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_errors.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_examples.py
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_formatter.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_formatter_datetime.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_formatter_group.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_formatter_naming.py
--rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_formatter_order.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_formatter_serial.py
--rw-r--r--   0        0        0     6091 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_formatter_version.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/test_ralativeserial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/perfs/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/tests/perfs/perf_fomatter_datetime.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/LICENSE
--rw-r--r--   0        0        0     9041 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/README.md
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    10019 2020-02-02 00:00:00.000000 dup_fmt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/.bumpversion.cfg
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/__about__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/cli.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/exceptions.py
+-rw-r--r--   0        0        0    74758 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/formatter.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/dup_fmt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_errors.py
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_datetime.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_group.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_naming.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_order.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_serial.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_formatter_version.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/test_ralativeserial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/examples/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/examples/test_formatter_datetime.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/examples/test_formatter_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/perfs/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/tests/perfs/perf_fomatter_datetime.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/LICENSE
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/README.md
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 dup_fmt-0.0.3/PKG-INFO
```

### Comparing `dup_fmt-0.0.2/dup_fmt/__init__.py` & `dup_fmt-0.0.3/dup_fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.2/dup_fmt/errors.py` & `dup_fmt-0.0.3/dup_fmt/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
 Define Errors Object for core engine
 """
-from typing import Union
+from __future__ import annotations
+
+from typing import Tuple, Union
 
 
 class BaseError(Exception):
     """Base Error Object that use for catch any errors statement of
     all step in this package.
     """
 
@@ -43,25 +45,27 @@
 
     :param argument: argument of this error that raise to client
     :type argument: Union[str, tuple]
     :param message: string message of this error
     :type message: str
     """
 
-    def __init__(self, argument: Union[str, tuple], message: str):
+    def __init__(self, argument: Union[str, Tuple[str, ...]], message: str):
         """Main Initialization that merge the argument and message input values
         with specific content message together like
 
             `__class__` with `argument`, `message`
         """
-        _argument: str = f"{argument!r}"
+        _argument: str
         if isinstance(argument, tuple):
             _last_arg: str = str(argument[-1])
-            _argument: str = (
+            _argument = (
                 (
                     ", ".join(f"{x!r}" for x in argument[:-1])
                     + f", and {_last_arg!r}"
                 )
                 if len(argument) > 1
                 else f"{_last_arg!r}"
             )
+        else:
+            _argument = f"{argument!r}"
         super().__init__(f"with {_argument}, {message}")
```

### Comparing `dup_fmt-0.0.2/dup_fmt/formatter.py` & `dup_fmt-0.0.3/dup_fmt/formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,34 +3,40 @@
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
 The main object of formatter is able to format every thing you want by less
 config when inherit base class.
 """
+from __future__ import annotations
+
 import re
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from functools import lru_cache, partial, reduce, total_ordering
 from typing import (
     Any,
     Callable,
     Dict,
     List,
+    Literal,
     Optional,
     Tuple,
     Type,
+    TypedDict,
     TypeVar,
     Union,
 )
 
+# TODO: Review ``semver`` package instead ``packaging``.
+#  docs: https://pypi.org/project/semver/
 import packaging.version as pck_version
 from dateutil.relativedelta import relativedelta
 
-from dup_fmt.errors import (
+from dup_fmt.exceptions import (
     FormatterArgumentError,
     FormatterKeyError,
     FormatterTypeError,
     FormatterValueError,
 )
 from dup_fmt.utils import caller, concat, itself, remove_pad
 
@@ -62,29 +68,29 @@
     )
 
     def __init__(self, level: int):
         """Main initialize of the slot object that define a slot list
         with level input value length of False.
         """
         self.level: int = level
-        self.slot: List[bool, ...] = [False] * level
+        self.slot: List[bool] = [False] * level
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(level={self.level})>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.level)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(tuple(self.slot))
 
-    def __eq__(self, other):
+    def __eq__(self, other: Union[SlotLevel, Any]) -> bool:
         return isinstance(other, self.__class__) and self.value == other.value
 
-    def __lt__(self, other):
+    def __lt__(self, other: SlotLevel) -> bool:
         return self.value < other.value
 
     @property
     def count(self) -> int:
         """Return the counting number of True value in the slot.
 
         :rtype: int
@@ -101,15 +107,15 @@
         :return: a sum of weighted value from a True value in any slot
             position.
         """
         return sum(x[0] * int(x[1]) for x in enumerate(self.slot, start=1))
 
     def update(
         self, numbers: Union[int, Tuple[int, ...]], strict: bool = True
-    ) -> "SlotLevel":
+    ) -> SlotLevel:
         """Update value in slot from False to True
 
         :param numbers: updated numbers of this SlotLevel object.
         :type numbers: Union[int, tuple]
         :param strict: a strict flag for raise error when pass out of
             range numbers.
         :type strict: bool(=True)
@@ -119,15 +125,15 @@
         :rtype: SlotLevel
         :return: Self that was updated level
         """
         for num in SlotLevel.make_tuple(numbers):
             if num == 0:
                 continue
             elif 0 <= (_num := (num - 1)) <= (self.level - 1):
-                self.slot[_num]: bool = True
+                self.slot[_num] = True
                 continue
             if strict:
                 raise FormatterValueError(
                     f"number for update the slot level object does not "
                     f"in range of 0 and {self.level}."
                 )
         return self
@@ -146,15 +152,15 @@
 
 
 @dataclass
 class PriorityData:
     """Priority Data class"""
 
     value: Callable = field(default=itself, repr=False)
-    level: Union[int, tuple] = field(default=(0,))
+    level: Union[int, Tuple[int, ...]] = field(default=(0,))
 
 
 @total_ordering
 class BaseFormatter:
     """Base formatter object for inherit to any formatter subclass that define
     format and parse method. The bese class will implement necessary
     properties and method for subclass that should implement or enhance such
@@ -205,15 +211,15 @@
 
     class Config:
         """Base Configuration"""
 
         base_config_value = None
 
     @classmethod
-    def parse(cls, value: str, fmt: Optional[str] = None) -> "BaseFormatter":
+    def parse(cls, value: str, fmt: Optional[str] = None) -> BaseFormatter:
         """Parse string value with its format to subclass of base formatter
         object.
 
         :param value: a string value that match with fmt.
         :type value: str
         :param fmt: a format value will use `cls.base_fmt` if it does not pass
             from input argument.
@@ -229,15 +235,15 @@
             format string.
         """
         _fmt: str = fmt or cls.base_fmt
 
         if not _fmt or isinstance(_fmt, NotImplementedError):
             raise NotImplementedError("This class does not set default format")
 
-        _fmt: str = reduce(
+        _fmt = reduce(
             lambda x, y: x.replace(y, cls.regex()[y]),
             re.findall(r"(%[-+!*]?\w)", _fmt),
             _fmt,
         )
 
         if _search := re.search(rf"^{_fmt}$", value):
             return cls(_search.groupdict())
@@ -251,16 +257,16 @@
     def regex(cls) -> Dict[str, str]:
         """Return mapping of formats and regular expression values of
         `cls.formatter`.
 
         :rtype: Dict[str, str]
         :return: a mapping of format, and it's regular expression string
         """
-        results: dict = {}
-        pre_results: dict = {}
+        results: Dict[str, str] = {}
+        pre_results: Dict[str, str] = {}
         for f, props in cls.formatter().items():
             if "regex" in props:
                 results[f] = props["regex"]
             elif "cregex" in props:
                 pre_results[f] = props["cregex"]
             else:
                 raise FormatterValueError(
@@ -292,32 +298,32 @@
         _formatter: Dict[str, dict] = self.formatter(self.value)
         fmt = fmt.replace("%%", "[ESCAPE]")
         for _sup_fmt in re.findall(r"(%[-+!*]?\w)", fmt):
             try:
                 _value: Union[Callable, str] = _formatter[_sup_fmt]["value"]
                 # FIXME: There shouldn't be any duplicate replaces to the
                 #  previous value
-                fmt: str = fmt.replace(
+                fmt = fmt.replace(
                     _sup_fmt, (_value() if callable(_value) else _value)
                 )
             except KeyError as err:
                 raise FormatterKeyError(
                     f"the format: {_sup_fmt!r} does not support for "
                     f"{self.__class__.__name__!r}"
                 ) from err
         return fmt.replace("[ESCAPE]", "%")
 
-    def __init__(self, formats: Optional[dict] = None):
+    def __init__(self, formats: Optional[Dict] = None):
         """Main initialization get the format mapping from input argument
         and generate the necessary attributes for define the value of this
         base formatter object.
 
             The setter of attribute does not do anything to __slot__ variable.
         """
-        _formats: dict = formats or {}
+        _formats: Dict = formats or {}
 
         # Set level of SlotLevel object that set from `base_level` and pass this
         # value to _level variable for update process in priorities loop.
         setattr(
             self,
             f"_{self.base_attr_prefix}_level",
             SlotLevel(level=self.base_level),
@@ -364,23 +370,23 @@
 
         # Run validate method.
         if not self.validate:
             raise FormatterValueError(
                 "Parsing value does not valid from validator"
             )
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         """Return hashed string value of str property"""
         return hash(self.string)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return string value of str property"""
         return self.string
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Return represent string"""
         return (
             f"<{self.__class__.__name__}"
             f".parse('{self.string}', "
             f"'{self.base_fmt}')>"
         )
 
@@ -544,30 +550,30 @@
         return (
             f"{int(value):0{str(Serial.Config.serial_max_binary)}b}"
             if value
             else ""
         )
 
 
-MONTHS: dict = {
+MONTHS: Dict[str, str] = {
     "Jan": "01",
     "Feb": "02",
     "Mar": "03",
     "Apr": "04",
     "May": "05",
     "Jun": "06",
     "Jul": "07",
     "Aug": "08",
     "Sep": "09",
     "Oct": "10",
     "Nov": "11",
     "Dec": "12",
 }
 
-WEEKS: dict = {
+WEEKS: Dict[str, str] = {
     "Mon": "0",
     "Thu": "1",
     "Wed": "2",
     "Tue": "3",
     "Fri": "4",
     "Sat": "5",
     "Sun": "6",
@@ -595,15 +601,15 @@
         "_dt_minute",
         "_dt_second",
         "_dt_microsecond",
         "_dt_local",
         "_dt_datetime",
     )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"<{self.__class__.__name__}"
             f".parse('{self.string}000', "
             f"'{self.base_fmt}')>"
         )
 
     @property
@@ -1054,15 +1060,15 @@
         "_vs_micro",
         "_vs_pre",
         "_vs_post",
         "_vs_dev",
         "_vs_local",
     )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         _fmt: str = "v%m.%n.%c"
         if self._vs_epoch != "0":
             _fmt: str = f"%e{_fmt[1:]}"
         if self._vs_pre:
             _fmt: str = f"{_fmt}%q"
         if self._vs_post:
             _fmt: str = f"{_fmt}%p"
@@ -1217,17 +1223,15 @@
             },
             "%-e": {
                 "value": lambda: str(_version.epoch),
                 "regex": r"(?P<epoch_num>[0-9]+)",
             },
             "%q": {
                 "value": lambda: (
-                    concat(str(x) for x in _pre)
-                    if (_pre := _version.pre)
-                    else ""
+                    concat(map(str, _pre)) if (_pre := _version.pre) else ""
                 ),
                 "regex": (
                     r"(?P<pre>(a|b|c|rc|alpha|beta|pre|preview)[-_\.]?[0-9]+)"
                 ),
             },
             "%p": {
                 "value": lambda: str(_version.post or ""),
@@ -1667,45 +1671,50 @@
     }
 )
 
 Formatter = TypeVar("Formatter", bound=BaseFormatter)
 
 FormatterType = Type[Formatter]
 
-FORMATTERS: Dict[str, Type[Formatter]] = {
+FORMATTERS: Dict[str, Type[BaseFormatter]] = {
     "timestamp": Datetime,
     "version": Version,
     "serial": Serial,
     "naming": Naming,
     "envconst": EnvConstant,
 }
 
-FORMATTERS_ADJUST: dict = {
+FORMATTERS_ADJUST: Dict[str, Any] = {
     "timestamp": relativedelta,
     "serial": relativedelta,
 }
 
 
+class ExpectRegexValue(TypedDict):
+    regex: str
+    value: Callable[[], Any]
+
+
 def extract_regex_with_value(
     fmt: FormatterType, value: Optional[Any] = None, called: bool = False
-) -> Dict[str, dict]:
+) -> Dict[str, ExpectRegexValue]:
     """Return extract data from `cls.regex` method and `cls.formatter`
 
     :param fmt: a formatter object
     :type fmt: FormatterType
     :param value:
     :type value: Optional[Any]
     :param called: a called flag for extract value if it callable
     :type called: bool(=False)
 
     :rtype: Dict[str, dict]
-    :return: a extract data from `cls.regex` method and `cls.formatter`
+    :return: an extract data from `cls.regex` method and `cls.formatter`
     """
-    regex: dict = fmt.regex()
-    formatter: dict = fmt.formatter(value)
+    regex: Dict[str, str] = fmt.regex()
+    formatter: Dict[str, Dict[str, Union[Callable, str]]] = fmt.formatter(value)
     return {
         i: {
             "regex": regex[i],
             "value": (
                 caller(formatter[i]["value"])
                 if called
                 else formatter[i]["value"]
@@ -1749,37 +1758,37 @@
 
     def __hash__(self):
         return hash(self.number)
 
     def __repr__(self):
         return f"<{self.__class__.__name__}(number={self.number})>"
 
-    def __eq__(self, other: Union[int, "relativeserial"]):
+    def __eq__(self, other: Union[int, relativeserial]):
         if isinstance(other, int):
             return self.number == other
         return self.number == other.number
 
     def __lt__(self, other):
         return self.number < other.number
 
     def __neg__(self):
         return self.__class__(number=-self.number)
 
-    def __rsub__(self, other: Union[int, "relativeserial"]):
+    def __rsub__(self, other: Union[int, relativeserial]):
         return other - self.number
 
-    def __sub__(self, other: Union[int, "relativeserial"]):
+    def __sub__(self, other: Union[int, relativeserial]):
         if isinstance(other, int):
             return self.number - other
         return self.__class__(number=(self.number - other.number))
 
-    def __radd__(self, other: Union[int, "relativeserial"]):
+    def __radd__(self, other: Union[int, relativeserial]):
         return other + self.number
 
-    def __add__(self, other: Union[int, "relativeserial"]):
+    def __add__(self, other: Union[int, relativeserial]):
         if isinstance(other, int):
             return self.__radd__(other)
         return self.__class__(number=(self.number + other.number))
 
 
 # TODO: create relativeversion
 # @total_ordering
@@ -1802,93 +1811,95 @@
         self.alpha: Optional[int] = alpha
         self.beta: Optional[int] = beta
         self.pre: Optional[int] = pre
         self.post: Optional[int] = post
         self.dev: Optional[int] = dev
         self.local: Optional[str] = local
 
-    def __hash__(self):
+    def __hash__(self) -> str:
         return ...
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}()>"
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:  # type: ignore
         return ...
 
-    def __neg__(self):
+    def __neg__(self) -> relativeversion:
         return ...
 
-    def __add__(self, other):
+    def __add__(self, other):  # type: ignore
         return ...
 
-    def __sub__(self, other):
+    def __sub__(self, other):  # type: ignore
         return ...
 
-    def __lt__(self, other):
+    def __lt__(self, other) -> bool:  # type: ignore
         return ...
 
 
 def adjust_datetime(
-    self: "OrderFormatter", metrics: Optional[dict] = None
-) -> "OrderFormatter":
+    self: OrderFormatter, metrics: Optional[Dict[str, int]] = None
+) -> OrderFormatter:
     """
     :param self: a OrderFormatter instance that want to adjust
     :type self: OrderFormatter
     :param metrics: a mapping of metric value
     :type metrics: Optional[dict](=None)
 
     :return: a adjusted OrderFormatter instance.
     """
-    metrics: dict = metrics or {}
+    _metrics: Dict[str, int] = metrics or {}
     if "timestamp" not in self.data:
         raise FormatterArgumentError(
             "timestamp",
             "order file object does not have `timestamp` in name " "formatter",
         )
-    _replace: list = [
+    _replace: List[BaseFormatter] = [
         FORMATTERS["timestamp"].parse(
             **{
-                "value": (time_data.value - relativedelta(**metrics)).strftime(
+                "value": (time_data.value - relativedelta(**_metrics)).strftime(
                     "%Y%m%d %H%M%S"
                 ),
                 "fmt": "%Y%m%d %H%M%S",
             }
         )
         for time_data in self.data["timestamp"]
     ]
-    self.data["timestamp"]: list = _replace
+    self.data["timestamp"]: List[BaseFormatter] = _replace
     return self
 
 
-def adjust_serial(self: "OrderFormatter", metrics: Optional[dict] = None):
+def adjust_serial(
+    self: OrderFormatter, metrics: Optional[Dict[str, int]] = None
+) -> OrderFormatter:
     """
     :param self: a OrderFormatter instance that want to adjust
     :type self: OrderFormatter
     :param metrics: a mapping of metric value
     :type metrics: Optional[dict](=None)
 
     :return: a adjusted OrderFormatter instance.
     """
-    metrics: dict = metrics or {}
+    _metrics: Dict[str, int] = metrics or {}
     if "serial" not in self.data:
         raise FormatterArgumentError(
             "serial",
             "order file object does not have `serial` in name " "formatter",
         )
-    _replace: list = [
+    _replace: List[BaseFormatter] = [
         FORMATTERS["serial"].parse(
             **{
-                "value": (str(serial.value - relativeserial(**metrics))),
+                "value": (str(serial.value - relativeserial(**_metrics))),
                 "fmt": "%n",
             }
         )
         for serial in self.data["serial"]
     ]
-    self.data["serial"]: list = _replace
+    self.data["serial"] = _replace
     return self
 
 
 # def adjust_version():
 #     ...
 #
 # def adjust_name():
@@ -1904,66 +1915,74 @@
 
     :raises TypeError: if value of mapping does not match with dict or
         BaseFormatter type.
     """
 
     __slots__ = ("data",)
 
-    def __init__(self, formatters: Dict[str, Union[Formatter, dict]]):
+    def __init__(
+        self, formatters: Dict[str, Union[BaseFormatter, Dict[str, Any]]]
+    ):
         """Main initialize process of the ordering formatter object."""
-        self.data: dict = {}
+        self.data: Dict[str, List[BaseFormatter]] = {}
         # TODO: add merge_dict function to mapping by {'serial': ...}
         #  before for-loop process
         for name in formatters:
             _name: str = re.sub(r"(_\d+)$", "", name)
-            name_value: list = self.data.setdefault(_name, [])
-            if isinstance(formatters[name], dict) and _name in FORMATTERS:
+
+            if _name not in FORMATTERS:
+                raise FormatterValueError(
+                    f"value of key {_name} does not support"
+                )
+
+            name_value: List[BaseFormatter] = self.data.setdefault(_name, [])
+            if isinstance(formatters[name], dict):
                 name_value.append(FORMATTERS[_name].parse(**formatters[name]))
-            elif isinstance(formatters[name], (dict, BaseFormatter)):
+            elif isinstance(formatters[name], BaseFormatter):
                 name_value.append(formatters[name])
             else:
                 raise FormatterTypeError(
                     f"value of key {_name} does not support for type "
                     f"{type(formatters[name])}"
                 )
 
-    def adjust(self, fmt: str, value: int):  # no cov
+    def adjust(self, fmt: str, value: int):  # type: ignore  # no cov
         # TODO: merge adjust methods to dynamic method
         if fmt not in self.data:
             raise FormatterArgumentError(
                 fmt,
                 f"order object does not have `{fmt}` in name " f"formatter",
             )
         return self
 
-    def adjust_timestamp(self, value: int) -> "OrderFormatter":
+    def adjust_timestamp(self, metrics: Dict[str, int]) -> OrderFormatter:
         """Adjust timestamp value in the order formatter object
 
-        :param value: a datetime value for this adjustment.
-        :type value: int
+        :param metrics: a datetime value for this adjustment.
+        :type metrics: Dict[str, int]
         """
-        return adjust_datetime(self, metrics={"months": value})
+        return adjust_datetime(self, metrics=metrics)
 
-    def adjust_version(self, value: str) -> "OrderFormatter":
+    def adjust_version(self, value: str) -> OrderFormatter:
         """Adjust version value in the order formatter object
 
         :param value: str : A version value for this adjustment with format
                 '%m.%n.%c'.
         """
         if "version" not in self.data:
             raise FormatterArgumentError(
                 "version",
                 "order file object does not have `version` "
                 "in name formatter",
             )
-        _replace: list = []
+        _replace: List[BaseFormatter] = []
         for version_data in self.data["version"]:
             # `versioning` must have 3 length of tuple
             versioning: Tuple[int, ...] = version_data.value.release
-            _values: List[int, ...] = [
+            _values: List[int] = [
                 -99 if v == "*" else int(v) for v in value.split(".")
             ]
             _results: List[str] = []
 
             # TODO: create function: `relativedelta` for version object
             for _ in range(3):
                 if _values[_] == 0:
@@ -1975,77 +1994,84 @@
                 else:
                     _results.append(str(major))
             _replace.append(
                 FORMATTERS["version"].parse(
                     **{"value": ".".join(_results), "fmt": "%m.%n.%c"}
                 )
             )
-        self.data["version"]: list = _replace
+        self.data["version"] = _replace
         return self
 
-    def adjust_serial(self, value: int) -> "OrderFormatter":
+    def adjust_serial(self, value: int) -> OrderFormatter:
         """Adjust serial value in the order formatter object
 
         .. note:: This adjust method will replace old value to new.
         """
         return adjust_serial(self, metrics={"number": value})
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(formatters={self.data})>"
 
     def __str__(self) -> str:
         return f"({', '.join([f'{k}={list(map(str, v))}' for k, v in self.data.items()])})"
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, self.__class__) and self.data == other.data
 
-    def __lt__(self, other):
+    def __lt__(self, other: OrderFormatter) -> bool:
         return next(
             (
                 self.data[name] < other.data[name]
                 for name in FORMATTERS
                 if (name in self.data and name in other.data)
             ),
             False,
         )
 
-    def __le__(self, other):
+    def __le__(self, other: OrderFormatter) -> bool:
         return next(
             (
                 self.data[name] <= other.data[name]
                 for name in FORMATTERS
                 if (name in self.data and name in other.data)
             ),
             self.__eq__(other),
         )
 
 
+class FormatterGroupParseArgs(TypedDict):
+    fmt: FormatterType[Any]
+    value: Optional[str]
+
+
 @dataclass
 class FormatterGroupData:
     """Formatter Data"""
 
-    fmt: FormatterType
+    fmt: FormatterType[Any]
     value: Any
 
     @classmethod
-    def parse(cls, value: Union[dict, Type[Formatter]]):
+    def parse(
+        cls, value: Union[FormatterGroupParseArgs, Type[Formatter]]
+    ) -> FormatterGroupData:
         """Parse any value to this FormatterGroupData class
 
         :param value: a value that want to parse
         :type value: Union[dict, Type[Formatter]]
         """
         if isinstance(value, dict):
             return cls.parse_dict(value)
         return cls(
             fmt=value,
             value=None,
         )
 
     @classmethod
-    def parse_dict(cls, values: dict):
+    def parse_dict(cls, values: FormatterGroupParseArgs) -> FormatterGroupData:
         """Parse dict value to this FormatterGroupData class
 
         :param values: a dict value
         :type values: dict
         """
         return cls(
             fmt=values["fmt"],
@@ -2061,111 +2087,124 @@
     :type formatters: Dict[str, dict]
     """
 
     __slots__ = "formatters"
 
     def __init__(
         self,
-        formatters: Dict[str, Union[FormatterGroupData, dict, Type[Formatter]]],
+        formatters: Dict[
+            str,
+            Union[FormatterGroupData, FormatterGroupParseArgs, Type[Formatter]],
+        ],
     ):
         """Main initialization get the formatter value, a mapping of name
         and formatter from input argument and generate the necessary
         attributes for define the value of this formatter group object.
         """
         self.formatters: Dict[str, FormatterGroupData] = {
             k: v
             if isinstance(v, FormatterGroupData)
             else FormatterGroupData.parse(v)
             for k, v in formatters.items()
         }
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({', '.join(self.formatters)})"
 
     @property
-    def groups(self) -> Dict[str, Formatter]:
+    def groups(self) -> Dict[str, Dict[str, ExpectRegexValue]]:
         """Return the groups of format value and extract Formatter
         values.
         """
         return {
             k: extract_regex_with_value(v.fmt, v.value)
             for k, v in self.formatters.items()
         }
 
-    def parser(self, value: str, fmt: str, _max: bool = True) -> dict:
+    def parser(
+        self, value: str, fmt: str, _max: bool = True
+    ) -> Dict[str, Formatter]:
         """Parse formatter by generator values like timestamp, version,
         or serial.
 
         :param value:
         :type value: str
         :param fmt:
         :type fmt: str
         :param _max: the max strategy for pick the maximum level from
             duplication formats in parser method.
         :type _max: bool(=True)
         """
         results, _ = self.__parser_all(value, fmt)
-        rs: dict = {}
+        if _max:
+            return self.__parser_max(results=results)
+
+        rs: Dict[str, Dict[str, str]] = {}
         for result in results:
             if (k := result.split("__", maxsplit=1)[0]) in rs:
-                if _max:
-                    rs[k].append(
-                        self.formatters[k].fmt.parse(**results[result])
-                    )
-                else:
-                    rs[k]["fmt"] += f"__{results[result]['fmt']}"
-                    rs[k]["value"] += f"__{results[result]['value']}"
-            elif _max:
-                rs[k] = [self.formatters[k].fmt.parse(**results[result])]
+                rs[k]["fmt"] += f"__{results[result]['fmt']}"
+                rs[k]["value"] += f"__{results[result]['value']}"
             else:
                 rs[k] = results[result]
-        return {
-            k: max(v, key=lambda x: x.level.value)
-            if _max
-            else self.formatters[k].fmt.parse(**v)
-            for k, v in rs.items()
-        }
+        return {k: self.formatters[k].fmt.parse(**v) for k, v in rs.items()}
+
+    def __parser_max(
+        self, results: Dict[str, Dict[str, str]]
+    ) -> Dict[str, Formatter]:
+        rs: Dict[str, List[Formatter]] = {}
+        for result in results:
+            if (k := result.split("__", maxsplit=1)[0]) in rs:
+                rs[k].append(self.formatters[k].fmt.parse(**results[result]))
+            else:
+                rs[k] = [self.formatters[k].fmt.parse(**results[result])]
+
+        def get_level_value(fmt: Formatter) -> int:
+            return fmt.level.value
+
+        return {k: max(v, key=get_level_value) for k, v in rs.items()}
 
     def format(self, fmt: str) -> str:
         """Fill the formatter to value input argument.
 
         :param fmt: a string format value
         :type fmt: str
         """
         for fmt_name, fmt_mapping in self.groups.items():
             # Case I: contain formatter values.
             for _search in re.finditer(
                 rf"(?P<name>{{{fmt_name}:(?P<format>[^{{}}]+)?}})", fmt
             ):
-                fmt: str = fmt.replace(
+                fmt = fmt.replace(
                     f'{{{fmt_name}:{_search.groupdict()["format"]}}}',
                     self.__loop_sub_fmt(
                         search=_search, mapping=fmt_mapping, key="value"
                     ),
                 )
             # Case II: does not set any formatter value or duplicate format
             # name but does not set formatter.
             if re.search(rf"(?P<name>{{{fmt_name}}})", fmt):
                 # Get the first format value from the formatter property.
-                fmt: str = fmt.replace(
+                fmt = fmt.replace(
                     f"{{{fmt_name}}}",
                     caller(fmt_mapping[list(fmt_mapping.keys())[0]]["value"]),
                 )
         return fmt
 
-    def __parser_all(self, value: str, fmt: str) -> Tuple[dict, dict]:
+    def __parser_all(
+        self, value: str, fmt: str
+    ) -> Tuple[Dict[str, Dict[str, str]], Dict[str, str]]:
         """Parse all formatter by generator that return getter and outer
         mapping.
 
         :param value:
         :type value: str
         :param fmt:
         :type fmt:  str
 
-        :rtype: Tuple[dict, dict]
+        :rtype: Tuple[Dict[str, Dict[str, str]], Dict[str, str]]
         :returns: a pair of mappings, like;
 
             {
                 'name': {'fmt': '%s', 'value': 'data_engineer'},
                 'name__1': {'fmt': '%a', 'value': 'de'},
                 'datetime': {'fmt': '%Y%m%d', 'value': '20220101'}
             }
@@ -2177,70 +2216,72 @@
         if not (_search := re.search(rf"^{_fmt_filled}$", value)):
             raise FormatterArgumentError(
                 "format",
                 f"{value!r} does not match with the format: "
                 f"'^{_fmt_filled}$'",
             )
 
-        _searches: dict = _search.groupdict()
-        _fmt_outer: dict = {}
+        _searches: Dict[str, str] = _search.groupdict()
+        _fmt_outer: Dict[str, str] = {}
         for name in _searches.copy():
             if name in _fmt_getter:
-                _fmt_getter[name]["value"]: str = _searches.pop(name)
+                _fmt_getter[name]["value"] = _searches.pop(name)
             else:
-                _fmt_outer[name]: str = _searches.pop(name)
+                _fmt_outer[name] = _searches.pop(name)
 
         return _fmt_getter, _fmt_outer
 
-    def __stage_parser(self, fmt: str) -> Tuple[str, dict]:
+    def __stage_parser(self, fmt: str) -> Tuple[str, Dict[str, Dict[str, str]]]:
         """Return the both of filled and getter format from the stage format
         value.
 
         :param fmt: a string format
         :type fmt: str
 
-        :rtype: Tuple[str, dict]
+        :rtype: Tuple[str, Dict[str, Dict[str, str]]]
         :returns: a pair of format value and result of regular expression.
         """
-        _get_format: dict = {}
+        _get_format: Dict[str, Dict[str, str]] = {}
         for fmt_name, fmt_mapping in self.groups.items():
             for _index, _search in enumerate(
                 re.finditer(
                     rf"(?P<name>{{{fmt_name}:?(?P<format>[^{{}}]+)?}})", fmt
                 ),
                 start=1,
             ):
+                _search_fmt: str
+                _search_fmt_re: str
                 _search_fmt_old: str = ""
                 if _search_fmt := _search.group("format"):
                     # Case I: contain formatter values.
-                    _search_fmt_old: str = f":{_search_fmt}"
-                    _search_fmt_re: str = self.__loop_sub_fmt(
+                    _search_fmt_old = f":{_search_fmt}"
+                    _search_fmt_re = self.__loop_sub_fmt(
                         search=_search,
                         mapping=fmt_mapping,
                         key="regex",
                         index=_index,
                     )
                 else:
                     # Case II: does not set any formatter value.
-                    _search_fmt: str = list(fmt_mapping.keys())[0]
-                    _search_fmt_re: str = fmt_mapping[_search_fmt]["regex"]
+                    _search_fmt = list(fmt_mapping.keys())[0]
+                    _search_fmt_re = fmt_mapping[_search_fmt]["regex"]
 
                 # Replace old format value with new mapping formatter
                 # value.
                 _fmt_name_index: str = (
                     f"{fmt_name}{self.__generate_index(_index)}"
                 )
-                fmt: str = fmt.replace(
+                fmt = fmt.replace(
                     f"{{{fmt_name}{_search_fmt_old}}}",
                     f"(?P<{_fmt_name_index}>{_search_fmt_re})",
                     1,
                 )
 
                 # Keep the searched format value to getter format dict.
-                _get_format[_fmt_name_index]: dict = {"fmt": _search_fmt}
+                _get_format[_fmt_name_index] = {"fmt": _search_fmt}
         return fmt, _get_format
 
     @staticmethod
     def __generate_index(index: int) -> str:
         """Return generated suffix string for duplication values.
 
         :param index: an index value.
@@ -2250,52 +2291,56 @@
         :return: a suffix string value for adding to index name when name
             was duplicated from string formatter.
         """
         return f"__{str(index - 1)}" if index > 1 else ""
 
     @staticmethod
     def __loop_sub_fmt(
-        search: re.Match, mapping: dict, key: str, index: int = 1
+        search: re.Match[str],
+        mapping: Dict[str, ExpectRegexValue],
+        key: Literal["regex", "value"],
+        index: int = 1,
     ) -> str:
         """Loop method for find any sub-format from search input argument.
 
         :param search: a Match object from searching process.
         :type search: re.Match
         :param mapping: a formatter mapping value for getting matching key.
-        :type mapping: dict
+        :type mapping: Dict[
+                str, Dict[str, Dict[str, Union[str, Callable[[], Any]]]]
+            ]
         :param key: A key value for get value from the `mapping` parameter.
         :type key: str
         :param index:
         :type index: int(=1)
 
         :rtype: str
         :returns: a searched value
         """
         assert key in {
             "value",
             "regex",
         }, "the `key` argument should be 'value' or 'regex' only."
-        _search_dict: dict = search.groupdict()
+        _search_dict: Dict[str, str] = search.groupdict()
         _search_re: str = _search_dict["format"]
         for _fmt in re.findall(r"(%[-+!*]?\w)", _search_re):
             try:
-                # print(mapping)
                 _fmt_replace: str = caller(mapping[_fmt][key])
                 if index > 1 and (
                     _sr := re.search(
                         r"\(\?P<(?P<alias_name>\w+)>", _fmt_replace
                     )
                 ):
                     _sr_re: str = _sr.groupdict()["alias_name"]
-                    _fmt_replace: str = re.sub(
+                    _fmt_replace = re.sub(
                         rf"\(\?P<{_sr_re}>",
                         rf"(?P<{_sr_re}_{str(index - 1)}>",
                         _fmt_replace,
                     )
-                _search_re: str = _search_re.replace(_fmt, _fmt_replace)
+                _search_re = _search_re.replace(_fmt, _fmt_replace)
             except KeyError as err:
                 raise FormatterArgumentError(
                     "format",
                     f'string formatter of {_search_dict["name"]!r} does not '
                     f"support for key {str(err)} in configuration",
                 ) from err
         return _search_re
```

### Comparing `dup_fmt-0.0.2/dup_fmt/utils.py` & `dup_fmt-0.0.3/dup_fmt/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import Any, Callable, Union
+from __future__ import annotations
 
-concat: Callable = "".join
+from typing import Any, Callable, Iterable, List, Union
+
+concat: Callable[[Union[List[str], Iterable[str]]], str] = "".join
 
 
 def remove_pad(value: str) -> str:
     """Remove zero padding of string
     .. usage::
         >>> remove_pad('000')
         '0'
@@ -19,15 +21,15 @@
 
 
 def itself(x: Any = None) -> Any:
     """Return itself value"""
     return x
 
 
-def caller(func: Union[Callable, Any]) -> Any:
+def caller(func: Union[Callable[[], Any], Any]) -> Any:
     """Call function if it was callable
     .. usage::
         >>> some_func = lambda: 100
         >>> caller(some_func)
         100
     """
     return func() if callable(func) else func
```

### Comparing `dup_fmt-0.0.2/tests/test_errors.py` & `dup_fmt-0.0.3/tests/test_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # license information.
 # --------------------------------------------------------------------------
 """
 Test the error object.
 """
 import unittest
 
-import dup_fmt.errors as err
+import dup_fmt.exceptions as err
 
 
 class ErrorsTestCase(unittest.TestCase):
     def setUp(self) -> None:
         ...
 
     def test_err_config_str_arg(self):
```

### Comparing `dup_fmt-0.0.2/tests/test_examples.py` & `dup_fmt-0.0.3/tests/examples/test_formatter_datetime.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,25 @@
 # -------------------------------------------------------------------------
 # Copyright (c) 2022 Korawich Anuttra. All rights reserved.
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
-Test the formatter object examples.
+Test the formatter object examples for Datetime.
 """
 import unittest
 from datetime import datetime
 
-from packaging.version import Version
-
 import dup_fmt.formatter as fmt
 
 
 class DatetimeExampleTestCase(unittest.TestCase):
     def test_parse_examples(self):
         self.assertEqual(
             datetime(2021, 1, 1, microsecond=135000),
             fmt.Datetime.parse("2021-01-1 135043", "%Y-%m-%-d %f").value,
         )
         # FIXME: this datetime does not match with monday in this week
         self.assertEqual(
             datetime(2021, 1, 3),
             fmt.Datetime.parse("2021-Jan Monday 3", "%Y-%b %A %-d").value,
         )
-
-
-class VersionExampleTestCase(unittest.TestCase):
-    def test_parse_examples(self):
-        self.assertEqual(
-            Version("1.0.5"),
-            fmt.Version.parse("version: 1-0-5", "version: %m-%n-%c").value,
-        )
```

### Comparing `dup_fmt-0.0.2/tests/test_formatter.py` & `dup_fmt-0.0.3/tests/test_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 Test the formatter object.
 """
 import unittest
 from typing import Dict, Optional, Type
 
 import dup_fmt.formatter as fmt
-from dup_fmt.errors import FormatterValueError
+from dup_fmt.exceptions import FormatterValueError
 
 
 class SlotLevelTestCase(unittest.TestCase):
     def setUp(self) -> None:
         self.sl = fmt.SlotLevel(level=5)
         self.sl.update(numbers=(2, 3, 4))
```

### Comparing `dup_fmt-0.0.2/tests/test_formatter_datetime.py` & `dup_fmt-0.0.3/tests/test_formatter_datetime.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.2/tests/test_formatter_group.py` & `dup_fmt-0.0.3/tests/test_formatter_group.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.2/tests/test_formatter_naming.py` & `dup_fmt-0.0.3/tests/test_formatter_naming.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.2/tests/test_formatter_order.py` & `dup_fmt-0.0.3/tests/test_formatter_order.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # Licensed under the MIT License. See LICENSE in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
 Test the formatter object.
 """
 import unittest
-from typing import Dict, List
+from typing import Any, Dict, List
 
 import dup_fmt.formatter as fmt
-from dup_fmt.errors import FormatterTypeError
+from dup_fmt.exceptions import FormatterTypeError, FormatterValueError
 
 
 class OrderFormatTestCase(unittest.TestCase):
     def setUp(self) -> None:
         # Set up Datetime formatter
         self.dt = fmt.Datetime.parse("20220101", "%Y%m%d")
         self.dt2 = fmt.Datetime.parse("20220102", "%Y%m%d")
@@ -27,14 +27,23 @@
 
         self.fmt_order = fmt.OrderFormatter({"timestamp": self.dt})
         self.fmt_order2 = fmt.OrderFormatter({"timestamp": self.dt2})
         self.fmt_order3 = fmt.OrderFormatter({"version": self.vs})
         self.fmt_order4 = fmt.OrderFormatter({"version": self.vs2})
         self.fmt_order5 = fmt.OrderFormatter({"serial": self.sr_dict})
         self.fmt_order6 = fmt.OrderFormatter({"serial": self.sr_dict2})
+        # self.fmt_order7 = fmt.OrderFormatter({"number": self.sr_dict2})
+
+    def test_order_raise_name_init(self):
+        raise_respec: Dict[str, Dict[Any, Any]] = {"number": self.sr_dict2}
+        with self.assertRaises(FormatterValueError) as context:
+            fmt.OrderFormatter(raise_respec)  # type: ignore
+        self.assertTrue(
+            "value of key number does not support" in str(context.exception)
+        )
 
     def test_order_raise_type_init(self):
         raise_respec: Dict[str, List[str]] = {"timestamp": ["20210101"]}
         with self.assertRaises(FormatterTypeError) as context:
             fmt.OrderFormatter(raise_respec)  # type: ignore
         self.assertTrue(
             (
@@ -76,20 +85,20 @@
         self.assertFalse(self.fmt_order6 < self.fmt_order)
         self.assertFalse(self.fmt_order6 <= self.fmt_order)
         self.assertTrue(self.fmt_order6 != self.fmt_order)
 
     def test_order_datetime_adjust(self):
         self.assertEqual(
             "(timestamp=['2021-12-01 00:00:00.000'])",
-            self.fmt_order.adjust_timestamp(value=1).__str__(),
+            self.fmt_order.adjust_timestamp(metrics={"months": 1}).__str__(),
         )
 
     def test_order_datetime_adjust_raise(self):
         with self.assertRaises(fmt.FormatterArgumentError) as context:
-            self.fmt_order3.adjust_timestamp(value=1)
+            self.fmt_order3.adjust_timestamp(metrics={"months": 1})
         self.assertTrue(
             (
                 "with 'timestamp', order file object does not have "
                 "`timestamp` in name formatter"
             )
             in str(context.exception)
         )
```

### Comparing `dup_fmt-0.0.2/tests/test_formatter_serial.py` & `dup_fmt-0.0.3/tests/test_formatter_serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # --------------------------------------------------------------------------
 """
 Test the Serial formatter object.
 """
 import unittest
 
 import dup_fmt.formatter as fmt
-from dup_fmt.errors import FormatterKeyError
+from dup_fmt.exceptions import FormatterKeyError
 
 
 class SerialTestCase(unittest.TestCase):
     def setUp(self) -> None:
         self.sr = fmt.Serial({"number": "781"})
         self.sr_default: fmt.Formatter = fmt.Serial()
         self.sr_p: fmt.Formatter = fmt.Serial.parse("009", "%p")
```

### Comparing `dup_fmt-0.0.2/tests/test_formatter_version.py` & `dup_fmt-0.0.3/tests/test_formatter_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Test the Version formatter object.
 """
 import unittest
 
 from packaging.version import Version
 
 import dup_fmt.formatter as fmt
-from dup_fmt.errors import FormatterValueError
+from dup_fmt.exceptions import FormatterValueError
 
 
 class VersionTestCase(unittest.TestCase):
     def setUp(self) -> None:
         self.maxDiff = None
         self.vs = fmt.Version(
             {
```

### Comparing `dup_fmt-0.0.2/tests/test_ralativeserial.py` & `dup_fmt-0.0.3/tests/test_ralativeserial.py`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.2/.gitignore` & `dup_fmt-0.0.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 # GitHub Action
 #  Want to add htmlcov/ to coverage branch
-# htmlcov/
+htmlcov/
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
```

### Comparing `dup_fmt-0.0.2/LICENSE` & `dup_fmt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dup_fmt-0.0.2/README.md` & `dup_fmt-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Data Utility Package: *Formatter*
 
 [![test](https://github.com/korawica/dup-fmt/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/dup-fmt/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/korawica/dup-fmt/branch/main/graph/badge.svg?token=J2MN63IFT0)](https://codecov.io/gh/korawica/dup-fmt)
 [![python support version](https://img.shields.io/pypi/pyversions/dup-fmt)](https://pypi.org/project/dup-fmt/)
 [![size](https://img.shields.io/github/languages/code-size/korawica/dup-fmt)](https://github.com/korawica/dup-fmt)
 
-**Type**: `DUP` | **Tag**: `Data Utility Package` `Data` `Utility`
+**Type**: `DUP` | **Tag**: `Data Utility Package` `Data` `Utility` `Formatter`
 
 **Table of Contents**:
 
 - [Formatter Objects](#formatter-objects)
   - [Datetime](#datetime)
   - [Version](#version)
   - [Serial](#serial)
@@ -17,15 +17,15 @@
   - [Constant](#constant)
 - [Ordered Formatter](#ordered-formatter)
 - [Formatter Group](#formatter-group)
 - [Make your Formatter Object](#make-your-formatter-object)
 
 This **Formatter** package was created for `parse` and `format` any string values
 that able to design format pattern with regular expression. This package be the
-co-pylot project for stating to my Python software developer role.
+co-pylot project for stating to my **Python Software Developer** role.
 
 **Install from PyPI**:
 
 ```shell
 pip install dup-fmt
 ```
 
@@ -145,15 +145,15 @@
 >>> 'Camel case is dataEngineer'
 ```
 
 ### Constant
 
 ```python
 from dup_fmt import Constant
-from dup_fmt.errors import FormatterError
+from dup_fmt.exceptions import FormatterError
 
 const = Constant({
     '%n': 'normal',
     '%s': 'special',
 })
 try:
     parse_const = const.parse(
```

### Comparing `dup_fmt-0.0.2/pyproject.toml` & `dup_fmt-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,93 @@
 [build-system]
-requires = ["hatchling"]
+requires = [
+    "hatchling>=1.8.0",
+    # This plug-in support for py-version >= 3.9
+    # "hatch-semver",
+]
 build-backend = "hatchling.build"
 
 [project]
 name = "dup-fmt"
 description = "The utility formatter objects for the data engine package"
 readme = "README.md"
 requires-python = ">=3.8.10"
 license = "MIT"
-keywords = []
+keywords = [
+    'data',
+    'formatter',
+]
 authors = [
     { name = "korawica", email = "korawich.anu@gmail.com" },
 ]
 classifiers = [
     "Topic :: Utilities",
+    "Natural Language :: English",
+    #"Development Status :: 3 - Alpha",
     "Development Status :: 4 - Beta",
+    #"Development Status :: 5 - Production/Stable",
+    "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "python-dateutil>=2.8.2,<3.0.0",
     "packaging>=23.1,<24",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://github.com/korawica/dup-fmt"
+Homepage = "https://github.com/korawica/dup-fmt/"
+"Source Code" = "https://github.com/korawica/dup-fmt/"
 
 [project.optional-dependencies]
 test = [
-    "pytest>=7.1.3,<8.0.0",
-    "coverage[toml]",
-    "mypy==0.982",
+    "pytest>=7.1.3",
+    "coverage[toml]>=7.0.0",
+    "mypy>=0.982",
+    "types-python-dateutil",
 ]
 dev = [
-    "ruff==0.0.138",
-    "pre-commit>=2.17.0,<3.0.0"
+    "hatch>=1.6.0",
+    "ruff>=0.0.138",
+    "pre-commit>=2.17.0",
+    "bump2version>=1.0.1"
 ]
 
+# TODO: Implement cli for use on cmd
+# [project.scripts]
+# dupfmt = "dup_fmt.cli:main"
+
 [tool.coverage.run]
 branch = true
+concurrency = ["thread", "multiprocessing"]
 parallel = true
 context = '${CONTEXT}'
 source = [
-    "tests",
-    "dup_fmt"
+    "dup_fmt",
 ]
 omit = [
+    "dup_fmt/__about__.py",
     "dup_fmt/utils.py",
 ]
 relative_files = true
 
 [tool.coverage.report]
 exclude_lines = [
     "no cov",
-    "if __name__ == .__main__.:",
+    "if __name__ == __main__:",
     "if TYPE_CHECKING:",
 ]
 
 [tool.hatch.version]
+scheme = "standard"
 source = "code"
 path = "dup_fmt/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     "/.github",
     "/docs",
@@ -85,17 +108,46 @@
 
 [tool.mypy]
 python_version = "3.8"
 files = ["dup_fmt"]
 show_error_codes = true
 pretty = true
 strict = true
-local_partial_types = true
+#local_partial_types = true
 warn_unreachable = true
 
+[[tool.mypy.overrides]]
+module = "dup_fmt.utils"
+warn_unused_ignores = false
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "tests.*"
+ignore_missing_imports = true
+check_untyped_defs = true
+
+[tool.black]
+line-length = 80
+target-version = ['py38']
+exclude = """
+/(
+    \\.git
+    | \\.__pycache__
+    | \\.idea
+    | \\.ruff_cache
+    | \\.mypy_cache
+    | \\.pytest_cache
+    | \\.venv
+    | _build
+    | buck-out
+    | build
+    | dist
+)/
+"""
+
 [tool.ruff]
 line-length = 80
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
```

### Comparing `dup_fmt-0.0.2/PKG-INFO` & `dup_fmt-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 Metadata-Version: 2.1
 Name: dup-fmt
-Version: 0.0.2
+Version: 0.0.3
 Summary: The utility formatter objects for the data engine package
-Project-URL: Homepage, https://github.com/korawica/dup-fmt
+Project-URL: Homepage, https://github.com/korawica/dup-fmt/
+Project-URL: Source Code, https://github.com/korawica/dup-fmt/
 Author-email: korawica <korawich.anu@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
+Keywords: data,formatter
 Classifier: Development Status :: 4 - Beta
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8.10
 Requires-Dist: packaging<24,>=23.1
 Requires-Dist: python-dateutil<3.0.0,>=2.8.2
 Provides-Extra: dev
-Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
-Requires-Dist: ruff==0.0.138; extra == 'dev'
+Requires-Dist: bump2version>=1.0.1; extra == 'dev'
+Requires-Dist: hatch>=1.6.0; extra == 'dev'
+Requires-Dist: pre-commit>=2.17.0; extra == 'dev'
+Requires-Dist: ruff>=0.0.138; extra == 'dev'
 Provides-Extra: test
-Requires-Dist: coverage[toml]; extra == 'test'
-Requires-Dist: mypy==0.982; extra == 'test'
-Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
+Requires-Dist: coverage[toml]>=7.0.0; extra == 'test'
+Requires-Dist: mypy>=0.982; extra == 'test'
+Requires-Dist: pytest>=7.1.3; extra == 'test'
+Requires-Dist: types-python-dateutil; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Data Utility Package: *Formatter*
 
 [![test](https://github.com/korawica/dup-fmt/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/dup-fmt/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/korawica/dup-fmt/branch/main/graph/badge.svg?token=J2MN63IFT0)](https://codecov.io/gh/korawica/dup-fmt)
 [![python support version](https://img.shields.io/pypi/pyversions/dup-fmt)](https://pypi.org/project/dup-fmt/)
 [![size](https://img.shields.io/github/languages/code-size/korawica/dup-fmt)](https://github.com/korawica/dup-fmt)
 
-**Type**: `DUP` | **Tag**: `Data Utility Package` `Data` `Utility`
+**Type**: `DUP` | **Tag**: `Data Utility Package` `Data` `Utility` `Formatter`
 
 **Table of Contents**:
 
 - [Formatter Objects](#formatter-objects)
   - [Datetime](#datetime)
   - [Version](#version)
   - [Serial](#serial)
@@ -43,15 +52,15 @@
   - [Constant](#constant)
 - [Ordered Formatter](#ordered-formatter)
 - [Formatter Group](#formatter-group)
 - [Make your Formatter Object](#make-your-formatter-object)
 
 This **Formatter** package was created for `parse` and `format` any string values
 that able to design format pattern with regular expression. This package be the
-co-pylot project for stating to my Python software developer role.
+co-pylot project for stating to my **Python Software Developer** role.
 
 **Install from PyPI**:
 
 ```shell
 pip install dup-fmt
 ```
 
@@ -171,15 +180,15 @@
 >>> 'Camel case is dataEngineer'
 ```
 
 ### Constant
 
 ```python
 from dup_fmt import Constant
-from dup_fmt.errors import FormatterError
+from dup_fmt.exceptions import FormatterError
 
 const = Constant({
     '%n': 'normal',
     '%s': 'special',
 })
 try:
     parse_const = const.parse(
```


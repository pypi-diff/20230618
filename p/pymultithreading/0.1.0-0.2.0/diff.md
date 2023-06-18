# Comparing `tmp/pymultithreading-0.1.0.tar.gz` & `tmp/pymultithreading-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultithreading-0.1.0.tar", last modified: Sat Jun 17 15:09:30 2023, max compression
+gzip compressed data, was "pymultithreading-0.2.0.tar", last modified: Sun Jun 18 08:05:59 2023, max compression
```

## Comparing `pymultithreading-0.1.0.tar` & `pymultithreading-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:09:30.915073 pymultithreading-0.1.0/
--rw-rw-rw-   0        0        0       98 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2045 2023-06-17 15:09:30.914075 pymultithreading-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.1.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.1.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:09:30.899039 pymultithreading-0.1.0/multithreading/
--rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.1.0/multithreading/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.1.0/multithreading/base.py
--rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.1.0/multithreading/document.py
--rw-rw-rw-   0        0        0    10505 2023-06-17 14:58:52.000000 pymultithreading-0.1.0/multithreading/process.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:09:30.913104 pymultithreading-0.1.0/pymultithreading.egg-info/
--rw-rw-rw-   0        0        0     2045 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.1.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 15:09:30.915073 pymultithreading-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1561 2023-06-17 15:09:21.000000 pymultithreading-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:05:59.893159 pymultithreading-0.2.0/
+-rw-rw-rw-   0        0        0       98 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2045 2023-06-18 08:05:59.893159 pymultithreading-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.2.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.2.0/build.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:05:59.877154 pymultithreading-0.2.0/multithreading/
+-rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.2.0/multithreading/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.2.0/multithreading/base.py
+-rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.2.0/multithreading/document.py
+-rw-rw-rw-   0        0        0    12586 2023-06-18 08:05:34.000000 pymultithreading-0.2.0/multithreading/process.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:05:59.892158 pymultithreading-0.2.0/pymultithreading.egg-info/
+-rw-rw-rw-   0        0        0     2045 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pymultithreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-06-18 08:05:59.000000 pymultithreading-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 08:05:59.894159 pymultithreading-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-06-18 08:05:50.000000 pymultithreading-0.2.0/setup.py
```

### Comparing `pymultithreading-0.1.0/PKG-INFO` & `pymultithreading-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.1.0/README.md` & `pymultithreading-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.1.0/build.py` & `pymultithreading-0.2.0/build.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.1.0/multithreading/base.py` & `pymultithreading-0.2.0/multithreading/base.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.1.0/multithreading/process.py` & `pymultithreading-0.2.0/multithreading/process.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,115 +9,171 @@
 )
 
 from represent import BaseModel, Modifiers
 
 __all__ = [
     "Caller",
     "CallDefinition",
-    "CallInfo",
+    "CallsResults",
     "multi_threaded_call",
     "multi_threaded_defined_call",
     "wait_call_completion",
-    "CallWaitingInfo",
+    "ProcessTime",
     "ProcessInfo",
-    "find_caller"
+    "find_caller",
+    "CallerInfo",
+    "CallResults"
 ]
 
-class Caller(BaseModel):
+class ProcessInfo(BaseModel, metaclass=ABCMeta):
+    """A class to contain the info of a call to the callers."""
+
+    modifiers = Modifiers(properties=True)
+
+    __slots__ = 'start', 'end'
+
+    def __init__(
+            self,
+            start: dt.datetime,
+            end: dt.datetime,
+    ) -> None:
+        """
+        Defines the class attributes.
+
+        :param start: The starting time for the call.
+        :param end: The ending time for the call.
+        """
+
+        self.start = start
+        self.end = end
+    # end __init__
+
+    @property
+    def time(self) -> dt.timedelta:
+        """
+        Returns the time duration of the call.
+
+        :return: The call time.
+        """
+
+        return self.end - self.start
+    # end time
+# end CallInfo
+
+
+class ProcessTime(ProcessInfo):
+    """A class to contain the info of a call to the callers."""
+# end ProcessTime
+
+class CallerInfo(ProcessInfo):
     """A class to represent a function caller object."""
 
     modifiers = Modifiers(excluded=["thread"], force=True)
 
+    __slots__ = "returns", "thread"
+
+    def __init__(
+            self,
+            returns: Optional[Any] = None,
+            thread: Optional[threading.Thread] = None,
+            start: Optional[dt.datetime] = None,
+            end: Optional[dt.datetime] = None,
+
+    ) -> None:
+        """
+        Defines the class attributes.
+
+        :param returns: The returned response.
+        """
+
+        super().__init__(start=start, end=end)
+
+        self.returns = returns
+        self.thread = thread
+    # end __init__
+# end Caller
+
+class CallResults(CallerInfo):
+    """A class to represent a container for the call results."""
+# end CallResults
+
+class Caller(BaseModel):
+    """A class to represent a function caller object."""
+
+    modifiers = Modifiers(excluded=["thread", "results"])
+
     __slots__ = (
-        "target", "identifier", "args", "kwargs", "returns",
-        "thread", "start", "end", "complete", "called"
+        "target", "identifier", "args", "kwargs",
+        "thread", "results", "complete", "called"
     )
 
     def __init__(
             self,
             target: Callable,
             identifier: Optional[Any] = None,
             args: Optional[Iterable[Any]] = None,
-            kwargs: Optional[Dict[str, Any]] = None,
-            returns: Optional[Any] = None
+            kwargs: Optional[Dict[str, Any]] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param target: The function to call.
         :param identifier: The identifier of the call.
         :param args: The positional arguments.
         :param kwargs: The keyword arguments.
-        :param returns: The returned response.
         """
 
         self.target = target
-        self.returns = returns
-
         self.args = args or ()
         self.kwargs = kwargs or {}
         self.identifier = identifier or self.target
 
-        self.thread: Optional[threading.Thread] = None
-
-        self.start: Optional[dt.timedelta] = None
-        self.end: Optional[dt.timedelta] = None
-
         self.complete = False
         self.called = False
+
+        self.thread: Optional[threading.Thread] = None
+        self.results: Optional[CallResults] = None
     # end __init__
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, *args: Any, **kwargs: Any) -> CallResults:
         """
         Calls the function and saves the response.
 
         :param args: The positional arguments.
         :param kwargs: The keyword arguments.
 
         :return: The returned response.
         """
 
-        self.start = dt.datetime.now()
+        start = dt.datetime.now()
 
         self.args = args or self.args
         self.kwargs = kwargs or self.kwargs
 
         self.called = True
 
-        self.returns = self.target(*self.args, **self.kwargs)
+        returns = self.target(*self.args, **self.kwargs)
 
         self.complete = True
 
-        self.end = dt.datetime.now()
-
-        return self.returns
-    # end __call__
-
-    @property
-    def time(self) -> dt.timedelta:
-        """
-        Calculates the time between start and end.
+        end = dt.datetime.now()
 
-        :return: The process time.
-        """
-
-        if self.start is None or self.end is None:
-            return dt.timedelta()
-        # end if
+        self.results = CallResults(
+            start=start, end=end,
+            thread=self.thread, returns=returns
+        )
 
-        return self.end - self.start
-    # end time
+        return self.results
+    # end __call__
 
     def reset(self) -> None:
         """Rests the values from the calls."""
 
-        self.returns = None
         self.called = False
         self.complete = False
-        self.modifiers = False
     # end reset
 # end Caller
 
 def find_caller(callers: Iterable[Caller], identifier: Any) -> Caller:
     """
     Finds the caller object by its identifier
 
@@ -136,14 +192,37 @@
     raise ValueError(
         f"Cannot find a caller object with the identifier: "
         f"{identifier}. valid identifiers are: "
         f"{', '.join(str(caller.identifier) for caller in callers)}"
     )
 # end find_caller
 
+def find_results(callers: Iterable[Caller], identifier: Any) -> Caller:
+    """
+    Finds the caller object by its identifier
+
+    :param callers: The callers in which to search.
+    :param identifier: The identifier of the caller to return.
+
+    :return: The matching caller object.
+    """
+
+    for caller in callers:
+        if caller.identifier == identifier:
+            return caller
+        # end if
+    # end for
+
+    raise ValueError(
+        f"Cannot find a caller object with the identifier: "
+        f"{identifier}. valid identifiers are: "
+        f"{', '.join(str(caller.identifier) for caller in callers)}"
+    )
+# end find_results
+
 class CallDefinition(BaseModel):
     """A class to represent the call definition."""
 
     WAIT = True
     RESET_BEFORE = True
     RESET_AFTER = False
 
@@ -186,91 +265,84 @@
         self.wait = wait
         self.reset_before = reset_before
         self.reset_after = reset_after
         self.sleep = sleep
     # end __init__
 # end CallDefinition
 
-class ProcessInfo(BaseModel, metaclass=ABCMeta):
+class CallsResults(BaseModel):
     """A class to contain the info of a call to the callers."""
 
-    modifiers = Modifiers(excluded=["thread"], properties=True)
-
-    __slots__ = 'callers', 'start', 'end', 'definition'
+    __slots__ = "waiting", "callers", "definition", "total"
 
     def __init__(
             self,
-            callers: Iterable[Caller],
-            start: dt.datetime,
-            end: dt.datetime,
+            callers: Dict[Caller, CallResults],
+            total: ProcessTime,
+            waiting: ProcessTime,
             definition: CallDefinition
     ) -> None:
         """
         Defines the class attributes.
 
         :param callers: The callers object.
-        :param start: The starting time for the call.
-        :param end: The ending time for the call.
+        :param total: The time object for the call.
         :param definition: The call definition object.
         """
 
         self.callers = callers
         self.definition = definition
-
-        self.start = start
-        self.end = end
+        self.total = total
+        self.waiting = waiting
     # end __init__
 
-    @property
-    def time(self) -> dt.timedelta:
+    def caller(self, identifier: Any) -> Caller:
         """
-        Returns the time duration of the call.
+        Finds the caller object by its identifier
 
-        :return: The call time.
-        """
+        :param identifier: The identifier of the caller to return.
 
-        return self.end - self.start
-    # end time
-# end CallInfo
+        :return: The matching caller object.
+        """
 
+        for caller in self.callers:
+            if caller.identifier == identifier:
+                return caller
+            # end if
+        # end for
 
-class CallWaitingInfo(ProcessInfo):
-    """A class to contain the info of a call to the callers."""
-# end CallWaitingInfo
+        raise ValueError(
+            f"Cannot find a caller object with the identifier: "
+            f"{identifier}. valid identifiers are: "
+            f"{', '.join(str(caller.identifier) for caller in self.callers)}"
+        )
+    # end caller
 
-class CallInfo(ProcessInfo):
-    """A class to contain the info of a call to the callers."""
+    def results(self, identifier: Any) -> CallResults:
+        """
+        Finds the caller object by its identifier
 
-    __slots__ = "waiting",
+        :param identifier: The identifier of the caller to return.
 
-    def __init__(
-            self,
-            callers: Iterable[Caller],
-            start: dt.datetime,
-            waiting: CallWaitingInfo,
-            end: dt.datetime,
-            definition: CallDefinition
-    ) -> None:
+        :return: The matching caller object.
         """
-        Defines the class attributes.
 
-        :param callers: The callers object.
-        :param start: The starting time for the call.
-        :param end: The ending time for the call.
-        :param definition: The call definition object.
-        """
+        for caller, results in self.callers.items():
+            if caller.identifier == identifier:
+                return results
+            # end if
+        # end for
 
-        super().__init__(
-            callers=callers, start=start,
-            end=end, definition=definition
+        raise ValueError(
+            f"Cannot find a caller object with the identifier: "
+            f"{identifier}. valid identifiers are: "
+            f"{', '.join(str(caller.identifier) for caller in self.callers)}"
         )
-
-        self.waiting = waiting
-    # end __init__
-# end CallInfo
+    # end results
+# end CallsResults
 
 def validate_callers(data: Any) -> Iterable[Caller]:
     """
     Validates the data as callers.
 
     :param data: The data to validate.
 
@@ -290,15 +362,15 @@
             f"{Caller} objects, not: {data}."
         ) from e
     # end try
 # end validate_callers
 
 def wait_call_completion(
         callers: Iterable[Caller], definition: CallDefinition
-) -> CallWaitingInfo:
+) -> ProcessTime:
     """
     Waits for the calls to complete.
 
     :param callers: The call objects for the functions.
     :param definition: The call definition object.
 
     :return: The waiting results.
@@ -318,24 +390,21 @@
         # end if
 
         time.sleep(sleep)
     # end while
 
     end = dt.datetime.now()
 
-    return CallWaitingInfo(
-        callers=callers, start=start,
-        end=end, definition=definition
-    )
+    return ProcessTime(start=start, end=end)
 # end wait_call_completion
 
 def multi_threaded_defined_call(
         callers: Iterable[Caller],
         definition: Optional[CallDefinition] = None
-) -> CallInfo:
+) -> CallsResults:
     """
     Calls the functions with the callers.
 
     :param callers: The call objects for the functions.
     :param definition: The call definition object.
 
     :return: The call results.
@@ -361,35 +430,37 @@
         caller.thread.start()
     # end for
 
     waiting = wait_call_completion(
         callers=callers, definition=definition
     )
 
+    results = {caller: caller.results for caller in callers}
+
     if definition.reset_after:
         for caller in callers:
             caller.reset()
         # end for
     # end if
 
     end = dt.datetime.now()
 
-    return CallInfo(
-        callers=callers, start=start, end=end,
+    return CallsResults(
+        callers=results, total=ProcessTime(start=start, end=end),
         definition=definition, waiting=waiting
     )
 # end multi_threaded_defined_call
 
 def multi_threaded_call(
         callers: Iterable[Caller],
         wait: Optional[bool] = None,
         reset_before: Optional[bool] = None,
         reset_after: Optional[bool] = None,
         sleep: Optional[Union[int, float, dt.timedelta]] = None
-) -> CallInfo:
+) -> CallsResults:
     """
     Calls the functions with the callers.
 
     :param callers: The call objects for the functions.
     :param wait: The value to wait.
     :param reset_before: The value to reset before running.
     :param reset_after: The value to reset after running.
```

### Comparing `pymultithreading-0.1.0/pymultithreading.egg-info/PKG-INFO` & `pymultithreading-0.2.0/pymultithreading.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.1.0
+Version: 0.2.0
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.1.0/pyproject.toml` & `pymultithreading-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pymultithreading'
-version = '0.1.0'
+version = '0.2.0'
 description = 'A python module for creating multithreading processes easily, in a more Pythonic way.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pymultithreading-0.1.0/setup.py` & `pymultithreading-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pymultithreading',
-        version='0.1.0',
+        version='0.2.0',
         description=(
             "A python module for creating multithreading "
             "processes easily, in a more Pythonic way."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```


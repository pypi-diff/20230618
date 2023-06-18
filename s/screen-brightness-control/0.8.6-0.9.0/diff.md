# Comparing `tmp/screen_brightness_control-0.8.6.tar.gz` & `tmp/screen_brightness_control-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screen_brightness_control-0.8.6.tar", last modified: Sun May 30 22:20:51 2021, max compression
+gzip compressed data, was "screen_brightness_control-0.9.0.tar", last modified: Mon Jul 12 12:16:31 2021, max compression
```

## Comparing `screen_brightness_control-0.8.6.tar` & `screen_brightness_control-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-05-30 22:20:51.229507 screen_brightness_control-0.8.6/
--rw-rw-rw-   0        0        0    13256 2021-05-30 22:20:51.200091 screen_brightness_control-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0    10630 2021-05-30 22:17:04.000000 screen_brightness_control-0.8.6/README.md
-drwxrwxrwx   0        0        0        0 2021-05-30 22:20:50.544714 screen_brightness_control-0.8.6/screen_brightness_control/
--rw-rw-rw-   0        0        0    29031 2021-05-30 22:17:38.000000 screen_brightness_control-0.8.6/screen_brightness_control/__init__.py
--rw-rw-rw-   0        0        0     6103 2021-03-03 20:44:50.000000 screen_brightness_control-0.8.6/screen_brightness_control/__main__.py
--rw-rw-rw-   0        0        0    43976 2021-05-30 22:19:36.000000 screen_brightness_control-0.8.6/screen_brightness_control/linux.py
--rw-rw-rw-   0        0        0    32933 2021-05-30 14:47:49.000000 screen_brightness_control-0.8.6/screen_brightness_control/windows.py
-drwxrwxrwx   0        0        0        0 2021-05-30 22:20:51.058716 screen_brightness_control-0.8.6/screen_brightness_control.egg-info/
--rw-rw-rw-   0        0        0    13256 2021-05-30 22:20:49.000000 screen_brightness_control-0.8.6/screen_brightness_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2021-05-30 22:20:49.000000 screen_brightness_control-0.8.6/screen_brightness_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-30 22:20:49.000000 screen_brightness_control-0.8.6/screen_brightness_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2021-05-30 22:20:49.000000 screen_brightness_control-0.8.6/screen_brightness_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2021-05-30 22:20:49.000000 screen_brightness_control-0.8.6/screen_brightness_control.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-30 22:20:51.254748 screen_brightness_control-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1069 2021-05-30 22:17:54.000000 screen_brightness_control-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-12 12:16:31.808406 screen_brightness_control-0.9.0/
+-rw-rw-rw-   0        0        0    14718 2021-07-12 12:16:31.793431 screen_brightness_control-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11924 2021-07-12 11:40:15.000000 screen_brightness_control-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2021-07-12 12:16:31.154546 screen_brightness_control-0.9.0/screen_brightness_control/
+-rw-rw-rw-   0        0        0    36692 2021-07-12 11:40:16.000000 screen_brightness_control-0.9.0/screen_brightness_control/__init__.py
+-rw-rw-rw-   0        0        0     6103 2021-07-12 11:39:52.000000 screen_brightness_control-0.9.0/screen_brightness_control/__main__.py
+-rw-rw-rw-   0        0        0    36983 2021-07-12 11:40:16.000000 screen_brightness_control-0.9.0/screen_brightness_control/linux.py
+-rw-rw-rw-   0        0        0    30628 2021-07-12 11:40:16.000000 screen_brightness_control-0.9.0/screen_brightness_control/windows.py
+drwxrwxrwx   0        0        0        0 2021-07-12 12:16:31.634408 screen_brightness_control-0.9.0/screen_brightness_control.egg-info/
+-rw-rw-rw-   0        0        0    14718 2021-07-12 12:16:28.000000 screen_brightness_control-0.9.0/screen_brightness_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2021-07-12 12:16:28.000000 screen_brightness_control-0.9.0/screen_brightness_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-12 12:16:28.000000 screen_brightness_control-0.9.0/screen_brightness_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2021-07-12 12:16:28.000000 screen_brightness_control-0.9.0/screen_brightness_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2021-07-12 12:16:28.000000 screen_brightness_control-0.9.0/screen_brightness_control.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-07-12 12:16:31.825305 screen_brightness_control-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2021-07-12 11:40:16.000000 screen_brightness_control-0.9.0/setup.py
```

### Comparing `screen_brightness_control-0.8.6/PKG-INFO` & `screen_brightness_control-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen_brightness_control
-Version: 0.8.6
+Version: 0.9.0
 Summary: A Python tool to control monitor brightness on Windows and Linux
 Home-page: https://github.com/Crozzers/screen_brightness_control
 Author: Crozzers
 Author-email: captaincrozzers@gmail.com
 License: MIT
 Project-URL: Documentation, https://crozzers.github.io/screen_brightness_control
 Project-URL: Issue Tracker, https://github.com/Crozzers/screen_brightness_control/issues
@@ -73,48 +73,53 @@
         ```
         
         # Quick Start
         
         You can read [the full documentation](https://crozzers.github.io/screen_brightness_control) for this project for more details but here are the basics.
         
         
-        ### get_brightness(`verbose_error=False, **kwargs`)
+        ### get_brightness(`display=None, method=None, verbose_error=False`)
         **Summary:**  
         Returns the current screen brightness as a percentage. It may return a list of values if you have multiple, brightness adjustable monitors.  
         Raises `ScreenBrightnessError` upon failure
         
         **Arguments:**
         
+        * `display` - the specific display you wish to adjust. This can be an integer or a string (EDID, serial, name or model)
+        * `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
         * `verbose_error` - a boolean value to control how much detail any error messages should contain
-        * `kwargs` - passed to the OS relevant brightness method
         
         **Usage:**  
         ```python
         import screen_brightness_control as sbc
         
-        #get the current screen brightness (for all detected displays)
+        # get the current screen brightness (for all detected displays)
         all_screens_brightness = sbc.get_brightness()
-        #get the brightness of the primary display
+        # get the brightness of the primary display
         primary_display_brightness = sbc.get_brightness(display=0)
-        #get the brightness of the secondary display (if connected)
+        # get the brightness of the secondary display (if connected)
         secondary_display_brightness = sbc.get_brightness(display=1)
+        # get the brightness for a named monitor
+        benq_brightness = sbc.get_brightness(display='BenQ GL2450H')
         ```  
         
         
-        ### set_brightness(`value, force=False, verbose_error=False, **kwargs`)
+        ### set_brightness(`value, display=None, method=None, force=False, verbose_error=False, no_return=False`)
         **Summary:**  
         Sets the brightness to `value`. If `value` is a string and contains "+" or "-" then that value is added to/subtracted from the current brightness.
         Raises `ScreenBrightnessError` upon failure
         
         **Arguments:**
         
         * `value` - the level to set the brightness to. Can either be an integer or a string.
+        * `display` - the specific display you wish to adjust. This can be an integer or a string (EDID, serial, name or model)
+        * `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
         * `force` (Linux only) - if set to `False` then the brightness is never set to less than 1 because on Linux this often turns the screen off. If set to `True` then it will bypass this check
         * `verbose_error` - a boolean value to control how much detail any error messages should contain
-        * `kwargs` - passed to the OS relevant brightness method
+        * `no_return` - boolean value, whether this function should return `None` or not. By default, the return value is the new brightness value but this behaviour is deprecated. In the future this function will return `None` by default.
         
         **Usage:**  
         ```python
         import screen_brightness_control as sbc
         
         #set brightness to 50%
         sbc.set_brightness(50)
@@ -164,14 +169,30 @@
         sbc.fade_brightness(90, start=100, interval=0.1)
         
         #fade the brightness to 100% in a new thread
         sbc.fade_brightness(100, blocking=False)
         ```
         
         
+        ### list_monitors(`method=None`)
+        **Summary:**  
+        Returns a list of the names of all detected monitors
+        
+        **Arguments:**
+        
+        * `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
+        
+        **Usage:**  
+        ```python
+        import screen_brightness_control as sbc
+        monitor_names = sbc.list_monitors()
+        # eg: ['BenQ GL2450H', 'Dell U2211H']
+        ```
+        
+        
         ## A Toast
         To GitHub users [lcharles](https://github.com/lcharles), [Ved Rathi](https://github.com/Ved-programmer), [Daniel Wong](https://github.com/drojf), [Melek REBAI](https://github.com/shadoWalker89) and [Mathias Johansson](https://github.com/Mathias9807) for contributing to this project
         
         ## License
         This software is licensed under the [MIT license](https://mit-license.org/)
         
         # FAQ
@@ -215,15 +236,15 @@
         
         ### When I call `get_brightness()` the returned value isn't what I set it to (Windows)
         Not all monitors can set the brightness for every value between 0 and 100. Some of them have a number of 'levels' that they can be set to.
         You can likely see this if you open your display settings and very slowly move the brightness slider.  
         You can find out your brightness 'levels' by running the following python code:
         ```python
         import wmi
-        monitor = wmi.WMI(namespace='wmi').MonitorBrightness[0]
+        monitor = wmi.WMI(namespace='wmi').WmiMonitorBrightness()[0]
         #the number of levels the monitor can be set to
         print(monitor.Levels)
         #the actual brightness values your monitor can be set to
         print(monitor.Level)
         ```
         
         # Things to note:
```

### Comparing `screen_brightness_control-0.8.6/README.md` & `screen_brightness_control-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,48 +63,53 @@
 ```
 
 # Quick Start
 
 You can read [the full documentation](https://crozzers.github.io/screen_brightness_control) for this project for more details but here are the basics.
 
 
-### get_brightness(`verbose_error=False, **kwargs`)
+### get_brightness(`display=None, method=None, verbose_error=False`)
 **Summary:**  
 Returns the current screen brightness as a percentage. It may return a list of values if you have multiple, brightness adjustable monitors.  
 Raises `ScreenBrightnessError` upon failure
 
 **Arguments:**
 
+* `display` - the specific display you wish to adjust. This can be an integer or a string (EDID, serial, name or model)
+* `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
 * `verbose_error` - a boolean value to control how much detail any error messages should contain
-* `kwargs` - passed to the OS relevant brightness method
 
 **Usage:**  
 ```python
 import screen_brightness_control as sbc
 
-#get the current screen brightness (for all detected displays)
+# get the current screen brightness (for all detected displays)
 all_screens_brightness = sbc.get_brightness()
-#get the brightness of the primary display
+# get the brightness of the primary display
 primary_display_brightness = sbc.get_brightness(display=0)
-#get the brightness of the secondary display (if connected)
+# get the brightness of the secondary display (if connected)
 secondary_display_brightness = sbc.get_brightness(display=1)
+# get the brightness for a named monitor
+benq_brightness = sbc.get_brightness(display='BenQ GL2450H')
 ```  
 
 
-### set_brightness(`value, force=False, verbose_error=False, **kwargs`)
+### set_brightness(`value, display=None, method=None, force=False, verbose_error=False, no_return=False`)
 **Summary:**  
 Sets the brightness to `value`. If `value` is a string and contains "+" or "-" then that value is added to/subtracted from the current brightness.
 Raises `ScreenBrightnessError` upon failure
 
 **Arguments:**
 
 * `value` - the level to set the brightness to. Can either be an integer or a string.
+* `display` - the specific display you wish to adjust. This can be an integer or a string (EDID, serial, name or model)
+* `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
 * `force` (Linux only) - if set to `False` then the brightness is never set to less than 1 because on Linux this often turns the screen off. If set to `True` then it will bypass this check
 * `verbose_error` - a boolean value to control how much detail any error messages should contain
-* `kwargs` - passed to the OS relevant brightness method
+* `no_return` - boolean value, whether this function should return `None` or not. By default, the return value is the new brightness value but this behaviour is deprecated. In the future this function will return `None` by default.
 
 **Usage:**  
 ```python
 import screen_brightness_control as sbc
 
 #set brightness to 50%
 sbc.set_brightness(50)
@@ -154,14 +159,30 @@
 sbc.fade_brightness(90, start=100, interval=0.1)
 
 #fade the brightness to 100% in a new thread
 sbc.fade_brightness(100, blocking=False)
 ```
 
 
+### list_monitors(`method=None`)
+**Summary:**  
+Returns a list of the names of all detected monitors
+
+**Arguments:**
+
+* `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
+
+**Usage:**  
+```python
+import screen_brightness_control as sbc
+monitor_names = sbc.list_monitors()
+# eg: ['BenQ GL2450H', 'Dell U2211H']
+```
+
+
 ## A Toast
 To GitHub users [lcharles](https://github.com/lcharles), [Ved Rathi](https://github.com/Ved-programmer), [Daniel Wong](https://github.com/drojf), [Melek REBAI](https://github.com/shadoWalker89) and [Mathias Johansson](https://github.com/Mathias9807) for contributing to this project
 
 ## License
 This software is licensed under the [MIT license](https://mit-license.org/)
 
 # FAQ
@@ -205,15 +226,15 @@
 
 ### When I call `get_brightness()` the returned value isn't what I set it to (Windows)
 Not all monitors can set the brightness for every value between 0 and 100. Some of them have a number of 'levels' that they can be set to.
 You can likely see this if you open your display settings and very slowly move the brightness slider.  
 You can find out your brightness 'levels' by running the following python code:
 ```python
 import wmi
-monitor = wmi.WMI(namespace='wmi').MonitorBrightness[0]
+monitor = wmi.WMI(namespace='wmi').WmiMonitorBrightness()[0]
 #the number of levels the monitor can be set to
 print(monitor.Levels)
 #the actual brightness values your monitor can be set to
 print(monitor.Level)
 ```
 
 # Things to note:
```

### Comparing `screen_brightness_control-0.8.6/screen_brightness_control/__init__.py` & `screen_brightness_control-0.9.0/screen_brightness_control/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,406 @@
 import platform
-import time
+import struct
 import threading
-from typing import List, Tuple, Union, Optional, Any
+import time
+import traceback
+from functools import lru_cache
+from typing import Any, List, Optional, Tuple, Union
 
 
-class __Cache(dict):
-    '''class to cache data with a short shelf life'''
-    def __init__(self):
-        self.enabled = True
-        super().__init__()
+def get_brightness(
+    display: Optional[Union[int, str]] = None,
+    method: Optional[str] = None,
+    verbose_error: bool = False
+) -> Union[List[int], int]:
+    '''
+    Returns the current display brightness
 
-    def __setitem__(self, key, value, *args, expires=1, **kwargs):
-        expires += time.time()
-        super().__setitem__(key, (value, expires, args, kwargs))
+    Args:
+        display (str or int): the specific display to query
+        method (str): the way in which displays will be accessed.
+            On Windows this can be 'wmi' or 'vcp'.
+            On Linux it's 'light', 'xrandr', 'ddcutil' or 'xbacklight'.
+        verbose_error (bool): controls the level of detail in the error messages
 
-    def __getitem__(self, key, *args, **kwargs):
-        if not self.enabled:
-            raise Exception
-        value, expires, orig_args, orig_kwargs = super().__getitem__(key)
-        if time.time() < expires and orig_args == args and orig_kwargs == kwargs:
-            return value
-        raise KeyError
+    Returns:
+        int: an integer from 0 to 100 if only one display is detected
+        list: if there a multiple displays connected it may return a list of integers (invalid monitors return `None`)
 
-    def get(self, *args, **kwargs):
-        return self.__getitem__(*args, **kwargs)
+    Example:
+        ```python
+        import screen_brightness_control as sbc
 
-    def store(self, *args, **kwargs):
-        return self.__setitem__(*args, **kwargs)
+        # get the current screen brightness (for all detected displays)
+        current_brightness = sbc.get_brightness()
 
-    def expire(self, key=None, startswith=None, endswith=None):
-        if key is not None:
+        # get the brightness of the primary display
+        primary_brightness = sbc.get_brightness(display=0)
+
+        # get the brightness of the secondary display (if connected)
+        secondary_brightness = sbc.get_brightness(display=1)
+        ```
+    '''
+    return __brightness(display=display, method=method, meta_method='get', verbose_error=verbose_error)
+
+
+def set_brightness(
+    value: Union[int, float, str],
+    display: Optional[Union[str, int]] = None,
+    method: Optional[str] = None,
+    force: bool = False,
+    verbose_error: bool = False,
+    no_return: bool = False
+) -> Union[List[int], int, None]:
+    '''
+    Sets the screen brightness
+
+    Args:
+        value (int or float or str): a value 0 to 100. This is a percentage or a string as '+5' or '-5'
+        display (int or str): the specific display to adjust
+        method (str): the way in which displays will be accessed.
+            On Windows this can be 'wmi' or 'vcp'.
+            On Linux it's 'light', 'xrandr', 'ddcutil' or 'xbacklight'.
+        force (bool): [*Linux Only*] if False the brightness will never be set lower than 1.
+            This is because on most displays a brightness of 0 will turn off the backlight.
+            If True, this check is bypassed
+        verbose_error (bool): boolean value controls the amount of detail error messages will contain
+        no_return (bool): if False, this function returns new brightness (by calling `get_brightness`).
+            If True, this function returns None. In the future this function will return `None` by default
+
+    Returns:
+        list: list of ints (0 to 100)
+        int: if only one display is affected
+        None: if the `no_return` kwarg is specified
+
+    Example:
+        ```python
+        import screen_brightness_control as sbc
+
+        # set brightness to 50%
+        sbc.set_brightness(50)
+
+        # set brightness to 0%
+        sbc.set_brightness(0, force=True)
+
+        # increase brightness by 25%
+        sbc.set_brightness('+25')
+
+        # decrease brightness by 30%
+        sbc.set_brightness('-30')
+
+        # set the brightness of display 0 to 50%
+        sbc.set_brightness(50, display=0)
+        ```
+    '''
+    if type(value) == str and ('+' in value or '-' in value):
+        value = int(float(value))
+        monitors = filter_monitors(display=display, method=method)
+        if len(monitors) > 1:
+            output = []
+            for monitor in monitors:
+                identifier = Monitor.get_identifier(monitor)[1]
+                output.append(
+                    set_brightness(
+                        get_brightness(display=identifier) + value,
+                        display=identifier,
+                        force=force,
+                        verbose_error=verbose_error,
+                        no_return=no_return
+                    )
+                )
+            output = flatten_list(output)
+            return output[0] if len(output) == 1 else output
+        else:
+            value += get_brightness(display=Monitor.get_identifier(monitors[0])[1])
+    else:
+        value = int(float(str(value)))
+
+    # make sure value is within bounds
+    value = max(min(100, value), 0)
+
+    if platform.system() == 'Linux' and not force:
+        value = max(1, value)
+
+    return __brightness(
+        value, display=display, method=method,
+        meta_method='set', no_return=no_return,
+        verbose_error=verbose_error
+    )
+
+
+def fade_brightness(
+    finish: Union[int, str],
+    start: Optional[Union[int, str]] = None,
+    interval: float = 0.01,
+    increment: int = 1,
+    blocking: bool = True,
+    **kwargs
+) -> Union[List[threading.Thread], List[int], int]:
+    '''
+    A function to somewhat gently fade the screen brightness from `start` to `finish`
+
+    Args:
+        finish (int or str): the brightness level to end up on
+        start (int or str): where the brightness should fade from.
+            If not specified the function starts from the current screen brightness
+        interval (float or int): the time delay between each step in brightness
+        increment (int): the amount to change the brightness by per step
+        blocking (bool): whether this should occur in the main thread (`True`) or a new daemonic thread (`False`)
+        kwargs (dict): passed directly to `set_brightness`.
+            Any compatible kwargs are passed to `filter_monitors` as well. (eg: display, method...)
+
+    Returns:
+        list: list of `threading.Thread` objects if `blocking == False`,
+            otherwise it returns the result of `get_brightness()`
+
+    Example:
+        ```python
+        import screen_brightness_control as sbc
+
+        # fade brightness from the current brightness to 50%
+        sbc.fade_brightness(50)
+
+        # fade the brightness from 25% to 75%
+        sbc.fade_brightness(75, start=25)
+
+        # fade the brightness from the current value to 100% in steps of 10%
+        sbc.fade_brightness(100, increment=10)
+
+        # fade the brightness from 100% to 90% with time intervals of 0.1 seconds
+        sbc.fade_brightness(90, start=100, interval=0.1)
+
+        # fade the brightness to 100% in a new thread
+        sbc.fade_brightness(100, blocking=False)
+        ```
+    '''
+    def fade(start, finish, increment, monitor):
+        for i in range(min(start, finish), max(start, finish), increment):
+            val = i
+            if start > finish:
+                val = start - (val - finish)
+            monitor.set_brightness(val, no_return=True)
+            time.sleep(interval)
+
+        if monitor.get_brightness() != finish:
+            monitor.set_brightness(finish, no_return=True)
+        return
+
+    threads = []
+    if 'verbose_error' in kwargs.keys():
+        del(kwargs['verbose_error'])
+
+    try:
+        # make sure only compatible kwargs are passed to filter_monitors
+        available_monitors = filter_monitors(
+            **{k: v for k, v in kwargs.items() if k in (
+                'display', 'haystack', 'method', 'include'
+            )}
+        )
+    except (IndexError, LookupError) as e:
+        raise ScreenBrightnessError(f'\n\tfilter_monitors -> {type(e).__name__}: {e}')
+    except ValueError as e:
+        if platform.system() == 'Linux' and (str(kwargs.get('method', '')).lower() == 'xbacklight'):
+            available_monitors = [method.XBacklight]
+        else:
+            raise ScreenBrightnessError(e)
+    except Exception as e:
+        raise ScreenBrightnessError(e)
+
+    for i in available_monitors:
+        try:
+            if (
+                platform.system() == 'Linux'
+                and str(kwargs.get('method', '')).lower() == 'xbacklight'
+            ):
+                monitor = i
+            else:
+                monitor = Monitor(i)
+            # same effect as monitor.is_active()
+            current = monitor.get_brightness()
+            st, fi = start, finish
+            # convert strings like '+5' to an actual brightness value
+            if isinstance(fi, str):
+                if "+" in fi or "-" in fi:
+                    fi = current + int(float(fi))
+            if isinstance(st, str):
+                if "+" in st or "-" in st:
+                    st = current + int(float(st))
+
+            st = current if st is None else st
+            # make sure both values are within the correct range
+            fi = min(max(int(float(fi)), 0), 100)
+            st = min(max(int(float(st)), 0), 100)
+
+            t1 = threading.Thread(target=fade, args=(st, fi, increment, monitor))
+            t1.start()
+            threads.append(t1)
+        except Exception:
+            pass
+
+    if not blocking:
+        return threads
+    else:
+        for t in threads:
+            t.join()
+        return get_brightness(**kwargs)
+
+
+def list_monitors_info(method: Optional[str] = None, allow_duplicates: bool = False) -> List[dict]:
+    '''
+    list detailed information about all monitors that are controllable by this library
+
+    Args:
+        method (str): the method to use to list the available monitors.
+            On Windows this can be `'wmi'` or `'vcp'`.
+            On Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`.
+        allow_duplicates (bool): whether to filter out duplicate displays or not
+
+    Returns:
+        list: list of dictionaries
+
+    Example:
+        ```python
+        import screen_brightness_control as sbc
+        monitors = sbc.list_monitors_info()
+        for monitor in monitors:
+            print('=======================')
+            # the manufacturer name plus the model
+            print('Name:', monitor['name'])
+            # the general model of the display
+            print('Model:', monitor['model'])
+            # the serial of the display
+            print('Serial:', monitor['serial'])
+            # the name of the brand of the monitor
+            print('Manufacturer:', monitor['manufacturer'])
+            # the 3 letter code corresponding to the brand name, EG: BNQ -> BenQ
+            print('Manufacturer ID:', monitor['manufacturer_id'])
+            # the index of that display FOR THE SPECIFIC METHOD THE DISPLAY USES
+            print('Index:', monitor['index'])
+            # the method this monitor can be addressed by
+            print('Method:', monitor['method'])
+            # the EDID string associated with that monitor
+            print('EDID:', monitor['edid'])
+        ```
+    '''
+    info = __cache__.get('monitors_info', method=method, allow_duplicates=allow_duplicates)
+    if info is None:
+        info = globals()['method'].list_monitors_info(method=method, allow_duplicates=allow_duplicates)
+        __cache__.store('monitors_info', info, method=method, allow_duplicates=allow_duplicates)
+    return info
+
+
+def list_monitors(method: Optional[str] = None) -> List[str]:
+    '''
+    List the names of all detected monitors
+
+    Args:
+        method (str): the method to use to list the available monitors.
+            On Windows this can be `'wmi'` or `'vcp'`.
+            On Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`.
+
+    Returns:
+        list: list of strings
+
+    Example:
+        ```python
+        import screen_brightness_control as sbc
+        monitor_names = sbc.list_monitors()
+        # eg: ['BenQ GL2450H', 'Dell U2211H']
+        ```
+    '''
+    return [i['name'] for i in list_monitors_info(method=method)]
+
+
+class EDID:
+    '''
+    Simple structure and method to extract monitor serial and name from an EDID string.
+
+    The EDID parsing was created with inspiration from the [pyedid library](https://github.com/jojonas/pyedid)
+    '''
+    EDID_FORMAT: str = (
+        ">"     # big-endian
+        "8s"    # constant header (8 bytes)
+        "H"     # manufacturer id (2 bytes)
+        "H"     # product id (2 bytes)
+        "I"     # serial number (4 bytes)
+        "B"     # manufactoring week (1 byte)
+        "B"     # manufactoring year (1 byte)
+        "B"     # edid version (1 byte)
+        "B"     # edid revision (1 byte)
+        "B"     # video input type (1 byte)
+        "B"     # horizontal size in cm (1 byte)
+        "B"     # vertical size in cm (1 byte)
+        "B"     # display gamma (1 byte)
+        "B"     # supported features (1 byte)
+        "10s"   # color characteristics (10 bytes)
+        "H"     # supported timings (2 bytes)
+        "B"     # reserved timing (1 byte)
+        "16s"   # EDID supported timings (16 bytes)
+        "18s"   # detailed timing block 1 (18 bytes)
+        "18s"   # detailed timing block 2 (18 bytes)
+        "18s"   # detailed timing block 3 (18 bytes)
+        "18s"   # detailed timing block 4 (18 bytes)
+        "B"     # extension flag (1 byte)
+        "B"     # checksum (1 byte)
+    )
+    '''The byte structure for EDID strings'''
+
+    @classmethod
+    def parse_edid(cls, edid: str) -> Tuple[Union[str, None], str]:
+        '''
+        Takes an EDID string (as string hex, formatted as: '00ffffff00...') and
+        attempts to extract the monitor's name and serial number from it
+
+        Args:
+            edid (str): the edid string
+
+        Returns:
+            tuple: First item can be None or str. Second item is always str.
+                This represents the name and serial respectively.
+                If the name (first item) is None then this function likely
+                failed to extract the serial correctly.
+
+        Example:
+            ```python
+            import screen_brightness_control as sbc
+
+            edid = sbc.list_monitors_info()[0]['edid']
+            name, serial = sbc.EDID.parse_edid(edid)
+            if name is not None:
+                print('Success!')
+                print('Name:', name)
+                print('Serial:', serial)
+            else:
+                print('Unable to extract the data')
+            ```
+        '''
+        def filter_hex(st):
+            st = str(st)
+            while '\\x' in st:
+                i = st.index('\\x')
+                st = st.replace(st[i:i + 4], '')
+            return st.replace('\\n', '')[2:-1]
+
+        if ' ' in edid:
+            edid = edid.replace(' ', '')
+        edid = bytes.fromhex(edid)
+        data = struct.unpack(cls.EDID_FORMAT, edid)
+        serial = filter_hex(data[18])
+        # other info can be anywhere in this range, I don't know why
+        name = None
+        for i in data[19:22]:
             try:
-                del(self[key])
+                st = str(i)[2:-1].rstrip(' ').rstrip('\t')
+                if st.index(' ') < len(st) - 1:
+                    name = filter_hex(i).split(' ')
+                    name = name[0].lower().capitalize() + ' ' + name[1]
             except Exception:
                 pass
-        else:
-            for i in list(self.keys()):
-                cond1 = startswith is not None and i.startswith(startswith)
-                cond2 = endswith is not None and i.endswith(endswith)
-                if cond1 and cond2:
-                    del(self[i])
-                elif cond1:
-                    del(self[i])
-                elif cond2:
-                    del(self[i])
-                else:
-                    pass
+        return name, serial.strip(' ')
 
 
 MONITOR_MANUFACTURER_CODES = {
     "AAC": "AcerView",
     "ACR": "Acer",
     "AOC": "AOC",
     "AIC": "AG Neovo",
@@ -112,28 +463,30 @@
     "VSC": "ViewSonic",
     "ZCM": "Zenith",
     "UNK": "Unknown",
     "_YV": "Fujitsu",
 }
 
 
+@lru_cache(maxsize=None)
 def _monitor_brand_lookup(search: str) -> Union[Tuple[str, str], None]:
     '''internal function to search the monitor manufacturer codes dict'''
-    keys = list(MONITOR_MANUFACTURER_CODES.keys())
-    keys_lower = [i.lower() for i in keys]
-    values = list(MONITOR_MANUFACTURER_CODES.values())
-    values_lower = [i.lower() for i in values]
-    search_lower = search.lower()
-
-    if search_lower in keys_lower:
-        index = keys_lower.index(search_lower)
-    elif search_lower in values_lower:
-        index = values_lower.index(search_lower)
+    keys = tuple(MONITOR_MANUFACTURER_CODES.keys())
+    keys_lower = tuple(map(str.lower, keys))
+    values = tuple(MONITOR_MANUFACTURER_CODES.values())
+    search = search.lower()
+
+    if search in keys_lower:
+        index = keys_lower.index(search)
     else:
-        return None
+        values_lower = tuple(map(str.lower, values))
+        if search in values_lower:
+            index = values_lower.index(search)
+        else:
+            return None
     return keys[index], values[index]
 
 
 class ScreenBrightnessError(Exception):
     '''
     Generic error class designed to make catching errors under one umbrella easy.
     Raised when the brightness cannot be set/retrieved.
@@ -153,28 +506,29 @@
 
 
 class Monitor():
     '''A class to manage a single monitor and its relevant information'''
     def __init__(self, display: Union[int, str, dict]):
         '''
         Args:
-            display (int or str): the index/name/model name/serial/edid of the display you wish to control.
-                Is passed to `filter_monitors` to decide which display to use
+            display (int or str or dict): the index/name/model name/serial/edid
+                of the display you wish to control. Is passed to `filter_monitors`
+                to decide which display to use.
 
         Raises:
             LookupError: if a matching display could not be found
             TypeError: if the given display type is not int or str
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # create a class for the primary monitor and then a specifically named monitor
             primary = sbc.Monitor(0)
-            benq_monitor = sbc.Monitor('BenQ GL2450HM')
+            benq_monitor = sbc.Monitor('BenQ GL2450H')
 
             # check if the benq monitor is the primary one
             if primary.serial == benq_monitor.serial:
                 print('BenQ GL2450HM is the primary display')
             else:
                 print('The primary display is', primary.name)
 
@@ -191,54 +545,69 @@
                 info = filter_monitors(
                     display=self.get_identifier(display),
                     haystack=monitors_info
                 )[0]
         else:
             info = filter_monitors(display=display, haystack=monitors_info)[0]
 
-        self.serial: str = info['serial']
+        # make a copy so that we don't alter the dict in-place
+        info = info.copy()
+
+        self.serial: str = info.pop('serial')
         '''the serial number of the display or (if serial is not available) an ID assigned by the OS'''
-        self.name: str = info['name']
+        self.name: str = info.pop('name')
         '''the monitors manufacturer name plus its model'''
-        self.method = info['method']
+        self.method = info.pop('method')
         '''the method by which this monitor can be addressed.
         This will be a class from either the windows or linux sub-module'''
-        self.manufacturer: str = info['manufacturer']
+        self.manufacturer: str = info.pop('manufacturer')
         '''the name of the brand of the monitor'''
-        self.manufacturer_id: str = info['manufacturer_id']
+        self.manufacturer_id: str = info.pop('manufacturer_id')
         '''the 3 letter manufacturing code corresponding to the manufacturer name'''
-        self.model: str = info['model']
+        self.model: str = info.pop('model')
         '''the general model of the display'''
-        self.index: int = info['index']
+        self.index: int = info.pop('index')
         '''the index of the monitor FOR THE SPECIFIC METHOD THIS MONITOR USES.'''
-        self.edid: str = info['edid']
+        self.edid: str = info.pop('edid')
         '''a unique string returned by the monitor that contains its DDC capabilities, serial and name'''
 
         # this assigns any extra info that is returned to this class
         # eg: the 'interface' key in XRandr monitors on Linux
         for key, value in info.items():
-            # exclude the 'brightness' key because that will quickly become out of date
-            if value is not None and key != 'brightness':
-                if key not in vars(self).keys():
-                    setattr(self, key, value)
+            if value is not None:
+                setattr(self, key, value)
 
     def __getitem__(self, item: Any) -> Any:
         return getattr(self, item)
 
-    def get_identifier(self, monitor: dict = None) -> Tuple[str, Any]:
+    def get_identifier(self, monitor: dict = None) -> Tuple[str, Union[int, str]]:
         '''
         Returns the piece of information used to identify this monitor.
         Will iterate through the EDID, serial, name and index and return the first
         value that is not equal to None
 
         Args:
             monitor (dict): extract an identifier from this dict instead of the monitor class
 
         Returns:
-            tuple: a key, value pair
+            tuple: the name of the property returned and the value of said property.
+                EG: `('serial', '123abc...')` or `('name', 'BenQ GL2450H')`
+
+        Example:
+            ```python
+            import screen_brightness_control as sbc
+            primary = sbc.Monitor(0)
+            print(primary.get_identifier())  # eg: ('serial', '123abc...')
+
+            secondary = sbc.list_monitors_info()[1]
+            print(primary.get_identifier(monitor=secondary))  # eg: ('serial', '456def...')
+
+            # you can also use the class uninitialized
+            print(sbc.Monitor.get_identifier(secondary))  # eg: ('serial', '456def...')
+            ```
         '''
         if monitor is None:
             monitor = self
 
         for key in ('edid', 'serial', 'name', 'index'):
             value = monitor[key]
             if value is not None:
@@ -262,98 +631,117 @@
             import screen_brightness_control as sbc
 
             # set the brightness of the primary monitor to 50%
             primary = sbc.Monitor(0)
             primary.set_brightness(50)
             ```
         '''
+        # refresh display info, in case another display has been unplugged or something
+        # which would change the index of this display
+        self.get_info()
         value = max(0, min(value, 100))
-        b = self.method.set_brightness(value, display=self.get_identifier()[1], no_return=no_return)
-        if b is not None:
-            return b[0]
-        return b
+        self.method.set_brightness(value, display=self.index)
+        if no_return:
+            return
+        return self.get_brightness()
 
-    def get_brightness(self, **kwargs) -> int:
+    def get_brightness(self) -> int:
         '''
-        Returns the brightness of this display. See `get_brightness` for the full docs
-
-        Args:
-            kwargs (dict): passed directly to this monitor's brightness method
-                The `display` kwarg is always overwritten
+        Returns the brightness of this display.
 
         Returns:
             int: from 0 to 100
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # get the brightness of the primary monitor
             primary = sbc.Monitor(0)
             primary_brightness = primary.get_brightness()
             ```
         '''
-        kwargs['display'] = self.get_identifier()[1]
-        return self.method.get_brightness(**kwargs)[0]
+        # refresh display info, in case another display has been unplugged or something
+        # which would change the index of this display
+        self.get_info()
+        return self.method.get_brightness(display=self.index)[0]
 
     def fade_brightness(self, *args, **kwargs) -> Union[threading.Thread, int]:
         '''
         Fades the brightness for this display. See `fade_brightness` for the full docs
 
         Args:
             args (tuple): passed directly to `fade_brightness`
             kwargs (dict): passed directly to `fade_brightness`.
-                The `display` kwarg is always overwritten.
-                The `method` kwarg may also be overwritten
+                The `display` and `method` kwargs are always
+                overwritten.
 
         Returns:
             threading.Thread: if the the blocking kwarg is False
             int: if the blocking kwarg is True
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # fade the brightness of the primary monitor to 50%
             primary = sbc.Monitor(0)
             primary.fade_brightness(50)
             ```
         '''
-        iden_key, kwargs['display'] = self.get_identifier()
-        if iden_key == 'index':
-            # the reason we override the method kwarg here is that
-            # the 'index' is method specific and `fade_brightness`
-            # is a top-level function. `self.set_brightness` and `self.get_brightness`
-            # call directly to the method so they don't need this step
-            kwargs['method'] = self.method.__name__.lower()
+        # refresh display info, in case another display has been unplugged or something
+        # which would change the index of this display
+        self.get_info(refresh=False)
+        kwargs['display'] = self.index
+        # the reason we override the method kwarg here is that
+        # the 'index' is method specific and `fade_brightness`
+        # is a top-level function. `self.set_brightness` and `self.get_brightness`
+        # call directly to the method so they don't need this step
+        kwargs['method'] = self.method.__name__.lower()
 
         b = fade_brightness(*args, **kwargs)
         # fade_brightness will call the top-level get_brightness
         # function, which will return list OR int
         if isinstance(b, list):
             return b[0]
         return b
 
-    def get_info(self) -> dict:
+    def get_info(self, refresh: bool = True) -> dict:
         '''
         Returns all known information about this monitor instance
 
+        Args:
+            refresh (bool): whether to refresh the information
+                or to return the cached version
+
         Returns:
             dict
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # initialize class for primary monitor
             primary = sbc.Monitor(0)
             # get the info
             info = primary.get_info()
             ```
         '''
+        if not refresh:
+            return vars(self)
+
+        identifier = self.get_identifier()
+
+        if identifier is not None:
+            # refresh the info we have on this monitor
+            info = filter_monitors(display=identifier[1], method=self.method.__name__)[0]
+            for key, value in info.items():
+                if value is not None:
+                    setattr(self, key, value)
+
         return vars(self)
 
     def is_active(self) -> bool:
         '''
         Attempts to retrieve the brightness for this display. If it works the display is deemed active
 
         Returns:
@@ -371,86 +759,17 @@
         try:
             self.get_brightness()
             return True
         except Exception:
             return False
 
 
-def list_monitors_info(**kwargs) -> List[dict]:
-    '''
-    list detailed information about all monitors that are controllable by this library
-
-    Args:
-        kwargs (dict): passed directly to OS relevant monitor list function
-
-    Returns:
-        list: list of dictionaries
-
-    Example:
-        ```python
-        import screen_brightness_control as sbc
-        monitors = sbc.list_monitors_info()
-        for monitor in monitors:
-            print('=======================')
-            # the manufacturer name plus the model
-            print('Name:', monitor['name'])
-
-            # the general model of the display
-            print('Model:', monitor['model'])
-
-            # a unique string assigned by Windows to this display
-            print('Serial:', monitor['serial'])
-
-            # the name of the brand of the monitor
-            print('Manufacturer:', monitor['manufacturer'])
-
-            # the 3 letter code corresponding to the brand name, EG: BNQ -> BenQ
-            print('Manufacturer ID:', monitor['manufacturer_id'])
-
-            # the index of that display FOR THE SPECIFIC METHOD THE DISPLAY USES
-            print('Index:', monitor['index'])
-
-            # the method this monitor can be addressed by
-            print('Method:', monitor['method'])
-
-            # the EDID string associated with that monitor
-            print('EDID:', monitor['edid'])
-        ```
-    '''
-    try:
-        return __cache__.get('monitors_info', **kwargs)
-    except Exception:
-        info = method.list_monitors_info(**kwargs)
-        __cache__.store('monitors_info', info, **kwargs)
-        return info
-
-
-def list_monitors(**kwargs) -> List[str]:
-    '''
-    List the names of all detected monitors
-
-    Args:
-        kwargs (dict): passed directly to OS relevant monitor list function
-
-    Returns:
-        list: list of strings
-
-    Example:
-        ```python
-        import screen_brightness_control as sbc
-        monitor_names = sbc.list_monitors()
-        # eg: ['BenQ GL2450H', 'Dell U2211H']
-        ```
-    '''
-    return [i['name'] for i in list_monitors_info(**kwargs)]
-
-
 def filter_monitors(
     display: Optional[Union[int, str]] = None,
-    haystack: Optional[list] = None,
+    haystack: Optional[List[dict]] = None,
     method: Optional[str] = None,
     include: List[str] = []
 ) -> List[dict]:
     '''
     Searches through the information for all detected displays
     and attempts to return the info matching the value given.
     Will attempt to match against index, name, model, edid, method and serial
@@ -486,24 +805,24 @@
         monitors_with_duplicates = haystack
         if method is not None:
             monitors_with_duplicates = [i for i in haystack if method.lower() == i['method'].__name__.lower()]
     else:
         monitors_with_duplicates = list_monitors_info(method=method, allow_duplicates=True)
 
     if display is not None and type(display) not in (str, int):
-        raise TypeError(f'display kwarg must be int or str, not {type(display)}')
+        raise TypeError(f'display kwarg must be int or str, not "{type(display).__name__}"')
 
     # This loop does two things: 1. Filters out duplicate monitors and 2. Matches the display kwarg (if applicable)
     unique_identifiers = []
     monitors = []
     for monitor in monitors_with_duplicates:
         # find a valid identifier for a monitor, excluding any which are equal to None
         added = False
         for identifier in ['edid', 'serial', 'name', 'model'] + include:
-            if monitor[identifier] is not None:
+            if monitor.get(identifier, None) is not None:
                 # check we haven't already added the monitor
                 if monitor[identifier] not in unique_identifiers:
                     # check if the display kwarg (if str) matches this monitor
                     if type(display) != str or (type(display) == str and monitor[identifier] == display):
                         # if valid and monitor[identifier] not in unique_identifiers:
                         if not added:
                             monitors.append(monitor)
@@ -522,15 +841,15 @@
                     break
 
     # if no monitors matched the query OR if display kwarg was an int
     # if the latter and we made it this far then the int was out of range
     if monitors == [] or type(display) is int:
         msg = 'no monitors found'
         if display is not None:
-            msg += f' with name/serial/model/edid/index of "{display}"'
+            msg += f' with name/serial/model/edid/index of {repr(display)}'
         if method is not None:
             msg += f' with method of "{method}"'
         raise LookupError(msg)
 
     return monitors
 
 
@@ -557,257 +876,123 @@
         if type(item) == list:
             flat_list += flatten_list(item)
         else:
             flat_list.append(item)
     return flat_list
 
 
-def set_brightness(
-    value: Union[int, float, str],
-    force: bool = False,
-    verbose_error: bool = False,
-    **kwargs
-) -> Union[List[int], int, None]:
-    '''
-    Sets the screen brightness
-
-    Args:
-        value (int or float or str): a value 0 to 100. This is a percentage or a string as '+5' or '-5'
-        force (bool): [Linux Only] if False the brightness will never be set lower than 1.
-            This is because on most displays a brightness of 0 will turn off the backlight.
-            If True, this check is bypassed
-        verbose_error (bool): boolean value controls the amount of detail error messages will contain
-        kwargs (dict): passed to the OS relevant brightness method
-
-    Returns:
-        list: list of ints (0 to 100)
-        int: if only one display is affected
-        None: if the `no_return` kwarg is specified
-
-    Example:
-        ```
-        import screen_brightness_control as sbc
-
-        # set brightness to 50%
-        sbc.set_brightness(50)
-
-        # set brightness to 0%
-        sbc.set_brightness(0, force=True)
+def __brightness(
+    *args, display=None, method=None, meta_method='get', no_return=False,
+    verbose_error=False, **kwargs
+):
+    '''Internal function used to get/set brightness'''
+
+    def format_exc(name, e):
+        errors.append((
+            name, e.__class__.__name__,
+            traceback.format_exc() if verbose_error else e
+        ))
+
+    output = []
+    errors = []
+    method = method.lower() if type(method) == str else method
 
-        # increase brightness by 25%
-        sbc.set_brightness('+25')
-
-        # decrease brightness by 30%
-        sbc.set_brightness('-30')
-
-        # set the brightness of display 0 to 50%
-        sbc.set_brightness(50, display=0)
-        ```
-    '''
-    if type(value) not in (int, float, str):
-        raise TypeError(f'value must be int, float or str, not {type(value)}')
-
-    # convert values like '+5' and '-25' to integers and add/subtract them from the current brightness
-    if isinstance(value, str) and value.startswith(('+', '-')):
-        if 'display' in kwargs.keys():
-            current = get_brightness(display=kwargs['display'])
+    try:
+        monitors = filter_monitors(display=display, method=method)
+    except (LookupError, ValueError) as e:
+        if platform.system() == 'Linux' and display is None and method in ('xbacklight', None):
+            try:
+                if meta_method == 'set':
+                    linux.XBacklight.set_brightness(*args)
+                output.append(linux.XBacklight.get_brightness())
+            except Exception as e:
+                format_exc('XBacklight', e)
         else:
-            current = get_brightness()
-
-        if isinstance(current, list):
-            # apply the offset to all displays by setting the brightness for each one individually
-            out: list = []
-            for i in range(len(current)):
-                out.append(set_brightness(current[i] + int(float(str(value))), display=i, **kwargs))
-            # flatten the list output
-            out = flatten_list(out)
-            return out[0] if len(out) == 1 else out
-
-        value = current + int(float(str(value)))
+            format_exc('filter_monitors', e)
+    except Exception as e:
+        format_exc('filter_monitors', e)
     else:
-        value = int(float(str(value)))
-
-    value = min(100, value)
+        for monitor in monitors:
+            try:
+                if meta_method == 'set':
+                    monitor['method'].set_brightness(*args, display=monitor['index'], **kwargs)
+                    if no_return:
+                        continue
+
+                output.append(monitor['method'].get_brightness(display=monitor['index'], **kwargs))
+            except Exception as e:
+                output.append(None)
+                format_exc(monitor, e)
+
+    output = flatten_list(output)
+
+    if output and not set(output) == {None}:
+        # if all of the outputs are None then all of the monitors failed
+        output = output[0] if len(output) == 1 else output
+        return output if not no_return else None
+    elif meta_method == 'set' and no_return:
+        return
 
-    if platform.system() == 'Linux':
-        if not force:
-            value = max(1, value)
+    # if the function hasn't returned then it has failed
+    msg = '\n'
+    if errors:
+        for monitor, exc_name, exc in errors:
+            if type(monitor) == str:
+                msg += f'\t{monitor}'
+            else:
+                msg += f'\t{monitor["name"]} ({monitor["serial"]})'
+            msg += f' -> {exc_name}: '
+            msg += str(exc).replace('\n', '\n\t\t') + '\n'
     else:
-        value = max(0, value)
-
-    try:
-        out = method.set_brightness(value, **kwargs)
-        return out[0] if (isinstance(out, list) and len(out) == 1) else out
-    except Exception as e:
-        if verbose_error:
-            raise ScreenBrightnessError from e
-        error = e
-
-    # if the function has not returned by now it failed
-    raise ScreenBrightnessError(f'Cannot set screen brightness: {error}')
-
-
-def fade_brightness(
-    finish: Union[int, str],
-    start: Optional[Union[int, str]] = None,
-    interval: float = 0.01,
-    increment: int = 1,
-    blocking: bool = True,
-    **kwargs
-) -> Union[List[threading.Thread], List[int], int]:
-    '''
-    A function to somewhat gently fade the screen brightness from `start` to `finish`
-
-    Args:
-        finish (int or str): the brightness level to end up on
-        start (int or str): where the brightness should fade from.
-            If not specified the function starts from the current screen brightness
-        interval (float or int): the time delay between each step in brightness
-        increment (int): the amount to change the brightness by per step
-        blocking (bool): whether this should occur in the main thread (`True`) or a new daemonic thread (`False`)
-        kwargs (dict): passed directly to set_brightness (see `set_brightness` docs for available kwargs).
-            Any compatible kwargs are passed to `filter_monitors` as well. (eg: display, method...)
-
-    Returns:
-        list: list of `threading.Thread` objects if `blocking == False`,
-            otherwise it returns the result of `get_brightness()`
+        msg += '\tno valid output was received from brightness methods'
 
-    Example:
-        ```
-        import screen_brightness_control as sbc
+    raise ScreenBrightnessError(msg)
 
-        # fade brightness from the current brightness to 50%
-        sbc.fade_brightness(50)
-
-        # fade the brightness from 25% to 75%
-        sbc.fade_brightness(75, start=25)
 
-        # fade the brightness from the current value to 100% in steps of 10%
-        sbc.fade_brightness(100, increment=10)
-
-        # fade the brightness from 100% to 90% with time intervals of 0.1 seconds
-        sbc.fade_brightness(90, start=100, interval=0.1)
-
-        # fade the brightness to 100% in a new thread
-        sbc.fade_brightness(100, blocking=False)
-        ```
-    '''
-    def fade(start, finish, increment, monitor):
-        for i in range(min(start, finish), max(start, finish), increment):
-            val = i
-            if start > finish:
-                val = start - (val - finish)
-            monitor.set_brightness(val, no_return=True)
-            time.sleep(interval)
-
-        if monitor.get_brightness() != finish:
-            monitor.set_brightness(finish, no_return=True)
-        return
-
-    threads = []
-    if 'verbose_error' in kwargs.keys():
-        del(kwargs['verbose_error'])
+class __Cache(dict):
+    '''class to cache data with a short shelf life'''
+    def __init__(self):
+        self.enabled = True
+        super().__init__()
 
-    try:
-        # sift through kwargs and find args that are compatible with filter_monitors
-        # this __code__.co_varnames is kinda hacky but since filter_monitors
-        # doesn't have any special *args or **kwargs it should be fine
-        kw = {}
-        for key, value in kwargs.items():
-            if key in filter_monitors.__code__.co_varnames[:filter_monitors.__code__.co_argcount]:
-                kw[key] = value
-        available_monitors = filter_monitors(**kw)
-        del(kw)
-    except (IndexError, LookupError) as e:
-        raise ScreenBrightnessError(f'{type(e).__name__} -> {e}')
-    except ValueError as e:
-        if platform.system() == 'Linux' and ('method' in kwargs and kwargs['method'].lower() == 'xbacklight'):
-            available_monitors = [method.XBacklight]
-        else:
-            raise e
+    def get(self, key, *args, **kwargs):
+        if not self.enabled:
+            return None
 
-    for i in available_monitors:
         try:
-            if (
-                platform.system() == 'Linux'
-                and (
-                    'method' in kwargs
-                    and kwargs['method'] is not None
-                    and kwargs['method'].lower() == 'xbacklight'
-                )
-            ):
-                monitor = i
+            value, expires, orig_args, orig_kwargs = super().__getitem__(key)
+            if time.time() < expires:
+                if orig_args == args and orig_kwargs == kwargs:
+                    return value
             else:
-                monitor = Monitor(i)
-            # same effect as monitor.is_active()
-            current = monitor.get_brightness()
-            st, fi = start, finish
-            # convert strings like '+5' to an actual brightness value
-            if isinstance(fi, str):
-                if "+" in fi or "-" in fi:
-                    fi = current + int(float(fi))
-            if isinstance(st, str):
-                if "+" in st or "-" in st:
-                    st = current + int(float(st))
-
-            st = current if st is None else st
-            # make sure both values are within the correct range
-            fi = min(max(int(fi), 0), 100)
-            st = min(max(int(st), 0), 100)
-
-            t1 = threading.Thread(target=fade, args=(st, fi, increment, monitor))
-            t1.start()
-            threads.append(t1)
-        except Exception:
+                super().__delitem__(key)
+        except KeyError:
             pass
 
-    if not blocking:
-        return threads
-    else:
-        for t in threads:
-            t.join()
-        return get_brightness(**kwargs)
+    def store(self, key, value, *args, expires=1, **kwargs):
+        super().__setitem__(key, (value, expires + time.time(), args, kwargs))
 
-
-def get_brightness(verbose_error: bool = False, **kwargs) -> Union[List[int], int]:
-    '''
-    Returns the current display brightness
-
-    Args:
-        verbose_error (bool): controls the level of detail in the error messages
-        kwargs (dict): is passed directly to the OS relevant brightness method
-
-    Returns:
-        int: an integer from 0 to 100 if only one display is detected
-        list: if there a multiple displays connected it may return a list of integers (invalid monitors return `None`)
-
-    Example:
-        ```python
-        import screen_brightness_control as sbc
-
-        # get the current screen brightness (for all detected displays)
-        current_brightness = sbc.get_brightness()
-
-        # get the brightness of the primary display
-        primary_brightness = sbc.get_brightness(display=0)
-
-        # get the brightness of the secondary display (if connected)
-        secondary_brightness = sbc.get_brightness(display=1)
-        ```
-    '''
-    try:
-        out = method.get_brightness(**kwargs)
-        return out[0] if (type(out) == list and len(out) == 1) else out
-    except Exception as e:
-        if verbose_error:
-            raise ScreenBrightnessError from e
-        error = e
-
-    # if the function has not returned by now it failed
-    raise ScreenBrightnessError(f'Cannot get screen brightness: {error}')
+    def expire(self, key=None, startswith=None, endswith=None):
+        if key is not None:
+            try:
+                super().__delitem__(key)
+            except Exception:
+                pass
+        else:
+            for i in tuple(self.keys()):
+                cond1 = startswith is not None and i.startswith(startswith)
+                cond2 = endswith is not None and i.endswith(endswith)
+                if cond1 and cond2:
+                    super().__delitem__(i)
+                elif cond1:
+                    super().__delitem__(i)
+                elif cond2:
+                    super().__delitem__(i)
+                else:
+                    pass
 
 
 __cache__ = __Cache()
 plat = platform.system()
 if plat == 'Windows':
     from . import windows
     method = windows
@@ -816,9 +1001,9 @@
     method = linux
 elif plat == 'Darwin':
     raise NotImplementedError('MAC is not yet supported')
 else:
     raise NotImplementedError(f'{plat} is not yet supported')
 del(plat)
 
-__version__ = '0.8.6'
+__version__ = '0.9.0'
 __author__ = 'Crozzers'
```

### Comparing `screen_brightness_control-0.8.6/screen_brightness_control/__main__.py` & `screen_brightness_control-0.9.0/screen_brightness_control/__main__.py`

 * *Files identical despite different names*

### Comparing `screen_brightness_control-0.8.6/screen_brightness_control/linux.py` & `screen_brightness_control-0.9.0/screen_brightness_control/linux.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,33 @@
 import subprocess
 import os
-import struct
-from . import flatten_list, _monitor_brand_lookup, filter_monitors, __cache__
-from typing import List, Tuple, Union, Optional
-
-
-class _EDID:
-    '''
-    Simple structure and method to extract monitor serial and name from an EDID string.
-
-    The EDID parsing was created with inspiration from the [pyedid library](https://github.com/jojonas/pyedid)
-    '''
-    EDID_FORMAT = (
-        ">"     # big-endian
-        "8s"    # constant header (8 bytes)
-        "H"     # manufacturer id (2 bytes)
-        "H"     # product id (2 bytes)
-        "I"     # serial number (4 bytes)
-        "B"     # manufactoring week (1 byte)
-        "B"     # manufactoring year (1 byte)
-        "B"     # edid version (1 byte)
-        "B"     # edid revision (1 byte)
-        "B"     # video input type (1 byte)
-        "B"     # horizontal size in cm (1 byte)
-        "B"     # vertical size in cm (1 byte)
-        "B"     # display gamma (1 byte)
-        "B"     # supported features (1 byte)
-        "10s"   # color characteristics (10 bytes)
-        "H"     # supported timings (2 bytes)
-        "B"     # reserved timing (1 byte)
-        "16s"   # EDID supported timings (16 bytes)
-        "18s"   # detailed timing block 1 (18 bytes)
-        "18s"   # detailed timing block 2 (18 bytes)
-        "18s"   # detailed timing block 3 (18 bytes)
-        "18s"   # detailed timing block 4 (18 bytes)
-        "B"     # extension flag (1 byte)
-        "B"     # checksum (1 byte)
-    )
-
-    @classmethod
-    def parse_edid(cls, edid: str) -> Tuple[Union[str, None], str]:
-        '''
-        Takes an EDID string (as string hex, formatted as: '00ffffff00...') and
-        attempts to extract the monitor's name and serial number from it
-
-        Args:
-            edid (str): the edid string
-
-        Returns:
-            tuple: First item can be None or str.
-                Second item is always str
-
-        Example:
-            ```python
-            import screen_brightness_control as sbc
-
-            edid = sbx.linux.list_monitors_info()[0]['edid']
-            name, serial = sbc.linux._EDID.parse_edid(edid)
-            if name is not None:
-                print('Success!')
-                print('Name:', name)
-                print('Serial:', serial)
-            else:
-                print('Unable to extract the data')
-            ```
-        '''
-        def filter_hex(st):
-            st = str(st)
-            while '\\x' in st:
-                i = st.index('\\x')
-                st = st.replace(st[i:i + 4], '')
-            return st.replace('\\n', '')[2:-1]
-
-        if ' ' in edid:
-            edid = edid.replace(' ', '')
-        edid = bytes.fromhex(edid)
-        data = struct.unpack(cls.EDID_FORMAT, edid)
-        serial = filter_hex(data[18])
-        # other info can be anywhere in this range, I don't know why
-        name = None
-        for i in data[19:22]:
-            try:
-                st = str(i)[2:-1].rstrip(' ').rstrip('\t')
-                if st.index(' ') < len(st) - 1:
-                    name = filter_hex(i).split(' ')
-                    name = name[0].lower().capitalize() + ' ' + name[1]
-            except Exception:
-                pass
-        return name, serial
+from . import flatten_list, _monitor_brand_lookup, filter_monitors, __cache__, EDID
+from typing import List, Union, Optional
+import warnings
+
+# edid class used to be defined here as _EDID
+_EDID = EDID
+
+
+def warn_deprecated(name, alternative=None):
+    '''Temporary function to warn you that things have been deprecated
+    and will be removed in the next update.'''
+    if alternative is None:
+        alternative = name
+
+    msg = f'screen_brightness_control.linux.{name} is deprecated.'
+    if alternative:
+        msg += f' Use screen_brightness_control.{alternative} instead'
+    warnings.warn(msg, DeprecationWarning)
 
 
 class Light:
     '''collection of screen brightness related methods using the light executable'''
 
-    executable = 'light'
+    executable: str = 'light'
     '''the light executable to be called'''
 
     @classmethod
     def get_display_info(cls, display: Optional[Union[int, str]] = None) -> List[dict]:
         '''
         Returns information about detected displays as reported by Light
 
@@ -120,166 +50,144 @@
             # get info about the primary monitor
             primary_info = sbc.linux.Light.get_display_info(0)[0]
 
             # get info about a monitor called 'edp-backlight'
             edp_info = sbc.linux.Light.get_display_info('edp-backlight')[0]
             ```
         '''
-        try:
-            displays = __cache__.get('light_monitors_info')
-        except Exception:
-            res = subprocess.run([cls.executable, '-L'], stdout=subprocess.PIPE).stdout.decode().split('\n')
-            displays = []
-            count = 0
-            for r in res:
-                if 'backlight' in r and 'sysfs/backlight/auto' not in r:
-                    r = r[r.index('backlight/') + 10:]
-                    if os.path.isfile(f'/sys/class/backlight/{r}/device/edid'):
-                        tmp = {
-                            'name': r,
-                            'path': f'/sys/class/backlight/{r}',
-                            'light_path': f'sysfs/backlight/{r}',
-                            'method': cls,
-                            'index': count,
-                            'model': None,
-                            'serial': None,
-                            'manufacturer': None,
-                            'manufacturer_id': None,
-                            'edid': None
-                        }
-                        count += 1
+        res = subprocess.run([cls.executable, '-L'], stdout=subprocess.PIPE).stdout.decode().split('\n')
+        displays = []
+        count = 0
+        for r in res:
+            if 'backlight' in r and 'sysfs/backlight/auto' not in r:
+                r = r[r.index('backlight/') + 10:]
+                if os.path.isfile(f'/sys/class/backlight/{r}/device/edid'):
+                    tmp = {
+                        'name': r,
+                        'path': f'/sys/class/backlight/{r}',
+                        'light_path': f'sysfs/backlight/{r}',
+                        'method': cls,
+                        'index': count,
+                        'model': None,
+                        'serial': None,
+                        'manufacturer': None,
+                        'manufacturer_id': None,
+                        'edid': None
+                    }
+                    count += 1
+                    try:
+                        out = subprocess.check_output(
+                            ['hexdump', tmp['path'] + '/device/edid'],
+                            stderr=subprocess.DEVNULL
+                        ).decode().split('\n')
+                        # either the hexdump reports each hex char backwards (ff00 instead of 00ff)
+                        # or both xrandr and ddcutil do. So I swap these bits around
+                        edid = ''
+                        for line in out:
+                            for i in line.split(' '):
+                                if len(i) == 4:
+                                    edid += i[2:] + i[:2]
+                        tmp['edid'] = edid
+                        name, serial = EDID.parse_edid(edid)
+                        if name is not None:
+                            tmp['serial'] = serial
+                            tmp['name'] = name
                         try:
-                            out = subprocess.check_output(
-                                ['hexdump', tmp['path'] + '/device/edid'],
-                                stderr=subprocess.DEVNULL
-                            ).decode().split('\n')
-                            # either the hexdump reports each hex char backwards (ff00 instead of 00ff)
-                            # or both xrandr and ddcutil do. So I swap these bits around
-                            edid = ''
-                            for line in out:
-                                for i in line.split(' '):
-                                    if len(i) == 4:
-                                        edid += i[2:] + i[:2]
-                            tmp['edid'] = edid
-                            name, serial = _EDID.parse_edid(edid)
-                            if name is not None:
-                                tmp['serial'] = serial
-                                tmp['name'] = name
-                            try:
-                                tmp['manufacturer_id'], tmp['manufacturer'] = _monitor_brand_lookup(name.split(' ')[0])
-                            except Exception:
-                                tmp['manufacturer'] = name.split(' ')[0]
-                                tmp['manufacturer_id'] = None
-                            tmp['model'] = name.split(' ')[1]
+                            tmp['manufacturer_id'], tmp['manufacturer'] = _monitor_brand_lookup(name.split(' ')[0])
                         except Exception:
-                            pass
-                        displays.append(tmp)
-            __cache__.store('light_monitors_info', displays)
+                            tmp['manufacturer'] = name.split(' ')[0]
+                            tmp['manufacturer_id'] = None
+                        tmp['model'] = name.split(' ')[1]
+                    except Exception:
+                        pass
+                    displays.append(tmp)
 
         if display is not None:
             displays = filter_monitors(display=display, haystack=displays, include=['path', 'light_path'])
         return displays
 
     @classmethod
     def get_display_names(cls) -> List[str]:
         '''
+        **DEPRECATED**.
         Returns the names of each display, as reported by light
 
         Returns:
             list: list of strings
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             names = sbc.linux.Light.get_display_names()
             # EG output: ['edp-backlight']
             ```
         '''
+        warn_deprecated('Light.get_display_names', 'list_monitors(method="light")')
         return [i['name'] for i in cls.get_display_info()]
 
     @classmethod
-    def set_brightness(
-        cls, value: int,
-        display: Optional[Union[int, str]] = None,
-        no_return: bool = False
-    ) -> Union[List[int], None]:
+    def set_brightness(cls, value: int, display: Optional[int] = None):
         '''
         Sets the brightness for a display using the light executable
 
         Args:
             value (int): Sets the brightness to this value
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial, path or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
-            no_return (bool): if True, this function returns None
-
-        Returns:
-            list: list of ints (0 to 100) (the result of `Light.get_brightness`)
-            None: if the `no_return` kwarg is True
+            display (int): The specific display you wish to query.
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # set the brightness to 50%
             sbc.linux.Light.set_brightness(50)
 
             # set the primary display brightness to 75%
             sbc.linux.Light.set_brightness(75, display = 0)
 
-            # set the display called 'edp-backlight' to 25%
-            sbc.linux.Light.set_brightness(75, display = 'edp-backlight')
+            # set the secondary display brightness to 25%
+            sbc.linux.Light.set_brightness(75, display = 1)
             ```
         '''
         info = cls.get_display_info()
         if display is not None:
-            if type(display) == int:
-                info = [info[display]]
-            else:
-                info = filter_monitors(display=display, haystack=info, include=['path', 'light_path'])
+            info = [info[display]]
+
         for i in info:
             subprocess.call(f'{cls.executable} -S {value} -s {i["light_path"]}'.split(" "))
-        return cls.get_brightness(display=display) if not no_return else None
 
     @classmethod
-    def get_brightness(cls, display: Optional[Union[int, str]] = None) -> List[int]:
+    def get_brightness(cls, display: Optional[int] = None) -> List[int]:
         '''
         Sets the brightness for a display using the light executable
 
         Args:
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial, path or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
+            display (int): The specific display you wish to query.
 
         Returns:
             list: list of ints (0 to 100)
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # get the current display brightness
             current_brightness = sbc.linux.Light.get_brightness()
 
             # get the brightness of the primary display
             primary_brightness = sbc.linux.Light.get_brightness(display = 0)[0]
 
-            # get the brightness of the display called 'edp-backlight'
-            edp_brightness = sbc.linux.Light.get_brightness(display = 'edp-backlight')[0]
+            # get the brightness of the secondary display
+            edp_brightness = sbc.linux.Light.get_brightness(display = 1)[0]
             ```
         '''
         info = cls.get_display_info()
         if display is not None:
-            if type(display) == int:
-                info = [info[display]]
-            else:
-                info = filter_monitors(display=display, haystack=info, include=['path', 'light_path'])
+            info = [info[display]]
+
         results = []
         for i in info:
             results.append(
                 subprocess.check_output(
                     [
                         cls.executable, '-G', '-s', i['light_path']
                     ]
@@ -288,48 +196,44 @@
         results = [int(round(float(i.decode()), 0)) for i in results]
         return results
 
 
 class XBacklight:
     '''collection of screen brightness related methods using the xbacklight executable'''
 
-    executable = 'xbacklight'
+    executable: str = 'xbacklight'
     '''the xbacklight executable to be called'''
 
     @classmethod
-    def set_brightness(cls, value: int, no_return: bool = False, **kwargs) -> Union[int, None]:
+    def set_brightness(cls, value: int, **kwargs):
         '''
         Sets the screen brightness to a supplied value
 
         Args:
-            no_return (bool): if True, this function returns None
-                Returns the result of `XBacklight.get_brightness()` otherwise
-
-        Returns:
-            int: from 0 to 100
-            None: if `no_return` is set to `True`
+            value (int): the value to set the brightnes to
+            **kwargs: arbitrary keyword arguments. Ignored
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # set the brightness to 100%
             sbc.linux.XBacklight.set_brightness(100)
             ```
         '''
         subprocess.call([cls.executable, '-set', str(value)])
-        return cls.get_brightness() if not no_return else None
 
     @classmethod
     def get_brightness(cls, **kwargs) -> int:
         '''
         Returns the screen brightness as reported by xbacklight
 
         Returns:
             int: from 0 to 100
+            **kwargs: arbitrary keyword arguments. Ignored
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             current_brightness = sbc.linux.XBacklight.get_brightness()
             ```
@@ -340,26 +244,28 @@
         ).stdout.decode()
         return int(round(float(str(res)), 0))
 
 
 class XRandr:
     '''collection of screen brightness related methods using the xrandr executable'''
 
-    executable = 'xrandr'
+    executable: str = 'xrandr'
     '''the xrandr executable to be called'''
 
     @classmethod
-    def get_display_info(cls, display: Optional[Union[int, str]] = None) -> List[dict]:
+    def get_display_info(cls, display: Optional[Union[int, str]] = None, brightness: bool = False) -> List[dict]:
         '''
         Returns info about all detected monitors as reported by xrandr
 
         Args:
             display (str or int): [*Optional*] The monitor to return info about.
                 Pass in the serial number, name, model, interface, edid or index.
                 This is passed to `filter_monitors`
+            brightness (bool): whether to include the current brightness
+                in the returned info
 
         Returns:
             list: list of dicts
 
         Example:
             ```python
             import screen_brightness_control as sbc
@@ -381,118 +287,113 @@
             if tmp != {}:
                 if tmp['serial'] is None or '\\x' not in tmp['serial']:
                     if 'line' in tmp:
                         del(tmp['line'])
                     return True
             return False
 
-        try:
-            data = __cache__.get('xrandr_monitors_info')
-        except Exception:
-            out = subprocess.check_output([cls.executable, '--verbose']).decode().split('\n')
-            names = cls.get_display_interfaces()
-            data = []
-            tmp = {}
-            count = 0
-            for i in out:
-                if i != '':
-                    if i.startswith(tuple(names)):
-                        if check_tmp(tmp):
-                            data.append(tmp)
-                        tmp = {
-                            'interface': i.split(' ')[0],
-                            'name': i.split(' ')[0],
-                            'line': i,
-                            'method': cls,
-                            'index': count,
-                            'model': None,
-                            'serial': None,
-                            'manufacturer': None,
-                            'manufacturer_id': None,
-                            'edid': None
-                        }
-                        count += 1
-                    elif 'EDID:' in i:
-                        st = out[out.index(tmp['line']):]
-                        edid = []
-                        for j in range(st.index(i) + 1, st.index(i) + 9):
-                            edid.append(st[j].replace('\t', '').replace(' ', ''))
-                        edid = ''.join(edid)
-                        tmp['edid'] = edid
-                        name, serial = _EDID.parse_edid(edid)
-                        tmp['name'] = name if name is not None else tmp['interface']
-                        if name is not None:
-                            tmp['manufacturer'] = name.split(' ')[0]
-                            try:
-                                tmp['manufacturer_id'], tmp['manufacturer'] = _monitor_brand_lookup(
-                                    tmp['manufacturer']
-                                )
-                            except Exception:
-                                tmp['manufacturer_id'] = None
-                            tmp['model'] = name.split(' ')[1]
-                            tmp['serial'] = serial
-                    elif 'Brightness:' in i:
-                        tmp['brightness'] = int(
-                            float(i.replace('Brightness:', '').replace(' ', '').replace('\t', '')) * 100
-                        )
-            if check_tmp(tmp):
-                data.append(tmp)
+        out = subprocess.check_output([cls.executable, '--verbose']).decode().split('\n')
+        names = cls.get_display_interfaces()
+        data = []
+        tmp = {}
+        count = 0
+        for i in out:
+            if i != '':
+                if i.startswith(tuple(names)):
+                    if check_tmp(tmp):
+                        data.append(tmp)
+                    tmp = {
+                        'interface': i.split(' ')[0],
+                        'name': i.split(' ')[0],
+                        'line': i,
+                        'method': cls,
+                        'index': count,
+                        'model': None,
+                        'serial': None,
+                        'manufacturer': None,
+                        'manufacturer_id': None,
+                        'edid': None
+                    }
+                    count += 1
+                elif 'EDID:' in i:
+                    st = out[out.index(tmp['line']):]
+                    edid = []
+                    for j in range(st.index(i) + 1, st.index(i) + 9):
+                        edid.append(st[j].replace('\t', '').replace(' ', ''))
+                    edid = ''.join(edid)
+                    tmp['edid'] = edid
+                    name, serial = EDID.parse_edid(edid)
+                    tmp['name'] = name if name is not None else tmp['interface']
+                    if name is not None:
+                        tmp['manufacturer'] = name.split(' ')[0]
+                        try:
+                            tmp['manufacturer_id'], tmp['manufacturer'] = _monitor_brand_lookup(
+                                tmp['manufacturer']
+                            )
+                        except Exception:
+                            tmp['manufacturer_id'] = None
+                        tmp['model'] = name.split(' ')[1]
+                        tmp['serial'] = serial
+                elif 'Brightness:' in i and brightness:
+                    tmp['brightness'] = int(
+                        float(i.replace('Brightness:', '').replace(' ', '').replace('\t', '')) * 100
+                    )
+        if check_tmp(tmp):
+            data.append(tmp)
 
-            __cache__.store('xrandr_monitors_info', data)
         if display is not None:
             data = filter_monitors(display=display, haystack=data, include=['interface'])
         return data
 
-    @staticmethod
-    def get_display_interfaces() -> List[str]:
+    @classmethod
+    def get_display_interfaces(cls) -> List[str]:
         '''
         Returns the interfaces of each display, as reported by xrandr
 
         Returns:
             list: list of strings
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
-            names = sbc.linux.XRandr.get_display_names()
+            names = sbc.linux.XRandr.get_display_interfaces()
             # EG output: ['eDP-1', 'HDMI1', 'HDMI2']
             ```
         '''
-        out = subprocess.check_output(['xrandr', '-q']).decode().split('\n')
+        out = subprocess.check_output([cls.executable, '-q']).decode().split('\n')
         return [i.split(' ')[0] for i in out if 'connected' in i and 'disconnected' not in i]
 
     @classmethod
     def get_display_names(cls) -> List[str]:
         '''
+        **DEPRECATED**.
         Returns the names of each display, as reported by xrandr
 
         Returns:
             list: list of strings
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             names = sbc.linux.XRandr.get_display_names()
             # EG output: ['BenQ GL2450HM', 'Dell U2211H']
             ```
         '''
+        warn_deprecated('XRandr.get_display_names', 'list_monitors(method="xrandr")')
         return [i['name'] for i in cls.get_display_info()]
 
     @classmethod
-    def get_brightness(cls, display: Optional[Union[int, str]] = None) -> List[int]:
+    def get_brightness(cls, display: Optional[int] = None) -> List[int]:
         '''
         Returns the brightness for a display using the xrandr executable
 
         Args:
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial, interface or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
+            display (int): The specific display you wish to query.
 
         Returns:
             list: list of integers (from 0 to 100)
 
         Example:
             ```python
             import screen_brightness_control as sbc
@@ -500,45 +401,29 @@
             # get the current brightness
             current_brightness = sbc.linux.XRandr.get_brightness()
 
             # get the current brightness for the primary display
             primary_brightness = sbc.linux.XRandr.get_brightness(display=0)[0]
             ```
         '''
-        monitors = cls.get_display_info()
+        monitors = cls.get_display_info(brightness=True)
         if display is not None:
-            if type(display) == int:
-                monitors = [monitors[display]]
-            else:
-                monitors = filter_monitors(display=display, haystack=monitors, include=['interface'])
+            monitors = [monitors[display]]
         brightness = [i['brightness'] for i in monitors]
 
         return brightness
 
     @classmethod
-    def set_brightness(
-        cls, value: int,
-        display: Optional[Union[int, str]] = None,
-        no_return: bool = False
-    ) -> Union[List[int], None]:
+    def set_brightness(cls, value: int, display: Optional[int] = None):
         '''
         Sets the brightness for a display using the xrandr executable
 
         Args:
             value (int): Sets the brightness to this value
             display (int): The specific display you wish to query.
-                Can be index, name, model, serial, interface or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
-            no_return (bool): if True, this function returns None
-                Returns the result of `XRandr.get_brightness()` otherwise
-
-        Returns:
-            list: list of ints (0 to 100) (the result of `XRandr.get_brightness`)
-            None: if the `no_return` kwarg is True
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # set the brightness to 50
             sbc.linux.XRandr.set_brightness(50)
@@ -546,39 +431,30 @@
             # set the brightness of the primary display to 75
             sbc.linux.XRandr.set_brightness(75, display=0)
             ```
         '''
         value = str(float(value) / 100)
         info = cls.get_display_info()
         if display is not None:
-            if type(display) == int:
-                info = [info[display]]
-            else:
-                info = filter_monitors(
-                    display=display,
-                    haystack=info,
-                    include=['interface']
-                )
+            info = [info[display]]
 
         for i in info:
             subprocess.run([cls.executable, '--output', i['interface'], '--brightness', value])
 
         # The get_brightness method takes the brightness value from get_display_info
         # The problem is that that display info is cached, meaning that the brightness
         # value is also cached. We must expire it here.
-        __cache__.expire('xrandr_monitors_info')
-        return cls.get_brightness(display=display) if not no_return else None
 
 
 class DDCUtil:
     '''collection of screen brightness related methods using the ddcutil executable'''
 
-    executable = 'ddcutil'
+    executable: str = 'ddcutil'
     '''the ddcutil executable to be called'''
-    sleep_multiplier = 0.5
+    sleep_multiplier: float = 0.5
     '''how long ddcutil should sleep between each DDC request (lower is shorter).
     See [the ddcutil docs](https://www.ddcutil.com/performance_options/) for more info.'''
 
     @classmethod
     def get_display_info(cls, display: Optional[Union[int, str]] = None) -> List[dict]:
         '''
         Returns information about all DDC compatible monitors shown by DDCUtil
@@ -612,17 +488,16 @@
         def check_tmp(tmp):
             if tmp != {} and 'Invalid display' not in tmp['tmp']:
                 if 'tmp' in tmp:
                     del(tmp['tmp'])
                 return True
             return False
 
-        try:
-            data = __cache__.get('ddcutil_monitors_info')
-        except Exception:
+        data = __cache__.get('ddcutil_monitors_info')
+        if data is None:
             out = []
             # Use -v to get EDID string but this means output cannot be decoded.
             # Or maybe it can. I don't know the encoding though, so let's assume it cannot be decoded.
             # Use str()[2:-1] workaround
             cmd_out = str(
                 subprocess.check_output(
                     [
@@ -692,39 +567,38 @@
         if display is not None:
             data = filter_monitors(display=display, haystack=data, include=['i2c_bus'])
         return data
 
     @classmethod
     def get_display_names(cls) -> List[str]:
         '''
+        **DEPRECATED**.
         Returns the names of each display, as reported by ddcutil
 
         Returns:
             list: list of strings
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             names = sbc.linux.DDCUtil.get_display_names()
             # EG output: ['Dell U2211H', 'BenQ GL2450H']
             ```
         '''
+        warn_deprecated('DDCUtil.get_display_names', 'list_monitors(method="ddcutil")')
         return [i['name'] for i in cls.get_display_info()]
 
     @classmethod
-    def get_brightness(cls, display: Optional[Union[int, str]] = None) -> List[int]:
+    def get_brightness(cls, display: Optional[int] = None) -> List[int]:
         '''
         Returns the brightness for a display using the ddcutil executable
 
         Args:
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial, i2c bus or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
+            display (int): The specific display you wish to query.
 
         Returns:
             list: list of ints (0 to 100)
 
         Example:
             ```python
             import screen_brightness_control as sbc
@@ -734,25 +608,20 @@
 
             # get the current brightness for the primary display
             primary_brightness = sbc.linux.DDCUtil.get_brightness(display=0)[0]
             ```
         '''
         monitors = cls.get_display_info()
         if display is not None:
-            if type(display) == int:
-                monitors = [monitors[display]]
-            else:
-                monitors = filter_monitors(display=display, haystack=monitors, include=['i2c_bus'])
+            monitors = [monitors[display]]
+
         res = []
         for m in monitors:
-            try:
-                out = __cache__.get('ddcutil_' + m['edid'] + '_brightness')
-                if out is None:
-                    raise Exception
-            except Exception:
+            out = __cache__.get('ddcutil_' + m['edid'] + '_brightness')
+            if out is None:
                 out = subprocess.check_output(
                     [
                         cls.executable,
                         'getvcp', '10', '-t',
                         '-b', str(m['bus_number']),
                         f'--sleep-multiplier={cls.sleep_multiplier}'
                     ]
@@ -761,69 +630,47 @@
             try:
                 res.append(int(out))
             except Exception:
                 pass
         return res
 
     @classmethod
-    def set_brightness(
-        cls, value: int,
-        display: Optional[Union[int, str]] = None,
-        no_return: bool = False
-    ) -> Union[List[int], None]:
+    def set_brightness(cls, value: int, display: Optional[int] = None):
         '''
         Sets the brightness for a display using the ddcutil executable
 
         Args:
             value (int): Sets the brightness to this value
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial, i2c bus or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
-            no_return (bool): if True, this function returns None.
-                Returns the result of `DDCUtil.get_brightness()` otherwise
-
-        Returns:
-            list: list of ints (0 to 100)
-            None: if `no_return` is True
+            display (int): The specific display you wish to query.
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # set the brightness to 50
             sbc.linux.DDCUtil.set_brightness(50)
 
             # set the brightness of the primary display to 75
             sbc.linux.DDCUtil.set_brightness(75, display=0)
             ```
         '''
         monitors = cls.get_display_info()
         if display is not None:
-            if type(display) == int:
-                monitors = [monitors[display]]
-            else:
-                monitors = filter_monitors(display=display, haystack=monitors, include=['i2c_bus'])
+            monitors = [monitors[display]]
 
         __cache__.expire(startswith='ddcutil_', endswith='_brightness')
         for m in monitors:
             subprocess.run(
                 [
-                    cls.executable,
-                    'setvcp',
-                    '10',
-                    str(value),
-                    '-b',
-                    str(m['bus_number']),
+                    cls.executable, 'setvcp', '10', str(value),
+                    '-b', str(m['bus_number']),
                     f'--sleep-multiplier={cls.sleep_multiplier}'
                 ]
             )
 
-        return cls.get_brightness(display=display) if not no_return else None
-
 
 def list_monitors_info(method: Optional[str] = None, allow_duplicates: bool = False) -> List[dict]:
     '''
     Lists detailed information about all detected monitors
 
     Args:
         method (str): the method the monitor can be addressed by. Can be 'xrandr' or 'ddcutil' or 'light'
@@ -838,40 +685,32 @@
     Example:
         ```python
         import screen_brightness_control as sbc
 
         monitors = sbc.linux.list_monitors_info()
         for monitor in monitors:
             print('=======================')
-
             # the manufacturer name plus the model OR a generic name for the monitor, depending on the method
             print('Name:', monitor['name'])
-
             # the general model of the display
             print('Model:', monitor['model'])
-
-            # a unique string assigned by Windows to this display
+            # the serial of the display
             print('Serial:', monitor['serial'])
-
             # the name of the brand of the monitor
             print('Manufacturer:', monitor['manufacturer'])
-
             # the 3 letter code corresponding to the brand name, EG: BNQ -> BenQ
             print('Manufacturer ID:', monitor['manufacturer_id'])
-
             # the index of that display FOR THE SPECIFIC METHOD THE DISPLAY USES
             print('Index:', monitor['index'])
-
             # the method this monitor can be addressed by
             print('Method:', monitor['method'])
         ```
     '''
-    try:
-        return __cache__.get('linux_monitors_info', method=method, allow_duplicates=allow_duplicates)
-    except Exception:
+    info = __cache__.get('linux_monitors_info', method=method, allow_duplicates=allow_duplicates)
+    if info is None:
         methods = [XRandr, DDCUtil, Light]
         if method is not None:
             method = method.lower()
             if method not in ('xrandr', 'ddcutil', 'light'):
                 raise ValueError('method must be \'xrandr\' or \'ddcutil\' or \'light\' to get monitor information')
 
         info = []
@@ -885,19 +724,20 @@
                     pass
                 else:
                     for i in tmp:
                         if allow_duplicates or i['edid'] not in edids:
                             edids.append(i['edid'])
                             info.append(i)
         __cache__.store('linux_monitors_info', info, method=method, allow_duplicates=allow_duplicates)
-        return info
+    return info
 
 
 def list_monitors(method: Optional[str] = None) -> List[str]:
     '''
+    **DEPRECATED**.
     Returns the names of all detected monitors
 
     Args:
         method (str): the method the monitor can be addressed by. Can be 'xrandr' or 'ddcutil' or 'light'
 
     Returns:
         list: list of strings
@@ -906,20 +746,22 @@
         ```python
         import screen_brightness_control as sbc
 
         monitors = sbc.linux.list_monitors()
         # EG output: ['BenQ GL2450HM', 'Dell U2211H', 'edp-backlight']
         ```
     '''
+    warn_deprecated('list_monitors')
     displays = [i['name'] for i in list_monitors_info(method=method)]
     return flatten_list(displays)
 
 
 def get_brightness_from_sysfiles(display: int = None) -> int:
     '''
+    **DEPRECATED**.
     Returns the current display brightness by reading files from `/sys/class/backlight`
 
     Args:
         display (int): The index of the display you wish to query
 
     Returns:
         int: from 0 to 100
@@ -932,14 +774,15 @@
         ```python
         import screen_brightness_control as sbc
 
         brightness = sbc.linux.get_brightness_from_sysfiles()
         # Eg Output: 100
         ```
     '''
+    warn_deprecated('get_brightness_from_sysfiles', False)
     backlight_dir = '/sys/class/backlight/'
     error = []
     # if function has not returned yet try reading the brightness file
     if os.path.isdir(backlight_dir) and os.listdir(backlight_dir) != []:
         # if the backlight dir exists and is not empty
         folders = [dir for dir in os.listdir(backlight_dir) if os.path.isdir(os.path.join(backlight_dir, dir))]
         if display is not None:
@@ -967,17 +810,19 @@
             exc += f'\n    {e[0]}: {e[1]}'
         raise Exception(exc)
     raise FileNotFoundError(f'Backlight directory {backlight_dir} not found')
 
 
 def __set_and_get_brightness(*args, display=None, method=None, meta_method='get', **kwargs) -> Union[List[int], None]:
     '''
+    **DEPRECATED**.
     Internal function, do not call. Either sets the brightness or gets it.
     Exists because set_brightness and get_brightness only have a couple differences
     '''
+    warn_deprecated('__set_and_get_brightness', '__brightness')
     errors = []
     try:  # filter known list of monitors according to kwargs
         if type(display) == int:
             monitors = [list_monitors_info(method=method)[display]]
         else:
             monitors = filter_monitors(display=display, method=method)
     except Exception as e:
@@ -1024,14 +869,15 @@
 def set_brightness(
     value: int,
     display: Optional[Union[int, str]] = None,
     method: Optional[str] = None,
     **kwargs
 ) -> Union[List[int], int, None]:
     '''
+    **DEPRECATED**.
     Sets the brightness for a display, cycles through Light, XRandr, DDCUtil and XBacklight methods until one works
 
     Args:
         value (int): Sets the brightness to this value
         display (int or str): The specific display you wish to adjust.
             Can be index, model, name or serial of the display.
             Can also be i2c bus (ddcutil), interface (xrandr) or path (light)
@@ -1059,26 +905,28 @@
         # set brightness of the primary display to 75%
         sbc.linux.set_brightness(75, display=0)
 
         # set the brightness to 25% via the XRandr method
         sbc.linux.set_brightness(25, method='xrandr')
         ```
     '''
+    warn_deprecated('set_brightness')
     if method is not None and method.lower() == 'xbacklight':
         return XBacklight.set_brightness(value, **kwargs)
     else:
         return __set_and_get_brightness(value, display=display, method=method, meta_method='set', **kwargs)
 
 
 def get_brightness(
     display: Optional[Union[int, str]] = None,
     method: Optional[str] = None,
     **kwargs
 ) -> Union[List[int], int]:
     '''
+    **DEPRECATED**.
     Returns the brightness for a display, cycles through Light, XRandr, DDCUtil and XBacklight methods until one works
 
     Args:
         display (int or str): The specific display you wish to adjust.
             Can be index, model, name or serial of the display.
             Can also be i2c bus (ddcutil), interface (xrandr) or path (light)
         method (str): the method to use ('light', 'xrandr', 'ddcutil' or 'xbacklight')
@@ -1107,11 +955,12 @@
         # get the brightness via the XRandr method
         xrandr_brightness = sbc.linux.get_brightness(method='xrandr')
 
         # get the brightness of the secondary display using Light
         light_brightness = sbc.get_brightness(display=1, method='light')[0]
         ```
     '''
+    warn_deprecated('get_brightness')
     if method is not None and method.lower() == 'xbacklight':
         return XBacklight.get_brightness(**kwargs)
     else:
         return __set_and_get_brightness(display=display, method=method, meta_method='get', **kwargs)
```

### Comparing `screen_brightness_control-0.8.6/screen_brightness_control/windows.py` & `screen_brightness_control-0.9.0/screen_brightness_control/windows.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,35 @@
 import threading
 import pythoncom
 import win32api
 import time
 import ctypes
 from ctypes import windll, byref, Structure, WinError, POINTER, WINFUNCTYPE
 from ctypes.wintypes import BOOL, HMONITOR, HDC, RECT, LPARAM, DWORD, BYTE, WCHAR, HANDLE
-from . import flatten_list, _monitor_brand_lookup, filter_monitors, __cache__, platform
+from . import flatten_list, _monitor_brand_lookup, filter_monitors, __cache__, platform, EDID
 from typing import List, Union, Optional
+import warnings
 # a bunch of typing classes were deprecated in Python 3.9
 # in favour of collections.abc (https://www.python.org/dev/peps/pep-0585/)
 if int(platform.python_version_tuple()[1]) < 9:
-    from typing import Iterable
+    from typing import Generator
 else:
-    from collections.abc import Iterable
+    from collections.abc import Generator
+
+
+def warn_deprecated(name, alternative=None):
+    '''Temporary function to warn you that things have been deprecated
+    and will be removed in the next update.'''
+    if alternative is None:
+        alternative = name
+
+    msg = f'screen_brightness_control.windows.{name} is deprecated.'
+    if alternative:
+        msg += f' Use screen_brightness_control.{alternative} instead'
+    warnings.warn(msg, DeprecationWarning)
 
 
 def _wmi_init():
     '''internal function to create and return a wmi instance'''
     # WMI calls don't work in new threads so we have to run this check
     if threading.current_thread() != threading.main_thread():
         pythoncom.CoInitialize()
@@ -37,18 +50,16 @@
         import screen_brightness_control as s
 
         info = s.windows.get_display_info()
         for display in info:
             print(display['name'])
         ```
     '''
-    try:
-        info = __cache__.get('windows_monitors_info_raw')
-    except Exception:
-        info = []
+    info = __cache__.get('windows_monitors_info_raw')
+    if info is None:
         try:
             # collect all monitor UIDs (derived from DeviceID)
             monitor_uids = {}
             last_good = 0
             for i in win32api.EnumDisplayMonitors():
                 tmp = win32api.GetMonitorInfo(i[0])
                 try:
@@ -72,107 +83,103 @@
                                 break
                         except Exception:
                             continue
 
             # gather list of laptop displays to check against later
             wmi = _wmi_init()
             try:
-                laptop_displays = []
-                for i in wmi.WmiMonitorBrightness():
-                    laptop_displays.append(
-                        i.InstanceName.replace('_0', '', 1).split('\\')[2]
-                    )
+                laptop_displays = [
+                    i.InstanceName
+                    for i in wmi.WmiMonitorBrightness()
+                ]
             except Exception:
-                pass
-            monitors = []
-            extras = []
-            uid_keys = list(monitor_uids.keys())
-            for m in wmi.WmiMonitorID():
-                name = m.InstanceName.replace('_0', '', 1).split('\\')[2]
-                if name in uid_keys:
-                    monitors.append(m)
-                else:
-                    extras.append(m)
-
-            # sort the monitors in the same order as win32api reports them
-            # because the first item in win32api's list is usually the primary display
-            monitors = sorted(
-                monitors,
-                key=lambda x: uid_keys.index(x.InstanceName.replace('_0', '', 1).split('\\')[2])
-            )
-
-            monitors += extras
-
-            # get all available edid strings
-            try:
-                descriptors = {
-                    i.InstanceName: i.WmiGetMonitorRawEEdidV1Block(0) for i in wmi.WmiMonitorDescriptorMethods()
-                }
-            except Exception:
-                pass
-            laptop = 0
-            desktop = 0
-            for monitor in monitors:
-                model, serial, manufacturer, man_id, edid = None, None, None, None, None
-                instance_name = monitor.InstanceName.replace('_0', '', 1).split('\\')[2]
-                pydevice = monitor_uids[instance_name]
+                laptop_displays = []
 
+            extras, desktop, laptop = [], 0, 0
+            uid_keys = list(monitor_uids.keys())
+            for monitor in wmi.WmiMonitorDescriptorMethods():
                 try:
-                    serial = bytes(monitor.SerialNumberID).decode().replace('\x00', '')
-                    manufacturer, model = bytes(monitor.UserFriendlyName).decode().replace('\x00', '').split(' ')
-                    manufacturer = manufacturer.lower().capitalize()
-                    try:
-                        man_id, manufacturer = _monitor_brand_lookup(manufacturer)
-                    except Exception:
-                        man_id = None
-                except Exception:
-                    devid = pydevice.DeviceID.split('#')
-                    serial = devid[2]
-                    man_id = devid[1][:3]
-                    model = devid[3:]
-                    del(devid)
-                    try:
-                        man_id, manufacturer = _monitor_brand_lookup(man_id)
-                    except Exception:
-                        manufacturer = None
-                try:
+                    model, serial, manufacturer, man_id, edid = None, None, None, None, None
+                    instance_name = monitor.InstanceName.replace('_0', '', 1).split('\\')[2]
+                    pydevice = monitor_uids[instance_name]
+
+                    # get the EDID
                     try:
-                        chars = descriptors[monitor.InstanceName][0]
-                    except Exception:
-                        chars = descriptors[pydevice.InstanceName][0]
-                    finally:
                         edid = ''
-                        for char in chars:
-                            char = str(hex(char)).replace('0x', '')
+                        for char in monitor.WmiGetMonitorRawEEdidV1Block(0)[0]:
+                            char = hex(char)[2:]
                             if len(char) == 1:
                                 char = '0' + char
                             edid += char
-                        del(chars)
-                except Exception:
-                    edid = None
+                    except Exception:
+                        edid = None
+
+                    # get serial, model, manufacturer and manufacturer ID
+                    try:
+                        if edid is None:
+                            raise Exception
+                        # we do the EDID parsing ourselves because calling wmi.WmiMonitorID
+                        # takes too long
+                        name, serial = EDID.parse_edid(edid)
+                        if name is None:
+                            raise Exception
+
+                        # split by last space because model numbers usually are one word
+                        # whereas brands can be multiple (EG: 'LG Electronics')
+                        manufacturer, model = name.rsplit(' ', 1)
+                        try:
+                            man_id, manufacturer = _monitor_brand_lookup(manufacturer)
+                        except Exception:
+                            man_id, manufacturer = None, manufacturer.lower().capitalize()
+                    except Exception:
+                        devid = pydevice.DeviceID.split('#')
+                        serial = devid[2]
+                        man_id = devid[1][:3]
+                        model = devid[3]
+                        del(devid)
+                        try:
+                            man_id, manufacturer = _monitor_brand_lookup(man_id)
+                        except Exception:
+                            manufacturer = None
 
-                if (serial, model) != (None, None):
-                    info.append(
-                        {
+                    if (serial, model) != (None, None):
+                        data = {
                             'name': f'{manufacturer} {model}',
                             'model': model,
                             'serial': serial,
                             'manufacturer': manufacturer,
                             'manufacturer_id': man_id,
                             'edid': edid
                         }
-                    )
-                    if instance_name in laptop_displays:
-                        info[-1]['index'] = laptop
-                        info[-1]['method'] = WMI
-                        laptop += 1
-                    else:
-                        info[-1]['index'] = desktop
-                        info[-1]['method'] = VCP
-                        desktop += 1
+                        if monitor.InstanceName in laptop_displays:
+                            data['index'] = laptop
+                            data['method'] = WMI
+                            laptop += 1
+                        else:
+                            data['method'] = VCP
+                            desktop += 1
+
+                        if instance_name in uid_keys:
+                            # insert the data into the uid_keys list because
+                            # uid_keys has the monitors sorted correctly. This
+                            # means we don't have to re-sort the list later
+                            uid_keys[uid_keys.index(instance_name)] = data
+                        else:
+                            extras.append(data)
+                except Exception:
+                    pass
+
+            info = uid_keys + extras
+            if desktop:
+                # now make sure desktop monitors have the correct index
+                count = 0
+                for item in info:
+                    if item['method'] == VCP:
+                        item['index'] = count
+                        count += 1
         except Exception:
             pass
         __cache__.store('windows_monitors_info_raw', info)
 
     return info
 
 
@@ -206,101 +213,82 @@
             # get information about the first WMI addressable monitor
             primary_info = sbc.windows.WMI.get_display_info(0)
 
             # get information about a monitor with a specific name
             benq_info = sbc.windows.WMI.get_display_info('BenQ GL2450H')
             ```
         '''
-        try:
-            info = __cache__.get('wmi_monitor_info')
-        except Exception:
+        info = __cache__.get('wmi_monitor_info')
+        if info is None:
             info = [i for i in get_display_info() if i['method'] == cls]
             __cache__.store('wmi_monitor_info', info)
         if display is not None:
             info = filter_monitors(display=display, haystack=info)
         return info
 
     @classmethod
     def get_display_names(cls) -> List[str]:
         '''
+        **DEPRECATED**.
         Returns names of all displays that can be addressed by WMI
 
         Returns:
             list: list of strings
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             for name in sbc.windows.WMI.get_display_names():
                 print(name)
             ```
         '''
+        warn_deprecated('WMI.get_display_names', 'list_monitors(method="wmi")')
         return [i['name'] for i in cls.get_display_info()]
 
     @classmethod
-    def set_brightness(
-        cls, value: int,
-        display: Optional[Union[int, str]] = None,
-        no_return: bool = False
-    ) -> Union[List[int], None]:
+    def set_brightness(cls, value: int, display: Optional[int] = None):
         '''
         Sets the display brightness for Windows using WMI
 
         Args:
             value (int): The percentage to set the brightness to
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
-            no_return (bool): if True, this function returns None
-                Otherwise it returns the result of `WMI.get_brightness()`
-
-        Returns:
-            list: list of integers (0 to 100)
-            None: if `no_return` is set to `True`
+            display (int): The specific display you wish to query.
 
         Raises:
             LookupError: if the given display cannot be found
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             # set brightness of WMI addressable monitors to 50%
             sbc.windows.WMI.set_brightness(50)
 
             # set the primary display brightness to 75%
             sbc.windows.WMI.set_brightness(75, display = 0)
 
-            # set the brightness of a named monitor to 25%
-            sbc.windows.WMI.set_brightness(25, display = 'BenQ GL2450H')
+            # set the brightness of the secondary display to 25%
+            sbc.windows.WMI.set_brightness(25, display = 1)
             ```
         '''
         brightness_method = _wmi_init().WmiMonitorBrightnessMethods()
         if display is not None:
-            if type(display) == int:
-                brightness_method = [brightness_method[display]]
-            else:
-                indexes = [i['index'] for i in filter_monitors(display=display, method='wmi')]
-                brightness_method = [brightness_method[i] for i in indexes]
+            brightness_method = [brightness_method[display]]
+
         for method in brightness_method:
             method.WmiSetBrightness(value, 0)
-        return cls.get_brightness(display=display) if not no_return else None
 
     @classmethod
-    def get_brightness(cls, display: Optional[Union[int, str]] = None) -> List[int]:
+    def get_brightness(cls, display: Optional[int] = None) -> List[int]:
         '''
         Returns the current display brightness using WMI
 
         Args:
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
+            display (int): The specific display you wish to query.
 
         Returns:
             list: list of integers (0 to 100)
 
         Raises:
             LookupError: if the given display cannot be found
 
@@ -314,25 +302,21 @@
                 print('There is only one detected display')
             else:
                 print('There are', len(current_brightness), 'detected displays')
 
             # get the primary display brightness
             primary_brightness = sbc.windows.WMI.get_brightness(display = 0)
 
-            # get the brightness of a named monitor
-            benq_brightness = sbc.windows.WMI.get_brightness(display = 'BenQ GL2450H')
+            # get the brightness of the secondary monitor
+            benq_brightness = sbc.windows.WMI.get_brightness(display = 1)
             ```
         '''
         brightness_method = _wmi_init().WmiMonitorBrightness()
         if display is not None:
-            if type(display) == int:
-                brightness_method = [brightness_method[display]]
-            else:
-                displays = cls.get_display_info(display)
-                brightness_method = [brightness_method[i['index']] for i in displays]
+            brightness_method = [brightness_method[display]]
 
         values = [i.CurrentBrightness for i in brightness_method]
         return values
 
 
 class VCP:
     '''Collection of screen brightness related methods using the DDC/CI commands'''
@@ -340,20 +324,23 @@
 
     class _PHYSICAL_MONITOR(Structure):
         '''internal class, do not call'''
         _fields_ = [('handle', HANDLE),
                     ('description', WCHAR * 128)]
 
     @classmethod
-    def iter_physical_monitors(cls) -> Iterable[ctypes.wintypes.HANDLE]:
+    def iter_physical_monitors(cls, start: int = 0) -> Generator[ctypes.wintypes.HANDLE, None, None]:
         '''
         A generator to iterate through all physical monitors
         and then close them again afterwards, yielding their handles.
         It is not recommended to use this function unless you are familiar with `ctypes` and `windll`
 
+        Args:
+            start (int): skip the first X handles
+
         Yields:
             ctypes.wintypes.HANDLE
 
         Raises:
             ctypes.WinError: upon failure to enumerate through the monitors
 
         Example:
@@ -367,27 +354,35 @@
         def callback(hmonitor, hdc, lprect, lparam):
             monitors.append(HMONITOR(hmonitor))
             return True
 
         monitors = []
         if not windll.user32.EnumDisplayMonitors(None, None, cls._MONITORENUMPROC(callback), None):
             raise WinError('EnumDisplayMonitors failed')
+
+        index = 0
+
         for monitor in monitors:
             # Get physical monitor count
             count = DWORD()
             if not windll.dxva2.GetNumberOfPhysicalMonitorsFromHMONITOR(monitor, byref(count)):
                 raise WinError()
             if count.value > 0:
+                if start and index + count.value < start:
+                    index += count.value
+                    continue
                 # Get physical monitor handles
                 physical_array = (cls._PHYSICAL_MONITOR * count.value)()
                 if not windll.dxva2.GetPhysicalMonitorsFromHMONITOR(monitor, count.value, physical_array):
                     raise WinError()
                 for item in physical_array:
-                    yield item.handle
+                    if not (start and index != start):
+                        yield item.handle
                     windll.dxva2.DestroyPhysicalMonitor(item.handle)
+                    index += 1
 
     @classmethod
     def get_display_info(cls, display: Optional[Union[int, str]] = None) -> List[dict]:
         '''
         Returns a dictionary of info about all detected monitors or a selection of monitors
 
         Args:
@@ -407,26 +402,26 @@
             # EG output: [{'name': 'BenQ GL2450H', ... }, {'name': 'Dell U2211H', ... }]
 
             # get information about a monitor with this specific model
             bnq_info = sbc.windows.VCP.get_display_info('GL2450H')
             # EG output: {'name': 'BenQ GL2450H', 'model': 'GL2450H', ... }
             ```
         '''
-        try:
-            info = __cache__.get('vcp_monitor_info')
-        except Exception:
+        info = __cache__.get('vcp_monitor_info')
+        if info is None:
             info = [i for i in get_display_info() if i['method'] == cls]
             __cache__.store('vcp_monitor_info', info)
         if display is not None:
             info = filter_monitors(display=display, haystack=info)
         return info
 
     @staticmethod
     def get_monitor_caps(monitor: ctypes.wintypes.HANDLE) -> str:
         '''
+        **DEPRECATED**.
         Fetches and returns the VCP capabilities string of a monitor.
         This function takes anywhere from 1-2 seconds to run
 
         Args:
             monitor: a monitor handle as returned by `VCP.iter_physical_monitors()`
 
         Returns:
@@ -437,51 +432,51 @@
             import screen_brightness_control as sbc
 
             for monitor in sbc.windows.VCP.iter_physical_monitors():
                 print(sbc.windows.VCP.get_monitor_caps(monitor))
             # EG output: '(prot(monitor)type(LCD)model(GL2450HM)cmds(01 02 03 07 0C F3)vcp(02...)'
             ```
         '''
+        warn_deprecated('VCP.get_monitor_caps', False)
         caps_string_length = DWORD()
         if not windll.dxva2.GetCapabilitiesStringLength(monitor, ctypes.byref(caps_string_length)):
             return
         caps_string = (ctypes.c_char * caps_string_length.value)()
         if not windll.dxva2.CapabilitiesRequestAndCapabilitiesReply(monitor, caps_string, caps_string_length):
             return
         return caps_string.value.decode('ASCII')
 
     @classmethod
     def get_display_names(cls) -> List[str]:
         '''
+        **DEPRECATED**.
         Return the names of each detected monitor
 
         Returns:
             list: list of strings
 
         Example:
             ```python
             import screen_brightness_control as sbc
 
             names = sbc.windows.VCP.get_display_names()
             print(names)
             # EG output: ['BenQ GL2450H', 'Dell U2211H']
             ```
         '''
+        warn_deprecated('VCP.get_display_names', 'list_monitors(method="vcp")')
         return [i['name'] for i in cls.get_display_info()]
 
     @classmethod
-    def get_brightness(cls, display: Optional[Union[int, str]] = None) -> List[int]:
+    def get_brightness(cls, display: Optional[int] = None) -> List[int]:
         '''
         Retrieve the brightness of all connected displays using the `ctypes.windll` API
 
         Args:
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
+            display (int): The specific display you wish to query.
 
         Returns:
             list: list of ints (0 to 100)
 
         Examples:
             ```python
             import screen_brightness_control as sbc
@@ -491,116 +486,81 @@
             print('There are', len(current_brightness), 'detected displays')
 
             # Get the brightness for the primary display
             primary_brightness = sbc.windows.VCP.get_brightness(display = 0)[0]
 
             # Get the brightness for a secondary display
             secondary_brightness = sbc.windows.VCP.get_brightness(display = 1)[0]
-
-            # Get the brightness for a display with the model 'GL2450H'
-            benq_brightness = sbc.windows.VCP.get_brightness(display = 'GL2450H')[0]
             ```
         '''
-        # filter monitors even if display kwarg is not specified due to oddities surrounding issues #7 and #8
-        # https://github.com/Crozzers/screen_brightness_control/issues/7
-        # https://github.com/Crozzers/screen_brightness_control/issues/8
-        # essentially, we get 'ghost' monitors showing up here that cannot actually
-        # be adjusted (even if no error gets raised) so we use this to filter out
-        # such ghost monitors by only attempting to get the brightness for valid monitors
-        # (determined by VCP.get_display_info)
-        # yes, it does add an unnecessary function call but that's only if you're using this module low-level.
-        # Top-level functions always end up specifying the display kwarg anyway
-        if type(display) == int:
-            indexes = [display]
-        else:
-            indexes = [i['index'] for i in filter_monitors(display=display, haystack=cls.get_display_info())]
-
-        count = 0
+        code = BYTE(0x10)
         values = []
-        for m in cls.iter_physical_monitors():
-            try:
-                v = __cache__.get(f'vcp_brightness_{count}')
-            except Exception:
+        for index, monitor in enumerate(
+            cls.iter_physical_monitors(start=display),
+            start=display if display is not None else 0
+        ):
+            current = __cache__.get(f'vcp_brightness_{index}')
+            if current is None:
                 cur_out = DWORD()
+                handle = HANDLE(monitor)
                 for _ in range(10):
-                    if windll.dxva2.GetVCPFeatureAndVCPFeatureReply(HANDLE(m), BYTE(0x10), None, byref(cur_out), None):
-                        v = cur_out.value
+                    if windll.dxva2.GetVCPFeatureAndVCPFeatureReply(handle, code, None, byref(cur_out), None):
+                        current = cur_out.value
                         break
                     else:
+                        current = None
                         time.sleep(0.02)
-                        v = None
-                del(cur_out)
-            if v is not None:
-                if count in indexes:
-                    try:
-                        __cache__.store(f'vcp_brightness_{count}', v, expires=0.1)
-                    except IndexError:
-                        pass
-                    values.append(v)
-                    if count >= max(indexes):
-                        break
-            count += 1
+
+            if current is not None:
+                __cache__.store(f'vcp_brightness_{index}', current, expires=0.1)
+                values.append(current)
+
+            if display == index:
+                # if we have just got the display we wanted then exit here
+                # no point iterating through all the other ones
+                break
 
         return values
 
     @classmethod
-    def set_brightness(
-        cls, value: int,
-        display: Optional[Union[int, str]] = None,
-        no_return: bool = False
-    ) -> Union[List[int], None]:
+    def set_brightness(cls, value: int, display: Optional[int] = None):
         '''
         Sets the brightness for all connected displays using the `ctypes.windll` API
 
         Args:
-            display (int or str): The specific display you wish to query.
-                Can be index, name, model, serial or edid string.
-                `int` is faster as it isn't passed to `filter_monitors` to be matched against.
-                `str` is slower as it is passed to `filter_monitors` to match to a display.
-            no_return (bool): if set to `True` this function will return `None`
-
-        Returns:
-            list: list of ints (0 to 100) (the result of `VCP.get_brightness`) if `no_return` is False
-            None: if `no_return` is True
+            display (int): The specific display you wish to query.
 
         Examples:
             ```python
             import screen_brightness_control as sbc
 
             # Set the brightness for all detected displays to 50%
             sbc.windows.VCP.set_brightness(50)
 
             # Set the brightness for the primary display to 75%
             sbc.windows.VCP.set_brightness(75, display = 0)
 
             # Set the brightness for a secondary display to 25%
             sbc.windows.VCP.set_brightness(25, display = 1)
-
-            # Set the brightness for a display with the model 'GL2450H' to 100%
-            sbc.windows.VCP.set_brightness(100, display = 'GL2450H')
             ```
         '''
-        if type(display) == int:
-            indexes = [display]
-        else:
-            # see VCP.set_brightness for the explanation for why we always gather this list
-            indexes = [i['index'] for i in filter_monitors(display=display, haystack=cls.get_display_info())]
-
         __cache__.expire(startswith='vcp_brightness_')
-
-        count = 0
-        for m in cls.iter_physical_monitors():
-            if display is None or (count in indexes):
+        code = BYTE(0x10)
+        for index, monitor in enumerate(
+            cls.iter_physical_monitors(start=display),
+            start=display if display is not None else 0
+        ):
+            if display is None or display == index:
+                handle = HANDLE(monitor)
+                value = DWORD(value)
                 for _ in range(10):
-                    if windll.dxva2.SetVCPFeature(HANDLE(m), BYTE(0x10), DWORD(value)):
+                    if windll.dxva2.SetVCPFeature(handle, code, value):
                         break
                     else:
                         time.sleep(0.02)
-            count += 1
-        return cls.get_brightness(display=display) if not no_return else None
 
 
 def list_monitors_info(method: Optional[str] = None, allow_duplicates: bool = False) -> List[dict]:
     '''
     Lists detailed information about all detected monitors
 
     Args:
@@ -616,64 +576,57 @@
     Example:
         ```python
         import screen_brightness_control as sbc
 
         monitors = sbc.windows.list_monitors_info()
         for info in monitors:
             print('=======================')
-
             # the manufacturer name plus the model
             print('Name:', info['name'])
-
             # the general model of the display
             print('Model:', info['model'])
-
             # a unique string assigned by Windows to this display
             print('Serial:', info['serial'])
-
             # the name of the brand of the monitor
             print('Manufacturer:', info['manufacturer'])
-
             # the 3 letter code corresponding to the brand name, EG: BNQ -> BenQ
             print('Manufacturer ID:', info['manufacturer_id'])
-
             # the index of that display FOR THE SPECIFIC METHOD THE DISPLAY USES
             print('Index:', info['index'])
-
             # the method this monitor can be addressed by
             print('Method:', info['method'])
-
             # the EDID string of the monitor
             print('EDID:', info['edid'])
         ```
     '''
-    try:
-        return __cache__.get(f'windows_monitors_info_{method}_{allow_duplicates}')
-    except Exception:
+    info = __cache__.get(f'windows_monitors_info_{method}_{allow_duplicates}')
+    if info is None:
         info = get_display_info()
 
         if method is not None:
             method = method.lower()
             if method not in ('wmi', 'vcp'):
-                raise ValueError('method kwarg must be \'wmi\' or \'vcp\'')
+                raise ValueError('method kwarg must be "wmi" or "vcp"')
 
         info_final = []
         serials = []
         # to make sure each display (with unique edid) is only reported once
         for i in info:
             if allow_duplicates or i['serial'] not in serials:
                 if method is None or method == i['method'].__name__.lower():
                     serials.append(i['serial'])
                     info_final.append(i)
         __cache__.store(f'windows_monitors_info_{method}_{allow_duplicates}', info_final)
-        return info_final
+        info = info_final
+    return info
 
 
 def list_monitors(method: Optional[str] = None) -> List[str]:
     '''
+    **DEPRECATED**.
     Returns a list of all addressable monitor names
 
     Args:
         method (str): the method the monitor can be addressed by. Can be 'wmi' or 'vcp'
 
     Returns:
         list: list of strings
@@ -682,22 +635,25 @@
         ```python
         import screen_brightness_control as sbc
 
         monitors = sbc.windows.list_monitors()
         # EG output: ['BenQ GL2450H', 'Dell U2211H']
         ```
     '''
+    warn_deprecated('list_monitors')
     return [i['name'] for i in list_monitors_info(method=method)]
 
 
 def __set_and_get_brightness(*args, display=None, method=None, meta_method='get', **kwargs) -> Union[List[int], None]:
     '''
+    **DEPRECATED**.
     Internal function, do not call. Either sets the brightness or gets it.
     Exists because set_brightness and get_brightness only have a couple differences
     '''
+    warn_deprecated('__set_and_get_brightness', '__brightness')
     errors = []
     try:  # filter known list of monitors according to kwargs
         if type(display) == int:
             monitors = [list_monitors_info(method=method)[display]]
         else:
             monitors = filter_monitors(display=display, method=method)
     except Exception as e:
@@ -736,14 +692,15 @@
 def set_brightness(
     value: int,
     display: Optional[Union[int, str]] = None,
     method: Optional[str] = None,
     **kwargs
 ) -> Union[List[int], None]:
     '''
+    **DEPRECATED**.
     Sets the brightness of any connected monitors
 
     Args:
         value (int): Sets the brightness to this value as a percentage
         display (int or str): The specific display you wish to adjust.
             Can be index, model, name or serial of the display
         method (str): the method to use ('wmi' or 'vcp')
@@ -772,21 +729,23 @@
         # set the brightness of any displays using VCP to 25%
         sbc.windows.set_brightness(25, method = 'vcp')
 
         # set the brightness of displays with model name 'BenQ GL2450H' to 100%
         sbc.windows.set_brightness(100, display = 'BenQ GL2450H')
         ```
     '''
+    warn_deprecated('set_brightness')
     # this function is called because set_brightness and get_brightness only differed by 1 line of code
     # so I made another internal function to reduce the filesize
     return __set_and_get_brightness(value, display=display, method=method, meta_method='set', **kwargs)
 
 
 def get_brightness(display: Optional[Union[int, str]] = None, method: Optional[str] = None, **kwargs) -> List[int]:
     '''
+    **DEPRECATED**.
     Returns the brightness of any connected monitors
 
     Args:
         display (int or str): The specific display you wish to adjust.
             Can be index, model, name or serial of the display
         method (str): the method to use ('wmi' or 'vcp')
         kwargs (dict): passed directly to chosen brightness method
@@ -817,10 +776,11 @@
         # get the brightness of any displays using VCP
         vcp_brightness = sbc.windows.get_brightness(method='vcp')
 
         # get the brightness of displays with the model name 'BenQ GL2450H'
         benq_brightness = sbc.windows.get_brightness(display='BenQ GL2450H')[0]
         ```
     '''
+    warn_deprecated('get_brightness')
     # this function is called because set_brightness and get_brightness only differed by 1 line of code
     # so I made another internal function to reduce the filesize
     return __set_and_get_brightness(display=display, method=method, meta_method='get', **kwargs)
```

### Comparing `screen_brightness_control-0.8.6/screen_brightness_control.egg-info/PKG-INFO` & `screen_brightness_control-0.9.0/screen_brightness_control.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen-brightness-control
-Version: 0.8.6
+Version: 0.9.0
 Summary: A Python tool to control monitor brightness on Windows and Linux
 Home-page: https://github.com/Crozzers/screen_brightness_control
 Author: Crozzers
 Author-email: captaincrozzers@gmail.com
 License: MIT
 Project-URL: Documentation, https://crozzers.github.io/screen_brightness_control
 Project-URL: Issue Tracker, https://github.com/Crozzers/screen_brightness_control/issues
@@ -73,48 +73,53 @@
         ```
         
         # Quick Start
         
         You can read [the full documentation](https://crozzers.github.io/screen_brightness_control) for this project for more details but here are the basics.
         
         
-        ### get_brightness(`verbose_error=False, **kwargs`)
+        ### get_brightness(`display=None, method=None, verbose_error=False`)
         **Summary:**  
         Returns the current screen brightness as a percentage. It may return a list of values if you have multiple, brightness adjustable monitors.  
         Raises `ScreenBrightnessError` upon failure
         
         **Arguments:**
         
+        * `display` - the specific display you wish to adjust. This can be an integer or a string (EDID, serial, name or model)
+        * `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
         * `verbose_error` - a boolean value to control how much detail any error messages should contain
-        * `kwargs` - passed to the OS relevant brightness method
         
         **Usage:**  
         ```python
         import screen_brightness_control as sbc
         
-        #get the current screen brightness (for all detected displays)
+        # get the current screen brightness (for all detected displays)
         all_screens_brightness = sbc.get_brightness()
-        #get the brightness of the primary display
+        # get the brightness of the primary display
         primary_display_brightness = sbc.get_brightness(display=0)
-        #get the brightness of the secondary display (if connected)
+        # get the brightness of the secondary display (if connected)
         secondary_display_brightness = sbc.get_brightness(display=1)
+        # get the brightness for a named monitor
+        benq_brightness = sbc.get_brightness(display='BenQ GL2450H')
         ```  
         
         
-        ### set_brightness(`value, force=False, verbose_error=False, **kwargs`)
+        ### set_brightness(`value, display=None, method=None, force=False, verbose_error=False, no_return=False`)
         **Summary:**  
         Sets the brightness to `value`. If `value` is a string and contains "+" or "-" then that value is added to/subtracted from the current brightness.
         Raises `ScreenBrightnessError` upon failure
         
         **Arguments:**
         
         * `value` - the level to set the brightness to. Can either be an integer or a string.
+        * `display` - the specific display you wish to adjust. This can be an integer or a string (EDID, serial, name or model)
+        * `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
         * `force` (Linux only) - if set to `False` then the brightness is never set to less than 1 because on Linux this often turns the screen off. If set to `True` then it will bypass this check
         * `verbose_error` - a boolean value to control how much detail any error messages should contain
-        * `kwargs` - passed to the OS relevant brightness method
+        * `no_return` - boolean value, whether this function should return `None` or not. By default, the return value is the new brightness value but this behaviour is deprecated. In the future this function will return `None` by default.
         
         **Usage:**  
         ```python
         import screen_brightness_control as sbc
         
         #set brightness to 50%
         sbc.set_brightness(50)
@@ -164,14 +169,30 @@
         sbc.fade_brightness(90, start=100, interval=0.1)
         
         #fade the brightness to 100% in a new thread
         sbc.fade_brightness(100, blocking=False)
         ```
         
         
+        ### list_monitors(`method=None`)
+        **Summary:**  
+        Returns a list of the names of all detected monitors
+        
+        **Arguments:**
+        
+        * `method` - the OS specific method to use. On Windows this can be `'wmi'` or `'vcp'` and on Linux this can be `'light'`, `'xrandr'`, `'ddcutil'` or `'xbacklight'`
+        
+        **Usage:**  
+        ```python
+        import screen_brightness_control as sbc
+        monitor_names = sbc.list_monitors()
+        # eg: ['BenQ GL2450H', 'Dell U2211H']
+        ```
+        
+        
         ## A Toast
         To GitHub users [lcharles](https://github.com/lcharles), [Ved Rathi](https://github.com/Ved-programmer), [Daniel Wong](https://github.com/drojf), [Melek REBAI](https://github.com/shadoWalker89) and [Mathias Johansson](https://github.com/Mathias9807) for contributing to this project
         
         ## License
         This software is licensed under the [MIT license](https://mit-license.org/)
         
         # FAQ
@@ -215,15 +236,15 @@
         
         ### When I call `get_brightness()` the returned value isn't what I set it to (Windows)
         Not all monitors can set the brightness for every value between 0 and 100. Some of them have a number of 'levels' that they can be set to.
         You can likely see this if you open your display settings and very slowly move the brightness slider.  
         You can find out your brightness 'levels' by running the following python code:
         ```python
         import wmi
-        monitor = wmi.WMI(namespace='wmi').MonitorBrightness[0]
+        monitor = wmi.WMI(namespace='wmi').WmiMonitorBrightness()[0]
         #the number of levels the monitor can be set to
         print(monitor.Levels)
         #the actual brightness values your monitor can be set to
         print(monitor.Level)
         ```
         
         # Things to note:
```

### Comparing `screen_brightness_control-0.8.6/setup.py` & `screen_brightness_control-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='screen_brightness_control',
-    version='0.8.6',
+    version='0.9.0',
     url='https://github.com/Crozzers/screen_brightness_control',
     project_urls={
         'Documentation': 'https://crozzers.github.io/screen_brightness_control',
         'Issue Tracker': 'https://github.com/Crozzers/screen_brightness_control/issues'
     },
     license='MIT',
     author='Crozzers',
```


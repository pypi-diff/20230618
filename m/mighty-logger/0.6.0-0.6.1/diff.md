# Comparing `tmp/mighty_logger-0.6.0.tar.gz` & `tmp/mighty_logger-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.6.0.tar", last modified: Wed Jun 14 15:04:27 2023, max compression
+gzip compressed data, was "mighty_logger-0.6.1.tar", last modified: Sun Jun 18 13:45:38 2023, max compression
```

## Comparing `mighty_logger-0.6.0.tar` & `mighty_logger-0.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.340353 mighty_logger-0.6.0/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.6.0/LICENSE
--rw-rw-rw-   0        0        0    10318 2023-06-14 15:04:27.340353 mighty_logger-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     9350 2023-06-12 16:10:21.000000 mighty_logger-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.249337 mighty_logger-0.6.0/mighty_logger/
--rw-rw-rw-   0        0        0      823 2023-06-12 12:55:27.000000 mighty_logger-0.6.0/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.300349 mighty_logger-0.6.0/mighty_logger/basic/
--rw-rw-rw-   0        0        0      857 2023-04-11 08:43:49.000000 mighty_logger-0.6.0/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     5371 2023-06-12 12:55:27.000000 mighty_logger-0.6.0/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1325 2023-04-12 11:19:28.000000 mighty_logger-0.6.0/mighty_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.6.0/mighty_logger/basic/patterns.py
--rw-rw-rw-   0        0        0     4009 2023-06-12 12:55:27.000000 mighty_logger-0.6.0/mighty_logger/basic/text_buffer_type.py
--rw-rw-rw-   0        0        0    70934 2023-06-12 14:16:59.000000 mighty_logger-0.6.0/mighty_logger/powerful_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.314351 mighty_logger-0.6.0/mighty_logger/src/
--rw-rw-rw-   0        0        0      943 2023-06-11 13:34:59.000000 mighty_logger-0.6.0/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     4572 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     8659 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/src/color_picker.py
--rw-rw-rw-   0        0        0     1293 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/src/log_enums.py
--rw-rw-rw-   0        0        0     5647 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/src/status_variables.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.335354 mighty_logger-0.6.0/mighty_logger/text/
--rw-rw-rw-   0        0        0      853 2023-06-10 14:12:03.000000 mighty_logger-0.6.0/mighty_logger/text/__init__.py
--rw-rw-rw-   0        0        0     5947 2023-06-11 16:58:31.000000 mighty_logger-0.6.0/mighty_logger/text/animation.py
--rw-rw-rw-   0        0        0     2872 2023-06-12 13:38:48.000000 mighty_logger-0.6.0/mighty_logger/text/icon_set.py
--rw-rw-rw-   0        0        0     5806 2023-06-12 16:08:04.000000 mighty_logger-0.6.0/mighty_logger/text/text_buffer.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.255339 mighty_logger-0.6.0/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0    10318 2023-06-14 15:04:27.000000 mighty_logger-0.6.0/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-06-14 15:04:27.000000 mighty_logger-0.6.0/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 15:04:27.000000 mighty_logger-0.6.0/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-14 15:04:27.000000 mighty_logger-0.6.0/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 15:04:27.342354 mighty_logger-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     2796 2023-06-14 14:55:46.000000 mighty_logger-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:04:27.338353 mighty_logger-0.6.0/test/
--rw-rw-rw-   0        0        0     2067 2023-06-14 12:00:28.000000 mighty_logger-0.6.0/test/test_console.py
--rw-rw-rw-   0        0        0     2099 2023-06-14 12:02:42.000000 mighty_logger-0.6.0/test/test_html.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.626365 mighty_logger-0.6.1/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0    10797 2023-06-18 13:45:38.645888 mighty_logger-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9824 2023-06-18 13:24:38.000000 mighty_logger-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.537706 mighty_logger-0.6.1/mighty_logger/
+-rw-rw-rw-   0        0        0      823 2023-06-18 13:45:30.000000 mighty_logger-0.6.1/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.582361 mighty_logger-0.6.1/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      857 2023-04-11 08:43:49.000000 mighty_logger-0.6.1/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     5371 2023-06-12 12:55:27.000000 mighty_logger-0.6.1/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1325 2023-04-12 11:19:28.000000 mighty_logger-0.6.1/mighty_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.6.1/mighty_logger/basic/patterns.py
+-rw-rw-rw-   0        0        0     4009 2023-06-12 12:55:27.000000 mighty_logger-0.6.1/mighty_logger/basic/text_buffer_type.py
+-rw-rw-rw-   0        0        0    80755 2023-06-18 13:42:58.000000 mighty_logger-0.6.1/mighty_logger/powerful_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.604562 mighty_logger-0.6.1/mighty_logger/src/
+-rw-rw-rw-   0        0        0      943 2023-06-11 13:34:59.000000 mighty_logger-0.6.1/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     4572 2023-06-11 16:58:31.000000 mighty_logger-0.6.1/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     8659 2023-06-11 16:58:31.000000 mighty_logger-0.6.1/mighty_logger/src/color_picker.py
+-rw-rw-rw-   0        0        0     1376 2023-06-18 11:06:25.000000 mighty_logger-0.6.1/mighty_logger/src/log_enums.py
+-rw-rw-rw-   0        0        0     5647 2023-06-11 16:58:31.000000 mighty_logger-0.6.1/mighty_logger/src/status_variables.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.615562 mighty_logger-0.6.1/mighty_logger/text/
+-rw-rw-rw-   0        0        0      853 2023-06-10 14:12:03.000000 mighty_logger-0.6.1/mighty_logger/text/__init__.py
+-rw-rw-rw-   0        0        0    10316 2023-06-18 13:17:24.000000 mighty_logger-0.6.1/mighty_logger/text/animation.py
+-rw-rw-rw-   0        0        0     3180 2023-06-18 10:25:46.000000 mighty_logger-0.6.1/mighty_logger/text/icon_set.py
+-rw-rw-rw-   0        0        0     6042 2023-06-17 14:04:56.000000 mighty_logger-0.6.1/mighty_logger/text/text_buffer.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.542708 mighty_logger-0.6.1/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0    10797 2023-06-18 13:45:38.000000 mighty_logger-0.6.1/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-06-18 13:45:38.000000 mighty_logger-0.6.1/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:45:38.000000 mighty_logger-0.6.1/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-18 13:45:38.000000 mighty_logger-0.6.1/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:45:38.646888 mighty_logger-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2796 2023-06-18 13:45:30.000000 mighty_logger-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.625364 mighty_logger-0.6.1/test/
+-rw-rw-rw-   0        0        0     2483 2023-06-18 13:19:47.000000 mighty_logger-0.6.1/test/test_console.py
+-rw-rw-rw-   0        0        0     2508 2023-06-18 11:18:04.000000 mighty_logger-0.6.1/test/test_html.py
```

### Comparing `mighty_logger-0.6.0/LICENSE` & `mighty_logger-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/PKG-INFO` & `mighty_logger-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mighty_logger
-Version: 0.6.0
+Version: 0.6.1
 Summary: Powerful functional logger with support for qt programming
 Home-page: https://github.com/Nakama3942/mighty_logger
 Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
@@ -91,27 +91,32 @@
 
 - [Content](#content)
 
 ## Important releases
 
 <details><summary>See the important releases (possible spoilers)</summary>
 
+- [x] v0.0.1 - Alpha-release (the very first version of the simplest Logger has been published)
+- [x] v0.0.2 - Little update (added multiple entry types and colors)
+- [x] v0.0.3 - Types update (added even more multiple entry types and colors)
+- [x] v0.0.4 - Color update (added the entire X11 color table and reworked the color system)
 - [x] v0.1.0 - First official release (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
-- [ ] v0.6.1 - Animation update (added animations in processes)
+- [x] v0.6.1 - Animation update (added animations in processes)
 - [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
 - [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
 - [ ] v0.7.2 - Search update (added search by log entry types)
-- [ ] v0.7.3 - Extension update (made wheel format and instruction of toml)
-- [ ] v0.8.0 - ? (???) in short, add export to csv
+- [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
+- [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
+- [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
@@ -149,16 +154,16 @@
 This is the simplest example of using the library:
 
 ```python
 from mighty_logger import Logger
 from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
-    logger = Logger(program_name="Test", console_width=115)
-    logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
+	logger = Logger(program_name="Test", console_width=115)
+	logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
 ```
 
 The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
 
 <pre>
 <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span>
 <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry>         </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span>
@@ -185,18 +190,18 @@
 All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/mighty_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/mighty_logger/blob/master/CODE_OF_CONDUCT.md).
 
 - [Content](#content)
 
 ## Authors
 
 <table align="center" style="border-width: 10; border-style: ridge">
-    <tr>
-        <td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
-        <!--<td></td>-->
-    </tr>
+	<tr>
+		<td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
+		<!--<td></td>-->
+	</tr>
 <!--
-    <tr>
-        <td></td>
-        <td></td>
-    </tr>
+	<tr>
+		<td></td>
+		<td></td>
+	</tr>
 -->
 </table>
```

### Comparing `mighty_logger-0.6.0/README.md` & `mighty_logger-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,27 +72,32 @@
 
 - [Content](#content)
 
 ## Important releases
 
 <details><summary>See the important releases (possible spoilers)</summary>
 
+- [x] v0.0.1 - Alpha-release (the very first version of the simplest Logger has been published)
+- [x] v0.0.2 - Little update (added multiple entry types and colors)
+- [x] v0.0.3 - Types update (added even more multiple entry types and colors)
+- [x] v0.0.4 - Color update (added the entire X11 color table and reworked the color system)
 - [x] v0.1.0 - First official release (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
-- [ ] v0.6.1 - Animation update (added animations in processes)
+- [x] v0.6.1 - Animation update (added animations in processes)
 - [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
 - [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
 - [ ] v0.7.2 - Search update (added search by log entry types)
-- [ ] v0.7.3 - Extension update (made wheel format and instruction of toml)
-- [ ] v0.8.0 - ? (???) in short, add export to csv
+- [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
+- [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
+- [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
@@ -130,16 +135,16 @@
 This is the simplest example of using the library:
 
 ```python
 from mighty_logger import Logger
 from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
-    logger = Logger(program_name="Test", console_width=115)
-    logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
+	logger = Logger(program_name="Test", console_width=115)
+	logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
 ```
 
 The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
 
 <pre>
 <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span>
 <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry>         </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span>
@@ -166,18 +171,18 @@
 All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/mighty_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/mighty_logger/blob/master/CODE_OF_CONDUCT.md).
 
 - [Content](#content)
 
 ## Authors
 
 <table align="center" style="border-width: 10; border-style: ridge">
-    <tr>
-        <td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
-        <!--<td></td>-->
-    </tr>
+	<tr>
+		<td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
+		<!--<td></td>-->
+	</tr>
 <!--
-    <tr>
-        <td></td>
-        <td></td>
-    </tr>
+	<tr>
+		<td></td>
+		<td></td>
+	</tr>
 -->
 </table>
```

### Comparing `mighty_logger-0.6.0/mighty_logger/__init__.py` & `mighty_logger-0.6.1/mighty_logger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .powerful_logger import Logger
 
 __authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.6.0/mighty_logger/basic/__init__.py` & `mighty_logger-0.6.1/mighty_logger/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/basic/basic_logger.py` & `mighty_logger-0.6.1/mighty_logger/basic/basic_logger.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/basic/exceptions.py` & `mighty_logger-0.6.1/mighty_logger/basic/exceptions.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/basic/patterns.py` & `mighty_logger-0.6.1/mighty_logger/basic/patterns.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/basic/text_buffer_type.py` & `mighty_logger-0.6.1/mighty_logger/basic/text_buffer_type.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/powerful_logger.py` & `mighty_logger-0.6.1/mighty_logger/powerful_logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -75,16 +75,17 @@
 			self._settings["status_message_global_entry"] = status_message_global_entry
 			self._settings["status_type_global_entry"] = status_type_global_entry
 			self._settings["message_global_entry"] = message_global_entry
 			self._ColorScheme: dict = {}
 			self._environment = log_environment
 			self._progress_rise = 0
 			self._progress_start: datetime | None = None
-			self._progress_time: str = "       "
+			self._progress_time: str = "        "
 			self._progress_interrupt = False
+			self._start_timer_value: datetime | None = None
 			self.global_background = global_background
 			self._color_scheme_init()
 			if self._environment == LogEnvironments.CONSOLE:
 				if TextBuffer._instance is not None:
 					self._buffer = TextBuffer._instance
 					self.notice(
 						message_text="An existing logger was taken into use",
@@ -258,14 +259,35 @@
 				# FAIL colors
 				self._ColorScheme['FAIL_TIME'] = [AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")]
 				self._ColorScheme['FAIL_STATUS'] = [AnsiColor('ORANGE', "foreground"), AnsiColor('ORANGE', "foreground")]
 				self._ColorScheme['FAIL_STATUS_MESSAGE'] = [AnsiColor('DARKORANGE', "foreground"), AnsiColor('DARKORANGE', "foreground")]
 				self._ColorScheme['TYPE_FAIL'] = [AnsiColor('FIREBRICK', "foreground"), AnsiColor('YELLOW', "foreground")]
 				self._ColorScheme['FAIL_MESSAGE'] = [AnsiColor('DARKRED', "foreground"), AnsiColor('DARKYELLOW', "foreground")]
 				self._ColorScheme['FAIL_BACKGROUND'] = ["", AnsiColor('DARKRED', "background")]
+				# START_TIMER colors
+				self._ColorScheme['START_TIMER_TIME'] = [AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")]
+				self._ColorScheme['START_TIMER_STATUS'] = [AnsiColor('ORANGE', "foreground"), AnsiColor('CHARTREUSE', "foreground")]
+				self._ColorScheme['START_TIMER_STATUS_MESSAGE'] = [AnsiColor('DARKORANGE', "foreground"), AnsiColor('LAWNGREEN', "foreground")]
+				self._ColorScheme['TYPE_START_TIMER'] = [AnsiColor('SEAGREEN', "foreground"), AnsiColor('PALEGREEN', "foreground")]
+				self._ColorScheme['START_TIMER_MESSAGE'] = [AnsiColor('FORESTGREEN', "foreground"), AnsiColor('LIGHTGREEN', "foreground")]
+				self._ColorScheme['START_TIMER_BACKGROUND'] = ["", AnsiColor('FORESTGREEN', "background")]
+				# TIMER_MARK colors
+				self._ColorScheme['TIMER_MARK_TIME'] = [AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")]
+				self._ColorScheme['TIMER_MARK_STATUS'] = [AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")]
+				self._ColorScheme['TIMER_MARK_STATUS_MESSAGE'] = [AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")]
+				self._ColorScheme['TYPE_TIMER_MARK'] = [AnsiColor('KHAKI', "foreground"), AnsiColor('SIENNA', "foreground")]
+				self._ColorScheme['TIMER_MARK_MESSAGE'] = [AnsiColor('DARKKHAKI', "foreground"), AnsiColor('SADDLEBROWN', "foreground")]
+				self._ColorScheme['TIMER_MARK_BACKGROUND'] = ["", AnsiColor('DARKKHAKI', "background")]
+				# STOP_TIMER colors
+				self._ColorScheme['STOP_TIMER_TIME'] = [AnsiColor('ORCHID', "foreground"), AnsiColor('PURPLE', "foreground")]
+				self._ColorScheme['STOP_TIMER_STATUS'] = [AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")]
+				self._ColorScheme['STOP_TIMER_STATUS_MESSAGE'] = [AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")]
+				self._ColorScheme['TYPE_STOP_TIMER'] = [AnsiColor('LIGHTSKYBLUE', "foreground"), AnsiColor('NAVY', "foreground")]
+				self._ColorScheme['STOP_TIMER_MESSAGE'] = [AnsiColor('SKYBLUE', "foreground"), AnsiColor('MIDNIGHTBLUE', "foreground")]
+				self._ColorScheme['STOP_TIMER_BACKGROUND'] = ["", AnsiColor('SKYBLUE', "background")]
 			case LogEnvironments.HTML:
 				self._ColorScheme['INITIAL_COLOR'] = [HexColor('GOLD'), HexColor('INDIGO')]
 				self._ColorScheme['INITIAL_BACKGROUND'] = ["", HexColor('GOLD')]
 				# DEBUG colors
 				self._ColorScheme['DEBUG_TIME'] = [HexColor('ORCHID'), HexColor('DARKMAGENTA')]
 				self._ColorScheme['DEBUG_STATUS'] = [HexColor('ORANGE'), HexColor('DARKRED')]
 				self._ColorScheme['DEBUG_STATUS_MESSAGE'] = [HexColor('DARKORANGE'), HexColor('MAROON')]
@@ -408,14 +430,35 @@
 				# FAIL colors
 				self._ColorScheme['FAIL_TIME'] = [HexColor('ORCHID'), HexColor('LAVENDERBLUSH')]
 				self._ColorScheme['FAIL_STATUS'] = [HexColor('ORANGE'), HexColor('ORANGE')]
 				self._ColorScheme['FAIL_STATUS_MESSAGE'] = [HexColor('DARKORANGE'), HexColor('DARKORANGE')]
 				self._ColorScheme['TYPE_FAIL'] = [HexColor('FIREBRICK'), HexColor('YELLOW')]
 				self._ColorScheme['FAIL_MESSAGE'] = [HexColor('DARKRED'), HexColor('DARKYELLOW')]
 				self._ColorScheme['FAIL_BACKGROUND'] = ["", HexColor('DARKRED')]
+				# START_TIMER colors
+				self._ColorScheme['START_TIMER_TIME'] = [HexColor('ORCHID'), HexColor('LAVENDERBLUSH')]
+				self._ColorScheme['START_TIMER_STATUS'] = [HexColor('ORANGE'), HexColor('CHARTREUSE')]
+				self._ColorScheme['START_TIMER_STATUS_MESSAGE'] = [HexColor('DARKORANGE'), HexColor('LAWNGREEN')]
+				self._ColorScheme['TYPE_START_TIMER'] = [HexColor('SEAGREEN'), HexColor('PALEGREEN')]
+				self._ColorScheme['START_TIMER_MESSAGE'] = [HexColor('FORESTGREEN'), HexColor('LIGHTGREEN')]
+				self._ColorScheme['START_TIMER_BACKGROUND'] = ["", HexColor('FORESTGREEN')]
+				# TIMER_MARK colors
+				self._ColorScheme['TIMER_MARK_TIME'] = [HexColor('ORCHID'), HexColor('DARKMAGENTA')]
+				self._ColorScheme['TIMER_MARK_STATUS'] = [HexColor('ORANGE'), HexColor('DARKRED')]
+				self._ColorScheme['TIMER_MARK_STATUS_MESSAGE'] = [HexColor('DARKORANGE'), HexColor('MAROON')]
+				self._ColorScheme['TYPE_TIMER_MARK'] = [HexColor('KHAKI'), HexColor('SIENNA')]
+				self._ColorScheme['TIMER_MARK_MESSAGE'] = [HexColor('DARKKHAKI'), HexColor('SADDLEBROWN')]
+				self._ColorScheme['TIMER_MARK_BACKGROUND'] = ["", HexColor('DARKKHAKI')]
+				# STOP_TIMER colors
+				self._ColorScheme['STOP_TIMER_TIME'] = [HexColor('ORCHID'), HexColor('PURPLE')]
+				self._ColorScheme['STOP_TIMER_STATUS'] = [HexColor('ORANGE'), HexColor('DARKRED')]
+				self._ColorScheme['STOP_TIMER_STATUS_MESSAGE'] = [HexColor('DARKORANGE'), HexColor('MAROON')]
+				self._ColorScheme['TYPE_STOP_TIMER'] = [HexColor('LIGHTSKYBLUE'), HexColor('NAVY')]
+				self._ColorScheme['STOP_TIMER_MESSAGE'] = [HexColor('SKYBLUE'), HexColor('MIDNIGHTBLUE')]
+				self._ColorScheme['STOP_TIMER_BACKGROUND'] = ["", HexColor('SKYBLUE')]
 
 	def _initial_log(self) -> None:
 		"""
 		Displays initialized information.
 		"""
 		if self._environment == LogEnvironments.HTML:
 			self._buffer << "<body style='background-color: #000000; color: #ffffff;'>"
@@ -480,14 +523,20 @@
 
 		:return: a text buffer object
 		"""
 		return self._buffer
 
 	#todo v0.7.1 сделать конвертер из Console в HTML и наоборот
 
+	# ######################################################################################## #
+	#                                                                                          #
+	#                                    Entering to Logger                                    #
+	#                                                                                          #
+	# ######################################################################################## #
+
 	def empty(
 		self,
 		*,
 		entry: str
 	) -> None:
 		"""
 		Empty logging:
@@ -1000,14 +1049,20 @@
 				self._ColorScheme['UNRESOLVED_MESSAGE'][background],
 				self._ColorScheme['UNRESOLVED_BACKGROUND'][background],
 			], self._progress_time, self._icon_set.unresolved, status_message.current_status_message, "!UNRESOLVED", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
+	# ######################################################################################## #
+	#                                                                                          #
+	#                                  Entering to Processes                                   #
+	#                                                                                          #
+	# ######################################################################################## #
+
 	def start_indefinite_process(
 		self,
 		*,
 		animation: IndefiniteAnimationType = IndefiniteAnimations.Line,
 		status_message: StatusMessageType = StatusMessageType("..."),
 		message_text: str = "...",
 		local_background: bool = None,
@@ -1028,15 +1083,15 @@
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		self._animation = animation
 
 		self._progress_start = datetime.now()
 		progress_stop = datetime.now()
-		self._progress_time = str(progress_stop - self._progress_start).split(".")[0]
+		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		func = getattr(self, "_initiation", None)
 		args = {}
 		if status_message != StatusMessageType("..."):
 			args['status_message'] = status_message
 		if message_text != "...":
 			args['message_text'] = message_text
 		if local_background is not None:
@@ -1117,15 +1172,15 @@
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		self._animation = progress_bar
 
 		self._progress_start = datetime.now()
 		progress_stop = datetime.now()
-		self._progress_time = str(progress_stop - self._progress_start).split(".")[0]
+		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		func = getattr(self, "_initiation", None)
 		args = {}
 		if status_message != StatusMessageType("..."):
 			args['status_message'] = status_message
 		if message_text != "...":
 			args['message_text'] = message_text
 		if local_background is not None:
@@ -1221,18 +1276,19 @@
 
 		:param entry_type: The type of entry to be entered in the progress history
 		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
+		sleep(0.001)
 		last = self._buffer.pop()
 
 		progress_stop = datetime.now()
-		self._progress_time = str(progress_stop - self._progress_start).split(".")[0]
+		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		func = getattr(self, entry_type, None)
 		args = {}
 		if status_message != StatusMessageType("..."):
 			args['status_message'] = status_message
 		if message_text != "...":
 			args['message_text'] = message_text
 		if local_background is not None:
@@ -1261,33 +1317,34 @@
 
 		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local entering settings
 		"""
 		self._progress_interrupt = True
+		sleep(0.11)
 		self._buffer.remove()
 
 		progress_stop = datetime.now()
-		self._progress_time = str(progress_stop - self._progress_start).split(".")[0]
+		self._progress_time = "&" + str(progress_stop - self._progress_start).split(".")[0]
 		func = getattr(self, "_success", None) if self._progress_rise == 100 else getattr(self, "_fail", None)
 		args = {}
 		if status_message != StatusMessageType("..."):
 			args['status_message'] = status_message
 		if message_text != "...":
 			args['message_text'] = message_text
 		if local_background is not None:
 			args['local_background'] = local_background
 		if local_settings is not None:
 			args['local_settings'] = local_settings
 		func(**args)
 
 		self._progress_rise = 0
 		self._progress_start = None
-		self._progress_time = "       "
+		self._progress_time = "        "
 		self._progress_interrupt = False
 
 	def _initiation(
 		self,
 		*,
 		status_message: StatusMessageType = StatusMessageType("..."),
 		message_text: str = "...",
@@ -1413,15 +1470,14 @@
 				self._ColorScheme['SUCCESS_STATUS'][local_background],
 				self._ColorScheme['SUCCESS_STATUS_MESSAGE'][local_background],
 				self._ColorScheme['TYPE_SUCCESS'][local_background],
 				self._ColorScheme['SUCCESS_MESSAGE'][local_background],
 				self._ColorScheme['SUCCESS_BACKGROUND'][local_background],
 			], self._progress_time, self._icon_set.success, status_message.current_status_message, "&SUCCESS", message_text, self._environment, local_settings
 		)
-		sleep(0.11)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
 	def _fail(
 		self,
 		*,
 		status_message: StatusMessageType = StatusMessageType("..."),
@@ -1448,10 +1504,135 @@
 				self._ColorScheme['FAIL_STATUS'][local_background],
 				self._ColorScheme['FAIL_STATUS_MESSAGE'][local_background],
 				self._ColorScheme['TYPE_FAIL'][local_background],
 				self._ColorScheme['FAIL_MESSAGE'][local_background],
 				self._ColorScheme['FAIL_BACKGROUND'][local_background],
 			], self._progress_time, self._icon_set.fail, status_message.current_status_message, "&FAIL", message_text, self._environment, local_settings
 		)
-		sleep(0.11)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
+
+	# ######################################################################################## #
+	#                                                                                          #
+	#                                     Entering to Timer                                    #
+	#                                                                                          #
+	# ######################################################################################## #
+
+	def start_timer(
+		self,
+		*,
+		status_message: StatusMessageType = StatusMessageType("..."),
+		message_text: str = "...",
+		local_background: bool = True,
+		local_settings: dict = None
+	) -> None:
+		"""
+		Information logging of starting Timer:
+		Used to notify the start of the Timer.
+
+		:param status_message: Log entry status message
+		:param message_text: Log entry message
+		:param local_background: Display entry with background?
+		:param local_settings: Dictionary of local entering settings
+		"""
+		self._start_timer_value = datetime.now()
+		stop_timer_value = datetime.now()
+		self._progress_time = "^" + str(stop_timer_value - self._start_timer_value).split(".")[0]
+
+		if local_settings is None:
+			local_settings = {}
+		if not 'italic' in local_settings:
+			local_settings["italic"] = True
+		self._buffer << self._assemble_entry(
+			[
+				self._ColorScheme['START_TIMER_TIME'][local_background],
+				self._ColorScheme['START_TIMER_STATUS'][local_background],
+				self._ColorScheme['START_TIMER_STATUS_MESSAGE'][local_background],
+				self._ColorScheme['TYPE_START_TIMER'][local_background],
+				self._ColorScheme['START_TIMER_MESSAGE'][local_background],
+				self._ColorScheme['START_TIMER_BACKGROUND'][local_background],
+			], self._progress_time, self._icon_set.start_timer, status_message.current_status_message, "^START TIMER", message_text, self._environment, local_settings
+		)
+		if self._environment == LogEnvironments.CONSOLE:
+			self._buffer.update_console()
+
+		self._progress_time = "        "
+
+	def timer_mark(
+		self,
+		*,
+		status_message: StatusMessageType = StatusMessageType("..."),
+		message_text: str = "...",
+		local_background: bool = True,
+		local_settings: dict = None
+	) -> None:
+		"""
+		Information logging of mark Timer:
+		Used to notify the mark of the Timer.
+
+		:param status_message: Log entry status message
+		:param message_text: Log entry message
+		:param local_background: Display entry with background?
+		:param local_settings: Dictionary of local entering settings
+		"""
+		stop_timer_value = datetime.now()
+		self._progress_time = "^" + str(stop_timer_value - self._start_timer_value).split(".")[0]
+
+		if local_settings is None:
+			local_settings = {}
+		if not 'italic' in local_settings:
+			local_settings["italic"] = True
+		self._buffer << self._assemble_entry(
+			[
+				self._ColorScheme['TIMER_MARK_TIME'][local_background],
+				self._ColorScheme['TIMER_MARK_STATUS'][local_background],
+				self._ColorScheme['TIMER_MARK_STATUS_MESSAGE'][local_background],
+				self._ColorScheme['TYPE_TIMER_MARK'][local_background],
+				self._ColorScheme['TIMER_MARK_MESSAGE'][local_background],
+				self._ColorScheme['TIMER_MARK_BACKGROUND'][local_background],
+			], self._progress_time, self._icon_set.timer_mark, status_message.current_status_message, "^TIMER MARK", message_text, self._environment, local_settings
+		)
+		if self._environment == LogEnvironments.CONSOLE:
+			self._buffer.update_console()
+
+		self._progress_time = "        "
+
+	def stop_timer(
+		self,
+		*,
+		status_message: StatusMessageType = StatusMessageType("..."),
+		message_text: str = "...",
+		local_background: bool = True,
+		local_settings: dict = None
+	) -> None:
+		"""
+		Information logging of stopping Timer:
+		Used to notify the stop of the Timer.
+
+		:param status_message: Log entry status message
+		:param message_text: Log entry message
+		:param local_background: Display entry with background?
+		:param local_settings: Dictionary of local entering settings
+		"""
+		stop_timer_value = datetime.now()
+		self._progress_time = "^" + str(stop_timer_value - self._start_timer_value).split(".")[0]
+
+
+		if local_settings is None:
+			local_settings = {}
+		if not 'italic' in local_settings:
+			local_settings["italic"] = True
+		self._buffer << self._assemble_entry(
+			[
+				self._ColorScheme['STOP_TIMER_TIME'][local_background],
+				self._ColorScheme['STOP_TIMER_STATUS'][local_background],
+				self._ColorScheme['STOP_TIMER_STATUS_MESSAGE'][local_background],
+				self._ColorScheme['TYPE_STOP_TIMER'][local_background],
+				self._ColorScheme['STOP_TIMER_MESSAGE'][local_background],
+				self._ColorScheme['STOP_TIMER_BACKGROUND'][local_background],
+			], self._progress_time, self._icon_set.stop_timer, status_message.current_status_message, "^STOP TIMER", message_text, self._environment, local_settings
+		)
+		if self._environment == LogEnvironments.CONSOLE:
+			self._buffer.update_console()
+
+		self._start_timer_value = None
+		self._progress_time = "        "
```

### Comparing `mighty_logger-0.6.0/mighty_logger/src/__init__.py` & `mighty_logger-0.6.1/mighty_logger/src/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/src/ansi_format.py` & `mighty_logger-0.6.1/mighty_logger/src/ansi_format.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/src/color_picker.py` & `mighty_logger-0.6.1/mighty_logger/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/src/log_enums.py` & `mighty_logger-0.6.1/mighty_logger/src/log_enums.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,7 +42,10 @@
 	WARNING = 'warning'
 	ERROR = 'error'
 	CRITICAL = 'critical'
 	RESOLVED = 'resolved'
 	UNRESOLVED = 'unresolved'
 	ACHIEVEMENT = '_achievement'
 	MILESTONE = '_milestone'
+	START_TIMER = 'start_timer'
+	TIMER_MARK = 'timer_mark'
+	STOP_TIMER = 'stop_timer'
```

### Comparing `mighty_logger-0.6.0/mighty_logger/src/status_variables.py` & `mighty_logger-0.6.1/mighty_logger/src/status_variables.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/text/__init__.py` & `mighty_logger-0.6.1/mighty_logger/text/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/mighty_logger/text/icon_set.py` & `mighty_logger-0.6.1/mighty_logger/text/icon_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 	unresolved = ''
 	initiation = ''
 	process = ''
 	achievement = ''
 	milestone = ''
 	success = ''
 	fail = ''
+	start_timer = ''
+	timer_mark = ''
+	stop_timer = ''
 
 class EmptyIconSet(IconSetType):
 	...
 
 class IconSet1(IconSetType):
 	"""
 	First icon set.
@@ -66,14 +69,17 @@
 	unresolved = '❎'
 	initiation = '🚀'
 	process = '⏳'
 	achievement = '🏆'
 	milestone = '🔖'
 	success = '✔️'
 	fail = '❌'
+	start_timer = '⏰'
+	timer_mark = '⌚'
+	stop_timer = '⏲️'
 
 class IconSet2(IconSetType):
 	"""
 	Second icon set.
 	"""
 	debug = '🐞'
 	debug_performance = '⌛️'
@@ -92,14 +98,17 @@
 	unresolved = '❓'
 	initiation = '🚀'
 	process = '🔄'
 	achievement = '🏆'
 	milestone = '🔖'
 	success = '🎉'
 	fail = '🚫'
+	start_timer = '🕑'
+	timer_mark = '🕕'
+	stop_timer = '🕙'
 
 class IconSet3(IconSetType):
 	"""
 	Third icon set.
 	"""
 	debug = '🚧'
 	debug_performance = '🔍'
@@ -118,14 +127,17 @@
 	unresolved = '🟥'
 	initiation = '🔥'
 	process = '⚙️'
 	achievement = '🌟'
 	milestone = '🎯'
 	success = '👍'
 	fail = '👎'
+	start_timer = '🟩'
+	timer_mark = '🟨'
+	stop_timer = '🟪'
 
 class IconSet4(IconSetType):
 	"""
 	Fourth icon set.
 	"""
 	debug = '🔬'
 	debug_performance = '📈'
@@ -144,7 +156,10 @@
 	unresolved = '🔴'
 	initiation = '🔧'
 	process = '🕰️'
 	achievement = '🎖️'
 	milestone = '🗺️'
 	success = '✅'
 	fail = '❎'
+	start_timer = '⏳'
+	timer_mark = '⏱️'
+	stop_timer = '⌛'
```

### Comparing `mighty_logger-0.6.0/mighty_logger/text/text_buffer.py` & `mighty_logger-0.6.1/mighty_logger/text/text_buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,20 +117,22 @@
 		else:
 			old_excess_console_strings = len(re.sub(r"\033\[.*?m", "", self._text_buffer[number_string])) // self.width
 			new_excess_console_strings = len(re.sub(r"\033\[.*?m", "", message)) // self.width
 			self._buffer_size += new_excess_console_strings - old_excess_console_strings
 			self._text_buffer[number_string] = f"{message}"
 
 	def pop(self, number_string: int = -1) -> str:
-		self._buffer_size -= 1
+		excess_console_string = len(re.sub(r"\033\[.*?m", "", self._text_buffer[-1])) // self.width
+		self._buffer_size -= 1 + excess_console_string
 		last = self._text_buffer.pop(number_string)
 		return last
 
 	def remove(self, number_string: int = -1) -> None:
-		self._buffer_size -= 1
+		excess_console_string = len(re.sub(r"\033\[.*?m", "", self._text_buffer[-1])) // self.width
+		self._buffer_size -= 1 + excess_console_string
 		self._text_buffer.pop(number_string)
 
 	def save(self, name_file: str = "buffer", clean: bool = True) -> None:
 		with open(name_file, "w", encoding="utf-8") as text_buffer_file:
 			if clean:
 				for item in self._text_buffer:
 					text_buffer_file.write("{}\n".format(re.sub(r"\033\[.*?m", "", item)))
```

### Comparing `mighty_logger-0.6.0/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-0.6.1/mighty_logger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mighty-logger
-Version: 0.6.0
+Version: 0.6.1
 Summary: Powerful functional logger with support for qt programming
 Home-page: https://github.com/Nakama3942/mighty_logger
 Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
@@ -91,27 +91,32 @@
 
 - [Content](#content)
 
 ## Important releases
 
 <details><summary>See the important releases (possible spoilers)</summary>
 
+- [x] v0.0.1 - Alpha-release (the very first version of the simplest Logger has been published)
+- [x] v0.0.2 - Little update (added multiple entry types and colors)
+- [x] v0.0.3 - Types update (added even more multiple entry types and colors)
+- [x] v0.0.4 - Color update (added the entire X11 color table and reworked the color system)
 - [x] v0.1.0 - First official release (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
-- [ ] v0.6.1 - Animation update (added animations in processes)
+- [x] v0.6.1 - Animation update (added animations in processes)
 - [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
 - [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
 - [ ] v0.7.2 - Search update (added search by log entry types)
-- [ ] v0.7.3 - Extension update (made wheel format and instruction of toml)
-- [ ] v0.8.0 - ? (???) in short, add export to csv
+- [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
+- [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
+- [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
@@ -149,16 +154,16 @@
 This is the simplest example of using the library:
 
 ```python
 from mighty_logger import Logger
 from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
-    logger = Logger(program_name="Test", console_width=115)
-    logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
+	logger = Logger(program_name="Test", console_width=115)
+	logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
 ```
 
 The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
 
 <pre>
 <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span>
 <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry>         </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span>
@@ -185,18 +190,18 @@
 All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/mighty_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/mighty_logger/blob/master/CODE_OF_CONDUCT.md).
 
 - [Content](#content)
 
 ## Authors
 
 <table align="center" style="border-width: 10; border-style: ridge">
-    <tr>
-        <td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
-        <!--<td></td>-->
-    </tr>
+	<tr>
+		<td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
+		<!--<td></td>-->
+	</tr>
 <!--
-    <tr>
-        <td></td>
-        <td></td>
-    </tr>
+	<tr>
+		<td></td>
+		<td></td>
+	</tr>
 -->
 </table>
```

### Comparing `mighty_logger-0.6.0/mighty_logger.egg-info/SOURCES.txt` & `mighty_logger-0.6.1/mighty_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.0/setup.py` & `mighty_logger-0.6.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name="mighty_logger",
-    version="0.6.0",
+    version="0.6.1",
 
     author="Kalynovsky 'Nakamura Akira' Valentin",
     author_email="nakama3942@gmail.com",
 
     description="Powerful functional logger with support for qt programming",
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `mighty_logger-0.6.0/test/test_console.py` & `mighty_logger-0.6.1/test/test_console.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from time import sleep
 
 from mighty_logger import Logger
 from mighty_logger.src import TypesEntries
+from mighty_logger.text import IndefiniteAnimations, DefiniteAnimations
 
 if __name__ == "__main__":
 	logger = Logger(program_name="Installer", console_width=115, status_message_global_entry=False)
 
 	logger.message(message_text="Program installation started")
+	logger.start_timer(message_text="Timer started")
 
 	sleep(1)
-	logger.start_indefinite_process(message_text="File upload")
+	logger.start_indefinite_process(animation=IndefiniteAnimations.SuperSpace, message_text="File upload")
 	sleep(2)
 	logger.note_process(entry_type=TypesEntries.ACHIEVEMENT, message_text="Files downloaded")
 	sleep(3)
 	logger.progress_rise(100)
 	logger.stop_process(message_text="Files unzipped")
 
 	logger.warning(message_text="Newer version found")
+	logger.timer_mark(message_text="Timer mark", local_background=False)
 
 	sleep(1)
-	logger.start_definite_process(message_text="Installing files")
+	logger.start_definite_process(progress_bar=DefiniteAnimations.Arrow, message_text="Installing files")
 	sleep(0.6)
 	logger.progress_rise(3)
 	sleep(0.4)
 	logger.progress_rise(7)
 	sleep(0.3)
 	logger.progress_rise(14)
 	sleep(0.5)
@@ -39,14 +42,15 @@
 	sleep(1.6)
 	logger.progress_rise(46)
 	sleep(1.1)
 	logger.progress_rise(47)
 	logger.note_process(entry_type=TypesEntries.MILESTONE, message_text="Files prepared")
 	sleep(3.7)
 	logger.progress_rise(76)
+	logger.note_process(entry_type=TypesEntries.TIMER_MARK, message_text="Timer mark")
 	sleep(1.5)
 	logger.progress_rise(77)
 	sleep(1.4)
 	logger.progress_rise(79)
 	sleep(1.1)
 	logger.progress_rise(81)
 	sleep(1.2)
@@ -72,8 +76,10 @@
 	sleep(1.8)
 	logger.progress_rise(97)
 	sleep(1.5)
 	logger.progress_rise(100)
 	sleep(1.3)
 	logger.stop_process(message_text="Program installed")
 
+	logger.stop_timer(message_text="Timer completed")
+
 	logger.buffer().save("log.txt")
```


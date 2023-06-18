# Comparing `tmp/cancli-1.0.0.tar.gz` & `tmp/cancli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cancli-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cancli-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cancli-1.0.0.tar` & `cancli-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      330 2023-04-26 07:59:36.360873 cancli-1.0.0/.gitignore
--rw-r--r--   0        0        0      657 2023-04-26 09:07:35.647689 cancli-1.0.0/LICENSE
--rw-r--r--   0        0        0     3643 2023-06-11 11:23:53.677404 cancli-1.0.0/README.md
--rw-r--r--   0        0        0      199 2023-04-26 10:37:08.721333 cancli-1.0.0/mypy.ini
--rw-r--r--   0        0        0      731 2023-06-11 09:15:39.627632 cancli-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0    11880 2023-06-11 11:36:29.099104 cancli-1.0.0/release.sh
--rw-r--r--   0        0        0        5 2023-06-07 08:49:16.337278 cancli-1.0.0/requirements-release.txt
--rw-r--r--   0        0        0       11 2023-06-07 08:49:16.337278 cancli-1.0.0/requirements-test.txt
--rw-r--r--   0        0        0       59 2023-06-11 09:33:26.238602 cancli-1.0.0/requirements.txt
--rw-r--r--   0        0        0       57 2023-06-11 11:36:29.102437 cancli-1.0.0/src/cancli/__init__.py
--rw-r--r--   0        0        0       83 2023-06-04 18:38:27.573269 cancli-1.0.0/src/cancli/__main__.py
--rw-r--r--   0        0        0     4987 2023-06-09 13:54:35.309580 cancli-1.0.0/src/cancli/can_handler.py
--rw-r--r--   0        0        0     4146 2023-06-10 16:42:44.839580 cancli-1.0.0/src/cancli/can_setup.py
--rw-r--r--   0        0        0    27973 2023-06-11 11:36:50.048971 cancli-1.0.0/src/cancli/main.py
--rw-r--r--   0        0        0      112 2023-06-11 11:43:17.246429 cancli-1.0.0/src/cancli/meta.py
--rw-r--r--   0        0        0     6111 2023-06-04 18:38:40.383152 cancli-1.0.0/src/cancli/parse_error_frame.py
--rwxr-xr-x   0        0        0      140 2023-06-04 05:59:57.475881 cancli-1.0.0/src/cancli/runmodule.sh
--rw-r--r--   0        0        0     1182 2023-06-07 09:02:19.858241 cancli-1.0.0/src/cancli/utils.py
--rw-r--r--   0        0        0      336 2023-06-11 10:55:18.149452 cancli-1.0.0/tox.ini
--rw-r--r--   0        0        0     4340 1970-01-01 00:00:00.000000 cancli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      330 2023-04-26 07:59:36.360873 cancli-1.0.1/.gitignore
+-rw-r--r--   0        0        0      657 2023-04-26 09:07:35.647689 cancli-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3657 2023-06-18 09:55:14.025247 cancli-1.0.1/README.md
+-rw-r--r--   0        0        0      199 2023-04-26 10:37:08.721333 cancli-1.0.1/mypy.ini
+-rw-r--r--   0        0        0      731 2023-06-11 09:15:39.627632 cancli-1.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0    11880 2023-06-11 11:36:29.099104 cancli-1.0.1/release.sh
+-rw-r--r--   0        0        0        5 2023-06-07 08:49:16.337278 cancli-1.0.1/requirements-release.txt
+-rw-r--r--   0        0        0       11 2023-06-07 08:49:16.337278 cancli-1.0.1/requirements-test.txt
+-rw-r--r--   0        0        0       59 2023-06-11 09:33:26.238602 cancli-1.0.1/requirements.txt
+-rw-r--r--   0        0        0       57 2023-06-11 11:36:29.102437 cancli-1.0.1/src/cancli/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-04 18:38:27.573269 cancli-1.0.1/src/cancli/__main__.py
+-rw-r--r--   0        0        0     5391 2023-06-18 09:55:14.025247 cancli-1.0.1/src/cancli/can_handler.py
+-rw-r--r--   0        0        0     4146 2023-06-10 16:42:44.839580 cancli-1.0.1/src/cancli/can_setup.py
+-rw-r--r--   0        0        0    28369 2023-06-18 09:55:14.025247 cancli-1.0.1/src/cancli/main.py
+-rw-r--r--   0        0        0      112 2023-06-18 09:55:14.025247 cancli-1.0.1/src/cancli/meta.py
+-rw-r--r--   0        0        0     6111 2023-06-04 18:38:40.383152 cancli-1.0.1/src/cancli/parse_error_frame.py
+-rwxr-xr-x   0        0        0      140 2023-06-04 05:59:57.475881 cancli-1.0.1/src/cancli/runmodule.sh
+-rw-r--r--   0        0        0     1182 2023-06-07 09:02:19.858241 cancli-1.0.1/src/cancli/utils.py
+-rw-r--r--   0        0        0      336 2023-06-11 10:55:18.149452 cancli-1.0.1/tox.ini
+-rw-r--r--   0        0        0     4354 1970-01-01 00:00:00.000000 cancli-1.0.1/PKG-INFO
```

### Comparing `cancli-1.0.0/LICENSE` & `cancli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cancli-1.0.0/README.md` & `cancli-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,25 +63,26 @@
 - [Bug tracker](https://gitlab.com/erzo/cancli/-/issues)
 - [Change log](https://gitlab.com/erzo/cancli/-/tags)
 
 
 ## Running the tests
 
 I am using [mypy](https://www.mypy-lang.org/) for static type checking.
-[tox](https://tox.wiki/en/latest/) creates a vitual environment and installs all dependencies for you.
+[tox](https://tox.wiki/en/latest/) creates a virtual environment and installs all dependencies for you.
 You can install tox with [pipx](https://pypa.github.io/pipx/) (`pipx install tox`).
 
 ```bash
 $ tox
 ```
 
 In order to make tox work without an internet connection install [devpi](https://devpi.net/docs/devpi/devpi/stable/%2Bd/index.html):
 
 ```bash
 $ pipx install devpi-server
+$ devpi-init
 $ devpi-gen-config
 $ su
 # cp gen-config/devpi.service /etc/systemd/system/
 # systemctl start devpi.service
 # systemctl enable devpi.service
 ```
```

### Comparing `cancli-1.0.0/pyproject.toml` & `cancli-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cancli-1.0.0/release.sh` & `cancli-1.0.1/release.sh`

 * *Files identical despite different names*

### Comparing `cancli-1.0.0/src/cancli/can_handler.py` & `cancli-1.0.1/src/cancli/can_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,7 +152,19 @@
 		signal_start = signal_start.casefold()
 		for sig in msg.signals:
 			if signal_start in sig.name.casefold():
 				out.append(sig.name)
 		if self.node_id_mask and signal_start in self.PARAM_NODE_ID:
 			out.append(self.PARAM_NODE_ID)
 		return out
+
+	def get_completions_for_signal_value(self, msg_name: str, signal_name: str, value_start: str) -> 'list[str]':
+		msg = self.get_cantools_message_by_name(msg_name)
+		if not msg:
+			return []
+
+		sig = msg.get_signal_by_name(signal_name)
+		if not sig.choices:
+			return []
+
+		value_start = value_start.casefold()
+		return [str(name) for name in sig.choices.values() if value_start in str(name).casefold()]
```

### Comparing `cancli-1.0.0/src/cancli/can_setup.py` & `cancli-1.0.1/src/cancli/can_setup.py`

 * *Files identical despite different names*

### Comparing `cancli-1.0.0/src/cancli/main.py` & `cancli-1.0.1/src/cancli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 	color_prompt = Config('color.prompt', 'ansiblue', type=Color())
 
 	print_raw = Config('print.raw', True, help="Print received raw data")
 	print_pretty = Config('print.pretty', True, help="Print decoded data")
 	print_error = Config('print.error', True, help="Print CAN bus errors")
 	prompt = Config('prompt', ">>> ")
 	pattern_message = Config('pattern.message', "{canmsg.arbitration_id:>0{id_width}x} {msg.name}", help="How to format a message. Wildcards: canmsg (a can.Message object), msg (a cantools.db.Message object) and id_width (the number of hex characters required to represent the biggest possible arbitration_id depending on is_extended_id)")
-	pattern_signal = Config('pattern.signal', "\t{key}: {val}", help="How to format a signal. Wildcards: key (a str) and val (a str, int or float).")
+	pattern_signal = Config('pattern.signal', "\t{key}: {val}{unit}", help="How to format a signal. Wildcards: key (a str), val (a str, int or float) and unit (a possibly empty str).")
 	pattern_remote = Config('pattern.remote', "\tremote frame", help="How to format a remote message. This is printed instead of the signals. No wildcards.")
 	min_time_span_between_can_errors_in_s = Config('print.min-time-span-between-errors', 1.0, unit="s", help="Do not print equal CAN bus errors more frequently than this")
 
 	editor = Config('editor', SubprocessCommandWithAlternatives.editor(visual=False), help="The editor to be used when opening the config file")
 
 	def __init__(self, argv: 'list[str]|None') -> None:
 		CancliCommand.app = self
@@ -207,23 +207,27 @@
 					self.colored_print(msgcolor, self.pattern_remote)
 					return msg
 				key: str
 				val: cantools.typechecking.SignalValueType
 				if self.bus_handler.is_node_id_set():
 					key = self.bus_handler.PARAM_NODE_ID
 					val = self.bus_handler.get_node_id(canmsg)
-					self.colored_print(self.color_sig.get_color(key, msgcolor) if val else msgcolor, prefix + self.pattern_signal.format(key=key, val=val))
+					self.colored_print(self.color_sig.get_color(key, msgcolor) if val else msgcolor, prefix + self.pattern_signal.format(key=key, val=val, unit=""))
 				raw_data = canmsg.data.copy()
 				while len(raw_data) < msg.length:
 					raw_data.append(0)
 				data = msg.decode_simple(raw_data)
 				for key, val in data.items():
 					if isinstance(val, TYPE_CANTOOLS_NAMED_SIGNAL_VALUE):
-						val = val.value
-					self.colored_print(self.color_sig.get_color(key, msgcolor) if val else msgcolor, prefix + self.pattern_signal.format(key=key, val=val))
+						nonzero = bool(val.value)
+					else:
+						nonzero = bool(val)
+					sig = msg.get_signal_by_name(key)
+					unit = sig.unit if sig.unit else ""
+					self.colored_print(self.color_sig.get_color(key, msgcolor) if nonzero else msgcolor, prefix + self.pattern_signal.format(key=key, val=val, unit=unit))
 			return msg
 
 		else:
 			if not ignore_filters and self._hide.get(canmsg.arbitration_id, 0) >= self._show.get(canmsg.arbitration_id, self.show_by_default):
 				return msg
 			self.colored_print(self.color_unknown_message, prefix + self.format_raw(canmsg))
 			return msg
@@ -569,14 +573,19 @@
 		return super().get_completions(cmd, argument_pos, cursor_pos, in_between=in_between, start_of_line=start_of_line, end_of_line=end_of_line)
 
 	def get_completions_for_positional_argument(self, position: int, start: str, *, start_of_line: str, end_of_line: str) -> 'tuple[str, list[str], str]':
 		if position == 0:
 			return start_of_line, self.app.bus_handler.get_completions_for_message_name(start), end_of_line
 
 		msg = next(w for w in self.__cmd[1:] if not w.startswith("-"))
+		if '=' in start:
+			sig_name, start = start.split('=', 1)
+			start_of_line += sig_name + '='
+			return start_of_line, self.app.bus_handler.get_completions_for_signal_value(msg, sig_name, start), end_of_line
+
 		return start_of_line, self.app.bus_handler.get_completions_for_signal_name(msg, start), end_of_line
 
 
 class MessageTakingCommand(CancliCommand, abstract=True):
 
 	'''
 	Messages can be specified by name or by id.
```

### Comparing `cancli-1.0.0/src/cancli/parse_error_frame.py` & `cancli-1.0.1/src/cancli/parse_error_frame.py`

 * *Files identical despite different names*

### Comparing `cancli-1.0.0/src/cancli/utils.py` & `cancli-1.0.1/src/cancli/utils.py`

 * *Files identical despite different names*

### Comparing `cancli-1.0.0/PKG-INFO` & `cancli-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cancli
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command line interface to send and receive CAN bus messages.
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Requires-Dist: prompt_toolkit
@@ -81,25 +81,26 @@
 - [Bug tracker](https://gitlab.com/erzo/cancli/-/issues)
 - [Change log](https://gitlab.com/erzo/cancli/-/tags)
 
 
 ## Running the tests
 
 I am using [mypy](https://www.mypy-lang.org/) for static type checking.
-[tox](https://tox.wiki/en/latest/) creates a vitual environment and installs all dependencies for you.
+[tox](https://tox.wiki/en/latest/) creates a virtual environment and installs all dependencies for you.
 You can install tox with [pipx](https://pypa.github.io/pipx/) (`pipx install tox`).
 
 ```bash
 $ tox
 ```
 
 In order to make tox work without an internet connection install [devpi](https://devpi.net/docs/devpi/devpi/stable/%2Bd/index.html):
 
 ```bash
 $ pipx install devpi-server
+$ devpi-init
 $ devpi-gen-config
 $ su
 # cp gen-config/devpi.service /etc/systemd/system/
 # systemctl start devpi.service
 # systemctl enable devpi.service
 ```
```


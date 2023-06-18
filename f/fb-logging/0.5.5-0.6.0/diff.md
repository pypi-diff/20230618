# Comparing `tmp/fb_logging-0.5.5.tar.gz` & `tmp/fb_logging-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb_logging-0.5.5.tar", last modified: Fri Dec 30 09:27:20 2022, max compression
+gzip compressed data, was "fb_logging-0.6.0.tar", last modified: Sun Jun 18 18:06:04 2023, max compression
```

## Comparing `fb_logging-0.5.5.tar` & `fb_logging-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 09:27:20.037531 fb_logging-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2022-12-30 09:27:14.000000 fb_logging-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-30 09:27:14.000000 fb_logging-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-30 09:27:20.037531 fb_logging-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-30 09:27:14.000000 fb_logging-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 09:27:20.037531 fb_logging-0.5.5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14224 2022-12-30 09:27:14.000000 fb_logging-0.5.5/bin/dch2speclog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 09:27:20.037531 fb_logging-0.5.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 09:27:20.037531 fb_logging-0.5.5/lib/fb_logging/
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2022-12-30 09:27:14.000000 fb_logging-0.5.5/lib/fb_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16459 2022-12-30 09:27:14.000000 fb_logging-0.5.5/lib/fb_logging/colored.py
--rw-r--r--   0 runner    (1001) docker     (123)    42932 2022-12-30 09:27:14.000000 fb_logging-0.5.5/lib/fb_logging/deb_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2022-12-30 09:27:14.000000 fb_logging-0.5.5/lib/fb_logging/deb_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2022-12-30 09:27:19.000000 fb_logging-0.5.5/lib/fb_logging/local_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2022-12-30 09:27:14.000000 fb_logging-0.5.5/lib/fb_logging/syslog_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2022-12-30 09:27:14.000000 fb_logging-0.5.5/lib/fb_logging/unix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 09:27:20.037531 fb_logging-0.5.5/lib/fb_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-30 09:27:19.000000 fb_logging-0.5.5/lib/fb_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-30 09:27:19.000000 fb_logging-0.5.5/lib/fb_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 09:27:19.000000 fb_logging-0.5.5/lib/fb_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-30 09:27:19.000000 fb_logging-0.5.5/lib/fb_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2022-12-30 09:27:20.037531 fb_logging-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2022-12-30 09:27:14.000000 fb_logging-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 09:27:20.037531 fb_logging-0.5.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2022-12-30 09:27:14.000000 fb_logging-0.5.5/test/general.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8419 2022-12-30 09:27:14.000000 fb_logging-0.5.5/test/test_colored.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10473 2022-12-30 09:27:14.000000 fb_logging-0.5.5/test/test_fb_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6375 2022-12-30 09:27:14.000000 fb_logging-0.5.5/test/test_syslog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:06:04.109845 fb_logging-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-18 18:05:55.000000 fb_logging-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 18:05:55.000000 fb_logging-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-18 18:06:04.109845 fb_logging-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-18 18:05:55.000000 fb_logging-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:06:04.109845 fb_logging-0.6.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14224 2023-06-18 18:05:55.000000 fb_logging-0.6.0/bin/dch2speclog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:06:04.105845 fb_logging-0.6.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:06:04.109845 fb_logging-0.6.0/lib/fb_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-06-18 18:05:55.000000 fb_logging-0.6.0/lib/fb_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16513 2023-06-18 18:05:55.000000 fb_logging-0.6.0/lib/fb_logging/colored.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42932 2023-06-18 18:05:55.000000 fb_logging-0.6.0/lib/fb_logging/deb_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12290 2023-06-18 18:05:55.000000 fb_logging-0.6.0/lib/fb_logging/deb_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-18 18:06:04.000000 fb_logging-0.6.0/lib/fb_logging/local_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-18 18:05:55.000000 fb_logging-0.6.0/lib/fb_logging/syslog_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-06-18 18:05:55.000000 fb_logging-0.6.0/lib/fb_logging/unix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:06:04.109845 fb_logging-0.6.0/lib/fb_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-18 18:06:04.000000 fb_logging-0.6.0/lib/fb_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-18 18:06:04.000000 fb_logging-0.6.0/lib/fb_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:06:04.000000 fb_logging-0.6.0/lib/fb_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 18:06:04.000000 fb_logging-0.6.0/lib/fb_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-18 18:06:04.113845 fb_logging-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-18 18:05:55.000000 fb_logging-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:06:04.109845 fb_logging-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-18 18:05:55.000000 fb_logging-0.6.0/test/general.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8419 2023-06-18 18:05:55.000000 fb_logging-0.6.0/test/test_colored.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10473 2023-06-18 18:05:55.000000 fb_logging-0.6.0/test/test_fb_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6375 2023-06-18 18:05:55.000000 fb_logging-0.6.0/test/test_syslog.py
```

### Comparing `fb_logging-0.5.5/LICENSE` & `fb_logging-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fb_logging-0.5.5/PKG-INFO` & `fb_logging-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb_logging
-Version: 0.5.5
+Version: 0.6.0
 Summary: Python modules to extend the logging mechanism in Python.
 Home-page: https://github.com/fbrehm/fb-logging
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_logging-0.5.5/bin/dch2speclog` & `fb_logging-0.6.0/bin/dch2speclog`

 * *Files identical despite different names*

### Comparing `fb_logging-0.5.5/lib/fb_logging/__init__.py` & `fb_logging-0.6.0/lib/fb_logging/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 @contact: frank@brehm-online.com
 @copyright: © 2022 by Frank Brehm, Berlin
 """
 
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
 __copyright__ = '(C) 2022 by Frank Brehm, Berlin'
 __contact__ = 'frank@brehm-online.com'
-__version__ = '0.5.5'
+__version__ = '0.6.0'
 __license__ = 'LGPL-3'
 
 # Standard modules
-import os
 import copy
 import logging
 import logging.handlers
+import os
 import syslog
-
 from numbers import Number
 
 
 # =============================================================================
 class FbLoggingError(Exception):
     """Base error class for all other self defined exceptions."""
 
@@ -50,15 +49,15 @@
     def __init__(self, value):
         """Construct this exception."""
         self.value = value
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Wrong variable {v!r} ({t}) given as a syslog facility id.".format(
+        msg = 'Wrong variable {v!r} ({t}) given as a syslog facility id.'.format(
             v=self.value, t=self.value.__class__.__name__)
         return msg
 
 
 # =============================================================================
 class WrongLogFacilityIdValueError(SyslogFacitityError, ValueError):
     """Error class about a wrong variable value as a Syslog facility Id.
@@ -71,15 +70,15 @@
     def __init__(self, value):
         """Construct this exception."""
         self.value = value
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Wrong variable {} given as a syslog facility id.".format(self.value)
+        msg = 'Wrong variable {} given as a syslog facility id.'.format(self.value)
         return msg
 
 
 # =============================================================================
 class WrongLogFacilityNameTypeError(SyslogFacitityError, TypeError):
     """Error class about a wrong variable type as a Syslog facility name.
 
@@ -91,15 +90,15 @@
     def __init__(self, value):
         """Construct this exception."""
         self.value = value
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Wrong variable {v!r} ({t}) given as a syslog facility name.".format(
+        msg = 'Wrong variable {v!r} ({t}) given as a syslog facility name.'.format(
             v=self.value, t=self.value.__class__.__name__)
         return msg
 
 
 # =============================================================================
 class WrongLogFacilityNameValueError(SyslogFacitityError, ValueError):
     """Error class about a wrong variable value as a Syslog facility name.
@@ -112,15 +111,15 @@
     def __init__(self, value):
         """Construct this exception."""
         self.value = value
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        msg = "Wrong variable {!r} given as a syslog facility name.".format(self.value)
+        msg = 'Wrong variable {!r} given as a syslog facility name.'.format(self.value)
         return msg
 
 
 # =============================================================================
 def stdout_is_redirected():
     """Check if stdout is redirected."""
     return os.fstat(0) != os.fstat(1)
```

### Comparing `fb_logging-0.5.5/lib/fb_logging/colored.py` & `fb_logging-0.6.0/lib/fb_logging/colored.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """@summary: Additional logging formatter for colored output via console."""
 
-import logging
 import copy
+import logging
 import re
-
-from numbers import Number
 from collections.abc import Sequence
+from numbers import Number
 
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 
 
 # =============================================================================
 class ColorNotFoundError(KeyError):
     """Class for an exception in case that a color was not found."""
 
     # -------------------------------------------------------------------------
     def __init__(self, color):
         """Construct this exception."""
         self.color = color
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        return "Color {!r} not found.".format(self.color)
+        return 'Color {!r} not found.'.format(self.color)
 
 
 # =============================================================================
 class WrongColorTypeError(TypeError):
     """Class for an exception in case that a wrong type for a color was given."""
 
     # -------------------------------------------------------------------------
     def __init__(self, color):
         """Construct this exception."""
         self.color = color
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
-        return "Color {c!r} has wrong type {t}.".format(
+        return 'Color {c!r} has wrong type {t}.'.format(
             c=self.color, t=self.color.__class__.__name__)
 
 
 # =============================================================================
 class Colors:
     """A class for handling terminal color codes."""
 
@@ -461,15 +460,15 @@
         return self.level_color['CRITICAL']
 
     @color_critical.setter
     def color_critical(self, value):
         self.level_color['CRITICAL'] = value
 
     # -------------------------------------------------------------------------
-    def format(self, record):
+    def format(self, record):                                           # noqa A003.
         """Format the specified record as text."""
         rcrd = copy.copy(record)
         levelname = rcrd.levelname
 
         if levelname in self.level_color:
 
             rcrd.name = colorstr(rcrd.name, 'bold')
```

### Comparing `fb_logging-0.5.5/lib/fb_logging/deb_changelog.py` & `fb_logging-0.6.0/lib/fb_logging/deb_changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         self._line = line
         super(ChangelogParseError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecasting into str."""
         # type: () -> str
-        return "Could not parse changelog: "+self._line
+        return 'Could not parse changelog: '+self._line
 
 
 # =============================================================================
 class ChangelogCreateError(_base_exception_class):
     """Indicates that changelog could not be created.
 
     Because as all the information required was not given.
@@ -175,15 +175,15 @@
         # type: (str) -> None
         self._version = version
         super(VersionError, self).__init__()
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecasting into str."""
-        return "Could not parse version: " + self._version
+        return 'Could not parse version: ' + self._version
 
 
 # =============================================================================
 class ChangeBlock(object):
     """Holds all the information about one block from the changelog.
 
     See `deb-changelog(5)
@@ -223,24 +223,24 @@
                  ):
         """Construct this object."""
         # type: (...) -> None
         self._raw_version = None   # type: Optional[str]
         self._set_version(version)
         self.package = package
         self.distributions = distributions
-        self.urgency = urgency or "unknown"
+        self.urgency = urgency or 'unknown'
         self.urgency_comment = urgency_comment or ''
         self._changes = changes or []   # type: List[Text]
         self.author = author
         self.date = date
         self._trailing = []    # type: List[Text]
         self.other_pairs = other_pairs or {}
         self._encoding = encoding
         self._no_trailer = False
-        self._trailer_separator = "  "
+        self._trailer_separator = '  '
 
     # -------------------------------------------------------------------------
     def _set_version(self, version):
         # type: (Optional[Union[Version, str]]) -> None
         if version is not None:
             self._raw_version = str(version)
 
@@ -250,27 +250,27 @@
         if self._raw_version is None:
             return None
         return Version(self._raw_version)
 
     # -------------------------------------------------------------------------
     version = property(
         _get_version, _set_version,
-        doc="The package version that this block pertains to"
+        doc='The package version that this block pertains to'
     )
 
     # -------------------------------------------------------------------------
     def other_keys_normalised(self):
         # type: () -> Dict[str, str]
         """Obtain a dict from the block header (other than urgency)."""
         norm_dict = {}
         for (key, value) in self.other_pairs.items():
             key = key[0].upper() + key[1:].lower()
             m = xbcs_re.match(key)
             if m is None:
-                key = "XS-%s" % key
+                key = 'XS-%s' % key
             norm_dict[key] = value
         return norm_dict
 
     # -------------------------------------------------------------------------
     def changes(self):
         # type: () -> List[str]
         """Get the changelog entries for this block as a list of str."""
@@ -308,15 +308,15 @@
     # -------------------------------------------------------------------------
     def _get_bugs_closed_generic(self, type_re):
         # type: (Pattern) -> List[int]
         changes = six.u(' ').join(self._changes)
         bugs = []
         for match in type_re.finditer(changes):
             closes_list = match.group(0)
-            for bugmatch in re.finditer(r"\d+", closes_list):
+            for bugmatch in re.finditer(r'\d+', closes_list):
                 bugs.append(int(bugmatch.group(0)))
         return bugs
 
     # -------------------------------------------------------------------------
     @property
     def bugs_closed(self):
         # type: () -> List[int]
@@ -330,43 +330,43 @@
         """List of Launchpad bugs closed by the block."""
         return self._get_bugs_closed_generic(closeslp)
 
     # -------------------------------------------------------------------------
     def _format(self):
         # type: () -> str
         # TODO(jsw): Switch to StringIO or a list to join at the end.
-        block = ""
+        block = ''
         if self.package is None:
-            raise ChangelogCreateError("Package not specified")
-        block += self.package + " "
+            raise ChangelogCreateError('Package not specified')
+        block += self.package + ' '
         if self._raw_version is None:
-            raise ChangelogCreateError("Version not specified")
-        block += "(" + self._raw_version + ") "
+            raise ChangelogCreateError('Version not specified')
+        block += '(' + self._raw_version + ') '
         if self.distributions is None:
-            raise ChangelogCreateError("Distribution not specified")
-        block += self.distributions + "; "
+            raise ChangelogCreateError('Distribution not specified')
+        block += self.distributions + '; '
         if self.urgency is None:
-            raise ChangelogCreateError("Urgency not specified")
-        block += "urgency=" + self.urgency + self.urgency_comment
+            raise ChangelogCreateError('Urgency not specified')
+        block += 'urgency=' + self.urgency + self.urgency_comment
         for (key, value) in self.other_pairs.items():
-            block += ", %s=%s" % (key, value)
+            block += ', %s=%s' % (key, value)
         block += '\n'
         if self.changes() is None:
-            raise ChangelogCreateError("Changes not specified")
+            raise ChangelogCreateError('Changes not specified')
         for change in self.changes():
-            block += change + "\n"
+            block += change + '\n'
         if not self._no_trailer:
             if self.author is None:
-                raise ChangelogCreateError("Author not specified")
+                raise ChangelogCreateError('Author not specified')
             if self.date is None:
-                raise ChangelogCreateError("Date not specified")
-            block += " -- " + self.author + self._trailer_separator \
-                + self.date + "\n"
+                raise ChangelogCreateError('Date not specified')
+            block += ' -- ' + self.author + self._trailer_separator \
+                + self.date + '\n'
         for line in self._trailing:
-            block += line + "\n"
+            block += line + '\n'
         return block
 
     # -------------------------------------------------------------------------
     __str__ = _format
 
     # -------------------------------------------------------------------------
     def __bytes__(self):
@@ -523,19 +523,19 @@
 
         If you create an Changelog object without specifying a changelog
         file, you can parse a changelog file with this method. If the
         changelog doesn't parse cleanly, a :class:`ChangelogParseError`
         exception is thrown. The constructor will parse the changelog on
         a best effort basis.
         """
-        first_heading = "first heading"
-        next_heading_or_eof = "next heading of EOF"
-        start_of_change_data = "start of change data"
-        more_changes_or_trailer = "more change data or trailer"
-        slurp_to_end = "slurp to end"
+        first_heading = 'first heading'
+        next_heading_or_eof = 'next heading of EOF'
+        start_of_change_data = 'start of change data'
+        more_changes_or_trailer = 'more change data or trailer'
+        slurp_to_end = 'slurp to end'
 
         encoding = encoding or self._encoding
 
         if file is None:
             self._parse_error('Empty changelog file.', strict)
             return
 
@@ -570,37 +570,37 @@
                     if (max_blocks is not None
                             and len(self._blocks) >= max_blocks):
                         return
                     current_block.package = top_match.group(1)
                     current_block._raw_version = top_match.group(2)
                     current_block.distributions = top_match.group(3).lstrip()
 
-                    pairs = line.split(";", 1)[1]
+                    pairs = line.split(';', 1)[1]
                     all_keys = {}      # type: Dict[str, str]
                     other_pairs = {}   # type: Dict[str, str]
                     for pair in pairs.split(','):
                         pair = pair.strip()
                         kv_match = keyvalue.match(pair)
                         if kv_match is None:
                             self._parse_error(
                                 "Invalid key-value pair after ';': %s" % pair,
                                 strict)
                             continue
                         key = kv_match.group(1)
                         value = kv_match.group(2)
                         if key.lower() in all_keys:
                             self._parse_error(
-                                "Repeated key-value: "
-                                "%s" % key.lower(), strict)
+                                'Repeated key-value: '
+                                '%s' % key.lower(), strict)
                         all_keys[key.lower()] = value
-                        if key.lower() == "urgency":
+                        if key.lower() == 'urgency':
                             val_match = value_re.match(value)
                             if val_match is None:
                                 self._parse_error(
-                                    "Badly formatted urgency value: %s" %
+                                    'Badly formatted urgency value: %s' %
                                     value, strict)
                             else:
                                 current_block.urgency = val_match.group(1)
                                 comment = val_match.group(2)
                                 if comment is not None:
                                     current_block.urgency_comment = comment
                         else:
@@ -641,15 +641,15 @@
                          or old_format_re8.match(line) is not None)
                             and state != first_heading):
                         self._blocks[-1].add_trailing_line(line)
                         old_state = state
                         state = slurp_to_end
                         continue
                     self._parse_error(
-                        "Unexpected line while looking for %s: %s" %
+                        'Unexpected line while looking for %s: %s' %
                         (state, line), strict)
                     if state == first_heading:
                         self.initial_blank_lines.append(line)
                     else:
                         self._blocks[-1].add_trailing_line(line)
             elif state in (start_of_change_data, more_changes_or_trailer):
                 change_match = changere.match(line)
@@ -658,28 +658,28 @@
                 blank_match = blankline.match(line)
                 if change_match is not None:
                     changes.append(line)
                     state = more_changes_or_trailer
                 elif end_match is not None:
                     if end_match.group(3) != '  ':
                         self._parse_error(
-                            "Badly formatted trailer line: %s" % line, strict)
+                            'Badly formatted trailer line: %s' % line, strict)
                         current_block._trailer_separator = end_match.group(3)
-                    current_block.author = "%s <%s>" \
+                    current_block.author = '%s <%s>' \
                         % (end_match.group(1), end_match.group(2))
                     current_block.date = end_match.group(4)
                     current_block._changes = changes
                     self._blocks.append(current_block)
                     changes = []
                     current_block = ChangeBlock(encoding=encoding)
                     state = next_heading_or_eof
                 elif end_no_details_match is not None:
                     if not allow_empty_author:
                         self._parse_error(
-                            "Badly formatted trailer line: %s" % line, strict)
+                            'Badly formatted trailer line: %s' % line, strict)
                         continue
                     current_block._changes = changes
                     self._blocks.append(current_block)
                     changes = []
                     current_block = ChangeBlock(encoding=encoding)
                     state = next_heading_or_eof
                 elif blank_match is not None:
@@ -689,28 +689,28 @@
                     comments_match = comments.match(line)
                     more_comments_match = more_comments.match(line)
                     if (cvs_match is not None or comments_match is not None
                             or more_comments_match is not None):
                         changes.append(line)
                         continue
                     self._parse_error(
-                        "Unexpected line while looking for %s: %s" %
+                        'Unexpected line while looking for %s: %s' %
                         (state, line), strict)
                     changes.append(line)
             elif state == slurp_to_end:
                 if old_state == next_heading_or_eof:
                     self._blocks[-1].add_trailing_line(line)
                 else:
                     changes.append(line)
             else:
-                assert False, "Unknown state: %s" % state
+                assert False, 'Unknown state: %s' % state
 
         if (state not in (next_heading_or_eof, slurp_to_end)
                 or (state == slurp_to_end and old_state != next_heading_or_eof)):
-            self._parse_error("Found eof where expected %s" % state, strict)
+            self._parse_error('Found eof where expected %s' % state, strict)
             current_block._changes = changes
             current_block._no_trailer = True
             self._blocks.append(current_block)
 
     # -------------------------------------------------------------------------
     def get_version(self):
         # type: () -> Version
@@ -733,36 +733,36 @@
             (Property that can both get and set the version.)"""
     )
 
     # -------------------------------------------------------------------------
     # For convenience, let's expose some of the version properties
     full_version = property(
         lambda self: self.version.full_version,
-        doc="The full version number of the last version"
+        doc='The full version number of the last version'
     )
     # -------------------------------------------------------------------------
     epoch = property(
         lambda self: self.version.epoch,
-        doc="The epoch number of the last revision, or `None` "
-        "if no epoch was used."
+        doc='The epoch number of the last revision, or `None` '
+        'if no epoch was used.'
     )
     # -------------------------------------------------------------------------
     debian_version = property(
         lambda self: self.version.debian_revision,
-        doc="The debian part of the version number of the last version."
+        doc='The debian part of the version number of the last version.'
     )
     # -------------------------------------------------------------------------
     debian_revision = property(
         lambda self: self.version.debian_revision,
-        doc="The debian part of the version number of the last version."
+        doc='The debian part of the version number of the last version.'
     )
     # -------------------------------------------------------------------------
     upstream_version = property(
         lambda self: self.version.upstream_version,
-        doc="The upstream part of the version number of the last version."
+        doc='The upstream part of the version number of the last version.'
     )
 
     # -------------------------------------------------------------------------
     def get_package(self):
         # type: () -> Optional[str]
         """Return the name of the package in the last entry."""
         return self._blocks[0].package
@@ -772,15 +772,15 @@
         # type: (str) -> None
         """Set the name of the package in the last entry."""
         self._blocks[0].package = package
 
     # -------------------------------------------------------------------------
     package = property(
         get_package, set_package,
-        doc="Name of the package in the last version"
+        doc='Name of the package in the last version'
     )
 
     # -------------------------------------------------------------------------
     def get_versions(self):
         """Return a list of version objects that the package went through."""
         # type: () -> List[Version]
         return [block.version for block in self._blocks]
@@ -969,15 +969,15 @@
     DEBEMAIL, DEBFULLNAME, EMAIL, NAME, /etc/mailname and gecos.
 
     :returns: a tuple of the full name, email pair as strings.
         Either of the pair may be None if that value couldn't
         be determined.
     """
     env = os.environ
-    regex = re.compile(r"^(.*)\s+<(.*)>$")
+    regex = re.compile(r'^(.*)\s+<(.*)>$')
 
     # Split email and name
     if 'DEBEMAIL' in env:
         match_obj = regex.match(env['DEBEMAIL'])
         if match_obj:
             if 'DEBFULLNAME' not in env:
                 env['DEBFULLNAME'] = match_obj.group(1)
@@ -1020,15 +1020,15 @@
         if not addr:
             addr = socket.getfqdn()
         if addr:
             user = pwd.getpwuid(os.getuid()).pw_name
             if not user:
                 addr = None
             else:
-                addr = "%s@%s" % (user, addr)
+                addr = '%s@%s' % (user, addr)
 
         if addr:
             email_address = addr
 
     return (maintainer, email_address)
```

### Comparing `fb_logging-0.5.5/lib/fb_logging/deb_version.py` & `fb_logging-0.6.0/lib/fb_logging/deb_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
 
 from __future__ import absolute_import, print_function
 
 import re
-
 import warnings
 
 try:
     # pylint: disable=unused-import
     from typing import (    # noqa: F401
         Any,
         Optional,
@@ -43,15 +42,15 @@
     Returns a new function that warns it is deprecated by function
     ``func``, then acts as a pass-through wrapper for ``func``.
     """
     try:
         func_name = func.__name__
     except AttributeError:
         func_name = func.__func__.__name__
-    warn_msg = "Use %s instead" % func_name
+    warn_msg = 'Use %s instead' % func_name
 
     def deprecated_func(*args, **kwargs):
         warnings.warn(warn_msg, DeprecationWarning, stacklevel=2)
         return func(*args, **kwargs)
     return deprecated_func
 
 
@@ -69,17 +68,17 @@
     recomputed and the rest of the properties set from that.
 
     It also implements __str__, just returning the raw version given to the
     initializer.
     """
 
     re_valid_version = re.compile(
-        r"^((?P<epoch>\d+):)?"
-        "(?P<upstream_version>[A-Za-z0-9.+:~-]+?)"
-        "(-(?P<debian_revision>[A-Za-z0-9+.~]+))?$")
+        r'^((?P<epoch>\d+):)?'
+        '(?P<upstream_version>[A-Za-z0-9.+:~-]+?)'
+        '(-(?P<debian_revision>[A-Za-z0-9+.~]+))?$')
     magic_attrs = (
         'full_version', 'epoch', 'upstream_version',
         'debian_revision', 'debian_version')
 
     # -------------------------------------------------------------------------
     def __init__(self, version):
         """Construct this object."""
@@ -89,78 +88,78 @@
         self.full_version = version
 
     # -------------------------------------------------------------------------
     def _set_full_version(self, version):
         # type: (str) -> None
         m = self.re_valid_version.match(version)
         if not m:
-            raise ValueError("Invalid version string %r" % version)
+            raise ValueError('Invalid version string %r' % version)
         # If there no epoch ("1:..."), then the upstream version can not
         # contain a :.
-        if m.group("epoch") is None and ":" in m.group("upstream_version"):
-            raise ValueError("Invalid version string %r" % version)
+        if m.group('epoch') is None and ':' in m.group('upstream_version'):
+            raise ValueError('Invalid version string %r' % version)
 
         # pylint: disable=attribute-defined-outside-init
         self.__full_version = version
-        self.__epoch = m.group("epoch")
-        self.__upstream_version = m.group("upstream_version")
-        self.__debian_revision = m.group("debian_revision")
+        self.__epoch = m.group('epoch')
+        self.__upstream_version = m.group('upstream_version')
+        self.__debian_revision = m.group('debian_revision')
 
     # -------------------------------------------------------------------------
     def __setattr__(self, attr, value):
         """Override attribute setter."""
         # type: (str, Optional[Text]) -> None
         if attr not in self.magic_attrs:
             super(BaseVersion, self).__setattr__(attr, value)
             return
 
         # For compatibility with the old changelog.Version class
-        if attr == "debian_version":
-            attr = "debian_revision"
+        if attr == 'debian_version':
+            attr = 'debian_revision'
 
-        if attr == "full_version":
+        if attr == 'full_version':
             self._set_full_version(str(value))
         else:
             if value is not None:
                 value = str(value)
-            private = "_BaseVersion__%s" % attr
+            private = '_BaseVersion__%s' % attr
             old_value = getattr(self, private)
             setattr(self, private, value)
             try:
                 self._update_full_version()
             except ValueError:
                 # Don't leave it in an invalid state
                 setattr(self, private, old_value)
                 self._update_full_version()
-                raise ValueError("Setting %s to %r results in invalid version"
+                raise ValueError('Setting %s to %r results in invalid version'
                                  % (attr, value))
 
     # -------------------------------------------------------------------------
     def __getattr__(self, attr):
         """Override attribute getter."""
         # type: (str) -> Optional[str]
         if attr not in self.magic_attrs:
             return super(BaseVersion, self).__getattribute__(attr)
 
         # For compatibility with the old changelog.Version class
-        if attr == "debian_version":
-            attr = "debian_revision"
+        if attr == 'debian_version':
+            attr = 'debian_revision'
 
-        private = "_BaseVersion__%s" % attr
+        private = '_BaseVersion__%s' % attr
         return getattr(self, private)
 
     # -------------------------------------------------------------------------
     def _update_full_version(self):
         # type: () -> None
-        version = ""
+        version = ''
         if self.__epoch is not None:
-            version += self.__epoch + ":"
+            version += self.__epoch + ':'
         version += self.__upstream_version
         if self.__debian_revision:
-            version += "-" + self.__debian_revision
+            version += '-' + self.__debian_revision
         self.full_version = version
 
     # -------------------------------------------------------------------------
     def __str__(self):
         """Typecast into str."""
         # type: () -> str
         return self.full_version
@@ -222,18 +221,18 @@
 
 # =============================================================================
 # NativeVersion based on the DpkgVersion class by Raphael Hertzog in
 # svn://svn.debian.org/qa/trunk/pts/www/bin/common.py r2361
 class Version(BaseVersion):
     """Represents a Debian package version, with native Python comparison."""
 
-    re_all_digits_or_not = re.compile(r"\d+|\D+")
-    re_digits = re.compile(r"\d+")
-    re_digit = re.compile(r"\d")
-    re_alpha = re.compile("[A-Za-z]")
+    re_all_digits_or_not = re.compile(r'\d+|\D+')
+    re_digits = re.compile(r'\d+')
+    re_digit = re.compile(r'\d')
+    re_alpha = re.compile('[A-Za-z]')
 
     # -------------------------------------------------------------------------
     def _compare(self, other):
         # type: (Any) -> int
         # Convert other into an instance of BaseVersion if it's not already.
         # (All we need is epoch, upstream_version, and debian_revision
         # attributes, which BaseVersion gives us.) Requires other's string
@@ -246,26 +245,26 @@
         if not isinstance(other, BaseVersion):
             try:
                 other = BaseVersion(str(other))
             except ValueError as e:
                 raise ValueError("Couldn't convert %r to BaseVersion: %s"
                                  % (other, e))
 
-        lepoch = int(self.epoch or "0")
-        repoch = int(other.epoch or "0")
+        lepoch = int(self.epoch or '0')
+        repoch = int(other.epoch or '0')
         if lepoch < repoch:
             return -1
         if lepoch > repoch:
             return 1
-        res = self._version_cmp_part(self.upstream_version or "0",
-                                     other.upstream_version or "0")
+        res = self._version_cmp_part(self.upstream_version or '0',
+                                     other.upstream_version or '0')
         if res != 0:
             return res
-        return self._version_cmp_part(self.debian_revision or "0",
-                                      other.debian_revision or "0")
+        return self._version_cmp_part(self.debian_revision or '0',
+                                      other.debian_revision or '0')
 
     # -------------------------------------------------------------------------
     @classmethod
     def _order(cls, x):
         # type: (str) -> int
         """Return an integer value for character x."""
         if x == '~':
@@ -298,16 +297,16 @@
     # -------------------------------------------------------------------------
     @classmethod
     def _version_cmp_part(cls, va, vb):
         # type: (str, str) -> int
         la = cls.re_all_digits_or_not.findall(va)
         lb = cls.re_all_digits_or_not.findall(vb)
         while la or lb:
-            a = "0"
-            b = "0"
+            a = '0'
+            b = '0'
             if la:
                 a = la.pop(0)
             if lb:
                 b = lb.pop(0)
             if cls.re_digits.match(a) and cls.re_digits.match(b):
                 aval = int(a)
                 bval = int(b)
```

### Comparing `fb_logging-0.5.5/lib/fb_logging/syslog_handler.py` & `fb_logging-0.6.0/lib/fb_logging/syslog_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,43 +3,42 @@
 """
 @summary: A wrapping logging handler for logging.handlers.SysLogHandler.
 
 It's intended to convert all log messages to utf-8.
 """
 
 # Standard modules
-import socket
-import sys
+import errno
 import os
+import socket
 import stat
-import errno
-
+import sys
 from logging.handlers import SYSLOG_UDP_PORT
 from logging.handlers import SysLogHandler
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 
 if sys.version_info[0] < 3:
-    raise RuntimeError("This module may only be used with Python > 3.1.")
+    raise RuntimeError('This module may only be used with Python > 3.1.')
 if sys.version_info[0] == 3 and sys.version_info[1] <= 1:
-    raise RuntimeError("This module may only be used with Python > 3.1")
+    raise RuntimeError('This module may only be used with Python > 3.1')
 
 
 # =============================================================================
 class FbSysLogHandler(SysLogHandler):
     """A wrapper logging handler for logging.handlers.SysLogHandler.
 
     It's intended to convert all log messages to utf-8.
     """
 
     def __init__(
         self, address=('localhost', SYSLOG_UDP_PORT),
             facility=SysLogHandler.LOG_USER,
             socktype=None,
-            encoding="utf-8"):
+            encoding='utf-8'):
         """Initialize the FbSysLogHandler.
 
         To log to a local syslogd, `FbSysLogHandler(address="/dev/log")`
         may be used.
 
         If facility is not specified, LOG_USER is used.
 
@@ -60,18 +59,18 @@
 
         if isinstance(address, str):
             if not os.path.exists(address):
                 raise OSError(errno.ENOENT, "File doesn't exists", address)
             mode = os.stat(address).st_mode
             if not stat.S_ISSOCK(mode):
                 raise OSError(
-                    errno.EPERM, "File is not a UNIX socket file", address)
+                    errno.EPERM, 'File is not a UNIX socket file', address)
             if not os.access(address, os.W_OK):
                 raise OSError(
-                    errno.EPERM, "No write access to socket", address)
+                    errno.EPERM, 'No write access to socket', address)
 
             do_ux_socket = True
 
         if do_ux_socket:
             SysLogHandler.__init__(self, address, facility, None)
         else:
             SysLogHandler.__init__(self, address, facility, socktype)
@@ -121,14 +120,14 @@
             msg = msg.decode(self.encoding)
             record.msg = msg
 
         SysLogHandler.emit(self, record)
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_logging-0.5.5/lib/fb_logging/unix_handler.py` & `fb_logging-0.6.0/lib/fb_logging/unix_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 @summary: An additional logging handler for the common logging framework.
 
 It's intended to combine it with syslog.
 """
 
 # Standard modules
 import logging
-import syslog
 import os.path
 import sys
-
+import syslog
 from numbers import Number
 
 # Third party modules
 
 # Own modules
 
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 
 if sys.version_info[0] < 3:
-    raise RuntimeError("This module may only be used with Python > 3.1.")
+    raise RuntimeError('This module may only be used with Python > 3.1.')
 
 
 # =============================================================================
 class UnixSyslogHandler(logging.Handler):
     """A handler class which sends formatted logging records over the C API."""
 
     # from <linux/sys/syslog.h>:
@@ -75,77 +74,77 @@
     LOG_PID = syslog.LOG_PID        # log the pid with each message
     LOG_CONS = syslog.LOG_CONS      # log on the console if errors in sending
     LOG_NDELAY = syslog.LOG_NDELAY  # don't delay open
     # if forking to log on console, don't wait()
     LOG_NOWAIT = syslog.LOG_NOWAIT
 
     priority_names = {
-        "alert": LOG_ALERT,
-        "crit": LOG_CRIT,
-        "debug": LOG_DEBUG,
-        "emerg": LOG_EMERG,
-        "err": LOG_ERR,
-        "info": LOG_INFO,
-        "notice": LOG_NOTICE,
-        "warning": LOG_WARNING,
+        'alert': LOG_ALERT,
+        'crit': LOG_CRIT,
+        'debug': LOG_DEBUG,
+        'emerg': LOG_EMERG,
+        'err': LOG_ERR,
+        'info': LOG_INFO,
+        'notice': LOG_NOTICE,
+        'warning': LOG_WARNING,
     }
 
     priority_ids = {}
     for key in list(priority_names.keys()):
         val = priority_names[key]
         if val not in priority_ids:
             priority_ids[val] = key
 
     # Deprecated priority names
-    priority_names["error"] = LOG_ERR
-    priority_names["panic"] = LOG_EMERG
-    priority_names["critical"] = LOG_CRIT
-    priority_names["warn"] = LOG_WARNING
+    priority_names['error'] = LOG_ERR
+    priority_names['panic'] = LOG_EMERG
+    priority_names['critical'] = LOG_CRIT
+    priority_names['warn'] = LOG_WARNING
 
     facility_names = {
-        "auth": LOG_AUTH,
-        "authpriv": LOG_AUTHPRIV,
-        "cron": LOG_CRON,
-        "daemon": LOG_DAEMON,
-        "ftp": LOG_FTP,
-        "kern": LOG_KERN,
-        "lpr": LOG_LPR,
-        "mail": LOG_MAIL,
-        "news": LOG_NEWS,
-        "user": LOG_USER,
-        "uucp": LOG_UUCP,
-        "local0": LOG_LOCAL0,
-        "local1": LOG_LOCAL1,
-        "local2": LOG_LOCAL2,
-        "local3": LOG_LOCAL3,
-        "local4": LOG_LOCAL4,
-        "local5": LOG_LOCAL5,
-        "local6": LOG_LOCAL6,
-        "local7": LOG_LOCAL7,
+        'auth': LOG_AUTH,
+        'authpriv': LOG_AUTHPRIV,
+        'cron': LOG_CRON,
+        'daemon': LOG_DAEMON,
+        'ftp': LOG_FTP,
+        'kern': LOG_KERN,
+        'lpr': LOG_LPR,
+        'mail': LOG_MAIL,
+        'news': LOG_NEWS,
+        'user': LOG_USER,
+        'uucp': LOG_UUCP,
+        'local0': LOG_LOCAL0,
+        'local1': LOG_LOCAL1,
+        'local2': LOG_LOCAL2,
+        'local3': LOG_LOCAL3,
+        'local4': LOG_LOCAL4,
+        'local5': LOG_LOCAL5,
+        'local6': LOG_LOCAL6,
+        'local7': LOG_LOCAL7,
     }
 
     facility_ids = {}
     for key in list(facility_names.keys()):
         val = facility_names[key]
         if val not in facility_ids:
             facility_ids[val] = key
 
     # Deprecated facility names
-    facility_names["security"] = LOG_AUTH
+    facility_names['security'] = LOG_AUTH
 
     priority_map = {
-        "DEBUG": "debug",
-        "INFO": "info",
-        "WARNING": "warning",
-        "ERROR": "err",
-        "CRITICAL": "crit"
+        'DEBUG': 'debug',
+        'INFO': 'info',
+        'WARNING': 'warning',
+        'ERROR': 'err',
+        'CRITICAL': 'crit'
     }
 
     # -------------------------------------------------------------------------
-    def __init__(self, ident=None, logopt=None, facility=None, encoding="utf-8"):
+    def __init__(self, ident=None, logopt=None, facility=None, encoding='utf-8'):
         """Initialize a handler.
 
         @param ident: Identifier of the syslog message, uses basename
                       or current running program, if not given
         @type ident: str
         @param logopt: options for syslog.openlog(), see there for possible
                        values (linked with a binary or). Uses LOG_PID,
@@ -216,21 +215,21 @@
         if self.opened:
             return
 
         used_facility = 'user'
         if isinstance(value, Number):
             v = int(value)
             if v not in self.facility_ids:
-                msg = "Invalid value {!r} for facility.".format(value)
+                msg = 'Invalid value {!r} for facility.'.format(value)
                 raise ValueError(msg)
             used_facility = self.facility_ids[v]
         else:
             used_facility = str(value).lower()
             if used_facility not in self.facility_names:
-                msg = "Invalid value {!r} for facility.".format(value)
+                msg = 'Invalid value {!r} for facility.'.format(value)
                 raise ValueError(msg)
         self._facility = used_facility
 
     # -------------------------------------------------------------------------
     @property
     def facility_id(self):
         """Return the numeric value of the syslog facility."""
@@ -256,15 +255,15 @@
 
         @param level_name: the level name, which should be mapped
         @type level_name: str
 
         @return: the numeric logging level code
         @rtype: str
         """
-        return self.priority_map.get(level_name.upper(), "warning")
+        return self.priority_map.get(level_name.upper(), 'warning')
 
     # -------------------------------------------------------------------------
     def emit(self, record):
         """Emit a record.
 
         The record is formatted, and then sent to the syslog server. If
         exception information is present, it is NOT sent to the server.
@@ -284,14 +283,14 @@
         except (KeyboardInterrupt, SystemExit):
             raise
         except Exception:
             self.handleError(record)
 
 
 # =============================================================================
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     pass
 
 # =============================================================================
 
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4
```

### Comparing `fb_logging-0.5.5/lib/fb_logging.egg-info/PKG-INFO` & `fb_logging-0.6.0/lib/fb_logging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-logging
-Version: 0.5.5
+Version: 0.6.0
 Summary: Python modules to extend the logging mechanism in Python.
 Home-page: https://github.com/fbrehm/fb-logging
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fb_logging-0.5.5/setup.cfg` & `fb_logging-0.6.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -37,13 +37,13 @@
 
 [pep8]
 max-line-length = 99
 
 [flake8]
 max-line-length = 99
 max-complexity = 20
-ignore = E226,E302,E41,E402,W503
+ignore = E226,E302,E41,E402,W503,B902
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fb_logging-0.5.5/setup.py` & `fb_logging-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 @contact: frank@brehm-online.com
 @copyright: © 2021 by Frank Brehm, Berlin
 @license: LGPL3+
 """
 
 from __future__ import print_function
 
+import datetime
 import os
-import sys
-import re
 import pprint
-import datetime
+import re
+import sys
 import textwrap
-
 from pathlib import Path
 
 # Third party modules
-from setuptools import setup
 
 # own modules:
 __module_name__ = 'fb_logging'
 __setup_script__ = Path(__file__).resolve()
 __base_dir__ = __setup_script__.parent
 __bin_dir__ = __base_dir__ / 'bin'
 __lib_dir__ = __base_dir__ / 'lib'
@@ -50,15 +48,17 @@
 # print("Paths:\n{}".format(pp(PATHS)))
 
 if os.path.exists(__module_dir__) and os.path.isfile(__init_py__):
     sys.path.insert(0, os.path.abspath(__lib_dir__))
 
 import fb_logging
 
-ENCODING = "utf-8"
+from setuptools import setup
+
+ENCODING = 'utf-8'
 
 __packet_version__ = fb_logging.__version__
 
 __packet_name__ = __module_name__
 __debian_pkg_name__ = __module_name__.replace('_', '-')
 
 __author__ = 'Frank Brehm'
```

### Comparing `fb_logging-0.5.5/test/general.py` & `fb_logging-0.6.0/test/general.py`

 * *Files identical despite different names*

### Comparing `fb_logging-0.5.5/test/test_colored.py` & `fb_logging-0.6.0/test/test_colored.py`

 * *Files identical despite different names*

### Comparing `fb_logging-0.5.5/test/test_fb_logging.py` & `fb_logging-0.6.0/test/test_fb_logging.py`

 * *Files identical despite different names*

### Comparing `fb_logging-0.5.5/test/test_syslog.py` & `fb_logging-0.6.0/test/test_syslog.py`

 * *Files identical despite different names*


# Comparing `tmp/coverxygen-1.7.0.tar.gz` & `tmp/coverxygen-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverxygen-1.7.0.tar", last modified: Tue Nov 23 15:29:03 2021, max compression
+gzip compressed data, was "coverxygen-1.8.0.tar", last modified: Sun Jun 18 19:44:52 2023, max compression
```

## Comparing `coverxygen-1.7.0.tar` & `coverxygen-1.8.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 psyco     (1000) psyco     (1000)        0 2021-11-23 15:29:03.647622 coverxygen-1.7.0/
--rw-rw-r--   0 psyco     (1000) psyco     (1000)      674 2021-11-23 15:29:03.647622 coverxygen-1.7.0/PKG-INFO
--rw-rw-r--   0 psyco     (1000) psyco     (1000)     6819 2021-11-23 15:13:28.000000 coverxygen-1.7.0/README.md
-drwxrwxr-x   0 psyco     (1000) psyco     (1000)        0 2021-11-23 15:29:03.647622 coverxygen-1.7.0/coverxygen/
--rw-rw-r--   0 psyco     (1000) psyco     (1000)    15461 2021-11-23 15:13:28.000000 coverxygen-1.7.0/coverxygen/__init__.py
--rw-rw-r--   0 psyco     (1000) psyco     (1000)     7379 2021-11-23 13:39:27.000000 coverxygen-1.7.0/coverxygen/__main__.py
-drwxrwxr-x   0 psyco     (1000) psyco     (1000)        0 2021-11-23 15:29:03.647622 coverxygen-1.7.0/coverxygen.egg-info/
--rw-r--r--   0 psyco     (1000) psyco     (1000)      674 2021-11-23 15:29:03.000000 coverxygen-1.7.0/coverxygen.egg-info/PKG-INFO
--rw-r--r--   0 psyco     (1000) psyco     (1000)      210 2021-11-23 15:29:03.000000 coverxygen-1.7.0/coverxygen.egg-info/SOURCES.txt
--rw-r--r--   0 psyco     (1000) psyco     (1000)        1 2021-11-23 15:29:03.000000 coverxygen-1.7.0/coverxygen.egg-info/dependency_links.txt
--rw-r--r--   0 psyco     (1000) psyco     (1000)       11 2021-11-23 15:29:03.000000 coverxygen-1.7.0/coverxygen.egg-info/top_level.txt
--rw-rw-r--   0 psyco     (1000) psyco     (1000)       79 2021-11-23 15:29:03.647622 coverxygen-1.7.0/setup.cfg
--rwxrwxr-x   0 psyco     (1000) psyco     (1000)      819 2019-07-04 13:23:55.000000 coverxygen-1.7.0/setup.py
+drwxrwxr-x   0 psyco     (1000) psyco     (1000)        0 2023-06-18 19:44:52.389773 coverxygen-1.8.0/
+-rw-rw-r--   0 psyco     (1000) psyco     (1000)    35141 2016-08-15 08:31:33.000000 coverxygen-1.8.0/LICENSE
+-rw-rw-r--   0 psyco     (1000) psyco     (1000)      685 2023-06-18 19:44:52.389773 coverxygen-1.8.0/PKG-INFO
+-rw-rw-r--   0 psyco     (1000) psyco     (1000)     7015 2023-06-18 16:41:43.000000 coverxygen-1.8.0/README.md
+drwxrwxr-x   0 psyco     (1000) psyco     (1000)        0 2023-06-18 19:44:52.389773 coverxygen-1.8.0/coverxygen/
+-rw-rw-r--   0 psyco     (1000) psyco     (1000)    17019 2023-06-18 16:40:01.000000 coverxygen-1.8.0/coverxygen/__init__.py
+-rw-rw-r--   0 psyco     (1000) psyco     (1000)     7497 2023-06-18 16:40:01.000000 coverxygen-1.8.0/coverxygen/__main__.py
+drwxrwxr-x   0 psyco     (1000) psyco     (1000)        0 2023-06-18 19:44:52.389773 coverxygen-1.8.0/coverxygen.egg-info/
+-rw-r--r--   0 psyco     (1000) psyco     (1000)      685 2023-06-18 19:44:52.000000 coverxygen-1.8.0/coverxygen.egg-info/PKG-INFO
+-rw-r--r--   0 psyco     (1000) psyco     (1000)      218 2023-06-18 19:44:52.000000 coverxygen-1.8.0/coverxygen.egg-info/SOURCES.txt
+-rw-r--r--   0 psyco     (1000) psyco     (1000)        1 2023-06-18 19:44:52.000000 coverxygen-1.8.0/coverxygen.egg-info/dependency_links.txt
+-rw-r--r--   0 psyco     (1000) psyco     (1000)       11 2023-06-18 19:44:52.000000 coverxygen-1.8.0/coverxygen.egg-info/top_level.txt
+-rw-rw-r--   0 psyco     (1000) psyco     (1000)       79 2023-06-18 19:44:52.389773 coverxygen-1.8.0/setup.cfg
+-rwxrwxr-x   0 psyco     (1000) psyco     (1000)      819 2016-12-27 22:14:58.000000 coverxygen-1.8.0/setup.py
```

### Comparing `coverxygen-1.7.0/PKG-INFO` & `coverxygen-1.8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: coverxygen
-Version: 1.7.0
+Version: 1.8.0
 Summary: Generate doxygen's documentation coverage report
 Home-page: https://github.com/psycofdj/coverxygen
 Author: Xavier MARCELET
 Author-email: xavier@marcelet.com
 License: UNKNOWN
-Download-URL: https://github.com/psycofdj/coverxygen/tarball/1.7.0
-Description: UNKNOWN
+Download-URL: https://github.com/psycofdj/coverxygen/tarball/1.8.0
 Keywords: doxygen,coverage,python
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `coverxygen-1.7.0/README.md` & `coverxygen-1.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -84,23 +84,24 @@
   --src-dir SRC_DIR  root source directory used to match prefix for relative path generated files
 
 optional arguments:
   -h, --help         show this help message and exit
   --version          print version and exit
   --verbose          enabled verbose output
   --json             (deprecated) same as --format json-legacy
-  --format FORMAT    output file format : 
-                     lcov         : lcov compatible format (default)
-                     json-v3      : json format which includes summary information
-                     json-v2      : simpler json format
-                     json-v1      : legacy json format
-                     json         : (deprecated) same as json-v2
-                     json-legacy  : (deprecated) same as json-v1
-                     json-summary : summary in json format
-                     summary      : textual summary table format
+  --format FORMAT    output file format :
+                     lcov             : lcov compatible format (default)
+                     json-v3          : json format which includes summary information
+                     json-v2          : simpler json format
+                     json-v1          : legacy json format
+                     json             : (deprecated) same as json-v2
+                     json-legacy      : (deprecated) same as json-v1
+                     json-summary     : summary in json format
+                     markdown-summary : ummary in markdown table format
+                     summary          : textual summary table format
   --prefix PREFIX    keep only file matching given path prefix
   --exclude EXCLUDE  exclude files whose absolute path matches a regular expression;
                      this option can be given multiple times
   --include INCLUDE  include files whose absolute path matches a regular expression
                      even if they also match an exclude filter (see --exclude) or if they
                      are not matching the patch prefix (see --prefix);
                      this option can be given multiple times
@@ -180,14 +181,15 @@
 Special thanks to Alvaro Lopez Ortega <[alvaro@gnu.org](mailto:alvaro@gnu.org)> who found a smart and efficient solution to retrieve doxygen informations from the generated xml.
 
 You can find his work at [alobbs/doxy-coverage](https://github.com/alobbs/doxy-coverage)
 
 ## Hall of Fame
 
 - [j-ulrich](https://github.com/j-ulrich) for his many contributions
+- [antoniovazquezblanco](https://github.com/antoniovazquezblanco) for his many contributions
 
 
 # Project status
 
 Unstable but usable.
 [![PyPI version](https://badge.fury.io/py/coverxygen.svg)](https://badge.fury.io/py/coverxygen)
```

### Comparing `coverxygen-1.7.0/coverxygen/__init__.py` & `coverxygen-1.8.0/coverxygen/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import xml.etree.ElementTree as ET
 from functools import reduce
 
 #------------------------------------------------------------------------------
 
 __author__       = "Xavier MARCELET <xavier@marcelet.com>"
 __copyright__    = "Copyright (C) 2016 Xavier MARCELET"
-__version__      = "1.7.0"
+__version__      = "1.8.0"
 __description__  = "Generate doxygen's documentation coverage report"
 __url__          = "https://github.com/psycofdj/coverxygen"
 __download_url__ = "https://github.com/psycofdj/coverxygen/tarball/%s" % __version__
 __keywords__     = ['doxygen', 'coverage', 'python']
 __classifiers__  = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
@@ -263,14 +263,16 @@
 
   def output_results(self, p_symbols):
     l_outStream = self.output_get_stream(self.m_output)
     if self.m_format == "summary":
       self.output_print_summary(l_outStream, p_symbols)
     elif self.m_format == "json-summary":
       self.output_print_json_summary(l_outStream, p_symbols)
+    elif self.m_format == "markdown-summary":
+      self.output_print_markdown_summary(l_outStream, p_symbols)
     else:
       l_symbolsByFile = Coverxygen.group_symbols_by_file(p_symbols)
       if self.m_format == "json-v3":
         self.output_print_json_v3(l_outStream, p_symbols, l_symbolsByFile)
       elif self.m_format == "json-v2":
         self.output_print_json_v2(l_outStream, l_symbolsByFile)
       elif self.m_format == "json-v1":
@@ -413,26 +415,52 @@
   @staticmethod
   def determine_first_column_width(p_symbolsKindCountsList):
     l_kindStringLengths = map(lambda c_symbolKindCount: len(c_symbolKindCount["kind"]), p_symbolsKindCountsList)
     l_longestKindStringLength = max(l_kindStringLengths, default=0)
     return l_longestKindStringLength
 
   @staticmethod
+  def get_value_summary_value(count, total):
+    percentage = 0 if total == 0 else (count / total) * 100.0
+    # Format: 100.0% (999/999)
+    return f'{percentage:5.1f}% ({count}/{total})'
+
+  @staticmethod
   def print_summary_line(p_stream, p_header, p_headerWidth, p_count, p_total):
-    l_percentage = 0 if p_total == 0 else (p_count / p_total) * 100.0
-    p_stream.write("%s: %5.1f%% (%d/%d)\n" % (("%%-%ds" % (p_headerWidth)) % p_header,
-                                                l_percentage, p_count, p_total))
+    value_string = Coverxygen.get_value_summary_value(p_count, p_total)
+    p_stream.write("%s: %s\n" % (("%%-%ds" % (p_headerWidth)) % p_header, value_string))
 
   @staticmethod
   def output_print_summary(p_stream, p_symbols):
     l_summary = Coverxygen.create_summary(p_symbols)
     l_symbolKindCountsList = Coverxygen.symbol_kind_counts_dict_to_list(l_summary["kinds"])
     l_totalCounts = l_summary["total"]
     l_firstColumnWidth = Coverxygen.determine_first_column_width(l_symbolKindCountsList)
     for c_symbolKindCount in l_symbolKindCountsList:
       Coverxygen.print_summary_line(p_stream, c_symbolKindCount["kind"], l_firstColumnWidth, c_symbolKindCount["documented_symbol_count"], c_symbolKindCount["symbol_count"])
     p_stream.write("%s\n" % ("-" * 35))
     Coverxygen.print_summary_line(p_stream, "Total", l_firstColumnWidth, l_totalCounts["documented_symbol_count"], l_totalCounts["symbol_count"])
 
+  @staticmethod
+  def output_print_markdown_summary(stream, symbols):
+    summary = Coverxygen.create_summary(symbols)
+    symbol_kind_counts_list = Coverxygen.symbol_kind_counts_dict_to_list(summary["kinds"])
+    symbol_kind_counts_list.append({
+        "kind": "Total",
+        "documented_symbol_count": summary["total"]["documented_symbol_count"],
+        "symbol_count": summary["total"]["symbol_count"]
+      })
+    # Append a value column in string format
+    second_column_width = 0
+    for symbol_kind_count in symbol_kind_counts_list:
+      symbol_kind_count['value_string'] = Coverxygen.get_value_summary_value(symbol_kind_count["documented_symbol_count"], symbol_kind_count["symbol_count"])
+      second_column_width = max(second_column_width, len(symbol_kind_count['value_string']))
+    # Render the table
+    first_column_width = max(Coverxygen.determine_first_column_width(symbol_kind_counts_list), 8)
+    stream.write(f'| {"Element".ljust(first_column_width)} | {"Value".ljust(second_column_width)} |\n')
+    stream.write(f'|{"-".ljust(first_column_width+2)}|{" ".ljust(second_column_width+2)}|\n')
+    for symbol_kind_count in symbol_kind_counts_list:
+      stream.write(f'| {symbol_kind_count["kind"].ljust(first_column_width)} | {symbol_kind_count["value_string"].ljust(second_column_width)} |\n')
+
 # Local Variables:
 # ispell-local-dictionary: "en"
 # End:
```

### Comparing `coverxygen-1.7.0/coverxygen/__main__.py` & `coverxygen-1.8.0/coverxygen/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,22 +30,23 @@
   l_optionalArgs.add_argument("--json",
                               action="store_true",
                               help="(deprecated) same as --format json-legacy",
                               default=None)
   l_optionalArgs.add_argument("--format",
                               action="store",
                               help="output file format :\n"
-                              "lcov         : lcov compatible format (default)\n"
-                              "json-v3      : json format which includes summary information\n"
-                              "json-v2      : simpler json format\n"
-                              "json-v1      : legacy json format\n"
-                              "json         : (deprecated) same as json-v2\n"
-                              "json-legacy  : (deprecated) same as json-v1\n"
-                              "json-summary : summary in json format\n"
-                              "summary      : textual summary table format\n",
+                              "lcov             : lcov compatible format (default)\n"
+                              "json-v3          : json format which includes summary information\n"
+                              "json-v2          : simpler json format\n"
+                              "json-v1          : legacy json format\n"
+                              "json             : (deprecated) same as json-v2\n"
+                              "json-legacy      : (deprecated) same as json-v1\n"
+                              "json-summary     : summary in json format\n"
+                              "markdown-summary : summary in markdown table format\n"
+                              "summary          : textual summary table format\n",
                               default="lcov")
   l_optionalArgs.add_argument("--prefix",
                               action="store",
                               help ="keep only file matching given path prefix",
                               default=None)
   l_optionalArgs.add_argument("--exclude",
                               action="append",
```

### Comparing `coverxygen-1.7.0/coverxygen.egg-info/PKG-INFO` & `coverxygen-1.8.0/coverxygen.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: coverxygen
-Version: 1.7.0
+Version: 1.8.0
 Summary: Generate doxygen's documentation coverage report
 Home-page: https://github.com/psycofdj/coverxygen
 Author: Xavier MARCELET
 Author-email: xavier@marcelet.com
 License: UNKNOWN
-Download-URL: https://github.com/psycofdj/coverxygen/tarball/1.7.0
-Description: UNKNOWN
+Download-URL: https://github.com/psycofdj/coverxygen/tarball/1.8.0
 Keywords: doxygen,coverage,python
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `coverxygen-1.7.0/setup.py` & `coverxygen-1.8.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/toolstr-0.9.6.tar.gz` & `tmp/toolstr-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolstr-0.9.6.tar", last modified: Thu Jun 15 06:36:11 2023, max compression
+gzip compressed data, was "toolstr-0.9.7.tar", last modified: Sun Jun 18 01:48:58 2023, max compression
```

## Comparing `toolstr-0.9.6.tar` & `toolstr-0.9.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.6/.gitignore
--rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.6/LICENSE
--rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.6/README.md
--rw-r--r--   0        0        0      612 2023-05-09 04:42:34.474533 toolstr-0.9.6/pyproject.toml
--rw-r--r--   0        0        0      268 2023-06-15 06:35:44.903539 toolstr-0.9.6/toolstr/__init__.py
--rw-r--r--   0        0        0       28 2023-05-19 00:35:26.933408 toolstr-0.9.6/toolstr/buffers/__init__.py
--rw-r--r--   0        0        0      592 2023-06-14 01:27:06.061946 toolstr-0.9.6/toolstr/buffers/stdout_utils.py
--rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.6/toolstr/charts/README.md
--rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.6/toolstr/charts/__init__.py
--rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.6/toolstr/charts/braille_utils.py
--rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.6/toolstr/charts/char_dicts.py
--rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.6/toolstr/charts/grid_utils.py
--rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.6/toolstr/charts/line_utils.py
--rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.6/toolstr/charts/plot_utils.py
--rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.6/toolstr/charts/raster_utils.py
--rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.6/toolstr/charts/render_utils.py
--rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.6/toolstr/charts/sextant_utils.py
--rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.6/toolstr/formats/__init__.py
--rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.6/toolstr/formats/bullet_formats.py
--rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.6/toolstr/formats/column_formats.py
--rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.6/toolstr/formats/datatype_formats.py
--rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.6/toolstr/formats/positional_formats.py
--rw-r--r--   0        0        0     2191 2023-06-03 05:09:21.785742 toolstr-0.9.6/toolstr/formats/rich_formats.py
--rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.6/toolstr/formats/template_formats.py
--rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.6/toolstr/outlines/__init__.py
--rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.6/toolstr/outlines/outline_chars.py
--rw-r--r--   0        0        0     7359 2023-05-08 16:02:35.196513 toolstr-0.9.6/toolstr/outlines/outline_printing.py
--rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.6/toolstr/py.typed
--rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.6/toolstr/spec.py
--rw-r--r--   0        0        0       58 2023-06-13 22:26:15.086201 toolstr-0.9.6/toolstr/summaries/__init__.py
--rw-r--r--   0        0        0     6145 2023-06-15 06:35:03.583900 toolstr-0.9.6/toolstr/summaries/nested_summary.py
--rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.6/toolstr/summaries/set_summary.py
--rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.6/toolstr/tables/__init__.py
--rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.6/toolstr/tables/multiline_tables.py
--rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.6/toolstr/tables/table_adapters.py
--rw-r--r--   0        0        0    33536 2023-06-14 01:33:04.639306 toolstr-0.9.6/toolstr/tables/table_utils.py
--rw-r--r--   0        0        0     8722 1970-01-01 00:00:00.000000 toolstr-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-01-01 01:26:00.835967 toolstr-0.9.7/.gitignore
+-rw-r--r--   0        0        0     1084 2022-12-09 18:24:40.520680 toolstr-0.9.7/LICENSE
+-rw-r--r--   0        0        0     8107 2022-12-09 18:24:40.520919 toolstr-0.9.7/README.md
+-rw-r--r--   0        0        0      612 2023-05-09 04:42:34.474533 toolstr-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-06-18 01:48:22.354181 toolstr-0.9.7/toolstr/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-19 00:35:26.933408 toolstr-0.9.7/toolstr/buffers/__init__.py
+-rw-r--r--   0        0        0      592 2023-06-14 01:27:06.061946 toolstr-0.9.7/toolstr/buffers/stdout_utils.py
+-rw-r--r--   0        0        0      475 2022-12-09 18:24:40.521992 toolstr-0.9.7/toolstr/charts/README.md
+-rw-r--r--   0        0        0      134 2022-12-09 18:24:40.522217 toolstr-0.9.7/toolstr/charts/__init__.py
+-rw-r--r--   0        0        0    12629 2022-12-09 18:24:40.522525 toolstr-0.9.7/toolstr/charts/braille_utils.py
+-rw-r--r--   0        0        0     2412 2022-12-09 18:24:40.522810 toolstr-0.9.7/toolstr/charts/char_dicts.py
+-rw-r--r--   0        0        0     3763 2022-12-09 18:24:40.523072 toolstr-0.9.7/toolstr/charts/grid_utils.py
+-rw-r--r--   0        0        0     2247 2022-12-09 18:24:40.523333 toolstr-0.9.7/toolstr/charts/line_utils.py
+-rw-r--r--   0        0        0     3682 2022-12-12 20:14:13.660011 toolstr-0.9.7/toolstr/charts/plot_utils.py
+-rw-r--r--   0        0        0     7038 2022-12-09 18:24:40.524040 toolstr-0.9.7/toolstr/charts/raster_utils.py
+-rw-r--r--   0        0        0     8161 2022-12-12 20:13:58.305050 toolstr-0.9.7/toolstr/charts/render_utils.py
+-rw-r--r--   0        0        0     2523 2022-12-09 18:24:40.524620 toolstr-0.9.7/toolstr/charts/sextant_utils.py
+-rw-r--r--   0        0        0      186 2023-04-24 03:18:32.307974 toolstr-0.9.7/toolstr/formats/__init__.py
+-rw-r--r--   0        0        0     1964 2022-12-09 18:24:40.525217 toolstr-0.9.7/toolstr/formats/bullet_formats.py
+-rw-r--r--   0        0        0     1997 2022-12-09 18:24:40.525609 toolstr-0.9.7/toolstr/formats/column_formats.py
+-rw-r--r--   0        0        0     7280 2023-03-27 19:55:46.509117 toolstr-0.9.7/toolstr/formats/datatype_formats.py
+-rw-r--r--   0        0        0     3143 2022-12-12 07:53:13.190851 toolstr-0.9.7/toolstr/formats/positional_formats.py
+-rw-r--r--   0        0        0     2191 2023-06-03 05:09:21.785742 toolstr-0.9.7/toolstr/formats/rich_formats.py
+-rw-r--r--   0        0        0     3167 2023-04-24 06:16:05.352543 toolstr-0.9.7/toolstr/formats/template_formats.py
+-rw-r--r--   0        0        0       61 2022-12-09 18:24:40.526678 toolstr-0.9.7/toolstr/outlines/__init__.py
+-rw-r--r--   0        0        0     9083 2022-12-09 18:24:40.526924 toolstr-0.9.7/toolstr/outlines/outline_chars.py
+-rw-r--r--   0        0        0     7359 2023-05-08 16:02:35.196513 toolstr-0.9.7/toolstr/outlines/outline_printing.py
+-rw-r--r--   0        0        0        0 2022-12-09 18:24:40.527329 toolstr-0.9.7/toolstr/py.typed
+-rw-r--r--   0        0        0     2402 2022-12-12 03:10:49.782218 toolstr-0.9.7/toolstr/spec.py
+-rw-r--r--   0        0        0       58 2023-06-13 22:26:15.086201 toolstr-0.9.7/toolstr/summaries/__init__.py
+-rw-r--r--   0        0        0     6667 2023-06-18 01:46:30.177013 toolstr-0.9.7/toolstr/summaries/nested_summary.py
+-rw-r--r--   0        0        0     6158 2023-04-05 16:58:38.202042 toolstr-0.9.7/toolstr/summaries/set_summary.py
+-rw-r--r--   0        0        0       89 2022-12-09 18:24:40.527921 toolstr-0.9.7/toolstr/tables/__init__.py
+-rw-r--r--   0        0        0     5083 2022-12-09 18:24:40.528163 toolstr-0.9.7/toolstr/tables/multiline_tables.py
+-rw-r--r--   0        0        0     2983 2023-04-24 06:16:44.834292 toolstr-0.9.7/toolstr/tables/table_adapters.py
+-rw-r--r--   0        0        0    33536 2023-06-14 01:33:04.639306 toolstr-0.9.7/toolstr/tables/table_utils.py
+-rw-r--r--   0        0        0     8722 1970-01-01 00:00:00.000000 toolstr-0.9.7/PKG-INFO
```

### Comparing `toolstr-0.9.6/LICENSE` & `toolstr-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/README.md` & `toolstr-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/pyproject.toml` & `toolstr-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/buffers/stdout_utils.py` & `toolstr-0.9.7/toolstr/buffers/stdout_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/charts/braille_utils.py` & `toolstr-0.9.7/toolstr/charts/braille_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/charts/char_dicts.py` & `toolstr-0.9.7/toolstr/charts/char_dicts.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/charts/grid_utils.py` & `toolstr-0.9.7/toolstr/charts/grid_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/charts/line_utils.py` & `toolstr-0.9.7/toolstr/charts/line_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/charts/plot_utils.py` & `toolstr-0.9.7/toolstr/charts/plot_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/charts/raster_utils.py` & `toolstr-0.9.7/toolstr/charts/raster_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/charts/render_utils.py` & `toolstr-0.9.7/toolstr/charts/render_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/charts/sextant_utils.py` & `toolstr-0.9.7/toolstr/charts/sextant_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/formats/bullet_formats.py` & `toolstr-0.9.7/toolstr/formats/bullet_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/formats/column_formats.py` & `toolstr-0.9.7/toolstr/formats/column_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/formats/datatype_formats.py` & `toolstr-0.9.7/toolstr/formats/datatype_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/formats/positional_formats.py` & `toolstr-0.9.7/toolstr/formats/positional_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/formats/rich_formats.py` & `toolstr-0.9.7/toolstr/formats/rich_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/formats/template_formats.py` & `toolstr-0.9.7/toolstr/formats/template_formats.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/outlines/outline_chars.py` & `toolstr-0.9.7/toolstr/outlines/outline_chars.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/outlines/outline_printing.py` & `toolstr-0.9.7/toolstr/outlines/outline_printing.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/spec.py` & `toolstr-0.9.7/toolstr/spec.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/summaries/nested_summary.py` & `toolstr-0.9.7/toolstr/summaries/nested_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,24 +111,27 @@
                 rhs_value = ''
         row = [diff['type'], index, lhs_value, rhs_value]
         rows.append(row)
 
     # convert to table
     if styles is None:
         styles = {}
-    return toolstr.print_table(  # type: ignore
+    return toolstr.print_multiline_table(  # type: ignore
         rows=rows,
         labels=['type', 'index', lhs_name, rhs_name],
-        column_justify={'index': 'left'},
+        column_justify={'index': 'left', lhs_name: 'left', rhs_name: 'left'},
+        label_justify='left',
+        vertical_justify='top',
         return_str=True,
-        max_column_widths=[6, 30, 30, 30],
+        max_column_widths=[6, 30, 32, 32],
         compact=3,
         label_style=styles.get('metavar'),
         border=styles.get('content'),
         indent=indent,
+        separate_all_rows=False,
     )
 
 
 #
 # # gather nested diffs
 #
 
@@ -149,15 +152,26 @@
         rhs_type = type(rhs).__name__
         diff = {'type': 'type', 'index': [], 'lhs': lhs_type, 'rhs': rhs_type}
         return [diff]
     elif isinstance(lhs, dict):
         return get_dict_diffs(lhs, rhs)
     elif isinstance(lhs, (list, tuple)):
         return get_list_diffs(lhs, rhs)
-    elif isinstance(lhs, (str, int, float, bool)):
+    elif isinstance(lhs, str):
+        size = 32
+        lhs_chunks = [lhs[i : i + size] for i in range(0, len(lhs), size)]
+        rhs_chunks = [rhs[i : i + size] for i in range(0, len(rhs), size)]
+        diff = {
+            'type': 'value',
+            'index': [],
+            'lhs': '\n'.join(lhs_chunks),
+            'rhs': '\n'.join(rhs_chunks),
+        }
+        return [diff]
+    elif isinstance(lhs, (int, float, bool)):
         diff = {'type': 'value', 'index': [], 'lhs': lhs, 'rhs': rhs}
         return [diff]
     else:
         raise Exception('not a valid nested type: ' + str(type(lhs)))
 
 
 def get_dict_diffs(
```

### Comparing `toolstr-0.9.6/toolstr/summaries/set_summary.py` & `toolstr-0.9.7/toolstr/summaries/set_summary.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/tables/multiline_tables.py` & `toolstr-0.9.7/toolstr/tables/multiline_tables.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/tables/table_adapters.py` & `toolstr-0.9.7/toolstr/tables/table_adapters.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/toolstr/tables/table_utils.py` & `toolstr-0.9.7/toolstr/tables/table_utils.py`

 * *Files identical despite different names*

### Comparing `toolstr-0.9.6/PKG-INFO` & `toolstr-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolstr
-Version: 0.9.6
+Version: 0.9.7
 Summary: toolstr is a suite of str processing tools, including formatting and drawing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: tooltime>=0.2.10
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: scikit-image>=0.19.2 ; extra == "full"
 Requires-Dist: rich>=12.1.0 ; extra == "full"
```


# Comparing `tmp/flake8-balanced-wrapping-0.1.3.tar.gz` & `tmp/flake8-balanced-wrapping-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-balanced-wrapping-0.1.3.tar", last modified: Sun Jun 18 16:47:45 2023, max compression
+gzip compressed data, was "flake8-balanced-wrapping-0.1.4.tar", last modified: Sun Jun 18 18:55:17 2023, max compression
```

## Comparing `flake8-balanced-wrapping-0.1.3.tar` & `flake8-balanced-wrapping-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-18 16:47:45.871380 flake8-balanced-wrapping-0.1.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-06-18 16:47:36.000000 flake8-balanced-wrapping-0.1.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-18 16:47:45.871380 flake8-balanced-wrapping-0.1.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-06-18 16:47:36.000000 flake8-balanced-wrapping-0.1.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-18 16:47:45.871380 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14150 2023-06-18 16:47:36.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1006 2023-06-18 16:47:45.871380 flake8-balanced-wrapping-0.1.3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-06-18 16:47:36.000000 flake8-balanced-wrapping-0.1.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-18 18:55:17.925705 flake8-balanced-wrapping-0.1.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-06-18 18:55:06.000000 flake8-balanced-wrapping-0.1.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-18 18:55:17.925705 flake8-balanced-wrapping-0.1.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-06-18 18:55:06.000000 flake8-balanced-wrapping-0.1.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-18 18:55:17.925705 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-18 18:55:17.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15837 2023-06-18 18:55:06.000000 flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1006 2023-06-18 18:55:17.929705 flake8-balanced-wrapping-0.1.4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-06-18 18:55:06.000000 flake8-balanced-wrapping-0.1.4/setup.py
```

### Comparing `flake8-balanced-wrapping-0.1.3/LICENSE` & `flake8-balanced-wrapping-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.3/PKG-INFO` & `flake8-balanced-wrapping-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.3
+Version: 0.1.4
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.3/README.md` & `flake8-balanced-wrapping-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/PKG-INFO` & `flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.3
+Version: 0.1.4
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.py` & `flake8-balanced-wrapping-0.1.4/flake8_balanced_wrapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -324,31 +324,35 @@
         if not summary.is_single_line_or_column:
             if not _check_single_entry_hugging():
                 self._record_error(node, by_line_no[summary.most_common_line_number])
 
         self.generic_visit(node)
 
     def visit_IfExp(self, node: ast.IfExp) -> None:
-        start_pos = Position(*self.asttokens.prev_token(_first_token(node)).start)
-
         by_line_no = self._get_nodes_by_line_number(
             node,
-            start_pos,
+            Position.from_node_start(node.body),
             # TODO: when we get to column validation we're going to need a way
             # to represent syntax here not just AST nodes.
             [node.body, node.test, node.orelse],
             include_node_end=False,
             include_node_start=False,
         )
 
         if expression_is_parenthesised(self.asttokens, node):
             # Also account for the parens
-            end_pos = Position(*self.asttokens.next_token(_last_token(node)).end)
-            by_line_no[start_pos.line].append(node)
-            by_line_no[end_pos.line].append(node)
+            open_paren = self.asttokens.prev_token(_first_token(node.body))
+            close_paren = self.asttokens.next_token(_last_token(node.orelse))
+
+            open_line = open_paren.start[0]
+            close_line = close_paren.start[0]
+
+            if open_line in by_line_no or close_line in by_line_no:
+                by_line_no[open_line].append(node)
+                by_line_no[close_line].append(node)
 
         summary = self._summarise_lines(by_line_no)
 
         if not summary.is_single_line_or_column:
             self._record_error(node, by_line_no[summary.most_common_line_number])
 
         self.generic_visit(node)
@@ -402,14 +406,61 @@
         if len(by_line_no) != 1:
             self._record_error(
                 node,
                 list(itertools.chain.from_iterable(by_line_no.values())),
                 error_type=OverWrappedError,
             )
 
+    def visit_BoolOp(self, node: ast.BoolOp) -> None:
+        start_pos = Position.from_node_start(node)
+
+        by_line_no = self._get_nodes_by_line_number(
+            node,
+            start_pos,
+            node.values,
+            include_node_end=False,
+            include_node_start=False,
+        )
+
+        summary = self._summarise_lines(by_line_no)
+
+        if not summary.is_single_line_or_column:
+            self._record_error(
+                node,
+                [node, *node.values],
+                error_type=OverWrappedError,
+            )
+
+        elif expression_is_parenthesised(self.asttokens, node):
+            # Also account for the parens
+            first_token = self.asttokens.prev_token(_first_token(node))
+            last_token = self.asttokens.next_token(_last_token(node))
+
+            if first_token.start[0] in by_line_no or last_token.start[0] in by_line_no:
+                by_line_no[first_token.line].append(node)
+                by_line_no[last_token.line].append(node)
+
+                self._record_error(
+                    node,
+                    [node, *node.values],
+                    error_type=OverWrappedError,
+                )
+
+        self.generic_visit(node)
+
+    def visit_UnaryOp(self, node: ast.UnaryOp) -> None:
+        if node.lineno != node.operand.lineno:
+            self._record_error(
+                node,
+                [node, node.operand],
+                error_type=OverWrappedError,
+            )
+
+        self.generic_visit(node)
+
     def visit_comprehension(self, node: ast.comprehension) -> None:
         self._check_over_wrapping(
             node,
             Position.from_node_start(node),
             [node.target, node.iter],
             include_node_end=False,
             include_node_start=False,
```

### Comparing `flake8-balanced-wrapping-0.1.3/setup.cfg` & `flake8-balanced-wrapping-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.3/setup.py` & `flake8-balanced-wrapping-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 setup(
     name='flake8-balanced-wrapping',
-    version='0.1.3',
+    version='0.1.4',
     url='https://github.com/PeterJCLaw/flake8-balanced-wrapping',
     project_urls={
         'Issue tracker': 'https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues',
     },
     description="A flake8 plugin that helps you wrap code with visual balance.",
     long_description=long_description,
     long_description_content_type='text/markdown',
```


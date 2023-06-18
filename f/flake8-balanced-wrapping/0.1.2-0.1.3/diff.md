# Comparing `tmp/flake8-balanced-wrapping-0.1.2.tar.gz` & `tmp/flake8-balanced-wrapping-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-balanced-wrapping-0.1.2.tar", last modified: Mon May 22 21:37:46 2023, max compression
+gzip compressed data, was "flake8-balanced-wrapping-0.1.3.tar", last modified: Sun Jun 18 16:47:45 2023, max compression
```

## Comparing `flake8-balanced-wrapping-0.1.2.tar` & `flake8-balanced-wrapping-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-22 21:37:46.653696 flake8-balanced-wrapping-0.1.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-05-22 21:37:35.000000 flake8-balanced-wrapping-0.1.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-05-22 21:37:46.657696 flake8-balanced-wrapping-0.1.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-05-22 21:37:35.000000 flake8-balanced-wrapping-0.1.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-22 21:37:46.653696 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-22 21:37:46.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11406 2023-05-22 21:37:35.000000 flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1005 2023-05-22 21:37:46.657696 flake8-balanced-wrapping-0.1.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-05-22 21:37:35.000000 flake8-balanced-wrapping-0.1.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-18 16:47:45.871380 flake8-balanced-wrapping-0.1.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11339 2023-06-18 16:47:36.000000 flake8-balanced-wrapping-0.1.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-18 16:47:45.871380 flake8-balanced-wrapping-0.1.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-06-18 16:47:36.000000 flake8-balanced-wrapping-0.1.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-18 16:47:45.871380 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2256 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      354 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-18 16:47:45.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14150 2023-06-18 16:47:36.000000 flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1006 2023-06-18 16:47:45.871380 flake8-balanced-wrapping-0.1.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1631 2023-06-18 16:47:36.000000 flake8-balanced-wrapping-0.1.3/setup.py
```

### Comparing `flake8-balanced-wrapping-0.1.2/LICENSE` & `flake8-balanced-wrapping-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.2/PKG-INFO` & `flake8-balanced-wrapping-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.2
+Version: 0.1.3
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.2/README.md` & `flake8-balanced-wrapping-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.egg-info/PKG-INFO` & `flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-balanced-wrapping
-Version: 0.1.2
+Version: 0.1.3
 Summary: A flake8 plugin that helps you wrap code with visual balance.
 Home-page: https://github.com/PeterJCLaw/flake8-balanced-wrapping
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues
 Platform: UNKNOWN
```

### Comparing `flake8-balanced-wrapping-0.1.2/flake8_balanced_wrapping.py` & `flake8-balanced-wrapping-0.1.3/flake8_balanced_wrapping.py`

 * *Files 21% similar despite different names*

```diff
@@ -37,39 +37,69 @@
         return (
             f"BWR001 {type(self.node).__name__} is wrapped badly - {len(self.conflicts)} "
             "elements on the same line"
         )
 
 
 @dataclasses.dataclass(frozen=True)
+class CallUnderWrappedError:
+    node: ast.Call
+    conflicts: list[Position]
+
+    @property
+    def position(self) -> Position:
+        return self.conflicts[0]
+
+    def __str__(self) -> str:
+        return (
+            "BWR002 Call is wrapped with separated positional and keyword args - "
+            f"{len(self.conflicts)} elements on the same line"
+        )
+
+
+@dataclasses.dataclass(frozen=True)
 class OverWrappedError:
     node: ast.AST
     positions: list[Position]
 
     @property
     def position(self) -> Position:
         return self.positions[0]
 
     def __str__(self) -> str:
         lines = set(x.line for x in self.positions)
         return (
-            f"BWR002 {type(self.node).__name__} is wrapped unexpectedly over "
+            f"BWR010 {type(self.node).__name__} is wrapped unexpectedly over "
             f"{len(lines)} lines"
         )
 
 
 class PositionsSummary(NamedTuple):
-    is_single_line_or_column: bool
+    is_single_line: bool
+    is_single_column: bool
     most_common_line_number: int
 
+    @property
+    def is_single_line_or_column(self) -> bool:
+        return self.is_single_line or self.is_single_column
+
 
 def get_start_position(node: ast.AST) -> Position:
     return Position.from_node_start(node)
 
 
+def get_start_positions(nodes: Iterable[ast.AST]) -> list[Position]:
+    positions = []
+    for node in nodes:
+        start = get_start_position(node)
+        if start is not None:
+            positions.append(start)
+    return positions
+
+
 def get_end_position(node: ast.AST) -> Position:
     return Position(*_last_token(node).end)
 
 
 def get_end_positions(nodes: Iterable[ast.AST]) -> list[Position]:
     positions = []
     for node in nodes:
@@ -105,38 +135,38 @@
         if include_node_end:
             end_line, end_col = _last_token(node).end
             just_before_end_pos = Position(end_line, end_col - 1)
             end_positions = get_end_positions(nodes)
 
             # Allow hugging, but otherwise add the containing node via its end
             # line too.
-            if just_before_end_pos not in end_positions:
+            if just_before_end_pos not in end_positions or end_line in by_line_no:
                 by_line_no[end_line].append(node)
 
         return by_line_no
 
     def _summarise_lines(
         self,
         nodes_by_line_number: dict[int, list[ast.AST]],
     ) -> PositionsSummary:
         counts = {x: len(y) for x, y in nodes_by_line_number.items()}
         (line_num, max_nodes_per_line), = collections.Counter(counts).most_common(1)
         return PositionsSummary(
-            len(counts) == 1 or max_nodes_per_line == 1,
-            line_num,
+            is_single_line=len(counts) == 1,
+            is_single_column=max_nodes_per_line == 1,
+            most_common_line_number=line_num,
         )
 
     def _record_error(
         self,
         node: ast.AST,
         nodes: list[ast.AST],
         error_type: type[UnderWrappedError] | type[OverWrappedError] = UnderWrappedError,
     ) -> None:
-        maybe_positions = [get_start_position(x) for x in nodes]
-        positions = [x for x in maybe_positions if x is not None]
+        positions = get_start_positions(nodes)
         assert positions
         self.errors.append(error_type(node, positions))
 
     def _check_under_wrapping(
         self,
         node: ast.AST,
         reference: Position,
@@ -170,15 +200,15 @@
             include_node_end=False,
         )
         self.generic_visit(node)
 
     def visit_FunctionDef(self, node: ast.FunctionDef | ast.AsyncFunctionDef) -> None:
         # TODO: also check the positional/args/kwargs markers?
         # TODO: returns will have a different column if wrapped
-        # TODO: check that argument defatuls are on the same line as their arguments?
+        # TODO: check that argument defaults are on the same line as their arguments?
         nodes: list[ast.AST | None] = [
             *node.args.args,
             node.args.vararg,
             *node.args.kwonlyargs,
             node.args.kwarg,
             node.returns,
         ]
@@ -197,20 +227,74 @@
         )
         self.generic_visit(node)
 
     visit_AsyncFunctionDef = visit_FunctionDef
 
     def visit_Call(self, node: ast.Call) -> None:
         open_paren = self.asttokens.find_token(_last_token(node.func), token.OP, '(')
-        self._check_under_wrapping(
+
+        by_line_no = self._get_nodes_by_line_number(
             node,
             Position(*open_paren.end),
             [*node.args, *node.keywords],
             include_node_end=True,
         )
+
+        has_error = False
+        if len(by_line_no) > 1:
+            kwargs_by_line_no = self._get_nodes_by_line_number(
+                node,
+                Position(*open_paren.end),
+                node.keywords,
+                include_node_end=True,
+                include_node_start=not node.args,
+            )
+
+            kwargs_summary = self._summarise_lines(kwargs_by_line_no)
+
+            if not kwargs_summary.is_single_column:
+                has_error = True
+                self._record_error(
+                    node,
+                    kwargs_by_line_no[kwargs_summary.most_common_line_number],
+                )
+
+            pos_args_by_line_no = self._get_nodes_by_line_number(
+                node,
+                Position(*open_paren.end),
+                node.args,
+                include_node_end=not node.keywords,
+                include_node_start=True,
+            )
+
+            pos_args_summary = self._summarise_lines(pos_args_by_line_no)
+
+            if not pos_args_summary.is_single_line_or_column:
+                has_error = True
+                self._record_error(
+                    node,
+                    pos_args_by_line_no[pos_args_summary.most_common_line_number],
+                )
+
+            if not has_error:
+                # Check that overall there is no error. This allows us to emit
+                # CallUnderWrappedError for cases such as:
+                #
+                #    call(42,
+                #        kwarg='',
+                #    )
+                #
+                # which we want to allow users to allow if they want.
+                summary = self._summarise_lines(by_line_no)
+
+                if not summary.is_single_line_or_column:
+                    positions = get_start_positions(by_line_no[summary.most_common_line_number])
+                    assert positions
+                    self.errors.append(CallUnderWrappedError(node, positions))
+
         self.generic_visit(node)
 
     def visit_Dict(self, node: ast.Dict) -> None:
         by_line_no = self._get_nodes_by_line_number(
             node,
             Position.from_node_start(node),
             [x for x in node.keys if x is not None],
```

### Comparing `flake8-balanced-wrapping-0.1.2/setup.cfg` & `flake8-balanced-wrapping-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	__pycache__,
 	build,
 	debian,
 	script
 ignore = 
 	C401
 	W504
-max_line_length = 95
+max_line_length = 105
 
 [isort]
 atomic = True
 balanced_wrapping = True
 combine_as_imports = True
 include_trailing_comma = True
 length_sort = True
```

### Comparing `flake8-balanced-wrapping-0.1.2/setup.py` & `flake8-balanced-wrapping-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 setup(
     name='flake8-balanced-wrapping',
-    version='0.1.2',
+    version='0.1.3',
     url='https://github.com/PeterJCLaw/flake8-balanced-wrapping',
     project_urls={
         'Issue tracker': 'https://github.com/PeterJCLaw/flake8-balanced-wrapping/issues',
     },
     description="A flake8 plugin that helps you wrap code with visual balance.",
     long_description=long_description,
     long_description_content_type='text/markdown',
```


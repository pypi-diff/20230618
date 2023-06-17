# Comparing `tmp/kithon-0.6.0.tar.gz` & `tmp/kithon-0.6.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kithon-0.6.0.tar", max compression
+gzip compressed data, was "kithon-0.6.0.post1.tar", max compression
```

## Comparing `kithon-0.6.0.tar` & `kithon-0.6.0.post1.tar`

### file list

```diff
@@ -1,57 +1,49 @@
--rw-r--r--   0        0        0     1083 2021-09-02 03:22:07.000000 kithon-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1167 2022-10-09 21:54:41.000000 kithon-0.6.0/README.md
--rw-r--r--   0        0        0      148 2022-08-18 14:27:45.000000 kithon-0.6.0/kithon/__init__.py
--rw-r--r--   0        0        0     3025 2022-11-14 21:17:00.000000 kithon-0.6.0/kithon/analogs.py
--rw-r--r--   0        0        0    13208 2022-11-14 21:22:32.000000 kithon-0.6.0/kithon/blocks.py
--rw-r--r--   0        0        0      243 2022-07-18 20:38:38.000000 kithon-0.6.0/kithon/commands/__init__.py
--rw-r--r--   0        0        0      972 2022-05-08 23:16:42.000000 kithon-0.6.0/kithon/commands/configurator.py
--rw-r--r--   0        0        0     4163 2022-10-29 18:43:01.000000 kithon-0.6.0/kithon/commands/gen.py
--rw-r--r--   0        0        0     1242 2022-04-22 18:12:44.000000 kithon-0.6.0/kithon/commands/new.py
--rw-r--r--   0        0        0     1654 2022-07-23 16:00:34.000000 kithon-0.6.0/kithon/commands/repl.py
--rw-r--r--   0        0        0     1547 2022-07-26 21:26:24.000000 kithon-0.6.0/kithon/commands/run.py
--rw-r--r--   0        0        0      856 2022-07-13 03:25:10.000000 kithon-0.6.0/kithon/commands/watch.py
--rw-r--r--   0        0        0      195 2022-11-13 20:59:00.000000 kithon-0.6.0/kithon/contexts.py
--rw-r--r--   0        0        0     2704 2022-04-25 23:11:31.000000 kithon-0.6.0/kithon/controls.py
--rw-r--r--   0        0        0     6971 2022-11-13 18:56:34.000000 kithon-0.6.0/kithon/core.py
--rw-r--r--   0        0        0    11639 2022-10-23 19:35:05.000000 kithon-0.6.0/kithon/expressions.py
--rw-r--r--   0        0        0     4797 2022-11-14 20:58:17.000000 kithon-0.6.0/kithon/node.py
--rw-r--r--   0        0        0      722 2022-06-13 18:49:54.000000 kithon-0.6.0/kithon/side_effects.py
--rw-r--r--   0        0        0     2381 2022-08-02 01:42:52.000000 kithon-0.6.0/kithon/types.py
--rw-r--r--   0        0        0     1664 2022-11-19 19:38:26.386414 kithon-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1060 2022-09-27 19:33:35.000000 kithon-0.6.0/translators/c-like/core.tp
--rw-r--r--   0        0        0      123 2022-04-22 01:34:16.000000 kithon-0.6.0/translators/c-like/macros.tp
--rw-r--r--   0        0        0     2869 2022-11-14 20:56:28.000000 kithon-0.6.0/translators/go/core.tp
--rw-r--r--   0        0        0     1012 2022-07-23 18:32:40.000000 kithon-0.6.0/translators/go/macros.tp
--rw-r--r--   0        0        0     3207 2022-09-15 19:33:28.000000 kithon-0.6.0/translators/go/objects/list.tp
--rw-r--r--   0        0        0      117 2022-01-31 12:50:43.000000 kithon-0.6.0/translators/go/objects/str.tp
--rw-r--r--   0        0        0        0 2022-07-29 21:16:26.000000 kithon-0.6.0/translators/go/slice.tpy~
--rw-r--r--   0        0        0     2890 2022-11-14 21:28:46.000000 kithon-0.6.0/translators/js/core.tp
--rw-r--r--   0        0        0     1304 2022-08-02 00:29:11.000000 kithon-0.6.0/translators/js/libs/dom.tp
--rw-r--r--   0        0        0     2121 2022-03-19 21:03:49.000000 kithon-0.6.0/translators/js/libs/html.tp~
--rw-r--r--   0        0        0      148 2022-03-19 20:15:16.000000 kithon-0.6.0/translators/js/libs/json.tp
--rw-r--r--   0        0        0      816 2022-07-23 16:03:59.000000 kithon-0.6.0/translators/js/libs/math.tp
--rw-r--r--   0        0        0      122 2022-07-23 17:38:31.000000 kithon-0.6.0/translators/js/libs/random.tp
--rw-r--r--   0        0        0      168 2022-02-12 17:36:42.000000 kithon-0.6.0/translators/js/libs/random.tp~
--rw-r--r--   0        0        0      828 2022-07-13 03:47:26.000000 kithon-0.6.0/translators/js/libs/react.tp
--rw-r--r--   0        0        0      772 2022-06-24 14:25:07.000000 kithon-0.6.0/translators/js/libs/react.tp~
--rw-r--r--   0        0        0       63 2022-05-23 17:15:25.000000 kithon-0.6.0/translators/js/libs/vue.tp~
--rw-r--r--   0        0        0     1489 2022-07-23 16:28:57.000000 kithon-0.6.0/translators/js/macros.tp
--rw-r--r--   0        0        0      404 2022-10-09 22:10:11.000000 kithon-0.6.0/translators/js/meta.tp
--rw-r--r--   0        0        0        0 2022-10-09 22:03:41.000000 kithon-0.6.0/translators/js/meta.tp~
--rw-r--r--   0        0        0      358 2022-05-27 23:28:36.000000 kithon-0.6.0/translators/js/objects/dataclass.tp
--rw-r--r--   0        0        0      362 2022-05-27 23:28:16.000000 kithon-0.6.0/translators/js/objects/dataclass.tp~
--rw-r--r--   0        0        0      272 2022-03-03 20:42:35.000000 kithon-0.6.0/translators/js/objects/dict.tp
--rw-r--r--   0        0        0      273 2022-03-03 20:33:32.000000 kithon-0.6.0/translators/js/objects/dict.tp~
--rw-r--r--   0        0        0     1075 2022-07-25 18:20:27.000000 kithon-0.6.0/translators/js/objects/list.tp
--rw-r--r--   0        0        0       62 2022-01-07 17:48:48.000000 kithon-0.6.0/translators/js/objects/str.tp
--rw-r--r--   0        0        0     2430 2022-11-14 20:36:07.000000 kithon-0.6.0/translators/python/core.tp
--rw-r--r--   0        0        0     1004 2022-07-23 15:56:15.000000 kithon-0.6.0/translators/python/libs/math.tp
--rw-r--r--   0        0        0     1019 2022-07-23 15:50:24.000000 kithon-0.6.0/translators/python/libs/math.tp~
--rw-r--r--   0        0        0       65 2022-07-23 17:38:38.000000 kithon-0.6.0/translators/python/libs/random.tp
--rw-r--r--   0        0        0        0 2022-07-23 17:37:25.000000 kithon-0.6.0/translators/python/libs/random.tp~
--rw-r--r--   0        0        0      123 2022-08-03 08:08:38.000000 kithon-0.6.0/translators/python/libs/typing.tp
--rw-r--r--   0        0        0      104 2022-08-02 18:18:32.000000 kithon-0.6.0/translators/python/libs/typing.tp~
--rw-r--r--   0        0        0       21 2022-07-23 18:31:58.000000 kithon-0.6.0/translators/python/macros.tp
--rw-r--r--   0        0        0      416 2022-08-02 18:19:54.000000 kithon-0.6.0/translators/python/type-inference-rules.tp
--rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 kithon-0.6.0/setup.py
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 kithon-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/LICENSE.txt
+-rw-r--r--   0        0        0     1251 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/README.md
+-rw-r--r--   0        0        0      148 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/__init__.py
+-rw-r--r--   0        0        0     3025 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/analogs.py
+-rw-r--r--   0        0        0    13523 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/blocks.py
+-rw-r--r--   0        0        0      243 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/commands/__init__.py
+-rw-r--r--   0        0        0      972 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/commands/configurator.py
+-rw-r--r--   0        0        0     4150 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/commands/gen.py
+-rw-r--r--   0        0        0     1242 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/commands/new.py
+-rw-r--r--   0        0        0     1654 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/commands/repl.py
+-rw-r--r--   0        0        0     1547 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/commands/run.py
+-rw-r--r--   0        0        0      856 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/commands/watch.py
+-rw-r--r--   0        0        0      282 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/contexts.py
+-rw-r--r--   0        0        0     2704 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/controls.py
+-rw-r--r--   0        0        0     7185 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/core.py
+-rw-r--r--   0        0        0    11639 2023-06-17 21:40:57.259539 kithon-0.6.0.post1/kithon/expressions.py
+-rw-r--r--   0        0        0     4894 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/kithon/node.py
+-rw-r--r--   0        0        0      626 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/kithon/side_effects.py
+-rw-r--r--   0        0        0     2381 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/kithon/types.py
+-rw-r--r--   0        0        0     1852 2023-06-17 21:54:26.360994 kithon-0.6.0.post1/pyproject.toml
+-rw-r--r--   0        0        0     1060 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/c-like/core.tp
+-rw-r--r--   0        0        0      123 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/c-like/macros.tp
+-rw-r--r--   0        0        0     3002 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/go/core.tp
+-rw-r--r--   0        0        0      352 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/go/libs/json.tp
+-rw-r--r--   0        0        0     1012 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/go/macros.tp
+-rw-r--r--   0        0        0     3207 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/go/objects/list.tp
+-rw-r--r--   0        0        0      117 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/go/objects/str.tp
+-rw-r--r--   0        0        0     2957 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/core.tp
+-rw-r--r--   0        0        0     1304 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/libs/dom.tp
+-rw-r--r--   0        0        0      166 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/libs/json.tp
+-rw-r--r--   0        0        0      816 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/libs/math.tp
+-rw-r--r--   0        0        0      122 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/libs/random.tp
+-rw-r--r--   0        0        0      828 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/libs/react.tp
+-rw-r--r--   0        0        0     1489 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/macros.tp
+-rw-r--r--   0        0        0      404 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/meta.tp
+-rw-r--r--   0        0        0     1075 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/objects/list.tp
+-rw-r--r--   0        0        0       62 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/js/objects/str.tp
+-rw-r--r--   0        0        0     1949 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/lua/core.tp
+-rw-r--r--   0        0        0      125 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/lua/macros.tp
+-rw-r--r--   0        0        0       67 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/lua/objects/list.tp
+-rw-r--r--   0        0        0       74 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/lua/tools.tp
+-rw-r--r--   0        0        0     2566 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/python/core.tp
+-rw-r--r--   0        0        0     1004 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/python/libs/math.tp
+-rw-r--r--   0        0        0       65 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/python/libs/random.tp
+-rw-r--r--   0        0        0      123 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/python/libs/typing.tp
+-rw-r--r--   0        0        0       21 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/python/macros.tp
+-rw-r--r--   0        0        0     1514 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/python/objects/str.tp
+-rw-r--r--   0        0        0      416 2023-06-17 21:40:57.262873 kithon-0.6.0.post1/translators/python/type-inference-rules.tp
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 kithon-0.6.0.post1/PKG-INFO
```

### Comparing `kithon-0.6.0/LICENSE.txt` & `kithon-0.6.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/README.md` & `kithon-0.6.0.post1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,8 +24,18 @@
 $ kithon run --to go hello_world.py
 ```
 It should be clear what to do. If not, ask us in our [Telegram chat](https://t.me/kithon).
 
 How to Contribute
 -----------------
 
-First, install `python>=3.9`, `poetry`
+Follow these steps:
+
+install `python>=3.9`, `poetry`
+
+```
+poetry install -E all --with docs --with test
+```
+
+```
+pytest
+```
```

#### html2text {}

```diff
@@ -6,8 +6,9 @@
 and integration with tools of target languages including cli and libraries **
 [Try out the web demo](https://alploskov.github.io/kithon-site/demo/)** Quick
 start ------------ First, you install it: ```text $ pip install kithon[all] ```
 Then, you translate your code to target language, in this example JavaSctipt
 ```text $ kithon gen --to js hello_world.py ``` Or translate and run resulting
 code ```text $ kithon run --to go hello_world.py ``` It should be clear what to
 do. If not, ask us in our [Telegram chat](https://t.me/kithon). How to
-Contribute ----------------- First, install `python>=3.9`, `poetry`
+Contribute ----------------- Follow these steps: install `python>=3.9`,
+`poetry` ``` poetry install -E all --with docs --with test ``` ``` pytest ```
```

### Comparing `kithon-0.6.0/kithon/analogs.py` & `kithon-0.6.0.post1/kithon/analogs.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/kithon/blocks.py` & `kithon-0.6.0.post1/kithon/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 import typing
 import _ast
 from .types import types
 from .contexts import Loop
-from .core import visitor
+from .core import visitor, dont_render
 from . import analogs
 
 
 @visitor
 def expr(self, tree: _ast.Expr):
     return self.node(
         tmp='expr',
@@ -168,14 +168,15 @@
             f"{self.ctx[-1].name}_broken", type='bool'
         )] if self.ctx[-1].els else [],
         tmp='while',
         parts={
             'condition': self.visit(tree.test),
             'body': expression_block(self, tree.body),
             'els': expression_block(self, tree.orelse) if tree.orelse else '',
+            'loop': self.ctx[-1],
         }
     )
     if self.templates['while']['meta'].get('gen_else'):
         analogs.loop_else(self, loop)
     self.ctx.pop()
     return loop
 
@@ -209,14 +210,15 @@
             f"{self.ctx[-1].name}_broken", type='bool'
         )] if self.ctx[-1].els else [],
         tmp=tmp,
         parts={
             'var': var,
             'body': expression_block(self, tree.body),
             'els': expression_block(self, tree.orelse) if tree.orelse else '',
+            'loop': self.ctx[-1],
         } | parts
     )
     if self.templates[tmp]['meta'].get('gen_else'):
         analogs.loop_else(self, loop)
     self.ctx.pop()
     return loop
 
@@ -326,23 +328,23 @@
     macro = decorating(self, decorators)
     node = self.node(
         tmp=macro.get('decorate', 'class'),
         name='class',
         parts={
             'name': tree.name,
             'body': body,
-            'init': next(filter(
+            'init': dont_render(next(filter(
                 lambda m: m.name == 'init',
                 body.parts['body']
-            ), ''),
+            ), '')),
             'attrs': attrs,
-            'methods': list(filter(
+            'methods': dont_render(list(filter(
                 lambda m: m.name == 'method',
                 body.parts['body']
-            )),
+            ))),
             'decorators': decorators
         }
     )
     self.namespace = self.previous_ns()
     return node
 
 @visitor
@@ -433,20 +435,26 @@
     return self.node(
         tmp='global',
         parts={'vars': vars}
     )
 
 @visitor
 def _break(self, tree: _ast.Break):
+    self.ctx[-1] = self.ctx[-1]._replace(is_broken=True)
     code_before = []
     if self.templates['break']['meta'].get('gen_else') and self.ctx[-1].els:
         code_before = [
             analogs.assign(self, f"{self.ctx[-1].name}_broken", True)
         ]
     return self.node(
         tmp='break',
-        code_before=code_before
+        code_before=code_before,
+        parts={'loop': self.ctx[-1]}
     )
 
 @visitor
 def _continue(self, tree: _ast.Continue):
-    return self.node(tmp='continue')
+    self.ctx[-1] = self.ctx[-1]._replace(is_continuing=True)
+    return self.node(
+        tmp='continue',
+        parts={'loop': self.ctx[-1]}
+    )
```

### Comparing `kithon-0.6.0/kithon/commands/configurator.py` & `kithon-0.6.0.post1/kithon/commands/configurator.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/kithon/commands/gen.py` & `kithon-0.6.0.post1/kithon/commands/gen.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import ast
 import os
 import sys
-from pathlib import Path
 from _ast import Import, ImportFrom
 from typing import Optional
 import typer
 from jinja2 import Template
 from . import configurator
 from .. import Transpiler
 from .watch import watch
 try:
     import packed
-    pyx = lambda code: packed.translate(code)
 except:
-    pyx = lambda code: code
+    packed = None
 
 
 def compilation_order(__dir__):
     modules = {}
     for _file in os.listdir(__dir__):
         if _file.startswith('.'):
             continue
         ext = _file.split('.')[-1]
         if ext in ['py', 'coco', 'hy', 'pyx', 'cocox']:
             name = os.path.split(_file)[1].removesuffix('.' + ext)
             code = open(os.path.join(__dir__, _file), 'r').read()
-            if ext.endswith('x'):
-                code = pyx(code)
+            if ext.endswith('x') and packed != None:
+                code = packed.translate(code)
             modules |= {name: {
                 'count_dependent': 0,
                 'code': code
             }}
     for mod in modules:
         tree = ast.parse(modules[mod]['code']).body
         for node in tree:
@@ -111,16 +109,16 @@
                 except:
                     print(f'\033[31mFaile compile {m}\033[38m')
             print('----------')
     else:
         ext = file_name.split('.')[-1]
         def g():
             code = open(file_name, 'r').read()
-            if ext.endswith('x'):
-                code = pyx(code)
+            if ext.endswith('x') and packed is not None:
+                code = packed.translate(code)
             lang = input_lang or ext.removesuffix('x')
             _code = transpiler.generate(
                     code, lang=lang
             )
             print(
                 _code,
                 file=open(out, 'w') if out else sys.stdout
```

### Comparing `kithon-0.6.0/kithon/commands/new.py` & `kithon-0.6.0.post1/kithon/commands/new.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/kithon/commands/repl.py` & `kithon-0.6.0.post1/kithon/commands/repl.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/kithon/commands/run.py` & `kithon-0.6.0.post1/kithon/commands/run.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/kithon/commands/watch.py` & `kithon-0.6.0.post1/kithon/commands/watch.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/kithon/controls.py` & `kithon-0.6.0.post1/kithon/controls.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/kithon/core.py` & `kithon-0.6.0.post1/kithon/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,27 +12,33 @@
 try:
     from coconut.convenience import parse, setup
 except ImportError:
     is_coconut_supported = False
 else:
     is_coconut_supported = True
 from jinja2 import Template
-from . import types, node as _node, __path__
+from .node import Node
+from . import types, __path__
 
 
 def visitor(func):
     setattr(Transpiler, func.__name__, func)
     annotations = func.__annotations__['tree']
     if isinstance(annotations, tuple):
         for ann in annotations:
             Transpiler.elements[ann] = func
     else:
         Transpiler.elements[annotations] = func
     return func
 
+class dont_render:
+    def __init__(self, node):
+        self.dont_render = True
+        self.node = node
+
 class Transpiler:
     elements = {}
 
     def __init__(self, lang='', templs=''):
         self.templates = {}
         self.get_lang('python')
         if lang:
@@ -102,15 +108,15 @@
 
     def previous_ns(self):
         if self.namespace == '__main__':
             return '__main__'
         return self.namespace[:self.namespace.rfind('.')]
 
     def node(self, **kwargs):
-        return _node.node(env=self, **kwargs)
+        return Node(env=self, **kwargs)
 
     def get_lang(self, lang):
         _dir = Path(__path__[0]).parent / 'translators' / lang
         if not _dir.exists():
             raise ValueError(f'{lang} is not supported')
         for templs in _dir.glob('**/*.tp'):
             self.load_templs(templs.open().read())
@@ -149,15 +155,15 @@
                     self.add_templ(name, value)
                 elif field in keywords:
                     self.templates[name].update({field: value})
                 else:
                     self.add_templ(f'{name}.{field}', value)
 
     def visit(self, tree, **kw):
-        if isinstance(tree, _node.node):
+        if isinstance(tree, Node):
             return tree
         if isinstance(tree, (int, str, float, bool)):
             tree = ast.Constant(value=tree)
         if type(tree) not in self.elements:
             return self.node()
         node = self.elements.get(type(tree))(
             self, tree,
@@ -186,18 +192,21 @@
             if not is_coconut_supported:
                 raise Exception(
                     "requires coconut library\n"
                     "\trun 'python -m pip install kithon[add-langs]' to fix"
                 )
             setup(target='sys')
             tree = ast.parse(parse(code, 'block')).body
-        for block in map(self.visit, tree):
-            if not block:
-                continue
-            self.strings.extend(block.render().split('\n'))
+        if mode == 'eval':
+            return self.visit(tree[0].value).render()
+        else:
+            for block in map(self.visit, tree):
+                if not block:
+                    continue
+                self.strings.extend(block.render().split('\n'))
         if mode != 'block':
             code = self.templates['main']['tmp'].render(
                 _body=self.strings,
                 body='\n'.join(self.strings),
                 env=self
             )
             if mode == 'main':
```

### Comparing `kithon-0.6.0/kithon/expressions.py` & `kithon-0.6.0.post1/kithon/expressions.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/kithon/node.py` & `kithon-0.6.0.post1/kithon/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         name='type',
         parts={
             f: type_to_node(env, getattr(_type, f))
             for f in _type.fields
         }
     )
 
-class node:
+class Node:
     def __init__(self, env=None, tmp='', name=None, parts={}, type=None, own=None, code_before=None):
         if tmp.startswith('type.'):
             self.name = 'type'
             self.tmp = Template(tmp.removeprefix('type.'))
         elif tmp in env.templates:
             self.name = name or tmp
             self.tmp = env.templates[tmp].get('tmp', '')
@@ -41,33 +41,35 @@
         self.ast = None
         self.parent = None
         self.part_name = ''
         self.own = own
         self.code_before = code_before or []
 
     def render(self):
-        _get_val = lambda el: el.render() if isinstance(el, node) else el
+        _get_val = lambda el: el.render() if isinstance(el, Node) else el
         _type = self.env.variables.get(
             self.own, {}
         ).get('type', self.type)
         if self.name != 'type':
             type = type_to_node(self.env, _type)
             type.render()
         else:
             type = _type
         for _name, part in self.parts.items():
+            if getattr(part, 'dont_render', None):
+                self.parts[_name] = part.node
             if self.name != 'type' and _name.endswith('type'):
                 self.parts[_name] = part = type_to_node(self.env, part)
-            if isinstance(part, node):
+            if isinstance(part, Node):
                 part.parent = self
                 part.part_name = _name
                 part.render()
             elif isinstance(part, list):
                 for part_el in part:
-                    if isinstance(part_el, node):
+                    if isinstance(part_el, Node):
                         part_el.parent = self
                         part_el.part_name = _name
                         part_el.render()
         if getattr(self, 'tmp', None):
             self.val = self.tmp.render(
                 env=self.env,
                 node=self,
@@ -118,28 +120,28 @@
     def __str__(self):
         return self.val
 
     def __call__(self):
         return self.render()
 
     def __eq__(self, other):
-        if isinstance(other, node):
+        if isinstance(other, Node):
             if self.is_const() and other.is_const():
                 return self.get_val() == other.get_val()
             return self.parts == other.parts
         if self.is_const():
             return self.get_val() == other
         return False
 
     def __ne__(self, other):
         return not self == other
 
 for op in (lt, le, ge, gt):
     def operation(op):
         def _(self, other):
             if self.is_const():
-                if isinstance(other, node) and other.is_const():
+                if isinstance(other, Node) and other.is_const():
                     return op(self.get_val(), other.get_val())
                 return op(self.get_val(), other)
             return False
         return _
-    setattr(node, f'__{op.__name__}__', operation(op))
+    setattr(Node, f'__{op.__name__}__', operation(op))
```

### Comparing `kithon-0.6.0/kithon/types.py` & `kithon-0.6.0.post1/kithon/types.py`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/pyproject.toml` & `kithon-0.6.0.post1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "kithon"
 readme = "README.md"
-version = "0.6.0"
+version = "0.6.0.post1"
 description = "transpiler python into other languages"
 authors = ["Aleksey Ploskov"]
 license = "MIT"
 repository = "https://github.com/alploskov/kithon"
 packages = [
         { include = "kithon" }
 ]
@@ -18,38 +18,38 @@
 	"translators/js/libs/*",
 	"translators/js/objects/*",
 
 	"translators/go/*",
 	"translators/go/libs/*",
 	"translators/go/objects/*",
 
+	"translators/lua/*",
+	"translators/lua/libs/*",
+	"translators/lua/objects/*",
+
 	"translators/c-like/*.tp"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9.0,<3.11"
+python = ">=3.9.0,<3.12"
 Jinja2 = ">=2.11.2,<4.0.0"
 PyYaml = ">=5.4.0"
 typer = "^0.4.0"
 
-hy = "<2.0"
+hy = {version = "<2.0", optional = true}
 coconut = {version = "^1.6.0", optional = true}
 
 pexpect = {version = "^4.8.0", optional = true}
 ptpython = {version = "^3.0.20", optional = true}
 
 watchdog = {version = "^2.1.7", optional = true}
 
 packed = "^0.2"
-mkdocs = {version = ">=1.1.2,<2.0.0", optional = true}
-mkdocs-material = {version = ">=8.1.4,<9.0.0", optional = true}
-mdx-include = {version = ">=1.4.1,<2.0.0", optional = true}
 
 [tool.poetry.dev-dependencies]
-hy = {path = "deps/hy-1.0a4-py3-none-any.whl", optional = true}
 packed = {path = "deps/packed-0.2.1-py3-none-any.whl", optional = true}
 
 [tool.poetry.scripts]
 kithon = "kithon.commands:kithon"
 
 [tool.poetry.extras]
 add-langs = ["coconut", "hy"]
@@ -57,18 +57,27 @@
 watch = ["watchdog"]
 pyx = ["packed"]
 all = [
      "packed", "watchdog",
      "coconut", "hy",
      "pexpect", "ptpython"
 ]
-doc = [
-    "mkdocs",
-    "mkdocs-material",
-    "mdx-include"
-]
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = {version = ">=1.1.2,<2.0.0", optional = true}
+mkdocs-material = {version = ">=8.1.4,<9.0.0", optional = true}
+mdx-include = {version = ">=1.4.1,<2.0.0", optional = true}
+
+[tool.poetry.group.test]
+optional = true
 
+[tool.poetry.group.test.dependencies]
+pytest = "*"
+PyExecJS = "^1.5"
+lupa = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kithon-0.6.0/translators/c-like/core.tp` & `kithon-0.6.0.post1/translators/c-like/core.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/translators/go/core.tp` & `kithon-0.6.0.post1/translators/go/core.tp`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 bool: "{{val|lower}}"
+ellipsis: ""
 
 operators:
   "or": "||"
   "and": "&&"
   "not": "!"
   "is": "=="
   "//": "/"
@@ -21,15 +22,15 @@
   meta: {"gen_negative_indexes": yes}
   tmp: ~
 steped_slice:
   meta: {"gen_negative_indexes": yes}
   tmp: ~
 
 new_var: "{{var}} := {{value}}"
-var_prototype: "var {{name}} {{type}}"
+var_prototype: "var {{name}} {{type}}{%if isinstance(default_val.type, types['list'])%} = {{default_val}}{%endif%}"
 if: "if {{condition}} {{body}} {{els}}"
 elif: "else if {{condition}} {{body}} {{els}}"
 else: "else {{body}}"
 ternary: ~
 
 func: "func {{name}}({{args|join(', ')}}){%if ret_type.val != 'None'%} {{ret_type}}{%endif%} {{body}}"
 
@@ -105,14 +106,17 @@
   {% if env.used %}
   import ({%- for used in env.used -%}
   {% if used.startswith('mod_')%}{{'\n    '}}"{{used[4:]}}"{%endif%}
   {%- endfor -%}{{'\n'}})
   {% endif %}
   {{body}}
 
+entry:
+  decorate: "func main() {{body}}"
+
 meta:
   run: "echo '{{code}}' > file1.go && go run file1.go && rm file1.go"
   build: |-
     {%- if out -%}
     go build {{out}}
     {%- else -%}
     echo '{{code}}' > main.go && go build main.go && rm main.go
```

### Comparing `kithon-0.6.0/translators/go/macros.tp` & `kithon-0.6.0.post1/translators/go/macros.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/translators/go/objects/list.tp` & `kithon-0.6.0.post1/translators/go/objects/list.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/translators/js/core.tp` & `kithon-0.6.0.post1/translators/js/core.tp`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 bool: "{{val|lower}}"
 str: "{%if '\n' in val%}`{{val}}`{%else%}\"{{val}}\"{%endif%}"
+ellipsis: "undefined"
 
 operators:
   "==": "==="
   "!=": "!=="
   "or": "||"
   "and": "&&"
   "not": "!"
@@ -18,15 +19,15 @@
   {%- else -%}
     {{obj}}
   {%- endif -%}.{{attr}}
 
 index: "{{obj}}[{{key}}]"
 
 list[any].__getitem__:
-  meta: {"gen_negative_indexes": yes}
+  code: "{{obj}}.at({{key}})"
 
 dict[any].__getitem__:
   code: >-
     {{obj}}[{%- if ctx == 'load' -%}
       {{key}}] == undefined?(()=>{throw "key error"})():{{obj}}[{{key}}
     {%-else-%}
       {{key}}
@@ -101,7 +102,10 @@
   {{'{'}}{% for st in body %}
   {{'    '*nl}}{{st}}{% endfor %}
   {{'    '*(nl-1)}}}
 import: 'import * as {{alias}} from "./{{name}}";'
 import_from: 'import {{"{"}}{{name}}{%if alias != name%} as {{alias}}{%endif%}} from "./{{module|replace(".", "/")}}";'
 global: no
 nonlocal: no
+
+entry:
+  decorate: "{{body.parts.body|join('\n')}}"
```

### Comparing `kithon-0.6.0/translators/js/libs/dom.tp` & `kithon-0.6.0.post1/translators/js/libs/dom.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/translators/js/libs/math.tp` & `kithon-0.6.0.post1/translators/js/libs/math.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/translators/js/libs/react.tp` & `kithon-0.6.0.post1/translators/js/libs/react.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/translators/js/macros.tp` & `kithon-0.6.0.post1/translators/js/macros.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/translators/js/objects/list.tp` & `kithon-0.6.0.post1/translators/js/objects/list.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/translators/python/core.tp` & `kithon-0.6.0.post1/translators/python/core.tp`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 operators: {}
 
 name: '{{name}}'
 int: '{{val}}'
 float: '{{val}}'
 bool: '{{val}}'
 str: "\"{{val}}\""
+ellipsis: "..."
 
 bin_op: |-
   {%-if parent.name == "bin_op"-%}
   ({{left}} {{op}} {{right}})
   {%-else-%}
   {{left}} {{op}} {{right}}
   {%-endif-%}
@@ -67,16 +68,23 @@
   :{%for st in body%}
   {{'    '*nl}}{{st}}{%endfor%}
 
 global: 'global {{vars|join(", ")}}'
 nonlocal: 'nonlocal {{vars|join(", ")}}'
 import: 'import {{name}}{%if alias != name%} as {{alias}}{%endif%}'
 import_from: "from {{module}} import {{name}}{%if alias != name%} as {{alias}}{%endif%}"
+
 main: '{{body}}'
 
+entry:
+  decorate: |-
+    if __name__ == "__main__":{% for st in body.parts.body %}
+    {{'    '}}{{st}}{% endfor %}
+
+
 meta:
   repl:
     name: python
     prompt: ">>> "
   run: "python -c '{{code}}'"
   keyword_tmp: "_{{keyword}}"
   keywords: []
```

### Comparing `kithon-0.6.0/translators/python/libs/math.tp` & `kithon-0.6.0.post1/translators/python/libs/math.tp`

 * *Files identical despite different names*

### Comparing `kithon-0.6.0/PKG-INFO` & `kithon-0.6.0.post1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: kithon
-Version: 0.6.0
+Version: 0.6.0.post1
 Summary: transpiler python into other languages
 Home-page: https://github.com/alploskov/kithon
 License: MIT
 Author: Aleksey Ploskov
-Requires-Python: >=3.9.0,<3.11
+Requires-Python: >=3.9.0,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: add-langs
 Provides-Extra: all
-Provides-Extra: doc
 Provides-Extra: pyx
 Provides-Extra: repl
 Provides-Extra: watch
 Requires-Dist: Jinja2 (>=2.11.2,<4.0.0)
 Requires-Dist: PyYaml (>=5.4.0)
-Requires-Dist: coconut (>=1.6.0,<2.0.0); extra == "add-langs" or extra == "all"
-Requires-Dist: hy (<2.0); extra == "add-langs" or extra == "all"
-Requires-Dist: mdx-include (>=1.4.1,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs (>=1.1.2,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs-material (>=8.1.4,<9.0.0); extra == "doc"
-Requires-Dist: packed (>=0.2,<0.3); extra == "pyx" or extra == "all"
-Requires-Dist: pexpect (>=4.8.0,<5.0.0); extra == "repl" or extra == "all"
-Requires-Dist: ptpython (>=3.0.20,<4.0.0); extra == "repl" or extra == "all"
+Requires-Dist: coconut (>=1.6.0,<2.0.0) ; extra == "add-langs" or extra == "all"
+Requires-Dist: hy (<2.0) ; extra == "add-langs" or extra == "all"
+Requires-Dist: packed (>=0.2,<0.3) ; extra == "pyx" or extra == "all"
+Requires-Dist: pexpect (>=4.8.0,<5.0.0) ; extra == "repl" or extra == "all"
+Requires-Dist: ptpython (>=3.0.20,<4.0.0) ; extra == "repl" or extra == "all"
 Requires-Dist: typer (>=0.4.0,<0.5.0)
-Requires-Dist: watchdog (>=2.1.7,<3.0.0); extra == "watch" or extra == "all"
+Requires-Dist: watchdog (>=2.1.7,<3.0.0) ; extra == "watch" or extra == "all"
 Project-URL: Repository, https://github.com/alploskov/kithon
 Description-Content-Type: text/markdown
 
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/alploskov/kithon/blob/master/LICENSE.txt) <a href="https://pypi.org/project/kithon" target="_blank"> <img src="https://img.shields.io/pypi/v/kithon?color=%2334D058&label=pypi%20package" alt="Package version"></a> ![lines of code](https://tokei.rs/b1/github/alploskov/kithon)
 
 **Kithon** is universal python transpiler for speedup python programs and use python in other platform, such as browser or game engines, it focused on generating human readable code and integration with tools of target languages including cli and libraries
 
@@ -57,9 +54,18 @@
 $ kithon run --to go hello_world.py
 ```
 It should be clear what to do. If not, ask us in our [Telegram chat](https://t.me/kithon).
 
 How to Contribute
 -----------------
 
-First, install `python>=3.9`, `poetry`
+Follow these steps:
 
+install `python>=3.9`, `poetry`
+
+```
+poetry install -E all --with docs --with test
+```
+
+```
+pytest
+```
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: kithon Version: 0.6.0 Summary: transpiler python
-into other languages Home-page: https://github.com/alploskov/kithon License:
-MIT Author: Aleksey Ploskov Requires-Python: >=3.9.0,<3.11 Classifier: License
-:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Provides-Extra: add-langs Provides-Extra: all
-Provides-Extra: doc Provides-Extra: pyx Provides-Extra: repl Provides-Extra:
-watch Requires-Dist: Jinja2 (>=2.11.2,<4.0.0) Requires-Dist: PyYaml (>=5.4.0)
-Requires-Dist: coconut (>=1.6.0,<2.0.0); extra == "add-langs" or extra == "all"
-Requires-Dist: hy (<2.0); extra == "add-langs" or extra == "all" Requires-Dist:
-mdx-include (>=1.4.1,<2.0.0); extra == "doc" Requires-Dist: mkdocs
-(>=1.1.2,<2.0.0); extra == "doc" Requires-Dist: mkdocs-material
-(>=8.1.4,<9.0.0); extra == "doc" Requires-Dist: packed (>=0.2,<0.3); extra ==
-"pyx" or extra == "all" Requires-Dist: pexpect (>=4.8.0,<5.0.0); extra ==
-"repl" or extra == "all" Requires-Dist: ptpython (>=3.0.20,<4.0.0); extra ==
-"repl" or extra == "all" Requires-Dist: typer (>=0.4.0,<0.5.0) Requires-Dist:
-watchdog (>=2.1.7,<3.0.0); extra == "watch" or extra == "all" Project-URL:
-Repository, https://github.com/alploskov/kithon Description-Content-Type: text/
-markdown [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)]
-(https://github.com/alploskov/kithon/blob/master/LICENSE.txt) [Package_version]
-![lines of code](https://tokei.rs/b1/github/alploskov/kithon) **Kithon** is
-universal python transpiler for speedup python programs and use python in other
-platform, such as browser or game engines, it focused on generating human
-readable code and integration with tools of target languages including cli and
-libraries **[Try out the web demo](https://alploskov.github.io/kithon-site/
-demo/)** Quick start ------------ First, you install it: ```text $ pip install
-kithon[all] ``` Then, you translate your code to target language, in this
-example JavaSctipt ```text $ kithon gen --to js hello_world.py ``` Or translate
-and run resulting code ```text $ kithon run --to go hello_world.py ``` It
-should be clear what to do. If not, ask us in our [Telegram chat](https://t.me/
-kithon). How to Contribute ----------------- First, install `python>=3.9`,
-`poetry`
+Metadata-Version: 2.1 Name: kithon Version: 0.6.0.post1 Summary: transpiler
+python into other languages Home-page: https://github.com/alploskov/kithon
+License: MIT Author: Aleksey Ploskov Requires-Python: >=3.9.0,<3.12 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Provides-Extra: add-langs Provides-Extra: all Provides-Extra:
+pyx Provides-Extra: repl Provides-Extra: watch Requires-Dist: Jinja2
+(>=2.11.2,<4.0.0) Requires-Dist: PyYaml (>=5.4.0) Requires-Dist: coconut
+(>=1.6.0,<2.0.0) ; extra == "add-langs" or extra == "all" Requires-Dist: hy
+(<2.0) ; extra == "add-langs" or extra == "all" Requires-Dist: packed
+(>=0.2,<0.3) ; extra == "pyx" or extra == "all" Requires-Dist: pexpect
+(>=4.8.0,<5.0.0) ; extra == "repl" or extra == "all" Requires-Dist: ptpython
+(>=3.0.20,<4.0.0) ; extra == "repl" or extra == "all" Requires-Dist: typer
+(>=0.4.0,<0.5.0) Requires-Dist: watchdog (>=2.1.7,<3.0.0) ; extra == "watch" or
+extra == "all" Project-URL: Repository, https://github.com/alploskov/kithon
+Description-Content-Type: text/markdown [![GitHub license](https://
+img.shields.io/badge/license-MIT-blue.svg)](https://github.com/alploskov/
+kithon/blob/master/LICENSE.txt) [Package_version] ![lines of code](https://
+tokei.rs/b1/github/alploskov/kithon) **Kithon** is universal python transpiler
+for speedup python programs and use python in other platform, such as browser
+or game engines, it focused on generating human readable code and integration
+with tools of target languages including cli and libraries **[Try out the web
+demo](https://alploskov.github.io/kithon-site/demo/)** Quick start -----------
+- First, you install it: ```text $ pip install kithon[all] ``` Then, you
+translate your code to target language, in this example JavaSctipt ```text $
+kithon gen --to js hello_world.py ``` Or translate and run resulting code
+```text $ kithon run --to go hello_world.py ``` It should be clear what to do.
+If not, ask us in our [Telegram chat](https://t.me/kithon). How to Contribute -
+---------------- Follow these steps: install `python>=3.9`, `poetry` ``` poetry
+install -E all --with docs --with test ``` ``` pytest ```
```


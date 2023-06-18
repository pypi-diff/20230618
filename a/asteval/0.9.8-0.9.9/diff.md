# Comparing `tmp/asteval-0.9.8.tar.gz` & `tmp/asteval-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asteval-0.9.8.tar", last modified: Thu Sep 29 13:11:35 2016, max compression
+gzip compressed data, was "dist/asteval-0.9.9.tar", last modified: Sat Oct 14 19:48:06 2017, max compression
```

## Comparing `asteval-0.9.8.tar` & `asteval-0.9.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2016-09-29 13:11:35.000000 asteval-0.9.8/
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2016-09-29 13:11:35.000000 asteval-0.9.8/asteval/
--rw-r--r--   0 Newville   (501) staff       (20)      862 2016-09-29 13:11:11.000000 asteval-0.9.8/asteval/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)    29488 2016-09-29 13:11:11.000000 asteval-0.9.8/asteval/asteval.py
--rw-r--r--   0 Newville   (501) staff       (20)    13457 2016-09-29 13:11:11.000000 asteval-0.9.8/asteval/astutils.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2016-09-29 13:11:35.000000 asteval-0.9.8/asteval.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)        1 2016-09-29 13:11:35.000000 asteval-0.9.8/asteval.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)     1328 2016-09-29 13:11:35.000000 asteval-0.9.8/asteval.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)      406 2016-09-29 13:11:35.000000 asteval-0.9.8/asteval.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        8 2016-09-29 13:11:35.000000 asteval-0.9.8/asteval.egg-info/top_level.txt
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2016-09-29 13:11:35.000000 asteval-0.9.8/doc/
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2016-09-29 13:11:35.000000 asteval-0.9.8/doc/_static/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2016-01-21 13:44:57.000000 asteval-0.9.8/doc/_static/empty
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2016-09-29 13:11:35.000000 asteval-0.9.8/doc/_templates/
--rw-r--r--   0 Newville   (501) staff       (20)      301 2016-09-29 13:11:11.000000 asteval-0.9.8/doc/_templates/indexsidebar.html
--rw-r--r--   0 Newville   (501) staff       (20)     2677 2016-09-29 13:11:11.000000 asteval-0.9.8/doc/api.rst
--rw-r--r--   0 Newville   (501) staff       (20)     5744 2016-09-29 13:11:11.000000 asteval-0.9.8/doc/basics.rst
--rw-r--r--   0 Newville   (501) staff       (20)     6653 2016-09-29 13:11:11.000000 asteval-0.9.8/doc/conf.py
--rw-r--r--   0 Newville   (501) staff       (20)     1983 2016-09-29 13:11:11.000000 asteval-0.9.8/doc/index.rst
--rw-r--r--   0 Newville   (501) staff       (20)     2244 2016-09-29 13:11:11.000000 asteval-0.9.8/doc/installation.rst
--rw-r--r--   0 Newville   (501) staff       (20)     3281 2016-01-21 13:44:57.000000 asteval-0.9.8/doc/Makefile
--rw-r--r--   0 Newville   (501) staff       (20)     5813 2016-09-29 13:11:11.000000 asteval-0.9.8/doc/motivation.rst
--rw-r--r--   0 Newville   (501) staff       (20)      312 2016-09-29 13:11:11.000000 asteval-0.9.8/INSTALL
--rw-r--r--   0 Newville   (501) staff       (20)     1185 2016-09-29 13:11:11.000000 asteval-0.9.8/LICENSE
--rw-r--r--   0 Newville   (501) staff       (20)      260 2016-09-29 13:11:11.000000 asteval-0.9.8/MANIFEST.in
--rw-r--r--   0 Newville   (501) staff       (20)     1328 2016-09-29 13:11:35.000000 asteval-0.9.8/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     1945 2016-09-29 13:11:11.000000 asteval-0.9.8/README.rst
--rw-r--r--   0 Newville   (501) staff       (20)       59 2016-09-29 13:11:35.000000 asteval-0.9.8/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)     1480 2016-09-29 13:11:11.000000 asteval-0.9.8/setup.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2016-09-29 13:11:35.000000 asteval-0.9.8/tests/
--rw-r--r--   0 Newville   (501) staff       (20)    28109 2016-09-29 13:11:11.000000 asteval-0.9.8/tests/testsuite.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2017-10-14 19:48:06.000000 asteval-0.9.9/
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2017-10-14 19:48:06.000000 asteval-0.9.9/asteval/
+-rw-r--r--   0 Newville   (501) staff       (20)      862 2017-10-08 01:57:44.000000 asteval-0.9.9/asteval/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)    33046 2017-10-14 19:42:52.000000 asteval-0.9.9/asteval/asteval.py
+-rw-r--r--   0 Newville   (501) staff       (20)    13458 2017-10-01 16:56:40.000000 asteval-0.9.9/asteval/astutils.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2017-10-14 19:48:06.000000 asteval-0.9.9/asteval.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2017-10-14 19:48:06.000000 asteval-0.9.9/asteval.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     1362 2017-10-14 19:48:06.000000 asteval-0.9.9/asteval.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)      406 2017-10-14 19:48:06.000000 asteval-0.9.9/asteval.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        8 2017-10-14 19:48:06.000000 asteval-0.9.9/asteval.egg-info/top_level.txt
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2017-10-14 19:48:06.000000 asteval-0.9.9/doc/
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2017-10-14 19:48:06.000000 asteval-0.9.9/doc/_static/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2016-01-21 13:44:57.000000 asteval-0.9.9/doc/_static/empty
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2017-10-14 19:48:06.000000 asteval-0.9.9/doc/_templates/
+-rw-r--r--   0 Newville   (501) staff       (20)      301 2017-10-01 12:45:46.000000 asteval-0.9.9/doc/_templates/indexsidebar.html
+-rw-r--r--   0 Newville   (501) staff       (20)     2283 2017-10-14 19:04:02.000000 asteval-0.9.9/doc/api.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     6015 2017-10-14 17:17:34.000000 asteval-0.9.9/doc/basics.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     6706 2017-10-14 18:51:06.000000 asteval-0.9.9/doc/conf.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2796 2017-10-14 13:23:57.000000 asteval-0.9.9/doc/index.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     2244 2017-10-09 04:52:09.000000 asteval-0.9.9/doc/installation.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     3269 2017-10-08 01:58:35.000000 asteval-0.9.9/doc/Makefile
+-rw-r--r--   0 Newville   (501) staff       (20)     7066 2017-10-14 17:08:46.000000 asteval-0.9.9/doc/motivation.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      312 2017-10-01 16:56:03.000000 asteval-0.9.9/INSTALL
+-rw-r--r--   0 Newville   (501) staff       (20)     1185 2017-10-01 12:45:46.000000 asteval-0.9.9/LICENSE
+-rw-r--r--   0 Newville   (501) staff       (20)      260 2017-10-01 12:44:16.000000 asteval-0.9.9/MANIFEST.in
+-rw-r--r--   0 Newville   (501) staff       (20)     1362 2017-10-14 19:48:06.000000 asteval-0.9.9/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     1945 2017-10-01 16:56:03.000000 asteval-0.9.9/README.rst
+-rw-r--r--   0 Newville   (501) staff       (20)       38 2017-10-14 19:48:06.000000 asteval-0.9.9/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)     1480 2017-10-01 16:56:03.000000 asteval-0.9.9/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2017-10-14 19:48:06.000000 asteval-0.9.9/tests/
+-rw-r--r--   0 Newville   (501) staff       (20)    29310 2017-10-01 16:56:03.000000 asteval-0.9.9/tests/testsuite.py
```

### Comparing `asteval-0.9.8/asteval/__init__.py` & `asteval-0.9.9/asteval/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,20 @@
    simple, flat namespace.
 
    Expressions can be compiled into ast node for later evaluation,
    using the values in the symbol table current at evaluation time.
 
    using python, ast module to parse a python expression.
 
-   version: 0.9.8
-   last update: 29-Sep-2016
+   version: 0.9.9
+   last update: 07-Oct-2017
    License:  BSD
    Author:  Matthew Newville <newville@cars.uchicago.edu>
             Center for Advanced Radiation Sources,
             The University of Chicago
 """
 
 from .asteval import Interpreter
 from .astutils import NameFinder, valid_symbol_name
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 __all__ = ['Interpreter', 'NameFinder', 'valid_symbol_name']
```

### Comparing `asteval-0.9.8/asteval/asteval.py` & `asteval-0.9.9/asteval/asteval.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from __future__ import division, print_function
 from sys import exc_info, stdout, stderr, version_info
 import ast
 import math
 from time import time
 
 import sys
+import six
 
 from .astutils import (FROM_PY, FROM_MATH, FROM_NUMPY, UNSAFE_ATTRS,
                        LOCALFUNCS, NUMPY_RENAMES, op2func,
                        ExceptionHolder, ReturnedNone, valid_symbol_name)
 
 HAS_NUMPY = False
 try:
@@ -32,63 +33,105 @@
     # print("Warning: numpy not available... functionality will be limited.")
     pass
 
 builtins = __builtins__
 if not isinstance(builtins, dict):
     builtins = builtins.__dict__
 
+ALL_NODES = ['arg', 'assert', 'assign', 'attribute', 'augassign', 'binop',
+             'boolop', 'break', 'call', 'compare', 'continue', 'delete',
+             'dict', 'ellipsis', 'excepthandler', 'expr', 'extslice',
+             'for', 'functiondef', 'if', 'ifexp', 'index', 'interrupt',
+             'list', 'listcomp', 'module', 'name', 'nameconstant', 'num',
+             'pass', 'print', 'raise', 'repr', 'return', 'slice', 'str',
+             'subscript', 'try', 'tuple', 'unaryop', 'while']
+
 
 # noinspection PyIncorrectDocstring
-class Interpreter:
-    """mathematical expression compiler and interpreter.
+class Interpreter(object):
+    """create an asteval Interpreter: a restricted, simplified interpreter
+    of mathematical expressions using Python syntax.
+
+    The interpreter uses a simple, flat namespace.  Many builtin Python
+    functions, functions from the `math` module, and functions from `numpy`
+    (if available) are pre-loaded into the namespace. Several builtin
+    functions such as 'eval', 'exec', and 'getattr' are not included, as
+    these are considered unsafe.
+
+    Many Python features aresupported by default, including
+       advanced slicing:    a[::-1], array[-3:, :, ::2]
+       if-then-elif-else conditionals
+       for loops
+       while loops
+       try-except-finally blocks
+       function definitions
+       if-expressions:      x = a if TEST else b
+       list comprehension:   out = [sqrt(i) for i in values]
+
+    with the exception of slicing, each of these features can be turned off
+    if desired.
+
+    Many Python syntax elements are not supported at all:
+        Import, Exec, Lambda, Class, Global, Generators, Yield, Decorators
+
+    Parameters
+    ----------
+    symtable : dict or `None`
+        dictionary to use as symbol table (if `None`, one will be created).
+    use_numpy : bool
+        whether to use functions from numpy.
+    writer : file-like or `None`
+        callable file-like object where standard output will be sent.
+    err_writer : file-like or `None`
+        callable file-like object where standard error will be sent.
+    minimal : bool
+        whether to make a minimal interpreter, with many options turned off (see Note 1).
+    no_if : bool
+        whether to support `if` blocks
+    no_for : bool
+        whether to support `for` blocks.
+    no_while : bool
+        whether to support `while` blocks.
+    no_try : bool
+        whether to support `try` blocks.
+    no_functiondef : bool
+        whether to support user-defined functions.
+    no_ifexp : bool
+        whether to support if expressions.
+    no_listcomp : bool
+        whether to support list comprehension.
+    no_augassign : bool
+        whether to support augemented assigments (`a += 1`, etc).
+    no_assert : bool
+        whether to support `assert`.
+    no_delete : bool
+        whether to support `del`.
+    no_raise : bool
+        whether to support `raise`.
+    no_print : bool
+        whether to support `print`.
+    max_time : float
+        deprecated.  maximum time (in seconds) to run (see Note 2)
+
+    Notes
+    -----
+    1. setting `minimal=True` is equivalent to setting all `no_***` options to `True`.
+    2. the max_time option is easily broken and not supportable.
+    """
 
-  This module compiles expressions and statements to AST representation,
-  using python's ast module, and then executes the AST representation
-  using a dictionary of named object (variable, functions).
-
-  The result is a restricted, simplified version of Python meant for
-  numerical caclulations that is somewhat safer than 'eval' because some
-  operations (such as 'import' and 'eval') are simply not allowed.  The
-  resulting language uses a flat namespace that works on Python objects,
-  but does not allow new classes to be defined.
-
-  Many parts of Python syntax are supported, including:
-     for loops, while loops, if-then-elif-else conditionals
-     try-except (including 'finally')
-     function definitions with def
-     advanced slicing:    a[::-1], array[-3:, :, ::2]
-     if-expressions:      out = one_thing if TEST else other
-     list comprehension   out = [sqrt(i) for i in values]
-
-  The following Python syntax elements are not supported:
-      Import, Exec, Lambda, Class, Global, Generators,
-      Yield, Decorators
-
-  In addition, while many builtin functions are supported, several
-  builtin functions are missing ('eval', 'exec', and 'getattr' for
-  example) that can be considered unsafe.
-
-  If numpy is installed, many numpy functions are also imported.
-
-  """
-
-    supported_nodes = ('arg', 'assert', 'assign', 'attribute', 'augassign',
-                       'binop', 'boolop', 'break', 'call', 'compare',
-                       'continue', 'delete', 'dict', 'ellipsis',
-                       'excepthandler', 'expr', 'extslice', 'for',
-                       'functiondef', 'if', 'ifexp', 'index', 'interrupt',
-                       'list', 'listcomp', 'module', 'name', 'nameconstant',
-                       'num', 'pass', 'print', 'raise', 'repr', 'return',
-                       'slice', 'str', 'subscript', 'try', 'tuple', 'unaryop',
-                       'while')
+    def __init__(self, symtable=None, writer=None, use_numpy=True,
+                 err_writer=None, minimal=False, no_if=False, no_for=False,
+                 no_while=False, no_try=False, no_functiondef=False,
+                 no_ifexp=False, no_listcomp=False, no_augassign=False,
+                 no_assert=False, no_delete=False, no_raise=False,
+                 no_print=False, max_time=30):
 
-    def __init__(self, symtable=None, writer=None, use_numpy=True, err_writer=None, max_time=5):
         self.writer = writer or stdout
         self.err_writer = err_writer or stderr
-        self.start = 0
+        self.start = time()
         self.max_time = max_time
 
         if symtable is None:
             symtable = {}
         self.symtable = symtable
         self._interrupt = None
         self.error = []
@@ -114,20 +157,37 @@
             for sym in FROM_NUMPY:
                 if hasattr(numpy, sym):
                     symtable[sym] = getattr(numpy, sym)
             for name, sym in NUMPY_RENAMES.items():
                 if hasattr(numpy, sym):
                     symtable[name] = getattr(numpy, sym)
 
-        self.node_handlers = dict(((node, getattr(self, "on_%s" % node))
-                                   for node in self.supported_nodes))
+        nodes = ALL_NODES[:]
+
+        if minimal or no_if:           nodes.remove('if')
+        if minimal or no_for:          nodes.remove('for')
+        if minimal or no_while:        nodes.remove('while')
+        if minimal or no_try:          nodes.remove('try')
+        if minimal or no_functiondef:  nodes.remove('functiondef')
+        if minimal or no_ifexp:        nodes.remove('ifexp')
+        if minimal or no_assert:       nodes.remove('assert')
+        if minimal or no_delete:       nodes.remove('delete')
+        if minimal or no_raise:        nodes.remove('raise')
+        if minimal or no_print:        nodes.remove('print')
+        if minimal or no_listcomp:     nodes.remove('listcomp')
+        if minimal or no_augassign:    nodes.remove('augassign')
+
+        self.node_handlers = {}
+        for node in nodes:
+            self.node_handlers[node] = getattr(self, "on_%s" % node)
 
         # to rationalize try/except try/finally for Python2.6 through Python3.3
-        self.node_handlers['tryexcept'] = self.node_handlers['try']
-        self.node_handlers['tryfinally'] = self.node_handlers['try']
+        if 'try' in self.node_handlers:
+            self.node_handlers['tryexcept'] = self.node_handlers['try']
+            self.node_handlers['tryfinally'] = self.node_handlers['try']
 
         self.no_deepcopy = []
         for key, val in symtable.items():
             if callable(val) or 'numpy.lib.index_tricks' in repr(val):
                 self.no_deepcopy.append(key)
 
     def unimplemented(self, node):
@@ -212,14 +272,15 @@
 
     def __call__(self, expr, **kw):
         return self.eval(expr, **kw)
 
     def eval(self, expr, lineno=0, show_errors=True):
         """evaluates a single statement"""
         self.lineno = lineno
+        self.error_msg = None
         self.error = []
         self.start = time()
 
         # noinspection PyBroadException
         try:
             node = self.parse(expr)
         except:
@@ -398,26 +459,28 @@
             self.raise_exception(node, exc=RuntimeError, msg=msg)
 
         sym = self.run(node.value)
         if ctx == ast.Del:
             return delattr(sym, node.attr)
 
         # ctx is ast.Load
-        fmt = "cannnot access attribute '%s' for %s"
-        if node.attr not in UNSAFE_ATTRS:
-            fmt = "no attribute '%s' for %s"
-            try:
-                return getattr(sym, node.attr)
-            except AttributeError:
-                pass
-
-        # AttributeError or accessed unsafe attribute
-        obj = self.run(node.value)
-        msg = fmt % (node.attr, obj)
-        self.raise_exception(node, exc=AttributeError, msg=msg)
+        errfmt = "'%s' object has not attribute '%s'"
+
+        if (node.attr in UNSAFE_ATTRS or
+            (isinstance(sym, six.string_types) and 'format' in node.attr) or
+            (isinstance(sym, Procedure) and node.attr not in dir(sym))):
+            self.raise_exception(node, exc=AttributeError,
+                                 msg=errfmt % (sym, node.attr))
+
+        try:
+            return getattr(sym, node.attr)
+        except AttributeError:
+            self.raise_exception(node, exc=AttributeError,
+                                 msg=errfmt % (sym, node.attr))
+
 
     def on_assign(self, node):  # ('targets', 'value')
         """simple assignment"""
         val = self.run(node.value)
         for tnode in node.targets:
             self.node_assign(tnode, val)
         return
@@ -647,15 +710,18 @@
             args = args + self.run(starargs)
 
         keywords = {}
         for key in node.keywords:
             if not isinstance(key, ast.keyword):
                 msg = "keyword error in function call '%s'" % func
                 self.raise_exception(node, msg=msg)
-            keywords[key.arg] = self.run(key.value)
+            if key.arg is None:   # Py3 **kwargs !
+                keywords.update(self.run(key.value))
+            else:
+                keywords[key.arg] = self.run(key.value)
 
         kwargs = getattr(node, 'kwargs', None)
         if kwargs is not None:
             keywords.update(self.run(kwargs))
 
         # noinspection PyBroadException
         try:
@@ -714,24 +780,35 @@
     This stores the parsed ast nodes as from the
     'functiondef' ast node for later evaluation.
     """
 
     def __init__(self, name, interp, doc=None, lineno=0,
                  body=None, args=None, kwargs=None,
                  vararg=None, varkws=None):
+        self.__ininit__ = True
         self.name = name
         self.__asteval__ = interp
         self.raise_exc = self.__asteval__.raise_exception
         self.__doc__ = doc
         self.body = body
         self.argnames = args
         self.kwargs = kwargs
         self.vararg = vararg
         self.varkws = varkws
         self.lineno = lineno
+        self.__ininit__ = False
+
+    def __setattr__(self, attr, val):
+        if not getattr(self, '__ininit__', True):
+            self.raise_exc(None, exc=TypeError,
+                           msg= "procedure is read-only")
+        self.__dict__[attr] = val
+
+    def __dir__(self):
+        return ['name']
 
     def __repr__(self):
         sig = ""
         if self.argnames:
             sig = "%s%s" % (sig, ', '.join(self.argnames))
         if self.vararg is not None:
             sig = "%s, *%s" % (sig, self.vararg)
@@ -747,39 +824,49 @@
         if self.__doc__ is not None:
             sig = "%s\n  %s" % (sig, self.__doc__)
         return sig
 
     def __call__(self, *args, **kwargs):
         symlocals = {}
         args = list(args)
-        n_args = len(args)
-        n_names = len(self.argnames)
-
-        # may need to move kwargs to args if names align!
-        if (n_args < n_names) and kwargs:
-            for name in self.argnames[n_args:]:
+        nargs = len(args)
+        nkws = len(kwargs)
+        nargs_expected = len(self.argnames)
+        # check for too few arguments, but the correct keyword given
+        if (nargs < nargs_expected) and nkws > 0:
+            for name in self.argnames[nargs:]:
                 if name in kwargs:
                     args.append(kwargs.pop(name))
-            n_args = len(args)
-            n_names = len(self.argnames)
-
-        if self.argnames and kwargs is not None:
-            msg = "multiple values for keyword argument '%s' in Procedure %s"
+            nargs = len(args)
+            nargs_expected = len(self.argnames)
+            nkws = len(kwargs)
+        if nargs < nargs_expected:
+            msg = "%s() takes at least %i arguments, got %i"
+            self.raise_exc(None, exc=TypeError,
+                           msg=msg % (self.name, nargs_expected, nargs))
+        # check for multiple values for named argument
+        if len(self.argnames) > 0 and kwargs is not None:
+            msg = "%s() got multiple values for keyword argument '%s'"
             for targ in self.argnames:
                 if targ in kwargs:
                     self.raise_exc(None, exc=TypeError,
-                                   msg=msg % (targ, self.name),
-                                   lineno=self.lineno)
+                                   msg=msg % (targ, self.name))
 
-        if n_args != n_names:
-            if n_args < n_names:
-                msg = 'not enough arguments for Procedure %s()' % self.name
-                msg = '%s (expected %i, got %i)' % (msg, n_names, n_args)
+        # check more args given than expected, varargs not given
+        if nargs > nargs_expected and self.vararg is None:
+            if nargs - nargs_expected > len(self.kwargs):
+                msg = 'too many arguments for %s() expected at most %i, got %i'
+                msg = msg % (self.name, len(self.kwargs)+nargs_expected, nargs)
                 self.raise_exc(None, exc=TypeError, msg=msg)
 
+            for i, xarg in enumerate(args[nargs_expected:]):
+                kw_name = self.kwargs[i][0]
+                if kw_name not in kwargs:
+                    kwargs[kw_name] = xarg
+
         for argname in self.argnames:
             symlocals[argname] = args.pop(0)
 
         try:
             if self.vararg is not None:
                 symlocals[self.vararg] = tuple(args)
 
@@ -810,13 +897,14 @@
         # evaluate script of function
         for node in self.body:
             self.__asteval__.run(node, expr='<>', lineno=self.lineno)
             if self.__asteval__.error:
                 break
             if self.__asteval__.retval is not None:
                 retval = self.__asteval__.retval
+                self.__asteval__.retval = None
                 if retval is ReturnedNone:
                     retval = None
                 break
 
         self.__asteval__.symtable = save_symtable
         return retval
```

### Comparing `asteval-0.9.8/asteval/astutils.py` & `asteval-0.9.9/asteval/astutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 UNSAFE_ATTRS = ('__subclasses__', '__bases__', '__globals__', '__code__',
                 '__closure__', '__func__', '__self__', '__module__',
                 '__dict__', '__class__', '__call__', '__get__',
                 '__getattribute__', '__subclasshook__', '__new__',
                 '__init__', 'func_globals', 'func_code', 'func_closure',
                 'im_class', 'im_func', 'im_self', 'gi_code', 'gi_frame',
-                '__asteval__', 'f_locals')
+                '__asteval__', 'f_locals', '__mro__')
 
 # inherit these from python's __builtins__
 FROM_PY = ('ArithmeticError', 'AssertionError', 'AttributeError',
            'BaseException', 'BufferError', 'BytesWarning',
            'DeprecationWarning', 'EOFError', 'EnvironmentError',
            'Exception', 'False', 'FloatingPointError', 'GeneratorExit',
            'IOError', 'ImportError', 'ImportWarning', 'IndentationError',
@@ -48,15 +48,15 @@
            'UnicodeTranslateError', 'UnicodeWarning', 'ValueError',
            'Warning', 'ZeroDivisionError', 'abs', 'all', 'any', 'bin',
            'bool', 'bytearray', 'bytes', 'chr', 'complex', 'dict', 'dir',
            'divmod', 'enumerate', 'filter', 'float', 'format', 'frozenset',
            'hash', 'hex', 'id', 'int', 'isinstance', 'len', 'list', 'map',
            'max', 'min', 'oct', 'ord', 'pow', 'range', 'repr',
            'reversed', 'round', 'set', 'slice', 'sorted', 'str', 'sum',
-           'tuple', 'type', 'zip')
+           'tuple', 'zip')
 
 # inherit these from python's math
 FROM_MATH = ('acos', 'acosh', 'asin', 'asinh', 'atan', 'atan2', 'atanh',
              'ceil', 'copysign', 'cos', 'cosh', 'degrees', 'e', 'exp',
              'fabs', 'factorial', 'floor', 'fmod', 'frexp', 'fsum',
              'hypot', 'isinf', 'isnan', 'ldexp', 'log', 'log10', 'log1p',
              'modf', 'pi', 'pow', 'radians', 'sin', 'sinh', 'sqrt', 'tan',
@@ -132,31 +132,36 @@
               'tensordot', 'tile', 'trace', 'transpose', 'trapz', 'tri',
               'tril', 'tril_indices', 'tril_indices_from', 'trim_zeros',
               'triu', 'triu_indices', 'triu_indices_from', 'true_divide',
               'trunc', 'ubyte', 'uint', 'uint0', 'uint16', 'uint32',
               'uint64', 'uint8', 'uintc', 'uintp', 'ulonglong', 'union1d',
               'unique', 'unravel_index', 'unsignedinteger', 'unwrap',
               'ushort', 'vander', 'var', 'vdot', 'vectorize', 'vsplit',
-              'vstack', 'where', 'who', 'zeros', 'zeros_like')
+              'vstack', 'where', 'who', 'zeros', 'zeros_like',
+              'fft', 'linalg', 'polynomial', 'random')
 
 NUMPY_RENAMES = {'ln': 'log', 'asin': 'arcsin', 'acos': 'arccos',
                  'atan': 'arctan', 'atan2': 'arctan2', 'atanh':
                  'arctanh', 'acosh': 'arccosh', 'asinh': 'arcsinh'}
 
 
 def _open(filename, mode='r', buffering=0):
     """read only version of open()"""
     if mode not in ('r', 'rb', 'rU'):
         raise RuntimeError("Invalid open file mode, must be 'r', 'rb', or 'rU'")
     if buffering > MAX_OPEN_BUFFER:
         raise RuntimeError("Invalid buffering value, max buffer size is {}".format(MAX_OPEN_BUFFER))
     return open(filename, mode, buffering)
 
+def _type(obj, *varargs, **varkws):
+    """type that prevents varargs and varkws"""
+    return type(obj).__name__
 
-LOCALFUNCS = {'open': _open}
+
+LOCALFUNCS = {'open': _open, 'type': _type}
 
 
 # Safe versions of functions to prevent denial of service issues
 
 def safe_pow(base, exp):
     if exp > MAX_EXPONENT:
         raise RuntimeError("Invalid exponent, max exponent is {}".format(MAX_EXPONENT))
@@ -290,16 +295,7 @@
         ast.NodeVisitor.__init__(self)
 
     def generic_visit(self, node):
         if node.__class__.__name__ == 'Name':
             if node.ctx.__class__ == ast.Load and node.id not in self.names:
                 self.names.append(node.id)
         ast.NodeVisitor.generic_visit(self, node)
-
-
-def get_ast_names(astnode):
-    """returns symbol Names from an AST node
-    :param astnode:
-    """
-    finder = NameFinder()
-    finder.generic_visit(astnode)
-    return finder.names
```

### Comparing `asteval-0.9.8/asteval.egg-info/PKG-INFO` & `asteval-0.9.9/asteval.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: asteval
-Version: 0.9.8
+Version: 0.9.9
 Summary: Safe, minimalistic evaluator of python expression using ast module
 Home-page: http://github.com/newville/asteval
 Author: Matthew Newville
 Author-email: newville@cars.uchicago.edu
 License: BSD
+Description-Content-Type: UNKNOWN
 Description: ASTEVAL provides a numpy-aware, safe(ish) 'eval' function
         
         Emphasis is on mathematical expressions, and so numpy ufuncs
         are used if available.  Symbols are held in the Interpreter
         symbol table 'symtable':  a simple dictionary supporting a
         simple, flat namespace.
```

### Comparing `asteval-0.9.8/doc/api.rst` & `asteval-0.9.9/doc/api.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,21 @@
+.. _asteval_api:
+
 ===================
 asteval reference
 ===================
 
 The asteval module provides an :class:`Interpreter` class, which creates an
 interpreter.  There is also a convenience function :func:`valid_symbol_name`
 
 .. _numpy: http://docs.scipy.org/doc/numpy
 
 .. module:: asteval
 
-.. class:: Interpreter(symtable=None[, writer=None[, use_numpy=True]])
-
-   create an asteval interpreter.
-
-   :param symtable: a Symbol table (if ``None``, one will be created).
-   :type symtable: ``None`` or dict.
-   :param writer: callable file-like object where standard output will be sent.
-   :type writer:  file-like.
-   :param use_numpy: whether to use functions from `numpy`_.
-   :type use_numpy:   boolean (``True`` / ``False``)
+.. autoclass:: Interpreter
 
 The symbol table will be loaded with several built in functions, several
 functions from the :py:mod:`math` module and, if available and requested,
 several functions from `numpy`_.  This will happen even for a symbol table
 explicitly provided.
 
 The ``writer`` argument can be used to provide a place to send all output
@@ -75,8 +68,7 @@
    of Exceptions raised.
 
 .. attribute:: error_msg
 
    the most recent error message.
 
 .. autofunction:: valid_symbol_name
-
```

### Comparing `asteval-0.9.8/doc/basics.rst` & `asteval-0.9.9/doc/basics.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 ================
 Using asteval
 ================
 
-The asteval module is very easy to use.   Import the module and create an Interpreter:
+This chapter gives a quick overview of asteval, showing basic usage and the
+most important features.  Further details can be found in the next chapter
+(:ref:`asteval_api`).
+
+
+creating and using an asteval Interpreter
+=============================================
+
+
+The asteval module is very easy to use.  Import the module and create an Interpreter:
 
     >>> from asteval import Interpreter
     >>> aeval = Interpreter()
 
 and now you have an embedded interpreter for a procedural, mathematical language
-that es very much like python, ready for use::
+that is very much like python::
 
     >>> aeval('x = sqrt(3)')
     >>> aeval('print x')
     1.73205080757
     >>> aeval('''for i in range(10):
     print i, sqrt(i), log(1+1)
     ''')
@@ -26,41 +35,43 @@
     7 2.64575131106 2.07944154168
     8 2.82842712475 2.19722457734
     9 3.0 2.30258509299
 
 
 
 accessing the symbol table
-===========================
+=============================
 
-The symbol table (that is, the mapping between variable and
-function names and the underlying objects) is a simple dictionary
-held in the :attr:`symtable` attribute of the interpreter.  Of
-course, this can be read or written to by the python program:
+The symbol table (that is, the mapping between variable and function names
+and the underlying objects) is a simple dictionary held in the
+:attr:`symtable` attribute of the interpreter, and can be read or written
+to::
 
     >>> aeval('x = sqrt(3)')
     >>> aeval.symtable['x']
     1.73205080757
     >>> aeval.symtable['y'] = 100
     >>> aeval('print y/8')
     12.5
 
-(Note the use of true division even though the operands are integers).
+Note here the use of true division even though the operands are integers.
+
+As with Python itself, valid symbol names must match the basic regular
+expression pattern::
 
-Certain names are reserved in Python, and cannot be used within
-the asteval interpreter.  These reserved words are:
+   valid_name = [a-zA-Z_][a-zA-Z0-9_]*
+
+In addition, certain names are reserved in Python, and cannot be used
+within the asteval interpreter.  These reserved words are:
 
     and, as, assert, break, class, continue, def, del, elif, else,
     except, exec, finally, for, from, global, if, import, in, is,
     lambda, not, or, pass, print, raise, return, try, while, with,
     True, False, None, eval, execfile, __import__, __package__
 
-Valid symbol names must match the basic regular expression pattern::
-
-   valid_name = [a-zA-Z_][a-zA-Z0-9_]*
 
 
 built-in functions
 =======================
 
 At startup, many symbols are loaded into the symbol table from
 Python's builtins and the **math** module.   The builtins include
@@ -118,17 +129,17 @@
     >>> aeval(code)
     sum =  114.049534067
 
 
 printing
 ===============
 
-For printing, asteval emulates Python's native :func:`print` function and
-:data:`print` statement (for python 2).  That is, the behavior mimics the
-version of python used.
+For printing, asteval emulates Python's native :func:`print` function (for
+Python 3) and :data:`print` statement (for Python 2).  That is, the
+behavior mimics the version of Python used.
 
 You can change where output is sent with the ``writer`` argument when
 creating the interpreter.  By default, outputs are sent to
 :py:data:`sys.stdout`.
 
 
 writing functions
@@ -169,8 +180,7 @@
    >>>     inp_string = raw_input('dsl:>')
    >>>     result = aeval(inp_string)
    >>>     if len(aeval.error)>0:
    >>>         for err in aeval.error:
    >>>             print(err.get_error())
    >>>     else:
    >>>         print(result)
-
```

### Comparing `asteval-0.9.8/doc/conf.py` & `asteval-0.9.9/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #sys.path.append(os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.todo',
+extensions = ['sphinx.ext.autodoc',
+              'sphinx.ext.napoleon',
+              'sphinx.ext.todo',
               'sphinx.ext.coverage',
               'sphinx.ext.mathjax', 'sphinx.ext.intersphinx']
 
 intersphinx_mapping = {'py': ('http://docs.python.org/', None)}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
@@ -130,15 +132,15 @@
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 #html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-html_use_smartypants = False # True
+# html_use_smartypants = False # True
 
 # Custom sidebar templates, maps document names to template names.
 html_sidebars = {'index': ['indexsidebar.html','searchbox.html']}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
 #html_additional_pages = {}
```

### Comparing `asteval-0.9.8/doc/index.rst` & `asteval-0.9.9/doc/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 .. asteval documentation master file,
 
 ASTEVAL: Minimal Python AST Evaluator
 ================================================
 
 .. _numpy: http://docs.scipy.org/doc/numpy
 
-ASTEVAL is a safe(ish) evaluator of Python expressions and statements,
-using Python's ast module.  The idea is to provide a simple, robust
-miniature mathematical language that is more complete than
-:py:func:`ast.literal_eval` and can handle user-input more safely than
-:py:func:`eval`.  The emphasis here is on mathematical calculations, so
-mathematical functions from Python's :py:mod:`math` module are available,
-and a large number of functions from `numpy`_ will be available if it is
-installed on your system.
-
-Many parts of the Python language are supported, including if-then-else
-conditionals, while loops, for loops, try-except blocks, list
-comprehension, slicing, subscripting, and writing user-defined functions.
-All objects are true python objects, and many built-in data structures
-(strings, dictionaries, tuple, lists, numpy arrays), are supported.  Still,
-there are important absences and differences, and asteval is by no means an
-attempt to reproduce Python with its own ast module.  Some of the
-differences and absences include:
+The asteval package evaluates mathematical expressions and statements,
+providing a safer alternative to Python's builtin :py:func:`eval` and a
+richer, easier to use alternative to :py:func:`ast.literal_eval`.  It does
+this by building an embedded interpreter for a subset of the Python
+language using Python's :py:mod:`ast` module.  The emphasis here and main
+area of application is the evaluation of mathematical expressions. Because
+of this, mathematical functions from Python's :py:mod:`math` module are
+available, and a large number of functions from `numpy`_ will be available
+if it is installed on your system.
+
+In addition to basic mathematical expressions, many parts of the Python
+language are supported by default, including array slicing and
+subscripting, if-then-else conditionals, while loops, for loops, try-except
+blocks, list comprehension, and user-defined functions.  All objects in the
+asteval interpreter are truly python objects, and all built-in data
+structures (strings, dictionaries, tuple, lists, numpy arrays), are
+supported. That is, the asteval mini-language will look and act very much
+like Python itself.
+
+Still, there are important differences and missing features compared to
+Python. Asteval is by no means an attempt to reproduce Python with its own
+:py:mod:`ast` module.  Some of the main differences and absences include:
 
  1. Variable and function symbol names are held in a simple symbol
     table - a single dictionary - giving a flat namespace.
  2. creating classes is not allowed.
  3. importing modules is not allowed.
  4. function decorators, generators, yield, and lambda are not supported.
  5. several builtins (:py:func:`eval`, :py:func:`execfile`,
@@ -33,14 +38,22 @@
     :py:func:`delattr`) are not allowed.
  6. Accessing several private object attributes that can provide access to
     the python interpreter are not allowed.
 
 The result of this makes asteval a decidedly restricted and limited language
 that is focused on mathematical calculations.
 
+Because asteval is suitable for evaluating user-supplied input strings,
+safety against malicious user input is an important concern.  Asteval tries
+as hard as possible to prevent user-supplied input from crashing the Python
+interpreter or from returning exploitable parts of the Python interpreter.
+In this sense asteval is certainly safer than using :py:func:`eval`.
+However, asteval is an open source project written by volunteers, and we
+cannot guarantee that it is safe against malicious attacks.
+
 .. toctree::
    :maxdepth: 2
 
    installation
    motivation
    basics
    api
```

### Comparing `asteval-0.9.8/doc/installation.rst` & `asteval-0.9.9/doc/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 .. _numpy: http://docs.scipy.org/doc/numpy
 .. _github:  http://github.com/newville/asteval
 .. _PyPI:  http://pypi.python.org/pypi/asteval/
 
 Requirements
 ~~~~~~~~~~~~~~~
 
-The asteval package is supported for use with Python 2.7, 3.3, 3.4, and 3.5.
-The package may work for Python 2.6, and Python 3.2, but no testing is done
+The asteval package is supported for use with Python 2.7, 3.4, 3.5, and 3.6.
+The package may work for Python 2.6, and Python 3.3, but no testing is done
 for these out-dated versions.  Asteval will make use of the `numpy`_ module
 if available.
 
 
 Download and Installation
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The latest stable version of asteval is 0.9.7 and is available at `PyPI`_ or as
+The latest stable version of asteval is 0.9.9 and is available at `PyPI`_ or as
 a conda package.  That is, you should be able to install asteval with::
 
    pip install asteval
 
 or::
 
    conda install -c newville asteval
```

### Comparing `asteval-0.9.8/doc/Makefile` & `asteval-0.9.9/doc/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
 
 asteval.pdf: latex
 	cd $(BUILDDIR)/latex && make all-pdf
 	cp -pr $(BUILDDIR)/latex/asteval.pdf ./asteval.pdf
 
-all: html asteval.pdf
+all: html
 
 install: all
 	cp -pr $(BUILDDIR)/latex/asteval.pdf $(INSTALLDIR)/asteval.pdf
 	cp -pr $(BUILDDIR)/html/* $(INSTALLDIR)/.
 
 help:
 	@echo "Please use \`make <target>' where <target> is one of"
```

### Comparing `asteval-0.9.8/doc/motivation.rst` & `asteval-0.9.9/doc/motivation.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 .. _lmfit: http://github.com/lmfit/lmfit-py
 .. _xraylarch: http://github.com/xraypy/xraylarch
 
 ########################
 Motivation for asteval
 ########################
 
-The asteval module provides a means to evaluate a large subset of the
-Python language from within a python program, without using
-:py:func:`eval`.  It is, in effect, a restricted version of Python's
-built-in :py:func:`eval`, forbidding several actions, and using using a
-simple dictionary as a flat namespace.  A completely fair question is: Why
-on earth would anyone do this?  That is, why not simply use
-:py:func:`eval`, or just use Python itself?
+The asteval module allows you to evaluate a large subset of the Python
+language from within a python program, without using :py:func:`eval`.  It
+is, in effect, a restricted version of Python's built-in :py:func:`eval`,
+forbidding several actions, and using using a simple dictionary as a flat
+namespace.  A completely fair question is: Why is this desirable?  That
+is, why not simply use :py:func:`eval`, or just use Python itself?
 
 The short answer is that sometimes you want to allow evaluation of user
 input, or expose a simple calculator inside a larger application.  For
 this, :py:func:`eval` is pretty scary, as it exposes *all* of Python, which
-can make user input difficult to trust.  Since asteval does not support the
+makes user input difficult to trust.  Since asteval does not support the
 **import** statement (or many other constructs), user code cannot access
 the :py:mod:`os` and :py:mod:`sys` modules or any functions or classes
 outside the provided symbol table.
 
 Other missing features (modules, classes, lambda, yield, generators) are
-similarly motivated.  The idea for asteval is to make a simple procedural,
-mathematically-oriented language that can be embedded safely into larger
-applications.
+similarly motivated by a desire for a safer version of :py:func:`eval`.
+The idea for asteval is to make a simple procedural, mathematically
+oriented language that can be embedded into larger applications.
 
 In fact, the asteval module grew out the the need for a simple expression
 evaluator for scientific applications such as the `lmfit`_ and `xraylarch`_
 modules.  A first attempt using the pyparsing module worked but was
 error-prone and difficult to maintain.  It turned out that using the Python
 :py:mod:`ast` module is so easy that adding more complex programming
 constructs like conditionals, loops, exception handling, complex assignment
@@ -39,88 +38,102 @@
 Tree.  Furthermore, the resulting AST is easy to walk through, greatly
 simplifying evaluation over any other approach.  What started as a desire
 for a simple expression evaluator grew into a quite useable procedural
 domain-specific language for mathematical applications.
 
 Asteval makes no claims about speed. Obviously,  evaluating the ast tree
 involves a lot of function calls, and will likely be slower than Python.
-In preliminary tests, it's about 4x slower than Python.
+In preliminary tests, it's about 4x slower than Python.  For certain use
+cases (see https://stackoverflow.com/questions/34106484), use of asteval
+and numpy can approach the speed of `eval` and the `numexpr` modules.
 
 How Safe is asteval?
 =======================
 
-I'll be completely honest:  I don't know.
-
-If you're looking for guarantees that malicious code cannot ever cause
-damage, you're definitely looking in the wrong place.  I don't suggest that
-asteval is completely safe, only that it is safer than the builtin
-:py:func:`eval`, and that you might find it useful.
-
-For why :py:func:`eval` is dangerous, see, for example `Eval is really
-dangerous
+Asteval definitely avoids many of the exploits that make :py:func:`eval` is
+dangerous. For reference, see, `Eval is really dangerous
 <http://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html>`_ and
 the comments and links therein.  Clearly, making :py:func:`eval` perfectly
 safe from malicious user input is a difficult prospect.  Basically, if one
-can cause Python to seg-fault, safety cannot be guaranteed.
+can cause Python to seg-fault, safety cannot be guaranteed. That said, we
+cannot guarantee that asteval is completely safe from malicious code.  We
+claim only that it is safer than the builtin :py:func:`eval`, and that you
+might find it useful.
 
-Asteval is meant to be safer than the builtin :py:func:`eval`, and does try
-to avoid any known exploits.  Many actions are not allowed from the asteval
-interpreter, including:
+Asteval tries to avoid many known exploits and unsafe actions.  Some of the
+things not  allowed in the asteval interpreter for safety reasons include:
 
-  * importing modules.  Neither 'import' nor '__import__' is supported.
+  * importing modules.  Neither 'import' nor '__import__' are supported.
   * create classes or modules.
   * access to Python's :py:func:`eval`, :py:func:`execfile`,
     :py:func:`getattr`, :py:func:`hasattr`, :py:func:`setattr`, and
     :py:func:`delattr`.
 
 In addition (and following the discussion in the link above), the following
 attributes are blacklisted for all objects, and cannot be accessed:
 
    __subclasses__, __bases__, __globals__, __code__, __closure__, __func__,
    __self__, __module__, __dict__, __class__, __call__, __get__,
    __getattribute__, __subclasshook__, __new__, __init__, func_globals,
    func_code, func_closure, im_class, im_func, im_self, gi_code, gi_frame
+   f_locals, __mro__
 
 Of course, this approach of making a blacklist cannot be guaranteed to be
 complete, but it does eliminate classes of attacks to seg-fault the Python
 interpreter.  On the other hand, asteval will typically expose numpy ufuncs
 from the numpy module, and several of these can seg-fault Python without
 too much trouble.  If you're paranoid about safe user input that can never
 cause a segmentation fault, you'll want to disable the use of numpy.
 
 There are important categories of safety that asteval does not even attempt
-to address. The most important of these is resource hogging.  There is no
-guaranteed timeout on any calculation, and so a reasonable looking
-calculation such as::
-
-   >>> from asteval import Interpreter
-   >>> aeval = Interpreter()
-   >>> txt = """nmax = 1e8
-   ... a = sqrt(arange(nmax))
-   ... """
-   >>> aeval.eval(txt)
+to address. The most important of these is resource hogging, which might be
+used for a denial-of-service attack.  There is no guaranteed timeout on any
+calculation, and so a reasonable looking calculation such as::
+
+   from asteval import Interpreter
+   aeval = Interpreter()
+   txt = """nmax = 1e8
+   a = sqrt(arange(nmax))
+   """
+   aeval.eval(txt)
 
-can take a noticeable amount of CPU time.  It it not hard to come up with
+can take a noticeable amount of CPU time.  It is not hard to come up with
 short program that would run for hundreds of years, which probably exceeds
-your threshold for an acceptable run-time.
-
-Nevertheless, you may try to limit the *recursion limit* when executing 
-expressions, with a code like this::
+anyones threshold for an acceptable run-time.  As a very simple example, it
+is very hard to predict how long the expression `x**y**z` will take to run
+without knowing the values of `x`, `y`, and `z`.   In short, runtime cannot
+be determined lexically.
+
+For a limited range of problems, you can try to avoid asteval taking too
+long.  For example, you may try to limit the *recursion limit* when
+executing expressions, with a code like this::
 
     import contextlib
-    
+
     @contextlib.contextmanager
     def limited_recursion(recursion_limit):
         old_limit = sys.getrecursionlimit()
         sys.setrecursionlimit(recursion_limit)
         try:
             yield
         finally:
             sys.setrecursionlimit(old_limit)
-    
+
     with limited_recursion(100):
         Interpreter().eval(...)
 
-
-In summary, there are many ways that asteval could be considered part of an
-un-safe programming environment.  Recommendations for how to improve this
-situation would be greatly appreciated.
+You can also pass in a `max_time` (in seconds) when you create an asteval
+Interpreter, wich will try to limit the amount of time an expression will
+take.  This is actually of limited utility, since the calculation must
+return to the asteval interpreter for the runtime to be checked at all.  Many
+long-running calculations will be stuck deep inside C-code evaluated by the
+Python interpreter itself, and not return or allow other threads to run
+until that calculation is done. That is, from within a single process,
+there really is not a foolproof way to tell asteval to have a maximum
+runtime.  The most reliable way to put a firm limit on runtime is to have a
+second process watching the execution time of the asteval process and
+interrupt or kill it.
+
+In summary, while asteval attempts to be safe and is definitely safer than
+using :py:func:`eval`, there are many ways that asteval could be considered
+part of an un-safe programming environment.  Recommendations for how to
+improve this situation would be greatly appreciated.
```

### Comparing `asteval-0.9.8/LICENSE` & `asteval-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asteval-0.9.8/PKG-INFO` & `asteval-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: asteval
-Version: 0.9.8
+Version: 0.9.9
 Summary: Safe, minimalistic evaluator of python expression using ast module
 Home-page: http://github.com/newville/asteval
 Author: Matthew Newville
 Author-email: newville@cars.uchicago.edu
 License: BSD
+Description-Content-Type: UNKNOWN
 Description: ASTEVAL provides a numpy-aware, safe(ish) 'eval' function
         
         Emphasis is on mathematical expressions, and so numpy ufuncs
         are used if available.  Symbols are held in the Interpreter
         symbol table 'symtable':  a simple dictionary supporting a
         simple, flat namespace.
```

### Comparing `asteval-0.9.8/README.rst` & `asteval-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `asteval-0.9.8/setup.py` & `asteval-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `asteval-0.9.8/tests/testsuite.py` & `asteval-0.9.9/tests/testsuite.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,15 +466,16 @@
         for expr, errname in (('x = 1/zero', 'ZeroDivisionError'),
                               ('x = zero + nonexistent', 'NameError'),
                               ('x = zero + astr', 'TypeError'),
                               ('x = zero()', 'TypeError'),
                               ('x = astr * atup', 'TypeError'),
                               ('x = arr.shapx', 'AttributeError'),
                               ('arr.shapx = 4', 'AttributeError'),
-                              ('del arr.shapx', 'KeyError')):
+                              ('del arr.shapx', 'KeyError'),
+                              ('x, y = atup', 'ValueError')):
             failed, errtype, errmsg = False, None, None
             # noinspection PyBroadException
             try:
                 self.interp(expr, show_errors=False)
             except:
                 failed = True
             self.assertTrue(failed)
@@ -670,17 +671,19 @@
         self.interp("a = fcn(4, scale=9)")
         self.isvalue("a", 18)
         self.interp("a = fcn(9, scale=0)")
         self.isvalue("a", 3)
         self.interp("print(fcn)")
         self.check_output('<Procedure fcn(x, scale=')
         self.interp("a = fcn()")
-        self.check_error('TypeError', 'not enough arg')
-        self.interp("a = fcn(x, bogus=3)")
-        self.check_error('NameError')
+        self.check_error('TypeError', 'takes at least 1 arguments, got 0')
+        self.interp("a = fcn(3,4,5,6,7)")
+        self.check_error('TypeError', 'expected at most 2, got')
+        self.interp("a = fcn(77.0, other='what?')")
+        self.check_error('TypeError', 'extra keyword arguments for')
 
     def test_function_vararg(self):
         """test function with var args"""
         self.interp(textwrap.dedent("""
             def fcn(*args):
                 'test varargs function'
                 out = 0
@@ -692,15 +695,15 @@
         self.isvalue('o', 14)
         self.interp("print(fcn)")
         self.check_output('<Procedure fcn(')
 
     def test_function_kwargs(self):
         """test function with kw args, no **kws"""
         self.interp(textwrap.dedent("""
-            def fcn(square=False, x=0, y=0, z=0, t=0):
+            def fcn(x=0, y=0, z=0, t=0, square=False):
                 'test varargs function'
                 out = 0
                 for i in (x, y, z, t):
                     if square:
                         out = out + i*i
                     else:
                         out = out + i
@@ -708,18 +711,30 @@
             """))
         self.interp("print(fcn)")
         self.check_output('<Procedure fcn(square')
         self.interp("o = fcn(x=1, y=2, z=3, square=False)")
         self.isvalue('o', 6)
         self.interp("o = fcn(x=1, y=2, z=3, square=True)")
         self.isvalue('o', 14)
+        self.interp("o = fcn(3, 4, 5)")
+        self.isvalue('o', 12)
+        self.interp("o = fcn(0, -1, 1)")
+        self.isvalue('o', 0)
+        self.interp("o = fcn(0, -1, 1, square=True)")
+        self.isvalue('o', 2)
+        self.interp("o = fcn(1, -1, 1, 1, True)")
+        self.isvalue('o', 4)
         self.interp("o = fcn(x=1, y=2, z=3, t=-2)")
         self.isvalue('o', 4)
         self.interp("o = fcn(x=1, y=2, z=3, t=-12, s=1)")
         self.check_error('TypeError', 'extra keyword arg')
+        self.interp("o = fcn(x=1, y=2, y=3)")
+        self.check_error('SyntaxError')
+        self.interp("o = fcn(0, 1, 2, 3, 4, 5, 6, 7, True)")
+        self.check_error('TypeError', 'too many arguments')
 
     def test_function_kwargs1(self):
         """test function with **kws arg"""
         self.interp(textwrap.dedent("""
             def fcn(square=False, **kws):
                 'test varargs function'
                 out = 0
@@ -754,14 +769,36 @@
         self.interp("o = fcn(y=2, x=7)")
         self.isvalue('o', 11)
         self.interp("o = fcn(1, y=2)")
         self.isvalue('o', 5)
         self.interp("o = fcn(1, x=2)")
         self.check_error('TypeError')
 
+    def test_nested_functions(self):
+        setup="""
+        def a(x=10):
+            if x > 5:
+                return 1
+            return -1
+
+        def b():
+            return 2.5
+
+        def c(x=10):
+            x = a(x=x)
+            y = b()
+            return x + y
+        """
+        self.interp(textwrap.dedent(setup))
+        self.interp("o1 = c()")
+        self.interp("o2 = c(x=0)")
+        self.isvalue('o1', 3.5)
+        self.isvalue('o2', 1.5)
+
+
     def test_astdump(self):
         """test ast parsing and dumping"""
         astnode = self.interp.parse('x = 1')
         self.assertTrue(isinstance(astnode, ast.Module))
         self.assertTrue(isinstance(astnode.body[0], ast.Assign))
         self.assertTrue(isinstance(astnode.body[0].targets[0], ast.Name))
         self.assertTrue(isinstance(astnode.body[0].value, ast.Num))
```


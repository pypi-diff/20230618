# Comparing `tmp/rebnf-0.6.tar.gz` & `tmp/rebnf-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebnf-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rebnf-0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rebnf-0.6.tar` & `rebnf-0.7.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0    32145 2023-06-13 15:45:36.893539 rebnf-0.6/LICENSE.md
--rw-r--r--   0        0        0     2783 2023-06-13 18:23:17.917564 rebnf-0.6/README.md
--rw-r--r--   0        0        0     1159 2023-06-13 18:25:15.789248 rebnf-0.6/pyproject.toml
--rw-r--r--   0        0        0     1813 2023-06-13 18:23:51.905464 rebnf-0.6/rebnf/__init__.py
--rw-r--r--   0        0        0     1474 2023-06-13 16:12:48.740888 rebnf-0.6/rebnf/__main__.py
--rw-r--r--   0        0        0     3347 2023-06-13 16:20:46.776221 rebnf-0.6/rebnf/lexers.py
--rw-r--r--   0        0        0     4272 2023-06-13 15:44:42.734837 rebnf-0.6/rebnf/parsers.py
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 rebnf-0.6/PKG-INFO
+-rw-r--r--   0        0        0    32145 2023-06-13 15:45:36.893539 rebnf-0.7/LICENSE.md
+-rw-r--r--   0        0        0     5966 2023-06-18 01:26:50.525570 rebnf-0.7/README.md
+-rw-r--r--   0        0        0     1149 2023-06-13 20:04:13.563937 rebnf-0.7/pyproject.toml
+-rw-r--r--   0        0        0     2108 2023-06-18 01:26:38.325518 rebnf-0.7/rebnf/__init__.py
+-rw-r--r--   0        0        0     3649 2023-06-17 22:11:44.842728 rebnf-0.7/rebnf/__main__.py
+-rw-r--r--   0        0        0      462 2023-06-18 01:24:42.388990 rebnf-0.7/rebnf/grammar/modular.rebnf
+-rw-r--r--   0        0        0     1048 2023-06-17 13:43:33.312773 rebnf-0.7/rebnf/grammar/spec.rebnf
+-rw-r--r--   0        0        0     4538 2023-06-16 19:39:25.524046 rebnf-0.7/rebnf/lexers.py
+-rw-r--r--   0        0        0    55818 2023-06-17 22:36:58.943956 rebnf-0.7/rebnf/parser.out
+-rw-r--r--   0        0        0     6661 2023-06-18 01:23:04.996491 rebnf-0.7/rebnf/parsers.py
+-rw-r--r--   0        0        0    11431 2023-06-17 22:36:58.943956 rebnf-0.7/rebnf/parsetab.py
+-rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 rebnf-0.7/PKG-INFO
```

### Comparing `rebnf-0.6/LICENSE.md` & `rebnf-0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rebnf-0.6/pyproject.toml` & `rebnf-0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,43 +15,43 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development",
   "Topic :: Text Processing",
 ]
 keywords = [
-  "backus-naur form",
   "bnf", 
-  "context-free grammar",
   "ebnf", 
+  "rebnf", 
+  "regex",
+  "regexes",
+  "backus-naur form",
   "extended backus-naur form",
+  "syntax", 
+  "metasyntax",
+  "lexer", 
+  "parser", 
+  "context-free grammar",
   "formal language",
   "grammar", 
   "language", 
-  "lexer", 
-  "metasyntax",
-  "parser", 
-  "parsing", 
-  "rebnf", 
-  "regex", 
-  "regexes", 
-  "syntax", 
-  "text processing", 
+  "text processing"
 ]
 dependencies = [ "ply" ]
 
 [project.optional-dependencies]
 docs = [
 
 ]
 dev = [
   "black",
   "flake8",
   "flit",
+  "build",
   "twine"
 ]
 
 [project.urls]
 Repository = "https://gitlab.com/opsocket/rebnf.git"
 
 [project.scripts]
-tokenize = "rebnf.__main__:main"
+rebnf = "rebnf.__main__:main"
```

### Comparing `rebnf-0.6/rebnf/__init__.py` & `rebnf-0.7/rebnf/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
-ReBNF: Regexes for Extended Backus-Naur Form
+ReBNF: Regexes for Extended Backus-Naur Form (EBNF)
 
 Copyright (C) 2023 opsocket <opsocket@pm.me>
 
 This program is free software: you can redistribute it and/or modify it under
 the terms of the GNU General Public License as published by the Free Software
 Foundation, either version 3 of the License, or (at your option) any later
 version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY
 WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with
-this program.  If not, see <https://www.gnu.org/licenses/>.
+this program.  If not, see <https://www.gnu.org/licenses>.
 """
 from . import lexers
 from . import parsers
 
 assert all((lexers, parsers))
 
 __author__ = "opsocket <opsocket@pm.me>"
 __description__ = "Lexer and parser for the ReBNF metasyntax language"
-__version__ = "0.6"
+__version__ = "0.7"
 __ascii__ = """
 ooooooooo.             oooooooooo.  ooooo      ooo oooooooooooo 
 `888   `Y88.           `888'   `Y8b `888b.     `8' `888'     `8 
  888   .d88'  .ooooo.   888     888  8 `88b.    8   888         
  888ooo88P'  d88' `88b  888oooo888'  8   `88b.  8   888oooo8    
  888`88b.    888ooo888  888    `88b  8     `88b.8   888    "    
  888  `88b.  888    .o  888    .88P  8       `888   888         
@@ -37,23 +37,33 @@
 {__ascii__} v{__version__}
 
 {__description__}
 
 """
 
 
-def tokenize(code):
+def tokenize(code) -> list[str]:
     """
-    Tokenizes the provided rebnf code using the lexer.
-
-    :param code: The rebnf code to tokenize.
-    :type code: str
-
-    :returns: A list of tokens representing the code.
-    :rtype: list[str]
+    Tokenizes the provided rebnf code using the REBNFLexer.
+    
+    :param      code:  The rebnf code to tokenize.
+    :type       code:  str
+    
+    :returns:   A list of tokens representing the code.
+    :rtype:     list[str]
     """
     lexer = lexers.REBNFLexer()
     return lexer.tokenize(code)
 
 
-def parse(code):
-    raise NotImplementedError()
+def parse(code) -> dict:
+    """
+    Parses the given code using the REBNFParser.
+    
+    :param      code:  The code to parse.
+    :type       code:  str
+    
+    :returns:   The parsed dictionary
+    :rtype:     dict
+    """
+    parser = parsers.REBNFParser()
+    return parser.parse(code)
```


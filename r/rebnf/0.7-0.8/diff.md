# Comparing `tmp/rebnf-0.7.tar.gz` & `tmp/rebnf-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebnf-0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rebnf-0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rebnf-0.7.tar` & `rebnf-0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    32145 2023-06-13 15:45:36.893539 rebnf-0.7/LICENSE.md
--rw-r--r--   0        0        0     5966 2023-06-18 01:26:50.525570 rebnf-0.7/README.md
--rw-r--r--   0        0        0     1149 2023-06-13 20:04:13.563937 rebnf-0.7/pyproject.toml
--rw-r--r--   0        0        0     2108 2023-06-18 01:26:38.325518 rebnf-0.7/rebnf/__init__.py
--rw-r--r--   0        0        0     3649 2023-06-17 22:11:44.842728 rebnf-0.7/rebnf/__main__.py
--rw-r--r--   0        0        0      462 2023-06-18 01:24:42.388990 rebnf-0.7/rebnf/grammar/modular.rebnf
--rw-r--r--   0        0        0     1048 2023-06-17 13:43:33.312773 rebnf-0.7/rebnf/grammar/spec.rebnf
--rw-r--r--   0        0        0     4538 2023-06-16 19:39:25.524046 rebnf-0.7/rebnf/lexers.py
--rw-r--r--   0        0        0    55818 2023-06-17 22:36:58.943956 rebnf-0.7/rebnf/parser.out
--rw-r--r--   0        0        0     6661 2023-06-18 01:23:04.996491 rebnf-0.7/rebnf/parsers.py
--rw-r--r--   0        0        0    11431 2023-06-17 22:36:58.943956 rebnf-0.7/rebnf/parsetab.py
--rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 rebnf-0.7/PKG-INFO
+-rw-r--r--   0        0        0    32145 2023-06-13 15:45:36.893539 rebnf-0.8/LICENSE.md
+-rw-r--r--   0        0        0     5966 2023-06-18 19:20:40.661609 rebnf-0.8/README.md
+-rw-r--r--   0        0        0     1149 2023-06-13 20:04:13.563937 rebnf-0.8/pyproject.toml
+-rw-r--r--   0        0        0     2117 2023-06-18 19:20:35.481633 rebnf-0.8/rebnf/__init__.py
+-rw-r--r--   0        0        0     3732 2023-06-18 19:20:00.829837 rebnf-0.8/rebnf/__main__.py
+-rw-r--r--   0        0        0      462 2023-06-18 01:24:42.388990 rebnf-0.8/rebnf/grammar/modular.rebnf
+-rw-r--r--   0        0        0     1048 2023-06-17 13:43:33.312773 rebnf-0.8/rebnf/grammar/spec.rebnf
+-rw-r--r--   0        0        0     4241 2023-06-18 19:18:21.514890 rebnf-0.8/rebnf/lexers.py
+-rw-r--r--   0        0        0    55729 2023-06-18 16:26:19.998244 rebnf-0.8/rebnf/parser.out
+-rw-r--r--   0        0        0     7235 2023-06-18 19:18:21.534890 rebnf-0.8/rebnf/parsers.py
+-rw-r--r--   0        0        0    11402 2023-06-18 16:26:19.998244 rebnf-0.8/rebnf/parsetab.py
+-rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 rebnf-0.8/PKG-INFO
```

### Comparing `rebnf-0.7/LICENSE.md` & `rebnf-0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rebnf-0.7/README.md` & `rebnf-0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ReBNF
 
 <div>
-  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.7-ec3832.svg?color=ec3832&style=flat"/></a>
+  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.8-ec3832.svg?color=ec3832&style=flat"/></a>
   <a href="https://opsocket.com" style="text-decoration: none;">
     <img alt="opsocket" height="42" src="https://gitlab.com/opsocket/rebnf/-/raw/main/docs/assets/imgs/logo.svg" loading="lazy" />
   </a>
 </div>
 
 
 **ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to define the
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # ReBNF
-[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.7-
+[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.8-
 ec3832.svg?color=ec3832&style=flat] [opsocket]
 **ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to
 define the syntax of a language using regular expressions. It is an extension
 of the EBNF (Extended Backus-Naur Form) notation, allowing for more flexibility
 and ease of use. ``` ooooooooo. oooooooooo. ooooo ooo oooooooooooo `888 `Y88.
 `888' `Y8b `888b. `8' `888' `8 888 .d88' .ooooo. 888 888 8 `88b. 8 888
 888ooo88P' d88' `88b 888oooo888' 8 `88b. 8 888oooo8 888`88b. 888ooo888 888 `88b
```

### Comparing `rebnf-0.7/pyproject.toml` & `rebnf-0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rebnf-0.7/rebnf/__init__.py` & `rebnf-0.8/rebnf/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from . import lexers
 from . import parsers
 
 assert all((lexers, parsers))
 
 __author__ = "opsocket <opsocket@pm.me>"
 __description__ = "Lexer and parser for the ReBNF metasyntax language"
-__version__ = "0.7"
+__version__ = "0.8"
 __ascii__ = """
 ooooooooo.             oooooooooo.  ooooo      ooo oooooooooooo 
 `888   `Y88.           `888'   `Y8b `888b.     `8' `888'     `8 
  888   .d88'  .ooooo.   888     888  8 `88b.    8   888         
  888ooo88P'  d88' `88b  888oooo888'  8   `88b.  8   888oooo8    
  888`88b.    888ooo888  888    `88b  8     `88b.8   888    "    
  888  `88b.  888    .o  888    .88P  8       `888   888         
@@ -40,30 +40,31 @@
 
 """
 
 
 def tokenize(code) -> list[str]:
     """
     Tokenizes the provided rebnf code using the REBNFLexer.
-    
+
     :param      code:  The rebnf code to tokenize.
     :type       code:  str
-    
+
     :returns:   A list of tokens representing the code.
     :rtype:     list[str]
     """
     lexer = lexers.REBNFLexer()
     return lexer.tokenize(code)
 
 
 def parse(code) -> dict:
     """
     Parses the given code using the REBNFParser.
-    
+
     :param      code:  The code to parse.
     :type       code:  str
-    
-    :returns:   The parsed dictionary
-    :rtype:     dict
+
+    :returns:   The parsed abstract syntax tree
+    :rtype:     tuple
     """
     parser = parsers.REBNFParser()
-    return parser.parse(code)
+    ast = parser.parse(code)
+    return ast
```

### Comparing `rebnf-0.7/rebnf/__main__.py` & `rebnf-0.8/rebnf/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,27 +86,31 @@
     # call appropriate function based on subcommand
     if hasattr(args, "func"):
         with open(args.filepath, "r") as code:
             if args.subcommand == "tokenize":
                 tokens = args.func(code.read())
                 print(
                     tabulate(
-                        [[t.lineno, t.column, t.lexpos, t.type, fmtok(t)] for t in tokens],
+                        [
+                            [t.lineno, t.column, t.lexpos, t.type, fmtok(t)]
+                            for t in tokens
+                        ],
                         headers=[
                             "LINE",
                             "COL",
                             "POS",
                             "TYPE",
                             "TOKEN",
                         ],
                     )
                 )
             else:
                 if args.pretty:
                     from pprint import pprint
+
                     pprint(args.func(code.read()))
                 else:
                     print(args.func(code.read()))
     else:
         parser.print_help()
```

### Comparing `rebnf-0.7/rebnf/grammar/spec.rebnf` & `rebnf-0.8/rebnf/grammar/spec.rebnf`

 * *Files identical despite different names*

### Comparing `rebnf-0.7/rebnf/lexers.py` & `rebnf-0.8/rebnf/lexers.py`

 * *Files 19% similar despite different names*

```diff
@@ -54,38 +54,31 @@
             self.column,
         )
 
     def __str__(self):
         return f"{self.__class__.__name__}({self.type}, {repr(self.value)}, {self.lcpos}, {self.lexpos})"
 
 
-# --
-
-# def group(*choices): return '(' + '|'.join(choices) + ')'
-# def maybe(*choices): return group(*choices) + '?'
-
-# --
-
 literal_type_map = {
-    '>': 'GREATER',
-    '{': 'LBRACE',
-    '<': 'LESS',
-    '(': 'LPAR',
-    '[': 'LSQB',
-    '-': 'MINUS',
-    '+': 'PLUS',
-    '}': 'RBRACE',
-    ')': 'RPAR',
-    ']': 'RSQB',
-    ';': 'SEMICOLON',
-    '*': 'ASTERISK',
-    '|': 'VBAR',
-    '?': 'OPTIONAL',
-    '.': 'DOT',
+    "{": "LBRACE",
+    "(": "LPAR",
+    "[": "LSQB",
+    "-": "MINUS",
+    "+": "PLUS",
+    "}": "RBRACE",
+    ")": "RPAR",
+    "]": "RSQB",
+    ";": "SEMICOLON",
+    "*": "ASTERISK",
+    "|": "VBAR",
+    "?": "OPTIONAL",
+    ".": "DOT",
     # "...": "ELLIPSIS",
+    # "<": "LESS",
+    # ">": "GREATER",
 }
 
 
 class REBNFLexer(object):
     """
     This class describes a rebnf lexer.
     """
@@ -122,49 +115,48 @@
         return t
 
     @lex.TOKEN("|".join(re.escape(k) for k in literal_type_map.keys()))
     def t_LITERAL(self, t):
         t.type = literal_type_map.get(t.value)
         return t
 
-    # @lex.TOKEN('|'.join([
-    #     r"import\ +(\w+(?:\ +as\ +\w+)?)",
-    #     r"from\ +(\.*\w+(?:\.\w+)*)\ +import\ +(\w+(?:\ +as\ +\w+)?(?:,\ *\w+(?:\ +as\ +\w+)?)*)\ *",
-    #     r"from\ +(\.*\w+(?:\.\w+)*)\ +import\ +\(\s+(\w+(?:\ +as\ +\w+)?(?:,\s+\w+(?:\ +as\ +\w+)?)*)\ *",
-    # ]))
-    # def t_IMPORT(self, t):
-    #     return t
-
     def t_NAME(self, t):
         r"<[a-zA-Z][a-zA-Z0-9_]*>|[a-zA-Z][a-zA-Z0-9_]*"
         # support for optional identifier enclosures
         if t.value.startswith("<") and t.value.endswith(">"):
             t.value = t.value[1:-1]
         return t
 
-    # def t_SYMBOL(self, t):
-    #     r"<|>|-|\n|\t|\r|\f|\b"
-    #     return t
-
-    def find_column(self, data, token):
-        line_start = data.rfind("\n", 0, token.lexpos) + 1
-        return (token.lexpos - line_start) + 1
+    def find_column(self, lexdata, lexpos):
+        line_start = lexdata.rfind("\n", 0, lexpos) + 1
+        return (lexpos - line_start) + 1
 
     def t_error(self, t):
         print(
-            f"\033[91mlexer error: at line {t.lineno}, column {self.find_column(t.lexer.lexdata, t)}, unexpected token {repr(t.value[0])}\033[0m"
+            f"\033[91mlexer error: at line {t.lineno}, "
+            f"column {self.find_column(t.lexer.lexdata, t.lexpos)}, "
+            f"unexpected token {repr(t.value[0])}\033[0m"
         )
         exit(1)
 
     def __init__(self):
         self.lexer = lex.lex(module=self)
 
     def token(self):
         return self.lexer.token()
 
     def tokenize(self, code):
+        """
+        Tokenizes the given code
+
+        :param      code:  The code to be tokenized
+        :type       code:  str
+
+        :returns:   A list of tokens
+        :rtype:     list[Token]
+        """
         self.lexer.input(code)
         output = list()
         while tok := self.lexer.token():
-            tok.column = self.find_column(self.lexer.lexdata, tok)
+            tok.column = self.find_column(self.lexer.lexdata, tok.lexpos)
             output.append(Token(tok))
         return output
```

### Comparing `rebnf-0.7/rebnf/parser.out` & `rebnf-0.8/rebnf/parser.out`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 Created by PLY version 3.11 (http://www.dabeaz.com/ply)
 
-Unused terminals:
-
-    GREATER
-    LESS
-
 Grammar
 
 Rule 0     S' -> start
 Rule 1     start -> grammar start
 Rule 2     start -> grammar
 Rule 3     grammar -> comment
 Rule 4     grammar -> import
@@ -43,79 +38,77 @@
 Rule 33    rhs -> factor rhs
 Rule 34    rhs -> factor
 Rule 35    factor -> term OPTIONAL
 Rule 36    factor -> term ASTERISK
 Rule 37    factor -> term PLUS
 Rule 38    factor -> term MINUS term
 Rule 39    factor -> term
-Rule 40    term_group -> factor NEWLINE VBAR term_group
-Rule 41    term_group -> factor VBAR term_group
-Rule 42    term_group -> factor term_group
-Rule 43    term_group -> factor
-Rule 44    term -> LPAR term_group RPAR
-Rule 45    term -> LSQB term_group RSQB
-Rule 46    term -> LBRACE term_group RBRACE
-Rule 47    term -> regex
-Rule 48    term -> string
-Rule 49    term -> name
+Rule 40    term -> LPAR term_group RPAR
+Rule 41    term -> LSQB term_group RSQB
+Rule 42    term -> LBRACE term_group RBRACE
+Rule 43    term -> regex
+Rule 44    term -> string
+Rule 45    term -> name
+Rule 46    term_group -> factor NEWLINE VBAR term_group
+Rule 47    term_group -> factor VBAR term_group
+Rule 48    term_group -> factor term_group
+Rule 49    term_group -> factor
 Rule 50    regex -> REGEX
 Rule 51    string -> STRING
 Rule 52    name -> NAME
 Rule 53    terminator -> SEMICOLON
 Rule 54    terminator -> DOT
 
 Terminals, with rules where they appear
 
 ,                    : 23
 ASSIGN               : 28 29
 ASTERISK             : 15 36
 COMMENT              : 9
 DOT                  : 19 20 21 54
-GREATER              : 
-LBRACE               : 46
-LESS                 : 
-LPAR                 : 27 44
-LSQB                 : 45
+LBRACE               : 42
+LPAR                 : 27 40
+LSQB                 : 41
 MINUS                : 38
 NAME                 : 14 15 15 16 16 21 22 25 25 25 26 28 29 52
-NEWLINE              : 7 8 27 27 30 32 40
+NEWLINE              : 7 8 27 27 30 32 46
 OPTIONAL             : 35
 PLUS                 : 37
-RBRACE               : 46
+RBRACE               : 42
 REGEX                : 50
-RPAR                 : 27 44
-RSQB                 : 45
+RPAR                 : 27 40
+RSQB                 : 41
 SEMICOLON            : 53
 STRING               : 51
-VBAR                 : 30 31 40 41
+VBAR                 : 30 31 46 47
 error                : 
 
 Nonterminals, with rules where they appear
 
 comment              : 3
 dots                 : 17 19
 dotted_name          : 15 16
-factor               : 30 31 32 33 34 40 41 42 43
+factor               : 30 31 32 33 34 46 47 48 49
 from_statement       : 12 13
 grammar              : 1 2
 import               : 4
 import_items         : 14 16 23
 import_items_multiline : 
 import_name          : 23 24 27
 import_statement     : 10 11
-name                 : 49
+name                 : 45
 name_parts           : 17 18 21
 newline              : 6 7 10 12
-regex                : 47
+regex                : 43
 rhs                  : 28 29 30 31 33
 rule                 : 5
 start                : 1 0
-string               : 48
+string               : 44
 term                 : 35 36 37 38 38 39
-term_group           : 40 41 42 44 45 46
+term_group           : 40 41 42 46 47 48
 terminator           : 28
 
 Parsing method: LALR
 
 state 0
 
     (0) S' -> . start
@@ -380,20 +373,20 @@
     (33) rhs -> . factor rhs
     (34) rhs -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -548,20 +541,20 @@
     (33) rhs -> . factor rhs
     (34) rhs -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
   ! shift/reduce conflict for NEWLINE resolved as shift
   ! shift/reduce conflict for NAME resolved as shift
     NEWLINE         shift and go to state 48
@@ -614,30 +607,30 @@
     RPAR            reduce using rule 39 (factor -> term .)
     RSQB            reduce using rule 39 (factor -> term .)
     RBRACE          reduce using rule 39 (factor -> term .)
 
 
 state 30
 
-    (44) term -> LPAR . term_group RPAR
-    (40) term_group -> . factor NEWLINE VBAR term_group
-    (41) term_group -> . factor VBAR term_group
-    (42) term_group -> . factor term_group
-    (43) term_group -> . factor
+    (40) term -> LPAR . term_group RPAR
+    (46) term_group -> . factor NEWLINE VBAR term_group
+    (47) term_group -> . factor VBAR term_group
+    (48) term_group -> . factor term_group
+    (49) term_group -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -650,30 +643,30 @@
     term                           shift and go to state 29
     regex                          shift and go to state 33
     string                         shift and go to state 34
     name                           shift and go to state 35
 
 state 31
 
-    (45) term -> LSQB . term_group RSQB
-    (40) term_group -> . factor NEWLINE VBAR term_group
-    (41) term_group -> . factor VBAR term_group
-    (42) term_group -> . factor term_group
-    (43) term_group -> . factor
+    (41) term -> LSQB . term_group RSQB
+    (46) term_group -> . factor NEWLINE VBAR term_group
+    (47) term_group -> . factor VBAR term_group
+    (48) term_group -> . factor term_group
+    (49) term_group -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -686,30 +679,30 @@
     term                           shift and go to state 29
     regex                          shift and go to state 33
     string                         shift and go to state 34
     name                           shift and go to state 35
 
 state 32
 
-    (46) term -> LBRACE . term_group RBRACE
-    (40) term_group -> . factor NEWLINE VBAR term_group
-    (41) term_group -> . factor VBAR term_group
-    (42) term_group -> . factor term_group
-    (43) term_group -> . factor
+    (42) term -> LBRACE . term_group RBRACE
+    (46) term_group -> . factor NEWLINE VBAR term_group
+    (47) term_group -> . factor VBAR term_group
+    (48) term_group -> . factor term_group
+    (49) term_group -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -722,85 +715,85 @@
     term                           shift and go to state 29
     regex                          shift and go to state 33
     string                         shift and go to state 34
     name                           shift and go to state 35
 
 state 33
 
-    (47) term -> regex .
+    (43) term -> regex .
 
-    OPTIONAL        reduce using rule 47 (term -> regex .)
-    ASTERISK        reduce using rule 47 (term -> regex .)
-    PLUS            reduce using rule 47 (term -> regex .)
-    MINUS           reduce using rule 47 (term -> regex .)
-    NEWLINE         reduce using rule 47 (term -> regex .)
-    VBAR            reduce using rule 47 (term -> regex .)
-    LPAR            reduce using rule 47 (term -> regex .)
-    LSQB            reduce using rule 47 (term -> regex .)
-    LBRACE          reduce using rule 47 (term -> regex .)
-    REGEX           reduce using rule 47 (term -> regex .)
-    STRING          reduce using rule 47 (term -> regex .)
-    NAME            reduce using rule 47 (term -> regex .)
-    SEMICOLON       reduce using rule 47 (term -> regex .)
-    DOT             reduce using rule 47 (term -> regex .)
-    COMMENT         reduce using rule 47 (term -> regex .)
-    $end            reduce using rule 47 (term -> regex .)
-    RPAR            reduce using rule 47 (term -> regex .)
-    RSQB            reduce using rule 47 (term -> regex .)
-    RBRACE          reduce using rule 47 (term -> regex .)
+    OPTIONAL        reduce using rule 43 (term -> regex .)
+    ASTERISK        reduce using rule 43 (term -> regex .)
+    PLUS            reduce using rule 43 (term -> regex .)
+    MINUS           reduce using rule 43 (term -> regex .)
+    NEWLINE         reduce using rule 43 (term -> regex .)
+    VBAR            reduce using rule 43 (term -> regex .)
+    LPAR            reduce using rule 43 (term -> regex .)
+    LSQB            reduce using rule 43 (term -> regex .)
+    LBRACE          reduce using rule 43 (term -> regex .)
+    REGEX           reduce using rule 43 (term -> regex .)
+    STRING          reduce using rule 43 (term -> regex .)
+    NAME            reduce using rule 43 (term -> regex .)
+    SEMICOLON       reduce using rule 43 (term -> regex .)
+    DOT             reduce using rule 43 (term -> regex .)
+    COMMENT         reduce using rule 43 (term -> regex .)
+    $end            reduce using rule 43 (term -> regex .)
+    RPAR            reduce using rule 43 (term -> regex .)
+    RSQB            reduce using rule 43 (term -> regex .)
+    RBRACE          reduce using rule 43 (term -> regex .)
 
 
 state 34
 
-    (48) term -> string .
+    (44) term -> string .
 
-    OPTIONAL        reduce using rule 48 (term -> string .)
-    ASTERISK        reduce using rule 48 (term -> string .)
-    PLUS            reduce using rule 48 (term -> string .)
-    MINUS           reduce using rule 48 (term -> string .)
-    NEWLINE         reduce using rule 48 (term -> string .)
-    VBAR            reduce using rule 48 (term -> string .)
-    LPAR            reduce using rule 48 (term -> string .)
-    LSQB            reduce using rule 48 (term -> string .)
-    LBRACE          reduce using rule 48 (term -> string .)
-    REGEX           reduce using rule 48 (term -> string .)
-    STRING          reduce using rule 48 (term -> string .)
-    NAME            reduce using rule 48 (term -> string .)
-    SEMICOLON       reduce using rule 48 (term -> string .)
-    DOT             reduce using rule 48 (term -> string .)
-    COMMENT         reduce using rule 48 (term -> string .)
-    $end            reduce using rule 48 (term -> string .)
-    RPAR            reduce using rule 48 (term -> string .)
-    RSQB            reduce using rule 48 (term -> string .)
-    RBRACE          reduce using rule 48 (term -> string .)
+    OPTIONAL        reduce using rule 44 (term -> string .)
+    ASTERISK        reduce using rule 44 (term -> string .)
+    PLUS            reduce using rule 44 (term -> string .)
+    MINUS           reduce using rule 44 (term -> string .)
+    NEWLINE         reduce using rule 44 (term -> string .)
+    VBAR            reduce using rule 44 (term -> string .)
+    LPAR            reduce using rule 44 (term -> string .)
+    LSQB            reduce using rule 44 (term -> string .)
+    LBRACE          reduce using rule 44 (term -> string .)
+    REGEX           reduce using rule 44 (term -> string .)
+    STRING          reduce using rule 44 (term -> string .)
+    NAME            reduce using rule 44 (term -> string .)
+    SEMICOLON       reduce using rule 44 (term -> string .)
+    DOT             reduce using rule 44 (term -> string .)
+    COMMENT         reduce using rule 44 (term -> string .)
+    $end            reduce using rule 44 (term -> string .)
+    RPAR            reduce using rule 44 (term -> string .)
+    RSQB            reduce using rule 44 (term -> string .)
+    RBRACE          reduce using rule 44 (term -> string .)
 
 
 state 35
 
-    (49) term -> name .
+    (45) term -> name .
 
-    OPTIONAL        reduce using rule 49 (term -> name .)
-    ASTERISK        reduce using rule 49 (term -> name .)
-    PLUS            reduce using rule 49 (term -> name .)
-    MINUS           reduce using rule 49 (term -> name .)
-    NEWLINE         reduce using rule 49 (term -> name .)
-    VBAR            reduce using rule 49 (term -> name .)
-    LPAR            reduce using rule 49 (term -> name .)
-    LSQB            reduce using rule 49 (term -> name .)
-    LBRACE          reduce using rule 49 (term -> name .)
-    REGEX           reduce using rule 49 (term -> name .)
-    STRING          reduce using rule 49 (term -> name .)
-    NAME            reduce using rule 49 (term -> name .)
-    SEMICOLON       reduce using rule 49 (term -> name .)
-    DOT             reduce using rule 49 (term -> name .)
-    COMMENT         reduce using rule 49 (term -> name .)
-    $end            reduce using rule 49 (term -> name .)
-    RPAR            reduce using rule 49 (term -> name .)
-    RSQB            reduce using rule 49 (term -> name .)
-    RBRACE          reduce using rule 49 (term -> name .)
+    OPTIONAL        reduce using rule 45 (term -> name .)
+    ASTERISK        reduce using rule 45 (term -> name .)
+    PLUS            reduce using rule 45 (term -> name .)
+    MINUS           reduce using rule 45 (term -> name .)
+    NEWLINE         reduce using rule 45 (term -> name .)
+    VBAR            reduce using rule 45 (term -> name .)
+    LPAR            reduce using rule 45 (term -> name .)
+    LSQB            reduce using rule 45 (term -> name .)
+    LBRACE          reduce using rule 45 (term -> name .)
+    REGEX           reduce using rule 45 (term -> name .)
+    STRING          reduce using rule 45 (term -> name .)
+    NAME            reduce using rule 45 (term -> name .)
+    SEMICOLON       reduce using rule 45 (term -> name .)
+    DOT             reduce using rule 45 (term -> name .)
+    COMMENT         reduce using rule 45 (term -> name .)
+    $end            reduce using rule 45 (term -> name .)
+    RPAR            reduce using rule 45 (term -> name .)
+    RSQB            reduce using rule 45 (term -> name .)
+    RBRACE          reduce using rule 45 (term -> name .)
 
 
 state 36
 
     (50) regex -> REGEX .
 
     OPTIONAL        reduce using rule 50 (regex -> REGEX .)
@@ -971,20 +964,20 @@
     (33) rhs -> . factor rhs
     (34) rhs -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -1073,20 +1066,20 @@
     RSQB            reduce using rule 37 (factor -> term PLUS .)
     RBRACE          reduce using rule 37 (factor -> term PLUS .)
 
 
 state 54
 
     (38) factor -> term MINUS . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -1097,49 +1090,49 @@
     term                           shift and go to state 65
     regex                          shift and go to state 33
     string                         shift and go to state 34
     name                           shift and go to state 35
 
 state 55
 
-    (44) term -> LPAR term_group . RPAR
+    (40) term -> LPAR term_group . RPAR
 
     RPAR            shift and go to state 66
 
 
 state 56
 
-    (40) term_group -> factor . NEWLINE VBAR term_group
-    (41) term_group -> factor . VBAR term_group
-    (42) term_group -> factor . term_group
-    (43) term_group -> factor .
-    (40) term_group -> . factor NEWLINE VBAR term_group
-    (41) term_group -> . factor VBAR term_group
-    (42) term_group -> . factor term_group
-    (43) term_group -> . factor
+    (46) term_group -> factor . NEWLINE VBAR term_group
+    (47) term_group -> factor . VBAR term_group
+    (48) term_group -> factor . term_group
+    (49) term_group -> factor .
+    (46) term_group -> . factor NEWLINE VBAR term_group
+    (47) term_group -> . factor VBAR term_group
+    (48) term_group -> . factor term_group
+    (49) term_group -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     NEWLINE         shift and go to state 67
     VBAR            shift and go to state 68
-    RPAR            reduce using rule 43 (term_group -> factor .)
-    RSQB            reduce using rule 43 (term_group -> factor .)
-    RBRACE          reduce using rule 43 (term_group -> factor .)
+    RPAR            reduce using rule 49 (term_group -> factor .)
+    RSQB            reduce using rule 49 (term_group -> factor .)
+    RBRACE          reduce using rule 49 (term_group -> factor .)
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
     REGEX           shift and go to state 36
     STRING          shift and go to state 37
     NAME            shift and go to state 26
 
@@ -1148,22 +1141,22 @@
     term                           shift and go to state 29
     regex                          shift and go to state 33
     string                         shift and go to state 34
     name                           shift and go to state 35
 
 state 57
 
-    (45) term -> LSQB term_group . RSQB
+    (41) term -> LSQB term_group . RSQB
 
     RSQB            shift and go to state 70
 
 
 state 58
 
-    (46) term -> LBRACE term_group . RBRACE
+    (42) term -> LBRACE term_group . RBRACE
 
     RBRACE          shift and go to state 71
 
 
 state 59
 
     (25) import_name -> NAME . NAME NAME
@@ -1218,20 +1211,20 @@
     (33) rhs -> . factor rhs
     (34) rhs -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -1277,62 +1270,62 @@
     RPAR            reduce using rule 38 (factor -> term MINUS term .)
     RSQB            reduce using rule 38 (factor -> term MINUS term .)
     RBRACE          reduce using rule 38 (factor -> term MINUS term .)
 
 
 state 66
 
-    (44) term -> LPAR term_group RPAR .
+    (40) term -> LPAR term_group RPAR .
 
-    OPTIONAL        reduce using rule 44 (term -> LPAR term_group RPAR .)
-    ASTERISK        reduce using rule 44 (term -> LPAR term_group RPAR .)
-    PLUS            reduce using rule 44 (term -> LPAR term_group RPAR .)
-    MINUS           reduce using rule 44 (term -> LPAR term_group RPAR .)
-    NEWLINE         reduce using rule 44 (term -> LPAR term_group RPAR .)
-    VBAR            reduce using rule 44 (term -> LPAR term_group RPAR .)
-    LPAR            reduce using rule 44 (term -> LPAR term_group RPAR .)
-    LSQB            reduce using rule 44 (term -> LPAR term_group RPAR .)
-    LBRACE          reduce using rule 44 (term -> LPAR term_group RPAR .)
-    REGEX           reduce using rule 44 (term -> LPAR term_group RPAR .)
-    STRING          reduce using rule 44 (term -> LPAR term_group RPAR .)
-    NAME            reduce using rule 44 (term -> LPAR term_group RPAR .)
-    SEMICOLON       reduce using rule 44 (term -> LPAR term_group RPAR .)
-    DOT             reduce using rule 44 (term -> LPAR term_group RPAR .)
-    COMMENT         reduce using rule 44 (term -> LPAR term_group RPAR .)
-    $end            reduce using rule 44 (term -> LPAR term_group RPAR .)
-    RPAR            reduce using rule 44 (term -> LPAR term_group RPAR .)
-    RSQB            reduce using rule 44 (term -> LPAR term_group RPAR .)
-    RBRACE          reduce using rule 44 (term -> LPAR term_group RPAR .)
+    OPTIONAL        reduce using rule 40 (term -> LPAR term_group RPAR .)
+    ASTERISK        reduce using rule 40 (term -> LPAR term_group RPAR .)
+    PLUS            reduce using rule 40 (term -> LPAR term_group RPAR .)
+    MINUS           reduce using rule 40 (term -> LPAR term_group RPAR .)
+    NEWLINE         reduce using rule 40 (term -> LPAR term_group RPAR .)
+    VBAR            reduce using rule 40 (term -> LPAR term_group RPAR .)
+    LPAR            reduce using rule 40 (term -> LPAR term_group RPAR .)
+    LSQB            reduce using rule 40 (term -> LPAR term_group RPAR .)
+    LBRACE          reduce using rule 40 (term -> LPAR term_group RPAR .)
+    REGEX           reduce using rule 40 (term -> LPAR term_group RPAR .)
+    STRING          reduce using rule 40 (term -> LPAR term_group RPAR .)
+    NAME            reduce using rule 40 (term -> LPAR term_group RPAR .)
+    SEMICOLON       reduce using rule 40 (term -> LPAR term_group RPAR .)
+    DOT             reduce using rule 40 (term -> LPAR term_group RPAR .)
+    COMMENT         reduce using rule 40 (term -> LPAR term_group RPAR .)
+    $end            reduce using rule 40 (term -> LPAR term_group RPAR .)
+    RPAR            reduce using rule 40 (term -> LPAR term_group RPAR .)
+    RSQB            reduce using rule 40 (term -> LPAR term_group RPAR .)
+    RBRACE          reduce using rule 40 (term -> LPAR term_group RPAR .)
 
 
 state 67
 
-    (40) term_group -> factor NEWLINE . VBAR term_group
+    (46) term_group -> factor NEWLINE . VBAR term_group
 
     VBAR            shift and go to state 73
 
 
 state 68
 
-    (41) term_group -> factor VBAR . term_group
-    (40) term_group -> . factor NEWLINE VBAR term_group
-    (41) term_group -> . factor VBAR term_group
-    (42) term_group -> . factor term_group
-    (43) term_group -> . factor
+    (47) term_group -> factor VBAR . term_group
+    (46) term_group -> . factor NEWLINE VBAR term_group
+    (47) term_group -> . factor VBAR term_group
+    (48) term_group -> . factor term_group
+    (49) term_group -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -1345,69 +1338,69 @@
     term                           shift and go to state 29
     regex                          shift and go to state 33
     string                         shift and go to state 34
     name                           shift and go to state 35
 
 state 69
 
-    (42) term_group -> factor term_group .
+    (48) term_group -> factor term_group .
 
-    RPAR            reduce using rule 42 (term_group -> factor term_group .)
-    RSQB            reduce using rule 42 (term_group -> factor term_group .)
-    RBRACE          reduce using rule 42 (term_group -> factor term_group .)
+    RPAR            reduce using rule 48 (term_group -> factor term_group .)
+    RSQB            reduce using rule 48 (term_group -> factor term_group .)
+    RBRACE          reduce using rule 48 (term_group -> factor term_group .)
 
 
 state 70
 
-    (45) term -> LSQB term_group RSQB .
+    (41) term -> LSQB term_group RSQB .
 
-    OPTIONAL        reduce using rule 45 (term -> LSQB term_group RSQB .)
-    ASTERISK        reduce using rule 45 (term -> LSQB term_group RSQB .)
-    PLUS            reduce using rule 45 (term -> LSQB term_group RSQB .)
-    MINUS           reduce using rule 45 (term -> LSQB term_group RSQB .)
-    NEWLINE         reduce using rule 45 (term -> LSQB term_group RSQB .)
-    VBAR            reduce using rule 45 (term -> LSQB term_group RSQB .)
-    LPAR            reduce using rule 45 (term -> LSQB term_group RSQB .)
-    LSQB            reduce using rule 45 (term -> LSQB term_group RSQB .)
-    LBRACE          reduce using rule 45 (term -> LSQB term_group RSQB .)
-    REGEX           reduce using rule 45 (term -> LSQB term_group RSQB .)
-    STRING          reduce using rule 45 (term -> LSQB term_group RSQB .)
-    NAME            reduce using rule 45 (term -> LSQB term_group RSQB .)
-    SEMICOLON       reduce using rule 45 (term -> LSQB term_group RSQB .)
-    DOT             reduce using rule 45 (term -> LSQB term_group RSQB .)
-    COMMENT         reduce using rule 45 (term -> LSQB term_group RSQB .)
-    $end            reduce using rule 45 (term -> LSQB term_group RSQB .)
-    RPAR            reduce using rule 45 (term -> LSQB term_group RSQB .)
-    RSQB            reduce using rule 45 (term -> LSQB term_group RSQB .)
-    RBRACE          reduce using rule 45 (term -> LSQB term_group RSQB .)
+    OPTIONAL        reduce using rule 41 (term -> LSQB term_group RSQB .)
+    ASTERISK        reduce using rule 41 (term -> LSQB term_group RSQB .)
+    PLUS            reduce using rule 41 (term -> LSQB term_group RSQB .)
+    MINUS           reduce using rule 41 (term -> LSQB term_group RSQB .)
+    NEWLINE         reduce using rule 41 (term -> LSQB term_group RSQB .)
+    VBAR            reduce using rule 41 (term -> LSQB term_group RSQB .)
+    LPAR            reduce using rule 41 (term -> LSQB term_group RSQB .)
+    LSQB            reduce using rule 41 (term -> LSQB term_group RSQB .)
+    LBRACE          reduce using rule 41 (term -> LSQB term_group RSQB .)
+    REGEX           reduce using rule 41 (term -> LSQB term_group RSQB .)
+    STRING          reduce using rule 41 (term -> LSQB term_group RSQB .)
+    NAME            reduce using rule 41 (term -> LSQB term_group RSQB .)
+    SEMICOLON       reduce using rule 41 (term -> LSQB term_group RSQB .)
+    DOT             reduce using rule 41 (term -> LSQB term_group RSQB .)
+    COMMENT         reduce using rule 41 (term -> LSQB term_group RSQB .)
+    $end            reduce using rule 41 (term -> LSQB term_group RSQB .)
+    RPAR            reduce using rule 41 (term -> LSQB term_group RSQB .)
+    RSQB            reduce using rule 41 (term -> LSQB term_group RSQB .)
+    RBRACE          reduce using rule 41 (term -> LSQB term_group RSQB .)
 
 
 state 71
 
-    (46) term -> LBRACE term_group RBRACE .
+    (42) term -> LBRACE term_group RBRACE .
 
-    OPTIONAL        reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    ASTERISK        reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    PLUS            reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    MINUS           reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    NEWLINE         reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    VBAR            reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    LPAR            reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    LSQB            reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    LBRACE          reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    REGEX           reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    STRING          reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    NAME            reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    SEMICOLON       reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    DOT             reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    COMMENT         reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    $end            reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    RPAR            reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    RSQB            reduce using rule 46 (term -> LBRACE term_group RBRACE .)
-    RBRACE          reduce using rule 46 (term -> LBRACE term_group RBRACE .)
+    OPTIONAL        reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    ASTERISK        reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    PLUS            reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    MINUS           reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    NEWLINE         reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    VBAR            reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    LPAR            reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    LSQB            reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    LBRACE          reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    REGEX           reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    STRING          reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    NAME            reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    SEMICOLON       reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    DOT             reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    COMMENT         reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    $end            reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    RPAR            reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    RSQB            reduce using rule 42 (term -> LBRACE term_group RBRACE .)
+    RBRACE          reduce using rule 42 (term -> LBRACE term_group RBRACE .)
 
 
 state 72
 
     (30) rhs -> factor NEWLINE VBAR rhs .
 
     SEMICOLON       reduce using rule 30 (rhs -> factor NEWLINE VBAR rhs .)
@@ -1416,30 +1409,30 @@
     NAME            reduce using rule 30 (rhs -> factor NEWLINE VBAR rhs .)
     NEWLINE         reduce using rule 30 (rhs -> factor NEWLINE VBAR rhs .)
     $end            reduce using rule 30 (rhs -> factor NEWLINE VBAR rhs .)
 
 
 state 73
 
-    (40) term_group -> factor NEWLINE VBAR . term_group
-    (40) term_group -> . factor NEWLINE VBAR term_group
-    (41) term_group -> . factor VBAR term_group
-    (42) term_group -> . factor term_group
-    (43) term_group -> . factor
+    (46) term_group -> factor NEWLINE VBAR . term_group
+    (46) term_group -> . factor NEWLINE VBAR term_group
+    (47) term_group -> . factor VBAR term_group
+    (48) term_group -> . factor term_group
+    (49) term_group -> . factor
     (35) factor -> . term OPTIONAL
     (36) factor -> . term ASTERISK
     (37) factor -> . term PLUS
     (38) factor -> . term MINUS term
     (39) factor -> . term
-    (44) term -> . LPAR term_group RPAR
-    (45) term -> . LSQB term_group RSQB
-    (46) term -> . LBRACE term_group RBRACE
-    (47) term -> . regex
-    (48) term -> . string
-    (49) term -> . name
+    (40) term -> . LPAR term_group RPAR
+    (41) term -> . LSQB term_group RSQB
+    (42) term -> . LBRACE term_group RBRACE
+    (43) term -> . regex
+    (44) term -> . string
+    (45) term -> . name
     (50) regex -> . REGEX
     (51) string -> . STRING
     (52) name -> . NAME
 
     LPAR            shift and go to state 30
     LSQB            shift and go to state 31
     LBRACE          shift and go to state 32
@@ -1452,28 +1445,28 @@
     term                           shift and go to state 29
     regex                          shift and go to state 33
     string                         shift and go to state 34
     name                           shift and go to state 35
 
 state 74
 
-    (41) term_group -> factor VBAR term_group .
+    (47) term_group -> factor VBAR term_group .
 
-    RPAR            reduce using rule 41 (term_group -> factor VBAR term_group .)
-    RSQB            reduce using rule 41 (term_group -> factor VBAR term_group .)
-    RBRACE          reduce using rule 41 (term_group -> factor VBAR term_group .)
+    RPAR            reduce using rule 47 (term_group -> factor VBAR term_group .)
+    RSQB            reduce using rule 47 (term_group -> factor VBAR term_group .)
+    RBRACE          reduce using rule 47 (term_group -> factor VBAR term_group .)
 
 
 state 75
 
-    (40) term_group -> factor NEWLINE VBAR term_group .
+    (46) term_group -> factor NEWLINE VBAR term_group .
 
-    RPAR            reduce using rule 40 (term_group -> factor NEWLINE VBAR term_group .)
-    RSQB            reduce using rule 40 (term_group -> factor NEWLINE VBAR term_group .)
-    RBRACE          reduce using rule 40 (term_group -> factor NEWLINE VBAR term_group .)
+    RPAR            reduce using rule 46 (term_group -> factor NEWLINE VBAR term_group .)
+    RSQB            reduce using rule 46 (term_group -> factor NEWLINE VBAR term_group .)
+    RBRACE          reduce using rule 46 (term_group -> factor NEWLINE VBAR term_group .)
 
 WARNING: 
 WARNING: Conflicts:
 WARNING: 
 WARNING: shift/reduce conflict for NEWLINE in state 8 resolved as shift
 WARNING: shift/reduce conflict for NEWLINE in state 9 resolved as shift
 WARNING: shift/reduce conflict for NEWLINE in state 11 resolved as shift
```

### Comparing `rebnf-0.7/rebnf/parsers.py` & `rebnf-0.8/rebnf/parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,73 +23,74 @@
 class REBNFParser:
     """
     This class describes a rebnf parser.
     """
 
     tokens = lexers.REBNFLexer.tokens
 
-    def __init__(self):
+    def __init__(self, debug=False, **kwargs):
         self.lexer = lexers.REBNFLexer()
-        self.parser = yacc.yacc(module=self)
-        # self.parser = yacc.yacc(module=self, debuglog=yacc.NullLogger())
-        self.ast = []
+        if not debug:
+            kwargs.update(debuglog=yacc.NullLogger())
+        self.parser = yacc.yacc(module=self, **kwargs)
+        self.ast = ()
 
     def p_start(self, p):
         """
         start : grammar start
               | grammar
         """
         p[0] = self.ast
 
     def p_grammar(self, p):
-        '''
+        """
         grammar : comment
                 | import
                 | rule
                 | newline
-        '''
+        """
         if p[1]:
-            self.ast += p[1],
+            self.ast += (p[1],)
 
     def p_newline(self, p):
-        '''
+        """
         newline : NEWLINE newline
                 | NEWLINE
-        '''
+        """
         pass
 
     def p_comment(self, p):
-        '''
+        """
         comment : COMMENT
-        '''
-        p[0] = ('COMMENT', p[1])
+        """
+        p[0] = ("COMMENT", p[1])
 
     # -- IMPORTS --
 
     def p_import(self, p):
-        '''
+        """
         import : import_statement newline
                | import_statement
                | from_statement newline
                | from_statement
-        '''
-        p[0] = ('IMPORT', p[1])
+        """
+        p[0] = ("IMPORT", p[1])
 
     def p_import_statement(self, p):
-        '''
+        """
         import_statement : NAME import_items
-        '''
-        if p[1] == 'import':
+        """
+        if p[1] == "import":
             p[0] = tuple(p[1:])
 
     def p_from_statement(self, p):
-        '''
+        """
         from_statement : NAME dotted_name NAME ASTERISK
                        | NAME dotted_name NAME import_items
-        '''
+        """
         if p[1] == "from" and p[3] == "import":
             p[0] = tuple(p[1:])
 
     def p_dotted_name(self, p):
         """
         dotted_name : dots name_parts
                     | name_parts
@@ -107,153 +108,166 @@
         """
         name_parts : NAME DOT name_parts
                    | NAME
         """
         p[0] = "".join(p[1:])
 
     def p_import_items(self, p):
-        '''
+        """
         import_items : import_name "," import_items
                      | import_name
-        '''
+        """
         if len(p) == 3:
             p[0] = itertools.chain.from_iterable([p[1], p[2]])
         if len(p) == 2:
             p[0] = p[1]
 
     def p_import_name(self, p):
-        '''
+        """
         import_name : NAME NAME NAME
                     | NAME
-        '''
+        """
         if len(p) == 4 and p[2] == "as":
             # ensure import names / aliases are lower case
             if p[1].islower() and p[3].islower():
-                p[0] = [p[1], p[3]]
+                p[0] = (p[1], p[3])
         elif len(p) == 2 and p[1].islower():
             p[0] = p[1]
 
     def p_import_items_multiline(self, p):
-        '''
+        """
         import_items_multiline : LPAR NEWLINE import_name NEWLINE RPAR
-        '''
+        """
 
     # -- RULES --
 
     def p_rule(self, p):
-        '''
+        """
         rule : NAME ASSIGN rhs terminator
              | NAME ASSIGN rhs
-        '''
-        p[0] = ('RULE', (p[1], p[3]))
+        """
+        p[0] = ("RULE", (p[1], p[3]))
 
     def p_rhs(self, p):
-        '''
+        """
         rhs : factor NEWLINE VBAR rhs
-            
             | factor VBAR rhs
-
             | factor NEWLINE
             | factor rhs
             | factor
-        '''
+        """
         if len(p) == 5:
             p[0] = (p[3], (p[1], p[4]))
         elif len(p) == 4:
             p[0] = (p[2], (p[1], p[3]))
         elif len(p) == 3:
-            p[0] = p[1]
             if isinstance(p[2], (list, tuple)):
                 p[0] = (p[1], p[2])
+            elif p[2] != "\n":
+                p[0] = (p[1], p[2])
             else:
-                if p[2] != "\n":
-                    p[0] = (p[1], p[2])
-                else:
-                    p[0] = p[1]
+                p[0] = p[1]
         elif len(p) == 2:
             p[0] = p[1]
 
     def p_factor(self, p):
         """
         factor : term OPTIONAL
                | term ASTERISK
                | term PLUS
                | term MINUS term
                | term
         """
         if len(p) == 4:
-            p[0] = [p[2], [p[1], p[3]]]
+            p[0] = (p[2], (p[1], p[3]))
         elif len(p) == 3:
-            p[0] =  [p[2], p[1]]
+            p[0] = (p[2], p[1])
         else:
             p[0] = p[1]
 
-    def p_term_group(self, p):
-        '''
-        term_group : factor NEWLINE VBAR term_group
-                   | factor VBAR term_group
-                   | factor term_group
-                   | factor
-        '''
-        if len(p) == 5:
-            p[0] = (p[3], [p[1], p[4]])
-        elif len(p) == 4:
-            p[0] = (p[2], [p[1], p[3]])
-        elif len(p) == 3:
-            p[0] = ('CONCAT', (p[1], p[2]))
-        elif len(p) == 2:
-            p[0] = p[1]
-
     def p_term(self, p):
         """
         term : LPAR term_group RPAR
              | LSQB term_group RSQB
              | LBRACE term_group RBRACE
              | regex
              | string
              | name
         """
         if len(p) == 4:
             p[0] = (lexers.literal_type_map.get(p[1]), p[2])
         elif len(p) == 2:
             p[0] = p[1]
 
+    def p_term_group(self, p):
+        """
+        term_group : factor NEWLINE VBAR term_group
+                   | factor VBAR term_group
+                   | factor term_group
+                   | factor
+        """
+        if len(p) == 5:
+            p[0] = (p[3], [p[1], p[4]])
+        elif len(p) == 4:
+            p[0] = (p[2], [p[1], p[3]])
+        elif len(p) == 3:
+            p[0] = (p[1], p[2])
+        elif len(p) == 2:
+            p[0] = p[1]
+
     def p_regex(self, p):
-        '''
+        """
         regex : REGEX
-        '''
-        p[0] = ('REGEX', p[1])
+        """
+        p[0] = ("REGEX", p[1])
 
     def p_string(self, p):
-        '''
+        """
         string : STRING
-        '''
-        p[0] = ('STRING', p[1])
+        """
+        p[0] = ("STRING", p[1])
 
     def p_name(self, p):
-        '''
+        """
         name : NAME
-        '''
-        p[0] = ('NAME', p[1])
+        """
+        p[0] = ("NAME", p[1])
 
     def p_terminator(self, p):
-        '''
+        """
         terminator : SEMICOLON
                    | DOT
-        '''
-        p[0] = ('TERMINATOR', p[1])
+        """
+        p[0] = ("TERMINATOR", p[1])
 
     def find_column(self, lexdata, lexpos):
         line_start = lexdata.rfind("\n", 0, lexpos) + 1
         return (lexpos - line_start) + 1
 
     def p_error(self, t):
         if t is not None:
-            print('error', self.parser.state)
+            print("error", self.parser.state)
             print(
                 f"\033[91msyntax error: at line {t.lineno}, column {self.find_column(t.lexer.lexdata, t.lexpos)}, unexpected token {repr(t.value[0])}\033[0m"
             )
             exit(1)
 
-    def parse(self, code, tracking=True):
+    def parse(self, code, tracking=True) -> tuple:
+        """
+        Parse the given code using a parser and return the abstract syntax tree
+
+        :param      code:      The code to be parsed
+        :type       code:      str
+        :param      tracking:  Flag indicating whether to enable tracking during
+                               parsing (default: True).
+        :type       tracking:  bool
+
+        :returns:   A tuple containing the abstract syntax tree (AST) of the
+                    parsed code.
+        :rtype:     tuple
+        """
+
+        # Call the parser's parse method to parse the code
         self.parser.parse(code, tracking=tracking)
+
+        # Return the abstract syntax tree (AST)
         return self.ast
```

### Comparing `rebnf-0.7/rebnf/parsetab.py` & `rebnf-0.8/rebnf/parsetab.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # parsetab.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'ASSIGN ASTERISK COMMENT DOT GREATER LBRACE LESS LPAR LSQB MINUS NAME NEWLINE OPTIONAL PLUS RBRACE REGEX RPAR RSQB SEMICOLON STRING VBAR\n        start : grammar start\n              | grammar\n        \n        grammar : comment\n                | import\n                | rule\n                | newline\n        \n        newline : NEWLINE newline\n                | NEWLINE\n        \n        comment : COMMENT\n        \n        import : import_statement newline\n               | import_statement\n               | from_statement newline\n               | from_statement\n        \n        import_statement : NAME import_items\n        \n        from_statement : NAME dotted_name NAME ASTERISK\n                       | NAME dotted_name NAME import_items\n        \n        dotted_name : dots name_parts\n                    | name_parts\n        \n        dots : DOT dots\n             | DOT\n        \n        name_parts : NAME DOT name_parts\n                   | NAME\n        \n        import_items : import_name "," import_items\n                     | import_name\n        \n        import_name : NAME NAME NAME\n                    | NAME\n        \n        import_items_multiline : LPAR NEWLINE import_name NEWLINE RPAR\n        \n        rule : NAME ASSIGN rhs terminator\n             | NAME ASSIGN rhs\n        \n        rhs : factor NEWLINE VBAR rhs\n            \n            | factor VBAR rhs\n\n            | factor NEWLINE\n            | factor rhs\n            | factor\n        \n        factor : term OPTIONAL\n               | term ASTERISK\n               | term PLUS\n               | term MINUS term\n               | term\n        \n        term_group : factor NEWLINE VBAR term_group\n                   | factor VBAR term_group\n                   | factor term_group\n                   | factor\n        \n        term : LPAR term_group RPAR\n             | LSQB term_group RSQB\n             | LBRACE term_group RBRACE\n             | regex\n             | string\n             | name\n        \n        regex : REGEX\n        \n        string : STRING\n        \n        name : NAME\n        \n        terminator : SEMICOLON\n                   | DOT\n        '
+_lr_signature = 'ASSIGN ASTERISK COMMENT DOT LBRACE LPAR LSQB MINUS NAME NEWLINE OPTIONAL PLUS RBRACE REGEX RPAR RSQB SEMICOLON STRING VBAR\n        start : grammar start\n              | grammar\n        \n        grammar : comment\n                | import\n                | rule\n                | newline\n        \n        newline : NEWLINE newline\n                | NEWLINE\n        \n        comment : COMMENT\n        \n        import : import_statement newline\n               | import_statement\n               | from_statement newline\n               | from_statement\n        \n        import_statement : NAME import_items\n        \n        from_statement : NAME dotted_name NAME ASTERISK\n                       | NAME dotted_name NAME import_items\n        \n        dotted_name : dots name_parts\n                    | name_parts\n        \n        dots : DOT dots\n             | DOT\n        \n        name_parts : NAME DOT name_parts\n                   | NAME\n        \n        import_items : import_name "," import_items\n                     | import_name\n        \n        import_name : NAME NAME NAME\n                    | NAME\n        \n        import_items_multiline : LPAR NEWLINE import_name NEWLINE RPAR\n        \n        rule : NAME ASSIGN rhs terminator\n             | NAME ASSIGN rhs\n        \n        rhs : factor NEWLINE VBAR rhs\n            | factor VBAR rhs\n            | factor NEWLINE\n            | factor rhs\n            | factor\n        \n        factor : term OPTIONAL\n               | term ASTERISK\n               | term PLUS\n               | term MINUS term\n               | term\n        \n        term : LPAR term_group RPAR\n             | LSQB term_group RSQB\n             | LBRACE term_group RBRACE\n             | regex\n             | string\n             | name\n        \n        term_group : factor NEWLINE VBAR term_group\n                   | factor VBAR term_group\n                   | factor term_group\n                   | factor\n        \n        regex : REGEX\n        \n        string : STRING\n        \n        name : NAME\n        \n        terminator : SEMICOLON\n                   | DOT\n        '
     
-_lr_action_items = {'COMMENT':([0,2,3,4,5,6,7,8,9,11,13,14,15,17,19,23,26,27,28,29,33,34,35,36,37,43,45,46,47,48,50,51,52,53,59,60,61,62,64,65,66,70,71,72,],[7,7,-3,-4,-5,-6,-9,-11,-13,-8,-10,-12,-26,-14,-24,-7,-52,-29,-34,-39,-47,-48,-49,-50,-51,-25,-28,-53,-54,-32,-33,-35,-36,-37,-26,-15,-16,-23,-31,-38,-44,-45,-46,-30,]),'NAME':([0,2,3,4,5,6,7,8,9,10,11,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,56,59,60,61,62,63,64,65,66,68,70,71,72,73,],[10,10,-3,-4,-5,-6,-9,-11,-13,15,-8,-10,-12,24,26,-14,38,-24,41,-18,-20,-7,43,41,-52,-29,26,-39,26,26,26,-47,-48,-49,-50,-51,59,59,-17,-22,-19,-25,-21,-28,-53,-54,-32,26,-33,-35,-36,-37,26,26,24,-15,-16,-23,26,-31,-38,-44,26,-45,-46,-30,26,]),'NEWLINE':([0,2,3,4,5,6,7,8,9,11,13,14,15,17,19,23,26,27,28,29,33,34,35,36,37,43,45,46,47,48,50,51,52,53,56,59,60,61,62,64,65,66,70,71,72,],[11,11,-3,-4,-5,-6,-9,11,11,11,-10,-12,-26,-14,-24,-7,-52,-29,48,-39,-47,-48,-49,-50,-51,-25,-28,-53,-54,-32,-33,-35,-36,-37,67,-26,-15,-16,-23,-31,-38,-44,-45,-46,-30,]),'$end':([1,2,3,4,5,6,7,8,9,11,12,13,14,15,17,19,23,26,27,28,29,33,34,35,36,37,43,45,46,47,48,50,51,52,53,59,60,61,62,64,65,66,70,71,72,],[0,-2,-3,-4,-5,-6,-9,-11,-13,-8,-1,-10,-12,-26,-14,-24,-7,-52,-29,-34,-39,-47,-48,-49,-50,-51,-25,-28,-53,-54,-32,-33,-35,-36,-37,-26,-15,-16,-23,-31,-38,-44,-45,-46,-30,]),'ASSIGN':([10,],[16,]),'DOT':([10,15,22,26,27,28,29,33,34,35,36,37,41,48,50,51,52,53,64,65,66,70,71,72,],[22,25,22,-52,47,-34,-39,-47,-48,-49,-50,-51,25,-32,-33,-35,-36,-37,-31,-38,-44,-45,-46,-30,]),',':([15,19,43,59,],[-26,39,-25,-26,]),'LPAR':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[30,-52,30,-39,30,30,30,-47,-48,-49,-50,-51,30,-35,-36,-37,30,30,30,-38,-44,30,-45,-46,30,]),'LSQB':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[31,-52,31,-39,31,31,31,-47,-48,-49,-50,-51,31,-35,-36,-37,31,31,31,-38,-44,31,-45,-46,31,]),'LBRACE':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[32,-52,32,-39,32,32,32,-47,-48,-49,-50,-51,32,-35,-36,-37,32,32,32,-38,-44,32,-45,-46,32,]),'REGEX':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[36,-52,36,-39,36,36,36,-47,-48,-49,-50,-51,36,-35,-36,-37,36,36,36,-38,-44,36,-45,-46,36,]),'STRING':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[37,-52,37,-39,37,37,37,-47,-48,-49,-50,-51,37,-35,-36,-37,37,37,37,-38,-44,37,-45,-46,37,]),'OPTIONAL':([26,29,33,34,35,36,37,66,70,71,],[-52,51,-47,-48,-49,-50,-51,-44,-45,-46,]),'ASTERISK':([26,29,33,34,35,36,37,38,66,70,71,],[-52,52,-47,-48,-49,-50,-51,60,-44,-45,-46,]),'PLUS':([26,29,33,34,35,36,37,66,70,71,],[-52,53,-47,-48,-49,-50,-51,-44,-45,-46,]),'MINUS':([26,29,33,34,35,36,37,66,70,71,],[-52,54,-47,-48,-49,-50,-51,-44,-45,-46,]),'VBAR':([26,28,29,33,34,35,36,37,48,51,52,53,56,65,66,67,70,71,],[-52,49,-39,-47,-48,-49,-50,-51,63,-35,-36,-37,68,-38,-44,73,-45,-46,]),'SEMICOLON':([26,27,28,29,33,34,35,36,37,48,50,51,52,53,64,65,66,70,71,72,],[-52,46,-34,-39,-47,-48,-49,-50,-51,-32,-33,-35,-36,-37,-31,-38,-44,-45,-46,-30,]),'RPAR':([26,29,33,34,35,36,37,51,52,53,55,56,65,66,69,70,71,74,75,],[-52,-39,-47,-48,-49,-50,-51,-35,-36,-37,66,-43,-38,-44,-42,-45,-46,-41,-40,]),'RSQB':([26,29,33,34,35,36,37,51,52,53,56,57,65,66,69,70,71,74,75,],[-52,-39,-47,-48,-49,-50,-51,-35,-36,-37,-43,70,-38,-44,-42,-45,-46,-41,-40,]),'RBRACE':([26,29,33,34,35,36,37,51,52,53,56,58,65,66,69,70,71,74,75,],[-52,-39,-47,-48,-49,-50,-51,-35,-36,-37,-43,71,-38,-44,-42,-45,-46,-41,-40,]),}
+_lr_action_items = {'COMMENT':([0,2,3,4,5,6,7,8,9,11,13,14,15,17,19,23,26,27,28,29,33,34,35,36,37,43,45,46,47,48,50,51,52,53,59,60,61,62,64,65,66,70,71,72,],[7,7,-3,-4,-5,-6,-9,-11,-13,-8,-10,-12,-26,-14,-24,-7,-52,-29,-34,-39,-43,-44,-45,-50,-51,-25,-28,-53,-54,-32,-33,-35,-36,-37,-26,-15,-16,-23,-31,-38,-40,-41,-42,-30,]),'NAME':([0,2,3,4,5,6,7,8,9,10,11,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,56,59,60,61,62,63,64,65,66,68,70,71,72,73,],[10,10,-3,-4,-5,-6,-9,-11,-13,15,-8,-10,-12,24,26,-14,38,-24,41,-18,-20,-7,43,41,-52,-29,26,-39,26,26,26,-43,-44,-45,-50,-51,59,59,-17,-22,-19,-25,-21,-28,-53,-54,-32,26,-33,-35,-36,-37,26,26,24,-15,-16,-23,26,-31,-38,-40,26,-41,-42,-30,26,]),'NEWLINE':([0,2,3,4,5,6,7,8,9,11,13,14,15,17,19,23,26,27,28,29,33,34,35,36,37,43,45,46,47,48,50,51,52,53,56,59,60,61,62,64,65,66,70,71,72,],[11,11,-3,-4,-5,-6,-9,11,11,11,-10,-12,-26,-14,-24,-7,-52,-29,48,-39,-43,-44,-45,-50,-51,-25,-28,-53,-54,-32,-33,-35,-36,-37,67,-26,-15,-16,-23,-31,-38,-40,-41,-42,-30,]),'$end':([1,2,3,4,5,6,7,8,9,11,12,13,14,15,17,19,23,26,27,28,29,33,34,35,36,37,43,45,46,47,48,50,51,52,53,59,60,61,62,64,65,66,70,71,72,],[0,-2,-3,-4,-5,-6,-9,-11,-13,-8,-1,-10,-12,-26,-14,-24,-7,-52,-29,-34,-39,-43,-44,-45,-50,-51,-25,-28,-53,-54,-32,-33,-35,-36,-37,-26,-15,-16,-23,-31,-38,-40,-41,-42,-30,]),'ASSIGN':([10,],[16,]),'DOT':([10,15,22,26,27,28,29,33,34,35,36,37,41,48,50,51,52,53,64,65,66,70,71,72,],[22,25,22,-52,47,-34,-39,-43,-44,-45,-50,-51,25,-32,-33,-35,-36,-37,-31,-38,-40,-41,-42,-30,]),',':([15,19,43,59,],[-26,39,-25,-26,]),'LPAR':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[30,-52,30,-39,30,30,30,-43,-44,-45,-50,-51,30,-35,-36,-37,30,30,30,-38,-40,30,-41,-42,30,]),'LSQB':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[31,-52,31,-39,31,31,31,-43,-44,-45,-50,-51,31,-35,-36,-37,31,31,31,-38,-40,31,-41,-42,31,]),'LBRACE':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[32,-52,32,-39,32,32,32,-43,-44,-45,-50,-51,32,-35,-36,-37,32,32,32,-38,-40,32,-41,-42,32,]),'REGEX':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[36,-52,36,-39,36,36,36,-43,-44,-45,-50,-51,36,-35,-36,-37,36,36,36,-38,-40,36,-41,-42,36,]),'STRING':([16,26,28,29,30,31,32,33,34,35,36,37,49,51,52,53,54,56,63,65,66,68,70,71,73,],[37,-52,37,-39,37,37,37,-43,-44,-45,-50,-51,37,-35,-36,-37,37,37,37,-38,-40,37,-41,-42,37,]),'OPTIONAL':([26,29,33,34,35,36,37,66,70,71,],[-52,51,-43,-44,-45,-50,-51,-40,-41,-42,]),'ASTERISK':([26,29,33,34,35,36,37,38,66,70,71,],[-52,52,-43,-44,-45,-50,-51,60,-40,-41,-42,]),'PLUS':([26,29,33,34,35,36,37,66,70,71,],[-52,53,-43,-44,-45,-50,-51,-40,-41,-42,]),'MINUS':([26,29,33,34,35,36,37,66,70,71,],[-52,54,-43,-44,-45,-50,-51,-40,-41,-42,]),'VBAR':([26,28,29,33,34,35,36,37,48,51,52,53,56,65,66,67,70,71,],[-52,49,-39,-43,-44,-45,-50,-51,63,-35,-36,-37,68,-38,-40,73,-41,-42,]),'SEMICOLON':([26,27,28,29,33,34,35,36,37,48,50,51,52,53,64,65,66,70,71,72,],[-52,46,-34,-39,-43,-44,-45,-50,-51,-32,-33,-35,-36,-37,-31,-38,-40,-41,-42,-30,]),'RPAR':([26,29,33,34,35,36,37,51,52,53,55,56,65,66,69,70,71,74,75,],[-52,-39,-43,-44,-45,-50,-51,-35,-36,-37,66,-49,-38,-40,-48,-41,-42,-47,-46,]),'RSQB':([26,29,33,34,35,36,37,51,52,53,56,57,65,66,69,70,71,74,75,],[-52,-39,-43,-44,-45,-50,-51,-35,-36,-37,-49,70,-38,-40,-48,-41,-42,-47,-46,]),'RBRACE':([26,29,33,34,35,36,37,51,52,53,56,58,65,66,69,70,71,74,75,],[-52,-39,-43,-44,-45,-50,-51,-35,-36,-37,-49,71,-38,-40,-48,-41,-42,-47,-46,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
@@ -53,32 +53,32 @@
   ('import_items -> import_name','import_items',1,'p_import_items','parsers.py',116),
   ('import_name -> NAME NAME NAME','import_name',3,'p_import_name','parsers.py',125),
   ('import_name -> NAME','import_name',1,'p_import_name','parsers.py',126),
   ('import_items_multiline -> LPAR NEWLINE import_name NEWLINE RPAR','import_items_multiline',5,'p_import_items_multiline','parsers.py',137),
   ('rule -> NAME ASSIGN rhs terminator','rule',4,'p_rule','parsers.py',144),
   ('rule -> NAME ASSIGN rhs','rule',3,'p_rule','parsers.py',145),
   ('rhs -> factor NEWLINE VBAR rhs','rhs',4,'p_rhs','parsers.py',151),
-  ('rhs -> factor VBAR rhs','rhs',3,'p_rhs','parsers.py',153),
-  ('rhs -> factor NEWLINE','rhs',2,'p_rhs','parsers.py',155),
-  ('rhs -> factor rhs','rhs',2,'p_rhs','parsers.py',156),
-  ('rhs -> factor','rhs',1,'p_rhs','parsers.py',157),
-  ('factor -> term OPTIONAL','factor',2,'p_factor','parsers.py',177),
-  ('factor -> term ASTERISK','factor',2,'p_factor','parsers.py',178),
-  ('factor -> term PLUS','factor',2,'p_factor','parsers.py',179),
-  ('factor -> term MINUS term','factor',3,'p_factor','parsers.py',180),
-  ('factor -> term','factor',1,'p_factor','parsers.py',181),
-  ('term_group -> factor NEWLINE VBAR term_group','term_group',4,'p_term_group','parsers.py',192),
-  ('term_group -> factor VBAR term_group','term_group',3,'p_term_group','parsers.py',193),
-  ('term_group -> factor term_group','term_group',2,'p_term_group','parsers.py',194),
-  ('term_group -> factor','term_group',1,'p_term_group','parsers.py',195),
-  ('term -> LPAR term_group RPAR','term',3,'p_term','parsers.py',208),
-  ('term -> LSQB term_group RSQB','term',3,'p_term','parsers.py',209),
-  ('term -> LBRACE term_group RBRACE','term',3,'p_term','parsers.py',210),
-  ('term -> regex','term',1,'p_term','parsers.py',211),
-  ('term -> string','term',1,'p_term','parsers.py',212),
-  ('term -> name','term',1,'p_term','parsers.py',213),
-  ('regex -> REGEX','regex',1,'p_regex','parsers.py',222),
-  ('string -> STRING','string',1,'p_string','parsers.py',228),
-  ('name -> NAME','name',1,'p_name','parsers.py',234),
-  ('terminator -> SEMICOLON','terminator',1,'p_terminator','parsers.py',240),
-  ('terminator -> DOT','terminator',1,'p_terminator','parsers.py',241),
+  ('rhs -> factor VBAR rhs','rhs',3,'p_rhs','parsers.py',152),
+  ('rhs -> factor NEWLINE','rhs',2,'p_rhs','parsers.py',153),
+  ('rhs -> factor rhs','rhs',2,'p_rhs','parsers.py',154),
+  ('rhs -> factor','rhs',1,'p_rhs','parsers.py',155),
+  ('factor -> term OPTIONAL','factor',2,'p_factor','parsers.py',173),
+  ('factor -> term ASTERISK','factor',2,'p_factor','parsers.py',174),
+  ('factor -> term PLUS','factor',2,'p_factor','parsers.py',175),
+  ('factor -> term MINUS term','factor',3,'p_factor','parsers.py',176),
+  ('factor -> term','factor',1,'p_factor','parsers.py',177),
+  ('term -> LPAR term_group RPAR','term',3,'p_term','parsers.py',188),
+  ('term -> LSQB term_group RSQB','term',3,'p_term','parsers.py',189),
+  ('term -> LBRACE term_group RBRACE','term',3,'p_term','parsers.py',190),
+  ('term -> regex','term',1,'p_term','parsers.py',191),
+  ('term -> string','term',1,'p_term','parsers.py',192),
+  ('term -> name','term',1,'p_term','parsers.py',193),
+  ('term_group -> factor NEWLINE VBAR term_group','term_group',4,'p_term_group','parsers.py',202),
+  ('term_group -> factor VBAR term_group','term_group',3,'p_term_group','parsers.py',203),
+  ('term_group -> factor term_group','term_group',2,'p_term_group','parsers.py',204),
+  ('term_group -> factor','term_group',1,'p_term_group','parsers.py',205),
+  ('regex -> REGEX','regex',1,'p_regex','parsers.py',218),
+  ('string -> STRING','string',1,'p_string','parsers.py',224),
+  ('name -> NAME','name',1,'p_name','parsers.py',230),
+  ('terminator -> SEMICOLON','terminator',1,'p_terminator','parsers.py',236),
+  ('terminator -> DOT','terminator',1,'p_terminator','parsers.py',237),
 ]
```

### Comparing `rebnf-0.7/PKG-INFO` & `rebnf-0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rebnf
-Version: 0.7
+Version: 0.8
 Summary: ReBNF: Regexes for Extended Backus-Naur Form (EBNF)
 Keywords: bnf,ebnf,rebnf,regex,regexes,backus-naur form,extended backus-naur form,syntax,metasyntax,lexer,parser,context-free grammar,formal language,grammar,language,text processing
 Author-email: opsocket <opsocket@pm.me>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -22,15 +22,15 @@
 Project-URL: Repository, https://gitlab.com/opsocket/rebnf.git
 Provides-Extra: dev
 Provides-Extra: docs
 
 # ReBNF
 
 <div>
-  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.7-ec3832.svg?color=ec3832&style=flat"/></a>
+  <a href="#"><img src="https://img.shields.io/badge/%F0%9F%94%96%20Version-0.8-ec3832.svg?color=ec3832&style=flat"/></a>
   <a href="https://opsocket.com" style="text-decoration: none;">
     <img alt="opsocket" height="42" src="https://gitlab.com/opsocket/rebnf/-/raw/main/docs/assets/imgs/logo.svg" loading="lazy" />
   </a>
 </div>
 
 
 **ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to define the
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: rebnf Version: 0.7 Summary: ReBNF: Regexes for
+Metadata-Version: 2.1 Name: rebnf Version: 0.8 Summary: ReBNF: Regexes for
 Extended Backus-Naur Form (EBNF) Keywords: bnf,ebnf,rebnf,regex,regexes,backus-
 naur form,extended backus-naur form,syntax,metasyntax,lexer,parser,context-free
 grammar,formal language,grammar,language,text processing Author-email: opsocket
 pm.me> Description-Content-Type: text/markdown Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Topic :: Software Development :: Libraries Classifier: Topic
 :: Software Development Classifier: Topic :: Text Processing Requires-Dist: ply
 Requires-Dist: black ; extra == "dev" Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev" Requires-Dist: build ; extra == "dev"
 Requires-Dist: twine ; extra == "dev" Project-URL: Repository, https://
 gitlab.com/opsocket/rebnf.git Provides-Extra: dev Provides-Extra: docs # ReBNF
-[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.7-
+[https://img.shields.io/badge/%F0%9F%94%96%20Version-0.8-
 ec3832.svg?color=ec3832&style=flat] [opsocket]
 **ReBNF** (*Regexes for Extended Backus-Naur Form*) is a notation used to
 define the syntax of a language using regular expressions. It is an extension
 of the EBNF (Extended Backus-Naur Form) notation, allowing for more flexibility
 and ease of use. ``` ooooooooo. oooooooooo. ooooo ooo oooooooooooo `888 `Y88.
 `888' `Y8b `888b. `8' `888' `8 888 .d88' .ooooo. 888 888 8 `88b. 8 888
 888ooo88P' d88' `88b 888oooo888' 8 `88b. 8 888oooo8 888`88b. 888ooo888 888 `88b
```


# Comparing `tmp/Humre-0.2.0.tar.gz` & `tmp/Humre-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Humre-0.2.0.tar", last modified: Tue Aug 30 20:14:16 2022, max compression
+gzip compressed data, was "Humre-1.0.0.tar", last modified: Sun Jun 18 01:51:51 2023, max compression
```

## Comparing `Humre-0.2.0.tar` & `Humre-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-08-30 20:14:16.896612 Humre-0.2.0/
--rw-rw-rw-   0        0        0     1072 2022-07-20 19:58:35.000000 Humre-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0    15530 2022-08-30 20:14:16.893617 Humre-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    14653 2022-08-30 20:13:20.000000 Humre-0.2.0/README.md
--rw-rw-rw-   0        0        0        0 2022-07-20 19:58:35.000000 Humre-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-30 20:14:16.896612 Humre-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1674 2022-08-07 01:48:29.000000 Humre-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-30 20:14:16.773613 Humre-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-30 20:14:16.879617 Humre-0.2.0/src/Humre.egg-info/
--rw-rw-rw-   0        0        0    15530 2022-08-30 20:14:16.000000 Humre-0.2.0/src/Humre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2022-08-30 20:14:16.000000 Humre-0.2.0/src/Humre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-30 20:14:16.000000 Humre-0.2.0/src/Humre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-08-30 20:14:16.000000 Humre-0.2.0/src/Humre.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-30 20:14:16.885607 Humre-0.2.0/src/humre/
--rw-rw-rw-   0        0        0    73708 2022-08-25 17:48:13.000000 Humre-0.2.0/src/humre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 01:51:51.642416 Humre-1.0.0/
+-rw-rw-rw-   0        0        0      657 2023-04-25 22:59:07.000000 Humre-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    14356 2023-06-18 01:51:51.642416 Humre-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12356 2023-06-18 01:46:29.000000 Humre-1.0.0/README.md
+-rw-rw-rw-   0        0        0     1347 2023-04-25 23:22:02.000000 Humre-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 01:51:51.642416 Humre-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2023-06-18 01:51:11.000000 Humre-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 01:51:51.595577 Humre-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 01:51:51.642416 Humre-1.0.0/src/Humre.egg-info/
+-rw-rw-rw-   0        0        0    14356 2023-06-18 01:51:51.000000 Humre-1.0.0/src/Humre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-06-18 01:51:51.000000 Humre-1.0.0/src/Humre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 01:51:51.000000 Humre-1.0.0/src/Humre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-18 01:51:51.000000 Humre-1.0.0/src/Humre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 01:51:51.642416 Humre-1.0.0/src/humre/
+-rw-rw-rw-   0        0        0    75360 2023-06-18 01:30:46.000000 Humre-1.0.0/src/humre/__init__.py
```

### Comparing `Humre-0.2.0/PKG-INFO` & `Humre-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 Metadata-Version: 2.1
 Name: Humre
-Version: 0.2.0
+Version: 1.0.0
 Summary: A human-readable regular expression module for Python. Humre handles regex syntax for you and creates regex strings to pass to Python's re.compile(). Pronounced "hum, ree".
 Home-page: https://github.com/asweigart/humre
 Author: Al Sweigart
-Author-email: al@inventwithpython.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+Author-email: Al Sweigart <al@inventwithpython.com>
+License: Copyright (c) 2022 Al Sweigart
+        
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU General Public License as published by
+        the Free Software Foundation, either version 3 of the License, or
+        (at your option) any later version.
+        
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU General Public License for more details.
+        
+        You should have received a copy of the GNU General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+Project-URL: Homepage, https://github.com/asweigart/humre
+Project-URL: Bug Tracker, https://github.com/asweigart/humre/issues
+Keywords: regex,re,regular expression
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # Humre
 
 A human-readable regular expression module for Python. Humre handles regex syntax for you and creates regex strings to pass to Python's re.compile(). Pronounced "hum, ree".
 
 It is similar to [Swift's regex DSL](https://swiftregex.com/) or an advanced form of Python regex's `re.VERBOSE` mode. Code is read far more often than it is written, so the verbose Humre code may take a few seconds longer to write but pays for itself by being much easier to read and understand.
 
 Note that until version 1.0 is released, the API for this module could change. Please send suggestions and feedback to [al@inventwithpython.com](mailto://al@inventwithpython.com).
 
 Quickstart
 ----------
 
+    >>> import re
     >>> from humre import *
     >>> regexStr = either(OPEN_PAREN + exactly(3, DIGIT) + CLOSE_PAREN, exactly(3, DIGIT)) + '-' + exactly(3, DIGIT) + '-' + exactly(4, DIGIT)
     >>> regexStr
     '\\(\\d{3}\\)|\\d{3}-\\d{3}-\\d{4}'
-    >>> patternObj = compile(regexStr)
+    >>> patternObj = re.compile(regexStr)
     >>> matchObj = patternObj.search('Call 415-555-1234 today!')
     >>> matchObj
     <re.Match object; span=(5, 17), match='415-555-1234'>
     >>> matchObj.group()
     '415-555-1234'
 
 
@@ -58,30 +79,30 @@
 
 **Doesn't Verbose Mode Fix That Problem?**
 
 A little. But because verbose mode still has the regex string as a string value, dev tools such as linters, syntax highlighting, and matching parentheses highlighting can't be employed. Also, dealing with escape characters can still be a pain.
 
 **Is Humre a New Reimplementation of Python's re Module?**
 
-No. Humre only creates the regex strings to pass to `re.compile()` (or to pass to `humre.compile()` which wraps it.)
+No. Humre only creates the regex strings to pass to `re.compile()`.
 
 **What Are Benefits of Using Humre Instead of Writing My Own Regex Strings?**
 
 * Your editor's parentheses matching works.
 * Your editor's syntax highlight works.
 * Your editor's linter and type hints tool picks up typos.
 * Your editor's autocomplete works.
 * Auto-formatter tools like Black can automatically format your regex code.
 * Humre handles raw strings/string escaping for you.
 * You can put actual Python comments alongside your Humre code.
 * Better error messages for invalid regexes.
 
 **Is It A Good Idea To Use The `from humre import *` Importing Syntax?**
 
-In this case, sure. Generally this form importing is frowned on, but it'll keep your `optional(group('cat' + DIGIT))` code from becoming `humre.optional(humre.group('cat' + humre.DIGIT))`. Note that this will overwrite the (infrequently-used) built-in `compile()` function with `humre.compile()`, which is a wrapper for `re.compile()`.
+In this case, sure. Generally this form importing is frowned on, but it'll keep your `optional(group('cat' + DIGIT))` code from becoming `humre.optional(humre.group('cat' + humre.DIGIT))`.
 
 **How Do I Combine Humre's Functions and Constants Together?**
 
 Every Humre function returns a regex string and every Humre constant is a string, so you can use f-strings and string concatenation to combine them:
 
     >>> from humre import *
 
@@ -95,18 +116,14 @@
     'I am looking for \\d{2} grapes.'
 
 
 **Humre Seems Nice for Beginners, But Why Would Experienced Devs Want to Use It?**
 
 TODO
 
-**Why Is the humre.compile() Function Not Working When I Pass Flags to It?**
-
-Most Humre functions combine their arguments into one string for ease of use (that is, `group('cat', 'dog')` is the same as `group('catdog')`). The `humre.compile()` function does this to, so if you want to pass flags such as
-
 **Isn't Using Humre a Performance Hit Compared to Using re?**
 
 No. Humre functions are simple functions that do basic string manipulation. You only need to call them once when you create the regex pattern object. Your program, whether large or small, will spend far more time doing the actual pattern matching than creating the regex string.
 
 **Most Regexes Are Short Enough That the Syntax Doesn't Get In the Way. Why Use Humre for These?**
 
 Sure, the phone number example is simple enough that anyone who knows regex syntax can understand it.
@@ -119,26 +136,28 @@
 American Phone Number with re:
 
     import re
     re.compile('\d{3}-\d{3}-\d{4}')
 
 American Phone Number with Humre:
 
+    import re
     from humre import *
-    compile(exactly(3, DIGIT), "-", exactly(3, DIGIT), "-", exactly(4, DIGIT))
+    re.compile(exactly(3, DIGIT), "-", exactly(3, DIGIT), "-", exactly(4, DIGIT))
 
 Hexadecimal Number with Optional Leading `0x` or `0X` and Consistent Casing with re:
 
     import re
     re.compile('(?:(?:0x|0X)[0-9a-f]+)|(?:(?:0x|0X)[0-9A-F]+)|(?:[0-9a-f]+)|(?:[0-9A-F]+)')
 
 Hexadecimal Number with Optional Leading `0x` or `0X` and Consistent Casing with re:
 
+    import re
     from humre import *
-    compile(
+    re.compile(
         either(
             noncap_group(noncap_group(either('0x', '0X')), one_or_more(chars('0-9a-f'))),
             noncap_group(noncap_group(either('0x', '0X')), one_or_more(chars('0-9A-F'))),
             noncap_group(one_or_more(chars('0-9a-f'))),
             noncap_group(one_or_more(chars('0-9A-F')))
         )
     )
@@ -146,16 +165,17 @@
 Number with or without comma-formatting including decimal point with re:
 
     import re
     re.compile(r'(?:\+|-)?(?:(?:\d{1,3}(?:,\d{3})+)|\d+)(?:\.\d+)?')
 
 Number with or without comma-formatting including decimal point with Humre:
 
+    import re
     from humre import *
-    compile(
+    re.compile(
         # optional negative or positive sign:
         optional(noncap_group(either(PLUS_SIGN, '-'))),
         # whole number section:
         noncap_group(either(
             # number with commas:
             noncap_group(between(1, 3, DIGIT), one_or_more(noncap_group(',', exactly(3, DIGIT)))),
             # number without commas:
@@ -163,16 +183,17 @@
         )),
         # fractional number section (optional)
         optional(noncap_group(PERIOD, one_or_more(DIGIT)))
         )
 
 Or you can use Humre's included `NUMBER` pattern:
 
+    import re
     from humre import *
-    compile(NUMBER)
+    re.compile(NUMBER)
 
 
 
 
 Quick Reference
 ----------------
 
@@ -182,15 +203,15 @@
 |----------------|------------------|
 | `group('A')` | `'(A)'` |
 | `optional('A')` | `'A?'` |
 | `either('A', 'B', 'C')` | `'A\|B\|C'` |
 | `exactly(3, 'A')` | `'A{3}'` |
 | `between(3, 5, 'A')` | `'A{3:5}'` |
 | `at_least(3, 'A')` | `'A{3,}'` |
-| `at_most(3, 'A')` | `'A{,3})'` |
+| `at_most(3, 'A')` | `'A{,3}'` |
 | `chars('A-Z')` | `'[A-Z]'` |
 | `nonchars('A-Z')` | `'[^A-Z]'` |
 | `zero_or_more('A')` | `'A*'` |
 | `zero_or_more_lazy('A')` | `'A*?'` |
 | `one_or_more('A')` | `'A+'` |
 | `one_or_more_lazy('A')` | `'A+?'` |
 | `starts_with('A')` | `'^A'` |
@@ -198,50 +219,44 @@
 | `starts_and_ends_with('A')` | `'^A$'` |
 | `named_group('group_name', 'A')` | `'(?P<group_name>A)'` |
 | `noncap_group('A')` | `'(?:A)'` |
 | `positive_lookahead('A')` | `'(?=A)'` |
 | `negative_lookahead('A')` | `'(?!A)'` |
 | `positive_lookbehind('A')` | `'(?<=A)'` |
 | `negative_lookbehind('A')` | `'(?<!A)'` |
-| `back_reference(1)` | `r'\1'` |
-| `back_ref(1)` | `r'\1'` |
 | `atomic_group('A')` | `'(?>A)'` |
 | `zero_or_more_possessive('A')` | `'A*+'` |
 | `one_or_more_possessive('A')` | `'A++'` |
 | `optional_possessive('A')` | `'A?+'` |
 
 
 The convenience group functions combine a Humre function with the `group()` (or `noncap_group()`) function since putting regexes in groups is so common, such as with `([A-Z])+` putting the character class
 
 | Convenience Function | Function Equivalent | Regex Equivalent |
 |----------------------------|---------------------|------------------|
-| `optional_group('A')` | `optional(noncap_group('A'))` | `'(A)?'` |
+| `optional_group('A')` | `optional(group('A'))` | `'(A)?'` |
 | `optional_noncap_group('A')` | `optional(noncap_group('A'))` | `'(?:A)?'` |
-| `group_either('A')` | `noncap_group(either('A', 'B', 'C'))` | `'(A\|B\|C)'` |
+| `group_either('A', 'B', 'C')` | `group(either('A', 'B', 'C'))` | `'(A\|B\|C)'` |
 | `noncap_group_either('A')` | `noncap_group(either('A', 'B', 'C'))` | `'(?:A\|B\|C)'` |
-| `group_exactly('A')` | `noncap_group(exactly(3, 'A'))` | `'(A){3}'` |
-| `noncap_group_exactly('A')` | `noncap_group(exactly(3, 'A'))` | `'(?:A){3}'` |
-| `group_between('A')` | `noncap_group(between(3, 5, 'A'))` | `'(A){3,5}'` |
-| `noncap_group_between('A')` | `noncap_group(between(3, 5, 'A'))` | `'(?:A){3,5}'` |
-| `group_at_least('A')` | `noncap_group(at_least(3, 'A'))` | `'(A){3,}'` |
-| `noncap_group_at_least('A')` | `noncap_group(at_least(3, 'A'))` | `'(?:A){3,}'` |
-| `group_at_most('A')` | `noncap_group(at_most(3, 'A'))` | `'(A){,3}'` |
-| `noncap_group_at_most('A')` | `noncap_group(at_most(3, 'A'))` | `'(?:A){,3}'` |
-| `zero_or_more_group('A')` | `zero_or_more(noncap_group('A'))` | `'(A)*'` |
+| `exactly_group(3, 'A')` | `exactly(3, group('A'))` | `'(A){3}'` |
+| `noncap_exactly_group(3, 'A')` | `exactly(3, noncap_group('A'))` | `'(?:A){3}'` |
+| `between_group(3, 5, 'A')` | `between(3, 5, group('A'))` | `'(A){3,5}'` |
+| `between_noncap_group(3, 5, 'A')` | `between(3, 5, noncap_group('A'))` | `'(?:A){3,5}'` |
+| `at_least_group(3, 'A')` | `at_least(3, group('A'))` | `'(A){3,}'` |
+| `at_least_noncap_group(3, 'A')` | `at_least(3, noncap_group('A'))` | `'(?:A){3,}'` |
+| `at_most_group(5, 'A')` | `at_most(3, group('A'))` | `'(A){,3}'` |
+| `at_most_noncap_group(5, 'A')` | `at_most(3, noncap_group('A'))` | `'(?:A){,3}'` |
+| `zero_or_more_group('A')` | `zero_or_more(group('A'))` | `'(A)*'` |
 | `zero_or_more_noncap_group('A')` | `zero_or_more(noncap_group('A'))` | `'(?:A)*'` |
-| `zero_or_more_lazy_group('A')` | `zero_or_more_lazy_noncap_group('A'))` | `'(A)*?'` |
-| `zero_or_more_lazy_noncap_group('A')` | `zero_or_more_lazy_noncap_group('A'))` | `'(?:A)*?'` |
-| `one_or_more_group('A')` | `one_or_more(noncap_group('A'))` | `'(A)+'` |
+| `zero_or_more_lazy_group('A')` | `zero_or_more_lazy(group('A'))` | `'(A)*?'` |
+| `zero_or_more_lazy_noncap_group('A')` | `zero_or_more_lazy(noncap_group('A'))` | `'(?:A)*?'` |
+| `one_or_more_group('A')` | `one_or_more(group('A'))` | `'(A)+'` |
 | `one_or_more_noncap_group('A')` | `one_or_more(noncap_group('A'))` | `'(?:A)+'` |
-| `one_or_more_lazy_group('A')` | `one_or_more_lazy(noncap_group('A'))` | `'(A)+?'` |
+| `one_or_more_lazy_group('A')` | `one_or_more_lazy(group('A'))` | `'(A)+?'` |
 | `one_or_more_lazy_noncap_group('A')` | `one_or_more_lazy(noncap_group('A'))` | `'(?:A)+?'` |
-| `group_chars('A-Z')` | `noncap_group(chars('A-Z'))` | `'([A-Z])'` |
-| `noncap_group_chars('A-Z')` | `noncap_group(chars('A-Z'))` | `'(?:[A-Z])'` |
-| `group_nonchars('A-Z')` | `noncap_group(nonchars('A-Z'))` | `(['^A-Z])'` |
-| `noncap_group_nonchars('A-Z')` | `noncap_group(nonchars('A-Z'))` | `(?:['^A-Z])'` |
 
 Humre provides constants for the `\d`, `\w`, and `\s` character classes as well several other characters that need to be escaped:
 
 | Constant | Regex Equivalent |
 |----------------|------------------|
 | `DIGIT` | `r'\d'` |
 | `WORD` | `r'\w'` |
@@ -269,29 +284,24 @@
 | `OPEN_BRACKET` | `r'\['` |
 | `CLOSE_BRACKET` | `r'\]'` |
 | `BACKSLASH` | `r'\\'` |
 | `PIPE` | `r'\|'` |
 | `BACK_1` | `r'\1'` |
 | `BACK_2` | `r'\2'` |
 | `BACK_3` | `r'\3'` |
-| `BACK_4` | `r'\4'` |
-| `BACK_5` | `r'\5'` |
-| `BACK_6` | `r'\6'` |
-| `BACK_7` | `r'\7'` |
-| `BACK_8` | `r'\8'` |
-| `BACK_9` | `r'\9'` |
+| ... | ... |
+| `BACK_99` | `r'\99'` |
 
 Humre also provides constants for commonly used patterns:
 
 | Humre Pattern Constants | Regex Equivalent | Note |
 |----------------------------------|------------------|------|
 | `ANYTHING` | `'.*?'` | lazy "zero or more of anything" match |
 | `EVERYTHING` | `'.*'` | greedy "zero or more of anything" match, aka dot star |
 | `SOMETHING` | `'.+?'` | lazy "one or more of anything" match |
-| `GREEDY_SOMETHING` | `'.+'` | greedy "one or more of anything" match |
 | `ANYCHAR` | `'.'` | |
 | `LETTER` | (too big to display) | Matches `isalpha()` |
 | `NONLETTER` | (too big to display) | Matches `not isalpha()` |
 | `UPPERCASE` | (too big to display) | Matches `isupper()` |
 | `NONUPPERCASE` | (too big to display) | Matches `not isupper()` |
 | `LOWERCASE` | (too big to display) | Matches `islower()` |
 | `NONLOWERCASE` | (too big to display) | Matches `not islower()` |
@@ -299,26 +309,9 @@
 | `NONALPHANUMERIC` | (too big to display) | Matches `not isalnum()` |
 | `HEXADECIMAL` | `'[0-9A-Fa-f]'` | |
 | `NONHEXADECIMAL` | `'[^0-9A-Fa-f]'` | |
 | `NUMBER` | `r'(?:\+&#124;-)?(?:(?:\d{1,3}(?:,\d{3})+)&#124;\d+)(?:\.\d+)?'` | Comma-formatted numbers |
 | `EURO_NUMBER` | `r'(?:\+&#124;-)?(?:(?:\d{1,3}(?:\.\d{3})+)&#124;\d+)(?:,\d+)?'` | Period-formatted numbers |
 | `HEXADECIMAL_NUMBER` | `'(?:(?:0x&#124;0X)[0-9a-f]+)&#124;(?:(?:0x&#124;0X)[0-9A-F]+)&#124;(?:[0-9a-f]+)&#124;(?:[0-9A-F]+)'` | Can have leading `0x` or `0X`. |
 
-Humre's `compile()` function's `flags` keyword argument takes the same flag values as `re.compile()`:
 
-| Humre `compile()` Flags | Equivalent `re.compile()` Flags | Meaning |
-|---|---|---|
-|`humre.A` | `re.A` | Same as `ASCII` |
-|`humre.ASCII` | `re.ASCII` | Makes several escapes like `\w`, `\b`, `\s` and `\d` match only on ASCII characters with the respective property. |
-|`humre.DEBUG` | `re.DEBUG` | Display debug information about compiled expression. |
-|`humre.I` | `re.I` | Same as `IGNORECASE` |
-|`humre.IGNORECASE` | `re.IGNORECASE` | Do case-insensitive matches. |
-|`humre.L` | `re.L` | Same as `LOCALE` |
-|`humre.LOCALE` | `re.LOCALE` | Do a locale-aware match. |
-|`humre.M` | `re.M` | Same as `MULTILINE` |
-|`humre.MULTILINE` | `re.MULTILINE` | Multi-line matching, affecting `^` and `$`. |
-|`humre.NOFLAG` | `re.NOFLAG` | Indicates no flag being applied. Used as a default value in function definitions. New in 3.11. |
-|`humre.S` | `re.S` | Same as `DOTALL`. Corresponds to the inline flag `(?s)`. |
-|`humre.DOTALL` | `re.DOTALL` | Make `.` match any character, including newlines. |
-|`humre.X` | `re.X` | Same as `VERBOSE` (X stands for "extended") |
-|`humre.VERBOSE` | `re.VERBOSE` | Enable verbose REs, which can be organized more cleanly and understandably. |
```

### Comparing `Humre-0.2.0/README.md` & `Humre-1.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 It is similar to [Swift's regex DSL](https://swiftregex.com/) or an advanced form of Python regex's `re.VERBOSE` mode. Code is read far more often than it is written, so the verbose Humre code may take a few seconds longer to write but pays for itself by being much easier to read and understand.
 
 Note that until version 1.0 is released, the API for this module could change. Please send suggestions and feedback to [al@inventwithpython.com](mailto://al@inventwithpython.com).
 
 Quickstart
 ----------
 
+    >>> import re
     >>> from humre import *
     >>> regexStr = either(OPEN_PAREN + exactly(3, DIGIT) + CLOSE_PAREN, exactly(3, DIGIT)) + '-' + exactly(3, DIGIT) + '-' + exactly(4, DIGIT)
     >>> regexStr
     '\\(\\d{3}\\)|\\d{3}-\\d{3}-\\d{4}'
-    >>> patternObj = compile(regexStr)
+    >>> patternObj = re.compile(regexStr)
     >>> matchObj = patternObj.search('Call 415-555-1234 today!')
     >>> matchObj
     <re.Match object; span=(5, 17), match='415-555-1234'>
     >>> matchObj.group()
     '415-555-1234'
 
 
@@ -38,30 +39,30 @@
 
 **Doesn't Verbose Mode Fix That Problem?**
 
 A little. But because verbose mode still has the regex string as a string value, dev tools such as linters, syntax highlighting, and matching parentheses highlighting can't be employed. Also, dealing with escape characters can still be a pain.
 
 **Is Humre a New Reimplementation of Python's re Module?**
 
-No. Humre only creates the regex strings to pass to `re.compile()` (or to pass to `humre.compile()` which wraps it.)
+No. Humre only creates the regex strings to pass to `re.compile()`.
 
 **What Are Benefits of Using Humre Instead of Writing My Own Regex Strings?**
 
 * Your editor's parentheses matching works.
 * Your editor's syntax highlight works.
 * Your editor's linter and type hints tool picks up typos.
 * Your editor's autocomplete works.
 * Auto-formatter tools like Black can automatically format your regex code.
 * Humre handles raw strings/string escaping for you.
 * You can put actual Python comments alongside your Humre code.
 * Better error messages for invalid regexes.
 
 **Is It A Good Idea To Use The `from humre import *` Importing Syntax?**
 
-In this case, sure. Generally this form importing is frowned on, but it'll keep your `optional(group('cat' + DIGIT))` code from becoming `humre.optional(humre.group('cat' + humre.DIGIT))`. Note that this will overwrite the (infrequently-used) built-in `compile()` function with `humre.compile()`, which is a wrapper for `re.compile()`.
+In this case, sure. Generally this form importing is frowned on, but it'll keep your `optional(group('cat' + DIGIT))` code from becoming `humre.optional(humre.group('cat' + humre.DIGIT))`.
 
 **How Do I Combine Humre's Functions and Constants Together?**
 
 Every Humre function returns a regex string and every Humre constant is a string, so you can use f-strings and string concatenation to combine them:
 
     >>> from humre import *
 
@@ -75,18 +76,14 @@
     'I am looking for \\d{2} grapes.'
 
 
 **Humre Seems Nice for Beginners, But Why Would Experienced Devs Want to Use It?**
 
 TODO
 
-**Why Is the humre.compile() Function Not Working When I Pass Flags to It?**
-
-Most Humre functions combine their arguments into one string for ease of use (that is, `group('cat', 'dog')` is the same as `group('catdog')`). The `humre.compile()` function does this to, so if you want to pass flags such as
-
 **Isn't Using Humre a Performance Hit Compared to Using re?**
 
 No. Humre functions are simple functions that do basic string manipulation. You only need to call them once when you create the regex pattern object. Your program, whether large or small, will spend far more time doing the actual pattern matching than creating the regex string.
 
 **Most Regexes Are Short Enough That the Syntax Doesn't Get In the Way. Why Use Humre for These?**
 
 Sure, the phone number example is simple enough that anyone who knows regex syntax can understand it.
@@ -99,26 +96,28 @@
 American Phone Number with re:
 
     import re
     re.compile('\d{3}-\d{3}-\d{4}')
 
 American Phone Number with Humre:
 
+    import re
     from humre import *
-    compile(exactly(3, DIGIT), "-", exactly(3, DIGIT), "-", exactly(4, DIGIT))
+    re.compile(exactly(3, DIGIT), "-", exactly(3, DIGIT), "-", exactly(4, DIGIT))
 
 Hexadecimal Number with Optional Leading `0x` or `0X` and Consistent Casing with re:
 
     import re
     re.compile('(?:(?:0x|0X)[0-9a-f]+)|(?:(?:0x|0X)[0-9A-F]+)|(?:[0-9a-f]+)|(?:[0-9A-F]+)')
 
 Hexadecimal Number with Optional Leading `0x` or `0X` and Consistent Casing with re:
 
+    import re
     from humre import *
-    compile(
+    re.compile(
         either(
             noncap_group(noncap_group(either('0x', '0X')), one_or_more(chars('0-9a-f'))),
             noncap_group(noncap_group(either('0x', '0X')), one_or_more(chars('0-9A-F'))),
             noncap_group(one_or_more(chars('0-9a-f'))),
             noncap_group(one_or_more(chars('0-9A-F')))
         )
     )
@@ -126,16 +125,17 @@
 Number with or without comma-formatting including decimal point with re:
 
     import re
     re.compile(r'(?:\+|-)?(?:(?:\d{1,3}(?:,\d{3})+)|\d+)(?:\.\d+)?')
 
 Number with or without comma-formatting including decimal point with Humre:
 
+    import re
     from humre import *
-    compile(
+    re.compile(
         # optional negative or positive sign:
         optional(noncap_group(either(PLUS_SIGN, '-'))),
         # whole number section:
         noncap_group(either(
             # number with commas:
             noncap_group(between(1, 3, DIGIT), one_or_more(noncap_group(',', exactly(3, DIGIT)))),
             # number without commas:
@@ -143,16 +143,17 @@
         )),
         # fractional number section (optional)
         optional(noncap_group(PERIOD, one_or_more(DIGIT)))
         )
 
 Or you can use Humre's included `NUMBER` pattern:
 
+    import re
     from humre import *
-    compile(NUMBER)
+    re.compile(NUMBER)
 
 
 
 
 Quick Reference
 ----------------
 
@@ -162,15 +163,15 @@
 |----------------|------------------|
 | `group('A')` | `'(A)'` |
 | `optional('A')` | `'A?'` |
 | `either('A', 'B', 'C')` | `'A\|B\|C'` |
 | `exactly(3, 'A')` | `'A{3}'` |
 | `between(3, 5, 'A')` | `'A{3:5}'` |
 | `at_least(3, 'A')` | `'A{3,}'` |
-| `at_most(3, 'A')` | `'A{,3})'` |
+| `at_most(3, 'A')` | `'A{,3}'` |
 | `chars('A-Z')` | `'[A-Z]'` |
 | `nonchars('A-Z')` | `'[^A-Z]'` |
 | `zero_or_more('A')` | `'A*'` |
 | `zero_or_more_lazy('A')` | `'A*?'` |
 | `one_or_more('A')` | `'A+'` |
 | `one_or_more_lazy('A')` | `'A+?'` |
 | `starts_with('A')` | `'^A'` |
@@ -178,50 +179,44 @@
 | `starts_and_ends_with('A')` | `'^A$'` |
 | `named_group('group_name', 'A')` | `'(?P<group_name>A)'` |
 | `noncap_group('A')` | `'(?:A)'` |
 | `positive_lookahead('A')` | `'(?=A)'` |
 | `negative_lookahead('A')` | `'(?!A)'` |
 | `positive_lookbehind('A')` | `'(?<=A)'` |
 | `negative_lookbehind('A')` | `'(?<!A)'` |
-| `back_reference(1)` | `r'\1'` |
-| `back_ref(1)` | `r'\1'` |
 | `atomic_group('A')` | `'(?>A)'` |
 | `zero_or_more_possessive('A')` | `'A*+'` |
 | `one_or_more_possessive('A')` | `'A++'` |
 | `optional_possessive('A')` | `'A?+'` |
 
 
 The convenience group functions combine a Humre function with the `group()` (or `noncap_group()`) function since putting regexes in groups is so common, such as with `([A-Z])+` putting the character class
 
 | Convenience Function | Function Equivalent | Regex Equivalent |
 |----------------------------|---------------------|------------------|
-| `optional_group('A')` | `optional(noncap_group('A'))` | `'(A)?'` |
+| `optional_group('A')` | `optional(group('A'))` | `'(A)?'` |
 | `optional_noncap_group('A')` | `optional(noncap_group('A'))` | `'(?:A)?'` |
-| `group_either('A')` | `noncap_group(either('A', 'B', 'C'))` | `'(A\|B\|C)'` |
+| `group_either('A', 'B', 'C')` | `group(either('A', 'B', 'C'))` | `'(A\|B\|C)'` |
 | `noncap_group_either('A')` | `noncap_group(either('A', 'B', 'C'))` | `'(?:A\|B\|C)'` |
-| `group_exactly('A')` | `noncap_group(exactly(3, 'A'))` | `'(A){3}'` |
-| `noncap_group_exactly('A')` | `noncap_group(exactly(3, 'A'))` | `'(?:A){3}'` |
-| `group_between('A')` | `noncap_group(between(3, 5, 'A'))` | `'(A){3,5}'` |
-| `noncap_group_between('A')` | `noncap_group(between(3, 5, 'A'))` | `'(?:A){3,5}'` |
-| `group_at_least('A')` | `noncap_group(at_least(3, 'A'))` | `'(A){3,}'` |
-| `noncap_group_at_least('A')` | `noncap_group(at_least(3, 'A'))` | `'(?:A){3,}'` |
-| `group_at_most('A')` | `noncap_group(at_most(3, 'A'))` | `'(A){,3}'` |
-| `noncap_group_at_most('A')` | `noncap_group(at_most(3, 'A'))` | `'(?:A){,3}'` |
-| `zero_or_more_group('A')` | `zero_or_more(noncap_group('A'))` | `'(A)*'` |
+| `exactly_group(3, 'A')` | `exactly(3, group('A'))` | `'(A){3}'` |
+| `noncap_exactly_group(3, 'A')` | `exactly(3, noncap_group('A'))` | `'(?:A){3}'` |
+| `between_group(3, 5, 'A')` | `between(3, 5, group('A'))` | `'(A){3,5}'` |
+| `between_noncap_group(3, 5, 'A')` | `between(3, 5, noncap_group('A'))` | `'(?:A){3,5}'` |
+| `at_least_group(3, 'A')` | `at_least(3, group('A'))` | `'(A){3,}'` |
+| `at_least_noncap_group(3, 'A')` | `at_least(3, noncap_group('A'))` | `'(?:A){3,}'` |
+| `at_most_group(5, 'A')` | `at_most(3, group('A'))` | `'(A){,3}'` |
+| `at_most_noncap_group(5, 'A')` | `at_most(3, noncap_group('A'))` | `'(?:A){,3}'` |
+| `zero_or_more_group('A')` | `zero_or_more(group('A'))` | `'(A)*'` |
 | `zero_or_more_noncap_group('A')` | `zero_or_more(noncap_group('A'))` | `'(?:A)*'` |
-| `zero_or_more_lazy_group('A')` | `zero_or_more_lazy_noncap_group('A'))` | `'(A)*?'` |
-| `zero_or_more_lazy_noncap_group('A')` | `zero_or_more_lazy_noncap_group('A'))` | `'(?:A)*?'` |
-| `one_or_more_group('A')` | `one_or_more(noncap_group('A'))` | `'(A)+'` |
+| `zero_or_more_lazy_group('A')` | `zero_or_more_lazy(group('A'))` | `'(A)*?'` |
+| `zero_or_more_lazy_noncap_group('A')` | `zero_or_more_lazy(noncap_group('A'))` | `'(?:A)*?'` |
+| `one_or_more_group('A')` | `one_or_more(group('A'))` | `'(A)+'` |
 | `one_or_more_noncap_group('A')` | `one_or_more(noncap_group('A'))` | `'(?:A)+'` |
-| `one_or_more_lazy_group('A')` | `one_or_more_lazy(noncap_group('A'))` | `'(A)+?'` |
+| `one_or_more_lazy_group('A')` | `one_or_more_lazy(group('A'))` | `'(A)+?'` |
 | `one_or_more_lazy_noncap_group('A')` | `one_or_more_lazy(noncap_group('A'))` | `'(?:A)+?'` |
-| `group_chars('A-Z')` | `noncap_group(chars('A-Z'))` | `'([A-Z])'` |
-| `noncap_group_chars('A-Z')` | `noncap_group(chars('A-Z'))` | `'(?:[A-Z])'` |
-| `group_nonchars('A-Z')` | `noncap_group(nonchars('A-Z'))` | `(['^A-Z])'` |
-| `noncap_group_nonchars('A-Z')` | `noncap_group(nonchars('A-Z'))` | `(?:['^A-Z])'` |
 
 Humre provides constants for the `\d`, `\w`, and `\s` character classes as well several other characters that need to be escaped:
 
 | Constant | Regex Equivalent |
 |----------------|------------------|
 | `DIGIT` | `r'\d'` |
 | `WORD` | `r'\w'` |
@@ -249,29 +244,24 @@
 | `OPEN_BRACKET` | `r'\['` |
 | `CLOSE_BRACKET` | `r'\]'` |
 | `BACKSLASH` | `r'\\'` |
 | `PIPE` | `r'\|'` |
 | `BACK_1` | `r'\1'` |
 | `BACK_2` | `r'\2'` |
 | `BACK_3` | `r'\3'` |
-| `BACK_4` | `r'\4'` |
-| `BACK_5` | `r'\5'` |
-| `BACK_6` | `r'\6'` |
-| `BACK_7` | `r'\7'` |
-| `BACK_8` | `r'\8'` |
-| `BACK_9` | `r'\9'` |
+| ... | ... |
+| `BACK_99` | `r'\99'` |
 
 Humre also provides constants for commonly used patterns:
 
 | Humre Pattern Constants | Regex Equivalent | Note |
 |----------------------------------|------------------|------|
 | `ANYTHING` | `'.*?'` | lazy "zero or more of anything" match |
 | `EVERYTHING` | `'.*'` | greedy "zero or more of anything" match, aka dot star |
 | `SOMETHING` | `'.+?'` | lazy "one or more of anything" match |
-| `GREEDY_SOMETHING` | `'.+'` | greedy "one or more of anything" match |
 | `ANYCHAR` | `'.'` | |
 | `LETTER` | (too big to display) | Matches `isalpha()` |
 | `NONLETTER` | (too big to display) | Matches `not isalpha()` |
 | `UPPERCASE` | (too big to display) | Matches `isupper()` |
 | `NONUPPERCASE` | (too big to display) | Matches `not isupper()` |
 | `LOWERCASE` | (too big to display) | Matches `islower()` |
 | `NONLOWERCASE` | (too big to display) | Matches `not islower()` |
@@ -279,26 +269,7 @@
 | `NONALPHANUMERIC` | (too big to display) | Matches `not isalnum()` |
 | `HEXADECIMAL` | `'[0-9A-Fa-f]'` | |
 | `NONHEXADECIMAL` | `'[^0-9A-Fa-f]'` | |
 | `NUMBER` | `r'(?:\+&#124;-)?(?:(?:\d{1,3}(?:,\d{3})+)&#124;\d+)(?:\.\d+)?'` | Comma-formatted numbers |
 | `EURO_NUMBER` | `r'(?:\+&#124;-)?(?:(?:\d{1,3}(?:\.\d{3})+)&#124;\d+)(?:,\d+)?'` | Period-formatted numbers |
 | `HEXADECIMAL_NUMBER` | `'(?:(?:0x&#124;0X)[0-9a-f]+)&#124;(?:(?:0x&#124;0X)[0-9A-F]+)&#124;(?:[0-9a-f]+)&#124;(?:[0-9A-F]+)'` | Can have leading `0x` or `0X`. |
 
-Humre's `compile()` function's `flags` keyword argument takes the same flag values as `re.compile()`:
-
-| Humre `compile()` Flags | Equivalent `re.compile()` Flags | Meaning |
-|---|---|---|
-|`humre.A` | `re.A` | Same as `ASCII` |
-|`humre.ASCII` | `re.ASCII` | Makes several escapes like `\w`, `\b`, `\s` and `\d` match only on ASCII characters with the respective property. |
-|`humre.DEBUG` | `re.DEBUG` | Display debug information about compiled expression. |
-|`humre.I` | `re.I` | Same as `IGNORECASE` |
-|`humre.IGNORECASE` | `re.IGNORECASE` | Do case-insensitive matches. |
-|`humre.L` | `re.L` | Same as `LOCALE` |
-|`humre.LOCALE` | `re.LOCALE` | Do a locale-aware match. |
-|`humre.M` | `re.M` | Same as `MULTILINE` |
-|`humre.MULTILINE` | `re.MULTILINE` | Multi-line matching, affecting `^` and `$`. |
-|`humre.NOFLAG` | `re.NOFLAG` | Indicates no flag being applied. Used as a default value in function definitions. New in 3.11. |
-|`humre.S` | `re.S` | Same as `DOTALL`. Corresponds to the inline flag `(?s)`. |
-|`humre.DOTALL` | `re.DOTALL` | Make `.` match any character, including newlines. |
-|`humre.X` | `re.X` | Same as `VERBOSE` (X stands for "extended") |
-|`humre.VERBOSE` | `re.VERBOSE` | Enable verbose REs, which can be organized more cleanly and understandably. |
-
```

### Comparing `Humre-0.2.0/setup.py` & `Humre-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,10 +37,12 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.9",
-
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `Humre-0.2.0/src/Humre.egg-info/PKG-INFO` & `Humre-1.0.0/src/Humre.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 Metadata-Version: 2.1
 Name: Humre
-Version: 0.2.0
+Version: 1.0.0
 Summary: A human-readable regular expression module for Python. Humre handles regex syntax for you and creates regex strings to pass to Python's re.compile(). Pronounced "hum, ree".
 Home-page: https://github.com/asweigart/humre
 Author: Al Sweigart
-Author-email: al@inventwithpython.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+Author-email: Al Sweigart <al@inventwithpython.com>
+License: Copyright (c) 2022 Al Sweigart
+        
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU General Public License as published by
+        the Free Software Foundation, either version 3 of the License, or
+        (at your option) any later version.
+        
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU General Public License for more details.
+        
+        You should have received a copy of the GNU General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+Project-URL: Homepage, https://github.com/asweigart/humre
+Project-URL: Bug Tracker, https://github.com/asweigart/humre/issues
+Keywords: regex,re,regular expression
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 # Humre
 
 A human-readable regular expression module for Python. Humre handles regex syntax for you and creates regex strings to pass to Python's re.compile(). Pronounced "hum, ree".
 
 It is similar to [Swift's regex DSL](https://swiftregex.com/) or an advanced form of Python regex's `re.VERBOSE` mode. Code is read far more often than it is written, so the verbose Humre code may take a few seconds longer to write but pays for itself by being much easier to read and understand.
 
 Note that until version 1.0 is released, the API for this module could change. Please send suggestions and feedback to [al@inventwithpython.com](mailto://al@inventwithpython.com).
 
 Quickstart
 ----------
 
+    >>> import re
     >>> from humre import *
     >>> regexStr = either(OPEN_PAREN + exactly(3, DIGIT) + CLOSE_PAREN, exactly(3, DIGIT)) + '-' + exactly(3, DIGIT) + '-' + exactly(4, DIGIT)
     >>> regexStr
     '\\(\\d{3}\\)|\\d{3}-\\d{3}-\\d{4}'
-    >>> patternObj = compile(regexStr)
+    >>> patternObj = re.compile(regexStr)
     >>> matchObj = patternObj.search('Call 415-555-1234 today!')
     >>> matchObj
     <re.Match object; span=(5, 17), match='415-555-1234'>
     >>> matchObj.group()
     '415-555-1234'
 
 
@@ -58,30 +79,30 @@
 
 **Doesn't Verbose Mode Fix That Problem?**
 
 A little. But because verbose mode still has the regex string as a string value, dev tools such as linters, syntax highlighting, and matching parentheses highlighting can't be employed. Also, dealing with escape characters can still be a pain.
 
 **Is Humre a New Reimplementation of Python's re Module?**
 
-No. Humre only creates the regex strings to pass to `re.compile()` (or to pass to `humre.compile()` which wraps it.)
+No. Humre only creates the regex strings to pass to `re.compile()`.
 
 **What Are Benefits of Using Humre Instead of Writing My Own Regex Strings?**
 
 * Your editor's parentheses matching works.
 * Your editor's syntax highlight works.
 * Your editor's linter and type hints tool picks up typos.
 * Your editor's autocomplete works.
 * Auto-formatter tools like Black can automatically format your regex code.
 * Humre handles raw strings/string escaping for you.
 * You can put actual Python comments alongside your Humre code.
 * Better error messages for invalid regexes.
 
 **Is It A Good Idea To Use The `from humre import *` Importing Syntax?**
 
-In this case, sure. Generally this form importing is frowned on, but it'll keep your `optional(group('cat' + DIGIT))` code from becoming `humre.optional(humre.group('cat' + humre.DIGIT))`. Note that this will overwrite the (infrequently-used) built-in `compile()` function with `humre.compile()`, which is a wrapper for `re.compile()`.
+In this case, sure. Generally this form importing is frowned on, but it'll keep your `optional(group('cat' + DIGIT))` code from becoming `humre.optional(humre.group('cat' + humre.DIGIT))`.
 
 **How Do I Combine Humre's Functions and Constants Together?**
 
 Every Humre function returns a regex string and every Humre constant is a string, so you can use f-strings and string concatenation to combine them:
 
     >>> from humre import *
 
@@ -95,18 +116,14 @@
     'I am looking for \\d{2} grapes.'
 
 
 **Humre Seems Nice for Beginners, But Why Would Experienced Devs Want to Use It?**
 
 TODO
 
-**Why Is the humre.compile() Function Not Working When I Pass Flags to It?**
-
-Most Humre functions combine their arguments into one string for ease of use (that is, `group('cat', 'dog')` is the same as `group('catdog')`). The `humre.compile()` function does this to, so if you want to pass flags such as
-
 **Isn't Using Humre a Performance Hit Compared to Using re?**
 
 No. Humre functions are simple functions that do basic string manipulation. You only need to call them once when you create the regex pattern object. Your program, whether large or small, will spend far more time doing the actual pattern matching than creating the regex string.
 
 **Most Regexes Are Short Enough That the Syntax Doesn't Get In the Way. Why Use Humre for These?**
 
 Sure, the phone number example is simple enough that anyone who knows regex syntax can understand it.
@@ -119,26 +136,28 @@
 American Phone Number with re:
 
     import re
     re.compile('\d{3}-\d{3}-\d{4}')
 
 American Phone Number with Humre:
 
+    import re
     from humre import *
-    compile(exactly(3, DIGIT), "-", exactly(3, DIGIT), "-", exactly(4, DIGIT))
+    re.compile(exactly(3, DIGIT), "-", exactly(3, DIGIT), "-", exactly(4, DIGIT))
 
 Hexadecimal Number with Optional Leading `0x` or `0X` and Consistent Casing with re:
 
     import re
     re.compile('(?:(?:0x|0X)[0-9a-f]+)|(?:(?:0x|0X)[0-9A-F]+)|(?:[0-9a-f]+)|(?:[0-9A-F]+)')
 
 Hexadecimal Number with Optional Leading `0x` or `0X` and Consistent Casing with re:
 
+    import re
     from humre import *
-    compile(
+    re.compile(
         either(
             noncap_group(noncap_group(either('0x', '0X')), one_or_more(chars('0-9a-f'))),
             noncap_group(noncap_group(either('0x', '0X')), one_or_more(chars('0-9A-F'))),
             noncap_group(one_or_more(chars('0-9a-f'))),
             noncap_group(one_or_more(chars('0-9A-F')))
         )
     )
@@ -146,16 +165,17 @@
 Number with or without comma-formatting including decimal point with re:
 
     import re
     re.compile(r'(?:\+|-)?(?:(?:\d{1,3}(?:,\d{3})+)|\d+)(?:\.\d+)?')
 
 Number with or without comma-formatting including decimal point with Humre:
 
+    import re
     from humre import *
-    compile(
+    re.compile(
         # optional negative or positive sign:
         optional(noncap_group(either(PLUS_SIGN, '-'))),
         # whole number section:
         noncap_group(either(
             # number with commas:
             noncap_group(between(1, 3, DIGIT), one_or_more(noncap_group(',', exactly(3, DIGIT)))),
             # number without commas:
@@ -163,16 +183,17 @@
         )),
         # fractional number section (optional)
         optional(noncap_group(PERIOD, one_or_more(DIGIT)))
         )
 
 Or you can use Humre's included `NUMBER` pattern:
 
+    import re
     from humre import *
-    compile(NUMBER)
+    re.compile(NUMBER)
 
 
 
 
 Quick Reference
 ----------------
 
@@ -182,15 +203,15 @@
 |----------------|------------------|
 | `group('A')` | `'(A)'` |
 | `optional('A')` | `'A?'` |
 | `either('A', 'B', 'C')` | `'A\|B\|C'` |
 | `exactly(3, 'A')` | `'A{3}'` |
 | `between(3, 5, 'A')` | `'A{3:5}'` |
 | `at_least(3, 'A')` | `'A{3,}'` |
-| `at_most(3, 'A')` | `'A{,3})'` |
+| `at_most(3, 'A')` | `'A{,3}'` |
 | `chars('A-Z')` | `'[A-Z]'` |
 | `nonchars('A-Z')` | `'[^A-Z]'` |
 | `zero_or_more('A')` | `'A*'` |
 | `zero_or_more_lazy('A')` | `'A*?'` |
 | `one_or_more('A')` | `'A+'` |
 | `one_or_more_lazy('A')` | `'A+?'` |
 | `starts_with('A')` | `'^A'` |
@@ -198,50 +219,44 @@
 | `starts_and_ends_with('A')` | `'^A$'` |
 | `named_group('group_name', 'A')` | `'(?P<group_name>A)'` |
 | `noncap_group('A')` | `'(?:A)'` |
 | `positive_lookahead('A')` | `'(?=A)'` |
 | `negative_lookahead('A')` | `'(?!A)'` |
 | `positive_lookbehind('A')` | `'(?<=A)'` |
 | `negative_lookbehind('A')` | `'(?<!A)'` |
-| `back_reference(1)` | `r'\1'` |
-| `back_ref(1)` | `r'\1'` |
 | `atomic_group('A')` | `'(?>A)'` |
 | `zero_or_more_possessive('A')` | `'A*+'` |
 | `one_or_more_possessive('A')` | `'A++'` |
 | `optional_possessive('A')` | `'A?+'` |
 
 
 The convenience group functions combine a Humre function with the `group()` (or `noncap_group()`) function since putting regexes in groups is so common, such as with `([A-Z])+` putting the character class
 
 | Convenience Function | Function Equivalent | Regex Equivalent |
 |----------------------------|---------------------|------------------|
-| `optional_group('A')` | `optional(noncap_group('A'))` | `'(A)?'` |
+| `optional_group('A')` | `optional(group('A'))` | `'(A)?'` |
 | `optional_noncap_group('A')` | `optional(noncap_group('A'))` | `'(?:A)?'` |
-| `group_either('A')` | `noncap_group(either('A', 'B', 'C'))` | `'(A\|B\|C)'` |
+| `group_either('A', 'B', 'C')` | `group(either('A', 'B', 'C'))` | `'(A\|B\|C)'` |
 | `noncap_group_either('A')` | `noncap_group(either('A', 'B', 'C'))` | `'(?:A\|B\|C)'` |
-| `group_exactly('A')` | `noncap_group(exactly(3, 'A'))` | `'(A){3}'` |
-| `noncap_group_exactly('A')` | `noncap_group(exactly(3, 'A'))` | `'(?:A){3}'` |
-| `group_between('A')` | `noncap_group(between(3, 5, 'A'))` | `'(A){3,5}'` |
-| `noncap_group_between('A')` | `noncap_group(between(3, 5, 'A'))` | `'(?:A){3,5}'` |
-| `group_at_least('A')` | `noncap_group(at_least(3, 'A'))` | `'(A){3,}'` |
-| `noncap_group_at_least('A')` | `noncap_group(at_least(3, 'A'))` | `'(?:A){3,}'` |
-| `group_at_most('A')` | `noncap_group(at_most(3, 'A'))` | `'(A){,3}'` |
-| `noncap_group_at_most('A')` | `noncap_group(at_most(3, 'A'))` | `'(?:A){,3}'` |
-| `zero_or_more_group('A')` | `zero_or_more(noncap_group('A'))` | `'(A)*'` |
+| `exactly_group(3, 'A')` | `exactly(3, group('A'))` | `'(A){3}'` |
+| `noncap_exactly_group(3, 'A')` | `exactly(3, noncap_group('A'))` | `'(?:A){3}'` |
+| `between_group(3, 5, 'A')` | `between(3, 5, group('A'))` | `'(A){3,5}'` |
+| `between_noncap_group(3, 5, 'A')` | `between(3, 5, noncap_group('A'))` | `'(?:A){3,5}'` |
+| `at_least_group(3, 'A')` | `at_least(3, group('A'))` | `'(A){3,}'` |
+| `at_least_noncap_group(3, 'A')` | `at_least(3, noncap_group('A'))` | `'(?:A){3,}'` |
+| `at_most_group(5, 'A')` | `at_most(3, group('A'))` | `'(A){,3}'` |
+| `at_most_noncap_group(5, 'A')` | `at_most(3, noncap_group('A'))` | `'(?:A){,3}'` |
+| `zero_or_more_group('A')` | `zero_or_more(group('A'))` | `'(A)*'` |
 | `zero_or_more_noncap_group('A')` | `zero_or_more(noncap_group('A'))` | `'(?:A)*'` |
-| `zero_or_more_lazy_group('A')` | `zero_or_more_lazy_noncap_group('A'))` | `'(A)*?'` |
-| `zero_or_more_lazy_noncap_group('A')` | `zero_or_more_lazy_noncap_group('A'))` | `'(?:A)*?'` |
-| `one_or_more_group('A')` | `one_or_more(noncap_group('A'))` | `'(A)+'` |
+| `zero_or_more_lazy_group('A')` | `zero_or_more_lazy(group('A'))` | `'(A)*?'` |
+| `zero_or_more_lazy_noncap_group('A')` | `zero_or_more_lazy(noncap_group('A'))` | `'(?:A)*?'` |
+| `one_or_more_group('A')` | `one_or_more(group('A'))` | `'(A)+'` |
 | `one_or_more_noncap_group('A')` | `one_or_more(noncap_group('A'))` | `'(?:A)+'` |
-| `one_or_more_lazy_group('A')` | `one_or_more_lazy(noncap_group('A'))` | `'(A)+?'` |
+| `one_or_more_lazy_group('A')` | `one_or_more_lazy(group('A'))` | `'(A)+?'` |
 | `one_or_more_lazy_noncap_group('A')` | `one_or_more_lazy(noncap_group('A'))` | `'(?:A)+?'` |
-| `group_chars('A-Z')` | `noncap_group(chars('A-Z'))` | `'([A-Z])'` |
-| `noncap_group_chars('A-Z')` | `noncap_group(chars('A-Z'))` | `'(?:[A-Z])'` |
-| `group_nonchars('A-Z')` | `noncap_group(nonchars('A-Z'))` | `(['^A-Z])'` |
-| `noncap_group_nonchars('A-Z')` | `noncap_group(nonchars('A-Z'))` | `(?:['^A-Z])'` |
 
 Humre provides constants for the `\d`, `\w`, and `\s` character classes as well several other characters that need to be escaped:
 
 | Constant | Regex Equivalent |
 |----------------|------------------|
 | `DIGIT` | `r'\d'` |
 | `WORD` | `r'\w'` |
@@ -269,29 +284,24 @@
 | `OPEN_BRACKET` | `r'\['` |
 | `CLOSE_BRACKET` | `r'\]'` |
 | `BACKSLASH` | `r'\\'` |
 | `PIPE` | `r'\|'` |
 | `BACK_1` | `r'\1'` |
 | `BACK_2` | `r'\2'` |
 | `BACK_3` | `r'\3'` |
-| `BACK_4` | `r'\4'` |
-| `BACK_5` | `r'\5'` |
-| `BACK_6` | `r'\6'` |
-| `BACK_7` | `r'\7'` |
-| `BACK_8` | `r'\8'` |
-| `BACK_9` | `r'\9'` |
+| ... | ... |
+| `BACK_99` | `r'\99'` |
 
 Humre also provides constants for commonly used patterns:
 
 | Humre Pattern Constants | Regex Equivalent | Note |
 |----------------------------------|------------------|------|
 | `ANYTHING` | `'.*?'` | lazy "zero or more of anything" match |
 | `EVERYTHING` | `'.*'` | greedy "zero or more of anything" match, aka dot star |
 | `SOMETHING` | `'.+?'` | lazy "one or more of anything" match |
-| `GREEDY_SOMETHING` | `'.+'` | greedy "one or more of anything" match |
 | `ANYCHAR` | `'.'` | |
 | `LETTER` | (too big to display) | Matches `isalpha()` |
 | `NONLETTER` | (too big to display) | Matches `not isalpha()` |
 | `UPPERCASE` | (too big to display) | Matches `isupper()` |
 | `NONUPPERCASE` | (too big to display) | Matches `not isupper()` |
 | `LOWERCASE` | (too big to display) | Matches `islower()` |
 | `NONLOWERCASE` | (too big to display) | Matches `not islower()` |
@@ -299,26 +309,9 @@
 | `NONALPHANUMERIC` | (too big to display) | Matches `not isalnum()` |
 | `HEXADECIMAL` | `'[0-9A-Fa-f]'` | |
 | `NONHEXADECIMAL` | `'[^0-9A-Fa-f]'` | |
 | `NUMBER` | `r'(?:\+&#124;-)?(?:(?:\d{1,3}(?:,\d{3})+)&#124;\d+)(?:\.\d+)?'` | Comma-formatted numbers |
 | `EURO_NUMBER` | `r'(?:\+&#124;-)?(?:(?:\d{1,3}(?:\.\d{3})+)&#124;\d+)(?:,\d+)?'` | Period-formatted numbers |
 | `HEXADECIMAL_NUMBER` | `'(?:(?:0x&#124;0X)[0-9a-f]+)&#124;(?:(?:0x&#124;0X)[0-9A-F]+)&#124;(?:[0-9a-f]+)&#124;(?:[0-9A-F]+)'` | Can have leading `0x` or `0X`. |
 
-Humre's `compile()` function's `flags` keyword argument takes the same flag values as `re.compile()`:
 
-| Humre `compile()` Flags | Equivalent `re.compile()` Flags | Meaning |
-|---|---|---|
-|`humre.A` | `re.A` | Same as `ASCII` |
-|`humre.ASCII` | `re.ASCII` | Makes several escapes like `\w`, `\b`, `\s` and `\d` match only on ASCII characters with the respective property. |
-|`humre.DEBUG` | `re.DEBUG` | Display debug information about compiled expression. |
-|`humre.I` | `re.I` | Same as `IGNORECASE` |
-|`humre.IGNORECASE` | `re.IGNORECASE` | Do case-insensitive matches. |
-|`humre.L` | `re.L` | Same as `LOCALE` |
-|`humre.LOCALE` | `re.LOCALE` | Do a locale-aware match. |
-|`humre.M` | `re.M` | Same as `MULTILINE` |
-|`humre.MULTILINE` | `re.MULTILINE` | Multi-line matching, affecting `^` and `$`. |
-|`humre.NOFLAG` | `re.NOFLAG` | Indicates no flag being applied. Used as a default value in function definitions. New in 3.11. |
-|`humre.S` | `re.S` | Same as `DOTALL`. Corresponds to the inline flag `(?s)`. |
-|`humre.DOTALL` | `re.DOTALL` | Make `.` match any character, including newlines. |
-|`humre.X` | `re.X` | Same as `VERBOSE` (X stands for "extended") |
-|`humre.VERBOSE` | `re.VERBOSE` | Enable verbose REs, which can be organized more cleanly and understandably. |
```

### Comparing `Humre-0.2.0/src/humre/__init__.py` & `Humre-1.0.0/src/humre/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,155 +3,105 @@
 
 A human-readable regular expression module for Python."""
 
 # TODO - add functionality to parse regex strings and create the humre code for it.
 # TODO - Add inline flags like '(?i)'
 
 import re
+from typing import List, Tuple  # noqa: F401
 
-try:
-    from typing import ParamSpecArgs
-except ImportError:
-    pass  # Do nothing if run with a version of Python that doesn't have type hints.
+__version__ = '1.0.0'
 
 # fmt: off
-__all__ = ['ALPHANUMERIC', 'ANYCHAR', 'ANYTHING', 'ASTERISK', 'BACKSLASH',
-'BACK_1', 'BACK_2', 'BACK_3', 'BACK_4', 'BACK_5', 'BACK_6', 'BACK_7',
-'BACK_8', 'BACK_9', 'BOUNDARY', 'CARET', 'CLOSE_BRACE', 'CLOSE_BRACKET',
-'CLOSE_PAREN', 'CLOSE_PARENTHESIS', 'DIGIT', 'DOLLAR', 'DOUBLE_QUOTE',
-'EURO_NUMBER', 'EVERYTHING', 'HEXADECIMAL',
-'HEXADECIMAL_NUMBER', 'LETTER', 'LOWERCASE', 'MINUS', 'NEWLINE',
-'NONALPHANUMERIC', 'NONDIGIT', 'NONHEXADECIMAL', 'NONLETTER', 'NONLOWERCASE',
-'NONNUMERIC', 'NONUPPERCASE', 'NONWHITESPACE', 'NONWORD', 'NUMBER',
-'NUMERIC', 'OPEN_BRACE', 'OPEN_BRACKET', 'OPEN_PAREN', 'OPEN_PARENTHESIS',
-'PERIOD', 'PIPE', 'PLUS', 'QUESTION_MARK', 'QUOTE', 'SOMETHING', 'TAB',
-'UPPERCASE', 'WHITESPACE', 'WORD', 'at_least', 'at_most',
-'atomic_group', 'back_ref', 'back_reference', 'between', 'chars', 'compile',
-'either', 'ends_with', 'esc', 'exactly', 'group', 'group_at_least',
-'group_at_most', 'group_between', 'group_chars', 'group_either',
-'group_exactly', 'group_nonchars', 'inline_flag', 'join', 'lookahead',
-'lookbehind', 'named_group', 'negative_lookahead', 'negative_lookbehind',
-'noncap_group', 'noncap_group_at_least', 'noncap_group_at_most',
-'noncap_group_between', 'noncap_group_chars', 'noncap_group_either',
-'noncap_group_exactly', 'noncap_group_nonchars', 'nonchars', 'one_or_more',
-'one_or_more_group', 'one_or_more_lazy', 'one_or_more_lazy_group',
-'one_or_more_lazy_noncap_group', 'one_or_more_noncap_group',
-'one_or_more_possessive', 'optional', 'optional_group',
-'optional_noncap_group', 'optional_possessive', 'positive_lookahead',
-'positive_lookbehind', 'starts_and_ends_with', 'starts_with', 'zero_or_more',
-'zero_or_more_group', 'zero_or_more_lazy', 'zero_or_more_lazy_group',
-'zero_or_more_lazy_noncap_group', 'zero_or_more_noncap_group',
-'zero_or_more_possessive']
+['ALPHANUMERIC', 'AMPERSAND', 'ANYCHAR', 'ANYTHING', 'ASTERISK', 'BACKSLASH', 'BACK_1', 'BACK_10', 'BACK_11', 'BACK_12', 'BACK_13', 'BACK_14', 'BACK_15', 'BACK_16', 'BACK_17', 'BACK_18', 'BACK_19', 'BACK_2', 'BACK_20', 'BACK_21', 'BACK_22', 'BACK_23', 'BACK_24', 'BACK_25', 'BACK_26', 'BACK_27', 'BACK_28', 'BACK_29', 'BACK_3', 'BACK_30', 'BACK_31', 'BACK_32', 'BACK_33', 'BACK_34', 'BACK_35', 'BACK_36', 'BACK_37', 'BACK_38', 'BACK_39', 'BACK_4', 'BACK_40', 'BACK_41', 'BACK_42', 'BACK_43', 'BACK_44', 'BACK_45', 'BACK_46', 'BACK_47', 'BACK_48', 'BACK_49', 'BACK_5', 'BACK_50', 'BACK_51', 'BACK_52', 'BACK_53', 'BACK_54', 'BACK_55', 'BACK_56', 'BACK_57', 'BACK_58', 'BACK_59', 'BACK_6', 'BACK_60', 'BACK_61', 'BACK_62', 'BACK_63', 'BACK_64', 'BACK_65', 'BACK_66', 'BACK_67', 'BACK_68', 'BACK_69', 'BACK_7', 'BACK_70', 'BACK_71', 'BACK_72', 'BACK_73', 'BACK_74', 'BACK_75', 'BACK_76', 'BACK_77', 'BACK_78', 'BACK_79', 'BACK_8', 'BACK_80', 'BACK_81', 'BACK_82', 'BACK_83', 'BACK_84', 'BACK_85', 'BACK_86', 'BACK_87', 'BACK_88', 'BACK_89', 'BACK_9', 'BACK_90', 'BACK_91', 'BACK_92', 'BACK_93', 'BACK_94', 'BACK_95', 'BACK_96', 'BACK_97', 'BACK_98', 'BACK_99', 'BOUNDARY', 'CARET', 'CLOSE_BRACE', 'CLOSE_BRACKET', 'CLOSE_PAREN', 'CLOSE_PARENTHESIS', 'DIGIT', 'DOLLAR', 'DOUBLE_QUOTE', 'EURO_NUMBER', 'EVERYTHING', 'HASHTAG', 'HEXADECIMAL', 'HEXADECIMAL_NUMBER', 'LETTER', 'LOWERCASE', 'MINUS', 'NEWLINE', 'NONALPHANUMERIC', 'NONDIGIT', 'NONHEXADECIMAL', 'NONLETTER', 'NONLOWERCASE', 'NONNUMERIC', 'NONUPPERCASE', 'NONWHITESPACE', 'NONWORD', 'NUMBER', 'NUMERIC', 'OPEN_BRACE', 'OPEN_BRACKET', 'OPEN_PAREN', 'OPEN_PARENTHESIS', 'PERIOD', 'PIPE', 'PLUS', 'QUESTION_MARK', 'QUOTE', 'SOMETHING', 'TAB', 'UPPERCASE', 'WHITESPACE', 'WORD', 'at_least', 'at_least_group', 'at_least_noncap_group', 'at_most', 'at_most_group', 'at_most_noncap_group', 'atomic_group', 'back_ref', 'back_reference', 'between', 'between_group', 'between_noncap_group', 'chars', 'either', 'ends_with', 'esc', 'exactly', 'exactly_group', 'exactly_noncap_group', 'group', 'group_either', 'inline_flag', 'join', 'lookahead', 'lookbehind', 'named_group', 'negative_lookahead', 'negative_lookbehind', 'noncap_group', 'noncap_group_either', 'nonchars', 'one_or_more', 'one_or_more_group', 'one_or_more_lazy', 'one_or_more_lazy_group', 'one_or_more_lazy_noncap_group', 'one_or_more_noncap_group', 'one_or_more_possessive', 'optional', 'optional_group', 'optional_noncap_group', 'optional_possessive', 'positive_lookahead', 'positive_lookbehind', 'starts_and_ends_with', 'starts_with', 'zero_or_more', 'zero_or_more_group', 'zero_or_more_lazy', 'zero_or_more_lazy_group', 'zero_or_more_lazy_noncap_group', 'zero_or_more_noncap_group', 'zero_or_more_possessive'] # type: List[str]
 # fmt: on
 
-__version__ = '0.2.0'
+# TODO - rename noncap to anon?
+
+
+DIGIT = r'\d'  # type: str
+WORD = r'\w'  # type: str
+WHITESPACE = r'\s'  # type: str
+NONDIGIT = r'\D'  # type: str
+NONWORD = r'\W'  # type: str
+NONWHITESPACE = r'\S'  # type: str
+
+BOUNDARY = r'\b'  # type: str
+# IGNORE_DIRECTIVE = '(?i)'    # type: str
 
-DIGIT = r'\d'
-WORD = r'\w'
-WHITESPACE = r'\s'
-NONDIGIT = r'\D'
-NONWORD = r'\W'
-NONWHITESPACE = r'\S'
-
-BOUNDARY = r'\b'
-# IGNORE_DIRECTIVE = '(?i)'
-
-
-# Constants copied from the re module. Note that these aren't included in
-# __all__ do the strong possibility that they'll conflict with existing
-# variable names.
-# Changed in version 3.6: Flag constants are now instances of RegexFlag,
-# which is a subclass of enum.IntFlag.
-"""
-# NOTE: Removed because names like A and DEBUG might be overriden.
-# We'll just use keyword arguments in compile() instead.
-A = re.A
-ASCII = re.ASCII
-DEBUG = re.DEBUG
-I = re.I
-IGNORECASE = re.IGNORECASE
-L = re.L
-LOCALE = re.LOCALE
-M = re.M
-MULTILINE = re.MULTILINE
-NOFLAG = 0  # re.NOFLAG  # New in 3.11
-S = re.S
-DOTALL = re.DOTALL
-X = re.X
-VERBOSE = re.VERBOSE
-"""
 
 # Built-in Humre character classes:
 
+
 # To avoid possible rendering issues with code editors, instead of
 # copy/pasting the unicode characters directly into the source, I'm
 # leaving them as integer ranges that get converted into the strings
-# by _getRegexCharacterClassStringFromCodePointRanges().
+# by _get_regex_character_class_string_from_code_point_ranges().
 # This part of the code is dedicated to Python core dev Łukasz Langa, who
 # is tired of having his name not be processed correctly by software.
 # https://youtu.be/7m5JA3XaZ4k
-def _getRegexCharacterClassStringFromCodePointRanges(tuple_of_ranges):
+def _get_regex_character_class_string_from_code_point_ranges(tuple_of_ranges):  # type: (List[Tuple[int, int]]) -> str
     # A helper function to convert integer ranges into regex character class strings.
     regex_str = []
     for start_range_code_point, end_range_code_point in tuple_of_ranges:
         if start_range_code_point == end_range_code_point:
             # This is not a range, just a single code point, so don't use a hyphen.
             regex_str.append(chr(start_range_code_point))
         else:
             regex_str.append(chr(start_range_code_point) + '-' + chr(end_range_code_point))
     return ''.join(regex_str)
 
 
 # fmt: off
 # These tuple of tuples of two integers are ranges of unicode code points.
-# We pass these to _getRegexCharacterClassStringFromCodePointRanges() to
+# We pass these to _get_regex_character_class_string_from_code_point_ranges() to
 # get a string to put inside a regex character class, like [a-z] but
 # much, much more specific.
 # The numbers come from testing every character against Python's islower(),
 # isupper(), isalpha(), and isnumeric() string methods.
-_lowercaseCharClass = _getRegexCharacterClassStringFromCodePointRanges(
-    (
-        (97, 122), (170, 170), (181, 181), (186, 186), (223, 246), (248, 255), (257, 257), (259, 259), (261, 261), (263, 263), (265, 265), (267, 267), (269, 269), (271, 271), (273, 273), (275, 275), (277, 277), (279, 279), (281, 281), (283, 283), (285, 285), (287, 287), (289, 289), (291, 291), (293, 293), (295, 295), (297, 297), (299, 299), (301, 301), (303, 303), (305, 305), (307, 307), (309, 309), (311, 312), (314, 314), (316, 316), (318, 318), (320, 320), (322, 322), (324, 324), (326, 326), (328, 329), (331, 331), (333, 333), (335, 335), (337, 337), (339, 339), (341, 341), (343, 343), (345, 345), (347, 347), (349, 349), (351, 351), (353, 353), (355, 355), (357, 357), (359, 359), (361, 361), (363, 363), (365, 365), (367, 367), (369, 369), (371, 371), (373, 373), (375, 375), (378, 378), (380, 380), (382, 384), (387, 387), (389, 389), (392, 392), (396, 397), (402, 402), (405, 405), (409, 411), (414, 414), (417, 417), (419, 419), (421, 421), (424, 424), (426, 427), (429, 429), (432, 432), (436, 436), (438, 438), (441, 442), (445, 447), (454, 454), (457, 457), (460, 460), (462, 462), (464, 464), (466, 466), (468, 468), (470, 470), (472, 472), (474, 474), (476, 477), (479, 479), (481, 481), (483, 483), (485, 485), (487, 487), (489, 489), (491, 491), (493, 493), (495, 496), (499, 499), (501, 501), (505, 505), (507, 507), (509, 509), (511, 511), (513, 513), (515, 515), (517, 517), (519, 519), (521, 521), (523, 523), (525, 525), (527, 527), (529, 529), (531, 531), (533, 533), (535, 535), (537, 537), (539, 539), (541, 541), (543, 543), (545, 545), (547, 547), (549, 549), (551, 551), (553, 553), (555, 555), (557, 557), (559, 559), (561, 561), (563, 569), (572, 572), (575, 576), (578, 578), (583, 583), (585, 585), (587, 587), (589, 589), (591, 659), (661, 696), (704, 705), (736, 740), (837, 837), (881, 881), (883, 883), (887, 887), (890, 893), (912, 912), (940, 974), (976, 977), (981, 983), (985, 985), (987, 987), (989, 989), (991, 991), (993, 993), (995, 995), (997, 997), (999, 999), (1001, 1001), (1003, 1003), (1005, 1005), (1007, 1011), (1013, 1013), (1016, 1016), (1019, 1020), (1072, 1119), (1121, 1121), (1123, 1123), (1125, 1125), (1127, 1127), (1129, 1129), (1131, 1131), (1133, 1133), (1135, 1135), (1137, 1137), (1139, 1139), (1141, 1141), (1143, 1143), (1145, 1145), (1147, 1147), (1149, 1149), (1151, 1151), (1153, 1153), (1163, 1163), (1165, 1165), (1167, 1167), (1169, 1169), (1171, 1171), (1173, 1173), (1175, 1175), (1177, 1177), (1179, 1179), (1181, 1181), (1183, 1183), (1185, 1185), (1187, 1187), (1189, 1189), (1191, 1191), (1193, 1193), (1195, 1195), (1197, 1197), (1199, 1199), (1201, 1201), (1203, 1203), (1205, 1205), (1207, 1207), (1209, 1209), (1211, 1211), (1213, 1213), (1215, 1215), (1218, 1218), (1220, 1220), (1222, 1222), (1224, 1224), (1226, 1226), (1228, 1228), (1230, 1231), (1233, 1233), (1235, 1235), (1237, 1237), (1239, 1239), (1241, 1241), (1243, 1243), (1245, 1245), (1247, 1247), (1249, 1249), (1251, 1251), (1253, 1253), (1255, 1255), (1257, 1257), (1259, 1259), (1261, 1261), (1263, 1263), (1265, 1265), (1267, 1267), (1269, 1269), (1271, 1271), (1273, 1273), (1275, 1275), (1277, 1277), (1279, 1279), (1281, 1281), (1283, 1283), (1285, 1285), (1287, 1287), (1289, 1289), (1291, 1291), (1293, 1293), (1295, 1295), (1297, 1297), (1299, 1299), (1301, 1301), (1303, 1303), (1305, 1305), (1307, 1307), (1309, 1309), (1311, 1311), (1313, 1313), (1315, 1315), (1317, 1317), (1319, 1319), (1321, 1321), (1323, 1323), (1325, 1325), (1327, 1327), (1376, 1416), (4304, 4346), (4349, 4351), (5112, 5117), (7296, 7304), (7424, 7615), (7681, 7681), (7683, 7683), (7685, 7685), (7687, 7687), (7689, 7689), (7691, 7691), (7693, 7693), (7695, 7695), (7697, 7697), (7699, 7699), (7701, 7701), (7703, 7703), (7705, 7705), (7707, 7707), (7709, 7709), (7711, 7711), (7713, 7713), (7715, 7715), (7717, 7717), (7719, 7719), (7721, 7721), (7723, 7723), (7725, 7725), (7727, 7727), (7729, 7729), (7731, 7731), (7733, 7733), (7735, 7735), (7737, 7737), (7739, 7739), (7741, 7741), (7743, 7743), (7745, 7745), (7747, 7747), (7749, 7749), (7751, 7751), (7753, 7753), (7755, 7755), (7757, 7757), (7759, 7759), (7761, 7761), (7763, 7763), (7765, 7765), (7767, 7767), (7769, 7769), (7771, 7771), (7773, 7773), (7775, 7775), (7777, 7777), (7779, 7779), (7781, 7781), (7783, 7783), (7785, 7785), (7787, 7787), (7789, 7789), (7791, 7791), (7793, 7793), (7795, 7795), (7797, 7797), (7799, 7799), (7801, 7801), (7803, 7803), (7805, 7805), (7807, 7807), (7809, 7809), (7811, 7811), (7813, 7813), (7815, 7815), (7817, 7817), (7819, 7819), (7821, 7821), (7823, 7823), (7825, 7825), (7827, 7827), (7829, 7837), (7839, 7839), (7841, 7841), (7843, 7843), (7845, 7845), (7847, 7847), (7849, 7849), (7851, 7851), (7853, 7853), (7855, 7855), (7857, 7857), (7859, 7859), (7861, 7861), (7863, 7863), (7865, 7865), (7867, 7867), (7869, 7869), (7871, 7871), (7873, 7873), (7875, 7875), (7877, 7877), (7879, 7879), (7881, 7881), (7883, 7883), (7885, 7885), (7887, 7887), (7889, 7889), (7891, 7891), (7893, 7893), (7895, 7895), (7897, 7897), (7899, 7899), (7901, 7901), (7903, 7903), (7905, 7905), (7907, 7907), (7909, 7909), (7911, 7911), (7913, 7913), (7915, 7915), (7917, 7917), (7919, 7919), (7921, 7921), (7923, 7923), (7925, 7925), (7927, 7927), (7929, 7929), (7931, 7931), (7933, 7933), (7935, 7943), (7952, 7957), (7968, 7975), (7984, 7991), (8000, 8005), (8016, 8023), (8032, 8039), (8048, 8061), (8064, 8071), (8080, 8087), (8096, 8103), (8112, 8116), (8118, 8119), (8126, 8126), (8130, 8132), (8134, 8135), (8144, 8147), (8150, 8151), (8160, 8167), (8178, 8180), (8182, 8183), (8305, 8305), (8319, 8319), (8336, 8348), (8458, 8458), (8462, 8463), (8467, 8467), (8495, 8495), (8500, 8500), (8505, 8505), (8508, 8509), (8518, 8521), (8526, 8526), (8560, 8575), (8580, 8580), (9424, 9449), (11312, 11358), (11361, 11361), (11365, 11366), (11368, 11368), (11370, 11370), (11372, 11372), (11377, 11377), (11379, 11380), (11382, 11389), (11393, 11393), (11395, 11395), (11397, 11397), (11399, 11399), (11401, 11401), (11403, 11403), (11405, 11405), (11407, 11407), (11409, 11409), (11411, 11411), (11413, 11413), (11415, 11415), (11417, 11417), (11419, 11419), (11421, 11421), (11423, 11423), (11425, 11425), (11427, 11427), (11429, 11429), (11431, 11431), (11433, 11433), (11435, 11435), (11437, 11437), (11439, 11439), (11441, 11441), (11443, 11443), (11445, 11445), (11447, 11447), (11449, 11449), (11451, 11451), (11453, 11453), (11455, 11455), (11457, 11457), (11459, 11459), (11461, 11461), (11463, 11463), (11465, 11465), (11467, 11467), (11469, 11469), (11471, 11471), (11473, 11473), (11475, 11475), (11477, 11477), (11479, 11479), (11481, 11481), (11483, 11483), (11485, 11485), (11487, 11487), (11489, 11489), (11491, 11492), (11500, 11500), (11502, 11502), (11507, 11507), (11520, 11557), (11559, 11559), (11565, 11565), (42561, 42561), (42563, 42563), (42565, 42565), (42567, 42567), (42569, 42569), (42571, 42571), (42573, 42573), (42575, 42575), (42577, 42577), (42579, 42579), (42581, 42581), (42583, 42583), (42585, 42585), (42587, 42587), (42589, 42589), (42591, 42591), (42593, 42593), (42595, 42595), (42597, 42597), (42599, 42599), (42601, 42601), (42603, 42603), (42605, 42605), (42625, 42625), (42627, 42627), (42629, 42629), (42631, 42631), (42633, 42633), (42635, 42635), (42637, 42637), (42639, 42639), (42641, 42641), (42643, 42643), (42645, 42645), (42647, 42647), (42649, 42649), (42651, 42653), (42787, 42787), (42789, 42789), (42791, 42791), (42793, 42793), (42795, 42795), (42797, 42797), (42799, 42801), (42803, 42803), (42805, 42805), (42807, 42807), (42809, 42809), (42811, 42811), (42813, 42813), (42815, 42815), (42817, 42817), (42819, 42819), (42821, 42821), (42823, 42823), (42825, 42825), (42827, 42827), (42829, 42829), (42831, 42831), (42833, 42833), (42835, 42835), (42837, 42837), (42839, 42839), (42841, 42841), (42843, 42843), (42845, 42845), (42847, 42847), (42849, 42849), (42851, 42851), (42853, 42853), (42855, 42855), (42857, 42857), (42859, 42859), (42861, 42861), (42863, 42872), (42874, 42874), (42876, 42876), (42879, 42879), (42881, 42881), (42883, 42883), (42885, 42885), (42887, 42887), (42892, 42892), (42894, 42894), (42897, 42897), (42899, 42901), (42903, 42903), (42905, 42905), (42907, 42907), (42909, 42909), (42911, 42911), (42913, 42913), (42915, 42915), (42917, 42917), (42919, 42919), (42921, 42921), (42927, 42927), (42933, 42933), (42935, 42935), (42937, 42937), (42939, 42939), (42941, 42941), (42943, 42943), (42947, 42947), (42952, 42952), (42954, 42954), (42998, 42998), (43000, 43002), (43824, 43866), (43868, 43880), (43888, 43967), (64256, 64262), (64275, 64279), (65345, 65370), (66600, 66639), (66776, 66811), (68800, 68850), (71872, 71903), (93792, 93823), (119834, 119859), (119886, 119892), (119894, 119911), (119938, 119963), (119990, 119993), (119995, 119995), (119997, 120003), (120005, 120015), (120042, 120067), (120094, 120119), (120146, 120171), (120198, 120223), (120250, 120275), (120302, 120327), (120354, 120379), (120406, 120431), (120458, 120485), (120514, 120538), (120540, 120545), (120572, 120596), (120598, 120603), (120630, 120654), (120656, 120661), (120688, 120712), (120714, 120719), (120746, 120770), (120772, 120777), (120779, 120779), (125218, 125251),
-    )
-)
-_uppercaseCharClass = _getRegexCharacterClassStringFromCodePointRanges(
-    (
-        (65, 90), (192, 214), (216, 222), (256, 256), (258, 258), (260, 260), (262, 262), (264, 264), (266, 266), (268, 268), (270, 270), (272, 272), (274, 274), (276, 276), (278, 278), (280, 280), (282, 282), (284, 284), (286, 286), (288, 288), (290, 290), (292, 292), (294, 294), (296, 296), (298, 298), (300, 300), (302, 302), (304, 304), (306, 306), (308, 308), (310, 310), (313, 313), (315, 315), (317, 317), (319, 319), (321, 321), (323, 323), (325, 325), (327, 327), (330, 330), (332, 332), (334, 334), (336, 336), (338, 338), (340, 340), (342, 342), (344, 344), (346, 346), (348, 348), (350, 350), (352, 352), (354, 354), (356, 356), (358, 358), (360, 360), (362, 362), (364, 364), (366, 366), (368, 368), (370, 370), (372, 372), (374, 374), (376, 377), (379, 379), (381, 381), (385, 386), (388, 388), (390, 391), (393, 395), (398, 401), (403, 404), (406, 408), (412, 413), (415, 416), (418, 418), (420, 420), (422, 423), (425, 425), (428, 428), (430, 431), (433, 435), (437, 437), (439, 440), (444, 444), (452, 452), (455, 455), (458, 458), (461, 461), (463, 463), (465, 465), (467, 467), (469, 469), (471, 471), (473, 473), (475, 475), (478, 478), (480, 480), (482, 482), (484, 484), (486, 486), (488, 488), (490, 490), (492, 492), (494, 494), (497, 497), (500, 500), (502, 504), (506, 506), (508, 508), (510, 510), (512, 512), (514, 514), (516, 516), (518, 518), (520, 520), (522, 522), (524, 524), (526, 526), (528, 528), (530, 530), (532, 532), (534, 534), (536, 536), (538, 538), (540, 540), (542, 542), (544, 544), (546, 546), (548, 548), (550, 550), (552, 552), (554, 554), (556, 556), (558, 558), (560, 560), (562, 562), (570, 571), (573, 574), (577, 577), (579, 582), (584, 584), (586, 586), (588, 588), (590, 590), (880, 880), (882, 882), (886, 886), (895, 895), (902, 902), (904, 906), (908, 908), (910, 911), (913, 929), (931, 939), (975, 975), (978, 980), (984, 984), (986, 986), (988, 988), (990, 990), (992, 992), (994, 994), (996, 996), (998, 998), (1000, 1000), (1002, 1002), (1004, 1004), (1006, 1006), (1012, 1012), (1015, 1015), (1017, 1018), (1021, 1071), (1120, 1120), (1122, 1122), (1124, 1124), (1126, 1126), (1128, 1128), (1130, 1130), (1132, 1132), (1134, 1134), (1136, 1136), (1138, 1138), (1140, 1140), (1142, 1142), (1144, 1144), (1146, 1146), (1148, 1148), (1150, 1150), (1152, 1152), (1162, 1162), (1164, 1164), (1166, 1166), (1168, 1168), (1170, 1170), (1172, 1172), (1174, 1174), (1176, 1176), (1178, 1178), (1180, 1180), (1182, 1182), (1184, 1184), (1186, 1186), (1188, 1188), (1190, 1190), (1192, 1192), (1194, 1194), (1196, 1196), (1198, 1198), (1200, 1200), (1202, 1202), (1204, 1204), (1206, 1206), (1208, 1208), (1210, 1210), (1212, 1212), (1214, 1214), (1216, 1217), (1219, 1219), (1221, 1221), (1223, 1223), (1225, 1225), (1227, 1227), (1229, 1229), (1232, 1232), (1234, 1234), (1236, 1236), (1238, 1238), (1240, 1240), (1242, 1242), (1244, 1244), (1246, 1246), (1248, 1248), (1250, 1250), (1252, 1252), (1254, 1254), (1256, 1256), (1258, 1258), (1260, 1260), (1262, 1262), (1264, 1264), (1266, 1266), (1268, 1268), (1270, 1270), (1272, 1272), (1274, 1274), (1276, 1276), (1278, 1278), (1280, 1280), (1282, 1282), (1284, 1284), (1286, 1286), (1288, 1288), (1290, 1290), (1292, 1292), (1294, 1294), (1296, 1296), (1298, 1298), (1300, 1300), (1302, 1302), (1304, 1304), (1306, 1306), (1308, 1308), (1310, 1310), (1312, 1312), (1314, 1314), (1316, 1316), (1318, 1318), (1320, 1320), (1322, 1322), (1324, 1324), (1326, 1326), (1329, 1366), (4256, 4293), (4295, 4295), (4301, 4301), (5024, 5109), (7312, 7354), (7357, 7359), (7680, 7680), (7682, 7682), (7684, 7684), (7686, 7686), (7688, 7688), (7690, 7690), (7692, 7692), (7694, 7694), (7696, 7696), (7698, 7698), (7700, 7700), (7702, 7702), (7704, 7704), (7706, 7706), (7708, 7708), (7710, 7710), (7712, 7712), (7714, 7714), (7716, 7716), (7718, 7718), (7720, 7720), (7722, 7722), (7724, 7724), (7726, 7726), (7728, 7728), (7730, 7730), (7732, 7732), (7734, 7734), (7736, 7736), (7738, 7738), (7740, 7740), (7742, 7742), (7744, 7744), (7746, 7746), (7748, 7748), (7750, 7750), (7752, 7752), (7754, 7754), (7756, 7756), (7758, 7758), (7760, 7760), (7762, 7762), (7764, 7764), (7766, 7766), (7768, 7768), (7770, 7770), (7772, 7772), (7774, 7774), (7776, 7776), (7778, 7778), (7780, 7780), (7782, 7782), (7784, 7784), (7786, 7786), (7788, 7788), (7790, 7790), (7792, 7792), (7794, 7794), (7796, 7796), (7798, 7798), (7800, 7800), (7802, 7802), (7804, 7804), (7806, 7806), (7808, 7808), (7810, 7810), (7812, 7812), (7814, 7814), (7816, 7816), (7818, 7818), (7820, 7820), (7822, 7822), (7824, 7824), (7826, 7826), (7828, 7828), (7838, 7838), (7840, 7840), (7842, 7842), (7844, 7844), (7846, 7846), (7848, 7848), (7850, 7850), (7852, 7852), (7854, 7854), (7856, 7856), (7858, 7858), (7860, 7860), (7862, 7862), (7864, 7864), (7866, 7866), (7868, 7868), (7870, 7870), (7872, 7872), (7874, 7874), (7876, 7876), (7878, 7878), (7880, 7880), (7882, 7882), (7884, 7884), (7886, 7886), (7888, 7888), (7890, 7890), (7892, 7892), (7894, 7894), (7896, 7896), (7898, 7898), (7900, 7900), (7902, 7902), (7904, 7904), (7906, 7906), (7908, 7908), (7910, 7910), (7912, 7912), (7914, 7914), (7916, 7916), (7918, 7918), (7920, 7920), (7922, 7922), (7924, 7924), (7926, 7926), (7928, 7928), (7930, 7930), (7932, 7932), (7934, 7934), (7944, 7951), (7960, 7965), (7976, 7983), (7992, 7999), (8008, 8013), (8025, 8025), (8027, 8027), (8029, 8029), (8031, 8031), (8040, 8047), (8120, 8123), (8136, 8139), (8152, 8155), (8168, 8172), (8184, 8187), (8450, 8450), (8455, 8455), (8459, 8461), (8464, 8466), (8469, 8469), (8473, 8477), (8484, 8484), (8486, 8486), (8488, 8488), (8490, 8493), (8496, 8499), (8510, 8511), (8517, 8517), (8544, 8559), (8579, 8579), (9398, 9423), (11264, 11310), (11360, 11360), (11362, 11364), (11367, 11367), (11369, 11369), (11371, 11371), (11373, 11376), (11378, 11378), (11381, 11381), (11390, 11392), (11394, 11394), (11396, 11396), (11398, 11398), (11400, 11400), (11402, 11402), (11404, 11404), (11406, 11406), (11408, 11408), (11410, 11410), (11412, 11412), (11414, 11414), (11416, 11416), (11418, 11418), (11420, 11420), (11422, 11422), (11424, 11424), (11426, 11426), (11428, 11428), (11430, 11430), (11432, 11432), (11434, 11434), (11436, 11436), (11438, 11438), (11440, 11440), (11442, 11442), (11444, 11444), (11446, 11446), (11448, 11448), (11450, 11450), (11452, 11452), (11454, 11454), (11456, 11456), (11458, 11458), (11460, 11460), (11462, 11462), (11464, 11464), (11466, 11466), (11468, 11468), (11470, 11470), (11472, 11472), (11474, 11474), (11476, 11476), (11478, 11478), (11480, 11480), (11482, 11482), (11484, 11484), (11486, 11486), (11488, 11488), (11490, 11490), (11499, 11499), (11501, 11501), (11506, 11506), (42560, 42560), (42562, 42562), (42564, 42564), (42566, 42566), (42568, 42568), (42570, 42570), (42572, 42572), (42574, 42574), (42576, 42576), (42578, 42578), (42580, 42580), (42582, 42582), (42584, 42584), (42586, 42586), (42588, 42588), (42590, 42590), (42592, 42592), (42594, 42594), (42596, 42596), (42598, 42598), (42600, 42600), (42602, 42602), (42604, 42604), (42624, 42624), (42626, 42626), (42628, 42628), (42630, 42630), (42632, 42632), (42634, 42634), (42636, 42636), (42638, 42638), (42640, 42640), (42642, 42642), (42644, 42644), (42646, 42646), (42648, 42648), (42650, 42650), (42786, 42786), (42788, 42788), (42790, 42790), (42792, 42792), (42794, 42794), (42796, 42796), (42798, 42798), (42802, 42802), (42804, 42804), (42806, 42806), (42808, 42808), (42810, 42810), (42812, 42812), (42814, 42814), (42816, 42816), (42818, 42818), (42820, 42820), (42822, 42822), (42824, 42824), (42826, 42826), (42828, 42828), (42830, 42830), (42832, 42832), (42834, 42834), (42836, 42836), (42838, 42838), (42840, 42840), (42842, 42842), (42844, 42844), (42846, 42846), (42848, 42848), (42850, 42850), (42852, 42852), (42854, 42854), (42856, 42856), (42858, 42858), (42860, 42860), (42862, 42862), (42873, 42873), (42875, 42875), (42877, 42878), (42880, 42880), (42882, 42882), (42884, 42884), (42886, 42886), (42891, 42891), (42893, 42893), (42896, 42896), (42898, 42898), (42902, 42902), (42904, 42904), (42906, 42906), (42908, 42908), (42910, 42910), (42912, 42912), (42914, 42914), (42916, 42916), (42918, 42918), (42920, 42920), (42922, 42926), (42928, 42932), (42934, 42934), (42936, 42936), (42938, 42938), (42940, 42940), (42942, 42942), (42946, 42946), (42948, 42951), (42953, 42953), (42997, 42997), (65313, 65338), (66560, 66599), (66736, 66771), (68736, 68786), (71840, 71871), (93760, 93791), (119808, 119833), (119860, 119885), (119912, 119937), (119964, 119964), (119966, 119967), (119970, 119970), (119973, 119974), (119977, 119980), (119982, 119989), (120016, 120041), (120068, 120069), (120071, 120074), (120077, 120084), (120086, 120092), (120120, 120121), (120123, 120126), (120128, 120132), (120134, 120134), (120138, 120144), (120172, 120197), (120224, 120249), (120276, 120301), (120328, 120353), (120380, 120405), (120432, 120457), (120488, 120512), (120546, 120570), (120604, 120628), (120662, 120686), (120720, 120744), (120778, 120778), (125184, 125217), (127280, 127305), (127312, 127337), (127344, 127369),
-    )
-)
-_letterCharClass = _getRegexCharacterClassStringFromCodePointRanges(
-    (
-        (65, 90), (97, 122), (170, 170), (181, 181), (186, 186), (192, 214), (216, 246), (248, 705), (710, 721), (736, 740), (748, 748), (750, 750), (880, 884), (886, 887), (890, 893), (895, 895), (902, 902), (904, 906), (908, 908), (910, 929), (931, 1013), (1015, 1153), (1162, 1327), (1329, 1366), (1369, 1369), (1376, 1416), (1488, 1514), (1519, 1522), (1568, 1610), (1646, 1647), (1649, 1747), (1749, 1749), (1765, 1766), (1774, 1775), (1786, 1788), (1791, 1791), (1808, 1808), (1810, 1839), (1869, 1957), (1969, 1969), (1994, 2026), (2036, 2037), (2042, 2042), (2048, 2069), (2074, 2074), (2084, 2084), (2088, 2088), (2112, 2136), (2144, 2154), (2208, 2228), (2230, 2247), (2308, 2361), (2365, 2365), (2384, 2384), (2392, 2401), (2417, 2432), (2437, 2444), (2447, 2448), (2451, 2472), (2474, 2480), (2482, 2482), (2486, 2489), (2493, 2493), (2510, 2510), (2524, 2525), (2527, 2529), (2544, 2545), (2556, 2556), (2565, 2570), (2575, 2576), (2579, 2600), (2602, 2608), (2610, 2611), (2613, 2614), (2616, 2617), (2649, 2652), (2654, 2654), (2674, 2676), (2693, 2701), (2703, 2705), (2707, 2728), (2730, 2736), (2738, 2739), (2741, 2745), (2749, 2749), (2768, 2768), (2784, 2785), (2809, 2809), (2821, 2828), (2831, 2832), (2835, 2856), (2858, 2864), (2866, 2867), (2869, 2873), (2877, 2877), (2908, 2909), (2911, 2913), (2929, 2929), (2947, 2947), (2949, 2954), (2958, 2960), (2962, 2965), (2969, 2970), (2972, 2972), (2974, 2975), (2979, 2980), (2984, 2986), (2990, 3001), (3024, 3024), (3077, 3084), (3086, 3088), (3090, 3112), (3114, 3129), (3133, 3133), (3160, 3162), (3168, 3169), (3200, 3200), (3205, 3212), (3214, 3216), (3218, 3240), (3242, 3251), (3253, 3257), (3261, 3261), (3294, 3294), (3296, 3297), (3313, 3314), (3332, 3340), (3342, 3344), (3346, 3386), (3389, 3389), (3406, 3406), (3412, 3414), (3423, 3425), (3450, 3455), (3461, 3478), (3482, 3505), (3507, 3515), (3517, 3517), (3520, 3526), (3585, 3632), (3634, 3635), (3648, 3654), (3713, 3714), (3716, 3716), (3718, 3722), (3724, 3747), (3749, 3749), (3751, 3760), (3762, 3763), (3773, 3773), (3776, 3780), (3782, 3782), (3804, 3807), (3840, 3840), (3904, 3911), (3913, 3948), (3976, 3980), (4096, 4138), (4159, 4159), (4176, 4181), (4186, 4189), (4193, 4193), (4197, 4198), (4206, 4208), (4213, 4225), (4238, 4238), (4256, 4293), (4295, 4295), (4301, 4301), (4304, 4346), (4348, 4680), (4682, 4685), (4688, 4694), (4696, 4696), (4698, 4701), (4704, 4744), (4746, 4749), (4752, 4784), (4786, 4789), (4792, 4798), (4800, 4800), (4802, 4805), (4808, 4822), (4824, 4880), (4882, 4885), (4888, 4954), (4992, 5007), (5024, 5109), (5112, 5117), (5121, 5740), (5743, 5759), (5761, 5786), (5792, 5866), (5873, 5880), (5888, 5900), (5902, 5905), (5920, 5937), (5952, 5969), (5984, 5996), (5998, 6000), (6016, 6067), (6103, 6103), (6108, 6108), (6176, 6264), (6272, 6276), (6279, 6312), (6314, 6314), (6320, 6389), (6400, 6430), (6480, 6509), (6512, 6516), (6528, 6571), (6576, 6601), (6656, 6678), (6688, 6740), (6823, 6823), (6917, 6963), (6981, 6987), (7043, 7072), (7086, 7087), (7098, 7141), (7168, 7203), (7245, 7247), (7258, 7293), (7296, 7304), (7312, 7354), (7357, 7359), (7401, 7404), (7406, 7411), (7413, 7414), (7418, 7418), (7424, 7615), (7680, 7957), (7960, 7965), (7968, 8005), (8008, 8013), (8016, 8023), (8025, 8025), (8027, 8027), (8029, 8029), (8031, 8061), (8064, 8116), (8118, 8124), (8126, 8126), (8130, 8132), (8134, 8140), (8144, 8147), (8150, 8155), (8160, 8172), (8178, 8180), (8182, 8188), (8305, 8305), (8319, 8319), (8336, 8348), (8450, 8450), (8455, 8455), (8458, 8467), (8469, 8469), (8473, 8477), (8484, 8484), (8486, 8486), (8488, 8488), (8490, 8493), (8495, 8505), (8508, 8511), (8517, 8521), (8526, 8526), (8579, 8580), (11264, 11310), (11312, 11358), (11360, 11492), (11499, 11502), (11506, 11507), (11520, 11557), (11559, 11559), (11565, 11565), (11568, 11623), (11631, 11631), (11648, 11670), (11680, 11686), (11688, 11694), (11696, 11702), (11704, 11710), (11712, 11718), (11720, 11726), (11728, 11734), (11736, 11742), (11823, 11823), (12293, 12294), (12337, 12341), (12347, 12348), (12353, 12438), (12445, 12447), (12449, 12538), (12540, 12543), (12549, 12591), (12593, 12686), (12704, 12735), (12784, 12799), (13312, 19903), (19968, 40956), (40960, 42124), (42192, 42237), (42240, 42508), (42512, 42527), (42538, 42539), (42560, 42606), (42623, 42653), (42656, 42725), (42775, 42783), (42786, 42888), (42891, 42943), (42946, 42954), (42997, 43009), (43011, 43013), (43015, 43018), (43020, 43042), (43072, 43123), (43138, 43187), (43250, 43255), (43259, 43259), (43261, 43262), (43274, 43301), (43312, 43334), (43360, 43388), (43396, 43442), (43471, 43471), (43488, 43492), (43494, 43503), (43514, 43518), (43520, 43560), (43584, 43586), (43588, 43595), (43616, 43638), (43642, 43642), (43646, 43695), (43697, 43697), (43701, 43702), (43705, 43709), (43712, 43712), (43714, 43714), (43739, 43741), (43744, 43754), (43762, 43764), (43777, 43782), (43785, 43790), (43793, 43798), (43808, 43814), (43816, 43822), (43824, 43866), (43868, 43881), (43888, 44002), (44032, 55203), (55216, 55238), (55243, 55291), (63744, 64109), (64112, 64217), (64256, 64262), (64275, 64279), (64285, 64285), (64287, 64296), (64298, 64310), (64312, 64316), (64318, 64318), (64320, 64321), (64323, 64324), (64326, 64433), (64467, 64829), (64848, 64911), (64914, 64967), (65008, 65019), (65136, 65140), (65142, 65276), (65313, 65338), (65345, 65370), (65382, 65470), (65474, 65479), (65482, 65487), (65490, 65495), (65498, 65500), (65536, 65547), (65549, 65574), (65576, 65594), (65596, 65597), (65599, 65613), (65616, 65629), (65664, 65786), (66176, 66204), (66208, 66256), (66304, 66335), (66349, 66368), (66370, 66377), (66384, 66421), (66432, 66461), (66464, 66499), (66504, 66511), (66560, 66717), (66736, 66771), (66776, 66811), (66816, 66855), (66864, 66915), (67072, 67382), (67392, 67413), (67424, 67431), (67584, 67589), (67592, 67592), (67594, 67637), (67639, 67640), (67644, 67644), (67647, 67669), (67680, 67702), (67712, 67742), (67808, 67826), (67828, 67829), (67840, 67861), (67872, 67897), (67968, 68023), (68030, 68031), (68096, 68096), (68112, 68115), (68117, 68119), (68121, 68149), (68192, 68220), (68224, 68252), (68288, 68295), (68297, 68324), (68352, 68405), (68416, 68437), (68448, 68466), (68480, 68497), (68608, 68680), (68736, 68786), (68800, 68850), (68864, 68899), (69248, 69289), (69296, 69297), (69376, 69404), (69415, 69415), (69424, 69445), (69552, 69572), (69600, 69622), (69635, 69687), (69763, 69807), (69840, 69864), (69891, 69926), (69956, 69956), (69959, 69959), (69968, 70002), (70006, 70006), (70019, 70066), (70081, 70084), (70106, 70106), (70108, 70108), (70144, 70161), (70163, 70187), (70272, 70278), (70280, 70280), (70282, 70285), (70287, 70301), (70303, 70312), (70320, 70366), (70405, 70412), (70415, 70416), (70419, 70440), (70442, 70448), (70450, 70451), (70453, 70457), (70461, 70461), (70480, 70480), (70493, 70497), (70656, 70708), (70727, 70730), (70751, 70753), (70784, 70831), (70852, 70853), (70855, 70855), (71040, 71086), (71128, 71131), (71168, 71215), (71236, 71236), (71296, 71338), (71352, 71352), (71424, 71450), (71680, 71723), (71840, 71903), (71935, 71942), (71945, 71945), (71948, 71955), (71957, 71958), (71960, 71983), (71999, 71999), (72001, 72001), (72096, 72103), (72106, 72144), (72161, 72161), (72163, 72163), (72192, 72192), (72203, 72242), (72250, 72250), (72272, 72272), (72284, 72329), (72349, 72349), (72384, 72440), (72704, 72712), (72714, 72750), (72768, 72768), (72818, 72847), (72960, 72966), (72968, 72969), (72971, 73008), (73030, 73030), (73056, 73061), (73063, 73064), (73066, 73097), (73112, 73112), (73440, 73458), (73648, 73648), (73728, 74649), (74880, 75075), (77824, 78894), (82944, 83526), (92160, 92728), (92736, 92766), (92880, 92909), (92928, 92975), (92992, 92995), (93027, 93047), (93053, 93071), (93760, 93823), (93952, 94026), (94032, 94032), (94099, 94111), (94176, 94177), (94179, 94179), (94208, 100343), (100352, 101589), (101632, 101640), (110592, 110878), (110928, 110930), (110948, 110951), (110960, 111355), (113664, 113770), (113776, 113788), (113792, 113800), (113808, 113817), (119808, 119892), (119894, 119964), (119966, 119967), (119970, 119970), (119973, 119974), (119977, 119980), (119982, 119993), (119995, 119995), (119997, 120003), (120005, 120069), (120071, 120074), (120077, 120084), (120086, 120092), (120094, 120121), (120123, 120126), (120128, 120132), (120134, 120134), (120138, 120144), (120146, 120485), (120488, 120512), (120514, 120538), (120540, 120570), (120572, 120596), (120598, 120628), (120630, 120654), (120656, 120686), (120688, 120712), (120714, 120744), (120746, 120770), (120772, 120779), (123136, 123180), (123191, 123197), (123214, 123214), (123584, 123627), (124928, 125124), (125184, 125251), (125259, 125259), (126464, 126467), (126469, 126495), (126497, 126498), (126500, 126500), (126503, 126503), (126505, 126514), (126516, 126519), (126521, 126521), (126523, 126523), (126530, 126530), (126535, 126535), (126537, 126537), (126539, 126539), (126541, 126543), (126545, 126546), (126548, 126548), (126551, 126551), (126553, 126553), (126555, 126555), (126557, 126557), (126559, 126559), (126561, 126562), (126564, 126564), (126567, 126570), (126572, 126578), (126580, 126583), (126585, 126588), (126590, 126590), (126592, 126601), (126603, 126619), (126625, 126627), (126629, 126633), (126635, 126651), (131072, 173789), (173824, 177972), (177984, 178205), (178208, 183969), (183984, 191456), (194560, 195101), (196608, 201546),
-    )
-)
-_numericCharClass = _getRegexCharacterClassStringFromCodePointRanges(
-    (
-        (48, 57), (178, 179), (185, 185), (188, 190), (1632, 1641), (1776, 1785), (1984, 1993), (2406, 2415), (2534, 2543), (2548, 2553), (2662, 2671), (2790, 2799), (2918, 2927), (2930, 2935), (3046, 3058), (3174, 3183), (3192, 3198), (3302, 3311), (3416, 3422), (3430, 3448), (3558, 3567), (3664, 3673), (3792, 3801), (3872, 3891), (4160, 4169), (4240, 4249), (4969, 4988), (5870, 5872), (6112, 6121), (6128, 6137), (6160, 6169), (6470, 6479), (6608, 6618), (6784, 6793), (6800, 6809), (6992, 7001), (7088, 7097), (7232, 7241), (7248, 7257), (8304, 8304), (8308, 8313), (8320, 8329), (8528, 8578), (8581, 8585), (9312, 9371), (9450, 9471), (10102, 10131), (11517, 11517), (12295, 12295), (12321, 12329), (12344, 12346), (12690, 12693), (12832, 12841), (12872, 12879), (12881, 12895), (12928, 12937), (12977, 12991), (13317, 13317), (13443, 13443), (14378, 14378), (15181, 15181), (19968, 19968), (19971, 19971), (19975, 19975), (19977, 19977), (20061, 20061), (20108, 20108), (20116, 20116), (20118, 20118), (20159, 20160), (20191, 20191), (20200, 20200), (20237, 20237), (20336, 20336), (20740, 20740), (20806, 20806), (20841, 20841), (20843, 20843), (20845, 20845), (21313, 21313), (21315, 21317), (21324, 21324), (21441, 21444), (22235, 22235), (22769, 22769), (22777, 22777), (24186, 24186), (24318, 24319), (24332, 24334), (24336, 24336), (25342, 25342), (25420, 25420), (26578, 26578), (28422, 28422), (29590, 29590), (30334, 30334), (32902, 32902), (33836, 33836), (36014, 36014), (36019, 36019), (36144, 36144), (38433, 38433), (38470, 38470), (38476, 38476), (38520, 38520), (38646, 38646), (42528, 42537), (42726, 42735), (43056, 43061), (43216, 43225), (43264, 43273), (43472, 43481), (43504, 43513), (43600, 43609), (44016, 44025), (63851, 63851), (63859, 63859), (63864, 63864), (63922, 63922), (63953, 63953), (63955, 63955), (63997, 63997), (65296, 65305), (65799, 65843), (65856, 65912), (65930, 65931), (66273, 66299), (66336, 66339), (66369, 66369), (66378, 66378), (66513, 66517), (66720, 66729), (67672, 67679), (67705, 67711), (67751, 67759), (67835, 67839), (67862, 67867), (68028, 68029), (68032, 68047), (68050, 68095), (68160, 68168), (68221, 68222), (68253, 68255), (68331, 68335), (68440, 68447), (68472, 68479), (68521, 68527), (68858, 68863), (68912, 68921), (69216, 69246), (69405, 69414), (69457, 69460), (69573, 69579), (69714, 69743), (69872, 69881), (69942, 69951), (70096, 70105), (70113, 70132), (70384, 70393), (70736, 70745), (70864, 70873), (71248, 71257), (71360, 71369), (71472, 71483), (71904, 71922), (72016, 72025), (72784, 72812), (73040, 73049), (73120, 73129), (73664, 73684), (74752, 74862), (92768, 92777), (93008, 93017), (93019, 93025), (93824, 93846), (119520, 119539), (119648, 119672), (120782, 120831), (123200, 123209), (123632, 123641), (125127, 125135), (125264, 125273), (126065, 126123), (126125, 126127), (126129, 126132), (126209, 126253), (126255, 126269), (127232, 127244), (130032, 130041), (131073, 131073), (131172, 131172), (131298, 131298), (131361, 131361), (133418, 133418), (133507, 133507), (133516, 133516), (133532, 133532), (133866, 133866), (133885, 133885), (133913, 133913), (140176, 140176), (141720, 141720), (146203, 146203), (156269, 156269), (194704, 194704),
-    )
-)
+_LOWERCASE_CHAR_CLASS = _get_regex_character_class_string_from_code_point_ranges(
+    [
+        (97, 122), (170, 170), (181, 181), (186, 186), (223, 246), (248, 255), (257, 257), (259, 259), (261, 261), (263, 263), (265, 265), (267, 267), (269, 269), (271, 271), (273, 273), (275, 275), (277, 277), (279, 279), (281, 281), (283, 283), (285, 285), (287, 287), (289, 289), (291, 291), (293, 293), (295, 295), (297, 297), (299, 299), (301, 301), (303, 303), (305, 305), (307, 307), (309, 309), (311, 312), (314, 314), (316, 316), (318, 318), (320, 320), (322, 322), (324, 324), (326, 326), (328, 329), (331, 331), (333, 333), (335, 335), (337, 337), (339, 339), (341, 341), (343, 343), (345, 345), (347, 347), (349, 349), (351, 351), (353, 353), (355, 355), (357, 357), (359, 359), (361, 361), (363, 363), (365, 365), (367, 367), (369, 369), (371, 371), (373, 373), (375, 375), (378, 378), (380, 380), (382, 384), (387, 387), (389, 389), (392, 392), (396, 397), (402, 402), (405, 405), (409, 411), (414, 414), (417, 417), (419, 419), (421, 421), (424, 424), (426, 427), (429, 429), (432, 432), (436, 436), (438, 438), (441, 442), (445, 447), (454, 454), (457, 457), (460, 460), (462, 462), (464, 464), (466, 466), (468, 468), (470, 470), (472, 472), (474, 474), (476, 477), (479, 479), (481, 481), (483, 483), (485, 485), (487, 487), (489, 489), (491, 491), (493, 493), (495, 496), (499, 499), (501, 501), (505, 505), (507, 507), (509, 509), (511, 511), (513, 513), (515, 515), (517, 517), (519, 519), (521, 521), (523, 523), (525, 525), (527, 527), (529, 529), (531, 531), (533, 533), (535, 535), (537, 537), (539, 539), (541, 541), (543, 543), (545, 545), (547, 547), (549, 549), (551, 551), (553, 553), (555, 555), (557, 557), (559, 559), (561, 561), (563, 569), (572, 572), (575, 576), (578, 578), (583, 583), (585, 585), (587, 587), (589, 589), (591, 659), (661, 696), (704, 705), (736, 740), (837, 837), (881, 881), (883, 883), (887, 887), (890, 893), (912, 912), (940, 974), (976, 977), (981, 983), (985, 985), (987, 987), (989, 989), (991, 991), (993, 993), (995, 995), (997, 997), (999, 999), (1001, 1001), (1003, 1003), (1005, 1005), (1007, 1011), (1013, 1013), (1016, 1016), (1019, 1020), (1072, 1119), (1121, 1121), (1123, 1123), (1125, 1125), (1127, 1127), (1129, 1129), (1131, 1131), (1133, 1133), (1135, 1135), (1137, 1137), (1139, 1139), (1141, 1141), (1143, 1143), (1145, 1145), (1147, 1147), (1149, 1149), (1151, 1151), (1153, 1153), (1163, 1163), (1165, 1165), (1167, 1167), (1169, 1169), (1171, 1171), (1173, 1173), (1175, 1175), (1177, 1177), (1179, 1179), (1181, 1181), (1183, 1183), (1185, 1185), (1187, 1187), (1189, 1189), (1191, 1191), (1193, 1193), (1195, 1195), (1197, 1197), (1199, 1199), (1201, 1201), (1203, 1203), (1205, 1205), (1207, 1207), (1209, 1209), (1211, 1211), (1213, 1213), (1215, 1215), (1218, 1218), (1220, 1220), (1222, 1222), (1224, 1224), (1226, 1226), (1228, 1228), (1230, 1231), (1233, 1233), (1235, 1235), (1237, 1237), (1239, 1239), (1241, 1241), (1243, 1243), (1245, 1245), (1247, 1247), (1249, 1249), (1251, 1251), (1253, 1253), (1255, 1255), (1257, 1257), (1259, 1259), (1261, 1261), (1263, 1263), (1265, 1265), (1267, 1267), (1269, 1269), (1271, 1271), (1273, 1273), (1275, 1275), (1277, 1277), (1279, 1279), (1281, 1281), (1283, 1283), (1285, 1285), (1287, 1287), (1289, 1289), (1291, 1291), (1293, 1293), (1295, 1295), (1297, 1297), (1299, 1299), (1301, 1301), (1303, 1303), (1305, 1305), (1307, 1307), (1309, 1309), (1311, 1311), (1313, 1313), (1315, 1315), (1317, 1317), (1319, 1319), (1321, 1321), (1323, 1323), (1325, 1325), (1327, 1327), (1376, 1416), (4304, 4346), (4349, 4351), (5112, 5117), (7296, 7304), (7424, 7615), (7681, 7681), (7683, 7683), (7685, 7685), (7687, 7687), (7689, 7689), (7691, 7691), (7693, 7693), (7695, 7695), (7697, 7697), (7699, 7699), (7701, 7701), (7703, 7703), (7705, 7705), (7707, 7707), (7709, 7709), (7711, 7711), (7713, 7713), (7715, 7715), (7717, 7717), (7719, 7719), (7721, 7721), (7723, 7723), (7725, 7725), (7727, 7727), (7729, 7729), (7731, 7731), (7733, 7733), (7735, 7735), (7737, 7737), (7739, 7739), (7741, 7741), (7743, 7743), (7745, 7745), (7747, 7747), (7749, 7749), (7751, 7751), (7753, 7753), (7755, 7755), (7757, 7757), (7759, 7759), (7761, 7761), (7763, 7763), (7765, 7765), (7767, 7767), (7769, 7769), (7771, 7771), (7773, 7773), (7775, 7775), (7777, 7777), (7779, 7779), (7781, 7781), (7783, 7783), (7785, 7785), (7787, 7787), (7789, 7789), (7791, 7791), (7793, 7793), (7795, 7795), (7797, 7797), (7799, 7799), (7801, 7801), (7803, 7803), (7805, 7805), (7807, 7807), (7809, 7809), (7811, 7811), (7813, 7813), (7815, 7815), (7817, 7817), (7819, 7819), (7821, 7821), (7823, 7823), (7825, 7825), (7827, 7827), (7829, 7837), (7839, 7839), (7841, 7841), (7843, 7843), (7845, 7845), (7847, 7847), (7849, 7849), (7851, 7851), (7853, 7853), (7855, 7855), (7857, 7857), (7859, 7859), (7861, 7861), (7863, 7863), (7865, 7865), (7867, 7867), (7869, 7869), (7871, 7871), (7873, 7873), (7875, 7875), (7877, 7877), (7879, 7879), (7881, 7881), (7883, 7883), (7885, 7885), (7887, 7887), (7889, 7889), (7891, 7891), (7893, 7893), (7895, 7895), (7897, 7897), (7899, 7899), (7901, 7901), (7903, 7903), (7905, 7905), (7907, 7907), (7909, 7909), (7911, 7911), (7913, 7913), (7915, 7915), (7917, 7917), (7919, 7919), (7921, 7921), (7923, 7923), (7925, 7925), (7927, 7927), (7929, 7929), (7931, 7931), (7933, 7933), (7935, 7943), (7952, 7957), (7968, 7975), (7984, 7991), (8000, 8005), (8016, 8023), (8032, 8039), (8048, 8061), (8064, 8071), (8080, 8087), (8096, 8103), (8112, 8116), (8118, 8119), (8126, 8126), (8130, 8132), (8134, 8135), (8144, 8147), (8150, 8151), (8160, 8167), (8178, 8180), (8182, 8183), (8305, 8305), (8319, 8319), (8336, 8348), (8458, 8458), (8462, 8463), (8467, 8467), (8495, 8495), (8500, 8500), (8505, 8505), (8508, 8509), (8518, 8521), (8526, 8526), (8560, 8575), (8580, 8580), (9424, 9449), (11312, 11358), (11361, 11361), (11365, 11366), (11368, 11368), (11370, 11370), (11372, 11372), (11377, 11377), (11379, 11380), (11382, 11389), (11393, 11393), (11395, 11395), (11397, 11397), (11399, 11399), (11401, 11401), (11403, 11403), (11405, 11405), (11407, 11407), (11409, 11409), (11411, 11411), (11413, 11413), (11415, 11415), (11417, 11417), (11419, 11419), (11421, 11421), (11423, 11423), (11425, 11425), (11427, 11427), (11429, 11429), (11431, 11431), (11433, 11433), (11435, 11435), (11437, 11437), (11439, 11439), (11441, 11441), (11443, 11443), (11445, 11445), (11447, 11447), (11449, 11449), (11451, 11451), (11453, 11453), (11455, 11455), (11457, 11457), (11459, 11459), (11461, 11461), (11463, 11463), (11465, 11465), (11467, 11467), (11469, 11469), (11471, 11471), (11473, 11473), (11475, 11475), (11477, 11477), (11479, 11479), (11481, 11481), (11483, 11483), (11485, 11485), (11487, 11487), (11489, 11489), (11491, 11492), (11500, 11500), (11502, 11502), (11507, 11507), (11520, 11557), (11559, 11559), (11565, 11565), (42561, 42561), (42563, 42563), (42565, 42565), (42567, 42567), (42569, 42569), (42571, 42571), (42573, 42573), (42575, 42575), (42577, 42577), (42579, 42579), (42581, 42581), (42583, 42583), (42585, 42585), (42587, 42587), (42589, 42589), (42591, 42591), (42593, 42593), (42595, 42595), (42597, 42597), (42599, 42599), (42601, 42601), (42603, 42603), (42605, 42605), (42625, 42625), (42627, 42627), (42629, 42629), (42631, 42631), (42633, 42633), (42635, 42635), (42637, 42637), (42639, 42639), (42641, 42641), (42643, 42643), (42645, 42645), (42647, 42647), (42649, 42649), (42651, 42653), (42787, 42787), (42789, 42789), (42791, 42791), (42793, 42793), (42795, 42795), (42797, 42797), (42799, 42801), (42803, 42803), (42805, 42805), (42807, 42807), (42809, 42809), (42811, 42811), (42813, 42813), (42815, 42815), (42817, 42817), (42819, 42819), (42821, 42821), (42823, 42823), (42825, 42825), (42827, 42827), (42829, 42829), (42831, 42831), (42833, 42833), (42835, 42835), (42837, 42837), (42839, 42839), (42841, 42841), (42843, 42843), (42845, 42845), (42847, 42847), (42849, 42849), (42851, 42851), (42853, 42853), (42855, 42855), (42857, 42857), (42859, 42859), (42861, 42861), (42863, 42872), (42874, 42874), (42876, 42876), (42879, 42879), (42881, 42881), (42883, 42883), (42885, 42885), (42887, 42887), (42892, 42892), (42894, 42894), (42897, 42897), (42899, 42901), (42903, 42903), (42905, 42905), (42907, 42907), (42909, 42909), (42911, 42911), (42913, 42913), (42915, 42915), (42917, 42917), (42919, 42919), (42921, 42921), (42927, 42927), (42933, 42933), (42935, 42935), (42937, 42937), (42939, 42939), (42941, 42941), (42943, 42943), (42947, 42947), (42952, 42952), (42954, 42954), (42998, 42998), (43000, 43002), (43824, 43866), (43868, 43880), (43888, 43967), (64256, 64262), (64275, 64279), (65345, 65370), (66600, 66639), (66776, 66811), (68800, 68850), (71872, 71903), (93792, 93823), (119834, 119859), (119886, 119892), (119894, 119911), (119938, 119963), (119990, 119993), (119995, 119995), (119997, 120003), (120005, 120015), (120042, 120067), (120094, 120119), (120146, 120171), (120198, 120223), (120250, 120275), (120302, 120327), (120354, 120379), (120406, 120431), (120458, 120485), (120514, 120538), (120540, 120545), (120572, 120596), (120598, 120603), (120630, 120654), (120656, 120661), (120688, 120712), (120714, 120719), (120746, 120770), (120772, 120777), (120779, 120779), (125218, 125251),  # noqa: E501
+    ]
+)  # type: str
+_UPPERCASE_CHAR_CLASS = _get_regex_character_class_string_from_code_point_ranges(
+    [
+        (65, 90), (192, 214), (216, 222), (256, 256), (258, 258), (260, 260), (262, 262), (264, 264), (266, 266), (268, 268), (270, 270), (272, 272), (274, 274), (276, 276), (278, 278), (280, 280), (282, 282), (284, 284), (286, 286), (288, 288), (290, 290), (292, 292), (294, 294), (296, 296), (298, 298), (300, 300), (302, 302), (304, 304), (306, 306), (308, 308), (310, 310), (313, 313), (315, 315), (317, 317), (319, 319), (321, 321), (323, 323), (325, 325), (327, 327), (330, 330), (332, 332), (334, 334), (336, 336), (338, 338), (340, 340), (342, 342), (344, 344), (346, 346), (348, 348), (350, 350), (352, 352), (354, 354), (356, 356), (358, 358), (360, 360), (362, 362), (364, 364), (366, 366), (368, 368), (370, 370), (372, 372), (374, 374), (376, 377), (379, 379), (381, 381), (385, 386), (388, 388), (390, 391), (393, 395), (398, 401), (403, 404), (406, 408), (412, 413), (415, 416), (418, 418), (420, 420), (422, 423), (425, 425), (428, 428), (430, 431), (433, 435), (437, 437), (439, 440), (444, 444), (452, 452), (455, 455), (458, 458), (461, 461), (463, 463), (465, 465), (467, 467), (469, 469), (471, 471), (473, 473), (475, 475), (478, 478), (480, 480), (482, 482), (484, 484), (486, 486), (488, 488), (490, 490), (492, 492), (494, 494), (497, 497), (500, 500), (502, 504), (506, 506), (508, 508), (510, 510), (512, 512), (514, 514), (516, 516), (518, 518), (520, 520), (522, 522), (524, 524), (526, 526), (528, 528), (530, 530), (532, 532), (534, 534), (536, 536), (538, 538), (540, 540), (542, 542), (544, 544), (546, 546), (548, 548), (550, 550), (552, 552), (554, 554), (556, 556), (558, 558), (560, 560), (562, 562), (570, 571), (573, 574), (577, 577), (579, 582), (584, 584), (586, 586), (588, 588), (590, 590), (880, 880), (882, 882), (886, 886), (895, 895), (902, 902), (904, 906), (908, 908), (910, 911), (913, 929), (931, 939), (975, 975), (978, 980), (984, 984), (986, 986), (988, 988), (990, 990), (992, 992), (994, 994), (996, 996), (998, 998), (1000, 1000), (1002, 1002), (1004, 1004), (1006, 1006), (1012, 1012), (1015, 1015), (1017, 1018), (1021, 1071), (1120, 1120), (1122, 1122), (1124, 1124), (1126, 1126), (1128, 1128), (1130, 1130), (1132, 1132), (1134, 1134), (1136, 1136), (1138, 1138), (1140, 1140), (1142, 1142), (1144, 1144), (1146, 1146), (1148, 1148), (1150, 1150), (1152, 1152), (1162, 1162), (1164, 1164), (1166, 1166), (1168, 1168), (1170, 1170), (1172, 1172), (1174, 1174), (1176, 1176), (1178, 1178), (1180, 1180), (1182, 1182), (1184, 1184), (1186, 1186), (1188, 1188), (1190, 1190), (1192, 1192), (1194, 1194), (1196, 1196), (1198, 1198), (1200, 1200), (1202, 1202), (1204, 1204), (1206, 1206), (1208, 1208), (1210, 1210), (1212, 1212), (1214, 1214), (1216, 1217), (1219, 1219), (1221, 1221), (1223, 1223), (1225, 1225), (1227, 1227), (1229, 1229), (1232, 1232), (1234, 1234), (1236, 1236), (1238, 1238), (1240, 1240), (1242, 1242), (1244, 1244), (1246, 1246), (1248, 1248), (1250, 1250), (1252, 1252), (1254, 1254), (1256, 1256), (1258, 1258), (1260, 1260), (1262, 1262), (1264, 1264), (1266, 1266), (1268, 1268), (1270, 1270), (1272, 1272), (1274, 1274), (1276, 1276), (1278, 1278), (1280, 1280), (1282, 1282), (1284, 1284), (1286, 1286), (1288, 1288), (1290, 1290), (1292, 1292), (1294, 1294), (1296, 1296), (1298, 1298), (1300, 1300), (1302, 1302), (1304, 1304), (1306, 1306), (1308, 1308), (1310, 1310), (1312, 1312), (1314, 1314), (1316, 1316), (1318, 1318), (1320, 1320), (1322, 1322), (1324, 1324), (1326, 1326), (1329, 1366), (4256, 4293), (4295, 4295), (4301, 4301), (5024, 5109), (7312, 7354), (7357, 7359), (7680, 7680), (7682, 7682), (7684, 7684), (7686, 7686), (7688, 7688), (7690, 7690), (7692, 7692), (7694, 7694), (7696, 7696), (7698, 7698), (7700, 7700), (7702, 7702), (7704, 7704), (7706, 7706), (7708, 7708), (7710, 7710), (7712, 7712), (7714, 7714), (7716, 7716), (7718, 7718), (7720, 7720), (7722, 7722), (7724, 7724), (7726, 7726), (7728, 7728), (7730, 7730), (7732, 7732), (7734, 7734), (7736, 7736), (7738, 7738), (7740, 7740), (7742, 7742), (7744, 7744), (7746, 7746), (7748, 7748), (7750, 7750), (7752, 7752), (7754, 7754), (7756, 7756), (7758, 7758), (7760, 7760), (7762, 7762), (7764, 7764), (7766, 7766), (7768, 7768), (7770, 7770), (7772, 7772), (7774, 7774), (7776, 7776), (7778, 7778), (7780, 7780), (7782, 7782), (7784, 7784), (7786, 7786), (7788, 7788), (7790, 7790), (7792, 7792), (7794, 7794), (7796, 7796), (7798, 7798), (7800, 7800), (7802, 7802), (7804, 7804), (7806, 7806), (7808, 7808), (7810, 7810), (7812, 7812), (7814, 7814), (7816, 7816), (7818, 7818), (7820, 7820), (7822, 7822), (7824, 7824), (7826, 7826), (7828, 7828), (7838, 7838), (7840, 7840), (7842, 7842), (7844, 7844), (7846, 7846), (7848, 7848), (7850, 7850), (7852, 7852), (7854, 7854), (7856, 7856), (7858, 7858), (7860, 7860), (7862, 7862), (7864, 7864), (7866, 7866), (7868, 7868), (7870, 7870), (7872, 7872), (7874, 7874), (7876, 7876), (7878, 7878), (7880, 7880), (7882, 7882), (7884, 7884), (7886, 7886), (7888, 7888), (7890, 7890), (7892, 7892), (7894, 7894), (7896, 7896), (7898, 7898), (7900, 7900), (7902, 7902), (7904, 7904), (7906, 7906), (7908, 7908), (7910, 7910), (7912, 7912), (7914, 7914), (7916, 7916), (7918, 7918), (7920, 7920), (7922, 7922), (7924, 7924), (7926, 7926), (7928, 7928), (7930, 7930), (7932, 7932), (7934, 7934), (7944, 7951), (7960, 7965), (7976, 7983), (7992, 7999), (8008, 8013), (8025, 8025), (8027, 8027), (8029, 8029), (8031, 8031), (8040, 8047), (8120, 8123), (8136, 8139), (8152, 8155), (8168, 8172), (8184, 8187), (8450, 8450), (8455, 8455), (8459, 8461), (8464, 8466), (8469, 8469), (8473, 8477), (8484, 8484), (8486, 8486), (8488, 8488), (8490, 8493), (8496, 8499), (8510, 8511), (8517, 8517), (8544, 8559), (8579, 8579), (9398, 9423), (11264, 11310), (11360, 11360), (11362, 11364), (11367, 11367), (11369, 11369), (11371, 11371), (11373, 11376), (11378, 11378), (11381, 11381), (11390, 11392), (11394, 11394), (11396, 11396), (11398, 11398), (11400, 11400), (11402, 11402), (11404, 11404), (11406, 11406), (11408, 11408), (11410, 11410), (11412, 11412), (11414, 11414), (11416, 11416), (11418, 11418), (11420, 11420), (11422, 11422), (11424, 11424), (11426, 11426), (11428, 11428), (11430, 11430), (11432, 11432), (11434, 11434), (11436, 11436), (11438, 11438), (11440, 11440), (11442, 11442), (11444, 11444), (11446, 11446), (11448, 11448), (11450, 11450), (11452, 11452), (11454, 11454), (11456, 11456), (11458, 11458), (11460, 11460), (11462, 11462), (11464, 11464), (11466, 11466), (11468, 11468), (11470, 11470), (11472, 11472), (11474, 11474), (11476, 11476), (11478, 11478), (11480, 11480), (11482, 11482), (11484, 11484), (11486, 11486), (11488, 11488), (11490, 11490), (11499, 11499), (11501, 11501), (11506, 11506), (42560, 42560), (42562, 42562), (42564, 42564), (42566, 42566), (42568, 42568), (42570, 42570), (42572, 42572), (42574, 42574), (42576, 42576), (42578, 42578), (42580, 42580), (42582, 42582), (42584, 42584), (42586, 42586), (42588, 42588), (42590, 42590), (42592, 42592), (42594, 42594), (42596, 42596), (42598, 42598), (42600, 42600), (42602, 42602), (42604, 42604), (42624, 42624), (42626, 42626), (42628, 42628), (42630, 42630), (42632, 42632), (42634, 42634), (42636, 42636), (42638, 42638), (42640, 42640), (42642, 42642), (42644, 42644), (42646, 42646), (42648, 42648), (42650, 42650), (42786, 42786), (42788, 42788), (42790, 42790), (42792, 42792), (42794, 42794), (42796, 42796), (42798, 42798), (42802, 42802), (42804, 42804), (42806, 42806), (42808, 42808), (42810, 42810), (42812, 42812), (42814, 42814), (42816, 42816), (42818, 42818), (42820, 42820), (42822, 42822), (42824, 42824), (42826, 42826), (42828, 42828), (42830, 42830), (42832, 42832), (42834, 42834), (42836, 42836), (42838, 42838), (42840, 42840), (42842, 42842), (42844, 42844), (42846, 42846), (42848, 42848), (42850, 42850), (42852, 42852), (42854, 42854), (42856, 42856), (42858, 42858), (42860, 42860), (42862, 42862), (42873, 42873), (42875, 42875), (42877, 42878), (42880, 42880), (42882, 42882), (42884, 42884), (42886, 42886), (42891, 42891), (42893, 42893), (42896, 42896), (42898, 42898), (42902, 42902), (42904, 42904), (42906, 42906), (42908, 42908), (42910, 42910), (42912, 42912), (42914, 42914), (42916, 42916), (42918, 42918), (42920, 42920), (42922, 42926), (42928, 42932), (42934, 42934), (42936, 42936), (42938, 42938), (42940, 42940), (42942, 42942), (42946, 42946), (42948, 42951), (42953, 42953), (42997, 42997), (65313, 65338), (66560, 66599), (66736, 66771), (68736, 68786), (71840, 71871), (93760, 93791), (119808, 119833), (119860, 119885), (119912, 119937), (119964, 119964), (119966, 119967), (119970, 119970), (119973, 119974), (119977, 119980), (119982, 119989), (120016, 120041), (120068, 120069), (120071, 120074), (120077, 120084), (120086, 120092), (120120, 120121), (120123, 120126), (120128, 120132), (120134, 120134), (120138, 120144), (120172, 120197), (120224, 120249), (120276, 120301), (120328, 120353), (120380, 120405), (120432, 120457), (120488, 120512), (120546, 120570), (120604, 120628), (120662, 120686), (120720, 120744), (120778, 120778), (125184, 125217), (127280, 127305), (127312, 127337), (127344, 127369),  # noqa: E501
+    ]
+)  # type: str
+_LETTER_CHAR_CLASS = _get_regex_character_class_string_from_code_point_ranges(
+    [
+        (65, 90), (97, 122), (170, 170), (181, 181), (186, 186), (192, 214), (216, 246), (248, 705), (710, 721), (736, 740), (748, 748), (750, 750), (880, 884), (886, 887), (890, 893), (895, 895), (902, 902), (904, 906), (908, 908), (910, 929), (931, 1013), (1015, 1153), (1162, 1327), (1329, 1366), (1369, 1369), (1376, 1416), (1488, 1514), (1519, 1522), (1568, 1610), (1646, 1647), (1649, 1747), (1749, 1749), (1765, 1766), (1774, 1775), (1786, 1788), (1791, 1791), (1808, 1808), (1810, 1839), (1869, 1957), (1969, 1969), (1994, 2026), (2036, 2037), (2042, 2042), (2048, 2069), (2074, 2074), (2084, 2084), (2088, 2088), (2112, 2136), (2144, 2154), (2208, 2228), (2230, 2247), (2308, 2361), (2365, 2365), (2384, 2384), (2392, 2401), (2417, 2432), (2437, 2444), (2447, 2448), (2451, 2472), (2474, 2480), (2482, 2482), (2486, 2489), (2493, 2493), (2510, 2510), (2524, 2525), (2527, 2529), (2544, 2545), (2556, 2556), (2565, 2570), (2575, 2576), (2579, 2600), (2602, 2608), (2610, 2611), (2613, 2614), (2616, 2617), (2649, 2652), (2654, 2654), (2674, 2676), (2693, 2701), (2703, 2705), (2707, 2728), (2730, 2736), (2738, 2739), (2741, 2745), (2749, 2749), (2768, 2768), (2784, 2785), (2809, 2809), (2821, 2828), (2831, 2832), (2835, 2856), (2858, 2864), (2866, 2867), (2869, 2873), (2877, 2877), (2908, 2909), (2911, 2913), (2929, 2929), (2947, 2947), (2949, 2954), (2958, 2960), (2962, 2965), (2969, 2970), (2972, 2972), (2974, 2975), (2979, 2980), (2984, 2986), (2990, 3001), (3024, 3024), (3077, 3084), (3086, 3088), (3090, 3112), (3114, 3129), (3133, 3133), (3160, 3162), (3168, 3169), (3200, 3200), (3205, 3212), (3214, 3216), (3218, 3240), (3242, 3251), (3253, 3257), (3261, 3261), (3294, 3294), (3296, 3297), (3313, 3314), (3332, 3340), (3342, 3344), (3346, 3386), (3389, 3389), (3406, 3406), (3412, 3414), (3423, 3425), (3450, 3455), (3461, 3478), (3482, 3505), (3507, 3515), (3517, 3517), (3520, 3526), (3585, 3632), (3634, 3635), (3648, 3654), (3713, 3714), (3716, 3716), (3718, 3722), (3724, 3747), (3749, 3749), (3751, 3760), (3762, 3763), (3773, 3773), (3776, 3780), (3782, 3782), (3804, 3807), (3840, 3840), (3904, 3911), (3913, 3948), (3976, 3980), (4096, 4138), (4159, 4159), (4176, 4181), (4186, 4189), (4193, 4193), (4197, 4198), (4206, 4208), (4213, 4225), (4238, 4238), (4256, 4293), (4295, 4295), (4301, 4301), (4304, 4346), (4348, 4680), (4682, 4685), (4688, 4694), (4696, 4696), (4698, 4701), (4704, 4744), (4746, 4749), (4752, 4784), (4786, 4789), (4792, 4798), (4800, 4800), (4802, 4805), (4808, 4822), (4824, 4880), (4882, 4885), (4888, 4954), (4992, 5007), (5024, 5109), (5112, 5117), (5121, 5740), (5743, 5759), (5761, 5786), (5792, 5866), (5873, 5880), (5888, 5900), (5902, 5905), (5920, 5937), (5952, 5969), (5984, 5996), (5998, 6000), (6016, 6067), (6103, 6103), (6108, 6108), (6176, 6264), (6272, 6276), (6279, 6312), (6314, 6314), (6320, 6389), (6400, 6430), (6480, 6509), (6512, 6516), (6528, 6571), (6576, 6601), (6656, 6678), (6688, 6740), (6823, 6823), (6917, 6963), (6981, 6987), (7043, 7072), (7086, 7087), (7098, 7141), (7168, 7203), (7245, 7247), (7258, 7293), (7296, 7304), (7312, 7354), (7357, 7359), (7401, 7404), (7406, 7411), (7413, 7414), (7418, 7418), (7424, 7615), (7680, 7957), (7960, 7965), (7968, 8005), (8008, 8013), (8016, 8023), (8025, 8025), (8027, 8027), (8029, 8029), (8031, 8061), (8064, 8116), (8118, 8124), (8126, 8126), (8130, 8132), (8134, 8140), (8144, 8147), (8150, 8155), (8160, 8172), (8178, 8180), (8182, 8188), (8305, 8305), (8319, 8319), (8336, 8348), (8450, 8450), (8455, 8455), (8458, 8467), (8469, 8469), (8473, 8477), (8484, 8484), (8486, 8486), (8488, 8488), (8490, 8493), (8495, 8505), (8508, 8511), (8517, 8521), (8526, 8526), (8579, 8580), (11264, 11310), (11312, 11358), (11360, 11492), (11499, 11502), (11506, 11507), (11520, 11557), (11559, 11559), (11565, 11565), (11568, 11623), (11631, 11631), (11648, 11670), (11680, 11686), (11688, 11694), (11696, 11702), (11704, 11710), (11712, 11718), (11720, 11726), (11728, 11734), (11736, 11742), (11823, 11823), (12293, 12294), (12337, 12341), (12347, 12348), (12353, 12438), (12445, 12447), (12449, 12538), (12540, 12543), (12549, 12591), (12593, 12686), (12704, 12735), (12784, 12799), (13312, 19903), (19968, 40956), (40960, 42124), (42192, 42237), (42240, 42508), (42512, 42527), (42538, 42539), (42560, 42606), (42623, 42653), (42656, 42725), (42775, 42783), (42786, 42888), (42891, 42943), (42946, 42954), (42997, 43009), (43011, 43013), (43015, 43018), (43020, 43042), (43072, 43123), (43138, 43187), (43250, 43255), (43259, 43259), (43261, 43262), (43274, 43301), (43312, 43334), (43360, 43388), (43396, 43442), (43471, 43471), (43488, 43492), (43494, 43503), (43514, 43518), (43520, 43560), (43584, 43586), (43588, 43595), (43616, 43638), (43642, 43642), (43646, 43695), (43697, 43697), (43701, 43702), (43705, 43709), (43712, 43712), (43714, 43714), (43739, 43741), (43744, 43754), (43762, 43764), (43777, 43782), (43785, 43790), (43793, 43798), (43808, 43814), (43816, 43822), (43824, 43866), (43868, 43881), (43888, 44002), (44032, 55203), (55216, 55238), (55243, 55291), (63744, 64109), (64112, 64217), (64256, 64262), (64275, 64279), (64285, 64285), (64287, 64296), (64298, 64310), (64312, 64316), (64318, 64318), (64320, 64321), (64323, 64324), (64326, 64433), (64467, 64829), (64848, 64911), (64914, 64967), (65008, 65019), (65136, 65140), (65142, 65276), (65313, 65338), (65345, 65370), (65382, 65470), (65474, 65479), (65482, 65487), (65490, 65495), (65498, 65500), (65536, 65547), (65549, 65574), (65576, 65594), (65596, 65597), (65599, 65613), (65616, 65629), (65664, 65786), (66176, 66204), (66208, 66256), (66304, 66335), (66349, 66368), (66370, 66377), (66384, 66421), (66432, 66461), (66464, 66499), (66504, 66511), (66560, 66717), (66736, 66771), (66776, 66811), (66816, 66855), (66864, 66915), (67072, 67382), (67392, 67413), (67424, 67431), (67584, 67589), (67592, 67592), (67594, 67637), (67639, 67640), (67644, 67644), (67647, 67669), (67680, 67702), (67712, 67742), (67808, 67826), (67828, 67829), (67840, 67861), (67872, 67897), (67968, 68023), (68030, 68031), (68096, 68096), (68112, 68115), (68117, 68119), (68121, 68149), (68192, 68220), (68224, 68252), (68288, 68295), (68297, 68324), (68352, 68405), (68416, 68437), (68448, 68466), (68480, 68497), (68608, 68680), (68736, 68786), (68800, 68850), (68864, 68899), (69248, 69289), (69296, 69297), (69376, 69404), (69415, 69415), (69424, 69445), (69552, 69572), (69600, 69622), (69635, 69687), (69763, 69807), (69840, 69864), (69891, 69926), (69956, 69956), (69959, 69959), (69968, 70002), (70006, 70006), (70019, 70066), (70081, 70084), (70106, 70106), (70108, 70108), (70144, 70161), (70163, 70187), (70272, 70278), (70280, 70280), (70282, 70285), (70287, 70301), (70303, 70312), (70320, 70366), (70405, 70412), (70415, 70416), (70419, 70440), (70442, 70448), (70450, 70451), (70453, 70457), (70461, 70461), (70480, 70480), (70493, 70497), (70656, 70708), (70727, 70730), (70751, 70753), (70784, 70831), (70852, 70853), (70855, 70855), (71040, 71086), (71128, 71131), (71168, 71215), (71236, 71236), (71296, 71338), (71352, 71352), (71424, 71450), (71680, 71723), (71840, 71903), (71935, 71942), (71945, 71945), (71948, 71955), (71957, 71958), (71960, 71983), (71999, 71999), (72001, 72001), (72096, 72103), (72106, 72144), (72161, 72161), (72163, 72163), (72192, 72192), (72203, 72242), (72250, 72250), (72272, 72272), (72284, 72329), (72349, 72349), (72384, 72440), (72704, 72712), (72714, 72750), (72768, 72768), (72818, 72847), (72960, 72966), (72968, 72969), (72971, 73008), (73030, 73030), (73056, 73061), (73063, 73064), (73066, 73097), (73112, 73112), (73440, 73458), (73648, 73648), (73728, 74649), (74880, 75075), (77824, 78894), (82944, 83526), (92160, 92728), (92736, 92766), (92880, 92909), (92928, 92975), (92992, 92995), (93027, 93047), (93053, 93071), (93760, 93823), (93952, 94026), (94032, 94032), (94099, 94111), (94176, 94177), (94179, 94179), (94208, 100343), (100352, 101589), (101632, 101640), (110592, 110878), (110928, 110930), (110948, 110951), (110960, 111355), (113664, 113770), (113776, 113788), (113792, 113800), (113808, 113817), (119808, 119892), (119894, 119964), (119966, 119967), (119970, 119970), (119973, 119974), (119977, 119980), (119982, 119993), (119995, 119995), (119997, 120003), (120005, 120069), (120071, 120074), (120077, 120084), (120086, 120092), (120094, 120121), (120123, 120126), (120128, 120132), (120134, 120134), (120138, 120144), (120146, 120485), (120488, 120512), (120514, 120538), (120540, 120570), (120572, 120596), (120598, 120628), (120630, 120654), (120656, 120686), (120688, 120712), (120714, 120744), (120746, 120770), (120772, 120779), (123136, 123180), (123191, 123197), (123214, 123214), (123584, 123627), (124928, 125124), (125184, 125251), (125259, 125259), (126464, 126467), (126469, 126495), (126497, 126498), (126500, 126500), (126503, 126503), (126505, 126514), (126516, 126519), (126521, 126521), (126523, 126523), (126530, 126530), (126535, 126535), (126537, 126537), (126539, 126539), (126541, 126543), (126545, 126546), (126548, 126548), (126551, 126551), (126553, 126553), (126555, 126555), (126557, 126557), (126559, 126559), (126561, 126562), (126564, 126564), (126567, 126570), (126572, 126578), (126580, 126583), (126585, 126588), (126590, 126590), (126592, 126601), (126603, 126619), (126625, 126627), (126629, 126633), (126635, 126651), (131072, 173789), (173824, 177972), (177984, 178205), (178208, 183969), (183984, 191456), (194560, 195101), (196608, 201546),  # noqa: E501
+    ]
+)  # type: str
+_NUMERIC_CHAR_CLASS = _get_regex_character_class_string_from_code_point_ranges(
+    [
+        (48, 57), (178, 179), (185, 185), (188, 190), (1632, 1641), (1776, 1785), (1984, 1993), (2406, 2415), (2534, 2543), (2548, 2553), (2662, 2671), (2790, 2799), (2918, 2927), (2930, 2935), (3046, 3058), (3174, 3183), (3192, 3198), (3302, 3311), (3416, 3422), (3430, 3448), (3558, 3567), (3664, 3673), (3792, 3801), (3872, 3891), (4160, 4169), (4240, 4249), (4969, 4988), (5870, 5872), (6112, 6121), (6128, 6137), (6160, 6169), (6470, 6479), (6608, 6618), (6784, 6793), (6800, 6809), (6992, 7001), (7088, 7097), (7232, 7241), (7248, 7257), (8304, 8304), (8308, 8313), (8320, 8329), (8528, 8578), (8581, 8585), (9312, 9371), (9450, 9471), (10102, 10131), (11517, 11517), (12295, 12295), (12321, 12329), (12344, 12346), (12690, 12693), (12832, 12841), (12872, 12879), (12881, 12895), (12928, 12937), (12977, 12991), (13317, 13317), (13443, 13443), (14378, 14378), (15181, 15181), (19968, 19968), (19971, 19971), (19975, 19975), (19977, 19977), (20061, 20061), (20108, 20108), (20116, 20116), (20118, 20118), (20159, 20160), (20191, 20191), (20200, 20200), (20237, 20237), (20336, 20336), (20740, 20740), (20806, 20806), (20841, 20841), (20843, 20843), (20845, 20845), (21313, 21313), (21315, 21317), (21324, 21324), (21441, 21444), (22235, 22235), (22769, 22769), (22777, 22777), (24186, 24186), (24318, 24319), (24332, 24334), (24336, 24336), (25342, 25342), (25420, 25420), (26578, 26578), (28422, 28422), (29590, 29590), (30334, 30334), (32902, 32902), (33836, 33836), (36014, 36014), (36019, 36019), (36144, 36144), (38433, 38433), (38470, 38470), (38476, 38476), (38520, 38520), (38646, 38646), (42528, 42537), (42726, 42735), (43056, 43061), (43216, 43225), (43264, 43273), (43472, 43481), (43504, 43513), (43600, 43609), (44016, 44025), (63851, 63851), (63859, 63859), (63864, 63864), (63922, 63922), (63953, 63953), (63955, 63955), (63997, 63997), (65296, 65305), (65799, 65843), (65856, 65912), (65930, 65931), (66273, 66299), (66336, 66339), (66369, 66369), (66378, 66378), (66513, 66517), (66720, 66729), (67672, 67679), (67705, 67711), (67751, 67759), (67835, 67839), (67862, 67867), (68028, 68029), (68032, 68047), (68050, 68095), (68160, 68168), (68221, 68222), (68253, 68255), (68331, 68335), (68440, 68447), (68472, 68479), (68521, 68527), (68858, 68863), (68912, 68921), (69216, 69246), (69405, 69414), (69457, 69460), (69573, 69579), (69714, 69743), (69872, 69881), (69942, 69951), (70096, 70105), (70113, 70132), (70384, 70393), (70736, 70745), (70864, 70873), (71248, 71257), (71360, 71369), (71472, 71483), (71904, 71922), (72016, 72025), (72784, 72812), (73040, 73049), (73120, 73129), (73664, 73684), (74752, 74862), (92768, 92777), (93008, 93017), (93019, 93025), (93824, 93846), (119520, 119539), (119648, 119672), (120782, 120831), (123200, 123209), (123632, 123641), (125127, 125135), (125264, 125273), (126065, 126123), (126125, 126127), (126129, 126132), (126209, 126253), (126255, 126269), (127232, 127244), (130032, 130041), (131073, 131073), (131172, 131172), (131298, 131298), (131361, 131361), (133418, 133418), (133507, 133507), (133516, 133516), (133532, 133532), (133866, 133866), (133885, 133885), (133913, 133913), (140176, 140176), (141720, 141720), (146203, 146203), (156269, 156269), (194704, 194704),  # noqa: E501
+    ]
+)  # type: str
 # fmt: on
 
 # These ranges include more than just A-Za-z, but all Unicode characters
 # that islower(), isupper(), and isalpha() identify as lowercase, uppercase,
 # and alphabetical letter characters.
-LETTER = '[' + _letterCharClass + ']'
-NONLETTER = '[^' + _letterCharClass + ']'
-UPPERCASE = '[' + _uppercaseCharClass + ']'
-NONUPPERCASE = '[^' + _uppercaseCharClass + ']'
-LOWERCASE = '[' + _lowercaseCharClass + ']'
-NONLOWERCASE = '[^' + _lowercaseCharClass + ']'
-ALPHANUMERIC = '[' + _numericCharClass + _letterCharClass + ']'
-NONALPHANUMERIC = '[^' + _numericCharClass + _letterCharClass + ']'
-NUMERIC = '[' + _numericCharClass + ']'
-NONNUMERIC = '[^' + _numericCharClass + ']'
-
-del _lowercaseCharClass
-del _uppercaseCharClass
-del _letterCharClass
-del _numericCharClass
+LETTER = '[' + _LETTER_CHAR_CLASS + ']'  # type: str
+NONLETTER = '[^' + _LETTER_CHAR_CLASS + ']'  # type: str
+UPPERCASE = '[' + _UPPERCASE_CHAR_CLASS + ']'  # type: str
+NONUPPERCASE = '[^' + _UPPERCASE_CHAR_CLASS + ']'  # type: str
+LOWERCASE = '[' + _LOWERCASE_CHAR_CLASS + ']'  # type: str
+NONLOWERCASE = '[^' + _LOWERCASE_CHAR_CLASS + ']'  # type: str
+ALPHANUMERIC = '[' + _NUMERIC_CHAR_CLASS + _LETTER_CHAR_CLASS + ']'  # type: str
+NONALPHANUMERIC = '[^' + _NUMERIC_CHAR_CLASS + _LETTER_CHAR_CLASS + ']'  # type: str
+NUMERIC = '[' + _NUMERIC_CHAR_CLASS + ']'  # type: str
+NONNUMERIC = '[^' + _NUMERIC_CHAR_CLASS + ']'  # type: str
+
+del _LOWERCASE_CHAR_CLASS
+del _UPPERCASE_CHAR_CLASS
+del _LETTER_CHAR_CLASS
+del _NUMERIC_CHAR_CLASS
 
 """
 # On second thought, I don't think these constants add much. It's easier
 # to just use the regex string themselves.
 ASCII_LETTER = '[A-Za-z]'
 ASCII_NONLETTER = '[^A-Za-z]'
 ASCII_UPPERCASE = '[A-Z]'
@@ -160,58 +110,154 @@
 ASCII_NONLOWERCASE = '[^a-z]'
 ASCII_ALPHANUMERIC = '[A-Za-z0-9]'
 ASCII_NONALPHANUMERIC = '[^A-Za-z0-9]'
 ASCII_NUMERIC = '[0-9]'
 ASCII_NONNUMERIC = '[^0-9]'
 """
 
-HEXADECIMAL = '[0-9A-Fa-f]'
-NONHEXADECIMAL = '[^0-9A-Fa-f]'
+HEXADECIMAL = '[0-9A-Fa-f]'  # type: str
+NONHEXADECIMAL = '[^0-9A-Fa-f]'  # type: str
 
 # Built-in Humre Patterns:
 # TODO - I'm still not sure about these names:
-ANYTHING = '.*?'
-EVERYTHING = '.*'
-# GREEDY_SOMETHING = '.+' # TODO: Maybe it's better to not even have this, rather than have it with an awkward name.
-SOMETHING = '.+?'
-ANYCHAR = '.'
+ANYTHING = '.*?'  # type: str
+EVERYTHING = '.*'  # type: str
+# TODO: Maybe it's better to not even have this, rather than have it with an awkward name:
+# GREEDY_SOMETHING = '.+'  # type: str
+SOMETHING = '.+?'  # type: str
+ANYCHAR = '.'  # type: str
 
 
 # labels for escaped regex metacharacters: . ^ $ * + ? { } [ ] \ | ( )
 # This full list copied from https://docs.python.org/3/howto/regex.html
-PERIOD = r'\.'
-CARET = r'\^'
-DOLLAR = r'\$'
-ASTERISK = r'\*'
-PLUS = r'\+'
-MINUS = r'\-'  # NOTE - Not strictly needed, but here since PLUS is.
-QUESTION_MARK = r'\?'
-OPEN_BRACE = r'\{'
-CLOSE_BRACE = r'\}'
-OPEN_BRACKET = r'\['
-CLOSE_BRACKET = r'\]'
-BACKSLASH = r'\\'
-PIPE = r'\|'
-OPEN_PAREN = OPEN_PARENTHESIS = r'\('
-CLOSE_PAREN = CLOSE_PARENTHESIS = r'\)'
-
-NEWLINE = r'\n'  # TODO - double check this: do I want r'\n' or '\n' here?
-TAB = r'\t'
-QUOTE = r"\'"
-DOUBLE_QUOTE = r'\"'
-
-BACK_1 = r'\1'
-BACK_2 = r'\2'
-BACK_3 = r'\3'
-BACK_4 = r'\4'
-BACK_5 = r'\5'
-BACK_6 = r'\6'
-BACK_7 = r'\7'
-BACK_8 = r'\8'
-BACK_9 = r'\9'
+# Note: Real list according to re.escape() is # $ & ( ) * + - . ? [ \ ] ^ { | } ~
+AMPERSAND = r'\&'  # type: str
+HASH_TAG = r'\#'  # type: str
+PERIOD = r'\.'  # type: str
+CARET = r'\^'  # type: str
+DOLLAR = r'\$'  # type: str
+ASTERISK = r'\*'  # type: str
+PLUS = r'\+'  # type: str
+MINUS = r'\-'  # type: str  # NOTE - Not strictly needed, but here since PLUS is.
+QUESTION_MARK = r'\?'  # type: str
+OPEN_BRACE = r'\{'  # type: str
+CLOSE_BRACE = r'\}'  # type: str
+OPEN_BRACKET = r'\['  # type: str
+CLOSE_BRACKET = r'\]'  # type: str
+BACKSLASH = r'\\'  # type: str
+PIPE = r'\|'  # type: str
+OPEN_PAREN = OPEN_PARENTHESIS = r'\('  # type: str
+CLOSE_PAREN = CLOSE_PARENTHESIS = r'\)'  # type: str
+TILDE = r'\~'  # type: str
+
+NEWLINE = r'\n'  # type: str  # TODO - double check this: do I want r'\n' or '\n' here?
+TAB = r'\t'  # type: str
+QUOTE = r"\'"  # type: str
+DOUBLE_QUOTE = r'\"'  # type: str
+
+BACK_1 = r'\1'  # type: str
+BACK_2 = r'\2'  # type: str
+BACK_3 = r'\3'  # type: str
+BACK_4 = r'\4'  # type: str
+BACK_5 = r'\5'  # type: str
+BACK_6 = r'\6'  # type: str
+BACK_7 = r'\7'  # type: str
+BACK_8 = r'\8'  # type: str
+BACK_9 = r'\9'  # type: str
+BACK_10 = r'\10'  # type: str
+BACK_11 = r'\11'  # type: str
+BACK_12 = r'\12'  # type: str
+BACK_13 = r'\13'  # type: str
+BACK_14 = r'\14'  # type: str
+BACK_15 = r'\15'  # type: str
+BACK_16 = r'\16'  # type: str
+BACK_17 = r'\17'  # type: str
+BACK_18 = r'\18'  # type: str
+BACK_19 = r'\19'  # type: str
+BACK_20 = r'\20'  # type: str
+BACK_21 = r'\21'  # type: str
+BACK_22 = r'\22'  # type: str
+BACK_23 = r'\23'  # type: str
+BACK_24 = r'\24'  # type: str
+BACK_25 = r'\25'  # type: str
+BACK_26 = r'\26'  # type: str
+BACK_27 = r'\27'  # type: str
+BACK_28 = r'\28'  # type: str
+BACK_29 = r'\29'  # type: str
+BACK_30 = r'\30'  # type: str
+BACK_31 = r'\31'  # type: str
+BACK_32 = r'\32'  # type: str
+BACK_33 = r'\33'  # type: str
+BACK_34 = r'\34'  # type: str
+BACK_35 = r'\35'  # type: str
+BACK_36 = r'\36'  # type: str
+BACK_37 = r'\37'  # type: str
+BACK_38 = r'\38'  # type: str
+BACK_39 = r'\39'  # type: str
+BACK_40 = r'\40'  # type: str
+BACK_41 = r'\41'  # type: str
+BACK_42 = r'\42'  # type: str
+BACK_43 = r'\43'  # type: str
+BACK_44 = r'\44'  # type: str
+BACK_45 = r'\45'  # type: str
+BACK_46 = r'\46'  # type: str
+BACK_47 = r'\47'  # type: str
+BACK_48 = r'\48'  # type: str
+BACK_49 = r'\49'  # type: str
+BACK_50 = r'\50'  # type: str
+BACK_51 = r'\51'  # type: str
+BACK_52 = r'\52'  # type: str
+BACK_53 = r'\53'  # type: str
+BACK_54 = r'\54'  # type: str
+BACK_55 = r'\55'  # type: str
+BACK_56 = r'\56'  # type: str
+BACK_57 = r'\57'  # type: str
+BACK_58 = r'\58'  # type: str
+BACK_59 = r'\59'  # type: str
+BACK_60 = r'\60'  # type: str
+BACK_61 = r'\61'  # type: str
+BACK_62 = r'\62'  # type: str
+BACK_63 = r'\63'  # type: str
+BACK_64 = r'\64'  # type: str
+BACK_65 = r'\65'  # type: str
+BACK_66 = r'\66'  # type: str
+BACK_67 = r'\67'  # type: str
+BACK_68 = r'\68'  # type: str
+BACK_69 = r'\69'  # type: str
+BACK_70 = r'\70'  # type: str
+BACK_71 = r'\71'  # type: str
+BACK_72 = r'\72'  # type: str
+BACK_73 = r'\73'  # type: str
+BACK_74 = r'\74'  # type: str
+BACK_75 = r'\75'  # type: str
+BACK_76 = r'\76'  # type: str
+BACK_77 = r'\77'  # type: str
+BACK_78 = r'\78'  # type: str
+BACK_79 = r'\79'  # type: str
+BACK_80 = r'\80'  # type: str
+BACK_81 = r'\81'  # type: str
+BACK_82 = r'\82'  # type: str
+BACK_83 = r'\83'  # type: str
+BACK_84 = r'\84'  # type: str
+BACK_85 = r'\85'  # type: str
+BACK_86 = r'\86'  # type: str
+BACK_87 = r'\87'  # type: str
+BACK_88 = r'\88'  # type: str
+BACK_89 = r'\89'  # type: str
+BACK_90 = r'\90'  # type: str
+BACK_91 = r'\91'  # type: str
+BACK_92 = r'\92'  # type: str
+BACK_93 = r'\93'  # type: str
+BACK_94 = r'\94'  # type: str
+BACK_95 = r'\95'  # type: str
+BACK_96 = r'\96'  # type: str
+BACK_97 = r'\97'  # type: str
+BACK_98 = r'\98'  # type: str
+BACK_99 = r'\99'  # type: str
+
 
 
 def back_reference(group_number):  # type: (int) -> str
     r"""Returns a string in the regex syntax for a back reference, such as
     \1, \2, etc.
 
     >>> from humre import *
@@ -248,59 +294,14 @@
     >>> import re
     >>> re.escape('!#$%&') == esc('!#$%&')
     True
     """
     return re.escape(''.join(regex_strs))
 
 
-def compile(
-    *regex_strs,
-    A=False,
-    ASCII=False,
-    DEBUG=False,
-    I=False,
-    IGNORECASE=False,
-    L=False,
-    LOCALE=False,
-    M=False,
-    MULTILINE=False,
-    S=False,
-    DOTALL=False,
-    X=False,
-    VERBOSE=False
-):  # TODO fix type hint
-    """A wrapper for re.compile(). This passes the strings in regex_strs
-    as a single concatenated string to re.compile(). All other arguments to
-    re.compile() must be passed to the flags keyword argument.
-
-    >>> from humre import *
-    >>> patternObj = compile('[a-z]+', IGNORECASE=True)
-    >>> patternObj.search('Hello')
-    <re.Match object; span=(0, 5), match='Hello'>
-    """
-    # Create the bitfield flags for re.compile():
-    flags = 0
-    if A or ASCII:
-        flags |= re.ASCII
-    if DEBUG:
-        flags |= re.DEBUG
-    if I or IGNORECASE:
-        flags |= re.IGNORECASE
-    if L or LOCALE:
-        flags |= re.LOCALE
-    if M or MULTILINE:
-        flags |= re.MULTILINE
-    if S or DOTALL:
-        flags |= re.DOTALL
-    if X or VERBOSE:
-        flags |= re.VERBOSE
-
-    return re.compile(''.join(regex_strs), flags=flags)
-
-
 def group(*regex_strs):  # type: (str) -> str
     """Returns a string in the regex syntax for a regex group surrounded by
     parentheses of the regex strings in regex_strs.
 
     >>> from humre import *
     >>> group('cat')
     '(cat)'
@@ -321,17 +322,18 @@
 
     In the following example, 'kitty' is matched but only if 'cat' follows
     'kitty'. Note that the match only includes 'kitty' and not 'kittycat'.
 
     >>> from humre import *
     >>> 'kitty' + positive_lookahead('cat')
     'kitty(?=cat)'
-    >>> compile('kitty' + positive_lookahead('cat')).search('kitty') == None
+    >>> import re
+    >>> re.compile('kitty' + positive_lookahead('cat')).search('kitty') == None
     True
-    >>> compile('kitty' + positive_lookahead('cat')).search('kittycat')
+    >>> re.compile('kitty' + positive_lookahead('cat')).search('kittycat')
     <re.Match object; span=(0, 5), match='kitty'>
     """
     return '(?=' + ''.join(regex_strs) + ')'
 
 
 positive_lookahead = lookahead
 
@@ -344,17 +346,18 @@
     In the following example, 'kitty' is matched but only if the 'cat'
     does not follow 'kitty'. Note that the match only includes 'kitty' and
     not 'kittycat'.
 
     >>> from humre import *
     >>> 'kitty' + negative_lookahead('cat')
     'kitty(?!cat)'
-    >>> compile('kitty' + negative_lookahead('cat')).search('kitty')
+    >>> import re
+    >>> re.compile('kitty' + negative_lookahead('cat')).search('kitty')
     <re.Match object; span=(0, 5), match='kitty'>
-    >>> compile('kitty' + negative_lookahead('cat')).search('kittycat') == None
+    >>> re.compile('kitty' + negative_lookahead('cat')).search('kittycat') == None
     True
     """
     return '(?!' + ''.join(regex_strs) + ')'
 
 
 def lookbehind(*regex_strs):  # type: (str) -> str
     """Returns a string in the regex syntax for a positive lookbehind
@@ -364,14 +367,15 @@
 
     In the following example, 'cat' is matched but only if 'kitty' is before
     'cat'. Note that the match only includes 'cat' and not 'kittycat'.
 
     >>> from humre import *
     >>> positive_lookbehind('kitty') + 'cat'
     '(?<=kitty)cat'
+    >>> import re
     >>> compile(positive_lookbehind('kitty') + 'cat').search('kittycat')
     <re.Match object; span=(5, 8), match='cat'>
     >>> compile(positive_lookbehind('kitty') + 'cat').search('cat') == None
     True
     """
     return '(?<=' + ''.join(regex_strs) + ')'
 
@@ -386,17 +390,18 @@
 
     In the following example, 'cat' is matched but only if 'kitty' is not
     before 'cat'. Note that the match only includes 'cat' and not 'kittycat'.
 
     >>> from humre import *
     >>> negative_lookbehind('kitty') + 'cat'
     '(?<!kitty)cat'
-    >>> compile(negative_lookbehind('kitty') + 'cat').search('kittycat') == None
+    >>> import re
+    >>> re.compile(negative_lookbehind('kitty') + 'cat').search('kittycat') == None
     True
-    >>> compile(negative_lookbehind('kitty') + 'cat').search('black cat')
+    >>> re.compile(negative_lookbehind('kitty') + 'cat').search('black cat')
     <re.Match object; span=(6, 9), match='cat'>
     """
     return '(?<!' + ''.join(regex_strs) + ')'
 
 
 def named_group(name, *regex_strs):  # type: (str, str) -> str
     r"""Returns a string in the regex syntax for a named group of the regex
@@ -443,54 +448,56 @@
 
     >>> from humre import *
     >>> optional('a')
     'a?'
     >>> optional(group('spam'))
     '(spam)?'
     """
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
-    return regexStr + '?'
+    return regex_str + '?'
 
 
-# TODO - it's going to be really easy to get this wrong when people pass multiple comma-separated arguments when they intended to pass fewer string arguments in. How do we avoid this problem?
+# TODO - it's going to be really easy to get this wrong when people pass multiple comma-separated arguments when they
+# intended to pass fewer string arguments in. How do we avoid this problem?
 def either(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for the alternation or "or"
     operator of the regex strings in regex_strs. This matches one of
     the strings in regex_strs.
 
     >>> from humre import *
     >>> either(group('cat'), group('dog'), group('moose'))
     '(cat)|(dog)|(moose)'
     """
-    regex_strs = tuple([s for s in regex_strs if s != ''])
+    regex_strs = tuple(s for s in regex_strs if s != '')
     if len(regex_strs) == 0:
         raise ValueError('regex_strs argument must have at least one nonblank value')
     return '|'.join(regex_strs)
 
 
 def exactly(quantity, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching an exact number
     of occurrences of the regex strings in regex_strs.
 
     >>> from humre import *
     >>> exactly(3, 'A')
     'A{3}'
-    >>> compile(exactly(3, 'a')).search('aaaaah!')
+    >>> import re
+    >>> re.compile(exactly(3, 'a')).search('aaaaah!')
     <re.Match object; span=(0, 3), match='aaa'>
     """
     if not isinstance(quantity, int):
         raise TypeError('quantity argument must be a positive int, not ' + type(quantity).__qualname__)
     if quantity < 0:
         raise ValueError('quantity argument must be a positive int, not ' + str(quantity))
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
-    return regexStr + '{' + str(quantity) + '}'
+    return regex_str + '{' + str(quantity) + '}'
 
 
 def between(minimum, maximum, *regex_strs):  # type: (int, int, str) -> str
     r"""Returns a string in the regex syntax for matching an between the
     minimum and maximum number of occurrences of the regex strings in
     regex_strs.
 
@@ -504,114 +511,114 @@
         raise ValueError('minimum argument must be a positive int, not ' + str(minimum))
     if not isinstance(maximum, int):
         raise TypeError('maximum argument must be a positive int, not ' + type(maximum).__qualname__)
     if maximum < 0:
         raise ValueError('maximum argument must be a positive int, not ' + str(maximum))
     if minimum > maximum:
         raise ValueError('minimum argument ' + str(minimum) + ' must be less than maximum argument ' + str(maximum))
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
-    return regexStr + '{' + str(minimum) + ',' + str(maximum) + '}'
+    return regex_str + '{' + str(minimum) + ',' + str(maximum) + '}'
 
 
 def at_least(minimum, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching a minimum number
     of occurrences of the regex strings in regex_strs.
 
     >>> from humre import *
     >>> at_least(3, 'abc')
     'abc{3,}'
     """
     if not isinstance(minimum, int):
         raise TypeError('minimum argument must be a positive int, not ' + type(minimum).__qualname__)
     if minimum < 0:
         raise ValueError('minimum argument must be a positive int, not ' + str(minimum))
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
-    return regexStr + '{' + str(minimum) + ',}'
+    return regex_str + '{' + str(minimum) + ',}'
 
 
 def at_most(maximum, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching a maximum number
     of occurrences of the regex strings in regex_strs.
 
     >>> from humre import *
     >>> at_most(3, 'abc')
     'abc{,3}'
     """
     if not isinstance(maximum, int):
         raise TypeError('maximum argument must be a positive int, not ' + type(maximum).__qualname__)
     if maximum < 0:
         raise ValueError('maximum argument must be a positive int, not ' + str(maximum))
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
-    return regexStr + '{,' + str(maximum) + '}'
+    return regex_str + '{,' + str(maximum) + '}'
 
 
 def zero_or_more(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for matching zero or more
     occurrences of the regex strings in regex_strs. This does a
     greedy match, which tries to make the largest match possible.
 
     >>> from humre import *
     >>> zero_or_more('abc')
     'abc*'
     """
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
     return ''.join(regex_strs) + '*'
 
 
 def zero_or_more_lazy(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for matching zero or more
     occurrences of the regex strings in regex_strs. This does a
     lazy match, which tries to make the smallest match possible.
 
     >>> from humre import *
     >>> zero_or_more_lazy('abc')
     'abc*?'
     """
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
-    return regexStr + '*?'
+    return regex_str + '*?'
 
 
 def one_or_more(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for matching zero or more
     occurrences of the regex strings in regex_strs. This does a
     lazy match, which tries to make the smallest match possible.
 
     >>> from humre import *
     >>> one_or_more('abc')
     'abc+'
     """
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
-    return regexStr + '+'
+    return regex_str + '+'
 
 
 def one_or_more_lazy(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for matching one or more
     occurrences of the regex strings in regex_strs. This does a
     lazy match, which tries to make the smallest match possible.
 
     >>> from humre import *
     >>> one_or_more_lazy('abc')
     'abc+?'
     """
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
-    return regexStr + '+?'
+    return regex_str + '+?'
 
 
 def starts_with(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for matching the pattern
     of the regex strings in regex_strs at the start of the searched
     text.
 
@@ -701,72 +708,72 @@
     operator of the patterns in regex_strs, and the alternation
     is placed in a group.
 
     >>> from humre import *
     >>> group_either('a', 'b', 'c')
     '(a|b|c)'
     """
-    regex_strs = tuple([s for s in regex_strs if s != ''])
+    regex_strs = tuple(s for s in regex_strs if s != '')
     return '(' + '|'.join(regex_strs) + ')'
 
 
 def noncap_group_either(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for the alternation or "or"
     operator of the patterns in regex_strs, and the alternation
     is placed in a noncapturing group.
 
     >>> from humre import *
     >>> noncap_group_either('a', 'b', 'c')
     '(?:a|b|c)'
     """
-    regex_strs = tuple([s for s in regex_strs if s != ''])
+    regex_strs = tuple(s for s in regex_strs if s != '')
     return '(?:' + '|'.join(regex_strs) + ')'
 
 
-def group_exactly(quantity, *regex_strs):  # type: (int, str) -> str
+def exactly_group(quantity, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching an exact number
     of occurrences of the regex strings in regex_strs, placed in a
     group.
 
     >>> from humre import *
-    >>> group_exactly(3, 'abc')
+    >>> exactly_group(3, 'abc')
     '(abc){3}'
     """
     if not isinstance(quantity, int):
         raise TypeError('quantity argument must be a positive int, not ' + type(quantity).__qualname__)
     if quantity < 0:
         raise ValueError('quantity argument must be a positive int, not ' + str(quantity))
 
     return '(' + ''.join(regex_strs) + '){' + str(quantity) + '}'
 
 
-def noncap_group_exactly(quantity, *regex_strs):  # type: (int, str) -> str
+def exactly_noncap_group(quantity, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching an exact number
     of occurrences of the regex strings in regex_strs, placed in a
     noncapturing group.
 
     >>> from humre import *
-    >>> noncap_group_exactly(3, 'abc')
+    >>> exactly_noncap_group(3, 'abc')
     '(?:abc){3}'
     """
     if not isinstance(quantity, int):
         raise TypeError('quantity argument must be a positive int, not ' + type(quantity).__qualname__)
     if quantity < 0:
         raise ValueError('quantity argument must be a positive int, not ' + str(quantity))
 
     return '(?:' + ''.join(regex_strs) + '){' + str(quantity) + '}'
 
 
-def group_between(minimum, maximum, *regex_strs):  # type: (int, int, str) -> str
+def between_group(minimum, maximum, *regex_strs):  # type: (int, int, str) -> str
     r"""Returns a string in the regex syntax for matching between a minimum
     and maximum number of occurrences of the regex strings in
     regex_strs, placed in a  group.
 
     >>> from humre import *
-    >>> group_between(3, 5, 'abc')
+    >>> between_group(3, 5, 'abc')
     '(abc){3,5}'
     """
     if not isinstance(minimum, int):
         raise TypeError('minimum argument must be a positive int, not ' + type(minimum).__qualname__)
     if minimum < 0:
         raise ValueError('minimum argument must be a positive int, not ' + str(minimum))
     if not isinstance(maximum, int):
@@ -775,21 +782,21 @@
         raise ValueError('maximum argument must be a positive int, not ' + str(maximum))
     if minimum > maximum:
         raise ValueError('minimum argument ' + str(minimum) + ' must be less than maximum argument ' + str(maximum))
 
     return '(' + ''.join(regex_strs) + '){' + str(minimum) + ',' + str(maximum) + '}'
 
 
-def noncap_group_between(minimum, maximum, *regex_strs):  # type: (int, int, str) -> str
+def between_noncap_group(minimum, maximum, *regex_strs):  # type: (int, int, str) -> str
     r"""Returns a string in the regex syntax for matching between a minimum
     and maximum number of occurrences of the regex strings in
     regex_strs, placed in a noncapturing group.
 
     >>> from humre import *
-    >>> noncap_group_between(3, 5, 'abc')
+    >>> between_noncap_group(3, 5, 'abc')
     '(?:abc){3,5}'
     """
     if not isinstance(minimum, int):
         raise TypeError('minimum argument must be a positive int, not ' + type(minimum).__qualname__)
     if minimum < 0:
         raise ValueError('minimum argument must be a positive int, not ' + str(minimum))
     if not isinstance(maximum, int):
@@ -798,72 +805,72 @@
         raise ValueError('maximum argument must be a positive int, not ' + str(maximum))
     if minimum > maximum:
         raise ValueError('minimum argument ' + str(minimum) + ' must be less than maximum argument ' + str(maximum))
 
     return '(?:' + ''.join(regex_strs) + '){' + str(minimum) + ',' + str(maximum) + '}'
 
 
-def group_at_least(minimum, *regex_strs):  # type: (int, str) -> str
+def at_least_group(minimum, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching a minimum number
     of occurrences of the regex strings in regex_strs, placed in a
     group.
 
     >>> from humre import *
-    >>> group_at_least(3, 'abc')
+    >>> at_least_group(3, 'abc')
     '(abc){3,}'
     """
     if not isinstance(minimum, int):
         raise TypeError('minimum argument must be a positive int, not ' + type(minimum).__qualname__)
     if minimum < 0:
         raise ValueError('minimum argument must be a positive int, not ' + str(minimum))
 
     return '(' + ''.join(regex_strs) + '){' + str(minimum) + ',}'
 
 
-def noncap_group_at_least(minimum, *regex_strs):  # type: (int, str) -> str
+def at_least_noncap_group(minimum, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching a minimum number
     of occurrences of the regex strings in regex_strs, placed in a
     noncapturing group.
 
     >>> from humre import *
-    >>> noncap_group_at_least(3, 'abc')
+    >>> at_least_noncap_group(3, 'abc')
     '(?:abc){3,}'
     """
     if not isinstance(minimum, int):
         raise TypeError('minimum argument must be a positive int, not ' + type(minimum).__qualname__)
     if minimum < 0:
         raise ValueError('minimum argument must be a positive int, not ' + str(minimum))
 
     return '(?:' + ''.join(regex_strs) + '){' + str(minimum) + ',}'
 
 
-def group_at_most(maximum, *regex_strs):  # type: (int, str) -> str
+def at_most_group(maximum, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching a maximum number
     of occurrences of the regex strings in regex_strs, placed in a
     group.
 
     >>> from humre import *
-    >>> group_at_most(3, 'abc')
+    >>> at_most_group(3, 'abc')
     '(abc){,3}'
     """
     if not isinstance(maximum, int):
         raise TypeError('maximum argument must be a positive int, not ' + type(maximum).__qualname__)
     if maximum < 0:
         raise ValueError('maximum argument must be a positive int, not ' + str(maximum))
 
     return '(' + ''.join(regex_strs) + '){,' + str(maximum) + '}'
 
 
-def noncap_group_at_most(maximum, *regex_strs):  # type: (int, str) -> str
+def at_most_noncap_group(maximum, *regex_strs):  # type: (int, str) -> str
     r"""Returns a string in the regex syntax for matching a maximum number
     of occurrences of the regex strings in regex_strs, placed in a
     group.
 
     >>> from humre import *
-    >>> noncap_group_at_most(3, 'abc')
+    >>> at_most_noncap_group(3, 'abc')
     '(?:abc){,3}'
     """
     if not isinstance(maximum, int):
         raise TypeError('maximum argument must be a positive int, not ' + type(maximum).__qualname__)
     if maximum < 0:
         raise ValueError('maximum argument must be a positive int, not ' + str(maximum))
 
@@ -966,127 +973,69 @@
     >>> from humre import *
     >>> one_or_more_lazy_noncap_group('abc')
     '(?:abc)+?'
     """
     return '(?:' + ''.join(regex_strs) + ')+?'
 
 
-def group_chars(*tuple_of_characters):  # type: (str) -> str
-    r"""Returns a string in the regex syntax for a character class including
-    the characters in tuple_of_characters, and placed in a group.
-
-    >>> from humre import *
-    >>> group_chars('abc')
-    '([abc])'
-    """
-    regexStr = ''.join(tuple_of_characters)
-    if regexStr == '':
-        raise ValueError('tuple_of_characters must have at least one nonblank value')
-    return '([' + regexStr + '])'
-
-
-def noncap_group_chars(*tuple_of_characters):  # type: (str) -> str
-    r"""Returns a string in the regex syntax for a character class including
-    the characters in tuple_of_characters, and placed in a noncapturing
-    group.
-
-    >>> from humre import *
-    >>> noncap_group_chars('abc')
-    '(?:[abc])'
-    """
-    regexStr = ''.join(tuple_of_characters)
-    if regexStr == '':
-        raise ValueError('tuple_of_characters must have at least one nonblank value')
-    return '(?:[' + regexStr + '])'
-
-
-def group_nonchars(*tuple_of_characters):  # type: (str) -> str
-    r"""Returns a string in the regex syntax for a character class excluding
-    the characters in tuple_of_characters, and placed in a group.
-
-    >>> from humre import *
-    >>> group_nonchars('abc')
-    '([^abc])'
-    """
-    regexStr = ''.join(tuple_of_characters)
-    if regexStr == '':
-        raise ValueError('tuple_of_characters must have at least one nonblank value')
-    return '([^' + regexStr + '])'
-
-
-def noncap_group_nonchars(*tuple_of_characters):  # type: (str) -> str
-    r"""Returns a string in the regex syntax for a character class excluding
-    the characters in tuple_of_characters, and placed in a noncapturing
-    group.
-
-    >>> from humre import *
-    >>> noncap_group_nonchars('abc')
-    '(?:[^abc])'
-    """
-    regexStr = ''.join(tuple_of_characters)
-    if regexStr == '':
-        raise ValueError('tuple_of_characters must have at least one nonblank value')
-    return '(?:[^' + regexStr + '])'
-
-
 # TODO - Are there better names for the atomic group and possessive quantifier functions?
 def atomic_group(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for an atomic group of the
     strings in regex_strs. Atomic groups are new in 3.11"""
     return '(?>' + ''.join(regex_strs) + ')'
 
 
 def zero_or_more_possessive(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for a possessive quantifier
     of zero or more matches of the strings in regex_strs.
     Possessive quantifiers are new in 3.11"""
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
     return ''.join(regex_strs) + '*+'
 
 
 def one_or_more_possessive(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for a possessive quantifier
     of one or more matches of the strings in regex_strs.
     Possessive quantifiers are new in 3.11"""
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
     return ''.join(regex_strs) + '++'
 
 
 def optional_possessive(*regex_strs):  # type: (str) -> str
     r"""Returns a string in the regex syntax for a possessive quantifier
     of zero or more matches of the strings in regex_strs.
     Possessive quantifiers are new in 3.11"""
-    regexStr = ''.join(regex_strs)
-    if regexStr == '':
+    regex_str = ''.join(regex_strs)
+    if regex_str == '':
         raise ValueError('regex_strs argument must have at least one nonblank value')
     return ''.join(regex_strs) + '?+'
 
 
 def inline_flag(flags, *regex_strs):  # type: (str, str) -> str
     r"""Returns a string in the regex syntax of the strings in
     regex_strs using inline flags."""
     if not isinstance(flags, str):
         raise TypeError("flags argument must be a str, not " + type(flags).__qualname__)
 
     for flag in flags:
         if flag not in 'aiLmsux-':
             raise ValueError("flags argument is limited to the characters aiLmsux-, and cannot be " + repr(flags)[:100])
 
-    mutuallyExclusiveFlagsCount = 0
+    mutually_exclusive_flags_count = 0
     if 'a' in flags:
-        mutuallyExclusiveFlagsCount += 1
+        mutually_exclusive_flags_count += 1
     if 'L' in flags:
-        mutuallyExclusiveFlagsCount += 1
+        mutually_exclusive_flags_count += 1
     if 'u' in flags:
-        mutuallyExclusiveFlagsCount += 1
-    if mutuallyExclusiveFlagsCount > 1:
+        mutually_exclusive_flags_count += 1
+    if mutually_exclusive_flags_count > 1:
         raise ValueError(
             "flags argument can only have at most one of 'a', 'L', and 'u'' flags, and cannot be " + repr(flags)[:100]
         )
     return '(?' + flags + ':' + ''.join(regex_strs) + ')'
 
 
 # More built-in Humre patterns:
@@ -1130,14 +1079,26 @@
     noncap_group(noncap_group(either('0x', '0X')), one_or_more(chars('0-9a-f'))),
     noncap_group(noncap_group(either('0x', '0X')), one_or_more(chars('0-9A-F'))),
     noncap_group(one_or_more(chars('0-9a-f'))),
     noncap_group(one_or_more(chars('0-9A-F'))),
 )
 
 
+def parse(regex_str, module_name_prefix=None):
+    r"""Given a regex string, returns the humre source code to produce that regex.
+
+    >>> import humre
+    >>> humre.parse('(?P<major>\\d+)(\\.(?P<minor>\\d+))?')
+    "named_group('major', one_or_more(DIGIT)) + optional_group(PERIOD + named_group('minor', one_or_more(DIGIT)))
+    >>> humre.parse('(?P<major>\\d+)(\\.(?P<minor>\\d+))?', 'humre')
+    "humre.named_group('major', humre.one_or_more(humre.DIGIT)) + humre.optional_group(humre.PERIOD + humre.named_group('minor', humre.one_or_more(humre.DIGIT)))
+    """
+
+    # TODO
+
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
 
 '''
 This test shows that using + for string concatenation is a bit faster than using ''.join() for our use cases.
@@ -1153,18 +1114,22 @@
 def group4(*regex_strs):  # type: (str) -> str
     return ''.join(('(', *regex_strs, ')'))
 import timeit
 print(timeit.timeit("group1('cat', 'dog')", globals=globals(), number=100000000))
 print(timeit.timeit("group2('cat', 'dog')", globals=globals(), number=100000000))
 print(timeit.timeit("group3('cat', 'dog')", globals=globals(), number=100000000))
 print(timeit.timeit("group4('cat', 'dog')", globals=globals(), number=100000000))
-print(timeit.timeit("group1('cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog')", globals=globals(), number=100000000))
-print(timeit.timeit("group2('cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog')", globals=globals(), number=100000000))
-print(timeit.timeit("group3('cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog')", globals=globals(), number=100000000))
-print(timeit.timeit("group4('cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog')", globals=globals(), number=100000000))
+print(timeit.timeit("group1('cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog')",
+    globals=globals(), number=100000000))
+print(timeit.timeit("group2('cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog')",
+    globals=globals(), number=100000000))
+print(timeit.timeit("group3('cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog')",
+    globals=globals(), number=100000000))
+print(timeit.timeit("group4('cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog', 'cat', 'dog')",
+    globals=globals(), number=100000000))
 # Times:
 #32.36761399998795
 #36.67457259999355
 #34.13985800003866
 #39.810779399995226
 #49.031997100042645
 #50.96271799999522
```


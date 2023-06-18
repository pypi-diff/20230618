# Comparing `tmp/sciform-0.6.1.tar.gz` & `tmp/sciform-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciform-0.6.1.tar", last modified: Sat May 27 22:09:18 2023, max compression
+gzip compressed data, was "sciform-0.7.0.tar", last modified: Sun May 28 08:03:10 2023, max compression
```

## Comparing `sciform-0.6.1.tar` & `sciform-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.232853 sciform-0.6.1/
--rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.6.1/LICENSE
--rw-rw-rw-   0        0        0    32842 2023-05-27 22:09:18.232853 sciform-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    32474 2023-05-27 22:08:11.000000 sciform-0.6.1/README.md
--rw-rw-rw-   0        0        0      589 2023-05-27 07:16:40.000000 sciform-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 22:09:18.232853 sciform-0.6.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.203997 sciform-0.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.220342 sciform-0.6.1/src/sciform/
--rw-rw-rw-   0        0        0       84 2023-05-27 22:08:47.000000 sciform-0.6.1/src/sciform/__init__.py
--rw-rw-rw-   0        0        0    16402 2023-05-27 21:42:44.000000 sciform-0.6.1/src/sciform/format_spec.py
--rw-rw-rw-   0        0        0     6226 2023-05-27 21:42:44.000000 sciform-0.6.1/src/sciform/format_utils.py
--rw-rw-rw-   0        0        0     2373 2023-05-26 18:40:38.000000 sciform-0.6.1/src/sciform/grouping.py
--rw-rw-rw-   0        0        0     4111 2023-05-27 21:42:44.000000 sciform-0.6.1/src/sciform/modes.py
--rw-rw-rw-   0        0        0     2258 2023-05-27 21:42:44.000000 sciform-0.6.1/src/sciform/prefix.py
--rw-rw-rw-   0        0        0     6996 2023-05-27 21:58:23.000000 sciform-0.6.1/src/sciform/sfloat.py
--rw-rw-rw-   0        0        0     3592 2023-05-27 06:34:06.000000 sciform-0.6.1/src/sciform/unc_format.py
-drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.230852 sciform-0.6.1/src/sciform.egg-info/
--rw-rw-rw-   0        0        0    32842 2023-05-27 22:09:18.000000 sciform-0.6.1/src/sciform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-05-27 22:09:18.000000 sciform-0.6.1/src/sciform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 22:09:18.000000 sciform-0.6.1/src/sciform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 22:09:18.000000 sciform-0.6.1/src/sciform.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 22:09:18.231853 sciform-0.6.1/tests/
--rw-rw-rw-   0        0        0    18672 2023-05-27 21:42:44.000000 sciform-0.6.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:03:10.845714 sciform-0.7.0/
+-rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0    33419 2023-05-28 08:03:10.845714 sciform-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    33051 2023-05-28 07:59:35.000000 sciform-0.7.0/README.md
+-rw-rw-rw-   0        0        0      589 2023-05-27 07:16:40.000000 sciform-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 08:03:10.846725 sciform-0.7.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 08:03:10.804022 sciform-0.7.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 08:03:10.830659 sciform-0.7.0/src/sciform/
+-rw-rw-rw-   0        0        0      401 2023-05-28 08:01:56.000000 sciform-0.7.0/src/sciform/__init__.py
+-rw-rw-rw-   0        0        0    16657 2023-05-28 06:32:39.000000 sciform-0.7.0/src/sciform/format_spec.py
+-rw-rw-rw-   0        0        0     6226 2023-05-28 02:13:38.000000 sciform-0.7.0/src/sciform/format_utils.py
+-rw-rw-rw-   0        0        0     2373 2023-05-26 18:40:38.000000 sciform-0.7.0/src/sciform/grouping.py
+-rw-rw-rw-   0        0        0     4111 2023-05-27 21:42:44.000000 sciform-0.7.0/src/sciform/modes.py
+-rw-rw-rw-   0        0        0     2258 2023-05-27 21:42:44.000000 sciform-0.7.0/src/sciform/prefix.py
+-rw-rw-rw-   0        0        0     6996 2023-05-27 21:58:23.000000 sciform-0.7.0/src/sciform/sfloat.py
+-rw-rw-rw-   0        0        0     5695 2023-05-28 07:57:46.000000 sciform-0.7.0/src/sciform/unc_format.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:03:10.844208 sciform-0.7.0/src/sciform.egg-info/
+-rw-rw-rw-   0        0        0    33419 2023-05-28 08:03:10.000000 sciform-0.7.0/src/sciform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-05-28 08:03:10.000000 sciform-0.7.0/src/sciform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 08:03:10.000000 sciform-0.7.0/src/sciform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-28 08:03:10.000000 sciform-0.7.0/src/sciform.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 08:03:10.844208 sciform-0.7.0/tests/
+-rw-rw-rw-   0        0        0    19364 2023-05-28 07:56:35.000000 sciform-0.7.0/tests/test.py
```

### Comparing `sciform-0.6.1/LICENSE` & `sciform-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sciform-0.6.1/PKG-INFO` & `sciform-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciform
-Version: 0.6.1
+Version: 0.7.0
 Summary: A package for formatting floats into scientific formatted strings.
 Author-email: Justin Gerber <justin.gerber48@gmail.com>
 Project-URL: Homepage, https://github.com/jagerber48/sciform
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -120,18 +120,29 @@
 Also, a valid built-in format specification may give different results 
 when used as part of the built-in FSML compared to when used as part of
 the `sciform` FSML.
 These incompatibilities are captured in a section below.
 
 The `sciform` format specification mini language is given by:
 ```
-[fill "="][sign]["#"][fill_top_digit]
-[thousands_separator][decimal_separator][thousandths_separator]
-[prec_mode precision][format_mode][exp][prefix_mode]
+    format_spec            ::=  [fill "="][sign]["#"][fill_top_digit][thousands_separator][decimal_separator][thousandths_separator][prec_mode precision][format_mode]["x" exp][prefix_mode]
+    
+    fill                   ::=  "0" | " "
+    sign                   ::=  "+" | "-" | " "
+    fill_top_digit         ::=  digit+
+    thousands_separator    ::=  "n" | "." | "," | "s" | "_"
+    decimal_separator      ::=  "." | ","
+    thousandths_separator  ::=  "n" | "s" | "_" 
+    prec_mode              ::=  "!" | "."
+    prec                   ::=  -?digit+
+    format_mode            ::=  "f" | "F" | "%" | "e" | "E" | "r" | "R" | "b" | "B" |
+    exp                    ::=  [+-]digit+
+    prefix_mode            ::=  p
 ```
+
 Where the terms are described in the table below.
 
 The `sciform` FSML is accessed via the `sfloat` object. Regular built-in
 floats are cast to `sfloat` objects which can be formatted using the 
 `sciform` FSML.
 
 ```
@@ -152,15 +163,15 @@
 | fill_top_digit <br/> (`\d+`)                                                      | Any non-negative integer, default (0). Indicates the decimal or binary place to which the formatted string should be padded. e.g. `f'{sfloat(123):0=4}'` will give `00123`, i.e. padding to the `10^4` place.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | thousands_separator <br/> (`'n'`, `'.'`, `','`, `'s'`, `'_'`)                     | Indicates the character to use as a thousands separator. `'n'` is no separator, `'s'` is a single-whitespace separator and `'.'`, `','`, and `'_'` are period, comma, and underscore separators. Note that NIST discourages the use of `','` or `'.'` as thousands seperators because they can be confused with the decimal separators depending on the locality. See [NIST Guide to the SI 10.5.3](https://www.nist.gov/pml/special-publication-811/nist-guide-si-chapter-10-more-printing-and-using-symbols-and-numbers#1053).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 | decimal_separator <br/> (`'.'`, `','`)                                            | Symbol to use as the decimal separator.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | thousandths_separator <br/> (`'n'`, `'s'`, `'_'`)                                 | Indicates the character to use as a thousandths separator. `'n'` is no separator, `'s'` is a single-whitespace separator and `'_'` is an underscore separators.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
 | prec_mode <br/> (`'!'`, `'.'`)                                                    | Indicates whether the float will be rounded and displayed according to precision (digits past the decimal point) or significant figure. `'.'` indicates precision mode and `'!'` indicates significant figure mode. E.g. `f'{sfloat(123.456):.2f}'` gives `'123.46'` while `f'{sfloat(123.456):!2f}'` gives `'120'`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 | prec <br/> (`-?\d+`)                                                              | Integer indicating the precision or number of significant figures to which the float shall be rounded and displayed. Can be negative for precision formatting mode. Must be greater than zero for significant figure mode. If no precision is supplied then an algorithm will be used to attempt to infer the least significant digit for the float and the precision will be chosen to match this least significant digit. This algorithm may have surprising behavior for floats with a large number (e.g. 15) of significant digits or due to the underlying binary nature of floats, e.g. `0.1+0.2 = 0.30000000000000004`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 | format_mode <br/> (`'f'`, `'F'`, `'%'`, `'e'`, `'E'`, `'r'`, `'R'`, `'b'`, `'B'`) | Indicates which formatting mode should be used. In all cases the capitalization of the exponent symbol matches the capitalization of the format mode flag. <br/> &nbsp; -`'f'` and `'F'` indicate fixed point mode in which no exponent is used to display the number. <br/> &nbsp; -`'%'` mode is like fixed mode but the number is first multiplied by 100 and presented followed by a `'%'` character.<br/> &nbsp; -`'e'` and `'E'` indicate scientific notation in which the exponent is chosen so that the mantissa satisfies `1 <= m < 10`. <br/> &nbsp; -`'r'` and `'R'` indicate engineering notation in which the exponent is chosen so that the mantissa satisfies `1 <= m <= 1000`. If the alternate mode is enabled then the mantissa satisfies `0.1 <= m < 100`. In both cases the exponent is always an integer multiple of 3.<br/>&nbsp; -`'b'` and `'B'` indicate binary mode in which the number is presented as a mantissa and exponent in base 2. The mantissa satisfies `1 <= m < 2`. If alternate mode is enabled the mantissa satisfies `1 <= m < 1024 = 2^10`. In this case the exponent is always an integer multiple of 10. |
-| exp <br/> (`[+-]\d+`)                                                             | Positive or negative integer that can be used to force the exponent to take a particular value. This flag is ignored in fixed format mode. If an explicit exponent is used in engineering mode or alternate binary mode which is incompatible with those modes (e.g. an exponent that is not a multiple of 3 for engineering notation), the exponent will be rounded down to the nearest compatible value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| exp <br/> (`x[+-]\d+`)                                                            | Positive or negative integer that can be used to force the exponent to take a particular value. This flag is ignored in fixed format mode. If an explicit exponent is used in engineering mode or alternate binary mode which is incompatible with those modes (e.g. an exponent that is not a multiple of 3 for engineering notation), the exponent will be rounded down to the nearest compatible value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | prefix_mode <br/> (`'p'`)                                                         | Flag (default off) indicating whether exponent strings should be replaced with SI or IEC prefix characters. E.g. `'123e+03' -> 123 k` or `857.2B+20 -> 857.2 Mi`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
  
 # Prefix Mode
 
 Prefix mode offers a simple translation between exponent strings and 
 one or two letter prefixes. 
 For scientific and engineering formats the prefixes are matched to
```

### Comparing `sciform-0.6.1/README.md` & `sciform-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -110,18 +110,29 @@
 Also, a valid built-in format specification may give different results 
 when used as part of the built-in FSML compared to when used as part of
 the `sciform` FSML.
 These incompatibilities are captured in a section below.
 
 The `sciform` format specification mini language is given by:
 ```
-[fill "="][sign]["#"][fill_top_digit]
-[thousands_separator][decimal_separator][thousandths_separator]
-[prec_mode precision][format_mode][exp][prefix_mode]
+    format_spec            ::=  [fill "="][sign]["#"][fill_top_digit][thousands_separator][decimal_separator][thousandths_separator][prec_mode precision][format_mode]["x" exp][prefix_mode]
+    
+    fill                   ::=  "0" | " "
+    sign                   ::=  "+" | "-" | " "
+    fill_top_digit         ::=  digit+
+    thousands_separator    ::=  "n" | "." | "," | "s" | "_"
+    decimal_separator      ::=  "." | ","
+    thousandths_separator  ::=  "n" | "s" | "_" 
+    prec_mode              ::=  "!" | "."
+    prec                   ::=  -?digit+
+    format_mode            ::=  "f" | "F" | "%" | "e" | "E" | "r" | "R" | "b" | "B" |
+    exp                    ::=  [+-]digit+
+    prefix_mode            ::=  p
 ```
+
 Where the terms are described in the table below.
 
 The `sciform` FSML is accessed via the `sfloat` object. Regular built-in
 floats are cast to `sfloat` objects which can be formatted using the 
 `sciform` FSML.
 
 ```
@@ -142,15 +153,15 @@
 | fill_top_digit <br/> (`\d+`)                                                      | Any non-negative integer, default (0). Indicates the decimal or binary place to which the formatted string should be padded. e.g. `f'{sfloat(123):0=4}'` will give `00123`, i.e. padding to the `10^4` place.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | thousands_separator <br/> (`'n'`, `'.'`, `','`, `'s'`, `'_'`)                     | Indicates the character to use as a thousands separator. `'n'` is no separator, `'s'` is a single-whitespace separator and `'.'`, `','`, and `'_'` are period, comma, and underscore separators. Note that NIST discourages the use of `','` or `'.'` as thousands seperators because they can be confused with the decimal separators depending on the locality. See [NIST Guide to the SI 10.5.3](https://www.nist.gov/pml/special-publication-811/nist-guide-si-chapter-10-more-printing-and-using-symbols-and-numbers#1053).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 | decimal_separator <br/> (`'.'`, `','`)                                            | Symbol to use as the decimal separator.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | thousandths_separator <br/> (`'n'`, `'s'`, `'_'`)                                 | Indicates the character to use as a thousandths separator. `'n'` is no separator, `'s'` is a single-whitespace separator and `'_'` is an underscore separators.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
 | prec_mode <br/> (`'!'`, `'.'`)                                                    | Indicates whether the float will be rounded and displayed according to precision (digits past the decimal point) or significant figure. `'.'` indicates precision mode and `'!'` indicates significant figure mode. E.g. `f'{sfloat(123.456):.2f}'` gives `'123.46'` while `f'{sfloat(123.456):!2f}'` gives `'120'`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 | prec <br/> (`-?\d+`)                                                              | Integer indicating the precision or number of significant figures to which the float shall be rounded and displayed. Can be negative for precision formatting mode. Must be greater than zero for significant figure mode. If no precision is supplied then an algorithm will be used to attempt to infer the least significant digit for the float and the precision will be chosen to match this least significant digit. This algorithm may have surprising behavior for floats with a large number (e.g. 15) of significant digits or due to the underlying binary nature of floats, e.g. `0.1+0.2 = 0.30000000000000004`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 | format_mode <br/> (`'f'`, `'F'`, `'%'`, `'e'`, `'E'`, `'r'`, `'R'`, `'b'`, `'B'`) | Indicates which formatting mode should be used. In all cases the capitalization of the exponent symbol matches the capitalization of the format mode flag. <br/> &nbsp; -`'f'` and `'F'` indicate fixed point mode in which no exponent is used to display the number. <br/> &nbsp; -`'%'` mode is like fixed mode but the number is first multiplied by 100 and presented followed by a `'%'` character.<br/> &nbsp; -`'e'` and `'E'` indicate scientific notation in which the exponent is chosen so that the mantissa satisfies `1 <= m < 10`. <br/> &nbsp; -`'r'` and `'R'` indicate engineering notation in which the exponent is chosen so that the mantissa satisfies `1 <= m <= 1000`. If the alternate mode is enabled then the mantissa satisfies `0.1 <= m < 100`. In both cases the exponent is always an integer multiple of 3.<br/>&nbsp; -`'b'` and `'B'` indicate binary mode in which the number is presented as a mantissa and exponent in base 2. The mantissa satisfies `1 <= m < 2`. If alternate mode is enabled the mantissa satisfies `1 <= m < 1024 = 2^10`. In this case the exponent is always an integer multiple of 10. |
-| exp <br/> (`[+-]\d+`)                                                             | Positive or negative integer that can be used to force the exponent to take a particular value. This flag is ignored in fixed format mode. If an explicit exponent is used in engineering mode or alternate binary mode which is incompatible with those modes (e.g. an exponent that is not a multiple of 3 for engineering notation), the exponent will be rounded down to the nearest compatible value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| exp <br/> (`x[+-]\d+`)                                                            | Positive or negative integer that can be used to force the exponent to take a particular value. This flag is ignored in fixed format mode. If an explicit exponent is used in engineering mode or alternate binary mode which is incompatible with those modes (e.g. an exponent that is not a multiple of 3 for engineering notation), the exponent will be rounded down to the nearest compatible value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | prefix_mode <br/> (`'p'`)                                                         | Flag (default off) indicating whether exponent strings should be replaced with SI or IEC prefix characters. E.g. `'123e+03' -> 123 k` or `857.2B+20 -> 857.2 Mi`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
  
 # Prefix Mode
 
 Prefix mode offers a simple translation between exponent strings and 
 one or two letter prefixes. 
 For scientific and engineering formats the prefixes are matched to
```

### Comparing `sciform-0.6.1/pyproject.toml` & `sciform-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciform-0.6.1/src/sciform/format_spec.py` & `sciform-0.7.0/src/sciform/format_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,25 +314,32 @@
                            **kwargs):
     global FMT_SPEC_GLOBAL_DEFAULTS
     if new_fmt_spec is not None:
         FMT_SPEC_GLOBAL_DEFAULTS = new_fmt_spec
     FMT_SPEC_GLOBAL_DEFAULTS.update(**kwargs)
 
 
+def reset_global_defaults():
+    global FMT_SPEC_GLOBAL_DEFAULTS
+    FMT_SPEC_GLOBAL_DEFAULTS = FMT_SPEC_PKG_DEFAULTS
+
+
+# TODO: Not possible to specify exp directly if nothing is specified between
+#       exp and sign and top digit place.
 pattern = re.compile(r'''^
                          (?:(?P<fill>[ 0])=)?
                          (?P<sign>[+\- ])?
                          (?P<alternate>\#)?                         
                          (?P<top_dig_place>\d+)?
                          (?P<thousands_separator>[n,.s_])?                     
                          (?P<decimal_separator>[.,])?            
                          (?P<thousandths_separator>[ns_])?                  
-                         (?:(?P<prec_mode>[.!])(?P<prec>-?\d+))?
+                         (?:(?P<prec_mode>[.!])(?P<prec>[+-]?\d+))?
                          (?P<format_mode>[fF%eErRbB])?
-                         (?P<exp>[+-]\d+)?
+                         (?:x(?P<exp>[+-]?\d+))?
                          (?P<prefix_mode>p)?
                          $''', re.VERBOSE)
 
 
 def parse_format_spec(
         fmt: str,
         format_spec_template: Optional[FormatSpec] = None) \
```

### Comparing `sciform-0.6.1/src/sciform/format_utils.py` & `sciform-0.7.0/src/sciform/format_utils.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.1/src/sciform/grouping.py` & `sciform-0.7.0/src/sciform/grouping.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.1/src/sciform/modes.py` & `sciform-0.7.0/src/sciform/modes.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.1/src/sciform/prefix.py` & `sciform-0.7.0/src/sciform/prefix.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.1/src/sciform/sfloat.py` & `sciform-0.7.0/src/sciform/sfloat.py`

 * *Files identical despite different names*

### Comparing `sciform-0.6.1/src/sciform.egg-info/PKG-INFO` & `sciform-0.7.0/src/sciform.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciform
-Version: 0.6.1
+Version: 0.7.0
 Summary: A package for formatting floats into scientific formatted strings.
 Author-email: Justin Gerber <justin.gerber48@gmail.com>
 Project-URL: Homepage, https://github.com/jagerber48/sciform
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -120,18 +120,29 @@
 Also, a valid built-in format specification may give different results 
 when used as part of the built-in FSML compared to when used as part of
 the `sciform` FSML.
 These incompatibilities are captured in a section below.
 
 The `sciform` format specification mini language is given by:
 ```
-[fill "="][sign]["#"][fill_top_digit]
-[thousands_separator][decimal_separator][thousandths_separator]
-[prec_mode precision][format_mode][exp][prefix_mode]
+    format_spec            ::=  [fill "="][sign]["#"][fill_top_digit][thousands_separator][decimal_separator][thousandths_separator][prec_mode precision][format_mode]["x" exp][prefix_mode]
+    
+    fill                   ::=  "0" | " "
+    sign                   ::=  "+" | "-" | " "
+    fill_top_digit         ::=  digit+
+    thousands_separator    ::=  "n" | "." | "," | "s" | "_"
+    decimal_separator      ::=  "." | ","
+    thousandths_separator  ::=  "n" | "s" | "_" 
+    prec_mode              ::=  "!" | "."
+    prec                   ::=  -?digit+
+    format_mode            ::=  "f" | "F" | "%" | "e" | "E" | "r" | "R" | "b" | "B" |
+    exp                    ::=  [+-]digit+
+    prefix_mode            ::=  p
 ```
+
 Where the terms are described in the table below.
 
 The `sciform` FSML is accessed via the `sfloat` object. Regular built-in
 floats are cast to `sfloat` objects which can be formatted using the 
 `sciform` FSML.
 
 ```
@@ -152,15 +163,15 @@
 | fill_top_digit <br/> (`\d+`)                                                      | Any non-negative integer, default (0). Indicates the decimal or binary place to which the formatted string should be padded. e.g. `f'{sfloat(123):0=4}'` will give `00123`, i.e. padding to the `10^4` place.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 | thousands_separator <br/> (`'n'`, `'.'`, `','`, `'s'`, `'_'`)                     | Indicates the character to use as a thousands separator. `'n'` is no separator, `'s'` is a single-whitespace separator and `'.'`, `','`, and `'_'` are period, comma, and underscore separators. Note that NIST discourages the use of `','` or `'.'` as thousands seperators because they can be confused with the decimal separators depending on the locality. See [NIST Guide to the SI 10.5.3](https://www.nist.gov/pml/special-publication-811/nist-guide-si-chapter-10-more-printing-and-using-symbols-and-numbers#1053).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
 | decimal_separator <br/> (`'.'`, `','`)                                            | Symbol to use as the decimal separator.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | thousandths_separator <br/> (`'n'`, `'s'`, `'_'`)                                 | Indicates the character to use as a thousandths separator. `'n'` is no separator, `'s'` is a single-whitespace separator and `'_'` is an underscore separators.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
 | prec_mode <br/> (`'!'`, `'.'`)                                                    | Indicates whether the float will be rounded and displayed according to precision (digits past the decimal point) or significant figure. `'.'` indicates precision mode and `'!'` indicates significant figure mode. E.g. `f'{sfloat(123.456):.2f}'` gives `'123.46'` while `f'{sfloat(123.456):!2f}'` gives `'120'`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 | prec <br/> (`-?\d+`)                                                              | Integer indicating the precision or number of significant figures to which the float shall be rounded and displayed. Can be negative for precision formatting mode. Must be greater than zero for significant figure mode. If no precision is supplied then an algorithm will be used to attempt to infer the least significant digit for the float and the precision will be chosen to match this least significant digit. This algorithm may have surprising behavior for floats with a large number (e.g. 15) of significant digits or due to the underlying binary nature of floats, e.g. `0.1+0.2 = 0.30000000000000004`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
 | format_mode <br/> (`'f'`, `'F'`, `'%'`, `'e'`, `'E'`, `'r'`, `'R'`, `'b'`, `'B'`) | Indicates which formatting mode should be used. In all cases the capitalization of the exponent symbol matches the capitalization of the format mode flag. <br/> &nbsp; -`'f'` and `'F'` indicate fixed point mode in which no exponent is used to display the number. <br/> &nbsp; -`'%'` mode is like fixed mode but the number is first multiplied by 100 and presented followed by a `'%'` character.<br/> &nbsp; -`'e'` and `'E'` indicate scientific notation in which the exponent is chosen so that the mantissa satisfies `1 <= m < 10`. <br/> &nbsp; -`'r'` and `'R'` indicate engineering notation in which the exponent is chosen so that the mantissa satisfies `1 <= m <= 1000`. If the alternate mode is enabled then the mantissa satisfies `0.1 <= m < 100`. In both cases the exponent is always an integer multiple of 3.<br/>&nbsp; -`'b'` and `'B'` indicate binary mode in which the number is presented as a mantissa and exponent in base 2. The mantissa satisfies `1 <= m < 2`. If alternate mode is enabled the mantissa satisfies `1 <= m < 1024 = 2^10`. In this case the exponent is always an integer multiple of 10. |
-| exp <br/> (`[+-]\d+`)                                                             | Positive or negative integer that can be used to force the exponent to take a particular value. This flag is ignored in fixed format mode. If an explicit exponent is used in engineering mode or alternate binary mode which is incompatible with those modes (e.g. an exponent that is not a multiple of 3 for engineering notation), the exponent will be rounded down to the nearest compatible value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| exp <br/> (`x[+-]\d+`)                                                            | Positive or negative integer that can be used to force the exponent to take a particular value. This flag is ignored in fixed format mode. If an explicit exponent is used in engineering mode or alternate binary mode which is incompatible with those modes (e.g. an exponent that is not a multiple of 3 for engineering notation), the exponent will be rounded down to the nearest compatible value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
 | prefix_mode <br/> (`'p'`)                                                         | Flag (default off) indicating whether exponent strings should be replaced with SI or IEC prefix characters. E.g. `'123e+03' -> 123 k` or `857.2B+20 -> 857.2 Mi`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
  
 # Prefix Mode
 
 Prefix mode offers a simple translation between exponent strings and 
 one or two letter prefixes. 
 For scientific and engineering formats the prefixes are matched to
```

### Comparing `sciform-0.6.1/tests/test.py` & `sciform-0.7.0/tests/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,10 @@
-from dataclasses import dataclass
 import unittest
 
-from sciform import sfloat
-from sciform.sfloat import GlobalDefaultsContext
-
-
-@dataclass
-class SingleFloatCase:
-    num: float
-    fmt_spec_result_mapping: dict[str, str]
-
-
-fmtcases: dict[float, dict[str, str]] = {
-    123.456: {'': '123.456',
-              'f': '123.456',
-              'e': '1.23456e+02',
-              'r': '123.456e+00',
-              '#r': '0.123456e+03',
-              '.3': '123.456',
-              '.3f': '123.456',
-              '.3e': '1.235e+02',
-              '.3r': '123.456e+00',
-              '#.3r': '0.123e+03',
-              '!3': '123',
-              '!3f': '123',
-              '!3e': '1.23e+02',
-              '!3r': '123e+00',
-              '#!3r': '0.123e+03',
-              '+': '+123.456',
-              '+f': '+123.456',
-              '+e': '+1.23456e+02',
-              '+r': '+123.456e+00',
-              '+#r': '+0.123456e+03',
-              ' ': ' 123.456',
-              ' f': ' 123.456',
-              ' e': ' 1.23456e+02',
-              ' r': ' 123.456e+00',
-              ' #r': ' 0.123456e+03',
-              '4': '  123.456',
-              '4f': '  123.456',
-              '4e': '    1.23456e+02',
-              '4r': '  123.456e+00',
-              '#4r': '    0.123456e+03',
-              },
-    -0.031415: {'': '-0.031415',
-                'f': '-0.031415',
-                'e': '-3.1415e-02',
-                'r': '-31.415e-03',
-                '#r': '-31.415e-03',
-                '.3': '-0.031',
-                '.3f': '-0.031',
-                '.3e': '-3.141e-02',
-                '.3r': '-31.415e-03',
-                '#.3r': '-31.415e-03',
-                '!3': '-0.0314',
-                '!3f': '-0.0314',
-                '!3e': '-3.14e-02',
-                '!3r': '-31.4e-03',
-                '#!3r': '-31.4e-03',
-                '+': '-0.031415',
-                '+f': '-0.031415',
-                '+e': '-3.1415e-02',
-                '+r': '-31.415e-03',
-                '+#r': '-31.415e-03',
-                ' ': '-0.031415',
-                ' f': '-0.031415',
-                ' e': '-3.1415e-02',
-                ' r': '-31.415e-03',
-                ' #r': '-31.415e-03',
-                '4': '-    0.031415',
-                '4f': '-    0.031415',
-                '4e': '-    3.1415e-02',
-                '4r': '-   31.415e-03',
-                '#4r': '-   31.415e-03',
-                '%': '-3.1415%'
-                },
-    0: {'': '0',
-        'f': '0',
-        'e': '0e+00',
-        'r': '0e+00',
-        '#r': '0e+00',
-        '.3': '0.000',
-        '.3f': '0.000',
-        '.3e': '0.000e+00',
-        '.3r': '0.000e+00',
-        '#.3r': '0.000e+00',
-        '!3': '0.00',
-        '!3f': '0.00',
-        '!3e': '0.00e+00',
-        '!3r': '0.00e+00',
-        '#!3r': '0.00e+00',
-        '0=2.3': '000.000',
-        '0=2.3f': '000.000',
-        '0=2.3e': '000.000e+00',
-        '0=2.3r': '000.000e+00',
-        '0=#2.3r': '000.000e+00',
-        '0=2!3': '000.00',
-        '0=2!3f': '000.00',
-        '0=2!3e': '000.00e+00',
-        '0=2!3r': '000.00e+00',
-        '0=#2!3r': '000.00e+00'},
-    float('nan'): {'': 'nan',
-                   'E': 'NAN'},
-    float('inf'): {'': 'inf',
-                   'E': 'INF'},
-    float('-inf'): {'': '-inf',
-                    'E': '-INF'}
-}
+from sciform import sfloat, GlobalDefaultsContext, vufloat
 
 
 class TestFormatting(unittest.TestCase):
     # TODO: exp symbol capitalization
 
     def do_test_case_dict(self, cases_dict: dict[float, dict[str, str]]):
         for num, fmt_dict in cases_dict.items():
@@ -118,14 +12,26 @@
                 snum = sfloat(num)
                 snum_str = f'{snum:{format_spec}}'
                 with self.subTest(num=num, format_spec=format_spec,
                                   expected_num_str=expected_num_str,
                                   actual_num_str=snum_str):
                     self.assertEqual(snum_str, expected_num_str)
 
+    def do_unc_val_test_case_dict(
+            self,
+            cases_dict: dict[tuple[float, float], dict[str, str]]):
+        for (val, unc), fmt_dict in cases_dict.items():
+            for format_spec, expected_str in fmt_dict.items():
+                vunum = vufloat(val, unc)
+                vunum_str = f'{vunum:{format_spec}}'
+                with self.subTest(val=val, unc=unc, format_spec=format_spec,
+                                  expected_str=expected_str,
+                                  actual_str=vunum_str):
+                    self.assertEqual(vunum_str, expected_str)
+
     def test_fixed_point(self):
         cases_dict: dict[float, dict[str, str]] = {
             123.456: {
                 'f': '123.456',
                 '.-3f': '0',
                 '.-2f': '100',
                 '.-1f': '120',
@@ -358,14 +264,69 @@
                 '!5r': '999.99e+00',
                 '!6r': '999.990e+00'
             }
         }
 
         self.do_test_case_dict(cases_dict)
 
+    def test_zero(self):
+        cases_dict = {
+            0: {
+                '': '0',
+                'f': '0',
+                'e': '0e+00',
+                'r': '0e+00',
+                '#r': '0e+00',
+                '.3': '0.000',
+                '.3f': '0.000',
+                '.3e': '0.000e+00',
+                '.3r': '0.000e+00',
+                '#.3r': '0.000e+00',
+                '!3': '0.00',
+                '!3f': '0.00',
+                '!3e': '0.00e+00',
+                '!3r': '0.00e+00',
+                '#!3r': '0.00e+00',
+                '0=2.3': '000.000',
+                '0=2.3f': '000.000',
+                '0=2.3e': '000.000e+00',
+                '0=2.3r': '000.000e+00',
+                '0=#2.3r': '000.000e+00',
+                '0=2!3': '000.00',
+                '0=2!3f': '000.00',
+                '0=2!3e': '000.00e+00',
+                '0=2!3r': '000.00e+00',
+                '0=#2!3r': '000.00e+00'
+            }
+        }
+        self.do_test_case_dict(cases_dict)
+
+    def test_non_finite(self):
+        cases_dict = {
+            float('nan'): {
+                '': 'nan',
+                'f': 'nan',
+                'F': 'NAN',
+                'E': 'NAN'
+            },
+            float('inf'): {
+                '': 'inf',
+                'f': 'inf',
+                'F': 'INF',
+                'E': 'INF'
+            },
+            float('-inf'): {
+                '': '-inf',
+                'f': '-inf',
+                'F': '-INF',
+                'E': '-INF'
+            }
+        }
+        self.do_test_case_dict(cases_dict)
+
     def test_separators(self):
         cases_dict: dict[float, dict[str, str]] = {
             123456.654321: {
                 '': '123456.654321',
                 ',': '123,456.654321',
                 ',.s': '123,456.654 321',
                 ',._': '123,456.654_321',
@@ -392,14 +353,75 @@
                 '_,_': '12_345,543_21',
                 's,s': '12 345,543 21',
             }
         }
 
         self.do_test_case_dict(cases_dict)
 
+    def test_signs(self):
+        cases_dict: dict[float, dict[str, str]] = {
+            +1: {
+                '': '1',
+                '-': '1',
+                '+': '+1',
+                ' ': ' 1'
+            },
+            -1: {
+                '': '-1',
+                '-': '-1',
+                '+': '-1',
+                ' ': '-1'
+            },
+            +0.0: {
+                '': '0',
+                '-': '0',
+                '+': '+0',
+                ' ': ' 0'
+            },
+            -0.0: {
+                '': '0',
+                '-': '0',
+                '+': '+0',
+                ' ': ' 0'
+            }
+        }
+
+        self.do_test_case_dict(cases_dict)
+
+    def test_capitalization(self):
+        cases_dict: dict[float, dict[str, str]] = {
+            16180.33: {
+                'e': '1.618033e+04',
+                'E': '1.618033E+04',
+                'r': '16.18033e+03',
+                'R': '16.18033E+03'
+            },
+            1024: {
+                '!3b': '1.00b+10',
+                '!3B': '1.00B+10'
+            }
+        }
+
+        self.do_test_case_dict(cases_dict)
+
+    def test_padding(self):
+        cases_dict: dict[float, dict[str, str]] = {
+            12: {
+                '': '12',
+                '4': '   12',
+                '4!3e': '    1.20e+01',
+                ' =4': '   12',
+                ' =4!3e': '    1.20e+01',
+                '0=4': '00012',
+                '0=4!3e': '00001.20e+01'
+            }
+        }
+
+        self.do_test_case_dict(cases_dict)
+
     def test_prefix(self):
         cases_dict: dict[float, dict[str, str]] = {
             3.1415e-30: {'ep': '3.1415 q'},
             3.1415e-29: {'ep': '3.1415e-29'},
             3.1415e-28: {'ep': '3.1415e-28'},
             3.1415e-27: {'ep': '3.1415 r'},
             3.1415e-26: {'ep': '3.1415e-26'},
@@ -480,15 +502,15 @@
         self.assertEqual(before_str, expected_before_str)
         self.assertEqual(during_str, expected_during_str)
         self.assertEqual(after_str, expected_before_str)
 
     def test_c_prefix(self):
         num = sfloat(123.456)
         with GlobalDefaultsContext(include_c=True):
-            num_str = f'{num:e-2p}'
+            num_str = f'{num:ex-2p}'
 
         expected_num_str = '12345.6 c'
 
         self.assertEqual(num_str, expected_num_str)
 
     def test_small_si_prefixes(self):
         num = sfloat(123.456)
@@ -496,16 +518,22 @@
         cases_dict = {-2: '12345.6 c',
                       -1: '1234.56 d',
                       +1: '12.3456 da',
                       +2: '1.23456 h'}
 
         with GlobalDefaultsContext(include_small_si_prefixes=True):
             for exp, expected_num_str in cases_dict.items():
-                num_str = f'{num:e{exp:+02}p}'
+                num_str = f'{num:ex{exp:+}p}'
                 self.assertEqual(num_str, expected_num_str)
 
-    def test_format(self):
-        self.do_test_case_dict(fmtcases)
+    def test_val_unc_rounding(self):
+        cases_dict = {
+            (0.0999, 0.0999): {
+                '!1e': '(1 +/- 1)e-01'},
+            (0.0999, 0.999): {
+                '!1e': '(0 +/- 1)e+00'}
+        }
+        self.do_unc_val_test_case_dict(cases_dict)
 
 
 if __name__ == '__main__':
     unittest.main()
```


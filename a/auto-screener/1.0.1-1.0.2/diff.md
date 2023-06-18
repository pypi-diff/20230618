# Comparing `tmp/auto-screener-1.0.1.tar.gz` & `tmp/auto-screener-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-1.0.1.tar", last modified: Sat Jun 17 15:20:49 2023, max compression
+gzip compressed data, was "auto-screener-1.0.2.tar", last modified: Sun Jun 18 16:06:35 2023, max compression
```

## Comparing `auto-screener-1.0.1.tar` & `auto-screener-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:20:49.423827 auto-screener-1.0.1/
--rw-rw-rw-   0        0        0       98 2023-06-17 15:20:49.000000 auto-screener-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-06-17 15:20:49.423827 auto-screener-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 15:20:49.418827 auto-screener-1.0.1/auto_screener/
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-1.0.1/auto_screener/base.py
--rw-rw-rw-   0        0        0    17321 2023-06-17 15:18:59.000000 auto-screener-1.0.1/auto_screener/collect.py
--rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-1.0.1/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-1.0.1/auto_screener/document.py
--rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-1.0.1/auto_screener/exchanges.py
--rw-rw-rw-   0        0        0    26654 2023-06-17 10:31:17.000000 auto-screener-1.0.1/auto_screener/feed.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-1.0.1/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-1.0.1/auto_screener/interval.py
--rw-rw-rw-   0        0        0    33713 2023-06-17 15:16:47.000000 auto-screener-1.0.1/auto_screener/screener.py
--rw-rw-rw-   0        0        0    32231 2023-06-17 15:14:52.000000 auto-screener-1.0.1/auto_screener/screening.py
--rw-rw-rw-   0        0        0    10070 2023-06-17 15:16:53.000000 auto-screener-1.0.1/auto_screener/symbols.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:20:49.422825 auto-screener-1.0.1/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-17 15:20:49.000000 auto-screener-1.0.1/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-06-17 15:20:49.000000 auto-screener-1.0.1/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:20:49.000000 auto-screener-1.0.1/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-06-17 15:20:49.000000 auto-screener-1.0.1/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-17 15:20:49.000000 auto-screener-1.0.1/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-1.0.1/build.py
--rw-rw-rw-   0        0        0      645 2023-06-17 15:20:49.000000 auto-screener-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       79 2023-06-17 10:23:38.000000 auto-screener-1.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       70 2023-06-17 10:23:38.000000 auto-screener-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 15:20:49.423827 auto-screener-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1564 2023-06-17 15:17:04.000000 auto-screener-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:06:35.272418 auto-screener-1.0.2/
+-rw-rw-rw-   0        0        0       98 2023-06-18 16:06:35.000000 auto-screener-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-06-18 16:06:35.272418 auto-screener-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 16:06:35.267418 auto-screener-1.0.2/auto_screener/
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-1.0.2/auto_screener/base.py
+-rw-rw-rw-   0        0        0    17321 2023-06-17 15:18:59.000000 auto-screener-1.0.2/auto_screener/collect.py
+-rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-1.0.2/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-1.0.2/auto_screener/document.py
+-rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-1.0.2/auto_screener/exchanges.py
+-rw-rw-rw-   0        0        0    26655 2023-06-18 16:06:18.000000 auto-screener-1.0.2/auto_screener/feed.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-1.0.2/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-1.0.2/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    33713 2023-06-17 15:16:47.000000 auto-screener-1.0.2/auto_screener/screener.py
+-rw-rw-rw-   0        0        0    32231 2023-06-17 15:14:52.000000 auto-screener-1.0.2/auto_screener/screening.py
+-rw-rw-rw-   0        0        0    11992 2023-06-18 16:06:04.000000 auto-screener-1.0.2/auto_screener/symbols.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:06:35.271418 auto-screener-1.0.2/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-18 16:06:35.000000 auto-screener-1.0.2/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-1.0.2/build.py
+-rw-rw-rw-   0        0        0      645 2023-06-18 16:06:35.000000 auto-screener-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       79 2023-06-17 10:23:38.000000 auto-screener-1.0.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       70 2023-06-17 10:23:38.000000 auto-screener-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:06:35.272418 auto-screener-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-06-18 16:06:25.000000 auto-screener-1.0.2/setup.py
```

### Comparing `auto-screener-1.0.1/PKG-INFO` & `auto-screener-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 1.0.1
+Version: 1.0.2
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-1.0.1/README.md` & `auto-screener-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/auto_screener/base.py` & `auto-screener-1.0.2/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/auto_screener/collect.py` & `auto-screener-1.0.2/auto_screener/collect.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/auto_screener/dataset.py` & `auto-screener-1.0.2/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/auto_screener/document.py` & `auto-screener-1.0.2/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/auto_screener/feed.py` & `auto-screener-1.0.2/auto_screener/feed.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,15 @@
     __slots__ = (
         "handler", "recorder", "updating",
         "update_process", "loop", "limited",
         "feeds_parameters", "screening_parameters"
     )
 
     DELAY = 10
-    AMOUNT = 5
+    AMOUNT = 50
 
     REFRESH = dt.timedelta(minutes=5)
 
     screeners: List[OrderBookScreener]
     recorder: MarketOrderBookRecorder
 
     COLUMNS = MarketOrderBookRecorder.COLUMNS
```

### Comparing `auto-screener-1.0.1/auto_screener/interval.py` & `auto-screener-1.0.2/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/auto_screener/screener.py` & `auto-screener-1.0.2/auto_screener/screener.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/auto_screener/screening.py` & `auto-screener-1.0.2/auto_screener/screening.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/auto_screener/symbols.py` & `auto-screener-1.0.2/auto_screener/symbols.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     "parts_to_pair",
     "pair_to_parts",
     "symbols_to_parts",
     "parts_to_symbol_parts",
     "parts_to_symbol_parts",
     "assets_to_symbols",
     "parts_to_symbols",
-    "Separator"
+    "Separator",
+    "filter_symbols",
+    "keep_symbols"
 ]
 
 class Separator:
     """A class to contain the separator value."""
 
     value = "/"
 # end Separator
@@ -411,8 +413,86 @@
             if base != quote and reverse_symbol(ticker) not in tickers:
                 tickers.append(ticker)
             # end if
         # end for
     # end for
 
     return tickers
-# end assets_to_symbols
+# end assets_to_symbols
+
+def keep_symbols(
+        symbols: Iterable[str],
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        included: Optional[Iterable[str]] = None
+) -> List[str]:
+    """
+    Removes all symbols with not matching base or quote.
+
+    :param symbols: The symbols to filter.
+    :param bases: The bases to include.
+    :param quotes: The quotes to include.
+    :param included: The symbols to include.
+
+    :return: The filtered symbols.
+    """
+
+    saved = []
+
+    quotes = quotes or []
+    bases = bases or []
+    excluded = included or []
+
+    for symbol in symbols:
+        if symbol in excluded:
+            saved.append(symbol)
+        # end if
+
+        base, quote = symbol_to_parts(symbol)
+
+        if (base in bases) or (quote in quotes):
+            saved.append(symbol)
+        # end if
+    # end for
+
+    return saved
+# end keep_symbols
+
+def filter_symbols(
+        symbols: Iterable[str],
+        bases: Optional[Iterable[str]] = None,
+        quotes: Optional[Iterable[str]] = None,
+        excluded: Optional[Iterable[str]] = None
+) -> List[str]:
+    """
+    Removes all symbols with the matching base or quote.
+
+    :param symbols: The symbols to filter.
+    :param bases: The bases to exclude.
+    :param quotes: The quotes to exclude.
+    :param excluded: The symbols to exclude.
+
+    :return: The filtered symbols.
+    """
+
+    saved = []
+
+    quotes = quotes or []
+    bases = bases or []
+    excluded = excluded or []
+
+    for symbol in symbols:
+        if symbol in excluded:
+            continue
+        # end if
+
+        base, quote = symbol_to_parts(symbol)
+
+        if (base in bases) or (quote in quotes):
+            continue
+        # end if
+
+        saved.append(symbol)
+    # end for
+
+    return saved
+# end filter_symbols
```

### Comparing `auto-screener-1.0.1/auto_screener.egg-info/PKG-INFO` & `auto-screener-1.0.2/auto_screener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 1.0.1
+Version: 1.0.2
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-1.0.1/auto_screener.egg-info/SOURCES.txt` & `auto-screener-1.0.2/auto_screener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/build.py` & `auto-screener-1.0.2/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-1.0.1/pyproject.toml` & `auto-screener-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '1.0.1'
+version = '1.0.2'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-1.0.1/setup.py` & `auto-screener-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='1.0.1',
+        version='1.0.2',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```


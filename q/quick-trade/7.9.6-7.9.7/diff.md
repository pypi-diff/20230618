# Comparing `tmp/quick_trade-7.9.6.tar.gz` & `tmp/quick_trade-7.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_trade-7.9.6.tar", last modified: Fri Mar 10 10:57:56 2023, max compression
+gzip compressed data, was "quick_trade-7.9.7.tar", last modified: Sat Jun 17 23:28:35 2023, max compression
```

## Comparing `quick_trade-7.9.6.tar` & `quick_trade-7.9.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-10 10:57:56.758971 quick_trade-7.9.6/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-03-09 01:24:21.000000 quick_trade-7.9.6/LICENSE.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9837 2023-03-10 10:57:56.758971 quick_trade-7.9.6/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8725 2023-03-09 02:04:24.000000 quick_trade-7.9.6/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-10 10:57:56.758971 quick_trade-7.9.6/quick_trade/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      125 2023-03-09 17:09:54.000000 quick_trade-7.9.6/quick_trade/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      603 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/_code_inspect.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1731 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/_saving.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     4405 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/brokers.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     6495 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/indicators.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    11916 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/plots.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    82173 2023-03-09 02:30:55.000000 quick_trade-7.9.6/quick_trade/trading_sys.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-10 10:57:56.758971 quick_trade-7.9.6/quick_trade/tuner/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1413 2023-03-09 17:08:43.000000 quick_trade-7.9.6/quick_trade/tuner/__init__.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-10 10:57:56.758971 quick_trade-7.9.6/quick_trade/tuner/avoid_overfitting/
--rw-r--r--   0 vlad      (1000) vlad      (1000)       86 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/tuner/avoid_overfitting/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5046 2023-03-10 10:55:44.000000 quick_trade-7.9.6/quick_trade/tuner/avoid_overfitting/validation_analysis.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    10336 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/tuner/avoid_overfitting/volatility.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     7912 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/tuner/avoid_overfitting/walkforward.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1856 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/tuner/core.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8350 2023-03-09 01:24:21.000000 quick_trade-7.9.6/quick_trade/tuner/tuner.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    17938 2023-03-10 10:56:22.000000 quick_trade-7.9.6/quick_trade/utils.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-10 10:57:56.758971 quick_trade-7.9.6/quick_trade.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     9837 2023-03-10 10:57:56.000000 quick_trade-7.9.6/quick_trade.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      688 2023-03-10 10:57:56.000000 quick_trade-7.9.6/quick_trade.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-10 10:57:56.000000 quick_trade-7.9.6/quick_trade.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       93 2023-03-10 10:57:56.000000 quick_trade-7.9.6/quick_trade.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       12 2023-03-10 10:57:56.000000 quick_trade-7.9.6/quick_trade.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-03-10 10:57:56.758971 quick_trade-7.9.6/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1723 2023-03-10 10:56:29.000000 quick_trade-7.9.6/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-17 23:28:35.577911 quick_trade-7.9.7/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-03-09 01:24:21.000000 quick_trade-7.9.7/LICENSE.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9837 2023-06-17 23:28:35.577911 quick_trade-7.9.7/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8725 2023-03-09 02:04:24.000000 quick_trade-7.9.7/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-17 23:28:35.574578 quick_trade-7.9.7/quick_trade/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      125 2023-03-09 17:09:54.000000 quick_trade-7.9.7/quick_trade/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      603 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/_code_inspect.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1731 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/_saving.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4405 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/brokers.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6498 2023-06-17 22:53:28.000000 quick_trade-7.9.7/quick_trade/indicators.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11916 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/plots.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    82173 2023-03-09 02:30:55.000000 quick_trade-7.9.7/quick_trade/trading_sys.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-17 23:28:35.574578 quick_trade-7.9.7/quick_trade/tuner/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1413 2023-03-09 17:08:43.000000 quick_trade-7.9.7/quick_trade/tuner/__init__.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-17 23:28:35.577911 quick_trade-7.9.7/quick_trade/tuner/avoid_overfitting/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       86 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/tuner/avoid_overfitting/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5046 2023-03-10 10:55:44.000000 quick_trade-7.9.7/quick_trade/tuner/avoid_overfitting/validation_analysis.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10336 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/tuner/avoid_overfitting/volatility.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7912 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/tuner/avoid_overfitting/walkforward.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1856 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/tuner/core.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8350 2023-03-09 01:24:21.000000 quick_trade-7.9.7/quick_trade/tuner/tuner.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17938 2023-06-17 22:58:39.000000 quick_trade-7.9.7/quick_trade/utils.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-06-17 23:28:35.574578 quick_trade-7.9.7/quick_trade.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9837 2023-06-17 23:28:35.000000 quick_trade-7.9.7/quick_trade.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      688 2023-06-17 23:28:35.000000 quick_trade-7.9.7/quick_trade.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-06-17 23:28:35.000000 quick_trade-7.9.7/quick_trade.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       93 2023-06-17 23:28:35.000000 quick_trade-7.9.7/quick_trade.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       12 2023-06-17 23:28:35.000000 quick_trade-7.9.7/quick_trade.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-06-17 23:28:35.577911 quick_trade-7.9.7/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1723 2023-06-17 22:58:02.000000 quick_trade-7.9.7/setup.py
```

### Comparing `quick_trade-7.9.6/LICENSE.md` & `quick_trade-7.9.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/PKG-INFO` & `quick_trade-7.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: quick_trade
-Version: 7.9.6
+Version: 7.9.7
 Summary: Library for easy management and customization of algorithmic trading.
-Download-URL: https://github.com/quick-trade/quick_trade/archive/7.9.6.tar.gz
+Download-URL: https://github.com/quick-trade/quick_trade/archive/7.9.7.tar.gz
 Author: Vlad Kochetov
 Author-email: vladyslavdrrragonkoch@gmail.com
 License: cc-by-sa-4.0
 Project-URL: Documentation, https://quick-trade.github.io/quick_trade/#/
 Project-URL: Source, https://github.com/quick-trade/quick_trade
 Project-URL: Twitter, https://twitter.com/quick_trade_tw
 Project-URL: Bug Tracker, https://github.com/quick-trade/quick_trade/issues
```

### Comparing `quick_trade-7.9.6/README.md` & `quick_trade-7.9.7/README.md`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/_code_inspect.py` & `quick_trade-7.9.7/quick_trade/_code_inspect.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/_saving.py` & `quick_trade-7.9.7/quick_trade/_saving.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/brokers.py` & `quick_trade-7.9.7/quick_trade/brokers.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/indicators.py` & `quick_trade-7.9.7/quick_trade/indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             else:
                 dir_[i] = dir_[i - 1]
                 if dir_[i] == BUY and lowerband.iloc[i] < lowerband.iloc[i - 1]:
                     lowerband.iloc[i] = lowerband.iloc[i - 1]
                 if dir_[i] == SELL and upperband.iloc[i] > upperband.iloc[i - 1]:
                     upperband.iloc[i] = upperband.iloc[i - 1]
 
-            if dir_[i] > 0:
+            if dir_[i] == BUY:
                 trend[i] = long[i] = lowerband.iloc[i]
             else:
                 trend[i] = short[i] = upperband.iloc[i]
 
         df = DataFrame(
             {
                 f"ST": trend,
```

### Comparing `quick_trade-7.9.6/quick_trade/plots.py` & `quick_trade-7.9.7/quick_trade/plots.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/trading_sys.py` & `quick_trade-7.9.7/quick_trade/trading_sys.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/tuner/__init__.py` & `quick_trade-7.9.7/quick_trade/tuner/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/tuner/avoid_overfitting/validation_analysis.py` & `quick_trade-7.9.7/quick_trade/tuner/avoid_overfitting/validation_analysis.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/tuner/avoid_overfitting/volatility.py` & `quick_trade-7.9.7/quick_trade/tuner/avoid_overfitting/volatility.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/tuner/avoid_overfitting/walkforward.py` & `quick_trade-7.9.7/quick_trade/tuner/avoid_overfitting/walkforward.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/tuner/core.py` & `quick_trade-7.9.7/quick_trade/tuner/core.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/tuner/tuner.py` & `quick_trade-7.9.7/quick_trade/tuner/tuner.py`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/quick_trade/utils.py` & `quick_trade-7.9.7/quick_trade/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 mean deviation: {}%
 Sharpe ratio: {}
 Sortino ratio: {}
 calmar ratio: {}
 max drawdown: {}%
 profit/deviation ratio: {}"""  # .format(Trader.losses, Trader.trades, ...)
 
-__version__: str = "7.9.6"
+__version__: str = "7.9.7"
 __author__: str = 'Vlad Kochetov'
 __credits__: List[str] = [
     "Hemerson Tacon -- Stack overflow",
     "hpaulj -- Stack overflow",
     "furas -- Stack overflow",
     "Devin Jeanpierre (edit: wjandrea) -- Stack overflow",
     "Voitenko Mykola Polikarpovich -- helped me test the system of interaction with the binance crypto exchange",
```

### Comparing `quick_trade-7.9.6/quick_trade.egg-info/PKG-INFO` & `quick_trade-7.9.7/quick_trade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: quick-trade
-Version: 7.9.6
+Version: 7.9.7
 Summary: Library for easy management and customization of algorithmic trading.
-Download-URL: https://github.com/quick-trade/quick_trade/archive/7.9.6.tar.gz
+Download-URL: https://github.com/quick-trade/quick_trade/archive/7.9.7.tar.gz
 Author: Vlad Kochetov
 Author-email: vladyslavdrrragonkoch@gmail.com
 License: cc-by-sa-4.0
 Project-URL: Documentation, https://quick-trade.github.io/quick_trade/#/
 Project-URL: Source, https://github.com/quick-trade/quick_trade
 Project-URL: Twitter, https://twitter.com/quick_trade_tw
 Project-URL: Bug Tracker, https://github.com/quick-trade/quick_trade/issues
```

### Comparing `quick_trade-7.9.6/quick_trade.egg-info/SOURCES.txt` & `quick_trade-7.9.7/quick_trade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quick_trade-7.9.6/setup.py` & `quick_trade-7.9.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 from distutils.core import setup
 
 
 with open('README.md') as file:
     long_desc = file.read()
 
-__version__ = "7.9.6"
+__version__ = "7.9.7"
 
 setup(
     name='quick_trade',
     author="Vlad Kochetov",
     author_email='vladyslavdrrragonkoch@gmail.com',
     packages=find_packages(),
     version=__version__,
@@ -20,20 +20,20 @@
     project_urls={
         'Documentation': 'https://quick-trade.github.io/quick_trade/#/',
         'Source': 'https://github.com/quick-trade/quick_trade',
         'Twitter': 'https://twitter.com/quick_trade_tw',
         'Bug Tracker': 'https://github.com/quick-trade/quick_trade/issues'
     },
     install_requires=[
-        'numpy==1.24.1',
-        'plotly==5.12.0',
-        'pandas==1.5.2',
+        'numpy==1.24.3',
+        'plotly==5.15.0',
+        'pandas==2.0.2',
         'ta==0.10.2',
-        'tqdm==4.64.1',
-        'ccxt==2.7.37',
+        'ccxt==3.1.41',
+        'tqdm==4.65.0',
         'scikit-learn',
     ],
     download_url=f'https://github.com/quick-trade/quick_trade/archive/{__version__}.tar.gz',
     keywords=[
         'technical-analysis',
         'python3',
         'trading',
```


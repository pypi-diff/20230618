# Comparing `tmp/zeroconf-0.68.0.tar.gz` & `tmp/zeroconf-0.68.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.68.0.tar", max compression
+gzip compressed data, was "zeroconf-0.68.1.tar", max compression
```

## Comparing `zeroconf-0.68.0.tar` & `zeroconf-0.68.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    53605 2023-06-17 18:52:40.372809 zeroconf-0.68.0/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-06-17 18:52:39.584798 zeroconf-0.68.0/COPYING
--rw-r--r--   0        0        0     4407 2023-06-17 18:52:39.584798 zeroconf-0.68.0/README.rst
--rw-r--r--   0        0        0     1060 2023-06-17 18:52:39.584798 zeroconf-0.68.0/build_ext.py
--rw-r--r--   0        0        0     6770 2023-06-17 18:52:39.584798 zeroconf-0.68.0/docs/Makefile
--rw-r--r--   0        0        0      234 2023-06-17 18:52:39.584798 zeroconf-0.68.0/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-06-17 18:52:39.584798 zeroconf-0.68.0/docs/conf.py
--rw-r--r--   0        0        0      991 2023-06-17 18:52:39.584798 zeroconf-0.68.0/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-06-17 18:52:40.444810 zeroconf-0.68.0/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-06-17 18:52:40.380809 zeroconf-0.68.0/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      897 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0    10036 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39337 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2119 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18270 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    24697 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2661 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    14335 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     2317 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17871 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2355 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    22413 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    27259 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3948 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4515 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-06-17 18:52:39.588798 zeroconf-0.68.0/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-06-17 18:52:39.588798 zeroconf-0.68.0/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-17 18:52:39.588798 zeroconf-0.68.0/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-06-17 18:52:39.588798 zeroconf-0.68.0/tests/services/__init__.py
--rw-r--r--   0        0        0    42949 2023-06-17 18:52:39.588798 zeroconf-0.68.0/tests/services/test_browser.py
--rw-r--r--   0        0        0    45240 2023-06-17 18:52:39.588798 zeroconf-0.68.0/tests/services/test_info.py
--rw-r--r--   0        0        0     4157 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/services/test_registry.py
--rw-r--r--   0        0        0     4681 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/services/test_types.py
--rw-r--r--   0        0        0    44525 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_cache.py
--rw-r--r--   0        0        0    32162 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_dns.py
--rw-r--r--   0        0        0     5021 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_exceptions.py
--rw-r--r--   0        0        0    67411 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_protocol.py
--rw-r--r--   0        0        0     8849 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-06-17 18:52:39.592798 zeroconf-0.68.0/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.68.0/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.68.0/PKG-INFO
+-rw-r--r--   0        0        0    53906 2023-06-18 20:28:21.097738 zeroconf-0.68.1/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-06-18 20:28:19.901724 zeroconf-0.68.1/COPYING
+-rw-r--r--   0        0        0     4407 2023-06-18 20:28:19.901724 zeroconf-0.68.1/README.rst
+-rw-r--r--   0        0        0     1060 2023-06-18 20:28:19.901724 zeroconf-0.68.1/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-06-18 20:28:19.901724 zeroconf-0.68.1/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-06-18 20:28:19.901724 zeroconf-0.68.1/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-06-18 20:28:19.901724 zeroconf-0.68.1/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-06-18 20:28:19.901724 zeroconf-0.68.1/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-06-18 20:28:21.201739 zeroconf-0.68.1/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-06-18 20:28:21.109738 zeroconf-0.68.1/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-18 20:28:19.901724 zeroconf-0.68.1/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0    10036 2023-06-18 20:28:19.901724 zeroconf-0.68.1/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39409 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2119 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18270 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    24697 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2661 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    14335 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     2317 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17871 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2355 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    22413 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    27259 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3948 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4515 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-06-18 20:28:19.905724 zeroconf-0.68.1/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-18 20:28:19.905724 zeroconf-0.68.1/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-06-18 20:28:19.905724 zeroconf-0.68.1/tests/services/__init__.py
+-rw-r--r--   0        0        0    42949 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/services/test_browser.py
+-rw-r--r--   0        0        0    45240 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/services/test_registry.py
+-rw-r--r--   0        0        0     4681 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/services/test_types.py
+-rw-r--r--   0        0        0    44525 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_cache.py
+-rw-r--r--   0        0        0    32599 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_dns.py
+-rw-r--r--   0        0        0     5021 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67411 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_protocol.py
+-rw-r--r--   0        0        0     8849 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.68.1/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.68.1/PKG-INFO
```

### Comparing `zeroconf-0.68.0/CHANGELOG.md` & `zeroconf-0.68.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.68.1 (2023-06-18)
+
+### Fix
+
+* Reduce debug logging overhead by adding missing checks to datagram_received ([#1188](https://github.com/python-zeroconf/python-zeroconf/issues/1188)) ([`ac5c50a`](https://github.com/python-zeroconf/python-zeroconf/commit/ac5c50afc70aaa33fcd20bf02222ff4f0c596fa3))
+
 ## v0.68.0 (2023-06-17)
 
 ### Feature
 
 * Reduce overhead to handle queries and responses ([#1184](https://github.com/python-zeroconf/python-zeroconf/issues/1184)) ([`81126b7`](https://github.com/python-zeroconf/python-zeroconf/commit/81126b7600f94848ef8c58b70bac0c6ab993c6ae))
 
 ## v0.67.0 (2023-06-17)
```

### Comparing `zeroconf-0.68.0/COPYING` & `zeroconf-0.68.1/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/README.rst` & `zeroconf-0.68.1/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/build_ext.py` & `zeroconf-0.68.1/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/docs/Makefile` & `zeroconf-0.68.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/docs/conf.py` & `zeroconf-0.68.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/docs/index.rst` & `zeroconf-0.68.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/pyproject.toml` & `zeroconf-0.68.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.68.0"
+version = "0.68.1"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.68.0/src/zeroconf/__init__.py` & `zeroconf-0.68.1/src/zeroconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.68.0'
+__version__ = '0.68.1'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.68.0/src/zeroconf/_cache.pxd` & `zeroconf-0.68.1/src/zeroconf/_cache.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_cache.py` & `zeroconf-0.68.1/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_core.py` & `zeroconf-0.68.1/src/zeroconf/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,26 +278,28 @@
         if len(addrs) == 2:
             # https://github.com/python/mypy/issues/1178
             addr, port = addrs  # type: ignore
             scope = None
         else:
             # https://github.com/python/mypy/issues/1178
             addr, port, flow, scope = addrs  # type: ignore
-            log.debug('IPv6 scope_id %d associated to the receiving interface', scope)
+            if debug:
+                log.debug('IPv6 scope_id %d associated to the receiving interface', scope)
             v6_flow_scope = (flow, scope)
 
         if data_len > _MAX_MSG_ABSOLUTE:
             # Guard against oversized packets to ensure bad implementations cannot overwhelm
             # the system.
-            log.debug(
-                "Discarding incoming packet with length %s, which is larger "
-                "than the absolute maximum size of %s",
-                data_len,
-                _MAX_MSG_ABSOLUTE,
-            )
+            if debug:
+                log.debug(
+                    "Discarding incoming packet with length %s, which is larger "
+                    "than the absolute maximum size of %s",
+                    data_len,
+                    _MAX_MSG_ABSOLUTE,
+                )
             return
 
         now = current_time_millis()
         if (
             self.data == data
             and (now - _DUPLICATE_PACKET_SUPPRESSION_INTERVAL) < self.last_time
             and self.last_message is not None
```

### Comparing `zeroconf-0.68.0/src/zeroconf/_dns.pxd` & `zeroconf-0.68.1/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_dns.py` & `zeroconf-0.68.1/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_exceptions.py` & `zeroconf-0.68.1/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_handlers.py` & `zeroconf-0.68.1/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_history.py` & `zeroconf-0.68.1/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_logger.py` & `zeroconf-0.68.1/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.68.1/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.68.1/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.68.1/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.68.1/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.68.1/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_services/__init__.py` & `zeroconf-0.68.1/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_services/browser.py` & `zeroconf-0.68.1/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_services/info.py` & `zeroconf-0.68.1/src/zeroconf/_services/info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_services/registry.py` & `zeroconf-0.68.1/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_services/types.py` & `zeroconf-0.68.1/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_updates.py` & `zeroconf-0.68.1/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_utils/__init__.py` & `zeroconf-0.68.1/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.68.1/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_utils/name.py` & `zeroconf-0.68.1/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_utils/net.py` & `zeroconf-0.68.1/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/_utils/time.py` & `zeroconf-0.68.1/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/asyncio.py` & `zeroconf-0.68.1/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/src/zeroconf/const.py` & `zeroconf-0.68.1/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/__init__.py` & `zeroconf-0.68.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/conftest.py` & `zeroconf-0.68.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/services/__init__.py` & `zeroconf-0.68.1/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/services/test_browser.py` & `zeroconf-0.68.1/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/services/test_info.py` & `zeroconf-0.68.1/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/services/test_registry.py` & `zeroconf-0.68.1/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/services/test_types.py` & `zeroconf-0.68.1/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_asyncio.py` & `zeroconf-0.68.1/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_cache.py` & `zeroconf-0.68.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_core.py` & `zeroconf-0.68.1/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -757,14 +757,30 @@
                 500,
                 b'path=/~paulsm/',
             )
         )
         is None
     )
 
+    logging.getLogger('zeroconf').setLevel(logging.INFO)
+
+    listener.datagram_received(over_sized_packet, ('::1', const._MDNS_PORT, 1, 1))
+    assert (
+        zc.cache.async_get_unique(
+            r.DNSText(
+                "packet0.local.",
+                const._TYPE_TXT,
+                const._CLASS_IN | const._CLASS_UNIQUE,
+                500,
+                b'path=/~paulsm/',
+            )
+        )
+        is None
+    )
+
     zc.close()
 
 
 def test_guard_against_duplicate_packets():
     """Ensure we do not process duplicate packets.
     These packets can quickly overwhelm the system.
     """
```

### Comparing `zeroconf-0.68.0/tests/test_dns.py` & `zeroconf-0.68.1/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_exceptions.py` & `zeroconf-0.68.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_handlers.py` & `zeroconf-0.68.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_history.py` & `zeroconf-0.68.1/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_init.py` & `zeroconf-0.68.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_logger.py` & `zeroconf-0.68.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_protocol.py` & `zeroconf-0.68.1/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_services.py` & `zeroconf-0.68.1/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/test_updates.py` & `zeroconf-0.68.1/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/utils/__init__.py` & `zeroconf-0.68.1/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/utils/test_asyncio.py` & `zeroconf-0.68.1/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/utils/test_name.py` & `zeroconf-0.68.1/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/tests/utils/test_net.py` & `zeroconf-0.68.1/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.0/setup.py` & `zeroconf-0.68.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.68.0',
+    'version': '0.68.1',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.68.0/PKG-INFO` & `zeroconf-0.68.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.68.0
+Version: 0.68.1
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


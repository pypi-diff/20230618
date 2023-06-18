# Comparing `tmp/zeroconf-0.68.1.tar.gz` & `tmp/zeroconf-0.69.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.68.1.tar", max compression
+gzip compressed data, was "zeroconf-0.69.0.tar", max compression
```

## Comparing `zeroconf-0.68.1.tar` & `zeroconf-0.69.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    53906 2023-06-18 20:28:21.097738 zeroconf-0.68.1/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-06-18 20:28:19.901724 zeroconf-0.68.1/COPYING
--rw-r--r--   0        0        0     4407 2023-06-18 20:28:19.901724 zeroconf-0.68.1/README.rst
--rw-r--r--   0        0        0     1060 2023-06-18 20:28:19.901724 zeroconf-0.68.1/build_ext.py
--rw-r--r--   0        0        0     6770 2023-06-18 20:28:19.901724 zeroconf-0.68.1/docs/Makefile
--rw-r--r--   0        0        0      234 2023-06-18 20:28:19.901724 zeroconf-0.68.1/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-06-18 20:28:19.901724 zeroconf-0.68.1/docs/conf.py
--rw-r--r--   0        0        0      991 2023-06-18 20:28:19.901724 zeroconf-0.68.1/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-06-18 20:28:21.201739 zeroconf-0.68.1/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-06-18 20:28:21.109738 zeroconf-0.68.1/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      897 2023-06-18 20:28:19.901724 zeroconf-0.68.1/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0    10036 2023-06-18 20:28:19.901724 zeroconf-0.68.1/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39409 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2119 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18270 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    24697 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2661 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    14335 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     2317 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17871 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2355 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    22413 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    27259 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3948 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4515 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-06-18 20:28:19.905724 zeroconf-0.68.1/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-06-18 20:28:19.905724 zeroconf-0.68.1/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-18 20:28:19.905724 zeroconf-0.68.1/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-06-18 20:28:19.905724 zeroconf-0.68.1/tests/services/__init__.py
--rw-r--r--   0        0        0    42949 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/services/test_browser.py
--rw-r--r--   0        0        0    45240 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/services/test_info.py
--rw-r--r--   0        0        0     4157 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/services/test_registry.py
--rw-r--r--   0        0        0     4681 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/services/test_types.py
--rw-r--r--   0        0        0    44525 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_cache.py
--rw-r--r--   0        0        0    32599 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_dns.py
--rw-r--r--   0        0        0     5021 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_exceptions.py
--rw-r--r--   0        0        0    67411 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_protocol.py
--rw-r--r--   0        0        0     8849 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-06-18 20:28:19.909724 zeroconf-0.68.1/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.68.1/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.68.1/PKG-INFO
+-rw-r--r--   0        0        0    54390 2023-06-18 20:43:33.739772 zeroconf-0.69.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-06-18 20:43:32.923760 zeroconf-0.69.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-06-18 20:43:32.927760 zeroconf-0.69.0/README.rst
+-rw-r--r--   0        0        0     1060 2023-06-18 20:43:32.927760 zeroconf-0.69.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-06-18 20:43:32.927760 zeroconf-0.69.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-06-18 20:43:32.927760 zeroconf-0.69.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-06-18 20:43:32.927760 zeroconf-0.69.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-06-18 20:43:32.927760 zeroconf-0.69.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-06-18 20:43:33.819774 zeroconf-0.69.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-06-18 20:43:33.751773 zeroconf-0.69.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0    10040 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39381 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2119 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18270 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    24697 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2661 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    14353 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     2317 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17896 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2355 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    22413 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    27259 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3948 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-06-18 20:43:32.927760 zeroconf-0.69.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-06-18 20:43:32.931760 zeroconf-0.69.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-06-18 20:43:32.931760 zeroconf-0.69.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-06-18 20:43:32.931760 zeroconf-0.69.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4515 2023-06-18 20:43:32.931760 zeroconf-0.69.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-06-18 20:43:32.931760 zeroconf-0.69.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    42949 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    45240 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     4681 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    44525 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_cache.py
+-rw-r--r--   0        0        0    32599 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_dns.py
+-rw-r--r--   0        0        0     5021 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67411 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     8849 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-06-18 20:43:32.931760 zeroconf-0.69.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.69.0/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.69.0/PKG-INFO
```

### Comparing `zeroconf-0.68.1/CHANGELOG.md` & `zeroconf-0.69.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.69.0 (2023-06-18)
+
+### Feature
+
+* Cython3 support ([#1190](https://github.com/python-zeroconf/python-zeroconf/issues/1190)) ([`8ae8ba1`](https://github.com/python-zeroconf/python-zeroconf/commit/8ae8ba1af324b0c8c2da3bd12c264a5c0f3dcc3d))
+* Reorder incoming data handler to reduce overhead ([#1189](https://github.com/python-zeroconf/python-zeroconf/issues/1189)) ([`32756ff`](https://github.com/python-zeroconf/python-zeroconf/commit/32756ff113f675b7a9cf16d3c0ab840ba733e5e4))
+
 ## v0.68.1 (2023-06-18)
 
 ### Fix
 
 * Reduce debug logging overhead by adding missing checks to datagram_received ([#1188](https://github.com/python-zeroconf/python-zeroconf/issues/1188)) ([`ac5c50a`](https://github.com/python-zeroconf/python-zeroconf/commit/ac5c50afc70aaa33fcd20bf02222ff4f0c596fa3))
 
 ## v0.68.0 (2023-06-17)
```

### Comparing `zeroconf-0.68.1/COPYING` & `zeroconf-0.69.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/README.rst` & `zeroconf-0.69.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/build_ext.py` & `zeroconf-0.69.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/docs/Makefile` & `zeroconf-0.69.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/docs/conf.py` & `zeroconf-0.69.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/docs/index.rst` & `zeroconf-0.69.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/pyproject.toml` & `zeroconf-0.69.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.68.1"
+version = "0.69.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.68.1/src/zeroconf/__init__.py` & `zeroconf-0.69.0/src/zeroconf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.68.1'
+__version__ = '0.69.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.68.1/src/zeroconf/_cache.pxd` & `zeroconf-0.69.0/src/zeroconf/_cache.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_cache.py` & `zeroconf-0.69.0/src/zeroconf/_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         """Gets all matching entries by details.
 
         This function is not thread-safe and must be called from
         the event loop.
         """
         return self._async_all_by_details(name, type_, class_)
 
-    def _async_all_by_details(self, name: _str, type_: int, class_: int) -> List[DNSRecord]:
+    def _async_all_by_details(self, name: _str, type_: _int, class_: _int) -> List[DNSRecord]:
         """Gets all matching entries by details.
 
         This function is not thread-safe and must be called from
         the event loop.
         """
         key = name.lower()
         records = self.cache.get(key)
@@ -254,9 +254,9 @@
         for name, type_, class_ in unique_types:
             for record in self._async_all_by_details(name, type_, class_):
                 if (now - record.created > _ONE_SECOND) and record not in answers_rrset:
                     # Expire in 1s
                     record.set_created_ttl(now, 1)
 
 
-def _dns_record_matches(record: _DNSRecord, key: _str, type_: int, class_: int) -> bool:
+def _dns_record_matches(record: _DNSRecord, key: _str, type_: _int, class_: _int) -> bool:
     return key == record.key and type_ == record.type and class_ == record.class_
```

### Comparing `zeroconf-0.68.1/src/zeroconf/_core.py` & `zeroconf-0.69.0/src/zeroconf/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,29 +267,17 @@
         self._timers: Dict[str, asyncio.TimerHandle] = {}
         super().__init__()
 
     def datagram_received(
         self, data: bytes, addrs: Union[Tuple[str, int], Tuple[str, int, int, int]]
     ) -> None:
         assert self.transport is not None
-        v6_flow_scope: Union[Tuple[()], Tuple[int, int]] = ()
         data_len = len(data)
         debug = log.isEnabledFor(logging.DEBUG)
 
-        if len(addrs) == 2:
-            # https://github.com/python/mypy/issues/1178
-            addr, port = addrs  # type: ignore
-            scope = None
-        else:
-            # https://github.com/python/mypy/issues/1178
-            addr, port, flow, scope = addrs  # type: ignore
-            if debug:
-                log.debug('IPv6 scope_id %d associated to the receiving interface', scope)
-            v6_flow_scope = (flow, scope)
-
         if data_len > _MAX_MSG_ABSOLUTE:
             # Guard against oversized packets to ensure bad implementations cannot overwhelm
             # the system.
             if debug:
                 log.debug(
                     "Discarding incoming packet with length %s, which is larger "
                     "than the absolute maximum size of %s",
@@ -304,23 +292,34 @@
             and (now - _DUPLICATE_PACKET_SUPPRESSION_INTERVAL) < self.last_time
             and self.last_message is not None
             and not self.last_message.has_qu_question()
         ):
             # Guard against duplicate packets
             if debug:
                 log.debug(
-                    'Ignoring duplicate message with no unicast questions received from %r:%r [socket %s] (%d bytes) as [%r]',
-                    addr,
-                    port,
+                    'Ignoring duplicate message with no unicast questions received from %s [socket %s] (%d bytes) as [%r]',
+                    addrs,
                     self.sock_description,
                     data_len,
                     data,
                 )
             return
 
+        v6_flow_scope: Union[Tuple[()], Tuple[int, int]] = ()
+        if len(addrs) == 2:
+            # https://github.com/python/mypy/issues/1178
+            addr, port = addrs  # type: ignore
+            scope = None
+        else:
+            # https://github.com/python/mypy/issues/1178
+            addr, port, flow, scope = addrs  # type: ignore
+            if debug:
+                log.debug('IPv6 scope_id %d associated to the receiving interface', scope)
+            v6_flow_scope = (flow, scope)
+
         msg = DNSIncoming(data, (addr, port), scope, now)
         self.data = data
         self.last_time = now
         self.last_message = msg
         if msg.valid:
             if debug:
                 log.debug(
```

### Comparing `zeroconf-0.68.1/src/zeroconf/_dns.pxd` & `zeroconf-0.69.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_dns.py` & `zeroconf-0.69.0/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_exceptions.py` & `zeroconf-0.69.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_handlers.py` & `zeroconf-0.69.0/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_history.py` & `zeroconf-0.69.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_logger.py` & `zeroconf-0.69.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.69.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.69.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.69.0/src/zeroconf/_protocol/incoming.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 UNPACK_3H = struct.Struct(b'!3H').unpack_from
 UNPACK_6H = struct.Struct(b'!6H').unpack_from
 UNPACK_HH = struct.Struct(b'!HH').unpack_from
 UNPACK_HHiH = struct.Struct(b'!HHiH').unpack_from
 
 _seen_logs: Dict[str, Union[int, tuple]] = {}
 _str = str
+_int = int
 
 
 class DNSIncoming:
     """Object representation of an incoming DNS packet"""
 
     __slots__ = (
         "_did_read_others",
@@ -227,15 +228,15 @@
 
     def _read_character_string(self) -> bytes:
         """Reads a character string from the packet"""
         length = self.data[self.offset]
         self.offset += 1
         return self._read_string(length)
 
-    def _read_string(self, length: int) -> bytes:
+    def _read_string(self, length: _int) -> bytes:
         """Reads a string of a given length from the packet"""
         info = self.data[self.offset : self.offset + length]
         self.offset += length
         return info
 
     def _read_others(self) -> None:
         """Reads the answers, authorities and additionals section of the
@@ -263,15 +264,15 @@
                     self.data,
                     exc_info=True,
                 )
             if rec is not None:
                 self._answers.append(rec)
 
     def _read_record(
-        self, domain: _str, type_: int, class_: int, ttl: int, length: int
+        self, domain: _str, type_: _int, class_: _int, ttl: _int, length: _int
     ) -> Optional[DNSRecord]:
         """Read known records types and skip unknown ones."""
         if type_ == _TYPE_A:
             dns_address = DNSAddress(domain, type_, class_, ttl, self._read_string(4))
             dns_address.created = self.now
             return dns_address
         if type_ in (_TYPE_CNAME, _TYPE_PTR):
@@ -320,15 +321,15 @@
             )
         # Try to ignore types we don't know about
         # Skip the payload for the resource record so the next
         # records can be parsed correctly
         self.offset += length
         return None
 
-    def _read_bitmap(self, end: int) -> List[int]:
+    def _read_bitmap(self, end: _int) -> List[int]:
         """Reads an NSEC bitmap from the packet."""
         rdtypes = []
         while self.offset < end:
             offset = self.offset
             offset_plus_one = offset + 1
             offset_plus_two = offset + 2
             window = self.data[offset]
@@ -351,15 +352,15 @@
         name = ".".join(labels) + "."
         if len(name) > MAX_NAME_LENGTH:
             raise IncomingDecodeError(
                 f"DNS name {name} exceeds maximum length of {MAX_NAME_LENGTH} from {self.source}"
             )
         return name
 
-    def _decode_labels_at_offset(self, off: int, labels: List[str], seen_pointers: Set[int]) -> int:
+    def _decode_labels_at_offset(self, off: _int, labels: List[str], seen_pointers: Set[int]) -> int:
         # This is a tight loop that is called frequently, small optimizations can make a difference.
         while off < self._data_len:
             length = self.data[off]
             if length == 0:
                 return off + DNS_COMPRESSION_HEADER_LEN
 
             if length < 0x40:
```

### Comparing `zeroconf-0.68.1/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.69.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.69.0/src/zeroconf/_protocol/outgoing.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     _MAX_MSG_ABSOLUTE,
     _MAX_MSG_TYPICAL,
 )
 from .incoming import DNSIncoming
 
 str_ = str
 float_ = float
+int_ = int
 DNSQuestion_ = DNSQuestion
 DNSRecord_ = DNSRecord
 
 
 class State(enum.Enum):
     init = 0
     finished = 1
@@ -193,28 +194,28 @@
         cached_entries = cache.get_all_by_details(name, type_, class_)
         if not cached_entries:
             self.add_question(DNSQuestion(name, type_, class_))
             return
         for cached_entry in cached_entries:
             self.add_answer_at_time(cached_entry, now)
 
-    def _write_byte(self, value: int) -> None:
+    def _write_byte(self, value: int_) -> None:
         """Writes a single byte to the packet"""
         self.data.append(value.to_bytes(1, 'big'))
         self.size += 1
 
-    def _insert_short_at_start(self, value: int) -> None:
+    def _insert_short_at_start(self, value: int_) -> None:
         """Inserts an unsigned short at the start of the packet"""
         self.data.insert(0, value.to_bytes(2, 'big'))
 
-    def _replace_short(self, index: int, value: int) -> None:
+    def _replace_short(self, index: int_, value: int_) -> None:
         """Replaces an unsigned short in a certain position in the packet"""
         self.data[index] = value.to_bytes(2, 'big')
 
-    def write_short(self, value: int) -> None:
+    def write_short(self, value: int_) -> None:
         """Writes an unsigned short to the packet"""
         self.data.append(value.to_bytes(2, 'big'))
         self.size += 2
 
     def _write_int(self, value: Union[float, int]) -> None:
         """Writes an unsigned integer to the packet"""
         self.data.append(int(value).to_bytes(4, 'big'))
@@ -317,15 +318,15 @@
         for d in self.data[index + 1 :]:
             length += len(d)
         # Here we replace the 0 length short we wrote
         # before with the actual length
         self._replace_short(index, length)
         return self._check_data_limit_or_rollback(start_data_length, start_size)
 
-    def _check_data_limit_or_rollback(self, start_data_length: int, start_size: int) -> bool:
+    def _check_data_limit_or_rollback(self, start_data_length: int_, start_size: int_) -> bool:
         """Check data limit, if we go over, then rollback and return False."""
         len_limit = _MAX_MSG_ABSOLUTE if self.allow_long else _MAX_MSG_TYPICAL
         self.allow_long = False
 
         if self.size <= len_limit:
             return True
 
@@ -334,40 +335,40 @@
         self.size = start_size
 
         rollback_names = [name for name, idx in self.names.items() if idx >= start_size]
         for name in rollback_names:
             del self.names[name]
         return False
 
-    def _write_questions_from_offset(self, questions_offset: int) -> int:
+    def _write_questions_from_offset(self, questions_offset: int_) -> int:
         questions_written = 0
         for question in self.questions[questions_offset:]:
             if not self._write_question(question):
                 break
             questions_written += 1
         return questions_written
 
-    def _write_answers_from_offset(self, answer_offset: int) -> int:
+    def _write_answers_from_offset(self, answer_offset: int_) -> int:
         answers_written = 0
         for answer, time_ in self.answers[answer_offset:]:
             if not self._write_record(answer, time_):
                 break
             answers_written += 1
         return answers_written
 
-    def _write_records_from_offset(self, records: Sequence[DNSRecord], offset: int) -> int:
+    def _write_records_from_offset(self, records: Sequence[DNSRecord], offset: int_) -> int:
         records_written = 0
         for record in records[offset:]:
             if not self._write_record(record, 0):
                 break
             records_written += 1
         return records_written
 
     def _has_more_to_add(
-        self, questions_offset: int, answer_offset: int, authority_offset: int, additional_offset: int
+        self, questions_offset: int_, answer_offset: int_, authority_offset: int_, additional_offset: int_
     ) -> bool:
         """Check if all questions, answers, authority, and additionals have been written to the packet."""
         return (
             questions_offset < len(self.questions)
             or answer_offset < len(self.answers)
             or authority_offset < len(self.authorities)
             or additional_offset < len(self.additionals)
```

### Comparing `zeroconf-0.68.1/src/zeroconf/_services/__init__.py` & `zeroconf-0.69.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_services/browser.py` & `zeroconf-0.69.0/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_services/info.py` & `zeroconf-0.69.0/src/zeroconf/_services/info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_services/registry.py` & `zeroconf-0.69.0/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_services/types.py` & `zeroconf-0.69.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_updates.py` & `zeroconf-0.69.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_utils/__init__.py` & `zeroconf-0.69.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.69.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_utils/name.py` & `zeroconf-0.69.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_utils/net.py` & `zeroconf-0.69.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/_utils/time.py` & `zeroconf-0.69.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/asyncio.py` & `zeroconf-0.69.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/src/zeroconf/const.py` & `zeroconf-0.69.0/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/__init__.py` & `zeroconf-0.69.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/conftest.py` & `zeroconf-0.69.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/services/__init__.py` & `zeroconf-0.69.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/services/test_browser.py` & `zeroconf-0.69.0/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/services/test_info.py` & `zeroconf-0.69.0/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/services/test_registry.py` & `zeroconf-0.69.0/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/services/test_types.py` & `zeroconf-0.69.0/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_asyncio.py` & `zeroconf-0.69.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_cache.py` & `zeroconf-0.69.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_core.py` & `zeroconf-0.69.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_dns.py` & `zeroconf-0.69.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_exceptions.py` & `zeroconf-0.69.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_handlers.py` & `zeroconf-0.69.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_history.py` & `zeroconf-0.69.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_init.py` & `zeroconf-0.69.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_logger.py` & `zeroconf-0.69.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_protocol.py` & `zeroconf-0.69.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_services.py` & `zeroconf-0.69.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/test_updates.py` & `zeroconf-0.69.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/utils/__init__.py` & `zeroconf-0.69.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/utils/test_asyncio.py` & `zeroconf-0.69.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/utils/test_name.py` & `zeroconf-0.69.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/tests/utils/test_net.py` & `zeroconf-0.69.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.68.1/setup.py` & `zeroconf-0.69.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.68.1',
+    'version': '0.69.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.68.1/PKG-INFO` & `zeroconf-0.69.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.68.1
+Version: 0.69.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


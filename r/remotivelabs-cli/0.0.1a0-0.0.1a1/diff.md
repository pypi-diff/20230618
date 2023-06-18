# Comparing `tmp/remotivelabs_cli-0.0.1a0.tar.gz` & `tmp/remotivelabs_cli-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotivelabs_cli-0.0.1a0.tar", max compression
+gzip compressed data, was "remotivelabs_cli-0.0.1a1.tar", max compression
```

## Comparing `remotivelabs_cli-0.0.1a0.tar` & `remotivelabs_cli-0.0.1a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       18 2023-06-15 10:09:58.758965 remotivelabs_cli-0.0.1a0/README.md
--rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a0/cli/__about__.py
--rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a0/cli/__init__.py
--rw-r--r--   0        0        0     3392 2023-06-09 09:05:12.660223 remotivelabs_cli-0.0.1a0/cli/brokers.py
--rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a0/cli/cloud/__init__.py
--rw-r--r--   0        0        0     3675 2023-06-09 11:46:02.064612 remotivelabs_cli-0.0.1a0/cli/cloud/auth.py
--rw-r--r--   0        0        0     2284 2023-05-30 06:23:51.161239 remotivelabs_cli-0.0.1a0/cli/cloud/brokers.py
--rw-r--r--   0        0        0     1691 2023-06-08 05:58:07.097588 remotivelabs_cli-0.0.1a0/cli/cloud/cloud_cli.py
--rw-r--r--   0        0        0     3153 2022-10-25 11:06:37.541648 remotivelabs_cli-0.0.1a0/cli/cloud/configs.py
--rw-r--r--   0        0        0     7259 2023-04-20 09:15:55.106560 remotivelabs_cli-0.0.1a0/cli/cloud/recordings.py
--rw-r--r--   0        0        0     2861 2023-06-09 09:54:06.620182 remotivelabs_cli-0.0.1a0/cli/cloud/rest_helper.py
--rw-r--r--   0        0        0     1580 2023-06-09 11:33:01.362939 remotivelabs_cli-0.0.1a0/cli/cloud/service_account_keys.py
--rw-r--r--   0        0        0     1251 2023-06-08 05:57:20.045566 remotivelabs_cli-0.0.1a0/cli/cloud/service_accounts.py
--rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a0/cli/lib/__about__.py
--rw-r--r--   0        0        0     4905 2022-10-20 06:14:07.629916 remotivelabs_cli-0.0.1a0/cli/lib/broker.py
--rw-r--r--   0        0        0      344 2023-06-16 17:25:52.071699 remotivelabs_cli-0.0.1a0/cli/remotive.py
--rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a0/cli/requirements.txt
--rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a0/cli/test/test_simple.py
--rw-r--r--   0        0        0      534 2023-06-16 17:29:07.424407 remotivelabs_cli-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2092 2023-06-18 17:01:10.908056 remotivelabs_cli-0.0.1a1/README.md
+-rw-r--r--   0        0        0      122 2022-10-26 14:05:47.581000 remotivelabs_cli-0.0.1a1/cli/__about__.py
+-rw-r--r--   0        0        0       26 2022-10-26 11:41:55.030088 remotivelabs_cli-0.0.1a1/cli/__init__.py
+-rw-r--r--   0        0        0     3392 2023-06-09 09:05:12.660223 remotivelabs_cli-0.0.1a1/cli/brokers.py
+-rw-r--r--   0        0        0        1 2022-10-24 12:45:02.134227 remotivelabs_cli-0.0.1a1/cli/cloud/__init__.py
+-rw-r--r--   0        0        0     3675 2023-06-09 11:46:02.064612 remotivelabs_cli-0.0.1a1/cli/cloud/auth.py
+-rw-r--r--   0        0        0     2284 2023-05-30 06:23:51.161239 remotivelabs_cli-0.0.1a1/cli/cloud/brokers.py
+-rw-r--r--   0        0        0     1691 2023-06-08 05:58:07.097588 remotivelabs_cli-0.0.1a1/cli/cloud/cloud_cli.py
+-rw-r--r--   0        0        0     3153 2022-10-25 11:06:37.541648 remotivelabs_cli-0.0.1a1/cli/cloud/configs.py
+-rw-r--r--   0        0        0     7259 2023-04-20 09:15:55.106560 remotivelabs_cli-0.0.1a1/cli/cloud/recordings.py
+-rw-r--r--   0        0        0     2861 2023-06-09 09:54:06.620182 remotivelabs_cli-0.0.1a1/cli/cloud/rest_helper.py
+-rw-r--r--   0        0        0     1580 2023-06-09 11:33:01.362939 remotivelabs_cli-0.0.1a1/cli/cloud/service_account_keys.py
+-rw-r--r--   0        0        0     1251 2023-06-08 05:57:20.045566 remotivelabs_cli-0.0.1a1/cli/cloud/service_accounts.py
+-rw-r--r--   0        0        0      141 2022-10-25 14:33:01.608000 remotivelabs_cli-0.0.1a1/cli/lib/__about__.py
+-rw-r--r--   0        0        0     4905 2022-10-20 06:14:07.629916 remotivelabs_cli-0.0.1a1/cli/lib/broker.py
+-rw-r--r--   0        0        0      342 2023-06-18 17:02:58.041218 remotivelabs_cli-0.0.1a1/cli/remotive.py
+-rw-r--r--   0        0        0       77 2023-06-08 06:07:23.995982 remotivelabs_cli-0.0.1a1/cli/requirements.txt
+-rw-r--r--   0        0        0       63 2023-03-21 06:24:07.422989 remotivelabs_cli-0.0.1a1/cli/test/test_simple.py
+-rw-r--r--   0        0        0      535 2023-06-18 17:03:59.797659 remotivelabs_cli-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 remotivelabs_cli-0.0.1a1/PKG-INFO
```

### Comparing `remotivelabs_cli-0.0.1a0/cli/brokers.py` & `remotivelabs_cli-0.0.1a1/cli/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/cloud/auth.py` & `remotivelabs_cli-0.0.1a1/cli/cloud/auth.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/cloud/brokers.py` & `remotivelabs_cli-0.0.1a1/cli/cloud/brokers.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/cloud/cloud_cli.py` & `remotivelabs_cli-0.0.1a1/cli/cloud/cloud_cli.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/cloud/configs.py` & `remotivelabs_cli-0.0.1a1/cli/cloud/configs.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/cloud/recordings.py` & `remotivelabs_cli-0.0.1a1/cli/cloud/recordings.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/cloud/rest_helper.py` & `remotivelabs_cli-0.0.1a1/cli/cloud/rest_helper.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/cloud/service_account_keys.py` & `remotivelabs_cli-0.0.1a1/cli/cloud/service_account_keys.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/cloud/service_accounts.py` & `remotivelabs_cli-0.0.1a1/cli/cloud/service_accounts.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/cli/lib/broker.py` & `remotivelabs_cli-0.0.1a1/cli/lib/broker.py`

 * *Files identical despite different names*

### Comparing `remotivelabs_cli-0.0.1a0/pyproject.toml` & `remotivelabs_cli-0.0.1a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "remotivelabs-cli"
-version = "0.0.1.a0"
+version = "0.0.1.a1"
 description = ""
 authors = ["Johan Rask <johan.rask@remotivelabs.com>"]
 readme = "README.md"
 packages = [{include = "cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = "^0.6.1"
-#remotivelabs-broker = "^0.1.0"
+remotivelabs-broker = "^0.1.0"
 rich = "^12.6.0"
 cryptography = "40.0.2"
 pyjwt = "^2.6.0"
 zeroconf = "^0.64.1"
-urllib3 = ">=1.26"
-requests = ">=2.25"
+#urllib3 = ">=1.26"
+#requests = ">=2.25"
 
 [tool.poetry.scripts]
 remotive = "cli.remotive:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```


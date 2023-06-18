# Comparing `tmp/koios-api-1.0.10.3.tar.gz` & `tmp/koios-api-1.0.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koios-api-1.0.10.3.tar", last modified: Mon May 22 06:49:31 2023, max compression
+gzip compressed data, was "koios-api-1.0.10.4.tar", last modified: Sun Jun 18 06:21:08 2023, max compression
```

## Comparing `koios-api-1.0.10.3.tar` & `koios-api-1.0.10.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/
--rw-rw-r--   0 george    (1000) george    (1000)     1080 2023-04-22 10:04:11.000000 koios-api-1.0.10.3/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)   106449 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)   105808 2023-05-22 06:46:32.000000 koios-api-1.0.10.3/README.md
--rw-rw-r--   0 george    (1000) george    (1000)      797 2023-05-22 06:41:10.000000 koios-api-1.0.10.3/pyproject.toml
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/setup.cfg
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/src/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/src/koios_api/
--rw-rw-r--   0 george    (1000) george    (1000)     1393 2023-05-11 12:12:45.000000 koios-api-1.0.10.3/src/koios_api/__config__.py
--rw-rw-r--   0 george    (1000) george    (1000)      228 2022-10-13 07:47:20.000000 koios-api-1.0.10.3/src/koios_api/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)    10715 2023-05-22 04:51:43.000000 koios-api-1.0.10.3/src/koios_api/account.py
--rw-rw-r--   0 george    (1000) george    (1000)     6164 2023-05-22 05:12:44.000000 koios-api-1.0.10.3/src/koios_api/address.py
--rw-rw-r--   0 george    (1000) george    (1000)    16024 2023-05-11 13:26:52.000000 koios-api-1.0.10.3/src/koios_api/asset.py
--rw-rw-r--   0 george    (1000) george    (1000)     3177 2023-05-11 12:03:49.000000 koios-api-1.0.10.3/src/koios_api/block.py
--rw-rw-r--   0 george    (1000) george    (1000)     2690 2023-05-11 08:51:55.000000 koios-api-1.0.10.3/src/koios_api/epoch.py
--rw-rw-r--   0 george    (1000) george    (1000)     2514 2023-05-11 08:41:06.000000 koios-api-1.0.10.3/src/koios_api/network.py
--rw-rw-r--   0 george    (1000) george    (1000)    10428 2023-05-19 07:44:11.000000 koios-api-1.0.10.3/src/koios_api/pool.py
--rw-rw-r--   0 george    (1000) george    (1000)     3595 2023-05-11 12:04:31.000000 koios-api-1.0.10.3/src/koios_api/script.py
--rw-rw-r--   0 george    (1000) george    (1000)     5414 2023-05-11 12:04:23.000000 koios-api-1.0.10.3/src/koios_api/transactions.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-05-22 06:49:31.777329 koios-api-1.0.10.3/src/koios_api.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)   106449 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)      490 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/SOURCES.txt
--rw-rw-r--   0 george    (1000) george    (1000)        1 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/dependency_links.txt
--rw-rw-r--   0 george    (1000) george    (1000)       17 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/requires.txt
--rw-rw-r--   0 george    (1000) george    (1000)       16 2023-05-22 06:49:31.000000 koios-api-1.0.10.3/src/koios_api.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-18 06:21:08.915686 koios-api-1.0.10.4/
+-rw-rw-r--   0 george    (1000) george    (1000)     1080 2023-04-22 10:04:11.000000 koios-api-1.0.10.4/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)   106767 2023-06-18 06:21:08.911686 koios-api-1.0.10.4/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)   106126 2023-06-18 04:53:30.000000 koios-api-1.0.10.4/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)      797 2023-06-18 04:46:57.000000 koios-api-1.0.10.4/pyproject.toml
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-06-18 06:21:08.915686 koios-api-1.0.10.4/setup.cfg
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-18 06:21:08.911686 koios-api-1.0.10.4/src/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-18 06:21:08.911686 koios-api-1.0.10.4/src/koios_api/
+-rw-rw-r--   0 george    (1000) george    (1000)     1395 2023-06-18 04:46:57.000000 koios-api-1.0.10.4/src/koios_api/__config__.py
+-rw-rw-r--   0 george    (1000) george    (1000)      228 2022-10-13 07:47:20.000000 koios-api-1.0.10.4/src/koios_api/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)    12344 2023-06-18 06:09:11.000000 koios-api-1.0.10.4/src/koios_api/account.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7027 2023-06-18 06:11:06.000000 koios-api-1.0.10.4/src/koios_api/address.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18802 2023-06-18 06:12:36.000000 koios-api-1.0.10.4/src/koios_api/asset.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3743 2023-06-18 06:13:11.000000 koios-api-1.0.10.4/src/koios_api/block.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3221 2023-06-18 06:06:02.000000 koios-api-1.0.10.4/src/koios_api/epoch.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3222 2023-06-18 06:06:24.000000 koios-api-1.0.10.4/src/koios_api/network.py
+-rw-rw-r--   0 george    (1000) george    (1000)    12583 2023-06-18 06:14:31.000000 koios-api-1.0.10.4/src/koios_api/pool.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4333 2023-06-18 06:14:51.000000 koios-api-1.0.10.4/src/koios_api/script.py
+-rw-rw-r--   0 george    (1000) george    (1000)     6491 2023-06-18 06:15:14.000000 koios-api-1.0.10.4/src/koios_api/transactions.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-18 06:21:08.911686 koios-api-1.0.10.4/src/koios_api.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)   106767 2023-06-18 06:21:08.000000 koios-api-1.0.10.4/src/koios_api.egg-info/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)      490 2023-06-18 06:21:08.000000 koios-api-1.0.10.4/src/koios_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 george    (1000) george    (1000)        1 2023-06-18 06:21:08.000000 koios-api-1.0.10.4/src/koios_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       17 2023-06-18 06:21:08.000000 koios-api-1.0.10.4/src/koios_api.egg-info/requires.txt
+-rw-rw-r--   0 george    (1000) george    (1000)       16 2023-06-18 06:21:08.000000 koios-api-1.0.10.4/src/koios_api.egg-info/top_level.txt
```

### Comparing `koios-api-1.0.10.3/LICENSE` & `koios-api-1.0.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `koios-api-1.0.10.3/PKG-INFO` & `koios-api-1.0.10.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koios-api
-Version: 1.0.10.3
+Version: 1.0.10.4
 Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
 Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
 Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
 Keywords: koios,cardano,blockchain,REST,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,14 +37,23 @@
 
 To work with a custom Api URL, set the environment variable:
 
 ```bash
 export API_BASE_URL=https://custom.url/api/v0
 ```
 
+Other environment variables that can be set, and their default versions, are:
+
+```bash
+SLEEP_TIME=1
+API_RESP_COUNT=1000
+```
+
+SLEEP_TIME is the time between retries after an API errors and API_RESP_COUNT is the maximum number of records the API should return (1000 is the absolute maximum supported by the Koios API).
+
 ## Using the module
 Importing the complete module:
 ```python
 import koios_api
 koios_api.get_tip()
 ```
 The result will be like this:
```

### Comparing `koios-api-1.0.10.3/README.md` & `koios-api-1.0.10.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,23 @@
 
 To work with a custom Api URL, set the environment variable:
 
 ```bash
 export API_BASE_URL=https://custom.url/api/v0
 ```
 
+Other environment variables that can be set, and their default versions, are:
+
+```bash
+SLEEP_TIME=1
+API_RESP_COUNT=1000
+```
+
+SLEEP_TIME is the time between retries after an API errors and API_RESP_COUNT is the maximum number of records the API should return (1000 is the absolute maximum supported by the Koios API).
+
 ## Using the module
 Importing the complete module:
 ```python
 import koios_api
 koios_api.get_tip()
 ```
 The result will be like this:
```

### Comparing `koios-api-1.0.10.3/pyproject.toml` & `koios-api-1.0.10.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 [project]
 name = "koios-api"
-version = "1.0.10.3"
+version = "1.0.10.4"
 authors = [
   { name="APEX Stake Pool", email="cardanoapexpool@gmail.com" },
 ]
 description = "A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)"
 keywords = [
     "koios",
     "cardano",
```

### Comparing `koios-api-1.0.10.3/src/koios_api/__config__.py` & `koios-api-1.0.10.4/src/koios_api/__config__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-VERSION = '1.0.10'
+VERSION = '1.0.10.4'
 env = dict(os.environ)
 if 'SLEEP_TIME' not in env:
     SLEEP_TIME = 1
 else:
     SLEEP_TIME = env['SLEEP_TIME']
 if 'API_RESP_COUNT' not in env:
     API_RESP_COUNT = 1000
```

### Comparing `koios-api-1.0.10.3/src/koios_api/account.py` & `koios-api-1.0.10.4/src/koios_api/account.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,20 +18,24 @@
     parameters = {}
     account_list = []
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, headers=headers, params=parameters).text)
-                break
+                response = requests.get(url, headers=headers, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('offset: %s, retrying...' % offset)
+                print(f"offset: {offset}, retrying...")
         account_list += resp
         if len(resp) < API_RESP_COUNT:
             if 0 < limit <= len(account_list):
                 account_list = account_list[0:limit]
             break
         else:
             offset += len(resp)
@@ -53,16 +57,20 @@
     stake_addresses = {}
     if isinstance(addr, list):
         stake_addresses['_stake_addresses'] = addr
     else:
         stake_addresses['_stake_addresses'] = [addr]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(stake_addresses))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -78,20 +86,24 @@
     parameters = {'_stake_address': addr}
     utxos = []
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         utxos += resp
         if len(resp) < API_RESP_COUNT:
             if 0 < limit <= len(utxos):
                 utxos = utxos[0:limit]
             break
         else:
             offset += len(resp)
@@ -113,16 +125,20 @@
     stake_addresses = {}
     if isinstance(addr, list):
         stake_addresses['_stake_addresses'] = addr
     else:
         stake_addresses['_stake_addresses'] = [addr]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(stake_addresses))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -141,16 +157,20 @@
         stake_addresses['_stake_addresses'] = addr
     else:
         stake_addresses['_stake_addresses'] = [addr]
     if isinstance(epoch, int) and epoch > 0:
         stake_addresses['_epoch_no'] = epoch
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(stake_addresses))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -167,16 +187,20 @@
     stake_addresses = {}
     if isinstance(addr, list):
         stake_addresses['_stake_addresses'] = addr
     else:
         stake_addresses['_stake_addresses'] = [addr]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(stake_addresses))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -196,16 +220,20 @@
         parameters['_stake_addresses'] = addr
     else:
         parameters['_stake_addresses'] = [addr]
     parameters['_first_only'] = first_only
     parameters['_empty'] = empty
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(parameters)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(parameters))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -227,21 +255,24 @@
     assets = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.post(url, headers=headers, params=parameters,
-                                                data=json.dumps(stake_addresses)).text)
-                break
+                response = requests.post(url, headers=headers, params=parameters, data=json.dumps(stake_addresses))
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         assets += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return assets
 
@@ -261,14 +292,18 @@
         stake_addresses['_stake_addresses'] = addr
     else:
         stake_addresses['_stake_addresses'] = [addr]
     if epoch:
         stake_addresses['_epoch_no'] = epoch
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(stake_addresses)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(stake_addresses))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.3/src/koios_api/address.py` & `koios-api-1.0.10.4/src/koios_api/address.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,16 +17,20 @@
     addresses = {}
     if isinstance(addr, list):
         addresses['_addresses'] = addr
     else:
         addresses['_addresses'] = [addr]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(addresses)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(addresses))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -51,21 +55,24 @@
     txs = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.post(url, headers=headers, params=parameters,
-                                                data=json.dumps(addresses)).text)
-                break
+                response = requests.post(url, headers=headers, params=parameters, data=json.dumps(addresses))
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-            print('retrying...')
+                print(f"offset: {offset}, retrying...")
         txs += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return txs
 
@@ -82,16 +89,20 @@
     credentials = {}
     if isinstance(cred, list):
         credentials['_payment_credentials'] = cred
     else:
         credentials['_payment_credentials'] = [cred]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(credentials)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(credentials))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -113,21 +124,24 @@
     assets = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.post(url, headers=headers, params=parameters,
-                                                data=json.dumps(addresses)).text)
-                break
+                response = requests.post(url, headers=headers, params=parameters, data=json.dumps(addresses))
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         assets += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return assets
 
@@ -148,14 +162,18 @@
         parameters['_payment_credentials'] = cred
     else:
         parameters['_payment_credentials'] = [cred]
     if after_block:
         parameters['_after_block_height'] = after_block
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(parameters)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(parameters))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.3/src/koios_api/asset.py` & `koios-api-1.0.10.4/src/koios_api/asset.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,20 +20,24 @@
     while True:
         if offset > 0:
             parameters['offset'] = offset
         if isinstance(policy, str) and policy != '':
             parameters['policy_id'] = 'eq.' + policy
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         assets_names_hex += resp
         if len(resp) < API_RESP_COUNT:
             if 0 < limit <= len(assets_names_hex):
                 assets_names_hex = assets_names_hex[0:limit]
             break
         else:
             offset += len(resp)
@@ -54,20 +58,24 @@
     assets_token_registry = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('offset: %d, retrying...' % offset)
+                print(f"offset: {offset}, retrying...")
         assets_token_registry += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return assets_token_registry
 
@@ -87,20 +95,24 @@
     wallets = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('offset: %d, retrying...' % offset)
+                print(f"offset: {offset}, retrying...")
         wallets += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return wallets
 
@@ -119,51 +131,59 @@
         url += '&_asset_name=%s' % name
     wallets = []
     offset = 0
     while True:
         paginated_url = url + '&offset=%d' % offset
         while True:
             try:
-                resp = json.loads(requests.get(paginated_url).text)
-                break
+                response = requests.get(paginated_url)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('offset: %d, retrying...' % offset)
+                print(f"offset: {offset}, retrying...")
         wallets += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return wallets
 
 
 def get_asset_nft_address(policy: str, name: str = '') -> list:
     """
     https://api.koios.rest/#get-/asset_nft_address
-    Get the address where specified NFT currently reside on.
+    Get the address where specified NFT currently reside on
     :param policy: Asset Policy
     :param name: Asset Name in hexadecimal format
     :returns: List of maps with the wallets holding the asset and the amount of assets per wallet
     """
     url = API_BASE_URL + '/asset_nft_address'
     parameters = {'_asset_policy': policy, '_asset_name': name}
     wallets = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('offset: %d, retrying...' % offset)
+                print(f"offset: {offset}, retrying...")
         wallets += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return wallets
 
@@ -176,16 +196,20 @@
     :param name: Asset Name in hexadecimal format
     :returns: List of maps with the wallets holding the asset and the amount of assets per wallet
     """
     url = API_BASE_URL + '/asset_info'
     parameters = {'_asset_policy': policy, '_asset_name': name}
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -200,16 +224,20 @@
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
     parameters = {'_asset_list': []}
     for asset in assets:
         asset_split = asset.split('.')
         parameters['_asset_list'].append([asset_split[0], asset_split[1]])
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(parameters)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(parameters))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -228,20 +256,24 @@
     assets = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         assets += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return assets
 
@@ -259,20 +291,24 @@
     parameters = {'_asset_policy': policy}
     asset_addresses = []
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         asset_addresses += resp
         if len(resp) < API_RESP_COUNT:
             if 0 < limit <= len(asset_addresses):
                 asset_addresses = asset_addresses[0:limit]
             break
         else:
             offset += len(resp)
@@ -295,20 +331,24 @@
     parameters = {'_asset_policy': policy}
     assets = []
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         assets += resp
         if len(resp) < API_RESP_COUNT:
             if 0 < limit <= len(assets):
                 assets = assets[0:limit]
             break
         else:
             offset += len(resp)
@@ -329,20 +369,24 @@
     url = API_BASE_URL + '/asset_policy_info?_asset_policy=%s' % policy
     assets = []
     offset = 0
     while True:
         paginated_url = url + '&offset=%d' % offset
         while True:
             try:
-                resp = json.loads(requests.get(paginated_url).text)
-                break
+                response = requests.get(paginated_url)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         assets += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return assets
 
@@ -360,20 +404,24 @@
     parameters = {'_asset_policy': policy}
     assets = []
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         assets += resp
         if len(resp) < API_RESP_COUNT:
             if 0 < limit <= len(assets):
                 assets = assets[0:limit]
             break
         else:
             offset += len(resp)
@@ -391,16 +439,20 @@
     :param name: Asset Name in hexadecimal format (optional), default: all policy assets
     :returns: List of maps with the mint/burn history of an asset
     """
     url = API_BASE_URL + '/asset_summary'
     parameters = {'_asset_policy': policy, '_asset_name': name}
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -423,19 +475,23 @@
     assets_txs = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         assets_txs += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return assets_txs
```

### Comparing `koios-api-1.0.10.3/src/koios_api/epoch.py` & `koios-api-1.0.10.4/src/koios_api/epoch.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,16 +18,20 @@
     parameters = {}
     if isinstance(epoch, int) and epoch > 0:
         parameters['_epoch_no'] = epoch
     if isinstance(include_next_epoch, bool):
         parameters['_include_next_epoch'] = str(include_next_epoch).lower()
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -40,16 +44,20 @@
     """
     url = API_BASE_URL + '/epoch_params'
     parameters = {}
     if isinstance(epoch, int) and epoch > 0:
         parameters['_epoch_no'] = epoch
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -62,14 +70,18 @@
     """
     url = API_BASE_URL + '/epoch_block_protocols'
     parameters = {}
     if isinstance(epoch, int) and epoch > 0:
         parameters['_epoch_no'] = epoch
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.3/src/koios_api/network.py` & `koios-api-1.0.10.4/src/koios_api/network.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,16 +10,20 @@
     https://api.koios.rest/#get-/tip
     Get the tip info about the latest block seen by chain
     :returns: A list with the tip as a map
     """
     url = API_BASE_URL + '/tip'
     while True:
         try:
-            resp = json.loads(requests.get(url).text)
-            break
+            response = requests.get(url)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -28,16 +32,20 @@
     https://api.koios.rest/#get-/genesis
     Get the Genesis parameters used to start specific era on chain
     :returns: A list with the genesis parameters map
     """
     url = API_BASE_URL + '/genesis'
     while True:
         try:
-            resp = json.loads(requests.get(url).text)
-            break
+            response = requests.get(url)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -51,16 +59,20 @@
     """
     url = API_BASE_URL + '/totals'
     parameters = {}
     if isinstance(epoch, int) and epoch > 0:
         parameters['_epoch_no'] = epoch
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -69,14 +81,18 @@
     https://api.koios.rest/#get-/param_updates
     Get all parameter update proposals submitted to the chain starting Shelley era
     :returns: A list with the parameters updates
     """
     url = API_BASE_URL + '/param_updates'
     while True:
         try:
-            resp = json.loads(requests.get(url).text)
-            break
+            response = requests.get(url)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.3/src/koios_api/pool.py` & `koios-api-1.0.10.4/src/koios_api/pool.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,20 +17,24 @@
     pools_list = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, headers=headers, params=parameters).text)
-                break
+                response = requests.get(url, headers=headers, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         pools_list += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return pools_list
 
@@ -48,16 +52,20 @@
     pool_ids = {}
     if isinstance(pool_id, list):
         pool_ids['_pool_bech32_ids'] = pool_id
     else:
         pool_ids['_pool_bech32_ids'] = [pool_id]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(pool_ids)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(pool_ids))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -68,58 +76,66 @@
     :param pool_id: stake pool bech32 id
     :returns: Pool snapshot as list of maps by epoch (current and previous 2)
     """
     url = API_BASE_URL + '/pool_stake_snapshot'
     parameters = {'_pool_bech32': pool_id}
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
 def get_pool_delegators(pool_id: str) -> list:
     """
     https://api.koios.rest/#get-/pool_delegators
-    Return information about live delegators for a given pool.
+    Return information about live delegators for a given pool
     :param pool_id: stake pool bech32 id
     :returns: The list of pool delegators maps
     """
     url = API_BASE_URL + '/pool_delegators'
     parameters = {'_pool_bech32': pool_id}
     delegators = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         delegators += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return delegators
 
 
 def get_pool_delegators_history(pool_id: str, epoch: int = 0) -> list:
     """
     https://api.koios.rest/#get-/pool_delegators_history
     Return information about active delegators (incl. history) for a given pool and epoch number
-    (all epochs if not specified).
+    (all epochs if not specified)
     :param pool_id: stake pool bech32 id
     :param epoch: (optional) epoch
     :returns: The list of pool delegators maps
     """
     url = API_BASE_URL + '/pool_delegators_history'
     parameters = {'_pool_bech32': pool_id}
     if isinstance(epoch, int) and epoch > 0:
@@ -127,20 +143,24 @@
     delegators = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         delegators += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return delegators
 
@@ -160,20 +180,24 @@
     blocks = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         blocks += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return blocks
 
@@ -189,16 +213,20 @@
     """
     url = API_BASE_URL + '/pool_history'
     parameters = {'_pool_bech32':  pool_id}
     if isinstance(epoch, int) and epoch > 0:
         parameters['_epoch_no'] = epoch
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -216,20 +244,24 @@
     if pool_id:
         parameters['_pool_bech32'] = pool_id
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         pool_updates += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return pool_updates
 
@@ -245,20 +277,24 @@
     relays = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('retrying...')
+                print(f"offset: {offset}, retrying...")
         relays += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return relays
 
@@ -275,16 +311,20 @@
     pool_ids = {}
     if isinstance(pool_id, list):
         pool_ids['_pool_bech32_ids'] = pool_id
     else:
         pool_ids['_pool_bech32_ids'] = [pool_id]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(pool_ids)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(pool_ids))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -294,14 +334,18 @@
     :returns: The list of retiring pools maps
     """
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
     url = API_BASE_URL + '/pool_updates'
     parameters = {'pool_status': 'eq.retiring'}
     while True:
         try:
-            resp = json.loads(requests.get(url, headers=headers, params=parameters).text)
-            break
+            response = requests.get(url, headers=headers, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.3/src/koios_api/script.py` & `koios-api-1.0.10.4/src/koios_api/script.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,20 +16,24 @@
     scripts_list = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('Offset %d, retrying...' % offset)
+                print(f"offset: {offset}, retrying...")
         scripts_list += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return scripts_list
 
@@ -45,20 +49,24 @@
     scripts_list = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print('Offset %d, retrying...' % offset)
+                print(f"offset: {offset}, retrying...")
         scripts_list += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return scripts_list
 
@@ -70,16 +78,20 @@
     :param script: script hash
     :returns resp: redeemers list as map
     """
     url = API_BASE_URL + '/script_redeemers'
     parameters = {'_script_hash':  script}
     while True:
         try:
-            resp = json.loads(requests.get(url, params=parameters).text)
-            break
+            response = requests.get(url, params=parameters)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -95,14 +107,18 @@
     datum_hashes = {}
     if isinstance(datum, list):
         datum_hashes['_datum_hashes'] = datum
     else:
         datum_hashes['_datum_hashes'] = [datum]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(datum_hashes)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(datum_hashes))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.3/src/koios_api/transactions.py` & `koios-api-1.0.10.4/src/koios_api/transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,41 +17,49 @@
     tx_hashes = {}
     if isinstance(txs, list):
         tx_hashes['_tx_hashes'] = txs
     else:
         tx_hashes['_tx_hashes'] = [txs]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(tx_hashes)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(tx_hashes))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
 def get_tx_utxos(txs: [str, list]) -> list:
     """
     https://api.koios.rest/#post-/tx_utxos
-    Get UTxO set (inputs/outputs) of transactions.
+    Get UTxO set (inputs/outputs) of transactions
     :param txs: transaction hash as a string (for one transaction) or list (for multiple transactions)
     :returns: The list of transactions UTxOs maps
     """
     url = API_BASE_URL + '/tx_utxos'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
     tx_hashes = {}
     if isinstance(txs, list):
         tx_hashes['_tx_hashes'] = txs
     else:
         tx_hashes['_tx_hashes'] = [txs]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(tx_hashes)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(tx_hashes))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -67,16 +75,20 @@
     tx_hashes = {}
     if isinstance(txs, list):
         tx_hashes['_tx_hashes'] = txs
     else:
         tx_hashes['_tx_hashes'] = [txs]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(tx_hashes)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(tx_hashes))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -91,41 +103,49 @@
     metalabels_list = []
     offset = 0
     while True:
         if offset > 0:
             parameters['offset'] = offset
         while True:
             try:
-                resp = json.loads(requests.get(url, params=parameters).text)
-                break
+                response = requests.get(url, params=parameters)
+                if response.status_code == 200:
+                    resp = json.loads(response.text)
+                    break
+                else:
+                    print(f"status code: {response.status_code}, retrying...")
             except Exception as e:
                 print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
                 sleep(SLEEP_TIME)
-                print(f"Offset {offset}, retrying...")
+                print(f"offset: {offset}, retrying...")
         metalabels_list += resp
         if len(resp) < API_RESP_COUNT:
             break
         else:
             offset += len(resp)
     return metalabels_list
 
 
 def submit_tx(tx: str) -> str:
     """
     https://api.koios.rest/#post-/submittx
-    Submit an already serialized transaction to the network.
+    Submit an already serialized transaction to the network
     :param tx: transaction in cbor format
     :returns: transaction hash
     """
     url = API_BASE_URL + '/submittx'
     headers = {'Accept': 'application/json', 'Content-Type': 'application/cbor'}
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=tx).text)
-            break
+            response = requests.post(url, headers=headers, data=tx)
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
 
 
@@ -141,14 +161,18 @@
     tx_hashes = {}
     if isinstance(txs, list):
         tx_hashes['_tx_hashes'] = txs
     else:
         tx_hashes['_tx_hashes'] = [txs]
     while True:
         try:
-            resp = json.loads(requests.post(url, headers=headers, data=json.dumps(tx_hashes)).text)
-            break
+            response = requests.post(url, headers=headers, data=json.dumps(tx_hashes))
+            if response.status_code == 200:
+                resp = json.loads(response.text)
+                break
+            else:
+                print(f"status code: {response.status_code}, retrying...")
         except Exception as e:
             print(f"Exception in {inspect.getframeinfo(inspect.currentframe()).function}: {e}")
             sleep(SLEEP_TIME)
             print('retrying...')
     return resp
```

### Comparing `koios-api-1.0.10.3/src/koios_api.egg-info/PKG-INFO` & `koios-api-1.0.10.4/src/koios_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koios-api
-Version: 1.0.10.3
+Version: 1.0.10.4
 Summary: A python package for the Cardano Blockchain Koios API (https://api.koios.rest/)
 Author-email: APEX Stake Pool <cardanoapexpool@gmail.com>
 Project-URL: Homepage, https://github.com/cardano-apexpool/koios-api-python
 Project-URL: Bug Tracker, https://github.com/cardano-apexpool/koios-api-python/issues
 Keywords: koios,cardano,blockchain,REST,API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,14 +37,23 @@
 
 To work with a custom Api URL, set the environment variable:
 
 ```bash
 export API_BASE_URL=https://custom.url/api/v0
 ```
 
+Other environment variables that can be set, and their default versions, are:
+
+```bash
+SLEEP_TIME=1
+API_RESP_COUNT=1000
+```
+
+SLEEP_TIME is the time between retries after an API errors and API_RESP_COUNT is the maximum number of records the API should return (1000 is the absolute maximum supported by the Koios API).
+
 ## Using the module
 Importing the complete module:
 ```python
 import koios_api
 koios_api.get_tip()
 ```
 The result will be like this:
```


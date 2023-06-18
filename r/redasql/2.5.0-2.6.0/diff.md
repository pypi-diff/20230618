# Comparing `tmp/redasql-2.5.0.tar.gz` & `tmp/redasql-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redasql-2.5.0.tar", max compression
+gzip compressed data, was "redasql-2.6.0.tar", max compression
```

## Comparing `redasql-2.5.0.tar` & `redasql-2.6.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1063 2022-07-03 00:17:57.211526 redasql-2.5.0/LICENSE
--rw-r--r--   0        0        0     8771 2022-07-03 00:17:57.211526 redasql-2.5.0/README.md
--rw-r--r--   0        0        0      960 2022-07-03 00:18:14.403642 redasql-2.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-03 00:17:57.211526 redasql-2.5.0/redasql/__init__.py
--rw-r--r--   0        0        0     4683 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/api_client.py
--rwxr-xr-x   0        0        0     8563 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/command.py
--rw-r--r--   0        0        0     4100 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/completer.py
--rw-r--r--   0        0        0    11214 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/constants.py
--rw-r--r--   0        0        0     6028 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/dto.py
--rw-r--r--   0        0        0      727 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/exceptions.py
--rw-r--r--   0        0        0    11760 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/metacommand_executor.py
--rw-r--r--   0        0        0     4314 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/result_formatter.py
--rw-r--r--   0        0        0     2008 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/result_outputter.py
--rw-r--r--   0        0        0      496 2022-07-03 00:17:57.215526 redasql-2.5.0/redasql/utils.py
--rw-r--r--   0        0        0    10015 2022-07-03 00:18:14.847343 redasql-2.5.0/setup.py
--rw-r--r--   0        0        0     9594 2022-07-03 00:18:14.848541 redasql-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-18 16:02:08.574356 redasql-2.6.0/LICENSE
+-rw-r--r--   0        0        0     8968 2023-06-18 16:02:08.574356 redasql-2.6.0/README.md
+-rw-r--r--   0        0        0      960 2023-06-18 16:02:25.174742 redasql-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/__init__.py
+-rw-r--r--   0        0        0     6537 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/api_client.py
+-rwxr-xr-x   0        0        0     9164 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/command.py
+-rw-r--r--   0        0        0     4100 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/completer.py
+-rw-r--r--   0        0        0    11214 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/constants.py
+-rw-r--r--   0        0        0     6080 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/dto.py
+-rw-r--r--   0        0        0      727 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/exceptions.py
+-rw-r--r--   0        0        0    11760 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/metacommand_executor.py
+-rw-r--r--   0        0        0     4314 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/result_formatter.py
+-rw-r--r--   0        0        0     2008 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/result_outputter.py
+-rw-r--r--   0        0        0      496 2023-06-18 16:02:08.574356 redasql-2.6.0/redasql/utils.py
+-rw-r--r--   0        0        0     9842 1970-01-01 00:00:00.000000 redasql-2.6.0/PKG-INFO
```

### Comparing `redasql-2.5.0/LICENSE` & `redasql-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redasql-2.5.0/README.md` & `redasql-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 
 ## How To Use
 
 redasql need some arguments or environment variables.
 redasql prioritizes arguments over environment variables.
 
 
-| argument         | env                     | mean                                                                                                        |required|
-|------------------|-------------------------|-------------------------------------------------------------------------------------------------------------|---|
-| -k/--api-key     | REDASQL_REDASH_APIKEY   | API KEY(user api key)                                                                                       |True|
-| -s/--server-host | REDASQL_REDASH_ENDPOINT | Redash server hostname. ex) https://your.redash.server.host/                                                |True|
-| -p/--proxy       | REDASQL_HTTP_PROXY      | if your redash server restricted by Proxy, set url format. ex)http://user:pass@your.proxy.server:proxy-port |False|
-| -d/--data-source | None                    | initial connect datasource name.                                                                            | False                                                                                                       |
+| argument         | env                     | mean                                                                                                        | required             |
+|------------------|-------------------------|-------------------------------------------------------------------------------------------------------------|----------------------|
+| -k/--api-key     | REDASQL_REDASH_APIKEY   | API KEY(user api key)                                                                                       | True                 |
+| -s/--server-host | REDASQL_REDASH_ENDPOINT | Redash server hostname. ex) https://your.redash.server.host/                                                | True                 |
+| -p/--proxy       | REDASQL_HTTP_PROXY      | if your redash server restricted by Proxy, set url format. ex)http://user:pass@your.proxy.server:proxy-port | False                |
+| -d/--data-source | None                    | initial connect datasource name.                                                                            | False                |
 | --ignore-rc      | None                    | ignore `.redasqlrc` file                                                                                    | False(default false) |
+|--wait-interval-sec| None                    | Wait Job Pooling Interval Sec| False(default 0.1)   |
+|--timeout-count| None                    |Wait Job Pooling Count(int) | False(default 600)   |
 | --debug          | None                    | debug mode                                                                                                  | False(default false) |
 
 
 if you want to use redasql with direnv, rename `.envrc.sample` to `.envrc` and set attributes.
 
 ### special commands
```

### Comparing `redasql-2.5.0/pyproject.toml` & `redasql-2.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redasql"
-version = "2.5.0"  # using poetry-dynamic-versioning
+version = "2.6.0"  # using poetry-dynamic-versioning
 description = ""
 authors = ["denzow <denzow@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/denzow/redasql"
 repository = "https://github.com/denzow/redasql"
 keywords = ["redash", "sql"]
```

### Comparing `redasql-2.5.0/redasql/api_client.py` & `redasql-2.6.0/redasql/api_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,31 +13,52 @@
     DataSourceNotFoundError,
     QueryTimeoutError,
 )
 
 
 class ApiClient:
 
-    def __init__(self, redash_url: str, api_key: str, proxy: str = None, debug: bool = False):
+    def __init__(
+        self,
+        redash_url: str,
+        api_key: str,
+        proxy: str = None,
+        wait_interval_sec: float = 0,
+        timeout_count: Optional[int] = 600,
+        debug: bool = False
+    ):
         self.redash_url = redash_url.rstrip('/')
         self.session = requests.Session()
         self.session.headers.update({'Authorization': f'Key {api_key}'})
         self.proxy = None
         if proxy:
             self.proxy = proxy
         if self.proxy:
             self.session.proxies.update({'http': self.proxy, 'https': self.proxy})
+        self.wait_interval_sec = wait_interval_sec
+        self.timeout_count = timeout_count
         if debug:
             import logging
             import http.client as http_client
             requests_log = logging.getLogger("requests.packages.urllib3")
             requests_log.setLevel(logging.DEBUG)
             fmt = "[DEBUG LOGGING][%(asctime)s] %(levelname)s %(name)s :%(message)s"
             logging.basicConfig(level=logging.DEBUG, format=fmt)
             http_client.HTTPConnection.debuglevel = 1
+        self._version: Optional[str] = None
+
+    @property
+    def version(self):
+        if not self._version:
+            self._version = self.get_version()
+        return self._version
+
+    @property
+    def major_version(self) -> int:
+        return int(self.version.split('.')[0])
 
     def get_data_sources(self) -> List[DataSourceResponse]:
         res = self._get('api/data_sources')
         res_json = res.json()
         return [DataSourceResponse.from_response(ds) for ds in res_json]
 
     def get_data_source_by_name(self, name: str) -> Optional[DataSourceResponse]:
@@ -48,16 +69,28 @@
 
     def get_data_source_by_id(self, data_source_id: int) -> Optional[DataSourceResponse]:
         for ds in self.get_data_sources():
             if ds.id == data_source_id:
                 return ds
         raise DataSourceNotFoundError(f'data source id [{data_source_id}] is not found.')
 
-    def get_schema(self, data_source_id: int) -> List[SchemaResponse]:
-        res = self._get(f'api/data_sources/{data_source_id}/schema')
+    def get_schema(self, data_source_id: int, refresh: bool = True) -> List[SchemaResponse]:
+        param = ''
+        if refresh:
+            param = '?refresh=true'
+        res = self._get(f'api/data_sources/{data_source_id}/schema{param}')
+        res_json = res.json()
+        # over redash ver10 return job, when refresh = true.
+        if 'job' in res_json:
+            return self._wait_job_for_schema(
+                res_json['job']['id'],
+                timeout=self.timeout_count,
+                wait_interval_sec=self.wait_interval_sec
+            )
+
         if 'schema' not in res.json():
             return []
         return [SchemaResponse.from_response(s) for s in res.json()['schema']]
 
     def get_queries(self):
         res = self._get('api/queries')
         return res.json()
@@ -72,15 +105,15 @@
         return res_json['client_config']['version']
 
     def get_query_result(self, query_result_id: int) -> QueryResultResponse:
         res = self._get(f'api/query_results/{query_result_id}')
         return QueryResultResponse.from_response(res.json()['query_result'])
 
     def execute_query(
-            self, query: str, data_source_id: int, max_age: int = -1, timeout=10*60
+            self, query: str, data_source_id: int, max_age: int = -1
     ) -> QueryResultResponse:
         res = self._post(
             'api/query_results',
             json={
                 'query': f'{query}',
                 'data_source_id': data_source_id,
                 'max_age': max_age,
@@ -89,17 +122,17 @@
         res_json = res.json()
         # has result
         if 'query_result' in res_json:
             return QueryResultResponse.from_response(res_json['query_result'])
 
         # no result, wait execution.
         job_id = res_json['job']['id']
-        return self._wait_job(job_id, timeout)
+        return self._wait_job(job_id, self.timeout_count, self.wait_interval_sec)
 
-    def _wait_job(self, job_id: str, timeout: int):
+    def _wait_job(self, job_id: str, timeout: int, wait_interval_sec: float):
         retry_counter = 0
         while True:
             res = self._get(f'api/jobs/{job_id}')
             res_json = res.json()
 
             # 3: success
             if res_json.get('job', {}).get('status') == 3:
@@ -107,18 +140,38 @@
                 return self.get_query_result(query_result_id)
 
             # 4: error
             if res_json.get('job', {}).get('status') == 4:
                 error_msg = res_json['job']['error']
                 raise QueryRuntimeError(error_msg)
 
+            time.sleep(wait_interval_sec)
             retry_counter += 1
             if retry_counter > timeout:
                 raise QueryTimeoutError(f'Wait Query Complete. but not completed[{timeout}].')
-            time.sleep(0.1)
+
+    def _wait_job_for_schema(self, job_id: str, timeout: int, wait_interval_sec: float):
+        retry_counter = 0
+        while True:
+            res = self._get(f'api/jobs/{job_id}')
+            res_json = res.json()
+
+            # 3: success
+            if res_json.get('job', {}).get('status') == 3:
+                schema_result = res_json['job']['result']
+                return [SchemaResponse.from_response(s) for s in schema_result]
+
+            # 4: error
+            if res_json.get('job', {}).get('status') == 4:
+                error_msg = res_json['job']['error']
+                raise QueryRuntimeError(error_msg)
+            time.sleep(wait_interval_sec)
+            retry_counter += 1
+            if retry_counter > timeout:
+                raise QueryTimeoutError(f'Wait Query Complete. but not completed[{timeout} * {wait_interval_sec}].')
 
     def _get(self, path, **kwargs):
         return self._request('GET', path, **kwargs)
 
     def _post(self, path, **kwargs):
         return self._request('POST', path, **kwargs)
```

### Comparing `redasql-2.5.0/redasql/command.py` & `redasql-2.6.0/redasql/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     def __init__(
         self,
         endpoint: str,
         api_key: str,
         proxy: str,
         data_source_name: Optional[str],
         ignore_rc: bool,
+        wait_interval_sec: float,
+        timeout_count: int,
         debug: bool,
     ):
         self.endpoint = endpoint if endpoint else os.environ.get('REDASQL_REDASH_ENDPOINT')
         self.api_key = api_key if api_key else os.environ.get('REDASQL_REDASH_APIKEY')
         if self.endpoint is None or self.api_key is None:
             raise InsufficientParametersError(dedent("""
             "endpoint" and "api key" are absolutely necessary. use args or environment
@@ -46,14 +48,16 @@
         self.proxy = proxy if proxy else os.environ.get('REDASQL_HTTP_PROXY')
         self.ignore_rc = ignore_rc
         self.debug = debug
         self.client = ApiClient(
             redash_url=self.endpoint,
             api_key=self.api_key,
             proxy=self.proxy,
+            wait_interval_sec=wait_interval_sec,
+            timeout_count=timeout_count,
             debug=debug,
         )
         self.pivoted = False
         self.output = out_putter_factory(OutputType.STDOUT)
         self.formatter = formatter_factory(FormatterType.TABLE)
         self.input_buffer = []
         self.complete_data = CompleteData()
@@ -256,27 +260,45 @@
         help=dedent("""
         ignore rc file
         """),
         action='store_true',
         default=False,
     )
     parser.add_argument(
+        '--wait-interval-sec',
+        help=dedent("""
+        Wait Job Pooling Interval Sec(float)
+        """),
+        type=float,
+        default=0.1,
+    )
+    parser.add_argument(
+        '--timeout-count',
+        help=dedent("""
+        Wait Job Pooling Count(int)
+        """),
+        type=int,
+        default=600,
+    )
+    parser.add_argument(
         '--debug',
         help=dedent("""
         debug mode on
         """),
         action='store_true',
         default=False,
     )
     args = parser.parse_args()
     return CommandArgs(
         api_key=args.api_key,
         endpoint=args.server_host,
         data_source_name=args.data_source,
         proxy=args.proxy,
+        wait_interval_sec=args.wait_interval_sec,
+        timeout_count=args.timeout_count,
         ignore_rc=args.ignore_rc,
         debug=args.debug,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `redasql-2.5.0/redasql/completer.py` & `redasql-2.6.0/redasql/completer.py`

 * *Files identical despite different names*

### Comparing `redasql-2.5.0/redasql/constants.py` & `redasql-2.6.0/redasql/constants.py`

 * *Files identical despite different names*

### Comparing `redasql-2.5.0/redasql/dto.py` & `redasql-2.6.0/redasql/dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 @dataclasses.dataclass(frozen=True)
 class CommandArgs:
     api_key: Optional[str]
     endpoint: Optional[str]
     data_source_name: Optional[str]
     proxy: Optional[str]
     ignore_rc: bool
+    wait_interval_sec: float
+    timeout_count: int
     debug: bool
 
     def to_dict(self):
         return dataclasses.asdict(self)
 
 
 @dataclasses.dataclass(frozen=True)
```

### Comparing `redasql-2.5.0/redasql/exceptions.py` & `redasql-2.6.0/redasql/exceptions.py`

 * *Files identical despite different names*

### Comparing `redasql-2.5.0/redasql/metacommand_executor.py` & `redasql-2.6.0/redasql/metacommand_executor.py`

 * *Files identical despite different names*

### Comparing `redasql-2.5.0/redasql/result_formatter.py` & `redasql-2.6.0/redasql/result_formatter.py`

 * *Files identical despite different names*

### Comparing `redasql-2.5.0/redasql/result_outputter.py` & `redasql-2.6.0/redasql/result_outputter.py`

 * *Files identical despite different names*

### Comparing `redasql-2.5.0/PKG-INFO` & `redasql-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: redasql
-Version: 2.5.0
+Version: 2.6.0
 Summary: 
 Home-page: https://github.com/denzow/redasql
 License: MIT
 Keywords: redash,sql
 Author: denzow
 Author-email: denzow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: prompt-toolkit (>=3.0.20,<4.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Project-URL: Repository, https://github.com/denzow/redasql
 Description-Content-Type: text/markdown
 
@@ -41,21 +42,23 @@
 
 ## How To Use
 
 redasql need some arguments or environment variables.
 redasql prioritizes arguments over environment variables.
 
 
-| argument         | env                     | mean                                                                                                        |required|
-|------------------|-------------------------|-------------------------------------------------------------------------------------------------------------|---|
-| -k/--api-key     | REDASQL_REDASH_APIKEY   | API KEY(user api key)                                                                                       |True|
-| -s/--server-host | REDASQL_REDASH_ENDPOINT | Redash server hostname. ex) https://your.redash.server.host/                                                |True|
-| -p/--proxy       | REDASQL_HTTP_PROXY      | if your redash server restricted by Proxy, set url format. ex)http://user:pass@your.proxy.server:proxy-port |False|
-| -d/--data-source | None                    | initial connect datasource name.                                                                            | False                                                                                                       |
+| argument         | env                     | mean                                                                                                        | required             |
+|------------------|-------------------------|-------------------------------------------------------------------------------------------------------------|----------------------|
+| -k/--api-key     | REDASQL_REDASH_APIKEY   | API KEY(user api key)                                                                                       | True                 |
+| -s/--server-host | REDASQL_REDASH_ENDPOINT | Redash server hostname. ex) https://your.redash.server.host/                                                | True                 |
+| -p/--proxy       | REDASQL_HTTP_PROXY      | if your redash server restricted by Proxy, set url format. ex)http://user:pass@your.proxy.server:proxy-port | False                |
+| -d/--data-source | None                    | initial connect datasource name.                                                                            | False                |
 | --ignore-rc      | None                    | ignore `.redasqlrc` file                                                                                    | False(default false) |
+|--wait-interval-sec| None                    | Wait Job Pooling Interval Sec| False(default 0.1)   |
+|--timeout-count| None                    |Wait Job Pooling Count(int) | False(default 600)   |
 | --debug          | None                    | debug mode                                                                                                  | False(default false) |
 
 
 if you want to use redasql with direnv, rename `.envrc.sample` to `.envrc` and set attributes.
 
 ### special commands
```


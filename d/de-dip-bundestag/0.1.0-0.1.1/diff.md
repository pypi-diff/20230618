# Comparing `tmp/de-dip-bundestag-0.1.0.tar.gz` & `tmp/de_dip_bundestag-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "de-dip-bundestag-0.1.0.tar", max compression
+gzip compressed data, was "de_dip_bundestag-0.1.1.tar", max compression
```

## Comparing `de-dip-bundestag-0.1.0.tar` & `de_dip_bundestag-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,68 @@
--rw-r--r--   0        0        0     5615 2022-03-11 02:54:17.181050 de-dip-bundestag-0.1.0/README.md
--rw-r--r--   0        0        0      653 2022-03-11 02:54:31.728797 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/__init__.py
--rw-r--r--   0        0        0      229 2022-03-11 02:54:17.181050 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/api/__init__.py
--rw-r--r--   0        0        0    72674 2022-03-11 02:54:31.756796 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/api/default_api.py
--rw-r--r--   0        0        0    37295 2022-03-11 02:54:31.720797 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/api_client.py
--rw-r--r--   0        0        0      477 2022-03-11 02:54:30.708810 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/apis/__init__.py
--rw-r--r--   0        0        0    17440 2022-03-11 02:54:31.724797 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/configuration.py
--rw-r--r--   0        0        0     5032 2022-03-11 02:54:30.908807 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/exceptions.py
--rw-r--r--   0        0        0      359 2022-03-11 02:54:17.181050 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/model/__init__.py
--rw-r--r--   0        0        0    81896 2022-03-11 02:54:31.740796 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/model_utils.py
--rw-r--r--   0        0        0      386 2022-03-11 02:54:30.908807 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/models/__init__.py
--rw-r--r--   0        0        0    14516 2022-03-11 02:54:31.708797 de-dip-bundestag-0.1.0/deutschland/dip_bundestag/rest.py
--rw-r--r--   0        0        0      766 2022-03-11 02:54:16.961054 de-dip-bundestag-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6658 2022-03-11 02:54:41.519483 de-dip-bundestag-0.1.0/setup.py
--rw-r--r--   0        0        0     6518 2022-03-11 02:54:41.520170 de-dip-bundestag-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9801 2023-06-18 00:45:55.341730 de_dip_bundestag-0.1.1/README.md
+-rw-r--r--   0        0        0      677 2023-06-18 00:46:16.343594 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/__init__.py
+-rw-r--r--   0        0        0      232 2023-06-18 00:45:55.325729 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api/__init__.py
+-rw-r--r--   0        0        0    17039 2023-06-18 00:46:16.387598 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api/aktivitten_api.py
+-rw-r--r--   0        0        0    29440 2023-06-18 00:46:16.379597 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api/drucksachen_api.py
+-rw-r--r--   0        0        0    14083 2023-06-18 00:46:16.395599 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api/personenstammdaten_api.py
+-rw-r--r--   0        0        0    28981 2023-06-18 00:46:16.391598 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api/plenarprotokolle_api.py
+-rw-r--r--   0        0        0    17828 2023-06-18 00:46:16.399599 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api/vorgangspositionen_api.py
+-rw-r--r--   0        0        0    16953 2023-06-18 00:46:16.383597 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api/vorgnge_api.py
+-rw-r--r--   0        0        0    38745 2023-06-18 00:46:16.351595 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api_client.py
+-rw-r--r--   0        0        0      909 2023-06-18 00:46:11.827199 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/apis/__init__.py
+-rw-r--r--   0        0        0    17768 2023-06-18 00:46:16.355595 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/configuration.py
+-rw-r--r--   0        0        0     5089 2023-06-18 00:46:12.111226 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/exceptions.py
+-rw-r--r--   0        0        0      359 2023-06-18 00:45:55.325729 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/__init__.py
+-rw-r--r--   0        0        0    16415 2023-06-18 00:46:16.447603 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/aktivitaet.py
+-rw-r--r--   0        0        0    12441 2023-06-18 00:46:16.431602 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/aktivitaet_anzeige.py
+-rw-r--r--   0        0        0    14646 2023-06-18 00:46:16.511609 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/aktivitaet_list_response.py
+-rw-r--r--   0        0        0    12143 2023-06-18 00:46:16.451603 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/aktivitaet_list_response_all_of.py
+-rw-r--r--   0        0        0    13676 2023-06-18 00:46:16.515609 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/beschlussfassung.py
+-rw-r--r--   0        0        0    14309 2023-06-18 00:46:16.495607 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/bundesland.py
+-rw-r--r--   0        0        0    12238 2023-06-18 00:46:16.479606 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/deskriptor.py
+-rw-r--r--   0        0        0    11889 2023-06-18 00:46:16.523610 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/dokument_text_base.py
+-rw-r--r--   0        0        0    18693 2023-06-18 00:46:16.423601 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/drucksache.py
+-rw-r--r--   0        0        0    12412 2023-06-18 00:46:16.527610 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/drucksache_autoren_anzeige_inner.py
+-rw-r--r--   0        0        0    14646 2023-06-18 00:46:16.499608 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/drucksache_list_response.py
+-rw-r--r--   0        0        0    12143 2023-06-18 00:46:16.507608 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/drucksache_list_response_all_of.py
+-rw-r--r--   0        0        0    19915 2023-06-18 00:46:16.495607 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/drucksache_text.py
+-rw-r--r--   0        0        0    14707 2023-06-18 00:46:16.411600 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/drucksache_text_list_response.py
+-rw-r--r--   0        0        0    12183 2023-06-18 00:46:16.491607 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/drucksache_text_list_response_all_of.py
+-rw-r--r--   0        0        0    16288 2023-06-18 00:46:16.439602 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/fundstelle.py
+-rw-r--r--   0        0        0    12224 2023-06-18 00:46:16.479606 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/get_vorgang404_response.py
+-rw-r--r--   0        0        0    12236 2023-06-18 00:46:16.543611 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/get_vorgang_list400_response.py
+-rw-r--r--   0        0        0    14055 2023-06-18 00:46:16.471605 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/get_vorgang_list401_response.py
+-rw-r--r--   0        0        0    11974 2023-06-18 00:46:16.531610 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/inkrafttreten.py
+-rw-r--r--   0        0        0    12017 2023-06-18 00:46:16.411600 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/list_response_base.py
+-rw-r--r--   0        0        0    14708 2023-06-18 00:46:16.515609 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/person.py
+-rw-r--r--   0        0        0    14586 2023-06-18 00:46:16.507608 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/person_list_response.py
+-rw-r--r--   0        0        0    12103 2023-06-18 00:46:16.503608 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/person_list_response_all_of.py
+-rw-r--r--   0        0        0    14119 2023-06-18 00:46:16.539611 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/person_role.py
+-rw-r--r--   0        0        0    16788 2023-06-18 00:46:16.471605 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/plenarprotokoll.py
+-rw-r--r--   0        0        0    14721 2023-06-18 00:46:16.463605 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/plenarprotokoll_list_response.py
+-rw-r--r--   0        0        0    12193 2023-06-18 00:46:16.519609 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/plenarprotokoll_list_response_all_of.py
+-rw-r--r--   0        0        0    18305 2023-06-18 00:46:16.483606 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/plenarprotokoll_text.py
+-rw-r--r--   0        0        0    14796 2023-06-18 00:46:16.407600 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/plenarprotokoll_text_list_response.py
+-rw-r--r--   0        0        0    12233 2023-06-18 00:46:16.463605 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/plenarprotokoll_text_list_response_all_of.py
+-rw-r--r--   0        0        0    12795 2023-06-18 00:46:16.415600 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/quadrant.py
+-rw-r--r--   0        0        0    12027 2023-06-18 00:46:16.423601 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/ressort.py
+-rw-r--r--   0        0        0    12685 2023-06-18 00:46:16.487607 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/ueberweisung.py
+-rw-r--r--   0        0        0    12478 2023-06-18 00:46:16.523610 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/urheber.py
+-rw-r--r--   0        0        0    14762 2023-06-18 00:46:16.539611 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/verkuendung.py
+-rw-r--r--   0        0        0    17724 2023-06-18 00:46:16.443603 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgang.py
+-rw-r--r--   0        0        0    14730 2023-06-18 00:46:16.535611 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgang_deskriptor.py
+-rw-r--r--   0        0        0    11938 2023-06-18 00:46:16.431602 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgang_deskriptor_all_of.py
+-rw-r--r--   0        0        0    14601 2023-06-18 00:46:16.475606 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgang_list_response.py
+-rw-r--r--   0        0        0    12113 2023-06-18 00:46:16.435602 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgang_list_response_all_of.py
+-rw-r--r--   0        0        0    12853 2023-06-18 00:46:16.527610 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgang_verlinkung.py
+-rw-r--r--   0        0        0    12374 2023-06-18 00:46:16.467605 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgangsbezug.py
+-rw-r--r--   0        0        0    24692 2023-06-18 00:46:16.455604 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgangsposition.py
+-rw-r--r--   0        0        0    14736 2023-06-18 00:46:16.439602 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgangsposition_list_response.py
+-rw-r--r--   0        0        0    12203 2023-06-18 00:46:16.459604 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgangsposition_list_response_all_of.py
+-rw-r--r--   0        0        0    14726 2023-06-18 00:46:16.427601 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgangspositionbezug.py
+-rw-r--r--   0        0        0    11913 2023-06-18 00:46:16.543611 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/vorgangspositionbezug_all_of.py
+-rw-r--r--   0        0        0    13234 2023-06-18 00:46:16.419601 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model/zuordnung.py
+-rw-r--r--   0        0        0    82024 2023-06-18 00:46:16.371596 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model_utils.py
+-rw-r--r--   0        0        0     4721 2023-06-18 00:46:15.115487 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/models/__init__.py
+-rw-r--r--   0        0        0    14542 2023-06-18 00:46:16.359595 de_dip_bundestag-0.1.1/deutschland/dip_bundestag/rest.py
+-rw-r--r--   0        0        0      715 2023-06-18 00:45:54.509652 de_dip_bundestag-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10704 1970-01-01 00:00:00.000000 de_dip_bundestag-0.1.1/PKG-INFO
```

### Comparing `de-dip-bundestag-0.1.0/deutschland/dip_bundestag/api_client.py` & `de_dip_bundestag-0.1.1/deutschland/dip_bundestag/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-    Bundestag: Dokumentations- und Informationssystem für Parlamentsmaterialien
+    Deutscher Bundestag - DIP
 
-    DIP Bundestag API  # noqa: E501
+    API des Dokumentations- und Informationssystems für Parlamentsmaterialien  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
-    Contact: kontakt@bund.dev
+    The version of the OpenAPI document: 1.2
+    Contact: parlamentsdokumentation@bundestag.de
     Generated by: https://openapi-generator.tech
 """
 
 
 import atexit
 import io
 import json
@@ -82,15 +82,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "OpenAPI-Generator/0.1.0/python"
+        self.user_agent = "OpenAPI-Generator/0.1.1/python"
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -143,16 +143,18 @@
         _preload_content: bool = True,
         _request_timeout: typing.Optional[
             typing.Union[int, float, typing.Tuple]
         ] = None,
         _host: typing.Optional[str] = None,
         _check_type: typing.Optional[bool] = None,
         _content_type: typing.Optional[str] = None,
+        _request_auths: typing.Optional[
+            typing.List[typing.Dict[str, typing.Any]]
+        ] = None,
     ):
-
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
             header_params["Cookie"] = self.cookie
@@ -188,15 +190,21 @@
 
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
         # auth setting
         self.update_params_for_auth(
-            header_params, query_params, auth_settings, resource_path, method, body
+            header_params,
+            query_params,
+            auth_settings,
+            resource_path,
+            method,
+            body,
+            request_auths=_request_auths,
         )
 
         # request url
         if _host is None:
             url = self.configuration.host + resource_path
         else:
             # use server/host defined in path or operation instead
@@ -374,14 +382,17 @@
         collection_formats: typing.Optional[typing.Dict[str, str]] = None,
         _preload_content: bool = True,
         _request_timeout: typing.Optional[
             typing.Union[int, float, typing.Tuple]
         ] = None,
         _host: typing.Optional[str] = None,
         _check_type: typing.Optional[bool] = None,
+        _request_auths: typing.Optional[
+            typing.List[typing.Dict[str, typing.Any]]
+        ] = None,
     ):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
@@ -421,14 +432,18 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _check_type: boolean describing if the data back from the server
             should have its type checked.
         :type _check_type: bool, optional
+        :param _request_auths: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auths: list, optional
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
         """
@@ -446,14 +461,15 @@
                 auth_settings,
                 _return_http_data_only,
                 collection_formats,
                 _preload_content,
                 _request_timeout,
                 _host,
                 _check_type,
+                _request_auths=_request_auths,
             )
 
         return self.pool.apply_async(
             self.__call_api,
             (
                 resource_path,
                 method,
@@ -467,14 +483,16 @@
                 auth_settings,
                 _return_http_data_only,
                 collection_formats,
                 _preload_content,
                 _request_timeout,
                 _host,
                 _check_type,
+                None,
+                _request_auths,
             ),
         )
 
     def request(
         self,
         method,
         url,
@@ -669,43 +687,64 @@
 
         if "application/json" in content_types or "*/*" in content_types:
             return "application/json"
         else:
             return content_types[0]
 
     def update_params_for_auth(
-        self, headers, queries, auth_settings, resource_path, method, body
+        self,
+        headers,
+        queries,
+        auth_settings,
+        resource_path,
+        method,
+        body,
+        request_auths=None,
     ):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
         :param queries: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
         :param resource_path: A string representation of the HTTP request resource path.
         :param method: A string representation of the HTTP request method.
         :param body: A object representing the body of the HTTP request.
             The object type is the return value of _encoder.default().
+        :param request_auths: if set, the provided settings will
+            override the token in the configuration.
         """
         if not auth_settings:
             return
 
+        if request_auths:
+            for auth_setting in request_auths:
+                self._apply_auth_params(
+                    headers, queries, resource_path, method, body, auth_setting
+                )
+            return
+
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if auth_setting:
-                if auth_setting["in"] == "cookie":
-                    headers["Cookie"] = auth_setting["value"]
-                elif auth_setting["in"] == "header":
-                    if auth_setting["type"] != "http-signature":
-                        headers[auth_setting["key"]] = auth_setting["value"]
-                elif auth_setting["in"] == "query":
-                    queries.append((auth_setting["key"], auth_setting["value"]))
-                else:
-                    raise ApiValueError(
-                        "Authentication token must be in `query` or `header`"
-                    )
+                self._apply_auth_params(
+                    headers, queries, resource_path, method, body, auth_setting
+                )
+
+    def _apply_auth_params(
+        self, headers, queries, resource_path, method, body, auth_setting
+    ):
+        if auth_setting["in"] == "cookie":
+            headers["Cookie"] = auth_setting["key"] + "=" + auth_setting["value"]
+        elif auth_setting["in"] == "header":
+            if auth_setting["type"] != "http-signature":
+                headers[auth_setting["key"]] = auth_setting["value"]
+        elif auth_setting["in"] == "query":
+            queries.append((auth_setting["key"], auth_setting["value"]))
+        else:
+            raise ApiValueError("Authentication token must be in `query` or `header`")
 
 
 class Endpoint(object):
     def __init__(
         self,
         settings=None,
         params_map=None,
@@ -756,14 +795,15 @@
                 "_preload_content",
                 "_request_timeout",
                 "_return_http_data_only",
                 "_check_input_type",
                 "_check_return_type",
                 "_content_type",
                 "_spec_property_naming",
+                "_request_auths",
             ]
         )
         self.params_map["nullable"].extend(["_request_timeout"])
         self.validations = root_map["validations"]
         self.allowed_values = root_map["allowed_values"]
         self.openapi_types = root_map["openapi_types"]
         extra_types = {
@@ -780,14 +820,15 @@
                 [int],
             ),
             "_return_http_data_only": (bool,),
             "_check_input_type": (bool,),
             "_check_return_type": (bool,),
             "_spec_property_naming": (bool,),
             "_content_type": (none_type, str),
+            "_request_auths": (none_type, list),
         }
         self.openapi_types.update(extra_types)
         self.attribute_map = root_map["attribute_map"]
         self.location_map = root_map["location_map"]
         self.collection_format_map = root_map["collection_format_map"]
         self.headers_map = headers_map
         self.api_client = api_client
@@ -861,25 +902,24 @@
 
         return params
 
     def __call__(self, *args, **kwargs):
         """This method is invoked when endpoints are called
         Example:
 
-        api_instance = DefaultApi()
-        api_instance.aktivitaet_get  # this is an instance of the class Endpoint
-        api_instance.aktivitaet_get()  # this invokes api_instance.aktivitaet_get.__call__()
+        api_instance = AktivittenApi()
+        api_instance.get_aktivitaet  # this is an instance of the class Endpoint
+        api_instance.get_aktivitaet()  # this invokes api_instance.get_aktivitaet.__call__()
         which then invokes the callable functions stored in that endpoint at
-        api_instance.aktivitaet_get.callable or self.callable in this class
+        api_instance.get_aktivitaet.callable or self.callable in this class
 
         """
         return self.callable(self, *args, **kwargs)
 
     def call_with_http_info(self, **kwargs):
-
         try:
             index = (
                 self.api_client.configuration.server_operation_index.get(
                     self.settings["operation_id"],
                     self.api_client.configuration.server_index,
                 )
                 if kwargs["_host_index"] is None
@@ -965,9 +1005,10 @@
             auth_settings=self.settings["auth"],
             async_req=kwargs["async_req"],
             _check_type=kwargs["_check_return_type"],
             _return_http_data_only=kwargs["_return_http_data_only"],
             _preload_content=kwargs["_preload_content"],
             _request_timeout=kwargs["_request_timeout"],
             _host=_host,
+            _request_auths=kwargs["_request_auths"],
             collection_formats=params["collection_format"],
         )
```

### Comparing `de-dip-bundestag-0.1.0/deutschland/dip_bundestag/configuration.py` & `de_dip_bundestag-0.1.1/deutschland/dip_bundestag/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-    Bundestag: Dokumentations- und Informationssystem für Parlamentsmaterialien
+    Deutscher Bundestag - DIP
 
-    DIP Bundestag API  # noqa: E501
+    API des Dokumentations- und Informationssystems für Parlamentsmaterialien  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
-    Contact: kontakt@bund.dev
+    The version of the OpenAPI document: 1.2
+    Contact: parlamentsdokumentation@bundestag.de
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -401,36 +401,45 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
-        if "ApiKeyAuth" in self.api_key:
-            auth["ApiKeyAuth"] = {
+        if "ApiKeyHeader" in self.api_key:
+            auth["ApiKeyHeader"] = {
                 "type": "api_key",
                 "in": "header",
                 "key": "Authorization",
                 "value": self.get_api_key_with_prefix(
-                    "ApiKeyAuth",
+                    "ApiKeyHeader",
+                ),
+            }
+        if "ApiKeyQuery" in self.api_key:
+            auth["ApiKeyQuery"] = {
+                "type": "api_key",
+                "in": "query",
+                "key": "apikey",
+                "value": self.get_api_key_with_prefix(
+                    "ApiKeyQuery",
                 ),
             }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
-            "Version of the API: 1.0.0\n"
-            "SDK Package Version: 0.1.0".format(env=sys.platform, pyversion=sys.version)
+            "Version of the API: 1.2\n"
+            "SDK Package Version: 0.1.1".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `de-dip-bundestag-0.1.0/deutschland/dip_bundestag/exceptions.py` & `de_dip_bundestag-0.1.1/deutschland/dip_bundestag/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-    Bundestag: Dokumentations- und Informationssystem für Parlamentsmaterialien
+    Deutscher Bundestag - DIP
 
-    DIP Bundestag API  # noqa: E501
+    API des Dokumentations- und Informationssystems für Parlamentsmaterialien  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
-    Contact: kontakt@bund.dev
+    The version of the OpenAPI document: 1.2
+    Contact: parlamentsdokumentation@bundestag.de
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
@@ -106,15 +106,17 @@
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
-        error_message = "({0})\n" "Reason: {1}\n".format(self.status, self.reason)
+        error_message = "Status Code: {0}\n" "Reason: {1}\n".format(
+            self.status, self.reason
+        )
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
```

### Comparing `de-dip-bundestag-0.1.0/deutschland/dip_bundestag/model_utils.py` & `de_dip_bundestag-0.1.1/deutschland/dip_bundestag/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-    Bundestag: Dokumentations- und Informationssystem für Parlamentsmaterialien
+    Deutscher Bundestag - DIP
 
-    DIP Bundestag API  # noqa: E501
+    API des Dokumentations- und Informationssystems für Parlamentsmaterialien  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
-    Contact: kontakt@bund.dev
+    The version of the OpenAPI document: 1.2
+    Contact: parlamentsdokumentation@bundestag.de
     Generated by: https://openapi-generator.tech
 """
 
 
 import inspect
 import io
 import os
@@ -184,23 +184,23 @@
         return self.__getitem__(attr)
 
     def __copy__(self):
         cls = self.__class__
         if self.get("_spec_property_naming", False):
             return cls._new_from_openapi_data(**self.__dict__)
         else:
-            return new_cls.__new__(cls, **self.__dict__)
+            return cls.__new__(cls, **self.__dict__)
 
     def __deepcopy__(self, memo):
         cls = self.__class__
 
         if self.get("_spec_property_naming", False):
             new_inst = cls._new_from_openapi_data()
         else:
-            new_inst = cls.__new__(cls)
+            new_inst = cls.__new__(cls, **self.__dict__)
 
         for k, v in self.__dict__.items():
             setattr(new_inst, k, deepcopy(v, memo))
         return new_inst
 
     def __new__(cls, *args, **kwargs):
         # this function uses the discriminator to
@@ -721,18 +721,16 @@
 
 # these are used to limit what type conversions we try to do
 # when we have a valid type already and we want to try converting
 # to another type
 UPCONVERSION_TYPE_PAIRS = (
     (str, datetime),
     (str, date),
-    (
-        int,
-        float,
-    ),  # A float may be serialized as an integer, e.g. '3' is a valid serialized float.
+    # A float may be serialized as an integer, e.g. '3' is a valid serialized float.
+    (int, float),
     (list, ModelComposed),
     (dict, ModelComposed),
     (str, ModelComposed),
     (int, ModelComposed),
     (float, ModelComposed),
     (list, ModelComposed),
     (list, ModelNormal),
@@ -1604,15 +1602,15 @@
     """
     results = get_required_type_classes(required_types_mixed, spec_property_naming)
     valid_classes, child_req_types_by_current_type = results
 
     input_class_simple = get_simple_class(input_value)
     valid_type = is_valid_type(input_class_simple, valid_classes)
     if not valid_type:
-        if configuration or (input_class_simple == dict and not dict in valid_classes):
+        if configuration or (input_class_simple == dict and dict not in valid_classes):
             # if input_value is not valid_type try to convert it
             converted_instance = attempt_convert_item(
                 input_value,
                 valid_classes,
                 path_to_item,
                 configuration,
                 spec_property_naming,
@@ -1698,19 +1696,21 @@
             will be converted to a dict.
 
     Keyword Args:
         serialize (bool): if True, the keys in the dict will be values from
             attribute_map
     """
     result = {}
-    extract_item = (
-        lambda item: (item[0], model_to_dict(item[1], serialize=serialize))
-        if hasattr(item[1], "_data_store")
-        else item
-    )
+
+    def extract_item(item):
+        return (
+            (item[0], model_to_dict(item[1], serialize=serialize))
+            if hasattr(item[1], "_data_store")
+            else item
+        )
 
     model_instances = [model_instance]
     if model_instance._composed_schemas:
         model_instances.extend(model_instance._composed_instances)
     seen_json_attribute_names = set()
     used_fallback_python_attribute_names = set()
     py_to_json_map = {}
@@ -1819,15 +1819,14 @@
             _visited_composed_classes
 
     Returns
         composed_instances (list)
     """
     composed_instances = []
     for allof_class in self._composed_schemas["allOf"]:
-
         try:
             if constant_args.get("_spec_property_naming"):
                 allof_instance = allof_class._from_openapi_data(
                     **model_args, **constant_args
                 )
             else:
                 allof_instance = allof_class(**model_args, **constant_args)
@@ -2075,15 +2074,17 @@
     """
     discarded_args = get_discarded_args(self, composed_instances, model_args)
 
     # map variable names to composed_instances
     var_name_to_model_instances = {}
     for prop_name in model_args:
         if prop_name not in discarded_args:
-            var_name_to_model_instances[prop_name] = [self] + composed_instances
+            var_name_to_model_instances[prop_name] = [self] + list(
+                filter(lambda x: prop_name in x.openapi_types, composed_instances)
+            )
 
     return [
         composed_instances,
         var_name_to_model_instances,
         additional_properties_model_instances,
         discarded_args,
     ]
```

### Comparing `de-dip-bundestag-0.1.0/deutschland/dip_bundestag/rest.py` & `de_dip_bundestag-0.1.1/deutschland/dip_bundestag/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
-    Bundestag: Dokumentations- und Informationssystem für Parlamentsmaterialien
+    Deutscher Bundestag - DIP
 
-    DIP Bundestag API  # noqa: E501
+    API des Dokumentations- und Informationssystems für Parlamentsmaterialien  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
-    Contact: kontakt@bund.dev
+    The version of the OpenAPI document: 1.2
+    Contact: parlamentsdokumentation@bundestag.de
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import ipaddress
 import json
@@ -393,14 +393,16 @@
             _preload_content=_preload_content,
             _request_timeout=_request_timeout,
             body=body,
         )
 
 
 # end of class RESTClientObject
+
+
 def is_ipv4(target):
     """Test if IPv4 address or not"""
     try:
         chk = ipaddress.IPv4Address(target)
         return True
     except ipaddress.AddressValueError:
         return False
```


# Comparing `tmp/fastgenerateapi-0.0.4.tar.gz` & `tmp/fastgenerateapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgenerateapi-0.0.4.tar", last modified: Fri Jun 16 06:33:07 2023, max compression
+gzip compressed data, was "fastgenerateapi-0.0.5.tar", last modified: Sun Jun 18 06:11:07 2023, max compression
```

## Comparing `fastgenerateapi-0.0.4.tar` & `fastgenerateapi-0.0.5.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.830804 fastgenerateapi-0.0.4/
--rw-rw-rw-   0        0        0    35821 2023-06-15 11:33:13.000000 fastgenerateapi-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      664 2023-06-16 06:33:07.830138 fastgenerateapi-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.773770 fastgenerateapi-0.0.4/fastgenerateapi/
--rw-rw-rw-   0        0        0      883 2023-06-16 01:37:51.000000 fastgenerateapi-0.0.4/fastgenerateapi/__init__.py
--rw-rw-rw-   0        0        0      496 2023-06-16 06:28:03.000000 fastgenerateapi-0.0.4/fastgenerateapi/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.790723 fastgenerateapi-0.0.4/fastgenerateapi/api_view/
--rw-rw-rw-   0        0        0       14 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/api_view.py
--rw-rw-rw-   0        0        0     9189 2023-06-16 03:02:52.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/base_view.py
--rw-rw-rw-   0        0        0     4177 2023-06-16 00:58:02.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/create_view.py
--rw-rw-rw-   0        0        0     3634 2023-06-16 01:26:57.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/delete_tree_view.py
--rw-rw-rw-   0        0        0     3061 2023-06-16 01:18:56.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/delete_view.py
--rw-rw-rw-   0        0        0     7426 2023-06-16 01:29:40.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_all_view.py
--rw-rw-rw-   0        0        0     3062 2023-06-16 01:03:06.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_one_view.py
--rw-rw-rw-   0        0        0     7235 2023-06-16 04:52:13.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_tree_view.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.798222 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-16 04:46:20.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/base_mixin.py
--rw-rw-rw-   0        0        0     3826 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
--rw-rw-rw-   0        0        0      266 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/get_mixin.py
--rw-rw-rw-   0        0        0     2290 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/response_mixin.py
--rw-rw-rw-   0        0        0      317 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/save_mixin.py
--rw-rw-rw-   0        0        0    13029 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/tool_mixin.py
--rw-rw-rw-   0        0        0     3070 2023-06-16 01:29:40.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/switch_view.py
--rw-rw-rw-   0        0        0     4006 2023-06-16 03:02:52.000000 fastgenerateapi-0.0.4/fastgenerateapi/api_view/update_view.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.802213 fastgenerateapi-0.0.4/fastgenerateapi/controller/
--rw-rw-rw-   0        0        0      316 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/__init__.py
--rw-rw-rw-   0        0        0     3391 2023-06-16 00:44:07.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/filter_controller.py
--rw-rw-rw-   0        0        0     2385 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/router_controller.py
--rw-rw-rw-   0        0        0     2298 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/rpc_controller.py
--rw-rw-rw-   0        0        0      873 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/controller/search_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.804208 fastgenerateapi-0.0.4/fastgenerateapi/data_type/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/data_type/__init__.py
--rw-rw-rw-   0        0        0      727 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/data_type/data_type.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.808197 fastgenerateapi-0.0.4/fastgenerateapi/deps/
--rw-rw-rw-   0        0        0      160 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/deps/__init__.py
--rw-rw-rw-   0        0        0      813 2023-06-16 02:41:05.000000 fastgenerateapi-0.0.4/fastgenerateapi/deps/filter_params_deps.py
--rw-rw-rw-   0        0        0     3171 2023-06-15 11:43:16.000000 fastgenerateapi-0.0.4/fastgenerateapi/deps/paginator_deps.py
--rw-rw-rw-   0        0        0     1061 2023-06-16 02:55:25.000000 fastgenerateapi-0.0.4/fastgenerateapi/deps/tree_params_deps.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.811194 fastgenerateapi-0.0.4/fastgenerateapi/example/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/example/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-06-16 05:36:12.000000 fastgenerateapi-0.0.4/fastgenerateapi/example/models.py
--rw-rw-rw-   0        0        0      195 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/example/routers.py
--rw-rw-rw-   0        0        0      400 2023-06-16 05:42:12.000000 fastgenerateapi-0.0.4/fastgenerateapi/example/views.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.814186 fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/__init__.py
--rw-rw-rw-   0        0        0      694 2023-06-16 00:57:41.000000 fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/base_model.py
--rw-rw-rw-   0        0        0     2814 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/json_encoders.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.823157 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/
--rw-rw-rw-   0        0        0      472 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/__init__.py
--rw-rw-rw-   0        0        0     4305 2023-06-16 00:44:35.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/common_function.py
--rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/create_schema_factory.py
--rw-rw-rw-   0        0        0     1284 2023-06-16 02:48:31.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/filter_schema_factory.py
--rw-rw-rw-   0        0        0     3303 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_all_schema_factory.py
--rw-rw-rw-   0        0        0     2194 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_one_schema_factory.py
--rw-rw-rw-   0        0        0     3187 2023-06-16 06:21:06.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
--rw-rw-rw-   0        0        0     1647 2023-06-16 00:43:56.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/response_factory.py
--rw-rw-rw-   0        0        0     2292 2023-06-16 01:54:38.000000 fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/update_schema_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.826149 fastgenerateapi-0.0.4/fastgenerateapi/settings/
--rw-rw-rw-   0        0        0        6 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/settings/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-16 00:40:41.000000 fastgenerateapi-0.0.4/fastgenerateapi/settings/register_settings.py
--rw-rw-rw-   0        0        0     3952 2023-06-16 06:01:18.000000 fastgenerateapi-0.0.4/fastgenerateapi/settings/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.829141 fastgenerateapi-0.0.4/fastgenerateapi/utils/
--rw-rw-rw-   0        0        0        0 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/utils/__init__.py
--rw-rw-rw-   0        0        0      121 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/utils/exception.py
--rw-rw-rw-   0        0        0      670 2023-06-15 11:43:17.000000 fastgenerateapi-0.0.4/fastgenerateapi/utils/parse_str.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:33:07.779753 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/
--rw-rw-rw-   0        0        0      664 2023-06-16 06:33:07.000000 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2443 2023-06-16 06:33:07.000000 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 06:33:07.000000 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-16 06:33:07.000000 fastgenerateapi-0.0.4/fastgenerateapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 06:33:07.830804 fastgenerateapi-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3832 2023-06-15 11:33:14.000000 fastgenerateapi-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.159244 fastgenerateapi-0.0.5/
+-rw-rw-rw-   0        0        0    35821 2023-06-18 00:11:53.000000 fastgenerateapi-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      664 2023-06-18 06:11:07.159244 fastgenerateapi-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.137299 fastgenerateapi-0.0.5/fastgenerateapi/
+-rw-rw-rw-   0        0        0     1022 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.5/fastgenerateapi/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.5/fastgenerateapi/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.143283 fastgenerateapi-0.0.5/fastgenerateapi/api_view/
+-rw-rw-rw-   0        0        0       14 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/api_view.py
+-rw-rw-rw-   0        0        0     9189 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/base_view.py
+-rw-rw-rw-   0        0        0     4177 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/create_view.py
+-rw-rw-rw-   0        0        0     3628 2023-06-18 03:11:06.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/delete_tree_view.py
+-rw-rw-rw-   0        0        0     3035 2023-06-18 03:11:06.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/delete_view.py
+-rw-rw-rw-   0        0        0     7469 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/get_all_view.py
+-rw-rw-rw-   0        0        0     3077 2023-06-18 01:49:07.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/get_one_view.py
+-rw-rw-rw-   0        0        0     9795 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/get_relation_view.py
+-rw-rw-rw-   0        0        0     7275 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/get_tree_view.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.146275 fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/__init__.py
+-rw-rw-rw-   0        0        0     4453 2023-06-18 04:59:15.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/base_mixin.py
+-rw-rw-rw-   0        0        0     3826 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/dbmodel_mixin.py
+-rw-rw-rw-   0        0        0      266 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/get_mixin.py
+-rw-rw-rw-   0        0        0     2290 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/response_mixin.py
+-rw-rw-rw-   0        0        0      317 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/save_mixin.py
+-rw-rw-rw-   0        0        0    13029 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/tool_mixin.py
+-rw-rw-rw-   0        0        0     3070 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/switch_view.py
+-rw-rw-rw-   0        0        0     3553 2023-06-18 04:41:09.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/update_relation_view.py
+-rw-rw-rw-   0        0        0     4006 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/api_view/update_view.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.148270 fastgenerateapi-0.0.5/fastgenerateapi/controller/
+-rw-rw-rw-   0        0        0      316 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/controller/__init__.py
+-rw-rw-rw-   0        0        0     3391 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/controller/filter_controller.py
+-rw-rw-rw-   0        0        0     2385 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/controller/router_controller.py
+-rw-rw-rw-   0        0        0     2298 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/controller/rpc_controller.py
+-rw-rw-rw-   0        0        0      873 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/controller/search_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.150265 fastgenerateapi-0.0.5/fastgenerateapi/data_type/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/data_type/__init__.py
+-rw-rw-rw-   0        0        0      727 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/data_type/data_type.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.151261 fastgenerateapi-0.0.5/fastgenerateapi/deps/
+-rw-rw-rw-   0        0        0      160 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/deps/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/deps/filter_params_deps.py
+-rw-rw-rw-   0        0        0     3171 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/deps/paginator_deps.py
+-rw-rw-rw-   0        0        0     1264 2023-06-18 01:09:58.000000 fastgenerateapi-0.0.5/fastgenerateapi/deps/tree_params_deps.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.153256 fastgenerateapi-0.0.5/fastgenerateapi/example/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/example/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/example/models.py
+-rw-rw-rw-   0        0        0      195 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/example/routers.py
+-rw-rw-rw-   0        0        0      400 2023-06-18 00:07:39.000000 fastgenerateapi-0.0.5/fastgenerateapi/example/views.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.153256 fastgenerateapi-0.0.5/fastgenerateapi/pydantic_utils/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/pydantic_utils/__init__.py
+-rw-rw-rw-   0        0        0      694 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/pydantic_utils/base_model.py
+-rw-rw-rw-   0        0        0     2814 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/pydantic_utils/json_encoders.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.157246 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/
+-rw-rw-rw-   0        0        0      472 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/__init__.py
+-rw-rw-rw-   0        0        0     4305 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/common_function.py
+-rw-rw-rw-   0        0        0     2292 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/create_schema_factory.py
+-rw-rw-rw-   0        0        0     1284 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/filter_schema_factory.py
+-rw-rw-rw-   0        0        0     3303 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/get_all_schema_factory.py
+-rw-rw-rw-   0        0        0     2194 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/get_one_schema_factory.py
+-rw-rw-rw-   0        0        0     2391 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/get_relation_schema_factory.py
+-rw-rw-rw-   0        0        0     3187 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/get_tree_schema_factory.py
+-rw-rw-rw-   0        0        0     1647 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/response_factory.py
+-rw-rw-rw-   0        0        0     2292 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/update_schema_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.158242 fastgenerateapi-0.0.5/fastgenerateapi/settings/
+-rw-rw-rw-   0        0        0        6 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/settings/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/settings/register_settings.py
+-rw-rw-rw-   0        0        0     4064 2023-06-18 06:05:08.000000 fastgenerateapi-0.0.5/fastgenerateapi/settings/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.159244 fastgenerateapi-0.0.5/fastgenerateapi/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      121 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/utils/exception.py
+-rw-rw-rw-   0        0        0      670 2023-06-18 00:07:40.000000 fastgenerateapi-0.0.5/fastgenerateapi/utils/parse_str.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:11:07.138301 fastgenerateapi-0.0.5/fastgenerateapi.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-06-18 06:11:06.000000 fastgenerateapi-0.0.5/fastgenerateapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2601 2023-06-18 06:11:07.000000 fastgenerateapi-0.0.5/fastgenerateapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 06:11:06.000000 fastgenerateapi-0.0.5/fastgenerateapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-18 06:11:06.000000 fastgenerateapi-0.0.5/fastgenerateapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 06:11:07.159244 fastgenerateapi-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2023-06-18 00:11:54.000000 fastgenerateapi-0.0.5/setup.py
```

### Comparing `fastgenerateapi-0.0.4/LICENSE` & `fastgenerateapi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/PKG-INFO` & `fastgenerateapi-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/__init__.py` & `fastgenerateapi-0.0.5/fastgenerateapi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 #  Y8ooooo. 88'  `88 88   88 88 88'  `88 88'  `88 88'  `88
 #        88 88    88 88   88 88 88.  .88 88    88 88.  .88
 #  `88888P' dP    dP dP   dP dP `88888P8 dP    dP `8888P88
 #                                                      .88
 #                                                  d8888P
 
 
-from fastgenerateapi.settings.register_settings import settings
 from fastgenerateapi.api_view.api_view import APIView, CreateView, GetOneView, GetAllView, UpdateView, DeleteView, \
     SwitchView
 from fastgenerateapi.api_view.get_tree_view import GetTreeView
 from fastgenerateapi.api_view.delete_tree_view import DeleteTreeView
 from fastgenerateapi.api_view.base_view import BaseView
-from fastgenerateapi.settings.settings import SettingsModel
 
+# 多对多关联 >> 查和改
+from fastgenerateapi.api_view.get_relation_view import GetRelationView
+from fastgenerateapi.api_view.update_relation_view import UpdateRelationView
 
+# 查看配置模型
+from fastgenerateapi.settings.settings import SettingsModel
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/api_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/api_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/base_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/base_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/create_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/create_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/delete_tree_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/delete_tree_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,28 @@
     delete_tree_schema: Optional[Type[BaseModel]] = IDList
     """
     delete_route: 删除路由开关，可以放依赖函数列表
     delete_schema: 删除请求模型
     """
 
     @atomic()
-    async def destroy_tree(self, request_data, request, *args, **kwargs):
+    async def destroy_tree(self, request_data, *args, **kwargs):
         delete_id_list = request_data.id_list
         parent_id_list = delete_id_list
         while parent_id_list:
-            children_id_list = await self.queryset.filter(parent_id__in=parent_id_list).values_list(self._get_pk_field(self.model_class), flat=True)
+            children_id_list = await self.queryset.filter(
+                parent_id__in=parent_id_list).values_list(self._get_pk_field(self.model_class), flat=True)
             if children_id_list:
                 delete_id_list += children_id_list
-                parent_id_list = delete_id_list
+                parent_id_list = children_id_list
             else:
                 break
 
         request_data.id_list = delete_id_list
-        queryset = await self.get_del_tree_queryset(request_data=request_data, request=request, *args, **kwargs)
+        queryset = await self.get_del_tree_queryset(request_data=request_data, *args, **kwargs)
         if unique_fields := self._get_unique_fields(self.model_class):
             for model in await queryset:
                 model.is_active = False
                 for field in unique_fields:
                     try:
                         setattr(model, field, getattr(model, field) + f"__{int(time.time() * 1000)}")
                     except Exception as e:
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/delete_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/delete_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     delete_schema: Optional[Type[BaseModel]] = IDList
     """
     delete_route: 删除路由开关，可以放依赖函数列表
     delete_schema: 删除请求模型
     """
 
     @atomic()
-    async def destroy(self, request_data, request, *args, **kwargs):
-        queryset = await self.get_del_queryset(request_data=request_data, request=request, *args, **kwargs)
+    async def destroy(self, request_data, *args, **kwargs):
+        queryset = await self.get_del_queryset(request_data=request_data, *args, **kwargs)
 
         if unique_fields := self._get_unique_fields(self.model_class):
             for model in await queryset:
                 model.is_active = False
                 for field in unique_fields:
                     try:
                         setattr(model, field, getattr(model, field) + f"__{int(time.time() * 1000)}")
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_all_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/get_all_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,39 +25,39 @@
     get_all_route: Union[bool, DEPENDENCIES] = True
     get_all_schema: Optional[Type[BaseModel]] = None
     search_fields: Union[None, list] = None
     filter_fields: Union[None, list] = None
     order_by_fields: Union[None, list] = None
     """
     get_all_route: 获取详情路由开关，可以放依赖函数列表
-    list_schema: 返回序列化
+    get_all_schema: 返回序列化
         优先级：  
             - 传入参数
             - 模型层get_all_include和get_all_exclude(同时存在交集)
             - get_one_schemas
     search_fields: search搜索对应字段 
         example：("name__contains", str, "name") 类型是str的时候可以省略，没有第三个值时，自动双下划线转单下划线
     filter_fields: 筛选对应字段
         example： name__contains or (create_at__gt, datetime) or (create_at__gt, datetime, create_time)
     order_by_fields: 排序对应字段
     """
 
-    async def get_all(self, search: str, filters: dict, request, *args, **kwargs) -> Union[BaseModel, dict, None]:
-        queryset = await self.get_queryset(search=search, filters=filters, request=request, *args, **kwargs)
+    async def get_all(self, search: str, filters: dict, *args, **kwargs) -> Union[BaseModel, dict, None]:
+        queryset = await self.get_queryset(search=search, filters=filters, *args, **kwargs)
 
-        return await self.pagination_data(queryset=queryset, request=request, fields=None, *args, **kwargs)
+        return await self.pagination_data(queryset=queryset, *args, **kwargs)
 
     async def get_queryset(self, search: str, filters: dict, *args, **kwargs) -> QuerySet:
         """
         处理search搜索；处理筛选字段；处理外键预加载；处理排序
         """
         queryset = self.search_controller.query(queryset=self.queryset, value=search)
         queryset = self.filter_queryset(queryset, filters)
-        queryset = self.filter_controller.query(queryset=queryset, values=filters).prefetch_related(
-            *self.prefetch_related_fields.keys()).order_by(*self.order_by_fields or [])
+        queryset = self.filter_controller.query(queryset=queryset, values=filters)
+        queryset = queryset.prefetch_related(*self.prefetch_related_fields.keys()).order_by(*self.order_by_fields or [])
 
         return queryset
 
     def filter_queryset(self, queryset: QuerySet, filters: dict) -> QuerySet:
         """
         处理filters
             example： value = filters.pop(value, None)   queryset = queryset.filter(field=value+string)
@@ -75,15 +75,15 @@
             queryset: QuerySet,
             paginator,
             fields: List[Union[str, tuple]] = None,
             *args, **kwargs
     ) -> Union[dict, str, None, BaseModel]:
 
         data_list = []
-        if getattr(paginator, settings.app_settings.DETERMINE_WHETHER_PAGE_FIELD):
+        if getattr(paginator, settings.app_settings.DETERMINE_WHETHER_PAGE_FIELD) == settings.app_settings.DETERMINE_NO_PAGE_VALUE:
             model_list = await queryset.all()
         else:
             count = await queryset.count()
             current_num = getattr(paginator, settings.app_settings.CURRENT_PAGE_FIELD)
             page_size = getattr(paginator, settings.app_settings.PAGE_SIZE_FIELD)
             queryset = queryset.offset(cast(int, (current_num - 1) * page_size))
             model_list = await queryset.limit(page_size)
@@ -97,15 +97,15 @@
             await self.set_get_all_model(model)
 
             if fields:
                 data_list.append(await self.getattr_model(model=model, fields=fields))
             else:
                 data_list.append(self.get_all_schema.from_orm(model))
 
-        if getattr(paginator, settings.app_settings.DETERMINE_WHETHER_PAGE_FIELD):
+        if getattr(paginator, settings.app_settings.DETERMINE_WHETHER_PAGE_FIELD) == settings.app_settings.DETERMINE_NO_PAGE_VALUE:
             return self.get_list_schema(**{
                 settings.app_settings.LIST_RESPONSE_FIELD: data_list,
             })
 
         return self.get_page_schema(**{
             settings.app_settings.CURRENT_PAGE_FIELD: current_num,
             settings.app_settings.PAGE_SIZE_FIELD: page_size,
@@ -142,15 +142,15 @@
         self.get_all_schema = self.get_all_schema or get_all_schema_factory(self.model_class) or self.get_one_schema if hasattr(self, "get_one_schema") else get_one_schema_factory(self.model_class)
         self.get_page_schema = get_page_schema_factory(self.get_all_schema)
         self.get_list_schema = get_list_schema_factory(self.get_all_schema)
         self.get_all_response_schema = response_factory(self.get_page_schema, name="GetPage")
 
         if self.get_all_route:
             doc = self.get_all.__doc__
-            summary = doc.strip().split("\n")[0] if self.get_all.__doc__ else "Get All"
+            summary = doc.strip().split("\n")[0] if doc else "Get All"
             path = f"/{settings.app_settings.ROUTER_GET_ALL_SUFFIX_FIELD}" if settings.app_settings.ROUTER_WHETHER_ADD_SUFFIX else ""
             self._add_api_route(
                 path=path,
                 endpoint=self._get_all_decorator(),
                 methods=["GET"],
                 response_model=self.get_all_response_schema,
                 summary=summary,
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_one_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/get_one_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 *args, **kwargs
             )
             return self.success(data=data)
         return route
 
     def _handler_get_one_settings(self):
 
-        self.get_one_schema = self.get_one_schema or get_one_schema_factory(model_class=self.model_class)
+        self.get_one_schema = self.schema or self.get_one_schema or get_one_schema_factory(model_class=self.model_class)
         self.get_one_response_schema = response_factory(self.get_one_schema, name="GetOne")
 
         if self.get_one_route:
             doc = self.get_one.__doc__
             summary = doc.strip().split("\n")[0] if self.get_one.__doc__ else "Get One"
             path = f"/{settings.app_settings.ROUTER_GET_ONE_SUFFIX_FIELD}/{'{pk}'}" if settings.app_settings.ROUTER_WHETHER_ADD_SUFFIX else "/{pk}"
             self._add_api_route(
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/get_tree_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/get_tree_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,44 +19,44 @@
 from fastgenerateapi.deps.tree_params_deps import tree_params_deps
 from fastgenerateapi.pydantic_utils.base_model import BaseModel
 from fastgenerateapi.schemas_factory import get_one_schema_factory, response_factory
 from fastgenerateapi.schemas_factory.get_tree_schema_factory import get_tree_schema_factory
 from fastgenerateapi.settings.register_settings import settings
 
 
-class GetTreeView(BaseView, GetMixin):
+class GetTreeView(BaseView):
 
     get_tree_route: Union[bool, DEPENDENCIES] = True
     get_tree_schema: Optional[Type[BaseModel]] = None
     search_fields: Union[None, list] = None
     filter_fields: Union[None, list] = None
     order_by_fields: Union[None, list] = None
     """
-    get_all_route: 获取详情路由开关，可以放依赖函数列表
-    list_schema: 返回序列化
+    get_tree_route: 获取梳妆数据路由开关，可以放依赖函数列表
+    get_tree_schema: 返回序列化
         优先级：  
             - 传入参数
-            - 模型层get_all_include和get_all_exclude(同时存在交集)
-            - get_one_schemas
+            - 模型层get_tree_include和get_tree_exclude(同时存在交集)
+            - include和exclude(同时存在交集)
     search_fields: search搜索对应字段 
         example：("name__contains", str, "name") 类型是str的时候可以省略，没有第三个值时，自动双下划线转单下划线
     filter_fields: 筛选对应字段
         example： name__contains or (create_at__gt, datetime) or (create_at__gt, datetime, create_time)
     order_by_fields: 排序对应字段
     """
 
     async def get_tree(
             self,
-            begin_id: Optional[str],
+            node_id: Optional[str],
             search: str,
             filters: dict,
             request, *args, **kwargs
     ) -> Union[BaseModel, dict, None]:
-        if begin_id:
-            queryset = self.queryset.filter(pk=begin_id).prefetch_related(settings.app_settings.DEFAULT_TREE_PARENT_FIELD)
+        if node_id:
+            queryset = self.queryset.filter(pk=node_id).prefetch_related(settings.app_settings.DEFAULT_TREE_PARENT_FIELD)
             queryset = await self.get_tree_queryset(queryset, search, filters)
             if not (top_node := await queryset.first()):
                 raise NOT_FOUND
             top_nodes = [top_node]
         else:
             queryset = self.queryset.filter(
                 eval(f"Q({settings.app_settings.DEFAULT_TREE_PARENT_FIELD + '_id'}={None})")
@@ -69,18 +69,18 @@
 
         return self.get_tree_data_schema(**{settings.app_settings.LIST_RESPONSE_FIELD: data_list})
 
     async def get_tree_queryset(self, queryset: QuerySet, search: str, filters: dict, *args, **kwargs) -> QuerySet:
         """
         处理search搜索；处理筛选字段；处理外键预加载；处理排序
         """
-        queryset = self.search_controller.query(queryset=queryset, value=search)
-        queryset = self.filter_tree_queryset(queryset, filters)
-        queryset = self.filter_controller.query(queryset=queryset, values=filters).prefetch_related(
-            *self.prefetch_related_fields.keys()).order_by(*self.order_by_fields or [])
+        # queryset = self.search_controller.query(queryset=queryset, value=search)
+        # queryset = self.filter_tree_queryset(queryset, filters)
+        # queryset = self.filter_controller.query(queryset=queryset, values=filters)
+        queryset = queryset.prefetch_related(*self.prefetch_related_fields.keys()).order_by(*self.order_by_fields or [])
 
         return queryset
 
     def filter_tree_queryset(self, queryset: QuerySet, filters: dict) -> QuerySet:
         """
         处理filters
             example： value = filters.pop(value, None)   queryset = queryset.filter(field=value+string)
@@ -107,20 +107,20 @@
         """
         return model
 
     def _get_tree_decorator(self, *args: Any, **kwargs: Any) -> DecoratedCallable:
         async def route(
                 request: Request,
                 search: str = Query(default="", description="搜索"),
-                begin_id: Optional[str] = Depends(tree_params_deps()),
+                node_id: Optional[str] = Depends(tree_params_deps()),
                 filters: dict = Depends(filter_params_deps(model_class=self.model_class, fields=self.filter_fields)),
         ) -> JSONResponse:
             data = await self.get_tree(
                 search=search,
-                begin_id=begin_id,
+                node_id=node_id,
                 filters=filters,
                 request=request,
                 *args,
                 **kwargs
             )
             return self.success(data=data)
         return route
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/base_mixin.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/base_mixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,20 +19,29 @@
     def queryset(self) -> QuerySet:
         if not self.model_class:
             return self.error(msg="model_class not allow None")
         queryset = self.model_class.filter(
             eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
         return queryset
 
+    @property
+    def relation_queryset(self) -> QuerySet:
+        if not self.relation_model_class:
+            return self.error(msg="relation_model_class not allow None")
+        queryset = self.relation_model_class.filter(
+            eval(f"Q({settings.app_settings.WHETHER_DELETE_FIELD}='{settings.app_settings.ACTIVE_DEFAULT_VALUE}')"))
+        return queryset
+
     @staticmethod
     def _get_routes(is_controller_field: bool = False) -> List[str]:
         if is_controller_field:
             return ["get_one_route", "get_all_route", "get_tree_route", "create_route",
-                    "update_route", "delete_route", "delete_tree_route", "switch_route_fields"]
-        return ["get_one", "get_all", "get_tree", "create",  "update", "destroy", "destroy_tree", "switch"]
+                    "update_route", "update_relation_route", "delete_route", "delete_tree_route", "switch_route_fields"]
+        return ["get_one", "get_all", "get_tree", "create", "update", "update_relation", "destroy", "destroy_tree",
+                "switch"]
 
     @classmethod
     def _get_cls_func(cls):
         func_list = inspect.getmembers(cls, inspect.isfunction)
         return [func[0] for func in func_list if func[0].startswith("view_")]
 
     def _add_api_route(
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/dbmodel_mixin.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/dbmodel_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/response_mixin.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/response_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/mixin/tool_mixin.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/mixin/tool_mixin.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/switch_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/switch_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/api_view/update_view.py` & `fastgenerateapi-0.0.5/fastgenerateapi/api_view/update_view.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/controller/filter_controller.py` & `fastgenerateapi-0.0.5/fastgenerateapi/controller/filter_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/controller/router_controller.py` & `fastgenerateapi-0.0.5/fastgenerateapi/controller/router_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/controller/rpc_controller.py` & `fastgenerateapi-0.0.5/fastgenerateapi/controller/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/controller/search_controller.py` & `fastgenerateapi-0.0.5/fastgenerateapi/controller/search_controller.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/data_type/data_type.py` & `fastgenerateapi-0.0.5/fastgenerateapi/data_type/data_type.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/deps/filter_params_deps.py` & `fastgenerateapi-0.0.5/fastgenerateapi/deps/filter_params_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/deps/paginator_deps.py` & `fastgenerateapi-0.0.5/fastgenerateapi/deps/paginator_deps.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/deps/tree_params_deps.py` & `fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/filter_schema_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,40 @@
-from typing import Type, Any, Optional
-
-from fastapi import Depends
-from pydantic.fields import FieldInfo
-
-from fastgenerateapi.settings.register_settings import settings
+from typing import Type, Union
 
+from fastapi import Query
 from fastgenerateapi.pydantic_utils.base_model import QueryConfig
 from pydantic import BaseModel, create_model
+from pydantic.fields import FieldInfo
 
+from fastgenerateapi.api_view.mixin.dbmodel_mixin import DBModelMixin
+from fastgenerateapi.controller.filter_controller import BaseFilter
+from tortoise import Model
 
-def tree_params_deps():
+
+def filter_schema_factory(model_class: Type[Model], fields: list[str, tuple[str, Type], BaseFilter] = None):
     """
-        生成 tree 开始筛选字段的依赖
+        generate filter schema
     """
-    filter_tree_params_model: Type[BaseModel] = create_model(
-        __model_name="TreeFilterParams", **{
-            settings.app_settings.DEFAULT_TREE_FILTER_FIELD: (Optional[str], FieldInfo(default=None, description="起始节点ID"))
-        },  __config__=QueryConfig)
-
-    def filter_query(filter_params: filter_tree_params_model = Depends(filter_tree_params_model)) -> dict[str, Any]:
-        """
-            filter 筛选字段依赖
-        :param filter_params:
-        :return:
-        """
-        result = getattr(filter_params, settings.app_settings.DEFAULT_TREE_FILTER_FIELD, None)
+    model_fields = {}
+
+    for field_info in fields or []:
+        if not isinstance(field_info, BaseFilter):
+            field_info = BaseFilter(field_info)
+        f = field_info.filter_field
+        t = field_info.field_type
+
+        model_fields.update({
+            f: (
+                Union[t, str],
+                FieldInfo(
+                    title=f"{f}",
+                    default=Query(""),
+                    description=f"{DBModelMixin.get_field_description(model_class, field_info.model_field)}"
+                ))
+        })
+
+    filter_params_model: Type[BaseModel] = create_model(__model_name="CommonFilterParams", **model_fields, __config__=QueryConfig)
 
-        return result or None
+    return filter_params_model
 
-    return filter_query
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/example/models.py` & `fastgenerateapi-0.0.5/fastgenerateapi/example/models.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/base_model.py` & `fastgenerateapi-0.0.5/fastgenerateapi/pydantic_utils/base_model.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/pydantic_utils/json_encoders.py` & `fastgenerateapi-0.0.5/fastgenerateapi/pydantic_utils/json_encoders.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/common_function.py` & `fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/common_function.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/create_schema_factory.py` & `fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/create_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_all_schema_factory.py` & `fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/get_all_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_one_schema_factory.py` & `fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/get_one_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/get_tree_schema_factory.py` & `fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/get_tree_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/response_factory.py` & `fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/response_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/schemas_factory/update_schema_factory.py` & `fastgenerateapi-0.0.5/fastgenerateapi/schemas_factory/update_schema_factory.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/settings/settings.py` & `fastgenerateapi-0.0.5/fastgenerateapi/settings/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 class AppSettings(BaseSettings):
     # 分页对应字段以及配置默认值
     CURRENT_PAGE_FIELD: Optional[str] = Field(default='page', description="当前页字段")
     PAGE_SIZE_FIELD: Optional[str] = Field(default='page_size', description="每页数量字段")
     TOTAL_SIZE_FIELD: Optional[str] = Field(default='total', description="统计数量字段")
     DETERMINE_WHETHER_PAGE_FIELD: Optional[str] = Field(default='no_page', description="判断是否分页字段")
-    DEFAULT_PAGE_SIZE: Optional[int] = Field(default=10, description="默认每页数量")
+    DETERMINE_NO_PAGE_VALUE: Optional[bool] = Field(default=True, description="分页对应的布尔值")
     DEFAULT_WHETHER_PAGE: Optional[bool] = Field(default=False, description="默认是否分页")
+    DEFAULT_PAGE_SIZE: Optional[int] = Field(default=10, description="默认每页数量")
     DEFAULT_MAX_PAGE_SIZE: Optional[int] = Field(default=200, description="默认最大每页数量")
 
     # 路由后缀字段是否添加以及配置默认值
     ROUTER_WHETHER_ADD_SUFFIX: Optional[bool] = Field(default=True, description="增删改查路由是否添加后缀")
     ROUTER_CREATE_SUFFIX_FIELD: Optional[str] = Field(default='create', description="创建路由后缀字段")
     ROUTER_GET_ONE_SUFFIX_FIELD: Optional[str] = Field(default='get-one', description="获取一个路由后缀字段")
     ROUTER_GET_ALL_SUFFIX_FIELD: Optional[str] = Field(default='get-all', description="获取列表路由后缀字段")
@@ -27,15 +28,15 @@
     WHETHER_DELETE_FIELD: Optional[str] = Field(default="is_active", description="是否删除字段")
     ACTIVE_DEFAULT_VALUE: Optional[bool] = Field(default=True, description="有效的默认值")
     GET_EXCLUDE_ACTIVE_VALUE: Optional[bool] = Field(default=True, description="查询结果是否排除有效字段")
     CREATE_EXCLUDE_ACTIVE_VALUE: Optional[bool] = Field(default=True, description="创建是否排除有效字段")
     UPDATE_EXCLUDE_ACTIVE_VALUE: Optional[bool] = Field(default=True, description="修改是否排除有效字段")
     DEFAULT_TREE_PARENT_FIELD: Optional[str] = Field(default="parent", description="默认递归父级字段")
     DEFAULT_TREE_CHILDREN_FIELD: Optional[str] = Field(default="children", description="默认递归子级字段")
-    DEFAULT_TREE_FILTER_FIELD: Optional[str] = Field(default="begin_id", description="默认递归起点筛选字段")
+    DEFAULT_TREE_FILTER_FIELD: Optional[str] = Field(default="node_id", description="默认递归筛选开始节点字段")
 
     # 返回格式字段配置默认值
     CODE_RESPONSE_FIELD: Optional[bool] = Field(default=True, description="code返回字段")
     SUCCESS_RESPONSE_FIELD: Optional[bool] = Field(default=True, description="success返回字段")
     MESSAGE_RESPONSE_FIELD: Optional[str] = Field(default="message", description="消息返回字段")
     DATA_RESPONSE_FIELD: Optional[str] = Field(default="data", description="数据返回字段")
     LIST_RESPONSE_FIELD: Optional[str] = Field(default='list', description="列表页返回字段")
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi/utils/parse_str.py` & `fastgenerateapi-0.0.5/fastgenerateapi/utils/parse_str.py`

 * *Files identical despite different names*

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi.egg-info/PKG-INFO` & `fastgenerateapi-0.0.5/fastgenerateapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastgenerateapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: FastAPIView Class View
 Author: ShiLiang
 Author-email: 2509144896@qq.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastgenerateapi-0.0.4/fastgenerateapi.egg-info/SOURCES.txt` & `fastgenerateapi-0.0.5/fastgenerateapi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 fastgenerateapi/api_view/api_view.py
 fastgenerateapi/api_view/base_view.py
 fastgenerateapi/api_view/create_view.py
 fastgenerateapi/api_view/delete_tree_view.py
 fastgenerateapi/api_view/delete_view.py
 fastgenerateapi/api_view/get_all_view.py
 fastgenerateapi/api_view/get_one_view.py
+fastgenerateapi/api_view/get_relation_view.py
 fastgenerateapi/api_view/get_tree_view.py
 fastgenerateapi/api_view/switch_view.py
+fastgenerateapi/api_view/update_relation_view.py
 fastgenerateapi/api_view/update_view.py
 fastgenerateapi/api_view/mixin/__init__.py
 fastgenerateapi/api_view/mixin/base_mixin.py
 fastgenerateapi/api_view/mixin/dbmodel_mixin.py
 fastgenerateapi/api_view/mixin/get_mixin.py
 fastgenerateapi/api_view/mixin/response_mixin.py
 fastgenerateapi/api_view/mixin/save_mixin.py
@@ -44,14 +46,15 @@
 fastgenerateapi/pydantic_utils/json_encoders.py
 fastgenerateapi/schemas_factory/__init__.py
 fastgenerateapi/schemas_factory/common_function.py
 fastgenerateapi/schemas_factory/create_schema_factory.py
 fastgenerateapi/schemas_factory/filter_schema_factory.py
 fastgenerateapi/schemas_factory/get_all_schema_factory.py
 fastgenerateapi/schemas_factory/get_one_schema_factory.py
+fastgenerateapi/schemas_factory/get_relation_schema_factory.py
 fastgenerateapi/schemas_factory/get_tree_schema_factory.py
 fastgenerateapi/schemas_factory/response_factory.py
 fastgenerateapi/schemas_factory/update_schema_factory.py
 fastgenerateapi/settings/__init__.py
 fastgenerateapi/settings/register_settings.py
 fastgenerateapi/settings/settings.py
 fastgenerateapi/utils/__init__.py
```

### Comparing `fastgenerateapi-0.0.4/setup.py` & `fastgenerateapi-0.0.5/setup.py`

 * *Files identical despite different names*


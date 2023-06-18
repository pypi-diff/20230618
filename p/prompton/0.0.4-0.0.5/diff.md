# Comparing `tmp/prompton-0.0.4.tar.gz` & `tmp/prompton-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompton-0.0.4.tar", max compression
+gzip compressed data, was "prompton-0.0.5.tar", max compression
```

## Comparing `prompton-0.0.4.tar` & `prompton-0.0.5.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.4/README.md
--rw-r--r--   0        0        0     2408 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/client.py
--rw-r--r--   0        0        0      348 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      367 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/not_found_error.py
--rw-r--r--   0        0        0      250 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/unauthorized_error.py
--rw-r--r--   0        0        0      257 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      268 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/authentication/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/authentication/client.py
--rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/inferences/__init__.py
--rw-r--r--   0        0        0     9839 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/inferences/client.py
--rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/orgs/__init__.py
--rw-r--r--   0        0        0    14702 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/orgs/client.py
--rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/prompt_versions/__init__.py
--rw-r--r--   0        0        0    16684 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/prompt_versions/client.py
--rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/prompts/__init__.py
--rw-r--r--   0        0        0    15828 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/server_status/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/server_status/client.py
--rw-r--r--   0        0        0       65 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/users/__init__.py
--rw-r--r--   0        0        0    13165 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/resources/users/client.py
--rw-r--r--   0        0        0     3055 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/__init__.py
--rw-r--r--   0        0        0      900 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/api_status_response.py
--rw-r--r--   0        0        0      936 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/body_get_access_token_extended_token_post.py
--rw-r--r--   0        0        0     1274 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_config.py
--rw-r--r--   0        0        0      152 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_config_stop.py
--rw-r--r--   0        0        0     1458 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_request.py
--rw-r--r--   0        0        0      153 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_request_stop.py
--rw-r--r--   0        0        0     1012 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_chat_completition_response.py
--rw-r--r--   0        0        0      856 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_completition_choice.py
--rw-r--r--   0        0        0      843 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_message.py
--rw-r--r--   0        0        0      666 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_role.py
--rw-r--r--   0        0        0      809 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/chat_gpt_token_usage.py
--rw-r--r--   0        0        0      773 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/db_status.py
--rw-r--r--   0        0        0      843 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/http_validation_error.py
--rw-r--r--   0        0        0     2205 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_create_by_prompt_id.py
--rw-r--r--   0        0        0     1805 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_create_by_prompt_version_id.py
--rw-r--r--   0        0        0      926 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_post_response.py
--rw-r--r--   0        0        0      293 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_post_response_response.py
--rw-r--r--   0        0        0     2730 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_read.py
--rw-r--r--   0        0        0      285 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_read_response.py
--rw-r--r--   0        0        0      965 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_request_data.py
--rw-r--r--   0        0        0     1229 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_response_data.py
--rw-r--r--   0        0        0     1051 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_response_error.py
--rw-r--r--   0        0        0     1049 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/inference_response_status.py
--rw-r--r--   0        0        0      330 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/new_inference_request.py
--rw-r--r--   0        0        0     1028 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/org_read.py
--rw-r--r--   0        0        0     1184 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_read.py
--rw-r--r--   0        0        0      507 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_status.py
--rw-r--r--   0        0        0      152 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_version_providers.py
--rw-r--r--   0        0        0     1651 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_version_read.py
--rw-r--r--   0        0        0      837 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/prompt_version_status.py
--rw-r--r--   0        0        0      767 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/token.py
--rw-r--r--   0        0        0     1236 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/user_read.py
--rw-r--r--   0        0        0      686 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/user_roles.py
--rw-r--r--   0        0        0      869 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-06-14 21:55:54.000000 prompton-0.0.4/prompton/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      450 2023-06-14 23:07:02.809554 prompton-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.5/README.md
+-rw-r--r--   0        0        0     2450 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/client.py
+-rw-r--r--   0        0        0      348 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      367 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/not_found_error.py
+-rw-r--r--   0        0        0      250 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      257 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      268 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/authentication/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/authentication/client.py
+-rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/inferences/__init__.py
+-rw-r--r--   0        0        0     9839 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/inferences/client.py
+-rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/orgs/__init__.py
+-rw-r--r--   0        0        0    14702 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/orgs/client.py
+-rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/prompt_versions/__init__.py
+-rw-r--r--   0        0        0    16684 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/prompt_versions/client.py
+-rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    15828 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/server_status/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/server_status/client.py
+-rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/users/__init__.py
+-rw-r--r--   0        0        0    13165 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/users/client.py
+-rw-r--r--   0        0        0     3121 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/api_status_response.py
+-rw-r--r--   0        0        0      936 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/body_get_access_token_extended_token_post.py
+-rw-r--r--   0        0        0     1274 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_config.py
+-rw-r--r--   0        0        0      152 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_config_stop.py
+-rw-r--r--   0        0        0     1458 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_request.py
+-rw-r--r--   0        0        0      153 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_request_stop.py
+-rw-r--r--   0        0        0     1012 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_response.py
+-rw-r--r--   0        0        0      856 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_completition_choice.py
+-rw-r--r--   0        0        0      843 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_message.py
+-rw-r--r--   0        0        0      666 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_role.py
+-rw-r--r--   0        0        0      809 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_token_usage.py
+-rw-r--r--   0        0        0      773 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/db_status.py
+-rw-r--r--   0        0        0      843 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/http_validation_error.py
+-rw-r--r--   0        0        0     2205 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_create_by_prompt_id.py
+-rw-r--r--   0        0        0     1805 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_create_by_prompt_version_id.py
+-rw-r--r--   0        0        0      813 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_error.py
+-rw-r--r--   0        0        0      926 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_post_response.py
+-rw-r--r--   0        0        0      293 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_post_response_response.py
+-rw-r--r--   0        0        0     2510 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_read.py
+-rw-r--r--   0        0        0      285 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_read_response.py
+-rw-r--r--   0        0        0      965 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_request_data.py
+-rw-r--r--   0        0        0     1229 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_response_data.py
+-rw-r--r--   0        0        0     1082 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_response_error.py
+-rw-r--r--   0        0        0     1049 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_response_status.py
+-rw-r--r--   0        0        0      330 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/new_inference_request.py
+-rw-r--r--   0        0        0     1136 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/org_read.py
+-rw-r--r--   0        0        0     1275 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_read.py
+-rw-r--r--   0        0        0      507 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_status.py
+-rw-r--r--   0        0        0      152 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_version_providers.py
+-rw-r--r--   0        0        0     1810 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_version_read.py
+-rw-r--r--   0        0        0      837 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_version_status.py
+-rw-r--r--   0        0        0      767 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/token.py
+-rw-r--r--   0        0        0     1327 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/user_read.py
+-rw-r--r--   0        0        0      686 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/user_roles.py
+-rw-r--r--   0        0        0      869 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      450 2023-06-18 18:13:00.945912 prompton-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.5/PKG-INFO
```

### Comparing `prompton-0.0.4/prompton/__init__.py` & `prompton-0.0.5/prompton/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     ChatGptMessage,
     ChatGptRole,
     ChatGptTokenUsage,
     DbStatus,
     HttpValidationError,
     InferenceCreateByPromptId,
     InferenceCreateByPromptVersionId,
+    InferenceError,
     InferencePostResponse,
     InferencePostResponseResponse,
     InferenceRead,
     InferenceReadResponse,
     InferenceRequestData,
     InferenceResponseData,
     InferenceResponseError,
@@ -53,14 +54,15 @@
     "ChatGptMessage",
     "ChatGptRole",
     "ChatGptTokenUsage",
     "DbStatus",
     "HttpValidationError",
     "InferenceCreateByPromptId",
     "InferenceCreateByPromptVersionId",
+    "InferenceError",
     "InferencePostResponse",
     "InferencePostResponseResponse",
     "InferenceRead",
     "InferenceReadResponse",
     "InferenceRequestData",
     "InferenceResponseData",
     "InferenceResponseError",
```

### Comparing `prompton-0.0.4/prompton/client.py` & `prompton-0.0.5/prompton/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/core/datetime_utils.py` & `prompton-0.0.5/prompton/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/core/jsonable_encoder.py` & `prompton-0.0.5/prompton/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/resources/authentication/client.py` & `prompton-0.0.5/prompton/resources/authentication/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/resources/inferences/client.py` & `prompton-0.0.5/prompton/resources/inferences/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/resources/orgs/client.py` & `prompton-0.0.5/prompton/resources/orgs/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/resources/prompt_versions/client.py` & `prompton-0.0.5/prompton/resources/prompt_versions/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/resources/prompts/client.py` & `prompton-0.0.5/prompton/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/resources/server_status/client.py` & `prompton-0.0.5/prompton/resources/server_status/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/resources/users/client.py` & `prompton-0.0.5/prompton/resources/users/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/__init__.py` & `prompton-0.0.5/prompton/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .chat_gpt_message import ChatGptMessage
 from .chat_gpt_role import ChatGptRole
 from .chat_gpt_token_usage import ChatGptTokenUsage
 from .db_status import DbStatus
 from .http_validation_error import HttpValidationError
 from .inference_create_by_prompt_id import InferenceCreateByPromptId
 from .inference_create_by_prompt_version_id import InferenceCreateByPromptVersionId
+from .inference_error import InferenceError
 from .inference_post_response import InferencePostResponse
 from .inference_post_response_response import InferencePostResponseResponse
 from .inference_read import InferenceRead
 from .inference_read_response import InferenceReadResponse
 from .inference_request_data import InferenceRequestData
 from .inference_response_data import InferenceResponseData
 from .inference_response_error import InferenceResponseError
@@ -48,14 +49,15 @@
     "ChatGptMessage",
     "ChatGptRole",
     "ChatGptTokenUsage",
     "DbStatus",
     "HttpValidationError",
     "InferenceCreateByPromptId",
     "InferenceCreateByPromptVersionId",
+    "InferenceError",
     "InferencePostResponse",
     "InferencePostResponseResponse",
     "InferenceRead",
     "InferenceReadResponse",
     "InferenceRequestData",
     "InferenceResponseData",
     "InferenceResponseError",
```

### Comparing `prompton-0.0.4/prompton/types/api_status_response.py` & `prompton-0.0.5/prompton/types/api_status_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/body_get_access_token_extended_token_post.py` & `prompton-0.0.5/prompton/types/body_get_access_token_extended_token_post.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/chat_gpt_chat_completition_config.py` & `prompton-0.0.5/prompton/types/chat_gpt_chat_completition_config.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/chat_gpt_chat_completition_request.py` & `prompton-0.0.5/prompton/types/chat_gpt_chat_completition_request.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/chat_gpt_chat_completition_response.py` & `prompton-0.0.5/prompton/types/chat_gpt_chat_completition_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/chat_gpt_completition_choice.py` & `prompton-0.0.5/prompton/types/chat_gpt_completition_choice.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/chat_gpt_message.py` & `prompton-0.0.5/prompton/types/chat_gpt_message.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/chat_gpt_role.py` & `prompton-0.0.5/prompton/types/chat_gpt_role.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/chat_gpt_token_usage.py` & `prompton-0.0.5/prompton/types/chat_gpt_token_usage.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/db_status.py` & `prompton-0.0.5/prompton/types/db_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/http_validation_error.py` & `prompton-0.0.5/prompton/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/inference_create_by_prompt_id.py` & `prompton-0.0.5/prompton/types/inference_create_by_prompt_id.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/inference_create_by_prompt_version_id.py` & `prompton-0.0.5/prompton/types/inference_create_by_prompt_version_id.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/inference_post_response.py` & `prompton-0.0.5/prompton/types/inference_post_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/inference_read.py` & `prompton-0.0.5/prompton/types/inference_read.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,46 +8,46 @@
 from ..core.datetime_utils import serialize_datetime
 from .inference_read_response import InferenceReadResponse
 from .inference_request_data import InferenceRequestData
 from .inference_response_status import InferenceResponseStatus
 
 
 class InferenceRead(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(alias="_id")
-    created_at: typing.Optional[str]
-    created_by_user_id: typing.Optional[str]
-    created_by_org_id: typing.Optional[str]
+    """
+    Base model for reading from MongoDB. Same as MongoBaseCreate but assumes all DB base fields are populated so generated clients doesn't requrie None checks
+    """
+
+    id: str = pydantic.Field(alias="_id")
+    created_at: str
+    created_by_user_id: str
+    created_by_org_id: str
     end_user_id: typing.Optional[str] = pydantic.Field(
         description=(
             "The API consumer's internal user reference for metrics. It is also relayed to the provider as part of the request if the provider supports it (eg. OpenAI's user field).\n"
         )
     )
     source: typing.Optional[str] = pydantic.Field(
         description=("The API consumer's source for metrics (e.g. AndroidApp etc).\n")
     )
     client_ref_id: typing.Optional[str] = pydantic.Field(
         description=("The API consumer's internal reference id to able to link references to their sessions.\n")
     )
-    template_args: typing.Optional[typing.Dict[str, str]]
+    template_args: typing.Dict[str, str]
     metadata: typing.Optional[typing.Dict[str, typing.Any]]
     request_timeout: typing.Optional[float] = pydantic.Field(
         description=(
             "Provider request timout in seconds. If not provided, then Prompton API's default timeout for the provider will be used (90sec or `DEFAULT_OPENAI_REQUEST_TIMEOUT_SECONDS` env var if provided).\n"
         )
     )
     prompt_version_id: str
-    prompt_version_ids_considered: typing.Optional[typing.List[str]] = pydantic.Field(
-        description=(
-            "If inference was by prompt_id then a list of all other prompt versions considered for this inference. I.e. all prompt versions in Live status at the time of the inference\n"
-        )
-    )
+    prompt_version_ids_considered: typing.List[str]
     prompt_id: str
-    prompt_version_name: typing.Optional[str]
-    status: typing.Optional[InferenceResponseStatus]
-    request: typing.Optional[InferenceRequestData]
+    prompt_version_name: str
+    status: InferenceResponseStatus
+    request: InferenceRequestData
     response: typing.Optional[InferenceReadResponse]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `prompton-0.0.4/prompton/types/inference_request_data.py` & `prompton-0.0.5/prompton/types/inference_request_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/inference_response_data.py` & `prompton-0.0.5/prompton/types/inference_response_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/inference_response_error.py` & `prompton-0.0.5/prompton/types/inference_response_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .inference_error import InferenceError
 
 
 class InferenceResponseError(pydantic.BaseModel):
     completed_at: typing.Optional[str]
     completition_duration_seconds: typing.Optional[float]
     is_client_connected_at_finish: typing.Optional[bool]
     is_error: typing.Optional[bool] = pydantic.Field(alias="isError")
-    error: typing.Optional[typing.Any]
+    error: InferenceError
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.4/prompton/types/inference_response_status.py` & `prompton-0.0.5/prompton/types/inference_response_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/org_read.py` & `prompton-0.0.5/prompton/types/token.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,27 +4,22 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class OrgRead(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(alias="_id")
-    created_at: typing.Optional[str]
-    created_by_user_id: typing.Optional[str]
-    created_by_org_id: typing.Optional[str]
-    name: str
-    access_keys: typing.Optional[typing.Dict[str, str]]
+class Token(pydantic.BaseModel):
+    access_token: str
+    token_type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `prompton-0.0.4/prompton/types/prompt_read.py` & `prompton-0.0.5/prompton/types/prompt_version_read.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,39 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .prompt_status import PromptStatus
-
-
-class PromptRead(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(alias="_id")
-    created_at: typing.Optional[str]
-    created_by_user_id: typing.Optional[str]
-    created_by_org_id: typing.Optional[str]
-    status: typing.Optional[PromptStatus]
+from .chat_gpt_chat_completition_config import ChatGptChatCompletitionConfig
+from .chat_gpt_message import ChatGptMessage
+from .prompt_version_providers import PromptVersionProviders
+from .prompt_version_status import PromptVersionStatus
+
+
+class PromptVersionRead(pydantic.BaseModel):
+    """
+    Base model for reading from MongoDB. Same as MongoBaseCreate but assumes all DB base fields are populated so generated clients doesn't requrie None checks
+    """
+
+    id: str = pydantic.Field(alias="_id")
+    created_at: str
+    created_by_user_id: str
+    created_by_org_id: str
+    status: PromptVersionStatus
+    provider: PromptVersionProviders
     name: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
     description: typing.Optional[str]
+    prompt_id: str
+    template: typing.List[ChatGptMessage]
+    model_config: typing.Optional[ChatGptChatCompletitionConfig]
+    template_arg_names: typing.List[str] = pydantic.Field(
+        description=("List of args in the template - populated by server at PATHC and POST\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.4/prompton/types/prompt_version_read.py` & `prompton-0.0.5/prompton/types/org_read.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,33 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_gpt_chat_completition_config import ChatGptChatCompletitionConfig
-from .chat_gpt_message import ChatGptMessage
-from .prompt_version_providers import PromptVersionProviders
-from .prompt_version_status import PromptVersionStatus
-
-
-class PromptVersionRead(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(alias="_id")
-    created_at: typing.Optional[str]
-    created_by_user_id: typing.Optional[str]
-    created_by_org_id: typing.Optional[str]
-    status: typing.Optional[PromptVersionStatus]
-    provider: typing.Optional[PromptVersionProviders]
-    name: str = pydantic.Field(description=('<span style="white-space: nowrap">`non-empty`</span>\n'))
-    description: typing.Optional[str]
-    prompt_id: str
-    template: typing.Optional[typing.List[ChatGptMessage]]
-    model_config: typing.Optional[ChatGptChatCompletitionConfig]
-    template_arg_names: typing.Optional[typing.List[str]]
+
+
+class OrgRead(pydantic.BaseModel):
+    """
+    Base model for reading from MongoDB. Same as MongoBaseCreate but assumes all DB base fields are populated so generated clients doesn't requrie None checks
+    """
+
+    id: str = pydantic.Field(alias="_id")
+    created_at: str
+    created_by_user_id: str
+    created_by_org_id: str
+    name: str
+    access_keys: typing.Optional[typing.Dict[str, str]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.4/prompton/types/prompt_version_status.py` & `prompton-0.0.5/prompton/types/prompt_version_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/token.py` & `prompton-0.0.5/prompton/types/validation_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class Token(pydantic.BaseModel):
-    access_token: str
-    token_type: str
+class ValidationError(pydantic.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.4/prompton/types/user_read.py` & `prompton-0.0.5/prompton/types/user_read.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .user_roles import UserRoles
 
 
 class UserRead(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(alias="_id")
-    created_at: typing.Optional[str]
-    created_by_user_id: typing.Optional[str]
-    created_by_org_id: typing.Optional[str]
+    """
+    Base model for reading from MongoDB. Same as MongoBaseCreate but assumes all DB base fields are populated so generated clients doesn't requrie None checks
+    """
+
+    id: str = pydantic.Field(alias="_id")
+    created_at: str
+    created_by_user_id: str
+    created_by_org_id: str
     full_name: typing.Optional[str] = pydantic.Field(
         description=('<span style="white-space: nowrap">`non-empty`</span>\n')
     )
-    disabled: typing.Optional[bool]
+    disabled: bool
     role: typing.Optional[UserRoles]
     org_id: str
     email: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `prompton-0.0.4/prompton/types/user_roles.py` & `prompton-0.0.5/prompton/types/user_roles.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.4/prompton/types/validation_error.py` & `prompton-0.0.5/prompton/types/inference_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class ValidationError(pydantic.BaseModel):
-    loc: typing.List[ValidationErrorLocItem]
-    msg: str
-    type: str
+class InferenceError(pydantic.BaseModel):
+    error_class: str
+    message: str
+    details: typing.Optional[typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `prompton-0.0.4/PKG-INFO` & `prompton-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompton
-Version: 0.0.4
+Version: 0.0.5
 Summary: Chat prompt template evaluation and inference monitoring
 Author: PromptOn
 Author-email: hello@prompton.ai
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


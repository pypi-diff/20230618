# Comparing `tmp/django_admin_action_tools-1.1.6a3.tar.gz` & `tmp/django_admin_action_tools-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_action_tools-1.1.6a3.tar", max compression
+gzip compressed data, was "django_admin_action_tools-1.1.7.tar", max compression
```

## Comparing `django_admin_action_tools-1.1.6a3.tar` & `django_admin_action_tools-1.1.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11358 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/LICENSE
--rw-r--r--   0        0        0     9571 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/README.md
--rw-r--r--   0        0        0       47 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/__init__.py
--rw-r--r--   0        0        0      278 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/admin/__init__.py
--rw-r--r--   0        0        0     2722 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/admin/base.py
--rw-r--r--   0        0        0    19366 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/admin/confirm_tool.py
--rw-r--r--   0        0        0     4402 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/admin/form_tool.py
--rw-r--r--   0        0        0      968 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/constants.py
--rw-r--r--   0        0        0     3680 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/file_cache.py
--rw-r--r--   0        0        0      800 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/static/admin/css/confirmation.css
--rw-r--r--   0        0        0     1968 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templates/admin/confirm_tool/action_confirmation.html
--rw-r--r--   0        0        0     2705 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templates/admin/confirm_tool/change_confirmation.html
--rw-r--r--   0        0        0     1580 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templates/admin/form_tool/action_form.html
--rw-r--r--   0        0        0      292 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templates/admin/submit_line.html
--rw-r--r--   0        0        0      532 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templates/include/change_data.html
--rw-r--r--   0        0        0      477 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templates/include/form.html
--rw-r--r--   0        0        0      556 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templates/include/submit_row.html
--rw-r--r--   0        0        0        0 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templatetags/__init__.py
--rw-r--r--   0        0        0     1010 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/templatetags/formatting.py
--rw-r--r--   0        0        0     4908 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/helpers.py
--rw-r--r--   0        0        0     7962 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_cache.py
--rw-r--r--   0        0        0     2066 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_change_actions.py
--rw-r--r--   0        0        0     5291 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_form_input_types.py
--rw-r--r--   0        0        0     7503 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_inlines.py
--rw-r--r--   0        0        0     7470 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_s3_storage.py
--rw-r--r--   0        0        0     7832 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_validators_integration.py
--rw-r--r--   0        0        0     5285 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/form-tool/test_with_form_actions.py
--rw-r--r--   0        0        0     3757 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/form-tool/test_with_multiple_forms.py
--rw-r--r--   0        0        0      332 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/test_smoke.py
--rw-r--r--   0        0        0   109790 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/snapshot/screenshot.png
--rw-r--r--   0        0        0    11629 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_admin_options.py
--rw-r--r--   0        0        0    11056 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirm_actions.py
--rw-r--r--   0        0        0    13935 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add.py
--rw-r--r--   0        0        0     8025 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add_m2m_field.py
--rw-r--r--   0        0        0    16779 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirm_save_actions.py
--rw-r--r--   0        0        0    16460 2023-06-18 01:17:57.471711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirmation_cache.py
--rw-r--r--   0        0        0    33930 2023-06-18 01:17:57.475711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirmation_using_file_cache.py
--rw-r--r--   0        0        0     1042 2023-06-18 01:17:57.475711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_file_cache.py
--rw-r--r--   0        0        0     4507 2023-06-18 01:17:57.475711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_model_field_types.py
--rw-r--r--   0        0        0    12545 2023-06-18 01:17:57.475711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_with_validators.py
--rw-r--r--   0        0        0     3370 2023-06-18 01:17:57.475711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/form-tool/test_form_action.py
--rw-r--r--   0        0        0     2136 2023-06-18 01:17:57.475711 django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/test_toolchain.py
--rw-r--r--   0        0        0     4236 2023-06-18 01:17:57.475711 django_admin_action_tools-1.1.6a3/admin_action_tools/toolchain.py
--rw-r--r--   0        0        0      667 2023-06-18 01:17:57.475711 django_admin_action_tools-1.1.6a3/admin_action_tools/utils.py
--rw-r--r--   0        0        0     3289 2023-06-18 01:18:12.692745 django_admin_action_tools-1.1.6a3/pyproject.toml
--rw-r--r--   0        0        0    10578 1970-01-01 00:00:00.000000 django_admin_action_tools-1.1.6a3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/LICENSE
+-rw-r--r--   0        0        0     9571 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/README.md
+-rw-r--r--   0        0        0       47 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/admin/__init__.py
+-rw-r--r--   0        0        0     2722 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/admin/base.py
+-rw-r--r--   0        0        0    19366 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/admin/confirm_tool.py
+-rw-r--r--   0        0        0     4402 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/admin/form_tool.py
+-rw-r--r--   0        0        0      968 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/constants.py
+-rw-r--r--   0        0        0     3680 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/file_cache.py
+-rw-r--r--   0        0        0      800 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/static/admin/css/confirmation.css
+-rw-r--r--   0        0        0     1968 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templates/admin/confirm_tool/action_confirmation.html
+-rw-r--r--   0        0        0     2705 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templates/admin/confirm_tool/change_confirmation.html
+-rw-r--r--   0        0        0     1580 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templates/admin/form_tool/action_form.html
+-rw-r--r--   0        0        0      292 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templates/admin/submit_line.html
+-rw-r--r--   0        0        0      532 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templates/include/change_data.html
+-rw-r--r--   0        0        0      477 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templates/include/form.html
+-rw-r--r--   0        0        0      556 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templates/include/submit_row.html
+-rw-r--r--   0        0        0        0 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templatetags/__init__.py
+-rw-r--r--   0        0        0     1010 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/templatetags/formatting.py
+-rw-r--r--   0        0        0     4908 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/tests/helpers.py
+-rw-r--r--   0        0        0     7962 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_cache.py
+-rw-r--r--   0        0        0     2066 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_change_actions.py
+-rw-r--r--   0        0        0     5291 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_form_input_types.py
+-rw-r--r--   0        0        0     7503 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_inlines.py
+-rw-r--r--   0        0        0     7470 2023-06-18 02:09:55.083213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_s3_storage.py
+-rw-r--r--   0        0        0     7832 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_validators_integration.py
+-rw-r--r--   0        0        0     5285 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/form-tool/test_with_form_actions.py
+-rw-r--r--   0        0        0     3757 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/form-tool/test_with_multiple_forms.py
+-rw-r--r--   0        0        0      332 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/test_smoke.py
+-rw-r--r--   0        0        0   109790 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/snapshot/screenshot.png
+-rw-r--r--   0        0        0    11629 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_admin_options.py
+-rw-r--r--   0        0        0    11056 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirm_actions.py
+-rw-r--r--   0        0        0    13935 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add.py
+-rw-r--r--   0        0        0     8025 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add_m2m_field.py
+-rw-r--r--   0        0        0    16779 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirm_save_actions.py
+-rw-r--r--   0        0        0    16460 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirmation_cache.py
+-rw-r--r--   0        0        0    33930 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirmation_using_file_cache.py
+-rw-r--r--   0        0        0     1042 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_file_cache.py
+-rw-r--r--   0        0        0     4507 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_model_field_types.py
+-rw-r--r--   0        0        0    12545 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_with_validators.py
+-rw-r--r--   0        0        0     3370 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/form-tool/test_form_action.py
+-rw-r--r--   0        0        0     2136 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/test_toolchain.py
+-rw-r--r--   0        0        0     4236 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/toolchain.py
+-rw-r--r--   0        0        0      667 2023-06-18 02:09:55.087213 django_admin_action_tools-1.1.7/admin_action_tools/utils.py
+-rw-r--r--   0        0        0     3281 2023-06-18 02:10:08.675415 django_admin_action_tools-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0    10576 1970-01-01 00:00:00.000000 django_admin_action_tools-1.1.7/PKG-INFO
```

### Comparing `django_admin_action_tools-1.1.6a3/LICENSE` & `django_admin_action_tools-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/README.md` & `django_admin_action_tools-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/admin/base.py` & `django_admin_action_tools-1.1.7/admin_action_tools/admin/base.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/admin/confirm_tool.py` & `django_admin_action_tools-1.1.7/admin_action_tools/admin/confirm_tool.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/admin/form_tool.py` & `django_admin_action_tools-1.1.7/admin_action_tools/admin/form_tool.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/constants.py` & `django_admin_action_tools-1.1.7/admin_action_tools/constants.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/file_cache.py` & `django_admin_action_tools-1.1.7/admin_action_tools/file_cache.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/static/admin/css/confirmation.css` & `django_admin_action_tools-1.1.7/admin_action_tools/static/admin/css/confirmation.css`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/templates/admin/confirm_tool/action_confirmation.html` & `django_admin_action_tools-1.1.7/admin_action_tools/templates/admin/confirm_tool/action_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/templates/admin/confirm_tool/change_confirmation.html` & `django_admin_action_tools-1.1.7/admin_action_tools/templates/admin/confirm_tool/change_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/templates/admin/form_tool/action_form.html` & `django_admin_action_tools-1.1.7/admin_action_tools/templates/admin/form_tool/action_form.html`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/templates/include/change_data.html` & `django_admin_action_tools-1.1.7/admin_action_tools/templates/include/change_data.html`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/templates/include/submit_row.html` & `django_admin_action_tools-1.1.7/admin_action_tools/templates/include/submit_row.html`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/templatetags/formatting.py` & `django_admin_action_tools-1.1.7/admin_action_tools/templatetags/formatting.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/helpers.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_cache.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_cache.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_change_actions.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_change_actions.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_form_input_types.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_form_input_types.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_inlines.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_inlines.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_s3_storage.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_s3_storage.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/confirm-tool/test_with_validators_integration.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/confirm-tool/test_with_validators_integration.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/form-tool/test_with_form_actions.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/form-tool/test_with_form_actions.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/integration/form-tool/test_with_multiple_forms.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/integration/form-tool/test_with_multiple_forms.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/snapshot/screenshot.png` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/snapshot/screenshot.png`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_admin_options.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_admin_options.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirm_actions.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirm_actions.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add_m2m_field.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirm_change_and_add_m2m_field.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirm_save_actions.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirm_save_actions.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirmation_cache.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirmation_cache.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_confirmation_using_file_cache.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_confirmation_using_file_cache.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_file_cache.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_file_cache.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_model_field_types.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_model_field_types.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/confirm-tool/test_with_validators.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/confirm-tool/test_with_validators.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/form-tool/test_form_action.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/form-tool/test_form_action.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/tests/unit/test_toolchain.py` & `django_admin_action_tools-1.1.7/admin_action_tools/tests/unit/test_toolchain.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/toolchain.py` & `django_admin_action_tools-1.1.7/admin_action_tools/toolchain.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/admin_action_tools/utils.py` & `django_admin_action_tools-1.1.7/admin_action_tools/utils.py`

 * *Files identical despite different names*

### Comparing `django_admin_action_tools-1.1.6a3/pyproject.toml` & `django_admin_action_tools-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 name = "django-admin-action-tools"
 authors = [
     "Thu Trang Pham <thuutrangpham@gmail.com>",
     "jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>",
 ]
 maintainers = ["jeanloup.monnier <jean-loup.monnier@spikeelabs.fr>"]
-version = "1.1.6-alpha.3"
+version = "1.1.7"
 description = "Tools for django admin"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/SpikeeLabs/django-admin-action-tools"
 classifiers = [
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
@@ -23,15 +23,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 Django = ">=3.2"
 django-widget-tweaks = "^1.4"
 
 [tool.poetry.dev-dependencies]
 factory-boy = "^3.0"
-coverage = "^5.4"
+coverage = "^6.4"
 pytest = "^7"
 pytest-django = "^4.1"
 readme-renderer = "^28.0"
 twine = "^3.3"
 coveralls = "^3.0"
 selenium = "^4.0"
 django-storages = "^1.11"
```

### Comparing `django_admin_action_tools-1.1.6a3/PKG-INFO` & `django_admin_action_tools-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-action-tools
-Version: 1.1.6a3
+Version: 1.1.7
 Summary: Tools for django admin
 Home-page: https://github.com/SpikeeLabs/django-admin-action-tools
 License: Apache-2.0
 Author: Thu Trang Pham
 Author-email: thuutrangpham@gmail.com
 Maintainer: jeanloup.monnier
 Maintainer-email: jean-loup.monnier@spikeelabs.fr
```


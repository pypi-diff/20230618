# Comparing `tmp/ormar-0.9.8.tar.gz` & `tmp/ormar-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ormar-0.9.8.tar", last modified: Wed Mar 10 13:16:28 2021, max compression
+gzip compressed data, was "ormar-0.9.9.tar", last modified: Mon Mar 15 18:01:50 2021, max compression
```

## Comparing `ormar-0.9.8.tar` & `ormar-0.9.9.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.175780 ormar-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-03-10 13:16:12.000000 ormar-0.9.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)    24490 2021-03-10 13:16:28.175780 ormar-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19182 2021-03-10 13:16:12.000000 ormar-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.167780 ormar-0.9.8/ormar/
--rw-r--r--   0 runner    (1001) docker     (121)     2598 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.167780 ormar-0.9.8/ormar/decorators/
--rw-r--r--   0 runner    (1001) docker     (121)      562 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/decorators/property_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     4000 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/decorators/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.167780 ormar-0.9.8/ormar/fields/
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13497 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    17074 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/foreign_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     8866 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/many_to_many.py
--rw-r--r--   0 runner    (1001) docker     (121)    17647 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/model_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6038 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/sqlalchemy_encrypted.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/sqlalchemy_uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/fields/through_field.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.171780 ormar-0.9.8/ormar/models/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9689 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/excludable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.171780 ormar-0.9.8/ormar/models/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5968 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5357 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/helpers/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/helpers/related_names_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8611 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/helpers/relations.py
--rw-r--r--   0 runner    (1001) docker     (121)    11329 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/helpers/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5867 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/helpers/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)    20389 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/metaclass.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.171780 ormar-0.9.8/ormar/models/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)      701 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/mixins/alias_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     7098 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/mixins/excludable_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/mixins/merge_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4746 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/mixins/prefetch_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     7634 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/mixins/relation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5485 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/mixins/save_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)    11799 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    15156 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/model_row.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/modelproxy.py
--rw-r--r--   0 runner    (1001) docker     (121)    28826 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/newbasemodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/models/quick_access_views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.171780 ormar-0.9.8/ormar/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/protocols/queryset_protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/protocols/relation_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.175780 ormar-0.9.8/ormar/queryset/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.175780 ormar-0.9.8/ormar/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5834 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/actions/filter_action.py
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/actions/order_action.py
--rw-r--r--   0 runner    (1001) docker     (121)     3203 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/actions/query_action.py
--rw-r--r--   0 runner    (1001) docker     (121)    11481 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/clause.py
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/filter_query.py
--rw-r--r--   0 runner    (1001) docker     (121)    12636 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/join.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/limit_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/offset_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/order_query.py
--rw-r--r--   0 runner    (1001) docker     (121)    23745 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/prefetch_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     9102 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/query.py
--rw-r--r--   0 runner    (1001) docker     (121)    35114 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/queryset.py
--rw-r--r--   0 runner    (1001) docker     (121)    10577 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/queryset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.175780 ormar-0.9.8/ormar/relations/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6458 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/relations/alias_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    24436 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/relations/querysetproxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6379 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/relations/relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6080 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/relations/relation_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6719 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/relations/relation_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/relations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.175780 ormar-0.9.8/ormar/signals/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2021-03-10 13:16:12.000000 ormar-0.9.8/ormar/signals/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-10 13:16:28.167780 ormar-0.9.8/ormar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    24490 2021-03-10 13:16:27.000000 ormar-0.9.8/ormar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2021-03-10 13:16:28.000000 ormar-0.9.8/ormar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-10 13:16:27.000000 ormar-0.9.8/ormar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-10 13:16:27.000000 ormar-0.9.8/ormar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-10 13:16:27.000000 ormar-0.9.8/ormar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-10 13:16:27.000000 ormar-0.9.8/ormar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-10 13:16:28.175780 ormar-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-03-10 13:16:12.000000 ormar-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.467600 ormar-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-03-15 18:01:41.000000 ormar-0.9.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)    24490 2021-03-15 18:01:50.467600 ormar-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    19182 2021-03-15 18:01:41.000000 ormar-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.455600 ormar-0.9.9/ormar/
+-rw-r--r--   0 runner    (1001) docker     (121)     2798 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.455600 ormar-0.9.9/ormar/decorators/
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/decorators/property_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5949 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/decorators/signals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.455600 ormar-0.9.9/ormar/fields/
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13589 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17724 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/foreign_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8523 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/many_to_many.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17647 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/model_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6038 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/sqlalchemy_encrypted.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/sqlalchemy_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2021 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/fields/through_field.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.459600 ormar-0.9.9/ormar/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9689 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/excludable.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.459600 ormar-0.9.9/ormar/models/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6055 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5357 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/helpers/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/helpers/related_names_validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8717 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/helpers/relations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11483 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/helpers/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5867 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/helpers/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20598 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/metaclass.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.459600 ormar-0.9.9/ormar/models/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2741 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/mixins/alias_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7098 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/mixins/excludable_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2834 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/mixins/merge_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4746 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/mixins/prefetch_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7634 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/mixins/relation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6333 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/mixins/save_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12079 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15156 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/model_row.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/modelproxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28979 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/newbasemodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1614 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/models/quick_access_views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.463600 ormar-0.9.9/ormar/protocols/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/protocols/queryset_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/protocols/relation_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.463600 ormar-0.9.9/ormar/queryset/
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.463600 ormar-0.9.9/ormar/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5834 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/actions/filter_action.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3474 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/actions/order_action.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3203 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/actions/query_action.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1818 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/actions/select_action.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11481 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/clause.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1143 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/filter_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15200 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/join.py
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/limit_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/offset_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/order_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23745 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/prefetch_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9513 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37955 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10577 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/queryset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.463600 ormar-0.9.9/ormar/relations/
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6458 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/relations/alias_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25710 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/relations/querysetproxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6379 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/relations/relation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6080 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/relations/relation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7635 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/relations/relation_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/relations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.467600 ormar-0.9.9/ormar/signals/
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3737 2021-03-15 18:01:41.000000 ormar-0.9.9/ormar/signals/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 18:01:50.455600 ormar-0.9.9/ormar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    24490 2021-03-15 18:01:50.000000 ormar-0.9.9/ormar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2182 2021-03-15 18:01:50.000000 ormar-0.9.9/ormar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-15 18:01:50.000000 ormar-0.9.9/ormar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-15 18:01:50.000000 ormar-0.9.9/ormar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-03-15 18:01:50.000000 ormar-0.9.9/ormar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-03-15 18:01:50.000000 ormar-0.9.9/ormar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-15 18:01:50.467600 ormar-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-03-15 18:01:41.000000 ormar-0.9.9/setup.py
```

### Comparing `ormar-0.9.8/LICENSE.md` & `ormar-0.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/PKG-INFO` & `ormar-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ormar
-Version: 0.9.8
+Version: 0.9.9
 Summary: A simple async ORM with fastapi in mind and pydantic validation.
 Home-page: https://github.com/collerek/ormar
 Author: Radosław Drążkiewicz
 Author-email: collerek@gmail.com
 License: MIT
 Description: # ormar
         <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ormar Version: 0.9.8 Summary: A simple async ORM
+Metadata-Version: 2.1 Name: ormar Version: 0.9.9 Summary: A simple async ORM
 with fastapi in mind and pydantic validation. Home-page: https://github.com/
 collerek/ormar Author: RadosÅaw DrÄÅ¼kiewicz Author-email: collerek@gmail.com
 License: MIT Description: # ormar
 [Pypi_version] [Pypi_version] [Build Status] [Coverage] [CodeFactor] [https://
 api.codeclimate.com/v1/badges/186bc79245724864a7aa/maintainability] [https://
 pepy.tech/badge/ormar]
 ### Overview The `ormar` package is an async mini ORM for Python, with support
```

### Comparing `ormar-0.9.8/README.md` & `ormar-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/__init__.py` & `ormar-0.9.9/ormar/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 
 And what's a better name for python ORM than snakes cabinet :)
 
 """
 from ormar.protocols import QuerySetProtocol, RelationProtocol  # noqa: I100
 from ormar.decorators import (  # noqa: I100
     post_delete,
+    post_relation_add,
+    post_relation_remove,
     post_save,
     post_update,
     pre_delete,
+    pre_relation_add,
+    pre_relation_remove,
     pre_save,
     pre_update,
     property_field,
 )
 from ormar.exceptions import (  # noqa: I100
     ModelDefinitionError,
     MultipleMatches,
@@ -67,15 +71,15 @@
 class UndefinedType:  # pragma no cover
     def __repr__(self) -> str:
         return "OrmarUndefined"
 
 
 Undefined = UndefinedType()
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 __all__ = [
     "Integer",
     "BigInteger",
     "Boolean",
     "Time",
     "Text",
     "String",
@@ -98,17 +102,21 @@
     "QuerySetProtocol",
     "RelationProtocol",
     "ModelMeta",
     "property_field",
     "post_delete",
     "post_save",
     "post_update",
+    "post_relation_add",
+    "post_relation_remove",
     "pre_delete",
     "pre_save",
     "pre_update",
+    "pre_relation_remove",
+    "pre_relation_add",
     "Signal",
     "BaseField",
     "ManyToManyField",
     "ForeignKeyField",
     "OrderAction",
     "ExcludableItems",
     "and_",
```

### Comparing `ormar-0.9.8/ormar/decorators/property_field.py` & `ormar-0.9.9/ormar/decorators/property_field.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/decorators/signals.py` & `ormar-0.9.9/ormar/decorators/signals.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     :return: returns the original function untouched
     :rtype: Callable
     """
 
     def _decorator(func: Callable) -> Callable:
         """
 
-        Internal decorator that does all the registeriing.
+        Internal decorator that does all the registering.
 
         :param func: function to register as receiver
         :type func: Callable
         :return: untouched function already registered for given signal
         :rtype: Callable
         """
         if not isinstance(senders, list):
@@ -113,7 +113,61 @@
     :param senders: one or a list of "Model" classes
     that should have the signal receiver registered
     :type senders: Union[Type["Model"], List[Type["Model"]]]
     :return: returns the original function untouched
     :rtype: Callable
     """
     return receiver(signal="pre_delete", senders=senders)
+
+
+def pre_relation_add(senders: Union[Type["Model"], List[Type["Model"]]]) -> Callable:
+    """
+    Connect given function to all senders for pre_relation_add signal.
+
+    :param senders: one or a list of "Model" classes
+    that should have the signal receiver registered
+    :type senders: Union[Type["Model"], List[Type["Model"]]]
+    :return: returns the original function untouched
+    :rtype: Callable
+    """
+    return receiver(signal="pre_relation_add", senders=senders)
+
+
+def post_relation_add(senders: Union[Type["Model"], List[Type["Model"]]]) -> Callable:
+    """
+    Connect given function to all senders for post_relation_add signal.
+
+    :param senders: one or a list of "Model" classes
+    that should have the signal receiver registered
+    :type senders: Union[Type["Model"], List[Type["Model"]]]
+    :return: returns the original function untouched
+    :rtype: Callable
+    """
+    return receiver(signal="post_relation_add", senders=senders)
+
+
+def pre_relation_remove(senders: Union[Type["Model"], List[Type["Model"]]]) -> Callable:
+    """
+    Connect given function to all senders for pre_relation_remove signal.
+
+    :param senders: one or a list of "Model" classes
+    that should have the signal receiver registered
+    :type senders: Union[Type["Model"], List[Type["Model"]]]
+    :return: returns the original function untouched
+    :rtype: Callable
+    """
+    return receiver(signal="pre_relation_remove", senders=senders)
+
+
+def post_relation_remove(
+    senders: Union[Type["Model"], List[Type["Model"]]]
+) -> Callable:
+    """
+    Connect given function to all senders for post_relation_remove signal.
+
+    :param senders: one or a list of "Model" classes
+    that should have the signal receiver registered
+    :type senders: Union[Type["Model"], List[Type["Model"]]]
+    :return: returns the original function untouched
+    :rtype: Callable
+    """
+    return receiver(signal="post_relation_remove", senders=senders)
```

### Comparing `ormar-0.9.8/ormar/exceptions.py` & `ormar-0.9.9/ormar/exceptions.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/fields/__init__.py` & `ormar-0.9.9/ormar/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/fields/base.py` & `ormar-0.9.9/ormar/fields/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     is_through: bool = False  # ThroughFields
 
     owner: Type["Model"]
     to: Type["Model"]
     through: Type["Model"]
     self_reference: bool = False
     self_reference_primary: Optional[str] = None
+    orders_by: Optional[List[str]] = None
+    related_orders_by: Optional[List[str]] = None
 
     encrypt_secret: str
     encrypt_backend: EncryptBackends = EncryptBackends.NONE
     encrypt_custom_backend: Optional[Type[EncryptBackend]] = None
 
     default: Any
     server_default: Any
```

### Comparing `ormar-0.9.8/ormar/fields/foreign_key.py` & `ormar-0.9.9/ormar/fields/foreign_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import string
 import sys
 import uuid
 from dataclasses import dataclass
 from random import choices
-from typing import Any, List, Optional, TYPE_CHECKING, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, TYPE_CHECKING, Tuple, Type, Union
 
 import sqlalchemy
 from pydantic import BaseModel, create_model
 from pydantic.typing import ForwardRef, evaluate_forwardref
 from sqlalchemy import UniqueConstraint
 
 import ormar  # noqa I101
@@ -115,14 +115,43 @@
             reference=fk_string, ondelete=ondelete, onupdate=onupdate, name=None
         )
     ]
     column_type = to_field.column_type
     return __type__, constraints, column_type
 
 
+def validate_not_allowed_fields(kwargs: Dict) -> None:
+    """
+    Verifies if not allowed parameters are set on relation models.
+    Usually they are omitted later anyway but this way it's explicitly
+    notify the user that it's not allowed/ supported.
+
+    :raises ModelDefinitionError: if any forbidden field is set
+    :param kwargs: dict of kwargs to verify passed to relation field
+    :type kwargs: Dict
+    """
+    default = kwargs.pop("default", None)
+    encrypt_secret = kwargs.pop("encrypt_secret", None)
+    encrypt_backend = kwargs.pop("encrypt_backend", None)
+    encrypt_custom_backend = kwargs.pop("encrypt_custom_backend", None)
+
+    not_supported = [
+        default,
+        encrypt_secret,
+        encrypt_backend,
+        encrypt_custom_backend,
+    ]
+    if any(x is not None for x in not_supported):
+        raise ModelDefinitionError(
+            f"Argument {next((x for x in not_supported if x is not None))} "
+            f"is not supported "
+            "on relation fields!"
+        )
+
+
 class UniqueColumns(UniqueConstraint):
     """
     Subclass of sqlalchemy.UniqueConstraint.
     Used to avoid importing anything from sqlalchemy by user.
     """
 
 
@@ -180,32 +209,18 @@
     :type kwargs: Any
     :return: ormar ForeignKeyField with relation to selected model
     :rtype: ForeignKeyField
     """
 
     owner = kwargs.pop("owner", None)
     self_reference = kwargs.pop("self_reference", False)
+    orders_by = kwargs.pop("orders_by", None)
+    related_orders_by = kwargs.pop("related_orders_by", None)
 
-    default = kwargs.pop("default", None)
-    encrypt_secret = kwargs.pop("encrypt_secret", None)
-    encrypt_backend = kwargs.pop("encrypt_backend", None)
-    encrypt_custom_backend = kwargs.pop("encrypt_custom_backend", None)
-
-    not_supported = [
-        default,
-        encrypt_secret,
-        encrypt_backend,
-        encrypt_custom_backend,
-    ]
-    if any(x is not None for x in not_supported):
-        raise ModelDefinitionError(
-            f"Argument {next((x for x in not_supported if x is not None))} "
-            f"is not supported "
-            "on relation fields!"
-        )
+    validate_not_allowed_fields(kwargs)
 
     if to.__class__ == ForwardRef:
         __type__ = to if not nullable else Optional[to]
         constraints: List = []
         column_type = None
     else:
         __type__, constraints, column_type = populate_fk_params_based_on_to_model(
@@ -233,14 +248,16 @@
         default=None,
         server_default=None,
         onupdate=onupdate,
         ondelete=ondelete,
         owner=owner,
         self_reference=self_reference,
         is_relation=True,
+        orders_by=orders_by,
+        related_orders_by=related_orders_by,
     )
 
     return type("ForeignKey", (ForeignKeyField, BaseField), namespace)
 
 
 class ForeignKeyField(BaseField):
     """
```

### Comparing `ormar-0.9.8/ormar/fields/many_to_many.py` & `ormar-0.9.9/ormar/fields/many_to_many.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from typing import Any, List, Optional, TYPE_CHECKING, Tuple, Type, Union, cast
 
 from pydantic.typing import ForwardRef, evaluate_forwardref
 import ormar  # noqa: I100
 from ormar import ModelDefinitionError
 from ormar.fields import BaseField
-from ormar.fields.foreign_key import ForeignKeyField
+from ormar.fields.foreign_key import ForeignKeyField, validate_not_allowed_fields
 
 if TYPE_CHECKING:  # pragma no cover
     from ormar.models import Model
 
     if sys.version_info < (3, 7):
         ToType = Type["Model"]
     else:
@@ -89,34 +89,21 @@
     :return: ormar ManyToManyField with m2m relation to selected model
     :rtype: ManyToManyField
     """
     related_name = kwargs.pop("related_name", None)
     nullable = kwargs.pop("nullable", True)
     owner = kwargs.pop("owner", None)
     self_reference = kwargs.pop("self_reference", False)
+    orders_by = kwargs.pop("orders_by", None)
+    related_orders_by = kwargs.pop("related_orders_by", None)
+
     if through is not None and through.__class__ != ForwardRef:
         forbid_through_relations(cast(Type["Model"], through))
 
-    default = kwargs.pop("default", None)
-    encrypt_secret = kwargs.pop("encrypt_secret", None)
-    encrypt_backend = kwargs.pop("encrypt_backend", None)
-    encrypt_custom_backend = kwargs.pop("encrypt_custom_backend", None)
-
-    not_supported = [
-        default,
-        encrypt_secret,
-        encrypt_backend,
-        encrypt_custom_backend,
-    ]
-    if any(x is not None for x in not_supported):
-        raise ModelDefinitionError(
-            f"Argument {next((x for x in not_supported if x is not None))} "
-            f"is not supported "
-            "on relation fields!"
-        )
+    validate_not_allowed_fields(kwargs)
 
     if to.__class__ == ForwardRef:
         __type__ = to if not nullable else Optional[to]
         column_type = None
     else:
         __type__, column_type = populate_m2m_params_based_on_to_model(
             to=to, nullable=nullable  # type: ignore
@@ -137,14 +124,16 @@
         pydantic_only=False,
         default=None,
         server_default=None,
         owner=owner,
         self_reference=self_reference,
         is_relation=True,
         is_multi=True,
+        orders_by=orders_by,
+        related_orders_by=related_orders_by,
     )
 
     return type("ManyToMany", (ManyToManyField, BaseField), namespace)
 
 
 class ManyToManyField(ForeignKeyField, ormar.QuerySetProtocol, ormar.RelationProtocol):
     """
```

### Comparing `ormar-0.9.8/ormar/fields/model_fields.py` & `ormar-0.9.9/ormar/fields/model_fields.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/fields/parsers.py` & `ormar-0.9.9/ormar/fields/parsers.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/fields/sqlalchemy_encrypted.py` & `ormar-0.9.9/ormar/fields/sqlalchemy_encrypted.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/fields/sqlalchemy_uuid.py` & `ormar-0.9.9/ormar/fields/sqlalchemy_uuid.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/fields/through_field.py` & `ormar-0.9.9/ormar/fields/through_field.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/__init__.py` & `ormar-0.9.9/ormar/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/excludable.py` & `ormar-0.9.9/ormar/models/excludable.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/helpers/__init__.py` & `ormar-0.9.9/ormar/models/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/helpers/models.py` & `ormar-0.9.9/ormar/models/helpers/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     """
     if not hasattr(new_model.Meta, "constraints"):
         new_model.Meta.constraints = []
     if not hasattr(new_model.Meta, "model_fields"):
         new_model.Meta.model_fields = model_fields
     if not hasattr(new_model.Meta, "abstract"):
         new_model.Meta.abstract = False
+    if not hasattr(new_model.Meta, "orders_by"):
+        new_model.Meta.orders_by = []
 
     if any(
         is_field_an_forward_ref(field) for field in new_model.Meta.model_fields.values()
     ):
         new_model.Meta.requires_ref_update = True
     else:
         new_model.Meta.requires_ref_update = False
```

### Comparing `ormar-0.9.8/ormar/models/helpers/pydantic.py` & `ormar-0.9.9/ormar/models/helpers/pydantic.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/helpers/related_names_validation.py` & `ormar-0.9.9/ormar/models/helpers/related_names_validation.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/helpers/relations.py` & `ormar-0.9.9/ormar/models/helpers/relations.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,27 +106,29 @@
             through=model_field.through,
             name=related_name,
             virtual=True,
             related_name=model_field.name,
             owner=model_field.to,
             self_reference=model_field.self_reference,
             self_reference_primary=model_field.self_reference_primary,
+            orders_by=model_field.related_orders_by,
         )
         # register foreign keys on through model
         model_field = cast(Type["ManyToManyField"], model_field)
         register_through_shortcut_fields(model_field=model_field)
         adjust_through_many_to_many_model(model_field=model_field)
     else:
         model_field.to.Meta.model_fields[related_name] = ForeignKey(
             model_field.owner,
             real_name=related_name,
             virtual=True,
             related_name=model_field.name,
             owner=model_field.to,
             self_reference=model_field.self_reference,
+            orders_by=model_field.related_orders_by,
         )
 
 
 def register_through_shortcut_fields(model_field: Type["ManyToManyField"]) -> None:
     """
     Registers m2m relation through shortcut on both ends of the relation.
```

### Comparing `ormar-0.9.8/ormar/models/helpers/sqlalchemy.py` & `ormar-0.9.9/ormar/models/helpers/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,17 @@
         )
 
     if pkname is None:
         raise ormar.ModelDefinitionError("Table has to have a primary key.")
 
     new_model.Meta.columns = columns
     new_model.Meta.pkname = pkname
+    if not new_model.Meta.orders_by:
+        # by default we sort by pk name if other option not provided
+        new_model.Meta.orders_by.append(pkname)
     return new_model
 
 
 def check_for_null_type_columns_from_forward_refs(meta: "ModelMeta") -> bool:
     """
     Check is any column is of NUllType() meaning it's empty column from ForwardRef
```

### Comparing `ormar-0.9.8/ormar/models/helpers/validation.py` & `ormar-0.9.9/ormar/models/helpers/validation.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/metaclass.py` & `ormar-0.9.9/ormar/models/metaclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         str, Union[Type[BaseField], Type[ForeignKeyField], Type[ManyToManyField]]
     ]
     alias_manager: AliasManager
     property_fields: Set
     signals: SignalEmitter
     abstract: bool
     requires_ref_update: bool
+    orders_by: List[str]
 
 
 def add_cached_properties(new_model: Type["Model"]) -> None:
     """
     Sets cached properties for both pydantic and ormar models.
 
     Quick access fields are fields grabbed in getattribute to skip all checks.
@@ -135,14 +136,18 @@
         signals = SignalEmitter()
         signals.pre_save = Signal()
         signals.pre_update = Signal()
         signals.pre_delete = Signal()
         signals.post_save = Signal()
         signals.post_update = Signal()
         signals.post_delete = Signal()
+        signals.pre_relation_add = Signal()
+        signals.post_relation_add = Signal()
+        signals.pre_relation_remove = Signal()
+        signals.post_relation_remove = Signal()
         new_model.Meta.signals = signals
 
 
 def verify_constraint_names(
     base_class: "Model", model_fields: Dict, parent_value: List
 ) -> None:
     """
```

### Comparing `ormar-0.9.8/ormar/models/mixins/__init__.py` & `ormar-0.9.9/ormar/models/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/mixins/alias_mixin.py` & `ormar-0.9.9/ormar/models/mixins/alias_mixin.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/mixins/excludable_mixin.py` & `ormar-0.9.9/ormar/models/mixins/excludable_mixin.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/mixins/merge_mixin.py` & `ormar-0.9.9/ormar/models/mixins/merge_mixin.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/mixins/prefetch_mixin.py` & `ormar-0.9.9/ormar/models/mixins/prefetch_mixin.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/mixins/relation_mixin.py` & `ormar-0.9.9/ormar/models/mixins/relation_mixin.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/mixins/save_mixin.py` & `ormar-0.9.9/ormar/models/mixins/save_mixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import uuid
 from typing import Dict, Optional, Set, TYPE_CHECKING
 
 import ormar
 from ormar.exceptions import ModelPersistenceError
 from ormar.models.helpers.validation import validate_choices
 from ormar.models.mixins import AliasMixin
 from ormar.models.mixins.relation_mixin import RelationMixin
@@ -52,14 +53,33 @@
         if new_kwargs.get(pkname, ormar.Undefined) is None and (
             pk.nullable or pk.autoincrement
         ):
             del new_kwargs[pkname]
         return new_kwargs
 
     @classmethod
+    def parse_non_db_fields(cls, model_dict: Dict) -> Dict:
+        """
+        Receives dictionary of model that is about to be saved and changes uuid fields
+        to strings in bulk_update.
+
+        :param model_dict: dictionary of model that is about to be saved
+        :type model_dict: Dict
+        :return: dictionary of model that is about to be saved
+        :rtype: Dict
+        """
+        for name, field in cls.Meta.model_fields.items():
+            if field.__type__ == uuid.UUID and name in model_dict:
+                parsers = {"string": lambda x: str(x), "hex": lambda x: "%.32x" % x.int}
+                uuid_format = field.column_type.uuid_format
+                parser = parsers.get(uuid_format, lambda x: x)
+                model_dict[name] = parser(model_dict[name])
+        return model_dict
+
+    @classmethod
     def substitute_models_with_pks(cls, model_dict: Dict) -> Dict:  # noqa  CCR001
         """
         Receives dictionary of model that is about to be saved and changes all related
         models that are stored as foreign keys to their fk value.
 
         :param model_dict: dictionary of model that is about to be saved
         :type model_dict: Dict
```

### Comparing `ormar-0.9.8/ormar/models/model.py` & `ormar-0.9.9/ormar/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,29 +65,28 @@
         Sends pre_save and post_save signals.
 
         Sets model save status to True.
 
         :return: saved Model
         :rtype: Model
         """
+        await self.signals.pre_save.send(sender=self.__class__, instance=self)
         self_fields = self._extract_model_db_fields()
 
         if not self.pk and self.Meta.model_fields[self.Meta.pkname].autoincrement:
             self_fields.pop(self.Meta.pkname, None)
         self_fields = self.populate_default_values(self_fields)
         self.update_from_dict(
             {
                 k: v
                 for k, v in self_fields.items()
                 if k not in self.extract_related_names()
             }
         )
 
-        await self.signals.pre_save.send(sender=self.__class__, instance=self)
-
         self_fields = self.translate_columns_to_aliases(self_fields)
         expr = self.Meta.table.insert()
         expr = expr.values(**self_fields)
 
         pk = await self.Meta.database.execute(expr)
         if pk and isinstance(pk, self.pk_type()):
             setattr(self, self.Meta.pkname, pk)
@@ -212,15 +211,17 @@
             self.update_from_dict(kwargs)
 
         if not self.pk:
             raise ModelPersistenceError(
                 "You cannot update not saved model! Use save or upsert method."
             )
 
-        await self.signals.pre_update.send(sender=self.__class__, instance=self)
+        await self.signals.pre_update.send(
+            sender=self.__class__, instance=self, passed_args=kwargs
+        )
         self_fields = self._extract_model_db_fields()
         self_fields.pop(self.get_column_name_from_alias(self.Meta.pkname))
         self_fields = self.translate_columns_to_aliases(self_fields)
         expr = self.Meta.table.update().values(**self_fields)
         expr = expr.where(self.pk_column == getattr(self, self.Meta.pkname))
 
         await self.Meta.database.execute(expr)
@@ -269,15 +270,18 @@
         kwargs = dict(row)
         kwargs = self.translate_aliases_to_columns(kwargs)
         self.update_from_dict(kwargs)
         self.set_save_status(True)
         return self
 
     async def load_all(
-        self: T, follow: bool = False, exclude: Union[List, str, Set, Dict] = None
+        self: T,
+        follow: bool = False,
+        exclude: Union[List, str, Set, Dict] = None,
+        order_by: Union[List, str] = None,
     ) -> T:
         """
         Allow to refresh existing Models fields from database.
         Performs refresh of the related models fields.
 
         By default loads only self and the directly related ones.
 
@@ -287,14 +291,16 @@
         to parent model visited models set is kept.
 
         That way already visited models that are nested are loaded, but the load do not
         follow them inside. So Model A -> Model B -> Model C -> Model A -> Model X
         will load second Model A but will never follow into Model X.
         Nested relations of those kind need to be loaded manually.
 
+        :param order_by: columns by which models should be sorted
+        :type order_by: Union[List, str]
         :raises NoMatch: If given pk is not found in database.
 
         :param exclude: related models to exclude
         :type exclude: Union[List, str, Set, Dict]
         :param follow: flag to trigger deep save -
         by default only directly related models are saved
         with follow=True also related models of related models are saved
@@ -304,11 +310,13 @@
         """
         relations = list(self.extract_related_names())
         if follow:
             relations = self._iterate_related_models()
         queryset = self.__class__.objects
         if exclude:
             queryset = queryset.exclude_fields(exclude)
+        if order_by:
+            queryset = queryset.order_by(order_by)
         instance = await queryset.select_related(relations).get(pk=self.pk)
         self._orm.clear()
         self.update_from_dict(instance.dict())
         return self
```

### Comparing `ormar-0.9.8/ormar/models/model_row.py` & `ormar-0.9.9/ormar/models/model_row.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/models/newbasemodel.py` & `ormar-0.9.9/ormar/models/newbasemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,16 @@
             model = (
                 object.__getattribute__(self, "Meta")
                 .model_fields[name]
                 .expand_relationship(value=value, child=self)
             )
             if isinstance(object.__getattribute__(self, "__dict__").get(name), list):
                 # virtual foreign key or many to many
+                # TODO: Fix double items in dict, no effect on real action ugly repr
+                # if model.pk not in [x.pk for  x in related_list]:
                 object.__getattribute__(self, "__dict__")[name].append(model)
             else:
                 # foreign key relation
                 object.__getattribute__(self, "__dict__")[name] = model
                 self.set_save_status(False)
         else:
             if name in object.__getattribute__(self, "_choices_fields"):
```

### Comparing `ormar-0.9.8/ormar/models/quick_access_views.py` & `ormar-0.9.9/ormar/models/quick_access_views.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/protocols/queryset_protocol.py` & `ormar-0.9.9/ormar/protocols/queryset_protocol.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/actions/filter_action.py` & `ormar-0.9.9/ormar/queryset/actions/filter_action.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/actions/order_action.py` & `ormar-0.9.9/ormar/queryset/actions/order_action.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/actions/query_action.py` & `ormar-0.9.9/ormar/queryset/actions/query_action.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/clause.py` & `ormar-0.9.9/ormar/queryset/clause.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/filter_query.py` & `ormar-0.9.9/ormar/queryset/filter_query.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/join.py` & `ormar-0.9.9/ormar/queryset/join.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from collections import OrderedDict
 from typing import (
     Any,
+    Dict,
     List,
     Optional,
     TYPE_CHECKING,
     Tuple,
     Type,
+    cast,
 )
 
 import sqlalchemy
 from sqlalchemy import text
 
 import ormar  # noqa I100
-from ormar.exceptions import RelationshipInstanceError
+from ormar.exceptions import ModelDefinitionError, RelationshipInstanceError
 from ormar.relations import AliasManager
 
 if TYPE_CHECKING:  # pragma no cover
-    from ormar import Model
+    from ormar import Model, ManyToManyField
     from ormar.queryset import OrderAction
     from ormar.models.excludable import ExcludableItems
 
 
 class SqlJoin:
     def __init__(  # noqa:  CFQ002
         self,
@@ -32,22 +34,26 @@
         sorted_orders: OrderedDict,
         main_model: Type["Model"],
         relation_name: str,
         relation_str: str,
         related_models: Any = None,
         own_alias: str = "",
         source_model: Type["Model"] = None,
+        already_sorted: Dict = None,
     ) -> None:
         self.relation_name = relation_name
         self.related_models = related_models or []
         self.select_from = select_from
         self.columns = columns
         self.excludable = excludable
+
         self.order_columns = order_columns
         self.sorted_orders = sorted_orders
+        self.already_sorted = already_sorted or dict()
+
         self.main_model = main_model
         self.own_alias = own_alias
         self.used_aliases = used_aliases
         self.target_field = self.main_model.Meta.model_fields[self.relation_name]
 
         self._next_model: Optional[Type["Model"]] = None
         self._next_alias: Optional[str] = None
@@ -201,14 +207,15 @@
             sorted_orders=self.sorted_orders,
             main_model=self.next_model,
             relation_name=related_name,
             related_models=remainder,
             relation_str="__".join([self.relation_str, related_name]),
             own_alias=self.next_alias,
             source_model=self.source_model or self.main_model,
+            already_sorted=self.already_sorted,
         )
         (
             self.used_aliases,
             self.select_from,
             self.columns,
             self.sorted_orders,
         ) = sql_join.build_join()
@@ -303,39 +310,92 @@
             self.alias_manager.prefixed_columns(
                 self.next_alias, target_table, self_related_fields
             )
         )
         self.used_aliases.append(self.next_alias)
 
     def _set_default_primary_key_order_by(self) -> None:
-        clause = ormar.OrderAction(
-            order_str=self.next_model.Meta.pkname,
-            model_cls=self.next_model,
-            alias=self.next_alias,
-        )
-        self.sorted_orders[clause] = clause.get_text_clause()
+        for order_by in self.next_model.Meta.orders_by:
+            clause = ormar.OrderAction(
+                order_str=order_by, model_cls=self.next_model, alias=self.next_alias,
+            )
+            self.sorted_orders[clause] = clause.get_text_clause()
+
+    def _verify_allowed_order_field(self, order_by: str) -> None:
+        """
+        Verifies if proper field string is used.
+        :param order_by: string with order by definition
+        :type order_by: str
+        """
+        parts = order_by.split("__")
+        if len(parts) > 2 or parts[0] != self.target_field.through.get_name():
+            raise ModelDefinitionError(
+                "You can order the relation only " "by related or link table columns!"
+            )
+
+    def _get_alias_and_model(self, order_by: str) -> Tuple[str, Type["Model"]]:
+        """
+        Returns proper model and alias to be applied in the clause.
+
+        :param order_by: string with order by definition
+        :type order_by: str
+        :return: alias and model to be used in clause
+        :rtype: Tuple[str, Type["Model"]]
+        """
+        if self.target_field.is_multi and "__" in order_by:
+            self._verify_allowed_order_field(order_by=order_by)
+            alias = self.next_alias
+            model = self.target_field.owner
+        elif self.target_field.is_multi:
+            alias = self.alias_manager.resolve_relation_alias(
+                from_model=self.target_field.through,
+                relation_name=cast(
+                    "ManyToManyField", self.target_field
+                ).default_target_field_name(),
+            )
+            model = self.target_field.to
+        else:
+            alias = self.alias_manager.resolve_relation_alias(
+                from_model=self.target_field.owner,
+                relation_name=self.target_field.name,
+            )
+            model = self.target_field.to
+
+        return alias, model
 
     def _get_order_bys(self) -> None:  # noqa: CCR001
         """
         Triggers construction of order bys if they are given.
         Otherwise by default each table is sorted by a primary key column asc.
         """
         alias = self.next_alias
+        current_table_sorted = False
+        if f"{alias}_{self.next_model.get_name()}" in self.already_sorted:
+            current_table_sorted = True
         if self.order_columns:
-            current_table_sorted = False
             for condition in self.order_columns:
                 if condition.check_if_filter_apply(
                     target_model=self.next_model, alias=alias
                 ):
                     current_table_sorted = True
                     self.sorted_orders[condition] = condition.get_text_clause()
-            if not current_table_sorted and not self.target_field.is_multi:
-                self._set_default_primary_key_order_by()
+                    self.already_sorted[
+                        f"{self.next_alias}_{self.next_model.get_name()}"
+                    ] = condition
+        if self.target_field.orders_by and not current_table_sorted:
+            current_table_sorted = True
+            for order_by in self.target_field.orders_by:
+                alias, model = self._get_alias_and_model(order_by=order_by)
+                clause = ormar.OrderAction(
+                    order_str=order_by, model_cls=model, alias=alias
+                )
+                self.sorted_orders[clause] = clause.get_text_clause()
+                self.already_sorted[f"{alias}_{model.get_name()}"] = clause
 
-        elif not self.target_field.is_multi:
+        if not current_table_sorted and not self.target_field.is_multi:
             self._set_default_primary_key_order_by()
 
     def _get_to_and_from_keys(self) -> Tuple[str, str]:
         """
         Based on the relation type, name of the relation and previous models and parts
         stored in JoinParameters it resolves the current to and from keys, which are
         different for ManyToMany relation, ForeignKey and reverse related of relations.
```

### Comparing `ormar-0.9.8/ormar/queryset/limit_query.py` & `ormar-0.9.9/ormar/queryset/limit_query.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/offset_query.py` & `ormar-0.9.9/ormar/queryset/offset_query.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/order_query.py` & `ormar-0.9.9/ormar/queryset/order_query.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/prefetch_query.py` & `ormar-0.9.9/ormar/queryset/prefetch_query.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/queryset/query.py` & `ormar-0.9.9/ormar/queryset/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,22 +59,31 @@
 
     def apply_order_bys_for_primary_model(self) -> None:  # noqa: CCR001
         """
         Applies order_by queries on main model when it's used as a subquery.
         That way the subquery with limit and offset only on main model has proper
         sorting applied and correct models are fetched.
         """
+        current_table_sorted = False
         if self.order_columns:
             for clause in self.order_columns:
                 if clause.is_source_model_order:
+                    current_table_sorted = True
                     self.sorted_orders[clause] = clause.get_text_clause()
-        else:
-            clause = ormar.OrderAction(
-                order_str=self.model_cls.Meta.pkname, model_cls=self.model_cls
-            )
+
+        if not current_table_sorted:
+            self._apply_default_model_sorting()
+
+    def _apply_default_model_sorting(self) -> None:
+        """
+        Applies orders_by from model Meta class (if provided), if it was not provided
+        it was filled by metaclass so it's always there and falls back to pk column
+        """
+        for order_by in self.model_cls.Meta.orders_by:
+            clause = ormar.OrderAction(order_str=order_by, model_cls=self.model_cls)
             self.sorted_orders[clause] = clause.get_text_clause()
 
     def _pagination_query_required(self) -> bool:
         """
         Checks if limit or offset are set, the flag limit_sql_raw is not set
         and query has select_related applied. Otherwise we can limit/offset normally
         at the end of whole query.
```

### Comparing `ormar-0.9.8/ormar/queryset/queryset.py` & `ormar-0.9.9/ormar/queryset/queryset.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import databases
 import sqlalchemy
 from sqlalchemy import bindparam
 
 import ormar  # noqa I100
 from ormar import MultipleMatches, NoMatch
 from ormar.exceptions import ModelError, ModelPersistenceError, QueryDefinitionError
-from ormar.queryset import FilterQuery
+from ormar.queryset import FilterQuery, SelectAction
 from ormar.queryset.actions.order_action import OrderAction
 from ormar.queryset.clause import FilterGroup, QueryClause
 from ormar.queryset.prefetch_query import PrefetchQuery
 from ormar.queryset.query import Query
 
 if TYPE_CHECKING:  # pragma no cover
     from ormar import Model
@@ -553,14 +553,79 @@
         :return: number of rows
         :rtype: int
         """
         expr = self.build_select_expression().alias("subquery_for_count")
         expr = sqlalchemy.func.count().select().select_from(expr)
         return await self.database.fetch_val(expr)
 
+    async def _query_aggr_function(self, func_name: str, columns: List) -> Any:
+        func = getattr(sqlalchemy.func, func_name)
+        select_actions = [
+            SelectAction(select_str=column, model_cls=self.model) for column in columns
+        ]
+        if func_name in ["sum", "avg"]:
+            if any(not x.is_numeric for x in select_actions):
+                raise QueryDefinitionError(
+                    "You can use sum and svg only with" "numeric types of columns"
+                )
+        select_columns = [x.apply_func(func, use_label=True) for x in select_actions]
+        expr = self.build_select_expression().alias(f"subquery_for_{func_name}")
+        expr = sqlalchemy.select(select_columns).select_from(expr)
+        # print("\n", expr.compile(compile_kwargs={"literal_binds": True}))
+        result = await self.database.fetch_one(expr)
+        return dict(result) if len(result) > 1 else result[0]  # type: ignore
+
+    async def max(self, columns: Union[str, List[str]]) -> Any:  # noqa: A003
+        """
+        Returns max value of columns for rows matching the given criteria
+        (applied with `filter` and `exclude` if set before).
+
+        :return: max value of column(s)
+        :rtype: Any
+        """
+        if not isinstance(columns, list):
+            columns = [columns]
+        return await self._query_aggr_function(func_name="max", columns=columns)
+
+    async def min(self, columns: Union[str, List[str]]) -> Any:  # noqa: A003
+        """
+        Returns min value of columns for rows matching the given criteria
+        (applied with `filter` and `exclude` if set before).
+
+        :return: min value of column(s)
+        :rtype: Any
+        """
+        if not isinstance(columns, list):
+            columns = [columns]
+        return await self._query_aggr_function(func_name="min", columns=columns)
+
+    async def sum(self, columns: Union[str, List[str]]) -> Any:  # noqa: A003
+        """
+        Returns sum value of columns for rows matching the given criteria
+        (applied with `filter` and `exclude` if set before).
+
+        :return: sum value of columns
+        :rtype: int
+        """
+        if not isinstance(columns, list):
+            columns = [columns]
+        return await self._query_aggr_function(func_name="sum", columns=columns)
+
+    async def avg(self, columns: Union[str, List[str]]) -> Any:
+        """
+        Returns avg value of columns for rows matching the given criteria
+        (applied with `filter` and `exclude` if set before).
+
+        :return: avg value of columns
+        :rtype: Union[int, float, List]
+        """
+        if not isinstance(columns, list):
+            columns = [columns]
+        return await self._query_aggr_function(func_name="avg", columns=columns)
+
     async def update(self, each: bool = False, **kwargs: Any) -> int:
         """
         Updates the model table after applying the filters from kwargs.
 
         You have to either pass a filter to narrow down a query or explicitly pass
         each=True flag to affect whole table.
 
@@ -769,15 +834,15 @@
         if "pk" in kwargs:
             kwargs[pk_name] = kwargs.pop("pk")
         if pk_name not in kwargs or kwargs.get(pk_name) is None:
             return await self.create(**kwargs)
         model = await self.get(pk=kwargs[pk_name])
         return await model.update(**kwargs)
 
-    async def all(self, **kwargs: Any) -> Sequence[Optional["Model"]]:  # noqa: A003
+    async def all(self, **kwargs: Any) -> List[Optional["Model"]]:  # noqa: A003
         """
         Returns all rows from a database for given model for set filter options.
 
         Passing kwargs is a shortcut and equals to calling `filter(**kwrags).all()`.
 
         If there are no rows meeting the criteria an empty list is returned.
 
@@ -902,14 +967,15 @@
         for objt in objects:
             new_kwargs = objt.dict()
             if pk_name not in new_kwargs or new_kwargs.get(pk_name) is None:
                 raise ModelPersistenceError(
                     "You cannot update unsaved objects. "
                     f"{self.model.__name__} has to have {pk_name} filled."
                 )
+            new_kwargs = self.model.parse_non_db_fields(new_kwargs)
             new_kwargs = self.model.substitute_models_with_pks(new_kwargs)
             new_kwargs = self.model.translate_columns_to_aliases(new_kwargs)
             new_kwargs = {"new_" + k: v for k, v in new_kwargs.items() if k in columns}
             ready_objects.append(new_kwargs)
 
         pk_column = self.model_meta.table.c.get(self.model.get_column_alias(pk_name))
         pk_column_name = self.model.get_column_alias(pk_name)
```

### Comparing `ormar-0.9.8/ormar/queryset/utils.py` & `ormar-0.9.9/ormar/queryset/utils.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/relations/alias_manager.py` & `ormar-0.9.9/ormar/relations/alias_manager.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/relations/querysetproxy.py` & `ormar-0.9.9/ormar/relations/querysetproxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     Sequence,
     Set,
     TYPE_CHECKING,
     Union,
     cast,
 )
 
-import ormar
+
+import ormar  # noqa: I100, I202
 from ormar.exceptions import ModelPersistenceError, QueryDefinitionError
 
 if TYPE_CHECKING:  # pragma no cover
     from ormar.relations import Relation
     from ormar.models import Model
     from ormar.queryset import QuerySet
     from ormar import RelationType
@@ -122,18 +123,15 @@
         final_kwargs = {**rel_kwargs, **kwargs}
         if child.pk is None:
             raise ModelPersistenceError(
                 f"You cannot save {child.get_name()} "
                 f"model without primary key set! \n"
                 f"Save the child model first."
             )
-        expr = model_cls.Meta.table.insert()
-        expr = expr.values(**final_kwargs)
-        # print("\n", expr.compile(compile_kwargs={"literal_binds": True}))
-        await model_cls.Meta.database.execute(expr)
+        await model_cls(**final_kwargs).save()
 
     async def update_through_instance(self, child: "Model", **kwargs: Any) -> None:
         """
         Updates a through model instance in the database for m2m relations.
 
         :param kwargs: dict of additional keyword arguments for through instance
         :type kwargs: Any
@@ -181,14 +179,54 @@
         Actual call delegated to QuerySet.
 
         :return: number of rows
         :rtype: int
         """
         return await self.queryset.count()
 
+    async def max(self, columns: Union[str, List[str]]) -> Any:  # noqa: A003
+        """
+        Returns max value of columns for rows matching the given criteria
+        (applied with `filter` and `exclude` if set before).
+
+        :return: max value of column(s)
+        :rtype: Any
+        """
+        return await self.queryset.max(columns=columns)
+
+    async def min(self, columns: Union[str, List[str]]) -> Any:  # noqa: A003
+        """
+        Returns min value of columns for rows matching the given criteria
+        (applied with `filter` and `exclude` if set before).
+
+        :return: min value of column(s)
+        :rtype: Any
+        """
+        return await self.queryset.min(columns=columns)
+
+    async def sum(self, columns: Union[str, List[str]]) -> Any:  # noqa: A003
+        """
+        Returns sum value of columns for rows matching the given criteria
+        (applied with `filter` and `exclude` if set before).
+
+        :return: sum value of columns
+        :rtype: int
+        """
+        return await self.queryset.sum(columns=columns)
+
+    async def avg(self, columns: Union[str, List[str]]) -> Any:
+        """
+        Returns avg value of columns for rows matching the given criteria
+        (applied with `filter` and `exclude` if set before).
+
+        :return: avg value of columns
+        :rtype: Union[int, float, List]
+        """
+        return await self.queryset.avg(columns=columns)
+
     async def clear(self, keep_reversed: bool = True) -> int:
         """
         Removes all related models from given relation.
 
         Removes all through models for m2m relation.
 
         For reverse FK relations keep_reversed flag marks if the reversed models
```

### Comparing `ormar-0.9.8/ormar/relations/relation.py` & `ormar-0.9.9/ormar/relations/relation.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/relations/relation_manager.py` & `ormar-0.9.9/ormar/relations/relation_manager.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/relations/utils.py` & `ormar-0.9.9/ormar/relations/utils.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar/signals/signal.py` & `ormar-0.9.9/ormar/signals/signal.py`

 * *Files identical despite different names*

### Comparing `ormar-0.9.8/ormar.egg-info/PKG-INFO` & `ormar-0.9.9/ormar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ormar
-Version: 0.9.8
+Version: 0.9.9
 Summary: A simple async ORM with fastapi in mind and pydantic validation.
 Home-page: https://github.com/collerek/ormar
 Author: Radosław Drążkiewicz
 Author-email: collerek@gmail.com
 License: MIT
 Description: # ormar
         <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ormar Version: 0.9.8 Summary: A simple async ORM
+Metadata-Version: 2.1 Name: ormar Version: 0.9.9 Summary: A simple async ORM
 with fastapi in mind and pydantic validation. Home-page: https://github.com/
 collerek/ormar Author: RadosÅaw DrÄÅ¼kiewicz Author-email: collerek@gmail.com
 License: MIT Description: # ormar
 [Pypi_version] [Pypi_version] [Build Status] [Coverage] [CodeFactor] [https://
 api.codeclimate.com/v1/badges/186bc79245724864a7aa/maintainability] [https://
 pepy.tech/badge/ormar]
 ### Overview The `ormar` package is an async mini ORM for Python, with support
```

### Comparing `ormar-0.9.8/ormar.egg-info/SOURCES.txt` & `ormar-0.9.9/ormar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 ormar/queryset/query.py
 ormar/queryset/queryset.py
 ormar/queryset/utils.py
 ormar/queryset/actions/__init__.py
 ormar/queryset/actions/filter_action.py
 ormar/queryset/actions/order_action.py
 ormar/queryset/actions/query_action.py
+ormar/queryset/actions/select_action.py
 ormar/relations/__init__.py
 ormar/relations/alias_manager.py
 ormar/relations/querysetproxy.py
 ormar/relations/relation.py
 ormar/relations/relation_manager.py
 ormar/relations/relation_proxy.py
 ormar/relations/utils.py
```

### Comparing `ormar-0.9.8/setup.py` & `ormar-0.9.9/setup.py`

 * *Files identical despite different names*


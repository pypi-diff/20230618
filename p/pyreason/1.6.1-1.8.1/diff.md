# Comparing `tmp/pyreason-1.6.1.tar.gz` & `tmp/pyreason-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.6.1.tar", last modified: Sun Jun 18 17:09:30 2023, max compression
+gzip compressed data, was "pyreason-1.8.1.tar", last modified: Fri Jun 16 11:07:41 2023, max compression
```

## Comparing `pyreason-1.6.1.tar` & `pyreason-1.8.1.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.379417 pyreason-1.6.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-18 17:09:19.000000 pyreason-1.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-18 17:09:19.000000 pyreason-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-18 17:09:30.379417 pyreason-1.6.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-06-18 17:09:19.000000 pyreason-1.6.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.355415 pyreason-1.6.1/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.359415 pyreason-1.6.1/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.363415 pyreason-1.6.1/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    28797 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.363415 pyreason-1.6.1/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.363415 pyreason-1.6.1/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.367416 pyreason-1.6.1/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.367416 pyreason-1.6.1/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.367416 pyreason-1.6.1/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    66970 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.367416 pyreason-1.6.1/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.367416 pyreason-1.6.1/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.371416 pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.371416 pyreason-1.6.1/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.375416 pyreason-1.6.1/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.375416 pyreason-1.6.1/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4587 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9058 2023-06-18 17:09:19.000000 pyreason-1.6.1/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:30.359415 pyreason-1.6.1/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-18 17:09:30.000000 pyreason-1.6.1/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-18 17:09:30.000000 pyreason-1.6.1/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:09:30.000000 pyreason-1.6.1/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 17:09:30.000000 pyreason-1.6.1/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 17:09:30.000000 pyreason-1.6.1/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:09:30.379417 pyreason-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-18 17:09:19.000000 pyreason-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.582791 pyreason-1.8.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-16 11:07:31.000000 pyreason-1.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 11:07:31.000000 pyreason-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-16 11:07:41.582791 pyreason-1.8.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-06-16 11:07:31.000000 pyreason-1.8.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27957 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    74858 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-06-16 11:07:31.000000 pyreason-1.8.1/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.574791 pyreason-1.8.1/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 11:07:41.000000 pyreason-1.8.1/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 11:07:41.582791 pyreason-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-16 11:07:31.000000 pyreason-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:07:41.578791 pyreason-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-16 11:07:31.000000 pyreason-1.8.1/tests/test_hello_world.py
```

### Comparing `pyreason-1.6.1/LICENSE.md` & `pyreason-1.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/PKG-INFO` & `pyreason-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.6.1
+Version: 1.8.1
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.6.1/README.md` & `pyreason-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/__init__.py` & `pyreason-1.8.1/pyreason/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # Set numba environment variable
 import os
 package_path = os.path.abspath(os.path.dirname(__file__))
 cache_path = os.path.join(package_path, 'cache')
 cache_status_path = os.path.join(package_path, '.cache_status.yaml')
-os.environ['NUMBA_CACHE_DIR'] =  cache_path
+os.environ['NUMBA_CACHE_DIR'] = cache_path
+
 
 from pyreason.pyreason import *
 import yaml
 
 
 with open(cache_status_path) as file:
     cache_status = yaml.safe_load(file)
 
 if not cache_status['initialized']:
     print('Imported PyReason for the first time. Initializing ... this will take a minute')
     graph_path = os.path.join(package_path, 'examples', 'hello-world', 'friends.graphml')
-    labels_path = os.path.join(package_path, 'examples', 'hello-world', 'labels.yaml')
-    facts_path = os.path.join(package_path, 'examples', 'hello-world', 'facts.yaml')
-    rules_path = os.path.join(package_path, 'examples', 'hello-world', 'rules.yaml')
-    ipl_path = os.path.join(package_path, 'examples', 'hello-world', 'ipl.yaml')
 
     settings.verbose = False
     load_graph(graph_path)
-    load_labels(labels_path)
-    load_facts(facts_path)
-    load_rules(rules_path)
-    load_inconsistent_predicate_list(ipl_path)
+    add_rule('popular(x) <-1 popular(y), Friends(x,y), owns(y,z), owns(x,z)', 'popular_rule')
+    add_fact(Fact('popular-fact', 'Mary', 'popular', [1, 1], 0, 2))
     reason(timesteps=2)
 
     # Update cache status
     cache_status['initialized'] = True
     with open(cache_status_path, 'w') as file:
         yaml.dump(cache_status, file)
```

### Comparing `pyreason-1.6.1/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.8.1/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.8.1/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.8.1/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/pyreason.py` & `pyreason-1.8.1/pyreason/pyreason.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # This is the file that will be imported when "import pyreason" is called. All content will be run automatically
 import numba
 import time
 import sys
 import warnings
-import numpy as np
 import memory_profiler as mp
 from typing import List, Type
 
 from pyreason.scripts.utils.output import Output
 from pyreason.scripts.utils.filter import Filter
 from pyreason.scripts.program.program import Program
 from pyreason.scripts.utils.graphml_parser import GraphmlParser
 import pyreason.scripts.utils.yaml_parser as yaml_parser
+import pyreason.scripts.utils.rule_parser as rule_parser
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.rule_type as rule
+from pyreason.scripts.facts.fact import Fact
 import pyreason.scripts.numba_wrapper.numba_types.fact_node_type as fact_node
 import pyreason.scripts.numba_wrapper.numba_types.fact_edge_type as fact_edge
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 
 
 # USER VARIABLES
 class _Settings:
@@ -336,14 +337,22 @@
     global __node_facts, __edge_facts, __node_labels, __edge_labels
     __node_facts = None
     __edge_facts = None
     __node_labels = None
     __edge_labels = None
 
 
+def reset_rules():
+    """
+    Resets rules to none
+    """
+    global __rules
+    __rules = None
+
+
 # FUNCTIONS
 def load_graph(path: str) -> None:
     """Loads graph from GraphMl file path into program
 
     :param path: Path for the GraphMl file
     """
     global __graph, __graphml_parser, __non_fluent_graph_facts_node, __non_fluent_graph_facts_edge, __specific_graph_node_labels, __specific_graph_edge_labels, settings
@@ -397,111 +406,76 @@
 
     :param path: Path for the YAML IPL file
     """
     global __ipl
     __ipl = yaml_parser.parse_ipl(path)
 
 
-def add_rules_from_text(rule_text: str, name: str) -> None:
+def add_rule(rule_text: str, name: str, infer_edges: bool = False, immediate_rule: bool = False) -> None:
     """Add a rule to pyreason from text format. This format is not as modular as the YAML format.
-    1. It is not possible to specify target criteria
-    2. It is not possible to specify delta_t. delta_t=0 by default.
-    3. It is not possible to specify thresholds. Threshold is greater than or equal to 1 by default
-    4. It is not possible to add edges between subsets of nodes
-    5. It is not possible to have an annotation function. We set to [1,1] by default
-    6. It is not possible to have weights for different clauses. Weights are 1 by default with bias 0
+    1. It is not possible to specify thresholds. Threshold is greater than or equal to 1 by default
+    2. It is not possible to have an annotation function.
+    3. It is not possible to have weights for different clauses. Weights are 1 by default with bias 0
+    TODO: Add threshold class where we can pass this as a parameter
+    TODO: Add weights as a parameter
+    TODO: Add annotation function and bounds as a parameter
 
     Example:
-    `'pred1(x,y) <- pred2(a, b), pred3(b, c)'`
+    `'pred1(x,y) : [0.2, 1] <- pred2(a, b) : [1,1], pred3(b, c)'`
 
     :param rule_text: The rule in text format
     :param name: The name of the rule. This will appear in the rule trace
+    :param infer_edges: Whether to infer new edges after edge rule fires
+    :param immediate_rule: Whether the rule is immediate. Immediate rules check for more applicable rules immediately after being applied
     """
     global __rules
 
-    # First remove all spaces from line
-    r = rule_text.replace(' ', '')
+    r = rule_parser.parse_rule(rule_text, name, infer_edges, immediate_rule)
+    # Add to collection of rules
+    if __rules is None:
+        __rules = numba.typed.List.empty_list(rule.rule_type)
+    __rules.append(r)
+
 
-    # Separate into head and body
-    head, body = r.split('<-')
+def add_rules_from_file(file_path: str, infer_edges: bool = False) -> None:
+    """ Add a set of rules from a text file
 
-    # Separate clauses in body
-    body = body[:-1].replace(')', '))') + ')'
-    body = body.split('),')
-
-    # Find the target predicate
-    idx = head.find('(')
-    target = head[:idx]
-    target = label.Label(target)
-
-    # Variable(s) in the head of the rule
-    head_variables = head[idx + 1:-1].split(',')
-
-    # Target criteria is empty for this text format to pyreason rule
-    target_criteria = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, interval.interval_type)))
-
-    # Get the variables in the body
-    body_predicates = []
-    body_variables = []
-    for clause in body:
-        idx = clause.find('(')
-        body_predicates.append(clause[:idx])
-        body_variables.append(clause[idx+1:-1].split(','))
-
-    # Replace the variables in the body with source/target if they match the variables in the head
-    head_var_map = {0: 'source', 1: 'target'}
-    for i in range(len(body_variables)):
-        for j in range(len(body_variables[i])):
-            # Loop through the head variables and see if there's a match
-            for k in range(len(head_variables)):
-                if body_variables[i][j] == head_variables[k]:
-                    body_variables[i][j] = head_var_map[k] if len(head_variables) == 2 else 'target'
-
-    # Start setting up neigh_criteria
-    # neigh_criteria = [c1, c2, c3, c4]
-    # thresholds = [t1, t2, t3, t4]
-
-    # Array of thresholds to keep track of for each neighbor criterion. Form [(comparison, (number/percent, total/available), thresh)]
-    thresholds = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), numba.types.float64)))
-
-    # Array to store clauses for nodes: node/edge, [subset]/[subset1, subset2], label, interval
-    neigh_criteria = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), label.label_type, interval.interval_type)))
-
-    # Loop though clauses
-    for predicate, variables in zip(body_predicates, body_variables):
-        # Neigh criteria
-        clause_type = 'node' if len(variables) == 1 else 'edge'
-        subset = (variables[0], variables[0]) if clause_type == 'node' else (variables[0], variables[1])
-        l = label.Label(predicate)
-        bnd = interval.closed(1, 1)
-        neigh_criteria.append((clause_type, subset, l, bnd))
-
-        # Threshold
-        quantifier = 'greater_equal'
-        quantifier_type = ('number', 'total')
-        thresh = 1
-        thresholds.append((quantifier, quantifier_type, thresh))
-
-    # Cannot add edges
-    edges = ('', '', label.Label(''))
-
-    # Bound to set atom if rule fires
-    bnd = interval.closed(1, 1)
-    ann_fn = ''
-    ann_label = label.Label('')
+    :param file_path: Path to the text file containing rules
+    :type file_path: str
+    :param infer_edges: Whether to infer edges on these rules if an edge doesn't exist between head variables and the body of the rule is satisfied
+    :type infer_edges: bool
+    :return: None
+    """
+    with open(file_path, 'r') as file:
+        rules = [line.rstrip() for line in file]
 
-    weights = np.ones(len(body_predicates), dtype=np.float64)
-    weights = np.append(weights, 0)
+    rule_offset = 0 if __rules is None else len(__rules)
+    for i, r in enumerate(rules):
+        add_rule(r, f'rule_{i+rule_offset}', infer_edges)
 
-    r = rule.Rule(name, target, target_criteria, numba.types.uint16(0), neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges)
 
-    # Add to collection of rules
-    if __rules is None:
-        __rules = numba.typed.List.empty_list(rule.rule_type)
-    __rules.append(r)
+def add_fact(pyreason_fact: Fact) -> None:
+    """Add a PyReason fact to the program.
+
+    :param pyreason_fact: PyReason fact created using pr.Fact(...)
+    :return: None
+    """
+    global __node_facts, __edge_facts
+
+    if pyreason_fact.type == 'node':
+        f = fact_node.Fact(pyreason_fact.name, pyreason_fact.component, pyreason_fact.label, pyreason_fact.interval, pyreason_fact.t_lower, pyreason_fact.t_upper, pyreason_fact.static)
+        if __node_facts is None:
+            __node_facts = numba.typed.List.empty_list(fact_node.fact_type)
+        __node_facts.append(f)
+
+    else:
+        f = fact_edge.Fact(pyreason_fact.name, pyreason_fact.component, pyreason_fact.label, pyreason_fact.interval, pyreason_fact.t_lower, pyreason_fact.t_upper, pyreason_fact.static)
+        if __edge_facts is None:
+            __edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
+        __edge_facts.append(f)
 
 
 def reason(timesteps: int=-1, convergence_threshold: int=-1, convergence_bound_threshold: float=-1, again: bool=False, node_facts: List[Type[fact_node.Fact]]=None, edge_facts: List[Type[fact_edge.Fact]]=None):
     """Function to start the main reasoning process. Graph and rules must already be loaded.
 
     :param timesteps: Max number of timesteps to run. -1 specifies run till convergence. If reasoning again, this is the number of timesteps to reason for extra (no zero timestep), defaults to -1
     :param convergence_threshold: Maximim number of interpretations that have changed between timesteps or fixed point operations until considered convergent. Program will end at convergence. -1 => no changes, perfect convergence, defaults to -1
@@ -560,16 +534,18 @@
         __node_labels = numba.typed.List.empty_list(label.label_type)
         __edge_labels = numba.typed.List.empty_list(label.label_type)
         __specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.string))
         __specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.Tuple((numba.types.string, numba.types.string))))
 
     if __node_facts is None and __edge_facts is None:
         if settings.verbose:
-            warnings.warn('Facts yaml file has not been loaded. Use `load_facts`. Only graph attributes will be used as facts\n')
+            warnings.warn('Facts have not been loaded. Use `add_fact` or `load_facts`. Only graph attributes will be used as facts\n')
+    if __node_facts is None:
         __node_facts = numba.typed.List.empty_list(fact_node.fact_type)
+    if __edge_facts is None:
         __edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
 
     if __ipl is None:
         if settings.verbose:
             warnings.warn('Inconsistent Predicate List yaml file has not been loaded. Use `load_ipl`. Loading IPL is optional\n')
         __ipl = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, label.label_type)))
 
@@ -582,16 +558,18 @@
 
     for label_name, edges in __specific_graph_edge_labels.items():
         if label_name in __specific_edge_labels:
             __specific_edge_labels[label_name].extend(edges)
         else:
             __specific_edge_labels[label_name] = edges
 
-    all_node_facts = numba.typed.List(__node_facts)
-    all_edge_facts = numba.typed.List(__edge_facts)
+    all_node_facts = numba.typed.List.empty_list(fact_node.fact_type)
+    all_edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
+    all_node_facts.extend(numba.typed.List(__node_facts))
+    all_edge_facts.extend(numba.typed.List(__edge_facts))
     all_node_facts.extend(__non_fluent_graph_facts_node)
     all_edge_facts.extend(__non_fluent_graph_facts_edge)
 
     # Atom trace cannot be true when store interpretations is false
     if not settings.store_interpretation_changes:
         settings.atom_trace = False
```

### Comparing `pyreason-1.6.1/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.8.1/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/args.py` & `pyreason-1.8.1/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/components/world.py` & `pyreason-1.8.1/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/diffuse.py` & `pyreason-1.8.1/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.8.1/pyreason/scripts/facts/fact_edge.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,13 +24,16 @@
     def get_time_lower(self):
         return self._t_lower
     
     def get_time_upper(self):
         return self._t_upper
 
     def __str__(self):
-        net_diff_dict = {}
-        net_diff_dict["component"] = str(self._component)
-        net_diff_dict["label"] = str(self._label)
-        net_diff_dict["confidence"] = self._interval.to_str()
-        net_diff_dict["time"] = '[' + str(self._t_lower) + ',' + str(self._t_upper) + ']'
-        return str(net_diff_dict)
+        fact = {
+            "type": 'pyreason edge fact',
+            "name": self._name,
+            "component": self._component,
+            "label": self._label,
+            "confidence": self._interval,
+            "time": '[' + str(self._t_lower) + ',' + str(self._t_upper) + ']'
+        }
+        return fact
```

### Comparing `pyreason-1.6.1/pyreason/scripts/facts/fact_node.py` & `pyreason-1.8.1/pyreason/scripts/facts/fact_node.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,13 +24,16 @@
     def get_time_lower(self):
         return self._t_lower
     
     def get_time_upper(self):
         return self._t_upper
 
     def __str__(self):
-        net_diff_dict = {}
-        net_diff_dict["component"] = str(self._component)
-        net_diff_dict["label"] = str(self._label)
-        net_diff_dict["confidence"] = self._interval.to_str()
-        net_diff_dict["time"] = '[' + str(self._t_lower) + ',' + str(self._t_upper) + ']'
-        return str(net_diff_dict)
+        fact = {
+            "type": 'pyreason node fact',
+            "name": self._name,
+            "component": self._component,
+            "label": self._label,
+            "confidence": self._interval,
+            "time": '[' + str(self._t_lower) + ',' + str(self._t_upper) + ']'
+        }
+        return fact
```

### Comparing `pyreason-1.6.1/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.8.1/pyreason/scripts/interpretation/interpretation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 import pyreason.scripts.numba_wrapper.numba_types.world_type as world
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
-import pyreason.scripts.annotation_functions.annotation_functions as ann_fn
+import pyreason.scripts.annotation_functions.annotation_functions as ann_fns
 
 import numba
 from numba import objmode
 
 
 # Types for the dictionaries
 node_type = numba.types.string
 edge_type = numba.types.UniTuple(numba.types.string, 2)
 
-# Type for storing list of qualified nodes
+# Type for storing list of qualified nodes/edges
 list_of_nodes = numba.types.ListType(node_type)
+list_of_edges = numba.types.ListType(edge_type)
 
-# Type for storing int tuple
-int_tuple = numba.types.UniTuple(numba.types.int64, 2)
+# Type for returning list of applicable rules for a certain rule
+# node/edge, annotations, qualified nodes, qualified edges, edges to be added
+node_applicable_rule_type = numba.types.Tuple((
+	node_type,
+	numba.types.ListType(numba.types.ListType(interval.interval_type)),
+	numba.types.ListType(numba.types.ListType(node_type)),
+	numba.types.ListType(numba.types.ListType(edge_type)),
+	numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type))
+))
+
+edge_applicable_rule_type = numba.types.Tuple((
+	edge_type,
+	numba.types.ListType(numba.types.ListType(interval.interval_type)),
+	numba.types.ListType(numba.types.ListType(node_type)),
+	numba.types.ListType(numba.types.ListType(edge_type)),
+	numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type))
+))
 
 
 class Interpretation:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(node_type))
 	specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(edge_type))
@@ -68,22 +84,40 @@
 		if len(self.available_labels_edge)==0:
 			self.available_labels_edge = numba.typed.List.empty_list(label.label_type)
 		else:
 			self.available_labels_edge = numba.typed.List(self.available_labels_edge)
 
 		self.interpretations_node = self._init_interpretations_node(numba.typed.List(self.graph.nodes()), self.available_labels_node, self.specific_node_labels)
 		self.interpretations_edge = self._init_interpretations_edge(numba.typed.List(self.graph.edges()), self.available_labels_edge, self.specific_edge_labels)
-		
-		# Setup graph neighbors
+
+		# Setup graph neighbors and reverse neighbors
 		self.neighbors = numba.typed.Dict.empty(key_type=node_type, value_type=numba.types.ListType(node_type))
 		for n in self.graph.nodes():
 			l = numba.typed.List.empty_list(node_type)
 			[l.append(neigh) for neigh in self.graph.neighbors(n)]
 			self.neighbors[n] = l
 
+		self.reverse_neighbors = self._init_reverse_neighbors(self.neighbors)
+
+	@staticmethod
+	@numba.njit(cache=True)
+	def _init_reverse_neighbors(neighbors):
+		reverse_neighbors = numba.typed.Dict.empty(key_type=node_type, value_type=list_of_nodes)
+		for n, neighbor_nodes in neighbors.items():
+			for neighbor_node in neighbor_nodes:
+				if neighbor_node in reverse_neighbors and n not in reverse_neighbors[neighbor_node]:
+					reverse_neighbors[neighbor_node].append(n)
+				else:
+					reverse_neighbors[neighbor_node] = numba.typed.List([n])
+			# This makes sure each node has a value
+			if n not in reverse_neighbors:
+				reverse_neighbors[n] = numba.typed.List.empty_list(node_type)
+
+		return reverse_neighbors
+
 	@staticmethod
 	@numba.njit(cache=True)
 	def _init_interpretations_node(nodes, available_labels, specific_labels):
 		interpretations = numba.typed.Dict.empty(key_type=node_type, value_type=world.world_type)
 		# General labels
 		for n in nodes:
 			interpretations[n] = world.World(available_labels)
@@ -147,83 +181,78 @@
 				graph_attribute = True if name=='graph-attribute-fact' else False
 				facts_to_be_applied_edge.append((numba.types.uint16(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
 				if atom_trace:
 					facts_to_be_applied_edge_trace.append(fact.get_name())
 		return max_time
 
 	def _start_fp(self, rules, max_facts_time, verbose):
-		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.available_labels_node, self.available_labels_edge, self.specific_node_labels, self.specific_edge_labels, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, self.store_interpretation_changes, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
+		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.reverse_neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, self.store_interpretation_changes, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
 		self.time = t - 1
 		# If we need to reason again, store the next timestep to start from
 		self.prev_reasoning_data[0] = t
 		self.prev_reasoning_data[1] = fp_cnt
 		if verbose:
 			print('Fixed Point iterations:', fp_cnt)
 
 	@staticmethod
 	@numba.njit(cache=True)
-	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, labels_node, labels_edge, specific_labels_node, specific_labels_edge, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, max_facts_time, convergence_mode, convergence_delta, verbose):
+	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, reverse_neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, max_facts_time, convergence_mode, convergence_delta, verbose):
 		t = prev_reasoning_data[0]
 		fp_cnt = prev_reasoning_data[1]
 		max_rules_time = 0
 		timestep_loop = True
 		facts_to_remove_idx = numba.typed.List.empty_list(numba.types.int64)
 		rules_to_remove_idx = numba.typed.List.empty_list(numba.types.int64)
 		while timestep_loop:
 			if t==tmax:
-				timestep_loop=False
+				timestep_loop = False
 			if verbose:
 				with objmode():
 					print('Timestep:', t, flush=True)
 			# Reset Interpretation at beginning of timestep if non-canonical
 			if t>0 and not canonical:
 				# Reset nodes (only if not static)
-				# General labels
 				for n in nodes:
-					for l in labels_node:
-						if not interpretations_node[n].world[l].is_static():
-							interpretations_node[n].world[l].reset()
-				# Specific labels
-				for l, ns in specific_labels_node.items():
-					for n in ns:
-						if not interpretations_node[n].world[l].is_static():
-							interpretations_node[n].world[l].reset()				
-				# Reset edges
-				# General labels
+					w = interpretations_node[n].world
+					for l in w:
+						if not w[l].is_static():
+							w[l].reset()
+
+				# Reset edges (only if not static)
 				for e in edges:
-					for l in labels_edge:
-						if not interpretations_edge[e].world[l].is_static():
-							interpretations_edge[e].world[l].reset()
-				# Specific labels
-				for l, es in specific_labels_edge.items():
-					for e in es:
-						if not interpretations_edge[e].world[l].is_static():
-							interpretations_edge[e].world[l].reset()
+					w = interpretations_edge[e].world
+					for l in w:
+						if not w[l].is_static():
+							w[l].reset()
 
 			# Convergence parameters
 			changes_cnt = 0
 			bound_delta = 0
 			update = False
 
 			# Parameters for immediate rules
 			immediate_node_rule_fire = False
 			immediate_edge_rule_fire = False
 			immediate_rule_applied = False
 			# When delta_t = 0, we don't want to check the same rule with the same node/edge after coming back to the fp operator
-			nodes_to_skip = numba.typed.List.empty_list(int_tuple)
-			edges_to_skip = numba.typed.List.empty_list(int_tuple)
+			nodes_to_skip = numba.typed.Dict.empty(key_type=numba.types.int64, value_type=list_of_nodes)
+			edges_to_skip = numba.typed.Dict.empty(key_type=numba.types.int64, value_type=list_of_edges)
+			# Initialize the above
+			for i in range(len(rules)):
+				nodes_to_skip[i] = numba.typed.List.empty_list(node_type)
+				edges_to_skip[i] = numba.typed.List.empty_list(edge_type)
 
 			# Start by applying facts
 			# Nodes
 			facts_to_remove_idx.clear()
 			for i in range(len(facts_to_be_applied_node)):
 				if facts_to_be_applied_node[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_node[i][1], facts_to_be_applied_node[i][2], facts_to_be_applied_node[i][3], facts_to_be_applied_node[i][4], facts_to_be_applied_node[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute and add ipl complement to rule trace as well
-					if interpretations_node[comp].world[l].is_static():
+					if l in interpretations_node[comp].world and interpretations_node[comp].world[l].is_static():
 						# Check if we should even store any of the changes to the rule trace etc.
 						# Inverse of this is: if not save_graph_attributes_to_rule_trace and graph_attribute
 						if (save_graph_attributes_to_rule_trace or not graph_attribute) and store_interpretation_changes:
 							rule_trace_node.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, l, bnd))
 							if atom_trace:
 								_update_rule_trace(rule_trace_node_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), bnd, facts_to_be_applied_node_trace[i])
 							for p1, p2 in ipl:
@@ -274,15 +303,15 @@
 
 			# Edges
 			facts_to_remove_idx.clear()
 			for i in range(len(facts_to_be_applied_edge)):
 				if facts_to_be_applied_edge[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_edge[i][1], facts_to_be_applied_edge[i][2], facts_to_be_applied_edge[i][3], facts_to_be_applied_edge[i][4], facts_to_be_applied_edge[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute, and add ipl complement to rule trace as well
-					if interpretations_edge[comp].world[l].is_static():
+					if l in interpretations_edge[comp].world and interpretations_edge[comp].world[l].is_static():
 						# Inverse of this is: if not save_graph_attributes_to_rule_trace and graph_attribute
 						if (save_graph_attributes_to_rule_trace or not graph_attribute) and store_interpretation_changes:
 							rule_trace_edge.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, l, interpretations_edge[comp].world[l]))
 							if atom_trace:
 								_update_rule_trace(rule_trace_edge_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), bnd, facts_to_be_applied_edge_trace[i])
 							for p1, p2 in ipl:
 								if p1==l:
@@ -496,15 +525,15 @@
 							# If t=0 we want to apply one rule and go back to the fp operator
 							# If t>0 we want to come back here and apply the rest of the rules
 							if immediate_edge_rule_fire:
 								break
 							elif not immediate_edge_rule_fire and u:
 								immediate_rule_applied = True
 								break
-								
+
 				# Remove from rules to be applied and edges to be applied lists after coming out from loop
 				rules_to_be_applied_edge[:] = numba.typed.List([rules_to_be_applied_edge[i] for i in range(len(rules_to_be_applied_edge)) if i not in rules_to_remove_idx])
 				edges_to_be_added_edge_rule[:] = numba.typed.List([edges_to_be_added_edge_rule[i] for i in range(len(edges_to_be_added_edge_rule)) if i not in rules_to_remove_idx])
 
 				# Fixed point
 				# if update or immediate_node_rule_fire or immediate_edge_rule_fire or immediate_rule_applied:
 				if update:
@@ -513,87 +542,79 @@
 						fp_cnt += 1
 
 					for i in range(len(rules)):
 						rule = rules[i]
 						immediate_rule = rule.is_immediate_rule()
 						immediate_node_rule_fire = False
 						immediate_edge_rule_fire = False
-						# Go through all nodes and check if any rules apply to them
-						# Only go through everything if the rule can be applied within the given timesteps, or we're running until convergence or it's an immediate rule.
-						# Otherwise, it's an unnecessary loop
+
+						# Only go through if the rule can be applied within the given timesteps, or we're running until convergence
 						delta_t = rule.get_delta()
-						if t+delta_t<=tmax or tmax==-1:
-							for j in range(len(nodes)):
-								if (i, j) in nodes_to_skip:
-									continue
-								n = nodes[j]
-								target_criteria_satisfaction = are_satisfied_node(interpretations_node, n, rule.get_target_criteria())
-								if (target_criteria_satisfaction and is_satisfied_node(interpretations_node, n, (rule.get_target(), interval.closed(0,1)))) or (target_criteria_satisfaction and rule.get_target().value==''):
-									result, annotations, qualified_nodes, qualified_edges, edges_to_add = _is_rule_applicable(interpretations_node, interpretations_edge, neighbors, n, rule.get_neigh_criteria(), rule.get_thresholds(), reverse_graph, rule.get_annotation_function(), rule.get_annotation_label(), rule.get_edges(), atom_trace)
-									if (result and rule.get_target().value=='') or (result and not interpretations_node[n].world[rule.get_target()].is_static()):
-										bnd = influence(rule, annotations, rule.get_weights())
-										max_rules_time = max(max_rules_time, t+delta_t)
-										edges_to_be_added_node_rule.append(edges_to_add)
-										rules_to_be_applied_node.append((numba.types.uint16(t+delta_t), n, rule.get_target(), bnd, immediate_rule))
-										if atom_trace:
-											rules_to_be_applied_node_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
-
-										# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
-										nodes_to_skip.append((i, j))
-
-										# Handle loop parameters for the next (maybe) fp operation
-										# If it is a t=0 rule or an immediate rule we want to go back for another fp operation to check for new rules that may fire
-										# Next fp operation we will skip this rule on this node because anyway there won't be an update
-										if delta_t==0:
-											in_loop = True
-											update = False
-										if immediate_rule and delta_t==0:
-											# immediate_rule_fire becomes True because we still need to check for more eligible rules, we're not done.
-											in_loop = True
-											update = True
-											immediate_node_rule_fire = True
-											break
+						if t + delta_t <= tmax or tmax == -1:
+							applicable_node_rules = _ground_node_rule(rule, interpretations_node, interpretations_edge, nodes, neighbors, reverse_neighbors, atom_trace, reverse_graph, nodes_to_skip[i])
+							applicable_edge_rules = _ground_edge_rule(rule, interpretations_node, interpretations_edge, nodes, edges, neighbors, reverse_neighbors, atom_trace, reverse_graph, edges_to_skip[i])
+
+							# Loop through applicable rules and add them to the rules to be applied for later or next fp operation
+							for applicable_rule in applicable_node_rules:
+								n, annotations, qualified_nodes, qualified_edges, edges_to_add = applicable_rule
+								# If there is an edge to add or the predicate doesn't exist or the interpretation is not static
+								if len(edges_to_add[0]) > 0 or rule.get_target() not in interpretations_node[n].world or not interpretations_node[n].world[rule.get_target()].is_static():
+									bnd = influence(rule, annotations, rule.get_weights())
+									max_rules_time = max(max_rules_time, t + delta_t)
+									edges_to_be_added_node_rule.append(edges_to_add)
+									rules_to_be_applied_node.append((numba.types.uint16(t + delta_t), n, rule.get_target(), bnd, immediate_rule))
+									if atom_trace:
+										rules_to_be_applied_node_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
+
+									# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
+									nodes_to_skip[i].append(n)
+
+									# Handle loop parameters for the next (maybe) fp operation
+									# If it is a t=0 rule or an immediate rule we want to go back for another fp operation to check for new rules that may fire
+									# Next fp operation we will skip this rule on this node because anyway there won't be an update
+									if delta_t == 0:
+										in_loop = True
+										update = False
+									if immediate_rule and delta_t == 0:
+										# immediate_rule_fire becomes True because we still need to check for more eligible rules, we're not done.
+										in_loop = True
+										update = True
+										immediate_node_rule_fire = True
+										break
 
 							# Break, apply immediate rule then come back to check for more applicable rules
 							if immediate_node_rule_fire:
 								break
 
-							# Go through all edges and check if any rules apply to them.
-							# Comment out the following lines if there are no labels or rules that deal with edges. It will be an unnecessary loop
-							for j in range(len(edges)):
-								if (i, j) in edges_to_skip:
-									continue
-								e = edges[j]
-								target_criteria_satisfaction = are_satisfied_edge(interpretations_edge, e, rule.get_target_criteria())
-								if (target_criteria_satisfaction and is_satisfied_node(interpretations_edge, e, (rule.get_target(), interval.closed(0,1)))) or (target_criteria_satisfaction and rule.get_target().value==''):
-									# Find out if rule is applicable. returns list of list, of qualified nodes and qualified edges. one for each clause
-									result, annotations, qualified_nodes, qualified_edges, edges_to_add = _is_rule_applicable_edge(interpretations_node, interpretations_edge, neighbors, e, rule.get_neigh_criteria(), rule.get_thresholds(), reverse_graph, rule.get_annotation_function(), rule.get_annotation_label(), rule.get_edges(), atom_trace)
-									if (result and rule.get_target().value=='') or (result and not interpretations_edge[e].world[rule.get_target()].is_static()):
-										bnd = influence(rule, annotations, rule.get_weights())
-										max_rules_time = max(max_rules_time, t+delta_t)
-										edges_to_be_added_edge_rule.append(edges_to_add)
-										rules_to_be_applied_edge.append((numba.types.uint16(t+delta_t), e, rule.get_target(), bnd, immediate_rule))
-										if atom_trace:
-											rules_to_be_applied_edge_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
-
-										# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
-										edges_to_skip.append((i, j))
-
-										# Handle loop parameters for the next (maybe) fp operation
-										# If it is a t=0 rule or an immediate rule we want to go back for another fp operation to check for new rules that may fire
-										# Next fp operation we will skip this rule on this node because anyway there won't be an update
-										if delta_t==0:
-											in_loop = True
-											update = False
-										if immediate_rule and delta_t == 0:
-											# immediate_rule_fire becomes True because we still need to check for more eligible rules, we're not done.
-											in_loop = True
-											update = True
-											immediate_edge_rule_fire = True
-											break
+							for applicable_rule in applicable_edge_rules:
+								e, annotations, qualified_nodes, qualified_edges, edges_to_add = applicable_rule
+								# If there is an edge to add or the predicate doesn't exist or the interpretation is not static
+								if len(edges_to_add[0]) > 0 or rule.get_target() not in interpretations_edge[e].world or not interpretations_edge[e].world[rule.get_target()].is_static():
+									bnd = influence(rule, annotations, rule.get_weights())
+									max_rules_time = max(max_rules_time, t+delta_t)
+									edges_to_be_added_edge_rule.append(edges_to_add)
+									rules_to_be_applied_edge.append((numba.types.uint16(t+delta_t), e, rule.get_target(), bnd, immediate_rule))
+									if atom_trace:
+										rules_to_be_applied_edge_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
+
+									# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
+									edges_to_skip[i].append(e)
+
+									# Handle loop parameters for the next (maybe) fp operation
+									# If it is a t=0 rule or an immediate rule we want to go back for another fp operation to check for new rules that may fire
+									# Next fp operation we will skip this rule on this node because anyway there won't be an update
+									if delta_t == 0:
+										in_loop = True
+										update = False
+									if immediate_rule and delta_t == 0:
+										# immediate_rule_fire becomes True because we still need to check for more eligible rules, we're not done.
+										in_loop = True
+										update = True
+										immediate_edge_rule_fire = True
+										break
 
 							# Break, apply immediate rule then come back to check for more applicable rules
 							if immediate_edge_rule_fire:
 								break
 								
 					# Go through all the rules and go back to applying the rules if we came here because of an immediate rule where delta_t>0
 					if immediate_rule_applied and not (immediate_node_rule_fire or immediate_edge_rule_fire):
@@ -629,263 +650,419 @@
 					# Be consistent with time returned when we don't converge
 					t += 1
 					break
 
 			# Increment t
 			t += 1
 
-		return fp_cnt, t	
+		return fp_cnt, t
 
 
 @numba.njit(cache=True)
-def _is_rule_applicable(interpretations_node, interpretations_edge, neighbors, target_node, neigh_criteria, thresholds, reverse_graph, ann_fn, ann_fn_label, edges, atom_trace):
-	# Initialize dictionary where keys are strings (x1, x2 etc.) and values are lists of qualified neighbors
-	# Keep track of all the edges that are qualified
-	# If it's a node clause update (x1 or x2 etc.) qualified neighbors, if it's an edge clause update the qualified neighbors for the source and target (x1, x2)
-	# First gather all the qualified nodes for each clause
-	subsets = numba.typed.Dict.empty(key_type=numba.types.string, value_type=list_of_nodes)
-	qualified_nodes = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
-	qualified_edges = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
-	annotations = numba.typed.List.empty_list(numba.typed.List.empty_list(interval.interval_type))
-	edges_to_be_added = (numba.typed.List.empty_list(node_type), numba.typed.List.empty_list(node_type), edges[-1])
+def _ground_node_rule(rule, interpretations_node, interpretations_edge, nodes, neighbors, reverse_neighbors, atom_trace, reverse_graph, nodes_to_skip):
+	# Extract rule params
+	rule_type = rule.get_type()
+	clauses = rule.get_clauses()
+	thresholds = rule.get_thresholds()
+	ann_fn = rule.get_annotation_function()
+	ann_fn_label = rule.get_annotation_label()
+	rule_edges = rule.get_edges()
+
+	# We return a list of tuples which specify the target nodes/edges that have made the rule body true
+	applicable_rules = numba.typed.List.empty_list(node_applicable_rule_type)
+
+	# Return empty list if rule is not node rule
+	if rule_type != 'node':
+		return applicable_rules
 
 	# Steps
-	# 1. Gather all qualified nodes/edges, and check if they satisfy the thresholds. If not, break
-	# 2. Gather all annotations associated with the qualified nodes/edges
-	# 3. Assemble all constants for atom trace (this happens inside step 1 for efficiency)
-	# 4. Collect edges and nodes to be added to the graph when rule fires
-
-	# 1.
-	satisfaction = True
-	for i, clause in enumerate(neigh_criteria):
-		# Gather qualified nodes/edges
-		if clause[0]=='node':
-			if clause[1][0]=='target':
-				subset = numba.typed.List([target_node])
-			else:
-				subset = neighbors[target_node] if clause[1][0] not in subsets else subsets[clause[1][0]]
+	# 1. Loop through all nodes and evaluate each clause with that node and check the truth with the thresholds
+	# 2. Inside the clause loop it may be necessary to loop through all nodes/edges while grounding the variables
+	# 3. If the clause is true add the qualified nodes and qualified edges to the atom trace, if on. Break otherwise
+	# 4. After going through all clauses, add to the annotations list all the annotations of the specified subset. These will be passed to the annotation function
+	# 5. Finally, if there are any edges to be added, place them in the list
+
+	for target_node in nodes:
+		if target_node in nodes_to_skip:
+			continue
+		# Initialize dictionary where keys are strings (x1, x2 etc.) and values are lists of qualified neighbors
+		# Keep track of qualified nodes and qualified edges
+		# If it's a node clause update (x1 or x2 etc.) qualified neighbors, if it's an edge clause update the qualified neighbors for the source and target (x1, x2)
+		subsets = numba.typed.Dict.empty(key_type=numba.types.string, value_type=list_of_nodes)
+		qualified_nodes = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
+		qualified_edges = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
+		annotations = numba.typed.List.empty_list(numba.typed.List.empty_list(interval.interval_type))
+		edges_to_be_added = (numba.typed.List.empty_list(node_type), numba.typed.List.empty_list(node_type), rule_edges[-1])
+
+		satisfaction = True
+		for i, clause in enumerate(clauses):
+			# Unpack clause variables
+			clause_type = clause[0]
+			clause_label = clause[1]
+			clause_var_1, clause_var_2 = clause[2][0], clause[2][1]
+			clause_bnd = clause[3]
+
+			# Unpack thresholds
+			# This value is total/available
+			threshold_quantifier_type = thresholds[i][1][1]
+
+			# This is a node clause
+			# The groundings for node clauses are either the target node, neighbors of the target node, or an existing subset of nodes
+			if clause_type == 'node':
+				if clause_var_1 == '__target':
+					subset = numba.typed.List([target_node])
+				else:
+					subset = neighbors[target_node] if clause_var_1 not in subsets else subsets[clause_var_1]
 
-			subsets[clause[1][0]] = get_qualified_components_node_clause(interpretations_node, subset, clause[2], clause[3])
-			if atom_trace:
-				qualified_nodes.append(numba.typed.List(subsets[clause[1][0]]))
-				qualified_edges.append(numba.typed.List.empty_list(edge_type))
+				subsets[clause_var_1] = get_qualified_components_node_clause(interpretations_node, subset, clause_label, clause_bnd)
+				if atom_trace:
+					qualified_nodes.append(numba.typed.List(subsets[clause_var_1]))
+					qualified_edges.append(numba.typed.List.empty_list(edge_type))
 
-		elif clause[0]=='edge':
-			# Set sources for possible edges, if target use target node as source
-			if clause[1][0]=='target':
-				subset_source = numba.typed.List([target_node])
+			# This is an edge clause
+			# There are 5 cases for predicate(Y,Z):
+			# 1. Either one or both of Y, Z are the target node
+			# 2. Both predicate variables Y and Z have not been encountered before
+			# 3. The source variable Y has not been encountered before but the target variable Z has
+			# 4. The target variable Z has not been encountered before but the source variable Y has
+			# 5. Both predicate variables Y and Z have been encountered before
 			else:
-				subset_source = neighbors[target_node] if clause[1][0] not in subsets else subsets[clause[1][0]]
+				# Case 1:
+				# Check if 1st variable or 1st and 2nd variables are the target
+				if clause_var_1 == '__target':
+					subset_source = numba.typed.List([target_node])
+
+					# If both variables are the same
+					if clause_var_2 == '__target':
+						subset_target = numba.typed.List([numba.typed.List([target_node])])
+					elif clause_var_2 in subsets:
+						subset_target = numba.typed.List([subsets[clause_var_2]])
+					else:
+						subset_target = numba.typed.List([neighbors[target_node]])
 
-			subset_target = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
-			if clause[1][1]=='target':
-				# Set targets for possible edges, if target use target node as target
-				for source in subset_source:
-					subset_target.append(numba.typed.List([target_node]))
-			else:
-				for source in subset_source:
-					subset_target.append(neighbors[source] if clause[1][1] not in subsets else subsets[clause[1][1]])
+				# Check if 2nd variable is the target (this means 1st variable isn't the target)
+				elif clause_var_2 == '__target':
+					subset_source = reverse_neighbors[target_node] if clause_var_1 not in subsets else subsets[clause_var_1]
+					subset_target = numba.typed.List([numba.typed.List([target_node]) for _ in subset_source])
+
+				# Case 2:
+				# We replace Y by all nodes and Z by the neighbors of each of these nodes
+				elif clause_var_1 not in subsets and clause_var_2 not in subsets:
+					subset_source = numba.typed.List(nodes)
+					subset_target = numba.typed.List([neighbors[n] for n in subset_source])
+
+				# Case 3:
+				# We replace Y by the sources of Z
+				elif clause_var_1 not in subsets and clause_var_2 in subsets:
+					subset_source = numba.typed.List.empty_list(node_type)
+					subset_target = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
+
+					for n in subsets[clause_var_2]:
+						sources = reverse_neighbors[n]
+						for source in sources:
+							subset_source.append(source)
+							subset_target.append(numba.typed.List([n]))
+
+				# Case 4:
+				# We replace Z by the neighbors of Y
+				elif clause_var_1 in subsets and clause_var_2 not in subsets:
+					subset_source = subsets[clause_var_1]
+					subset_target = numba.typed.List([neighbors[n] for n in subset_source])
 
-			qe = get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause[2], clause[3], reverse_graph)
-			subsets[clause[1][0]] = qe[0]
-			subsets[clause[1][1]] = qe[1]
+				# Case 5:
+				else:
+					subset_source = subsets[clause_var_1]
+					subset_target = numba.typed.List([subsets[clause_var_2] for _ in subset_source])
 
-			if atom_trace:
-				qualified_nodes.append(numba.typed.List.empty_list(node_type))
-				qualified_edges.append(numba.typed.List(zip(subsets[clause[1][0]], subsets[clause[1][1]])))
+				# Get qualified edges
+				qe = get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause_label, clause_bnd, reverse_graph)
+				subsets[clause_var_1] = qe[0]
+				subsets[clause_var_2] = qe[1]
 
-		# Check if the clause satisfies threshold
-		if thresholds[i][1][1]=='total':
-			if clause[0]=='node':
-				neigh_len = len(subset)
-			elif clause[0]=='edge':
-				neigh_len = sum([len(l) for l in subset_target])
-
-		# Available is all neighbors that have a particular label with bound inside [0,1]
-		elif thresholds[i][1][1]=='available':
-			if clause[0]=='node':
-				neigh_len = len(get_qualified_components_node_clause(interpretations_node, subset, clause[2], interval.closed(0,1)))
-			if clause[0]=='edge':
-				neigh_len = len(get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause[2], interval.closed(0,1), reverse_graph)[0])
-
-		qualified_neigh_len = len(subsets[clause[1][0]])
-		satisfaction = _satisfies_threshold(neigh_len, qualified_neigh_len, thresholds[i]) and satisfaction
-		# Exit loop if even one clause is not satisfied
-		if satisfaction==False:
-			break
-
-	# 2.
-	# Add to the subsets that will be used in annotation function
-	if satisfaction:
-		for clause in neigh_criteria:
-			if ann_fn!='':
-				a = numba.typed.List.empty_list(interval.interval_type)
-				if clause[0]=='node':
-					for qn in subsets[clause[1][0]]:
-						a.append(interpretations_node[qn].world[ann_fn_label])
-				elif clause[0]=='edge':
-					for qe in numba.typed.List(zip(subsets[clause[1][0]], subsets[clause[1][1]])):
-						a.append(interpretations_edge[qe].world[ann_fn_label])
-
-				annotations.append(a)
-
-	# 4.
-	# Collect edges to be added
-	if satisfaction:
-		source, target, _ = edges
-
-		# Edges to be added
-		if source!='' and target!='':
-			# Check if edge nodes are target
-			if source=='target':
-				edges_to_be_added[0].append(target_node)
-			elif source in subsets:
-				edges_to_be_added[0].extend(subsets[source])
-			else:
-				edges_to_be_added[0].append(source)
+				if atom_trace:
+					qualified_nodes.append(numba.typed.List.empty_list(node_type))
+					qualified_edges.append(numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])))
 
-			if target=='target':
-				edges_to_be_added[1].append(target_node)			
-			elif target in subsets:
-				edges_to_be_added[1].extend(subsets[target])
-			else:
-				edges_to_be_added[1].append(target)
+			# Check if thresholds are satisfied
+			if threshold_quantifier_type == 'total':
+				if clause_type == 'node':
+					neigh_len = len(subset)
+				else:
+					neigh_len = sum([len(l) for l in subset_target])
 
-	return (satisfaction, annotations, qualified_nodes, qualified_edges, edges_to_be_added)
+			# Available is all neighbors that have a particular label with bound inside [0,1]
+			elif threshold_quantifier_type == 'available':
+				if clause_type == 'node':
+					neigh_len = len(get_qualified_components_node_clause(interpretations_node, subset, clause_label, interval.closed(0,1)))
+				else:
+					neigh_len = len(get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause_label, interval.closed(0,1), reverse_graph)[0])
+
+			qualified_neigh_len = len(subsets[clause_var_1])
+			satisfaction = _satisfies_threshold(neigh_len, qualified_neigh_len, thresholds[i]) and satisfaction
+			# Exit loop if even one clause is not satisfied
+			if not satisfaction:
+				break
+
+		# Here we are done going through each clause of the rule
+		# If all clauses we're satisfied, proceed to collect annotations and prepare edges to be added
+		if satisfaction:
+			# Collect the annotations that might be used in the annotation function according to the correct subset
+			for clause in clauses:
+				clause_type = clause[0]
+				clause_var_1, clause_var_2 = clause[2][0], clause[2][1]
+				if ann_fn != '':
+					a = numba.typed.List.empty_list(interval.interval_type)
+					if clause_type == 'node':
+						for qn in subsets[clause_var_1]:
+							a.append(interpretations_node[qn].world[ann_fn_label])
+					else:
+						for qe in numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])):
+							a.append(interpretations_edge[qe].world[ann_fn_label])
+
+					annotations.append(a)
+
+			# Collect edges to be added
+			source, target, _ = rule_edges
+
+			# Edges to be added
+			if source != '' and target != '':
+				# Check if edge nodes are target
+				if source == '__target':
+					edges_to_be_added[0].append(target_node)
+				elif source in subsets:
+					edges_to_be_added[0].extend(subsets[source])
+				else:
+					edges_to_be_added[0].append(source)
+
+				if target == '__target':
+					edges_to_be_added[1].append(target_node)
+				elif target in subsets:
+					edges_to_be_added[1].extend(subsets[target])
+				else:
+					edges_to_be_added[1].append(target)
+
+			# node/edge, annotations, qualified nodes, qualified edges, edges to be added
+			applicable_rules.append((target_node, annotations, qualified_nodes, qualified_edges, edges_to_be_added))
+
+	return applicable_rules
 
 
 @numba.njit(cache=True)
-def _is_rule_applicable_edge(interpretations_node, interpretations_edge, neighbors, target_edge, neigh_criteria, thresholds, reverse_graph, ann_fn, ann_fn_label, edges, atom_trace):
-	# Initialize dictionary where keys are strings (x1, x2 etc.) and values are lists of qualified neighbors
-	# Keep track of all the edges that are qualified
-	# If it's a node clause update (x1 or x2 etc.) qualified neighbors, if it's an edge clause update the qualified neighbors for the source and target (x1, x2)
-	# First gather all the qualified nodes for each clause
-	subsets = numba.typed.Dict.empty(key_type=numba.types.string, value_type=list_of_nodes)
-	qualified_nodes = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
-	qualified_edges = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
-	annotations = numba.typed.List.empty_list(numba.typed.List.empty_list(interval.interval_type))
-	edges_to_be_added = (numba.typed.List.empty_list(node_type), numba.typed.List.empty_list(node_type), edges[-1])
+def _ground_edge_rule(rule, interpretations_node, interpretations_edge, nodes, edges, neighbors, reverse_neighbors, atom_trace, reverse_graph, edges_to_skip):
+	# Extract rule params
+	rule_type = rule.get_type()
+	clauses = rule.get_clauses()
+	thresholds = rule.get_thresholds()
+	ann_fn = rule.get_annotation_function()
+	ann_fn_label = rule.get_annotation_label()
+	rule_edges = rule.get_edges()
+
+	# We return a list of tuples which specify the target nodes/edges that have made the rule body true
+	applicable_rules = numba.typed.List.empty_list(edge_applicable_rule_type)
+
+	# Return empty list if rule is not node rule
+	if rule_type != 'edge':
+		return applicable_rules
 
 	# Steps
-	# 1. Gather all qualified nodes/edges, and check if they satisfy the thresholds. If not, break
-	# 2. Gather all annotations associated with the qualified nodes/edges
-	# 3. Assemble all constants for atom trace (this happens inside step 1 for efficiency)
-	# 4. Collect edges and nodes to be added to the graph when rule fires
-
-	# 1.
-	satisfaction = True
-	for i, clause in enumerate(neigh_criteria):
-		# Gather qualified nodes/edges
-		# For nodes gather source neighbors only, not target neighbors
-		if clause[0]=='node':
-			if clause[1][0]=='source':
-				subset = numba.typed.List([target_edge[0]])
-			elif clause[1][0]=='target':
-				subset = numba.typed.List([target_edge[1]])
-			else:
-				subset = neighbors[target_edge[0]] if clause[1][0] not in subsets else subsets[clause[1][0]]
+	# 1. Loop through all nodes and evaluate each clause with that node and check the truth with the thresholds
+	# 2. Inside the clause loop it may be necessary to loop through all nodes/edges while grounding the variables
+	# 3. If the clause is true add the qualified nodes and qualified edges to the atom trace, if on. Break otherwise
+	# 4. After going through all clauses, add to the annotations list all the annotations of the specified subset. These will be passed to the annotation function
+	# 5. Finally, if there are any edges to be added, place them in the list
+
+	for target_edge in edges:
+		if target_edge in edges_to_skip:
+			continue
+		# Initialize dictionary where keys are strings (x1, x2 etc.) and values are lists of qualified neighbors
+		# Keep track of qualified nodes and qualified edges
+		# If it's a node clause update (x1 or x2 etc.) qualified neighbors, if it's an edge clause update the qualified neighbors for the source and target (x1, x2)
+		subsets = numba.typed.Dict.empty(key_type=numba.types.string, value_type=list_of_nodes)
+		qualified_nodes = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
+		qualified_edges = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
+		annotations = numba.typed.List.empty_list(numba.typed.List.empty_list(interval.interval_type))
+		edges_to_be_added = (numba.typed.List.empty_list(node_type), numba.typed.List.empty_list(node_type), rule_edges[-1])
+
+		satisfaction = True
+		for i, clause in enumerate(clauses):
+			# Unpack clause variables
+			clause_type = clause[0]
+			clause_label = clause[1]
+			clause_var_1, clause_var_2 = clause[2][0], clause[2][1]
+			clause_bnd = clause[3]
+
+			# Unpack thresholds
+			# This value is total/available
+			threshold_quantifier_type = thresholds[i][1][1]
+
+			# This is a node clause
+			# The groundings for node clauses are either the source, target, neighbors of the source node, or an existing subset of nodes
+			if clause_type == 'node':
+				if clause_var_1 == '__source':
+					subset = numba.typed.List([target_edge[0]])
+				elif clause_var_1 == '__target':
+					subset = numba.typed.List([target_edge[1]])
+				else:
+					subset = neighbors[target_edge[0]] if clause_var_1 not in subsets else subsets[clause_var_1]
 
-			subsets[clause[1][0]] = get_qualified_components_node_clause(interpretations_node, subset, clause[2], clause[3])
-			if atom_trace:
-				qualified_nodes.append(numba.typed.List(subsets[clause[1][0]]))
-				qualified_edges.append(numba.typed.List.empty_list(edge_type))
+				subsets[clause_var_1] = get_qualified_components_node_clause(interpretations_node, subset, clause_label, clause_bnd)
+				if atom_trace:
+					qualified_nodes.append(numba.typed.List(subsets[clause_var_1]))
+					qualified_edges.append(numba.typed.List.empty_list(edge_type))
 
-		elif clause[0]=='edge':
-			# Set sources for possible edges, if target use target node as source
-			# By default we take the subset_source to be the neighbors of the source node.
-			if clause[1][0]=='source':
-				subset_source = numba.typed.List([target_edge[0]])
-			elif clause[1][0]=='target':
-				subset_source = numba.typed.List([target_edge[1]])
+			# This is an edge clause
+			# There are 5 cases for predicate(Y,Z):
+			# 1. Either one or both of Y, Z are the source or target node
+			# 2. Both predicate variables Y and Z have not been encountered before
+			# 3. The source variable Y has not been encountered before but the target variable Z has
+			# 4. The target variable Z has not been encountered before but the source variable Y has
+			# 5. Both predicate variables Y and Z have been encountered before
 			else:
-				subset_source = neighbors[target_edge[0]] if clause[1][0] not in subsets else subsets[clause[1][0]]
-				
-			subset_target = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
-			if clause[1][1]=='source':
-				# Set targets for possible edges, if source use source node as target
-				for source in subset_source:
-					subset_target.append(numba.typed.List([target_edge[0]]))
-			elif clause[1][1]=='target':
-				# Set targets for possible edges, if target use target node as target
-				for source in subset_source:
-					subset_target.append(numba.typed.List([target_edge[1]]))
-			else:
-				for source in subset_source:
-					subset_target.append(neighbors[source] if clause[1][1] not in subsets else subsets[clause[1][1]])
+				# Case 1:
+				# Check if 1st variable is the source
+				if clause_var_1 == '__source':
+					subset_source = numba.typed.List([target_edge[0]])
+
+					# If 2nd variable is source/target/something else
+					if clause_var_2 == '__source':
+						subset_target = numba.typed.List([numba.typed.List([target_edge[0]])])
+					elif clause_var_2 == '__target':
+						subset_target = numba.typed.List([numba.typed.List([target_edge[1]])])
+					elif clause_var_2 in subsets:
+						subset_target = numba.typed.List([subsets[clause_var_2]])
+					else:
+						subset_target = numba.typed.List([neighbors[target_edge[0]]])
 
-			qe = get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause[2], clause[3], reverse_graph)
-			subsets[clause[1][0]] = qe[0]
-			subsets[clause[1][1]] = qe[1]
+				# if 1st variable is the target
+				elif clause_var_1 == '__target':
+					subset_source = numba.typed.List([target_edge[1]])
+
+					# if 2nd variable is source/target/something else
+					if clause_var_2 == '__source':
+						subset_target = numba.typed.List([numba.typed.List([target_edge[0]])])
+					elif clause_var_2 == '__target':
+						subset_target = numba.typed.List([numba.typed.List([target_edge[1]])])
+					elif clause_var_2 in subsets:
+						subset_target = numba.typed.List([subsets[clause_var_2]])
+					else:
+						subset_target = numba.typed.List([neighbors[target_edge[1]]])
 
-			if atom_trace:
-				qualified_nodes.append(numba.typed.List.empty_list(node_type))
-				qualified_edges.append(numba.typed.List(zip(subsets[clause[1][0]], subsets[clause[1][1]])))
+				# Handle the cases where the 2nd variable is source/target but the 1st is something else (cannot be source/target)
+				elif clause_var_2 == '__source':
+					subset_source = reverse_neighbors[target_edge[0]] if clause_var_1 not in subsets else subsets[clause_var_1]
+					subset_target = numba.typed.List([numba.typed.List([target_edge[0]]) for _ in subset_source])
+
+				elif clause_var_2 == '__target':
+					subset_source = reverse_neighbors[target_edge[1]] if clause_var_1 not in subsets else subsets[clause_var_1]
+					subset_target = numba.typed.List([numba.typed.List([target_edge[1]]) for _ in subset_source])
+
+				# Case 2:
+				# We replace Y by all nodes and Z by the neighbors of each of these nodes
+				elif clause_var_1 not in subsets and clause_var_2 not in subsets:
+					subset_source = numba.typed.List(nodes)
+					subset_target = numba.typed.List([neighbors[n] for n in subset_source])
+
+				# Case 3:
+				# We replace Y by the sources of Z
+				elif clause_var_1 not in subsets and clause_var_2 in subsets:
+					subset_source = numba.typed.List.empty_list(node_type)
+					subset_target = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
+
+					for n in subsets[clause_var_2]:
+						sources = reverse_neighbors[n]
+						for source in sources:
+							subset_source.append(source)
+							subset_target.append(numba.typed.List([n]))
+
+				# Case 4:
+				# We replace Z by the neighbors of Y
+				elif clause_var_1 in subsets and clause_var_2 not in subsets:
+					subset_source = subsets[clause_var_1]
+					subset_target = numba.typed.List([neighbors[n] for n in subset_source])
 
-		# Check if the clause satisfies threshold
-		if thresholds[i][1][1]=='total':
-			if clause[0]=='node':
-				neigh_len = len(subset)
-			elif clause[0]=='edge':
-				neigh_len = sum([len(l) for l in subset_target])
-
-		# Available is all neighbors that have a particular label with bound inside [0,1]
-		elif thresholds[i][1][1]=='available':
-			if clause[0]=='node':
-				neigh_len = len(get_qualified_components_node_clause(interpretations_node, subset, clause[2], interval.closed(0,1)))
-			if clause[0]=='edge':
-				neigh_len = len(get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause[2], interval.closed(0,1), reverse_graph)[0])
-
-		qualified_neigh_len = len(subsets[clause[1][0]])
-		satisfaction = _satisfies_threshold(neigh_len, qualified_neigh_len, thresholds[i]) and satisfaction
-		# Exit loop if even one clause is not satisfied
-		if satisfaction==False:
-			break
-
-	# 2.
-	# Add to the subsets that will be used in annotation function
-	if satisfaction:
-		for clause in neigh_criteria:
-			if ann_fn!='':
-				a = numba.typed.List.empty_list(interval.interval_type)
-				if clause[0]=='node':
-					for qn in subsets[clause[1][0]]:
-						a.append(interpretations_node[qn].world[ann_fn_label])
-				elif clause[0]=='edge':
-					for qe in numba.typed.List(zip(subsets[clause[1][0]], subsets[clause[1][1]])):
-						a.append(interpretations_edge[qe].world[ann_fn_label])
-
-				annotations.append(a)
-
-	# 4.
-	# Collect edges to be added
-	if satisfaction:
-		source, target, _ = edges
-
-		# Edges to be added
-		if source!='' and target!='':
-			# Check if edge nodes are source or target
-			if source=='source':
-				edges_to_be_added[0].append(target_edge[0])
-			elif source=='target':
-				edges_to_be_added[0].append(target_edge[1])
-			elif source in subsets:
-				edges_to_be_added[0].extend(subsets[source])
-			else:
-				edges_to_be_added[0].append(source)
+				# Case 5:
+				else:
+					subset_source = subsets[clause_var_1]
+					subset_target = numba.typed.List([subsets[clause_var_2] for _ in subset_source])
 
-			if target=='source':
-				edges_to_be_added[1].append(target_edge[0])
-			elif target=='target':
-				edges_to_be_added[1].append(target_edge[1])			
-			elif target in subsets:
-				edges_to_be_added[1].extend(subsets[target])
-			else:
-				edges_to_be_added[1].append(target)
+				# Get qualified edges
+				qe = get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause_label, clause_bnd, reverse_graph)
+				subsets[clause_var_1] = qe[0]
+				subsets[clause_var_2] = qe[1]
+
+				if atom_trace:
+					qualified_nodes.append(numba.typed.List.empty_list(node_type))
+					qualified_edges.append(numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])))
+
+			# Check if thresholds are satisfied
+			if threshold_quantifier_type == 'total':
+				if clause_type == 'node':
+					neigh_len = len(subset)
+				else:
+					neigh_len = sum([len(l) for l in subset_target])
+
+			# Available is all neighbors that have a particular label with bound inside [0,1]
+			elif threshold_quantifier_type == 'available':
+				if clause_type == 'node':
+					neigh_len = len(get_qualified_components_node_clause(interpretations_node, subset, clause_label, interval.closed(0, 1)))
+				else:
+					neigh_len = len(get_qualified_components_edge_clause(interpretations_edge, subset_source, subset_target, clause_label, interval.closed(0, 1), reverse_graph)[0])
+
+			qualified_neigh_len = len(subsets[clause_var_1])
+			satisfaction = _satisfies_threshold(neigh_len, qualified_neigh_len, thresholds[i]) and satisfaction
+			# Exit loop if even one clause is not satisfied
+			if not satisfaction:
+				break
+
+		# Here we are done going through each clause of the rule
+		# If all clauses we're satisfied, proceed to collect annotations and prepare edges to be added
+		if satisfaction:
+			# Collect the annotations that might be used in the annotation function according to the correct subset
+			for clause in clauses:
+				clause_type = clause[0]
+				clause_var_1, clause_var_2 = clause[2][0], clause[2][1]
+				if ann_fn != '':
+					a = numba.typed.List.empty_list(interval.interval_type)
+					if clause_type == 'node':
+						for qn in subsets[clause_var_1]:
+							a.append(interpretations_node[qn].world[ann_fn_label])
+					else:
+						for qe in numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])):
+							a.append(interpretations_edge[qe].world[ann_fn_label])
+
+					annotations.append(a)
+
+			# Collect edges to be added
+			source, target, _ = rule_edges
 
-	return (satisfaction, annotations, qualified_nodes, qualified_edges, edges_to_be_added)
+			# Edges to be added
+			if source != '' and target != '':
+				# Check if edge nodes are source/target
+				if source == '__source':
+					edges_to_be_added[0].append(target_edge[0])
+				elif source == '__target':
+					edges_to_be_added[0].append(target_edge[1])
+				elif source in subsets:
+					edges_to_be_added[0].extend(subsets[source])
+				else:
+					edges_to_be_added[0].append(source)
+
+				if target == '__source':
+					edges_to_be_added[1].append(target_edge[0])
+				elif target == '__target':
+					edges_to_be_added[1].append(target_edge[1])
+				elif target in subsets:
+					edges_to_be_added[1].extend(subsets[target])
+				else:
+					edges_to_be_added[1].append(target)
+
+			# node/edge, annotations, qualified nodes, qualified edges, edges to be added
+			applicable_rules.append((target_edge, annotations, qualified_nodes, qualified_edges, edges_to_be_added))
+
+	return applicable_rules
 
 
 @numba.njit(cache=True)
 def get_qualified_components_node_clause(interpretations_node, candidates, l, bnd):
 	# Get all the qualified neighbors for a particular clause
 	qualified_nodes = numba.typed.List.empty_list(node_type)
 	for n in candidates:
@@ -947,14 +1124,18 @@
 	updated = False
 	# This is to prevent a key error in case the label is a specific label
 	try:
 		world = interpretations[comp]
 		l, bnd = na
 		updated_bnds = numba.typed.List.empty_list(interval.interval_type)
 
+		# Add label to world if it is not there
+		if l not in world.world:
+			world.world[l] = interval.closed(0, 1)
+
 		# Check if update is necessary with previous bnd
 		prev_bnd = world.world[l].copy()
 
 		# override will not check for inconsistencies
 		if override:
 			world.world[l].set_lower_upper(bnd.lower, bnd.upper)
 		else:
@@ -1000,15 +1181,15 @@
 					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
 					world.world[p1].set_lower_upper(lower, upper)
 					world.world[p1].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p1])
 					if store_interpretation_changes:
 						rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
-		
+
 		# Gather convergence data
 		change = 0
 		if updated:
 			# Find out if it has changed from previous interp
 			current_bnd = world.world[l]
 			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
 			if current_bnd != prev_t_bnd:
@@ -1032,14 +1213,18 @@
 	updated = False
 	# This is to prevent a key error in case the label is a specific label
 	try:
 		world = interpretations[comp]
 		l, bnd = na
 		updated_bnds = numba.typed.List.empty_list(interval.interval_type)
 
+		# Add label to world if it is not there
+		if l not in world.world:
+			world.world[l] = interval.closed(0, 1)
+
 		# Check if update is necessary with previous bnd
 		prev_bnd = world.world[l].copy()
 
 		# override will not check for inconsistencies
 		if override:
 			world.world[l].set_lower_upper(bnd.lower, bnd.upper)
 		else:
@@ -1164,37 +1349,43 @@
 
 @numba.njit(cache=True)
 def influence(rule, annotations, weights):
 	func_name = rule.get_annotation_function()
 	if func_name=='':
 		return interval.closed(rule.get_bnd().lower, rule.get_bnd().upper)
 	elif func_name=='average':
-		return ann_fn.average(annotations, weights)
+		return ann_fns.average(annotations, weights)
 	elif func_name=='average_lower':
-		return ann_fn.average_lower(annotations, weights)
+		return ann_fns.average_lower(annotations, weights)
 	elif func_name=='minimum':
-		return ann_fn.minimum(annotations, weights)
+		return ann_fns.minimum(annotations, weights)
 	elif func_name=='maximum':
-		return ann_fn.maximum(annotations, weights)
+		return ann_fns.maximum(annotations, weights)
 
 
 @numba.njit(cache=True)
 def check_consistent_node(interpretations, comp, na):
 	world = interpretations[comp]
-	bnd = world.world[na[0]]
+	if na[0] in world.world:
+		bnd = world.world[na[0]]
+	else:
+		bnd = interval.closed(0, 1)
 	if (na[1].lower > bnd.upper) or (bnd.lower > na[1].upper):
 		return False
 	else:
 		return True
 
 
 @numba.njit(cache=True)
 def check_consistent_edge(interpretations, comp, na):
 	world = interpretations[comp]
-	bnd = world.world[na[0]]
+	if na[0] in world.world:
+		bnd = world.world[na[0]]
+	else:
+		bnd = interval.closed(0, 1)
 	if (na[1].lower > bnd.upper) or (bnd.lower > na[1].upper):
 		return False
 	else:
 		return True
 
 
 @numba.njit(cache=True)
@@ -1224,36 +1415,36 @@
 			if store_interpretation_changes:
 				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 	# Add inconsistent predicates to a list 
 
 
 @numba.njit(cache=True)
 def resolve_inconsistency_edge(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms, store_interpretation_changes):
-	world = interpretations[comp]
+	w = interpretations[comp]
 	if store_interpretation_changes:
 		rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
 		if atom_trace:
-			_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[na[0]], 'Inconsistency')
+			_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), w.world[na[0]], 'Inconsistency')
 	# Resolve inconsistency and set static
-	world.world[na[0]].set_lower_upper(0, 1)
-	world.world[na[0]].set_static(True)
+	w.world[na[0]].set_lower_upper(0, 1)
+	w.world[na[0]].set_static(True)
 	for p1, p2 in ipl:
 		if p1==na[0]:
 			if atom_trace:
-				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], 'Inconsistency')
-			world.world[p2].set_lower_upper(0, 1)
-			world.world[p2].set_static(True)
+				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), w.world[p2], 'Inconsistency')
+			w.world[p2].set_lower_upper(0, 1)
+			w.world[p2].set_static(True)
 			if store_interpretation_changes:
 				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(0,1)))
 
 		if p2==na[0]:
 			if atom_trace:
-				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], 'Inconsistency')
-			world.world[p1].set_lower_upper(0, 1)
-			world.world[p1].set_static(True)
+				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), w.world[p1], 'Inconsistency')
+			w.world[p1].set_lower_upper(0, 1)
+			w.world[p1].set_static(True)
 			if store_interpretation_changes:
 				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 
 
 @numba.njit(cache=True)
 def _add_node(node, neighbors, nodes, interpretations_node):
 	nodes.append(node)
@@ -1266,15 +1457,15 @@
 	# If not a node, add to list of nodes and initialize neighbors
 	if source not in nodes:
 		_add_node(source, neighbors, nodes, interpretations_node)
 
 	if target not in nodes:
 		_add_node(target, neighbors, nodes, interpretations_node)
 
-	# Make sure edge doesnt already exist
+	# Make sure edge doesn't already exist
 	# Make sure, if l=='', not to add the label
 	# Make sure, if edge exists, that we don't override the l label if it exists
 	edge = (source, target)
 	new_edge = False
 	if edge not in edges:
 		new_edge = True
 		edges.append(edge)
@@ -1282,15 +1473,15 @@
 		if l.value!='':
 			interpretations_edge[edge] = world.World(numba.typed.List([l]))
 		else:
 			interpretations_edge[edge] = world.World(numba.typed.List.empty_list(label.label_type))
 	else:
 		if l not in interpretations_edge[edge].world and l.value!='':
 			new_edge = True
-			interpretations_edge[edge].world[l] = interval.closed(0,1)
+			interpretations_edge[edge].world[l] = interval.closed(0, 1)
 
 	return (edge, new_edge)
 
 
 @numba.njit(cache=True)
 def _add_edges(sources, targets, neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
 	changes = 0
```

### Comparing `pyreason-1.6.1/pyreason/scripts/interval/interval.py` & `pyreason-1.8.1/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,121 +19,121 @@
     def __init__(self):
         super(RuleType, self).__init__(name='Rule')
 
 
 rule_type = RuleType()
 
 
-# Type ann_fnerence
+# Type ann_fn
 @typeof_impl.register(Rule)
 def typeof_rule(val, c):
     return rule_type
 
 
 # Construct object from Numba functions (Doesn't work. We don't need this currently)
 @type_callable(Rule)
 def type_rule(context):
-    def typer(name, target, tc, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule):
-        if isinstance(name, types.UnicodeType) and isinstance(target, label.LabelType) and isinstance(tc, (types.NoneType, types.ListType)) and isinstance(delta, types.Integer) and isinstance(neigh_criteria, (types.NoneType, types.ListType)) and isinstance(bnd, interval.IntervalType) and isinstance(thresholds, types.ListType) and isinstance(ann_fn, types.UnicodeType) and isinstance(ann_label, label.LabelType) and isinstance(weights, types.Array) and isinstance(edges, types.Tuple) and isinstance(immediate_rule, types.Boolean):
+    def typer(rule_str, type, target, delta, clauses, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule):
+        if isinstance(rule_str, types.UnicodeType) and isinstance(type, types.UnicodeType) and isinstance(target, label.LabelType) and isinstance(delta, types.Integer) and isinstance(clauses, (types.NoneType, types.ListType)) and isinstance(bnd, interval.IntervalType) and isinstance(thresholds, types.ListType) and isinstance(ann_fn, types.UnicodeType) and isinstance(ann_label, label.LabelType) and isinstance(weights, types.Array) and isinstance(edges, types.Tuple) and isinstance(immediate_rule, types.Boolean):
             return rule_type
     return typer
 
 
-# Define native representation: datamodel
+# Define native representation: data-model
 @register_model(RuleType)
 class RuleModel(models.StructModel):
     def __init__(self, dmm, fe_type):
         members = [
-            ('name', types.string),
+            ('rule_str', types.string),
+            ('type', types.string),
             ('target', label.label_type),
-            ('target_criteria', types.ListType(types.Tuple((label.label_type, interval.interval_type)))),
             ('delta', types.uint16),
-            ('neigh_criteria', types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type)))),
+            ('clauses', types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type)))),
             ('bnd', interval.interval_type),
             ('thresholds', types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64)))),
             ('ann_fn', types.string),
             ('ann_label', label.label_type),
             ('weights', types.float64[::1]),
             ('edges', types.Tuple((types.string, types.string, label.label_type))),
             ('immediate_rule', types.boolean)
             ]
         models.StructModel.__init__(self, dmm, fe_type, members)
 
 
-# Expose datamodel attributes
-make_attribute_wrapper(RuleType, 'name', 'name')
+# Expose data-model attributes
+make_attribute_wrapper(RuleType, 'rule_str', 'rule_str')
+make_attribute_wrapper(RuleType, 'type', 'type')
 make_attribute_wrapper(RuleType, 'target', 'target')
-make_attribute_wrapper(RuleType, 'target_criteria', 'target_criteria')
 make_attribute_wrapper(RuleType, 'delta', 'delta')
-make_attribute_wrapper(RuleType, 'neigh_criteria', 'neigh_criteria')
+make_attribute_wrapper(RuleType, 'clauses', 'clauses')
 make_attribute_wrapper(RuleType, 'bnd', 'bnd')
 make_attribute_wrapper(RuleType, 'thresholds', 'thresholds')
 make_attribute_wrapper(RuleType, 'ann_fn', 'ann_fn')
 make_attribute_wrapper(RuleType, 'ann_label', 'ann_label')
 make_attribute_wrapper(RuleType, 'weights', 'weights')
 make_attribute_wrapper(RuleType, 'edges', 'edges')
 make_attribute_wrapper(RuleType, 'immediate_rule', 'immediate_rule')
 
 
 # Implement constructor
-@lower_builtin(Rule, types.string, label.label_type, types.ListType(types.Tuple((label.label_type, interval.interval_type))), types.uint16, types.ListType(types.Tuple((types.string, label.label_type, interval.interval_type))), interval.interval_type, types.ListType(types.ListType(types.Tuple((types.string, types.string, types.float64)))), types.string, label.label_type, types.float64[::1], types.Tuple((types.string, types.string, label.label_type)), types.boolean)
+@lower_builtin(Rule, types.string, types.string, label.label_type, types.uint16, types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), interval.interval_type, types.ListType(types.ListType(types.Tuple((types.string, types.string, types.float64)))), types.string, label.label_type, types.float64[::1], types.Tuple((types.string, types.string, label.label_type)), types.boolean)
 def impl_rule(context, builder, sig, args):
     typ = sig.return_type
-    name, target, target_criteria, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule = args
-    context.nrt.incref(builder, types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), neigh_criteria)
+    rule_str, type, target, delta, clauses, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule = args
+    context.nrt.incref(builder, types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), clauses)
     context.nrt.incref(builder, types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), thresholds)
     rule = cgutils.create_struct_proxy(typ)(context, builder)
-    rule.name = name
+    rule.rule_str = rule_str
+    rule.type = type
     rule.target = target
-    rule.target_criteria = target_criteria
     rule.delta = delta
-    rule.neigh_criteria = neigh_criteria
+    rule.clauses = clauses
     rule.bnd = bnd
     rule.thresholds = thresholds
     rule.ann_fn = ann_fn
     rule.ann_label = ann_label
     rule.weights = weights
     rule.edges = edges
     rule.immediate_rule = immediate_rule
     return rule._getvalue()
 
 
 # Expose properties
 @overload_method(RuleType, "get_name")
 def get_name(rule):
     def getter(rule):
-        return rule.name
+        return rule.rule_str
     return getter
 
 
-@overload_method(RuleType, "get_target")
-def get_target(rule):
+@overload_method(RuleType, "get_type")
+def get_type(rule):
     def getter(rule):
-        return rule.target
+        return rule.type
     return getter
 
 
-@overload_method(RuleType, "get_target_criteria")
-def get_target_criteria(rule):
+@overload_method(RuleType, "get_target")
+def get_target(rule):
     def getter(rule):
-        return rule.target_criteria
+        return rule.target
     return getter
 
 
 @overload_method(RuleType, "get_delta")
 def get_delta(rule):
     def getter(rule):
         return rule.delta
     return getter
 
 
-@overload_method(RuleType, "get_neigh_criteria")
-def get_neigh_criteria(rule):
+@overload_method(RuleType, "get_clauses")
+def get_clauses(rule):
     def getter(rule):
-        return rule.neigh_criteria
+        return rule.clauses
     return getter
 
 
 @overload_method(RuleType, "get_bnd")
 def get_bnd(rule):
     def impl(rule):
         return rule.bnd
@@ -181,44 +181,44 @@
         return rule.immediate_rule
     return impl
 
 
 # Tell numba how to make native
 @unbox(RuleType)
 def unbox_rule(typ, obj, c):
-    name_obj = c.pyapi.object_getattr_string(obj, "_name")
+    name_obj = c.pyapi.object_getattr_string(obj, "_rule_str")
+    type_obj = c.pyapi.object_getattr_string(obj, "_type")
     target_obj = c.pyapi.object_getattr_string(obj, "_target")
-    tc_obj = c.pyapi.object_getattr_string(obj, "_target_criteria")
     delta_obj = c.pyapi.object_getattr_string(obj, "_delta")
-    neigh_criteria_obj = c.pyapi.object_getattr_string(obj, "_neigh_criteria")
+    clauses_obj = c.pyapi.object_getattr_string(obj, "_clauses")
     bnd_obj = c.pyapi.object_getattr_string(obj, "_bnd")
     thresholds_obj = c.pyapi.object_getattr_string(obj, "_thresholds")
     ann_fn_obj = c.pyapi.object_getattr_string(obj, "_ann_fn")
     ann_label_obj = c.pyapi.object_getattr_string(obj, "_ann_label")
     weights_obj = c.pyapi.object_getattr_string(obj, "_weights")
     edges_obj = c.pyapi.object_getattr_string(obj, "_edges")
     immediate_rule_obj = c.pyapi.object_getattr_string(obj, "_immediate_rule")
     rule = cgutils.create_struct_proxy(typ)(c.context, c.builder)
-    rule.name = c.unbox(types.string, name_obj).value
+    rule.rule_str = c.unbox(types.string, name_obj).value
+    rule.type = c.unbox(types.string, type_obj).value
     rule.target = c.unbox(label.label_type, target_obj).value
-    rule.target_criteria = c.unbox(types.ListType(types.Tuple((label.label_type, interval.interval_type))), tc_obj).value
     rule.delta = c.unbox(types.uint16, delta_obj).value
-    rule.neigh_criteria = c.unbox(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), neigh_criteria_obj).value
+    rule.clauses = c.unbox(types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), clauses_obj).value
     rule.bnd = c.unbox(interval.interval_type, bnd_obj).value
     rule.thresholds = c.unbox(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), thresholds_obj).value
     rule.ann_fn = c.unbox(types.string, ann_fn_obj).value
     rule.ann_label = c.unbox(label.label_type, ann_label_obj).value
     rule.weights = c.unbox(types.float64[::1], weights_obj).value
     rule.edges = c.unbox(types.Tuple((types.string, types.string, label.label_type)), edges_obj).value
     rule.immediate_rule = c.unbox(types.boolean, immediate_rule_obj).value
     c.pyapi.decref(name_obj)
+    c.pyapi.decref(type_obj)
     c.pyapi.decref(target_obj)
-    c.pyapi.decref(tc_obj)
     c.pyapi.decref(delta_obj)
-    c.pyapi.decref(neigh_criteria_obj)
+    c.pyapi.decref(clauses_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(thresholds_obj)
     c.pyapi.decref(ann_fn_obj)
     c.pyapi.decref(ann_label_obj)
     c.pyapi.decref(weights_obj)
     c.pyapi.decref(edges_obj)
     c.pyapi.decref(immediate_rule_obj)
@@ -226,32 +226,32 @@
     return NativeValue(rule._getvalue(), is_error=is_error)
 
 
 @box(RuleType)
 def box_rule(typ, val, c):
     rule = cgutils.create_struct_proxy(typ)(c.context, c.builder, value=val)
     class_obj = c.pyapi.unserialize(c.pyapi.serialize_object(Rule))
-    name_obj = c.box(types.string, rule.name)
+    name_obj = c.box(types.string, rule.rule_str)
+    type_obj = c.box(types.string, rule.type)
     target_obj = c.box(label.label_type, rule.target)
-    tc_obj = c.box(types.ListType(types.Tuple((label.label_type, interval.interval_type))), rule.target_criteria)
     delta_obj = c.box(types.uint16, rule.delta)
-    neigh_criteria_obj = c.box(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), rule.neigh_criteria)
+    clauses_obj = c.box(types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), rule.clauses)
     bnd_obj = c.box(interval.interval_type, rule.bnd)
     thresholds_obj = c.box(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), rule.thresholds)
     ann_fn_obj = c.box(types.string, rule.ann_fn)
     ann_label_obj = c.box(label.label_type, rule.ann_label)
     weights_obj = c.box(types.float64[::1], rule.weights)
     edges_obj = c.box(types.Tuple((types.string, types.string, label.label_type)), rule.edges)
     immediate_rule_obj = c.box(types.boolean, rule.immediate_rule)
-    res = c.pyapi.call_function_objargs(class_obj, (name_obj, target_obj, tc_obj, delta_obj, neigh_criteria_obj, bnd_obj, thresholds_obj, ann_fn_obj, ann_label_obj, weights_obj, edges_obj, immediate_rule_obj))
+    res = c.pyapi.call_function_objargs(class_obj, (name_obj, type_obj, target_obj, delta_obj, clauses_obj, bnd_obj, thresholds_obj, ann_fn_obj, ann_label_obj, weights_obj, edges_obj, immediate_rule_obj))
     c.pyapi.decref(name_obj)
+    c.pyapi.decref(type_obj)
     c.pyapi.decref(target_obj)
-    c.pyapi.decref(tc_obj)
     c.pyapi.decref(delta_obj)
-    c.pyapi.decref(neigh_criteria_obj)
+    c.pyapi.decref(clauses_obj)
     c.pyapi.decref(ann_fn_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(thresholds_obj)
     c.pyapi.decref(ann_label_obj)
     c.pyapi.decref(weights_obj)
     c.pyapi.decref(edges_obj)
     c.pyapi.decref(immediate_rule_obj)
```

### Comparing `pyreason-1.6.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.8.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/program/program.py` & `pyreason-1.8.1/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/rules/rule.py` & `pyreason-1.8.1/pyreason/scripts/rules/rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 class Rule:
 
-    def __init__(self, name, target, target_criteria, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule):
-        self._name = name
+    def __init__(self, rule_str, rule_type, target, delta, clauses, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule):
+        self._rule_str = rule_str
+        self._type = rule_type
         self._target = target
-        self._target_criteria = target_criteria
         self._delta = delta
-        self._neigh_criteria = neigh_criteria
+        self._clauses = clauses
         self._bnd = bnd
         self._thresholds = thresholds
         self._ann_fn = ann_fn
         self._ann_label = ann_label
         self._weights = weights
         self._edges = edges
         self._immediate_rule = immediate_rule
 
-    def get_name(self):
-        return self._name
-    
+    def get_rule_str(self):
+        return self._rule_str
+
+    def get_rule_type(self):
+        return self._type
+
     def get_target(self):
         return self._target
 
-    def get_target_criteria(self):
-        return self._target_criteria
-
     def get_delta(self):
         return self._delta
 
     def get_neigh_criteria(self):
-        return self._neigh_criteria
+        return self._clauses
     
     def get_bnd(self):
         return self._bnd
 
     def get_thresholds(self):
         return self._thresholds
```

### Comparing `pyreason-1.6.1/pyreason/scripts/utils/filter.py` & `pyreason-1.8.1/pyreason/scripts/utils/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,13 +103,15 @@
                     edges[t][comp][l.get_value()] = [bnd.lower, bnd.upper]
 
         dataframes = []
         for t in range(self.tmax+1):
             dataframe = pd.DataFrame.from_dict(edges[t]).transpose()
             dataframe = dataframe.reset_index()
             if not dataframe.empty:
-                dataframe.columns = ['component', *labels]
+                dataframe.columns = ['source', 'target', *labels]
+                dataframe['component'] = dataframe[['source', 'target']].apply(tuple, axis=1)
+                dataframe.drop(columns=['source', 'target'], inplace=True)
+                dataframe = dataframe[['component', *labels]]
             else:
                 dataframe = pd.DataFrame(columns=['component', *labels])
             dataframes.append(dataframe)
         return dataframes
-
```

### Comparing `pyreason-1.6.1/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.8.1/pyreason/scripts/utils/graphml_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,87 +7,80 @@
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 
 
 class GraphmlParser:
     def __init__(self):
         self.graph = None
         self.non_fluent_facts = None
-
+        
     def parse_graph(self, graph_path, reverse):
         self.graph = nx.read_graphml(graph_path)
         if reverse:
             self.graph = self.graph.reverse()
 
         return self.graph
 
     def parse_graph_attributes(self, static_facts):
         facts_node = numba.typed.List.empty_list(fact_node.fact_type)
         facts_edge = numba.typed.List.empty_list(fact_edge.fact_type)
-        specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type,
-                                                      value_type=numba.types.ListType(numba.types.string))
-        specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(
-            numba.types.Tuple((numba.types.string, numba.types.string))))
+        specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.string))
+        specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.Tuple((numba.types.string, numba.types.string))))
         for n in self.graph.nodes:
             for key, value in self.graph.nodes[n].items():
                 # IF attribute is a float or int and it is less than 1, then make it a bound, else make it a label
-                if (isinstance(value, (float, int)) and 1 >= value >= 0) or (
-                        isinstance(value, str) and value.replace('.', '').isdigit() and 1 >= float(value) >= 0):
+                if isinstance(value, (float, int)) and value<=1 and value>=0:
                     l = str(key)
                     l_bnd = float(value)
                     u_bnd = 1
                 else:
                     l = f'{key}-{value}'
                     l_bnd = 1
                     u_bnd = 1
                 if isinstance(value, str):
                     bnd_str = value.split(',')
-                    if len(bnd_str) == 2:
+                    if len(bnd_str)==2:
                         try:
                             low = int(bnd_str[0])
                             up = int(bnd_str[1])
-                            if 1 >= low >= 0 and 1 >= up >= 0:
+                            if low<=1 and low>=0 and up<=1 and up>=0:
                                 l_bnd = low
                                 u_bnd = up
                                 l = str(key)
                         except:
                             pass
-
+                
                 if label.Label(l) not in specific_node_labels.keys():
                     specific_node_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.string)
                 specific_node_labels[label.Label(l)].append(n)
-                f = fact_node.Fact('graph-attribute-fact', n, label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0,
-                                   static=static_facts)
+                f = fact_node.Fact('graph-attribute-fact', n, label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
                 facts_node.append(f)
         for e in self.graph.edges:
             for key, value in self.graph.edges[e].items():
                 # IF attribute is a float or int and it is less than 1, then make it a bound, else make it a label
-                if (isinstance(value, (float, int)) and 1 >= value >= 0) or (
-                        isinstance(value, str) and value.replace('.', '').isdigit() and 1 >= float(value) >= 0):
+                if isinstance(value, (float, int)) and value<=1 and value>=0:
                     l = str(key)
                     l_bnd = float(value)
                     u_bnd = 1
                 else:
                     l = f'{key}-{value}'
                     l_bnd = 1
                     u_bnd = 1
                 if isinstance(value, str):
                     bnd_str = value.split(',')
-                    if len(bnd_str) == 2:
+                    if len(bnd_str)==2:
                         try:
                             low = int(bnd_str[0])
                             up = int(bnd_str[1])
-                            if 1 >= low >= 0 and 1 >= up >= 0:
+                            if low<=1 and low>=0 and up<=1 and up>=0:
                                 l_bnd = low
                                 u_bnd = up
                                 l = str(key)
                         except:
                             pass
 
                 if label.Label(l) not in specific_edge_labels.keys():
-                    specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(
-                        numba.types.Tuple((numba.types.string, numba.types.string)))
+                    specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.string)))
                 specific_edge_labels[label.Label(l)].append((e[0], e[1]))
-                f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd),
-                                   0, 0, static=static_facts)
+                f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
                 facts_edge.append(f)
 
         return facts_node, facts_edge, specific_node_labels, specific_edge_labels
```

### Comparing `pyreason-1.6.1/pyreason/scripts/utils/output.py` & `pyreason-1.8.1/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/utils/plotter.py` & `pyreason-1.8.1/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/utils/visuals.py` & `pyreason-1.8.1/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.6.1/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.8.1/pyreason/scripts/utils/yaml_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,41 +17,35 @@
     immediate_rules = numba.typed.List.empty_list(rule.rule_type)
     for rule_name, values in rules_yaml.items():
         # Set rule target
         target = label.Label('')
         if values['target'] is not None:
             target = label.Label(values['target'])
 
-        # Set rule target criteria
-        target_criteria = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, interval.interval_type)))
-        if values['target_criteria'] is not None:
-            for tc in values['target_criteria']:
-                target_criteria.append((label.Label(tc[0]), interval.closed(tc[1], tc[2])))
-
         # Set delta t
         delta_t = numba.types.uint16(values['delta_t'])
 
         # neigh_criteria = [c1, c2, c3, c4]
         # thresholds = [t1, t2, t3, t4]
 
         # Array of thresholds to keep track of for each neighbor criterion. Form [(comparison, (number/percent, total/available), thresh)]
         thresholds = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), numba.types.float64)))
 
         # Array to store clauses for nodes: node/edge, [subset]/[subset1, subset2], label, interval
-        neigh_criteria = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), label.label_type, interval.interval_type)))
+        neigh_criteria = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, label.label_type, numba.types.UniTuple(numba.types.string, 2), interval.interval_type)))
         if values['neigh_criteria'] is not None:
             # Loop through clauses
             for clause in values['neigh_criteria']:
 
                 # Append clause
                 clause_type = clause[0]
                 subset = (clause[1][0], clause[1][0]) if clause_type=='node' else (clause[1][0], clause[1][1])
                 l = label.Label(clause[2])
                 bnd = interval.closed(clause[3][0], clause[3][1])
-                neigh_criteria.append((clause_type, subset, l, bnd))
+                neigh_criteria.append((clause_type, l, subset, bnd))
 
                 # Append threshold corresponding to clause if specified in rule, else use default of greater equal to 1
                 if len(clause)>4:
                     quantifier = clause[4][0]
                     if clause[4][1]=='number':
                         quantifier_type = ('number', 'total')
                     else:
@@ -94,15 +88,16 @@
             weights = np.array(values['weights'], dtype=np.float64)
 
         # Immediate rule flag -- whether to be applied before all other rules
         immediate_rule = False
         if 'immediate' in values and values['immediate'] is not None:
             immediate_rule = True
 
-        r = rule.Rule(rule_name, target, target_criteria, delta_t, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule)
+        # Dummy rule type. this file is deprecated
+        r = rule.Rule(rule_name, 'node', target, delta_t, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule)
 
         # Insert to beginning of list if flag for immediate rule is true
         if immediate_rule:
             immediate_rules.append(r)
         else:
             rules.append(r)
```

### Comparing `pyreason-1.6.1/pyreason.egg-info/PKG-INFO` & `pyreason-1.8.1/pyreason.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.6.1
+Version: 1.8.1
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.6.1/pyreason.egg-info/SOURCES.txt` & `pyreason-1.8.1/pyreason.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 pyreason/scripts/diffuse.py
 pyreason/scripts/annotation_functions/__init__.py
 pyreason/scripts/annotation_functions/annotation_functions.py
 pyreason/scripts/components/__init__.py
 pyreason/scripts/components/label.py
 pyreason/scripts/components/world.py
 pyreason/scripts/facts/__init__.py
+pyreason/scripts/facts/fact.py
 pyreason/scripts/facts/fact_edge.py
 pyreason/scripts/facts/fact_node.py
 pyreason/scripts/interpretation/__init__.py
 pyreason/scripts/interpretation/interpretation.py
 pyreason/scripts/interval/__init__.py
 pyreason/scripts/interval/interval.py
 pyreason/scripts/numba_wrapper/__init__.py
@@ -45,9 +46,11 @@
 pyreason/scripts/rules/__init__.py
 pyreason/scripts/rules/rule.py
 pyreason/scripts/utils/__init__.py
 pyreason/scripts/utils/filter.py
 pyreason/scripts/utils/graphml_parser.py
 pyreason/scripts/utils/output.py
 pyreason/scripts/utils/plotter.py
+pyreason/scripts/utils/rule_parser.py
 pyreason/scripts/utils/visuals.py
-pyreason/scripts/utils/yaml_parser.py
+pyreason/scripts/utils/yaml_parser.py
+tests/test_hello_world.py
```

### Comparing `pyreason-1.6.1/setup.py` & `pyreason-1.8.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from setuptools import setup, find_packages
 
 # Read the contents of README file
 from pathlib import Path
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-
 setup(
-    name = 'pyreason',
-    version = '1.6.1',
-    author = 'Dyuman Aditya',
-    author_email = 'dyuman.aditya@gmail.com',
-    description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
-    long_description = long_description,
-    long_description_content_type = 'text/markdown',
-    url = 'https://github.com/lab-v2/pyreason',
-    license = 'BSD 3-clause',
-    project_urls = {
+    name='pyreason',
+    version='1.8.1',
+    author='Dyuman Aditya',
+    author_email='dyuman.aditya@gmail.com',
+    description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/lab-v2/pyreason',
+    license='BSD 3-clause',
+    project_urls={
         'Bug Tracker': 'https://github.com/lab-v2/pyreason/issues',
         'Repository': 'https://github.com/lab-v2/pyreason'
     },
-    classifiers = [
+    classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent"
     ],
-    python_requires = '>3.6',
-    install_requires = [
+    python_requires='>3.6',
+    install_requires=[
         'networkx',
         'pyyaml',
         'pandas',
         'numba',
         'numpy',
-        'memory_profiler'
+        'memory_profiler',
+        'pytest'
     ],
-    packages = find_packages(),
+    packages=find_packages(),
     include_package_data=True
 )
```


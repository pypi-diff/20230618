# Comparing `tmp/mash-shell-0.2.5.tar.gz` & `tmp/mash-shell-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mash-shell-0.2.5.tar", last modified: Sun Apr 23 19:27:43 2023, max compression
+gzip compressed data, was "mash-shell-0.2.6.tar", last modified: Fri Apr 28 11:41:05 2023, max compression
```

## Comparing `mash-shell-0.2.5.tar` & `mash-shell-0.2.6.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.193546 mash-shell-0.2.5/
--rw-r--r--   0 mark       (501) staff       (20)    35149 2022-11-28 19:29:51.000000 mash-shell-0.2.5/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)     8824 2023-04-23 19:27:43.192740 mash-shell-0.2.5/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     8256 2023-04-23 07:49:30.000000 mash-shell-0.2.5/README.md
--rw-r--r--   0 mark       (501) staff       (20)      736 2023-04-23 19:27:30.000000 mash-shell-0.2.5/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 10:23:14.000000 mash-shell-0.2.5/requirements.txt
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-23 19:27:43.193709 mash-shell-0.2.5/setup.cfg
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.099550 mash-shell-0.2.5/src/
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.111259 mash-shell-0.2.5/src/examples/
--rw-r--r--   0 mark       (501) staff       (20)       91 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/examples/_extend_path.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2059 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/examples/discoverable.py
--rwxr-xr-x   0 mark       (501) staff       (20)      965 2023-03-22 06:58:11.000000 mash-shell-0.2.5/src/examples/discoverable_api.py
--rw-r--r--   0 mark       (501) staff       (20)     1019 2023-04-23 07:55:55.000000 mash-shell-0.2.5/src/examples/discoverable_with_oas.py
--rwxr-xr-x   0 mark       (501) staff       (20)      785 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/examples/filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     1126 2023-03-24 06:51:08.000000 mash-shell-0.2.5/src/examples/ms_graph_api.py
--rwxr-xr-x   0 mark       (501) staff       (20)     3477 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/examples/object_parser.py
--rwxr-xr-x   0 mark       (501) staff       (20)     1324 2023-04-11 19:57:54.000000 mash-shell-0.2.5/src/examples/shell_example.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.127605 mash-shell-0.2.5/src/mash/
--rw-r--r--   0 mark       (501) staff       (20)       43 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/__main__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     2209 2023-03-18 14:32:23.000000 mash-shell-0.2.5/src/mash/cli.py
--rw-r--r--   0 mark       (501) staff       (20)     2479 2023-04-11 19:57:54.000000 mash-shell-0.2.5/src/mash/doc_inference.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.134285 mash-shell-0.2.5/src/mash/filesystem/
--rw-r--r--   0 mark       (501) staff       (20)      121 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/filesystem/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     6953 2023-04-15 12:12:40.000000 mash-shell-0.2.5/src/mash/filesystem/discoverable.py
--rw-r--r--   0 mark       (501) staff       (20)    10642 2023-04-23 06:48:12.000000 mash-shell-0.2.5/src/mash/filesystem/filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     3252 2023-03-18 14:32:23.000000 mash-shell-0.2.5/src/mash/filesystem/scope.py
--rw-r--r--   0 mark       (501) staff       (20)     4662 2023-04-23 08:14:44.000000 mash-shell-0.2.5/src/mash/filesystem/view.py
--rw-r--r--   0 mark       (501) staff       (20)     3455 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/html_table.py
--rw-r--r--   0 mark       (501) staff       (20)     2048 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/html_table_data.py
--rw-r--r--   0 mark       (501) staff       (20)     5161 2023-03-24 07:32:34.000000 mash-shell-0.2.5/src/mash/io_util.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.141885 mash-shell-0.2.5/src/mash/object_parser/
--rw-r--r--   0 mark       (501) staff       (20)      733 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     8289 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/factory.py
--rw-r--r--   0 mark       (501) staff       (20)     4505 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/oas.py
--rw-r--r--   0 mark       (501) staff       (20)     1727 2023-03-18 14:24:14.000000 mash-shell-0.2.5/src/mash/object_parser/object_parser.py
--rw-r--r--   0 mark       (501) staff       (20)     1129 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/object_parser_standards.py
--rw-r--r--   0 mark       (501) staff       (20)     4322 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser/spec.py
--rwxr-xr-x   0 mark       (501) staff       (20)      574 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/object_parser_server.py
--rw-r--r--   0 mark       (501) staff       (20)     8032 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/parallel.py
--rw-r--r--   0 mark       (501) staff       (20)     4176 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/parallel_requests.py
--rw-r--r--   0 mark       (501) staff       (20)     9208 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/pipeline.py
--rw-r--r--   0 mark       (501) staff       (20)      230 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/progress_bar.py
--rw-r--r--   0 mark       (501) staff       (20)     2761 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/server.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.150903 mash-shell-0.2.5/src/mash/shell/
--rw-r--r--   0 mark       (501) staff       (20)      215 2023-04-11 19:57:54.000000 mash-shell-0.2.5/src/mash/shell/__init__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.161655 mash-shell-0.2.5/src/mash/shell/ast/
--rw-r--r--   0 mark       (501) staff       (20)      880 2023-04-15 11:14:26.000000 mash-shell-0.2.5/src/mash/shell/ast/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     4686 2023-04-15 11:49:14.000000 mash-shell-0.2.5/src/mash/shell/ast/conditions.py
--rw-r--r--   0 mark       (501) staff       (20)     1740 2023-04-15 11:25:14.000000 mash-shell-0.2.5/src/mash/shell/ast/function_definition.py
--rw-r--r--   0 mark       (501) staff       (20)     5723 2023-04-23 08:24:39.000000 mash-shell-0.2.5/src/mash/shell/ast/infix.py
--rw-r--r--   0 mark       (501) staff       (20)     4735 2023-04-15 11:49:14.000000 mash-shell-0.2.5/src/mash/shell/ast/node.py
--rw-r--r--   0 mark       (501) staff       (20)     2738 2023-04-23 08:25:52.000000 mash-shell-0.2.5/src/mash/shell/ast/nodes.py
--rw-r--r--   0 mark       (501) staff       (20)     3158 2023-04-23 06:48:12.000000 mash-shell-0.2.5/src/mash/shell/ast/term.py
--rw-r--r--   0 mark       (501) staff       (20)    10985 2023-04-16 15:55:13.000000 mash-shell-0.2.5/src/mash/shell/base.py
--rw-r--r--   0 mark       (501) staff       (20)     6330 2023-04-15 10:44:24.000000 mash-shell-0.2.5/src/mash/shell/cmd2.py
--rw-r--r--   0 mark       (501) staff       (20)      136 2023-03-18 14:32:23.000000 mash-shell-0.2.5/src/mash/shell/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     2139 2023-04-15 11:49:00.000000 mash-shell-0.2.5/src/mash/shell/function.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.172328 mash-shell-0.2.5/src/mash/shell/grammer/
--rw-r--r--   0 mark       (501) staff       (20)      965 2023-04-16 15:54:19.000000 mash-shell-0.2.5/src/mash/shell/grammer/delimiters.py
--rw-r--r--   0 mark       (501) staff       (20)    13347 2023-04-23 07:07:47.000000 mash-shell-0.2.5/src/mash/shell/grammer/lex_yacc.py
--rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-15 11:17:58.000000 mash-shell-0.2.5/src/mash/shell/grammer/parsetab.py
--rw-r--r--   0 mark       (501) staff       (20)     4272 2023-04-23 07:21:26.000000 mash-shell-0.2.5/src/mash/shell/grammer/parsing.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.177254 mash-shell-0.2.5/src/mash/shell/internals/
--rw-r--r--   0 mark       (501) staff       (20)     4570 2023-04-15 11:49:14.000000 mash-shell-0.2.5/src/mash/shell/internals/helpers.py
--rw-r--r--   0 mark       (501) staff       (20)     2348 2023-04-15 11:24:38.000000 mash-shell-0.2.5/src/mash/shell/internals/if_statement.py
--rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-10 18:49:45.000000 mash-shell-0.2.5/src/mash/shell/parsetab.py
--rwxr-xr-x   0 mark       (501) staff       (20)    11208 2023-04-23 07:36:36.000000 mash-shell-0.2.5/src/mash/shell/shell.py
--rw-r--r--   0 mark       (501) staff       (20)     6593 2023-04-23 08:15:29.000000 mash-shell-0.2.5/src/mash/shell/with_filesystem.py
--rw-r--r--   0 mark       (501) staff       (20)     3223 2023-04-15 11:46:06.000000 mash-shell-0.2.5/src/mash/subshell.py
--rw-r--r--   0 mark       (501) staff       (20)    18188 2023-04-11 18:51:45.000000 mash-shell-0.2.5/src/mash/util.py
--rw-r--r--   0 mark       (501) staff       (20)     4024 2023-03-18 13:42:50.000000 mash-shell-0.2.5/src/mash/verify_server.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.180965 mash-shell-0.2.5/src/mash_shell.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     8824 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1984 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)      161 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       18 2023-04-23 19:27:43.000000 mash-shell-0.2.5/src/mash_shell.egg-info/top_level.txt
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 19:27:43.191671 mash-shell-0.2.5/test/
--rw-r--r--   0 mark       (501) staff       (20)      822 2022-12-04 19:37:35.000000 mash-shell-0.2.5/test/test_html_table.py
--rw-r--r--   0 mark       (501) staff       (20)     1106 2023-03-18 14:17:38.000000 mash-shell-0.2.5/test/test_parallel.py
--rw-r--r--   0 mark       (501) staff       (20)    10304 2023-03-18 14:16:22.000000 mash-shell-0.2.5/test/test_pipeline.py
--rw-r--r--   0 mark       (501) staff       (20)     4054 2023-03-18 14:32:23.000000 mash-shell-0.2.5/test/test_server.py
--rw-r--r--   0 mark       (501) staff       (20)     8153 2022-12-11 09:47:43.000000 mash-shell-0.2.5/test/test_util.py
--rw-r--r--   0 mark       (501) staff       (20)     2500 2022-12-04 19:39:10.000000 mash-shell-0.2.5/test/test_verify_server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.473622 mash-shell-0.2.6/
+-rw-r--r--   0 mark       (501) staff       (20)    35149 2022-11-28 19:29:51.000000 mash-shell-0.2.6/LICENSE
+-rw-r--r--   0 mark       (501) staff       (20)     8824 2023-04-28 11:41:05.472705 mash-shell-0.2.6/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     8256 2023-04-23 07:49:30.000000 mash-shell-0.2.6/README.md
+-rw-r--r--   0 mark       (501) staff       (20)      736 2023-04-28 09:08:01.000000 mash-shell-0.2.6/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)      161 2023-03-18 10:23:14.000000 mash-shell-0.2.6/requirements.txt
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-28 11:41:05.473798 mash-shell-0.2.6/setup.cfg
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.391571 mash-shell-0.2.6/src/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.402325 mash-shell-0.2.6/src/examples/
+-rw-r--r--   0 mark       (501) staff       (20)       91 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/examples/_extend_path.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2059 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/examples/discoverable.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      965 2023-03-22 06:58:11.000000 mash-shell-0.2.6/src/examples/discoverable_api.py
+-rw-r--r--   0 mark       (501) staff       (20)     1019 2023-04-23 07:55:55.000000 mash-shell-0.2.6/src/examples/discoverable_with_oas.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      785 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/examples/filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     1126 2023-03-24 06:51:08.000000 mash-shell-0.2.6/src/examples/ms_graph_api.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     3477 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/examples/object_parser.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     1324 2023-04-11 19:57:54.000000 mash-shell-0.2.6/src/examples/shell_example.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.420666 mash-shell-0.2.6/src/mash/
+-rw-r--r--   0 mark       (501) staff       (20)       43 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/__main__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     2209 2023-03-18 14:32:23.000000 mash-shell-0.2.6/src/mash/cli.py
+-rw-r--r--   0 mark       (501) staff       (20)     2479 2023-04-11 19:57:54.000000 mash-shell-0.2.6/src/mash/doc_inference.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.427314 mash-shell-0.2.6/src/mash/filesystem/
+-rw-r--r--   0 mark       (501) staff       (20)      121 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/filesystem/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     6953 2023-04-15 12:12:40.000000 mash-shell-0.2.6/src/mash/filesystem/discoverable.py
+-rw-r--r--   0 mark       (501) staff       (20)    10642 2023-04-23 06:48:12.000000 mash-shell-0.2.6/src/mash/filesystem/filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     3252 2023-03-18 14:32:23.000000 mash-shell-0.2.6/src/mash/filesystem/scope.py
+-rw-r--r--   0 mark       (501) staff       (20)     4662 2023-04-23 08:14:44.000000 mash-shell-0.2.6/src/mash/filesystem/view.py
+-rw-r--r--   0 mark       (501) staff       (20)     3455 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/html_table.py
+-rw-r--r--   0 mark       (501) staff       (20)     2048 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/html_table_data.py
+-rw-r--r--   0 mark       (501) staff       (20)     5161 2023-03-24 07:32:34.000000 mash-shell-0.2.6/src/mash/io_util.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.433034 mash-shell-0.2.6/src/mash/object_parser/
+-rw-r--r--   0 mark       (501) staff       (20)      733 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/object_parser/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     8289 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/object_parser/factory.py
+-rw-r--r--   0 mark       (501) staff       (20)     4505 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/object_parser/oas.py
+-rw-r--r--   0 mark       (501) staff       (20)     1727 2023-03-18 14:24:14.000000 mash-shell-0.2.6/src/mash/object_parser/object_parser.py
+-rw-r--r--   0 mark       (501) staff       (20)     1129 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/object_parser/object_parser_standards.py
+-rw-r--r--   0 mark       (501) staff       (20)     4322 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/object_parser/spec.py
+-rwxr-xr-x   0 mark       (501) staff       (20)      574 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/object_parser_server.py
+-rw-r--r--   0 mark       (501) staff       (20)     8032 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/parallel.py
+-rw-r--r--   0 mark       (501) staff       (20)     4176 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/parallel_requests.py
+-rw-r--r--   0 mark       (501) staff       (20)     9208 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/pipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)      230 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/progress_bar.py
+-rw-r--r--   0 mark       (501) staff       (20)     2761 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.442423 mash-shell-0.2.6/src/mash/shell/
+-rw-r--r--   0 mark       (501) staff       (20)      215 2023-04-11 19:57:54.000000 mash-shell-0.2.6/src/mash/shell/__init__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.450589 mash-shell-0.2.6/src/mash/shell/ast/
+-rw-r--r--   0 mark       (501) staff       (20)      880 2023-04-15 11:14:26.000000 mash-shell-0.2.6/src/mash/shell/ast/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     4692 2023-04-28 08:35:08.000000 mash-shell-0.2.6/src/mash/shell/ast/conditions.py
+-rw-r--r--   0 mark       (501) staff       (20)     1738 2023-04-28 08:35:07.000000 mash-shell-0.2.6/src/mash/shell/ast/function_definition.py
+-rw-r--r--   0 mark       (501) staff       (20)     5746 2023-04-28 08:47:44.000000 mash-shell-0.2.6/src/mash/shell/ast/infix.py
+-rw-r--r--   0 mark       (501) staff       (20)     4733 2023-04-28 08:35:08.000000 mash-shell-0.2.6/src/mash/shell/ast/node.py
+-rw-r--r--   0 mark       (501) staff       (20)     2744 2023-04-28 08:35:08.000000 mash-shell-0.2.6/src/mash/shell/ast/nodes.py
+-rw-r--r--   0 mark       (501) staff       (20)     3166 2023-04-28 08:08:42.000000 mash-shell-0.2.6/src/mash/shell/ast/term.py
+-rw-r--r--   0 mark       (501) staff       (20)    10763 2023-04-28 08:35:08.000000 mash-shell-0.2.6/src/mash/shell/base.py
+-rw-r--r--   0 mark       (501) staff       (20)     6330 2023-04-15 10:44:24.000000 mash-shell-0.2.6/src/mash/shell/cmd2.py
+-rw-r--r--   0 mark       (501) staff       (20)      136 2023-03-18 14:32:23.000000 mash-shell-0.2.6/src/mash/shell/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     2139 2023-04-15 11:49:00.000000 mash-shell-0.2.6/src/mash/shell/function.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.461837 mash-shell-0.2.6/src/mash/shell/grammer/
+-rw-r--r--   0 mark       (501) staff       (20)      922 2023-04-28 08:48:17.000000 mash-shell-0.2.6/src/mash/shell/grammer/literals.py
+-rw-r--r--   0 mark       (501) staff       (20)     4264 2023-04-28 08:46:53.000000 mash-shell-0.2.6/src/mash/shell/grammer/parse_functions.py
+-rw-r--r--   0 mark       (501) staff       (20)     9558 2023-04-28 09:04:48.000000 mash-shell-0.2.6/src/mash/shell/grammer/parser.py
+-rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-15 11:17:58.000000 mash-shell-0.2.6/src/mash/shell/grammer/parsetab.py
+-rw-r--r--   0 mark       (501) staff       (20)     3836 2023-04-28 09:04:15.000000 mash-shell-0.2.6/src/mash/shell/grammer/tokenizer.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.464019 mash-shell-0.2.6/src/mash/shell/internals/
+-rw-r--r--   0 mark       (501) staff       (20)     4568 2023-04-28 08:35:08.000000 mash-shell-0.2.6/src/mash/shell/internals/helpers.py
+-rw-r--r--   0 mark       (501) staff       (20)     2346 2023-04-28 08:35:07.000000 mash-shell-0.2.6/src/mash/shell/internals/if_statement.py
+-rw-r--r--   0 mark       (501) staff       (20)    24815 2023-04-10 18:49:45.000000 mash-shell-0.2.6/src/mash/shell/parsetab.py
+-rwxr-xr-x   0 mark       (501) staff       (20)    11204 2023-04-28 08:35:08.000000 mash-shell-0.2.6/src/mash/shell/shell.py
+-rw-r--r--   0 mark       (501) staff       (20)     6593 2023-04-23 08:15:29.000000 mash-shell-0.2.6/src/mash/shell/with_filesystem.py
+-rw-r--r--   0 mark       (501) staff       (20)     3223 2023-04-15 11:46:06.000000 mash-shell-0.2.6/src/mash/subshell.py
+-rw-r--r--   0 mark       (501) staff       (20)    18188 2023-04-11 18:51:45.000000 mash-shell-0.2.6/src/mash/util.py
+-rw-r--r--   0 mark       (501) staff       (20)     4024 2023-03-18 13:42:50.000000 mash-shell-0.2.6/src/mash/verify_server.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.466819 mash-shell-0.2.6/src/mash_shell.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     8824 2023-04-28 11:41:05.000000 mash-shell-0.2.6/src/mash_shell.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     2024 2023-04-28 11:41:05.000000 mash-shell-0.2.6/src/mash_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-28 11:41:05.000000 mash-shell-0.2.6/src/mash_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)      161 2023-04-28 11:41:05.000000 mash-shell-0.2.6/src/mash_shell.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       18 2023-04-28 11:41:05.000000 mash-shell-0.2.6/src/mash_shell.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:41:05.471881 mash-shell-0.2.6/test/
+-rw-r--r--   0 mark       (501) staff       (20)      822 2022-12-04 19:37:35.000000 mash-shell-0.2.6/test/test_html_table.py
+-rw-r--r--   0 mark       (501) staff       (20)     1106 2023-03-18 14:17:38.000000 mash-shell-0.2.6/test/test_parallel.py
+-rw-r--r--   0 mark       (501) staff       (20)    10304 2023-03-18 14:16:22.000000 mash-shell-0.2.6/test/test_pipeline.py
+-rw-r--r--   0 mark       (501) staff       (20)     4054 2023-03-18 14:32:23.000000 mash-shell-0.2.6/test/test_server.py
+-rw-r--r--   0 mark       (501) staff       (20)     8153 2022-12-11 09:47:43.000000 mash-shell-0.2.6/test/test_util.py
+-rw-r--r--   0 mark       (501) staff       (20)     2500 2022-12-04 19:39:10.000000 mash-shell-0.2.6/test/test_verify_server.py
```

### Comparing `mash-shell-0.2.5/LICENSE` & `mash-shell-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/PKG-INFO` & `mash-shell-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mash-shell
-Version: 0.2.5
+Version: 0.2.6
 Summary: A shell and other utils
 Author-email: voschezang <mark.voschezang@student.uva.nl>
 Project-URL: Homepage, https://github.com/voschezang/mash
 Project-URL: Bug Tracker, https://github.com/voschezang/mash/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Shells
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mash-shell Version: 0.2.5 Summary: A shell and
+Metadata-Version: 2.1 Name: mash-shell Version: 0.2.6 Summary: A shell and
 other utils Author-email: voschezang
 voschezang@student.uva.nl> Project-URL: Homepage, https://github.com/
 voschezang/mash Project-URL: Bug Tracker, https://github.com/voschezang/mash/
 issues Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 System :: Shells Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE !
```

### Comparing `mash-shell-0.2.5/README.md` & `mash-shell-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/pyproject.toml` & `mash-shell-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mash-shell"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="voschezang", email="mark.voschezang@student.uva.nl" },
 ]
 description = "A shell and other utils"
 dynamic = ["dependencies"]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mash-shell-0.2.5/src/examples/discoverable.py` & `mash-shell-0.2.6/src/examples/discoverable.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/examples/discoverable_api.py` & `mash-shell-0.2.6/src/examples/discoverable_api.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/examples/discoverable_with_oas.py` & `mash-shell-0.2.6/src/examples/discoverable_with_oas.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/examples/filesystem.py` & `mash-shell-0.2.6/src/examples/filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/examples/ms_graph_api.py` & `mash-shell-0.2.6/src/examples/ms_graph_api.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/examples/object_parser.py` & `mash-shell-0.2.6/src/examples/object_parser.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/examples/shell_example.py` & `mash-shell-0.2.6/src/examples/shell_example.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/cli.py` & `mash-shell-0.2.6/src/mash/cli.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/doc_inference.py` & `mash-shell-0.2.6/src/mash/doc_inference.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/filesystem/discoverable.py` & `mash-shell-0.2.6/src/mash/filesystem/discoverable.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/filesystem/filesystem.py` & `mash-shell-0.2.6/src/mash/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/filesystem/scope.py` & `mash-shell-0.2.6/src/mash/filesystem/scope.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/filesystem/view.py` & `mash-shell-0.2.6/src/mash/filesystem/view.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/html_table.py` & `mash-shell-0.2.6/src/mash/html_table.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/html_table_data.py` & `mash-shell-0.2.6/src/mash/html_table_data.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/io_util.py` & `mash-shell-0.2.6/src/mash/io_util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/object_parser/errors.py` & `mash-shell-0.2.6/src/mash/object_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/object_parser/factory.py` & `mash-shell-0.2.6/src/mash/object_parser/factory.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/object_parser/oas.py` & `mash-shell-0.2.6/src/mash/object_parser/oas.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/object_parser/object_parser.py` & `mash-shell-0.2.6/src/mash/object_parser/object_parser.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/object_parser/object_parser_standards.py` & `mash-shell-0.2.6/src/mash/object_parser/object_parser_standards.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/object_parser/spec.py` & `mash-shell-0.2.6/src/mash/object_parser/spec.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/object_parser_server.py` & `mash-shell-0.2.6/src/mash/object_parser_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/parallel.py` & `mash-shell-0.2.6/src/mash/parallel.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/parallel_requests.py` & `mash-shell-0.2.6/src/mash/parallel_requests.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/pipeline.py` & `mash-shell-0.2.6/src/mash/pipeline.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/server.py` & `mash-shell-0.2.6/src/mash/server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/shell/ast/__init__.py` & `mash-shell-0.2.6/src/mash/shell/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/shell/ast/conditions.py` & `mash-shell-0.2.6/src/mash/shell/ast/conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from mash.shell.ast.node import Node
 from mash.shell.base import BaseShell
-from mash.shell.grammer.delimiters import FALSE, IF, INLINE_ELSE, INLINE_THEN, THEN, TRUE
+from mash.shell.grammer.literals import FALSE, IF, INLINE_ELSE, INLINE_THEN, THEN, TRUE
 from mash.shell.internals.if_statement import Abort, State, handle_else_statement, handle_then_statement
-from mash.shell.grammer.parsing import to_bool
+from mash.shell.grammer.parse_functions import to_bool
 
 
 class Condition(Node):
     def __init__(self, condition=None, then=None, otherwise=None):
         self.condition = condition
         self.then = then
         self.otherwise = otherwise
```

### Comparing `mash-shell-0.2.5/src/mash/shell/ast/function_definition.py` & `mash-shell-0.2.6/src/mash/shell/ast/function_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from mash.shell.grammer.delimiters import DEFINE_FUNCTION
+from mash.shell.grammer.literals import DEFINE_FUNCTION
 from mash.shell.ast.node import Node
 from mash.shell.base import BaseShell
 from mash.shell.errors import ShellError
 from mash.shell.function import InlineFunction
 from mash.util import has_method
```

### Comparing `mash-shell-0.2.5/src/mash/shell/ast/infix.py` & `mash-shell-0.2.6/src/mash/shell/ast/infix.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 from mash.shell.ast.node import Math, Node, run_shell_command
 from mash.shell.ast.nodes import Terms
 from mash.shell.ast.term import Quoted, Term
 from mash.shell.base import BaseShell
 from mash.shell.errors import ShellError, ShellSyntaxError
 from mash.shell.function import LAST_RESULTS, LAST_RESULTS_INDEX
-from mash.shell.grammer.delimiters import comparators, FALSE, TRUE
-from mash.shell.grammer.parsing import quote_items, quote_return_value, to_bool
+from mash.shell.grammer import literals
+from mash.shell.grammer.literals import FALSE, TRUE
+
+from mash.shell.grammer.parse_functions import quote_items, to_bool
 from mash.shell.internals.helpers import set_env_variables
 from mash.util import quote_all
 
 
 ################################################################################
 # Infix Operator Expressions
 ################################################################################
@@ -89,15 +91,15 @@
 
         op = self.op
         a = shell.run_commands(self.lhs, run=not lazy)
         b = shell.run_commands(self.rhs, run=not lazy)
 
         line = ' '.join(quote_items([a, op, b]))
 
-        if op in comparators:
+        if op in literals.comparators:
             if not lazy:
                 return Math.eval(line, shell.env)
             return a, op, b
 
         if op in '+-*/':
             # math
             if not lazy:
```

### Comparing `mash-shell-0.2.5/src/mash/shell/ast/node.py` & `mash-shell-0.2.6/src/mash/shell/ast/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import UserString
 import re
 from typing import List
 from mash.io_util import log
 from mash.shell.base import BaseShell
-from mash.shell.grammer.delimiters import FALSE, IF, INLINE_ELSE, INLINE_THEN
+from mash.shell.grammer.literals import FALSE, IF, INLINE_ELSE, INLINE_THEN
 from mash.shell.errors import ShellSyntaxError
 from mash.shell.internals.if_statement import LINE_INDENT, Abort, close_prev_if_statements, handle_prev_then_else_statements
 from mash.shell.internals.helpers import ReturnValue, run_function, run_shell_command
 from mash.util import quote_all, translate_items
 
 
 class Node(UserString):
```

### Comparing `mash-shell-0.2.5/src/mash/shell/ast/nodes.py` & `mash-shell-0.2.6/src/mash/shell/ast/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Containers
 Nodes that contain multiple nodes.
 """
 
 from typing import List
 from mash.shell.ast.conditions import ElseCondition, Then
-from mash.shell.grammer.delimiters import IF
+from mash.shell.grammer.literals import IF
 from mash.shell.internals.helpers import ReturnValue
 from mash.shell.ast.node import Indent, Node
 from mash.shell.ast.term import Term
 from mash.shell.base import BaseShell
 from mash.shell.internals.if_statement import LINE_INDENT, close_prev_if_statements
-from mash.shell.grammer.parsing import indent_width, to_string
+from mash.shell.grammer.parse_functions import indent_width, to_string
 
 
 class Nodes(Node):
     def __init__(self, values: List[Node]):
         self._values = values
 
     @property
```

### Comparing `mash-shell-0.2.5/src/mash/shell/ast/term.py` & `mash-shell-0.2.6/src/mash/shell/ast/term.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from mash.shell.internals.if_statement import Abort
 from mash.shell.internals.helpers import run_function
 from mash.shell.ast.node import Node
 from mash.shell.base import BaseShell
-from mash.shell.grammer.parsing import expand_variables
+from mash.shell.grammer.parse_functions import expand_variables
 from mash.util import quote_all
 
 
 class Term(Node):
     def __eq__(self, other):
         """Literal comparison
         """
```

### Comparing `mash-shell-0.2.5/src/mash/shell/base.py` & `mash-shell-0.2.6/src/mash/shell/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from typing import Any, Callable, Dict, List
 import logging
 
 from mash.shell.cmd2 import Cmd2
 from mash.filesystem.filesystem import FileSystem
 from mash.filesystem.scope import Scope, show
 from mash.io_util import log, print_shell_ready_signal
-from mash.shell.grammer import delimiters
-from mash.shell.grammer.delimiters import FALSE, IF, TRUE
+from mash.shell.grammer import literals
+from mash.shell.grammer.literals import FALSE, IF, TRUE
 from mash.shell.errors import ShellError
 from mash.shell.function import LAST_RESULTS, LAST_RESULTS_INDEX, InlineFunction, scope
 from mash.shell.function import ShellFunction as Function
-from mash.shell.grammer.parsing import to_bool
+from mash.shell.grammer.parse_functions import to_bool
 from mash.util import has_method, identity
 
 
 default_session_filename = '.shell_session.json'
 default_function_group_key = '_'
 
 ENV = 'env'
@@ -83,23 +83,14 @@
         self._default_method = identity
 
     def init_current_scope(self):
         self.locals.set(IF, [])
         self.locals.set(ENV, {})
 
     @property
-    def delimiters(self):
-        """Return the most recent values of the delimiters.
-        """
-        items = delimiters.all.copy()
-        items.remove('=')
-        items.remove('#')
-        return items
-
-    @property
     def _last_if(self):
         return self.locals[IF][-1]
 
     @property
     def _last_results(self):
         return self.env[LAST_RESULTS]
 
@@ -236,15 +227,15 @@
         if isinstance(method, Function):
             return method.func
 
         return method
 
     def add_special_function(self, char: str, method: Command):
         # TODO merge this with self.add_functions
-        if char in delimiters.all or char in '!?':
+        if char in literals.all or char in '!?':
             raise ShellError(f'Char {char} is already in use.')
 
         self.add_functions({char: method}, CHAR)
 
     def run_special_function(self, k: str, args):
         return self.function_groups[CHAR][k](*args)
```

### Comparing `mash-shell-0.2.5/src/mash/shell/cmd2.py` & `mash-shell-0.2.6/src/mash/shell/cmd2.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/shell/function.py` & `mash-shell-0.2.6/src/mash/shell/function.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/shell/grammer/parsetab.py` & `mash-shell-0.2.6/src/mash/shell/grammer/parsetab.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/shell/grammer/parsing.py` & `mash-shell-0.2.6/src/mash/shell/grammer/parse_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from logging import debug
 from typing import Any, Iterable, List, Tuple
 import shlex
 
 from mash.io_util import log
-from mash.shell.grammer import delimiters
-from mash.shell.grammer.delimiters import FALSE, TRUE
+from mash.shell.grammer import literals
+from mash.shell.grammer.literals import FALSE, TRUE
 from mash.shell.errors import ShellError
 from mash.util import is_globbable, is_valid_method_name, match_words, quote, quote_all, glob
 
 
 def expand_variables(terms: List[str], env: dict,
                      completenames_options: List[str],
                      ignore_invalid_syntax: bool,
@@ -107,15 +107,15 @@
 
 def quote_items(items: List[str]) -> Iterable[str]:
     """Map shlex.quote() to all items.
     Do not modify python delimiters.
     """
     for arg in items:
         arg = str(arg)
-        if arg in delimiters.python or arg in delimiters.comparators:
+        if arg in literals.python or arg in literals.comparators:
             yield arg
         else:
             yield shlex.quote(arg)
 
 
 def indent_width(line: str) -> Tuple[str, str]:
     """Return a tuple that represents the length of the indentation in spaces and tabs.
```

### Comparing `mash-shell-0.2.5/src/mash/shell/internals/helpers.py` & `mash-shell-0.2.6/src/mash/shell/internals/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import shlex
 import subprocess
 from typing import List, Union
 from mash.filesystem.filesystem import cd
 from mash.io_util import log
 from mash.shell.base import BaseShell
-from mash.shell.grammer.delimiters import bash, FALSE
+from mash.shell.grammer.literals import bash, FALSE
 from mash.shell.errors import ShellError
 from mash.shell.function import scope
 from mash.shell.internals.if_statement import Abort
 from mash.util import quote_all
 
 INNER_SCOPE = 'inner_scope'
```

### Comparing `mash-shell-0.2.5/src/mash/shell/internals/if_statement.py` & `mash-shell-0.2.6/src/mash/shell/internals/if_statement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from mash.shell.grammer.delimiters import ELSE, IF, THEN
+from mash.shell.grammer.literals import ELSE, IF, THEN
 from mash.shell.errors import ShellError
 
 LINE_INDENT = 'line_indent'
 RAW_LINE_INDENT = 'raw_line_indent'
 
 
 class Abort(RuntimeError):
```

### Comparing `mash-shell-0.2.5/src/mash/shell/parsetab.py` & `mash-shell-0.2.6/src/mash/shell/parsetab.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/shell/shell.py` & `mash-shell-0.2.6/src/mash/shell/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 from mash import io_util
 from mash.io_util import ArgparseWrapper, bold, has_argument, has_output, log, log_once
 from mash.shell.function import LAST_RESULTS
 from mash.shell.ast import ElseCondition, Indent, Lines, Map, Math, Node, Term, Terms
 from mash.shell.base import BaseShell
 from mash.shell.cmd2 import default_prompt, run
-from mash.shell.grammer.delimiters import DEFINE_FUNCTION
+from mash.shell.grammer.literals import DEFINE_FUNCTION
 from mash.shell.errors import ShellError, ShellPipeError, ShellSyntaxError
 from mash.shell.errors import ShellSyntaxError
 from mash.shell.function import ShellFunction as Function
 from mash.shell.internals.if_statement import Abort, handle_prev_then_else_statements
-from mash.shell.grammer.lex_yacc import parse
+from mash.shell.grammer.parser import parse
 from mash.util import has_method, is_valid_method_name
 
 description = 'If no positional arguments are given then an interactive subshell is started.'
 epilog = f"""
 --------------------------------------------------------------------------------
 {bold('Default Commands')}
 Run shell commands by prefixing them with `!`.
```

### Comparing `mash-shell-0.2.5/src/mash/shell/with_filesystem.py` & `mash-shell-0.2.6/src/mash/shell/with_filesystem.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/subshell.py` & `mash-shell-0.2.6/src/mash/subshell.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/util.py` & `mash-shell-0.2.6/src/mash/util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash/verify_server.py` & `mash-shell-0.2.6/src/mash/verify_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/src/mash_shell.egg-info/PKG-INFO` & `mash-shell-0.2.6/src/mash_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mash-shell
-Version: 0.2.5
+Version: 0.2.6
 Summary: A shell and other utils
 Author-email: voschezang <mark.voschezang@student.uva.nl>
 Project-URL: Homepage, https://github.com/voschezang/mash
 Project-URL: Bug Tracker, https://github.com/voschezang/mash/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Shells
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mash-shell Version: 0.2.5 Summary: A shell and
+Metadata-Version: 2.1 Name: mash-shell Version: 0.2.6 Summary: A shell and
 other utils Author-email: voschezang
 voschezang@student.uva.nl> Project-URL: Homepage, https://github.com/
 voschezang/mash Project-URL: Bug Tracker, https://github.com/voschezang/mash/
 issues Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 System :: Shells Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE !
```

### Comparing `mash-shell-0.2.5/src/mash_shell.egg-info/SOURCES.txt` & `mash-shell-0.2.6/src/mash_shell.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,19 @@
 src/mash/shell/ast/__init__.py
 src/mash/shell/ast/conditions.py
 src/mash/shell/ast/function_definition.py
 src/mash/shell/ast/infix.py
 src/mash/shell/ast/node.py
 src/mash/shell/ast/nodes.py
 src/mash/shell/ast/term.py
-src/mash/shell/grammer/delimiters.py
-src/mash/shell/grammer/lex_yacc.py
+src/mash/shell/grammer/literals.py
+src/mash/shell/grammer/parse_functions.py
+src/mash/shell/grammer/parser.py
 src/mash/shell/grammer/parsetab.py
-src/mash/shell/grammer/parsing.py
+src/mash/shell/grammer/tokenizer.py
 src/mash/shell/internals/helpers.py
 src/mash/shell/internals/if_statement.py
 src/mash_shell.egg-info/PKG-INFO
 src/mash_shell.egg-info/SOURCES.txt
 src/mash_shell.egg-info/dependency_links.txt
 src/mash_shell.egg-info/requires.txt
 src/mash_shell.egg-info/top_level.txt
```

### Comparing `mash-shell-0.2.5/test/test_html_table.py` & `mash-shell-0.2.6/test/test_html_table.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/test/test_parallel.py` & `mash-shell-0.2.6/test/test_parallel.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/test/test_pipeline.py` & `mash-shell-0.2.6/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/test/test_server.py` & `mash-shell-0.2.6/test/test_server.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/test/test_util.py` & `mash-shell-0.2.6/test/test_util.py`

 * *Files identical despite different names*

### Comparing `mash-shell-0.2.5/test/test_verify_server.py` & `mash-shell-0.2.6/test/test_verify_server.py`

 * *Files identical despite different names*


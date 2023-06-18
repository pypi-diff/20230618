# Comparing `tmp/pddl-plus-parser-3.3.9.tar.gz` & `tmp/pddl-plus-parser-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pddl-plus-parser-3.3.9.tar", last modified: Mon May  1 08:11:48 2023, max compression
+gzip compressed data, was "pddl-plus-parser-3.4.0.tar", last modified: Sun Jun 18 20:53:12 2023, max compression
```

## Comparing `pddl-plus-parser-3.3.9.tar` & `pddl-plus-parser-3.4.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.074838 pddl-plus-parser-3.3.9/
--rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.3.9/LICENSE
--rw-rw-rw-   0        0        0     1519 2023-05-01 08:11:48.074838 pddl-plus-parser-3.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     1249 2023-04-17 12:20:18.000000 pddl-plus-parser-3.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.957041 pddl-plus-parser-3.3.9/pddl_plus_parser/
--rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.971779 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/
--rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/__init__.py
--rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/domain_exporter.py
--rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/enhsp_output_parser.py
--rw-rw-rw-   0        0        0     3613 2022-06-02 06:33:08.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/ff_output_parser.py
--rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
--rw-rw-rw-   0        0        0     4458 2022-08-21 11:50:38.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/problem_exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.985771 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/
--rw-rw-rw-   0        0        0      376 2023-04-17 14:54:54.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/__init__.py
--rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/domain_parser.py
--rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/effects_parser.py
--rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/parsing_utils.py
--rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
--rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
--rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/preconditions_parser.py
--rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/problem_parser.py
--rw-rw-rw-   0        0        0    10281 2023-02-20 11:23:13.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/trajectory_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.013235 pddl-plus-parser-3.3.9/pddl_plus_parser/models/
--rw-rw-rw-   0        0        0      835 2023-05-01 08:05:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/__init__.py
--rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/action_call.py
--rw-rw-rw-   0        0        0     1935 2023-05-01 08:11:11.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/conditional_effect.py
--rw-rw-rw-   0        0        0     5945 2023-04-17 10:57:12.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounded_effect.py
--rw-rw-rw-   0        0        0    13069 2023-04-30 16:17:41.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounded_precondition.py
--rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounding_utils.py
--rw-rw-rw-   0        0        0     7500 2023-04-16 13:28:59.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/numerical_expression.py
--rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/observation.py
--rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_action.py
--rw-rw-rw-   0        0        0     1415 2022-08-21 09:16:42.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_domain.py
--rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_function.py
--rw-rw-rw-   0        0        0      372 2022-01-17 15:22:52.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_object.py
--rw-rw-rw-   0        0        0     8653 2023-04-30 16:08:01.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_operator.py
--rw-rw-rw-   0        0        0     9709 2023-04-27 10:37:17.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_precondition.py
--rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_predicate.py
--rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_problem.py
--rw-rw-rw-   0        0        0     2845 2023-04-30 16:46:24.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_state.py
--rw-rw-rw-   0        0        0     1135 2022-03-15 08:50:58.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_type.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.022755 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/
--rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/common.py
--rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
--rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
--rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
--rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.037780 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/
--rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/__init__.py
--rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/common.py
--rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/counters_generator.py
--rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/depots_generator.py
--rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/farmland_generator.py
--rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/plant_watering_generator.py
--rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/sailing_generator.py
--rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/settlers_problem_generator.py
--rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/zenotravel_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.963040 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/
--rw-rw-rw-   0        0        0     1519 2023-05-01 08:11:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3519 2023-05-01 08:11:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 08:11:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-01 08:11:47.000000 pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 08:11:48.075839 pddl-plus-parser-3.3.9/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-05-01 08:11:35.000000 pddl-plus-parser-3.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:47.953025 pddl-plus-parser-3.3.9/tests/
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.040780 pddl-plus-parser-3.3.9/tests/exporters_tests/
--rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.3.9/tests/exporters_tests/__init__.py
--rw-rw-rw-   0        0        0    10765 2023-04-30 16:18:40.000000 pddl-plus-parser-3.3.9/tests/exporters_tests/numeric_trajectory_exporter_test.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.050301 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/
--rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/__init__.py
--rw-rw-rw-   0        0        0     3288 2023-04-17 12:07:14.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/consts.py
--rw-rw-rw-   0        0        0    39905 2023-04-17 12:16:07.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/domain_parser_test.py
--rw-rw-rw-   0        0        0     3578 2023-04-09 11:50:45.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/pddl_tokenizer_test.py
--rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/problem_parser_test.py
--rw-rw-rw-   0        0        0     6285 2023-02-21 16:00:23.000000 pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/trajectory_parser_test.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.062837 pddl-plus-parser-3.3.9/tests/models_tests/
--rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.3.9/tests/models_tests/__init__.py
--rw-rw-rw-   0        0        0      427 2022-12-05 14:12:59.000000 pddl-plus-parser-3.3.9/tests/models_tests/consts.py
--rw-rw-rw-   0        0        0    15208 2023-04-17 10:08:25.000000 pddl-plus-parser-3.3.9/tests/models_tests/grounded_effect_test.py
--rw-rw-rw-   0        0        0    25195 2023-04-30 16:17:00.000000 pddl-plus-parser-3.3.9/tests/models_tests/grounded_precondition_test.py
--rw-rw-rw-   0        0        0     3516 2022-06-08 11:36:39.000000 pddl-plus-parser-3.3.9/tests/models_tests/numerical_expression_test.py
--rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.3.9/tests/models_tests/operator_test.py
--rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.3.9/tests/models_tests/pddl_function_test.py
--rw-rw-rw-   0        0        0     6075 2023-04-27 10:33:43.000000 pddl-plus-parser-3.3.9/tests/models_tests/pddl_precondition_test.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:11:48.072839 pddl-plus-parser-3.3.9/tests/multi_agent_tests/
--rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/__init__.py
--rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/consts.py
--rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_domain_converter_test.py
--rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_problem_converter_test.py
--rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
--rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.3.9/tests/multi_agent_tests/single_agent_plan_converter_test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.435533 pddl-plus-parser-3.4.0/
+-rw-rw-rw-   0        0        0    11499 2022-01-08 09:02:31.000000 pddl-plus-parser-3.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1519 2023-06-18 20:53:12.435533 pddl-plus-parser-3.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1249 2023-04-17 12:20:18.000000 pddl-plus-parser-3.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.354249 pddl-plus-parser-3.4.0/pddl_plus_parser/
+-rw-rw-rw-   0        0        0        0 2022-03-13 12:11:09.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.364768 pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/
+-rw-rw-rw-   0        0        0      264 2022-08-21 09:19:40.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/__init__.py
+-rw-rw-rw-   0        0        0     7553 2022-08-21 12:45:31.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/domain_exporter.py
+-rw-rw-rw-   0        0        0     1348 2022-06-02 13:51:41.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/enhsp_output_parser.py
+-rw-rw-rw-   0        0        0     3613 2022-06-02 06:33:08.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/ff_output_parser.py
+-rw-rw-rw-   0        0        0     6141 2023-03-14 07:34:52.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/numeric_trajectory_exporter.py
+-rw-rw-rw-   0        0        0     4458 2022-08-21 11:50:38.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/problem_exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.378293 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/
+-rw-rw-rw-   0        0        0      376 2023-06-18 20:40:16.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/__init__.py
+-rw-rw-rw-   0        0        0    14713 2023-04-13 11:10:47.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/domain_parser.py
+-rw-rw-rw-   0        0        0    10635 2023-04-17 10:32:20.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/effects_parser.py
+-rw-rw-rw-   0        0        0     2998 2023-04-13 11:23:17.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/parsing_utils.py
+-rw-rw-rw-   0        0        0      200 2022-01-09 12:51:47.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/pddl_parser_types.py
+-rw-rw-rw-   0        0        0     2610 2022-12-05 08:48:42.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py
+-rw-rw-rw-   0        0        0     5558 2023-04-13 11:44:39.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/preconditions_parser.py
+-rw-rw-rw-   0        0        0    11961 2022-12-05 08:49:12.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/problem_parser.py
+-rw-rw-rw-   0        0        0    13065 2023-06-18 20:51:11.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/trajectory_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.394335 pddl-plus-parser-3.4.0/pddl_plus_parser/models/
+-rw-rw-rw-   0        0        0      835 2023-05-01 08:05:47.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/__init__.py
+-rw-rw-rw-   0        0        0     1296 2023-02-19 07:22:18.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/action_call.py
+-rw-rw-rw-   0        0        0     1935 2023-05-01 08:11:11.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/conditional_effect.py
+-rw-rw-rw-   0        0        0     5945 2023-04-17 10:57:12.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/grounded_effect.py
+-rw-rw-rw-   0        0        0    13240 2023-05-14 10:03:56.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/grounded_precondition.py
+-rw-rw-rw-   0        0        0     6340 2023-04-16 14:57:28.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/grounding_utils.py
+-rw-rw-rw-   0        0        0     7500 2023-04-16 13:28:59.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/numerical_expression.py
+-rw-rw-rw-   0        0        0     3753 2022-12-05 08:50:29.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/observation.py
+-rw-rw-rw-   0        0        0     1293 2023-04-13 13:54:50.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_action.py
+-rw-rw-rw-   0        0        0     1415 2022-08-21 09:16:42.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_domain.py
+-rw-rw-rw-   0        0        0     3973 2023-04-16 13:39:30.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_function.py
+-rw-rw-rw-   0        0        0      372 2022-01-17 15:22:52.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_object.py
+-rw-rw-rw-   0        0        0     8675 2023-05-16 11:04:11.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_operator.py
+-rw-rw-rw-   0        0        0     9660 2023-06-08 13:07:17.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_precondition.py
+-rw-rw-rw-   0        0        0     4737 2023-04-16 13:37:45.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_predicate.py
+-rw-rw-rw-   0        0        0     1953 2022-11-18 11:18:07.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_problem.py
+-rw-rw-rw-   0        0        0     2845 2023-04-30 16:46:24.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_state.py
+-rw-rw-rw-   0        0        0     1135 2022-03-15 08:50:58.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_type.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.399334 pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/
+-rw-rw-rw-   0        0        0      324 2023-02-21 12:20:37.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-04-17 11:31:48.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/common.py
+-rw-rw-rw-   0        0        0     3282 2023-04-17 10:59:23.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py
+-rw-rw-rw-   0        0        0     3031 2022-12-05 09:13:45.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py
+-rw-rw-rw-   0        0        0     7079 2023-02-19 14:32:32.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py
+-rw-rw-rw-   0        0        0    10857 2023-04-17 11:26:47.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/single_agent_plan_converter.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.410936 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/
+-rw-rw-rw-   0        0        0       40 2022-05-10 14:32:52.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/__init__.py
+-rw-rw-rw-   0        0        0      357 2022-09-28 11:37:49.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/common.py
+-rw-rw-rw-   0        0        0     3325 2022-09-28 12:05:01.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/counters_generator.py
+-rw-rw-rw-   0        0        0    12536 2022-05-16 08:10:09.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/depots_generator.py
+-rw-rw-rw-   0        0        0     5992 2022-09-28 12:09:35.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/farmland_generator.py
+-rw-rw-rw-   0        0        0     3756 2022-08-04 13:43:32.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/plant_watering_generator.py
+-rw-rw-rw-   0        0        0     3679 2022-09-28 11:53:25.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/sailing_generator.py
+-rw-rw-rw-   0        0        0    12311 2022-05-16 19:14:35.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/settlers_problem_generator.py
+-rw-rw-rw-   0        0        0     8805 2022-09-28 12:16:10.000000 pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/zenotravel_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.358249 pddl-plus-parser-3.4.0/pddl_plus_parser.egg-info/
+-rw-rw-rw-   0        0        0     1519 2023-06-18 20:53:12.000000 pddl-plus-parser-3.4.0/pddl_plus_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3519 2023-06-18 20:53:12.000000 pddl-plus-parser-3.4.0/pddl_plus_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 20:53:12.000000 pddl-plus-parser-3.4.0/pddl_plus_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-18 20:53:12.000000 pddl-plus-parser-3.4.0/pddl_plus_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 20:53:12.435533 pddl-plus-parser-3.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-06-18 20:51:11.000000 pddl-plus-parser-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.350774 pddl-plus-parser-3.4.0/tests/
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.413148 pddl-plus-parser-3.4.0/tests/exporters_tests/
+-rw-rw-rw-   0        0        0        0 2022-02-28 12:11:52.000000 pddl-plus-parser-3.4.0/tests/exporters_tests/__init__.py
+-rw-rw-rw-   0        0        0    10765 2023-04-30 16:18:40.000000 pddl-plus-parser-3.4.0/tests/exporters_tests/numeric_trajectory_exporter_test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.418654 pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-09 08:03:59.000000 pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/__init__.py
+-rw-rw-rw-   0        0        0     3503 2023-06-18 20:27:00.000000 pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/consts.py
+-rw-rw-rw-   0        0        0    40370 2023-05-15 14:36:27.000000 pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/domain_parser_test.py
+-rw-rw-rw-   0        0        0     3578 2023-04-09 11:50:45.000000 pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/pddl_tokenizer_test.py
+-rw-rw-rw-   0        0        0    17734 2022-08-21 10:17:02.000000 pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/problem_parser_test.py
+-rw-rw-rw-   0        0        0     7601 2023-06-18 20:45:34.000000 pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/trajectory_parser_test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.428001 pddl-plus-parser-3.4.0/tests/models_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-10 14:06:38.000000 pddl-plus-parser-3.4.0/tests/models_tests/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-05-14 10:23:24.000000 pddl-plus-parser-3.4.0/tests/models_tests/consts.py
+-rw-rw-rw-   0        0        0    15208 2023-04-17 10:08:25.000000 pddl-plus-parser-3.4.0/tests/models_tests/grounded_effect_test.py
+-rw-rw-rw-   0        0        0    27127 2023-05-14 10:23:35.000000 pddl-plus-parser-3.4.0/tests/models_tests/grounded_precondition_test.py
+-rw-rw-rw-   0        0        0     3516 2022-06-08 11:36:39.000000 pddl-plus-parser-3.4.0/tests/models_tests/numerical_expression_test.py
+-rw-rw-rw-   0        0        0    19392 2023-04-17 09:59:27.000000 pddl-plus-parser-3.4.0/tests/models_tests/operator_test.py
+-rw-rw-rw-   0        0        0     1646 2022-06-21 11:55:51.000000 pddl-plus-parser-3.4.0/tests/models_tests/pddl_function_test.py
+-rw-rw-rw-   0        0        0     6075 2023-04-27 10:33:43.000000 pddl-plus-parser-3.4.0/tests/models_tests/pddl_precondition_test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:53:12.433536 pddl-plus-parser-3.4.0/tests/multi_agent_tests/
+-rw-rw-rw-   0        0        0        0 2022-08-18 10:56:04.000000 pddl-plus-parser-3.4.0/tests/multi_agent_tests/__init__.py
+-rw-rw-rw-   0        0        0     1706 2022-11-13 14:49:21.000000 pddl-plus-parser-3.4.0/tests/multi_agent_tests/consts.py
+-rw-rw-rw-   0        0        0     2123 2023-04-17 11:05:34.000000 pddl-plus-parser-3.4.0/tests/multi_agent_tests/multi_agent_domain_converter_test.py
+-rw-rw-rw-   0        0        0     2256 2022-10-27 12:17:55.000000 pddl-plus-parser-3.4.0/tests/multi_agent_tests/multi_agent_problem_converter_test.py
+-rw-rw-rw-   0        0        0     8908 2022-12-05 15:59:59.000000 pddl-plus-parser-3.4.0/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py
+-rw-rw-rw-   0        0        0     6939 2022-10-27 08:18:32.000000 pddl-plus-parser-3.4.0/tests/multi_agent_tests/single_agent_plan_converter_test.py
```

### Comparing `pddl-plus-parser-3.3.9/LICENSE` & `pddl-plus-parser-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/PKG-INFO` & `pddl-plus-parser-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.3.9
+Version: 3.4.0
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDDL Plus Parser
```

### Comparing `pddl-plus-parser-3.3.9/README.md` & `pddl-plus-parser-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/domain_exporter.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/domain_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/enhsp_output_parser.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/enhsp_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/ff_output_parser.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/ff_output_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/numeric_trajectory_exporter.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/numeric_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/exporters/problem_exporter.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/exporters/problem_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/domain_parser.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/domain_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/effects_parser.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/effects_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/parsing_utils.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/pddl_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/preconditions_parser.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/preconditions_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/problem_parser.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/problem_parser.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/lisp_parsers/trajectory_parser.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/lisp_parsers/trajectory_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """Module to parse a serialized trajectory and export it as an object fitted for learning."""
 import logging
 from collections import defaultdict
 from pathlib import Path
-from typing import List, Union
+from typing import List, Union, Optional, Dict
 
 from pddl_plus_parser.lisp_parsers.pddl_tokenizer import PDDLTokenizer
 from pddl_plus_parser.models import Domain, Observation, State, ActionCall, PDDLFunction, Predicate, GroundedPredicate, \
-    Problem, MultiAgentObservation, NOP_ACTION
+    Problem, MultiAgentObservation, NOP_ACTION, PDDLObject
 
 
 class TrajectoryParser:
     """Class that is able to parse a trajectory file and extract its content.
 
     Note: This class assumes that the trajectory size is tractable and thus, reads the entire file at once.
     For lay loading of a trajectory future development is needed.
+
+    Warning: if the problem object is none, all objects should be present in the initial state of the trajectory.
+    Furthermore, in this case the script will not support type hierarchy or type checking for the observation objects.
     """
 
     partial_domain: Domain  # domain containing only the publicly known information.
     problem: Problem
     logger: logging.Logger
 
-    def __init__(self, partial_domain: Domain, problem: Problem):
+    def __init__(self, partial_domain: Domain, problem: Optional[Problem]=None):
         self.partial_domain = partial_domain
         self.problem = problem
         self.logger = logging.getLogger(__name__)
 
     def _read_trajectory_file(self, trajectory_file_path: Path) -> PDDLTokenizer:
         """Reads the trajectory file and exports the lines containing the data about the trajectory.
 
@@ -83,14 +86,22 @@
         # For now, assuming that fluents have valid parameters.
         fluent_signature_items = grounded_numeric_fluent[1:]
         if len(fluent_signature_items) != len(lifted_function.signature):
             raise ValueError(
                 f"Received fluent - {function_name} with wrong number of parameters! "
                 f"Expected - {len(lifted_function.signature)} and received - {len(fluent_signature_items)}")
 
+        if self.problem is None:
+            self.logger.debug("Since we don't know the objects in the problem, we don't need to validate their types.")
+            fluent_signature = {
+                object_name: list(lifted_function.signature.values())[index]
+                for index, object_name in enumerate(fluent_signature_items)
+            }
+            return PDDLFunction(name=function_name, signature=fluent_signature)
+
         possible_objects = {**self.problem.objects, **self.partial_domain.constants}
         fluent_signature = {
             object_name: possible_objects[object_name].type for object_name in fluent_signature_items
         }
         for grounded_param_type, lifted_param_type in zip(fluent_signature.values(),
                                                           lifted_function.signature.values()):
             assert grounded_param_type.is_sub_type(lifted_param_type)
@@ -146,32 +157,71 @@
                 actions.append(ActionCall(name=NOP_ACTION, grounded_parameters=[]))
                 continue
 
             actions.append(self.parse_action_call([action_call_ast]))
 
         return actions
 
+
+    def deduce_problem_objects(
+            self, initial_state_expression: List[List[Union[str, List[str]]]]) -> Dict[str, PDDLObject]:
+        """Deduce the problem objects from the state.
+
+        :param initial_state_expression: the initial state expression that should contain predicates and functions that
+            can be used to deduce the problem objects from.
+        :return: the problem objects.
+        """
+        self.logger.info("Extracting the observation objects.")
+        observation_objects = {}
+        for expression in initial_state_expression:
+            if expression[0] == "=":  # This is an assignment of a grounded numeric fluent.
+                function_data = expression[1]
+                function_objects = function_data[1:]
+                lifted_function_signature = self.partial_domain.functions[function_data[0]].signature
+                for object_name, object_type in zip(function_objects, lifted_function_signature.values()):
+                    observation_objects[object_name] = PDDLObject(name=object_name, type=object_type)
+
+                continue
+
+            if expression[0] in self.partial_domain.predicates:
+                lifted_predicate_name = expression[0]
+                grounded_predicate_signature = expression[1:]
+                lifted_predicate_signature = self.partial_domain.predicates[lifted_predicate_name].signature
+                for object_name, object_type in zip(grounded_predicate_signature, lifted_predicate_signature.values()):
+                    observation_objects[object_name] = PDDLObject(name=object_name, type=object_type)
+
+                continue
+
+        return observation_objects
+
     def parse_trajectory(self, trajectory_file_path: Path,
                          executing_agents: List[str] = None) -> Union[Observation, MultiAgentObservation]:
         """Parse a trajectory and extracts the observed data into objects.
 
         :param trajectory_file_path: the path to the trajectory file.
         :param executing_agents: the list of agents that partake in the observation.
         :return: the observation extracted from the serialized trajectory.
         """
         self.logger.info("Starting to read the trajectory file!")
         tokenizer = self._read_trajectory_file(trajectory_file_path)
         observation_expression = tokenizer.parse()
         observation = MultiAgentObservation(
             executing_agents=executing_agents) if executing_agents is not None else Observation()
 
-        observation.add_problem_objects(self.problem.objects)
         self.logger.debug("Starting to generate the observation from the input trajectory.")
         for index in range(0, len(observation_expression) - 2, 2):
             macro_expression = observation_expression[index]
+            if macro_expression[0] == ":init":
+                if self.problem is not None:
+                    observation.add_problem_objects(self.problem.objects)
+
+                else:
+                    self.logger.debug("Parsing the initial state and extracting the objects from the state's data.")
+                    observation.add_problem_objects(self.deduce_problem_objects(macro_expression[1:]))
+
             if macro_expression[0] == ":init" or macro_expression[0] == ":state":
                 previous_state = self.parse_state(macro_expression[1:])
                 macro_expression = observation_expression[index + 1]
                 if macro_expression[0] == "operator:":
                     action_call = self.parse_action_call(macro_expression[1:])
 
                 elif macro_expression[0] == "operators:":
```

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/__init__.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/action_call.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/action_call.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/conditional_effect.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/conditional_effect.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounded_effect.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/grounded_effect.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounded_precondition.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/grounded_precondition.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,17 @@
                 if isinstance(sub_condition, GroundedPredicate):
                     is_applicable = self._validate_predicates_hold(sub_condition, is_applicable, condition, state)
 
                 elif isinstance(sub_condition, NumericalExpressionTree):
                     is_applicable = self._validate_numeric_expression_hold(sub_condition, is_applicable, condition,
                                                                            state)
 
+                elif isinstance(sub_condition, Precondition):
+                    is_applicable = self._is_condition_applicable(sub_condition, state, problem_objects)
+
         return is_applicable
 
     def _is_condition_applicable(self, preconditions: Precondition, state: State,
                                  problem_objects: Optional[Dict[str, PDDLObject]] = None) -> bool:
         """Validate if the given condition is applicable in the given state.
 
         :param preconditions: the condition to validate.
```

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/grounding_utils.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/grounding_utils.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/numerical_expression.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/numerical_expression.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/observation.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/observation.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_action.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_action.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_domain.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_domain.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_function.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_function.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_operator.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         :param state: the state prior to the action's execution.
         :return: whether the action is applicable.
         """
         if not self.grounded:
             self.ground()
 
-        return self.grounded_preconditions.is_applicable(state)
+        return self.grounded_preconditions.is_applicable(state, self.problem_objects)
 
     def apply(self, previous_state: State, allow_inapplicable_actions: bool = False) -> State:
         """Applies an action on a state and changes the state according to the action's effects.
 
         :param previous_state: the state in which the operator is being applied on.
         :param allow_inapplicable_actions: whether to allow inapplicable actions to be applied.
         :return: the new state that was created by applying the operator.
```

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_precondition.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_precondition.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,25 +97,25 @@
     def add_condition(self,
                       condition: Union["Precondition", Predicate, GroundedPredicate, NumericalExpressionTree]) -> None:
         """Add a condition to the precondition.
 
         :param condition: the condition to add.
         """
         if isinstance(condition, (Predicate, GroundedPredicate)):
-            current_predicates = [cond.untyped_representation for cond in self.__iter__() if
+            current_predicates = [cond.untyped_representation for _, cond in self.__iter__() if
                                   isinstance(cond, Predicate)]
             if condition.untyped_representation not in current_predicates:
                 self.operands.add(condition)
         elif isinstance(condition, NumericalExpressionTree):
-            current_expressions = [cond.to_pddl() for cond in self.__iter__() if
+            current_expressions = [cond.to_pddl() for _, cond in self.__iter__() if
                                    isinstance(cond, NumericalExpressionTree)]
             if condition.to_pddl() not in current_expressions:
                 self.operands.add(condition)
         else:
-            current_compound_conditions = [str(cond) for cond in self.__iter__() if isinstance(cond, Precondition)]
+            current_compound_conditions = [str(cond) for _, cond in self.__iter__() if isinstance(cond, Precondition)]
             if str(condition) not in current_compound_conditions:
                 self.operands.add(condition)
 
     @staticmethod
     def _remove_condition(
             condition_to_remove: Union["Precondition", Predicate, GroundedPredicate, NumericalExpressionTree],
             searched_condition: "Precondition") -> bool:
@@ -163,18 +163,18 @@
 
     def __init__(self, quantified_parameter: str, quantified_type: PDDLType, binary_operator: str = "and"):
         self.quantified_parameter = quantified_parameter
         self.quantified_type = quantified_type
         super().__init__(binary_operator)
 
     def __str__(self):
-        internal_condition_string = super()._print_self()
-        if internal_condition_string == "(and ))":  # there are no internal conditions at all
+        if len(self.operands) == 0:
             return ""
 
+        internal_condition_string = super()._print_self()
         return f"(forall ({self.quantified_parameter} - {self.quantified_type.name})" \
                f"\n\t{internal_condition_string})"
 
     def __hash__(self) -> int:
         return hash(str(self))
 
     def __eq__(self, other: "UniversalPrecondition") -> bool:
```

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_predicate.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_predicate.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_problem.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_problem.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_state.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_state.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/models/pddl_type.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/models/pddl_type.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/common.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/common.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/multi_agent_domain_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/multi_agent_problem_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/multi_agent_trajectory_exporter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/multi_agent/single_agent_plan_converter.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/multi_agent/single_agent_plan_converter.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/counters_generator.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/counters_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/depots_generator.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/depots_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/farmland_generator.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/farmland_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/plant_watering_generator.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/plant_watering_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/sailing_generator.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/sailing_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/settlers_problem_generator.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/settlers_problem_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser/problem_generators/zenotravel_generator.py` & `pddl-plus-parser-3.4.0/pddl_plus_parser/problem_generators/zenotravel_generator.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/PKG-INFO` & `pddl-plus-parser-3.4.0/pddl_plus_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-plus-parser
-Version: 3.3.9
+Version: 3.4.0
 Summary: Parser of PDDL+ domains and problems for learning purposes
 Author: Argaman Mordoch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PDDL Plus Parser
```

### Comparing `pddl-plus-parser-3.3.9/pddl_plus_parser.egg-info/SOURCES.txt` & `pddl-plus-parser-3.4.0/pddl_plus_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/exporters_tests/numeric_trajectory_exporter_test.py` & `pddl-plus-parser-3.4.0/tests/exporters_tests/numeric_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/consts.py` & `pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/consts.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 
 PLANT_WATERING_DOMAIN = Path(CWD, "plant_watering_domain.pddl")
 
 WOODWORKING_COMBINED_DOMAIN_PATH = Path(CWD) / "woodworking_combined_domain.pddl"
 WOODWORKING_COMBINED_PROBLEM_PATH = Path(CWD) / "woodworking_combined_problem.pddl"
 WOODWORKING_COMBINED_TRAJECTORY_PATH = Path(CWD) / "ma_woodworking_trajectory.trajectory"
 
+MICONIC_LEARNED_DOMAIN_PATH = Path(CWD) / "learned_domain_miconic.pddl"
+
+STARCRAFT_DOMAIN_PATH = Path(CWD) / "starcraft_domain.pddl"
+STARCRAFT_TRAJECTORY_PATH = Path(CWD) / "starcraft_trajectory.trajectory"
+
+
 UMT2_DOMAIN_PATH = Path(CWD) / "UMT2_domain.pddl"
 
 
 TEST_PREDICATES_FOR_CONDITIONAL_DOMAIN = """((on ?c1 - card ?c2 - cardposition)
     (clear ?c - cardposition)
     (in-play ?c - card)
     (current-deal ?d - deal)
```

### Comparing `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/domain_parser_test.py` & `pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/domain_parser_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pytest import fixture, raises, fail
 
 from pddl_plus_parser.lisp_parsers import DomainParser, PDDLTokenizer
 from pddl_plus_parser.models import PDDLType, Predicate, Action, CompoundPrecondition
 from tests.lisp_parsers_tests.consts import TEST_PARSING_FILE_PATH, TEST_WOODWORKING_DOMAIN_PATH, \
     TEST_NUMERIC_DEPOT_DOMAIN_PATH, PLANT_WATERING_DOMAIN, TEST_CONSTANTS_FOR_CONDITIONAL_DOMAIN, \
     TEST_TYPES_FOR_CONDITIONAL_DOMAIN, TEST_PREDICATES_FOR_CONDITIONAL_DOMAIN, SPIDER_DOMAIN_PATH, \
-    TYPES_FOR_UNIVERSAL_CONDITIONAL_DOMAIN, TEST_PREDICATES_FOR_UNIVERSAL_QUANTIFIER_DOMAIN, UMT2_DOMAIN_PATH
+    TYPES_FOR_UNIVERSAL_CONDITIONAL_DOMAIN, TEST_PREDICATES_FOR_UNIVERSAL_QUANTIFIER_DOMAIN, UMT2_DOMAIN_PATH, \
+    MICONIC_LEARNED_DOMAIN_PATH
 
 test_types_with_no_parent = ['acolour', 'awood', 'woodobj', 'machine', 'surface', 'treatmentstatus', 'aboardsize',
                              'apartsize']
 
 nested_types = ['acolour', 'awood', 'woodobj', 'machine', 'surface', 'treatmentstatus', 'aboardsize', 'apartsize',
                 '-', 'object', 'highspeed-saw', 'saw', 'glazer', 'grinder', 'immersion-varnisher', 'planer',
                 'spray-varnisher', '-', 'machine', 'board', 'part', '-', 'woodobj']
@@ -746,7 +747,18 @@
         for action in domain.actions.values():
             print(action.name)
             print(action.preconditions)
             print()
     except Exception:
         fail("Parsing domain with nested action schema failed.")
 
+
+def test_parse_domain_with_nested_universal_preconditions_does_not_fail():
+    domain_parser = DomainParser(MICONIC_LEARNED_DOMAIN_PATH)
+    try:
+        domain = domain_parser.parse_domain()
+        for action in domain.actions.values():
+            print(action.name)
+            print(action.preconditions)
+            print()
+    except Exception:
+        fail("Parsing domain with nested action schema failed.")
```

### Comparing `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/pddl_tokenizer_test.py` & `pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/pddl_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/problem_parser_test.py` & `pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/problem_parser_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/lisp_parsers_tests/trajectory_parser_test.py` & `pddl-plus-parser-3.4.0/tests/lisp_parsers_tests/trajectory_parser_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pddl_plus_parser.lisp_parsers import DomainParser, ProblemParser, TrajectoryParser
 from pddl_plus_parser.models import Domain, Problem, MultiAgentObservation
 from tests.lisp_parsers_tests.consts import TEST_NUMERIC_DEPOT_DOMAIN, TEST_NUMERIC_DEPOT_PROBLEM, \
     TEST_NUMERIC_DEPOT_TRAJECTORY, FARMLAND_NUMERIC_DOMAIN, FARMLAND_NUMERIC_PROBLEM, FARMLAND_NUMERIC_TRAJECTORY, \
     WOODWORKING_COMBINED_DOMAIN_PATH, WOODWORKING_COMBINED_PROBLEM_PATH, WOODWORKING_COMBINED_TRAJECTORY_PATH, \
     DEPOT_MA_PROBLEM_PATH, DEPOT_MA_DOMAIN_PATH, DEPOT_MA_TRAJECTORY_PATH, LOGISTICS_MA_DOMAIN_PATH, \
-    LOGISTICS_MA_PROBLEM_PATH, LOGISTICS_MA_TRAJECTORY_PATH
+    LOGISTICS_MA_PROBLEM_PATH, LOGISTICS_MA_TRAJECTORY_PATH, STARCRAFT_DOMAIN_PATH, STARCRAFT_TRAJECTORY_PATH
 from tests.multi_agent_tests.consts import WOODWORKING_AGENT_NAMES
 
 
 @fixture()
 def domain() -> Domain:
     domain_parser = DomainParser(TEST_NUMERIC_DEPOT_DOMAIN, partial_parsing=True)
     return domain_parser.parse_domain()
@@ -84,14 +84,25 @@
 
 
 @fixture()
 def ma_logistics_trajectory_parser(ma_logistics_domain: Domain, ma_logistics_problem: Problem) -> TrajectoryParser:
     return TrajectoryParser(ma_logistics_domain, ma_logistics_problem)
 
 
+@fixture()
+def starcraft_domain() -> Domain:
+    domain_parser = DomainParser(STARCRAFT_DOMAIN_PATH, partial_parsing=True)
+    return domain_parser.parse_domain()
+
+
+@fixture()
+def starcraft_trajectory_parser(starcraft_domain: Domain) -> TrajectoryParser:
+    return TrajectoryParser(starcraft_domain)
+
+
 def test_parse_trajectory(trajectory_parser: TrajectoryParser):
     observation = trajectory_parser.parse_trajectory(TEST_NUMERIC_DEPOT_TRAJECTORY)
     assert len(observation.components) == 19
 
 
 def test_parse_farmland_trajectory(farmland_trajectory_parser: TrajectoryParser):
     observation = farmland_trajectory_parser.parse_trajectory(FARMLAND_NUMERIC_TRAJECTORY)
@@ -118,22 +129,41 @@
             for predicate in predicate_set:
                 assert predicate.is_positive
 
 
 def test_parse_ma_combined_trajectory_parse_joint_actions_correctly_and_does_not_remove_actions_from_joint_actions(
         ma_logistics_trajectory_parser: TrajectoryParser):
     observation: MultiAgentObservation = ma_logistics_trajectory_parser.parse_trajectory(
-        LOGISTICS_MA_TRAJECTORY_PATH, executing_agents=["apn1", "apn2", "tru1", "tru2", "tru3","tru4", "tru5"])
+        LOGISTICS_MA_TRAJECTORY_PATH, executing_agents=["apn1", "apn2", "tru1", "tru2", "tru3", "tru4", "tru5"])
     for component in observation.components:
         joint_actions = component.grounded_joint_action
         if joint_actions.action_count == 1:
             assert "dummy" not in str(joint_actions)
 
 
 def test_parse_depot_combined_trajectory(ma_depot_trajectory_parser: TrajectoryParser):
     observation = ma_depot_trajectory_parser.parse_trajectory(DEPOT_MA_TRAJECTORY_PATH,
                                                               executing_agents=["depot0", "distributor0",
                                                                                 "distributor1",
                                                                                 "distributor2", "distributor3",
                                                                                 "truck0",
                                                                                 "truck1", "truck2", "truck3"])
     assert "(clear pallet6)" not in observation.components[0].next_state.serialize()
+
+
+def test_parse_starcraft_ma_trajectory_without_problem_objects_returns_correct_objects(
+        starcraft_trajectory_parser: TrajectoryParser):
+    observation = starcraft_trajectory_parser.parse_trajectory(
+        STARCRAFT_TRAJECTORY_PATH, executing_agents=["agent0", "agent1", "agent2", "agent3", "agent4"])
+    assert observation.grounded_objects is not None
+    assert len(observation.grounded_objects) == 5
+    assert len(observation.components) == 40
+
+
+def test_parse_depot_trajectory_with_trajectory_parser_without_problem_returns_correct_trajectory_data(
+        domain: Domain):
+    depot_trajectory_parser = TrajectoryParser(domain)
+    observation = depot_trajectory_parser.parse_trajectory(TEST_NUMERIC_DEPOT_TRAJECTORY)
+    assert observation.grounded_objects is not None
+    assert len(observation.grounded_objects) == 15
+    assert len(observation.components) == 19
+    print(observation.grounded_objects.keys())
```

### Comparing `pddl-plus-parser-3.3.9/tests/models_tests/grounded_effect_test.py` & `pddl-plus-parser-3.4.0/tests/models_tests/grounded_effect_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/models_tests/grounded_precondition_test.py` & `pddl-plus-parser-3.4.0/tests/models_tests/grounded_precondition_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Module test for the grounded precondition class."""
 from typing import Dict, Set, List
 
 from pytest import fixture, fail
 
-from pddl_plus_parser.lisp_parsers import DomainParser, ProblemParser, PDDLTokenizer
+from pddl_plus_parser.lisp_parsers import DomainParser, ProblemParser, PDDLTokenizer, TrajectoryParser
 from pddl_plus_parser.models import Domain, Action, GroundedPredicate, PDDLFunction, State, Problem, Precondition, \
-    NumericalExpressionTree
+    NumericalExpressionTree, Observation
 from pddl_plus_parser.models.grounded_precondition import GroundedPrecondition
 from tests.lisp_parsers_tests.consts import SPIDER_PROBLEM_PATH
 from tests.models_tests.consts import TEST_HARD_NUMERIC_DOMAIN, TEST_NUMERIC_DOMAIN, SPIDER_DOMAIN_PATH, \
-    NURIKABE_DOMAIN_PATH, NURIKABE_PROBLEM_PATH
+    NURIKABE_DOMAIN_PATH, NURIKABE_PROBLEM_PATH, MICONIC_NESTED_DOMAIN_PATH, MICONIC_NESTED_PROBLEM_PATH, \
+    MICONIC_DOMAIN_PATH, MICONIC_TRAJECTORY_PATH
 
 TEST_LIFTED_SIGNATURE_ITEMS = ["?s", "?d", "?i", "?m"]
 TEST_GROUNDED_ACTION_CALL = ["s1", "test_direction", "test_instrument", "test_mode"]
 
 AGRICOLA_LIFTED_SIGNATURE_ITEMS = ["?w1", "?w2", "?wmax", "?r", "?i1", "?i2"]
 AGRICOLA_GROUNDED_ACTION_CALL = ["noworker", "w1", "w2", "round1", "n1", "n2"]
 
@@ -44,24 +45,41 @@
 @fixture()
 def nurikabe_domain() -> Domain:
     domain_parser = DomainParser(NURIKABE_DOMAIN_PATH)
     return domain_parser.parse_domain()
 
 
 @fixture()
+def miconic_nested_domain() -> Domain:
+    domain_parser = DomainParser(MICONIC_NESTED_DOMAIN_PATH)
+    return domain_parser.parse_domain()
+
+
+@fixture()
+def miconic_domain() -> Domain:
+    domain_parser = DomainParser(MICONIC_DOMAIN_PATH)
+    return domain_parser.parse_domain()
+
+
+@fixture()
 def spider_problem(spider_domain: Domain) -> Problem:
     return ProblemParser(problem_path=SPIDER_PROBLEM_PATH, domain=spider_domain).parse_problem()
 
 
 @fixture()
 def nurikabe_problem(nurikabe_domain: Domain) -> Problem:
     return ProblemParser(problem_path=NURIKABE_PROBLEM_PATH, domain=nurikabe_domain).parse_problem()
 
 
 @fixture()
+def miconic_nested_problem(miconic_domain: Domain) -> Problem:
+    return ProblemParser(problem_path=MICONIC_NESTED_PROBLEM_PATH, domain=miconic_domain).parse_problem()
+
+
+@fixture()
 def take_image_numeric_action(satellite_domain: Domain) -> Action:
     return satellite_domain.actions["take_image"]
 
 
 @fixture()
 def agricola_numeric_action(agricola_domain: Domain) -> Action:
     return agricola_domain.actions["take_food"]
@@ -84,14 +102,19 @@
 
 @fixture()
 def nurikabe_conditional_action(nurikabe_domain: Domain) -> Action:
     return nurikabe_domain.actions["move-painting"]
 
 
 @fixture()
+def miconic_stop_action(miconic_nested_domain: Domain) -> Action:
+    return miconic_nested_domain.actions["stop"]
+
+
+@fixture()
 def satellite_action_precondition(satellite_domain: Domain, take_image_numeric_action: Action) -> GroundedPrecondition:
     return GroundedPrecondition(take_image_numeric_action.preconditions, satellite_domain, take_image_numeric_action)
 
 
 @fixture()
 def agricola_action_precondition(agricola_domain: Domain, agricola_numeric_action: Action) -> GroundedPrecondition:
     return GroundedPrecondition(agricola_numeric_action.preconditions, agricola_domain, agricola_numeric_action)
@@ -99,14 +122,20 @@
 
 @fixture()
 def spider_action_precondition(spider_domain: Domain, spider_conditional_action: Action) -> GroundedPrecondition:
     return GroundedPrecondition(spider_conditional_action.preconditions, spider_domain, spider_conditional_action)
 
 
 @fixture()
+def miconic_stop_action_precondition(miconic_nested_domain: Domain,
+                                     miconic_stop_action: Action) -> GroundedPrecondition:
+    return GroundedPrecondition(miconic_stop_action.preconditions, miconic_nested_domain, miconic_stop_action)
+
+
+@fixture()
 def complete_state_predicates(satellite_domain: Domain) -> Dict[str, Set[GroundedPredicate]]:
     calibrated_predicate = satellite_domain.predicates["calibrated"]
     on_board_predicate = satellite_domain.predicates["on_board"]
     supports_predicate = satellite_domain.predicates["supports"]
     power_on_predicate = satellite_domain.predicates["power_on"]
     pointing_predicate = satellite_domain.predicates["pointing"]
     return {
@@ -170,14 +199,19 @@
     numeric_state_variables[data_function.untyped_representation].set_value(5.3)
     return State(predicates=complete_state_predicates, fluents={
         **numeric_state_variables,
         data_stored_function.untyped_representation: data_stored_function
     })
 
 
+@fixture()
+def miconic_observation(miconic_domain: Domain, miconic_nested_problem: Problem) -> Observation:
+    return TrajectoryParser(miconic_domain, miconic_nested_problem).parse_trajectory(MICONIC_TRAJECTORY_PATH)
+
+
 def test_ground_equality_objects_returns_correct_grounded_objects(satellite_action_precondition: GroundedPrecondition):
     equality_precondition = {("?size_before", "?size_after")}
     parameter_map = {"?size_before": "size1", "?size_after": "size2"}
     grounded_objects = satellite_action_precondition._ground_equality_objects(equality_precondition, parameter_map)
     assert grounded_objects == {("size1", "size2")}
 
 
@@ -481,7 +515,17 @@
     }
     grounded_precondition.ground_preconditions(test_parameter_map)
     try:
         grounded_precondition.is_applicable(valid_previous_state)
 
     except Exception:
         fail()
+
+
+def test_is_applicable_returns_true_when_the_action_has_nested_universal_precondition_but_is_logically_the_same_as_the_original_action(
+        miconic_nested_domain: Domain, miconic_nested_problem: Problem,
+        miconic_stop_action_precondition: GroundedPrecondition, miconic_observation: Observation):
+    miconic_stop_action_comp = miconic_observation.components[1]
+    miconic_previous_state = miconic_stop_action_comp.previous_state
+    test_parameters_map = {"?f": "f1"}
+    miconic_stop_action_precondition.ground_preconditions(test_parameters_map)
+    assert miconic_stop_action_precondition.is_applicable(miconic_previous_state)
```

### Comparing `pddl-plus-parser-3.3.9/tests/models_tests/numerical_expression_test.py` & `pddl-plus-parser-3.4.0/tests/models_tests/numerical_expression_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/models_tests/operator_test.py` & `pddl-plus-parser-3.4.0/tests/models_tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/models_tests/pddl_function_test.py` & `pddl-plus-parser-3.4.0/tests/models_tests/pddl_function_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/models_tests/pddl_precondition_test.py` & `pddl-plus-parser-3.4.0/tests/models_tests/pddl_precondition_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/multi_agent_tests/consts.py` & `pddl-plus-parser-3.4.0/tests/multi_agent_tests/consts.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_domain_converter_test.py` & `pddl-plus-parser-3.4.0/tests/multi_agent_tests/multi_agent_domain_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_problem_converter_test.py` & `pddl-plus-parser-3.4.0/tests/multi_agent_tests/multi_agent_problem_converter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py` & `pddl-plus-parser-3.4.0/tests/multi_agent_tests/multi_agent_trajectory_exporter_test.py`

 * *Files identical despite different names*

### Comparing `pddl-plus-parser-3.3.9/tests/multi_agent_tests/single_agent_plan_converter_test.py` & `pddl-plus-parser-3.4.0/tests/multi_agent_tests/single_agent_plan_converter_test.py`

 * *Files identical despite different names*


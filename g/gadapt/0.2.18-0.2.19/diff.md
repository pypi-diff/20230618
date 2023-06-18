# Comparing `tmp/gadapt-0.2.18.tar.gz` & `tmp/gadapt-0.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.18.tar", last modified: Sun Jun 18 17:40:29 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.19.tar", last modified: Sun Jun 18 18:17:44 2023, max compression
```

## Comparing `gadapt-0.2.18.tar` & `gadapt-0.2.19.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.664468 gadapt-0.2.18/
--rw-rw-rw-   0        0        0    21892 2023-06-18 17:40:29.665469 gadapt-0.2.18/PKG-INFO
--rw-rw-rw-   0        0        0    19530 2023-06-18 17:34:09.000000 gadapt-0.2.18/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.382450 gadapt-0.2.18/gadapt/
--rw-rw-rw-   0        0        0       34 2023-06-18 17:04:48.000000 gadapt-0.2.18/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.415451 gadapt-0.2.18/gadapt/cost_finding/
--rw-rw-rw-   0        0        0       64 2023-06-18 16:13:43.000000 gadapt-0.2.18/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      783 2023-06-03 19:52:53.000000 gadapt-0.2.18/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2169 2023-06-03 19:53:08.000000 gadapt-0.2.18/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.418951 gadapt-0.2.18/gadapt/crossover/
--rw-rw-rw-   0        0        0       33 2023-06-18 16:13:59.000000 gadapt-0.2.18/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     7080 2023-06-03 19:52:23.000000 gadapt-0.2.18/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1300 2023-06-03 19:52:35.000000 gadapt-0.2.18/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.421952 gadapt-0.2.18/gadapt/execution/
--rw-rw-rw-   0        0        0       48 2023-06-18 16:27:33.000000 gadapt-0.2.18/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3302 2023-06-03 20:49:46.000000 gadapt-0.2.18/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.428452 gadapt-0.2.18/gadapt/exit_check/
--rw-rw-rw-   0        0        0       56 2023-06-18 16:29:21.000000 gadapt-0.2.18/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      379 2023-06-03 19:51:29.000000 gadapt-0.2.18/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1113 2023-06-03 19:50:16.000000 gadapt-0.2.18/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      365 2023-06-03 19:51:48.000000 gadapt-0.2.18/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      449 2023-06-03 19:51:58.000000 gadapt-0.2.18/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.431454 gadapt-0.2.18/gadapt/factory/
--rw-rw-rw-   0        0        0       74 2023-06-18 16:31:20.000000 gadapt-0.2.18/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0    10398 2023-06-18 16:54:21.000000 gadapt-0.2.18/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0    26501 2023-06-03 20:44:22.000000 gadapt-0.2.18/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.433952 gadapt-0.2.18/gadapt/ga_logging/
--rw-rw-rw-   0        0        0       26 2023-06-18 16:31:46.000000 gadapt-0.2.18/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2188 2023-06-03 19:19:12.000000 gadapt-0.2.18/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.572463 gadapt-0.2.18/gadapt/ga_model/
--rw-rw-rw-   0        0        0       33 2023-06-18 16:32:02.000000 gadapt-0.2.18/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     8611 2023-06-03 20:28:37.000000 gadapt-0.2.18/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      723 2023-06-03 20:31:30.000000 gadapt-0.2.18/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     6427 2023-06-03 20:15:33.000000 gadapt-0.2.18/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     2137 2023-06-03 20:09:38.000000 gadapt-0.2.18/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1472 2023-06-03 20:05:45.000000 gadapt-0.2.18/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2704 2023-06-03 20:06:52.000000 gadapt-0.2.18/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.18/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    12730 2023-06-03 20:00:59.000000 gadapt-0.2.18/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      881 2023-06-03 20:04:36.000000 gadapt-0.2.18/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.578463 gadapt-0.2.18/gadapt/gene_combination/
--rw-rw-rw-   0        0        0       91 2023-06-18 16:44:14.000000 gadapt-0.2.18/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      367 2023-06-03 19:46:03.000000 gadapt-0.2.18/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0     1102 2023-06-18 16:36:56.000000 gadapt-0.2.18/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.579963 gadapt-0.2.18/gadapt/immigration/
--rw-rw-rw-   0        0        0       54 2023-06-18 16:45:34.000000 gadapt-0.2.18/gadapt/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.583464 gadapt-0.2.18/gadapt/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0       69 2023-06-18 16:45:47.000000 gadapt-0.2.18/gadapt/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      676 2023-06-03 19:42:17.000000 gadapt-0.2.18/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      407 2023-06-03 19:43:54.000000 gadapt-0.2.18/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.587964 gadapt-0.2.18/gadapt/immigration/population_immigration/
--rw-rw-rw-   0        0        0       79 2023-06-18 16:46:42.000000 gadapt-0.2.18/gadapt/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      239 2023-06-03 19:44:12.000000 gadapt-0.2.18/gadapt/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0      993 2023-06-03 19:45:35.000000 gadapt-0.2.18/gadapt/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.589464 gadapt-0.2.18/gadapt/mutation/
--rw-rw-rw-   0        0        0       38 2023-06-18 16:47:20.000000 gadapt-0.2.18/gadapt/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.610465 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0       42 2023-06-18 16:47:50.000000 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      956 2023-06-03 19:39:26.000000 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     3031 2023-06-03 19:37:17.000000 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0     1009 2023-06-03 19:37:53.000000 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.616465 gadapt-0.2.18/gadapt/mutation/population_mutation/
--rw-rw-rw-   0        0        0       51 2023-06-18 17:07:55.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-06-03 19:39:16.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1365 2023-06-03 19:40:00.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/composed_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.619466 gadapt-0.2.18/gadapt/mutation/population_mutation/cost_diversity/
--rw-rw-rw-   0        0        0       56 2023-06-18 17:07:58.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-06-03 19:41:44.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     2045 2023-06-03 19:40:53.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1130 2023-06-03 19:41:22.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.630467 gadapt-0.2.18/gadapt/parent_selection/
--rw-rw-rw-   0        0        0       37 2023-06-18 16:59:38.000000 gadapt-0.2.18/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      395 2023-06-03 19:27:41.000000 gadapt-0.2.18/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0     1172 2023-06-03 19:31:52.000000 gadapt-0.2.18/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.641466 gadapt-0.2.18/gadapt/sampling/
--rw-rw-rw-   0        0        0      128 2023-06-18 17:00:39.000000 gadapt-0.2.18/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      793 2023-06-03 19:32:22.000000 gadapt-0.2.18/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      534 2023-06-03 19:33:37.000000 gadapt-0.2.18/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      512 2023-06-03 19:33:50.000000 gadapt-0.2.18/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1954 2023-06-03 19:34:36.000000 gadapt-0.2.18/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2717 2023-06-03 19:35:01.000000 gadapt-0.2.18/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.643968 gadapt-0.2.18/gadapt/string_operation/
--rw-rw-rw-   0        0        0       90 2023-06-18 17:02:51.000000 gadapt-0.2.18/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-06-03 20:30:52.000000 gadapt-0.2.18/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.646968 gadapt-0.2.18/gadapt/utils/
--rw-rw-rw-   0        0        0      281 2023-06-03 20:30:21.000000 gadapt-0.2.18/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0       35 2023-06-18 17:03:05.000000 gadapt-0.2.18/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1313 2023-06-03 20:30:37.000000 gadapt-0.2.18/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.650468 gadapt-0.2.18/gadapt/validation/
--rw-rw-rw-   0        0        0       31 2023-06-18 17:03:27.000000 gadapt-0.2.18/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      846 2023-06-03 20:29:38.000000 gadapt-0.2.18/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    17474 2023-06-03 20:29:54.000000 gadapt-0.2.18/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.662969 gadapt-0.2.18/gadapt/variable_update/
--rw-rw-rw-   0        0        0       53 2023-06-18 17:04:05.000000 gadapt-0.2.18/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      234 2023-06-03 20:28:58.000000 gadapt-0.2.18/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2052 2023-06-03 20:29:16.000000 gadapt-0.2.18/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.412450 gadapt-0.2.18/gadapt.egg-info/
--rw-rw-rw-   0        0        0    21892 2023-06-18 17:40:29.000000 gadapt-0.2.18/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-06-18 17:40:29.000000 gadapt-0.2.18/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 17:40:29.000000 gadapt-0.2.18/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 17:40:29.000000 gadapt-0.2.18/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-18 17:40:29.674470 gadapt-0.2.18/setup.cfg
--rw-rw-rw-   0        0        0      465 2023-06-18 17:38:21.000000 gadapt-0.2.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.296217 gadapt-0.2.19/
+-rw-rw-rw-   0        0        0    22014 2023-06-18 18:17:44.296716 gadapt-0.2.19/PKG-INFO
+-rw-rw-rw-   0        0        0    19628 2023-06-18 18:14:25.000000 gadapt-0.2.19/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.180213 gadapt-0.2.19/gadapt/
+-rw-rw-rw-   0        0        0       34 2023-06-18 17:04:48.000000 gadapt-0.2.19/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.209214 gadapt-0.2.19/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0       64 2023-06-18 16:13:43.000000 gadapt-0.2.19/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      783 2023-06-03 19:52:53.000000 gadapt-0.2.19/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2169 2023-06-03 19:53:08.000000 gadapt-0.2.19/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.213214 gadapt-0.2.19/gadapt/crossover/
+-rw-rw-rw-   0        0        0       33 2023-06-18 16:13:59.000000 gadapt-0.2.19/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7080 2023-06-03 19:52:23.000000 gadapt-0.2.19/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1300 2023-06-03 19:52:35.000000 gadapt-0.2.19/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.217214 gadapt-0.2.19/gadapt/execution/
+-rw-rw-rw-   0        0        0       48 2023-06-18 16:27:33.000000 gadapt-0.2.19/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3302 2023-06-03 20:49:46.000000 gadapt-0.2.19/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.223213 gadapt-0.2.19/gadapt/exit_check/
+-rw-rw-rw-   0        0        0       56 2023-06-18 16:29:21.000000 gadapt-0.2.19/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      379 2023-06-03 19:51:29.000000 gadapt-0.2.19/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1113 2023-06-03 19:50:16.000000 gadapt-0.2.19/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      365 2023-06-03 19:51:48.000000 gadapt-0.2.19/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      449 2023-06-03 19:51:58.000000 gadapt-0.2.19/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.225715 gadapt-0.2.19/gadapt/factory/
+-rw-rw-rw-   0        0        0       74 2023-06-18 16:31:20.000000 gadapt-0.2.19/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0    10398 2023-06-18 16:54:21.000000 gadapt-0.2.19/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0    26501 2023-06-03 20:44:22.000000 gadapt-0.2.19/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.228714 gadapt-0.2.19/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0       26 2023-06-18 16:31:46.000000 gadapt-0.2.19/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-06-03 19:19:12.000000 gadapt-0.2.19/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.241214 gadapt-0.2.19/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       33 2023-06-18 16:32:02.000000 gadapt-0.2.19/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     8611 2023-06-03 20:28:37.000000 gadapt-0.2.19/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      723 2023-06-03 20:31:30.000000 gadapt-0.2.19/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     6427 2023-06-03 20:15:33.000000 gadapt-0.2.19/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     2137 2023-06-03 20:09:38.000000 gadapt-0.2.19/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1472 2023-06-03 20:05:45.000000 gadapt-0.2.19/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2704 2023-06-03 20:06:52.000000 gadapt-0.2.19/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.19/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    12730 2023-06-03 20:00:59.000000 gadapt-0.2.19/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      881 2023-06-03 20:04:36.000000 gadapt-0.2.19/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.245215 gadapt-0.2.19/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0       91 2023-06-18 16:44:14.000000 gadapt-0.2.19/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      367 2023-06-03 19:46:03.000000 gadapt-0.2.19/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0     1102 2023-06-18 16:36:56.000000 gadapt-0.2.19/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.247214 gadapt-0.2.19/gadapt/immigration/
+-rw-rw-rw-   0        0        0       54 2023-06-18 16:45:34.000000 gadapt-0.2.19/gadapt/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.250214 gadapt-0.2.19/gadapt/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0       69 2023-06-18 16:45:47.000000 gadapt-0.2.19/gadapt/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-06-03 19:42:17.000000 gadapt-0.2.19/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      407 2023-06-03 19:43:54.000000 gadapt-0.2.19/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.254215 gadapt-0.2.19/gadapt/immigration/population_immigration/
+-rw-rw-rw-   0        0        0       79 2023-06-18 16:46:42.000000 gadapt-0.2.19/gadapt/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      239 2023-06-03 19:44:12.000000 gadapt-0.2.19/gadapt/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0      993 2023-06-03 19:45:35.000000 gadapt-0.2.19/gadapt/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.256215 gadapt-0.2.19/gadapt/mutation/
+-rw-rw-rw-   0        0        0       38 2023-06-18 16:47:20.000000 gadapt-0.2.19/gadapt/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.261715 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:47:50.000000 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      956 2023-06-03 19:39:26.000000 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     3031 2023-06-03 19:37:17.000000 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     1009 2023-06-03 19:37:53.000000 gadapt-0.2.19/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.267716 gadapt-0.2.19/gadapt/mutation/population_mutation/
+-rw-rw-rw-   0        0        0       51 2023-06-18 17:07:55.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-06-03 19:39:16.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/base_population_mutator.py
+-rw-rw-rw-   0        0        0     1365 2023-06-03 19:40:00.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/composed_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.271216 gadapt-0.2.19/gadapt/mutation/population_mutation/cost_diversity/
+-rw-rw-rw-   0        0        0       56 2023-06-18 17:07:58.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-06-03 19:41:44.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     2045 2023-06-03 19:40:53.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1130 2023-06-03 19:41:22.000000 gadapt-0.2.19/gadapt/mutation/population_mutation/random_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.275216 gadapt-0.2.19/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0       37 2023-06-18 16:59:38.000000 gadapt-0.2.19/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-03 19:27:41.000000 gadapt-0.2.19/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0     1172 2023-06-03 19:31:52.000000 gadapt-0.2.19/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.281216 gadapt-0.2.19/gadapt/sampling/
+-rw-rw-rw-   0        0        0      128 2023-06-18 17:00:39.000000 gadapt-0.2.19/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      793 2023-06-03 19:32:22.000000 gadapt-0.2.19/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      534 2023-06-03 19:33:37.000000 gadapt-0.2.19/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      512 2023-06-03 19:33:50.000000 gadapt-0.2.19/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1954 2023-06-03 19:34:36.000000 gadapt-0.2.19/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2717 2023-06-03 19:35:01.000000 gadapt-0.2.19/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.284215 gadapt-0.2.19/gadapt/string_operation/
+-rw-rw-rw-   0        0        0       90 2023-06-18 17:02:51.000000 gadapt-0.2.19/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-06-03 20:30:52.000000 gadapt-0.2.19/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.288215 gadapt-0.2.19/gadapt/utils/
+-rw-rw-rw-   0        0        0      281 2023-06-03 20:30:21.000000 gadapt-0.2.19/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       35 2023-06-18 17:03:05.000000 gadapt-0.2.19/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1313 2023-06-03 20:30:37.000000 gadapt-0.2.19/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.290717 gadapt-0.2.19/gadapt/validation/
+-rw-rw-rw-   0        0        0       31 2023-06-18 17:03:27.000000 gadapt-0.2.19/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      846 2023-06-03 20:29:38.000000 gadapt-0.2.19/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    17474 2023-06-03 20:29:54.000000 gadapt-0.2.19/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.295216 gadapt-0.2.19/gadapt/variable_update/
+-rw-rw-rw-   0        0        0       53 2023-06-18 17:04:05.000000 gadapt-0.2.19/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      234 2023-06-03 20:28:58.000000 gadapt-0.2.19/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2052 2023-06-03 20:29:16.000000 gadapt-0.2.19/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:17:44.202713 gadapt-0.2.19/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    22014 2023-06-18 18:17:44.000000 gadapt-0.2.19/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-06-18 18:17:44.000000 gadapt-0.2.19/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 18:17:44.000000 gadapt-0.2.19/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 18:17:44.000000 gadapt-0.2.19/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-18 18:17:44.298716 gadapt-0.2.19/setup.cfg
+-rw-rw-rw-   0        0        0      465 2023-06-18 17:45:52.000000 gadapt-0.2.19/setup.py
```

### Comparing `gadapt-0.2.18/PKG-INFO` & `gadapt-0.2.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.2.18
+Version: 0.2.19
 Summary: GAdapt: A Python Library for Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 License: UNKNOWN
 Description: # GAdapt: Self-Adaptive Genetic Algorithm
-        [GAdapt] (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
+        [GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
         
         # What innovations does GAdapt bring?
         **GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
         
         
         # Installation
         To install **GAdapt**, use **pip** with the following command:
         
         ```
         pip install gadapt
         ```
         
+        # Releases
+        Latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
+        
         # Source Code
-        The source code is stored on GitHub at the following address: [https://github.com/bpzoran/gadapt/] https://github.com/bpzoran/gadapt
+        The source code is stored at the GitHub repository: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
         
         # API Documentation
-        The API documentation can be found on the following address: [https://www.gadapt.com/api/] https://www.gadapt.com/api
+        The API documentation can be found at the following link: [GAdapt API Documentation](https://www.gadapt.com/api/)
         
         # Getting started
         The following example optimizes variable values for a complex trigonometric function.
         ```python
         from gadapt.ga import GA
         import math
```

### Comparing `gadapt-0.2.18/README.md` & `gadapt-0.2.19/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # GAdapt: Self-Adaptive Genetic Algorithm
-[GAdapt] (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
+[GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
 
 # What innovations does GAdapt bring?
 **GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
 
 
 # Installation
 To install **GAdapt**, use **pip** with the following command:
 
 ```
 pip install gadapt
 ```
 
+# Releases
+Latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
+
 # Source Code
-The source code is stored on GitHub at the following address: [https://github.com/bpzoran/gadapt/] https://github.com/bpzoran/gadapt
+The source code is stored at the GitHub repository: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
 
 # API Documentation
-The API documentation can be found on the following address: [https://www.gadapt.com/api/] https://www.gadapt.com/api
+The API documentation can be found at the following link: [GAdapt API Documentation](https://www.gadapt.com/api/)
 
 # Getting started
 The following example optimizes variable values for a complex trigonometric function.
 ```python
 from gadapt.ga import GA
 import math
```

### Comparing `gadapt-0.2.18/gadapt/cost_finding/base_cost_finder.py` & `gadapt-0.2.19/gadapt/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.19/gadapt/cost_finding/common_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/crossover/base_crossover.py` & `gadapt-0.2.19/gadapt/crossover/base_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.19/gadapt/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/execution/ga_executor.py` & `gadapt-0.2.19/gadapt/execution/ga_executor.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.19/gadapt/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/factory/ga_factory.py` & `gadapt-0.2.19/gadapt/factory/ga_factory.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga.py` & `gadapt-0.2.19/gadapt/ga.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.19/gadapt/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_model/chromosome.py` & `gadapt-0.2.19/gadapt/ga_model/chromosome.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_model/definitions.py` & `gadapt-0.2.19/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_model/ga_options.py` & `gadapt-0.2.19/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_model/ga_results.py` & `gadapt-0.2.19/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_model/gene.py` & `gadapt-0.2.19/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.19/gadapt/ga_model/genetic_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_model/population.py` & `gadapt-0.2.19/gadapt/ga_model/population.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.19/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.19/gadapt/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.2.19/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.2.19/gadapt/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py` & `gadapt-0.2.19/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py` & `gadapt-0.2.19/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.2.19/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.2.19/gadapt/mutation/population_mutation/base_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/mutation/population_mutation/composed_population_mutator.py` & `gadapt-0.2.19/gadapt/mutation/population_mutation/composed_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py` & `gadapt-0.2.19/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py` & `gadapt-0.2.19/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.2.19/gadapt/mutation/population_mutation/random_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.19/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/sampling/base_sampling.py` & `gadapt-0.2.19/gadapt/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/sampling/from_top_to_bottom_sampling.py` & `gadapt-0.2.19/gadapt/sampling/from_top_to_bottom_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/sampling/random_sampling.py` & `gadapt-0.2.19/gadapt/sampling/random_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.19/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.19/gadapt/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.19/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/utils/ga_utils.py` & `gadapt-0.2.19/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/validation/base_options_validator.py` & `gadapt-0.2.19/gadapt/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/validation/common_options_validator.py` & `gadapt-0.2.19/gadapt/validation/common_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.19/gadapt/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.18/gadapt.egg-info/PKG-INFO` & `gadapt-0.2.19/gadapt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.2.18
+Version: 0.2.19
 Summary: GAdapt: A Python Library for Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 License: UNKNOWN
 Description: # GAdapt: Self-Adaptive Genetic Algorithm
-        [GAdapt] (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
+        [GAdapt](https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
         
         # What innovations does GAdapt bring?
         **GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
         
         
         # Installation
         To install **GAdapt**, use **pip** with the following command:
         
         ```
         pip install gadapt
         ```
         
+        # Releases
+        Latest releases of GAdapt can be found at the PyPI repository: [GAdapt on PyPI](https://pypi.org/project/gadapt/)
+        
         # Source Code
-        The source code is stored on GitHub at the following address: [https://github.com/bpzoran/gadapt/] https://github.com/bpzoran/gadapt
+        The source code is stored at the GitHub repository: [GAdapt on GitHub](https://github.com/bpzoran/gadapt/)
         
         # API Documentation
-        The API documentation can be found on the following address: [https://www.gadapt.com/api/] https://www.gadapt.com/api
+        The API documentation can be found at the following link: [GAdapt API Documentation](https://www.gadapt.com/api/)
         
         # Getting started
         The following example optimizes variable values for a complex trigonometric function.
         ```python
         from gadapt.ga import GA
         import math
```

### Comparing `gadapt-0.2.18/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.19/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/gadapt-0.2.17.tar.gz` & `tmp/gadapt-0.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.17.tar", last modified: Wed May 31 14:56:47 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.18.tar", last modified: Sun Jun 18 17:40:29 2023, max compression
```

## Comparing `gadapt-0.2.17.tar` & `gadapt-0.2.18.tar`

### file list

```diff
@@ -1,107 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.302404 gadapt-0.2.17/
--rw-rw-rw-   0        0        0    21692 2023-05-31 14:56:47.302904 gadapt-0.2.17/PKG-INFO
--rw-rw-rw-   0        0        0    19354 2023-05-31 09:31:35.000000 gadapt-0.2.17/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.015403 gadapt-0.2.17/gadapt/
--rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.17/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.129404 gadapt-0.2.17/gadapt/cost_finding/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.17/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.17/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.166903 gadapt-0.2.17/gadapt/crossover/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.17/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     7034 2023-05-28 13:24:31.000000 gadapt-0.2.17/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.17/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.169404 gadapt-0.2.17/gadapt/execution/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.17/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3233 2023-05-27 11:13:47.000000 gadapt-0.2.17/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.177905 gadapt-0.2.17/gadapt/exit_check/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.17/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.17/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.17/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.17/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.180904 gadapt-0.2.17/gadapt/factory/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.17/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     9949 2023-05-28 13:25:45.000000 gadapt-0.2.17/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0     8920 2023-05-28 13:38:36.000000 gadapt-0.2.17/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.184903 gadapt-0.2.17/gadapt/ga_logging/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.17/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-05-24 07:42:21.000000 gadapt-0.2.17/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.202404 gadapt-0.2.17/gadapt/ga_model/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.17/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     6671 2023-05-28 13:24:31.000000 gadapt-0.2.17/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      680 2023-05-28 13:25:45.000000 gadapt-0.2.17/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     5248 2023-05-25 16:08:26.000000 gadapt-0.2.17/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     1398 2023-05-24 16:01:11.000000 gadapt-0.2.17/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.17/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    10169 2023-05-24 16:00:25.000000 gadapt-0.2.17/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.205903 gadapt-0.2.17/gadapt/gene_combination/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.17/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.17/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.208404 gadapt-0.2.17/gadapt/immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.17/gadapt/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.216904 gadapt-0.2.17/gadapt/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.17/gadapt/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.17/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.223403 gadapt-0.2.17/gadapt/immigration/population_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.17/gadapt/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.17/gadapt/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.224904 gadapt-0.2.17/gadapt/mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.17/gadapt/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.229904 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.17/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.237405 gadapt-0.2.17/gadapt/mutation/population_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/composed_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.239405 gadapt-0.2.17/gadapt/mutation/population_mutation/cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1976 2023-05-28 15:09:04.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.259404 gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
--rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.17/gadapt/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.268404 gadapt-0.2.17/gadapt/parent_selection/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.17/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.17/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.285905 gadapt-0.2.17/gadapt/sampling/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.17/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.17/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.17/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.17/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.17/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.17/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.288404 gadapt-0.2.17/gadapt/string_operation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.17/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.17/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.292405 gadapt-0.2.17/gadapt/utils/
--rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.17/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.17/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1272 2023-05-25 15:37:31.000000 gadapt-0.2.17/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.296905 gadapt-0.2.17/gadapt/validation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.17/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.17/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    17413 2023-05-28 13:25:45.000000 gadapt-0.2.17/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.301406 gadapt-0.2.17/gadapt/variable_update/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.17/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.17/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.17/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:56:47.123925 gadapt-0.2.17/gadapt.egg-info/
--rw-rw-rw-   0        0        0    21692 2023-05-31 14:56:46.000000 gadapt-0.2.17/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3460 2023-05-31 14:56:46.000000 gadapt-0.2.17/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:56:46.000000 gadapt-0.2.17/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 14:56:46.000000 gadapt-0.2.17/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-31 14:56:47.304905 gadapt-0.2.17/setup.cfg
--rw-rw-rw-   0        0        0      465 2023-05-31 09:29:04.000000 gadapt-0.2.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.664468 gadapt-0.2.18/
+-rw-rw-rw-   0        0        0    21892 2023-06-18 17:40:29.665469 gadapt-0.2.18/PKG-INFO
+-rw-rw-rw-   0        0        0    19530 2023-06-18 17:34:09.000000 gadapt-0.2.18/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.382450 gadapt-0.2.18/gadapt/
+-rw-rw-rw-   0        0        0       34 2023-06-18 17:04:48.000000 gadapt-0.2.18/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.415451 gadapt-0.2.18/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0       64 2023-06-18 16:13:43.000000 gadapt-0.2.18/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      783 2023-06-03 19:52:53.000000 gadapt-0.2.18/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2169 2023-06-03 19:53:08.000000 gadapt-0.2.18/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.418951 gadapt-0.2.18/gadapt/crossover/
+-rw-rw-rw-   0        0        0       33 2023-06-18 16:13:59.000000 gadapt-0.2.18/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7080 2023-06-03 19:52:23.000000 gadapt-0.2.18/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1300 2023-06-03 19:52:35.000000 gadapt-0.2.18/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.421952 gadapt-0.2.18/gadapt/execution/
+-rw-rw-rw-   0        0        0       48 2023-06-18 16:27:33.000000 gadapt-0.2.18/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3302 2023-06-03 20:49:46.000000 gadapt-0.2.18/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.428452 gadapt-0.2.18/gadapt/exit_check/
+-rw-rw-rw-   0        0        0       56 2023-06-18 16:29:21.000000 gadapt-0.2.18/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      379 2023-06-03 19:51:29.000000 gadapt-0.2.18/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1113 2023-06-03 19:50:16.000000 gadapt-0.2.18/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      365 2023-06-03 19:51:48.000000 gadapt-0.2.18/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      449 2023-06-03 19:51:58.000000 gadapt-0.2.18/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.431454 gadapt-0.2.18/gadapt/factory/
+-rw-rw-rw-   0        0        0       74 2023-06-18 16:31:20.000000 gadapt-0.2.18/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0    10398 2023-06-18 16:54:21.000000 gadapt-0.2.18/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0    26501 2023-06-03 20:44:22.000000 gadapt-0.2.18/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.433952 gadapt-0.2.18/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0       26 2023-06-18 16:31:46.000000 gadapt-0.2.18/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2188 2023-06-03 19:19:12.000000 gadapt-0.2.18/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.572463 gadapt-0.2.18/gadapt/ga_model/
+-rw-rw-rw-   0        0        0       33 2023-06-18 16:32:02.000000 gadapt-0.2.18/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     8611 2023-06-03 20:28:37.000000 gadapt-0.2.18/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      723 2023-06-03 20:31:30.000000 gadapt-0.2.18/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     6427 2023-06-03 20:15:33.000000 gadapt-0.2.18/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     2137 2023-06-03 20:09:38.000000 gadapt-0.2.18/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1472 2023-06-03 20:05:45.000000 gadapt-0.2.18/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2704 2023-06-03 20:06:52.000000 gadapt-0.2.18/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.18/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    12730 2023-06-03 20:00:59.000000 gadapt-0.2.18/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      881 2023-06-03 20:04:36.000000 gadapt-0.2.18/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.578463 gadapt-0.2.18/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0       91 2023-06-18 16:44:14.000000 gadapt-0.2.18/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      367 2023-06-03 19:46:03.000000 gadapt-0.2.18/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0     1102 2023-06-18 16:36:56.000000 gadapt-0.2.18/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.579963 gadapt-0.2.18/gadapt/immigration/
+-rw-rw-rw-   0        0        0       54 2023-06-18 16:45:34.000000 gadapt-0.2.18/gadapt/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.583464 gadapt-0.2.18/gadapt/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0       69 2023-06-18 16:45:47.000000 gadapt-0.2.18/gadapt/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-06-03 19:42:17.000000 gadapt-0.2.18/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      407 2023-06-03 19:43:54.000000 gadapt-0.2.18/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.587964 gadapt-0.2.18/gadapt/immigration/population_immigration/
+-rw-rw-rw-   0        0        0       79 2023-06-18 16:46:42.000000 gadapt-0.2.18/gadapt/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      239 2023-06-03 19:44:12.000000 gadapt-0.2.18/gadapt/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0      993 2023-06-03 19:45:35.000000 gadapt-0.2.18/gadapt/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.589464 gadapt-0.2.18/gadapt/mutation/
+-rw-rw-rw-   0        0        0       38 2023-06-18 16:47:20.000000 gadapt-0.2.18/gadapt/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.610465 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:47:50.000000 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      956 2023-06-03 19:39:26.000000 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     3031 2023-06-03 19:37:17.000000 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     1009 2023-06-03 19:37:53.000000 gadapt-0.2.18/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.616465 gadapt-0.2.18/gadapt/mutation/population_mutation/
+-rw-rw-rw-   0        0        0       51 2023-06-18 17:07:55.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-06-03 19:39:16.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/base_population_mutator.py
+-rw-rw-rw-   0        0        0     1365 2023-06-03 19:40:00.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/composed_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.619466 gadapt-0.2.18/gadapt/mutation/population_mutation/cost_diversity/
+-rw-rw-rw-   0        0        0       56 2023-06-18 17:07:58.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-06-03 19:41:44.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     2045 2023-06-03 19:40:53.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1130 2023-06-03 19:41:22.000000 gadapt-0.2.18/gadapt/mutation/population_mutation/random_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.630467 gadapt-0.2.18/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0       37 2023-06-18 16:59:38.000000 gadapt-0.2.18/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      395 2023-06-03 19:27:41.000000 gadapt-0.2.18/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0     1172 2023-06-03 19:31:52.000000 gadapt-0.2.18/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.641466 gadapt-0.2.18/gadapt/sampling/
+-rw-rw-rw-   0        0        0      128 2023-06-18 17:00:39.000000 gadapt-0.2.18/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      793 2023-06-03 19:32:22.000000 gadapt-0.2.18/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      534 2023-06-03 19:33:37.000000 gadapt-0.2.18/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      512 2023-06-03 19:33:50.000000 gadapt-0.2.18/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1954 2023-06-03 19:34:36.000000 gadapt-0.2.18/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2717 2023-06-03 19:35:01.000000 gadapt-0.2.18/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.643968 gadapt-0.2.18/gadapt/string_operation/
+-rw-rw-rw-   0        0        0       90 2023-06-18 17:02:51.000000 gadapt-0.2.18/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-06-03 20:30:52.000000 gadapt-0.2.18/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.646968 gadapt-0.2.18/gadapt/utils/
+-rw-rw-rw-   0        0        0      281 2023-06-03 20:30:21.000000 gadapt-0.2.18/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0       35 2023-06-18 17:03:05.000000 gadapt-0.2.18/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1313 2023-06-03 20:30:37.000000 gadapt-0.2.18/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.650468 gadapt-0.2.18/gadapt/validation/
+-rw-rw-rw-   0        0        0       31 2023-06-18 17:03:27.000000 gadapt-0.2.18/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      846 2023-06-03 20:29:38.000000 gadapt-0.2.18/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    17474 2023-06-03 20:29:54.000000 gadapt-0.2.18/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.662969 gadapt-0.2.18/gadapt/variable_update/
+-rw-rw-rw-   0        0        0       53 2023-06-18 17:04:05.000000 gadapt-0.2.18/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      234 2023-06-03 20:28:58.000000 gadapt-0.2.18/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2052 2023-06-03 20:29:16.000000 gadapt-0.2.18/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:29.412450 gadapt-0.2.18/gadapt.egg-info/
+-rw-rw-rw-   0        0        0    21892 2023-06-18 17:40:29.000000 gadapt-0.2.18/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-06-18 17:40:29.000000 gadapt-0.2.18/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:40:29.000000 gadapt-0.2.18/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 17:40:29.000000 gadapt-0.2.18/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-18 17:40:29.674470 gadapt-0.2.18/setup.cfg
+-rw-rw-rw-   0        0        0      465 2023-06-18 17:38:21.000000 gadapt-0.2.18/setup.py
```

### Comparing `gadapt-0.2.17/PKG-INFO` & `gadapt-0.2.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.2.17
+Version: 0.2.18
 Summary: GAdapt: A Python Library for Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 License: UNKNOWN
 Description: # GAdapt: Self-Adaptive Genetic Algorithm
-        **GAdapt** (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
+        [GAdapt] (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
         
         # What innovations does GAdapt bring?
         **GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
         
         
         # Installation
         To install **GAdapt**, use **pip** with the following command:
         
         ```
         pip install gadapt
         ```
         
         # Source Code
-        The source code is stored on GitHub at the following address: https://github.com/bpzoran/gadapt
+        The source code is stored on GitHub at the following address: [https://github.com/bpzoran/gadapt/] https://github.com/bpzoran/gadapt
+        
+        # API Documentation
+        The API documentation can be found on the following address: [https://www.gadapt.com/api/] https://www.gadapt.com/api
         
         # Getting started
         The following example optimizes variable values for a complex trigonometric function.
         ```python
         from gadapt.ga import GA
         import math
         
@@ -168,15 +171,15 @@
         - *"random"* - Random selection algorithm uses a uniform random number generator to select genes for mutation. In this case, selection for the mutation will not depend on gene cross-diversity.  
             
         **immigration_number**=*0* - Refers to the "Random Immigrants" concepts. This strategy introduces a certain number of individuals into the population during the evolution process. These new individuals are generated randomly and injected into the population.
         
         **logging**=*False* - If this parameter has a True value, the log file will be created in the current working directory. The log file contains the flow of genetic algorithm execution, along with values of chromosomes, genes and cost functions in each generation
         
         # Adding Variables
-        Variables to be optimized can be added by callning the *add* method of the *GA* object. Parameters of this method are the minimum value, the maximum value, and the step. The minimum and maximum value determine a range of possible variable values. The *step* parameter specifies the step that will be used in changing the variables values during the optimization.
+        Variables to be optimized can be added by calling the *add* method of the *GA* object. Parameters of this method are the minimum value, the maximum value, and the step. The minimum and maximum value determine a range of possible variable values. The *step* parameter specifies the step that will be used in changing the variables values during the optimization.
         
         For example:
         ```python
         ga.add(1.0, 4.0, 0.01)
         ```
         means that the corresponding parameter can have values between 1.0 and 4.0, and the step for changing variable values in optimization is 0.01.
```

### Comparing `gadapt-0.2.17/README.md` & `gadapt-0.2.18/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # GAdapt: Self-Adaptive Genetic Algorithm
-**GAdapt** (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
+[GAdapt] (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
 
 # What innovations does GAdapt bring?
 **GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
 
 
 # Installation
 To install **GAdapt**, use **pip** with the following command:
 
 ```
 pip install gadapt
 ```
 
 # Source Code
-The source code is stored on GitHub at the following address: https://github.com/bpzoran/gadapt
+The source code is stored on GitHub at the following address: [https://github.com/bpzoran/gadapt/] https://github.com/bpzoran/gadapt
+
+# API Documentation
+The API documentation can be found on the following address: [https://www.gadapt.com/api/] https://www.gadapt.com/api
 
 # Getting started
 The following example optimizes variable values for a complex trigonometric function.
 ```python
 from gadapt.ga import GA
 import math
 
@@ -160,15 +163,15 @@
 - *"random"* - Random selection algorithm uses a uniform random number generator to select genes for mutation. In this case, selection for the mutation will not depend on gene cross-diversity.  
     
 **immigration_number**=*0* - Refers to the "Random Immigrants" concepts. This strategy introduces a certain number of individuals into the population during the evolution process. These new individuals are generated randomly and injected into the population.
 
 **logging**=*False* - If this parameter has a True value, the log file will be created in the current working directory. The log file contains the flow of genetic algorithm execution, along with values of chromosomes, genes and cost functions in each generation
 
 # Adding Variables
-Variables to be optimized can be added by callning the *add* method of the *GA* object. Parameters of this method are the minimum value, the maximum value, and the step. The minimum and maximum value determine a range of possible variable values. The *step* parameter specifies the step that will be used in changing the variables values during the optimization.
+Variables to be optimized can be added by calling the *add* method of the *GA* object. Parameters of this method are the minimum value, the maximum value, and the step. The minimum and maximum value determine a range of possible variable values. The *step* parameter specifies the step that will be used in changing the variables values during the optimization.
 
 For example:
 ```python
 ga.add(1.0, 4.0, 0.01)
 ```
 means that the corresponding parameter can have values between 1.0 and 4.0, and the step for changing variable values in optimization is 0.01.
```

### Comparing `gadapt-0.2.17/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.18/gadapt/cost_finding/common_cost_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 from typing import List
 from gadapt.cost_finding.base_cost_finder import BaseCostFinder
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.population import Population
 import gadapt.utils.ga_utils as ga_utils
 
 class CommonCostFinder(BaseCostFinder):
+
+    """
+    Common class for cost finding
+    """
+
     def find_costs_for_chromosome(self, population: Population):
         if (population is None):
             raise Exception("population must not be null!")
         chromosomes_for_execution: List[Chromosome] = [
             c for c in population if (math.isnan(c.cost_value)) or (c.is_immigrant and c.population_generation == population.population_generation)]
         for c in chromosomes_for_execution:
             self.execute_function(population.options.cost_function, c)
```

### Comparing `gadapt-0.2.17/gadapt/crossover/base_crossover.py` & `gadapt-0.2.18/gadapt/crossover/base_crossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
 import gadapt.utils.ga_utils as ga_utils
 import gadapt.ga_model.definitions as definitions
 
 class BaseCrossover:
+
+    """
+    Base Crossover Class
+    """
     
     def __init__(self, gene_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator):
         self._mutation_on_both_sides = True
         self.gene_combination = gene_combination
         self.mutator = mutator
         self.immigrator = immigrator
```

### Comparing `gadapt-0.2.17/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.18/gadapt/crossover/uniform_crossover.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from gadapt.crossover.base_crossover import BaseCrossover
 from gadapt.ga_model.gene import Gene
 from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
 
 class UniformCrossover(BaseCrossover):
+
+    """
+    Uniform Crossover
+    """
     
     def __init__(self, var_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator):
         super(UniformCrossover, self).__init__(var_combination, mutator, immigrator)
         self.gene_combination = var_combination
     
     def get_mother_father_genes(self, mother: Chromosome, father: Chromosome):
         father_gene = father[self.current_gene_number]
```

### Comparing `gadapt-0.2.17/gadapt/execution/ga_executor.py` & `gadapt-0.2.18/gadapt/execution/ga_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from gadapt.ga_logging.logging_settings import init_logging
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.ga_results import GAResults
 from gadapt.ga_model.population import Population
 import gadapt.ga_model.message_levels as message_levels
 
 class GAExecutor:
+
+    """
+    Executor for the genetic algorithm
+    """
+
     def __init__(self, ga_options: GAOptions, factory: GAFactory) -> None:
         if (not ga_options is None):
             self.ga_options = ga_options    
         self.factory = factory          
 
 
     def execute(self) -> GAResults:
@@ -34,15 +39,15 @@
             population = Population(self.ga_options,
                                     chromosome_mutator=chromosome_mutator,
                                     population_mutator=population_mutator,
                                     exit_checker=exit_checker,
                                     cost_finder=cost_finder,
                                     population_immigrator=population_immigrator,
                                     chromosome_immigrator=chromosome_immigrator,
-                                    selector=selector,
+                                    parent_selector=selector,
                                     crossover=crossover,
                                     variable_updater=variable_updater)
             population.find_costs()
             while not population.exit():
                 population.immigrate()
                 population.mate()
                 population.mutate()
```

### Comparing `gadapt-0.2.17/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.18/gadapt/exit_check/base_exit_checker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import logging
 from datetime import datetime
 import gadapt.ga_model.definitions as definitions
 
 class BaseExitChecker:
+
+    """
+    Base class for exit check
+    """
+
     def __init__(self, max_attempt_no: int) -> None:
         self.max_attempt_no = max_attempt_no
         self.attempt_no = 0              
     
     @property
     def attempt_no(self) -> int:
         return self._attempt_no
```

### Comparing `gadapt-0.2.17/gadapt/factory/ga_factory.py` & `gadapt-0.2.18/gadapt/factory/ga_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,34 +13,33 @@
 from gadapt.immigration.population_immigration.common_population_immigrator import CommonPopulationImmigrator
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 from gadapt.mutation.chromosome_mutation.cross_diversity_chromosome_mutator import CrossDiversityChromosomeMutator
 from gadapt.mutation.chromosome_mutation.random_chromosome_mutator import RandomChromosomeMutator
 from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
 from gadapt.mutation.population_mutation.composed_population_mutator import ComposedPopulationMutator
 from gadapt.mutation.population_mutation.cost_diversity.cost_diversity_population_mutator import CostDiversityPopulationMutator
-from gadapt.mutation.population_mutation.parent_diversity_population_mutator import ParentsDiversityPopulationMutator
-from gadapt.mutation.population_mutation.previous_cost_diversity.previous_cost_diversity_population_mutator import PreviousCostDiversityPopulationMutator
-from gadapt.mutation.population_mutation.previous_cost_diversity.previous_cost_diversity_property_taker import AvgPreviousCostCostDiversityPropertyTaker, BasePreviousCostDiversityPropertyTaker, MinPreviousCostCostDiversityPropertyTaker
+from gadapt.mutation.population_mutation.parent_diversity_population_mutator import ParentDiversityPopulationMutator
 from gadapt.mutation.population_mutation.random_population_mutator import RandomPopulationMutator
 from gadapt.parent_selection.base_parent_selector import BaseParentSelector
 from gadapt.parent_selection.sampling_parent_selector import SamplingParentSelector
 from gadapt.sampling.base_sampling import BaseSampling
 from gadapt.sampling.from_top_to_bottom_sampling import FromTopToBottomSampling
 from gadapt.sampling.random_sampling import RandomSampling
 from gadapt.sampling.roulette_wheel_sampling import RouletteWheelSampling
 from gadapt.sampling.tournament_sampling import TournamentSampling
-from gadapt.validation.base_options_validator import BaseOptionsValidator
-from gadapt.validation.common_options_validator import CommonOptionsValidator
 from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
 from gadapt.gene_combination.blending_gene_combination import BlendingGeneCombination
 from gadapt.variable_update.common_variable_updater import CommonVariableUpdater
 import gadapt.ga_model.definitions as definitions
 
 
 class GAFactory:
+    """
+    Factory for creating  class instances based on GA options
+    """
     def __init__(self, ga, options: GAOptions) -> None:
         self.ga = ga
         self.options = options
 
     @property
     def ga(self):
         return self._ga
@@ -54,91 +53,124 @@
         return self._options
 
     @options.setter
     def options(self, value):
         self._options = value
 
     def get_cost_finder(self) -> BaseCostFinder:
+        """
+        Cost Finder instance
+        """
         return CommonCostFinder()
 
     def get_population_immigrator(self) -> BasePopulationImmigrator:
+        """
+        Population Immigrator Instance
+        """
         return CommonPopulationImmigrator()
 
     def get_chromosome_immigrator(self) -> BaseChromosomeImmigrator:
+        """
+        Chromosome Immigrator Instance
+        """
         return RandomChromosomeImmigrator()
 
     def get_chromosome_mutator(self) -> BaseChromosomeMutator:
+        """
+        Chromosome Mutator Instance
+        """
         if self.ga.chromosome_mutation.strip() == definitions.CROSS_DIVERSITY:
             return CrossDiversityChromosomeMutator(self.get_sampling_method(self.ga.cross_diversity_mutation_gene_selection))
         elif self.ga.chromosome_mutation.strip() == definitions.RANDOM:
             return RandomChromosomeMutator()
         else:
             raise Exception("unknown chromosome mutation")
 
     def population_mutator_options_validation(self):
+        """
+        Validates population mutator options
+        """
         mutator_strings = self.ga.population_mutation.split(definitions.PARAM_SEPARATOR)
         for s in mutator_strings:
             if not s.strip() in definitions.POPULATION_MUTATOR_STRINGS:
                 raise Exception(s + " is not defined as option for population mutation")
 
     def get_population_mutator(self, population_mutator_string=None) -> BasePopulationMutator:
+        """
+        Population Mutator Instance
+        """
         self.population_mutator_options_validation()
         if population_mutator_string is None:
             population_mutator_string = self.ga.population_mutation.strip()
         if population_mutator_string.find(definitions.PARAM_SEPARATOR) > -1:
             return self.get_population_mutator_combined()
         elif population_mutator_string == definitions.COST_DIVERSITY:
-            return CostDiversityPopulationMutator(self.options, ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
+            return CostDiversityPopulationMutator(self.options, ParentDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
         elif population_mutator_string == definitions.PARENT_DIVERSITY:
-            return ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options)
+            return ParentDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options)
         elif population_mutator_string == definitions.RANDOM:
             return RandomPopulationMutator(self.options)
         else:
             raise Exception("unknown population mutation")
 
-    def get_previous_cost_diversity_property_taker(self) -> BasePreviousCostDiversityPropertyTaker:
-        return AvgPreviousCostCostDiversityPropertyTaker()
-
     def get_population_mutator_combined(self) -> ComposedPopulationMutator:
+        """
+        Population Mutator Instance - combined
+        """
         mutator_strings = [ms.strip() for ms in self.ga.population_mutation.split(definitions.PARAM_SEPARATOR)]
         if (self.is_cost_diversity_random(mutator_strings)):
             return CostDiversityPopulationMutator(self.options, RandomPopulationMutator(self.options))
         if (self.is_cost_diversity_parent_diversity(mutator_strings)):
-            return CostDiversityPopulationMutator(self.options, ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
+            return CostDiversityPopulationMutator(self.options, ParentDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
         if self.is_cost_diversity_parent_diversity_random(mutator_strings):
             composedPopulationMutator = ComposedPopulationMutator(self.options)
-            composedPopulationMutator.append(ParentsDiversityPopulationMutator(self.get_sampling_method(
+            composedPopulationMutator.append(ParentDiversityPopulationMutator(self.get_sampling_method(
                 self.ga.parent_diversity_mutation_chromosome_selection), self.options))
             composedPopulationMutator.append(
                 RandomPopulationMutator(self.options))
-            return PreviousCostDiversityPopulationMutator(self.options, composedPopulationMutator)
+            return CostDiversityPopulationMutator(self.options, composedPopulationMutator)
         composedPopulationMutator = ComposedPopulationMutator(self.options)
         for ms in mutator_strings:
             composedPopulationMutator.append(self.get_population_mutator(ms))
         return composedPopulationMutator
 
     def is_cost_diversity_random(self, mutator_strings: list):
+        """
+        Is population mutator cost diversity and random
+        """
         if len(mutator_strings) == 2 and definitions.COST_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
             return True
         return False
 
     def is_cost_diversity_parent_diversity(self, mutator_strings: list):
+        """
+        Is population mutator cost diversity and parent diversity
+        """
         if len(mutator_strings) == 2 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENT_DIVERSITY in mutator_strings:
             return True
         return False
 
     def is_cost_diversity_parent_diversity_random(self, mutator_strings: list):
+        """
+        Is population mutator cost diversity, parent diversity and random
+        """
         if len(mutator_strings) == 3 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENT_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
             return True
         return False
 
     def get_parent_selector(self) -> BaseParentSelector:
+        """
+        Parent Selector Instance
+        """
         return SamplingParentSelector(self.get_sampling_method(self.ga.parent_selection))
 
     def get_sampling_method(self, str) -> BaseSampling:
+        """
+        Sampling Methos Instance
+        """
         str_value = str
         sampling_method_strings = str.split(definitions.PARAM_SEPARATOR)
         other_value = None
         if len(sampling_method_strings) > 1:
             str_value = sampling_method_strings[0]
             try:
                 other_value = int(sampling_method_strings[1])
@@ -149,21 +181,33 @@
         elif str_value == definitions.FROM_TOP_TO_BOTTOM:
             return FromTopToBottomSampling()
         elif str_value == definitions.RANDOM:
             return RandomSampling()
         return RouletteWheelSampling()
 
     def get_gene_combination(self) -> BaseGeneCombination:
+        """
+        Gene Combination Instance
+        """
         return BlendingGeneCombination()
 
     def get_exit_checker(self) -> BaseExitChecker:
+        """
+        Exit Checker Instance
+        """
         if self.ga.exit_check == definitions.AVG_COST:
             return AvgCostExitChecker(self.ga.max_attempt_no)
         if self.ga.exit_check == definitions.MIN_COST:
             return MinCostExitChecker(self.ga.max_attempt_no)
         return RequestedCostExitChecker(self.ga.requested_cost)
 
     def get_crossover(self, gene_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator) -> BaseCrossover:
+        """
+        Crossover Instance
+        """
         return UniformCrossover(gene_combination, mutator, immigrator)
 
     def get_variable_updater(self):
+        """
+        Variable Updater Instance
+        """
         return CommonVariableUpdater()
```

### Comparing `gadapt-0.2.17/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.18/gadapt/ga_logging/logging_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import logging
 import os
 from os.path import isfile, join
 import traceback
 from gadapt.utils.TimeStampFormatter import TimestampFormatter
 
 def init_logging(is_logging: bool):
+    """
+    Initializes logging for genetic algorithm
+    """
     def get_last_num(s: str) -> int:
         try:
             if not s.startswith("log.log"):
                 return -1
             if s == "log.log":
                 return 0
             n_last_number = int(s_last_number)
```

### Comparing `gadapt-0.2.17/gadapt/ga_model/definitions.py` & `gadapt-0.2.18/gadapt/ga_model/definitions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Genetic algorithm definitions
+"""
+
 RANDOM = "random"
 COST_DIVERSITY = "cost_diversity"
 PARENT_DIVERSITY = "parent_diversity"
 CROSS_DIVERSITY = "cross_diversity"
 TOURNAMENT = "tournament"
 FROM_TOP_TO_BOTTOM = "from_top_to_bottom"
 ROULETTE_WHEEL = "roulette_wheel"
```

### Comparing `gadapt-0.2.17/gadapt/ga_model/ga_options.py` & `gadapt-0.2.18/gadapt/ga_model/ga_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,172 @@
 from typing import List
 from gadapt.ga_model.genetic_variable import GeneticVariable
 class GAOptions():
    
+    """
+    Genetic algorithm options
+    """
+    
     def __init__(self, ga) -> None:
         super().__init__()           
         self._population_size = ga.population_size
         self._cost_function = ga.cost_function                
         self._immigration_number = ga.immigration_number
-        self.set_number_of_mutation_chromosomes(ga)
+        self._set_number_of_mutation_chromosomes(ga)
         self._max_attempt_no = ga.max_attempt_no
         self._requested_cost = ga.requested_cost
         self._logging = ga.logging
         self._genetic_variables = ga._genetic_variables
-        self.set_number_of_mutation_genes(ga)
+        self._set_number_of_mutation_genes(ga)
         self._must_mutate_for_same_parents = ga.must_mutate_for_same_parents
         self._timeout = ga.timeout
 
-    def set_number_of_mutation_chromosomes(self, ga):
+    def _set_number_of_mutation_chromosomes(self, ga):
         if (not ga.number_of_mutation_chromosomes is None) and isinstance(ga.number_of_mutation_chromosomes, int) and ga.number_of_mutation_chromosomes >= 0:                  
             self._number_of_mutation_chromosomes = ga.number_of_mutation_chromosomes
         elif (not ga.percentage_of_mutation_chromosomes is None) and isinstance(ga.percentage_of_mutation_chromosomes, float) and ga.percentage_of_mutation_chromosomes >= 0.0 and ga.percentage_of_mutation_chromosomes <= 100:
             nomc = round(self.population_size * (ga.percentage_of_mutation_chromosomes / 100))
             while nomc >= self.population_size //2 - self.immigration_number:
                 nomc -= 1
             if nomc < 0:
                 raise Exception("Invalid percentage of mutation chromosomes and immigration number")
             self._number_of_mutation_chromosomes = nomc
         else:
             self._number_of_mutation_chromosomes = ga.number_of_mutation_chromosomes
 
-    def set_number_of_mutation_genes(self, ga):
+    def _set_number_of_mutation_genes(self, ga):
         if (not ga.number_of_mutation_genes is None) and isinstance(ga.number_of_mutation_genes, int) and ga.number_of_mutation_genes >= 0:
             self._number_of_mutation_genes = ga.number_of_mutation_genes  
         elif (not ga.percentage_of_mutation_genes is None) and isinstance(ga.percentage_of_mutation_genes, float) and ga.percentage_of_mutation_genes >= 0.0 and ga.percentage_of_mutation_genes <= 100:
             self._number_of_mutation_genes = round(float(len(self._genetic_variables)) * (ga.percentage_of_mutation_genes / 100))
         else:
             self._number_of_mutation_genes = ga.number_of_mutation_genes
     
     @property
     def requested_cost(self) -> float:
+        """
+        Determines the requested value which causes the exit from the genetic algorithm
+        """
         return self._requested_cost
 
     @requested_cost.setter
     def requested_cost(self, value: float):
         self._requested_cost = value
     
     @property
     def max_attempt_no(self) -> int:
+        """
+        Determines the number of generations in which there is no improvement in the average/minimal cost.
+        """
         return self._max_attempt_no
 
     @max_attempt_no.setter
     def max_attempt_no(self, value: int):
         self._max_attempt_no = value
     
     @property
     def immigration_number(self) -> int:
+        """
+        Number of immigration chromosomes
+        """
         return self._immigration_number
     
     @immigration_number.setter
     def immigration_number(self, value: int):
         self._immigration_number = value
     
     @property
     def number_of_mutation_chromosomes(self) -> int:
+        """
+        The number of mutation chromosomes in the population.
+        """
         return self._number_of_mutation_chromosomes
     
     @number_of_mutation_chromosomes.setter
     def number_of_mutation_chromosomes(self, value: int):
         self._number_of_mutation_chromosomes = value
     
     @property
     def number_of_mutation_genes(self) -> int:
+        """
+        The number of mutated genes in each chromosome. 
+        """
         return self._number_of_mutation_genes
     
     @number_of_mutation_genes.setter
     def number_of_mutation_genes(self, value: int):
         self._number_of_mutation_genes = value
     
     @property
     def cost_function(self):
+        """
+        Custom function for the cost calculation (fitness)
+        """
         return self._cost_function
     
     @cost_function.setter
     def cost_function(self, value):
         self._cost_function = value
     
     @property
     def population_size(self) -> int:
+        """
+        Number of chromosomes in the population.
+        """
         return self._population_size
     
     @population_size.setter
     def population_size(self, value: int):
         self._population_size = value
     
     @property
     def genetic_variables(self) -> List[GeneticVariable]:
+        """
+        Collection of genetic variables
+        """
         return self._genetic_variables  
 
     @property
-    def abandon_number(self) -> int:
-        return self.get_abandon_number()
+    def _abandon_number(self) -> int:
+        return self._get_abandon_number()
     
-    def get_abandon_number(self) -> int:
+    def _get_abandon_number(self) -> int:
         if self.population_size % 2 == 0:
             return self.population_size // 2
         return self.population_size // 2 - 1
     
     @property
     def keep_number(self) -> int:
-        return self.population_size - self.abandon_number    
+        return self.population_size - self._abandon_number    
 
     @property
     def logging(self) -> bool:
+        """
+        If True, the log file will be created in the current working directory. 
+        """
         return self._logging
     
     @logging.setter
     def logging(self, value: bool):
         self._logging = value
 
     @property
     def must_mutate_for_same_parents(self) -> bool:
+        """
+        Indicates if completely the same parents must influence mutation for their children.
+        """
         return self._must_mutate_for_same_parents
     
     @must_mutate_for_same_parents.setter
     def must_mutate_for_same_parents(self, value: bool):
         self._must_mutate_for_same_parents = value
 
     @property
     def timeout(self) -> int:
+        """
+         A number of seconds after which the genetic algorithm optimisation will exit, regardless of whether exit_check criteria is reached.
+        """
         return self._timeout
     
     @timeout.setter
     def timeout(self, value: int):
         self._timeout = value
```

### Comparing `gadapt-0.2.17/gadapt/ga_model/gene.py` & `gadapt-0.2.18/gadapt/ga_model/gene.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import math
 from gadapt.ga_model.genetic_variable import GeneticVariable
 from gadapt.ga_model.ranking_model import RankingModel
 import gadapt.string_operation.ga_strings as ga_strings
 import gadapt.ga_model.definitions as definitions
 class Gene(RankingModel):
 
+    """
+    Gene class. Gene is a part of chromosome.
+    It contains concrete values for genetic variables.
+    
+    """
+    
     def __init__(self, gen_variable, var_value = None):
         super().__init__()
         self.genetic_variable = gen_variable        
         self.variable_value = var_value
         self._rank = -1
         self._cummulative_probability = definitions.FLOAT_NAN
         if (self.variable_value == None or math.isnan(self.variable_value)):
```

### Comparing `gadapt-0.2.17/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.18/gadapt/ga_model/genetic_variable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import random
 import gadapt.ga_model.definitions as definitions
 class GeneticVariable:
 
+    """
+    Genetic variable class defines genes.
+    It contains common values for genes: variable id, maximal value, minimal value, step.
+    """
+    
     def __init__(self, id: int) -> None:
         self.variable_id = id
         self._standard_deviation = definitions.FLOAT_NAN
     
     def __eq__(self, other):
         if not isinstance(other, GeneticVariable):
             return False
```

### Comparing `gadapt-0.2.17/gadapt/ga_model/population.py` & `gadapt-0.2.18/gadapt/ga_model/population.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,41 +6,69 @@
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.gene import Gene
 from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
 from gadapt.immigration.population_immigration.base_population_immigrator import BasePopulationImmigrator
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
 from gadapt.mutation.population_mutation.composed_population_mutator import ComposedPopulationMutator
+from gadapt.parent_selection.base_parent_selector import BaseParentSelector
 from gadapt.variable_update.base_variable_updater import BaseVariableUpdater
 import gadapt.string_operation.ga_strings as ga_strings
 from datetime import datetime
 import gadapt.ga_model.definitions as definitions
 
 class Population:
 
+    """
+    Population for the genetic algorithm. It contains a collection of chromosomes, as well as additional parameters
+    """
+
     def __init__(self, options: GAOptions,
                  chromosome_mutator: BaseChromosomeMutator,
                  population_mutator: BasePopulationMutator,
                  exit_checker: BaseExitChecker,
                  cost_finder: BaseCostFinder,
                  population_immigrator: BasePopulationImmigrator,
                  chromosome_immigrator: BaseChromosomeImmigrator,
-                 selector,
+                 parent_selector: BaseParentSelector,
                  crossover: BaseCrossover,
                  variable_updater: BaseVariableUpdater):
+        """
+        Initializator for the Population class.
+
+        options: Genetic Algorithm Options
+
+        chromosome_mutator: Chromosome Mutator Instance
+
+        population_mutator: Population Mutator Instance
+
+        exit_checker: Exit Checker Instance
+
+        cost_finder: Cost Finder Instance
+
+        population_immigrator: Population Immigrator Instance
+
+        chromosome_immigrator: Chromosome Immigrator Instance
+
+        parent_selector: Parent Selector Instance
+
+        crossover: Crossover Instance
+
+        variable_updater: Variable Updater Instance
+        """
         if options.population_size < 4:
             raise Exception("Population size 4 must be higher than 3")        
         self.options = options
         self.chromosome_mutator = chromosome_mutator
         self.population_mutator = population_mutator
         self.exit_checker = exit_checker
         self.cost_finder = cost_finder
         self.population_immigrator = population_immigrator
         self.chromosome_immigrator = chromosome_immigrator
-        self.selector = selector
+        self.parent_selector = parent_selector
         self.crossover = crossover
         self.variable_updater = variable_updater
         self.set_init_values()
         self.last_chromosome_id = 1
         self._population_generation = 0
         self.options = options
         self.chromosomes = []
@@ -79,218 +107,303 @@
         self.previous_avg_cost = float_init_value
         self.min_cost = float_init_value
         self.previous_min_cost = float_init_value
         self.first_cost = float_init_value
 
     @property
     def options(self) -> GAOptions:
+        """
+        Genetic algorithm options
+        """
         return self._options
 
     @options.setter
     def options(self, value: GAOptions):
         self._options = value
 
     @property
     def avg_cost(self) -> float:
+        """
+        Average cost of the population
+        """
         return self._avg_cost
 
     @avg_cost.setter
     def avg_cost(self, value: float):
         self._avg_cost = value
 
     @property
     def previous_avg_cost(self) -> float:
+        """
+        Previous average cost
+        """
         return self._previous_avg_cost
 
     @previous_avg_cost.setter
     def previous_avg_cost(self, value: float):
         self._previous_avg_cost = value
 
     @property
     def min_cost(self):
+        """
+        Minimum cost
+        """
         return self._min_cost
 
     @min_cost.setter
     def min_cost(self, value: float) -> float:
         self._min_cost = value
 
     @property
     def previous_min_cost(self):
+        """
+        Previous minimum cost
+        """
         return self._previous_min_cost
 
     @previous_min_cost.setter
     def previous_min_cost(self, value: float) -> float:
         self._previous_min_cost = value
 
     @property
     def first_cost(self) -> float:
+        """
+        First cost found
+        """
         return self._first_cost
 
     @first_cost.setter
     def first_cost(self, value: float):
         self._first_cost = value
 
     @property
     def best_individual(self) -> Chromosome:
+        """
+        Best individual chromosome
+        """
         return self._best_individual
 
     @best_individual.setter
     def best_individual(self, value: Chromosome):
         self._best_individual = value
 
     @property
     def population_generation(self):
+        """
+        Current generation of the population
+        """
         return self._population_generation
 
     @population_generation.setter
     def population_generation(self, value):
         self._population_generation = value
 
     @property
     def chromosome_mutator(self) -> BaseChromosomeMutator:
+        """
+        Chromosome mutator algorithm
+        """
         return self._chromosome_mutator
 
     @chromosome_mutator.setter
     def chromosome_mutator(self, value: BaseChromosomeMutator):
         self._chromosome_mutator = value
 
     @property
     def population_mutator(self) -> BasePopulationMutator:
+        """
+        Population mutator algorithm
+        """
         return self._population_mutator
 
     @population_mutator.setter
     def population_mutator(self, value: BasePopulationMutator):
         self._population_mutator = value
 
     def append_population_mutator(self, value: BasePopulationMutator):
+        """
+        Appends population mutator algorithm
+        """
         if self._population_mutator is None or not isinstance(self._population_mutator, ComposedPopulationMutator):
             self.population_mutator = ComposedPopulationMutator(self.options)
         self.population_mutator.append(value)
 
     @property
     def cost_finder(self) -> BaseCostFinder:
+        """
+        Cost finding algorithm
+        """
         return self._cost_finder
 
     @cost_finder.setter
     def cost_finder(self, value: BaseCostFinder):
         self._cost_finder = value
 
     @property
-    def selector(self):
-        return self._selector
-
-    @selector.setter
-    def selector(self, value):
-        self._selector = value
+    def parent_selector(self):
+        """
+        Parent selection algorithm
+        """
+        return self._parent_selector
+
+    @parent_selector.setter
+    def parent_selector(self, value):
+        self._parent_selector = value
 
     @property
     def population_immigrator(self) -> BasePopulationImmigrator:
+        """
+        Population immigration algorithm
+        """
         return self._population_immigrator
 
     @population_immigrator.setter
     def population_immigrator(self, value: BasePopulationImmigrator):
         self._population_immigrator = value
 
     @property
     def chromosome_immigrator(self) -> BasePopulationImmigrator:
+        """
+        Chromosome immigration algorithm
+        """
         return self._chromosome_immigrator
 
     @chromosome_immigrator.setter
     def chromosome_immigrator(self, value: BasePopulationImmigrator):
         self._chromosome_immigrator = value
 
     @property
     def crossover(self) -> BaseCrossover:
+        """
+        Crossover algorithm
+        """
         return self._crossover
 
     @crossover.setter
     def crossover(self, value: BaseCrossover):
         self._crossover = value
 
     @property
     def variable_updater(self) -> BaseVariableUpdater:
+        """
+        Variable update algorithm
+        """
         return self._variable_updater
 
     @variable_updater.setter
     def variable_updater(self, value: BaseVariableUpdater):
         self._variable_updater = value
 
     @property
-    def population_immigrator(self) -> BasePopulationImmigrator:
-        return self._population_immigrator
-
-    @population_immigrator.setter
-    def population_immigrator(self, value: BasePopulationImmigrator):
-        self._population_immigrator = value
-
-    @property
     def cost_finder(self) -> BaseCostFinder:
+        """
+        Cost finding algorithm
+        """
         return self._cost_finder
 
     @cost_finder.setter
     def cost_finder(self, value: BaseCostFinder):
         self._cost_finder = value
 
     @property
     def exit_checker(self) -> BaseExitChecker:
+        """
+        Exit checking algorithm
+        """
         return self._exit_checker
 
     @exit_checker.setter
     def exit_checker(self, value: BaseExitChecker):
         self._exit_checker = value
 
     def exit(self) -> bool:
+        """
+        Check exit from the GA
+        """
         self.population_generation += 1
         self.population_mutator.before_exit_check(self)
         return self.exit_checker.check(self)
 
     def immigrate(self):
+        """
+        Immigrates new chromosomes
+        """
         self.population_immigrator.immigrate(self)
 
     def select_mates(self) -> List[Tuple[Chromosome, Chromosome]]:
-        return self.selector.select_mates(self)
+        """
+        Selects mates for pairing
+        """
+        return self.parent_selector.select_mates(self)
 
     def mate(self):
+        """
+        Mates chromosomes
+        """
         chromosome_pairs = self.select_mates()
         for chromosome1, chromosome2 in chromosome_pairs:
             offspring1, offspring2 = self.crossover.mate(chromosome1, chromosome2, self.population_generation)
             self.add_chromosomes((offspring1, offspring2))
 
     def mutate(self):
+        """
+        Mutates chromosomes in the population
+        """
         self.population_mutator.mutate(self)
 
     def find_costs(self):
+        """
+        Finds costs for chromosomes
+        """
         self.previous_avg_cost = self.avg_cost
         self.previous_min_cost = self.min_cost
         self.cost_finder.find_costs_for_chromosome(self)
 
     def clear(self):
+        """
+        Clears all chromosomes
+        """
         self.chromosomes.clear()
 
     def clear_and_add_chromosomes(self, chromosomes: List[Chromosome]):
+        """
+        Clears chromosomes and adds new ones
+        """
         self.chromosomes.clear()
         self.add_chromosomes(chromosomes)
 
     def add_chromosomes(self, chromosomes):
+        """
+        Adds chromosomes to population
+        """
         for c in chromosomes:
             self.add_chromosome(c)
 
     def add_new_chromosome(self):
+        """
+        Adds new chromosomes to the population
+        """
         chromosome = Chromosome(self.chromosome_mutator, self.chromosome_immigrator, self.population_generation)
         chromosome.chromosome_generation = 1
         self.add_chromosome(chromosome)
 
     def add_chromosome(self, chromosome):
+        """
+        Adds chromosome to the population
+        """
         if len(self) >= self.options.population_size:
             return
         if chromosome.chromosome_id is None or chromosome.chromosome_id == -1:
             chromosome.chromosome_id = self.last_chromosome_id            
             self.last_chromosome_id += 1            
         if len(chromosome) == 0:
             for gv in self.options.genetic_variables:
                 g = Gene(gv)
                 chromosome.append(g)
         self.append(chromosome)
 
     def update_variables(self):
+        """
+        Updates genetic variables
+        """
         self.variable_updater.update_variables(self)
```

### Comparing `gadapt-0.2.17/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.18/gadapt/ga_model/ranking_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import gadapt.ga_model.definitions as definitions
 class RankingModel:
+
+    """
+    Base class for the object that can be ranked (chromosomes and genes)
+    """
+
     def __init__(self):
         self._rank = -1
         self._cummulative_probability = definitions.FLOAT_NAN
     
     @property
     def rank(self):
         return self._rank
```

### Comparing `gadapt-0.2.17/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.18/gadapt/gene_combination/blending_gene_combination.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 import random
 from gadapt.ga_model.gene import Gene
 from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
 
 class BlendingGeneCombination(BaseGeneCombination):
+
+    """
+    Blending gene combination combines
+    gene values from the two parents into new variable values in offsprings.
+    One value of the offspring variable comes from a combination of the two
+    corresponding values of the parental genes
+    """
+
     def combine(self, mother_gene: Gene, father_gene: Gene):
         genetic_variable = father_gene.genetic_variable
         val_father = father_gene.variable_value
         val_mother = mother_gene.variable_value
         x = 1
         if val_mother > val_father:
             x = -1
```

### Comparing `gadapt-0.2.17/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.2.18/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import gadapt.ga_model.definitions as definitions
 class BaseChromosomeImmigrator:
+
+    """
+    Base class for chromosome immigration
+    """
+
     def immigrate(self, c):
         self.immigrate_chromosome(c)
         self.chromosome_immigrated(c)
 
     def immigrate_chromosome(self, c):
         raise Exception(definitions.NOT_IMPLEMENTED)
```

### Comparing `gadapt-0.2.17/gadapt/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.2.18/gadapt/immigration/population_immigration/common_population_immigrator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from typing import List
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.immigration.population_immigration.base_population_immigrator import BasePopulationImmigrator
 
 class CommonPopulationImmigrator(BasePopulationImmigrator):
 
+    """
+    Common class for the population immigration.
+    In kept part of the population lower ranked chromosomes are replaced with new ones
+    """
+    
     def immigrate(self, population):
         if population.options.immigration_number < 1:
             return
         keep_number = population.options.keep_number
         chromosome_list: List[Chromosome] = list(population.get_sorted(
             key=lambda c: c.cost_value))[:keep_number]
         chromosome_list = sorted(chromosome_list,
```

### Comparing `gadapt-0.2.17/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py` & `gadapt-0.2.18/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from typing import List
 import gadapt.ga_model.definitions as definitions
-class BaseChromosomeMutator:    
+class BaseChromosomeMutator:   
+
+    """
+    Base class for the mutation of chromosome.
+    Mutates specific genes in the chromosome.
+    """ 
     
     def mutate(self, c, number_of_mutation_genes: int):
         self.before_mutated(c)
         self.mutate_chromosome(c, number_of_mutation_genes)
         self.chromosome_mutated(c)
     
     def mutate_chromosome(self, c, number_of_mutation_genes: int):
```

### Comparing `gadapt-0.2.17/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py` & `gadapt-0.2.18/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import random
 from gadapt.mutation.chromosome_mutation.random_chromosome_mutator import RandomChromosomeMutator
 from gadapt.sampling.base_sampling import BaseSampling
 import gadapt.utils.ga_utils as ga_utils
 
 class CrossDiversityChromosomeMutator(RandomChromosomeMutator):
                     
+    """
+    Class for the mutation of chromosome based on cross diversity.
+    """ 
+    
     def __init__(self, sampling: BaseSampling) -> None:
         super().__init__()
         self.sampling = sampling
     
     def mutate_chromosome(self, c: Chromosome, number_of_mutation_genes: int):
         if number_of_mutation_genes == 0:
             return
```

### Comparing `gadapt-0.2.17/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.2.18/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.gene import Gene
 from typing import List
 import random
 
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 
+
 class RandomChromosomeMutator(BaseChromosomeMutator):
+
+    """
+    Class for the random mutation of chromosome.
+    """ 
     def mutate_chromosome(self, c: Chromosome, number_of_mutation_genes: int):
         if number_of_mutation_genes == 0:
             return
         genes_to_mutate = list(c)
         random.shuffle(genes_to_mutate)
         var_num = random.randint(1, number_of_mutation_genes)
         genes_to_mutate = genes_to_mutate[:var_num]
```

### Comparing `gadapt-0.2.17/gadapt/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.2.18/gadapt/mutation/population_mutation/base_population_mutator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import math
 import random
 from typing import List
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.ga_options import GAOptions
 import gadapt.ga_model.definitions as definitions
 class BasePopulationMutator:
+
+    """
+    Base class for mutating chromosomes in population
+    """
     
     def __init__(self, options: GAOptions) -> None:
         self.options = options
 
     def before_exit_check(self, population):
         pass
```

### Comparing `gadapt-0.2.17/gadapt/mutation/population_mutation/composed_population_mutator.py` & `gadapt-0.2.18/gadapt/mutation/population_mutation/composed_population_mutator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from ast import List
 import random
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
 
 class ComposedPopulationMutator(BasePopulationMutator):
+
+    """
+    Population mutator that consists of more different population mutators
+    """
         
     def __init__(self, options: GAOptions) -> None:
         super().__init__(options)
         self.mutators = []
             
     def append(self, mutator: BasePopulationMutator):
         self.mutators.append(mutator)
```

### Comparing `gadapt-0.2.17/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py` & `gadapt-0.2.18/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
 import gadapt.utils.ga_utils as ga_utils
 import statistics as stat
 import gadapt.ga_model.definitions as definitions
 
 class CostDiversityPopulationMutator(BasePopulationMutator):
         
+    """
+    Population mutator based on cost diversity
+    """
+    
     def __init__(self, options: GAOptions, population_mutator_for_execution: BasePopulationMutator) -> None:
         super().__init__(options)
         self.population_mutator_for_execution = population_mutator_for_execution
         self.first_cost = definitions.FLOAT_NAN
         
     @property
     def first_cost(self) -> float:
```

### Comparing `gadapt-0.2.17/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py` & `gadapt-0.2.18/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from ast import List
 import random
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
 from gadapt.sampling.base_sampling import BaseSampling
 
-class ParentsDiversityPopulationMutator(BasePopulationMutator):
+class ParentDiversityPopulationMutator(BasePopulationMutator):
+
+    """
+    Population mutator based on parent diversity
+    """
         
     def __init__(self, sampling: BaseSampling, options: GAOptions) -> None:
         super().__init__(options)
         self.sampling = sampling
             
     def sort_key_parent_diversity_random(self, c: Chromosome):
         return (c.parent_diversity, random.random())
```

### Comparing `gadapt-0.2.17/gadapt/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.2.18/gadapt/mutation/population_mutation/random_population_mutator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import random
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
 
 class RandomPopulationMutator(BasePopulationMutator):
+    
+    """
+    Random population mutator
+    """
+    
     def __init__(self, options: GAOptions) -> None:
         super().__init__(options)
 
     def get_number_of_mutation_cromosomes(self) -> int:
         return self.options.number_of_mutation_chromosomes
 
     def mutate_population(self, population, number_of_mutation_chromosomes):
```

### Comparing `gadapt-0.2.17/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.18/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.parent_selection.base_parent_selector import BaseParentSelector
 from gadapt.sampling.base_sampling import BaseSampling
 
 
 class SamplingParentSelector(BaseParentSelector):
 
+    """
+    Parent Selector based on sampling.
+    Sampling is the algorithm for extracting a sample from the population,
+    based on specific value of the chromosme.
+    In this case sampling depends on cost value.
+
+    Selects mates for mating from the population
+    """
+    
     def __init__(self, sampling: BaseSampling) -> None:
         super().__init__()
         self.sampling = sampling
 
     def select_mates(self, population) -> List[Tuple[Chromosome, Chromosome]]:
         working_chromosomes = self.sampling.get_sample(
             population.chromosomes, len(population), lambda c: c.cost_value)
```

### Comparing `gadapt-0.2.17/gadapt/sampling/base_sampling.py` & `gadapt-0.2.18/gadapt/sampling/base_sampling.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from typing import List
 from gadapt.ga_model.ranking_model import RankingModel
 import gadapt.ga_model.definitions as definitions
 class BaseSampling:
+
+    """
+    The algorithm for extracting a sample from the population.
+    """
+
     def get_sample(self, lst: List[RankingModel], max_num, sort_key=None) -> List[RankingModel]:
         if len(lst) == 0:
             return lst
         for m in lst:
             m.reset_for_sampling()
         if max_num < 1 or max_num > len(lst):
             self.max_num = len(lst)
```

### Comparing `gadapt-0.2.17/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.18/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import random
 from typing import List
 from gadapt.ga_model.ranking_model import RankingModel
 from gadapt.sampling.base_sampling import BaseSampling
 
 class RouletteWheelSampling(BaseSampling):
     
+    """
+    "RouletteWheel" (also known as "Weighted Random Pairing") algorithm for extracting a sample from the population.
+    """
+    
     def prepare_sample(self, lst: List[RankingModel]) -> List[RankingModel]:
         rank_sum = sum(range(1, len(lst) + 1))
         cummultative_probability_list: List[float] = []
         cummulative_probability = 0.0
         n_keep = len(lst)
         for j in range(len(lst)):
             n = n_keep - j
```

### Comparing `gadapt-0.2.17/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.18/gadapt/sampling/tournament_sampling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import random
 from typing import List
 from gadapt.ga_model.ranking_model import RankingModel
 from gadapt.sampling.base_sampling import BaseSampling
 
 class TournamentSampling(BaseSampling):
+
+    """
+    "Tournament" algorithm for extracting a sample from the population.
+    """
+
     def __init__(self, group_size = None) -> None:
         super().__init__()
         self.group_size = group_size
     
     def prepare_sample(self, lst: List[RankingModel]) -> List[RankingModel]:
         ls = []
         ls = sorted(lst, key=self.sort_key)
```

### Comparing `gadapt-0.2.17/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.18/gadapt/string_operation/ga_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import math
 
+"""
+Genetic algorithm string operations
+"""
+
 def gene_to_string(g):
     return str(g.genetic_variable.variable_id) + ": " + str(round(g.variable_value, 2))
 
 def chromosome_to_string(c):
     str_res = "Chromosome "
     id_str = str(c.chromosome_id)
     while len(id_str) < 4:
```

### Comparing `gadapt-0.2.17/gadapt/utils/ga_utils.py` & `gadapt-0.2.18/gadapt/utils/ga_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 
 from functools import reduce
 import math
 import random
 from typing import List
 import gadapt.ga_model.definitions as definitions
+
+"""
+Genetic algorithm utility
+"""
+
 def get_rand_bool():
     rand_int = random.getrandbits(1)
     return bool(rand_int)
 
 def get_rand_bool_with_probability(f: float):
     r = random.uniform(0, 1)
     if r <= f:
```

### Comparing `gadapt-0.2.17/gadapt/validation/base_options_validator.py` & `gadapt-0.2.18/gadapt/validation/base_options_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from typing import List, Tuple
 import gadapt.ga_model.message_levels as message_levels
 import gadapt.ga_model.definitions as definitions
 
 class BaseOptionsValidator:
+
+    """
+    Base class for options validation
+    """
     
     def __init__(self, options) -> None:
         self._validation_messages = []
         self.options = options
         self.success = True
     
     def validate(self) -> bool:
```

### Comparing `gadapt-0.2.17/gadapt/validation/common_options_validator.py` & `gadapt-0.2.18/gadapt/validation/common_options_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from gadapt.validation.base_options_validator import BaseOptionsValidator
 import gadapt.ga_model.definitions as definitions
 import gadapt.ga_model.definitions as definitions
 class CommonOptionsValidator(BaseOptionsValidator):
 
+    """
+    Common class for options validation
+    """
+
     def __init__(self, options) -> None:
         super().__init__(options)
         self._validation_messages = []        
 
     def validate(self):        
         self.success &= self.check_nones_types_and_values()
         self.success &= self.check_genetic_variables()
```

### Comparing `gadapt-0.2.17/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.18/gadapt/variable_update/common_variable_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import statistics as stat
 from gadapt.ga_model.genetic_variable import GeneticVariable
 import gadapt.utils.ga_utils as ga_utils
 
 class CommonVariableUpdater:
+
+    """
+    Common variable updater
+    """
+
     def update_variables(self, population):
         def scale_values(gv: GeneticVariable, values):
             rslt = []
             max_val = max(values)
             diff = (gv.max_value - max_val)
             if (gv.min_value < 0):
                 diff = diff - gv.min_value
```

### Comparing `gadapt-0.2.17/gadapt.egg-info/PKG-INFO` & `gadapt-0.2.18/gadapt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: gadapt
-Version: 0.2.17
+Version: 0.2.18
 Summary: GAdapt: A Python Library for Self-Adaptive Genetic Algorithm.
 Home-page: https://github.com/bpzoran/gadapt
 Author: Zoran Jankovic
 Author-email: bpzoran@yahoo.com
 License: UNKNOWN
 Description: # GAdapt: Self-Adaptive Genetic Algorithm
-        **GAdapt** (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
+        [GAdapt] (https://gadapt.com) is an open-source Python library for Genetic Algorithm optimization. It implements innovative concepts for the adaptive mutation of genes and chromosomes.
         
         # What innovations does GAdapt bring?
         **GAdapt** introduces self-adaptive determination of how many and which chromosomes and genes will be mutated. This determination is based on the diversity of parents, diversity of cost and cross-diversity of genetic variables in the population. Less diversity increases the probability of mutation. Consequently, it increases the accuracy and the performance of the optimization. Default settings provide a self-adaptive determination of mutation chromosomes and genes.
         
         
         # Installation
         To install **GAdapt**, use **pip** with the following command:
         
         ```
         pip install gadapt
         ```
         
         # Source Code
-        The source code is stored on GitHub at the following address: https://github.com/bpzoran/gadapt
+        The source code is stored on GitHub at the following address: [https://github.com/bpzoran/gadapt/] https://github.com/bpzoran/gadapt
+        
+        # API Documentation
+        The API documentation can be found on the following address: [https://www.gadapt.com/api/] https://www.gadapt.com/api
         
         # Getting started
         The following example optimizes variable values for a complex trigonometric function.
         ```python
         from gadapt.ga import GA
         import math
         
@@ -168,15 +171,15 @@
         - *"random"* - Random selection algorithm uses a uniform random number generator to select genes for mutation. In this case, selection for the mutation will not depend on gene cross-diversity.  
             
         **immigration_number**=*0* - Refers to the "Random Immigrants" concepts. This strategy introduces a certain number of individuals into the population during the evolution process. These new individuals are generated randomly and injected into the population.
         
         **logging**=*False* - If this parameter has a True value, the log file will be created in the current working directory. The log file contains the flow of genetic algorithm execution, along with values of chromosomes, genes and cost functions in each generation
         
         # Adding Variables
-        Variables to be optimized can be added by callning the *add* method of the *GA* object. Parameters of this method are the minimum value, the maximum value, and the step. The minimum and maximum value determine a range of possible variable values. The *step* parameter specifies the step that will be used in changing the variables values during the optimization.
+        Variables to be optimized can be added by calling the *add* method of the *GA* object. Parameters of this method are the minimum value, the maximum value, and the step. The minimum and maximum value determine a range of possible variable values. The *step* parameter specifies the step that will be used in changing the variables values during the optimization.
         
         For example:
         ```python
         ga.add(1.0, 4.0, 0.01)
         ```
         means that the corresponding parameter can have values between 1.0 and 4.0, and the step for changing variable values in optimization is 0.01.
```

### Comparing `gadapt-0.2.17/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.18/gadapt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -52,17 +52,14 @@
 gadapt/mutation/population_mutation/__init__.py
 gadapt/mutation/population_mutation/base_population_mutator.py
 gadapt/mutation/population_mutation/composed_population_mutator.py
 gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
 gadapt/mutation/population_mutation/random_population_mutator.py
 gadapt/mutation/population_mutation/cost_diversity/__init__.py
 gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
-gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
-gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
-gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
 gadapt/parent_selection/__init__.py
 gadapt/parent_selection/base_parent_selector.py
 gadapt/parent_selection/sampling_parent_selector.py
 gadapt/sampling/__init__.py
 gadapt/sampling/base_sampling.py
 gadapt/sampling/from_top_to_bottom_sampling.py
 gadapt/sampling/random_sampling.py
```


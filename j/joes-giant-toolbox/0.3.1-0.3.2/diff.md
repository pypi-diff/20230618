# Comparing `tmp/joes_giant_toolbox-0.3.1.tar.gz` & `tmp/joes_giant_toolbox-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joes_giant_toolbox-0.3.1.tar", last modified: Sat Jun 17 20:54:24 2023, max compression
+gzip compressed data, was "joes_giant_toolbox-0.3.2.tar", last modified: Sun Jun 18 09:48:10 2023, max compression
```

## Comparing `joes_giant_toolbox-0.3.1.tar` & `joes_giant_toolbox-0.3.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.030395 joes_giant_toolbox-0.3.1/
--rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.3.1/LICENSE
--rw-r--r--   0 josephbolton   (501) staff       (20)    60529 2023-06-17 20:54:24.030156 joes_giant_toolbox-0.3.1/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)    19249 2023-06-15 14:31:57.000000 joes_giant_toolbox-0.3.1/README.md
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.011605 joes_giant_toolbox-0.3.1/joes_giant_toolbox/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/__init__.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.024752 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/__init__.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/ascii_density_histogram.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     9531 2023-04-30 11:40:27.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/compare_metric_to_prev_period.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      720 2023-06-06 19:54:23.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/cosine_similarity.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10222 2023-06-14 09:08:13.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    11774 2023-06-17 20:38:49.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_parallel_google_cloud_run_job_template.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_project_scope_doc.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/duckduckgo_search_multipage.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     3585 2023-06-15 14:32:03.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/gcloud_vm_deletes_itself.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2791 2023-06-11 19:39:57.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/list_all_python_imports.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1098 2023-05-30 08:06:59.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/manual_keyword_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/print_progress_bar.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2117 2023-04-27 07:33:31.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/python_plotting_tutorials.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     8743 2023-05-07 19:34:54.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/regex_rules_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4776 2023-05-30 08:19:34.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/run_python_function_in_parallel.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    13751 2023-05-06 11:30:11.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/string_cleaner.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1793 2023-06-11 19:47:40.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/view_nested_dict_structure.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2804 2023-05-30 08:07:39.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      496 2023-05-30 08:02:52.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/convenience.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/dataviz.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1635 2023-06-15 14:31:51.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/google_cloud.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.027439 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/
--rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/ascii_barplot.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/query_wikipedia_api.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/recsys_data_simulator.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      205 2023-06-04 10:41:28.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/maths.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/proj_mgmt.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/sklearn.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/stats.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      450 2023-05-03 07:44:37.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/text.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox/web.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.012630 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/
--rw-r--r--   0 josephbolton   (501) staff       (20)    60529 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)     2870 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)      215 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/requires.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-06-17 20:54:24.000000 joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/top_level.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)     1118 2023-06-17 20:46:17.000000 joes_giant_toolbox-0.3.1/pyproject.toml
--rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-06-17 20:54:24.030448 joes_giant_toolbox-0.3.1/setup.cfg
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-17 20:54:24.029591 joes_giant_toolbox-0.3.1/tests/
--rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.3.1/tests/test_conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.3.1/tests/test_longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.3.1/tests/test_make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.3.1/tests/test_rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.3.1/tests/test_string_cleaner.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-18 09:48:10.536295 joes_giant_toolbox-0.3.2/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.3.2/LICENSE
+-rw-r--r--   0 josephbolton   (501) staff       (20)    60529 2023-06-18 09:48:10.536053 joes_giant_toolbox-0.3.2/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)    19249 2023-06-18 09:47:37.000000 joes_giant_toolbox-0.3.2/README.md
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-18 09:48:10.521044 joes_giant_toolbox-0.3.2/joes_giant_toolbox/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/__init__.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-18 09:48:10.531751 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/__init__.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/ascii_density_histogram.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     9531 2023-04-30 11:40:27.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/compare_metric_to_prev_period.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      720 2023-06-06 19:54:23.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/cosine_similarity.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10222 2023-06-14 09:08:13.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    11778 2023-06-18 09:46:02.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/create_parallel_google_cloud_run_job_template.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/create_project_scope_doc.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/duckduckgo_search_multipage.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3585 2023-06-15 14:32:03.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/gcloud_vm_deletes_itself.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2791 2023-06-11 19:39:57.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/list_all_python_imports.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1098 2023-05-30 08:06:59.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/manual_keyword_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/print_progress_bar.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2117 2023-04-27 07:33:31.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/python_plotting_tutorials.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8743 2023-05-07 19:34:54.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/regex_rules_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4776 2023-05-30 08:19:34.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/run_python_function_in_parallel.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    13751 2023-05-06 11:30:11.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/string_cleaner.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1793 2023-06-11 19:47:40.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/view_nested_dict_structure.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2804 2023-05-30 08:07:39.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      496 2023-05-30 08:02:52.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/convenience.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/dataviz.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1635 2023-06-15 14:31:51.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/google_cloud.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-18 09:48:10.533754 joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/ascii_barplot.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/query_wikipedia_api.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/recsys_data_simulator.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      205 2023-06-04 10:41:28.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/maths.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/proj_mgmt.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/sklearn.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/stats.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      450 2023-05-03 07:44:37.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/text.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox/web.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-18 09:48:10.522208 joes_giant_toolbox-0.3.2/joes_giant_toolbox.egg-info/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    60529 2023-06-18 09:48:10.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2870 2023-06-18 09:48:10.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-06-18 09:48:10.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)      215 2023-06-18 09:48:10.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox.egg-info/requires.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-06-18 09:48:10.000000 joes_giant_toolbox-0.3.2/joes_giant_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1118 2023-06-18 09:46:43.000000 joes_giant_toolbox-0.3.2/pyproject.toml
+-rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-06-18 09:48:10.536345 joes_giant_toolbox-0.3.2/setup.cfg
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-06-18 09:48:10.535548 joes_giant_toolbox-0.3.2/tests/
+-rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.3.2/tests/test_conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.3.2/tests/test_longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.3.2/tests/test_make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.3.2/tests/test_rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.3.2/tests/test_string_cleaner.py
```

### Comparing `joes_giant_toolbox-0.3.1/LICENSE` & `joes_giant_toolbox-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/PKG-INFO` & `joes_giant_toolbox-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joes_giant_toolbox
-Version: 0.3.1
+Version: 0.3.2
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -756,15 +756,15 @@
 
 * [Text and Natural Language Processing](#text-and-natural-language-processing)
 
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
+| anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         4        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 | cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | create_parallel_google_cloud_run_job_template | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
 | create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
```

### Comparing `joes_giant_toolbox-0.3.1/README.md` & `joes_giant_toolbox-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 * [Text and Natural Language Processing](#text-and-natural-language-processing)
 
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
+| anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         4        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 | cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | create_parallel_google_cloud_run_job_template | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
 | create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
```

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/ascii_density_histogram.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/ascii_density_histogram.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/compare_metric_to_prev_period.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/compare_metric_to_prev_period.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/cosine_similarity.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/create_gcloud_vm_docker_template.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_parallel_google_cloud_run_job_template.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/create_parallel_google_cloud_run_job_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     ...     task_code=[
     ...         "joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket(",
     ...         '   contents_str=f"batch {BATCH_ID}, item {item_idx}",',
     ...         '   bucket_name="cloud_run_jobs_test",',
     ...         '   filename_on_bucket=f"completed_files/{item}.txt",',
     ...         '   file_type="text"',
     ...         ")",
-    ...         "time.sleep( random.uniform(1,5) )",
+    ...         "time.sleep( random.uniform(0.1,0.5) )",
     ...     ],
     ...     target_dir=code_output_dir,
     ...     gcp_region="europe-west2",
     ...     cloud_run_job_name="temp-once-off-job",
     ...     instruction_file_bucket_name="cloud_run_jobs_test",
     ...     instruction_file_path="names_to_process.txt",
     ...     requirements_list=[
```

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/create_project_scope_doc.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/create_project_scope_doc.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/duckduckgo_search_multipage.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/duckduckgo_search_multipage.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/gcloud_vm_deletes_itself.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/gcloud_vm_deletes_itself.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/list_all_python_imports.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/list_all_python_imports.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/make_url_request.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/print_progress_bar.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/print_progress_bar.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/python_plotting_tutorials.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/python_plotting_tutorials.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/rapid_binary_classifier.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/regex_rules_classifier.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/regex_rules_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/run_python_function_in_parallel.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/run_python_function_in_parallel.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/string_cleaner.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/view_nested_dict_structure.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/view_nested_dict_structure.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/google_cloud.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/google_cloud.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/ascii_barplot.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/ascii_barplot.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/in_progress/recsys_data_simulator.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/in_progress/recsys_data_simulator.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox/web.py` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox/web.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/PKG-INFO` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joes-giant-toolbox
-Version: 0.3.1
+Version: 0.3.2
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -756,15 +756,15 @@
 
 * [Text and Natural Language Processing](#text-and-natural-language-processing)
 
 ..or you can just scroll through the master list:
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
-| anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         2        |
+| anonymous_view_public_linkedin_page               | Extracts the information (HTML) from a public LinkedIn page (e.g. person or company) using a virtual browser |         4        |
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 | cosine_similarity                                 | Calculates the cosine similarity between two 1-dimensional numpy arrays | 2 |
 | create_gcloud_vm_docker_template | Creates a folder containing the files necessary to quickly build a python docker container to run on a google cloud Virtual Machine | 4
 | create_parallel_google_cloud_run_job_template | Run a task in parallel using a Google Cloud Run job (code-generating function)| 2 |
 | create_project_scope_doc                          | Creates a basic project scope document (markdown) by prompting the user for input                            |         3        |
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
```

### Comparing `joes_giant_toolbox-0.3.1/joes_giant_toolbox.egg-info/SOURCES.txt` & `joes_giant_toolbox-0.3.2/joes_giant_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/pyproject.toml` & `joes_giant_toolbox-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "joes_giant_toolbox"
-version = "0.3.01"
+version = "0.3.02"
 description = "A large collection of general python functions and classes that I use in my daily work"
 readme = "README.md"
 authors = [{ name = "Joseph Bolton", email = "joseph.jazz.bolton@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `joes_giant_toolbox-0.3.1/tests/test_conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.3.2/tests/test_conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/tests/test_longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.3.2/tests/test_longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/tests/test_make_url_request.py` & `joes_giant_toolbox-0.3.2/tests/test_make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/tests/test_rapid_binary_classifier.py` & `joes_giant_toolbox-0.3.2/tests/test_rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.3.1/tests/test_string_cleaner.py` & `joes_giant_toolbox-0.3.2/tests/test_string_cleaner.py`

 * *Files identical despite different names*


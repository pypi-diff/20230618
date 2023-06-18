# Comparing `tmp/khoj_assistant-0.6.3.dev53.tar.gz` & `tmp/khoj_assistant-0.6.3.dev64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Jun 17 06:58:47 2023, max compression
+gzip compressed data, last modified: Sun Jun 18 09:21:32 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev53.tar` & `khoj_assistant-0.6.3.dev64.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/__init__.py
--rw-r--r--   0        0        0    10845 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17706 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0     9707 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0      546 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0    12314 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0      437 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/config.css
--rw-r--r--   0        0        0     4526 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/config.js
--rw-r--r--   0        0        0   275822 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    26348 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0   162910 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-144x144.ico
--rw-r--r--   0        0        0    29325 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-144x144.png
--rw-r--r--   0        0        0   113060 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     3815 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    11901 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0      803 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3027 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4008 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1239 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/LICENSE
--rw-r--r--   0        0        0    22877 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/README.md
--rw-r--r--   0        0        0     2783 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/pyproject.toml
--rw-r--r--   0        0        0    25217 2023-06-17 06:58:47.000000 khoj_assistant-0.6.3.dev53/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10845 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17706 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0     9707 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0      546 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0    12523 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0      437 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/config.css
+-rw-r--r--   0        0        0     4526 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/config.js
+-rw-r--r--   0        0        0   275822 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    26348 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0   162910 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-144x144.ico
+-rw-r--r--   0        0        0    29325 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-144x144.png
+-rw-r--r--   0        0        0   113060 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     6985 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    11901 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0      803 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3027 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4008 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1239 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/LICENSE
+-rw-r--r--   0        0        0    22877 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/README.md
+-rw-r--r--   0        0        0     2785 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/pyproject.toml
+-rw-r--r--   0        0        0    25217 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev64/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/main.py` & `khoj_assistant-0.6.3.dev64/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
             var orgHTMLDocument = orgDocument.convert(Org.ConverterHTML, { htmlClassPrefix: classPrefix });
             return orgHTMLDocument.toString();
         }
 
         function render_markdown(query, data) {
             var md = window.markdownit();
             return md.render(data.map(function (item) {
+                lines = item.entry.split("\n")
+                if (item.additional.file.startsWith("http"))
+                    return `${lines[0]}\t[*](${item.additional.file})\n${lines.slice(1).join("\n")}`
                 return `${item.entry}`
             }).join("\n"));
         }
 
         function render_ledger(query, data) {
             return `<div id="results-ledger">` + data.map(function (item) {
                 return `<p>${item.entry}</p>`
```

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/config.js` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/config.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-144x144.ico` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-144x144.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon-144x144.png` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-144x144.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev64/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev64/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev64/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev64/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev64/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev64/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev64/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev64/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev64/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev64/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/.gitignore` & `khoj_assistant-0.6.3.dev64/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/LICENSE` & `khoj_assistant-0.6.3.dev64/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/README.md` & `khoj_assistant-0.6.3.dev64/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev53/pyproject.toml` & `khoj_assistant-0.6.3.dev64/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "schedule == 1.1.0",
     "sentence-transformers == 2.2.2",
     "torch == 1.13.1",
     "uvicorn == 0.17.6",
     "aiohttp == 3.8.4",
     "langchain >= 0.0.187",
     "pypdf >= 3.9.0",
-    "llama-hub==0.0.3",
+    "requests >= 2.26.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/debanjum/khoj#readme"
 Issues = "https://github.com/debanjum/khoj/issues"
 Discussions = "https://github.com/debanjum/khoj/discussions"
```

### Comparing `khoj_assistant-0.6.3.dev53/PKG-INFO` & `khoj_assistant-0.6.3.dev64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev53
+Version: 0.6.3.dev64
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/debanjum/khoj#readme
 Project-URL: Issues, https://github.com/debanjum/khoj/issues
 Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
 Project-URL: Releases, https://github.com/debanjum/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -24,21 +24,21 @@
 Requires-Python: <3.11,>=3.8
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: dateparser==1.1.1
 Requires-Dist: defusedxml==0.7.1
 Requires-Dist: fastapi==0.77.1
 Requires-Dist: jinja2==3.1.2
 Requires-Dist: langchain>=0.0.187
-Requires-Dist: llama-hub==0.0.3
 Requires-Dist: openai>=0.27.0
 Requires-Dist: pillow==9.3.0
 Requires-Dist: pydantic>=1.9.1
 Requires-Dist: pypdf>=3.9.0
 Requires-Dist: pyqt6==6.3.1
 Requires-Dist: pyyaml==6.0
+Requires-Dist: requests>=2.26.0
 Requires-Dist: rich>=13.3.1
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentence-transformers==2.2.2
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: tiktoken>=0.3.0
 Requires-Dist: torch==1.13.1
 Requires-Dist: uvicorn==0.17.6
```


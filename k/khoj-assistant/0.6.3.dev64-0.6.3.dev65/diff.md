# Comparing `tmp/khoj_assistant-0.6.3.dev64.tar.gz` & `tmp/khoj_assistant-0.6.3.dev65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jun 18 09:21:32 2023, max compression
+gzip compressed data, last modified: Sun Jun 18 09:26:03 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev64.tar` & `khoj_assistant-0.6.3.dev65.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/__init__.py
--rw-r--r--   0        0        0    10845 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17706 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0     9707 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0      546 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0    12523 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0      437 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/config.css
--rw-r--r--   0        0        0     4526 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/config.js
--rw-r--r--   0        0        0   275822 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    26348 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0   162910 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-144x144.ico
--rw-r--r--   0        0        0    29325 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-144x144.png
--rw-r--r--   0        0        0   113060 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     6985 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    11901 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0      803 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3027 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4008 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1239 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/LICENSE
--rw-r--r--   0        0        0    22877 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/README.md
--rw-r--r--   0        0        0     2785 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/pyproject.toml
--rw-r--r--   0        0        0    25217 2023-06-18 09:21:32.000000 khoj_assistant-0.6.3.dev64/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10848 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17706 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0     9707 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0      546 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0    12550 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0      437 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/config.css
+-rw-r--r--   0        0        0     4526 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/config.js
+-rw-r--r--   0        0        0   275822 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    26348 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0   162910 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-144x144.ico
+-rw-r--r--   0        0        0    29325 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-144x144.png
+-rw-r--r--   0        0        0   113060 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     6985 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    11901 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0      803 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3027 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4008 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1239 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/LICENSE
+-rw-r--r--   0        0        0    22877 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/README.md
+-rw-r--r--   0        0        0     2785 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/pyproject.toml
+-rw-r--r--   0        0        0    25217 2023-06-18 09:26:03.000000 khoj_assistant-0.6.3.dev65/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev65/src/khoj/configure.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             search_config=config.search_type.symmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter(), FileFilter()],
         )
 
     # Initialize PDF Search
     if (t == state.SearchType.Pdf or t == None) and config.content_type.pdf:
-        logger.info("💸 Setting up search for pdf")
+        logger.info("🖨️ Setting up search for pdf")
         # Extract Entries, Generate PDF Embeddings
         model.pdf_search = text_search.setup(
             PdfToJsonl,
             config.content_type.pdf,
             search_config=config.search_type.asymmetric,
             regenerate=regenerate,
             filters=[DateFilter(), WordFilter(), FileFilter()],
```

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/main.py` & `khoj_assistant-0.6.3.dev65/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/config.html` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,19 @@
             var orgHTMLDocument = orgDocument.convert(Org.ConverterHTML, { htmlClassPrefix: classPrefix });
             return orgHTMLDocument.toString();
         }
 
         function render_markdown(query, data) {
             var md = window.markdownit();
             return md.render(data.map(function (item) {
-                lines = item.entry.split("\n")
-                if (item.additional.file.startsWith("http"))
-                    return `${lines[0]}\t[*](${item.additional.file})\n${lines.slice(1).join("\n")}`
-                return `${item.entry}`
+                if (item.additional.file.startsWith("http")) {
+                    lines = item.entry.split("\n");
+                    return `${lines[0]}\t[*](${item.additional.file})\n${lines.slice(1).join("\n")}`;
+                }
+                return `${item.entry}`;
             }).join("\n"));
         }
 
         function render_ledger(query, data) {
             return `<div id="results-ledger">` + data.map(function (item) {
                 return `<p>${item.entry}</p>`
             }).join("\n") + `</div>`;
```

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/config.js` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/config.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-144x144.ico` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-144x144.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon-144x144.png` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon-144x144.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev65/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev65/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev65/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev65/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev65/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev65/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev65/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev65/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev65/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev65/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev65/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/.gitignore` & `khoj_assistant-0.6.3.dev65/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/LICENSE` & `khoj_assistant-0.6.3.dev65/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/README.md` & `khoj_assistant-0.6.3.dev65/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/pyproject.toml` & `khoj_assistant-0.6.3.dev65/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev64/PKG-INFO` & `khoj_assistant-0.6.3.dev65/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev64
+Version: 0.6.3.dev65
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/debanjum/khoj#readme
 Project-URL: Issues, https://github.com/debanjum/khoj/issues
 Project-URL: Discussions, https://github.com/debanjum/khoj/discussions
 Project-URL: Releases, https://github.com/debanjum/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```


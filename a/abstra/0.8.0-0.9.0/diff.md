# Comparing `tmp/abstra-0.8.0.tar.gz` & `tmp/abstra-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/abstra-0.8.0.tar", last modified: Fri Mar 17 14:32:18 2023, max compression
+gzip compressed data, was "dist/abstra-0.9.0.tar", last modified: Fri Mar 17 14:49:52 2023, max compression
```

## Comparing `abstra-0.8.0.tar` & `abstra-0.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:32:18.000000 abstra-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-17 14:32:18.000000 abstra-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-17 14:32:05.000000 abstra-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/dashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra/widgets/library/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/AnswerSheetInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/CardsInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/CheckboxInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/ChecklistInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/ClickInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/CnpjInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/CodeInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/CpfInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/CurrencyInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/DateInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/DropdownInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/EmailInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/FileInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/FileOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/HtmlOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/IframeOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/ImageInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/ImageOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/KanbanBoardInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/LatexOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/LinkOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/ListInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/MarkdownOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/MultipleChoiceInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/NpsInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/NumberInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/NumberSliderInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/PandasOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/PandasRowSelectionInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/PasswordInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/PhoneInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/PlotlyOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/ProgressOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/RatingInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/TagInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/TextInput.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/TextOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/TextareaInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/TimeInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/ToggleInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/VideoInput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/library/widget_base.py
--rw-r--r--   0 runner    (1001) docker     (123)   280192 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/response_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/widget_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-17 14:32:05.000000 abstra-0.8.0/abstra/widgets/widget_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 14:32:18.000000 abstra-0.8.0/abstra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 14:32:18.000000 abstra-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-17 14:32:05.000000 abstra-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-17 14:49:52.000000 abstra-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-17 14:49:37.000000 abstra-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/abstra/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/dashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/abstra/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/abstra/widgets/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/AnswerSheetInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CardsInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CheckboxInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ChecklistInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ClickInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CnpjInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CodeInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CpfInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/CurrencyInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/DateInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/DropdownInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/EmailInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/FileInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/FileOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/HtmlOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/IframeOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ImageInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ImageOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/KanbanBoardInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/LatexOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/LinkOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ListInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/MarkdownOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/MultipleChoiceInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/NpsInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/NumberInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/NumberSliderInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PandasOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PandasRowSelectionInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PasswordInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PhoneInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/PlotlyOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ProgressOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/RatingInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TagInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TextInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TextOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TextareaInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/TimeInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/ToggleInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/VideoInput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/library/widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   280192 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/response_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-17 14:49:37.000000 abstra-0.9.0/abstra/widgets/widget_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 14:49:52.000000 abstra-0.9.0/abstra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 14:49:51.000000 abstra-0.9.0/abstra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 14:49:52.000000 abstra-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-17 14:49:37.000000 abstra-0.9.0/setup.py
```

### Comparing `abstra-0.8.0/PKG-INFO` & `abstra-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstra
-Version: 0.8.0
+Version: 0.9.0
 Summary: Abstra Lib
 Home-page: https://github.com/abstra-app/abstra-lib
 License: MIT
 Description: [![pypi](https://img.shields.io/pypi/v/abstra.svg)](https://pypi.python.org/pypi/abstra)
         [![PyPI Downloads](https://img.shields.io/pypi/dm/abstra.svg)](https://pypi.org/project/abstra/)
         [![Code check](https://github.com/abstra-app/abstra-lib/actions/workflows/code_check.yml/badge.svg)](https://github.com/abstra-app/abstra-lib/actions/workflows/code_check.yml)
```

### Comparing `abstra-0.8.0/README.md` & `abstra-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/connectors.py` & `abstra-0.9.0/abstra/connectors.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/hooks.py` & `abstra-0.9.0/abstra/hooks.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/tables.py` & `abstra-0.9.0/abstra/tables.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/apis.py` & `abstra-0.9.0/abstra/widgets/apis.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/file_utils.py` & `abstra-0.9.0/abstra/widgets/file_utils.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/AnswerSheetInput.py` & `abstra-0.9.0/abstra/widgets/library/AnswerSheetInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/CardsInput.py` & `abstra-0.9.0/abstra/widgets/library/CardsInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/CheckboxInput.py` & `abstra-0.9.0/abstra/widgets/library/CheckboxInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/ChecklistInput.py` & `abstra-0.9.0/abstra/widgets/library/ChecklistInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/ClickInput.py` & `abstra-0.9.0/abstra/widgets/library/ClickInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/CnpjInput.py` & `abstra-0.9.0/abstra/widgets/library/CnpjInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/CodeInput.py` & `abstra-0.9.0/abstra/widgets/library/CodeInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/CpfInput.py` & `abstra-0.9.0/abstra/widgets/library/CpfInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/CurrencyInput.py` & `abstra-0.9.0/abstra/widgets/library/CurrencyInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/DateInput.py` & `abstra-0.9.0/abstra/widgets/library/DateInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/DropdownInput.py` & `abstra-0.9.0/abstra/widgets/library/DropdownInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/EmailInput.py` & `abstra-0.9.0/abstra/widgets/library/EmailInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/FileInput.py` & `abstra-0.9.0/abstra/widgets/library/FileInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/FileOutput.py` & `abstra-0.9.0/abstra/widgets/library/FileOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/IframeOutput.py` & `abstra-0.9.0/abstra/widgets/library/IframeOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/ImageInput.py` & `abstra-0.9.0/abstra/widgets/library/ImageInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/ImageOutput.py` & `abstra-0.9.0/abstra/widgets/library/ImageOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/KanbanBoardInput.py` & `abstra-0.9.0/abstra/widgets/library/KanbanBoardInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/LinkOutput.py` & `abstra-0.9.0/abstra/widgets/library/LinkOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/ListInput.py` & `abstra-0.9.0/abstra/widgets/library/ListInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/MultipleChoiceInput.py` & `abstra-0.9.0/abstra/widgets/library/MultipleChoiceInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/NpsInput.py` & `abstra-0.9.0/abstra/widgets/library/NpsInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/NumberInput.py` & `abstra-0.9.0/abstra/widgets/library/NumberInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/NumberSliderInput.py` & `abstra-0.9.0/abstra/widgets/library/NumberSliderInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/PandasOutput.py` & `abstra-0.9.0/abstra/widgets/library/PandasOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/PandasRowSelectionInput.py` & `abstra-0.9.0/abstra/widgets/library/PandasRowSelectionInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/PasswordInput.py` & `abstra-0.9.0/abstra/widgets/library/PasswordInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/PhoneInput.py` & `abstra-0.9.0/abstra/widgets/library/PhoneInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/PlotlyOutput.py` & `abstra-0.9.0/abstra/widgets/library/PlotlyOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/ProgressOutput.py` & `abstra-0.9.0/abstra/widgets/library/ProgressOutput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/RatingInput.py` & `abstra-0.9.0/abstra/widgets/library/RatingInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/TagInput.py` & `abstra-0.9.0/abstra/widgets/library/TagInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/TextInput.py` & `abstra-0.9.0/abstra/widgets/library/TextInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/TextareaInput.py` & `abstra-0.9.0/abstra/widgets/library/TextareaInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/TimeInput.py` & `abstra-0.9.0/abstra/widgets/library/TimeInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/ToggleInput.py` & `abstra-0.9.0/abstra/widgets/library/ToggleInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/VideoInput.py` & `abstra-0.9.0/abstra/widgets/library/VideoInput.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/library/__init__.py` & `abstra-0.9.0/abstra/widgets/library/__init__.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/metadata.py` & `abstra-0.9.0/abstra/widgets/metadata.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/response_types.py` & `abstra-0.9.0/abstra/widgets/response_types.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/types.py` & `abstra-0.9.0/abstra/widgets/types.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra/widgets/validation.py` & `abstra-0.9.0/abstra/widgets/validation.py`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/abstra.egg-info/PKG-INFO` & `abstra-0.9.0/abstra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstra
-Version: 0.8.0
+Version: 0.9.0
 Summary: Abstra Lib
 Home-page: https://github.com/abstra-app/abstra-lib
 License: MIT
 Description: [![pypi](https://img.shields.io/pypi/v/abstra.svg)](https://pypi.python.org/pypi/abstra)
         [![PyPI Downloads](https://img.shields.io/pypi/dm/abstra.svg)](https://pypi.org/project/abstra/)
         [![Code check](https://github.com/abstra-app/abstra-lib/actions/workflows/code_check.yml/badge.svg)](https://github.com/abstra-app/abstra-lib/actions/workflows/code_check.yml)
```

### Comparing `abstra-0.8.0/abstra.egg-info/SOURCES.txt` & `abstra-0.9.0/abstra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abstra-0.8.0/setup.py` & `abstra-0.9.0/setup.py`

 * *Files identical despite different names*


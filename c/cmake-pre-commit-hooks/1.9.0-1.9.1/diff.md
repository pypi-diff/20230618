# Comparing `tmp/cmake_pre_commit_hooks-1.9.0.tar.gz` & `tmp/cmake_pre_commit_hooks-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmake_pre_commit_hooks-1.9.0.tar", last modified: Wed May 24 18:52:10 2023, max compression
+gzip compressed data, was "cmake_pre_commit_hooks-1.9.1.tar", last modified: Sun Jun 18 10:20:02 2023, max compression
```

## Comparing `cmake_pre_commit_hooks-1.9.0.tar` & `cmake_pre_commit_hooks-1.9.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.codespell.allow
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.421768 cmake_pre_commit_hooks-1.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.421768 cmake_pre_commit_hooks-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/draft_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_call_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_cmake.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/clang_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/clang_tidy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/cppcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/cpplint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/include_what_you_use.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1738 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/lizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 18:52:10.000000 cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/misc/license_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 18:52:10.429768 cmake_pre_commit_hooks-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/sonar-project.properties
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/bad.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/.pre-commit-win.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/cmake_good/good.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:52:10.425768 cmake_pre_commit_hooks-1.9.0/tests/python/
--rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_argparse_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_call_process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_cmake_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/clang_format_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/clang_tidy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/cppcheck_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/cpplint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/iwyu_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/python/lizard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/run_tests.ps1
--rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-05-24 18:52:01.000000 cmake_pre_commit_hooks-1.9.0/tests/run_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.817317 cmake_pre_commit_hooks-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.codespell.allow
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.809317 cmake_pre_commit_hooks-1.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.809317 cmake_pre_commit_hooks-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/draft_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-06-18 10:20:02.817317 cmake_pre_commit_hooks-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.809317 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_call_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_cmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/clang_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/clang_tidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/cppcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/cpplint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/include_what_you_use.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1738 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/lizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-18 10:20:02.000000 cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/misc/license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-18 10:20:02.817317 cmake_pre_commit_hooks-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/sonar-project.properties
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/bad.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.813317 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/.pre-commit-win.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/cmake_good/good.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:20:02.817317 cmake_pre_commit_hooks-1.9.1/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_argparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_call_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18568 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_cmake_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/clang_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/clang_tidy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/cppcheck_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/cpplint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/iwyu_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/python/lizard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/run_tests.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-06-18 10:19:51.000000 cmake_pre_commit_hooks-1.9.1/tests/run_tests.sh
```

### Comparing `cmake_pre_commit_hooks-1.9.0/.github/workflows/ci.yml` & `cmake_pre_commit_hooks-1.9.1/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -131,16 +131,20 @@
 
           Write-Output 'Import-Module "${ENV:ChocolateyInstall}\helpers\chocolateyProfile.psm1"' | Out-File -FilePath $PROFILE -Append -Encoding utf8
           Write-Output 'Update-SessionEnvironment' | Out-File -FilePath $PROFILE -Append -Encoding utf8
           Write-Output '$id = vswhere -property instanceId' | Out-File -FilePath $PROFILE -Append -Encoding utf8
           Write-Output 'Import-Module "C:\Program Files\Microsoft Visual Studio\2022\Enterprise\Common7\Tools\Microsoft.VisualStudio.DevShell.dll"' `
           | Out-File -FilePath $PROFILE -Append -Encoding utf8
           Write-Output 'Enter-VsDevShell -InstanceId $id' | Out-File -FilePath $PROFILE -Append -Encoding utf8
+          Write-Output 'Set-Location -Path "${ENV:GITHUB_WORKSPACE}"' | Out-File -FilePath $PROFILE -Append -Encoding utf8
+          Get-Content -Path $PROFILE
 
           . $PROFILE
+          Get-Location
+
           Write-Output "CMAKE_PREFIX_PATH=$env:PATH" | Out-File -FilePath $env:GITHUB_ENV -Encoding utf8 -Append
 
           python -m pip install pre-commit cpplint lizard
 
           Get-Command @("python", "clang-format", "clang-tidy", "cppcheck", "cpplint", "lizard", "pre-commit")
 
       - name: Build and install package
```

### Comparing `cmake_pre_commit_hooks-1.9.0/.github/workflows/codeql-analysis.yml` & `cmake_pre_commit_hooks-1.9.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/.github/workflows/draft_release.yml` & `cmake_pre_commit_hooks-1.9.1/.github/workflows/draft_release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -12,49 +12,45 @@
 jobs:
   new-release:
     name: "Draft a new release"
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
 
-      - name: Create release branch
-        run: |
-          git checkout -b release/${{ github.event.inputs.tag }}
-
-      - name: Update changelog
-        uses: thomaseizinger/keep-a-changelog-new-release@1.3.0
+      - name: Setup Python
+        uses: actions/setup-python@v3
         with:
-          version: ${{ github.event.inputs.tag }}
+          python-version: '3.11'
+          cache: 'pip'
+          cache-dependency-path: '**/setup.cfg'
 
-      - name: Initialize mandatory git config
+      - name: Update CHANGELOG
         run: |
-          git config user.name "GitHub actions"
-          git config user.email noreply@github.com
+          python3 -m pip install mdformat-gfm 'git+https://github.com/Takishima/keepachangelog@v1.0.1'
+          python3 -m keepachangelog release "${{ github.event.inputs.tag }}"
+          python3 -m mdformat CHANGELOG.md
 
-      - name: Commit changelog and manifest files
+      - name: Commit changes
+        uses: stefanzweifel/git-auto-commit-action@v4
         id: make-commit
-        run: |
-          git add CHANGELOG.md
-          git commit --message "Preparing release ${{ github.event.inputs.tag }}"
-          echo "::set-output name=commit::$(git rev-parse HEAD)"
-
-      - name: Push new branch
-        run: git push origin release/${{ github.event.inputs.tag }}
+        with:
+          branch: release/${{ github.event.inputs.tag }}
+          create_branch: true
+          file_pattern: 'CHANGELOG.md'
+          commit_message: Preparing release ${{ github.event.inputs.tag }}
+          commit_author: github-actions[bot] <noreply@github.com>
 
       # yamllint disable rule:line-length
       - name: Create pull request
         uses: thomaseizinger/create-pull-request@1.3.0
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           head: release/${{ github.event.inputs.tag }}
           base: main
           title: Release version ${{ github.event.inputs.tag }}
           reviewers: ${{ github.actor }}
-          # Write a nice message to the user.
-          # We are claiming things here based on the `publish-new-release.yml` workflow.
-          # You should obviously adopt it to say the truth depending on your release workflow :)
           body: |
             Hi @${{ github.actor }}!
             This PR was created in response to a manual trigger of the release workflow here: https://github.com/${{ github.repository }}/actions/runs/${{ github.run_id }}.
-            I've updated the changelog and bumped the versions in the manifest files in this commit: ${{ steps.make-commit.outputs.commit }}.
+            I've updated the changelog and bumped the versions in the manifest files in this commit: ${{ steps.make-commit.outputs.commit_hash }}.
             Merging this PR will create a GitHub release and upload any assets that are created as part of the release build.
```

### Comparing `cmake_pre_commit_hooks-1.9.0/.github/workflows/format.yml` & `cmake_pre_commit_hooks-1.9.1/.github/workflows/format.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,29 +18,29 @@
       && (startsWith(github.event.pull_request.head.ref, 'release/')
           || startsWith(github.event.pull_request.head.ref, 'hotfix/'))
     steps:
       - uses: actions/checkout@v3
       - name: Installing parse-changelog
         env:
           target: x86_64-unknown-linux-musl
-          parse_changelog_tag: v0.5.1
+          parse_changelog_tag: v0.5.4
           source_url: https://github.com/taiki-e/parse-changelog/releases/download
         run: |
           curl -LsSf "${source_url}/${parse_changelog_tag}/parse-changelog-${target}.tar.gz" | tar xzf -
       - name: Extract version from branch name (for release branches)
         if: github.event_name == 'pull_request' && startsWith(github.event.pull_request.head.ref, 'release/')
         run: |
           BRANCH_NAME="${{ github.event.pull_request.head.ref }}"
-          VERSION=${BRANCH_NAME#release/}
+          VERSION=${BRANCH_NAME#release/v}
           echo "RELEASE_VERSION=$VERSION" >> $GITHUB_ENV
           git tag v${RELEASE_VERSION}
 
       - name: Extract version from branch name (for hotfix branches)
         if: github.event_name == 'pull_request'  && startsWith(github.event.pull_request.head.ref, 'hotfix/')
         run: |
           BRANCH_NAME="${{ github.event.pull_request.head.ref }}"
-          VERSION=${BRANCH_NAME#hotfix/}
+          VERSION=${BRANCH_NAME#hotfix/v}
           echo "RELEASE_VERSION=$VERSION" >> $GITHUB_ENV
           git tag v${RELEASE_VERSION}
 
       - name: Calling parse-changelog
         run: ./parse-changelog CHANGELOG.md "${RELEASE_VERSION}"
```

### Comparing `cmake_pre_commit_hooks-1.9.0/.github/workflows/publish_release.yml` & `cmake_pre_commit_hooks-1.9.1/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/.gitignore` & `cmake_pre_commit_hooks-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     rev: v2.2.4
     hooks:
       - id: codespell
         files: .*\.(py|txt|cmake|md|rst|sh|ps1|hpp|tpp|cpp|cc)$
         args: [-I, .codespell.allow]
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.2
+    rev: v0.9.0.5
     hooks:
       - id: shellcheck
         require_serial: false
         args: [-x, --severity=info]
 
   - repo: https://github.com/adrienverge/yamllint.git
     rev: v1.32.0
@@ -60,11 +60,11 @@
     rev: 1.13.0
     hooks:
       - id: blacken-docs
         args: [-S, -l, '120']
         additional_dependencies: [black==22.12.0]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.269
+    rev: v0.0.272
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-source, --show-fixes]
```

### Comparing `cmake_pre_commit_hooks-1.9.0/.pre-commit-hooks.yaml` & `cmake_pre_commit_hooks-1.9.1/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/CHANGELOG.md` & `cmake_pre_commit_hooks-1.9.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,329 +1,330 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v1.9.1] - 2023-06-18
+
+### Changed
+
+- Add proper support for clang-format "linter" mode (ie. `--dry-run`)
+
+### Fixed
+
+- Avoid setting up CMake arguments for clang-format hook
+
+### Repository
+
+- Update release drafting GitHub workflow
+- Modify pull requests workflow to automatically update CHANGELOG file if it was created by pre-commit.ci
+- Update `charliermarsh/ruff-pre-commit` hook to v0.0.272
+- Update `shellcheck-py/shellcheck-py` hook to v0.9.0.5
+
 ## [v1.9.0] - 2023-05-24
 
 ### Added
 
--   Added Python tests using PyTest
--   Added support for parsing hook parameters from TOML configuration files
--   Added option to dump the current configuration as TOML-formatted output on the standard output (`--dump-toml`)
--   Added option to parse CMake trace output to detect files generated using `configure_file(...)`
+- Added Python tests using PyTest
+- Added support for parsing hook parameters from TOML configuration files
+- Added option to dump the current configuration as TOML-formatted output on the standard output (`--dump-toml`)
+- Added option to parse CMake trace output to detect files generated using `configure_file(...)`
 
 ### Fixed
 
--   Fixed potential issue with CppCheck hook always running on all files in compile database
+- Fixed potential issue with CppCheck hook always running on all files in compile database
 
 ### Changed
 
--   CppCheck hook will now exclude C++ header files by default since those are not present within the compilatioon databasebecauzse
--   Make default logging level `INFO` instead of `WARNING`
--   Move all CMake handling code into dedicated sub-module
--   Minor adjustments to logging output format
--   Update README
+- CppCheck hook will now exclude C++ header files by default since those are not present within the compilatioon databasebecauzse
+- Make default logging level `INFO` instead of `WARNING`
+- Move all CMake handling code into dedicated sub-module
+- Minor adjustments to logging output format
+- Update README
 
 ### Repository
 
--   Use [ruff](https://beta.ruff.rs/docs/) for linting over other Python linters
--   System tests now run using LOGLEVEL=DEBUG
--   Improved configuration for external linters (e.g. SonarCloud, Codacy)
--   Update `yamllint` hook to v1.32.0
+- Use [ruff](https://beta.ruff.rs/docs/) for linting over other Python linters
+- System tests now run using LOGLEVEL=DEBUG
+- Improved configuration for external linters (e.g. SonarCloud, Codacy)
+- Update `yamllint` hook to v1.32.0
 
 ## [v1.8.1] - 2023-04-20
 
 ### Added
 
--   Added support for C++ module files by default
+- Added support for C++ module files by default
 
 ### Fixed
 
--   Fixed some typos in the README file (thanks to @onuralpszr)
+- Fixed some typos in the README file (thanks to @onuralpszr)
 
 ### Changed
 
--   Require users to explicitly set `-B`\|`--build-dir` if they pass `--preset` to CMake (see issue [#63](https://github.com/Takishima/cmake-pre-commit-hooks/issues/63))
+- Require users to explicitly set `-B`|`--build-dir` if they pass `--preset` to CMake (see issue [#63](https://github.com/Takishima/cmake-pre-commit-hooks/issues/63))
 
 ### Repository
 
--   Update `Lucas-C/pre-commit-hooks` hook to v1.5.1
--   Update `codespell` to v2.2.4
--   Update `yamllint` hook to v1.30.0
--   Update `black` hook to v23.3.0
--   Update `bandit` hook to v1.7.5
--   Update `isort` hook to v5.12.0
+- Update `Lucas-C/pre-commit-hooks` hook to v1.5.1
+- Update `codespell` to v2.2.4
+- Update `yamllint` hook to v1.30.0
+- Update `black` hook to v23.3.0
+- Update `bandit` hook to v1.7.5
+- Update `isort` hook to v5.12.0
 
 ## [v1.8.0] - 2023-02-16
 
 ### Added
 
--   Added support for the CMake `--preset` command line argument
+- Added support for the CMake `--preset` command line argument
 
 ## [v1.7.0] - 2023-02-09
 
 ### Added
 
--   Added support for reading `compile_commands.json` (generated by CMake) when running the hooks in order to
-    automatically discover files
+- Added support for reading `compile_commands.json` (generated by CMake) when running the hooks in order to
+  automatically discover files
 
 ### Updated
 
--   Added some more pre-commit hooks:
-    -   shellcheck
-    -   bandit
+- Added some more pre-commit hooks:
+  - shellcheck
+  - bandit
 
 ### Repository
 
--   Add new badges to README file for CodeFactor.io and SonarCloud
--   Update `black` hook to v23.1.0
+- Add new badges to README file for CodeFactor.io and SonarCloud
+- Update `black` hook to v23.1.0
 
 ## [v1.6.0] - 2023-02-07
 
 ### Added
 
--   Added `include-what-you-use-conda` and `cppcheck-conda` hooks to install both tools using conda environments
+- Added `include-what-you-use-conda` and `cppcheck-conda` hooks to install both tools using conda environments
 
 ### Changed
 
--   Changed minimum Python version to 3.8.X
--   Allow `lizard` hook to handle Fortran files
+- Changed minimum Python version to 3.8.X
+- Allow `lizard` hook to handle Fortran files
 
 ### Updated
 
--   Update GitHub release publishing workflow
--   Added some more pre-commit hooks:
-    -   doc8
-    -   codespell
-    -   yamllint
-    -   blacken-docs
-    -   pyupgrade
+- Update GitHub release publishing workflow
+- Added some more pre-commit hooks:
+  - doc8
+  - codespell
+  - yamllint
+  - blacken-docs
+  - pyupgrade
 
 ### Repository
 
--   Update `action/setup-python` GitHub Action to v4
--   Update `ilammy/msvc-dev-cmd` GitHub Action to v1.12.1
--   Update `thomaseizinger/create-pull-request` GitHub Action to v1.3.0
--   Update `Lucas-C/pre-commit-hooks` hook to v1.4.2
--   Update `asottile/pyupgrade` to v3.2.0
--   Update `black` hook to v22.10.0
--   Update `blacken-docs` hook to v1.13.0
--   Update `flake8` hook to v5.0.4
--   Update `pre-commit/mirrors-pylint` to v3.0.0a5
--   Update `pre-commit/pre-commit-hooks` to v4.3.0
--   Update `pyupgrade` hook to v3.3.1
--   Update `yamllint` hook to v1.29.0
--   Update `isort` hook to v5.12.0
+- Update `action/setup-python` GitHub Action to v4
+- Update `ilammy/msvc-dev-cmd` GitHub Action to v1.12.1
+- Update `thomaseizinger/create-pull-request` GitHub Action to v1.3.0
+- Update `Lucas-C/pre-commit-hooks` hook to v1.4.2
+- Update `asottile/pyupgrade` to v3.2.0
+- Update `black` hook to v22.10.0
+- Update `blacken-docs` hook to v1.13.0
+- Update `flake8` hook to v5.0.4
+- Update `pre-commit/mirrors-pylint` to v3.0.0a5
+- Update `pre-commit/pre-commit-hooks` to v4.3.0
+- Update `pyupgrade` hook to v3.3.1
+- Update `yamllint` hook to v1.29.0
+- Update `isort` hook to v5.12.0
 
-## [1.5.3] - 2022-06-14
+## [v1.5.3] - 2022-06-14
 
 ### Added
 
--   Add support for installing `clang-format` using Python if not found on the system
--   Add support for installing `lizard` automatically if not found on the system
+- Add support for installing `clang-format` using Python if not found on the system
+- Add support for installing `lizard` automatically if not found on the system
 
 ### Fixed
 
--   Correctly pass on the default argument list to `CLinters`
--   Fixed issues with release publishing workflows on GitHub
+- Correctly pass on the default argument list to `CLinters`
+- Fixed issues with release publishing workflows on GitHub
 
 ### Repository
 
--   Update GitHub's CodeQL action to v2
--   Update `pre-commit/pre-commit-hooks` hook to v4.3.0
--   Update `Lucas-C/pre-commit-hooks` hook to v1.2.0
--   Update `pre-commit/mirrors-pylint` hook to v3.0.0a5
--   Update `dangoslen/changelog-enforcer` GitHub action to v3
--   Update `thomaseizinger/create-pull-request` GitHub action to v1.2.2
--   Update `black` hook to v22.3.0
--   Update `check-manifest` to v0.48
+- Update GitHub's CodeQL action to v2
+- Update `pre-commit/pre-commit-hooks` hook to v4.3.0
+- Update `Lucas-C/pre-commit-hooks` hook to v1.2.0
+- Update `pre-commit/mirrors-pylint` hook to v3.0.0a5
+- Update `dangoslen/changelog-enforcer` GitHub action to v3
+- Update `thomaseizinger/create-pull-request` GitHub action to v1.2.2
+- Update `black` hook to v22.3.0
+- Update `check-manifest` to v0.48
 
-## [1.5.2] - 2021-12-08
+## [v1.5.2] - 2021-12-08
 
 ### Fixed
 
--   Fixed indentation issue
+- Fixed indentation issue
 
-## [1.5.1] - 2021-12-08
+## [v1.5.1] - 2021-12-08
 
 ### Fixed
 
--   Fixed locating of compilation database in presence of a symbolic link in the source directory
+- Fixed locating of compilation database in presence of a symbolic link in the source directory
 
 ### Repository
 
--   New step in "Format" GitHub action to make sure the CHANGELOG is updated with proper version section for hotfix/_
-    and release/_ branches
--   Update `isort` hook to v5.10.1
--   Update `black` hook to v21.12b0
+- New step in "Format" GitHub action to make sure the CHANGELOG is updated with proper version section for hotfix/\_
+  and release/\_ branches
+- Update `isort` hook to v5.10.1
+- Update `black` hook to v21.12b0
 
-## [1.5.0] - 2021-11-08
+## [v1.5.0] - 2021-11-08
 
 ### Added
 
--   Support for `cpplint`
--   Support for `lizard`, a code complexity analyzer
+- Support for `cpplint`
+- Support for `lizard`, a code complexity analyzer
 
 ### Repository
 
--   Update pre-commit hooks
--   Update `thomaseizinger/create-pull-request` GiHub action to v1.3.0
--   Update `isort` hook to v5.10.0
--   Update `black` hook to v21.10b0
--   Update `check-manifest` hook to v0.47
--   Update `flake8` hook to v4.0.1
+- Update pre-commit hooks
+- Update `thomaseizinger/create-pull-request` GiHub action to v1.3.0
+- Update `isort` hook to v5.10.0
+- Update `black` hook to v21.10b0
+- Update `check-manifest` hook to v0.47
+- Update `flake8` hook to v4.0.1
 
-## [1.4.0] - 2021-07-16
+## [v1.4.0] - 2021-07-16
 
 ### Added
 
--   Support for simultaneous processing of all files using `--all-at-once`
+- Support for simultaneous processing of all files using `--all-at-once`
 
 ### Updated
 
--   Improved code handling standard output and error stream in case of multiple files
--   Minor improvements to debugging output
+- Improved code handling standard output and error stream in case of multiple files
+- Minor improvements to debugging output
 
 ### Fixed
 
--   Do not attempt to copy the compilation database in the source directory if it exists and is a symbolic link
--   Properly handle the `--cmake` command line option
+- Do not attempt to copy the compilation database in the source directory if it exists and is a symbolic link
+- Properly handle the `--cmake` command line option
 
 ### Repository
 
--   Cleanup of `pre-commit-config.yaml` and added
--   Added some more flake8 plugins to the list used by `pre-commit`:
-    -   flake8-breakpoint
-    -   flake8-comprehensions
-    -   flake8-docstrings
-    -   flake8-eradicate
-    -   flake8-mutable
+- Cleanup of `pre-commit-config.yaml` and added
+- Added some more flake8 plugins to the list used by `pre-commit`:
+  - flake8-breakpoint
+  - flake8-comprehensions
+  - flake8-docstrings
+  - flake8-eradicate
+  - flake8-mutable
 
-## [1.3.0] - 2021-06-27
+## [v1.3.0] - 2021-06-27
 
 ### Added
 
--   Support for platform-specific CMake options
-    Use `--linux`, `--mac` and `--win` to specify CMake flags that need to be provided only on the specific
-    platform. `--unix` can be used as a shortcut to specifying `--linux` and `--mac`.
+- Support for platform-specific CMake options
+  Use `--linux`, `--mac` and `--win` to specify CMake flags that need to be provided only on the specific
+  platform. `--unix` can be used as a shortcut to specifying `--linux` and `--mac`.
 
-## [1.2.0] - 2021-06-27
+## [v1.2.0] - 2021-06-27
 
 ### Added
 
--   Support for Include-What-You-Use
+- Support for Include-What-You-Use
 
 ### Fixed
 
--   Double-dash arguments not present in debug output
+- Double-dash arguments not present in debug output
 
 ### Repository
 
--   Add tests that use pre-commit directly
--   Add isort pre-commit hook
+- Add tests that use pre-commit directly
+- Add isort pre-commit hook
 
-## [1.1.2] - 2021-06-26
+## [v1.1.2] - 2021-06-26
 
 ### Added
 
--   Added debug command line option to show the exact commands being run when using pre-commit regardless of exit status
+- Added debug command line option to show the exact commands being run when using pre-commit regardless of exit status
 
 ### Fixed
 
--   Properly handle double-dash arguments for clang-tidy when multiple files are passed to the hook
+- Properly handle double-dash arguments for clang-tidy when multiple files are passed to the hook
 
-## [1.1.1] - 2021-06-26
+## [v1.1.1] - 2021-06-26
 
 ### Updated
 
--   Added support for CUDA files by default
+- Added support for CUDA files by default
 
 ### Fixed
 
--   Default source directory is now correctly set to the current directory
+- Default source directory is now correctly set to the current directory
 
 ### Repository
 
--   Fix automatic release publication workflow
+- Fix automatic release publication workflow
 
-## [1.1.0] - 2021-06-22
+## [v1.1.0] - 2021-06-22
 
 ### Updated
 
--   Added Python 3.9 in the package's metadata
--   Support for specifying more than one build directory
-    If one of those exists and contains a configured CMake directory, that one will be chosen. If none already exist,
-    the first specified alternative will be chosen.
+- Added Python 3.9 in the package's metadata
+- Support for specifying more than one build directory
+  If one of those exists and contains a configured CMake directory, that one will be chosen. If none already exist,
+  the first specified alternative will be chosen.
 
 ### Fixed
 
--   Issues with arguments parsing for arguments that are specified more than once
--   Fix issue with CMake configure step when running hooks in parallel
+- Issues with arguments parsing for arguments that are specified more than once
+- Fix issue with CMake configure step when running hooks in parallel
 
 ### Repository
 
--   Update pre-commit configuration
+- Update pre-commit configuration
 
-## [1.0.1] - 2021-06-20
+## [v1.0.1] - 2021-06-20
 
 ### Added
 
--   Support for GitHub actions
--   Small test scripts for Linux, MacOS and Windows (only partial testing)
+- Support for GitHub actions
+- Small test scripts for Linux, MacOS and Windows (only partial testing)
 
 ### Updated
 
--   Slightly more verbose output on certain failures
+- Slightly more verbose output on certain failures
 
 ### Fixed
 
--   Issue when passing paths to `subprocess.run()` on Windows
--   CMake arguments being parsed more than once
+- Issue when passing paths to `subprocess.run()` on Windows
+- CMake arguments being parsed more than once
 
-## [1.0.0] - 2021-06-18
+## [v1.0.0] - 2021-06-18
 
 Initial release with support for:
 
--   clang-format
--   clang-tidy
--   cppcheck
-
-[Unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.0...HEAD
-
-[v1.9.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.1...v1.9.0
-
-[v1.8.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.0...v1.8.1
-
-[v1.8.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.7.0...v1.8.0
-
-[v1.7.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.6.0...v1.7.0
-
+- clang-format
+- clang-tidy
+- cppcheck
+
+[unreleased]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.1...HEAD
+[v1.0.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/20b1113bf223273cda31a14a82c9d573a342de4a...v1.0.0
+[v1.0.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.0.0...v1.0.1
+[v1.1.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.0.1...v1.1.0
+[v1.1.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.0...v1.1.1
+[v1.1.2]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.1...v1.1.2
+[v1.2.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.2...v1.2.0
+[v1.3.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.2.0...v1.3.0
+[v1.4.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.3.0...v1.4.0
+[v1.5.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.4.0...v1.5.0
+[v1.5.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.0...v1.5.1
+[v1.5.2]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.1...v1.5.2
+[v1.5.3]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.2...v1.5.3
 [v1.6.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.3...v1.6.0
-
-[1.5.3]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.2...v1.5.3
-
-[1.5.2]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.1...v1.5.2
-
-[1.5.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.5.0...v1.5.1
-
-[1.5.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.4.0...v1.5.0
-
-[1.4.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.3.0...v1.4.0
-
-[1.3.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.2.0...v1.3.0
-
-[1.2.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.2...v1.2.0
-
-[1.1.2]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.1...v1.1.2
-
-[1.1.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.1.0...v1.1.1
-
-[1.1.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.0.1...v1.1.0
-
-[1.0.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.0.0...v1.0.1
-
-[1.0.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/20b1113bf223273cda31a14a82c9d573a342de4a...v1.0.0
+[v1.7.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.6.0...v1.7.0
+[v1.8.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.7.0...v1.8.0
+[v1.8.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.0...v1.8.1
+[v1.9.0]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.8.1...v1.9.0
+[v1.9.1]: https://github.com/Takishima/cmake-pre-commit-hooks/compare/v1.9.0...v1.9.1
```

### Comparing `cmake_pre_commit_hooks-1.9.0/LICENSE` & `cmake_pre_commit_hooks-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/PKG-INFO` & `cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cmake_pre_commit_hooks
-Version: 1.9.0
+Name: cmake-pre-commit-hooks
+Version: 1.9.1
 Summary: pre-commit hooks for CMake based projects
 Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
 Author: Damien Nguyen
 Author-email: ngn.damien@gmail.com
 License: Apache2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cmake_pre_commit_hooks-1.9.0/README.md` & `cmake_pre_commit_hooks-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/__init__.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_argparse.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_argparse.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_call_process.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_call_process.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_cmake.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,14 +293,18 @@
         """
         Run a CMake configure step (multi-process safe).
 
         Args:
             command (str): Name of calling command
             clean_build (bool): Clean build directory before calling CMake configure
         """
+        if self.source_dir is None:
+            logging.error('No source dir was for CMake! Did you call `setup_cmake_args()`?')
+            sys.exit(1)
+
         cmake_configure_lock_file = Path(self.build_dir, '_cmake_configure_lock')
         cmake_configure_try_lock_file = Path(self.build_dir, '_cmake_configure_try_lock')
 
         self.build_dir.mkdir(exist_ok=True)
 
         cmake_configure_try_lock = filelock.FileLock(cmake_configure_try_lock_file)
         cmake_configure_lock = fasteners.InterProcessReaderWriterLock(cmake_configure_lock_file)
```

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/_utils.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         return [entry['file'] for entry in data]
     return []
 
 
 class Command(hooks.utils.Command):  # pylint: disable=too-many-instance-attributes
     """Super class that all commands inherit."""
 
+    setup_cmake = True
+
     def __init__(self, command, look_behind, args):
         """Initialize a Command object."""
         super().__init__(command, look_behind, args)
         self.ddash_args = []
         self.cmake = CMakeCommand()
         self.clean_build = False
         self.all_at_once = False
@@ -93,19 +95,20 @@
         self.all_at_once = known_args.all_at_once
         self.read_json_db = known_args.read_json_db
         self.clean_build = known_args.clean
 
         if not known_args.build_dir and known_args.preset:
             raise RuntimeError('You *must* specify -B|--build-dir if you pass --preset as a CMake argument!')
 
-        self.cmake.setup_cmake_args(known_args)
+        if self.setup_cmake:
+            self.cmake.setup_cmake_args(known_args)
 
-        if not self.cmake.source_dir.exists() and not self.cmake.source_dir.is_dir():
-            sys.stderr.write(f'{self.cmake.source_dir} is not a valid source directory\n')
-            sys.exit(1)
+            if not self.cmake.source_dir.exists() and not self.cmake.source_dir.is_dir():
+                sys.stderr.write(f'{self.cmake.source_dir} is not a valid source directory\n')
+                sys.exit(1)
 
         if known_args.version:
             actual_version = self.get_version_str()
             self.assert_version(actual_version, known_args.version)
 
         # NB: if '--' may be present on the command line, the command class for that particular command needs to call
         #     handle_ddash_args() in order to properly handle the filenames in those cases.
@@ -181,23 +184,35 @@
             self.ddash_args.extend(['--'] + self.files[0:-idx])
         self.files = files
 
 
 class FormatterCmd(Command, hooks.utils.FormatterCmd):
     """Commands that format code: clang-format, uncrustify."""
 
+    setup_cmake = False
+
+    def __init__(self, command: str, look_behind: str, args: list[str]):
+        super().__init__(command, look_behind, args)
+        self.dry_run = '-n' in self.args or '--dry-run' in self.args
+
     def get_formatted_lines(self, filename: bytes) -> list:  # pragma: nocover
         """Get the expected output for a command applied to a file."""
         filename_opts = self.get_filename_opts(filename)
         args = [self.command, *self.args, *filename_opts]
         # NB: only change w.r.t original method to handle both bytes and string argument types
         child = _call_process.call_process([arg.decode() if isinstance(arg, bytes) else arg for arg in args])
         if len(child.stderr) > 0 or child.returncode != 0:
             problem = f'Unexpected Stderr/return code received when analyzing {filename}.\nArgs: {args}'
             self.raise_error(problem, child.stdout + child.stderr)
+
+        if self.dry_run:
+            # clang-format dry-run mode is '-n'
+            # If dry-run mode then we only look at the return code -> read the lines
+            self.returncode = 0
+            return self.get_filelines(filename)
         if not child.stdout:
             return []
         return child.stdout.encode().split(b'\x0a')
 
 
 class StaticAnalyzerCmd(Command, hooks.utils.StaticAnalyzerCmd):
     """Commands that analyze code and are not formatters."""
```

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/clang_format.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/clang_format.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/clang_tidy.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/clang_tidy.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/cppcheck.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/cppcheck.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/cpplint.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/cpplint.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/include_what_you_use.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/include_what_you_use.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pc_hooks/lizard.py` & `cmake_pre_commit_hooks-1.9.1/cmake_pc_hooks/lizard.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/PKG-INFO` & `cmake_pre_commit_hooks-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cmake-pre-commit-hooks
-Version: 1.9.0
+Name: cmake_pre_commit_hooks
+Version: 1.9.1
 Summary: pre-commit hooks for CMake based projects
 Home-page: https://github.com/Takishima/cmake-pre-commit-hooks
 Author: Damien Nguyen
 Author-email: ngn.damien@gmail.com
 License: Apache2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cmake_pre_commit_hooks-1.9.0/cmake_pre_commit_hooks.egg-info/SOURCES.txt` & `cmake_pre_commit_hooks-1.9.1/cmake_pre_commit_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/misc/license_header.txt` & `cmake_pre_commit_hooks-1.9.1/misc/license_header.txt`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/pyproject.toml` & `cmake_pre_commit_hooks-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/setup.cfg` & `cmake_pre_commit_hooks-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/setup.py` & `cmake_pre_commit_hooks-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/cmake_bad/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.1/tests/cmake_bad/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/cmake_good/.pre-commit-config.yaml` & `cmake_pre_commit_hooks-1.9.1/tests/cmake_good/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/_argparse_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/_argparse_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/_call_process_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/_call_process_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/_cmake_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/_cmake_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import platform
 from pathlib import Path
 from textwrap import dedent
 
 import fasteners
 import filelock
 import pytest
+from _test_utils import ExitError
 
 from cmake_pc_hooks._cmake import CMakeCommand, get_cmake_command
 
 # ==============================================================================
 
 _has_cmake = get_cmake_command() is not None
 
@@ -34,14 +35,21 @@
 def parser():
     cmake = CMakeCommand()
     parser = argparse.ArgumentParser()
     cmake.add_cmake_arguments_to_parser(parser)
     return parser
 
 
+# ------------------------------------------------------------------------------
+
+filelock_module_name = 'filelock.FileLock'
+interprocess_rw_lock_module_name = 'fasteners.InterProcessReaderWriterLock'
+internal_cmake_configure_name = 'cmake_pc_hooks._cmake.CMakeCommand._configure'
+
+
 # ==============================================================================
 
 
 def test_cmake_command_init():
     cmake = CMakeCommand()
     assert cmake.command is None or isinstance(cmake.command, list)
     assert cmake.source_dir is None
@@ -207,19 +215,19 @@
 
 @pytest.mark.parametrize('detect_configured_files', [False, True], ids=['no_trace', 'w_trace'])
 @pytest.mark.parametrize('returncode', [0, 1])
 @pytest.mark.parametrize('clean_build', [False, True])
 def test_configure_cmake(mocker, tmp_path, clean_build, returncode, detect_configured_files):
     sys_exit = mocker.patch('sys.exit')
     FileLock = mocker.MagicMock(filelock.FileLock)  # noqa: N806
-    mocker.patch('filelock.FileLock', FileLock)
+    mocker.patch(filelock_module_name, FileLock)
     InterProcessReaderWriterLock = mocker.MagicMock(fasteners.InterProcessReaderWriterLock)  # noqa: N806
-    mocker.patch('fasteners.InterProcessReaderWriterLock', InterProcessReaderWriterLock)
+    mocker.patch(interprocess_rw_lock_module_name, InterProcessReaderWriterLock)
     _configure = mocker.Mock(return_value=returncode)
-    mocker.patch('cmake_pc_hooks._cmake.CMakeCommand._configure', _configure)
+    mocker.patch(internal_cmake_configure_name, _configure)
     parse_log = mocker.patch('cmake_pc_hooks._cmake.CMakeCommand._parse_cmake_trace_log')
 
     # ----------------------------------
 
     build_dir = tmp_path / 'build'
     build_dir.mkdir(parents=True, exist_ok=True)
 
@@ -257,21 +265,21 @@
 
     def timeout(blocking):  # noqa: ARG001
         raise RuntimeError
 
     args = {'acquire.side_effect': timeout}
     file_lock = mocker.MagicMock(filelock.FileLock, **args)
     FileLock = mocker.MagicMock(filelock.FileLock, return_value=file_lock)  # noqa: N806
-    mocker.patch('filelock.FileLock', FileLock)
+    mocker.patch(filelock_module_name, FileLock)
 
     interprocess_lock = mocker.MagicMock()
     InterProcessReaderWriterLock = mocker.MagicMock(return_value=interprocess_lock)  # noqa: N806
-    mocker.patch('fasteners.InterProcessReaderWriterLock', InterProcessReaderWriterLock)
+    mocker.patch(interprocess_rw_lock_module_name, InterProcessReaderWriterLock)
     _configure = mocker.Mock(return_value=0)
-    mocker.patch('cmake_pc_hooks._cmake.CMakeCommand._configure', _configure)
+    mocker.patch(internal_cmake_configure_name, _configure)
 
     # ----------------------------------
 
     build_dir = tmp_path / 'build'
     build_dir.mkdir(parents=True, exist_ok=True)
 
     cmake = CMakeCommand()
@@ -285,14 +293,32 @@
 
     FileLock.assert_called_once()
     InterProcessReaderWriterLock.assert_called_once()
     interprocess_lock.read_lock.assert_called_once()
     _configure.assert_not_called()
 
 
+def test_configure_invalid(mocker):
+    mocker.patch('sys.exit', side_effect=ExitError)
+
+    FileLock = mocker.MagicMock(filelock.FileLock)  # noqa: N806
+    mocker.patch(filelock_module_name, FileLock)
+    InterProcessReaderWriterLock = mocker.MagicMock(fasteners.InterProcessReaderWriterLock)  # noqa: N806
+    mocker.patch(interprocess_rw_lock_module_name, InterProcessReaderWriterLock)
+    _configure = mocker.Mock(return_value=1)
+    mocker.patch(internal_cmake_configure_name, _configure)
+
+    # ----------------------------------
+
+    cmake = CMakeCommand()
+    assert cmake.source_dir is None
+    with pytest.raises(ExitError):
+        cmake.configure(command='test')
+
+
 @pytest.mark.parametrize('detect_configured_files', [False, True], ids=['no_trace', 'w_trace'])
 @pytest.mark.parametrize('clean_build', [False, True], ids=['no_clean_build', 'clean_build'])
 def test_configure_cmake_internal(mocker, tmp_path, clean_build, detect_configured_files):
     mocker.patch('shutil.rmtree')
     call_cmake = mocker.patch(
         'cmake_pc_hooks._cmake.CMakeCommand._call_cmake', return_value=mocker.Mock(stdout='', stderr='', returncode=0)
     )
```

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/_test_utils.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/_test_utils.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/_utils_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/_utils_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/clang_format_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/clang_format_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/clang_tidy_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/clang_tidy_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 
 import pytest
 from _test_utils import command_main_asserts, run_command_default_assertions
 
 from cmake_pc_hooks import clang_tidy
 
-
 # ==============================================================================
 
 
 @pytest.mark.parametrize('stdout', ['', 'aaa'], ids=['<empty>', 'aaa'])
 @pytest.mark.parametrize(
     'error_msg', [None, '1 error generated.', '2 errors generated.'], ids=['<empty>', '1_error', '2_errors']
 )
```

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/conftest.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/conftest.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/cppcheck_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/cppcheck_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/cpplint_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/cpplint_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/iwyu_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/iwyu_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/python/lizard_test.py` & `cmake_pre_commit_hooks-1.9.1/tests/python/lizard_test.py`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/run_tests.ps1` & `cmake_pre_commit_hooks-1.9.1/tests/run_tests.ps1`

 * *Files identical despite different names*

### Comparing `cmake_pre_commit_hooks-1.9.0/tests/run_tests.sh` & `cmake_pre_commit_hooks-1.9.1/tests/run_tests.sh`

 * *Files identical despite different names*


# Comparing `tmp/pykoopman-0.2.0.tar.gz` & `tmp/pykoopman-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pykoopman-0.2.0.tar", last modified: Sat Dec 26 21:07:33 2020, max compression
+gzip compressed data, was "pykoopman-1.0.0.tar", last modified: Sun Jun 18 02:27:45 2023, max compression
```

## Comparing `pykoopman-0.2.0.tar` & `pykoopman-1.0.0.tar`

### file list

```diff
@@ -1,70 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-12-26 21:07:30.000000 pykoopman-0.2.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-12-26 21:07:30.000000 pykoopman-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      626 2020-12-26 21:07:30.000000 pykoopman-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1413 2020-12-26 21:07:30.000000 pykoopman-0.2.0/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (116)      326 2020-12-26 21:07:30.000000 pykoopman-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      526 2020-12-26 21:07:30.000000 pykoopman-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      125 2020-12-26 21:07:30.000000 pykoopman-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1084 2020-12-26 21:07:30.000000 pykoopman-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4325 2020-12-26 21:07:33.000000 pykoopman-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2742 2020-12-26 21:07:30.000000 pykoopman-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     3096 2020-12-26 21:07:30.000000 pykoopman-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      331 2020-12-26 21:07:30.000000 pykoopman-0.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      393 2020-12-26 21:07:30.000000 pykoopman-0.2.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)    39151 2020-12-26 21:07:30.000000 pykoopman-0.2.0/examples/differentiation.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2020-12-26 21:07:30.000000 pykoopman-0.2.0/examples/example_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)   222645 2020-12-26 21:07:30.000000 pykoopman-0.2.0/examples/observables.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)  1097839 2020-12-26 21:07:30.000000 pykoopman-0.2.0/examples/tutorial_dmdc_sparse_linear_system.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)   270074 2020-12-26 21:07:30.000000 pykoopman-0.2.0/examples/tutorial_koopman_linearsystem.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)    24792 2020-12-26 21:07:30.000000 pykoopman-0.2.0/examples/tutorial_koopman_with_control.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)   207012 2020-12-26 21:07:30.000000 pykoopman-0.2.0/examples/tutorial_linear_random_control_system.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman/
--rw-r--r--   0 runner    (1001) docker     (116)      397 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman/common/
--rw-r--r--   0 runner    (1001) docker     (116)      361 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14074 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/common/examples.py
--rw-r--r--   0 runner    (1001) docker     (116)     2082 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/common/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman/differentiation/
--rw-r--r--   0 runner    (1001) docker     (116)      131 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/differentiation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2707 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/differentiation/_derivative.py
--rw-r--r--   0 runner    (1001) docker     (116)      222 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/differentiation/_finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (116)    15724 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/koopman.py
--rw-r--r--   0 runner    (1001) docker     (116)     4361 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/koopman_continuous.py
--rw-r--r--   0 runner    (1001) docker     (116)     2597 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/koopman_discrete.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman/observables/
--rw-r--r--   0 runner    (1001) docker     (116)      226 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/observables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2254 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/observables/_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     7612 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/observables/_custom_observables.py
--rw-r--r--   0 runner    (1001) docker     (116)     2968 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/observables/_identity.py
--rw-r--r--   0 runner    (1001) docker     (116)     7239 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/observables/_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (116)     7683 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/observables/_time_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman/regression/
--rw-r--r--   0 runner    (1001) docker     (116)      124 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      834 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1680 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/regression/_dmd.py
--rw-r--r--   0 runner    (1001) docker     (116)     9372 2020-12-26 21:07:30.000000 pykoopman-0.2.0/pykoopman/regression/_dmdc.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4325 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1567 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       48 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2020-12-26 21:07:33.000000 pykoopman-0.2.0/pykoopman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      280 2020-12-26 21:07:30.000000 pykoopman-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)       48 2020-12-26 21:07:30.000000 pykoopman-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      373 2020-12-26 21:07:33.000000 pykoopman-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1344 2020-12-26 21:07:30.000000 pykoopman-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)     4770 2020-12-26 21:07:30.000000 pykoopman-0.2.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/test/differentiation/
--rw-r--r--   0 runner    (1001) docker     (116)     2119 2020-12-26 21:07:30.000000 pykoopman-0.2.0/test/differentiation/test_differentiation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/test/observables/
--rw-r--r--   0 runner    (1001) docker     (116)     4734 2020-12-26 21:07:30.000000 pykoopman-0.2.0/test/observables/test_observables.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-26 21:07:33.000000 pykoopman-0.2.0/test/regression/
--rw-r--r--   0 runner    (1001) docker     (116)      555 2020-12-26 21:07:30.000000 pykoopman-0.2.0/test/regression/test_regressors.py
--rw-r--r--   0 runner    (1001) docker     (116)     6171 2020-12-26 21:07:30.000000 pykoopman-0.2.0/test/test_koopman.py
--rw-r--r--   0 runner    (1001) docker     (116)      487 2020-12-26 21:07:30.000000 pykoopman-0.2.0/test/test_koopman_continuous.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.884422 pykoopman-1.0.0/
+-rw-rw-rw-   0        0        0       24 2023-02-16 18:09:30.000000 pykoopman-1.0.0/.git_archival.txt
+-rw-rw-rw-   0        0        0      169 2023-02-16 18:09:30.000000 pykoopman-1.0.0/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.824047 pykoopman-1.0.0/.github/
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.836445 pykoopman-1.0.0/.github/workflows/
+-rw-rw-rw-   0        0        0      656 2023-06-15 07:39:59.000000 pykoopman-1.0.0/.github/workflows/release.yaml
+-rw-rw-rw-   0        0        0     1337 2023-06-15 23:56:43.000000 pykoopman-1.0.0/.github/workflows/run-tests.yml
+-rw-rw-rw-   0        0        0      418 2023-03-27 06:02:36.000000 pykoopman-1.0.0/.gitignore
+-rw-rw-rw-   0        0        0      788 2023-02-16 18:09:30.000000 pykoopman-1.0.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      773 2023-06-15 07:39:59.000000 pykoopman-1.0.0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1118 2023-06-15 07:39:59.000000 pykoopman-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     9102 2023-06-18 02:27:45.884422 pykoopman-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8325 2023-06-18 02:27:38.000000 pykoopman-1.0.0/README.rst
+-rw-rw-rw-   0        0        0      246 2023-06-15 07:39:59.000000 pykoopman-1.0.0/codecov.yml
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.853443 pykoopman-1.0.0/docs/
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.858440 pykoopman-1.0.0/docs/JOSS/
+-rw-rw-rw-   0        0        0   128421 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/Fig1.png
+-rw-rw-rw-   0        0        0    66677 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/Fig2.png
+-rw-rw-rw-   0        0        0    28248 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/Fig3.png
+-rw-rw-rw-   0        0        0     1824 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/codemeta.json
+-rw-rw-rw-   0        0        0    16242 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/default.csl
+-rw-rw-rw-   0        0        0     4820 2023-04-12 18:22:22.000000 pykoopman-1.0.0/docs/JOSS/generate.rb
+-rw-rw-rw-   0        0        0    37209 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/paper.bib
+-rw-rw-rw-   0        0        0    11132 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/paper.md
+-rw-rw-rw-   0        0        0      654 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/Makefile
+-rw-rw-rw-   0        0        0     3388 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/conf.py
+-rw-rw-rw-   0        0        0     1222 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/make.bat
+-rw-rw-rw-   0        0        0  1048136 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_compose_observables.ipynb
+-rw-rw-rw-   0        0        0    70466 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_compute_differentiation.ipynb
+-rw-rw-rw-   0        0        0  1660826 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_failed_for_pde_examples.ipynb
+-rw-rw-rw-   0        0        0   412334 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb
+-rw-rw-rw-   0        0        0  1433953 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_succeeds_pde_examples.ipynb
+-rw-rw-rw-   0        0        0  1363247 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_with_control_128d_system.ipynb
+-rw-rw-rw-   0        0        0    42474 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_with_control_2d_system.ipynb
+-rw-rw-rw-   0        0        0   215931 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_edmd_with_rbf.ipynb
+-rw-rw-rw-   0        0        0   494059 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb
+-rw-rw-rw-   0        0        0   389950 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb
+-rw-rw-rw-   0        0        0   450330 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb
+-rw-rw-rw-   0        0        0   393560 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb
+-rw-rw-rw-   0        0        0   622478 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_havok_3d_lorenz.ipynb
+-rw-rw-rw-   0        0        0   397898 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb
+-rw-rw-rw-   0        0        0   242503 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_nndmd_examples.ipynb
+-rw-rw-rw-   0        0        0   344701 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_linear_random_control_system.ipynb
+-rw-rw-rw-   0        0        0  1152333 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb
+-rw-rw-rw-   0        0        0   299511 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.860442 pykoopman-1.0.0/pykoopman/
+-rw-rw-rw-   0        0        0      473 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.869322 pykoopman-1.0.0/pykoopman/analytics/
+-rw-rw-rw-   0        0        0      237 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/analytics/__init__.py
+-rw-rw-rw-   0        0        0     3024 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/analytics/_base_analyzer.py
+-rw-rw-rw-   0        0        0    20052 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/analytics/_ms_pd21.py
+-rw-rw-rw-   0        0        0     5270 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/analytics/_pruned_koopman.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.872419 pykoopman-1.0.0/pykoopman/common/
+-rw-rw-rw-   0        0        0      860 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/common/__init__.py
+-rw-rw-rw-   0        0        0     7292 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/common/cqgle.py
+-rw-rw-rw-   0        0        0    34090 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/common/examples.py
+-rw-rw-rw-   0        0        0     6092 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/common/ks.py
+-rw-rw-rw-   0        0        0     5893 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/common/nlse.py
+-rw-rw-rw-   0        0        0     2184 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/common/validation.py
+-rw-rw-rw-   0        0        0     5204 2023-05-22 05:30:39.000000 pykoopman-1.0.0/pykoopman/common/vbe.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.873415 pykoopman-1.0.0/pykoopman/differentiation/
+-rw-rw-rw-   0        0        0      173 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/differentiation/__init__.py
+-rw-rw-rw-   0        0        0     2535 2023-05-22 05:30:38.000000 pykoopman-1.0.0/pykoopman/differentiation/_derivative.py
+-rw-rw-rw-   0        0        0      270 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/differentiation/_finite_difference.py
+-rw-rw-rw-   0        0        0    22105 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/koopman.py
+-rw-rw-rw-   0        0        0     6067 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/koopman_continuous.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.877412 pykoopman-1.0.0/pykoopman/observables/
+-rw-rw-rw-   0        0        0      471 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/observables/__init__.py
+-rw-rw-rw-   0        0        0    15145 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_base.py
+-rw-rw-rw-   0        0        0     9757 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_custom_observables.py
+-rw-rw-rw-   0        0        0     2671 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_identity.py
+-rw-rw-rw-   0        0        0    10957 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_polynomial.py
+-rw-rw-rw-   0        0        0    11943 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_radial_basis_functions.py
+-rw-rw-rw-   0        0        0     7035 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_random_fourier_features.py
+-rw-rw-rw-   0        0        0     7467 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_time_delay.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.881413 pykoopman-1.0.0/pykoopman/regression/
+-rw-rw-rw-   0        0        0      465 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/__init__.py
+-rw-rw-rw-   0        0        0     2727 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_base.py
+-rw-rw-rw-   0        0        0    16027 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_base_ensemble.py
+-rw-rw-rw-   0        0        0    12635 2023-06-16 08:24:08.000000 pykoopman-1.0.0/pykoopman/regression/_dmd.py
+-rw-rw-rw-   0        0        0    16367 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_dmdc.py
+-rw-rw-rw-   0        0        0     8161 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_edmd.py
+-rw-rw-rw-   0        0        0     7484 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_edmdc.py
+-rw-rw-rw-   0        0        0    10858 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_havok.py
+-rw-rw-rw-   0        0        0    16987 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_kdmd.py
+-rw-rw-rw-   0        0        0    50849 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_nndmd.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.867452 pykoopman-1.0.0/pykoopman.egg-info/
+-rw-rw-rw-   0        0        0     9102 2023-06-18 02:27:45.000000 pykoopman-1.0.0/pykoopman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2924 2023-06-18 02:27:45.000000 pykoopman-1.0.0/pykoopman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 02:27:45.000000 pykoopman-1.0.0/pykoopman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-18 02:27:45.000000 pykoopman-1.0.0/pykoopman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      913 2023-06-18 02:16:13.000000 pykoopman-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      408 2023-06-15 07:39:59.000000 pykoopman-1.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       31 2023-03-26 19:57:13.000000 pykoopman-1.0.0/requirements-torch.txt
+-rw-rw-rw-   0        0        0      167 2023-06-15 23:45:02.000000 pykoopman-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 02:27:45.884422 pykoopman-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.882410 pykoopman-1.0.0/test/
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.882410 pykoopman-1.0.0/test/analytics/
+-rw-rw-rw-   0        0        0     2351 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/analytics/test_analytics.py
+-rw-rw-rw-   0        0        0     7373 2023-02-24 05:43:30.000000 pykoopman-1.0.0/test/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.883413 pykoopman-1.0.0/test/differentiation/
+-rw-rw-rw-   0        0        0     2306 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/differentiation/test_differentiation.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.883413 pykoopman-1.0.0/test/observables/
+-rw-rw-rw-   0        0        0    14048 2023-04-06 03:39:16.000000 pykoopman-1.0.0/test/observables/test_observables.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.883413 pykoopman-1.0.0/test/regression/
+-rw-rw-rw-   0        0        0     3195 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/regression/test_regressors.py
+-rw-rw-rw-   0        0        0    28511 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/test_koopman.py
+-rw-rw-rw-   0        0        0     1612 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/test_koopman_continuous.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pykoopman-0.2.0/.pre-commit-config.yaml` & `pykoopman-1.0.0/.pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# Settings for pre-commit
-fail_fast: false
-repos:
-- repo: git://github.com/pre-commit/pre-commit-hooks
-  rev: master
-  hooks:
-    - id: check-added-large-files
-      args: ["--maxkb=775"]
-    - id: check-merge-conflict
-- repo: https://github.com/asottile/reorder_python_imports
-  rev: v1.0.1
-  hooks:
-    - id: reorder-python-imports
-- repo: https://github.com/ambv/black
-  rev: stable
-  hooks:
-    - id: black
-- repo: https://gitlab.com/pycqa/flake8
-  rev: master
-  hooks:
-    - id: flake8
-      args: ["--config=setup.cfg"]
+# Settings for pre-commit
+fail_fast: false
+repos:
+- repo: https://github.com/pre-commit/pre-commit-hooks
+  rev: v4.3.0
+  hooks:
+    - id: check-added-large-files
+      args: ["--maxkb=102400"]
+    - id: check-merge-conflict
+    - id: trailing-whitespace
+    - id: end-of-file-fixer
+-   repo: https://github.com/asottile/reorder_python_imports
+    rev: v3.9.0
+    hooks:
+      -   id: reorder-python-imports
+          exclude: ^(pre_commit/resources/|testing/resources/python3_hooks_repo/)
+          args: [--py37-plus, --add-import, 'from __future__ import annotations']
+- repo: https://github.com/ambv/black
+  rev: 22.8.0
+  hooks:
+    - id: black
+- repo: https://github.com/PyCQA/flake8
+  rev: 5.0.4
+  hooks:
+    - id: flake8
+      args: ["--config=setup.cfg"]
```

### Comparing `pykoopman-0.2.0/LICENSE` & `pykoopman-1.0.0/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright 2020 Eurika Kaiser and Brian de Silva
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright 2023 Eurika Kaiser, Brian de Silva and Shaowu Pan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pykoopman-0.2.0/docs/conf.py` & `pykoopman-1.0.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,127 @@
-import importlib
-import pathlib
-
-author = "Eurika Kaiser and Brian de Silva"
-project = "pykoopman"  # package name
-
-
-# no need to edit below this line
-
-copyright = f"2020, {author}"
-
-module = importlib.import_module(project)
-version = release = getattr(module, "__version__")
-# version = "0.0.1"
-
-# The master toctree document.
-master_doc = "index"
-
-extensions = [
-    "sphinxcontrib.apidoc",
-    "sphinx.ext.autodoc",
-    "sphinx.ext.viewcode",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.mathjax",
-    "sphinx_nbexamples",
-    "sphinx.ext.intersphinx",
-]
-
-apidoc_module_dir = f"../{project}"
-apidoc_excluded_paths = ["tests"]
-apidoc_toc_file = False
-
-autodoc_default_options = {"members": True}
-autodoc_member_order = "bysource"
-autoclass_content = "init"
-
-language = None
-
-here = pathlib.Path(__file__).parent
-
-if (here / "static/custom.css").exists():
-
-    html_static_path = ["static"]
-
-    def setup(app):
-        app.add_stylesheet("custom.css")
-
-
-exclude_patterns = ["build", "_build", "Thumbs.db", ".DS_Store"]
-# pygments_style = "sphinx"
-
-add_module_names = True
-add_function_parentheses = False
-
-html_theme = "sphinx_rtd_theme"
-html_show_sourcelink = False
-html_show_sphinx = False
-html_show_copyright = True
-
-default_role = "any"
-html_sourcelink_suffix = ""
-
-example_gallery_config = dict(
-    dont_preprocess=True,
-    examples_dirs=["../examples"],
-    gallery_dirs=["examples"],
-    pattern=".+.ipynb",
-)
-
-intersphinx_mapping = {
-    "derivative": ("https://derivative.readthedocs.io/en/latest/", None)
-}
-
-# -- Options for manual page output ---------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, "pykoopman", "pykoopman Documentation", [author], 1)]
-
-# If true, show URL addresses after external links.
-# man_show_urls = False
-
-
-# -- Extensions to the  Napoleon GoogleDocstring class ---------------------
-# michaelgoerz.net/notes/extending-sphinx-napoleon-docstring-sections.html
-from sphinx.ext.napoleon.docstring import GoogleDocstring  # noqa: E402
-
-
-def parse_keys_section(self, section):
-    return self._format_fields("Keys", self._consume_fields())
-
-
-GoogleDocstring._parse_keys_section = parse_keys_section
-
-
-def parse_attributes_section(self, section):
-    return self._format_fields("Attributes", self._consume_fields())
-
-
-GoogleDocstring._parse_attributes_section = parse_attributes_section
-
-
-def parse_class_attributes_section(self, section):
-    return self._format_fields("Class Attributes", self._consume_fields())
-
-
-GoogleDocstring._parse_class_attributes_section = parse_class_attributes_section
-
-
-def patched_parse(self):
-    """
-    we now patch the parse method to guarantee that the the above methods are
-    assigned to the _section dict
-    """
-    self._sections["keys"] = self._parse_keys_section
-    self._sections["class attributes"] = self._parse_class_attributes_section
-    self._unpatched_parse()
-
-
-GoogleDocstring._unpatched_parse = GoogleDocstring._parse
-GoogleDocstring._parse = patched_parse
+from __future__ import annotations
+
+import importlib
+import pathlib
+
+author = "Shaowu Pan, Eurika Kaiser and Brian de Silva"
+project = "pykoopman"  # package name
+
+# no need to edit below this line
+
+copyright = f"2023, {author}"
+
+module = importlib.import_module(project)
+version = release = getattr(module, "__version__")
+# version = "0.0.1"
+
+# The master toctree document.
+master_doc = "index"
+
+extensions = [
+    "nbsphinx",
+    "sphinx_codeautolink",
+    "sphinxcontrib.apidoc",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.mathjax",
+    "sphinx_nbexamples",
+    "sphinx.ext.intersphinx",
+]
+
+apidoc_module_dir = f"../{project}"
+apidoc_excluded_paths = ["tests"]
+apidoc_toc_file = False
+
+autodoc_default_options = {"members": True}
+autodoc_member_order = "bysource"
+autoclass_content = "init"
+
+language = "en"
+
+here = pathlib.Path(__file__).parent
+
+if (here / "static/custom.css").exists():
+
+    html_static_path = ["static"]
+
+    def setup(app):
+        app.add_stylesheet("custom.css")
+
+
+exclude_patterns = ["build", "_build", "Thumbs.db", ".DS_Store"]
+# pygments_style = "sphinx"
+
+add_module_names = True
+add_function_parentheses = False
+
+html_theme = "sphinx_rtd_theme"
+html_show_sourcelink = False
+html_show_sphinx = False
+html_show_copyright = True
+
+default_role = "any"
+html_sourcelink_suffix = ""
+
+example_gallery_config = dict(
+    dont_preprocess=True,
+    examples_dirs=["../examples"],
+    gallery_dirs=["examples"],
+    pattern=".+.ipynb",
+    urls="https://github.com/dynamicslab/pykoopman/blob/master/examples",
+)
+
+
+intersphinx_mapping = {
+    "derivative": ("https://derivative.readthedocs.io/en/latest/", None)
+}
+
+# -- Options for manual page output ---------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [(master_doc, "pykoopman", "pykoopman Documentation", [author], 1)]
+
+# If true, show URL addresses after external links.
+# man_show_urls = False
+
+
+# -- Extensions to the  Napoleon GoogleDocstring class ---------------------
+# michaelgoerz.net/notes/extending-sphinx-napoleon-docstring-sections.html
+from sphinx.ext.napoleon.docstring import GoogleDocstring  # noqa: E402
+
+
+def parse_keys_section(self, section):
+    return self._format_fields("Keys", self._consume_fields())
+
+
+GoogleDocstring._parse_keys_section = parse_keys_section
+
+
+def parse_attributes_section(self, section):
+    return self._format_fields("Attributes", self._consume_fields())
+
+
+GoogleDocstring._parse_attributes_section = parse_attributes_section
+
+
+def parse_class_attributes_section(self, section):
+    return self._format_fields("Class Attributes", self._consume_fields())
+
+
+GoogleDocstring._parse_class_attributes_section = parse_class_attributes_section
+
+
+def patched_parse(self):
+    """
+    we now patch the parse method to guarantee that the the above methods are
+    assigned to the _section dict
+    """
+    self._sections["keys"] = self._parse_keys_section
+    self._sections["class attributes"] = self._parse_class_attributes_section
+    self._unpatched_parse()
+
+
+GoogleDocstring._unpatched_parse = GoogleDocstring._parse
+GoogleDocstring._parse = patched_parse
```

### Comparing `pykoopman-0.2.0/pykoopman/common/validation.py` & `pykoopman-1.0.0/pykoopman/common/validation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,66 @@
-import numpy as np
-from sklearn.utils import check_array as skl_check_array
-
-T_DEFAULT = object()
-
-
-def validate_input(x, t=T_DEFAULT):
-    if not isinstance(x, np.ndarray):
-        raise ValueError("x must be array-like")
-    elif x.ndim == 1:
-        x = x.reshape(-1, 1)
-    x = check_array(x)
-
-    if t is not T_DEFAULT:
-        if t is None:
-            raise ValueError("t must be a scalar or array-like.")
-        # Apply this check if t is a scalar
-        elif np.ndim(t) == 0 and (isinstance(t, int) or isinstance(t, float)):
-            if t <= 0:
-                raise ValueError("t must be positive")
-        # Only apply these tests if t is array-like
-        elif isinstance(t, np.ndarray):
-            if not len(t) == x.shape[0]:
-                raise ValueError("Length of t should match x.shape[0].")
-            if not np.all(t[:-1] < t[1:]):
-                raise ValueError("Values in t should be in strictly increasing order.")
-        else:
-            raise ValueError("t must be a scalar or array-like.")
-
-    return x
-
-
-def check_array(x, **kwargs):
-    if np.iscomplexobj(x):
-        return skl_check_array(x.real, **kwargs) + 1j * skl_check_array(
-            x.imag, **kwargs
-        )
-    else:
-        return skl_check_array(x, **kwargs)
-
-
-def drop_nan_rows(arr, *args):
-    """
-    Remove rows in all inputs for which `arr` has `_np.nan` entries.
-
-    Parameters
-    ----------
-    arr : numpy.ndarray
-        Array whose rows are checked for nan entries.
-        Any rows containing nans are removed from ``arr`` and all arguments
-        passed via ``args``.
-    *args : variable length argument list of numpy.ndarray
-        Additional arrays from which to remove rows.
-        Each argument should have the same number of rows as ``arr``.
-
-    Returns
-    -------
-    arrays : tuple of numpy.ndarray
-        Arrays with nan rows dropped.
-        The first entry corresponds to ``arr`` and all following entries
-        to ``*args``.
-    """
-    nan_inds = np.isnan(arr).any(axis=1)
-    return (arr[~nan_inds], *[arg[~nan_inds] for arg in args])
+from __future__ import annotations
+
+import numpy as np
+from sklearn.utils import check_array as skl_check_array
+
+T_DEFAULT = object()
+
+
+def validate_input(x, t=T_DEFAULT):
+    if not isinstance(x, np.ndarray):
+        raise ValueError("x must be array-like")
+    elif x.ndim == 1:
+        x = x.reshape(-1, 1)
+    x = check_array(x)
+
+    if t is not T_DEFAULT:
+        if t is None:
+            raise ValueError("t must be a scalar or array-like.")
+        # Apply this check if t is a scalar
+        elif np.ndim(t) == 0 and (isinstance(t, int) or isinstance(t, float)):
+            if t <= 0:
+                raise ValueError("t must be positive")
+        # Only apply these tests if t is array-like
+        elif isinstance(t, np.ndarray):
+            if not len(t) == x.shape[0]:
+                raise ValueError("Length of t should match x.shape[0].")
+            if not np.all(t[:-1] < t[1:]):
+                raise ValueError("Values in t should be in strictly increasing order.")
+        else:
+            raise ValueError("t must be a scalar or array-like.")
+
+    return x
+
+
+def check_array(x, **kwargs):
+    if np.iscomplexobj(x):
+        return skl_check_array(x.real, **kwargs) + 1j * skl_check_array(
+            x.imag, **kwargs
+        )
+    else:
+        return skl_check_array(x, **kwargs)
+
+
+def drop_nan_rows(arr, *args):
+    """
+    Remove rows in all inputs for which `arr` has `_np.nan` entries.
+
+    Parameters
+    ----------
+    arr : numpy.ndarray
+        Array whose rows are checked for nan entries.
+        Any rows containing nans are removed from ``arr`` and all arguments
+        passed via ``args``.
+    *args : variable length argument list of numpy.ndarray
+        Additional arrays from which to remove rows.
+        Each argument should have the same number of rows as ``arr``.
+
+    Returns
+    -------
+    arrays : tuple of numpy.ndarray
+        Arrays with nan rows dropped.
+        The first entry corresponds to ``arr`` and all following entries
+        to ``*args``.
+    """
+    nan_inds = np.isnan(arr).any(axis=1)
+    return (arr[~nan_inds], *[arg[~nan_inds] for arg in args])
```

### Comparing `pykoopman-0.2.0/pykoopman/differentiation/_derivative.py` & `pykoopman-1.0.0/pykoopman/differentiation/_derivative.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-"""
-Wrapper classes for differentiation methods from the :doc:`derivative:index` package.
+"""Wrapper classes for differentiation methods from the :doc:`derivative:index` package.
 
 Some default values used here may differ from those used in :doc:`derivative:index`.
 """
+from __future__ import annotations
+
 from derivative import dxdt
 from numpy import arange
 from sklearn.base import BaseEstimator
 
 from ..common import validate_input
 
 
@@ -35,17 +36,14 @@
 
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def set_params(self, **params):
         """
         Set the parameters of this estimator.
-        Modification of the pysindy method to allow unknown kwargs. This allows using
-        the full range of derivative parameters that are not defined as member variables
-        in sklearn grid search.
 
         Returns
         -------
         self
         """
         if not params:
             # Simple optimization to gain speed (inspect is slow)
```

### Comparing `pykoopman-0.2.0/pykoopman/observables/_custom_observables.py` & `pykoopman-1.0.0/pykoopman/observables/_time_delay.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,224 +1,210 @@
-"""
-Linear observables
-"""
-from itertools import combinations
-from itertools import combinations_with_replacement
-
-from numpy import empty
-from sklearn.utils.validation import check_is_fitted
-
-from ..common import validate_input
-from ._base import BaseObservables
-
-
-class CustomObservables(BaseObservables):
-    """
-    Custom observable functions.
-
-    To ensure invertibility of the set of observables, the identity map is
-    automatically included along with user-specified observables.
-
-    Parameters
-    ----------
-    observables: list of callable
-        A list of functions mapping from state variables to observables.
-        Univariate functions are applied to each state variable in turn and
-        multivariable functions are applied to each combination of state
-        variables.
-        Note that the identity map is automatically prepended to this list.
-
-    observable_names: list of callable, optional (default None)
-        A list of functions mapping from names of state variables to names
-        of observables. For example, the observable name
-        :code:`lambda x: f"{x}^2"` would correspond to the function :math:`x^2`.
-        If None, the names "f0(...)", "f1(...)", ... will be used.
-
-    interaction_only: bool, optional (default True)
-        Whether to omit self-interaction terms.
-        If True, function evaluations of the form :math:`f(x,x)` and :math:`f(x,y,x)`
-        will be omitted, but those of the form :math:`f(x,y)` and :math:`f(x,y,z)`
-        will be included.
-        If False, all combinations will be included.
-
-    Attributes
-    ----------
-    n_input_features_ : int
-        Number of input features.
-
-    n_output_features_ : int
-        Number of output features.
-    """
-
-    def __init__(self, observables, observable_names=None, interaction_only=True):
-        super(CustomObservables, self).__init__()
-        self.observables = [identity, *observables]
-        if observable_names and (len(observables) != len(observable_names)):
-            raise ValueError(
-                "observables and observable_names must have the same length"
-            )
-        self.observable_names = observable_names
-        self.interaction_only = interaction_only
-
-    def fit(self, x, y=None):
-        """
-        Fit to measurement data.
-
-        Determines the number of input and output features and creates
-        default values for :code:`observable_names` if necessary.
-
-        Parameters
-        ----------
-        x: array-like, shape (n_samples, n_input_features)
-            Measurement data to be fit.
-
-        y: None
-            Dummy parameter retained for sklearn compatibility.
-
-        Returns
-        -------
-        self: a fit :class:`pykoopman.observables.CustomObservables` instance
-        """
-        n_samples, n_features = validate_input(x).shape
-
-        n_output_features = 0
-        for f in self.observables:
-            n_args = f.__code__.co_argcount
-            n_output_features += len(
-                list(self._combinations(n_features, n_args, self.interaction_only))
-            )
-
-        self.n_input_features_ = n_features
-        self.n_output_features_ = n_output_features
-
-        if self.observable_names is None:
-            self.observable_names = list(
-                map(
-                    lambda i: (lambda *x: "f" + str(i) + "(" + ",".join(x) + ")"),
-                    range(len(self.observables)),
-                )
-            )
-        # First map is the identity
-        self.observable_names.insert(0, identity_name)
-
-        return self
-
-    def transform(self, x):
-        """
-        Apply custom transformations to data, computing observables.
-
-        Parameters
-        ----------
-        x: array-like, shape (n_samples, n_input_features)
-            Measurement data to be transformed.
-
-        Returns
-        -------
-        y: array-like, shape (n_samples, n_output_features)
-            Transformed data (observables).
-        """
-        check_is_fitted(self, "n_input_features_")
-        x = validate_input(x)
-
-        n_samples, n_features = x.shape
-
-        if n_features != self.n_input_features_:
-            raise ValueError("x.shape[1] does not match n_input_features_")
-
-        x_transformed = empty((n_samples, self.n_output_features_), dtype=x.dtype)
-        observables_idx = 0
-        for f in self.observables:
-            for c in self._combinations(
-                self.n_input_features_, f.__code__.co_argcount, self.interaction_only
-            ):
-                x_transformed[:, observables_idx] = f(*[x[:, j] for j in c])
-                observables_idx += 1
-
-        return x_transformed
-
-    def inverse(self, y):
-        """
-        Invert the transformation.
-
-        This function satisfies
-        :code:`self.inverse(self.transform(x)) == x`
-
-        Parameters
-        ----------
-        y: array-like, shape (n_samples, n_output_features)
-            Data to which to apply the inverse.
-            Must have the same number of features as the transformed data
-
-        Returns
-        -------
-        x: array-like, shape (n_samples, n_input_features)
-            Output of inverse map applied to y.
-            In this case, x is identical to y.
-        """
-        y = validate_input(y)
-        check_is_fitted(self, "n_input_features_")
-        if y.shape[1] != self.n_output_features_:
-            raise ValueError(
-                "Wrong number of input features."
-                f"Expected y.shape[1] = {self.n_out_features_}; "
-                f"instead y.shape[1] = {y.shape[1]}."
-            )
-        # self.observables[0] is the identity, so original features are
-        # just the first self.n_input_features_ columns
-        return y[:, : self.n_input_features_]
-
-    def get_feature_names(self, input_features=None):
-        """
-        Get the names of the output features.
-
-        Parameters
-        ----------
-        input_features: list of string, length n_input_features, \
-                optional (default None)
-            String names for input features, if available. By default,
-            the names "x0", "x1", ... ,"xn_input_features" are used.
-
-        Returns
-        -------
-        output_feature_names: list of string, length n_ouput_features
-            Output feature names.
-        """
-        check_is_fitted(self, "n_input_features_")
-        if input_features is None:
-            input_features = [f"x{i}" for i in range(self.n_input_features_)]
-        else:
-            if len(input_features) != self.n_input_features_:
-                raise ValueError(
-                    "input_features must have n_input_features_ "
-                    f"({self.n_input_features_}) elements"
-                )
-
-        feature_names = []
-        for i, f in enumerate(self.observables):
-            feature_names.extend(
-                [
-                    self.observable_names[i](*[input_features[j] for j in c])
-                    for c in self._combinations(
-                        self.n_input_features_,
-                        f.__code__.co_argcount,
-                        self.interaction_only,
-                    )
-                ]
-            )
-
-        return feature_names
-
-    @staticmethod
-    def _combinations(n_features, n_args, interaction_only):
-        """Get the combinations of features to be passed to observable functions."""
-        comb = combinations if interaction_only else combinations_with_replacement
-        return comb(range(n_features), n_args)
-
-
-def identity(x):
-    """Identity map."""
-    return x
-
-
-def identity_name(x):
-    """Name for identity map."""
-    return str(x)
+"""moduel for time-delay observables"""
+from __future__ import annotations
+
+import numpy as np
+from numpy import arange
+from numpy import empty
+from sklearn.utils.validation import check_is_fitted
+
+from ..common import validate_input
+from ._base import BaseObservables
+
+
+class TimeDelay(BaseObservables):
+    """
+    A class for creating time-delay observables. These observables are formed by
+    taking time-lagged measurements of state variables and interpreting them as new
+    state variables.
+
+    The two state variables :math:`[x(t), y(t)]` could be supplemented with two
+    time-delays each, yielding a new set of observables:
+
+    .. math::
+        [x(t), y(t), x(t-\\Delta$ t), y(t-\\Delta t),
+        x(t-2\\Delta t), y(t - 2\\Delta t)]
+
+    This example corresponds to taking :code:`delay =` :math:`\\Delta t` and
+    :code:`n_delays = 2`.
+
+    Note that when transforming data the first :code:`delay * n_delays` rows/samples
+    are dropped as there is insufficient time history to form time-delays for them.
+
+    For more information, see the following references:
+
+        Brunton, Steven L., et al.
+        "Chaos as an intermittently forced linear system."
+        Nature communications 8.1 (2017): 1-9.
+
+        Susuki, Yoshihiko, and Igor Mezić.
+        "A prony approximation of Koopman mode decomposition."
+        2015 54th IEEE Conference on Decision and Control (CDC). IEEE, 2015.
+
+        Arbabi, Hassan, and Igor Mezic.
+        "Ergodic theory, dynamic mode decomposition, and computation
+        of spectral properties of the Koopman operator."
+        SIAM Journal on Applied Dynamical Systems 16.4 (2017): 2096-2126.
+
+    Args:
+        delay (int, optional): The length of each delay. Defaults to 1.
+        n_delays (int, optional): The number of delays to compute for each
+            variable. Defaults to 2.
+
+    Attributes:
+        include_state (bool): If True, includes the system state.
+        delay (int): The length of each delay.
+        n_delays (int): The number of delays to compute for each variable.
+        _n_consumed_samples (int): Number of samples consumed when :code:`transform`
+            is called,i.e. :code:`n_delays * delay`.
+    """
+
+    def __init__(self, delay=1, n_delays=2):
+        """
+        Initialize the TimeDelay class with given parameters.
+
+        Args:
+            delay (int, optional): The length of each delay. Defaults to 1.
+            n_delays (int, optional): The number of delays to compute for each
+                variable. Defaults to 2.
+
+        Raises:
+            ValueError: If delay or n_delays are negative.
+        """
+        super(TimeDelay, self).__init__()
+        if delay < 0:
+            raise ValueError("delay must be a nonnegative int")
+        if n_delays < 0:
+            raise ValueError("n_delays must be a nonnegative int")
+
+        self.include_state = True
+        self.delay = int(delay)
+        self.n_delays = int(n_delays)
+        self._n_consumed_samples = self.delay * self.n_delays
+
+    def fit(self, x, y=None):
+        """
+        Fit the model to measurement data.
+
+        Args:
+            x (array-like): The input data, shape (n_samples, n_input_features).
+            y (None): Dummy parameter for sklearn compatibility.
+
+        Returns:
+            TimeDelay: The fitted instance.
+        """
+
+        x = validate_input(x)
+        n_samples, n_features = x.shape
+
+        self.n_input_features_ = n_features
+        self.n_output_features_ = n_features * (1 + self.n_delays)
+
+        self.measurement_matrix_ = np.zeros(
+            (self.n_input_features_, self.n_output_features_)
+        )
+        self.measurement_matrix_[
+            : self.n_input_features_, : self.n_input_features_
+        ] = np.eye(self.n_input_features_)
+
+        return self
+
+    def transform(self, x):
+        """
+        Add time-delay features to the data, dropping the first :code:`delay -
+        n_delays` samples.
+
+        Args:
+            x (array-like): The input data, shape (n_samples, n_input_features).
+                It is assumed that rows correspond to examples that are equi-spaced
+                in time and are in sequential order.
+
+        Returns:
+            y (array-like): The transformed data, shape (n_samples - delay * n_delays,
+            n_output_features).
+        """
+
+        check_is_fitted(self, "n_input_features_")
+        x = validate_input(x)
+
+        if x.shape[1] != self.n_input_features_:
+            raise ValueError(
+                "Wrong number of input features. "
+                f"Expected x.shape[1] = {self.n_input_features_}; "
+                f"instead x.shape[1] = {x.shape[1]}."
+            )
+
+        self._n_consumed_samples = self.delay * self.n_delays
+        if len(x) < self._n_consumed_samples + 1:
+            raise ValueError(
+                "x has too few rows. To compute time-delay features with "
+                f"delay = {self.delay} and n_delays = {self.n_delays} "
+                f"x must have at least {self._n_consumed_samples + 1} rows."
+            )
+
+        y = empty(
+            (x.shape[0] - self._n_consumed_samples, self.n_output_features_),
+            dtype=x.dtype,
+        )
+        y[:, : self.n_input_features_] = x[self._n_consumed_samples :]
+
+        for i in range(self._n_consumed_samples, x.shape[0]):
+            y[i - self._n_consumed_samples, self.n_input_features_ :] = x[
+                self._delay_inds(i), :
+            ].flatten()
+
+        return y
+
+    def get_feature_names(self, input_features=None):
+        """
+        Get the names of the output features.
+
+        Args:
+            input_features (list of str, optional): Names for input features.
+                If None, defaults to "x0", "x1", ... ,"xn_input_features".
+
+        Returns:
+            list of str: Names of the output features.
+        """
+        check_is_fitted(self, "n_input_features_")
+        if input_features is None:
+            input_features = [f"x{i}" for i in range(self.n_input_features_)]
+        else:
+            if len(input_features) != self.n_input_features_:
+                raise ValueError(
+                    "input_features must have n_input_features_ "
+                    f"({self.n_input_features_}) elements"
+                )
+
+        output_features = [f"{xi}(t)" for xi in input_features]
+        output_features.extend(
+            [
+                f"{xi}(t-{i * self.delay}dt)"
+                for i in range(1, self.n_delays + 1)
+                for xi in input_features
+            ]
+        )
+
+        return output_features
+
+    def _delay_inds(self, index):
+        """
+        Private method to get the indices for the delayed data.
+
+        Args:
+            index (int): The index from which to calculate the delay indices.
+
+        Returns:
+            array-like: The delay indices.
+        """
+        return index - self.delay * arange(1, self.n_delays + 1)
+
+    @property
+    def n_consumed_samples(self):
+        """
+        The number of samples that are consumed as "initial conditions" for
+        other samples, i.e., the number of samples for which time delays cannot
+        be computed.
+
+        Returns:
+            int: The number of consumed samples.
+        """
+        return self._n_consumed_samples
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pykoopman-0.2.0/pykoopman/observables/_identity.py` & `pykoopman-1.0.0/pykoopman/observables/_identity.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,104 +1,81 @@
-"""
-Linear observables
-"""
-from sklearn.utils.validation import check_is_fitted
-
-from ._base import BaseObservables
-
-
-class Identity(BaseObservables):
-    """
-    A dummy observables class that simply returns its input.
-    """
-
-    def __init__(self):
-        super().__init__()
-
-    def fit(self, x, y=None):
-        """
-        Fit to measurement data.
-
-        Parameters
-        ----------
-        x: array-like, shape (n_samples, n_input_features)
-            Measurement data to be fit.
-
-        y: None
-            Dummy parameter retained for sklearn compatibility.
-
-        Returns
-        -------
-        self: a fit :class:`pykoopman.observables.Identity` instance
-        """
-        # TODO: validate input
-        self.n_input_features_ = self.n_output_features_ = x.shape[1]
-
-        return self
-
-    def transform(self, x):
-        """
-        Apply Identity transformation to data.
-
-        Parameters
-        ----------
-        x: array-like, shape (n_samples, n_input_features)
-            Measurement data to be transformed.
-
-        Returns
-        -------
-        y: array-like, shape (n_samples, n_input_features)
-            Transformed data (same as x in this case).
-        """
-        # TODO validate input
-        check_is_fitted(self, "n_input_features_")
-        return x
-
-    def inverse(self, y):
-        """
-        Invert the transformation.
-
-        This function satisfies
-        :code:`self.inverse(self.transform(x)) == x`
-
-        Parameters
-        ----------
-        y: array-like, shape (n_samples, n_output_features)
-            Data to which to apply the inverse.
-            Must have the same number of features as the transformed data
-
-        Returns
-        -------
-        x: array-like, shape (n_samples, n_input_features)
-            Output of inverse map applied to y.
-            In this case, x is identical to y.
-        """
-        # TODO: validate input
-        check_is_fitted(self, "n_input_features_")
-        return y
-
-    def get_feature_names(self, input_features=None):
-        """
-        Get the names of the output features.
-
-        Parameters
-        ----------
-        input_features: list of string, length n_input_features,\
-         optional (default None)
-            String names for input features, if available. By default,
-            the names "x0", "x1", ... ,"xn_input_features" are used.
-
-        Returns
-        -------
-        output_feature_names: list of string, length n_ouput_features
-            Output feature names.
-        """
-        check_is_fitted(self, "n_input_features_")
-        if input_features is None:
-            input_features = [f"x{i}" for i in range(self.n_input_features_)]
-        else:
-            if len(input_features) != self.n_input_features_:
-                raise ValueError(
-                    "input_features must have n_input_features_ "
-                    f"({self.n_input_features_}) elements"
-                )
-        return input_features
+"""module for Linear observables"""
+from __future__ import annotations
+
+import numpy as np
+from sklearn.utils.validation import check_is_fitted
+
+from ..common import validate_input
+from ._base import BaseObservables
+
+
+class Identity(BaseObservables):
+    """
+    A dummy observables class that simply returns its input.
+    """
+
+    def __init__(self):
+        """
+        Initialize the Identity class.
+
+        This constructor initializes the Identity class which simply returns its input
+        when transformed.
+        """
+        super().__init__()
+        self.include_state = True
+
+    def fit(self, x, y=None):
+        """
+        Fit the model to the provided measurement data.
+
+        Args:
+            x (array-like): The measurement data to be fit. It must have a shape of
+                (n_samples, n_input_features).
+            y (None): This parameter is retained for sklearn compatibility.
+
+        Returns:
+            self: Returns a fit instance of the class `pykoopman.observables.Identity`.
+        """
+        x = validate_input(x)
+        self.n_input_features_ = self.n_output_features_ = x.shape[1]
+        self.n_consumed_samples = 0
+
+        self.measurement_matrix_ = np.eye(x.shape[1]).T
+        return self
+
+    def transform(self, x):
+        """
+        Apply Identity transformation to the provided data.
+
+        Args:
+            x (array-like): The measurement data to be transformed. It must have a
+                shape of (n_samples, n_input_features).
+
+        Returns:
+            array-like: Returns the transformed data which is the same as the input
+                data in this case.
+        """
+        check_is_fitted(self, "n_input_features_")
+        return x
+
+    def get_feature_names(self, input_features=None):
+        """
+        Get the names of the output features.
+
+        Args:
+            input_features (list of string, optional): The string names for input
+                features, if available. By default, the names "x0", "x1", ... ,
+                "xn_input_features" are used.
+
+        Returns:
+            list of string: Returns the output feature names.
+        """
+        check_is_fitted(self, "n_input_features_")
+        if input_features is None:
+            input_features = [f"x{i}" for i in range(self.n_input_features_)]
+        else:
+            if len(input_features) != self.n_input_features_:
+                raise ValueError(
+                    "input_features must have n_input_features_ "
+                    f"({self.n_input_features_}) elements"
+                )
+        return input_features
```

### Comparing `pykoopman-0.2.0/pykoopman/regression/_dmdc.py` & `pykoopman-1.0.0/pykoopman/regression/_havok.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,277 +1,327 @@
-import numpy as np
-from sklearn.utils.validation import check_is_fitted
-
-from ._base import BaseRegressor
-
-
-class DMDc(BaseRegressor):
-    """
-    DMD with control (DMDc) regressor.
-
-    Aims to determine the system matrices A,B
-    that satisfy x' = Ax + Bu, where x' is the time-shifted
-    state w.r.t. x und u is the control input, for
-    known and unknown B.
-
-    Minimizes the objective function
-    :math:`\\|X'-AX-BU\\|_F`
-    using least-squares regression and singular value decomposition
-    of the input [X,U] and output spaces [X'] to cope with
-    high-dimensionality of X.
-
-    See the following reference for more details:
-
-        `Procter, Joshua L., Brunton, Steven L., and Kutz, J. Nathan.
-        "Dynamic Mode Decomposition with Control."
-        SIAM J. Appl. Dyn. Syst., 15(1), 142–161.
-        <https://epubs.siam.org/doi/abs/10.1137/15M1013857?mobileUi=0>`_
-
-    Parameters
-    ----------
-    svd_rank : int, optional (default None)
-        SVD rank of the input data (x,u), which determines the dimensionality
-        of the projected state and control matrices.
-
-    svd_output_rank : int, optional (default 0)
-        Input and output spaces may vary.
-
-    Attributed
-    ----------
-    coef_ : array, shape (n_input_features_, n_input_features_) or
-        (n_input_features_, n_input_features_ + n_control_features_)
-        Weight vectors of the regression problem. Corresponds to either [A] or [A,B]
-
-    state_matrix_ : array, shape (n_input_features_, n_input_features_)
-        Identified state transition matrix A of the underlying system.
-
-    control_matrix_ : array, shape (n_input_features_, n_control_features_)
-        Identified control matrix B of the underlying system.
-
-    projection_matrix_ : array, shape (n_input_features_+n_control_features_, svd_rank)
-        Projection matrix into low-dimensional subspace.
-
-    projection_matrix_output_ : array, shape (n_input_features_+n_control_features_,
-                                              svd_output_rank)
-        Projection matrix into low-dimensional subspace.
-
-     Examples
-    --------
-    For known B
-    >>> import numpy as np
-    >>> import pykoopman as pk
-    >>> A = np.matrix([[1.5, 0],[0, 0.1]])
-    >>> B = np.matrix([[1],[0]])
-    >>> x0 = np.array([4,7])
-    >>> u = np.array([-4, -2, -1, -0.5, 0, 0.5, 1, 3, 5])
-    >>> n = len(u)+1
-    >>> x = np.zeros([n,len(x0)])
-    >>> x[0,:] = x0
-    >>> for i in range(n-1):
-    >>>     x[i+1,:] = A.dot(x[i,:]) + B.dot(u[np.newaxis,i])
-    >>> X1 = x[:-1,:]
-    >>> X2 = x[1:,:]
-    >>> C = u[:,np.newaxis]
-    >>> DMDc = pk.regression.DMDc(svd_rank=3, control_matrix=B)
-    >>> model = pk.Koopman(regressor=DMDc)
-    >>> model.fit(x,C)
-    >>> Aest = model.state_transition_matrix
-    >>> Best = model.control_matrix
-    >>> print(Aest)
-    >>> np.allclose(A,Aest)
-    [[ 1.50000000e+00 -1.36609474e-17]
-     [-1.58023594e-17  1.00000000e-01]]
-    True
-
-    For unknown B
-    >>> DMDc = pk.regression.DMDc(svd_rank=3)
-    >>> model = pk.Koopman(regressor=DMDc)
-    >>> model.fit(x,C)
-    >>> Aest = model.state_transition_matrix
-    >>> Best = model.control_matrix
-    >>> print(Aest)
-    >>> print(Best)
-    >>> np.allclose(np.concatenate((A,B),axis=1),np.concatenate((Aest,Best),axis=1))
-    [[ 1.5000000e+00  4.6891744e-17]
-     [-1.3259342e-17  1.0000000e-01]]
-    [[1.00000000e+00]
-     [6.88569357e-18]]
-    True
-    """
-
-    def __init__(self, svd_rank=None, svd_output_rank=None, control_matrix=None):
-        self.svd_rank = svd_rank
-        self.svd_output_rank = svd_output_rank
-        self.control_matrix_ = control_matrix
-
-    def fit(self, x, u, y=None, dt=None):
-        """
-        Parameters
-        ----------
-        x: numpy ndarray, shape (n_samples, n_features)
-            Measurement data to be fit.
-
-        u: numpy.ndarray, shape (n_samples, n_control_features), \
-                optional (default None)
-            Time series of external actuation/control.
-
-        Returns
-        -------
-        self: returns a fitted ``DMDc`` instance
-        """
-        self.n_samples_, self.n_input_features_ = x.shape
-        # if dt is None:
-        #     self.time_ = dict([ ('tstart', 0),
-        #                         ('tend', self.n_samples_ - 1),
-        #                         ('dt', 1)])
-        # else:
-        #     self.time_ = dict([('tstart', 0),
-        #                        ('tend', dt*(self.n_samples_ - 1)),
-        #                        ('dt', dt)])
-
-        if y is None:
-            X1 = x[:-1, :]
-            X2 = x[1:, :]
-        else:
-            X1 = x
-            X2 = y
-
-        if u.ndim == 1:
-            if len(u) > X1.shape[0]:
-                u = u[:-1]
-            C = u[np.newaxis, :]
-        elif u.ndim == 2:
-            if u.shape[0] > X1.shape[0]:
-                u = u[:-1, :]
-            C = u
-        self.n_control_features_ = C.shape[1]
-
-        if self.svd_rank is None:
-            self.svd_rank = self.n_input_features_ + self.n_control_features_
-        r = self.svd_rank
-
-        if self.svd_output_rank is None:
-            self.svd_output_rank = self.n_input_features_
-        rout = self.svd_output_rank
-
-        if self.control_matrix_ is None:
-            self.fit_unknown_B(X1, X2, C, r, rout)
-
-        else:
-            self.fit_known_B(X1, X2, C, r)
-        return self
-
-    def fit_unknown_B(self, X1, X2, C, r, rout):
-        Omega = np.vstack([X1.T, C.T])
-
-        # SVD of input space
-        U, s, Vh = np.linalg.svd(Omega, full_matrices=False)
-        Ur = U[:, 0:r]
-        Sr = np.diag(s[0:r])
-        Vr = Vh[0:r, :].T
-
-        # SVD of output space
-        if rout is not self.n_input_features_:
-            Uhat, _, _ = np.linalg.svd(X2.T, full_matrices=False)
-            Uhatr = Uhat[:, 0:rout]
-        else:
-            Uhatr = np.identity(self.n_input_features_)
-
-        U1 = Ur[: self.n_input_features_, :]
-        U2 = Ur[self.n_input_features_ :, :]
-        self.state_matrix_ = np.dot(
-            Uhatr.T,
-            np.dot(X2.T, np.dot(Vr, np.dot(np.linalg.inv(Sr), np.dot(U1.T, Uhatr)))),
-        )
-        self.control_matrix_ = np.dot(
-            Uhatr.T, np.dot(X2.T, np.dot(Vr, np.dot(np.linalg.inv(Sr), U2.T)))
-        )
-        G = np.concatenate((self.state_matrix_, self.control_matrix_), axis=1)
-
-        self.coef_ = G
-        self.projection_matrix_ = Ur
-        self.projection_matrix_output_ = Uhatr
-
-        # Compute Koopman modes, eigenvectors, eigenvalues
-        [self.eigenvalues_, self.eigenvectors_] = np.linalg.eig(self.state_matrix_)
-        self.modes_ = np.dot(
-            X2.T,
-            np.dot(
-                Vr,
-                np.dot(
-                    np.linalg.inv(Sr), np.dot(U1.T, np.dot(Uhatr, self.eigenvectors_))
-                ),
-            ),
-        )
-
-    def fit_known_B(self, X1, X2, C, r):
-        if self.n_input_features_ in self.control_matrix_.shape is False:
-            raise TypeError("Control vector/matrix B has wrong shape.")
-        if self.control_matrix_.shape[1] == self.n_input_features_:
-            self.control_matrix_ = self.control_matrix_.T
-        if self.control_matrix_.shape[1] != self.n_control_features_:
-            raise TypeError(
-                "The control matrix B must have the same number of inputs as the "
-                "control variable u."
-            )
-
-        U, s, Vh = np.linalg.svd(X1.T, full_matrices=False)
-        A = np.dot(
-            X2.T - np.dot(self.control_matrix_, C.T),
-            np.dot(Vh.T * (s ** (-1)), U.T),
-        )
-        self.state_matrix_ = A
-        G = A
-        Ur = np.identity(self.n_input_features_)
-        Uhatr = np.identity(self.n_input_features_)
-
-        self.coef_ = G
-        self.projection_matrix_ = Ur
-        self.projection_matrix_output_ = Uhatr
-
-        # Compute Koopman modes, eigenvectors, eigenvalues
-        [self.eigenvalues_, self.eigenvectors_] = np.linalg.eig(self.state_matrix_)
-        self.modes_ = np.dot(
-            X2.T, np.dot(Vh.T * (s ** (-1)), np.dot(U.T, self.eigenvectors_))
-        )
-
-    def predict(self, x, u):
-        """
-        Parameters
-        ----------
-        x: numpy ndarray, shape (n_samples, n_features)
-            Measurement data upon which to base prediction.
-
-        u: numpy.ndarray, shape (n_samples, n_control_features), \
-                optional (default None)
-            Time series of external actuation/control.
-
-        Returns
-        -------
-        y: numpy ndarray, shape (n_samples, n_features)
-            Prediction of x one timestep in the future.
-
-        """
-        check_is_fitted(self, "coef_")
-        y = np.dot(self.state_matrix_, x.T) + np.dot(self.control_matrix_, u.T)
-        return y.T
-
-    # @property
-    # def frequencies_(self):
-    #     """
-    #     Oscillation frequencies of Koopman modes/eigenvectors
-    #     """
-    #     check_is_fitted(self, "coef_")
-    #     dt = self.time_['dt']
-    #     return np.imag(np.log(self.eigenvalues_)/dt)/(2*np.pi)
-
-    # @property
-    # def eigenvalues_continuous_(self):
-    #     """
-    #     Continuous-time Koopman eigenvalues obtained from spectral decomposition of
-    #     the Koopman matrix
-    #     """
-    #     check_is_fitted(self, "coef_")
-    #     dt = self.time_['dt']
-    #     return np.log(self.eigenvalues_) / dt
-
-    # TODO: function to set time information --> in Koopman, here not necessary
+"""module for havok"""
+from __future__ import annotations
+
+from warnings import warn
+
+import numpy as np
+from matplotlib import pyplot as plt
+from optht import optht
+from scipy.signal import lsim
+from scipy.signal import lti
+from sklearn.utils.validation import check_is_fitted
+
+from ..common import drop_nan_rows
+from ..differentiation._derivative import Derivative
+from ._base import BaseRegressor
+
+
+class HAVOK(BaseRegressor):
+    """
+    HAVOK (Hankel Alternative View of Koopman) regressor.
+
+    Aims to determine the system matrices A, B that satisfy d/dt v = Av + Bu,
+    where v is the vector of the leading delay coordinates and u is a low-energy
+    delay coordinate acting as forcing. A and B are the unknown system and control
+    matrices, respectively. The delay coordinates are obtained by computing the
+    SVD from a Hankel matrix.
+
+    The objective function, \\|dV-AV-BU\\|_F, is minimized using least-squares
+    regression.
+
+    See the following reference for more details:
+        Brunton, S.L., Brunton, B.W., Proctor, J.L., Kaiser, E. & Kutz, J.N.
+        "Chaos as an intermittently forced linear system."
+        Nature Communications, Vol. 8(19), 2017.
+        <https://www.nature.com/articles/s41467-017-00030-8>
+
+    Parameters:
+        svd_rank (int, optional):
+            Rank of the SVD used for model reduction. Defaults to None.
+        differentiator (Derivative, optional):
+            Differentiation method to compute the time derivative. Defaults to
+            Derivative(kind="finite_difference", k=1).
+        plot_sv (bool, optional):
+            Whether to plot the singular values. Defaults to False.
+
+    Attributes:
+        coef_ (array):
+            Weight vectors of the regression problem. Corresponds to either [A] or
+            [A,B].
+        state_matrix_ (array):
+            Identified state transition matrix A of the underlying system.
+        control_matrix_ (array):
+            Identified control matrix B of the underlying system.
+        projection_matrix_ (array):
+            Projection matrix into low-dimensional subspace of shape (n_input_features
+            +n_control_features, svd_rank).
+        projection_matrix_output_ (array):
+            Projection matrix into low-dimensional subspace of shape (n_input_features
+            +n_control_features, svd_output_rank).
+    """
+
+    def __init__(
+        self,
+        svd_rank=None,
+        differentiator=Derivative(kind="finite_difference", k=1),
+        plot_sv=False,
+    ):
+        """
+        Initialize the HAVOK regressor.
+
+        Args:
+            svd_rank (int, optional):
+                Rank of the SVD used for model reduction. Defaults to None.
+            differentiator (Derivative, optional):
+                Differentiation method to compute the time derivative. Defaults to
+                Derivative(kind="finite_difference", k=1).
+            plot_sv (bool, optional):
+                Whether to plot the singular values. Defaults to False.
+        """
+        self.svd_rank = svd_rank
+        self.differentiator = differentiator
+        self.plot_sv = plot_sv
+
+    def fit(self, x, y=None, dt=None):
+        """
+        Fit the HAVOK regressor to the given data.
+
+        Args:
+            x (numpy.ndarray):
+                Measurement data to be fit.
+            y (not used):
+                Time-shifted measurement data to be fit. Ignored.
+            dt (scalar):
+                Discrete time-step.
+
+        Returns:
+            self: Fitted HAVOK instance.
+        """
+
+        if y is not None:
+            warn("havok regressor does not require the y argument when fitting.")
+
+        if dt is None:
+            raise ValueError("havok regressor requires a timestep dt when fitting.")
+
+        self.dt_ = dt
+        self.n_samples_, self.n_input_features_ = x.shape
+        self.n_control_features_ = 1
+
+        # Create time vector
+        t = np.arange(0, self.dt_ * self.n_samples_, self.dt_)
+
+        # SVD to calculate intrinsic observables
+        U, s, Vh = np.linalg.svd(x.T, full_matrices=False)
+
+        if self.plot_sv:
+            plt.figure()
+            plt.semilogy(s)
+            plt.xlabel("number of terms")
+            plt.ylabel("singular values")
+            plt.show()
+
+        # calculate rank using optimal hard threshold by Gavish & Donoho
+        if self.svd_rank is None:
+            self.svd_rank = optht(x, sv=s, sigma=None)
+        Vrh = Vh[: self.svd_rank, :]
+        Vr = Vrh.T
+        Ur = U[:, : self.svd_rank]
+        sr = s[: self.svd_rank]
+
+        # calculate time derivative dxdt of only the first rank-1 & normalize
+        dVr = self.differentiator(Vr[:, :-1], t)
+        # this line actually makes vh and dvh transposed
+        dVr, t, V = drop_nan_rows(dVr, t, Vh.T)
+
+        # regression on intrinsic variables v
+        # xi = np.zeros((self.svd_rank - 1, self.svd_rank))
+        # for i in range(self.svd_rank - 1):
+        #     # here, we use rank terms in V to fit the rank-1 terms dV/dt
+        #     # we perform column wise
+        #     xi[i, :] = np.linalg.lstsq(Vr, dVr[:, i], rcond=None)[0]
+
+        xi = np.linalg.lstsq(Vr, dVr, rcond=None)[0].T
+        assert xi.shape == (self.svd_rank - 1, self.svd_rank)
+
+        self.forcing_signal = Vr[:, -1]
+        self._state_matrix_ = xi[:, :-1]
+        self._control_matrix_ = xi[:, -1].reshape(-1, 1)
+
+        self.svals = s
+        self._ur = Ur[:, :-1] @ np.diag(sr[:-1])
+        self._coef_ = np.hstack([self.state_matrix_, self.control_matrix_])
+
+        eigenvalues_, self._eigenvectors_ = np.linalg.eig(self.state_matrix_)
+        # because we fit the model in continuous time,
+        # so we need to convert to discrete time
+        self._eigenvalues_ = np.exp(eigenvalues_ * dt)
+
+        self._unnormalized_modes = self._ur @ self.eigenvectors_
+        self._tmp_compute_psi = np.linalg.inv(self.eigenvectors_) @ self._ur.T
+
+        # self.C = np.linalg.multi_dot(
+        #     [
+        #         np.linalg.inv(self.eigenvectors_),
+        #         np.diag(np.reciprocal(s[: self.svd_rank - 1])),
+        #         U[:, : self.svd_rank - 1].T,
+        #     ]
+        # )
+
+    def predict(self, x, u, t):
+        """
+        Predict the output based on the input data.
+
+        Args:
+            x (numpy.ndarray):
+                Measurement data upon which to base prediction.
+            u (numpy.ndarray):
+                Time series of external actuation/control, which is sampled at time
+                instances in `t`.
+            t (numpy.ndarray):
+                Time vector. Instances at which the solution vector shall be provided.
+                Note: The time vector must start at 0.
+
+        Returns:
+            y (numpy.ndarray):
+                Prediction of `x` at the time instances provided in `t`.
+        """
+        # if t[0] != 0:
+        #    raise ValueError("the time vector must start at 0.")
+
+        check_is_fitted(self, "coef_")
+        y0 = (
+            # np.linalg.inv(np.diag(self.svals[: self.svd_rank - 1]))
+            # @
+            np.linalg.pinv(self._ur)
+            @ x.T
+        )
+        sys = lti(
+            self.state_matrix_,
+            self.control_matrix_,
+            self._ur,
+            np.zeros((self.n_input_features_, self.n_control_features_)),
+        )
+        tout, ypred, xpred = lsim(sys, U=u, T=t, X0=y0.T)
+        return ypred
+
+    def _compute_phi(self, x_col):
+        """
+        Compute the feature vector `phi(x)` given `x`.
+
+        Args:
+            x_col (numpy.ndarray):
+                Input data `x` for computing `phi(x)`.
+
+        Returns:
+            phi (numpy.ndarray):
+                Value of `phi(x)`.
+
+        """
+        if x_col.ndim == 1:
+            x_col = x_col.reshape(-1, 1)
+        phi = self._ur.T @ x_col
+        return phi
+
+    def _compute_psi(self, x_col):
+        """
+        Compute the feature vector `psi(x)` given `x`.
+
+        Args:
+            x_col (numpy.ndarray):
+                Input data `x` for computing `psi(x)`.
+
+        Returns:
+            psi (numpy.ndarray):
+                Value of `psi(x)`.
+
+        """
+        # compute psi - one column if x is a row
+        if x_col.ndim == 1:
+            x_col = x_col.reshape(-1, 1)
+        psi = self._tmp_compute_psi @ x_col
+        return psi
+
+    @property
+    def coef_(self):
+        """
+        Get the weight vectors of the regression problem.
+
+        Returns:
+            coef (numpy.ndarray):
+                Weight vectors of the regression problem. Corresponds to either [A]
+                or [A,B].
+        """
+        check_is_fitted(self, "_coef_")
+        return self._coef_
+
+    @property
+    def state_matrix_(self):
+        """
+        Get the identified state transition matrix A of the underlying system.
+
+        Returns:
+            state_matrix (numpy.ndarray):
+                Identified state transition matrix A.
+        """
+        check_is_fitted(self, "_state_matrix_")
+        return self._state_matrix_
+
+    @property
+    def control_matrix_(self):
+        """
+        Get the identified control matrix B of the underlying system.
+
+        Returns:
+            control_matrix (numpy.ndarray):
+                Identified control matrix B.
+        """
+        check_is_fitted(self, "_control_matrix_")
+        return self._control_matrix_
+
+    @property
+    def eigenvectors_(self):
+        """
+        Get the identified eigenvectors of the state matrix A.
+
+        Returns:
+            eigenvectors (numpy.ndarray):
+                Identified eigenvectors of the state matrix A.
+        """
+        check_is_fitted(self, "_eigenvectors_")
+        return self._eigenvectors_
+
+    @property
+    def eigenvalues_(self):
+        """
+        Get the identified eigenvalues of the state matrix A.
+
+        Returns:
+            eigenvalues (numpy.ndarray):
+                Identified eigenvalues of the state matrix A.
+        """
+        check_is_fitted(self, "_eigenvalues_")
+        return self._eigenvalues_
+
+    @property
+    def unnormalized_modes(self):
+        """
+        Get the identified unnormalized modes.
+
+        Returns:
+            unnormalized_modes (numpy.ndarray):
+                Identified unnormalized modes.
+        """
+        check_is_fitted(self, "_unnormalized_modes")
+        return self._unnormalized_modes
+
+    @property
+    def ur(self):
+        """
+        Get the matrix UR.
+
+        Returns:
+            ur (numpy.ndarray):
+                Matrix UR.
+        """
+        check_is_fitted(self, "_ur")
+        return self._ur
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pykoopman-0.2.0/pykoopman.egg-info/SOURCES.txt` & `pykoopman-1.0.0/pykoopman.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,90 @@
 .git_archival.txt
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
-.readthedocs.yml
+.readthedocs.yaml
 LICENSE
 README.rst
+codecov.yml
+pyproject.toml
 requirements-dev.txt
+requirements-torch.txt
 requirements.txt
-setup.cfg
-setup.py
 .github/workflows/release.yaml
 .github/workflows/run-tests.yml
+docs/Makefile
 docs/conf.py
 docs/index.rst
-examples/README.rst
-examples/differentiation.ipynb
-examples/example_notebook.ipynb
-examples/observables.ipynb
-examples/tutorial_dmdc_sparse_linear_system.ipynb
-examples/tutorial_koopman_linearsystem.ipynb
-examples/tutorial_koopman_with_control.ipynb
-examples/tutorial_linear_random_control_system.ipynb
+docs/make.bat
+docs/tutorial_compose_observables.ipynb
+docs/tutorial_compute_differentiation.ipynb
+docs/tutorial_dmd_failed_for_pde_examples.ipynb
+docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb
+docs/tutorial_dmd_succeeds_pde_examples.ipynb
+docs/tutorial_dmd_with_control_128d_system.ipynb
+docs/tutorial_dmd_with_control_2d_system.ipynb
+docs/tutorial_koopman_edmd_with_rbf.ipynb
+docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb
+docs/tutorial_koopman_edmdc_for_vdp_system.ipynb
+docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb
+docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb
+docs/tutorial_koopman_havok_3d_lorenz.ipynb
+docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb
+docs/tutorial_koopman_nndmd_examples.ipynb
+docs/tutorial_linear_random_control_system.ipynb
+docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb
+docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb
+docs/JOSS/Fig1.png
+docs/JOSS/Fig2.png
+docs/JOSS/Fig3.png
+docs/JOSS/codemeta.json
+docs/JOSS/default.csl
+docs/JOSS/generate.rb
+docs/JOSS/paper.bib
+docs/JOSS/paper.md
 pykoopman/__init__.py
 pykoopman/koopman.py
 pykoopman/koopman_continuous.py
-pykoopman/koopman_discrete.py
 pykoopman.egg-info/PKG-INFO
 pykoopman.egg-info/SOURCES.txt
 pykoopman.egg-info/dependency_links.txt
-pykoopman.egg-info/requires.txt
 pykoopman.egg-info/top_level.txt
+pykoopman/analytics/__init__.py
+pykoopman/analytics/_base_analyzer.py
+pykoopman/analytics/_ms_pd21.py
+pykoopman/analytics/_pruned_koopman.py
 pykoopman/common/__init__.py
+pykoopman/common/cqgle.py
 pykoopman/common/examples.py
+pykoopman/common/ks.py
+pykoopman/common/nlse.py
 pykoopman/common/validation.py
+pykoopman/common/vbe.py
 pykoopman/differentiation/__init__.py
 pykoopman/differentiation/_derivative.py
 pykoopman/differentiation/_finite_difference.py
 pykoopman/observables/__init__.py
 pykoopman/observables/_base.py
 pykoopman/observables/_custom_observables.py
 pykoopman/observables/_identity.py
 pykoopman/observables/_polynomial.py
+pykoopman/observables/_radial_basis_functions.py
+pykoopman/observables/_random_fourier_features.py
 pykoopman/observables/_time_delay.py
 pykoopman/regression/__init__.py
 pykoopman/regression/_base.py
+pykoopman/regression/_base_ensemble.py
 pykoopman/regression/_dmd.py
 pykoopman/regression/_dmdc.py
+pykoopman/regression/_edmd.py
+pykoopman/regression/_edmdc.py
+pykoopman/regression/_havok.py
+pykoopman/regression/_kdmd.py
+pykoopman/regression/_nndmd.py
 test/conftest.py
 test/test_koopman.py
 test/test_koopman_continuous.py
+test/analytics/test_analytics.py
 test/differentiation/test_differentiation.py
 test/observables/test_observables.py
 test/regression/test_regressors.py
```


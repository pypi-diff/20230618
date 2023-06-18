# Comparing `tmp/pykoopman-1.0.0.tar.gz` & `tmp/pykoopman-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykoopman-1.0.0.tar", last modified: Sun Jun 18 02:27:45 2023, max compression
+gzip compressed data, was "pykoopman-1.0.1.tar", last modified: Sun Jun 18 03:08:37 2023, max compression
```

## Comparing `pykoopman-1.0.0.tar` & `pykoopman-1.0.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.884422 pykoopman-1.0.0/
--rw-rw-rw-   0        0        0       24 2023-02-16 18:09:30.000000 pykoopman-1.0.0/.git_archival.txt
--rw-rw-rw-   0        0        0      169 2023-02-16 18:09:30.000000 pykoopman-1.0.0/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.824047 pykoopman-1.0.0/.github/
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.836445 pykoopman-1.0.0/.github/workflows/
--rw-rw-rw-   0        0        0      656 2023-06-15 07:39:59.000000 pykoopman-1.0.0/.github/workflows/release.yaml
--rw-rw-rw-   0        0        0     1337 2023-06-15 23:56:43.000000 pykoopman-1.0.0/.github/workflows/run-tests.yml
--rw-rw-rw-   0        0        0      418 2023-03-27 06:02:36.000000 pykoopman-1.0.0/.gitignore
--rw-rw-rw-   0        0        0      788 2023-02-16 18:09:30.000000 pykoopman-1.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      773 2023-06-15 07:39:59.000000 pykoopman-1.0.0/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1118 2023-06-15 07:39:59.000000 pykoopman-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     9102 2023-06-18 02:27:45.884422 pykoopman-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8325 2023-06-18 02:27:38.000000 pykoopman-1.0.0/README.rst
--rw-rw-rw-   0        0        0      246 2023-06-15 07:39:59.000000 pykoopman-1.0.0/codecov.yml
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.853443 pykoopman-1.0.0/docs/
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.858440 pykoopman-1.0.0/docs/JOSS/
--rw-rw-rw-   0        0        0   128421 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/Fig1.png
--rw-rw-rw-   0        0        0    66677 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/Fig2.png
--rw-rw-rw-   0        0        0    28248 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/Fig3.png
--rw-rw-rw-   0        0        0     1824 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/codemeta.json
--rw-rw-rw-   0        0        0    16242 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/default.csl
--rw-rw-rw-   0        0        0     4820 2023-04-12 18:22:22.000000 pykoopman-1.0.0/docs/JOSS/generate.rb
--rw-rw-rw-   0        0        0    37209 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/paper.bib
--rw-rw-rw-   0        0        0    11132 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/JOSS/paper.md
--rw-rw-rw-   0        0        0      654 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/Makefile
--rw-rw-rw-   0        0        0     3388 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/conf.py
--rw-rw-rw-   0        0        0     1222 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/index.rst
--rwxrwxrwx   0        0        0      800 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/make.bat
--rw-rw-rw-   0        0        0  1048136 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_compose_observables.ipynb
--rw-rw-rw-   0        0        0    70466 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_compute_differentiation.ipynb
--rw-rw-rw-   0        0        0  1660826 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_failed_for_pde_examples.ipynb
--rw-rw-rw-   0        0        0   412334 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb
--rw-rw-rw-   0        0        0  1433953 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_succeeds_pde_examples.ipynb
--rw-rw-rw-   0        0        0  1363247 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_with_control_128d_system.ipynb
--rw-rw-rw-   0        0        0    42474 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_dmd_with_control_2d_system.ipynb
--rw-rw-rw-   0        0        0   215931 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_edmd_with_rbf.ipynb
--rw-rw-rw-   0        0        0   494059 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb
--rw-rw-rw-   0        0        0   389950 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb
--rw-rw-rw-   0        0        0   450330 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb
--rw-rw-rw-   0        0        0   393560 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb
--rw-rw-rw-   0        0        0   622478 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_havok_3d_lorenz.ipynb
--rw-rw-rw-   0        0        0   397898 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb
--rw-rw-rw-   0        0        0   242503 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_koopman_nndmd_examples.ipynb
--rw-rw-rw-   0        0        0   344701 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_linear_random_control_system.ipynb
--rw-rw-rw-   0        0        0  1152333 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb
--rw-rw-rw-   0        0        0   299511 2023-06-15 07:39:59.000000 pykoopman-1.0.0/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.860442 pykoopman-1.0.0/pykoopman/
--rw-rw-rw-   0        0        0      473 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.869322 pykoopman-1.0.0/pykoopman/analytics/
--rw-rw-rw-   0        0        0      237 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/analytics/__init__.py
--rw-rw-rw-   0        0        0     3024 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/analytics/_base_analyzer.py
--rw-rw-rw-   0        0        0    20052 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/analytics/_ms_pd21.py
--rw-rw-rw-   0        0        0     5270 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/analytics/_pruned_koopman.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.872419 pykoopman-1.0.0/pykoopman/common/
--rw-rw-rw-   0        0        0      860 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/common/__init__.py
--rw-rw-rw-   0        0        0     7292 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/common/cqgle.py
--rw-rw-rw-   0        0        0    34090 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/common/examples.py
--rw-rw-rw-   0        0        0     6092 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/common/ks.py
--rw-rw-rw-   0        0        0     5893 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/common/nlse.py
--rw-rw-rw-   0        0        0     2184 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/common/validation.py
--rw-rw-rw-   0        0        0     5204 2023-05-22 05:30:39.000000 pykoopman-1.0.0/pykoopman/common/vbe.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.873415 pykoopman-1.0.0/pykoopman/differentiation/
--rw-rw-rw-   0        0        0      173 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/differentiation/__init__.py
--rw-rw-rw-   0        0        0     2535 2023-05-22 05:30:38.000000 pykoopman-1.0.0/pykoopman/differentiation/_derivative.py
--rw-rw-rw-   0        0        0      270 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/differentiation/_finite_difference.py
--rw-rw-rw-   0        0        0    22105 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/koopman.py
--rw-rw-rw-   0        0        0     6067 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/koopman_continuous.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.877412 pykoopman-1.0.0/pykoopman/observables/
--rw-rw-rw-   0        0        0      471 2023-02-16 18:09:30.000000 pykoopman-1.0.0/pykoopman/observables/__init__.py
--rw-rw-rw-   0        0        0    15145 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_base.py
--rw-rw-rw-   0        0        0     9757 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_custom_observables.py
--rw-rw-rw-   0        0        0     2671 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_identity.py
--rw-rw-rw-   0        0        0    10957 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_polynomial.py
--rw-rw-rw-   0        0        0    11943 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_radial_basis_functions.py
--rw-rw-rw-   0        0        0     7035 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_random_fourier_features.py
--rw-rw-rw-   0        0        0     7467 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/observables/_time_delay.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.881413 pykoopman-1.0.0/pykoopman/regression/
--rw-rw-rw-   0        0        0      465 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/__init__.py
--rw-rw-rw-   0        0        0     2727 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_base.py
--rw-rw-rw-   0        0        0    16027 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_base_ensemble.py
--rw-rw-rw-   0        0        0    12635 2023-06-16 08:24:08.000000 pykoopman-1.0.0/pykoopman/regression/_dmd.py
--rw-rw-rw-   0        0        0    16367 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_dmdc.py
--rw-rw-rw-   0        0        0     8161 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_edmd.py
--rw-rw-rw-   0        0        0     7484 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_edmdc.py
--rw-rw-rw-   0        0        0    10858 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_havok.py
--rw-rw-rw-   0        0        0    16987 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_kdmd.py
--rw-rw-rw-   0        0        0    50849 2023-06-15 07:39:59.000000 pykoopman-1.0.0/pykoopman/regression/_nndmd.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.867452 pykoopman-1.0.0/pykoopman.egg-info/
--rw-rw-rw-   0        0        0     9102 2023-06-18 02:27:45.000000 pykoopman-1.0.0/pykoopman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2924 2023-06-18 02:27:45.000000 pykoopman-1.0.0/pykoopman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 02:27:45.000000 pykoopman-1.0.0/pykoopman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-18 02:27:45.000000 pykoopman-1.0.0/pykoopman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      913 2023-06-18 02:16:13.000000 pykoopman-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      408 2023-06-15 07:39:59.000000 pykoopman-1.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       31 2023-03-26 19:57:13.000000 pykoopman-1.0.0/requirements-torch.txt
--rw-rw-rw-   0        0        0      167 2023-06-15 23:45:02.000000 pykoopman-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 02:27:45.884422 pykoopman-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.882410 pykoopman-1.0.0/test/
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.882410 pykoopman-1.0.0/test/analytics/
--rw-rw-rw-   0        0        0     2351 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/analytics/test_analytics.py
--rw-rw-rw-   0        0        0     7373 2023-02-24 05:43:30.000000 pykoopman-1.0.0/test/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.883413 pykoopman-1.0.0/test/differentiation/
--rw-rw-rw-   0        0        0     2306 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/differentiation/test_differentiation.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.883413 pykoopman-1.0.0/test/observables/
--rw-rw-rw-   0        0        0    14048 2023-04-06 03:39:16.000000 pykoopman-1.0.0/test/observables/test_observables.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:27:45.883413 pykoopman-1.0.0/test/regression/
--rw-rw-rw-   0        0        0     3195 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/regression/test_regressors.py
--rw-rw-rw-   0        0        0    28511 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/test_koopman.py
--rw-rw-rw-   0        0        0     1612 2023-06-15 07:39:59.000000 pykoopman-1.0.0/test/test_koopman_continuous.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.313803 pykoopman-1.0.1/
+-rw-rw-rw-   0        0        0       24 2023-02-16 18:09:30.000000 pykoopman-1.0.1/.git_archival.txt
+-rw-rw-rw-   0        0        0      169 2023-02-16 18:09:30.000000 pykoopman-1.0.1/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.260660 pykoopman-1.0.1/.github/
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.270768 pykoopman-1.0.1/.github/workflows/
+-rw-rw-rw-   0        0        0      656 2023-06-15 07:39:59.000000 pykoopman-1.0.1/.github/workflows/release.yaml
+-rw-rw-rw-   0        0        0     1337 2023-06-15 23:56:43.000000 pykoopman-1.0.1/.github/workflows/run-tests.yml
+-rw-rw-rw-   0        0        0      418 2023-03-27 06:02:36.000000 pykoopman-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0      788 2023-06-18 03:02:02.000000 pykoopman-1.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      773 2023-06-15 07:39:59.000000 pykoopman-1.0.1/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1118 2023-06-15 07:39:59.000000 pykoopman-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     9102 2023-06-18 03:08:37.314804 pykoopman-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8325 2023-06-18 02:27:38.000000 pykoopman-1.0.1/README.rst
+-rw-rw-rw-   0        0        0      246 2023-06-15 07:39:59.000000 pykoopman-1.0.1/codecov.yml
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.285803 pykoopman-1.0.1/docs/
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.289804 pykoopman-1.0.1/docs/JOSS/
+-rw-rw-rw-   0        0        0   128421 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/JOSS/Fig1.png
+-rw-rw-rw-   0        0        0    66677 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/JOSS/Fig2.png
+-rw-rw-rw-   0        0        0    28248 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/JOSS/Fig3.png
+-rw-rw-rw-   0        0        0     1824 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/JOSS/codemeta.json
+-rw-rw-rw-   0        0        0    16242 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/JOSS/default.csl
+-rw-rw-rw-   0        0        0     4820 2023-04-12 18:22:22.000000 pykoopman-1.0.1/docs/JOSS/generate.rb
+-rw-rw-rw-   0        0        0    37209 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/JOSS/paper.bib
+-rw-rw-rw-   0        0        0    11132 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/JOSS/paper.md
+-rw-rw-rw-   0        0        0      654 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/Makefile
+-rw-rw-rw-   0        0        0     3388 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/conf.py
+-rw-rw-rw-   0        0        0     1222 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/make.bat
+-rw-rw-rw-   0        0        0  1048136 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_compose_observables.ipynb
+-rw-rw-rw-   0        0        0    70466 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_compute_differentiation.ipynb
+-rw-rw-rw-   0        0        0  1660826 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_dmd_failed_for_pde_examples.ipynb
+-rw-rw-rw-   0        0        0   412334 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb
+-rw-rw-rw-   0        0        0  1433953 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_dmd_succeeds_pde_examples.ipynb
+-rw-rw-rw-   0        0        0  1363247 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_dmd_with_control_128d_system.ipynb
+-rw-rw-rw-   0        0        0    42474 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_dmd_with_control_2d_system.ipynb
+-rw-rw-rw-   0        0        0   215931 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_koopman_edmd_with_rbf.ipynb
+-rw-rw-rw-   0        0        0   494059 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb
+-rw-rw-rw-   0        0        0   389950 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb
+-rw-rw-rw-   0        0        0   450330 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb
+-rw-rw-rw-   0        0        0   399779 2023-06-18 03:05:19.000000 pykoopman-1.0.1/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb
+-rw-rw-rw-   0        0        0   622478 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_koopman_havok_3d_lorenz.ipynb
+-rw-rw-rw-   0        0        0   397898 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb
+-rw-rw-rw-   0        0        0   242503 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_koopman_nndmd_examples.ipynb
+-rw-rw-rw-   0        0        0   344701 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_linear_random_control_system.ipynb
+-rw-rw-rw-   0        0        0  1152333 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb
+-rw-rw-rw-   0        0        0   299511 2023-06-15 07:39:59.000000 pykoopman-1.0.1/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.290804 pykoopman-1.0.1/pykoopman/
+-rw-rw-rw-   0        0        0      473 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.298804 pykoopman-1.0.1/pykoopman/analytics/
+-rw-rw-rw-   0        0        0      237 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/analytics/__init__.py
+-rw-rw-rw-   0        0        0     3024 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/analytics/_base_analyzer.py
+-rw-rw-rw-   0        0        0    20052 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/analytics/_ms_pd21.py
+-rw-rw-rw-   0        0        0     5270 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/analytics/_pruned_koopman.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.301803 pykoopman-1.0.1/pykoopman/common/
+-rw-rw-rw-   0        0        0      860 2023-02-16 18:09:30.000000 pykoopman-1.0.1/pykoopman/common/__init__.py
+-rw-rw-rw-   0        0        0     7292 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/common/cqgle.py
+-rw-rw-rw-   0        0        0    34090 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/common/examples.py
+-rw-rw-rw-   0        0        0     6092 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/common/ks.py
+-rw-rw-rw-   0        0        0     5893 2023-02-16 18:09:30.000000 pykoopman-1.0.1/pykoopman/common/nlse.py
+-rw-rw-rw-   0        0        0     2184 2023-02-16 18:09:30.000000 pykoopman-1.0.1/pykoopman/common/validation.py
+-rw-rw-rw-   0        0        0     5204 2023-05-22 05:30:39.000000 pykoopman-1.0.1/pykoopman/common/vbe.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.303804 pykoopman-1.0.1/pykoopman/differentiation/
+-rw-rw-rw-   0        0        0      173 2023-02-16 18:09:30.000000 pykoopman-1.0.1/pykoopman/differentiation/__init__.py
+-rw-rw-rw-   0        0        0     2535 2023-05-22 05:30:38.000000 pykoopman-1.0.1/pykoopman/differentiation/_derivative.py
+-rw-rw-rw-   0        0        0      270 2023-02-16 18:09:30.000000 pykoopman-1.0.1/pykoopman/differentiation/_finite_difference.py
+-rw-rw-rw-   0        0        0    22105 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/koopman.py
+-rw-rw-rw-   0        0        0     6067 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/koopman_continuous.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.306804 pykoopman-1.0.1/pykoopman/observables/
+-rw-rw-rw-   0        0        0      471 2023-02-16 18:09:30.000000 pykoopman-1.0.1/pykoopman/observables/__init__.py
+-rw-rw-rw-   0        0        0    15145 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/observables/_base.py
+-rw-rw-rw-   0        0        0     9757 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/observables/_custom_observables.py
+-rw-rw-rw-   0        0        0     2671 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/observables/_identity.py
+-rw-rw-rw-   0        0        0    10957 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/observables/_polynomial.py
+-rw-rw-rw-   0        0        0    11943 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/observables/_radial_basis_functions.py
+-rw-rw-rw-   0        0        0     7035 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/observables/_random_fourier_features.py
+-rw-rw-rw-   0        0        0     7467 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/observables/_time_delay.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.310804 pykoopman-1.0.1/pykoopman/regression/
+-rw-rw-rw-   0        0        0      465 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/__init__.py
+-rw-rw-rw-   0        0        0     2727 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/_base.py
+-rw-rw-rw-   0        0        0    16027 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/_base_ensemble.py
+-rw-rw-rw-   0        0        0    12635 2023-06-16 08:24:08.000000 pykoopman-1.0.1/pykoopman/regression/_dmd.py
+-rw-rw-rw-   0        0        0    16367 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/_dmdc.py
+-rw-rw-rw-   0        0        0     8161 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/_edmd.py
+-rw-rw-rw-   0        0        0     7484 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/_edmdc.py
+-rw-rw-rw-   0        0        0    10858 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/_havok.py
+-rw-rw-rw-   0        0        0    16987 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/_kdmd.py
+-rw-rw-rw-   0        0        0    50849 2023-06-15 07:39:59.000000 pykoopman-1.0.1/pykoopman/regression/_nndmd.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.297805 pykoopman-1.0.1/pykoopman.egg-info/
+-rw-rw-rw-   0        0        0     9102 2023-06-18 03:08:37.000000 pykoopman-1.0.1/pykoopman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-06-18 03:08:37.000000 pykoopman-1.0.1/pykoopman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 03:08:37.000000 pykoopman-1.0.1/pykoopman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-18 03:08:37.000000 pykoopman-1.0.1/pykoopman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      915 2023-06-18 03:08:13.000000 pykoopman-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      408 2023-06-15 07:39:59.000000 pykoopman-1.0.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       31 2023-03-26 19:57:13.000000 pykoopman-1.0.1/requirements-torch.txt
+-rw-rw-rw-   0        0        0      167 2023-06-15 23:45:02.000000 pykoopman-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0      395 2023-06-18 03:08:37.317844 pykoopman-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.311804 pykoopman-1.0.1/test/
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.312803 pykoopman-1.0.1/test/analytics/
+-rw-rw-rw-   0        0        0     2351 2023-06-15 07:39:59.000000 pykoopman-1.0.1/test/analytics/test_analytics.py
+-rw-rw-rw-   0        0        0     7373 2023-02-24 05:43:30.000000 pykoopman-1.0.1/test/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.312803 pykoopman-1.0.1/test/differentiation/
+-rw-rw-rw-   0        0        0     2306 2023-06-15 07:39:59.000000 pykoopman-1.0.1/test/differentiation/test_differentiation.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.312803 pykoopman-1.0.1/test/observables/
+-rw-rw-rw-   0        0        0    14048 2023-04-06 03:39:16.000000 pykoopman-1.0.1/test/observables/test_observables.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:08:37.313803 pykoopman-1.0.1/test/regression/
+-rw-rw-rw-   0        0        0     3195 2023-06-15 07:39:59.000000 pykoopman-1.0.1/test/regression/test_regressors.py
+-rw-rw-rw-   0        0        0    28511 2023-06-15 07:39:59.000000 pykoopman-1.0.1/test/test_koopman.py
+-rw-rw-rw-   0        0        0     1612 2023-06-15 07:39:59.000000 pykoopman-1.0.1/test/test_koopman_continuous.py
```

### Comparing `pykoopman-1.0.0/.github/workflows/release.yaml` & `pykoopman-1.0.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/.github/workflows/run-tests.yml` & `pykoopman-1.0.1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/.pre-commit-config.yaml` & `pykoopman-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/.readthedocs.yaml` & `pykoopman-1.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/LICENSE` & `pykoopman-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/PKG-INFO` & `pykoopman-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykoopman
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for data-driven approximations to the Koopman operator.
 Author-email: Shaowu Pan <shawnpan@uw.edu>, Eurika Kaiser <eurika@uw.edu>, Brian de Silva <bdesilva@uw.edu>
 Project-URL: Homepage, https://github.com/dynamicslab/pykoopman
 Project-URL: Bug Tracker, https://github.com/dynamicslab/pykoopman/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pykoopman-1.0.0/README.rst` & `pykoopman-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/JOSS/Fig1.png` & `pykoopman-1.0.1/docs/JOSS/Fig1.png`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/JOSS/Fig2.png` & `pykoopman-1.0.1/docs/JOSS/Fig2.png`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/JOSS/Fig3.png` & `pykoopman-1.0.1/docs/JOSS/Fig3.png`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/JOSS/codemeta.json` & `pykoopman-1.0.1/docs/JOSS/codemeta.json`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/JOSS/default.csl` & `pykoopman-1.0.1/docs/JOSS/default.csl`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/JOSS/generate.rb` & `pykoopman-1.0.1/docs/JOSS/generate.rb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/JOSS/paper.bib` & `pykoopman-1.0.1/docs/JOSS/paper.bib`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/JOSS/paper.md` & `pykoopman-1.0.1/docs/JOSS/paper.md`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/Makefile` & `pykoopman-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/conf.py` & `pykoopman-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/index.rst` & `pykoopman-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/make.bat` & `pykoopman-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_compose_observables.ipynb` & `pykoopman-1.0.1/docs/tutorial_compose_observables.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_compute_differentiation.ipynb` & `pykoopman-1.0.1/docs/tutorial_compute_differentiation.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_dmd_failed_for_pde_examples.ipynb` & `pykoopman-1.0.1/docs/tutorial_dmd_failed_for_pde_examples.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb` & `pykoopman-1.0.1/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_dmd_succeeds_pde_examples.ipynb` & `pykoopman-1.0.1/docs/tutorial_dmd_succeeds_pde_examples.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_dmd_with_control_128d_system.ipynb` & `pykoopman-1.0.1/docs/tutorial_dmd_with_control_128d_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_dmd_with_control_2d_system.ipynb` & `pykoopman-1.0.1/docs/tutorial_dmd_with_control_2d_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_koopman_edmd_with_rbf.ipynb` & `pykoopman-1.0.1/docs/tutorial_koopman_edmd_with_rbf.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb` & `pykoopman-1.0.1/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb` & `pykoopman-1.0.1/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb` & `pykoopman-1.0.1/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb` & `pykoopman-1.0.1/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999609375%*

 * *Differences: {"'cells'": "{8: {'outputs': {0: {'data': {'text/html': ['<style>#sk-container-id-1 {color: "*

 * *            'black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 '*

 * *            'div.sk-toggleable {background-color: white;}#sk-container-id-1 '*

 * *            'label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: '*

 * *            '0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 '*

 * *            'label.sk-toggleable__label-arrow […]*

```diff
@@ -160,14 +160,17 @@
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [
                 {
                     "data": {
+                        "text/html": [
+                            "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>Koopman(observables=TimeDelay(n_delays=9), regressor=DMDc())</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item sk-dashed-wrapped\"><div class=\"sk-label-container\"><div class=\"sk-label sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" ><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">Koopman</label><div class=\"sk-toggleable__content\"><pre>Koopman(observables=TimeDelay(n_delays=9), regressor=DMDc())</pre></div></div></div><div class=\"sk-parallel\"><div class=\"sk-parallel-item\"><div class=\"sk-item\"><div class=\"sk-label-container\"><div class=\"sk-label sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-2\" type=\"checkbox\" ><label for=\"sk-estimator-id-2\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">observables: TimeDelay</label><div class=\"sk-toggleable__content\"><pre>TimeDelay(n_delays=9)</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-3\" type=\"checkbox\" ><label for=\"sk-estimator-id-3\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">TimeDelay</label><div class=\"sk-toggleable__content\"><pre>TimeDelay(n_delays=9)</pre></div></div></div></div></div></div><div class=\"sk-parallel-item\"><div class=\"sk-item\"><div class=\"sk-label-container\"><div class=\"sk-label sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-4\" type=\"checkbox\" ><label for=\"sk-estimator-id-4\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">regressor: DMDc</label><div class=\"sk-toggleable__content\"><pre>DMDc()</pre></div></div></div><div class=\"sk-serial\"><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-5\" type=\"checkbox\" ><label for=\"sk-estimator-id-5\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">DMDc</label><div class=\"sk-toggleable__content\"><pre>DMDc()</pre></div></div></div></div></div></div></div></div></div></div>"
+                        ],
                         "text/plain": [
                             "Koopman(observables=TimeDelay(n_delays=9), regressor=DMDc())"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
```

### Comparing `pykoopman-1.0.0/docs/tutorial_koopman_havok_3d_lorenz.ipynb` & `pykoopman-1.0.1/docs/tutorial_koopman_havok_3d_lorenz.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb` & `pykoopman-1.0.1/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_koopman_nndmd_examples.ipynb` & `pykoopman-1.0.1/docs/tutorial_koopman_nndmd_examples.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_linear_random_control_system.ipynb` & `pykoopman-1.0.1/docs/tutorial_linear_random_control_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb` & `pykoopman-1.0.1/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb` & `pykoopman-1.0.1/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/analytics/_base_analyzer.py` & `pykoopman-1.0.1/pykoopman/analytics/_base_analyzer.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/analytics/_ms_pd21.py` & `pykoopman-1.0.1/pykoopman/analytics/_ms_pd21.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/analytics/_pruned_koopman.py` & `pykoopman-1.0.1/pykoopman/analytics/_pruned_koopman.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/common/__init__.py` & `pykoopman-1.0.1/pykoopman/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/common/cqgle.py` & `pykoopman-1.0.1/pykoopman/common/cqgle.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/common/examples.py` & `pykoopman-1.0.1/pykoopman/common/examples.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/common/ks.py` & `pykoopman-1.0.1/pykoopman/common/ks.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/common/nlse.py` & `pykoopman-1.0.1/pykoopman/common/nlse.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/common/validation.py` & `pykoopman-1.0.1/pykoopman/common/validation.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/common/vbe.py` & `pykoopman-1.0.1/pykoopman/common/vbe.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/differentiation/_derivative.py` & `pykoopman-1.0.1/pykoopman/differentiation/_derivative.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/koopman.py` & `pykoopman-1.0.1/pykoopman/koopman.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/koopman_continuous.py` & `pykoopman-1.0.1/pykoopman/koopman_continuous.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/observables/_base.py` & `pykoopman-1.0.1/pykoopman/observables/_base.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/observables/_custom_observables.py` & `pykoopman-1.0.1/pykoopman/observables/_custom_observables.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/observables/_identity.py` & `pykoopman-1.0.1/pykoopman/observables/_identity.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/observables/_polynomial.py` & `pykoopman-1.0.1/pykoopman/observables/_polynomial.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/observables/_radial_basis_functions.py` & `pykoopman-1.0.1/pykoopman/observables/_radial_basis_functions.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/observables/_random_fourier_features.py` & `pykoopman-1.0.1/pykoopman/observables/_random_fourier_features.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/observables/_time_delay.py` & `pykoopman-1.0.1/pykoopman/observables/_time_delay.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_base.py` & `pykoopman-1.0.1/pykoopman/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_base_ensemble.py` & `pykoopman-1.0.1/pykoopman/regression/_base_ensemble.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_dmd.py` & `pykoopman-1.0.1/pykoopman/regression/_dmd.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_dmdc.py` & `pykoopman-1.0.1/pykoopman/regression/_dmdc.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_edmd.py` & `pykoopman-1.0.1/pykoopman/regression/_edmd.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_edmdc.py` & `pykoopman-1.0.1/pykoopman/regression/_edmdc.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_havok.py` & `pykoopman-1.0.1/pykoopman/regression/_havok.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_kdmd.py` & `pykoopman-1.0.1/pykoopman/regression/_kdmd.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman/regression/_nndmd.py` & `pykoopman-1.0.1/pykoopman/regression/_nndmd.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/pykoopman.egg-info/PKG-INFO` & `pykoopman-1.0.1/pykoopman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykoopman
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for data-driven approximations to the Koopman operator.
 Author-email: Shaowu Pan <shawnpan@uw.edu>, Eurika Kaiser <eurika@uw.edu>, Brian de Silva <bdesilva@uw.edu>
 Project-URL: Homepage, https://github.com/dynamicslab/pykoopman
 Project-URL: Bug Tracker, https://github.com/dynamicslab/pykoopman/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pykoopman-1.0.0/pykoopman.egg-info/SOURCES.txt` & `pykoopman-1.0.1/pykoopman.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 LICENSE
 README.rst
 codecov.yml
 pyproject.toml
 requirements-dev.txt
 requirements-torch.txt
 requirements.txt
+setup.cfg
 .github/workflows/release.yaml
 .github/workflows/run-tests.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/tutorial_compose_observables.ipynb
```

### Comparing `pykoopman-1.0.0/pyproject.toml` & `pykoopman-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0",
     "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pykoopman"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="Shaowu Pan", email="shawnpan@uw.edu" },
     { name="Eurika Kaiser", email="eurika@uw.edu" },
     { name="Brian de Silva", email="bdesilva@uw.edu" }
 ]
 description = "Python package for data-driven approximations to the Koopman operator."
 readme = "README.rst"
@@ -22,8 +22,8 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dynamicslab/pykoopman"
-"Bug Tracker" = "https://github.com/dynamicslab/pykoopman/issues"
+"Bug Tracker" = "https://github.com/dynamicslab/pykoopman/issues"
```

### Comparing `pykoopman-1.0.0/test/analytics/test_analytics.py` & `pykoopman-1.0.1/test/analytics/test_analytics.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/test/conftest.py` & `pykoopman-1.0.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/test/differentiation/test_differentiation.py` & `pykoopman-1.0.1/test/differentiation/test_differentiation.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/test/observables/test_observables.py` & `pykoopman-1.0.1/test/observables/test_observables.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/test/regression/test_regressors.py` & `pykoopman-1.0.1/test/regression/test_regressors.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/test/test_koopman.py` & `pykoopman-1.0.1/test/test_koopman.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.0/test/test_koopman_continuous.py` & `pykoopman-1.0.1/test/test_koopman_continuous.py`

 * *Files identical despite different names*


# Comparing `tmp/pykoopman-1.0.2.tar.gz` & `tmp/pykoopman-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykoopman-1.0.2.tar", last modified: Sun Jun 18 03:37:51 2023, max compression
+gzip compressed data, was "pykoopman-1.0.3.tar", last modified: Sun Jun 18 03:40:08 2023, max compression
```

## Comparing `pykoopman-1.0.2.tar` & `pykoopman-1.0.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.450828 pykoopman-1.0.2/
--rw-rw-rw-   0        0        0       24 2023-02-16 18:09:30.000000 pykoopman-1.0.2/.git_archival.txt
--rw-rw-rw-   0        0        0      169 2023-02-16 18:09:30.000000 pykoopman-1.0.2/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.396785 pykoopman-1.0.2/.github/
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.405784 pykoopman-1.0.2/.github/workflows/
--rw-rw-rw-   0        0        0      656 2023-06-15 07:39:59.000000 pykoopman-1.0.2/.github/workflows/release.yaml
--rw-rw-rw-   0        0        0     1337 2023-06-15 23:56:43.000000 pykoopman-1.0.2/.github/workflows/run-tests.yml
--rw-rw-rw-   0        0        0      418 2023-03-27 06:02:36.000000 pykoopman-1.0.2/.gitignore
--rw-rw-rw-   0        0        0      788 2023-06-18 03:02:02.000000 pykoopman-1.0.2/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      773 2023-06-15 07:39:59.000000 pykoopman-1.0.2/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1118 2023-06-15 07:39:59.000000 pykoopman-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     9246 2023-06-18 03:37:51.450828 pykoopman-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8469 2023-06-18 03:37:17.000000 pykoopman-1.0.2/README.rst
--rw-rw-rw-   0        0        0      246 2023-06-15 07:39:59.000000 pykoopman-1.0.2/codecov.yml
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.421855 pykoopman-1.0.2/docs/
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.425828 pykoopman-1.0.2/docs/JOSS/
--rw-rw-rw-   0        0        0   128421 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/JOSS/Fig1.png
--rw-rw-rw-   0        0        0    66677 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/JOSS/Fig2.png
--rw-rw-rw-   0        0        0    28248 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/JOSS/Fig3.png
--rw-rw-rw-   0        0        0     1824 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/JOSS/codemeta.json
--rw-rw-rw-   0        0        0    16242 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/JOSS/default.csl
--rw-rw-rw-   0        0        0     4820 2023-04-12 18:22:22.000000 pykoopman-1.0.2/docs/JOSS/generate.rb
--rw-rw-rw-   0        0        0    37209 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/JOSS/paper.bib
--rw-rw-rw-   0        0        0    11132 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/JOSS/paper.md
--rw-rw-rw-   0        0        0      654 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/Makefile
--rw-rw-rw-   0        0        0     3388 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/conf.py
--rw-rw-rw-   0        0        0     1222 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/index.rst
--rwxrwxrwx   0        0        0      800 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/make.bat
--rw-rw-rw-   0        0        0  1048136 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_compose_observables.ipynb
--rw-rw-rw-   0        0        0    70466 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_compute_differentiation.ipynb
--rw-rw-rw-   0        0        0  1660826 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_dmd_failed_for_pde_examples.ipynb
--rw-rw-rw-   0        0        0   412334 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb
--rw-rw-rw-   0        0        0  1433953 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_dmd_succeeds_pde_examples.ipynb
--rw-rw-rw-   0        0        0  1363247 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_dmd_with_control_128d_system.ipynb
--rw-rw-rw-   0        0        0    42474 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_dmd_with_control_2d_system.ipynb
--rw-rw-rw-   0        0        0   215931 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_koopman_edmd_with_rbf.ipynb
--rw-rw-rw-   0        0        0   494059 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb
--rw-rw-rw-   0        0        0   389950 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb
--rw-rw-rw-   0        0        0   450330 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb
--rw-rw-rw-   0        0        0   399779 2023-06-18 03:05:19.000000 pykoopman-1.0.2/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb
--rw-rw-rw-   0        0        0   622478 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_koopman_havok_3d_lorenz.ipynb
--rw-rw-rw-   0        0        0   397898 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb
--rw-rw-rw-   0        0        0   242503 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_koopman_nndmd_examples.ipynb
--rw-rw-rw-   0        0        0   344701 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_linear_random_control_system.ipynb
--rw-rw-rw-   0        0        0  1152333 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb
--rw-rw-rw-   0        0        0   299511 2023-06-15 07:39:59.000000 pykoopman-1.0.2/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.426828 pykoopman-1.0.2/pykoopman/
--rw-rw-rw-   0        0        0      473 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.436828 pykoopman-1.0.2/pykoopman/analytics/
--rw-rw-rw-   0        0        0      237 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/analytics/__init__.py
--rw-rw-rw-   0        0        0     3024 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/analytics/_base_analyzer.py
--rw-rw-rw-   0        0        0    20052 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/analytics/_ms_pd21.py
--rw-rw-rw-   0        0        0     5270 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/analytics/_pruned_koopman.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.439827 pykoopman-1.0.2/pykoopman/common/
--rw-rw-rw-   0        0        0      860 2023-02-16 18:09:30.000000 pykoopman-1.0.2/pykoopman/common/__init__.py
--rw-rw-rw-   0        0        0     7292 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/common/cqgle.py
--rw-rw-rw-   0        0        0    34090 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/common/examples.py
--rw-rw-rw-   0        0        0     6092 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/common/ks.py
--rw-rw-rw-   0        0        0     5893 2023-02-16 18:09:30.000000 pykoopman-1.0.2/pykoopman/common/nlse.py
--rw-rw-rw-   0        0        0     2184 2023-02-16 18:09:30.000000 pykoopman-1.0.2/pykoopman/common/validation.py
--rw-rw-rw-   0        0        0     5204 2023-05-22 05:30:39.000000 pykoopman-1.0.2/pykoopman/common/vbe.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.440830 pykoopman-1.0.2/pykoopman/differentiation/
--rw-rw-rw-   0        0        0      173 2023-02-16 18:09:30.000000 pykoopman-1.0.2/pykoopman/differentiation/__init__.py
--rw-rw-rw-   0        0        0     2535 2023-05-22 05:30:38.000000 pykoopman-1.0.2/pykoopman/differentiation/_derivative.py
--rw-rw-rw-   0        0        0      270 2023-02-16 18:09:30.000000 pykoopman-1.0.2/pykoopman/differentiation/_finite_difference.py
--rw-rw-rw-   0        0        0    22105 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/koopman.py
--rw-rw-rw-   0        0        0     6067 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/koopman_continuous.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.443828 pykoopman-1.0.2/pykoopman/observables/
--rw-rw-rw-   0        0        0      471 2023-02-16 18:09:30.000000 pykoopman-1.0.2/pykoopman/observables/__init__.py
--rw-rw-rw-   0        0        0    15145 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/observables/_base.py
--rw-rw-rw-   0        0        0     9757 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/observables/_custom_observables.py
--rw-rw-rw-   0        0        0     2671 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/observables/_identity.py
--rw-rw-rw-   0        0        0    10957 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/observables/_polynomial.py
--rw-rw-rw-   0        0        0    11943 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/observables/_radial_basis_functions.py
--rw-rw-rw-   0        0        0     7035 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/observables/_random_fourier_features.py
--rw-rw-rw-   0        0        0     7467 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/observables/_time_delay.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.447829 pykoopman-1.0.2/pykoopman/regression/
--rw-rw-rw-   0        0        0      465 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/__init__.py
--rw-rw-rw-   0        0        0     2727 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/_base.py
--rw-rw-rw-   0        0        0    16027 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/_base_ensemble.py
--rw-rw-rw-   0        0        0    12635 2023-06-16 08:24:08.000000 pykoopman-1.0.2/pykoopman/regression/_dmd.py
--rw-rw-rw-   0        0        0    16367 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/_dmdc.py
--rw-rw-rw-   0        0        0     8161 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/_edmd.py
--rw-rw-rw-   0        0        0     7484 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/_edmdc.py
--rw-rw-rw-   0        0        0    10858 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/_havok.py
--rw-rw-rw-   0        0        0    16987 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/_kdmd.py
--rw-rw-rw-   0        0        0    50849 2023-06-15 07:39:59.000000 pykoopman-1.0.2/pykoopman/regression/_nndmd.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.435829 pykoopman-1.0.2/pykoopman.egg-info/
--rw-rw-rw-   0        0        0     9246 2023-06-18 03:37:51.000000 pykoopman-1.0.2/pykoopman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2934 2023-06-18 03:37:51.000000 pykoopman-1.0.2/pykoopman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 03:37:51.000000 pykoopman-1.0.2/pykoopman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-18 03:37:51.000000 pykoopman-1.0.2/pykoopman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      915 2023-06-18 03:37:31.000000 pykoopman-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      408 2023-06-15 07:39:59.000000 pykoopman-1.0.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       31 2023-03-26 19:57:13.000000 pykoopman-1.0.2/requirements-torch.txt
--rw-rw-rw-   0        0        0      167 2023-06-15 23:45:02.000000 pykoopman-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0      395 2023-06-18 03:37:51.454828 pykoopman-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.448827 pykoopman-1.0.2/test/
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.448827 pykoopman-1.0.2/test/analytics/
--rw-rw-rw-   0        0        0     2351 2023-06-15 07:39:59.000000 pykoopman-1.0.2/test/analytics/test_analytics.py
--rw-rw-rw-   0        0        0     7373 2023-02-24 05:43:30.000000 pykoopman-1.0.2/test/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.449828 pykoopman-1.0.2/test/differentiation/
--rw-rw-rw-   0        0        0     2306 2023-06-15 07:39:59.000000 pykoopman-1.0.2/test/differentiation/test_differentiation.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.449828 pykoopman-1.0.2/test/observables/
--rw-rw-rw-   0        0        0    14048 2023-04-06 03:39:16.000000 pykoopman-1.0.2/test/observables/test_observables.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:37:51.449828 pykoopman-1.0.2/test/regression/
--rw-rw-rw-   0        0        0     3195 2023-06-15 07:39:59.000000 pykoopman-1.0.2/test/regression/test_regressors.py
--rw-rw-rw-   0        0        0    28511 2023-06-15 07:39:59.000000 pykoopman-1.0.2/test/test_koopman.py
--rw-rw-rw-   0        0        0     1612 2023-06-15 07:39:59.000000 pykoopman-1.0.2/test/test_koopman_continuous.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.863376 pykoopman-1.0.3/
+-rw-rw-rw-   0        0        0       24 2023-02-16 18:09:30.000000 pykoopman-1.0.3/.git_archival.txt
+-rw-rw-rw-   0        0        0      169 2023-02-16 18:09:30.000000 pykoopman-1.0.3/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.802271 pykoopman-1.0.3/.github/
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.815272 pykoopman-1.0.3/.github/workflows/
+-rw-rw-rw-   0        0        0      656 2023-06-15 07:39:59.000000 pykoopman-1.0.3/.github/workflows/release.yaml
+-rw-rw-rw-   0        0        0     1337 2023-06-15 23:56:43.000000 pykoopman-1.0.3/.github/workflows/run-tests.yml
+-rw-rw-rw-   0        0        0      418 2023-03-27 06:02:36.000000 pykoopman-1.0.3/.gitignore
+-rw-rw-rw-   0        0        0      788 2023-06-18 03:02:02.000000 pykoopman-1.0.3/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0      773 2023-06-15 07:39:59.000000 pykoopman-1.0.3/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1118 2023-06-15 07:39:59.000000 pykoopman-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     9348 2023-06-18 03:40:08.863376 pykoopman-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8571 2023-06-18 03:39:46.000000 pykoopman-1.0.3/README.rst
+-rw-rw-rw-   0        0        0      246 2023-06-15 07:39:59.000000 pykoopman-1.0.3/codecov.yml
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.832292 pykoopman-1.0.3/docs/
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.836270 pykoopman-1.0.3/docs/JOSS/
+-rw-rw-rw-   0        0        0   128421 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/JOSS/Fig1.png
+-rw-rw-rw-   0        0        0    66677 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/JOSS/Fig2.png
+-rw-rw-rw-   0        0        0    28248 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/JOSS/Fig3.png
+-rw-rw-rw-   0        0        0     1824 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/JOSS/codemeta.json
+-rw-rw-rw-   0        0        0    16242 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/JOSS/default.csl
+-rw-rw-rw-   0        0        0     4820 2023-04-12 18:22:22.000000 pykoopman-1.0.3/docs/JOSS/generate.rb
+-rw-rw-rw-   0        0        0    37209 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/JOSS/paper.bib
+-rw-rw-rw-   0        0        0    11132 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/JOSS/paper.md
+-rw-rw-rw-   0        0        0      654 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/Makefile
+-rw-rw-rw-   0        0        0     3388 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/conf.py
+-rw-rw-rw-   0        0        0     1222 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/make.bat
+-rw-rw-rw-   0        0        0  1048136 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_compose_observables.ipynb
+-rw-rw-rw-   0        0        0    70466 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_compute_differentiation.ipynb
+-rw-rw-rw-   0        0        0  1660826 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_dmd_failed_for_pde_examples.ipynb
+-rw-rw-rw-   0        0        0   412334 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb
+-rw-rw-rw-   0        0        0  1433953 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_dmd_succeeds_pde_examples.ipynb
+-rw-rw-rw-   0        0        0  1363247 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_dmd_with_control_128d_system.ipynb
+-rw-rw-rw-   0        0        0    42474 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_dmd_with_control_2d_system.ipynb
+-rw-rw-rw-   0        0        0   215931 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_koopman_edmd_with_rbf.ipynb
+-rw-rw-rw-   0        0        0   494059 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb
+-rw-rw-rw-   0        0        0   389950 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb
+-rw-rw-rw-   0        0        0   450330 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb
+-rw-rw-rw-   0        0        0   399779 2023-06-18 03:05:19.000000 pykoopman-1.0.3/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb
+-rw-rw-rw-   0        0        0   622478 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_koopman_havok_3d_lorenz.ipynb
+-rw-rw-rw-   0        0        0   397898 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb
+-rw-rw-rw-   0        0        0   242503 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_koopman_nndmd_examples.ipynb
+-rw-rw-rw-   0        0        0   344701 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_linear_random_control_system.ipynb
+-rw-rw-rw-   0        0        0  1152333 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb
+-rw-rw-rw-   0        0        0   299511 2023-06-15 07:39:59.000000 pykoopman-1.0.3/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.837271 pykoopman-1.0.3/pykoopman/
+-rw-rw-rw-   0        0        0      473 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.849376 pykoopman-1.0.3/pykoopman/analytics/
+-rw-rw-rw-   0        0        0      237 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/analytics/__init__.py
+-rw-rw-rw-   0        0        0     3024 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/analytics/_base_analyzer.py
+-rw-rw-rw-   0        0        0    20052 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/analytics/_ms_pd21.py
+-rw-rw-rw-   0        0        0     5270 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/analytics/_pruned_koopman.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.851376 pykoopman-1.0.3/pykoopman/common/
+-rw-rw-rw-   0        0        0      860 2023-02-16 18:09:30.000000 pykoopman-1.0.3/pykoopman/common/__init__.py
+-rw-rw-rw-   0        0        0     7292 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/common/cqgle.py
+-rw-rw-rw-   0        0        0    34090 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/common/examples.py
+-rw-rw-rw-   0        0        0     6092 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/common/ks.py
+-rw-rw-rw-   0        0        0     5893 2023-02-16 18:09:30.000000 pykoopman-1.0.3/pykoopman/common/nlse.py
+-rw-rw-rw-   0        0        0     2184 2023-02-16 18:09:30.000000 pykoopman-1.0.3/pykoopman/common/validation.py
+-rw-rw-rw-   0        0        0     5204 2023-05-22 05:30:39.000000 pykoopman-1.0.3/pykoopman/common/vbe.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.853376 pykoopman-1.0.3/pykoopman/differentiation/
+-rw-rw-rw-   0        0        0      173 2023-02-16 18:09:30.000000 pykoopman-1.0.3/pykoopman/differentiation/__init__.py
+-rw-rw-rw-   0        0        0     2535 2023-05-22 05:30:38.000000 pykoopman-1.0.3/pykoopman/differentiation/_derivative.py
+-rw-rw-rw-   0        0        0      270 2023-02-16 18:09:30.000000 pykoopman-1.0.3/pykoopman/differentiation/_finite_difference.py
+-rw-rw-rw-   0        0        0    22105 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/koopman.py
+-rw-rw-rw-   0        0        0     6067 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/koopman_continuous.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.856377 pykoopman-1.0.3/pykoopman/observables/
+-rw-rw-rw-   0        0        0      471 2023-02-16 18:09:30.000000 pykoopman-1.0.3/pykoopman/observables/__init__.py
+-rw-rw-rw-   0        0        0    15145 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/observables/_base.py
+-rw-rw-rw-   0        0        0     9757 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/observables/_custom_observables.py
+-rw-rw-rw-   0        0        0     2671 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/observables/_identity.py
+-rw-rw-rw-   0        0        0    10957 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/observables/_polynomial.py
+-rw-rw-rw-   0        0        0    11943 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/observables/_radial_basis_functions.py
+-rw-rw-rw-   0        0        0     7035 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/observables/_random_fourier_features.py
+-rw-rw-rw-   0        0        0     7467 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/observables/_time_delay.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.860378 pykoopman-1.0.3/pykoopman/regression/
+-rw-rw-rw-   0        0        0      465 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/__init__.py
+-rw-rw-rw-   0        0        0     2727 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/_base.py
+-rw-rw-rw-   0        0        0    16027 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/_base_ensemble.py
+-rw-rw-rw-   0        0        0    12635 2023-06-16 08:24:08.000000 pykoopman-1.0.3/pykoopman/regression/_dmd.py
+-rw-rw-rw-   0        0        0    16367 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/_dmdc.py
+-rw-rw-rw-   0        0        0     8161 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/_edmd.py
+-rw-rw-rw-   0        0        0     7484 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/_edmdc.py
+-rw-rw-rw-   0        0        0    10858 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/_havok.py
+-rw-rw-rw-   0        0        0    16987 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/_kdmd.py
+-rw-rw-rw-   0        0        0    50849 2023-06-15 07:39:59.000000 pykoopman-1.0.3/pykoopman/regression/_nndmd.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.847377 pykoopman-1.0.3/pykoopman.egg-info/
+-rw-rw-rw-   0        0        0     9348 2023-06-18 03:40:08.000000 pykoopman-1.0.3/pykoopman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-06-18 03:40:08.000000 pykoopman-1.0.3/pykoopman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 03:40:08.000000 pykoopman-1.0.3/pykoopman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-18 03:40:08.000000 pykoopman-1.0.3/pykoopman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      915 2023-06-18 03:39:46.000000 pykoopman-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      408 2023-06-15 07:39:59.000000 pykoopman-1.0.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       31 2023-03-26 19:57:13.000000 pykoopman-1.0.3/requirements-torch.txt
+-rw-rw-rw-   0        0        0      167 2023-06-15 23:45:02.000000 pykoopman-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0      395 2023-06-18 03:40:08.867509 pykoopman-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.861377 pykoopman-1.0.3/test/
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.862376 pykoopman-1.0.3/test/analytics/
+-rw-rw-rw-   0        0        0     2351 2023-06-15 07:39:59.000000 pykoopman-1.0.3/test/analytics/test_analytics.py
+-rw-rw-rw-   0        0        0     7373 2023-02-24 05:43:30.000000 pykoopman-1.0.3/test/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.862376 pykoopman-1.0.3/test/differentiation/
+-rw-rw-rw-   0        0        0     2306 2023-06-15 07:39:59.000000 pykoopman-1.0.3/test/differentiation/test_differentiation.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.863376 pykoopman-1.0.3/test/observables/
+-rw-rw-rw-   0        0        0    14048 2023-04-06 03:39:16.000000 pykoopman-1.0.3/test/observables/test_observables.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:40:08.863376 pykoopman-1.0.3/test/regression/
+-rw-rw-rw-   0        0        0     3195 2023-06-15 07:39:59.000000 pykoopman-1.0.3/test/regression/test_regressors.py
+-rw-rw-rw-   0        0        0    28511 2023-06-15 07:39:59.000000 pykoopman-1.0.3/test/test_koopman.py
+-rw-rw-rw-   0        0        0     1612 2023-06-15 07:39:59.000000 pykoopman-1.0.3/test/test_koopman_continuous.py
```

### Comparing `pykoopman-1.0.2/.github/workflows/release.yaml` & `pykoopman-1.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/.github/workflows/run-tests.yml` & `pykoopman-1.0.3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/.pre-commit-config.yaml` & `pykoopman-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/.readthedocs.yaml` & `pykoopman-1.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/LICENSE` & `pykoopman-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/PKG-INFO` & `pykoopman-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykoopman
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package for data-driven approximations to the Koopman operator.
 Author-email: Shaowu Pan <shawnpan@uw.edu>, Eurika Kaiser <eurika@uw.edu>, Brian de Silva <bdesilva@uw.edu>
 Project-URL: Homepage, https://github.com/dynamicslab/pykoopman
 Project-URL: Bug Tracker, https://github.com/dynamicslab/pykoopman/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
@@ -37,26 +37,26 @@
 
 .. math::
     z = \Phi(x).
 
 If the system state is also contained in such subspace, then effectively, the nonlinear dynamical system is (approximately)
 linearized in a global sense.
 
-.. figure:: ./docs/JOSS/Fig1.png
+.. figure:: https://github.com/dynamicslab/pykoopman/blob/master/docs/JOSS/Fig1.png
 
     Schematic of data-driven approximation of Koopman operator
 
 The goal of data-driven approximation of Koopman
 operator is to find such a set of functions that span such lifted space and the
 transition matrix associated with the lifted system.
 
 Structure of PyKoopman
 ^^^^^^^^^^^^^^^^^^^^^^
 
-.. figure:: ./docs/JOSS/Fig2.png
+.. figure:: https://github.com/dynamicslab/pykoopman/blob/master/docs/JOSS/Fig2.png
 
 PyKoopman package is centered around the ``Koopman`` class and ``KoopmanContinuous`` class. It consists of two key components
 
 * ``observables``: a set of observables functions, which spans the subspace for projection.
 
 * ``regressor``: the optimization algorithm to find the best `fit` for the projection of Koopman operator.
```

### Comparing `pykoopman-1.0.2/README.rst` & `pykoopman-1.0.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 
 .. math::
     z = \Phi(x).
 
 If the system state is also contained in such subspace, then effectively, the nonlinear dynamical system is (approximately)
 linearized in a global sense.
 
-.. figure:: ./docs/JOSS/Fig1.png
+.. figure:: https://github.com/dynamicslab/pykoopman/blob/master/docs/JOSS/Fig1.png
 
     Schematic of data-driven approximation of Koopman operator
 
 The goal of data-driven approximation of Koopman
 operator is to find such a set of functions that span such lifted space and the
 transition matrix associated with the lifted system.
 
 Structure of PyKoopman
 ^^^^^^^^^^^^^^^^^^^^^^
 
-.. figure:: ./docs/JOSS/Fig2.png
+.. figure:: https://github.com/dynamicslab/pykoopman/blob/master/docs/JOSS/Fig2.png
 
 PyKoopman package is centered around the ``Koopman`` class and ``KoopmanContinuous`` class. It consists of two key components
 
 * ``observables``: a set of observables functions, which spans the subspace for projection.
 
 * ``regressor``: the optimization algorithm to find the best `fit` for the projection of Koopman operator.
```

### Comparing `pykoopman-1.0.2/docs/JOSS/Fig1.png` & `pykoopman-1.0.3/docs/JOSS/Fig1.png`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/JOSS/Fig2.png` & `pykoopman-1.0.3/docs/JOSS/Fig2.png`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/JOSS/Fig3.png` & `pykoopman-1.0.3/docs/JOSS/Fig3.png`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/JOSS/codemeta.json` & `pykoopman-1.0.3/docs/JOSS/codemeta.json`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/JOSS/default.csl` & `pykoopman-1.0.3/docs/JOSS/default.csl`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/JOSS/generate.rb` & `pykoopman-1.0.3/docs/JOSS/generate.rb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/JOSS/paper.bib` & `pykoopman-1.0.3/docs/JOSS/paper.bib`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/JOSS/paper.md` & `pykoopman-1.0.3/docs/JOSS/paper.md`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/Makefile` & `pykoopman-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/conf.py` & `pykoopman-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/index.rst` & `pykoopman-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/make.bat` & `pykoopman-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_compose_observables.ipynb` & `pykoopman-1.0.3/docs/tutorial_compose_observables.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_compute_differentiation.ipynb` & `pykoopman-1.0.3/docs/tutorial_compute_differentiation.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_dmd_failed_for_pde_examples.ipynb` & `pykoopman-1.0.3/docs/tutorial_dmd_failed_for_pde_examples.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb` & `pykoopman-1.0.3/docs/tutorial_dmd_separating_two_mixed_signals_400d_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_dmd_succeeds_pde_examples.ipynb` & `pykoopman-1.0.3/docs/tutorial_dmd_succeeds_pde_examples.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_dmd_with_control_128d_system.ipynb` & `pykoopman-1.0.3/docs/tutorial_dmd_with_control_128d_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_dmd_with_control_2d_system.ipynb` & `pykoopman-1.0.3/docs/tutorial_dmd_with_control_2d_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_koopman_edmd_with_rbf.ipynb` & `pykoopman-1.0.3/docs/tutorial_koopman_edmd_with_rbf.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb` & `pykoopman-1.0.3/docs/tutorial_koopman_edmdc_for_chaotic_duffing_oscillator.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb` & `pykoopman-1.0.3/docs/tutorial_koopman_edmdc_for_vdp_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb` & `pykoopman-1.0.3/docs/tutorial_koopman_eigenfunction_model_slow_manifold.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb` & `pykoopman-1.0.3/docs/tutorial_koopman_hankel_dmdc_for_vdp_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_koopman_havok_3d_lorenz.ipynb` & `pykoopman-1.0.3/docs/tutorial_koopman_havok_3d_lorenz.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb` & `pykoopman-1.0.3/docs/tutorial_koopman_kdmd_on_slow_manifold.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_koopman_nndmd_examples.ipynb` & `pykoopman-1.0.3/docs/tutorial_koopman_nndmd_examples.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_linear_random_control_system.ipynb` & `pykoopman-1.0.3/docs/tutorial_linear_random_control_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb` & `pykoopman-1.0.3/docs/tutorial_linear_system_koopman_eigenfunctions_with_edmd_and_nndmd.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb` & `pykoopman-1.0.3/docs/tutorial_sparse_modes_selection_2d_linear_system.ipynb`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/analytics/_base_analyzer.py` & `pykoopman-1.0.3/pykoopman/analytics/_base_analyzer.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/analytics/_ms_pd21.py` & `pykoopman-1.0.3/pykoopman/analytics/_ms_pd21.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/analytics/_pruned_koopman.py` & `pykoopman-1.0.3/pykoopman/analytics/_pruned_koopman.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/common/__init__.py` & `pykoopman-1.0.3/pykoopman/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/common/cqgle.py` & `pykoopman-1.0.3/pykoopman/common/cqgle.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/common/examples.py` & `pykoopman-1.0.3/pykoopman/common/examples.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/common/ks.py` & `pykoopman-1.0.3/pykoopman/common/ks.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/common/nlse.py` & `pykoopman-1.0.3/pykoopman/common/nlse.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/common/validation.py` & `pykoopman-1.0.3/pykoopman/common/validation.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/common/vbe.py` & `pykoopman-1.0.3/pykoopman/common/vbe.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/differentiation/_derivative.py` & `pykoopman-1.0.3/pykoopman/differentiation/_derivative.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/koopman.py` & `pykoopman-1.0.3/pykoopman/koopman.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/koopman_continuous.py` & `pykoopman-1.0.3/pykoopman/koopman_continuous.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/observables/_base.py` & `pykoopman-1.0.3/pykoopman/observables/_base.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/observables/_custom_observables.py` & `pykoopman-1.0.3/pykoopman/observables/_custom_observables.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/observables/_identity.py` & `pykoopman-1.0.3/pykoopman/observables/_identity.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/observables/_polynomial.py` & `pykoopman-1.0.3/pykoopman/observables/_polynomial.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/observables/_radial_basis_functions.py` & `pykoopman-1.0.3/pykoopman/observables/_radial_basis_functions.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/observables/_random_fourier_features.py` & `pykoopman-1.0.3/pykoopman/observables/_random_fourier_features.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/observables/_time_delay.py` & `pykoopman-1.0.3/pykoopman/observables/_time_delay.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_base.py` & `pykoopman-1.0.3/pykoopman/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_base_ensemble.py` & `pykoopman-1.0.3/pykoopman/regression/_base_ensemble.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_dmd.py` & `pykoopman-1.0.3/pykoopman/regression/_dmd.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_dmdc.py` & `pykoopman-1.0.3/pykoopman/regression/_dmdc.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_edmd.py` & `pykoopman-1.0.3/pykoopman/regression/_edmd.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_edmdc.py` & `pykoopman-1.0.3/pykoopman/regression/_edmdc.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_havok.py` & `pykoopman-1.0.3/pykoopman/regression/_havok.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_kdmd.py` & `pykoopman-1.0.3/pykoopman/regression/_kdmd.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman/regression/_nndmd.py` & `pykoopman-1.0.3/pykoopman/regression/_nndmd.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pykoopman.egg-info/PKG-INFO` & `pykoopman-1.0.3/pykoopman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykoopman
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package for data-driven approximations to the Koopman operator.
 Author-email: Shaowu Pan <shawnpan@uw.edu>, Eurika Kaiser <eurika@uw.edu>, Brian de Silva <bdesilva@uw.edu>
 Project-URL: Homepage, https://github.com/dynamicslab/pykoopman
 Project-URL: Bug Tracker, https://github.com/dynamicslab/pykoopman/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 4 - Beta
@@ -37,26 +37,26 @@
 
 .. math::
     z = \Phi(x).
 
 If the system state is also contained in such subspace, then effectively, the nonlinear dynamical system is (approximately)
 linearized in a global sense.
 
-.. figure:: ./docs/JOSS/Fig1.png
+.. figure:: https://github.com/dynamicslab/pykoopman/blob/master/docs/JOSS/Fig1.png
 
     Schematic of data-driven approximation of Koopman operator
 
 The goal of data-driven approximation of Koopman
 operator is to find such a set of functions that span such lifted space and the
 transition matrix associated with the lifted system.
 
 Structure of PyKoopman
 ^^^^^^^^^^^^^^^^^^^^^^
 
-.. figure:: ./docs/JOSS/Fig2.png
+.. figure:: https://github.com/dynamicslab/pykoopman/blob/master/docs/JOSS/Fig2.png
 
 PyKoopman package is centered around the ``Koopman`` class and ``KoopmanContinuous`` class. It consists of two key components
 
 * ``observables``: a set of observables functions, which spans the subspace for projection.
 
 * ``regressor``: the optimization algorithm to find the best `fit` for the projection of Koopman operator.
```

### Comparing `pykoopman-1.0.2/pykoopman.egg-info/SOURCES.txt` & `pykoopman-1.0.3/pykoopman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/pyproject.toml` & `pykoopman-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0",
     "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pykoopman"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name="Shaowu Pan", email="shawnpan@uw.edu" },
     { name="Eurika Kaiser", email="eurika@uw.edu" },
     { name="Brian de Silva", email="bdesilva@uw.edu" }
 ]
 description = "Python package for data-driven approximations to the Koopman operator."
 readme = "README.rst"
```

### Comparing `pykoopman-1.0.2/test/analytics/test_analytics.py` & `pykoopman-1.0.3/test/analytics/test_analytics.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/test/conftest.py` & `pykoopman-1.0.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/test/differentiation/test_differentiation.py` & `pykoopman-1.0.3/test/differentiation/test_differentiation.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/test/observables/test_observables.py` & `pykoopman-1.0.3/test/observables/test_observables.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/test/regression/test_regressors.py` & `pykoopman-1.0.3/test/regression/test_regressors.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/test/test_koopman.py` & `pykoopman-1.0.3/test/test_koopman.py`

 * *Files identical despite different names*

### Comparing `pykoopman-1.0.2/test/test_koopman_continuous.py` & `pykoopman-1.0.3/test/test_koopman_continuous.py`

 * *Files identical despite different names*


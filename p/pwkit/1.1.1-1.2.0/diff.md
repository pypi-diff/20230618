# Comparing `tmp/pwkit-1.1.1.tar.gz` & `tmp/pwkit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwkit-1.1.1.tar", last modified: Sun Jun 18 20:15:28 2023, max compression
+gzip compressed data, was "pwkit-1.2.0.tar", last modified: Sun Jun 18 21:33:36 2023, max compression
```

## Comparing `pwkit-1.1.1.tar` & `pwkit-1.2.0.tar`

### file list

```diff
@@ -1,223 +1,221 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.005752 pwkit-1.1.1/
--rw-r--r--   0 vsts      (1001) docker     (123)      189 2023-06-18 20:14:45.000000 pwkit-1.1.1/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (123)     1063 2023-06-18 20:14:51.000000 pwkit-1.1.1/CHANGELOG.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1072 2023-06-18 20:14:45.000000 pwkit-1.1.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      227 2023-06-18 20:14:45.000000 pwkit-1.1.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      892 2023-06-18 20:15:28.005752 pwkit-1.1.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2215 2023-06-18 20:14:45.000000 pwkit-1.1.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.985752 pwkit-1.1.1/docs/
--rw-r--r--   0 vsts      (1001) docker     (123)     7414 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/Makefile
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.985752 pwkit-1.1.1/docs/source/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.985752 pwkit-1.1.1/docs/source/_static/
--rw-r--r--   0 vsts      (1001) docker     (123)      422 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/_static/pwkit.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.985752 pwkit-1.1.1/docs/source/_templates/
--rw-r--r--   0 vsts      (1001) docker     (123)       85 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/_templates/layout.html
--rw-r--r--   0 vsts      (1001) docker     (123)       83 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/_templates/page.html
--rw-r--r--   0 vsts      (1001) docker     (123)     3919 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/about.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/cli-tools/
--rw-r--r--   0 vsts      (1001) docker     (123)      448 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/cli-tools/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      374 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/cli-tools/pwkit-cli-multitool.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/cli-tools/pwkit-cli-toplevel.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/cli-tools/pwkit-kwargv.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     2991 2023-06-18 20:14:48.000000 pwkit-1.1.1/docs/source/conf.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/environments/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/environments/casa/
--rw-r--r--   0 vsts      (1001) docker     (123)     1678 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/casa/dftdynspec.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     2862 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/casa/dftphotom.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     2276 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/casa/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     7886 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/casa/tasks.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/casa/utilities.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/environments/heasoft/
--rw-r--r--   0 vsts      (1001) docker     (123)     2514 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/heasoft/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      467 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/index.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/environments/sas/
--rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/sas/data.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      532 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/environments/sas/index.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/foundations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3264 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/foundations/core.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      426 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/foundations/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)    13160 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/foundations/io.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     5981 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/foundations/numerical.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/foundations/parallel.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      428 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/foundations/pwkit-simpleenum.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      556 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/index.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/infrastructure/
--rw-r--r--   0 vsts      (1001) docker     (123)      433 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/infrastructure/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      377 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/infrastructure/pwkit-environments-toplevel.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      379 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/infrastructure/pwkit-method_decorator.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/io/
--rw-r--r--   0 vsts      (1001) docker     (123)      483 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/io/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/io/pwkit-inifile.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/io/pwkit-latex.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      425 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/io/pwkit-tabfile.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      382 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/io/pwkit-tinifile.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      383 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/io/pwkit-unicode_to_latex.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     8981 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/io/slurp.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/pwkit/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/pwkit/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)      424 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/cli/astrotool.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      440 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/cli/imtool.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      414 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/cli/latexdriver.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/cli/wrapout.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      371 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/colormaps.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      347 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/contours.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      379 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/data_gui_helpers.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.985752 pwkit-1.1.1/docs/source/pwkit/environments/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/pwkit/environments/casa/
--rw-r--r--   0 vsts      (1001) docker     (123)      407 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/environments/casa/scripting.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      411 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/environments/casa/spwglue.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.989752 pwkit-1.1.1/docs/source/pwkit/environments/ciao/
--rw-r--r--   0 vsts      (1001) docker     (123)      394 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/environments/ciao/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      442 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/ndshow_gtk2.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      442 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/pwkit/ndshow_gtk3.rst
--rw-r--r--   0 vsts      (1001) docker     (123)       52 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/requirements.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.993752 pwkit-1.1.1/docs/source/science/
--rw-r--r--   0 vsts      (1001) docker     (123)     6197 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/basic-astro.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1614 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/dulk-models.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1593 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/fk10-code.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/index.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1835 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/least-squares-modeling.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      448 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-astimage.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      358 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-bblocks.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      380 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-cgs.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      444 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-ellipses.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      390 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-immodel.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      430 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-kbn_conf.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      450 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-lmmin.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      368 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-msmt.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      370 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-pdm.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      378 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-phoenix.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      442 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-radio_cal_models.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      481 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/pwkit-ucd_physics.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     1692 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/sherpa.rst
--rw-r--r--   0 vsts      (1001) docker     (123)     2859 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/science/synphot.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      459 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/section-cli.rst
--rw-r--r--   0 vsts      (1001) docker     (123)      479 2023-06-18 20:14:45.000000 pwkit-1.1.1/docs/source/section-viz.rst
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.993752 pwkit-1.1.1/lmmin_reference/
--rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/dataf
--rw-r--r--   0 vsts      (1001) docker     (123)     3340 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/fdjac2.f
--rw-r--r--   0 vsts      (1001) docker     (123)    15443 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/lmder.f
--rw-r--r--   0 vsts      (1001) docker     (123)    49879 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/lmder1.all.f
--rw-r--r--   0 vsts      (1001) docker     (123)    15544 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/lmdif.f
--rw-r--r--   0 vsts      (1001) docker     (123)    52113 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/lmdif1.all.f
--rw-r--r--   0 vsts      (1001) docker     (123)     8243 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/lmpar.f
--rw-r--r--   0 vsts      (1001) docker     (123)   142529 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/mpfit.pro
--rwxr-xr-x   0 vsts      (1001) docker     (123)    91069 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/mpfit.py
--rw-r--r--   0 vsts      (1001) docker     (123)    96774 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/nmpfit.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6178 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/qrsolv.f
--rw-r--r--   0 vsts      (1001) docker     (123)    28363 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/test.lmder.f
--rw-r--r--   0 vsts      (1001) docker     (123)    19200 2023-06-18 20:14:45.000000 pwkit-1.1.1/lmmin_reference/test.lmdif.f
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.997752 pwkit-1.1.1/pwkit/
--rw-r--r--   0 vsts      (1001) docker     (123)     7842 2023-06-18 20:14:48.000000 pwkit-1.1.1/pwkit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    42907 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/astimage.py
--rw-r--r--   0 vsts      (1001) docker     (123)    52257 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/astutil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16490 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/bblocks.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3877 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/cgs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.001752 pwkit-1.1.1/pwkit/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)    18847 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16143 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/cli/astrotool.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20425 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/cli/imtool.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16802 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/cli/latexdriver.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13022 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/cli/multitool.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10356 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/cli/wrapout.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19078 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/colormaps.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8123 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/contours.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:27.985752 pwkit-1.1.1/pwkit/data/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.001752 pwkit-1.1.1/pwkit/data/bandpasses/
--rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_2mass_H.dat
--rw-r--r--   0 vsts      (1001) docker     (123)     2180 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_2mass_J.dat
--rw-r--r--   0 vsts      (1001) docker     (123)     1614 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_2mass_Ks.dat
--rw-r--r--   0 vsts      (1001) docker     (123)      482 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_bessell_B.dat
--rw-r--r--   0 vsts      (1001) docker     (123)      406 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_bessell_I.dat
--rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_bessell_R.dat
--rw-r--r--   0 vsts      (1001) docker     (123)      628 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_bessell_UX.dat
--rw-r--r--   0 vsts      (1001) docker     (123)      417 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_bessell_V.dat
--rw-r--r--   0 vsts      (1001) docker     (123)      698 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_galex_fuv.dat
--rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_galex_nuv.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    11273 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_lbt_lmircam_L.dat
--rw-r--r--   0 vsts      (1001) docker     (123)      914 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_mearth_ccd715.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    40313 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_J.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    25811 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_Ks.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    33727 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_Lp.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    14615 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_Mp.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    21901 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_h.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    10472 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_wise_1.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    14372 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_wise_2.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    66658 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_wise_3.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    66658 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/filter_wise_4.dat
--rw-r--r--   0 vsts      (1001) docker     (123)    34560 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/sdss3_filter_responses.fits
--rw-r--r--   0 vsts      (1001) docker     (123)    23040 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data/bandpasses/swuw1_20041120v106.arf
--rw-r--r--   0 vsts      (1001) docker     (123)     9871 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/data_gui_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15020 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/dulk_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16299 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/ellipses.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.005752 pwkit-1.1.1/pwkit/environments/
--rw-r--r--   0 vsts      (1001) docker     (123)     7764 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.005752 pwkit-1.1.1/pwkit/environments/casa/
--rw-r--r--   0 vsts      (1001) docker     (123)     6776 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    29520 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/closures.py
--rw-r--r--   0 vsts      (1001) docker     (123)      651 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/cscript_flagcmd.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1031 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/cscript_genantpos.py
--rw-r--r--   0 vsts      (1001) docker     (123)      926 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/cscript_getopacities.py
--rw-r--r--   0 vsts      (1001) docker     (123)      985 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/cscript_importalma.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1017 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/cscript_importevla.py
--rw-r--r--   0 vsts      (1001) docker     (123)      733 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/cscript_plotants.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/cscript_plotcal.py
--rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/cscript_setjy.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13770 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/dftdynspec.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14832 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/dftphotom.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11976 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/dftspect.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21041 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/gpdiagnostics.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5781 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/polmodel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9001 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/scripting.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4663 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/scripting_driver.py
--rw-r--r--   0 vsts      (1001) docker     (123)    22451 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/spwglue.py
--rw-r--r--   0 vsts      (1001) docker     (123)   127155 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/tasks.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12495 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/casa/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.005752 pwkit-1.1.1/pwkit/environments/ciao/
--rw-r--r--   0 vsts      (1001) docker     (123)     5615 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/ciao/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6635 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/ciao/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16793 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/ciao/data.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3294 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/heasoft.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.005752 pwkit-1.1.1/pwkit/environments/jupyter/
--rw-r--r--   0 vsts      (1001) docker     (123)     5805 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/jupyter/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.005752 pwkit-1.1.1/pwkit/environments/sas/
--rw-r--r--   0 vsts      (1001) docker     (123)    21130 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/sas/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17394 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/environments/sas/data.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)    28603 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/fk10.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17764 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/immodel.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10056 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/inifile.py
--rw-r--r--   0 vsts      (1001) docker     (123)    37391 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/io.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4169 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/kbn_conf.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16112 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/kwargv.py
--rw-r--r--   0 vsts      (1001) docker     (123)    22936 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/latex.py
--rw-r--r--   0 vsts      (1001) docker     (123)    92610 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/lmmin.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35377 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/lsqmdl.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8629 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/method_decorator.py
--rw-r--r--   0 vsts      (1001) docker     (123)    68358 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/msmt.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27909 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/ndshow_gtk2.py
--rw-r--r--   0 vsts      (1001) docker     (123)    31984 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/ndshow_gtk3.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6059 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/ninja_syntax.py
--rw-r--r--   0 vsts      (1001) docker     (123)    31478 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/numutil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17148 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/parallel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6754 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/pdm.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3678 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/phoenix.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7694 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/radio_cal_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25865 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/sherpa.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3033 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/simpleenum.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6464 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/slurp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    34181 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/synphot.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9163 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/tabfile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4312 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/tinifile.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11354 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/ucd_physics.py
--rw-r--r--   0 vsts      (1001) docker     (123)    81062 2023-06-18 20:14:45.000000 pwkit-1.1.1/pwkit/unicode_to_latex.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 20:15:28.001752 pwkit-1.1.1/pwkit.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      892 2023-06-18 20:15:27.000000 pwkit-1.1.1/pwkit.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     6010 2023-06-18 20:15:27.000000 pwkit-1.1.1/pwkit.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-18 20:15:27.000000 pwkit-1.1.1/pwkit.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      345 2023-06-18 20:15:27.000000 pwkit-1.1.1/pwkit.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-18 20:15:27.000000 pwkit-1.1.1/pwkit.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       84 2023-06-18 20:15:27.000000 pwkit-1.1.1/pwkit.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-18 20:15:27.000000 pwkit-1.1.1/pwkit.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       84 2023-06-18 20:14:45.000000 pwkit-1.1.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-18 20:15:28.005752 pwkit-1.1.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     3501 2023-06-18 20:14:48.000000 pwkit-1.1.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.059906 pwkit-1.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-06-18 21:32:42.000000 pwkit-1.2.0/.readthedocs.yml
+-rw-r--r--   0 vsts      (1001) docker     (123)     1230 2023-06-18 21:32:48.000000 pwkit-1.2.0/CHANGELOG.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1072 2023-06-18 21:32:42.000000 pwkit-1.2.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      227 2023-06-18 21:32:42.000000 pwkit-1.2.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      892 2023-06-18 21:33:36.059906 pwkit-1.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2215 2023-06-18 21:32:42.000000 pwkit-1.2.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.035905 pwkit-1.2.0/docs/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7414 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/Makefile
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.035905 pwkit-1.2.0/docs/source/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.035905 pwkit-1.2.0/docs/source/_static/
+-rw-r--r--   0 vsts      (1001) docker     (123)      422 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/_static/pwkit.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.035905 pwkit-1.2.0/docs/source/_templates/
+-rw-r--r--   0 vsts      (1001) docker     (123)       85 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/_templates/layout.html
+-rw-r--r--   0 vsts      (1001) docker     (123)       83 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/_templates/page.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     3773 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/about.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.035905 pwkit-1.2.0/docs/source/cli-tools/
+-rw-r--r--   0 vsts      (1001) docker     (123)      448 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/cli-tools/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      374 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/cli-tools/pwkit-cli-multitool.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/cli-tools/pwkit-cli-toplevel.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/cli-tools/pwkit-kwargv.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     2991 2023-06-18 21:32:44.000000 pwkit-1.2.0/docs/source/conf.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.035905 pwkit-1.2.0/docs/source/environments/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.035905 pwkit-1.2.0/docs/source/environments/casa/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1678 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/casa/dftdynspec.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     2862 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/casa/dftphotom.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     2276 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/casa/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     7886 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/casa/tasks.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/casa/utilities.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.035905 pwkit-1.2.0/docs/source/environments/heasoft/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2514 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/heasoft/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      467 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/index.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.039905 pwkit-1.2.0/docs/source/environments/sas/
+-rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/sas/data.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      532 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/environments/sas/index.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.039905 pwkit-1.2.0/docs/source/foundations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3285 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/foundations/core.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      426 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/foundations/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)    13160 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/foundations/io.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     5981 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/foundations/numerical.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/foundations/parallel.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      428 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/foundations/pwkit-simpleenum.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      556 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/index.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.039905 pwkit-1.2.0/docs/source/infrastructure/
+-rw-r--r--   0 vsts      (1001) docker     (123)      433 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/infrastructure/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      377 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/infrastructure/pwkit-environments-toplevel.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      379 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/infrastructure/pwkit-method_decorator.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.039905 pwkit-1.2.0/docs/source/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)      483 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/io/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/io/pwkit-inifile.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/io/pwkit-latex.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      425 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/io/pwkit-tabfile.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      382 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/io/pwkit-tinifile.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      383 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/io/pwkit-unicode_to_latex.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     8981 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/io/slurp.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.039905 pwkit-1.2.0/docs/source/pwkit/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.039905 pwkit-1.2.0/docs/source/pwkit/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)      424 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/cli/astrotool.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      440 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/cli/imtool.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      414 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/cli/latexdriver.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/cli/wrapout.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      371 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/colormaps.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      347 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/contours.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      379 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/data_gui_helpers.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.031905 pwkit-1.2.0/docs/source/pwkit/environments/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.039905 pwkit-1.2.0/docs/source/pwkit/environments/casa/
+-rw-r--r--   0 vsts      (1001) docker     (123)      407 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/environments/casa/scripting.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      411 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/environments/casa/spwglue.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.039905 pwkit-1.2.0/docs/source/pwkit/environments/ciao/
+-rw-r--r--   0 vsts      (1001) docker     (123)      394 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/environments/ciao/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      442 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/pwkit/ndshow_gtk3.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)       40 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/requirements.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.043905 pwkit-1.2.0/docs/source/science/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6197 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/basic-astro.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1614 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/dulk-models.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1593 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/fk10-code.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1835 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/least-squares-modeling.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      448 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-astimage.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      358 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-bblocks.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      380 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-cgs.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      444 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-ellipses.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      390 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-immodel.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      430 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-kbn_conf.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      450 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-lmmin.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      368 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-msmt.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      370 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-pdm.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      378 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-phoenix.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      442 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-radio_cal_models.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      481 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/pwkit-ucd_physics.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     1692 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/sherpa.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)     2859 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/science/synphot.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      459 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/section-cli.rst
+-rw-r--r--   0 vsts      (1001) docker     (123)      454 2023-06-18 21:32:42.000000 pwkit-1.2.0/docs/source/section-viz.rst
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.047905 pwkit-1.2.0/lmmin_reference/
+-rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/dataf
+-rw-r--r--   0 vsts      (1001) docker     (123)     3340 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/fdjac2.f
+-rw-r--r--   0 vsts      (1001) docker     (123)    15443 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/lmder.f
+-rw-r--r--   0 vsts      (1001) docker     (123)    49879 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/lmder1.all.f
+-rw-r--r--   0 vsts      (1001) docker     (123)    15544 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/lmdif.f
+-rw-r--r--   0 vsts      (1001) docker     (123)    52113 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/lmdif1.all.f
+-rw-r--r--   0 vsts      (1001) docker     (123)     8243 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/lmpar.f
+-rw-r--r--   0 vsts      (1001) docker     (123)   142529 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/mpfit.pro
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    91069 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/mpfit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    96774 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/nmpfit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6178 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/qrsolv.f
+-rw-r--r--   0 vsts      (1001) docker     (123)    28363 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/test.lmder.f
+-rw-r--r--   0 vsts      (1001) docker     (123)    19200 2023-06-18 21:32:42.000000 pwkit-1.2.0/lmmin_reference/test.lmdif.f
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.051905 pwkit-1.2.0/pwkit/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7444 2023-06-18 21:32:44.000000 pwkit-1.2.0/pwkit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    42842 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/astimage.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    52181 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/astutil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16462 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/bblocks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3877 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/cgs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.051905 pwkit-1.2.0/pwkit/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18611 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16406 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/cli/astrotool.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20606 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/cli/imtool.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16865 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/cli/latexdriver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12781 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/cli/multitool.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10356 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/cli/wrapout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19066 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/colormaps.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8123 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/contours.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.031905 pwkit-1.2.0/pwkit/data/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.055905 pwkit-1.2.0/pwkit/data/bandpasses/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_2mass_H.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)     2180 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_2mass_J.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)     1614 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_2mass_Ks.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)      482 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_bessell_B.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)      406 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_bessell_I.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_bessell_R.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)      628 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_bessell_UX.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)      417 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_bessell_V.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)      698 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_galex_fuv.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_galex_nuv.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    11273 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_lbt_lmircam_L.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)      914 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_mearth_ccd715.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    40313 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_J.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    25811 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_Ks.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    33727 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_Lp.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    14615 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_Mp.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    21901 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_h.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    10472 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_wise_1.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    14372 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_wise_2.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    66658 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_wise_3.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    66658 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/filter_wise_4.dat
+-rw-r--r--   0 vsts      (1001) docker     (123)    34560 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/sdss3_filter_responses.fits
+-rw-r--r--   0 vsts      (1001) docker     (123)    23040 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data/bandpasses/swuw1_20041120v106.arf
+-rw-r--r--   0 vsts      (1001) docker     (123)     9882 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/data_gui_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15020 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/dulk_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16299 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/ellipses.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.055905 pwkit-1.2.0/pwkit/environments/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7729 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.059906 pwkit-1.2.0/pwkit/environments/casa/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6579 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    29702 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/closures.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      651 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/cscript_flagcmd.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1031 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/cscript_genantpos.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      926 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/cscript_getopacities.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      985 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/cscript_importalma.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1017 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/cscript_importevla.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      733 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/cscript_plotants.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/cscript_plotcal.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/cscript_setjy.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13778 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/dftdynspec.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14876 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/dftphotom.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11987 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/dftspect.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21374 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/gpdiagnostics.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5838 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/polmodel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8958 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/scripting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4663 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/scripting_driver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    22335 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/spwglue.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   126866 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/tasks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12713 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/casa/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.059906 pwkit-1.2.0/pwkit/environments/ciao/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5380 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/ciao/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6635 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/ciao/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17013 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/ciao/data.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3294 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/heasoft.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.059906 pwkit-1.2.0/pwkit/environments/jupyter/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5719 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/jupyter/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.059906 pwkit-1.2.0/pwkit/environments/sas/
+-rw-r--r--   0 vsts      (1001) docker     (123)    21117 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/sas/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17279 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/environments/sas/data.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    28603 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/fk10.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17564 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/immodel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9906 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/inifile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    37662 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/io.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4127 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/kbn_conf.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16352 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/kwargv.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    22926 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/latex.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    95241 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/lmmin.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35221 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/lsqmdl.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8629 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/method_decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    68401 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/msmt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    31897 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/ndshow_gtk3.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6059 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/ninja_syntax.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    31346 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/numutil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17025 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/parallel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6635 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/pdm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3678 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/phoenix.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7863 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/radio_cal_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25865 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/sherpa.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3033 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/simpleenum.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6446 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/slurp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    34146 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/synphot.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9145 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/tabfile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4188 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/tinifile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11354 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/ucd_physics.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    78640 2023-06-18 21:32:42.000000 pwkit-1.2.0/pwkit/unicode_to_latex.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-18 21:33:36.051905 pwkit-1.2.0/pwkit.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      892 2023-06-18 21:33:36.000000 pwkit-1.2.0/pwkit.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5955 2023-06-18 21:33:36.000000 pwkit-1.2.0/pwkit.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-18 21:33:36.000000 pwkit-1.2.0/pwkit.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      345 2023-06-18 21:33:36.000000 pwkit-1.2.0/pwkit.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-18 21:33:36.000000 pwkit-1.2.0/pwkit.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-06-18 21:33:36.000000 pwkit-1.2.0/pwkit.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-18 21:33:36.000000 pwkit-1.2.0/pwkit.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       84 2023-06-18 21:32:42.000000 pwkit-1.2.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-18 21:33:36.059906 pwkit-1.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3479 2023-06-18 21:32:44.000000 pwkit-1.2.0/setup.py
```

### Comparing `pwkit-1.1.1/CHANGELOG.md` & `pwkit-1.2.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# pwkit 1.2.0 (2023-06-18)
+
+- Remove the dependency on `six`
+- Remove the long-unused `pwkit.ndshow_gtk2` module
+- A further attempt to fix the ReadTheDocs build.
+
+
 # pwkit 1.1.1 (2023-06-18)
 
 No code changes.
 
 - The last release did not publish to PyPI due to a problem with
   the CI automation; attempt to fix that.
 - Also attempt to fix the ReadTheDocs build.
@@ -12,15 +19,15 @@
 A test release, after many years of inactivity, because the previous release
 won't even import noawadays due to the use of very old Numpy features that have
 been removed.
 
 - Switch to Cranko CI and release automation
 - Smattering of modernizations
 - Replace deprecated `np.{int,float,complex,bool}` with corresponding built-in types
-- Remove uses of np.asscalar(), which has been removed in latest Numpys
+- Remove uses of `np.asscalar()`, which has been removed in latest Numpys
 - `pwkit/inifile.py`: untested hacks to get it working on Python 3
 - `pwkit/astutil.py`: fix up `sastrom`
 - `pwkit/colormaps.py`: update to use Gtk 3
 
 
 # Version 1.0.0 (2019 Dec 19)
```

### Comparing `pwkit-1.1.1/LICENSE` & `pwkit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/PKG-INFO` & `pwkit-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwkit
-Version: 1.1.1
+Version: 1.2.0
 Summary: Miscellaneous scientific and astronomical tools
 Home-page: https://github.com/pkgw/pwkit/
 Author: Peter Williams
 Author-email: peter@newton.cx
 License: MIT
 Keywords: astronomy science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pwkit-1.1.1/README.md` & `pwkit-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/Makefile` & `pwkit-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/about.rst` & `pwkit-1.2.0/docs/source/about.rst`

 * *Files 5% similar despite different names*

```diff
@@ -29,24 +29,20 @@
 
 Some ``pwkit`` functionality requires additional Python modules such as
 `scipy`_; these issues should be very obvious as they manifest as
 ``ImportErrors`` triggered for the relevant modules. Bare minimum
 functionality requires:
 
 * `numpy`_ >= 1.6
-* `six`_ >= 1.9
-* on Python 2.x only, `pathlib`_ >= 1.0
 
 If you install ``pwkit`` through standard means, these modules should be
 automatically installed too if they weren’t already available.
 
 .. _scipy: http://www.scipy.org/
 .. _numpy: http://www.numpy.org/
-.. _six: https://pypi.org/project/six/
-.. _pathlib: https://pypi.python.org/pypi/pathlib/
 
 
 Citation
 ========
 
 .. Note: this text is mirrored in the toplevel README.rst
```

### Comparing `pwkit-1.1.1/docs/source/conf.py` & `pwkit-1.2.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "sphinx.ext.autosummary",
     "sphinx.ext.intersphinx",
     "sphinx.ext.imgmath",
     "sphinx.ext.viewcode",
 ]
 
 project = "pwkit"
-release = "1.1.1"  # cranko project-version
+release = "1.2.0"  # cranko project-version
 version = ".".join(release.split(".")[:2])
 
 copyright = "2015-2023, Peter K. G. Williams and collaborators"
 author = "Peter K. G. Williams and collaborators"
 
 templates_path = ["_templates"]
 source_suffix = ".rst"
```

### Comparing `pwkit-1.1.1/docs/source/environments/casa/dftdynspec.rst` & `pwkit-1.2.0/docs/source/environments/casa/dftdynspec.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/environments/casa/dftphotom.rst` & `pwkit-1.2.0/docs/source/environments/casa/dftphotom.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/environments/casa/index.rst` & `pwkit-1.2.0/docs/source/environments/casa/index.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/environments/casa/tasks.rst` & `pwkit-1.2.0/docs/source/environments/casa/tasks.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/environments/casa/utilities.rst` & `pwkit-1.2.0/docs/source/environments/casa/utilities.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/environments/heasoft/index.rst` & `pwkit-1.2.0/docs/source/environments/heasoft/index.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/environments/sas/data.rst` & `pwkit-1.2.0/docs/source/environments/sas/data.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/environments/sas/index.rst` & `pwkit-1.2.0/docs/source/environments/sas/index.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/foundations/core.rst` & `pwkit-1.2.0/docs/source/foundations/core.rst`

 * *Files 3% similar despite different names*

```diff
@@ -80,19 +80,20 @@
 
 
 .. _py3-abstractions:
 
 Abstractions between Python versions 2 and 3
 ------------------------------------------------------------------------
 
-The toplevel :mod:`pwkit` module imports the following variables from the
-:mod:`six` package that helps with Python 2/3 compatibility:
+The toplevel :mod:`pwkit` module defines the following variables as a holdover
+from the times when it was concerned with compatibility between Python 2 and
+Python 3:
 
-- :data:`~six.binary_type`
-- :data:`~six.text_type`
+- :data:`binary_type`
+- :data:`text_type`
 
 .. function:: unicode_to_str(s)
 
    A function for implementing the ``__str__`` method of classes, the meaning
    of which differs between Python versions 2 and 3. In all cases, you should
    implement ``__unicode__`` on your classes. Setting the ``__str__`` property
    of a class to :func:`unicode_to_str` will cause it to Do The Right Thing™,
```

### Comparing `pwkit-1.1.1/docs/source/foundations/io.rst` & `pwkit-1.2.0/docs/source/foundations/io.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/foundations/numerical.rst` & `pwkit-1.2.0/docs/source/foundations/numerical.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/foundations/parallel.rst` & `pwkit-1.2.0/docs/source/foundations/parallel.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/index.rst` & `pwkit-1.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/io/slurp.rst` & `pwkit-1.2.0/docs/source/io/slurp.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/science/basic-astro.rst` & `pwkit-1.2.0/docs/source/science/basic-astro.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/science/dulk-models.rst` & `pwkit-1.2.0/docs/source/science/dulk-models.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/science/fk10-code.rst` & `pwkit-1.2.0/docs/source/science/fk10-code.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/science/index.rst` & `pwkit-1.2.0/docs/source/science/index.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/science/least-squares-modeling.rst` & `pwkit-1.2.0/docs/source/science/least-squares-modeling.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/science/sherpa.rst` & `pwkit-1.2.0/docs/source/science/sherpa.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/docs/source/science/synphot.rst` & `pwkit-1.2.0/docs/source/science/synphot.rst`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/dataf` & `pwkit-1.2.0/lmmin_reference/dataf`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/fdjac2.f` & `pwkit-1.2.0/lmmin_reference/fdjac2.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/lmder.f` & `pwkit-1.2.0/lmmin_reference/lmder.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/lmder1.all.f` & `pwkit-1.2.0/lmmin_reference/lmder1.all.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/lmdif.f` & `pwkit-1.2.0/lmmin_reference/lmdif.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/lmdif1.all.f` & `pwkit-1.2.0/lmmin_reference/lmdif1.all.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/lmpar.f` & `pwkit-1.2.0/lmmin_reference/lmpar.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/mpfit.pro` & `pwkit-1.2.0/lmmin_reference/mpfit.pro`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/mpfit.py` & `pwkit-1.2.0/lmmin_reference/mpfit.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/nmpfit.py` & `pwkit-1.2.0/lmmin_reference/nmpfit.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/qrsolv.f` & `pwkit-1.2.0/lmmin_reference/qrsolv.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/test.lmder.f` & `pwkit-1.2.0/lmmin_reference/test.lmder.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/lmmin_reference/test.lmdif.f` & `pwkit-1.2.0/lmmin_reference/test.lmdif.f`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/__init__.py` & `pwkit-1.2.0/pwkit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,27 +5,21 @@
 """A toolkit for science and astronomy in Python.
 
 """
 from __future__ import absolute_import, division, print_function
 
 __all__ = "Holder PKError binary_type reraise_context text_type unicode_to_str".split()
 
-__version__ = "1.1.1"  # cranko project-version
+__version__ = "1.2.0"  # cranko project-version
 
-# Simultaneous Python 2/3 compatibility through the 'six' module. I started
-# out hoping that I could do this all "in-house" without adding the dep, but
-# it became clear that 'six' was going to end up being helpful.
-
-import six
-from six import binary_type, text_type
-
-if six.PY2:
-    unicode_to_str = lambda s: s.__unicode__().encode("utf8")
-else:
-    unicode_to_str = lambda s: s.__unicode__()
+# Archaic Python 2/3 compatibility support
+
+binary_type = bytes
+text_type = str
+unicode_to_str = lambda s: s.__unicode__()
 
 
 class PKError(Exception):
     """A generic base class for exceptions.
 
     All custom exceptions raised by :mod:`pwkit` modules should be subclasses
     of this class.
@@ -40,17 +34,17 @@
     If only a single argument is given, the exception text is its
     stringification without applying ``printf``-style formatting.
 
     """
 
     def __init__(self, fmt, *args):
         if not len(args):
-            self.args = (text_type(fmt),)
+            self.args = (str(fmt),)
         else:
-            self.args = (text_type(fmt) % args,)
+            self.args = (str(fmt) % args,)
 
     def __unicode__(self):
         return self.args[0]
 
     __str__ = unicode_to_str
 
     def __repr__(self):
@@ -96,15 +90,15 @@
 
     """
     import sys
 
     if len(args):
         cstr = fmt % args
     else:
-        cstr = text_type(fmt)
+        cstr = str(fmt)
 
     ex = sys.exc_info()[1]
 
     if isinstance(ex, EnvironmentError):
         ex.strerror = "%s: %s" % (cstr, ex.strerror)
         ex.args = (ex.errno, ex.strerror)
     else:
@@ -122,54 +116,50 @@
 
     The *__decorating* keyword is used to implement the :class:`Holder`
     decorator functionality, described below.
 
     """
 
     def __init__(self, __decorating=None, **kwargs):
-        import types
-
         if __decorating is None:
             values = kwargs
-        elif isinstance(__decorating, six.class_types):
+        elif isinstance(__decorating, type):
             # We're decorating a class definition. Transform the definition
             # into a Holder instance thusly:
             values = dict(
-                kv
-                for kv in six.iteritems(__decorating.__dict__)
-                if not kv[0].startswith("__")
+                kv for kv in __decorating.__dict__.items() if not kv[0].startswith("__")
             )
         else:
             # You could imagine allowing @Holder on a function and doing
             # something with its return value, but I can't think of a use that
             # would be more sensible than just creating and returning a Holder
             # directly.
             raise ValueError(
                 "unexpected use of Holder as a decorator (on %r)" % __decorating
             )
 
         self.set(**values)
 
     def __unicode__(self):
         d = self.__dict__
-        s = sorted(six.iterkeys(d))
+        s = sorted(d.keys())
         return "{" + ", ".join("%s=%s" % (k, d[k]) for k in s) + "}"
 
     __str__ = unicode_to_str
 
     def __repr__(self):
         d = self.__dict__
-        s = sorted(six.iterkeys(d))
+        s = sorted(d.keys())
         return "%s(%s)" % (
             self.__class__.__name__,
             ", ".join("%s=%r" % (k, d[k]) for k in s),
         )
 
     def __iter__(self):
-        return six.iteritems(self.__dict__)
+        return self.__dict__.items()
 
     def __contains__(self, key):
         return key in self.__dict__
 
     def set(self, **kwargs):
         """For each keyword argument, sets an attribute on this :class:`Holder` to its
         value.
@@ -239,11 +229,11 @@
             template = "%-*s = %r"
         else:
             raise ValueError('unrecognized value for "format": %r' % format)
 
         d = self.__dict__
         maxlen = 0
 
-        for k in six.iterkeys(d):
+        for k in d.keys():
             maxlen = max(maxlen, len(k))
 
-        return "\n".join(template % (maxlen, k, d[k]) for k in sorted(six.iterkeys(d)))
+        return "\n".join(template % (maxlen, k, d[k]) for k in sorted(d.keys()))
```

### Comparing `pwkit-1.1.1/pwkit/astimage.py` & `pwkit-1.2.0/pwkit/astimage.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 AstroImage
 MIRIADImage
 PyrapImage
 FITSImage
 SimpleImage
 open""".split()
 
-import six
-from six.moves import range
 import numpy as np
 from numpy import pi
 
 from . import PKError
 from .astutil import D2R, R2D
 
 
@@ -653,30 +651,30 @@
         from pyrap.quanta import quantity
 
         self._wcscale = wcscale = np.ones(self.shape.size)
         c = self._handle.coordinates()
         radian = quantity(1.0, "rad")
 
         for item in c.get_axes():
-            if isinstance(item, six.string_types):
+            if isinstance(item, str):
                 self.axdescs.append(item.replace(" ", "_"))
             else:
                 for subitem in item:
                     self.axdescs.append(subitem.replace(" ", "_"))
 
         def getconversion(text):
             q = quantity(1.0, text)
             if q.conforms(radian):
                 return q.get_value("rad")
             return 1
 
         i = 0
 
         for item in c.get_unit():
-            if isinstance(item, six.string_types):
+            if isinstance(item, str):
                 wcscale[i] = getconversion(item)
                 i += 1
             elif len(item) == 0:
                 wcscale[i] = 1  # null unit
                 i += 1
             else:
                 for subitem in item:
```

### Comparing `pwkit-1.1.1/pwkit/astutil.py` & `pwkit-1.2.0/pwkit/astutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 __all__ = str(
     """np pi twopi halfpi R2A A2R R2D D2R R2H H2R F2S S2F J2000 angcen orientcen
                   fmthours fmtdeglon fmtdeglat fmtradec parsehours parsedeglat
                   parsedeglon sphdist sphbear sphofs parang gaussian_convolve
                   gaussian_deconvolve load_skyfield_data AstrometryInfo app2abs abs2app"""
 ).split()
 
-import six
-from six.moves import range
 import numpy as np
 
-from . import text_type, unicode_to_str, PKError
+from . import unicode_to_str, PKError
 from .numutil import broadcastize
 
 
 # Workaround for Sphinx bug 1641. Without this, the "autoattribute" directive
 # does not work if the print_function future is used. Copied from
 # https://github.com/sphinx-doc/sphinx/issues/1641#issuecomment-204323049.
 # See commit message associated with this code for more detail.
@@ -87,15 +85,15 @@
 
     precision = max(int(precision), 0)
     if precision == 0:
         width = 2
     else:
         width = precision + 3
 
-    basewidth = len(text_type(basemax))
+    basewidth = len(str(basemax))
 
     bs = int(np.floor(base))
     min = int(np.floor((base - bs) * 60))
     sec = round(3600 * (base - bs - min / 60.0), precision)
 
     if sec >= 60:
         # Can happen if we round up
@@ -305,15 +303,15 @@
       and arcseconds components of the Dec/lat coordinate.
     intersep (default " ")
       The string separating the RA/lon and Dec/lat coordinates
 
     """
     return (
         fmthours(rarad, precision=precision + 1, seps=raseps)
-        + text_type(intersep)
+        + str(intersep)
         + fmtdeglat(decrad, precision=precision, seps=decseps)
     )
 
 
 # Parsing routines are currently very lame.
 
 
@@ -1044,15 +1042,15 @@
 
     """
 
     def __init__(self, simbadident=None, **kwargs):
         if simbadident is not None:
             self.fill_from_simbad(simbadident)
 
-        for k, v in six.iteritems(kwargs):
+        for k, v in kwargs.items():
             setattr(self, k, v)
 
     def _partial_info(self, val0, *rest):
         if not len(rest):
             return False
 
         first = val0 is None
@@ -1343,15 +1341,15 @@
 
         Returns *self*.
 
         """
         info = get_simbad_astrometry_info(ident, debug=debug)
         posref = "unknown"
 
-        for k, v in six.iteritems(info):
+        for k, v in info.items():
             if "~" in v:
                 continue  # no info
 
             if k == "COO(d;A)":
                 self.ra = float(v) * D2R
             elif k == "COO(d;D)":
                 self.dec = float(v) * D2R
```

### Comparing `pwkit-1.1.1/pwkit/bblocks.py` & `pwkit-1.2.0/pwkit/bblocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 __all__ = str("nlogn bin_bblock tt_bblock bs_tt_bblock").split()
 
 
-from six.moves import range
 import numpy as np
 
 from . import Holder
 
 
 def nlogn(n, dt):
     # I really feel like there must be a cleverer way to do this
```

### Comparing `pwkit-1.1.1/pwkit/cgs.py` & `pwkit-1.2.0/pwkit/cgs.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/cli/__init__.py` & `pwkit-1.2.0/pwkit/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,58 +24,53 @@
 Submodules:
 
 multitool - Framework for command-line programs with sub-commands.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''check_usage die fork_detached_process pop_option print_tracebacks
+__all__ = str(
+    """check_usage die fork_detached_process pop_option print_tracebacks
                   propagate_sigint show_usage unicode_stdio warn
-                  wrong_usage''').split ()
+                  wrong_usage"""
+).split()
 
-import codecs, os, signal, six, sys, traceback
-from .. import text_type
+import os, signal, sys
 
 
-def unicode_stdio ():
+def unicode_stdio():
     """Make sure that the standard I/O streams accept Unicode.
 
-    In Python 2, the standard I/O streams accept bytes, not Unicode
-    characters. This means that in principle every Unicode string that we want
-    to output should be encoded to utf-8 before print()ing. But Python 2.X has
-    a hack where, if the output is a terminal, it will automatically encode
-    your strings, using UTF-8 in most cases.
+    This function does nothing, because we have dropped support for Python 2. In
+    Python 3 it is not necessary.
+
+    In Python 2, the standard I/O streams accept bytes, not Unicode characters.
+    This means that in principle every Unicode string that we want to output
+    should be encoded to utf-8 before print()ing. But Python 2.X has a hack
+    where, if the output is a terminal, it will automatically encode your
+    strings, using UTF-8 in most cases.
 
     BUT this hack doesn't kick in if you pipe your program's output to another
     program. So it's easy to write a tool that works fine in most cases but then
     blows up when you log its output to a file.
 
     The proper solution is just to do the encoding right. This function sets
-    things up to do this in the most sensible way I can devise, if we're
-    running on Python 2. This approach sets up compatibility with Python 3,
-    which has the stdio streams be in text mode rather than bytes mode to
-    begin with.
+    things up to do this in the most sensible way I can devise, if we're running
+    on Python 2. This approach sets up compatibility with Python 3, which has
+    the stdio streams be in text mode rather than bytes mode to begin with.
 
     Basically, every command-line Python program should call this right at
     startup. I'm tempted to just invoke this code whenever this module is
     imported since I foresee many accidentally omissions of the call.
 
     """
-    if six.PY3:
-        return
-
-    enc = sys.stdin.encoding or 'utf-8'
-    sys.stdin = codecs.getreader (enc) (sys.stdin)
-    enc = sys.stdout.encoding or enc
-    sys.stdout = codecs.getwriter (enc) (sys.stdout)
-    enc = sys.stderr.encoding or enc
-    sys.stderr = codecs.getwriter (enc) (sys.stderr)
+    return
 
 
-class _InterruptSignalPropagator (object):
+class _InterruptSignalPropagator(object):
     """Ensure that calling shells know when we die from SIGINT.
 
     Imagine that a shell script is running a long-running subprogram and the
     user hits control-C to interrupt the program. What happens is that both
     the shell and the subprogram are sent SIGINT, which usually causes the
     subprogram to die immediately. However, the shell's behavior is more
     complicated. Certain subprograms might handle the SIGINT and *not* die
@@ -102,83 +97,92 @@
     honest-to-God uncaught SIGINT.
 
     This is all accomplished by placing in a shim sys.excepthook() handler for
     KeyboardInterrupt exceptions. The previous excepthook can be accessed as
     `pwkit.cli.propagate_sigint.inner_excepthook`.
 
     """
+
     inner_excepthook = None
 
-    def __call__ (self):
+    def __call__(self):
         """Set sys.excepthook to our special version.
 
         It chains to the previous excepthook, of course. This value can be
         accessed as `pwkit.cli.propagate_sigint.inner_excepthook`.
 
         """
         if self.inner_excepthook is None:
             self.inner_excepthook = sys.excepthook
             sys.excepthook = self.excepthook
 
-    def excepthook (self, etype, evalue, etb):
+    def excepthook(self, etype, evalue, etb):
         """Handle an uncaught exception. We always forward the exception on to
         whatever `sys.excepthook` was present upon setup. However, if the
         exception is a KeyboardInterrupt, we additionally kill ourselves with
         an uncaught SIGINT, so that invoking programs know what happened.
 
         """
-        self.inner_excepthook (etype, evalue, etb)
+        self.inner_excepthook(etype, evalue, etb)
 
-        if issubclass (etype, KeyboardInterrupt):
+        if issubclass(etype, KeyboardInterrupt):
             # Don't try this at home, kids. On some systems os.kill (0, ...)
             # signals our entire progress group, which is not what we want,
             # so we use os.getpid ().
-            signal.signal (signal.SIGINT, signal.SIG_DFL)
-            os.kill (os.getpid (), signal.SIGINT)
+            signal.signal(signal.SIGINT, signal.SIG_DFL)
+            os.kill(os.getpid(), signal.SIGINT)
 
-propagate_sigint = _InterruptSignalPropagator ()
 
+propagate_sigint = _InterruptSignalPropagator()
 
-def _print_backtrace_signal_handler (signum, frame):
+
+def _print_backtrace_signal_handler(signum, frame):
     try:
         import traceback
-        print ('*** Printing traceback due to receipt of signal #%d' % signum,
-               file=sys.stderr)
-        for fn, line, func, text in traceback.extract_stack (frame):
-            print ('***   %s (%s:%d): %s' % (fn, func, line, text or '??'),
-                   file=sys.stderr)
-        print ('*** End of traceback (innermost call is last)',
-               file=sys.stderr)
+
+        print(
+            "*** Printing traceback due to receipt of signal #%d" % signum,
+            file=sys.stderr,
+        )
+        for fn, line, func, text in traceback.extract_stack(frame):
+            print(
+                "***   %s (%s:%d): %s" % (fn, func, line, text or "??"), file=sys.stderr
+            )
+        print("*** End of traceback (innermost call is last)", file=sys.stderr)
         assert False
     except Exception as e:
-        print ('*** Failed to print traceback on receipt of signal #%d: %s (%s)'
-               % (signum, e, e.__class__.__name__), file=sys.stderr)
+        print(
+            "*** Failed to print traceback on receipt of signal #%d: %s (%s)"
+            % (signum, e, e.__class__.__name__),
+            file=sys.stderr,
+        )
 
 
-def backtrace_on_usr1 ():
+def backtrace_on_usr1():
     """Install a signal handler such that this program prints a Python traceback
     upon receipt of SIGUSR1. This could be useful for checking that
     long-running programs are behaving properly, or for discovering where an
     infinite loop is occurring.
 
     Note, however, that the Python interpreter does not invoke Python signal
     handlers exactly when the process is signaled. For instance, a signal
     delivered in the midst of a time.sleep() call will only be seen by Python
     code after that call completes. This means that this feature may not be as
     helpful as one might like for debugging certain kinds of problems.
 
     """
     import signal
+
     try:
-        signal.signal (signal.SIGUSR1, _print_backtrace_signal_handler)
+        signal.signal(signal.SIGUSR1, _print_backtrace_signal_handler)
     except Exception as e:
-        warn ('failed to set up Python backtraces on SIGUSR1: %s', e)
+        warn("failed to set up Python backtraces on SIGUSR1: %s", e)
 
 
-def die (fmt, *args):
+def die(fmt, *args):
     """Raise a :exc:`SystemExit` exception with a formatted error message.
 
     :arg str fmt: a format string
     :arg args: arguments to the format string
 
     If *args* is empty, a :exc:`SystemExit` exception is raised with the
     argument ``'error: ' + str (fmt)``. Otherwise, the string component is
@@ -187,29 +191,29 @@
 
     Example::
 
        if ndim != 3:
           die ('require exactly 3 dimensions, not %d', ndim)
 
     """
-    if not len (args):
-        raise SystemExit ('error: ' + text_type (fmt))
-    raise SystemExit ('error: ' + (fmt % args))
+    if not len(args):
+        raise SystemExit("error: " + str(fmt))
+    raise SystemExit("error: " + (fmt % args))
 
 
-def warn (fmt, *args):
-    if not len (args):
-        s = text_type (fmt)
+def warn(fmt, *args):
+    if not len(args):
+        s = str(fmt)
     else:
         s = fmt % args
 
-    print ('warning:', s, file=sys.stderr)
+    print("warning:", s, file=sys.stderr)
 
 
-class print_tracebacks (object):
+class print_tracebacks(object):
     """Context manager that catches exceptions and prints their tracebacks without
     reraising them. Intended for robust programs that want to continue
     execution even if something bad happens; this provides the infrastructure
     to swallow exceptions while still preserving exception information for
     later debugging.
 
     You can specify which exception classes to catch with the `types` keyword
@@ -220,49 +224,51 @@
 
     Instances preserve the exception information in the fields 'etype',
     'evalue', and 'etb' if your program in fact wants to do something with the
     information. One basic use would be checking whether an exception did, in
     fact, occur.
 
     """
-    header = 'Swallowed exception:'
 
-    def __init__ (self, types=(Exception,), header=None, file=None):
+    header = "Swallowed exception:"
+
+    def __init__(self, types=(Exception,), header=None, file=None):
         self.types = types
         self.file = file
 
         if header is not None:
             self.header = header
 
-    def __enter__ (self):
+    def __enter__(self):
         self.etype = self.evalue = self.etb = None
         return self
 
-    def __exit__ (self, etype, evalue, etb):
+    def __exit__(self, etype, evalue, etb):
         if etype is None:
-            return False # all good, woohoo
+            return False  # all good, woohoo
 
-        if not isinstance (evalue, self.types):
+        if not isinstance(evalue, self.types):
             # Exception happened but not something of the kind we expect. Reraise.
             return False
 
         # Exception happened and we should do our thing.
         self.etype = etype
         self.evalue = evalue
         self.etb = etb
 
         if self.header is not None:
-            print (self.header, file=self.file or sys.stderr)
+            print(self.header, file=self.file or sys.stderr)
 
         from traceback import print_exception
-        print_exception (etype, evalue, etb, file=self.file)
-        return True # swallow this exception
+
+        print_exception(etype, evalue, etb, file=self.file)
+        return True  # swallow this exception
 
 
-def fork_detached_process ():
+def fork_detached_process():
     """Fork this process, creating a subprocess detached from the current context.
 
     Returns a :class:`pwkit.Holder` instance with information about what
     happened. Its fields are:
 
     whoami
       A string, either "original" or "forked" depending on which process we are.
@@ -305,78 +311,80 @@
     `PEP 3143`_.
 
     .. _PEP 3143: https://www.python.org/dev/peps/pep-3143/
 
     """
     import os, struct
     from .. import Holder
-    payload = struct.Struct ('L')
 
-    info = Holder ()
-    readfd, writefd = os.pipe ()
+    payload = struct.Struct("L")
 
-    pid1 = os.fork ()
+    info = Holder()
+    readfd, writefd = os.pipe()
+
+    pid1 = os.fork()
     if pid1 > 0:
-        info.whoami = 'original'
-        info.pipe = os.fdopen (readfd, 'rb')
-        os.close (writefd)
+        info.whoami = "original"
+        info.pipe = os.fdopen(readfd, "rb")
+        os.close(writefd)
 
-        retcode = os.waitpid (pid1, 0)[1]
+        retcode = os.waitpid(pid1, 0)[1]
         if retcode:
-            raise Exception ('child process exited with error code %d' % retcode)
+            raise Exception("child process exited with error code %d" % retcode)
 
-        (info.forkedpid,) = payload.unpack (info.pipe.read (payload.size))
+        (info.forkedpid,) = payload.unpack(info.pipe.read(payload.size))
     else:
         # We're the intermediate child process. Start new session and process
         # groups, detaching us from TTY signals and whatnot.
-        os.setsid ()
+        os.setsid()
 
-        pid2 = os.fork ()
+        pid2 = os.fork()
         if pid2 > 0:
             # We're the intermediate process; we're all done
-            os._exit (0)
+            os._exit(0)
 
         # If we get here, we're the detached child process.
-        info.whoami = 'forked'
-        info.pipe = os.fdopen (writefd, 'wb')
-        os.close (readfd)
-        info.forkedpid = os.getpid ()
-        info.pipe.write (payload.pack (info.forkedpid))
+        info.whoami = "forked"
+        info.pipe = os.fdopen(writefd, "wb")
+        os.close(readfd)
+        info.forkedpid = os.getpid()
+        info.pipe.write(payload.pack(info.forkedpid))
 
     return info
 
 
 # Simple-minded argument handling -- see also kwargv.
 
-def pop_option (ident, argv=None):
+
+def pop_option(ident, argv=None):
     """A lame routine for grabbing command-line arguments. Returns a boolean
     indicating whether the option was present. If it was, it's removed from
     the argument string. Because of the lame behavior, options can't be
     combined, and non-boolean options aren't supported. Operates on sys.argv
     by default.
 
     Note that this will proceed merrily if argv[0] matches your option.
 
     """
     if argv is None:
         from sys import argv
 
-    if len (ident) == 1:
-        ident = '-' + ident
+    if len(ident) == 1:
+        ident = "-" + ident
     else:
-        ident = '--' + ident
+        ident = "--" + ident
 
     found = ident in argv
     if found:
-        argv.remove (ident)
+        argv.remove(ident)
 
     return found
 
 
-def show_usage (docstring, short, stream, exitcode):
+def show_usage(docstring, short, stream, exitcode):
     """Print program usage information and exit.
 
     :arg str docstring: the program help text
 
     This function just prints *docstring* and exits. In most cases, the
     function :func:`check_usage` should be used: it automatically checks
     :data:`sys.argv` for a sole "-h" or "--help" argument and invokes this
@@ -388,33 +396,35 @@
     message and exits with an error code.
 
     """
     if stream is None:
         from sys import stdout as stream
 
     if not short:
-        print ('Usage:', docstring.strip (), file=stream)
+        print("Usage:", docstring.strip(), file=stream)
     else:
         intext = False
-        for l in docstring.splitlines ():
+        for l in docstring.splitlines():
             if intext:
-                if not len (l):
+                if not len(l):
                     break
-                print (l, file=stream)
-            elif len (l):
+                print(l, file=stream)
+            elif len(l):
                 intext = True
-                print ('Usage:', l, file=stream)
+                print("Usage:", l, file=stream)
 
-        print ('\nRun with a sole argument --help for more detailed '
-               'usage information.', file=stream)
+        print(
+            "\nRun with a sole argument --help for more detailed " "usage information.",
+            file=stream,
+        )
 
-    raise SystemExit (exitcode)
+    raise SystemExit(exitcode)
 
 
-def check_usage (docstring, argv=None, usageifnoargs=False):
+def check_usage(docstring, argv=None, usageifnoargs=False):
     """Check if the program has been run with a --help argument; if so,
     print usage information and exit.
 
     :arg str docstring: the program help text
     :arg argv: the program arguments; taken as :data:`sys.argv` if
         given as :const:`None` (the default). (Note that this implies
         ``argv[0]`` should be the program name and not the first option.)
@@ -437,21 +447,21 @@
 
     See also :func:`wrong_usage`.
 
     """
     if argv is None:
         from sys import argv
 
-    if len (argv) == 1 and usageifnoargs:
-        show_usage (docstring, (usageifnoargs != 'long'), None, 0)
-    if len (argv) == 2 and argv[1] in ('-h', '--help'):
-        show_usage (docstring, False, None, 0)
+    if len(argv) == 1 and usageifnoargs:
+        show_usage(docstring, (usageifnoargs != "long"), None, 0)
+    if len(argv) == 2 and argv[1] in ("-h", "--help"):
+        show_usage(docstring, False, None, 0)
 
 
-def wrong_usage (docstring, *rest):
+def wrong_usage(docstring, *rest):
     """Print a message indicating invalid command-line arguments and exit with an
     error code.
 
     :arg str docstring: the program help text
     :arg rest: an optional specific error message
 
     This function is intended for small programs launched from the command
@@ -485,16 +495,16 @@
     percent-formatted with the remaining values. See the above example.
 
     See also :func:`check_usage` and :func:`show_usage`.
 
     """
     intext = False
 
-    if len (rest) == 0:
-        detail = 'invalid command-line arguments'
-    elif len (rest) == 1:
+    if len(rest) == 0:
+        detail = "invalid command-line arguments"
+    elif len(rest) == 1:
         detail = rest[0]
     else:
-        detail = rest[0] % tuple (rest[1:])
+        detail = rest[0] % tuple(rest[1:])
 
-    print ('error:', detail, '\n', file=sys.stderr) # extra NL
-    show_usage (docstring, True, sys.stderr, 1)
+    print("error:", detail, "\n", file=sys.stderr)  # extra NL
+    show_usage(docstring, True, sys.stderr, 1)
```

### Comparing `pwkit-1.1.1/pwkit/cli/astrotool.py` & `pwkit-1.2.0/pwkit/cli/astrotool.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,521 +2,567 @@
 # Copyright 2014 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 """pwkit.cli.astrotool - the 'astrotool' program."""
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('commandline').split ()
+__all__ = str("commandline").split()
 
-import math, numpy as np, os, sys
-from six.moves import range
+import math, numpy as np
 
-from .. import PKError
 from ..astutil import *
 from ..cgs import *
 from . import multitool
 from . import *
 
 
-def fparse (text):
+def fparse(text):
     try:
         # note: totally reckless about globals/locals passed, etc.
         # nice to have * from astutil and cgs available.
-        v = eval (text)
+        v = eval(text)
     except Exception as e:
-        die ('cannot evaluate "%s": %s (%s)', text, str (e), e.__class__.__name__)
+        die('cannot evaluate "%s": %s (%s)', text, str(e), e.__class__.__name__)
 
     try:
-        f = float (v)
+        f = float(v)
     except Exception as e:
-        die ('evaluted "%s", but could not floatify result %r: %s (%s)', text, v,
-             str (e), e.__class__.__name__)
+        die(
+            'evaluted "%s", but could not floatify result %r: %s (%s)',
+            text,
+            v,
+            str(e),
+            e.__class__.__name__,
+        )
 
     return f
 
 
-def fmt (v):
-    f1 = '%.4g' % v
-    f2 = '%.3e' % v
+def fmt(v):
+    f1 = "%.4g" % v
+    f2 = "%.3e" % v
 
     if f1 == f2:
         reprs = [f1]
     else:
         reprs = [f1, f2]
 
     if v > 0:
-        reprs.append ('10**(%.2f)' % log10 (v))
+        reprs.append("10**(%.2f)" % log10(v))
 
-    return ' = '.join (reprs)
+    return " = ".join(reprs)
 
 
 # The commands.
 
-class Abs2app (multitool.Command):
-    name = 'abs2app'
-    argspec = '<absmag [mag]> <dist [pc]>'
-    summary = 'Convert absolute to apparent magnitude.'
-
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('abs2app expected exactly 2 arguments')
-
-        absmag = fparse (args[0])
-        dist = fparse (args[1])
-        print (fmt (abs2app (absmag, dist)))
-
-
-class App2abs (multitool.Command):
-    name = 'app2abs'
-    argspec = '<appmag [mag]> <dist [pc]>'
-    summary = 'Convert apparent to absolute magnitude.'
-
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('app2abs expected exactly 2 arguments')
-
-        appmag = fparse (args[0])
-        dist = fparse (args[1])
-        print (fmt (app2abs (appmag, dist)))
-
-
-class C2m (multitool.Command):
-    name = 'c2m'
-    argspec = '<year> <month> <frac.day> [hour] [min] [sec]'
-    summary = 'Convert a UTC calendar date to MJD[TAI].'
-    more_help = '''Note that fractional UTC days are not well-specified because of
-the possibility of leap seconds.'''
 
-    def invoke (self, args, **kwargs):
+class Abs2app(multitool.Command):
+    name = "abs2app"
+    argspec = "<absmag [mag]> <dist [pc]>"
+    summary = "Convert absolute to apparent magnitude."
+
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError("abs2app expected exactly 2 arguments")
+
+        absmag = fparse(args[0])
+        dist = fparse(args[1])
+        print(fmt(abs2app(absmag, dist)))
+
+
+class App2abs(multitool.Command):
+    name = "app2abs"
+    argspec = "<appmag [mag]> <dist [pc]>"
+    summary = "Convert apparent to absolute magnitude."
+
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError("app2abs expected exactly 2 arguments")
+
+        appmag = fparse(args[0])
+        dist = fparse(args[1])
+        print(fmt(app2abs(appmag, dist)))
+
+
+class C2m(multitool.Command):
+    name = "c2m"
+    argspec = "<year> <month> <frac.day> [hour] [min] [sec]"
+    summary = "Convert a UTC calendar date to MJD[TAI]."
+    more_help = """Note that fractional UTC days are not well-specified because of
+the possibility of leap seconds."""
+
+    def invoke(self, args, **kwargs):
         """c2m  - UTC calendar to MJD[TAI]"""
 
-        if len (args) not in (3, 6):
-            raise multitool.UsageError ('c2m expected exactly 3 or 6 arguments')
+        if len(args) not in (3, 6):
+            raise multitool.UsageError("c2m expected exactly 3 or 6 arguments")
 
-        year = int (args[0])
-        month = int (args[1])
+        year = int(args[0])
+        month = int(args[1])
 
         import astropy.time
 
-        if len (args) == 3:
-            day = float (args[2])
-            iday = int (math.floor (day))
+        if len(args) == 3:
+            day = float(args[2])
+            iday = int(math.floor(day))
             r = 24 * (day - iday)
-            hour = int (np.floor (r))
+            hour = int(np.floor(r))
             r = 60 * (r - hour)
-            minute = int (np.floor (r))
+            minute = int(np.floor(r))
             second = 60 * (r - minute)
         else:
-            iday = int (args[2])
-            hour = int (args[3])
-            minute = int (args[4])
-            second = float (args[5])
+            iday = int(args[2])
+            hour = int(args[3])
+            minute = int(args[4])
+            second = float(args[5])
 
-        s = '%d-%02d-%02d %02d:%02d:%02.8f' % (year, month, iday,
-                                               hour, minute, second)
-        t = astropy.time.Time (s, format='iso', scale='utc')
-        print ('%.4f' % t.tai.mjd)
+        s = "%d-%02d-%02d %02d:%02d:%02.8f" % (year, month, iday, hour, minute, second)
+        t = astropy.time.Time(s, format="iso", scale="utc")
+        print("%.4f" % t.tai.mjd)
 
 
-class Calc (multitool.Command):
-    name = 'calc'
-    argspec = '{expr...}'
-    summary = 'Evaluate and print an expression.'
+class Calc(multitool.Command):
+    name = "calc"
+    argspec = "{expr...}"
+    summary = "Evaluate and print an expression."
 
-    def invoke (self, args, **kwargs):
-        if not len (args):
-            raise multitool.UsageError ('calc expected arguments')
+    def invoke(self, args, **kwargs):
+        if not len(args):
+            raise multitool.UsageError("calc expected arguments")
 
-        print (fmt (fparse (' '.join (args))))
+        print(fmt(fparse(" ".join(args))))
 
 
-class Csep (multitool.Command):
-    name = 'csep'
-    argspec = '<RA 1> <dec 1> <RA 2> <dec 2>'
-    summary = 'Print separation between two positions; args in sexagesimal.'
+class Csep(multitool.Command):
+    name = "csep"
+    argspec = "<RA 1> <dec 1> <RA 2> <dec 2>"
+    summary = "Print separation between two positions; args in sexagesimal."
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 4:
-            raise multitool.UsageError ('csep expected 4 arguments')
+    def invoke(self, args, **kwargs):
+        if len(args) != 4:
+            raise multitool.UsageError("csep expected 4 arguments")
 
         try:
-            lat1 = parsedeglat (args[1])
-            lon1 = parsehours (args[0])
-            lat2 = parsedeglat (args[3])
-            lon2 = parsehours (args[2])
+            lat1 = parsedeglat(args[1])
+            lon1 = parsehours(args[0])
+            lat2 = parsedeglat(args[3])
+            lon2 = parsehours(args[2])
         except Exception as e:
-            die (e)
+            die(e)
 
-        print ('degree:', fmt (sphdist (lat1, lon1, lat2, lon2) * R2D))
-        print ('arcsec:', fmt (sphdist (lat1, lon1, lat2, lon2) * R2A))
+        print("degree:", fmt(sphdist(lat1, lon1, lat2, lon2) * R2D))
+        print("arcsec:", fmt(sphdist(lat1, lon1, lat2, lon2) * R2A))
 
 
-class D2sh (multitool.Command):
-    name = 'd2sh'
-    argspec = '{expr}'
-    summary = 'Convert decimal degrees to sexagesimal hours (RA).'
+class D2sh(multitool.Command):
+    name = "d2sh"
+    argspec = "{expr}"
+    summary = "Convert decimal degrees to sexagesimal hours (RA)."
 
-    def invoke (self, args, **kwargs):
-        if not len (args):
-            raise multitool.UsageError ('d2sh expected arguments')
+    def invoke(self, args, **kwargs):
+        if not len(args):
+            raise multitool.UsageError("d2sh expected arguments")
 
-        deglon = fparse (' '.join (args))
-        print (fmthours (deglon * D2R))
+        deglon = fparse(" ".join(args))
+        print(fmthours(deglon * D2R))
 
 
-class D2sl (multitool.Command):
-    name = 'd2sl'
-    argspec = '{expr}'
-    summary = 'Convert decimal degrees to a sexagesimal latitude (declination).'
+class D2sl(multitool.Command):
+    name = "d2sl"
+    argspec = "{expr}"
+    summary = "Convert decimal degrees to a sexagesimal latitude (declination)."
 
-    def invoke (self, args, **kwargs):
-        if not len (args):
-            raise multitool.UsageError ('d2sl expected arguments')
+    def invoke(self, args, **kwargs):
+        if not len(args):
+            raise multitool.UsageError("d2sl expected arguments")
 
-        deglat = fparse (' '.join (args))
-        print (fmtdeglat (deglat * D2R))
+        deglat = fparse(" ".join(args))
+        print(fmtdeglat(deglat * D2R))
 
 
-class Ephem (multitool.Command):
-    name = 'ephem'
-    argspec = '<name> <mjd>'
-    summary = 'Compute position of ephemeris object at a given time.'
+class Ephem(multitool.Command):
+    name = "ephem"
+    argspec = "<name> <mjd>"
+    summary = "Compute position of ephemeris object at a given time."
 
-    def invoke (self, args, **kwargs):
+    def invoke(self, args, **kwargs):
         # This is obviously not going to be super high accuracy.
 
-        if len (args) != 2:
-            raise multitool.UsageError ('ephem expected exactly 2 arguments')
+        if len(args) != 2:
+            raise multitool.UsageError("ephem expected exactly 2 arguments")
 
         try:
             import skyfield
         except ImportError:
-            die ('need the "skyfield" module')
+            die('need the "skyfield" module')
 
         # TODO: might want to make it possible to use a different ephemeris
         # file, if the hardcoded standard doesn't contain the ones we want.
 
         from ..astutil import load_skyfield_data
+
         planets, ts = load_skyfield_data()
 
         try:
-            earth = planets['earth']
+            earth = planets["earth"]
             obj = planets[args[0]]
         except Exception as e:
-            die (e)
+            die(e)
 
-        mjd = fparse (args[1])
-        t = ts.tdb(jd = mjd + 2400000.5)
+        mjd = fparse(args[1])
+        t = ts.tdb(jd=mjd + 2400000.5)
 
         ra, dec, _ = earth.at(t).observe(obj).radec()
 
-        print(fmtradec (ra.radians, dec.radians))
+        print(fmtradec(ra.radians, dec.radians))
 
 
-class Flux2lum (multitool.Command):
-    name = 'flux2lum'
-    argspec = '<flux [cgs]> <dist [pc]>'
-    summary = 'Compute luminosity from flux and distance.'
+class Flux2lum(multitool.Command):
+    name = "flux2lum"
+    argspec = "<flux [cgs]> <dist [pc]>"
+    summary = "Compute luminosity from flux and distance."
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('flux2lum expected exactly 2 arguments')
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError("flux2lum expected exactly 2 arguments")
 
-        flux = fparse (args[0])
-        dist = fparse (args[1])
-        lum = flux * 4 * pi * (dist * cmperpc)**2
-        print (fmt (lum))
+        flux = fparse(args[0])
+        dist = fparse(args[1])
+        lum = flux * 4 * pi * (dist * cmperpc) ** 2
+        print(fmt(lum))
 
 
-class Lum2flux (multitool.Command):
-    name = 'lum2flux'
-    argspec = '<lum [cgs]> <dist [pc]>'
-    summary = 'Compute flux from luminosity and distance.'
+class Lum2flux(multitool.Command):
+    name = "lum2flux"
+    argspec = "<lum [cgs]> <dist [pc]>"
+    summary = "Compute flux from luminosity and distance."
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('lum2flux expected exactly 2 arguments')
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError("lum2flux expected exactly 2 arguments")
 
-        lum = fparse (args[0])
-        dist = fparse (args[1])
-        flux = lum / (4 * pi * (dist * cmperpc)**2)
-        print (fmt (flux))
+        lum = fparse(args[0])
+        dist = fparse(args[1])
+        flux = lum / (4 * pi * (dist * cmperpc) ** 2)
+        print(fmt(flux))
 
 
-class M2c (multitool.Command):
-    name = 'm2c'
-    argspec = '<MJD>'
-    summary = 'Convert MJD[TAI] to a UTC calendar date.'
+class M2c(multitool.Command):
+    name = "m2c"
+    argspec = "<MJD>"
+    summary = "Convert MJD[TAI] to a UTC calendar date."
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 1:
-            raise multitool.UsageError ('m2c expected exactly 1 argument')
+    def invoke(self, args, **kwargs):
+        if len(args) != 1:
+            raise multitool.UsageError("m2c expected exactly 1 argument")
 
-        mjd = float (args[0])
+        mjd = float(args[0])
 
         import astropy.time
-        t = astropy.time.Time (mjd, format='mjd', scale='tai')
-        print (t.utc.iso, 'UTC')
+
+        t = astropy.time.Time(mjd, format="mjd", scale="tai")
+        print(t.utc.iso, "UTC")
 
 
-class Sastrom (multitool.Command):
-    name = 'sastrom'
-    argspec = '[-v] <source name> <MJD>'
-    summary = 'Compute source location using Simbad data.'
+class Sastrom(multitool.Command):
+    name = "sastrom"
+    argspec = "[-v] <source name> <MJD>"
+    summary = "Compute source location using Simbad data."
 
-    def invoke (self, args, **kwargs):
-        verbose = pop_option ('v', args)
+    def invoke(self, args, **kwargs):
+        verbose = pop_option("v", args)
 
-        if len (args) != 2:
-            raise multitool.UsageError ('sastrom expected 2 arguments')
+        if len(args) != 2:
+            raise multitool.UsageError("sastrom expected 2 arguments")
 
         ident = args[0]
-        mjd = float (args[1])
+        mjd = float(args[1])
 
-        info = AstrometryInfo ()
-        info.fill_from_simbad (ident, debug=verbose)
-        p = info.predict (mjd)
-        print ('%s at %.3f:' % (ident, mjd))
-        print ()
-        info.print_prediction (p)
-
-
-class Sesame (multitool.Command):
-    name = 'sesame'
-    argspec = '{source name}'
-    summary = 'Print source information from Sesame/Simbad.'
-
-    def invoke (self, args, **kwargs):
-        if not len (args):
-            raise multitool.UsageError ('sesame expected an argument')
+        info = AstrometryInfo()
+        info.fill_from_simbad(ident, debug=verbose)
+        p = info.predict(mjd)
+        print("%s at %.3f:" % (ident, mjd))
+        print()
+        info.print_prediction(p)
+
+
+class Sesame(multitool.Command):
+    name = "sesame"
+    argspec = "{source name}"
+    summary = "Print source information from Sesame/Simbad."
+
+    def invoke(self, args, **kwargs):
+        if not len(args):
+            raise multitool.UsageError("sesame expected an argument")
 
-        src = ' '.join (args)
+        src = " ".join(args)
         from ..astutil import AstrometryInfo
 
         try:
-            obj = AstrometryInfo(simbadident = src)
+            obj = AstrometryInfo(simbadident=src)
         except Exception as e:
-            die ('couldn\'t look up "%s": %s (%s)', src, e, e.__class__.__name__)
+            die('couldn\'t look up "%s": %s (%s)', src, e, e.__class__.__name__)
 
         print(obj)
 
 
-class Senscale (multitool.Command):
-    name = 'senscale'
-    argspec = '<sens 1> <time 1> <time 2>'
-    summary = 'Scale a sensitivity to a different integration time.'
-
-    def invoke (self, args, **kwargs):
-        if len (args) != 3:
-            raise multitool.UsageError ('senscale expected 3 arguments')
-
-        s1 = fparse (args[0])
-        t1 = fparse (args[1])
-        t2 = fparse (args[2])
-        s2 = s1 * np.sqrt (t1 / t2)
-        print (fmt (s2))
-
-
-class Sh2d (multitool.Command):
-    name = 'sh2d'
-    argspec = '<sexagesimal hours>'
-    summary = 'Convert sexagesimal hours to decimal degrees.'
+class Senscale(multitool.Command):
+    name = "senscale"
+    argspec = "<sens 1> <time 1> <time 2>"
+    summary = "Scale a sensitivity to a different integration time."
+
+    def invoke(self, args, **kwargs):
+        if len(args) != 3:
+            raise multitool.UsageError("senscale expected 3 arguments")
+
+        s1 = fparse(args[0])
+        t1 = fparse(args[1])
+        t2 = fparse(args[2])
+        s2 = s1 * np.sqrt(t1 / t2)
+        print(fmt(s2))
+
+
+class Sh2d(multitool.Command):
+    name = "sh2d"
+    argspec = "<sexagesimal hours>"
+    summary = "Convert sexagesimal hours to decimal degrees."
     more_help = """The argument should look like "12:20:14.6"."""
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 1:
-            raise multitool.UsageError ('sh2d expected 1 argument')
+    def invoke(self, args, **kwargs):
+        if len(args) != 1:
+            raise multitool.UsageError("sh2d expected 1 argument")
 
         try:
-            rarad = parsehours (args[0])
+            rarad = parsehours(args[0])
         except Exception as e:
-            die ('couldn\'t parse "%s" as sexagesimal hours: %s (%s)',
-                 args[0], e, e.__class__.__name__)
-
-        print ('%.8f' % (rarad * R2D))
-
-
-class Sl2d (multitool.Command):
-    name = 'sl2d'
-    argspec = '<sexagesimal latitude in degrees>'
-    summary = 'Convert sexagesimal latitude (ie, declination) to decimal degrees.'
-    more_help = """The argument should look like "47:20:14.6". The leading sign is optional."""
-
-    def invoke (self, args, **kwargs):
-        if len (args) != 1:
-            raise multitool.UsageError ('sl2d expected 1 argument')
+            die(
+                'couldn\'t parse "%s" as sexagesimal hours: %s (%s)',
+                args[0],
+                e,
+                e.__class__.__name__,
+            )
+
+        print("%.8f" % (rarad * R2D))
+
+
+class Sl2d(multitool.Command):
+    name = "sl2d"
+    argspec = "<sexagesimal latitude in degrees>"
+    summary = "Convert sexagesimal latitude (ie, declination) to decimal degrees."
+    more_help = (
+        """The argument should look like "47:20:14.6". The leading sign is optional."""
+    )
+
+    def invoke(self, args, **kwargs):
+        if len(args) != 1:
+            raise multitool.UsageError("sl2d expected 1 argument")
 
         try:
-            decrad = parsedeglat (args[0])
+            decrad = parsedeglat(args[0])
         except Exception as e:
-            die ('couldn\'t parse "%s" as sexagesimal latitude in degrees: %s (%s)',
-                 args[0], e, e.__class__.__name__)
-
-        print ('%.8f' % (decrad * R2D))
-
-
-class Ssep (multitool.Command):
-    name = 'ssep'
-    argspec = '<source name> <source name>'
-    summary = 'Print separation between two sources identified by name.'
-
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('ssep expected 2 arguments')
+            die(
+                'couldn\'t parse "%s" as sexagesimal latitude in degrees: %s (%s)',
+                args[0],
+                e,
+                e.__class__.__name__,
+            )
+
+        print("%.8f" % (decrad * R2D))
+
+
+class Ssep(multitool.Command):
+    name = "ssep"
+    argspec = "<source name> <source name>"
+    summary = "Print separation between two sources identified by name."
+
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError("ssep expected 2 arguments")
 
         from ..astutil import AstrometryInfo
 
         try:
             obj1 = AstrometryInfo(simbadident=args[0])
         except Exception as e:
-            die ('couldn\'t look up "%s": %s (%s)', args[0], e, e.__class__.__name__)
+            die('couldn\'t look up "%s": %s (%s)', args[0], e, e.__class__.__name__)
 
         try:
             obj2 = AstrometryInfo(simbadident=args[1])
         except Exception as e:
-            die ('couldn\'t look up "%s": %s (%s)', args[1], e, e.__class__.__name__)
+            die('couldn\'t look up "%s": %s (%s)', args[1], e, e.__class__.__name__)
 
-        print ('degree:', fmt (sphdist (obj1.dec, obj1.ra, obj2.dec, obj2.ra) * R2D))
-        print ('arcsec:', fmt (sphdist (obj1.dec, obj1.ra, obj2.dec, obj2.ra) * R2A))
+        print("degree:", fmt(sphdist(obj1.dec, obj1.ra, obj2.dec, obj2.ra) * R2D))
+        print("arcsec:", fmt(sphdist(obj1.dec, obj1.ra, obj2.dec, obj2.ra) * R2A))
 
 
-class Summfits (multitool.Command):
-    name = 'summfits'
-    argspec = '<path>'
-    summary = 'Summarize contents of a FITS file.'
-
-    _commentary_card_names = frozenset (('HISTORY', 'COMMENT'))
-    _skip_headers = frozenset (('XTENSION', 'BITPIX', 'SIMPLE', 'EXTEND',
-                                'EXTNAME', 'PCOUNT', 'GCOUNT', 'TFIELDS',
-                                '')) # <= STScI FITS files can use blank keys for spacing
-    _skip_prefixes = frozenset (('NAXIS', 'TTYPE', 'TFORM', 'TDIM', 'TUNIT'))
-
-    def invoke (self, args, **kwargs):
-        if len (args) != 1:
-            raise multitool.UsageError ('summfits expected 1 argument')
+class Summfits(multitool.Command):
+    name = "summfits"
+    argspec = "<path>"
+    summary = "Summarize contents of a FITS file."
+
+    _commentary_card_names = frozenset(("HISTORY", "COMMENT"))
+    _skip_headers = frozenset(
+        (
+            "XTENSION",
+            "BITPIX",
+            "SIMPLE",
+            "EXTEND",
+            "EXTNAME",
+            "PCOUNT",
+            "GCOUNT",
+            "TFIELDS",
+            "",
+        )
+    )  # <= STScI FITS files can use blank keys for spacing
+    _skip_prefixes = frozenset(("NAXIS", "TTYPE", "TFORM", "TDIM", "TUNIT"))
+
+    def invoke(self, args, **kwargs):
+        if len(args) != 1:
+            raise multitool.UsageError("summfits expected 1 argument")
 
         try:
             from astropy.io import fits
         except ImportError:
             try:
                 import pyfits as fits
-                warn ('falling back to untested "pyfits" backend')
+
+                warn('falling back to untested "pyfits" backend')
             except ImportError:
-                die ('need either the "astropy.io.fits" or the "pyfits" modules')
+                die('need either the "astropy.io.fits" or the "pyfits" modules')
 
         fitspath = args[0]
 
         try:
-            hdulist = fits.open (fitspath)
+            hdulist = fits.open(fitspath)
         except Exception as e:
-            die ('couldn\'t open "%s" as a FITS file: %s', fitspath, e)
+            die('couldn\'t open "%s" as a FITS file: %s', fitspath, e)
 
-        def output (depth, fmt, *args):
-            print ('  ' * depth, fmt % args, sep='')
+        def output(depth, fmt, *args):
+            print("  " * depth, fmt % args, sep="")
 
-        output (0, '%s: %d HDUs', fitspath, len (hdulist))
-        hduidxwidth = len (str (len (hdulist)))
+        output(0, "%s: %d HDUs", fitspath, len(hdulist))
+        hduidxwidth = len(str(len(hdulist)))
         hdunamewidth = 0
 
         for hdu in hdulist:
-            hdunamewidth = max (hdunamewidth, len (hdu.name))
+            hdunamewidth = max(hdunamewidth, len(hdu.name))
 
-        for hduidx, hdu in enumerate (hdulist):
+        for hduidx, hdu in enumerate(hdulist):
             # TODO: handle more HDU kinds. See
             # astropy/io/fits/hdu/__init__.py. Looks like possibilities are
             # Primary, Image, Table, BinTable, Groups, CompImage,
             # nonstandard/Fits, and Streaming.
 
             if hdu.data is None:
-                kind = 'empty'
-            elif hasattr (hdu, 'columns'):
-                kind = 'table'
+                kind = "empty"
+            elif hasattr(hdu, "columns"):
+                kind = "table"
             elif hdu.is_image:
-                kind = 'image'
+                kind = "image"
             else:
-                kind = '???'
+                kind = "???"
 
-            output (1, 'HDU %*d = %*s: kind=%s size=%d ver=%s level=%s',
-                    hduidxwidth, hduidx, hdunamewidth, hdu.name, kind, hdu.size,
-                    hdu.ver, hdu.level)
+            output(
+                1,
+                "HDU %*d = %*s: kind=%s size=%d ver=%s level=%s",
+                hduidxwidth,
+                hduidx,
+                hdunamewidth,
+                hdu.name,
+                kind,
+                hdu.size,
+                hdu.ver,
+                hdu.level,
+            )
 
-            output (2, '%d headers (some omitted)', len (hdu.header))
+            output(2, "%d headers (some omitted)", len(hdu.header))
 
             for k, value, comment in hdu.header.cards:
                 if k in self._commentary_card_names or k in self._skip_headers:
                     continue
 
                 for pfx in self._skip_prefixes:
                     if k.startswith(pfx):
                         break
                 else:
                     # We did not break out of the loop -> shouldn't be skipped.
-                    output(3, '%-8s = %r # %s', k, value, comment)
+                    output(3, "%-8s = %r # %s", k, value, comment)
 
             for ck in self._commentary_card_names:
                 # hacky linewrapping logic here
                 if ck not in hdu.header:
                     continue
 
-                buf = ''
+                buf = ""
                 h = hdu.header[ck]
-                output (2, '%s commentary', ck)
+                output(2, "%s commentary", ck)
 
-                for ccidx in range (len (h)):
+                for ccidx in range(len(h)):
                     s = h[ccidx]
                     buf += s
 
-                    if len (s) in (71, 72):
-                        continue # assume hard linewrapping
+                    if len(s) in (71, 72):
+                        continue  # assume hard linewrapping
 
-                    output (3, '%s', buf)
-                    buf = ''
+                    output(3, "%s", buf)
+                    buf = ""
 
-                if len (buf):
-                    output (3, '%s', buf)
+                if len(buf):
+                    output(3, "%s", buf)
 
-            if kind == 'table':
-                colidxwidth = len (str (len (hdu.columns)))
+            if kind == "table":
+                colidxwidth = len(str(len(hdu.columns)))
                 colnamewidth = 0
 
-                output (2, '%d rows, %d columns', hdu.data.size, len (hdu.columns))
+                output(2, "%d rows, %d columns", hdu.data.size, len(hdu.columns))
 
                 for col in hdu.columns:
-                    colnamewidth = max (colnamewidth, len (col.name))
-
-                for colidx, col in enumerate (hdu.columns):
-                    output (3, 'col %*d = %*s: format=%s unit=%s', colidxwidth,
-                            colidx, colnamewidth, col.name, col.format, col.unit)
-            elif kind == 'image':
-                output (2, 'data shape=%r dtype=%s', hdu.data.shape, hdu.data.dtype)
+                    colnamewidth = max(colnamewidth, len(col.name))
 
-
-class T2m (multitool.Command):
-    name = 't2m'
-    argspec = '<text>'
-    summary = 'Convert a textual time in UTC to MJD[TAI].'
-    more_help = '''This uses the Astropy time parsing code. See
+                for colidx, col in enumerate(hdu.columns):
+                    output(
+                        3,
+                        "col %*d = %*s: format=%s unit=%s",
+                        colidxwidth,
+                        colidx,
+                        colnamewidth,
+                        col.name,
+                        col.format,
+                        col.unit,
+                    )
+            elif kind == "image":
+                output(2, "data shape=%r dtype=%s", hdu.data.shape, hdu.data.dtype)
+
+
+class T2m(multitool.Command):
+    name = "t2m"
+    argspec = "<text>"
+    summary = "Convert a textual time in UTC to MJD[TAI]."
+    more_help = """This uses the Astropy time parsing code. See
 http://docs.astropy.org/en/stable/time/#time-format for a list of allowed
 formats. If multiple arguments are supplied, they will be joined with spaces
-before parsing.'''
+before parsing."""
 
-    def invoke (self, args, **kwargs):
-        if not len (args):
-            raise multitool.UsageError ('t2m expected at least one argument')
+    def invoke(self, args, **kwargs):
+        if not len(args):
+            raise multitool.UsageError("t2m expected at least one argument")
 
         from astropy.time import Time
-        s = ' '.join (args)
-        t = Time (s, scale='utc')
-        print ('%.4f' % t.tai.mjd)
+
+        s = " ".join(args)
+        t = Time(s, scale="utc")
+        print("%.4f" % t.tai.mjd)
 
 
 # The driver.
 
 from .multitool import HelpCommand
 
-class Astrotool (multitool.Multitool):
-    cli_name = 'astrotool'
-    summary = 'Perform miscellaneous astronomical calculations.'
 
-def commandline ():
-    multitool.invoke_tool (globals ())
+class Astrotool(multitool.Multitool):
+    cli_name = "astrotool"
+    summary = "Perform miscellaneous astronomical calculations."
+
+
+def commandline():
+    multitool.invoke_tool(globals())
```

### Comparing `pwkit-1.1.1/pwkit/cli/imtool.py` & `pwkit-1.2.0/pwkit/cli/imtool.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,602 +3,660 @@
 # Licensed under the MIT License.
 
 """pwkit.cli.imtool - the 'imtool' program.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('commandline').split ()
+__all__ = str("commandline").split()
 
 import numpy as np, sys
-from six.moves import range
 
-from .. import PKError
 from . import multitool
 from . import *
 from .. import astimage
 from ..io import Path
 
 
-def load_ndshow ():
+def load_ndshow():
     try:
         from .. import ndshow_gtk3 as ndshow
     except ImportError as e:
-        try:
-            from .. import ndshow_gtk2 as ndshow
-        except ImportError as e:
-            die ('cannot load graphics backend for viewing images: %s', e)
+        die("cannot load graphics backend for viewing images: %s", e)
 
     return ndshow
 
 
 # The commands.
 
-class BlinkCommand (multitool.Command):
-    name = 'blink'
-    argspec = '[-f] <images...>'
-    summary = 'Blink zero or more images.'
+
+class BlinkCommand(multitool.Command):
+    name = "blink"
+    argspec = "[-f] <images...>"
+    summary = "Blink zero or more images."
     more_help = """
 -f  - Show the 2D FFT of the images
 
 WCS support isn't fantastic and sometimes causes crashes.
 
 If an input image has multiple planes, they will be showed separately.
 """
 
-    def _load (self, path, fft, maxnorm):
+    def _load(self, path, fft, maxnorm):
         try:
-            img = astimage.open (path, 'r', eat_warnings=True)
+            img = astimage.open(path, "r", eat_warnings=True)
         except Exception as e:
-            die ('can\'t open path “%s”: %s', path, e)
+            die("can't open path “%s”: %s", path, e)
 
         def getplanes():
             try:
-                simg = img.simple ()
+                simg = img.simple()
             except Exception as e:
                 # Multi-dimensional image -- iterate over outer planes
                 fulldata = img.read(flip=True)
 
                 for index in np.ndindex(*img.shape[:-2]):
-                    yield fulldata[index], None, ' ' + repr(index)
+                    yield fulldata[index], None, " " + repr(index)
             else:
-                yield simg.read (flip=True), img.toworld, ''
+                yield simg.read(flip=True), img.toworld, ""
 
         for data, toworld, desc in getplanes():
             if fft:
                 from numpy.fft import ifftshift, fft2, fftshift
-                data = np.abs (ifftshift (fft2 (fftshift (data.filled (0)))))
-                data = np.ma.MaskedArray (data)
+
+                data = np.abs(ifftshift(fft2(fftshift(data.filled(0)))))
+                data = np.ma.MaskedArray(data)
                 toworld = None
 
             if maxnorm:
-                data /= np.ma.max (data)
+                data /= np.ma.max(data)
 
             yield data, toworld, desc
 
-
-    def invoke (self, args, **kwargs):
-        fft = pop_option ('f', args)
-        maxnorm = pop_option ('m', args)
-        ndshow = load_ndshow ()
+    def invoke(self, args, **kwargs):
+        fft = pop_option("f", args)
+        maxnorm = pop_option("m", args)
+        ndshow = load_ndshow()
 
         images = []
         toworlds = []
         names = []
 
         for path in args:
-            for image, toworld, desc in self._load (path, fft, maxnorm):
-                images.append (image)
-                toworlds.append (toworld)
+            for image, toworld, desc in self._load(path, fft, maxnorm):
+                images.append(image)
+                toworlds.append(toworld)
                 names.append(path + desc)
 
-        if not len (images):
+        if not len(images):
             return
 
         shape = images[0].shape
-        for i, im in enumerate (images[1:]):
+        for i, im in enumerate(images[1:]):
             if im.shape != shape:
-                die ('shape of “%s” (%s) does not agree with that '
-                     'of “%s” (%s)',
-                     args[i+1], '×'.join (map (str, im.shape)),
-                     args[0], '×'.join (map (str, shape)))
+                die(
+                    "shape of “%s” (%s) does not agree with that " "of “%s” (%s)",
+                    args[i + 1],
+                    "×".join(map(str, im.shape)),
+                    args[0],
+                    "×".join(map(str, shape)),
+                )
 
         # Merge masks. This is more complicated than you might think since you
         # can't "or" nomask with itself.
 
         jointmask = np.ma.nomask
 
-        for i in range (len (images)):
+        for i in range(len(images)):
             if jointmask is np.ma.nomask:
                 if images[i].mask is not np.ma.nomask:
                     jointmask = images[i].mask
             else:
-                np.logical_or (jointmask, images[i].mask, jointmask)
+                np.logical_or(jointmask, images[i].mask, jointmask)
 
         for im in images:
             im.mask = jointmask
 
-        ndshow.cycle (images, names, toworlds=toworlds, yflip=True)
+        ndshow.cycle(images, names, toworlds=toworlds, yflip=True)
 
 
-class FitsrcCommand (multitool.ArgparsingCommand):
-    name = 'fitsrc'
-    summary = 'Fit a compact-source model to a location in an image.'
-
-    def get_arg_parser (self, **kwargs):
-        ap = super (FitsrcCommand, self).get_arg_parser (**kwargs)
-        ap.add_argument ('--forcepoint', '-p', action='store_true',
-                         help='Force the use of a point-source model.')
-        ap.add_argument ('--display', '-d', action='store_true',
-                         help='Display the fit results graphically.')
-        ap.add_argument ('--format', metavar='FORMAT', default='shell',
-                         help='Output format for results: "shell", "yaml".')
-        ap.add_argument ('--dest', metavar='PATH',
-                         help='Path in which to save results.')
-        ap.add_argument ('--section', metavar='LOCATION.TO.SECTION',
-                         help='Save results in the named dot-separated section of the output file.')
-        ap.add_argument ('image', metavar='IMAGE-PATH',
-                         help='The path to an image.')
-        ap.add_argument ('x', metavar='X-PIXEL', type=int,
-                         help='The X pixel coordinate near which to search for a source.')
-        ap.add_argument ('y', metavar='Y-PIXEL', type=int,
-                         help='The Y pixel coordinate near which to search for a source.')
+class FitsrcCommand(multitool.ArgparsingCommand):
+    name = "fitsrc"
+    summary = "Fit a compact-source model to a location in an image."
+
+    def get_arg_parser(self, **kwargs):
+        ap = super(FitsrcCommand, self).get_arg_parser(**kwargs)
+        ap.add_argument(
+            "--forcepoint",
+            "-p",
+            action="store_true",
+            help="Force the use of a point-source model.",
+        )
+        ap.add_argument(
+            "--display",
+            "-d",
+            action="store_true",
+            help="Display the fit results graphically.",
+        )
+        ap.add_argument(
+            "--format",
+            metavar="FORMAT",
+            default="shell",
+            help='Output format for results: "shell", "yaml".',
+        )
+        ap.add_argument("--dest", metavar="PATH", help="Path in which to save results.")
+        ap.add_argument(
+            "--section",
+            metavar="LOCATION.TO.SECTION",
+            help="Save results in the named dot-separated section of the output file.",
+        )
+        ap.add_argument("image", metavar="IMAGE-PATH", help="The path to an image.")
+        ap.add_argument(
+            "x",
+            metavar="X-PIXEL",
+            type=int,
+            help="The X pixel coordinate near which to search for a source.",
+        )
+        ap.add_argument(
+            "y",
+            metavar="Y-PIXEL",
+            type=int,
+            help="The Y pixel coordinate near which to search for a source.",
+        )
         return ap
 
-
-    def invoke (self, args, **kwargs):
+    def invoke(self, args, **kwargs):
         from ..immodel import fit_one_source
 
         # TODO: would be nice to have a consistent API for outputting
         # structured data in a variety of formats, preferably supporting
         # streaming.
 
         close_me = None
 
-        if args.format == 'shell':
+        if args.format == "shell":
             if args.dest is not None:
-                dest = close_me = open (args.dest, 'wt')
+                dest = close_me = open(args.dest, "wt")
             else:
                 import sys
+
                 dest = sys.stdout
 
-            def report_func (key, fmt, value):
-                print (key, '=', fmt % value, sep='', file=dest)
-        elif args.format == 'yaml':
+            def report_func(key, fmt, value):
+                print(key, "=", fmt % value, sep="", file=dest)
+
+        elif args.format == "yaml":
             from collections import OrderedDict
 
             try:
                 from ruamel import yaml as ruamel_yaml
             except ImportError:
-                import ruamel_yaml # how Conda packages it, grr ...
+                import ruamel_yaml  # how Conda packages it, grr ...
 
             if args.dest is None:
                 toplevel = None
             else:
-                with Path (args.dest).try_open ('rt') as f:
-                    toplevel = ruamel_yaml.load (f, ruamel_yaml.RoundTripLoader)
+                with Path(args.dest).try_open("rt") as f:
+                    toplevel = ruamel_yaml.load(f, ruamel_yaml.RoundTripLoader)
 
             if toplevel is None:
                 toplevel = OrderedDict()
 
             dest_section = toplevel
 
             if args.section is not None:
-                for piece in args.section.split ('.'):
-                    dest_section = dest_section.setdefault (piece, OrderedDict())
+                for piece in args.section.split("."):
+                    dest_section = dest_section.setdefault(piece, OrderedDict())
 
-            dest_section.clear ()
+            dest_section.clear()
 
-            def report_func (key, fmt, value):
-                if isinstance (value, np.number):
-                    value = value.item ()
+            def report_func(key, fmt, value):
+                if isinstance(value, np.number):
+                    value = value.item()
                 dest_section[key] = value
+
         else:
-            die ('unrecognized output format %r', args.format)
+            die("unrecognized output format %r", args.format)
 
-        im = astimage.open (args.image, 'r', eat_warnings=True).simple ()
-        fit_one_source (im, args.x, args.y, forcepoint=args.forcepoint,
-                        display=args.display, report_func=report_func)
+        im = astimage.open(args.image, "r", eat_warnings=True).simple()
+        fit_one_source(
+            im,
+            args.x,
+            args.y,
+            forcepoint=args.forcepoint,
+            display=args.display,
+            report_func=report_func,
+        )
 
         if close_me is not None:
-            close_me.close ()
+            close_me.close()
 
-        if args.format == 'yaml':
+        if args.format == "yaml":
             if args.dest is None:
                 import sys
-                ruamel_yaml.dump (toplevel, stream=sys.stdout, Dumper=ruamel_yaml.RoundTripDumper)
+
+                ruamel_yaml.dump(
+                    toplevel, stream=sys.stdout, Dumper=ruamel_yaml.RoundTripDumper
+                )
             else:
-                with Path (args.dest).open ('wt') as f:
-                    ruamel_yaml.dump (toplevel, stream=f, Dumper=ruamel_yaml.RoundTripDumper)
+                with Path(args.dest).open("wt") as f:
+                    ruamel_yaml.dump(
+                        toplevel, stream=f, Dumper=ruamel_yaml.RoundTripDumper
+                    )
 
 
-class HackdataCommand (multitool.Command):
-    name = 'hackdata'
-    argspec = '<inpath> <outpath>'
-    summary = 'Blindly copy pixel data from one image to another.'
-
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('expect exactly two arguments')
+class HackdataCommand(multitool.Command):
+    name = "hackdata"
+    argspec = "<inpath> <outpath>"
+    summary = "Blindly copy pixel data from one image to another."
+
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError("expect exactly two arguments")
 
         inpath, outpath = args
 
         try:
-            with astimage.open (inpath, 'r', eat_warnings=True) as imin:
-                indata = imin.read ()
+            with astimage.open(inpath, "r", eat_warnings=True) as imin:
+                indata = imin.read()
         except Exception as e:
-            die ('cannot open input "%s": %s', inpath, e)
+            die('cannot open input "%s": %s', inpath, e)
 
         try:
-            with astimage.open (outpath, 'rw') as imout:
+            with astimage.open(outpath, "rw") as imout:
                 if imout.size != indata.size:
-                    die ('cannot import data: input has %d pixels; output has %d',
-                         indata.size, imout.size)
+                    die(
+                        "cannot import data: input has %d pixels; output has %d",
+                        indata.size,
+                        imout.size,
+                    )
 
-                imout.write (indata)
+                imout.write(indata)
         except Exception as e:
-            die ('cannot write to output "%s": %s', outpath, e)
+            die('cannot write to output "%s": %s', outpath, e)
 
 
-class InfoCommand (multitool.ArgparsingCommand):
+class InfoCommand(multitool.ArgparsingCommand):
     # XXX terrible code duplication while my output format stuff is half-baked.
 
-    name = 'info'
-    summary = 'Print properties of one or more images.'
+    name = "info"
+    summary = "Print properties of one or more images."
 
-    def get_arg_parser (self, **kwargs):
-        ap = super (InfoCommand, self).get_arg_parser (**kwargs)
-        ap.add_argument ('--format', metavar='FORMAT', default='pretty',
-                         help='Output format for results: "pretty", "yaml".')
-        ap.add_argument ('--dest', metavar='PATH',
-                         help='Path in which to save results.')
-        ap.add_argument ('--section', metavar='LOCATION.TO.SECTION',
-                         help='Save results in the named dot-separated section of the output file.')
-        ap.add_argument ('images', metavar='IMAGE-PATH', nargs='+',
-                         help='The path to an image.')
+    def get_arg_parser(self, **kwargs):
+        ap = super(InfoCommand, self).get_arg_parser(**kwargs)
+        ap.add_argument(
+            "--format",
+            metavar="FORMAT",
+            default="pretty",
+            help='Output format for results: "pretty", "yaml".',
+        )
+        ap.add_argument("--dest", metavar="PATH", help="Path in which to save results.")
+        ap.add_argument(
+            "--section",
+            metavar="LOCATION.TO.SECTION",
+            help="Save results in the named dot-separated section of the output file.",
+        )
+        ap.add_argument(
+            "images", metavar="IMAGE-PATH", nargs="+", help="The path to an image."
+        )
         return ap
 
-
-    def invoke (self, args, **kwargs):
-        if args.format == 'pretty':
-            self._invoke_pretty_format (args.images)
-        elif args.format == 'yaml':
-            self._invoke_yaml_format (args)
+    def invoke(self, args, **kwargs):
+        if args.format == "pretty":
+            self._invoke_pretty_format(args.images)
+        elif args.format == "yaml":
+            self._invoke_yaml_format(args)
         else:
-            die ('unrecognized output format %r', args.format)
+            die("unrecognized output format %r", args.format)
 
-
-    def _invoke_pretty_format (self, impaths):
-        if len (impaths) == 1:
-            self._print (impaths[0])
+    def _invoke_pretty_format(self, impaths):
+        if len(impaths) == 1:
+            self._print(impaths[0])
         else:
-            for i, path in enumerate (impaths):
+            for i, path in enumerate(impaths):
                 if i > 0:
-                    print ()
-                print ('path     =', path)
-                self._print (path)
-
+                    print()
+                print("path     =", path)
+                self._print(path)
 
-    def _print (self, path):
+    def _print(self, path):
         from ..astutil import fmtradec, R2A, R2D
 
         try:
-            im = astimage.open (path, 'r', eat_warnings=True)
+            im = astimage.open(path, "r", eat_warnings=True)
         except Exception as e:
-            die ('can\'t open "%s": %s', path, e)
+            die('can\'t open "%s": %s', path, e)
 
-        print ('kind     =', im.__class__.__name__)
+        print("kind     =", im.__class__.__name__)
 
         latcell = loncell = None
 
         if im.toworld is not None:
             latax, lonax = im._latax, im._lonax
             delta = 1e-6
-            p = 0.5 * (np.asfarray (im.shape) - 1)
-            w1 = im.toworld (p)
+            p = 0.5 * (np.asfarray(im.shape) - 1)
+            w1 = im.toworld(p)
             p[latax] += delta
-            w2 = im.toworld (p)
+            w2 = im.toworld(p)
             latcell = (w2[latax] - w1[latax]) / delta
             p[latax] -= delta
             p[lonax] += delta
-            w2 = im.toworld (p)
-            loncell = (w2[lonax] - w1[lonax]) / delta * np.cos (w2[latax])
+            w2 = im.toworld(p)
+            loncell = (w2[lonax] - w1[lonax]) / delta * np.cos(w2[latax])
 
         if im.pclat is not None:
-            print ('center   =', fmtradec (im.pclon, im.pclat), '# pointing')
+            print("center   =", fmtradec(im.pclon, im.pclat), "# pointing")
         elif im.toworld is not None:
-            w = im.toworld (0.5 * (np.asfarray (im.shape) - 1))
-            print ('center   =', fmtradec (w[lonax], w[latax]), '# lattice')
+            w = im.toworld(0.5 * (np.asfarray(im.shape) - 1))
+            print("center   =", fmtradec(w[lonax], w[latax]), "# lattice")
 
         if im.shape is not None:
-            print ('shape    =', ' '.join (str (x) for x in im.shape))
+            print("shape    =", " ".join(str(x) for x in im.shape))
             npix = 1
             for x in im.shape:
                 npix *= x
-            print ('npix     =', npix)
+            print("npix     =", npix)
 
         if im.axdescs is not None:
-            print ('axdescs  =', ' '.join (x for x in im.axdescs))
+            print("axdescs  =", " ".join(x for x in im.axdescs))
 
         if im.charfreq is not None:
-            print ('charfreq = %f GHz' % im.charfreq)
+            print("charfreq = %f GHz" % im.charfreq)
 
         if im.mjd is not None:
             from time import gmtime, strftime
-            posix = 86400. * (im.mjd - 40587.)
-            ts = strftime ('%Y-%m-%dT%H-%M-%SZ', gmtime (posix))
-            print ('mjd      = %f # %s' % (im.mjd, ts))
+
+            posix = 86400.0 * (im.mjd - 40587.0)
+            ts = strftime("%Y-%m-%dT%H-%M-%SZ", gmtime(posix))
+            print("mjd      = %f # %s" % (im.mjd, ts))
 
         if latcell is not None:
-            print ('ctrcell  = %fʺ × %fʺ # lat, lon' % (latcell * R2A,
-                                                        loncell * R2A))
+            print("ctrcell  = %fʺ × %fʺ # lat, lon" % (latcell * R2A, loncell * R2A))
 
         if im.bmaj is not None:
-            print ('beam     = %fʺ × %fʺ @ %f°' % (im.bmaj * R2A,
-                                                   im.bmin * R2A,
-                                                   im.bpa * R2D))
+            print(
+                "beam     = %fʺ × %fʺ @ %f°"
+                % (im.bmaj * R2A, im.bmin * R2A, im.bpa * R2D)
+            )
 
             if latcell is not None:
-                bmrad2 = 2 * np.pi * im.bmaj * im.bmin / (8 * np.log (2))
+                bmrad2 = 2 * np.pi * im.bmaj * im.bmin / (8 * np.log(2))
                 cellrad2 = latcell * loncell
-                print ('ctrbmvol = %f px' % np.abs (bmrad2 / cellrad2))
+                print("ctrbmvol = %f px" % np.abs(bmrad2 / cellrad2))
 
         if im.units is not None:
-            print ('units    =', im.units)
-
+            print("units    =", im.units)
 
-    def _invoke_yaml_format (self, args):
+    def _invoke_yaml_format(self, args):
         from collections import OrderedDict
         from ..astutil import fmtdeglat, fmthours, R2A, R2D
 
-        if len (args.images) > 1:
-            die ('can only use YAML output format with one image')
+        if len(args.images) > 1:
+            die("can only use YAML output format with one image")
 
         try:
-            im = astimage.open (args.images[0], 'r', eat_warnings=True)
+            im = astimage.open(args.images[0], "r", eat_warnings=True)
         except Exception as e:
-            die ('can\'t open "%s": %s', args.images[0], e)
+            die('can\'t open "%s": %s', args.images[0], e)
 
         try:
             from ruamel import yaml as ruamel_yaml
         except ImportError:
-            import ruamel_yaml # how Conda packages it, grr ...
+            import ruamel_yaml  # how Conda packages it, grr ...
 
         if args.dest is None:
             toplevel = None
         else:
-            with Path (args.dest).try_open ('rt') as f:
-                toplevel = ruamel_yaml.load (f, ruamel_yaml.RoundTripLoader)
+            with Path(args.dest).try_open("rt") as f:
+                toplevel = ruamel_yaml.load(f, ruamel_yaml.RoundTripLoader)
 
         if toplevel is None:
             toplevel = OrderedDict()
 
         dest_section = toplevel
 
         if args.section is not None:
-            for piece in args.section.split ('.'):
-                dest_section = dest_section.setdefault (piece, OrderedDict())
+            for piece in args.section.split("."):
+                dest_section = dest_section.setdefault(piece, OrderedDict())
 
         def okeys(**kwargs):
             return OrderedDict(sorted(kwargs.items(), key=lambda t: t[0]))
 
-        dest_section.clear ()
-        dest_section['kind'] = im.__class__.__name__
+        dest_section.clear()
+        dest_section["kind"] = im.__class__.__name__
 
         latcell = loncell = None
 
         if im.toworld is not None:
             latax, lonax = im._latax, im._lonax
             delta = 1e-6
-            p = 0.5 * (np.asfarray (im.shape) - 1)
-            w1 = im.toworld (p)
+            p = 0.5 * (np.asfarray(im.shape) - 1)
+            w1 = im.toworld(p)
             p[latax] += delta
-            w2 = im.toworld (p)
+            w2 = im.toworld(p)
             latcell = (w2[latax] - w1[latax]) / delta
             p[latax] -= delta
             p[lonax] += delta
-            w2 = im.toworld (p)
-            loncell = (w2[lonax] - w1[lonax]) / delta * np.cos (w2[latax])
+            w2 = im.toworld(p)
+            loncell = (w2[lonax] - w1[lonax]) / delta * np.cos(w2[latax])
 
         if im.pclat is not None:
-            dest_section['center'] = okeys(
-                kind = 'pointing',
-                lat = fmtdeglat (im.pclat),
-                lon = fmthours (im.pclon),
+            dest_section["center"] = okeys(
+                kind="pointing",
+                lat=fmtdeglat(im.pclat),
+                lon=fmthours(im.pclon),
             )
         elif im.toworld is not None:
-            w = im.toworld (0.5 * (np.asfarray (im.shape) - 1))
-            dest_section['center'] = okeys(
-                kind = 'lattice',
-                lat = fmtdeglat (w[latax]),
-                lon = fmthours (w[lonax]),
+            w = im.toworld(0.5 * (np.asfarray(im.shape) - 1))
+            dest_section["center"] = okeys(
+                kind="lattice",
+                lat=fmtdeglat(w[latax]),
+                lon=fmthours(w[lonax]),
             )
 
         if im.shape is not None:
-            dest_section['shape'] = [x.item () for x in im.shape]
+            dest_section["shape"] = [x.item() for x in im.shape]
             npix = 1
             for x in im.shape:
                 npix *= x
-            dest_section['npix'] = npix.item ()
+            dest_section["npix"] = npix.item()
 
         if im.axdescs is not None:
-            dest_section['axdescs'] = list (im.axdescs)
+            dest_section["axdescs"] = list(im.axdescs)
 
         if im.charfreq is not None:
-            dest_section['charfreq'] = im.charfreq
+            dest_section["charfreq"] = im.charfreq
 
         if im.mjd is not None:
-            dest_section['mjd'] = im.mjd
+            dest_section["mjd"] = im.mjd
 
         if latcell is not None:
-            dest_section['ctrcell'] = okeys(
-                lat = latcell.item (),
-                lon = loncell.item (),
+            dest_section["ctrcell"] = okeys(
+                lat=latcell.item(),
+                lon=loncell.item(),
             )
 
         if im.bmaj is not None:
-            dest_section['beam'] = okeys(
-                major = im.bmaj,
-                minor = im.bmin,
-                posang = im.bpa,
+            dest_section["beam"] = okeys(
+                major=im.bmaj,
+                minor=im.bmin,
+                posang=im.bpa,
             )
 
             if latcell is not None:
-                bmrad2 = 2 * np.pi * im.bmaj * im.bmin / (8 * np.log (2))
+                bmrad2 = 2 * np.pi * im.bmaj * im.bmin / (8 * np.log(2))
                 cellrad2 = latcell * loncell
-                dest_section['ctrbmvol'] = np.abs (bmrad2 / cellrad2).item ()
+                dest_section["ctrbmvol"] = np.abs(bmrad2 / cellrad2).item()
 
         if im.units is not None:
-            dest_section['units'] = im.units
+            dest_section["units"] = im.units
 
         if args.dest is None:
             import sys
-            ruamel_yaml.dump (toplevel, stream=sys.stdout, Dumper=ruamel_yaml.RoundTripDumper)
-        else:
-            with Path (args.dest).open ('wt') as f:
-                ruamel_yaml.dump (toplevel, stream=f, Dumper=ruamel_yaml.RoundTripDumper)
-
 
+            ruamel_yaml.dump(
+                toplevel, stream=sys.stdout, Dumper=ruamel_yaml.RoundTripDumper
+            )
+        else:
+            with Path(args.dest).open("wt") as f:
+                ruamel_yaml.dump(toplevel, stream=f, Dumper=ruamel_yaml.RoundTripDumper)
 
-class SetrectCommand (multitool.Command):
-    name = 'setrect'
-    argspec = '<image> <x> <y> <halfwidth> <value>'
-    summary = 'Set a rectangle in an image to a constant.'
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 5:
-            raise multitool.UsageError ('expected exactly 5 arguments')
+class SetrectCommand(multitool.Command):
+    name = "setrect"
+    argspec = "<image> <x> <y> <halfwidth> <value>"
+    summary = "Set a rectangle in an image to a constant."
+
+    def invoke(self, args, **kwargs):
+        if len(args) != 5:
+            raise multitool.UsageError("expected exactly 5 arguments")
 
         path = args[0]
 
         try:
-            x = int (args[1])
-            y = int (args[2])
-            halfwidth = int (args[3])
-            value = float (args[4])
+            x = int(args[1])
+            y = int(args[2])
+            halfwidth = int(args[3])
+            value = float(args[4])
         except ValueError:
-            raise multitool.UsageError ('could not parse one of the numeric arguments')
+            raise multitool.UsageError("could not parse one of the numeric arguments")
 
         try:
-            img = astimage.open (path, 'rw', eat_warnings=True)
+            img = astimage.open(path, "rw", eat_warnings=True)
         except Exception as e:
-            die ('can\'t open path “%s”: %s', path, e)
+            die("can't open path “%s”: %s", path, e)
 
-        data = img.read ()
-        data[...,y-halfwidth:y+halfwidth,x-halfwidth:x+halfwidth] = value
-        img.write (data)
+        data = img.read()
+        data[..., y - halfwidth : y + halfwidth, x - halfwidth : x + halfwidth] = value
+        img.write(data)
 
 
-class ShowCommand (multitool.Command):
-    name = 'show'
-    argspec = '[--no-coords] [-f] <image> [images...]'
-    summary = 'Show images interactively.'
+class ShowCommand(multitool.Command):
+    name = "show"
+    argspec = "[--no-coords] [-f] <image> [images...]"
+    summary = "Show images interactively."
     more_help = """--no-coords - Do not show coordinates even if available
 -f          - Show the 2D FFT of the image
 
 WCS support isn't fantastic and sometimes causes crashes."""
 
-    def invoke (self, args, **kwargs):
+    def invoke(self, args, **kwargs):
         anyfailures = False
-        ndshow = load_ndshow ()
+        ndshow = load_ndshow()
 
-        fft = pop_option ('f', args)
-        no_coords = pop_option ('no-coords', args)
+        fft = pop_option("f", args)
+        no_coords = pop_option("no-coords", args)
 
         for path in args:
             try:
-                img = astimage.open (path, 'r', eat_warnings=True)
+                img = astimage.open(path, "r", eat_warnings=True)
             except Exception as e:
-                print ('imtool show: can\'t open path “%s”: %s' % (path, e), file=sys.stderr)
+                print(
+                    "imtool show: can't open path “%s”: %s" % (path, e), file=sys.stderr
+                )
                 anyfailures = True
                 continue
 
             try:
-                img = img.simple ()
+                img = img.simple()
             except Exception as e:
-                print ('imtool show: can\'t convert “%s” to simple 2D sky image; taking '
-                       ' first plane' % path, file=sys.stderr)
-                data = img.read (flip=True)[tuple(np.zeros (img.shape.size - 2, dtype=int))]
+                print(
+                    "imtool show: can't convert “%s” to simple 2D sky image; taking "
+                    " first plane" % path,
+                    file=sys.stderr,
+                )
+                data = img.read(flip=True)[
+                    tuple(np.zeros(img.shape.size - 2, dtype=int))
+                ]
                 toworld = None
             else:
-                data = img.read (flip=True)
+                data = img.read(flip=True)
                 toworld = img.toworld
 
             if fft:
                 from numpy.fft import ifftshift, fft2, fftshift
-                data = np.abs (ifftshift (fft2 (fftshift (data.filled (0)))))
-                data = np.ma.MaskedArray (data)
+
+                data = np.abs(ifftshift(fft2(fftshift(data.filled(0)))))
+                data = np.ma.MaskedArray(data)
                 toworld = None
 
             if no_coords:
                 toworld = None
 
-            ndshow.view (data, title=path + ' — Array Viewer',
-                         toworld=toworld, yflip=True)
+            ndshow.view(
+                data, title=path + " — Array Viewer", toworld=toworld, yflip=True
+            )
 
-        sys.exit (int (anyfailures))
+        sys.exit(int(anyfailures))
 
 
-class StatsCommand (multitool.Command):
-    name = 'stats'
-    argspec = '<images...>'
-    summary = 'Compute and print statistics of a 64×64 patch at image center.'
+class StatsCommand(multitool.Command):
+    name = "stats"
+    argspec = "<images...>"
+    summary = "Compute and print statistics of a 64×64 patch at image center."
 
-    def _print (self, path):
+    def _print(self, path):
         try:
-            img = astimage.open (path, 'r', eat_warnings=True)
+            img = astimage.open(path, "r", eat_warnings=True)
         except Exception as e:
-            die ('error: can\'t open "%s": %s', path, e)
+            die('error: can\'t open "%s": %s', path, e)
 
         try:
-            img = img.simple ()
+            img = img.simple()
         except Exception as e:
-            print ('imstats: can\'t convert “%s” to simple 2D sky image; '
-                   'taking first plane' % path, file=sys.stderr)
-            data = img.read ()[tuple (np.zeros (img.shape.size - 2))]
+            print(
+                "imstats: can't convert “%s” to simple 2D sky image; "
+                "taking first plane" % path,
+                file=sys.stderr,
+            )
+            data = img.read()[tuple(np.zeros(img.shape.size - 2))]
         else:
-            data = img.read ()
+            data = img.read()
 
         h, w = data.shape
         patchhalfsize = 32
 
-        p = data[h//2 - patchhalfsize:h//2 + patchhalfsize,
-                 w//2 - patchhalfsize:w//2 + patchhalfsize]
+        p = data[
+            h // 2 - patchhalfsize : h // 2 + patchhalfsize,
+            w // 2 - patchhalfsize : w // 2 + patchhalfsize,
+        ]
+
+        mx = p.max()
+        mn = p.min()
+        med = np.median(p)
+        rms = np.sqrt((p**2).mean())
 
-        mx = p.max ()
-        mn = p.min ()
-        med = np.median (p)
-        rms = np.sqrt ((p**2).mean ())
-
-        sc = max (abs (mx), abs (mn))
+        sc = max(abs(mx), abs(mn))
         if sc <= 0:
             expt = 0
         else:
-            expt = 3 * (int (np.floor (np.log10 (sc))) // 3)
+            expt = 3 * (int(np.floor(np.log10(sc))) // 3)
         f = 10**-expt
 
-        print ('min  = %.2f * 10^%d' % (f * mn, expt))
-        print ('max  = %.2f * 10^%d' % (f * mx, expt))
-        print ('med  = %.2f * 10^%d' % (f * med, expt))
-        print ('rms  = %.2f * 10^%d' % (f * rms, expt))
-
-    def invoke (self, args, **kwargs):
-        if len (args) == 1:
-            self._print (args[0])
+        print("min  = %.2f * 10^%d" % (f * mn, expt))
+        print("max  = %.2f * 10^%d" % (f * mx, expt))
+        print("med  = %.2f * 10^%d" % (f * med, expt))
+        print("rms  = %.2f * 10^%d" % (f * rms, expt))
+
+    def invoke(self, args, **kwargs):
+        if len(args) == 1:
+            self._print(args[0])
         else:
-            for i, path in enumerate (args):
+            for i, path in enumerate(args):
                 if i > 0:
-                    print ()
-                print ('path =', path)
-                self._print (path)
+                    print()
+                print("path =", path)
+                self._print(path)
 
 
 # The driver.
 
 from .multitool import HelpCommand
 
-class Imtool (multitool.Multitool):
-    cli_name = 'imtool'
-    summary = 'Perform miscellaneous tasks with astronomical images.'
 
-def commandline ():
-    multitool.invoke_tool (globals ())
+class Imtool(multitool.Multitool):
+    cli_name = "imtool"
+    summary = "Perform miscellaneous tasks with astronomical images."
+
+
+def commandline():
+    multitool.invoke_tool(globals())
```

### Comparing `pwkit-1.1.1/pwkit/cli/latexdriver.py` & `pwkit-1.2.0/pwkit/cli/latexdriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,45 +7,45 @@
 This used to be a nice little shell script, but for portability it's better to
 do this in Python. And now we can optionally provide some BibTeX-related
 magic.
 
 """
 from __future__ import absolute_import, division, print_function
 
-__all__ = 'commandline'.split()
+__all__ = "commandline".split()
 
-import signal, six, subprocess, sys
-from six.moves import range
+import signal, subprocess, sys
 
 from .. import PKError
 from ..io import Path
 from . import *
 
 
 # This batch of code implements the magic BibTeX merging feature.
 
+
 def cited_names_from_aux_file(stream):
     """Parse a LaTeX ".aux" file and generate a list of names cited according to
     LaTeX ``\\citation`` commands. Repeated names are generated only once. The
     argument should be a opened I/O stream.
 
     """
     cited = set()
 
     for line in stream:
-        if not line.startswith(r'\citation{'):
+        if not line.startswith(r"\citation{"):
             continue
 
         line = line.rstrip()
-        if line[-1] != '}':
-            continue # should issue a warning or something
+        if line[-1] != "}":
+            continue  # should issue a warning or something
 
         entries = line[10:-1]
 
-        for name in entries.split(','):
+        for name in entries.split(","):
             name = name.strip()
 
             if name not in cited:
                 yield name
                 cited.add(name)
 
 
@@ -66,35 +66,38 @@
     for ed in extradicts:
         allrecords.update(ed)
 
     allrecords.update(maindict)
 
     missing = []
     from collections import OrderedDict
+
     records = OrderedDict()
     from itertools import chain
-    wantednames = sorted(chain(citednames, six.viewkeys(maindict)))
+
+    wantednames = sorted(chain(citednames, maindict.keys()))
 
     for name in wantednames:
         rec = allrecords.get(name)
         if rec is None:
             missing.append(name)
         else:
             records[name] = rec
 
     if len(missing) and not allow_missing:
         # TODO: custom exception so caller can actually see what's missing;
         # could conceivably stub out missing records or something.
-        raise PKError('missing BibTeX records: %s', ' '.join(missing))
+        raise PKError("missing BibTeX records: %s", " ".join(missing))
 
     return records
 
 
 def get_bibtex_dict(stream):
     from bibtexparser.bparser import BibTexParser
+
     parser = BibTexParser()
     parser.ignore_nonstandard_types = False
     parser.homogenise_fields = False
 
     # TODO: one bit of homogenization that might be nice: it seems that
     # newlines get preserved, in `author` records at least. Those should be
     # replaced with spaces (and multiple spaces collapsed if needed).
@@ -107,27 +110,29 @@
     writes it out in one go. I'm sure it will always all fit in RAM but some
     things just will not stand.
 
     """
     from bibtexparser.bwriter import BibTexWriter
 
     writer = BibTexWriter()
-    writer.indent = '  '
-    writer.entry_separator = ''
+    writer.indent = "  "
+    writer.entry_separator = ""
     first = True
 
     for rec in entries:
         if first:
             first = False
         else:
-            stream.write(b'\n')
-        stream.write(writer._entry_to_bibtex(rec).encode('utf8'))
+            stream.write(b"\n")
+        stream.write(writer._entry_to_bibtex(rec).encode("utf8"))
 
 
-def merge_bibtex_with_aux(auxpath, mainpath, extradir, parse=get_bibtex_dict, allow_missing=False):
+def merge_bibtex_with_aux(
+    auxpath, mainpath, extradir, parse=get_bibtex_dict, allow_missing=False
+):
     """Merge multiple BibTeX files into a single homogeneously-formatted output,
     using a LaTeX .aux file to know which records are worth paying attention
     to.
 
     The file identified by `mainpath` will be overwritten with the new .bib
     contents. This function is intended to be used in a version-control
     context.
@@ -137,80 +142,84 @@
     `mainpath` always take precedence.
 
     """
     auxpath = Path(auxpath)
     mainpath = Path(mainpath)
     extradir = Path(extradir)
 
-    with auxpath.open('rt') as aux:
+    with auxpath.open("rt") as aux:
         citednames = sorted(cited_names_from_aux_file(aux))
 
-    main = mainpath.try_open(mode='rt')
+    main = mainpath.try_open(mode="rt")
     if main is None:
         maindict = {}
     else:
         maindict = parse(main)
         main.close()
 
     def gen_extra_dicts():
         # If extradir does not exist, Path.glob() will return an empty list,
         # which seems acceptable to me.
-        for item in sorted(extradir.glob('*.bib')):
-            with item.open('rt') as extra:
+        for item in sorted(extradir.glob("*.bib")):
+            with item.open("rt") as extra:
                 yield parse(extra)
 
-    merged = merge_bibtex_collections(citednames, maindict, gen_extra_dicts(),
-                                      allow_missing=allow_missing)
+    merged = merge_bibtex_collections(
+        citednames, maindict, gen_extra_dicts(), allow_missing=allow_missing
+    )
 
-    with mainpath.make_tempfile(want='handle', resolution='overwrite') as newbib:
-        write_bibtex_dict(newbib, six.viewvalues(merged))
+    with mainpath.make_tempfile(want="handle", resolution="overwrite") as newbib:
+        write_bibtex_dict(newbib, merged.values())
 
 
 # This batch of code implements the filename-recorder-to-Makefile magic.
 
-def convert_fls_to_makefile(flspath, finalpath, prefix, replacement, work, mfpath, foreign_deps_ok):
+
+def convert_fls_to_makefile(
+    flspath, finalpath, prefix, replacement, work, mfpath, foreign_deps_ok
+):
     texpwd = None
 
-    with flspath.open('rt') as fls, mfpath.open('wt') as mf:
-        mf.write(six.text_type(finalpath))
-        mf.write(':')
+    with flspath.open("rt") as fls, mfpath.open("wt") as mf:
+        mf.write(str(finalpath))
+        mf.write(":")
 
         for line in fls:
             kind, path = line.strip().split(None, 1)
             path = Path(path)
 
-            if kind == 'PWD':
-                texpwd = path # this is always the first line
+            if kind == "PWD":
+                texpwd = path  # this is always the first line
                 if prefix is not None:
-                    r_prefix = six.text_type((texpwd / prefix).resolve())
-                r_work = six.text_type((texpwd / work).resolve())
+                    r_prefix = str((texpwd / prefix).resolve())
+                r_work = str((texpwd / work).resolve())
 
-            if kind != 'INPUT':
+            if kind != "INPUT":
                 continue
 
             # properly handles absolute and relative `path`:
-            r_full = six.text_type((texpwd / path).resolve())
+            r_full = str((texpwd / path).resolve())
 
             if r_full.startswith(r_work):
-                continue # ignore .bbl, etc
+                continue  # ignore .bbl, etc
 
             if prefix is not None:
                 if r_full.startswith(r_prefix):
-                    r_full = r_full[len(r_prefix) + 1:]
+                    r_full = r_full[len(r_prefix) + 1 :]
 
                     if replacement is not None:
                         r_full = replacement + r_full
                 elif not foreign_deps_ok:
-                    warn('unexpected dependent file path %r' % r_full)
+                    warn("unexpected dependent file path %r" % r_full)
                     continue
 
-            mf.write(' ')
+            mf.write(" ")
             mf.write(r_full)
 
-        mf.write('\n')
+        mf.write("\n")
 
 
 # The actual command-line program
 
 usage = """latexdriver [-lAxbBRq] [-eSTYLE] [-ESTYLE] [-M<args>] input.tex output.pdf
 
 Drive (xe)latex sensibly. Create output.pdf from input.tex, rerunning as
@@ -230,274 +239,298 @@
 -f      - Allow "foreign" dependencies from the '-recorder' option that do not
           begin with the PREFIX given to the '-M' option.
 -R      - Be reckless and ignore errors from tools.
 -q      - Be quiet and avoid printing anything on success.
 
 """
 
-default_args = ['-interaction', 'nonstopmode',
-                '-halt-on-error',
-                '-file-line-error']
+default_args = ["-interaction", "nonstopmode", "-halt-on-error", "-file-line-error"]
 
 max_iterations = 10
 
 
 def logrun(command, boring_args, interesting_arg, logpath, quiet=False, reckless=False):
     if not quiet:
         if len(boring_args):
-            print('+', command, '...', interesting_arg)
+            print("+", command, "...", interesting_arg)
         else:
-            print('+', command, interesting_arg)
+            print("+", command, interesting_arg)
 
     argv = [command] + boring_args + [interesting_arg]
 
     try:
-        with logpath.open('wb') as f:
-            print('## running:', ' '.join(argv), file=f)
+        with logpath.open("wb") as f:
+            print("## running:", " ".join(argv), file=f)
             f.flush()
             subprocess.check_call(argv, stdout=f, stderr=f)
     except subprocess.CalledProcessError as e:
         if quiet:
-            print('ran:', ' '.join(argv), file=sys.stderr)
+            print("ran:", " ".join(argv), file=sys.stderr)
 
-        with logpath.open('rt') as f:
+        with logpath.open("rt") as f:
             for line in f:
-                print(line, end='', file=sys.stderr)
+                print(line, end="", file=sys.stderr)
         print(file=sys.stderr)
 
         if e.returncode == -signal.SIGINT:
-            raise KeyboardInterrupt() # make sure to propagate SIGINT
+            raise KeyboardInterrupt()  # make sure to propagate SIGINT
 
         if e.returncode > 0:
-            msg = 'command "%s" failed with exit status %d' % (' '.join(argv),
-                                                               e.returncode)
+            msg = 'command "%s" failed with exit status %d' % (
+                " ".join(argv),
+                e.returncode,
+            )
         else:
-            msg = 'command "%s" killed by signal %d' % (' '.join(argv),
-                                                        -e.returncode)
+            msg = 'command "%s" killed by signal %d' % (" ".join(argv), -e.returncode)
 
         if reckless:
-            warn(msg + '; ignoring')
+            warn(msg + "; ignoring")
         else:
             die(msg)
     except Exception:
         if quiet:
-            print('ran:', ' '.join(argv), file=sys.stderr)
+            print("ran:", " ".join(argv), file=sys.stderr)
         raise
 
 
-def bib_export(style, auxpath, bibpath, no_tool_ok=False, quiet=False, ignore_missing=False):
-    args = ['bib', 'btexport']
+def bib_export(
+    style, auxpath, bibpath, no_tool_ok=False, quiet=False, ignore_missing=False
+):
+    args = ["bib", "btexport"]
     if ignore_missing:
-        args += ['-i']
+        args += ["-i"]
     args += [style, str(auxpath)]
 
     if not quiet:
-        print('+', ' '.join(args), '>' + str(bibpath))
+        print("+", " ".join(args), ">" + str(bibpath))
 
     try:
-        with bibpath.open('wb') as f:
+        with bibpath.open("wb") as f:
             subprocess.check_call(args, stdout=f)
     except OSError as e:
         if e.errno == 2 and no_tool_ok:
             bibpath.try_unlink()
             return
         if quiet:
-            print('ran:', ' '.join(args), file=sys.stderr)
+            print("ran:", " ".join(args), file=sys.stderr)
         raise
     except subprocess.CalledProcessError as e:
         if quiet:
-            print('ran:', ' '.join(args), file=sys.stderr)
+            print("ran:", " ".join(args), file=sys.stderr)
         if e.returncode > 0:
-            die('command "%s >%s" failed with exit status %d',
-                ' '.join(args), bibpath, e.returncode)
+            die(
+                'command "%s >%s" failed with exit status %d',
+                " ".join(args),
+                bibpath,
+                e.returncode,
+            )
         elif e.returncode == -signal.SIGINT:
-            raise KeyboardInterrupt() # make sure to propagate SIGINT
+            raise KeyboardInterrupt()  # make sure to propagate SIGINT
         else:
-            die('command "%s >%s" killed by signal %d',
-                ' '.join(args), bibpath, -e.returncode)
+            die(
+                'command "%s >%s" killed by signal %d',
+                " ".join(args),
+                bibpath,
+                -e.returncode,
+            )
 
 
 def just_smart_bibtools(bib_style, aux, bib):
     """Tectonic has taken over most of the features that this tool used to provide,
     but here's a hack to keep my smart .bib file generation working.
 
     """
-    extradir = Path('.bibtex')
+    extradir = Path(".bibtex")
     extradir.ensure_dir(parents=True)
 
-    bib_export(bib_style, aux, extradir / 'ZZ_bibtools.bib',
-               no_tool_ok=True, quiet=True, ignore_missing=True)
+    bib_export(
+        bib_style,
+        aux,
+        extradir / "ZZ_bibtools.bib",
+        no_tool_ok=True,
+        quiet=True,
+        ignore_missing=True,
+    )
     merge_bibtex_with_aux(aux, bib, extradir)
 
 
 def commandline(argv=None):
     if argv is None:
         argv = sys.argv
         propagate_sigint()
         unicode_stdio()
 
-    check_usage(usage, argv, usageifnoargs='long')
+    check_usage(usage, argv, usageifnoargs="long")
 
     bib_style = None
     makefile_prefix = None
     makefile_replacement = None
     makefile_dest = None
     engine_args = default_args
-    engine = 'pdflatex'
+    engine = "pdflatex"
 
     # Hooray hack
 
-    if argv[1] == '--just-smart-bibtools':
+    if argv[1] == "--just-smart-bibtools":
         if len(argv) == 4:
             bib_style = argv[2]
             auxpath = argv[3]
-            assert auxpath.endswith('.aux')
-            bibpath = auxpath[:-4] + '.bib'
+            assert auxpath.endswith(".aux")
+            bibpath = auxpath[:-4] + ".bib"
         elif len(argv) == 5:
             bib_style = argv[2]
             auxpath = argv[3]
             bibpath = argv[4]
         else:
-            die('--just-smart-bibtools expects exactly 2 or 3 additional arguments')
+            die("--just-smart-bibtools expects exactly 2 or 3 additional arguments")
         just_smart_bibtools(bib_style, auxpath, bibpath)
         return
 
     # I should probably start using a real arg parser.
 
-    do_bibtex = pop_option('b', argv)
-    do_smart_bibtex = pop_option('B', argv)
-    do_xetex = pop_option('x', argv)
-    do_letterpaper = pop_option('l', argv)
-    do_a4paper = pop_option('A', argv)
-    do_reckless = pop_option('R', argv)
-    do_foreign_deps = pop_option('f', argv)
-    quiet = pop_option('q', argv)
+    do_bibtex = pop_option("b", argv)
+    do_smart_bibtex = pop_option("B", argv)
+    do_xetex = pop_option("x", argv)
+    do_letterpaper = pop_option("l", argv)
+    do_a4paper = pop_option("A", argv)
+    do_reckless = pop_option("R", argv)
+    do_foreign_deps = pop_option("f", argv)
+    quiet = pop_option("q", argv)
     do_smart_bibtools = False
 
     for i in range(1, len(argv)):
-        if argv[i].startswith('-e') or argv[i].startswith('-E'):
-            do_smart_bibtools = argv[i].startswith('-E')
+        if argv[i].startswith("-e") or argv[i].startswith("-E"):
+            do_smart_bibtools = argv[i].startswith("-E")
             bib_style = argv[i][2:]
             del argv[i]
             break
 
     for i in range(1, len(argv)):
-        if argv[i].startswith('-M'):
-            pieces = argv[i][2:].split(',', 2)
+        if argv[i].startswith("-M"):
+            pieces = argv[i][2:].split(",", 2)
             if len(pieces) == 2:
                 makefile_prefix, makefile_dest = pieces
             elif len(pieces) == 3:
                 makefile_prefix, makefile_replacement, makefile_dest = pieces
             else:
-                wrong_usage(usage, 'could not parse -M argument')
+                wrong_usage(usage, "could not parse -M argument")
             del argv[i]
             break
 
     if len(argv) != 3:
-        wrong_usage(usage, 'expect exactly 2 non-option arguments')
+        wrong_usage(usage, "expect exactly 2 non-option arguments")
 
     if do_letterpaper and do_a4paper:
         wrong_usage(usage, 'only one of "-l" and "-A" may be specified')
 
     input = Path(argv[1])
     output = Path(argv[2])
 
     if do_smart_bibtools:
         do_smart_bibtex = True
     if bib_style is not None or do_smart_bibtex:
         do_bibtex = True
     if do_xetex:
-        engine = 'xelatex'
+        engine = "xelatex"
     if do_letterpaper:
-        engine_args += ['-papersize', 'letter']
+        engine_args += ["-papersize", "letter"]
     if do_a4paper:
-        engine_args += ['-papersize', 'A4']
+        engine_args += ["-papersize", "A4"]
     if makefile_dest is not None:
-        engine_args += ['-recorder']
+        engine_args += ["-recorder"]
 
     if not input.exists():
         die('input "%s" does not exist', input)
 
     base = input.stem
     if not len(base):
         die('failed to strip extension from input path "%s"', input)
 
     # I stash the annoying LaTeX output files in a hidden directory called
     # .latexwork. However, some LaTeX distributions refuse to write to hidden
     # paths by default. I figured out how to hack the configuration, but
     # that's not a scalable solution. Instead I just create a temporary
     # symlink with an acceptable name -- good jorb security.
-    workdir = input.with_name('.latexwork')
-    workalias = input.with_name('_latexwork')
+    workdir = input.with_name(".latexwork")
+    workalias = input.with_name("_latexwork")
 
     workdir.ensure_dir(parents=True)
     workalias.rellink_to(workdir, force=True)
 
     job = workalias / base
-    tlog = workalias / (base + '.hllog')
-    blog = workalias / (base + '.hlblg')
-    engine_args += ['-jobname', str(job)]
+    tlog = workalias / (base + ".hllog")
+    blog = workalias / (base + ".hlblg")
+    engine_args += ["-jobname", str(job)]
 
     try:
         logrun(engine, engine_args, base, tlog, quiet=quiet)
 
         if do_bibtex:
-            bib = input.with_suffix('.bib')
-            aux = job.with_suffix('.aux')
+            bib = input.with_suffix(".bib")
+            aux = job.with_suffix(".aux")
 
             if do_smart_bibtex:
-                extradir = input.with_name('.bibtex')
+                extradir = input.with_name(".bibtex")
 
                 if bib_style is not None:
                     extradir.ensure_dir(parents=True)
-                    bib_export(bib_style, aux, extradir / 'ZZ_bibtools.bib',
-                               no_tool_ok=True, quiet=quiet, ignore_missing=True)
+                    bib_export(
+                        bib_style,
+                        aux,
+                        extradir / "ZZ_bibtools.bib",
+                        no_tool_ok=True,
+                        quiet=quiet,
+                        ignore_missing=True,
+                    )
 
                 if not quiet:
-                    print('+', '(generate and normalize)', bib)
+                    print("+", "(generate and normalize)", bib)
                 merge_bibtex_with_aux(aux, bib, extradir)
             elif bib_style is not None:
                 bib_export(bib_style, aux, bib, quiet=quiet)
 
-            job.with_suffix('.bib').rellink_to(bib, force=True)
-            logrun('bibtex', [], str(job), blog, reckless=do_reckless, quiet=quiet)
+            job.with_suffix(".bib").rellink_to(bib, force=True)
+            logrun("bibtex", [], str(job), blog, reckless=do_reckless, quiet=quiet)
 
-            with blog.open('rt') as f:
+            with blog.open("rt") as f:
                 for line in f:
-                    if 'Warning' in line:
-                        print(line, end='', file=sys.stderr)
+                    if "Warning" in line:
+                        print(line, end="", file=sys.stderr)
 
             # force at least one extra run:
             logrun(engine, engine_args, base, tlog, quiet=quiet)
 
         for _ in range(max_iterations):
             keepgoing = False
 
             # longtables seem to always tell you to rerun latex. Stripping out
             # lines containing "longtable" makes us ignore these prompts.
-            with tlog.open('rt') as f:
+            with tlog.open("rt") as f:
                 for line in f:
-                    if 'longtable' in line:
+                    if "longtable" in line:
                         continue
-                    if 'Rerun' in line:
+                    if "Rerun" in line:
                         keepgoing = True
                         break
 
             if not keepgoing:
                 break
 
             logrun(engine, engine_args, base, tlog, quiet=quiet)
         else:
             # we didn't break out of the loop -- ie hit max_iterations
             die('too many iterations; check "%s"', tlog)
 
-        job.with_suffix('.pdf').rename(output)
+        job.with_suffix(".pdf").rename(output)
 
         if makefile_dest is not None:
-            convert_fls_to_makefile(job.with_suffix('.fls'), output,
-                                    Path(makefile_prefix),
-                                    makefile_replacement,
-                                    workalias,
-                                    Path(makefile_dest),
-                                    do_foreign_deps)
+            convert_fls_to_makefile(
+                job.with_suffix(".fls"),
+                output,
+                Path(makefile_prefix),
+                makefile_replacement,
+                workalias,
+                Path(makefile_dest),
+                do_foreign_deps,
+            )
     finally:
         workalias.unlink()
```

### Comparing `pwkit-1.1.1/pwkit/cli/multitool.py` & `pwkit-1.2.0/pwkit/cli/multitool.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,28 +43,29 @@
 
   def commandline ():
     multitool.invoke_tool (globals ())
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''invoke_tool Command DelegatingCommand HelpCommand Multitool
-                  UsageError''').split ()
+__all__ = str(
+    """invoke_tool Command DelegatingCommand HelpCommand Multitool
+                  UsageError"""
+).split()
 
-from six import itervalues
 from .. import PKError
 from . import check_usage, wrong_usage
 
 
-class UsageError (PKError):
+class UsageError(PKError):
     """Raised if illegal command-line arguments are used in a Multitool
     program."""
 
 
-class Command (object):
+class Command(object):
     """A command in a multifunctional CLI tool.
 
     For historical reasons, this class defaults to a homebrew argument parsing
     system. Use `ArgparsingCommand` for a better system based on the
     `argparse` module.
 
     Attributes:
@@ -88,60 +89,59 @@
     ``invoke(self, args, **kwargs)``
       Execute this command.
 
     'name' must be set; other attributes are optional, although at least
     'summary' and 'argspec' should be set. 'invoke()' must be implemented.
 
     """
+
     name = None
-    argspec = ''
-    summary = ''
-    more_help = ''
+    argspec = ""
+    summary = ""
+    more_help = ""
     help_if_no_args = True
 
-    def invoke (self, args, **kwargs):
+    def invoke(self, args, **kwargs):
         """Invoke this command. 'args' is a list of the remaining command-line
         arguments. 'kwargs' contains at least 'argv0', which is the equivalent
         of, well, `argv[0]` for this command; 'tool', the originating
         Multitool instance; and 'parent', the parent DelegatingCommand
         instance. Other kwargs may be added in an application-specific manner.
         Basic processing of '--help' will already have been done if invoked
         through invoke_with_usage().
 
         """
-        raise NotImplementedError ()
-
+        raise NotImplementedError()
 
-    def invoke_with_usage (self, args, **kwargs):
+    def invoke_with_usage(self, args, **kwargs):
         """Invoke the command with standardized usage-help processing. Same calling
         convention as `Command.invoke()`.
 
         """
-        argv0 = kwargs['argv0']
-        usage = self._usage (argv0)
+        argv0 = kwargs["argv0"]
+        usage = self._usage(argv0)
         argv = [argv0] + args
-        uina = 'long' if self.help_if_no_args else False
-        check_usage (usage, argv, usageifnoargs=uina)
+        uina = "long" if self.help_if_no_args else False
+        check_usage(usage, argv, usageifnoargs=uina)
 
         try:
-            return self.invoke (args, **kwargs)
+            return self.invoke(args, **kwargs)
         except UsageError as e:
-            wrong_usage (usage, str (e))
-
+            wrong_usage(usage, str(e))
 
-    def _usage (self, argv0):
-        text = '%s %s' % (argv0, self.argspec)
-        if len (self.summary):
-            text += '\n\n' + self.summary
-        if len (self.more_help):
-            text += '\n\n' + self.more_help
+    def _usage(self, argv0):
+        text = "%s %s" % (argv0, self.argspec)
+        if len(self.summary):
+            text += "\n\n" + self.summary
+        if len(self.more_help):
+            text += "\n\n" + self.more_help
         return text
 
 
-class ArgparsingCommand (Command):
+class ArgparsingCommand(Command):
     """A multifunctional CLI command that uses the "argparse" module.
 
     Attributes:
 
     name
       The command's name, as should be specified at the CLI.
     summary
@@ -155,53 +155,52 @@
     ``invoke(self, args, **kwargs)``
       Execute this command.
 
     'name' must be set; other attributes are optional. 'invoke()' must be
     implemented.
 
     """
+
     name = None
-    summary = ''
+    summary = ""
 
-    def get_arg_parser (self, **kwargs):
+    def get_arg_parser(self, **kwargs):
         """Return an instance of `argparse.ArgumentParser` used to process
         this tool's command-line arguments.
 
         """
         import argparse
-        ap = argparse.ArgumentParser (
-            prog = kwargs['argv0'],
-            description = self.summary,
+
+        ap = argparse.ArgumentParser(
+            prog=kwargs["argv0"],
+            description=self.summary,
         )
         return ap
 
-
-    def invoke_with_usage (self, args, **kwargs):
+    def invoke_with_usage(self, args, **kwargs):
         """Invoke the command with standardized usage-help processing. Same
         calling convention as `Command.invoke()`, except here *args* is an
         un-parsed list of strings.
 
         """
-        ap = self.get_arg_parser (**kwargs)
-        args = ap.parse_args (args)
-        return self.invoke (args, **kwargs)
+        ap = self.get_arg_parser(**kwargs)
+        args = ap.parse_args(args)
+        return self.invoke(args, **kwargs)
 
 
-def is_strict_subclass (value, klass):
+def is_strict_subclass(value, klass):
     """Check that `value` is a subclass of `klass` but that it is not actually
     `klass`. Unlike issubclass(), does not raise an exception if `value` is
     not a type.
 
     """
-    return (isinstance (value, type) and
-            issubclass (value, klass) and
-            value is not klass)
+    return isinstance(value, type) and issubclass(value, klass) and value is not klass
 
 
-class DelegatingCommand (Command):
+class DelegatingCommand(Command):
     """A command that delegates to sub-commands.
 
     Attributes:
 
     cmd_desc
       The noun used to desribe the sub-commands.
     usage_tmpl
@@ -212,118 +211,119 @@
 
     register
       Register a new sub-command.
     populate
       Register many sub-commands automatically.
 
     """
-    argspec = '<command> [arguments...]'
-    cmd_desc = 'sub-command'
+
+    argspec = "<command> [arguments...]"
+    cmd_desc = "sub-command"
     usage_tmpl = """%(argv0)s %(argspec)s
 
 %(summary)s
 
 Commands are:
 
 %(indented_command_help)s
 
 %(more_help)s
 """
-    more_help = 'Most commands will give help if run with no arguments.'
+    more_help = "Most commands will give help if run with no arguments."
 
-    def __init__ (self, populate_from_self=True):
+    def __init__(self, populate_from_self=True):
         self.commands = {}
 
         if populate_from_self:
             # Avoiding '_' items is important; otherwise we'll recurse
             # infinitely on self.__class__!
-            self.populate (getattr (self, n) for n in dir (self)
-                           if not n.startswith ('_'))
-
+            self.populate(getattr(self, n) for n in dir(self) if not n.startswith("_"))
 
-    def register (self, cmd):
+    def register(self, cmd):
         """Register a new command with the tool. 'cmd' is expected to be an instance
         of `Command`, although here only the `cmd.name` attribute is
         investigated. Multiple commands with the same name are not allowed to
         be registered. Returns 'self'.
 
         """
         if cmd.name is None:
-            raise ValueError ('no name set for Command object %r' % cmd)
+            raise ValueError("no name set for Command object %r" % cmd)
         if cmd.name in self.commands:
-            raise ValueError ('a command named "%s" has already been '
-                              'registered' % cmd.name)
+            raise ValueError(
+                'a command named "%s" has already been ' "registered" % cmd.name
+            )
 
         self.commands[cmd.name] = cmd
         return self
 
-
-    def populate (self, values):
+    def populate(self, values):
         """Register multiple new commands by investigating the iterable `values`. For
         each item in `values`, instances of `Command` are registered, and
         subclasses of `Command` are instantiated (with no arguments passed to
         the constructor) and registered. Other kinds of values are ignored.
         Returns 'self'.
 
         """
         for value in values:
-            if isinstance (value, Command):
-                self.register (value)
-            elif is_strict_subclass (value, Command) and getattr (value, 'name') is not None:
-                self.register (value ())
+            if isinstance(value, Command):
+                self.register(value)
+            elif (
+                is_strict_subclass(value, Command)
+                and getattr(value, "name") is not None
+            ):
+                self.register(value())
 
         return self
 
-
-    def invoke_command (self, cmd, args, **kwargs):
+    def invoke_command(self, cmd, args, **kwargs):
         """This function mainly exists to be overridden by subclasses."""
-        new_kwargs = kwargs.copy ()
-        new_kwargs['argv0'] = kwargs['argv0'] + ' ' + cmd.name
-        new_kwargs['parent'] = self
-        new_kwargs['parent_kwargs'] = kwargs
-        return cmd.invoke_with_usage (args, **new_kwargs)
-
-
-    def invoke (self, args, **kwargs):
-        if len (args) < 1:
-            raise UsageError ('need to specify a %s', self.cmd_desc)
+        new_kwargs = kwargs.copy()
+        new_kwargs["argv0"] = kwargs["argv0"] + " " + cmd.name
+        new_kwargs["parent"] = self
+        new_kwargs["parent_kwargs"] = kwargs
+        return cmd.invoke_with_usage(args, **new_kwargs)
+
+    def invoke(self, args, **kwargs):
+        if len(args) < 1:
+            raise UsageError("need to specify a %s", self.cmd_desc)
 
         cmdname = args[0]
-        cmd = self.commands.get (cmdname)
+        cmd = self.commands.get(cmdname)
         if cmd is None:
-            raise UsageError ('no such %s "%s"', self.cmd_desc, cmdname)
-
-        self.invoke_command (cmd, args[1:], **kwargs)
+            raise UsageError('no such %s "%s"', self.cmd_desc, cmdname)
 
+        self.invoke_command(cmd, args[1:], **kwargs)
 
-    def _usage (self, argv0):
-        return self.usage_tmpl % self._usage_keys (argv0)
+    def _usage(self, argv0):
+        return self.usage_tmpl % self._usage_keys(argv0)
 
-
-    def _usage_keys (self, argv0):
-        scmds = sorted ((cmd for cmd in itervalues (self.commands)
-                         if cmd.name[0] != '_'),
-                        key=lambda c: c.name)
+    def _usage_keys(self, argv0):
+        scmds = sorted(
+            (cmd for cmd in self.commands.values() if cmd.name[0] != "_"),
+            key=lambda c: c.name,
+        )
         maxlen = 0
 
         for cmd in scmds:
-            maxlen = max (maxlen, len (cmd.name))
+            maxlen = max(maxlen, len(cmd.name))
 
-        ich = '\n'.join ('  %s %-*s - %s' %
-                         (argv0, maxlen, cmd.name, cmd.summary)
-                         for cmd in scmds)
+        ich = "\n".join(
+            "  %s %-*s - %s" % (argv0, maxlen, cmd.name, cmd.summary) for cmd in scmds
+        )
 
-        return dict (argspec=self.argspec,
-                     argv0=argv0,
-                     indented_command_help=ich,
-                     more_help=self.more_help,
-                     summary=self.summary)
+        return dict(
+            argspec=self.argspec,
+            argv0=argv0,
+            indented_command_help=ich,
+            more_help=self.more_help,
+            summary=self.summary,
+        )
 
 
-class Multitool (DelegatingCommand):
+class Multitool(DelegatingCommand):
     """A command-line tool with multiple sub-commands.
 
     Attributes:
 
       cli_name  - The usual name of this tool on the command line.
       more_help - Additional help text.
       summary   - A one-line summary of this tool's functionality.
@@ -331,38 +331,37 @@
     Functions:
 
       commandline - Execute a command as if invoked from the command-line.
       register    - Register a new command.
       populate    - Register many commands automatically.
 
     """
-    cli_name = '<no name>'
-    cmd_desc = 'command'
 
-    def __init__ (self):
-        super (Multitool, self).__init__ (populate_from_self=False)
+    cli_name = "<no name>"
+    cmd_desc = "command"
 
-    def commandline (self, argv):
+    def __init__(self):
+        super(Multitool, self).__init__(populate_from_self=False)
+
+    def commandline(self, argv):
         """Run as if invoked from the command line. 'argv' is a Unix-style list of
         arguments, where the zeroth item is the program name (which is ignored
         here). Usage help is printed if deemed appropriate (e.g., no arguments
         are given). This function always terminates with an exception, with
         the exception being a SystemExit(0) in case of success.
 
         Note that we don't actually use `argv[0]` to set `argv0` because it
         will generally be the full path to the script name, which is
         unattractive.
 
         """
-        self.invoke_with_usage (argv[1:],
-                                tool=self,
-                                argv0=self.cli_name)
+        self.invoke_with_usage(argv[1:], tool=self, argv0=self.cli_name)
 
 
-def invoke_tool (namespace, tool_class=None):
+def invoke_tool(namespace, tool_class=None):
     """Invoke a tool and exit.
 
     `namespace` is a namespace-type dict from which the tool is initialized.
     It should contain exactly one value that is a `Multitool` subclass, and
     this subclass will be instantiated and populated (see
     `Multitool.populate()`) using the other items in the namespace. Instances
     and subclasses of `Command` will therefore be registered with the
@@ -381,37 +380,38 @@
     If `tool_class` is not None, this is used as the tool class rather than
     searching `namespace`, potentially avoiding problems with modules
     containing multiple `Multitool` implementations.
 
     """
     import sys
     from .. import cli
-    cli.propagate_sigint ()
-    cli.unicode_stdio ()
-    cli.backtrace_on_usr1 ()
+
+    cli.propagate_sigint()
+    cli.unicode_stdio()
+    cli.backtrace_on_usr1()
 
     if tool_class is None:
-        for value in itervalues (namespace):
-            if is_strict_subclass (value, Multitool):
+        for value in namespace.values():
+            if is_strict_subclass(value, Multitool):
                 if tool_class is not None:
-                    raise PKError ('do not know which Multitool implementation to use')
+                    raise PKError("do not know which Multitool implementation to use")
                 tool_class = value
 
     if tool_class is None:
-        raise PKError ('no Multitool implementation to use')
+        raise PKError("no Multitool implementation to use")
 
-    tool = tool_class ()
-    tool.populate (itervalues (namespace))
-    tool.commandline (sys.argv)
+    tool = tool_class()
+    tool.populate(namespace.values())
+    tool.commandline(sys.argv)
 
 
-class HelpCommand (Command):
-    name = 'help'
-    argspec = '<command name>'
-    summary = 'Show help on other commands.'
+class HelpCommand(Command):
+    name = "help"
+    argspec = "<command name>"
+    summary = "Show help on other commands."
     help_if_no_args = False
 
-    def invoke (self, args, parent=None, parent_kwargs=None, **kwargs):
+    def invoke(self, args, parent=None, parent_kwargs=None, **kwargs):
         # This will Do The Right Thing if someone does the equivalent of "git
         # help remote show". Other than that it's kind of open to weird
         # misusage ...
-        parent.invoke_with_usage (args + ['--help'], **parent_kwargs)
+        parent.invoke_with_usage(args + ["--help"], **parent_kwargs)
```

### Comparing `pwkit-1.1.1/pwkit/cli/wrapout.py` & `pwkit-1.2.0/pwkit/cli/wrapout.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/colormaps.py` & `pwkit-1.2.0/pwkit/colormaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 """
 from __future__ import absolute_import, division, print_function
 
 __all__ = "base_factory_names factory_map".split()
 
 
-import numpy as np, six
+import numpy as np
 
 base_factory_names = (
     "moreland_bluered cubehelix_dagreen cubehelix_blue "
     "pkgw black_to_white black_to_red "
     "black_to_green black_to_blue "
     "white_to_black white_to_red "
     "white_to_green white_to_blue"
@@ -617,15 +617,15 @@
     win.show_all()
     Gtk.main()
 
 
 def printmaps():
     print("Available color maps:")
 
-    for m in sorted(six.iterkeys(factory_map)):
+    for m in sorted(factory_map.keys()):
         print("\t" + m)
 
 
 if __name__ == "__main__":
     import sys
 
     if len(sys.argv) < 2:
```

### Comparing `pwkit-1.1.1/pwkit/contours.py` & `pwkit-1.2.0/pwkit/contours.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_2mass_H.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_2mass_H.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_2mass_J.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_2mass_J.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_2mass_Ks.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_2mass_Ks.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_bessell_UX.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_bessell_UX.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_galex_fuv.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_galex_fuv.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_galex_nuv.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_galex_nuv.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_lbt_lmircam_L.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_lbt_lmircam_L.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_mearth_ccd715.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_mearth_ccd715.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_J.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_J.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_Ks.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_Ks.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_Lp.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_Lp.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_Mp.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_Mp.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_mko_h.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_mko_h.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_wise_1.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_wise_1.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_wise_2.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_wise_2.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_wise_3.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_wise_3.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/filter_wise_4.dat` & `pwkit-1.2.0/pwkit/data/bandpasses/filter_wise_4.dat`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/sdss3_filter_responses.fits` & `pwkit-1.2.0/pwkit/data/bandpasses/sdss3_filter_responses.fits`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data/bandpasses/swuw1_20041120v106.arf` & `pwkit-1.2.0/pwkit/data/bandpasses/swuw1_20041120v106.arf`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/data_gui_helpers.py` & `pwkit-1.2.0/pwkit/data_gui_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,58 +14,55 @@
 
 data_to_argb32       - Turn arbitrary data values into ARGB32 colors.
 data_to_imagesurface - Turn arbitrary data values into a Cairo ImageSurface.
 
 """
 from __future__ import absolute_import, division, print_function
 
-__all__ = '''
+__all__ = """
 data_to_argb32
 data_to_imagesurface
 Clipper
 ColorMapper
 LazyComputer
-Stretcher'''.split()
+Stretcher""".split()
 
 import numpy as np
-from six.moves import range
 
 from . import colormaps
 
 
 DEFAULT_TILESIZE = 128
 
+
 class LazyComputer(object):
     buffer = None
     tilesize = None
     valid = None
 
     def set_buffer(self, buffer):
         self.buffer = buffer
         return self
 
-
     def alloc_buffer(self, template):
         if np.ma.is_masked(template):
             self.buffer = np.ma.empty(template.shape)
             self.buffer.mask = template.mask
         else:
             self.buffer = np.empty(template.shape)
         return self
 
-
     def set_tile_size(self, tilesize=DEFAULT_TILESIZE):
         self.tilesize = tilesize
         h, w = self.buffer.shape
         nxt = (w + tilesize - 1) // tilesize
         nyt = (h + tilesize - 1) // tilesize
         self.valid = np.zeros((nyt, nxt))
         return self
 
-
     def ensure_region_updated(self, data, xoffset, yoffset, width, height):
         ts = self.tilesize
         buf = self.buffer
         valid = self.valid
         func = self._make_func(np.ma.is_masked(data))
 
         tilej = xoffset // ts
@@ -77,31 +74,31 @@
         pyofs = tilei * ts
 
         for i in range(nyt):
             txofs = tilej
             pxofs = tilej * ts
 
             for j in range(nxt):
-                if not valid[tyofs,txofs]:
-                    func(data[pyofs:pyofs+ts,pxofs:pxofs+ts],
-                         buf[pyofs:pyofs+ts,pxofs:pxofs+ts])
-                    valid[tyofs,txofs] = 1
+                if not valid[tyofs, txofs]:
+                    func(
+                        data[pyofs : pyofs + ts, pxofs : pxofs + ts],
+                        buf[pyofs : pyofs + ts, pxofs : pxofs + ts],
+                    )
+                    valid[tyofs, txofs] = 1
 
                 pxofs += ts
                 txofs += 1
             pyofs += ts
             tyofs += 1
 
         return self
 
-
     def ensure_all_updated(self, data):
         return self.ensure_region_updated(data, 0, 0, data.shape[1], data.shape[0])
 
-
     def invalidate(self):
         self.valid.fill(0)
         return self
 
 
 class Clipper(LazyComputer):
     dmin = None
@@ -115,30 +112,32 @@
         if not np.isfinite(dmax):
             dmax = data[np.ma.where(np.isfinite(data))].max()
 
         self.dmin = dmin
         self.dmax = dmax
         return self
 
-
     def _make_func(self, ismasked):
         dmin = self.dmin
-        scale = 1. / (self.dmax - dmin)
+        scale = 1.0 / (self.dmax - dmin)
 
         if ismasked:
+
             def func(src, dest):
                 # As of Numpy 1.13, the `mask` parameter gets turned into a
                 # scalar of we operate on the full MaskedArray object (e.g.,
                 # `dest` not `dest.data`), which causes the vector mask
                 # assignment to fail.
                 np.subtract(src, dmin, dest.data)
                 np.multiply(dest.data, scale, dest.data)
                 np.clip(dest.data, 0, 1, dest.data)
                 dest.mask[...] = src.mask
+
         else:
+
             def func(src, dest):
                 np.subtract(src, dmin, dest)
                 np.multiply(dest, scale, dest)
                 np.clip(dest, 0, 1, dest)
 
         return func
 
@@ -154,90 +153,90 @@
 
     def offset_cbrt(src, dest):
         """This stretch is useful when you have values that are symmetrical around
         zero, and you want to enhance contrasts at small values while
         preserving sign.
 
         """
-        np.subtract(src, 0.5, out=dest) # [0, 1] -> [-0.5, 0.5]
-        np.multiply(dest, 2, out=dest) # [-0.5, 0.5] => [-1, 1]
-        np.cbrt(dest, out=dest) # domain remains same
-        np.multiply(dest, 0.5, out=dest) # [-1, 1] => [-0.5, 0.5]
-        np.add(dest, 0.5, out=dest) # [-0.5, 0.5] => [0, 1]
+        np.subtract(src, 0.5, out=dest)  # [0, 1] -> [-0.5, 0.5]
+        np.multiply(dest, 2, out=dest)  # [-0.5, 0.5] => [-1, 1]
+        np.cbrt(dest, out=dest)  # domain remains same
+        np.multiply(dest, 0.5, out=dest)  # [-1, 1] => [-0.5, 0.5]
+        np.add(dest, 0.5, out=dest)  # [-0.5, 0.5] => [0, 1]
 
     modes = {
-        'linear': passthrough,
-        'offset_cbrt': offset_cbrt,
-        'sqrt': np.sqrt,
-        'square': np.square,
+        "linear": passthrough,
+        "offset_cbrt": offset_cbrt,
+        "sqrt": np.sqrt,
+        "square": np.square,
     }
 
     def __init__(self, mode):
         if mode not in self.modes:
-            raise ValueError('unrecognized Stretcher mode %r', mode)
+            raise ValueError("unrecognized Stretcher mode %r", mode)
 
         self.mode = mode
 
     def _make_func(self, ismasked):
         return self.modes[self.mode]
 
 
 class ColorMapper(LazyComputer):
     mapper = None
 
     def __init__(self, mapname):
         if mapname is not None:
             self.mapper = colormaps.factory_map[mapname]()
 
-
     def alloc_buffer(self, template):
         self.buffer = np.empty(template.shape, dtype=np.uint32)
         self.buffer.fill(0xFF000000)
         return self
 
-
     def _make_func(self, ismasked):
         mapper = self.mapper
 
         if not ismasked:
+
             def func(src, dest):
                 mapped = mapper(src)
                 dest.fill(0xFF000000)
-                effscratch = (mapped[:,:,0] * 0xFF).astype(np.uint32)
+                effscratch = (mapped[:, :, 0] * 0xFF).astype(np.uint32)
                 np.left_shift(effscratch, 16, effscratch)
                 np.bitwise_or(dest, effscratch, dest)
-                effscratch = (mapped[:,:,1] * 0xFF).astype(np.uint32)
+                effscratch = (mapped[:, :, 1] * 0xFF).astype(np.uint32)
                 np.left_shift(effscratch, 8, effscratch)
                 np.bitwise_or(dest, effscratch, dest)
-                effscratch = (mapped[:,:,2] * 0xFF).astype(np.uint32)
+                effscratch = (mapped[:, :, 2] * 0xFF).astype(np.uint32)
                 np.bitwise_or(dest, effscratch, dest)
+
         else:
             scratch2 = np.zeros((self.tilesize, self.tilesize), dtype=np.uint32)
 
             def func(src, dest):
-                effscratch2 = scratch2[:dest.shape[0],:dest.shape[1]]
+                effscratch2 = scratch2[: dest.shape[0], : dest.shape[1]]
                 mapped = mapper(src)
 
                 dest.fill(0xFF000000)
-                effscratch = (mapped[:,:,0] * 0xFF).astype(np.uint32)
+                effscratch = (mapped[:, :, 0] * 0xFF).astype(np.uint32)
                 np.left_shift(effscratch, 16, effscratch)
                 np.bitwise_or(dest, effscratch, dest)
-                effscratch = (mapped[:,:,1] * 0xFF).astype(np.uint32)
+                effscratch = (mapped[:, :, 1] * 0xFF).astype(np.uint32)
                 np.left_shift(effscratch, 8, effscratch)
                 np.bitwise_or(dest, effscratch, dest)
-                effscratch = (mapped[:,:,2] * 0xFF).astype(np.uint32)
+                effscratch = (mapped[:, :, 2] * 0xFF).astype(np.uint32)
                 np.bitwise_or(dest, effscratch, dest)
 
                 np.invert(src.mask, effscratch2)
                 np.multiply(dest, effscratch2, dest)
 
         return func
 
 
-def data_to_argb32(data, cmin=None, cmax=None, stretch='linear', cmap='black_to_blue'):
+def data_to_argb32(data, cmin=None, cmax=None, stretch="linear", cmap="black_to_blue"):
     """Turn arbitrary data values into ARGB32 colors.
 
     There are three steps to this process: clipping the data values to a
     maximum and minimum; stretching the spacing between those values; and
     converting their amplitudes into colors with some kind of color map.
 
     `data`    - Input data; can (and should) be a MaskedArray if some values are
@@ -291,20 +290,19 @@
     way to quickly visualize 2D data.
 
     """
     import cairo
 
     data = np.atleast_2d(data)
     if data.ndim != 2:
-        raise ValueError('input array may not have more than 2 dimensions')
+        raise ValueError("input array may not have more than 2 dimensions")
 
     argb32 = data_to_argb32(data, **kwargs)
 
     format = cairo.FORMAT_ARGB32
     height, width = argb32.shape
     stride = cairo.ImageSurface.format_stride_for_width(format, width)
 
     if argb32.strides[0] != stride:
-        raise ValueError('stride of data array not compatible with ARGB32')
+        raise ValueError("stride of data array not compatible with ARGB32")
 
-    return cairo.ImageSurface.create_for_data(argb32, format,
-                                              width, height, stride)
+    return cairo.ImageSurface.create_for_data(argb32, format, width, height, stride)
```

### Comparing `pwkit-1.1.1/pwkit/dulk_models.py` & `pwkit-1.2.0/pwkit/dulk_models.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/ellipses.py` & `pwkit-1.2.0/pwkit/ellipses.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/__init__.py` & `pwkit-1.2.0/pwkit/environments/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from __future__ import absolute_import, division, print_function
 
 """For reference: the Python docs state that Python automatically decodes
 Unicode environment variables as UTF-8 on non-Windows, so we don't need to be
 crazy about bytes-ifying values.
 
 """
-__all__ = 'Environment prepend_environ_path prepend_path user_data_path'.split()
+__all__ = "Environment prepend_environ_path prepend_path user_data_path".split()
 
 import os, subprocess, sys
 
 from .. import cli
 from ..cli import multitool
 
 
@@ -45,51 +45,70 @@
         """Modify the passed-in dictionary of environment variables to be suitable for
         executing programs in this software environment. Make sure to copy
         os.environ() if you don't want to modify it for the current process.
 
         """
         raise NotImplementedError()
 
-
     def _preexec(self, env, **kwargs):
         pass
 
-
-    def launch(self, argv, stdin=None, stdout=None, stderr=None,
-               close_fds=False, env=None, shell=False, cwd=None,
-               preexec_fn=None, executable=None, **kwargs):
+    def launch(
+        self,
+        argv,
+        stdin=None,
+        stdout=None,
+        stderr=None,
+        close_fds=False,
+        env=None,
+        shell=False,
+        cwd=None,
+        preexec_fn=None,
+        executable=None,
+        **kwargs
+    ):
         if env is None:
             env = os.environ
 
         env = self.modify_environment(env.copy())
         self._preexec(env, **kwargs)
-        return subprocess.Popen(argv, stdin=stdin, stdout=stdout,
-                                stderr=stderr, close_fds=close_fds,
-                                env=env, shell=shell, cwd=cwd,
-                                preexec_fn=preexec_fn, executable=executable)
+        return subprocess.Popen(
+            argv,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+            close_fds=close_fds,
+            env=env,
+            shell=shell,
+            cwd=cwd,
+            preexec_fn=preexec_fn,
+            executable=executable,
+        )
 
     def execvpe(self, argv, env=None, **kwargs):
         if env is None:
             env = os.environ
 
         env = self.modify_environment(env.copy())
         self._preexec(env, **kwargs)
         # unlike subprocess.Popen, execvpe doesn't use the new path to find
         # the program. But we're about to replace ourselves with the new
         # program, so no worries about mutating os.environ. If the exec fails
         # the mutation will remain, though.
-        os.environ['PATH'] = env['PATH']
+        os.environ["PATH"] = env["PATH"]
         os.execvpe(argv[0], argv, env)
 
     def slurp(self, **kwargs):
         from ..slurp import Slurper
+
         return Slurper(subproc_factory=self.launch, **kwargs)
 
     def get_wrapout_wrapper(self, **kwargs):
         from ..cli.wrapout import Wrapper
+
         w = Wrapper(**kwargs)
         w.slurp_factory = self.slurp
         return w
 
 
 def prepend_path(orig, text, pathsep=os.pathsep):
     """Returns a $PATH-like environment variable with `text` prepended. `orig` is
@@ -100,18 +119,18 @@
 
     newpath = cli.prepend_path(oldpath, '/mypackage/bin')
 
     See also `prepend_environ_path`.
 
     """
     if orig is None:
-        orig = ''
+        orig = ""
     if not len(orig):
         return text
-    return ''.join([text, pathsep, orig])
+    return "".join([text, pathsep, orig])
 
 
 def prepend_environ_path(env, name, text, pathsep=os.pathsep):
     """Prepend `text` into a $PATH-like environment variable. `env` is a
     dictionary of environment variables and `name` is the variable name.
     `pathsep` is the character separating path elements, defaulting to
     `os.pathsep`. The variable will be created if it is not already in `env`.
@@ -127,116 +146,123 @@
 
     """
     env[name] = prepend_path(env.get(name), text, pathsep=pathsep)
     return env
 
 
 def _make_user_data_pather():
-    datadir = os.environ.get('XDG_DATA_HOME', os.path.expanduser('~/.local/share'))
+    datadir = os.environ.get("XDG_DATA_HOME", os.path.expanduser("~/.local/share"))
 
     def pathfunc(*args):
         return os.path.join(datadir, *args)
 
     return pathfunc
 
+
 user_data_path = _make_user_data_pather()
 
 
 # Command-line access
 
+
 class DefaultExecCommand(multitool.Command):
-    name = 'exec'
-    argspec = '<command> [args...]'
-    summary = 'Run a program in the environment.'
+    name = "exec"
+    argspec = "<command> [args...]"
+    summary = "Run a program in the environment."
 
     def invoke(self, args, envclass=None, **kwargs):
         if len(args) < 1:
-            raise multitool.UsageError('exec requires at least 1 argument')
+            raise multitool.UsageError("exec requires at least 1 argument")
 
         envclass().execvpe(args)
 
 
 class DefaultShellCommand(multitool.Command):
     # XXX we hardcode bash!
-    name = 'shell'
-    argspec = ''
-    summary = 'Start an interactive shell in the environment.'
+    name = "shell"
+    argspec = ""
+    summary = "Start an interactive shell in the environment."
     help_if_no_args = False
 
     def invoke(self, args, envname=None, envclass=None, **kwargs):
         if len(args):
-            raise multitool.UsageError('shell expects no arguments')
+            raise multitool.UsageError("shell expects no arguments")
 
         from tempfile import NamedTemporaryFile
-        with NamedTemporaryFile(mode='wt', delete=False) as f:
-            print('''[ -e ~/.bashrc ] && source ~/.bashrc
+
+        with NamedTemporaryFile(mode="wt", delete=False) as f:
+            print(
+                """[ -e ~/.bashrc ] && source ~/.bashrc
 PS1="%s $PS1"
-rm %s''' % (envname, f.name), file=f)
+rm %s"""
+                % (envname, f.name),
+                file=f,
+            )
 
-        envclass().execvpe(['bash',
-                            '--rcfile', f.name,
-                            '-i'])
+        envclass().execvpe(["bash", "--rcfile", f.name, "-i"])
 
 
 class DefaultTool(multitool.Multitool):
     def __init__(self, envname, envclass, module):
         super(DefaultTool, self).__init__()
         self.envname = envname
         self.envclass = envclass
         self.module = module
 
-        self.cli_name = 'pkenvtool ' + envname
-        self.summary = 'Run tools in the %s environment.' % envname
-
+        self.cli_name = "pkenvtool " + envname
+        self.summary = "Run tools in the %s environment." % envname
 
     def invoke_command(self, cmd, args, **kwargs):
-        return super(DefaultTool, self).invoke_command(cmd, args,
-                                                       envname=self.envname,
-                                                       envclass=self.envclass,
-                                                       module=self.module,
-                                                       **kwargs)
+        return super(DefaultTool, self).invoke_command(
+            cmd,
+            args,
+            envname=self.envname,
+            envclass=self.envclass,
+            module=self.module,
+            **kwargs
+        )
 
 
 def _default_env_commandline(envname, module, argv):
-    from six import itervalues
-
     for name in dir(module):
         v = getattr(module, name)
         if v is not Environment and issubclass(v, Environment):
             envclass = v
             break
     else:
-        cli.die('internal error: cannot identify environment class for %s', envname)
+        cli.die("internal error: cannot identify environment class for %s", envname)
 
     tool = DefaultTool(envname, envclass, module)
-    tool.populate(itervalues(globals()))
+    tool.populate(globals().values())
     tool.commandline(argv)
 
 
 def commandline(argv=sys.argv):
     cli.propagate_sigint()
     cli.backtrace_on_usr1()
     cli.unicode_stdio()
 
-    if len(argv) < 2 or argv[1] in ('-h', '--help'):
-        print('''usage: pkenvtool <environment> [args...]
+    if len(argv) < 2 or argv[1] in ("-h", "--help"):
+        print(
+            """usage: pkenvtool <environment> [args...]
 
-Where acceptable "args" depend on the environment in question.''')
+Where acceptable "args" depend on the environment in question."""
+        )
         return
 
     envname = argv[1]
-    if not len(envname) or envname[0] == '.':
-        cli.die('illegal environment name %r', envname)
+    if not len(envname) or envname[0] == ".":
+        cli.die("illegal environment name %r", envname)
 
     from importlib import import_module
 
     try:
-        envmod = import_module('.' + envname, package=__package__)
+        envmod = import_module("." + envname, package=__package__)
     except Exception:
-        cli.die('unable to load module for environment %r', envname)
+        cli.die("unable to load module for environment %r", envname)
 
-    modargv = ['pkenvtool ' + argv[1]] + argv[2:]
+    modargv = ["pkenvtool " + argv[1]] + argv[2:]
 
-    if hasattr(envmod, 'commandline'):
+    if hasattr(envmod, "commandline"):
         envmod.commandline(modargv)
     else:
         _default_env_commandline(envname, envmod, modargv)
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/__init__.py` & `pwkit-1.2.0/pwkit/environments/casa/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   Python code in a way that allows you to analyze its output, check for
   error conditions, and so on. This is useful for certain features that are not
   currently available in the :mod:`~pwkit.environments.casa.tasks` module.
 
 """
 from __future__ import absolute_import, division, print_function
 
-__all__ = 'CasaEnvironment CasaTool commandline'.split()
+__all__ = "CasaEnvironment CasaTool commandline".split()
 
 import glob, io, os.path
 
 from ... import PKError, cli
 from ...cli import multitool
 from .. import Environment, prepend_environ_path, user_data_path
 
@@ -70,94 +70,98 @@
 
     def __init__(self, rootdir=None):
         if rootdir is None:
             rootdir = self._default_rootdir()
 
         self._rootdir = os.path.abspath(rootdir)
 
-
     def _default_rootdir(self):
-        d = os.environ.get('PWKIT_CASA')
+        d = os.environ.get("PWKIT_CASA")
         if d is None:
-            raise PKError('CASA installation directory must be specified '
-                          'in the $PWKIT_CASA environment variable')
+            raise PKError(
+                "CASA installation directory must be specified "
+                "in the $PWKIT_CASA environment variable"
+            )
         return d
 
-
     def modify_environment(self, env):
         """Maintaining compatibility with different CASA versions is a pain."""
 
         # Ugh. I don't see any way out of special-casing the RPM-based
         # installations ... which only exist on NRAO computers, AFAICT.
         # Hardcoding 64-bitness, hopefully that won't come back to bite me.
-        is_rpm_install = self._rootdir.startswith('/usr/lib64/casapy/release/')
+        is_rpm_install = self._rootdir.startswith("/usr/lib64/casapy/release/")
 
         def path(*args):
             return os.path.join(self._rootdir, *args)
 
-        env['CASAROOT'] = path()
-        env['CASAPATH'] = ' '.join([path(),
-                                    os.uname()[0].lower(),
-                                    'local',
-                                    os.uname()[1]])
+        env["CASAROOT"] = path()
+        env["CASAPATH"] = " ".join(
+            [path(), os.uname()[0].lower(), "local", os.uname()[1]]
+        )
 
         if is_rpm_install:
-            env['CASA_INSTALLATION_TYPE'] = 'rpm-installation'
-            prepend_environ_path(env, 'PATH', '/usr/lib64/casa/01/bin')
-            prepend_environ_path(env, 'PATH', path('bin'))
+            env["CASA_INSTALLATION_TYPE"] = "rpm-installation"
+            prepend_environ_path(env, "PATH", "/usr/lib64/casa/01/bin")
+            prepend_environ_path(env, "PATH", path("bin"))
         else:
-            env['CASA_INSTALLATION_TYPE'] = 'tar-installation'
+            env["CASA_INSTALLATION_TYPE"] = "tar-installation"
 
-            lib = 'lib64' if os.path.isdir(path('lib64')) else 'lib'
+            lib = "lib64" if os.path.isdir(path("lib64")) else "lib"
             # 4.3.1 comes with both python2.6 and python2.7???
-            pydir = sorted(glob.glob(path(lib, 'python2*')))[-1]
+            pydir = sorted(glob.glob(path(lib, "python2*")))[-1]
 
-            tcldir = path('share', 'tcl')
+            tcldir = path("share", "tcl")
             if os.path.isdir(tcldir):
-                env['TCL_LIBRARY'] = tcldir
+                env["TCL_LIBRARY"] = tcldir
             else:
-                tcl_versioned_dirs = glob.glob(path('share', 'tcl*'))
+                tcl_versioned_dirs = glob.glob(path("share", "tcl*"))
                 if len(tcl_versioned_dirs):
-                    env['TCL_LIBRARY'] = tcl_versioned_dirs[-1]
+                    env["TCL_LIBRARY"] = tcl_versioned_dirs[-1]
 
-            bindir = path(lib, 'casa', 'bin')
+            bindir = path(lib, "casa", "bin")
             if not os.path.isdir(bindir):
-                bindir = path(lib, 'casapy', 'bin')
-            prepend_environ_path(env, 'PATH', bindir)
+                bindir = path(lib, "casapy", "bin")
+            prepend_environ_path(env, "PATH", bindir)
 
-            env['CASA_INSTALLATION_DIRECTORY'] = env['CASAROOT']
-            env['__CASAPY_PYTHONDIR'] = pydir
-            env['MATPLOTLIBRC'] = path('share', 'matplotlib')
-            env['PYTHONHOME'] = env['CASAROOT']
-            env['TK_LIBRARY'] = path('share', 'tk')
-            env['QT_PLUGIN_PATH'] = path(lib, 'qt4', 'plugins')
+            env["CASA_INSTALLATION_DIRECTORY"] = env["CASAROOT"]
+            env["__CASAPY_PYTHONDIR"] = pydir
+            env["MATPLOTLIBRC"] = path("share", "matplotlib")
+            env["PYTHONHOME"] = env["CASAROOT"]
+            env["TK_LIBRARY"] = path("share", "tk")
+            env["QT_PLUGIN_PATH"] = path(lib, "qt4", "plugins")
 
-            prepend_environ_path(env, 'LD_LIBRARY_PATH', path(lib))
+            prepend_environ_path(env, "LD_LIBRARY_PATH", path(lib))
             # should we overwite PYTHONPATH instead?
-            prepend_environ_path(env, 'PYTHONPATH', os.path.join(pydir, 'site-packages'))
-            prepend_environ_path(env, 'PYTHONPATH', os.path.join(pydir, 'heuristics'))
-            prepend_environ_path(env, 'PYTHONPATH', pydir)
+            prepend_environ_path(
+                env, "PYTHONPATH", os.path.join(pydir, "site-packages")
+            )
+            prepend_environ_path(env, "PYTHONPATH", os.path.join(pydir, "heuristics"))
+            prepend_environ_path(env, "PYTHONPATH", pydir)
 
         return env
 
 
 # Command-line interface
 
 from .. import DefaultExecCommand, DefaultShellCommand
 
+
 class CasaTool(multitool.Multitool):
-    cli_name = 'pkenvtool casa'
-    summary = 'Run programs in the CASA environment.'
+    cli_name = "pkenvtool casa"
+    summary = "Run programs in the CASA environment."
 
     def invoke_command(self, cmd, args, **kwargs):
-        return super(CasaTool, self).invoke_command(cmd, args,
-                                                    envname='casa',
-                                                    envclass=CasaEnvironment,
-                                                    module=__package__,
-                                                    **kwargs)
+        return super(CasaTool, self).invoke_command(
+            cmd,
+            args,
+            envname="casa",
+            envclass=CasaEnvironment,
+            module=__package__,
+            **kwargs
+        )
 
 
 def commandline(argv):
-    from six import itervalues
     tool = CasaTool()
-    tool.populate(itervalues(globals()))
+    tool.populate(globals().values())
     tool.commandline(argv)
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/closures.py` & `pwkit-1.2.0/pwkit/environments/casa/closures.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 
 For most results to make sense, the data should be observations of a bright
 point source at phase center.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('Config ClosureCalculator closures_cli').split ()
+__all__ = str("Config ClosureCalculator closures_cli").split()
 
 import collections
-import six, numpy as np
-from six.moves import range, zip
+import numpy as np
 
 from ...cli import check_usage, die
 from ...kwargv import ParseKeywords, Custom
 from ...environments.casa import util
 from ...environments.casa.util import sanitize_unicode as b
 
-closures_doc = \
-"""
+closures_doc = """
 casatask closures vis=MS [keywords...]
 
 THIS TASK IS CURRENTLY BROKEN AND WILL REFUSE TO RUN.
 
 Plot diagnostics related to phase closure triple.
 
 vis=
@@ -42,78 +40,113 @@
 datacol=
   Name of the column to use for visibility data. Defaults to 'data'.
   You might want it to be 'corrected_data', although the point of
   phase closure analysis is that antenna-based calibrations don't
   affect its results ...
 """
 
-class Config (ParseKeywords):
-    vis = Custom (str, required=True)
-    datacol = 'data'
+
+class Config(ParseKeywords):
+    vis = Custom(str, required=True)
+    datacol = "data"
 
     # MeasurementSet filters
     array = str
     baseline = str
     field = str
     observation = str
-    polarization = 'RR,LL'
+    polarization = "RR,LL"
     scan = str
     scanintent = str
     spw = str
     taql = str
     time = str
     uvdist = str
 
-    loglevel = 'warn'
+    loglevel = "warn"
 
 
 # ########################################################################
 # Begin copying/emulating mirtask.util
 
 FPOL_X = 0
 FPOL_Y = 1
 FPOL_R = 2
 FPOL_L = 3
 FPOL_I = 4
 FPOL_Q = 5
 FPOL_U = 6
 FPOL_V = 7
 
-fpol_names = 'XYRLIQUV'
+fpol_names = "XYRLIQUV"
 
 # This table helps split a CASA pol code into a pair of fpol values. The pair
 # is packed into 8 bits, the upper 3 being for the left pol and the lower 4
 # being for the right.
 
-_pol_to_fpol = np.array ([
-    0xFFFF, # ?, illegal
-    0x44, 0x55, 0x66, 0x77, # I Q U V
-    0x22, 0x23, 0x32, 0x33, # RR RL LR LL
-    0x00, 0x01, 0x10, 0x11, # XX XY YX YY
-    0x20, 0x21, 0x30, 0x31, # RX RY LX LY
-    0x02, 0x03, 0x12, 0x13, # XR XL YR YL
-    # not bothering with the rest because seriously
-])
-
-pol_is_intensity = np.array ([
-    False, # ?, illegal
-    True, True, True, True, # I Q U V
-    True, False, False, True, # RR RL LR LL
-    True, False, False, True, # XX XY YX YY
-    False, False, False, False, # RX RY LX LY
-    False, False, False, False, # XR XL YR YL
-    # not bothering with the rest because seriously
-])
+_pol_to_fpol = np.array(
+    [
+        0xFFFF,  # ?, illegal
+        0x44,
+        0x55,
+        0x66,
+        0x77,  # I Q U V
+        0x22,
+        0x23,
+        0x32,
+        0x33,  # RR RL LR LL
+        0x00,
+        0x01,
+        0x10,
+        0x11,  # XX XY YX YY
+        0x20,
+        0x21,
+        0x30,
+        0x31,  # RX RY LX LY
+        0x02,
+        0x03,
+        0x12,
+        0x13,  # XR XL YR YL
+        # not bothering with the rest because seriously
+    ]
+)
+
+pol_is_intensity = np.array(
+    [
+        False,  # ?, illegal
+        True,
+        True,
+        True,
+        True,  # I Q U V
+        True,
+        False,
+        False,
+        True,  # RR RL LR LL
+        True,
+        False,
+        False,
+        True,  # XX XY YX YY
+        False,
+        False,
+        False,
+        False,  # RX RY LX LY
+        False,
+        False,
+        False,
+        False,  # XR XL YR YL
+        # not bothering with the rest because seriously
+    ]
+)
 
 # This table performs the reverse mapping, with index being the two f-pol
 # values packed into four bits each. A value of 0xFF indicates an illegal
 # pairing. The values come from pwkit.environments.casa.util:pol_names
 
-_fpol_to_pol = np.ndarray (128, dtype=np.int8)
-_fpol_to_pol.fill (0xFF)
+_fpol_to_pol = np.ndarray(128, dtype=np.int8)
+_fpol_to_pol.fill(0xFF)
 _fpol_to_pol[0x00] = 9
 _fpol_to_pol[0x01] = 10
 _fpol_to_pol[0x10] = 11
 _fpol_to_pol[0x11] = 12
 _fpol_to_pol[0x22] = 5
 _fpol_to_pol[0x23] = 5
 _fpol_to_pol[0x32] = 7
@@ -125,377 +158,391 @@
 
 # A "antpol" (AP) is an integer identifying an antenna/fpol pair. It
 # can be decoded without any external information. We used zero-based
 # integer antenna numbers so that
 #
 #   AP = M << 3 + FP
 
-def ap_format (ap, getname=str):
-    return '%s%c' % (getname (ap >> 3), fpol_names[ap & 0x7])
+
+def ap_format(ap, getname=str):
+    return "%s%c" % (getname(ap >> 3), fpol_names[ap & 0x7])
+
 
 ap_ant = lambda ap: ap >> 3
 ap_fpol = lambda ap: ap & 0x7
 antpol_to_ap = lambda antnum, fpol: (antnum << 3) + fpol
 
 # A "basepol" is 2-tuple of antpols.
 
-def bp_format (bp, getname=str):
+
+def bp_format(bp, getname=str):
     ap1, ap2 = bp
     if ap1 < 0:
-        raise ValueError ('first antpol %d is negative' % ap1)
+        raise ValueError("first antpol %d is negative" % ap1)
     if ap2 < 0:
-        raise ValueError ('second antpol %d is negative' % ap2)
+        raise ValueError("second antpol %d is negative" % ap2)
+
+    return "%s%c-%s%c" % (
+        getname(ap1 >> 3),
+        fpol_names[ap1 & 0x7],
+        getname(ap2 >> 3),
+        fpol_names[ap2 & 0x7],
+    )
 
-    return '%s%c-%s%c' % (getname (ap1 >> 3), fpol_names[ap1 & 0x7],
-                          getname (ap2 >> 3), fpol_names[ap2 & 0x7])
 
-def bp_to_aap (bp):
+def bp_to_aap(bp):
     """Converts a basepol into a tuple of (ant1, ant2, pol)."""
 
     ap1, ap2 = bp
     if ap1 < 0:
-        raise ValueError ('first antpol %d is negative' % ap1)
+        raise ValueError("first antpol %d is negative" % ap1)
     if ap2 < 0:
-        raise ValueError ('second antpol %d is negative' % ap2)
+        raise ValueError("second antpol %d is negative" % ap2)
 
     pol = _fpol_to_pol[((ap1 & 0x7) << 4) + (ap2 & 0x7)]
     if pol == 0xFF:
-        raise ValueError ('no CASA polarization code for pairing '
-                          '%c-%c' % (fpol_names[ap1 & 0x7],
-                                     fpol_names[ap2 & 0x7]))
+        raise ValueError(
+            "no CASA polarization code for pairing "
+            "%c-%c" % (fpol_names[ap1 & 0x7], fpol_names[ap2 & 0x7])
+        )
 
     return ap1 >> 3, ap2 >> 3, pol
 
-def aap_to_bp (ant1, ant2, pol):
+
+def aap_to_bp(ant1, ant2, pol):
     """Create a basepol from antenna numbers and a CASA polarization code."""
 
     if ant1 < 0:
-        raise ValueError ('first antenna is below 0: %s' % ant1)
+        raise ValueError("first antenna is below 0: %s" % ant1)
     if ant2 < ant1:
-        raise ValueError ('second antenna is below first: %s' % ant2)
+        raise ValueError("second antenna is below first: %s" % ant2)
     if pol < 1 or pol > 12:
-        raise ValueError ('illegal polarization code %s' % pol)
+        raise ValueError("illegal polarization code %s" % pol)
 
     fps = _pol_to_fpol[pol]
     ap1 = (ant1 << 3) + ((fps >> 4) & 0x07)
     ap2 = (ant2 << 3) + (fps & 0x07)
     return ap1, ap2
 
+
 # End copying/emulating mirtask.util
 # ########################################################################
 
 
-class StatsCollector (object):
-    def __init__ (self, chunk0size=64):
+class StatsCollector(object):
+    def __init__(self, chunk0size=64):
         self.chunk0size = chunk0size
-        self._keymap = collections.defaultdict (lambda: len (self._keymap))
-        self._m0 = None # 0th moment
-        self._m1 = None #
-        self._m2 = None # 2nd moment
-
+        self._keymap = collections.defaultdict(lambda: len(self._keymap))
+        self._m0 = None  # 0th moment
+        self._m1 = None  #
+        self._m2 = None  # 2nd moment
 
-    def accum (self, key, value, weight=1):
+    def accum(self, key, value, weight=1):
         index = self._keymap[key]
 
         if self._m0 is None:
-            self._m0 = np.zeros ((self.chunk0size,), dtype=np.result_type (weight))
-            self._m1 = np.zeros ((self.chunk0size,), dtype=np.result_type (value, weight))
-            self._m2 = np.zeros_like (self._m1)
+            self._m0 = np.zeros((self.chunk0size,), dtype=np.result_type(weight))
+            self._m1 = np.zeros((self.chunk0size,), dtype=np.result_type(value, weight))
+            self._m2 = np.zeros_like(self._m1)
         elif index >= self._m0.size:
-            self._m0 = np.concatenate ((self._m0, np.zeros_like (self._m0)))
-            self._m1 = np.concatenate ((self._m1, np.zeros_like (self._m1)))
-            self._m2 = np.concatenate ((self._m2, np.zeros_like (self._m2)))
+            self._m0 = np.concatenate((self._m0, np.zeros_like(self._m0)))
+            self._m1 = np.concatenate((self._m1, np.zeros_like(self._m1)))
+            self._m2 = np.concatenate((self._m2, np.zeros_like(self._m2)))
 
         self._m0[index] += weight
         q = weight * value
         self._m1[index] += q
         q *= value
         self._m2[index] += q
         return self
 
-
-    def finish (self, keyset, mask=True):
+    def finish(self, keyset, mask=True):
         """Returns (weights, means, variances), where:
 
         weights
           ndarray of number of samples per key
         means
           computed mean value for each key
         variances
           computed variance for each key
 
         """
-        n_us = len (self._keymap)
+        n_us = len(self._keymap)
         # By definition (for now), wt >= 1 everywhere, so we don't need to
         # worry about div-by-zero.
         wt_us = self._m0[:n_us]
         mean_us = self._m1[:n_us] / wt_us
         var_us = self._m2[:n_us] / wt_us - mean_us**2
 
-        n_them = len (keyset)
-        wt = np.zeros (n_them, dtype=self._m0.dtype)
-        mean = np.empty (n_them, dtype=self._m1.dtype)
-        mean.fill (np.nan)
-        var = np.empty_like (mean)
-        var.fill (np.nan)
+        n_them = len(keyset)
+        wt = np.zeros(n_them, dtype=self._m0.dtype)
+        mean = np.empty(n_them, dtype=self._m1.dtype)
+        mean.fill(np.nan)
+        var = np.empty_like(mean)
+        var.fill(np.nan)
 
         us_idx = []
         them_idx = []
 
-        for them_i, key in enumerate (keyset):
+        for them_i, key in enumerate(keyset):
             us_i = self._keymap[key]
             if us_i < n_us:
-                them_idx.append (them_i)
-                us_idx.append (us_i)
+                them_idx.append(them_i)
+                us_idx.append(us_i)
             # otherwise, we must not have seen that key
 
         wt[them_idx] = wt_us[us_idx]
         mean[them_idx] = mean_us[us_idx]
         var[them_idx] = var_us[us_idx]
 
         if mask:
-            m = ~np.isfinite (mean)
-            mean = np.ma.MaskedArray (mean, m)
-            var = np.ma.MaskedArray (var, m)
+            m = ~np.isfinite(mean)
+            mean = np.ma.MaskedArray(mean, m)
+            var = np.ma.MaskedArray(var, m)
 
         self._m0 = self._m1 = self._m2 = None
-        self._keymap.clear ()
+        self._keymap.clear()
 
         return wt, mean, var
 
 
-class StatsCollector2D (object):
-    def __init__ (self, chunk0size=64):
+class StatsCollector2D(object):
+    def __init__(self, chunk0size=64):
         self.chunk0size = chunk0size
-        self._key1map = collections.defaultdict (lambda: len (self._key1map))
-        self._key2map = collections.defaultdict (lambda: len (self._key2map))
+        self._key1map = collections.defaultdict(lambda: len(self._key1map))
+        self._key2map = collections.defaultdict(lambda: len(self._key2map))
         self._m0 = None
         self._m1 = None
         self._m2 = None
 
-
-    def accum (self, key1, key2, value, weight=1):
+    def accum(self, key1, key2, value, weight=1):
         index1 = self._key1map[key1]
         index2 = self._key2map[key2]
 
         if self._m0 is None:
-            self._m0 = np.zeros ((self.chunk0size, self.chunk0size), dtype=np.result_type (weight))
-            self._m1 = np.zeros ((self.chunk0size, self.chunk0size), dtype=np.result_type (value, weight))
-            self._m2 = np.zeros_like (self._m1)
+            self._m0 = np.zeros(
+                (self.chunk0size, self.chunk0size), dtype=np.result_type(weight)
+            )
+            self._m1 = np.zeros(
+                (self.chunk0size, self.chunk0size), dtype=np.result_type(value, weight)
+            )
+            self._m2 = np.zeros_like(self._m1)
 
         if index1 >= self._m0.shape[0]:
-            self._m0 = np.concatenate ((self._m0, np.zeros_like (self._m0)), axis=0)
-            self._m1 = np.concatenate ((self._m1, np.zeros_like (self._m1)), axis=0)
-            self._m2 = np.concatenate ((self._m2, np.zeros_like (self._m2)), axis=0)
+            self._m0 = np.concatenate((self._m0, np.zeros_like(self._m0)), axis=0)
+            self._m1 = np.concatenate((self._m1, np.zeros_like(self._m1)), axis=0)
+            self._m2 = np.concatenate((self._m2, np.zeros_like(self._m2)), axis=0)
 
         if index2 >= self._m0.shape[1]:
-            self._m0 = np.concatenate ((self._m0, np.zeros_like (self._m0)), axis=1)
-            self._m1 = np.concatenate ((self._m1, np.zeros_like (self._m1)), axis=1)
-            self._m2 = np.concatenate ((self._m2, np.zeros_like (self._m2)), axis=1)
+            self._m0 = np.concatenate((self._m0, np.zeros_like(self._m0)), axis=1)
+            self._m1 = np.concatenate((self._m1, np.zeros_like(self._m1)), axis=1)
+            self._m2 = np.concatenate((self._m2, np.zeros_like(self._m2)), axis=1)
 
-        self._m0[index1,index2] += weight
+        self._m0[index1, index2] += weight
         q = weight * value
-        self._m1[index1,index2] += q
+        self._m1[index1, index2] += q
         q *= value
-        self._m2[index1,index2] += q
+        self._m2[index1, index2] += q
         return self
 
-
-    def finish (self, key1set, key2set, mask=True):
+    def finish(self, key1set, key2set, mask=True):
         """Returns (weights, means, variances), where:
 
         weights
           ndarray of number of samples per key; shape (n1, n2), where n1 is the
           size of key1set and n2 is the size of key2set.
         means
           computed mean value for each key
         variances
           computed variance for each key
 
         """
-        n1_us = len (self._key1map)
-        n2_us = len (self._key2map)
-        wt_us = self._m0[:n1_us,:n2_us]
-        badwt = (wt_us == 0) | ~np.isfinite (wt_us)
+        n1_us = len(self._key1map)
+        n2_us = len(self._key2map)
+        wt_us = self._m0[:n1_us, :n2_us]
+        badwt = (wt_us == 0) | ~np.isfinite(wt_us)
         wt_us[badwt] = 1
-        mean_us = self._m1[:n1_us,:n2_us] / wt_us
-        var_us = self._m2[:n1_us,:n2_us] / wt_us - mean_us**2
+        mean_us = self._m1[:n1_us, :n2_us] / wt_us
+        var_us = self._m2[:n1_us, :n2_us] / wt_us - mean_us**2
         wt_us[badwt] = 0
         mean_us[badwt] = np.nan
         var_us[badwt] = np.nan
 
-        n1_them = len (key1set)
-        n2_them = len (key2set)
-        wt = np.zeros ((n1_them, n2_them), dtype=self._m0.dtype)
-        mean = np.empty ((n1_them, n2_them), dtype=self._m1.dtype)
-        mean.fill (np.nan)
-        var = np.empty_like (mean)
-        var.fill (np.nan)
+        n1_them = len(key1set)
+        n2_them = len(key2set)
+        wt = np.zeros((n1_them, n2_them), dtype=self._m0.dtype)
+        mean = np.empty((n1_them, n2_them), dtype=self._m1.dtype)
+        mean.fill(np.nan)
+        var = np.empty_like(mean)
+        var.fill(np.nan)
 
         # You can't fancy-index on two axes simultaneously, so we do a manual
         # loop on the first axis.
 
         us_idx2 = []
         them_idx2 = []
 
-        for them_i2, key2 in enumerate (key2set):
+        for them_i2, key2 in enumerate(key2set):
             us_i2 = self._key2map[key2]
             if us_i2 < n2_us:
-                them_idx2.append (them_i2)
-                us_idx2.append (us_i2)
+                them_idx2.append(them_i2)
+                us_idx2.append(us_i2)
             # otherwise, we must not have seen that key
 
-        for them_i1, key1 in enumerate (key1set):
+        for them_i1, key1 in enumerate(key1set):
             us_i1 = self._key1map[key1]
             if us_i1 >= n1_us:
-                continue # don't have this key
+                continue  # don't have this key
 
-            wt[them_i1,them_idx2] = wt_us[us_i1,us_idx2]
-            mean[them_i1,them_idx2] = mean_us[us_i1,us_idx2]
-            var[them_i1,them_idx2] = var_us[us_i1,us_idx2]
+            wt[them_i1, them_idx2] = wt_us[us_i1, us_idx2]
+            mean[them_i1, them_idx2] = mean_us[us_i1, us_idx2]
+            var[them_i1, them_idx2] = var_us[us_i1, us_idx2]
 
         if mask:
-            m = ~np.isfinite (mean)
-            mean = np.ma.MaskedArray (mean, m)
-            var = np.ma.MaskedArray (var, m)
+            m = ~np.isfinite(mean)
+            mean = np.ma.MaskedArray(mean, m)
+            var = np.ma.MaskedArray(var, m)
 
         self._m0 = self._m1 = self._m2 = None
-        self._key1map.clear ()
-        self._key2map.clear ()
+        self._key1map.clear()
+        self._key2map.clear()
 
         return wt, mean, var
 
 
-class StatsCollectorND (object):
+class StatsCollectorND(object):
     """This is vaguely like StatsCollector2D, but rather than having two discrete
     keyed axes, we are passed one key and an N-dimensional vector of values.
 
     """
-    def __init__ (self, chunk0size=64):
+
+    def __init__(self, chunk0size=64):
         self.chunk0size = chunk0size
-        self._keymap = collections.defaultdict (lambda: len (self._keymap))
+        self._keymap = collections.defaultdict(lambda: len(self._keymap))
         self._m0 = None
         self._m1 = None
         self._m2 = None
 
-
-    def accum (self, key, values, weights=1):
+    def accum(self, key, values, weights=1):
         index = self._keymap[key]
-        values = np.asarray (values)
-        weights = np.broadcast_to (weights, values.shape)
+        values = np.asarray(values)
+        weights = np.broadcast_to(weights, values.shape)
 
         if self._m0 is None:
-            self._m0 = np.zeros ((self.chunk0size,) + values.shape, dtype=weights.dtype)
-            self._m1 = np.zeros ((self.chunk0size,) + values.shape, dtype=np.result_type (weights, values))
-            self._m2 = np.zeros_like (self._m1)
+            self._m0 = np.zeros((self.chunk0size,) + values.shape, dtype=weights.dtype)
+            self._m1 = np.zeros(
+                (self.chunk0size,) + values.shape, dtype=np.result_type(weights, values)
+            )
+            self._m2 = np.zeros_like(self._m1)
         elif index >= self._m0.size:
-            self._m0 = np.concatenate ((self._m0, np.zeros_like (self._m0)))
-            self._m1 = np.concatenate ((self._m1, np.zeros_like (self._m1)))
-            self._m2 = np.concatenate ((self._m2, np.zeros_like (self._m2)))
+            self._m0 = np.concatenate((self._m0, np.zeros_like(self._m0)))
+            self._m1 = np.concatenate((self._m1, np.zeros_like(self._m1)))
+            self._m2 = np.concatenate((self._m2, np.zeros_like(self._m2)))
 
         if values.shape != self._m0.shape[1:]:
-            raise ValueError ('inconsistent `values` shapes: had %r, got %r' % (
-                self._m0.shape[1:], values.shape))
+            raise ValueError(
+                "inconsistent `values` shapes: had %r, got %r"
+                % (self._m0.shape[1:], values.shape)
+            )
 
         self._m0[index] += weights
         q = weights * values
         self._m1[index] += q
         q *= values
         self._m2[index] += q
         return self
 
-
-    def finish (self, keyset, mask=True):
+    def finish(self, keyset, mask=True):
         """Returns (weights, means, variances), where:
 
         weights
           total weights per key
         means
           computed mean value for each key
         variances
           computed variance for each key
 
         The arrays all have a shape of `(nkeys,)+shape(values)`.
 
         """
-        n_us = len (self._keymap)
+        n_us = len(self._keymap)
         wt_us = self._m0[:n_us]
-        badwt = (wt_us == 0) | ~np.isfinite (wt_us)
-        wt_us[badwt] = 1.
+        badwt = (wt_us == 0) | ~np.isfinite(wt_us)
+        wt_us[badwt] = 1.0
         mean_us = self._m1[:n_us] / wt_us
         var_us = self._m2[:n_us] / wt_us - mean_us**2
         wt_us[badwt] = 0
         mean_us[badwt] = np.nan
         var_us[badwt] = np.nan
 
-        n_them = len (keyset)
-        wt = np.zeros ((n_them,) + mean_us.shape[1:], dtype=self._m0.dtype)
-        mean = np.empty ((n_them,) + mean_us.shape[1:], dtype=self._m1.dtype)
-        mean.fill (np.nan)
-        var = np.empty_like (mean)
-        var.fill (np.nan)
+        n_them = len(keyset)
+        wt = np.zeros((n_them,) + mean_us.shape[1:], dtype=self._m0.dtype)
+        mean = np.empty((n_them,) + mean_us.shape[1:], dtype=self._m1.dtype)
+        mean.fill(np.nan)
+        var = np.empty_like(mean)
+        var.fill(np.nan)
 
         us_idx = []
         them_idx = []
 
-        for them_i, key in enumerate (keyset):
+        for them_i, key in enumerate(keyset):
             us_i = self._keymap[key]
             if us_i < n_us:
-                them_idx.append (them_i)
-                us_idx.append (us_i)
+                them_idx.append(them_i)
+                us_idx.append(us_i)
             # otherwise, we must not have seen that key
 
         wt[them_idx] = wt_us[us_idx]
         mean[them_idx] = mean_us[us_idx]
         var[them_idx] = var_us[us_idx]
 
         if mask:
-            m = ~np.isfinite (mean)
-            mean = np.ma.MaskedArray (mean, m)
-            var = np.ma.MaskedArray (var, m)
+            m = ~np.isfinite(mean)
+            mean = np.ma.MaskedArray(mean, m)
+            var = np.ma.MaskedArray(var, m)
 
         self._m0 = self._m1 = self._m2 = None
-        self._keymap.clear ()
+        self._keymap.clear()
 
         return wt, mean, var
 
 
-def postproc (stats_result):
+def postproc(stats_result):
     """Simple helper to postprocess angular outputs from StatsCollectors in the
     way we want.
 
     """
     n, mean, scat = stats_result
-    mean *= 180 / np.pi # rad => deg
-    scat /= n # variance-of-samples => variance-of-mean
-    scat **= 0.5 # variance => stddev
-    scat *= 180 / np.pi # rad => deg
+    mean *= 180 / np.pi  # rad => deg
+    scat /= n  # variance-of-samples => variance-of-mean
+    scat **= 0.5  # variance => stddev
+    scat *= 180 / np.pi  # rad => deg
     return mean, scat
 
 
-def postproc_mask (stats_result):
+def postproc_mask(stats_result):
     """Simple helper to postprocess angular outputs from StatsCollectors in the
     way we want.
 
     """
     n, mean, scat = stats_result
 
-    ok = np.isfinite (mean)
+    ok = np.isfinite(mean)
     n = n[ok]
     mean = mean[ok]
     scat = scat[ok]
 
-    mean *= 180 / np.pi # rad => deg
-    scat /= n # variance-of-samples => variance-of-mean
-    scat **= 0.5 # variance => stddev
-    scat *= 180 / np.pi # rad => deg
+    mean *= 180 / np.pi  # rad => deg
+    scat /= n  # variance-of-samples => variance-of-mean
+    scat **= 0.5  # variance => stddev
+    scat *= 180 / np.pi  # rad => deg
     return ok, mean, scat
 
 
-def grid_bp_data (bps, items, mask=True):
+def grid_bp_data(bps, items, mask=True):
     """Given a bunch of scalars associated with intensity-type basepols, place
     them onto a grid. There should be only two polarizations represented (e.g.
     RR, LL); baselines for one of them will be put into the upper triangle of
     the grid, while baselines for the other will be put into the lower triangle.
 
     `bps` is an iterable that yields a superset of all bps to be gridded.
 
@@ -516,100 +563,106 @@
       basepols are filled with NaNs, or masked if `mask` is True.
 
     The basepol (ant1, ant2, pol1) is gridded into `data[i1,i2]`, where `i1`
     is the index of `ant1` in `ants`, etc. The basepol (ant1, ant2, pol2) is
     gridded into `data[i2,i1]`.
 
     """
-    seen_ants = set ()
-    seen_pols = set ()
+    seen_ants = set()
+    seen_pols = set()
 
-    for ant1, ant2, pol in (bp_to_aap (bp) for bp in bps):
-        seen_ants.add (ant1)
-        seen_ants.add (ant2)
-        seen_pols.add (pol)
-
-    if len (seen_pols) != 2:
-        raise Exception ('can only work with 2 polarizations')
-    pol1, pol2 = sorted (seen_pols)
+    for ant1, ant2, pol in (bp_to_aap(bp) for bp in bps):
+        seen_ants.add(ant1)
+        seen_ants.add(ant2)
+        seen_pols.add(pol)
+
+    if len(seen_pols) != 2:
+        raise Exception("can only work with 2 polarizations")
+    pol1, pol2 = sorted(seen_pols)
 
-    seen_ants = np.array (sorted (seen_ants))
-    ant_map = dict ((a, i) for (i, a) in enumerate (seen_ants))
+    seen_ants = np.array(sorted(seen_ants))
+    ant_map = dict((a, i) for (i, a) in enumerate(seen_ants))
 
     data = None
-    n = len (seen_ants)
+    n = len(seen_ants)
 
     for bp, value in items:
         if data is None:
-            data = np.empty ((n, n), dtype=np.result_type (value))
-            data.fill (np.nan)
+            data = np.empty((n, n), dtype=np.result_type(value))
+            data.fill(np.nan)
 
-        ant1, ant2, pol = bp_to_aap (bp)
+        ant1, ant2, pol = bp_to_aap(bp)
         i1 = ant_map[ant1]
         i2 = ant_map[ant2]
 
         if pol == pol1:
-            data[i1,i2] = value
+            data[i1, i2] = value
         else:
-            data[i2,i1] = value
+            data[i2, i1] = value
 
     if mask:
-        data = np.ma.MaskedArray (data, ~np.isfinite (data))
+        data = np.ma.MaskedArray(data, ~np.isfinite(data))
 
     return pol1, pol2, seen_ants, data
 
 
-class ClosureCalculator (object):
-    def process (self, cfg):
+class ClosureCalculator(object):
+    def process(self, cfg):
         # Initialize whole-run buffers.
-        raise Exception('BROKEN: NEEDS UPDATE TO SELECT ON DATA_DESC_ID')
+        raise Exception("BROKEN: NEEDS UPDATE TO SELECT ON DATA_DESC_ID")
 
-        self.all_aps = set ()
-        self.all_bps = set ()
-        self.all_times = set ()
-        self.global_stats_by_time = StatsCollector ()
-        self.ap_stats_by_ddid = collections.defaultdict (StatsCollector)
-        self.bp_stats_by_ddid = collections.defaultdict (StatsCollector)
-        self.ap_spec_stats_by_ddid = collections.defaultdict (StatsCollectorND)
-        self.ap_time_stats_by_ddid = collections.defaultdict (StatsCollector2D)
+        self.all_aps = set()
+        self.all_bps = set()
+        self.all_times = set()
+        self.global_stats_by_time = StatsCollector()
+        self.ap_stats_by_ddid = collections.defaultdict(StatsCollector)
+        self.bp_stats_by_ddid = collections.defaultdict(StatsCollector)
+        self.ap_spec_stats_by_ddid = collections.defaultdict(StatsCollectorND)
+        self.ap_time_stats_by_ddid = collections.defaultdict(StatsCollector2D)
 
-        self._process_ms (cfg)
+        self._process_ms(cfg)
         return self
 
-
-    def _process_ms (self, cfg):
-        tb = util.tools.table ()
-        ms = util.tools.ms ()
-        me = util.tools.measures ()
+    def _process_ms(self, cfg):
+        tb = util.tools.table()
+        ms = util.tools.ms()
+        me = util.tools.measures()
 
         # Prep.
 
-        ms.open (b(cfg.vis))
-        ms.msselect (b(dict ((n, cfg.get (n)) for n in util.msselect_keys
-                             if cfg.get (n) is not None)))
-
-        rangeinfo = ms.range (b'data_desc_id field_id'.split ())
-        ddids = rangeinfo['data_desc_id']
-        fields = rangeinfo['field_id']
-
-        tb.open (b(cfg.vis + '/DATA_DESCRIPTION'), nomodify=True)
-        ddid_to_polid = tb.getcol (b'POLARIZATION_ID')
-        ddid_to_spwid = tb.getcol (b'SPECTRAL_WINDOW_ID')
-        tb.close ()
+        ms.open(b(cfg.vis))
+        ms.msselect(
+            b(
+                dict(
+                    (n, cfg.get(n))
+                    for n in util.msselect_keys
+                    if cfg.get(n) is not None
+                )
+            )
+        )
+
+        rangeinfo = ms.range(b"data_desc_id field_id".split())
+        ddids = rangeinfo["data_desc_id"]
+        fields = rangeinfo["field_id"]
+
+        tb.open(b(cfg.vis + "/DATA_DESCRIPTION"), nomodify=True)
+        ddid_to_polid = tb.getcol(b"POLARIZATION_ID")
+        ddid_to_spwid = tb.getcol(b"SPECTRAL_WINDOW_ID")
+        tb.close()
 
-        tb.open (b(cfg.vis + '/POLARIZATION'), nomodify=True)
+        tb.open(b(cfg.vis + "/POLARIZATION"), nomodify=True)
         polid_to_polns = {}
-        for i in range (tb.nrows ()):
-            polid_to_polns[i] = tb.getcell (b'CORR_TYPE', i)
-        tb.close ()
-
-        tb.open (b(cfg.vis + '/ANTENNA'), nomodify=True)
-        self.ant_names = tb.getcol (b'NAME')
-        self.ant_stations = tb.getcol (b'STATION')
-        tb.close ()
+        for i in range(tb.nrows()):
+            polid_to_polns[i] = tb.getcell(b"CORR_TYPE", i)
+        tb.close()
+
+        tb.open(b(cfg.vis + "/ANTENNA"), nomodify=True)
+        self.ant_names = tb.getcol(b"NAME")
+        self.ant_stations = tb.getcol(b"STATION")
+        tb.close()
 
         # Read stuff in. We can't expect that weight values have their
         # absolute scale set correctly, but we can still use them to set the
         # relative weighting of the data points.
         #
         #   datacol is (ncorr, nchan, nchunk)
         #   flag is (ncorr, nchan, nchunk); zero means OK data
@@ -621,254 +674,248 @@
         #
         #   spw, time, baseline, poln, frequency
         #
         # We are encouraged to use the new iteration interface
         # (ms.niterinit(), etc), but as of 4.6.0 it is fundamentally broken
         # (asking for ANTENNA2 gets you ANTENNA1) so never mind.
 
-        colnames = [cfg.datacol] + 'flag weight time antenna1 antenna2'.split ()
+        colnames = [cfg.datacol] + "flag weight time antenna1 antenna2".split()
         colnames = b(colnames)
 
         for ddid in ddids:
-            raise Exception('UPDATE TO SELECT ON DATA_DESC_ID BECAUSE CASA IS BROKEN')
+            raise Exception("UPDATE TO SELECT ON DATA_DESC_ID BECAUSE CASA IS BROKEN")
 
-            ms.selectinit (ddid)
-            ms.iterinit (maxrows=4096)
-            ms.iterorigin ()
+            ms.selectinit(ddid)
+            ms.iterinit(maxrows=4096)
+            ms.iterorigin()
 
             self.cur_ddid = ddid
-            self.cur_time = -1.
-            self._start_timeslot ()
+            self.cur_time = -1.0
+            self._start_timeslot()
             all_polns = polid_to_polns[ddid_to_polid[ddid]]
-            polinfo = [(i, p) for i, p in enumerate (all_polns) if pol_is_intensity[p]]
+            polinfo = [(i, p) for i, p in enumerate(all_polns) if pol_is_intensity[p]]
 
             while True:
-                cols = ms.getdata (items=colnames)
+                cols = ms.getdata(items=colnames)
 
-                for i in range (cols['time'].size): # all records
-                    time = cols['time'][i]
+                for i in range(cols["time"].size):  # all records
+                    time = cols["time"][i]
                     if time != self.cur_time:
-                        self._finish_timeslot ()
+                        self._finish_timeslot()
                         self.cur_time = time
-                        self._start_timeslot ()
+                        self._start_timeslot()
 
-                    antenna1 = cols['antenna1'][i]
-                    antenna2 = cols['antenna2'][i]
+                    antenna1 = cols["antenna1"][i]
+                    antenna2 = cols["antenna2"][i]
                     if antenna1 == antenna2:
-                        continue # no autocorrelations
+                        continue  # no autocorrelations
 
-                    for j, poln in polinfo: # all polns
-                        flags = cols['flag'][j,:,i]
-                        if flags.all ():
-                            continue # all flagged
+                    for j, poln in polinfo:  # all polns
+                        flags = cols["flag"][j, :, i]
+                        if flags.all():
+                            continue  # all flagged
 
-                        data = cols[cfg.datacol][j,:,i]
+                        data = cols[cfg.datacol][j, :, i]
                         # data and flags are now both shape (nchan,)
-                        np.logical_not (flags, flags)
+                        np.logical_not(flags, flags)
                         # flags=1 now indicates good data
 
-                        self.all_times.add (time)
-                        bp = aap_to_bp (antenna1, antenna2, poln)
-                        self.all_bps.add (bp)
-                        self.data_by_bp[bp] = (data, flags) # + weight spectrum?
+                        self.all_times.add(time)
+                        bp = aap_to_bp(antenna1, antenna2, poln)
+                        self.all_bps.add(bp)
+                        self.data_by_bp[bp] = (data, flags)  # + weight spectrum?
 
                         # Here we exploit the fact that we're only considering
                         # intensity-type polarizations, so bp[0] and bp[1]
                         # always have the same fpol. Also that ap_by_fpol is a
                         # defaultdict.
                         for ap in bp:
-                            self.all_aps.add (ap)
-                            self.ap_by_fpol[ap & 0x7].add (ap)
+                            self.all_aps.add(ap)
+                            self.ap_by_fpol[ap & 0x7].add(ap)
 
-                if not ms.iternext ():
-                    self._finish_timeslot ()
+                if not ms.iternext():
+                    self._finish_timeslot()
                     break
 
-        ms.close ()
+        ms.close()
         return self
 
+    def _getname(self, antidx):
+        return "%s@%s:" % (self.ant_names[antidx], self.ant_stations[antidx])
 
-    def _getname (self, antidx):
-        return '%s@%s:' % (self.ant_names[antidx], self.ant_stations[antidx])
-
-
-    def _start_timeslot (self):
+    def _start_timeslot(self):
         self.data_by_bp = {}
-        self.ap_by_fpol = collections.defaultdict (set)
+        self.ap_by_fpol = collections.defaultdict(set)
 
-
-    def _finish_timeslot (self):
+    def _finish_timeslot(self):
         """We have loaded in all of the visibilities in one timeslot. We can now
         compute the phase closure triples.
 
         XXX: we should only process independent triples. Are we???
 
         """
-        for fpol, aps in self.ap_by_fpol.items ():
-            aps = sorted (aps)
-            nap = len (aps)
+        for fpol, aps in self.ap_by_fpol.items():
+            aps = sorted(aps)
+            nap = len(aps)
 
-            for i1, ap1 in enumerate (aps):
-                for i2 in range (i1, nap):
+            for i1, ap1 in enumerate(aps):
+                for i2 in range(i1, nap):
                     ap2 = aps[i2]
                     bp1 = (ap1, ap2)
-                    info = self.data_by_bp.get (bp1)
+                    info = self.data_by_bp.get(bp1)
                     if info is None:
                         continue
 
                     data1, flags1 = info
 
-                    for i3 in range (i2, nap):
+                    for i3 in range(i2, nap):
                         ap3 = aps[i3]
                         bp2 = (ap2, ap3)
-                        info = self.data_by_bp.get (bp2)
+                        info = self.data_by_bp.get(bp2)
                         if info is None:
                             continue
 
                         data2, flags2 = info
                         bp3 = (ap1, aps[i3])
-                        info = self.data_by_bp.get (bp3)
+                        info = self.data_by_bp.get(bp3)
                         if info is None:
                             continue
 
                         data3, flags3 = info
 
                         # try to minimize allocations:
                         tflags = flags1 & flags2
-                        np.logical_and (tflags, flags3, tflags)
-                        if not tflags.any ():
+                        np.logical_and(tflags, flags3, tflags)
+                        if not tflags.any():
                             continue
 
-                        triple = data3.conj ()
-                        np.multiply (triple, data1, triple)
-                        np.multiply (triple, data2, triple)
-                        self._process_sample (ap1, ap2, ap3, triple, tflags)
+                        triple = data3.conj()
+                        np.multiply(triple, data1, triple)
+                        np.multiply(triple, data2, triple)
+                        self._process_sample(ap1, ap2, ap3, triple, tflags)
 
         # Reset for next timeslot
 
-        self.cur_time = -1.
+        self.cur_time = -1.0
         self.bp_by_ap = None
         self.ap_by_fpol = None
 
-
-    def _process_sample (self, ap1, ap2, ap3, triple, tflags):
-        """We have computed one independent phase closure triple in one timeslot.
-
-        """
+    def _process_sample(self, ap1, ap2, ap3, triple, tflags):
+        """We have computed one independent phase closure triple in one timeslot."""
         # Frequency-resolved:
-        np.divide (triple, np.abs (triple), triple)
-        phase = np.angle (triple)
+        np.divide(triple, np.abs(triple), triple)
+        phase = np.angle(triple)
 
-        self.ap_spec_stats_by_ddid[self.cur_ddid].accum (ap1, phase, tflags + 0.)
-        self.ap_spec_stats_by_ddid[self.cur_ddid].accum (ap2, phase, tflags + 0.)
-        self.ap_spec_stats_by_ddid[self.cur_ddid].accum (ap3, phase, tflags + 0.)
+        self.ap_spec_stats_by_ddid[self.cur_ddid].accum(ap1, phase, tflags + 0.0)
+        self.ap_spec_stats_by_ddid[self.cur_ddid].accum(ap2, phase, tflags + 0.0)
+        self.ap_spec_stats_by_ddid[self.cur_ddid].accum(ap3, phase, tflags + 0.0)
 
         # Frequency-averaged:
-        triple = np.dot (triple, tflags) / tflags.sum ()
-        phase = np.angle (triple)
-
-        self.global_stats_by_time.accum (self.cur_time, phase)
-
-        self.ap_stats_by_ddid[self.cur_ddid].accum (ap1, phase)
-        self.ap_stats_by_ddid[self.cur_ddid].accum (ap2, phase)
-        self.ap_stats_by_ddid[self.cur_ddid].accum (ap3, phase)
-        self.bp_stats_by_ddid[self.cur_ddid].accum ((ap1, ap2), phase)
-        self.bp_stats_by_ddid[self.cur_ddid].accum ((ap1, ap3), phase)
-        self.bp_stats_by_ddid[self.cur_ddid].accum ((ap2, ap3), phase)
+        triple = np.dot(triple, tflags) / tflags.sum()
+        phase = np.angle(triple)
 
-        self.ap_time_stats_by_ddid[self.cur_ddid].accum (self.cur_time, ap1, phase)
-        self.ap_time_stats_by_ddid[self.cur_ddid].accum (self.cur_time, ap2, phase)
-        self.ap_time_stats_by_ddid[self.cur_ddid].accum (self.cur_time, ap3, phase)
+        self.global_stats_by_time.accum(self.cur_time, phase)
 
+        self.ap_stats_by_ddid[self.cur_ddid].accum(ap1, phase)
+        self.ap_stats_by_ddid[self.cur_ddid].accum(ap2, phase)
+        self.ap_stats_by_ddid[self.cur_ddid].accum(ap3, phase)
+        self.bp_stats_by_ddid[self.cur_ddid].accum((ap1, ap2), phase)
+        self.bp_stats_by_ddid[self.cur_ddid].accum((ap1, ap3), phase)
+        self.bp_stats_by_ddid[self.cur_ddid].accum((ap2, ap3), phase)
+
+        self.ap_time_stats_by_ddid[self.cur_ddid].accum(self.cur_time, ap1, phase)
+        self.ap_time_stats_by_ddid[self.cur_ddid].accum(self.cur_time, ap2, phase)
+        self.ap_time_stats_by_ddid[self.cur_ddid].accum(self.cur_time, ap3, phase)
 
-    def report (self, cfg):
+    def report(self, cfg):
         import omega as om
         import omega.gtk3
         from pwkit import ndshow_gtk3
 
-        self.all_aps = np.sort (list (self.all_aps))
-        self.all_bps = sorted (self.all_bps)
-        self.all_times = np.sort (list (self.all_times))
+        self.all_aps = np.sort(list(self.all_aps))
+        self.all_bps = sorted(self.all_bps)
+        self.all_times = np.sort(list(self.all_times))
 
         # Antpols by DDID, time:
         data = []
         descs = []
 
-        for ddid, stats in self.ap_time_stats_by_ddid.items ():
-            mean, scat = postproc (stats.finish (self.all_times, self.all_aps))
-            data.append (mean / scat)
-            descs.append ('DDID %d' % ddid)
+        for ddid, stats in self.ap_time_stats_by_ddid.items():
+            mean, scat = postproc(stats.finish(self.all_times, self.all_aps))
+            data.append(mean / scat)
+            descs.append("DDID %d" % ddid)
 
-        print ('Viewing X axis: antpol; Y axis: time; iteration: DDID (~= spwid) ...')
-        ndshow_gtk3.cycle (data, descs, run_main=True)
+        print("Viewing X axis: antpol; Y axis: time; iteration: DDID (~= spwid) ...")
+        ndshow_gtk3.cycle(data, descs, run_main=True)
 
         # Antpols by DDID, freq:
         data = []
         descs = []
 
-        for ddid, stats in self.ap_spec_stats_by_ddid.items ():
-            mean, scat = postproc (stats.finish (self.all_aps))
-            data.append (mean / scat)
-            descs.append ('DDID %d' % ddid)
+        for ddid, stats in self.ap_spec_stats_by_ddid.items():
+            mean, scat = postproc(stats.finish(self.all_aps))
+            data.append(mean / scat)
+            descs.append("DDID %d" % ddid)
 
-        print ('Viewing X axis: frequency; Y axis: antpol; iteration: DDID ...')
-        ndshow_gtk3.cycle (data, descs, run_main=True)
+        print("Viewing X axis: frequency; Y axis: antpol; iteration: DDID ...")
+        ndshow_gtk3.cycle(data, descs, run_main=True)
 
         # Antpols by DDID
-        p = om.RectPlot ()
+        p = om.RectPlot()
 
-        for ddid, stats in self.ap_stats_by_ddid.items ():
-            ok, mean, scat = postproc_mask (stats.finish (self.all_aps))
-            p.addXYErr (np.arange (len (self.all_aps))[ok], mean, scat, 'DDID %d' % ddid)
-
-        p.setBounds (-0.5, len (self.all_aps) - 0.5)
-        p.setLabels ('Antpol number', 'Mean closure phase (rad)')
-        p.addHLine (0, keyText=None, zheight=-1)
-        print ('Viewing everything grouped by antpol ...')
-        p.show ()
+        for ddid, stats in self.ap_stats_by_ddid.items():
+            ok, mean, scat = postproc_mask(stats.finish(self.all_aps))
+            p.addXYErr(np.arange(len(self.all_aps))[ok], mean, scat, "DDID %d" % ddid)
+
+        p.setBounds(-0.5, len(self.all_aps) - 0.5)
+        p.setLabels("Antpol number", "Mean closure phase (rad)")
+        p.addHLine(0, keyText=None, zheight=-1)
+        print("Viewing everything grouped by antpol ...")
+        p.show()
 
         # Basepols by DDID
         data = []
         descs = []
         tostatuses = []
 
-        def bpgrid_status (pol1, pol2, ants, yx):
-            i, j = [int (_) for _ in np.floor (yx + 0.5)]
+        def bpgrid_status(pol1, pol2, ants, yx):
+            i, j = [int(_) for _ in np.floor(yx + 0.5)]
             if i < 0 or j < 0 or i >= ants.size or j >= ants.size:
-                return ''
+                return ""
 
-            ni = self._getname (ants[i])
-            nj = self._getname (ants[j])
+            ni = self._getname(ants[i])
+            nj = self._getname(ants[j])
 
             if i <= j:
-                return '%s-%s %s' % (ni, nj, util.pol_names[pol1])
-            return '%s-%s %s' % (nj, ni, util.pol_names[pol2])
+                return "%s-%s %s" % (ni, nj, util.pol_names[pol1])
+            return "%s-%s %s" % (nj, ni, util.pol_names[pol2])
 
-        for ddid, stats in self.bp_stats_by_ddid.items ():
-            mean, scat = postproc (stats.finish (self.all_bps))
+        for ddid, stats in self.bp_stats_by_ddid.items():
+            mean, scat = postproc(stats.finish(self.all_bps))
             nmean = mean / scat
-            pol1, pol2, ants, grid = grid_bp_data (self.all_bps,
-                                                   zip(self.all_bps, nmean))
-            data.append (grid)
-            descs.append ('DDID %d' % ddid)
-            tostatuses.append (lambda yx: bpgrid_status (pol1, pol2, ants, yx))
+            pol1, pol2, ants, grid = grid_bp_data(
+                self.all_bps, zip(self.all_bps, nmean)
+            )
+            data.append(grid)
+            descs.append("DDID %d" % ddid)
+            tostatuses.append(lambda yx: bpgrid_status(pol1, pol2, ants, yx))
 
-        print ('Viewing X axis: antpol1; Y axis: antpol2; iteration: DDID ...')
-        ndshow_gtk3.cycle (data, descs, tostatuses=tostatuses, run_main=True)
+        print("Viewing X axis: antpol1; Y axis: antpol2; iteration: DDID ...")
+        ndshow_gtk3.cycle(data, descs, tostatuses=tostatuses, run_main=True)
 
         # Everything by time
-        ok, mean, scat = postproc_mask (self.global_stats_by_time.finish (self.all_times))
+        ok, mean, scat = postproc_mask(self.global_stats_by_time.finish(self.all_times))
         stimes = self.all_times[ok] / 86400
-        st0 = int (np.floor (stimes.min ()))
+        st0 = int(np.floor(stimes.min()))
         stimes -= st0
-        p = om.quickXYErr (stimes, mean, scat)
-        p.addHLine (0, keyText=None, zheight=-1)
-        p.setLabels ('MJD - %d' % st0, 'Mean closure phase (rad)')
-        print ('Viewing everything grouped by time ...')
-        p.show ()
+        p = om.quickXYErr(stimes, mean, scat)
+        p.addHLine(0, keyText=None, zheight=-1)
+        p.setLabels("MJD - %d" % st0, "Mean closure phase (rad)")
+        print("Viewing everything grouped by time ...")
+        p.show()
 
 
-def closures_cli (argv):
-    check_usage (closures_doc, argv, usageifnoargs=True)
-    cfg = Config ().parse (argv[1:])
-    util.logger (cfg.loglevel)
-    ClosureCalculator ().process (cfg).report (cfg)
+def closures_cli(argv):
+    check_usage(closures_doc, argv, usageifnoargs=True)
+    cfg = Config().parse(argv[1:])
+    util.logger(cfg.loglevel)
+    ClosureCalculator().process(cfg).report(cfg)
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/cscript_flagcmd.py` & `pwkit-1.2.0/pwkit/environments/casa/cscript_flagcmd.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/cscript_genantpos.py` & `pwkit-1.2.0/pwkit/environments/casa/cscript_genantpos.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/cscript_getopacities.py` & `pwkit-1.2.0/pwkit/environments/casa/cscript_getopacities.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/cscript_importalma.py` & `pwkit-1.2.0/pwkit/environments/casa/cscript_importalma.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/cscript_importevla.py` & `pwkit-1.2.0/pwkit/environments/casa/cscript_importevla.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/cscript_plotants.py` & `pwkit-1.2.0/pwkit/environments/casa/cscript_plotants.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/cscript_plotcal.py` & `pwkit-1.2.0/pwkit/environments/casa/cscript_plotcal.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/cscript_setjy.py` & `pwkit-1.2.0/pwkit/environments/casa/cscript_setjy.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/dftdynspec.py` & `pwkit-1.2.0/pwkit/environments/casa/dftdynspec.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,28 @@
 
 """This module provides code to extract dynamic spectra from CASA Measurement
 Sets. CASA doesn't have a task that does this.
 
 """
 from __future__ import absolute_import, division, print_function
 
-__all__ = 'Config Loader dftdynspec dftdynspec_cli'.split()
+__all__ = "Config Loader dftdynspec dftdynspec_cli".split()
 
-import io, os.path, sys
+import io, os.path
 import numpy as np
-import six
-from six.moves import range
 
-from ... import binary_type, text_type
 # Note: zany spacing so that Sphinx can parse the file correctly.
-from . ..astutil import *
-from . ..cli import check_usage, die
-from . ..io import get_stdout_bytes
-from . ..kwargv import ParseKeywords, Custom
+from ...astutil import *
+from ...cli import check_usage, die
+from ...io import get_stdout_bytes
+from ...kwargv import ParseKeywords, Custom
 from . import util
 from .util import sanitize_unicode as b
 
-dftdynspec_doc = \
-"""
+dftdynspec_doc = """
 casatask dftdynspec vis=<MS> [keywords...]
 
 Extract a dynamic spectrum from the visibilities in a measurement set. See
 below the keyword docs for some important caveats.
 
 vis=
   Path of the MeasurementSet dataset to read. Required.
@@ -77,25 +73,26 @@
 
 The output data are stored as a file containing several serialized Numpy
 arrays. The Python class `pwkit.environments.casa.dftdynspec.Loader` can be
 used to load the data into a Python program.
 
 """
 
+
 class Config(ParseKeywords):
     vis = Custom(str, required=True)
-    datacol = 'data'
+    datacol = "data"
     believeweights = False
 
-    @Custom(str, uiname='out')
+    @Custom(str, uiname="out")
     def outstream(val):
         if val is None:
             return get_stdout_bytes()
         try:
-            return open(val, 'wb')
+            return open(val, "wb")
         except Exception as e:
             die('cannot open path "%s" for writing', val)
 
     @Custom([str, str], default=None)
     def rephase(val):
         if val is None:
             return None
@@ -108,23 +105,23 @@
         return ra, dec
 
     # MeasurementSet filters
     array = str
     baseline = str
     field = str
     observation = str
-    polarization = 'RR,LL'
+    polarization = "RR,LL"
     scan = str
     scanintent = str
     spw = str
     taql = str
     time = str
     uvdist = str
 
-    loglevel = 'warn'
+    loglevel = "warn"
 
 
 def dftdynspec(cfg):
     tb = util.tools.table()
     ms = util.tools.ms()
     me = util.tools.measures()
 
@@ -140,201 +137,207 @@
     # axis_info.corr_axis is (ncorr)
     # axis_info.freq_axis.chan_freq is (nchan, 1) [for now?]
     #
     # Note that we apply msselect() again when reading the data because
     # selectinit() is broken, but the invocation here is good because it
     # affects the results from ms.range() and friends.
 
-    if ':' in (cfg.spw or ''):
-        warn('it looks like you are attempting to select channels within one or more spws')
-        warn('this is NOT IMPLEMENTED; I will process the whole spw instead')
+    if ":" in (cfg.spw or ""):
+        warn(
+            "it looks like you are attempting to select channels within one or more spws"
+        )
+        warn("this is NOT IMPLEMENTED; I will process the whole spw instead")
 
     ms.open(b(cfg.vis))
     totrows = ms.nrow()
-    ms_sels = dict((n, cfg.get(n)) for n in util.msselect_keys
-                   if cfg.get(n) is not None)
+    ms_sels = dict(
+        (n, cfg.get(n)) for n in util.msselect_keys if cfg.get(n) is not None
+    )
     ms.msselect(b(ms_sels))
 
-    rangeinfo = ms.range(b'data_desc_id field_id'.split())
-    ddids = rangeinfo['data_desc_id']
-    fields = rangeinfo['field_id']
-    colnames = [cfg.datacol] + 'flag weight time axis_info'.split()
-    rephase = (cfg.rephase is not None)
+    rangeinfo = ms.range(b"data_desc_id field_id".split())
+    ddids = rangeinfo["data_desc_id"]
+    fields = rangeinfo["field_id"]
+    colnames = [cfg.datacol] + "flag weight time axis_info".split()
+    rephase = cfg.rephase is not None
 
     if fields.size != 1:
         # I feel comfortable making this a fatal error, even if we're
         # not rephasing.
-        die('selected data should contain precisely one field; got %d', fields.size)
+        die("selected data should contain precisely one field; got %d", fields.size)
 
-    tb.open(b(os.path.join(cfg.vis, 'DATA_DESCRIPTION')))
-    ddspws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    tb.open(b(os.path.join(cfg.vis, "DATA_DESCRIPTION")))
+    ddspws = tb.getcol(b"SPECTRAL_WINDOW_ID")
     tb.close()
 
     # Get frequencies and precompute merged, sorted frequency array
     # FIXME: below we get 'freqs' on the fly; should honor that.
     # But then mapping and data storage get super inefficient.
 
-    tb.open(b(os.path.join(cfg.vis, 'SPECTRAL_WINDOW')))
+    tb.open(b(os.path.join(cfg.vis, "SPECTRAL_WINDOW")))
     nspw = tb.nrows()
     spwfreqs = []
     for i in range(nspw):
-        spwfreqs.append(tb.getcell(b'CHAN_FREQ', i) * 1e-9) # -> GHz
+        spwfreqs.append(tb.getcell(b"CHAN_FREQ", i) * 1e-9)  # -> GHz
     tb.close()
 
     allfreqs = set()
     for freqs in spwfreqs:
         allfreqs.update(freqs)
     allfreqs = np.asarray(sorted(allfreqs))
     nfreq = allfreqs.size
 
     freqmaps = []
     for i in range(nspw):
         freqmaps.append(np.searchsorted(allfreqs, spwfreqs[i]))
 
     if rephase:
         fieldid = fields[0]
-        tb.open(b(os.path.join(cfg.vis, 'FIELD')))
-        phdirinfo = tb.getcell(b'PHASE_DIR', fieldid)
+        tb.open(b(os.path.join(cfg.vis, "FIELD")))
+        phdirinfo = tb.getcell(b"PHASE_DIR", fieldid)
         tb.close()
 
         if phdirinfo.shape[1] != 1:
-            die('trying to rephase but target field (#%d) has a '
-                'time-variable phase center, which I can\'t handle', fieldid)
-        ra0, dec0 = phdirinfo[:,0] # in radians.
+            die(
+                "trying to rephase but target field (#%d) has a "
+                "time-variable phase center, which I can't handle",
+                fieldid,
+            )
+        ra0, dec0 = phdirinfo[:, 0]  # in radians.
 
         # based on intflib/pwflux.py, which was copied from
         # hex/hex-lib-calcgainerr:
 
         dra = cfg.rephase[0] - ra0
         dec = cfg.rephase[1]
         l = np.sin(dra) * np.cos(dec)
         m = np.sin(dec) * np.cos(dec0) - np.cos(dra) * np.cos(dec) * np.sin(dec0)
         n = np.sin(dec) * np.sin(dec0) + np.cos(dra) * np.cos(dec) * np.cos(dec0)
-        n -= 1 # makes the work below easier
+        n -= 1  # makes the work below easier
         lmn = np.asarray([l, m, n])
-        colnames.append('uvw')
+        colnames.append("uvw")
 
     tbins = {}
     colnames = b(colnames)
 
     for ddindex, ddid in enumerate(ddids):
         # Starting in CASA 4.6, selectinit(ddid) stopped actually filtering
         # your data to match the specified DDID! What garbage. Work around
         # with our own filtering.
-        ms_sels['taql'] = 'DATA_DESC_ID == %d' % ddid
+        ms_sels["taql"] = "DATA_DESC_ID == %d" % ddid
         ms.msselect(b(ms_sels))
 
         ms.selectinit(ddid)
         if cfg.polarization is not None:
-            ms.selectpolarization(b(cfg.polarization.split(',')))
+            ms.selectpolarization(b(cfg.polarization.split(",")))
         ms.iterinit(maxrows=4096)
         ms.iterorigin()
 
         spwid = ddspws[ddid]
 
         while True:
             cols = ms.getdata(items=colnames)
 
             if rephase:
                 # With appropriate spw/DDID selection, `freqs` has shape
                 # (nchan, 1). Convert to m^-1 so we can multiply against UVW
                 # directly.
-                freqs = cols['axis_info']['freq_axis']['chan_freq']
-                assert freqs.shape[1] == 1, 'internal inconsistency, chan_freq??'
-                freqs = freqs[:,0] * util.INVERSE_C_MS
+                freqs = cols["axis_info"]["freq_axis"]["chan_freq"]
+                assert freqs.shape[1] == 1, "internal inconsistency, chan_freq??"
+                freqs = freqs[:, 0] * util.INVERSE_C_MS
 
-            for i in range(cols['time'].size): # all records
-                time = cols['time'][i]
+            for i in range(cols["time"].size):  # all records
+                time = cols["time"][i]
                 # get out of UTC as fast as we can! For some reason
                 # giving 'unit=s' below doesn't do what one might hope it would.
                 # CASA can convert to a variety of timescales; TAI is probably
                 # the safest conversion in terms of being helpful while remaining
                 # close to the fundamental data, but TT is possible and should
                 # be perfectly precise for standard applications.
-                mq = me.epoch(b'utc', b({'value': time / 86400., 'unit': 'd'}))
-                mjdtt = me.measure(b(mq), b'tt')['m0']['value']
+                mq = me.epoch(b"utc", b({"value": time / 86400.0, "unit": "d"}))
+                mjdtt = me.measure(b(mq), b"tt")["m0"]["value"]
 
                 tdata = tbins.get(mjdtt)
                 if tdata is None:
                     tdata = tbins[mjdtt] = np.zeros((nfreq, 7))
 
                 if rephase:
-                    uvw = cols['uvw'][:,i]
-                    ph = np.exp((0-2j) * np.pi * np.dot(lmn, uvw) * freqs)
+                    uvw = cols["uvw"][:, i]
+                    ph = np.exp((0 - 2j) * np.pi * np.dot(lmn, uvw) * freqs)
 
-                for j in range(cols['flag'].shape[0]): # all polns
+                for j in range(cols["flag"].shape[0]):  # all polns
                     # We just average together all polarizations right now!
                     # (Not actively, but passively by just iterating over them.)
-                    data = cols[cfg.datacol][j,:,i]
-                    flags = cols['flag'][j,:,i]
+                    data = cols[cfg.datacol][j, :, i]
+                    flags = cols["flag"][j, :, i]
 
                     # XXXXX casacore is currently broken and returns the raw
                     # weights from the dataset rather than applying the
                     # polarization selection. Fortunately all of our weights
                     # are the same, and you can never fetch more pol types
                     # than the dataset has, so this bit works despite the bug.
 
                     w = np.where(~flags)[0]
                     if not w.size:
-                        continue # all flagged
+                        continue  # all flagged
 
                     if rephase:
                         data *= ph
 
                     m = freqmaps[spwid][w]
                     d = data[w]
-                    wt = cols['weight'][j,i]
+                    wt = cols["weight"][j, i]
 
-                    tdata[m,0] += wt * d.real
-                    tdata[m,1] += wt * d.imag
-                    tdata[m,2] += wt * d.real**2
-                    tdata[m,3] += wt * d.imag**2
-                    tdata[m,4] += wt
-                    tdata[m,5] += wt**2
-                    tdata[m,6] += 1
+                    tdata[m, 0] += wt * d.real
+                    tdata[m, 1] += wt * d.imag
+                    tdata[m, 2] += wt * d.real**2
+                    tdata[m, 3] += wt * d.imag**2
+                    tdata[m, 4] += wt
+                    tdata[m, 5] += wt**2
+                    tdata[m, 6] += 1
 
             if not ms.iternext():
                 break
 
-        ms.reset() # reset selection filter so we can get next DDID
+        ms.reset()  # reset selection filter so we can get next DDID
 
     ms.close()
 
     # Could gain some efficiency by using a better data structure than a dict().
 
-    smjd = np.asarray(sorted(six.iterkeys(tbins)))
+    smjd = np.asarray(sorted(tbins.keys()))
     data = np.zeros((5, smjd.size, nfreq))
 
     for tid in range(smjd.size):
         mjd = smjd[tid]
 
         wr, wi, wr2, wi2, wt, wt2, n = tbins[mjd].T
         w = np.where(n > 0)[0]
-        if w.size < 3: # not enough data for meaningful statistics
+        if w.size < 3:  # not enough data for meaningful statistics
             continue
 
         r = wr[w] / wt[w]
         i = wi[w] / wt[w]
 
         if cfg.believeweights:
-            ru = wt[w]**-0.5
-            iu = wt[w]**-0.5
+            ru = wt[w] ** -0.5
+            iu = wt[w] ** -0.5
         else:
             r2 = wr2[w] / wt[w]
             i2 = wi2[w] / wt[w]
-            rv = r2 - r**2 # variance among real/imag msmts
+            rv = r2 - r**2  # variance among real/imag msmts
             iv = i2 - i**2
-            ru = np.sqrt(rv * wt2[w]) / wt[w] # uncert in mean real/img values
+            ru = np.sqrt(rv * wt2[w]) / wt[w]  # uncert in mean real/img values
             iu = np.sqrt(iv * wt2[w]) / wt[w]
 
-        data[0,tid,w] = r
-        data[1,tid,w] = ru
-        data[2,tid,w] = i
-        data[3,tid,w] = iu
-        data[4,tid,w] = n[w]
+        data[0, tid, w] = r
+        data[1, tid, w] = ru
+        data[2, tid, w] = i
+        data[3, tid, w] = iu
+        data[4, tid, w] = n[w]
 
     np.save(cfg.outstream, smjd)
     np.save(cfg.outstream, allfreqs)
     np.save(cfg.outstream, data)
 
 
 def dftdynspec_cli(argv):
@@ -349,14 +352,15 @@
 
     **Constructor arguments**
 
     *path*
       The path of the file to read.
 
     """
+
     mjds = None
     "A 1D sorted array of the MJDs of the data samples."
 
     freqs = None
     "A 1D sorted array of the frequencies of the data samples, measured in GHz."
 
     reals = None
@@ -380,25 +384,24 @@
 
     """
     counts = None
     """A 2D array recording the number of visibilities that went into each
     average. Shape is `(mjds.size, freqs.size)`.
 
     """
+
     def __init__(self, path):
-        with io.open(path, 'rb') as f:
+        with io.open(path, "rb") as f:
             self.mjds = np.load(f)
             self.freqs = np.load(f)
             cube = np.load(f)
             self.reals, self.u_reals, self.imags, self.u_imags, self.counts = cube
 
-
     @property
     def n_mjds(self):
         "The size of the MJD axis of the data arrays; an integer."
         return self.mjds.size
 
-
     @property
     def n_freqs(self):
         "The size of the frequency axis of the data arrays; an integer."
         return self.freqs.size
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/dftphotom.py` & `pwkit-1.2.0/pwkit/environments/casa/dftphotom.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,29 +10,26 @@
 command line, run ``casatask dftphotom --help``. The command’s help text will
 also describe some of the parameters below in more detail than is currently
 found here.
 
 """
 from __future__ import absolute_import, division, print_function
 
-__all__ = 'Config dftphotom dftphotom_cli'.split()
+__all__ = "Config dftphotom dftphotom_cli".split()
 
-import six, sys, os.path, numpy as np
-from six.moves import range
+import sys, os.path, numpy as np
 
-from ... import binary_type, text_type
 # Note: zany spacing so that Sphinx can parse the file correctly.
-from . ..astutil import *
-from . ..cli import check_usage, die, warn
-from . ..kwargv import ParseKeywords, Custom
+from ...astutil import *
+from ...cli import check_usage, die, warn
+from ...kwargv import ParseKeywords, Custom
 from . import util
 from .util import sanitize_unicode as b
 
-dftphotom_doc = \
-"""
+dftphotom_doc = """
 casatask dftphotom vis=MS [keywords...]
 
 Extract photometry from the visibilities in a measurement set. See the full
 documentation for some important caveats.
 
 vis=
   Path of the MeasurementSet dataset to read. Required.
@@ -96,72 +93,79 @@
 with sorted MJDs, one record for each timestamp present in the dataset,
 with all fluxes in ujy. dt is simply (MJD - MJD[0]) * 1440. The units
 of re, im, mag, and their uncertainties are microjansky by default,
 but see the datascale keyword, and there's no way to know if the
 data have actually been flux-calibrated or not.
 """
 
+
 class HumaneOutputFormat(object):
     def header(self, cfg):
         pass
 
     def row(self, cfg, mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n):
-        print('%12.5f %6.2f %10.2f %10.2f %10.2f %10.2f %10.2f %10.2f %d' %
-              (mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n),
-              file=cfg.outstream)
+        print(
+            "%12.5f %6.2f %10.2f %10.2f %10.2f %10.2f %10.2f %10.2f %d"
+            % (mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n),
+            file=cfg.outstream,
+        )
 
 
 class PandasOutputFormat(object):
     def header(self, cfg):
-        print('mjd dtmin re ure im uim abs uabs nsamp'.replace(' ', '\t'),
-              file=cfg.outstream)
+        print(
+            "mjd dtmin re ure im uim abs uabs nsamp".replace(" ", "\t"),
+            file=cfg.outstream,
+        )
 
     def row(self, cfg, *args):
-        print('\t'.join(str(x) for x in args), file=cfg.outstream)
+        print("\t".join(str(x) for x in args), file=cfg.outstream)
 
 
 class Config(ParseKeywords):
     vis = Custom(str, required=True)
     """The path to the visibility MeasurementSet to process. No default; you
     must specify a value before calling :func:`dftphotom`."""
 
-    datacol = 'data'
+    datacol = "data"
     """A string specifying which visibility data column to process: ``data``,
     ``corrected_data``, or ``model_data``. Default ``'data'``.
 
     """
     believeweights = False
     """Whether to trust that the data-weight information in the MS accurately
     describe the noise in their corresponding visibilities. Default False.
 
     """
-    @Custom(str, uiname='out')
+
+    @Custom(str, uiname="out")
     def outstream(val):
         if val is None:
             return sys.stdout
         try:
-            return open(val, 'w')
+            return open(val, "w")
         except Exception as e:
             die('cannot open path "%s" for writing', val)
 
     datascale = 1e6
     """The amount by which to scale the computed values before emitting them as
     text. The default is 1e6, which means that the output will be in
     microJanskys if the underlying data are calibrated to Jansky units.
 
     """
-    @Custom(str, default='humane')
+
+    @Custom(str, default="humane")
     def format(val):
-        if val is None or val == 'humane':
+        if val is None or val == "humane":
             return HumaneOutputFormat()
 
-        if val == 'pandas':
+        if val == "pandas":
             return PandasOutputFormat()
 
-        die('unrecognized output format %r', val)
+        die("unrecognized output format %r", val)
 
     @Custom([str, str], default=None)
     def rephase(val):
         if val is None:
             return None
 
         try:
@@ -172,23 +176,23 @@
         return ra, dec
 
     # MeasurementSet filters
     array = str
     baseline = str
     field = str
     observation = str
-    polarization = 'RR,LL'
+    polarization = "RR,LL"
     scan = str
     scanintent = str
     spw = str
     taql = str
     time = str
     uvdist = str
 
-    loglevel = 'warn'
+    loglevel = "warn"
 
 
 def dftphotom(cfg):
     """Run the discrete-Fourier-transform photometry algorithm.
 
     See the module-level documentation and the output of ``casatask dftphotom
     --help`` for help. All of the algorithm configuration is specified in the
@@ -211,173 +215,179 @@
     # axis_info.corr_axis is (ncorr)
     # axis_info.freq_axis.chan_freq is (nchan, 1) [for now?]
     #
     # Note that we apply msselect() again when reading the data because
     # selectinit() is broken, but the invocation here is good because it
     # affects the results from ms.range() and friends.
 
-    if ':' in (cfg.spw or ''):
-        warn('it looks like you are attempting to select channels within one or more spws')
-        warn('this is NOT IMPLEMENTED; I will average over the whole spw instead')
+    if ":" in (cfg.spw or ""):
+        warn(
+            "it looks like you are attempting to select channels within one or more spws"
+        )
+        warn("this is NOT IMPLEMENTED; I will average over the whole spw instead")
 
     ms.open(b(cfg.vis))
     totrows = ms.nrow()
-    ms_sels = dict((n, cfg.get(n)) for n in util.msselect_keys
-                   if cfg.get(n) is not None)
+    ms_sels = dict(
+        (n, cfg.get(n)) for n in util.msselect_keys if cfg.get(n) is not None
+    )
     ms.msselect(b(ms_sels))
 
-    rangeinfo = ms.range(b'data_desc_id field_id'.split())
-    ddids = rangeinfo['data_desc_id']
-    fields = rangeinfo['field_id']
-    colnames = [cfg.datacol] + 'flag weight time axis_info'.split()
-    rephase = (cfg.rephase is not None)
+    rangeinfo = ms.range(b"data_desc_id field_id".split())
+    ddids = rangeinfo["data_desc_id"]
+    fields = rangeinfo["field_id"]
+    colnames = [cfg.datacol] + "flag weight time axis_info".split()
+    rephase = cfg.rephase is not None
 
     if fields.size != 1:
         # I feel comfortable making this a fatal error, even if we're
         # not rephasing.
-        die('selected data should contain precisely one field; got %d', fields.size)
+        die("selected data should contain precisely one field; got %d", fields.size)
 
     if rephase:
         fieldid = fields[0]
-        tb.open(b(os.path.join(cfg.vis, 'FIELD')))
-        phdirinfo = tb.getcell(b'PHASE_DIR', fieldid)
+        tb.open(b(os.path.join(cfg.vis, "FIELD")))
+        phdirinfo = tb.getcell(b"PHASE_DIR", fieldid)
         tb.close()
 
         if phdirinfo.shape[1] != 1:
-            die('trying to rephase but target field (#%d) has a '
-                'time-variable phase center, which I can\'t handle', fieldid)
-        ra0, dec0 = phdirinfo[:,0] # in radians.
+            die(
+                "trying to rephase but target field (#%d) has a "
+                "time-variable phase center, which I can't handle",
+                fieldid,
+            )
+        ra0, dec0 = phdirinfo[:, 0]  # in radians.
 
         # based on intflib/pwflux.py, which was copied from
         # hex/hex-lib-calcgainerr:
 
         dra = cfg.rephase[0] - ra0
         dec = cfg.rephase[1]
         l = np.sin(dra) * np.cos(dec)
         m = np.sin(dec) * np.cos(dec0) - np.cos(dra) * np.cos(dec) * np.sin(dec0)
         n = np.sin(dec) * np.sin(dec0) + np.cos(dra) * np.cos(dec) * np.cos(dec0)
-        n -= 1 # makes the work below easier
+        n -= 1  # makes the work below easier
         lmn = np.asarray([l, m, n])
-        colnames.append('uvw')
+        colnames.append("uvw")
 
         # Also need this although 99% of the time `ddid` and `spwid` are the same
-        tb.open(b(os.path.join(cfg.vis, 'DATA_DESCRIPTION')))
-        ddspws = np.asarray(tb.getcol(b'SPECTRAL_WINDOW_ID'))
+        tb.open(b(os.path.join(cfg.vis, "DATA_DESCRIPTION")))
+        ddspws = np.asarray(tb.getcol(b"SPECTRAL_WINDOW_ID"))
         tb.close()
 
     tbins = {}
     colnames = b(colnames)
 
     for ddindex, ddid in enumerate(ddids):
         # Starting in CASA 4.6, selectinit(ddid) stopped actually filtering
         # your data to match the specified DDID! What garbage. Work around
         # with our own filtering.
-        ms_sels['taql'] = 'DATA_DESC_ID == %d' % ddid
+        ms_sels["taql"] = "DATA_DESC_ID == %d" % ddid
         ms.msselect(b(ms_sels))
 
         ms.selectinit(ddid)
         if cfg.polarization is not None:
-            ms.selectpolarization(b(cfg.polarization.split(',')))
+            ms.selectpolarization(b(cfg.polarization.split(",")))
         ms.iterinit(maxrows=4096)
         ms.iterorigin()
 
         while True:
             cols = ms.getdata(items=colnames)
 
             if rephase:
                 # With appropriate spw/DDID selection, `freqs` has shape
                 # (nchan, 1). Convert to m^-1 so we can multiply against UVW
                 # directly.
-                freqs = cols['axis_info']['freq_axis']['chan_freq']
-                assert freqs.shape[1] == 1, 'internal inconsistency, chan_freq??'
-                freqs = freqs[:,0] * util.INVERSE_C_MS
+                freqs = cols["axis_info"]["freq_axis"]["chan_freq"]
+                assert freqs.shape[1] == 1, "internal inconsistency, chan_freq??"
+                freqs = freqs[:, 0] * util.INVERSE_C_MS
 
-            for i in range(cols['time'].size): # all records
-                time = cols['time'][i]
+            for i in range(cols["time"].size):  # all records
+                time = cols["time"][i]
                 # get out of UTC as fast as we can! For some reason
                 # giving 'unit=s' below doesn't do what one might hope it would.
                 # CASA can convert to a variety of timescales; TAI is probably
                 # the safest conversion in terms of being helpful while remaining
                 # close to the fundamental data, but TT is possible and should
                 # be perfectly precise for standard applications.
-                mq = me.epoch(b'utc', b({'value': time / 86400., 'unit': 'd'}))
-                mjdtt = me.measure(b(mq), b'tt')['m0']['value']
+                mq = me.epoch(b"utc", b({"value": time / 86400.0, "unit": "d"}))
+                mjdtt = me.measure(b(mq), b"tt")["m0"]["value"]
 
                 tdata = tbins.get(mjdtt, None)
                 if tdata is None:
-                    tdata = tbins[mjdtt] = [0., 0., 0., 0., 0]
+                    tdata = tbins[mjdtt] = [0.0, 0.0, 0.0, 0.0, 0]
 
                 if rephase:
-                    uvw = cols['uvw'][:,i]
-                    ph = np.exp((0-2j) * np.pi * np.dot(lmn, uvw) * freqs)
+                    uvw = cols["uvw"][:, i]
+                    ph = np.exp((0 - 2j) * np.pi * np.dot(lmn, uvw) * freqs)
 
-                for j in range(cols['flag'].shape[0]): # all polns
+                for j in range(cols["flag"].shape[0]):  # all polns
                     # We just average together all polarizations right now!
                     # (Not actively, but passively by just iterating over them.)
-                    data = cols[cfg.datacol][j,:,i]
-                    flags = cols['flag'][j,:,i]
+                    data = cols[cfg.datacol][j, :, i]
+                    flags = cols["flag"][j, :, i]
 
                     # XXXXX casacore is currently (ca. 2012) broken and
                     # returns the raw weights from the dataset rather than
                     # applying the polarization selection. Fortunately all of
                     # our weights are the same, and you can never fetch more
                     # pol types than the dataset has, so this bit works
                     # despite the bug.
 
                     w = np.where(~flags)[0]
                     if not w.size:
-                        continue # all flagged
+                        continue  # all flagged
 
                     if rephase:
                         data *= ph
 
                     d = data[w].mean()
                     # account for flagged parts. 90% sure this is the
                     # right thing to do:
-                    wt = cols['weight'][j,i] * w.size / data.size
+                    wt = cols["weight"][j, i] * w.size / data.size
                     wd = wt * d
                     # note a little bit of a hack here to encode real^2 and
                     # imag^2 separately:
                     wd2 = wt * (d.real**2 + (1j) * d.imag**2)
 
                     tdata[0] += wd
                     tdata[1] += wd2
                     tdata[2] += wt
                     tdata[3] += wt**2
                     tdata[4] += 1
 
             if not ms.iternext():
                 break
 
-        ms.reset() # reset selection filter so we can get next DDID
+        ms.reset()  # reset selection filter so we can get next DDID
 
     ms.close()
 
     # Could gain some efficiency by using a better data structure than a dict().
-    smjd = sorted(six.iterkeys(tbins))
+    smjd = sorted(tbins.keys())
     cfg.format.header(cfg)
 
     for mjd in smjd:
         wd, wd2, wt, wt2, n = tbins[mjd]
-        if n < 3: # not enough data for meaningful statistics
+        if n < 3:  # not enough data for meaningful statistics
             continue
 
         dtmin = 1440 * (mjd - smjd[0])
         r_sc = wd.real / wt * cfg.datascale
         i_sc = wd.imag / wt * cfg.datascale
         r2_sc = wd2.real / wt * cfg.datascale**2
         i2_sc = wd2.imag / wt * cfg.datascale**2
 
         if cfg.believeweights:
             ru_sc = wt**-0.5 * cfg.datascale
             iu_sc = wt**-0.5 * cfg.datascale
         else:
-            rv_sc = r2_sc - r_sc**2 # variance among real/imag msmts
+            rv_sc = r2_sc - r_sc**2  # variance among real/imag msmts
             iv_sc = i2_sc - i_sc**2
-            ru_sc = np.sqrt(rv_sc * wt2) / wt # uncert in mean real/img values
+            ru_sc = np.sqrt(rv_sc * wt2) / wt  # uncert in mean real/img values
             iu_sc = np.sqrt(iv_sc * wt2) / wt
 
         mag = np.sqrt(r_sc**2 + i_sc**2)
         umag = np.sqrt(r_sc**2 * ru_sc**2 + i_sc**2 * iu_sc**2) / mag
         cfg.format.row(cfg, mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n)
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/dftspect.py` & `pwkit-1.2.0/pwkit/environments/casa/dftspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 """High-resolution point-source spectra from visibilities
 
 CASA doesn't yet have a task to do this.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str('Config dftspect dftspect_cli').split()
+__all__ = str("Config dftspect dftspect_cli").split()
 
-import six, sys, os.path, numpy as np
-from six.moves import range
+import sys, os.path, numpy as np
 
-from ... import binary_type, text_type
 from ...astutil import *
-from ...cli import check_usage, die
+from ...cli import die
 from ...kwargv import ParseKeywords, Custom
 from . import util
 from .util import sanitize_unicode as b
 
-dftspect_doc = \
-"""
+dftspect_doc = """
 casatask dftspect vis=<MS> [keywords...]
 
 Extract fluxes from the visibilities in a measurement set as a function of
 spectral window (and hence, presumably, frequency). See below the keyword docs
 for some important caveats.
 
 vis=
@@ -85,58 +82,63 @@
 
 sorted by frequency, where the frequency is the mean frequency of its
 associated spectral window. The units of re, im, mag, and their uncertainties
 are microjansky by default, but see the datascale keyword, and there's no way
 to know if the data have actually been flux-calibrated or not.
 """
 
+
 class HumaneOutputFormat(object):
     def header(self, cfg):
         pass
 
     def row(self, cfg, freq, spwnum, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n):
-        print('%10.2f %2d %10.2f %10.2f %10.2f %10.2f %10.2f %10.2f %d' %
-              (freq, spwnum, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n),
-              file=cfg.outstream)
+        print(
+            "%10.2f %2d %10.2f %10.2f %10.2f %10.2f %10.2f %10.2f %d"
+            % (freq, spwnum, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n),
+            file=cfg.outstream,
+        )
 
 
 class PandasOutputFormat(object):
     def header(self, cfg):
-        print('freq spwnum re ure im uim abs uabs nsamp'.replace(' ', '\t'),
-              file=cfg.outstream)
+        print(
+            "freq spwnum re ure im uim abs uabs nsamp".replace(" ", "\t"),
+            file=cfg.outstream,
+        )
 
     def row(self, cfg, *args):
-        print('\t'.join(str(x) for x in args), file=cfg.outstream)
+        print("\t".join(str(x) for x in args), file=cfg.outstream)
 
 
 class Config(ParseKeywords):
     vis = Custom(str, required=True)
-    datacol = 'data'
+    datacol = "data"
     believeweights = False
 
-    @Custom(str, uiname='out')
+    @Custom(str, uiname="out")
     def outstream(val):
         if val is None:
             return sys.stdout
         try:
-            return open(val, 'w')
+            return open(val, "w")
         except Exception as e:
             die('cannot open path "%s" for writing', val)
 
     datascale = 1e6
 
-    @Custom(str, default='humane')
+    @Custom(str, default="humane")
     def format(val):
-        if val is None or val == 'humane':
+        if val is None or val == "humane":
             return HumaneOutputFormat()
 
-        if val == 'pandas':
+        if val == "pandas":
             return PandasOutputFormat()
 
-        die('unrecognized output format %r', val)
+        die("unrecognized output format %r", val)
 
     @Custom([str, str], default=None)
     def rephase(val):
         if val is None:
             return None
 
         try:
@@ -147,23 +149,23 @@
         return ra, dec
 
     # MeasurementSet filters
     array = str
     baseline = str
     field = str
     observation = str
-    polarization = 'RR,LL'
+    polarization = "RR,LL"
     scan = str
     scanintent = str
     spw = str
     taql = str
     time = str
     uvdist = str
 
-    loglevel = 'warn'
+    loglevel = "warn"
 
 
 def dftspect(cfg):
     tb = util.tools.table()
     ms = util.tools.ms()
 
     # Read stuff in. Even if the weight values don't have their
@@ -179,158 +181,162 @@
     # axis_info.freq_axis.chan_freq is (nchan, 1) [for now?]
     #
     # Note that we apply msselect() again when reading the data because
     # selectinit() is broken, but the invocation here is good because it
     # affects the results from ms.range() and friends.
 
     ms.open(b(cfg.vis))
-    ms_sels = dict((n, cfg.get(n)) for n in util.msselect_keys
-                   if cfg.get(n) is not None)
+    ms_sels = dict(
+        (n, cfg.get(n)) for n in util.msselect_keys if cfg.get(n) is not None
+    )
     ms.msselect(b(ms_sels))
 
-    rangeinfo = ms.range(b'data_desc_id field_id'.split())
-    ddids = rangeinfo['data_desc_id']
-    fields = rangeinfo['field_id']
-    colnames = [cfg.datacol] + 'flag weight axis_info'.split()
-    rephase = (cfg.rephase is not None)
+    rangeinfo = ms.range(b"data_desc_id field_id".split())
+    ddids = rangeinfo["data_desc_id"]
+    fields = rangeinfo["field_id"]
+    colnames = [cfg.datacol] + "flag weight axis_info".split()
+    rephase = cfg.rephase is not None
 
     if fields.size != 1:
         # I feel comfortable making this a fatal error, even if we're
         # not rephasing.
-        die('selected data should contain precisely one field; got %d', fields.size)
+        die("selected data should contain precisely one field; got %d", fields.size)
 
-    tb.open(b(os.path.join(cfg.vis, 'DATA_DESCRIPTION')))
-    ddspws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    tb.open(b(os.path.join(cfg.vis, "DATA_DESCRIPTION")))
+    ddspws = tb.getcol(b"SPECTRAL_WINDOW_ID")
     tb.close()
 
-    tb.open(b(os.path.join(cfg.vis, 'SPECTRAL_WINDOW')))
+    tb.open(b(os.path.join(cfg.vis, "SPECTRAL_WINDOW")))
     spwmfreqs = np.zeros(tb.nrows())
     for i in range(spwmfreqs.size):
-        spwmfreqs[i] = tb.getcell(b'CHAN_FREQ', i).mean() * 1e-9 # -> GHz
+        spwmfreqs[i] = tb.getcell(b"CHAN_FREQ", i).mean() * 1e-9  # -> GHz
     tb.close()
 
     if rephase:
         fieldid = fields[0]
-        tb.open(b(os.path.join(cfg.vis, 'FIELD')))
-        phdirinfo = tb.getcell(b'PHASE_DIR', fieldid)
+        tb.open(b(os.path.join(cfg.vis, "FIELD")))
+        phdirinfo = tb.getcell(b"PHASE_DIR", fieldid)
         tb.close()
 
         if phdirinfo.shape[1] != 1:
-            die('trying to rephase but target field (#%d) has a '
-                'time-variable phase center, which I can\'t handle', fieldid)
-        ra0, dec0 = phdirinfo[:,0] # in radians.
+            die(
+                "trying to rephase but target field (#%d) has a "
+                "time-variable phase center, which I can't handle",
+                fieldid,
+            )
+        ra0, dec0 = phdirinfo[:, 0]  # in radians.
 
         # based on intflib/pwflux.py, which was copied from
         # hex/hex-lib-calcgainerr:
 
         dra = cfg.rephase[0] - ra0
         dec = cfg.rephase[1]
         l = np.sin(dra) * np.cos(dec)
         m = np.sin(dec) * np.cos(dec0) - np.cos(dra) * np.cos(dec) * np.sin(dec0)
         n = np.sin(dec) * np.sin(dec0) + np.cos(dra) * np.cos(dec) * np.cos(dec0)
-        n -= 1 # makes the work below easier
+        n -= 1  # makes the work below easier
         lmn = np.asarray([l, m, n])
-        colnames.append('uvw')
+        colnames.append("uvw")
 
     spwbins = {}
     colnames = b(colnames)
 
     for ddid in ddids:
         # Starting in CASA 4.6, selectinit(ddid) stopped actually filtering
         # your data to match the specified DDID! What garbage. Work around
         # with our own filtering.
-        ms_sels['taql'] = 'DATA_DESC_ID == %d' % ddid
+        ms_sels["taql"] = "DATA_DESC_ID == %d" % ddid
         ms.msselect(b(ms_sels))
 
         ms.selectinit(ddid)
         if cfg.polarization is not None:
-            ms.selectpolarization(b(cfg.polarization.split(',')))
+            ms.selectpolarization(b(cfg.polarization.split(",")))
         ms.iterinit()
         ms.iterorigin()
 
         spw = ddspws[ddid]
         sdata = spwbins.get(spw)
-        if sdata is None: # might have multiple ddids going to one spw
-            sdata = spwbins[spw] = [0., 0., 0., 0., 0]
+        if sdata is None:  # might have multiple ddids going to one spw
+            sdata = spwbins[spw] = [0.0, 0.0, 0.0, 0.0, 0]
 
         while True:
             cols = ms.getdata(items=colnames)
 
             if rephase:
                 # With appropriate spw/DDID selection, `freqs` has shape
                 # (nchan, 1). Convert to m^-1 so we can multiply against UVW
                 # directly.
-                freqs = cols['axis_info']['freq_axis']['chan_freq']
-                assert freqs.shape[1] == 1, 'internal inconsistency, chan_freq??'
-                freqs = freqs[:,0] * util.INVERSE_C_MS
+                freqs = cols["axis_info"]["freq_axis"]["chan_freq"]
+                assert freqs.shape[1] == 1, "internal inconsistency, chan_freq??"
+                freqs = freqs[:, 0] * util.INVERSE_C_MS
 
-            for i in range(cols['flag'].shape[-1]): # all records
+            for i in range(cols["flag"].shape[-1]):  # all records
                 if rephase:
-                    uvw = cols['uvw'][:,i]
-                    ph = np.exp((0-2j) * np.pi * np.dot(lmn, uvw) * freqs)
+                    uvw = cols["uvw"][:, i]
+                    ph = np.exp((0 - 2j) * np.pi * np.dot(lmn, uvw) * freqs)
 
-                for j in range(cols['flag'].shape[0]): # all polns
-                    data = cols[cfg.datacol][j,:,i]
-                    flags = cols['flag'][j,:,i]
+                for j in range(cols["flag"].shape[0]):  # all polns
+                    data = cols[cfg.datacol][j, :, i]
+                    flags = cols["flag"][j, :, i]
 
                     # XXXXX casacore is currently broken and returns the raw
                     # weights from the dataset rather than applying the
                     # polarization selection. Fortunately all of our weights
                     # are the same, and you can never fetch more pol types
                     # than the dataset has, so this bit works despite the bug.
 
                     w = np.where(~flags)[0]
                     if not w.size:
-                        continue # all flagged
+                        continue  # all flagged
 
                     if rephase:
                         data *= ph
 
                     d = data[w].mean()
                     # account for flagged parts. 90% sure this is the
                     # right thing to do:
-                    wt = cols['weight'][j,i] * w.size / data.size
+                    wt = cols["weight"][j, i] * w.size / data.size
                     wd = wt * d
                     # note a little bit of a hack here to encode real^2 and
                     # imag^2 separately:
                     wd2 = wt * (d.real**2 + (1j) * d.imag**2)
 
                     sdata[0] += wd
                     sdata[1] += wd2
                     sdata[2] += wt
                     sdata[3] += wt**2
                     sdata[4] += 1
 
             if not ms.iternext():
                 break
 
-        ms.reset() # reset selection filter so we can get next DDID
+        ms.reset()  # reset selection filter so we can get next DDID
 
     ms.close()
 
-    spws = sorted(six.iterkeys(spwbins), key=lambda s: spwmfreqs[s])
+    spws = sorted(spwbins.keys(), key=lambda s: spwmfreqs[s])
     cfg.format.header(cfg)
 
     for spw in spws:
         wd, wd2, wt, wt2, n = spwbins[spw]
-        if n < 3: # not enough data for meaningful statistics
+        if n < 3:  # not enough data for meaningful statistics
             continue
 
         r_sc = wd.real / wt * cfg.datascale
         i_sc = wd.imag / wt * cfg.datascale
         r2_sc = wd2.real / wt * cfg.datascale**2
         i2_sc = wd2.imag / wt * cfg.datascale**2
 
         if cfg.believeweights:
             ru_sc = wt**-0.5 * cfg.datascale
             iu_sc = wt**-0.5 * cfg.datascale
         else:
-            rv_sc = r2_sc - r_sc**2 # variance among real/imag msmts
+            rv_sc = r2_sc - r_sc**2  # variance among real/imag msmts
             iv_sc = i2_sc - i_sc**2
-            ru_sc = np.sqrt(rv_sc * wt2) / wt # uncert in mean real/img values
+            ru_sc = np.sqrt(rv_sc * wt2) / wt  # uncert in mean real/img values
             iu_sc = np.sqrt(iv_sc * wt2) / wt
 
         mag = np.sqrt(r_sc**2 + i_sc**2)
         umag = np.sqrt(r_sc**2 * ru_sc**2 + i_sc**2 * iu_sc**2) / mag
         cfg.format.row(cfg, spwmfreqs[spw], spw, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n)
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/gpdiagnostics.py` & `pwkit-1.2.0/pwkit/environments/casa/gpdiagnostics.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,35 @@
 """Compute diagnostics regarding the quality of gain/phase calibration.
 
 NB. The GainCal class should be generically useful.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''
+__all__ = str(
+    """
 GainCal
 EmulatedMultiStamp
 ManualStampKeyPainter
 Config
 DiagnosticsTool
 gpdiagnostics_cli
-''').split ()
+"""
+).split()
 
-import six
-from six.moves import range
 import numpy as np
 from scipy.stats import scoreatpercentile
 import omega as om, omega.render
 from pwkit.kwargv import ParseKeywords, Custom
 from pwkit.io import Path
-from pwkit import cli, numutil
+from pwkit import cli
 from pwkit.environments.casa import util
 
 
-gpdiagnostics_doc = \
-"""
+gpdiagnostics_doc = """
 casatask gpdiagnostics vis=MS [keywords...]
 
 Solve for antenna calibration gains assuming a point-source model, and
 generate diagnostic plots useful for identifying bad baselines and/or
 antennas.
 
 vis=
@@ -75,15 +74,16 @@
 
 You probably want to time-average your data before running this program (see
 `casatask split`) because it is not clever enough to average the input data on
 the fly.
 
 """
 
-class GainCal (object):
+
+class GainCal(object):
     nants = None
     "Number of unique antennas in this solution."
 
     ants = None
     """Array mapping antenna solution-local antenna indices to global antenna
     numbers.
 
@@ -110,433 +110,447 @@
     "The solved-for antenna gains; shape (nants,)."
 
     normvis = None
     """The calibrated visibilities, i.e. self.vis multiplied by self.gains
     appropriately; shape (nsamps,).
 
     """
-    def fill_from_dict (self, bybl):
-        self.nsamps = len (bybl)
 
-        seenants = set ()
-        for a1, a2 in six.viewkeys (bybl):
-            seenants.add (a1)
-            seenants.add (a2)
-        self.ants = np.array (sorted (seenants))
+    def fill_from_dict(self, bybl):
+        self.nsamps = len(bybl)
+
+        seenants = set()
+        for a1, a2 in bybl.keys():
+            seenants.add(a1)
+            seenants.add(a2)
+        self.ants = np.array(sorted(seenants))
         self.nants = self.ants.size
-        self.ant_to_antidx = dict ((num, idx) for idx, num in enumerate (self.ants))
+        self.ant_to_antidx = dict((num, idx) for idx, num in enumerate(self.ants))
 
-        self.ncontrib = np.empty ((self.nsamps,), dtype=int)
-        self.vis = np.empty ((self.nsamps,), dtype=complex)
-        self.blidxs = np.empty ((self.nsamps, 2), dtype=int)
-        self.nperant = np.zeros ((self.nants,), dtype=int)
+        self.ncontrib = np.empty((self.nsamps,), dtype=int)
+        self.vis = np.empty((self.nsamps,), dtype=complex)
+        self.blidxs = np.empty((self.nsamps, 2), dtype=int)
+        self.nperant = np.zeros((self.nants,), dtype=int)
 
-        for i, (bl, (data, flags)) in enumerate (six.viewitems (bybl)):
+        for i, (bl, (data, flags)) in enumerate(bybl.items()):
             ok = ~flags
-            self.ncontrib[i] = ok.sum ()
-            self.vis[i] = data[ok].mean ()
+            self.ncontrib[i] = ok.sum()
+            self.vis[i] = data[ok].mean()
             i1 = self.ant_to_antidx[bl[0]]
             i2 = self.ant_to_antidx[bl[1]]
             self.blidxs[i] = i1, i2
             self.nperant[i1] += 1
             self.nperant[i2] += 1
 
-
-    def solve (self):
+    def solve(self):
         if self.nants > self.nsamps:
-            cli.warn ('not enough measurements to solve: %d ants, %d samples'
-                      % (self.nants, self.nsamps))
+            cli.warn(
+                "not enough measurements to solve: %d ants, %d samples"
+                % (self.nants, self.nsamps)
+            )
             return
 
         # First solve for (log) amplitudes, which we can do as a classic
         # linear least squares problem (in log space). We're implicitly
         # modeling the source as 1+0j on all baselines, i.e., we're assuming a
         # point source and solving for amplitudes in units of the source flux
         # density.
 
-        lna_A = np.zeros ((self.nsamps, self.nants))
+        lna_A = np.zeros((self.nsamps, self.nants))
 
-        for i in range (self.nsamps):
+        for i in range(self.nsamps):
             i1, i2 = self.blidxs[i]
-            lna_A[i,i1] = 1
-            lna_A[i,i2] = 1
+            lna_A[i, i1] = 1
+            lna_A[i, i2] = 1
 
-        lna_b = np.log (np.abs (self.vis))
-        lna_x, lna_chisq, lna_rank, lna_sing = np.linalg.lstsq (lna_A, lna_b)
+        lna_b = np.log(np.abs(self.vis))
+        lna_x, lna_chisq, lna_rank, lna_sing = np.linalg.lstsq(lna_A, lna_b)
         lna_chisq = lna_chisq[0]
 
         # We just solved for log values to model visibilities; to bring
         # visibilities into model domain, we need the inverses of these
         # values. We can then normalize the amplitudes of all of the observed
         # visibilities.
 
-        amps = np.exp (-lna_x)
-        normvis = self.vis.copy ()
+        amps = np.exp(-lna_x)
+        normvis = self.vis.copy()
 
-        for i in range (self.nsamps):
+        for i in range(self.nsamps):
             i1, i2 = self.blidxs[i]
             normvis[i] *= amps[i1] * amps[i2]
 
         # Now, solve for the phases with a bespoke (but simple) iterative
         # algorithm. For each antenna we just compute the phase of the summed
         # differences between it and the "model" and alter the phase by that.
         # Loosely modeled on MIRIAD gpcal PhaseSol().
 
-        curphasors = np.ones (self.nants, dtype=complex)
-        newphasors = np.empty (self.nants, dtype=complex)
+        curphasors = np.ones(self.nants, dtype=complex)
+        newphasors = np.empty(self.nants, dtype=complex)
         tol = 1e-5
         damping = 0.9
 
-        for iter_num in range (100):
-            newphasors.fill (0)
+        for iter_num in range(100):
+            newphasors.fill(0)
 
-            for i, vis in enumerate (normvis):
+            for i, vis in enumerate(normvis):
                 i1, i2 = self.blidxs[i]
                 newphasors[i1] += curphasors[i2] * vis
-                newphasors[i2] += curphasors[i1] * np.conj (vis)
+                newphasors[i2] += curphasors[i1] * np.conj(vis)
 
-            newphasors /= np.abs (newphasors)
+            newphasors /= np.abs(newphasors)
             temp = curphasors + damping * (newphasors - curphasors)
-            temp /= np.abs (temp)
-            delta = (np.abs (temp - curphasors)**2).mean ()
-            #print ('ZZ', iter_num, delta, np.angle (temp, deg=True))
+            temp /= np.abs(temp)
+            delta = (np.abs(temp - curphasors) ** 2).mean()
+            # print ('ZZ', iter_num, delta, np.angle (temp, deg=True))
             curphasors = temp
 
             if delta < tol:
                 break
 
         # Calibrate out phases too
 
-        np.conj (curphasors, curphasors)
+        np.conj(curphasors, curphasors)
         gains = amps * curphasors
 
-        for i in range (self.nsamps):
+        for i in range(self.nsamps):
             i1, i2 = self.blidxs[i]
-            normvis[i] *= curphasors[i1] * np.conj (curphasors[i2])
+            normvis[i] *= curphasors[i1] * np.conj(curphasors[i2])
 
         self.gains = gains
         self.normvis = normvis
 
-
-    def stats (self, antnames):
+    def stats(self, antnames):
         """XXX may be out of date."""
-        nbyant = np.zeros (self.nants, dtype=int)
-        sum = np.zeros (self.nants, dtype=complex)
-        sumsq = np.zeros (self.nants)
-        q = np.abs (self.normvis - 1)
+        nbyant = np.zeros(self.nants, dtype=int)
+        sum = np.zeros(self.nants, dtype=complex)
+        sumsq = np.zeros(self.nants)
+        q = np.abs(self.normvis - 1)
 
-        for i in range (self.nsamps):
+        for i in range(self.nsamps):
             i1, i2 = self.blidxs[i]
             nbyant[i1] += 1
             nbyant[i2] += 1
             sum[i1] += q[i]
             sum[i2] += q[i]
-            sumsq[i1] += q[i]**2
-            sumsq[i2] += q[i]**2
+            sumsq[i1] += q[i] ** 2
+            sumsq[i2] += q[i] ** 2
 
         avg = sum / nbyant
-        std = np.sqrt (sumsq / nbyant - avg**2)
-        navg = 1. / np.median (avg)
-        nstd = 1. / np.median (std)
-
-        for i in range (self.nants):
-            print ('  %2d %10s %3d %f %f %f %f' %
-                   (i, antnames[i], nbyant[i], avg[i], std[i], avg[i] * navg, std[i] * nstd))
-
-
-    def get_normalized (self, antidx):
-        buff = np.empty (self.nperant[antidx], dtype=complex)
-        otherant = np.empty (self.nperant[antidx], dtype=int)
+        std = np.sqrt(sumsq / nbyant - avg**2)
+        navg = 1.0 / np.median(avg)
+        nstd = 1.0 / np.median(std)
+
+        for i in range(self.nants):
+            print(
+                "  %2d %10s %3d %f %f %f %f"
+                % (
+                    i,
+                    antnames[i],
+                    nbyant[i],
+                    avg[i],
+                    std[i],
+                    avg[i] * navg,
+                    std[i] * nstd,
+                )
+            )
+
+    def get_normalized(self, antidx):
+        buff = np.empty(self.nperant[antidx], dtype=complex)
+        otherant = np.empty(self.nperant[antidx], dtype=int)
         ofs = 0
 
-        for i in range (self.nsamps):
+        for i in range(self.nsamps):
             i1, i2 = self.blidxs[i]
 
             if i1 == antidx:
                 buff[ofs] = self.normvis[i]
                 otherant[ofs] = i2
                 ofs += 1
             elif i2 == antidx:
                 buff[ofs] = self.normvis[i]
                 otherant[ofs] = i1
                 ofs += 1
 
         return buff, self.ants[otherant]
 
 
-class Config (ParseKeywords):
-    vis = Custom (str, required=True)
+class Config(ParseKeywords):
+    vis = Custom(str, required=True)
     out = str
     dims = [800, 900]
     margins = [4, 4, 4, 4]
-    loglevel = 'warn'
-    datacol = 'data'
+    loglevel = "warn"
+    datacol = "data"
 
     array = str
     baseline = str
     field = str
     observation = str
     polarization = str
     scan = str
     scanintent = str
     spw = str
     taql = str
     time = str
     uvdist = str
 
 
-ms_selectors = frozenset ('''
+ms_selectors = frozenset(
+    """
 array baseline field observation polarization scan scanintent
 spw taql time uvdist
-'''.split ())
+""".split()
+)
 
 iter_maxrows = 1024
 
 b = util.sanitize_unicode
 
 
-class EmulatedMultiStamp (om.stamps.RStamp):
-    def __init__ (self, shape, cnum, size, fill=True):
+class EmulatedMultiStamp(om.stamps.RStamp):
+    def __init__(self, shape, cnum, size, fill=True):
         self.shape = shape
         self.cnum = cnum
         self.size = size
         self.fill = fill
 
-    def paintAt (self, ctxt, style, x, y):
-        symfunc = style.data.getStrictSymbolFunc (self.shape)
-        c = style.colors.getDataColor (self.cnum)
-
-        ctxt.save ()
-        om.styles.apply_color (ctxt, c)
-        ctxt.translate (x, y)
-        symfunc (ctxt, style, self.size, self.fill)
-        ctxt.restore ()
+    def paintAt(self, ctxt, style, x, y):
+        symfunc = style.data.getStrictSymbolFunc(self.shape)
+        c = style.colors.getDataColor(self.cnum)
+
+        ctxt.save()
+        om.styles.apply_color(ctxt, c)
+        ctxt.translate(x, y)
+        symfunc(ctxt, style, self.size, self.fill)
+        ctxt.restore()
 
 
-class ManualStampKeyPainter (om.rect.GenericKeyPainter):
-    def __init__ (self, keytext, stamp, stampstyle=None):
+class ManualStampKeyPainter(om.rect.GenericKeyPainter):
+    def __init__(self, keytext, stamp, stampstyle=None):
         self.keytext = keytext
         self.stamp = stamp
         self.stampStyle = stampstyle
-        stamp.setData ('no data allowed for key-only stamp')
+        stamp.setData("no data allowed for key-only stamp")
 
-    def _getText (self):
+    def _getText(self):
         return self.keytext
 
-    def _drawLine (self):
+    def _drawLine(self):
         return False
 
-    def _drawStamp (self):
+    def _drawStamp(self):
         return True
 
-    def _drawRegion (self):
+    def _drawRegion(self):
         return False
 
-    def _applyStampStyle (self, style, ctxt):
-        style.apply (ctxt, self.stampStyle)
+    def _applyStampStyle(self, style, ctxt):
+        style.apply(ctxt, self.stampStyle)
 
-    def _getStamp (self):
+    def _getStamp(self):
         return self.stamp
 
 
-class DiagnosticsTool (object):
-    def __init__ (self, cfg):
+class DiagnosticsTool(object):
+    def __init__(self, cfg):
         self.cfg = cfg
 
-
-    def start_chunk (self):
+    def start_chunk(self):
         self.buffer = {}
 
-
-    def finish_chunk (self, *key):
-        if not len (self.buffer):
+    def finish_chunk(self, *key):
+        if not len(self.buffer):
             return
 
         spw, time = key
 
-        for polname, bybl in six.viewitems (self.buffer):
-            self.finish_polarization (spw, time, polname, bybl)
+        for polname, bybl in self.buffer.items():
+            self.finish_polarization(spw, time, polname, bybl)
 
-
-    def finish_polarization (self, spw, time, polname, bybl):
-        gc = GainCal ()
-        gc.fill_from_dict (bybl)
-        gc.solve ()
+    def finish_polarization(self, spw, time, polname, bybl):
+        gc = GainCal()
+        gc.fill_from_dict(bybl)
+        gc.solve()
         self.results[spw, polname, time] = gc
 
-
-    def load (self):
-        vis = Path (self.cfg.vis)
-        tb = util.tools.table ()
-        ms = util.tools.ms ()
+    def load(self):
+        vis = Path(self.cfg.vis)
+        tb = util.tools.table()
+        ms = util.tools.ms()
 
         # Polarization info
 
-        tb.open (b(vis / 'DATA_DESCRIPTION'))
-        ddid_to_pid = tb.getcol (b'POLARIZATION_ID')
-        ddid_to_spwid = tb.getcol (b'SPECTRAL_WINDOW_ID')
-        tb.close ()
+        tb.open(b(vis / "DATA_DESCRIPTION"))
+        ddid_to_pid = tb.getcol(b"POLARIZATION_ID")
+        ddid_to_spwid = tb.getcol(b"SPECTRAL_WINDOW_ID")
+        tb.close()
 
-        tb.open (b(vis / 'POLARIZATION'))
-        numcorrs = tb.getcol (b'NUM_CORR')
+        tb.open(b(vis / "POLARIZATION"))
+        numcorrs = tb.getcol(b"NUM_CORR")
         npids = numcorrs.size
         prodinfo = [None] * npids
 
-        for i in range (npids):
-            corrtypes = tb.getcell (b'CORR_TYPE', i)
-            prodinfo[i] = [(j, util.pol_names[c])  for j, c in enumerate (corrtypes)
-                           if util.pol_is_intensity[c]]
+        for i in range(npids):
+            corrtypes = tb.getcell(b"CORR_TYPE", i)
+            prodinfo[i] = [
+                (j, util.pol_names[c])
+                for j, c in enumerate(corrtypes)
+                if util.pol_is_intensity[c]
+            ]
 
-        tb.close ()
+        tb.close()
 
         ddprods = [prodinfo[p] for p in ddid_to_pid]
 
         # Antenna info
 
-        tb.open (b(vis / 'ANTENNA'))
-        nants = tb.getcol (b'DISH_DIAMETER').size
-        names = tb.getcol (b'NAME')
-        stations = tb.getcol (b'STATION')
-        self.antnames = ['%s@%s' % (names[i], stations[i]) for i in range (nants)]
+        tb.open(b(vis / "ANTENNA"))
+        nants = tb.getcol(b"DISH_DIAMETER").size
+        names = tb.getcol(b"NAME")
+        stations = tb.getcol(b"STATION")
+        self.antnames = ["%s@%s" % (names[i], stations[i]) for i in range(nants)]
 
         # Open and set up filtering. msselect() says it supports 'polarization' as
         # a field, but it doesn't seem to do anything?
 
-        ms.open (b(vis))
+        ms.open(b(vis))
 
         mssel = {}
         for sel in ms_selectors:
-            val = getattr (self.cfg, sel, None)
+            val = getattr(self.cfg, sel, None)
             if val is not None:
                 mssel[sel] = val
-        ms.msselect (b(mssel))
+        ms.msselect(b(mssel))
 
         totrows = 0
         curkey = ()
         self.results = {}
-        self.start_chunk ()
+        self.start_chunk()
 
-        colnames = b([self.cfg.datacol] +
-                     'time antenna1 antenna2 data_desc_id flag uvw'.split ())
-        ms.iterinit (maxrows=iter_maxrows)
-        ms.iterorigin ()
+        colnames = b(
+            [self.cfg.datacol] + "time antenna1 antenna2 data_desc_id flag uvw".split()
+        )
+        ms.iterinit(maxrows=iter_maxrows)
+        ms.iterorigin()
 
         while True:
-            cols = ms.getdata (items=colnames)
+            cols = ms.getdata(items=colnames)
             if self.cfg.datacol not in cols:
-                raise Exception ('no such data column %s' % self.cfg.datacol)
+                raise Exception("no such data column %s" % self.cfg.datacol)
 
             # flag and data are (npol, nchan, nrows)
             #   [`data` is complex128!!! converting is super slow and sad :-(]
             # uvw is (3, nrows)
             # rest are scalars, shape (nrows,)
 
-            nrows = cols['time'].size
+            nrows = cols["time"].size
             data = cols[self.cfg.datacol]
-            flags = cols['flag']
+            flags = cols["flag"]
 
-            for i in range (nrows):
-                bl = (cols['antenna1'][i], cols['antenna2'][i])
+            for i in range(nrows):
+                bl = (cols["antenna1"][i], cols["antenna2"][i])
                 if bl[0] == bl[1]:
                     continue
 
-                t = cols['time'][i] / 86400. # CASA to MJD
-                ddid = cols['data_desc_id'][i]
+                t = cols["time"][i] / 86400.0  # CASA to MJD
+                ddid = cols["data_desc_id"][i]
                 spw = ddid_to_spwid[ddid]
                 pi = ddprods[ddid]
-                npol = len (pi)
+                npol = len(pi)
                 totrows += 1
-                key = (spw, t) # XXX being cavalier about ddid vs spwid
+                key = (spw, t)  # XXX being cavalier about ddid vs spwid
 
                 if key != curkey:
-                    self.finish_chunk (*curkey)
+                    self.finish_chunk(*curkey)
                     curkey = key
-                    self.start_chunk ()
+                    self.start_chunk()
 
                 for j, polname in pi:
-                    #uvw = cols['uvw'][:,i] * util.INVERSE_C_MNS
-                    d = data[j,:,i]
-                    f = flags[j,:,i]
-                    if not np.all (f):
-                        self.buffer.setdefault (polname, {})[bl] = (d, f)
+                    # uvw = cols['uvw'][:,i] * util.INVERSE_C_MNS
+                    d = data[j, :, i]
+                    f = flags[j, :, i]
+                    if not np.all(f):
+                        self.buffer.setdefault(polname, {})[bl] = (d, f)
 
-            if not ms.iternext ():
+            if not ms.iternext():
                 break
 
-        ms.close ()
-        self.finish_chunk (*curkey)
+        ms.close()
+        self.finish_chunk(*curkey)
 
-
-    def plot (self):
-        if isinstance (self.cfg.out, omega.render.Pager):
+    def plot(self):
+        if isinstance(self.cfg.out, omega.render.Pager):
             # This is for non-CLI invocation.
             pager = self.cfg.out
         elif self.cfg.out is None:
             from omega import gtk3
-            pager = om.makeDisplayPager ()
+
+            pager = om.makeDisplayPager()
         else:
-            pager = om.makePager (self.cfg.out,
-                                  dims=self.cfg.dims,
-                                  margins=self.cfg.margins,
-                                  style=om.styles.ColorOnWhiteVector ())
+            pager = om.makePager(
+                self.cfg.out,
+                dims=self.cfg.dims,
+                margins=self.cfg.margins,
+                style=om.styles.ColorOnWhiteVector(),
+            )
 
         # Collect the data as loaded
 
-        skeys = sorted (six.viewkeys (self.results))
+        skeys = sorted(self.results.keys())
         normalized = {}
-        spws = set ()
-        polns = set ()
+        spws = set()
+        polns = set()
 
-        for antnum, antname in enumerate (self.antnames):
+        for antnum, antname in enumerate(self.antnames):
             for key in skeys:
                 spw, poln, time = key
                 gc = self.results[key]
-                idx = gc.ant_to_antidx.get (antnum)
+                idx = gc.ant_to_antidx.get(antnum)
                 if idx is None:
                     continue
 
-                samps, otherant = gc.get_normalized (idx)
-                bysp = normalized.setdefault (antname, {})
-                bytime = bysp.setdefault ((spw, poln), {})
+                samps, otherant = gc.get_normalized(idx)
+                bysp = normalized.setdefault(antname, {})
+                bytime = bysp.setdefault((spw, poln), {})
                 bytime[time] = (samps, otherant)
-                polns.add (poln)
-                spws.add (spw)
+                polns.add(poln)
+                spws.add(spw)
 
-        spws = sorted (spws)
-        polns = sorted (polns)
-        spwseq = dict ((s, i) for (i, s) in enumerate (spws))
-        polnseq = dict ((p, i) for (i, p) in enumerate (polns))
+        spws = sorted(spws)
+        polns = sorted(polns)
+        spwseq = dict((s, i) for (i, s) in enumerate(spws))
+        polnseq = dict((p, i) for (i, p) in enumerate(polns))
 
         # Group by time and get dims
 
         rmin = rmax = imin = imax = amin = amax = None
 
-        for antname, bysp in six.viewitems (normalized):
-            for spwpol in list (six.viewkeys (bysp)):
+        for antname, bysp in normalized.items():
+            for spwpol in list(bysp.keys()):
                 bytime = bysp[spwpol]
-                times = sorted (six.viewkeys (bytime))
-                samps = np.concatenate (tuple (bytime[t][0] for t in times))
-                otherants = np.concatenate (tuple (bytime[t][1] for t in times))
-                logamps = np.log10 (np.abs (samps))
+                times = sorted(bytime.keys())
+                samps = np.concatenate(tuple(bytime[t][0] for t in times))
+                otherants = np.concatenate(tuple(bytime[t][1] for t in times))
+                logamps = np.log10(np.abs(samps))
                 bysp[spwpol] = samps, otherants, logamps
 
                 if rmin is None:
-                    rmin = samps.real.min ()
-                    rmax = samps.real.max ()
-                    imin = samps.imag.min ()
-                    imax = samps.imag.max ()
-                    amin = logamps.min ()
-                    amax = logamps.max ()
+                    rmin = samps.real.min()
+                    rmax = samps.real.max()
+                    imin = samps.imag.min()
+                    imax = samps.imag.max()
+                    amin = logamps.min()
+                    amax = logamps.max()
                 else:
-                    rmin = min (rmin, samps.real.min ())
-                    rmax = max (rmax, samps.real.max ())
-                    imin = min (imin, samps.imag.min ())
-                    imax = max (imax, samps.imag.max ())
-                    amin = min (amin, logamps.min ())
-                    amax = max (amax, logamps.max ())
+                    rmin = min(rmin, samps.real.min())
+                    rmax = max(rmax, samps.real.max())
+                    imin = min(imin, samps.imag.min())
+                    imax = max(imax, samps.imag.max())
+                    amin = min(amin, logamps.min())
+                    amax = max(amax, logamps.max())
 
         # Square things up in the real/imag plot and add little margins
 
         rrange = rmax - rmin
         irange = imax - imin
         arange = amax - amin
 
@@ -556,98 +570,124 @@
         imax += 0.05 * irange
         imin -= 0.05 * irange
         amax += 0.05 * arange
         amin -= 0.05 * arange
 
         # Info for overplotted cumulative histogram of log-ampls
 
-        def getlogamps ():
-            for bysp in six.viewvalues (normalized):
-                for samps, otherant, logamp in six.viewvalues (bysp):
+        def getlogamps():
+            for bysp in normalized.values():
+                for samps, otherant, logamp in bysp.values():
                     yield logamp
 
-        all_log_amps = np.concatenate (tuple (getlogamps ()))
-        all_log_amps.sort ()
-        all_log_amps_x = np.linspace (0., len (self.antnames), all_log_amps.size)
-        all_log_amps_bounds = scoreatpercentile (all_log_amps, [2.5, 97.5])
+        all_log_amps = np.concatenate(tuple(getlogamps()))
+        all_log_amps.sort()
+        all_log_amps_x = np.linspace(0.0, len(self.antnames), all_log_amps.size)
+        all_log_amps_bounds = scoreatpercentile(all_log_amps, [2.5, 97.5])
 
         # Actually plot
 
         for antname in self.antnames:
-            bysp = normalized.get (antname)
+            bysp = normalized.get(antname)
             if bysp is None:
-                continue # no data
+                continue  # no data
 
-            reim = om.RectPlot ()
-            reim.addKeyItem (antname)
-            reim.addHLine (0, keyText=None, zheight=-2, dsn=0, lineStyle={'color': (0,0,0), 'dashing': (2, 2)})
-            reim.addVLine (1, keyText=None, zheight=-2, dsn=0, lineStyle={'color': (0,0,0), 'dashing': (2, 2)})
-
-            loga = om.RectPlot ()
-            loga.addHLine (0, keyText=None, zheight=-2, dsn=0, lineStyle={'color': (0,0,0), 'dashing': (2, 2)})
-            loga.addXY (all_log_amps_x, all_log_amps, None, lineStyle={'color': (0,0,0)})
+            reim = om.RectPlot()
+            reim.addKeyItem(antname)
+            reim.addHLine(
+                0,
+                keyText=None,
+                zheight=-2,
+                dsn=0,
+                lineStyle={"color": (0, 0, 0), "dashing": (2, 2)},
+            )
+            reim.addVLine(
+                1,
+                keyText=None,
+                zheight=-2,
+                dsn=0,
+                lineStyle={"color": (0, 0, 0), "dashing": (2, 2)},
+            )
+
+            loga = om.RectPlot()
+            loga.addHLine(
+                0,
+                keyText=None,
+                zheight=-2,
+                dsn=0,
+                lineStyle={"color": (0, 0, 0), "dashing": (2, 2)},
+            )
+            loga.addXY(
+                all_log_amps_x, all_log_amps, None, lineStyle={"color": (0, 0, 0)}
+            )
             for a in all_log_amps_bounds:
-                loga.addHLine (a, keyText=None, zheight=-2, dsn=0, lineStyle={'color': (0,0,0), 'dashing': (1, 3)})
+                loga.addHLine(
+                    a,
+                    keyText=None,
+                    zheight=-2,
+                    dsn=0,
+                    lineStyle={"color": (0, 0, 0), "dashing": (1, 3)},
+                )
 
-            for (spw, poln), (samps, otherant, logamp) in six.viewitems (bysp):
+            for (spw, poln), (samps, otherant, logamp) in bysp.items():
                 # Real/imag plot
-                ms = om.stamps.MultiStamp ('cnum', 'shape', 'tlines')
+                ms = om.stamps.MultiStamp("cnum", "shape", "tlines")
                 ms.fixedsize = 4
-                ms.fixedlinestyle = {'color': 'muted'}
+                ms.fixedlinestyle = {"color": "muted"}
 
-                cnum = np.zeros (samps.size, dtype=int)
-                cnum.fill (spwseq[spw])
+                cnum = np.zeros(samps.size, dtype=int)
+                cnum.fill(spwseq[spw])
 
-                shape = np.zeros_like (cnum)
-                shape.fill (polnseq[poln])
+                shape = np.zeros_like(cnum)
+                shape.fill(polnseq[poln])
 
-                dp = om.rect.XYDataPainter (lines=False, pointStamp=ms, keyText=None)
-                dp.setInts (cnum, shape, otherant + 1)
-                dp.setFloats (samps.real, samps.imag)
-                reim.add (dp)
+                dp = om.rect.XYDataPainter(lines=False, pointStamp=ms, keyText=None)
+                dp.setInts(cnum, shape, otherant + 1)
+                dp.setFloats(samps.real, samps.imag)
+                reim.add(dp)
 
                 # Log-amplitudes plot
-                ms = om.stamps.MultiStamp ('cnum', 'shape', 'tlines')
+                ms = om.stamps.MultiStamp("cnum", "shape", "tlines")
                 ms.fixedsize = 4
-                ms.fixedlinestyle = {'color': 'muted'}
+                ms.fixedlinestyle = {"color": "muted"}
 
-                cnum = np.zeros (samps.size, dtype=int)
-                cnum.fill (spwseq[spw])
+                cnum = np.zeros(samps.size, dtype=int)
+                cnum.fill(spwseq[spw])
 
-                shape = np.zeros_like (cnum)
-                shape.fill (polnseq[poln])
+                shape = np.zeros_like(cnum)
+                shape.fill(polnseq[poln])
 
-                dp = om.rect.XYDataPainter (lines=False, pointStamp=ms, keyText=None)
-                dp.setInts (cnum, shape, otherant + 1)
-                dp.setFloats (otherant, np.log10 (np.abs (samps)))
-                loga.add (dp)
+                dp = om.rect.XYDataPainter(lines=False, pointStamp=ms, keyText=None)
+                dp.setInts(cnum, shape, otherant + 1)
+                dp.setFloats(otherant, np.log10(np.abs(samps)))
+                loga.add(dp)
 
             for spw in spws:
                 for poln in polns:
-                    s = EmulatedMultiStamp (polnseq[poln], spwseq[spw], 4)
-                    reim.addKeyItem (ManualStampKeyPainter ('spw#%d %s' % (spw, poln), s))
+                    s = EmulatedMultiStamp(polnseq[poln], spwseq[spw], 4)
+                    reim.addKeyItem(ManualStampKeyPainter("spw#%d %s" % (spw, poln), s))
 
-            reim.setLabels ('Normalized real part', 'Normalized imaginary part')
-            reim.setBounds (rmin, rmax, imin, imax)
+            reim.setLabels("Normalized real part", "Normalized imaginary part")
+            reim.setBounds(rmin, rmax, imin, imax)
             # Unfortunately this is not compatible with VBox layout right now.
-            #reim.fieldAspect = 1.
+            # reim.fieldAspect = 1.
 
-            loga.setLabels ('Paired antenna number', 'Log10 amplitude ratio')
-            loga.setBounds (-0.5, len (self.antnames) + 0.5, amin, amax)
+            loga.setLabels("Paired antenna number", "Log10 amplitude ratio")
+            loga.setBounds(-0.5, len(self.antnames) + 0.5, amin, amax)
 
-            vb = om.layout.VBox (2)
+            vb = om.layout.VBox(2)
             vb[0] = reim
             vb[1] = loga
-            vb.setWeight (0, 3)
-            pager.send (vb)
+            vb.setWeight(0, 3)
+            pager.send(vb)
 
-        pager.done ()
+        pager.done()
 
 
-def gpdiagnostics_cli (argv):
-    cli.check_usage (gpdiagnostics_doc, argv, usageifnoargs=True)
-    cfg = Config ().parse (argv[1:])
-    util.logger (cfg.loglevel)
+def gpdiagnostics_cli(argv):
+    cli.check_usage(gpdiagnostics_doc, argv, usageifnoargs=True)
+    cfg = Config().parse(argv[1:])
+    util.logger(cfg.loglevel)
 
-    tool = DiagnosticsTool (cfg)
-    tool.load ()
-    tool.plot ()
+    tool = DiagnosticsTool(cfg)
+    tool.load()
+    tool.plot()
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/polmodel.py` & `pwkit-1.2.0/pwkit/environments/casa/polmodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,193 +3,206 @@
 # Licensed under the MIT License.
 
 """Insert a simple polarized point source model into a dataset.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('Config polmodel polmodel_cli').split ()
+__all__ = str("Config polmodel polmodel_cli").split()
 
-import six, numpy as np, tempfile
-from six.moves import range
+import numpy as np, tempfile
 
 from ...astutil import A2R, D2R, sphdist
 from ...cli import check_usage, die
 from ...io import Path
 from ...kwargv import ParseKeywords, Custom
 from . import util
 from .util import sanitize_unicode as b
 
-polmodel_doc = \
-"""
+polmodel_doc = """
 casatask polmodel vis=<MS> field=<field specification>
 
 Insert polarization information for a model into a Measurement Set. Uses a
 built-in table of polarization properties to generate Stokes QUV information
 from CASA's built-in Stokes I models.
 
 The only currently supported source is 3C286 in C band.
 
 """
 
-class Config (ParseKeywords):
-    vis = Custom (str, required=True)
-    field = Custom (str, required=True)
+
+class Config(ParseKeywords):
+    vis = Custom(str, required=True)
+    field = Custom(str, required=True)
 
 
-class PolSource (object):
-    name = None # fed to imager.predictcomp(objname)
-    ra = None # rad
-    dec = None # rad
+class PolSource(object):
+    name = None  # fed to imager.predictcomp(objname)
+    ra = None  # rad
+    dec = None  # rad
     models = None
 
-    def __init__ (self, **kwargs):
-        self.__dict__.update (kwargs)
+    def __init__(self, **kwargs):
+        self.__dict__.update(kwargs)
 
 
-class PolModel (object):
+class PolModel(object):
     name = None
-    fmin = None # GHz
-    fmax = None # GHz
-    polfrac = None # [0,1]
-    polpa = None # degr
+    fmin = None  # GHz
+    fmax = None  # GHz
+    polfrac = None  # [0,1]
+    polpa = None  # degr
 
-    def __init__ (self, **kwargs):
-        self.__dict__.update (kwargs)
+    def __init__(self, **kwargs):
+        self.__dict__.update(kwargs)
 
-    def getquv (self, i):
+    def getquv(self, i):
         # In the future, we might have different models that derive QUV
         # from I in a different way. Probably won't, though.
 
         a = self.polpa * D2R
         p = i * self.polfrac
-        return p * np.cos (a), p * np.sin (a), 0.
+        return p * np.cos(a), p * np.sin(a), 0.0
 
 
 position_tolerance = 1 * A2R
-fluxscale_standard = 'Perley-Butler 2010'
+fluxscale_standard = "Perley-Butler 2010"
 
 sources = [
-    PolSource (name='3C286', ra=-2.74392753, dec=0.53248521,
-               models=[PolModel (name='C', fmin=3.9, fmax=8.1, polfrac=0.112, polpa=66.)])
-    ]
+    PolSource(
+        name="3C286",
+        ra=-2.74392753,
+        dec=0.53248521,
+        models=[PolModel(name="C", fmin=3.9, fmax=8.1, polfrac=0.112, polpa=66.0)],
+    )
+]
 
 
-def polmodel (cfg):
-    ms = util.tools.ms ()
-    tb = util.tools.table ()
-    im = util.tools.imager ()
-    cl = util.tools.componentlist ()
-    vis = Path (cfg.vis)
+def polmodel(cfg):
+    ms = util.tools.ms()
+    tb = util.tools.table()
+    im = util.tools.imager()
+    cl = util.tools.componentlist()
+    vis = Path(cfg.vis)
 
     # Set up MS selection so we know what data we actually care about.
 
-    ms.open (b(cfg.vis))
-    ms.msselect (b(dict (field=cfg.field)))
-    rangeinfo = ms.range (b'data_desc_id field_id'.split ())
-    ddids = rangeinfo['data_desc_id']
-    fields = rangeinfo['field_id']
+    ms.open(b(cfg.vis))
+    ms.msselect(b(dict(field=cfg.field)))
+    rangeinfo = ms.range(b"data_desc_id field_id".split())
+    ddids = rangeinfo["data_desc_id"]
+    fields = rangeinfo["field_id"]
 
     # Check that we know the field and pull up its model
 
     if fields.size != 1:
-        die ('selection should pick exactly one field, but got %d', fields.size)
+        die("selection should pick exactly one field, but got %d", fields.size)
 
-    tb.open (b(vis / 'FIELD'))
-    refdir = tb.getcell (b'REFERENCE_DIR', fields[0])
-    tb.close ()
+    tb.open(b(vis / "FIELD"))
+    refdir = tb.getcell(b"REFERENCE_DIR", fields[0])
+    tb.close()
 
     if refdir.shape[1] != 1:
-        die ('selected field %s has a time-variable reference direction, which I can\'t handle', cfg.field)
+        die(
+            "selected field %s has a time-variable reference direction, which I can't handle",
+            cfg.field,
+        )
 
-    ra, dec = refdir[:,0]
+    ra, dec = refdir[:, 0]
 
     for source in sources:
-        if sphdist (dec, ra, source.dec, source.ra) < position_tolerance:
+        if sphdist(dec, ra, source.dec, source.ra) < position_tolerance:
             break
     else:
-        die ('found no match in my data table for field %s', cfg.field)
+        die("found no match in my data table for field %s", cfg.field)
 
     # Now we can get the spws and check that we have a model for them.
 
-    tb.open (b(vis / 'DATA_DESCRIPTION'))
-    ddspws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    tb.close ()
+    tb.open(b(vis / "DATA_DESCRIPTION"))
+    ddspws = tb.getcol(b"SPECTRAL_WINDOW_ID")
+    tb.close()
 
-    spws = list (set (ddspws[ddid] for ddid in ddids))
+    spws = list(set(ddspws[ddid] for ddid in ddids))
 
     freqranges = {}
     models = {}
     allfreqs = []
-    tb.open (b(vis / 'SPECTRAL_WINDOW'))
+    tb.open(b(vis / "SPECTRAL_WINDOW"))
 
     for spw in spws:
-        freqs = tb.getcell (b'CHAN_FREQ', spw)
+        freqs = tb.getcell(b"CHAN_FREQ", spw)
         freqranges[spw] = (freqs[0], freqs[-1])
         allfreqs += [freqs[0], freqs[-1]]
 
         for model in source.models:
             if freqs[0] >= model.fmin * 1e9 and freqs[-1] <= model.fmax * 1e9:
                 models[spw] = model
                 break
         else:
-            die ('spw %d is out of frequency bounds for all of my models of '
-                 'field %s (%s): spw range is (%f, %f) GHz', spw, cfg.field,
-                 source.name, freqs[0] * 1e-9, freqs[-1] * 1e-9)
+            die(
+                "spw %d is out of frequency bounds for all of my models of "
+                "field %s (%s): spw range is (%f, %f) GHz",
+                spw,
+                cfg.field,
+                source.name,
+                freqs[0] * 1e-9,
+                freqs[-1] * 1e-9,
+            )
 
-    tb.close ()
+    tb.close()
 
     # Now it's worth using predictcomp() to get the Stokes I fluxes.
 
-    workdir = tempfile.mkdtemp (prefix='mspolmodel')
+    workdir = tempfile.mkdtemp(prefix="mspolmodel")
     try:
-        cp = im.predictcomp (
-            objname = b(source.name),
-            standard = b(fluxscale_standard),
-            freqs = allfreqs,
-            pfx = b(workdir + '/')
+        cp = im.predictcomp(
+            objname=b(source.name),
+            standard=b(fluxscale_standard),
+            freqs=allfreqs,
+            pfx=b(workdir + "/"),
         )
-        cl.open (cp)
-        if cl.length () != 1:
-            die ('expected one component in predicted list; got %d (%s)',
-                 cl.length (), cp)
-        stokesi = cl.getcomponent (0)['spectrum']['ival']
+        cl.open(cp)
+        if cl.length() != 1:
+            die(
+                "expected one component in predicted list; got %d (%s)", cl.length(), cp
+            )
+        stokesi = cl.getcomponent(0)["spectrum"]["ival"]
         # log=False: we'll have to run the risk that the user won't be aware that
         # we closed the component list structure. Scary.
-        cl.close (log=False)
+        cl.close(log=False)
     finally:
-        Path (workdir).rmtree ()
+        Path(workdir).rmtree()
 
     # And now we have everything we need. Invoke setjy() a bunch.
 
-    im.open (b(vis), usescratch=False)
+    im.open(b(vis), usescratch=False)
 
-    for i, spw in enumerate (spws):
+    for i, spw in enumerate(spws):
         model = models[spw]
         f1, f2 = freqranges[spw]
-        i1, i2 = stokesi[i*2:i*2+2]
+        i1, i2 = stokesi[i * 2 : i * 2 + 2]
 
-        spindex = np.log (i2 / i1) / np.log (f2 / f1)
-        q, u, v = model.getquv (i1)
-        reffreq = '%.3fMHz' % (f1 * 1e-6)
+        spindex = np.log(i2 / i1) / np.log(f2 / f1)
+        q, u, v = model.getquv(i1)
+        reffreq = "%.3fMHz" % (f1 * 1e-6)
 
-        #print ('%2d/%d: %d %.3f-%.3f %.3f-%.3f [%.3f %.3f %.3f %3f] %.3f %s' \
+        # print ('%2d/%d: %d %.3f-%.3f %.3f-%.3f [%.3f %.3f %.3f %3f] %.3f %s' \
         #      % (i + 1, len (spws), spw, f1*1e-9, f2*1e-9, i1, i2,
         #         i1, q, u, v, spindex, reffreq))
-        im.setjy (
-            field = b(cfg.field),
-            spw = b(str(spw)),
-            modimage = b'',
-            fluxdensity = [i1, q, u, v],
-            spix = spindex,
-            standard = b(fluxscale_standard),
-            scalebychan = True,
-            reffreq = b(reffreq),
+        im.setjy(
+            field=b(cfg.field),
+            spw=b(str(spw)),
+            modimage=b"",
+            fluxdensity=[i1, q, u, v],
+            spix=spindex,
+            standard=b(fluxscale_standard),
+            scalebychan=True,
+            reffreq=b(reffreq),
         )
 
-    im.close ()
+    im.close()
 
 
-def polmodel_cli (argv):
-    check_usage (polmodel_doc, argv, usageifnoargs=True)
-    cfg = Config ().parse (argv[1:])
-    polmodel (cfg)
+def polmodel_cli(argv):
+    check_usage(polmodel_doc, argv, usageifnoargs=True)
+    cfg = Config().parse(argv[1:])
+    polmodel(cfg)
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/scripting.py` & `pwkit-1.2.0/pwkit/environments/casa/scripting.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 write standalone scripts with a hashbang line of "#! /usr/bin/env
 pkcasascript" -- hashbang lines support only one extra command-line
 argument, so if we're using "env" we can't take a multitool approach.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str('CasapyScript commandline').split()
+__all__ = str("CasapyScript commandline").split()
 
-import os.path, shutil, signal, six, sys, tempfile
+import os.path, shutil, signal, sys, tempfile
 from ... import PKError, cli, reraise_context
 from . import CasaEnvironment
 
 
-casapy_argv = ['casa', '--log2term', '--nogui', '-c']
+casapy_argv = ["casa", "--log2term", "--nogui", "-c"]
 
 signals_for_child = [
     signal.SIGHUP,
     signal.SIGINT,
     signal.SIGQUIT,
     signal.SIGTERM,
     signal.SIGUSR1,
@@ -71,124 +71,125 @@
     wrapped
       the path to the wrapper script run inside casapy.
 
     There is a very large overhead to running casapy scripts. The outer Python
     code sleeps for at least 5 seconds to allow various cleanups to happen.
 
     """
+
     def __init__(self, script, raise_on_error=True, **kwargs):
         self.script = script
         self.kwargs = kwargs
         self.raise_on_error = raise_on_error
 
-
     def __enter__(self):
         # We read in the entire script and save it in the wrapper. That way we
         # don't have to worry about dealing with file-not-found errors inside
         # casapy, where exception handling is annoying and the startup time is
         # significant.
 
         try:
             with open(self.script) as f:
                 text = f.read()
         except Exception:
-            reraise_context('while trying to read %r', self.script)
+            reraise_context("while trying to read %r", self.script)
 
-        self.workdir = tempfile.mkdtemp(prefix='casascript', dir='.')
-        self.wrapped = os.path.join(self.workdir, 'wrapped.py')
+        self.workdir = tempfile.mkdtemp(prefix="casascript", dir=".")
+        self.wrapped = os.path.join(self.workdir, "wrapped.py")
 
-        with open(self.wrapped, 'w') as wrapper:
-            print('_pkcs_script = ' + repr(self.script), file=wrapper)
-            print('_pkcs_text = ' + repr(text), file=wrapper)
-            print('_pkcs_kwargs = ' + repr(self.kwargs), file=wrapper)
-            print('_pkcs_origcwd = ' + repr(os.getcwd()), file=wrapper)
+        with open(self.wrapped, "w") as wrapper:
+            print("_pkcs_script = " + repr(self.script), file=wrapper)
+            print("_pkcs_text = " + repr(text), file=wrapper)
+            print("_pkcs_kwargs = " + repr(self.kwargs), file=wrapper)
+            print("_pkcs_origcwd = " + repr(os.getcwd()), file=wrapper)
 
-            driver = __file__.replace('.pyc', '.py').replace('.py', '_driver.py')
+            driver = __file__.replace(".pyc", ".py").replace(".py", "_driver.py")
             with open(driver) as driver:
                 for line in driver:
-                    print(line, end='', file=wrapper)
+                    print(line, end="", file=wrapper)
 
         def preexec():
             # Start new session and process groups so that the module can kill all
             # CASA-related processes as best we can.
             os.setsid()
 
             # We want to direct casapy's stdout and stderr to separate files since
             # they're full of chatter, while still giving the script access to
             # intentional output on the wrapper's stdout and stderr. At this
             # point, FD's 1 and 2 are the latter. We want to move them to FD's 3
             # and 4, while changing 1 and 2 to the temp files. The close_fds logic
             # of subprocess runs after this function, so we have to set close_fds
             # to False.
 
-            os.dup2(1, 3) # dup2 closes target fd if needed.
+            os.dup2(1, 3)  # dup2 closes target fd if needed.
             os.dup2(2, 4)
 
-            with open('casa_stdout', 'wb') as stdout:
+            with open("casa_stdout", "wb") as stdout:
                 os.dup2(stdout.fileno(), 1)
 
-            with open('casa_stderr', 'wb') as stderr:
+            with open("casa_stderr", "wb") as stderr:
                 os.dup2(stderr.fileno(), 2)
 
         self.env = CasaEnvironment()
-        self.proc = self.env.launch(casapy_argv + ['wrapped.py'],
-                                    cwd=self.workdir,
-                                    stdin=open(os.devnull, 'rb'),
-                                    preexec_fn=preexec,
-                                    close_fds=False)
+        self.proc = self.env.launch(
+            casapy_argv + ["wrapped.py"],
+            cwd=self.workdir,
+            stdin=open(os.devnull, "rb"),
+            preexec_fn=preexec,
+            close_fds=False,
+        )
 
         # Set up signal handlers to propagate to the child process. Copied from
         # wrapout.py.
         prev_handlers = {}
 
         def handle(signum, frame):
             self.proc.send_signal(signum)
 
         for signum in signals_for_child:
             prev_handlers[signum] = signal.signal(signum, handle)
 
         self.exitcode = self.proc.wait()
 
-        for signum, prev_handler in six.iteritems(prev_handlers):
+        for signum, prev_handler in prev_handlers.items():
             signal.signal(signum, prev_handler)
 
         # default: delte workdir on success or intentional script abort
-        self.rmtree = (self.exitcode == 0 or self.exitcode == 127)
+        self.rmtree = self.exitcode == 0 or self.exitcode == 127
 
         if self.raise_on_error and self.exitcode != 0:
             # Note that we have to raise the exception here to prevent the
             # `with` statement body from executing. In that case __exit__
             # isn't called so we need to do that too.
             self._cleanup()
 
             if self.exitcode < 0:
-                raise PKError('casapy was killed by signal %d', -self.exitcode)
+                raise PKError("casapy was killed by signal %d", -self.exitcode)
             elif self.exitcode == 127:
-                raise PKError('the casapy script signaled an internal error')
+                raise PKError("the casapy script signaled an internal error")
             else:
-                raise PKError('casapy exited with error code %d', self.exitcode)
+                raise PKError("casapy exited with error code %d", self.exitcode)
 
         return self
 
-
     def __exit__(self, etype, evalue, etb):
         if etype is not None:
             self.rmtree = False
 
         self._cleanup()
-        return False # propagate exceptions
-
+        return False  # propagate exceptions
 
     def _cleanup(self):
         # Ugh, I hate having a hardcoded sleep, but it seems to be necessary
         # to let the watchdog clean everything up. Or something. The casapy
         # process tree is a mess several process groups being created, and I
         # think the only way we can really contain it is with cgroups, which
         # would be difficult and make us Linux-specific. Grrr.
         import time
+
         time.sleep(4)
 
         # If I'm interpreting things correctly, this bit is needed to kill
         # the "watchdog" process.
 
         try:
             os.killpg(self.proc.pid, signal.SIGTERM)
@@ -201,45 +202,49 @@
             os.killpg(self.proc.pid, signal.SIGKILL)
         except Exception as e:
             pass
 
         # OK, blow away the directory.
 
         if not self.rmtree:
-            cli.warn('preserving directory tree %r since script %r failed',
-                     self.workdir, self.script)
+            cli.warn(
+                "preserving directory tree %r since script %r failed",
+                self.workdir,
+                self.script,
+            )
         else:
             shutil.rmtree(self.workdir, ignore_errors=True)
 
 
 cli_usage = """pkcasascript <scriptfile> [more args...]
 
 Run a specially-designed script inside a CASA environment. This program is not
 meant for regular users. See the documentation of the module
 `pwkit.environments.casa.scripting` for more information."""
 
+
 def commandline(argv=None):
     if argv is None:
         argv = sys.argv
         cli.propagate_sigint()
         cli.unicode_stdio()
         cli.backtrace_on_usr1()
 
-    cli.check_usage(cli_usage, argv, usageifnoargs='long')
+    cli.check_usage(cli_usage, argv, usageifnoargs="long")
     script = argv[1]
     args = argv[2:]
 
     try:
         with CasapyScript(script, cli_args=args) as cs:
             pass
     except Exception:
-        reraise_context('when running casapy script %r', script)
+        reraise_context("when running casapy script %r", script)
 
     if cs.exitcode < 0:
         signum = -cs.exitcode
-        print('casascript error: casapy died with signal %d' % signum)
+        print("casascript error: casapy died with signal %d" % signum)
         signal.signal(signum, signal.SIG_DFL)
         os.kill(os.getpid(), signum)
     elif cs.exitcode:
         if cs.exitcode != 127:
-            print('casascript error: casapy died with exit code %d' % cs.exitcode)
+            print("casascript error: casapy died with exit code %d" % cs.exitcode)
         sys.exit(cs.exitcode)
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/scripting_driver.py` & `pwkit-1.2.0/pwkit/environments/casa/scripting_driver.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/casa/spwglue.py` & `pwkit-1.2.0/pwkit/environments/casa/spwglue.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 procesing step is very slow, however.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 __all__ = str("Progress Config spwglue spwglue_cli").split()
 
-import six
-from six.moves import range
 import numpy as np
-from ... import binary_type, text_type
 from ...kwargv import ParseKeywords, Custom
 from ...cli import check_usage, die
 from . import util
 from .util import sanitize_unicode as b
 
 
 def _sfmt(t):
@@ -309,15 +306,15 @@
 def fillsmall(path, rows):
     tb = util.tools.table()
     tb.open(b(path), nomodify=False)
     tb.addrows(len(rows))
 
     try:
         for i, data in enumerate(rows):
-            for col, val in six.iteritems(data):
+            for col, val in data.items():
                 tb.putcell(b(col), i, val)
     except Exception as e:
         raise Exception(
             "error putting: %d %s %s (%s): %s" % (i, col, val, val.__class__, e)
         )
 
     tb.close()
@@ -512,17 +509,15 @@
     if cfg.corr_to_main:
         dt.removecols([b"CORRECTED_DATA"])
 
     outrow = 0
 
     for outspw in range(nout):
         q = " or ".join(
-            "DATA_DESC_ID == %d" % t[0]
-            for t in six.iteritems(indd2outdd)
-            if t[1][0] == outspw
+            "DATA_DESC_ID == %d" % t[0] for t in indd2outdd.items() if t[1][0] == outspw
         )
         if cfg.hackfield is not None:
             q = "(FIELD_ID == %s or FIELD_ID == %s) and (%s)" % (
                 thisfield,
                 cfg.hackfield,
                 q,
             )
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/tasks.py` & `pwkit-1.2.0/pwkit/environments/casa/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 library, with no side effects, so that data processing can be scripted
 tractably. These tasks are also accessible through the ``casatask`` command
 line program provided with :mod:`pwkit`.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-import os.path, six, sys
-from six.moves import range
+import os.path, sys
 import numpy as np
 
 from . import util
-from ... import binary_type, reraise_context, text_type, PKError
+from ... import reraise_context, PKError
 from ...cli import check_usage, wrong_usage, warn, die
 from ...kwargv import ParseKeywords, Custom
 
 # Keep the tasks alphabetized!
 
 __all__ = str(
     """
@@ -518,15 +517,15 @@
 
     for ispw in seenspws:
         spw_to_offset[ispw] = tot_seen_nchan
         tot_seen_nchan += nchan[ispw]
 
     # normalize phases to avoid distracting wraps
 
-    for iant, ipol in sorted(six.iterkeys(antpols)):
+    for iant, ipol in sorted(antpols.keys()):
         for ispw, isoln in antpols[iant, ipol]:
             f = flags[isoln][ipol]
             meanph = np.angle(vals[isoln][ipol, ~f].mean())
             vals[isoln][ipol] *= np.exp(-1j * meanph)
 
     # find plot limits
 
@@ -574,15 +573,15 @@
     if min_ph < -160:
         min_ph = -180
 
     polnames = "RL"  # XXX: identification doesn't seem to be stored in cal table
 
     # plot away
 
-    for iant, ipol in sorted(six.iterkeys(antpols)):
+    for iant, ipol in sorted(antpols.keys()):
         p_am = om.RectPlot()
         p_ph = om.RectPlot()
 
         for ispw, isoln in antpols[iant, ipol]:
             f = flags[isoln][ipol]
             a = np.abs(vals[isoln][ipol])
             p = np.angle(vals[isoln][ipol], deg=True)
@@ -840,20 +839,15 @@
     tb.open(b(mspath), nomodify=False)
     cols = frozenset(tb.colnames())
     toremove = [b(c) for c in wantremove if c in cols]
     if len(toremove):
         tb.removecols(toremove)
     tb.close()
 
-    # We want to return a `str` type, which is what we already
-    # have in Python 2 but not in 3.
-    if six.PY2:
-        return toremove
-    else:
-        return [c.decode("utf8") for c in toremove]
+    return [c.decode("utf8") for c in toremove]
 
 
 def delcal_cli(argv):
     check_usage(delcal_doc, argv, usageifnoargs=True)
     util.logger()
 
     for mspath in argv[1:]:
@@ -1785,15 +1779,15 @@
         solkws[sk] = getattr(cfg, ck)
 
     if isinstance(cfg.solint, (int, float)):
         solkws["t"] = "%fs" % cfg.solint  # sugar
     else:
         solkws["t"] = str(cfg.solint)
 
-    if isinstance(cfg.refant, six.string_types):
+    if isinstance(cfg.refant, str):
         solkws["refant"] = cfg.refant
     else:
         solkws["refant"] = ",".join(cfg.refant)
 
     solkws["combine"] = ",".join(cfg.combine)
     solkws["phaseonly"] = False
     solkws["type"] = cfg.gaintype.upper()
@@ -2629,20 +2623,18 @@
         try:
             proc = subprocess.Popen(
                 pager, stdin=subprocess.PIPE, close_fds=True, shell=True
             )
         except Exception as e:
             warn("couldn't start pager %r: %s", pager, e)
         else:
-            out = proc.stdin
+            import codecs
 
-            if not six.PY2:
-                import codecs
-
-                out = codecs.getwriter("utf8")(out)
+            out = proc.stdin
+            out = codecs.getwriter("utf8")(out)
 
     for line in listobs(vis):
         print(line, file=out)
 
     if proc is not None:
         proc.stdin.close()
         proc.wait()  # ignore return code
@@ -4222,15 +4214,15 @@
     max_val += 0.05 * span
     min_val -= 0.05 * span
 
     polnames = "XY"  # XXX: identification doesn't seem to be stored in cal table
 
     # plot away
 
-    for iant, ipol in sorted(six.iterkeys(antpols)):
+    for iant, ipol in sorted(antpols.keys()):
         p = om.RectPlot()
         p.addKeyItem("%s %s" % (antnames[iant], polnames[ipol]))
 
         for ifield in seenfields:
             antpols = apbyfield[ifield]
             kt = fieldnames[ifield]
 
@@ -4458,15 +4450,15 @@
 
 def cmdline_usage(stream, exitcode):
     print("usage: casatask <task> [task-specific arguments]", file=stream)
     print(file=stream)
     print("Supported tasks:", file=stream)
     print(file=stream)
 
-    for name in sorted(six.iterkeys(globals())):
+    for name in sorted(globals().keys()):
         if name.endswith("_cli"):
             print(name[:-4], file=stream)
 
     raise SystemExit(exitcode)
 
 
 def commandline(argv=None):
```

### Comparing `pwkit-1.1.1/pwkit/environments/casa/util.py` & `pwkit-1.2.0/pwkit/environments/casa/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,63 +4,120 @@
 
 """This module provides low-level tools and utilities for interacting with the
 ``casac`` module provided by CASA.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str('''INVERSE_C_MS INVERSE_C_MNS pol_names pol_to_miriad msselect_keys
-datadir logger forkandlog sanitize_unicode tools''').split()
-
-import six
-from ... import text_type
+__all__ = str(
+    """INVERSE_C_MS INVERSE_C_MNS pol_names pol_to_miriad msselect_keys
+datadir logger forkandlog sanitize_unicode tools"""
+).split()
 
 # Some constants that can be useful.
 
-INVERSE_C_MS  = 3.3356409519815204e-09 # inverse speed of light in m/s
-INVERSE_C_MNS = 3.3356409519815204 # inverse speed of light in m/ns
+INVERSE_C_MS = 3.3356409519815204e-09  # inverse speed of light in m/s
+INVERSE_C_MNS = 3.3356409519815204  # inverse speed of light in m/ns
 
 pol_names = {
-    0: '?',
-    1: 'I', 2: 'Q', 3: 'U', 4: 'V',
-    5: 'RR', 6: 'RL', 7: 'LR', 8: 'LL',
-    9: 'XX', 10: 'XY', 11: 'YX', 12: 'YY',
-    13: 'RX', 14: 'RY', 15: 'LX', 16: 'LY',
-    17: 'XR', 18: 'XL', 19: 'YR', 20: 'YL',
-    21: 'PP', 22: 'PQ', 23: 'QP', 24: 'QQ',
-    25: 'RCirc', 26: 'Lcirc', 27: 'Lin', 28: 'Ptot', 29: 'Plin',
-    30: 'PFtot', 31: 'PFlin', 32: 'Pang',
+    0: "?",
+    1: "I",
+    2: "Q",
+    3: "U",
+    4: "V",
+    5: "RR",
+    6: "RL",
+    7: "LR",
+    8: "LL",
+    9: "XX",
+    10: "XY",
+    11: "YX",
+    12: "YY",
+    13: "RX",
+    14: "RY",
+    15: "LX",
+    16: "LY",
+    17: "XR",
+    18: "XL",
+    19: "YR",
+    20: "YL",
+    21: "PP",
+    22: "PQ",
+    23: "QP",
+    24: "QQ",
+    25: "RCirc",
+    26: "Lcirc",
+    27: "Lin",
+    28: "Ptot",
+    29: "Plin",
+    30: "PFtot",
+    31: "PFlin",
+    32: "Pang",
 }
 
 pol_to_miriad = {
     # see mirtask.util for the MIRIAD magic numbers.
-    1: 1, 2: 2, 3: 3, 4: 4, # IQUV
-    5: -1, 6: -3, 7: -4, 8: -2, # R/L
-    9: -5, 10: -7, 11: -8, 12: -6, # X/Y
+    1: 1,
+    2: 2,
+    3: 3,
+    4: 4,  # IQUV
+    5: -1,
+    6: -3,
+    7: -4,
+    8: -2,  # R/L
+    9: -5,
+    10: -7,
+    11: -8,
+    12: -6,  # X/Y
     # rest are inexpressible
 }
 
 pol_is_intensity = {
     0: False,
-    1: True, 2: False, 3: False, 4: False, # IQUV
-    5: True, 6: False, 7: False, 8: True, # RR RL LR LL
-    9: True, 10: False, 11: False, 12: True, # XX XY YX YY
-    13: False, 14: False, 15: False, 16: False, # RX RY LX LY
-    17: False, 18: False, 19: False, 20: False, # XR XL YR YL
-    21: True, 22: False, 23: False, 24: True, # PP PQ QP QQ
-    25: False, 26: False, 27: False, 28: False, 29: False,
-    30: False, 31: False, 32: False,
+    1: True,
+    2: False,
+    3: False,
+    4: False,  # IQUV
+    5: True,
+    6: False,
+    7: False,
+    8: True,  # RR RL LR LL
+    9: True,
+    10: False,
+    11: False,
+    12: True,  # XX XY YX YY
+    13: False,
+    14: False,
+    15: False,
+    16: False,  # RX RY LX LY
+    17: False,
+    18: False,
+    19: False,
+    20: False,  # XR XL YR YL
+    21: True,
+    22: False,
+    23: False,
+    24: True,  # PP PQ QP QQ
+    25: False,
+    26: False,
+    27: False,
+    28: False,
+    29: False,
+    30: False,
+    31: False,
+    32: False,
 }
 
 # "polarization" is technically valid as an MS selection, but it pretty much
 # doesn't do what you'd want since records generally contain multiple pols.
 # ms.selectpolarization() should be used instead. Maybe ditto for spw?
 
-msselect_keys = frozenset('array baseline field observation '
-                          'scan scaninent spw taql time uvdist'.split())
+msselect_keys = frozenset(
+    "array baseline field observation " "scan scaninent spw taql time uvdist".split()
+)
 
 
 def sanitize_unicode(item):
     """Safely pass string values to the CASA tools.
 
     item
       A value to be passed to a CASA tool.
@@ -85,30 +142,32 @@
 
       tb = tools.table()
       path = u'data.ms'
       tb.open(path) # => raises exception
       tb.open(b(path)) # => works
 
     """
-    if isinstance(item, text_type):
-        return item.encode('utf8')
+    if isinstance(item, str):
+        return item.encode("utf8")
     if isinstance(item, dict):
-        return dict((sanitize_unicode(k), sanitize_unicode(v)) for k, v in six.iteritems(item))
-    if isinstance(item,(list, tuple)):
+        return dict((sanitize_unicode(k), sanitize_unicode(v)) for k, v in item.items())
+    if isinstance(item, (list, tuple)):
         return item.__class__(sanitize_unicode(x) for x in item)
 
     from ...io import Path
+
     if isinstance(item, Path):
         return str(item)
 
     return item
 
 
 # Finding the data directory
 
+
 def datadir(*subdirs):
     """Get a path within the CASA data directory.
 
     subdirs
       Extra elements to append to the returned path.
 
     This function locates the directory where CASA resource data files (tables
@@ -121,63 +180,68 @@
 
       cal_image_path = util.datadir('nrao', 'VLA', 'CalModels', '3C286_C.im')
       tb = util.tools.image()
       tb.open(cal_image_path)
 
     """
     import os.path
+
     data = None
 
-    if 'CASAPATH' in os.environ:
-        data = os.path.join(os.environ['CASAPATH'].split()[0], 'data')
+    if "CASAPATH" in os.environ:
+        data = os.path.join(os.environ["CASAPATH"].split()[0], "data")
 
     if data is None:
         # The Conda CASA directory layout:
         try:
             import casadef
         except ImportError:
             pass
         else:
-            data = os.path.join(os.path.dirname(casadef.task_directory), 'data')
+            data = os.path.join(os.path.dirname(casadef.task_directory), "data")
             if not os.path.isdir(data):
                 # Sigh, hack for CASA 4.7 + Conda; should be straightened out:
                 dn = os.path.dirname
-                data = os.path.join(dn(dn(dn(casadef.task_directory))), 'lib', 'casa', 'data')
+                data = os.path.join(
+                    dn(dn(dn(casadef.task_directory))), "lib", "casa", "data"
+                )
                 if not os.path.isdir(data):
                     data = None
 
     if data is None:
         import casac
 
         prevp = None
         p = os.path.dirname(casac.__file__)
         while len(p) and p != prevp:
-            data = os.path.join(p, 'data')
+            data = os.path.join(p, "data")
             if os.path.isdir(data):
                 break
             prevp = p
             p = os.path.dirname(p)
 
     if not os.path.isdir(data):
-        raise RuntimeError('cannot identify CASA data directory')
+        raise RuntimeError("cannot identify CASA data directory")
 
     return os.path.join(data, *subdirs)
 
 
 # Trying to use the logging facility in a sane way.
 #
 # As soon as you create a logsink, it creates a file called casapy.log.
 # So we do some junk to not leave turds all around the filesystem.
 
+
 def _rmtree_error(func, path, excinfo):
     from ...cli import warn
-    warn('couldn\'t delete temporary file %s: %s (%s)', path, excinfo[0], func)
 
+    warn("couldn't delete temporary file %s: %s (%s)", path, excinfo[0], func)
 
-def logger(filter='WARN'):
+
+def logger(filter="WARN"):
     """Set up CASA to write log messages to standard output.
 
     filter
       The log level filter: less urgent messages will not be shown. Valid values
       are strings: "DEBUG1", "INFO5", ... "INFO1", "INFO", "WARN", "SEVERE".
 
     This function creates and returns a CASA ”log sink” object that is
@@ -190,22 +254,22 @@
     """
     import os, shutil, tempfile
 
     cwd = os.getcwd()
     tempdir = None
 
     try:
-        tempdir = tempfile.mkdtemp(prefix='casautil')
+        tempdir = tempfile.mkdtemp(prefix="casautil")
 
         try:
             os.chdir(tempdir)
             sink = tools.logsink()
             sink.setlogfile(sanitize_unicode(os.devnull))
             try:
-                os.unlink('casapy.log')
+                os.unlink("casapy.log")
             except OSError as e:
                 if e.errno != 2:
                     raise
                 # otherwise, it's a ENOENT, in which case, no worries.
         finally:
             os.chdir(cwd)
     finally:
@@ -214,15 +278,15 @@
 
     sink.showconsole(True)
     sink.setglobal(True)
     sink.filter(sanitize_unicode(filter.upper()))
     return sink
 
 
-def forkandlog(function, filter='INFO5', debug=False):
+def forkandlog(function, filter="INFO5", debug=False):
     """Fork a child process and read its CASA log output.
 
     function
       A function to run in the child process
     filter
       The CASA log level filter to apply in the child process: less urgent
       messages will not be shown. Valid values are strings: "DEBUG1", "INFO5",
@@ -274,20 +338,20 @@
         # Python exception info), it'll get sent along the pipe too. The
         # caller would have to be much more complex to be able to detect and
         # handle such output.
 
         os.close(readfd)
 
         if not debug:
-            f = open(os.devnull, 'w')
+            f = open(os.devnull, "w")
             os.dup2(f.fileno(), 1)
             os.dup2(f.fileno(), 2)
 
         sink = logger(filter=filter)
-        sink.setlogfile(b'/dev/fd/%d' % writefd)
+        sink.setlogfile(b"/dev/fd/%d" % writefd)
         function(sink)
         sys.exit(0)
 
     # Original process.
 
     os.close(writefd)
 
@@ -296,51 +360,55 @@
             yield line
 
     info = os.waitpid(pid, 0)
 
     if info[1]:
         # Because we're a generator, this is the only way for us to signal if
         # the process died. We could be rewritten as a context manager.
-        e = RuntimeError('logging child process PID %d exited '
-                         'with error code %d' % tuple(info))
+        e = RuntimeError(
+            "logging child process PID %d exited " "with error code %d" % tuple(info)
+        )
         e.pid, e.exitcode = info
         raise e
 
 
 # Tool factories.
 
+
 class _Tools(object):
     """This class is structured so that it supports useful tab-completion
     interactively, but also so that new tools can be constructed if the
     underlying library provides them.
 
     """
-    _builtinNames = '''agentflagger atmosphere calanalysis calibrater calplot
+
+    _builtinNames = """agentflagger atmosphere calanalysis calibrater calplot
                      componentlist coordsys deconvolver fitter flagger
                      functional image imagepol imager logsink measures
                      msmetadata ms msplot mstransformer plotms regionmanager
                      simulator spectralline quanta table tableplot utils
-                     vlafiller vpmanager'''.split()
+                     vlafiller vpmanager""".split()
 
     def __getattribute__(self, n):
         """Returns factories, not instances."""
         # We need to make this __getattribute__, not __getattr__, only because
         # we set the builtin names in the class __dict__ to enable tab-completion.
         import casac
 
-        if hasattr(casac, 'casac'): # casapy >= 4.0?
+        if hasattr(casac, "casac"):  # casapy >= 4.0?
             t = getattr(casac.casac, n, None)
             if t is None:
                 raise AttributeError('tool "%s" not present' % n)
             return t
         else:
             try:
-                return casac.homefinder.find_home_by_name(n + 'Home').create
+                return casac.homefinder.find_home_by_name(n + "Home").create
             except Exception:
                 # raised exception is class 'homefinder.error'; it appears unavailable
                 # on the Python layer
                 raise AttributeError('tool "%s" not present' % n)
 
+
 for n in _Tools._builtinNames:
-    setattr(_Tools, n, None) # ease autocompletion
+    setattr(_Tools, n, None)  # ease autocompletion
 
 tools = _Tools()
```

### Comparing `pwkit-1.1.1/pwkit/environments/ciao/__init__.py` & `pwkit-1.2.0/pwkit/environments/ciao/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,135 +24,142 @@
 tarballs and installing CIAO itself. This may also download and install the
 large “caldb” data set. All of the files will end up in a subdirectory such as
 ``/soft/ciao/ciao-4.8``.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('CiaoEnvironment CiaoTool').split ()
+__all__ = str("CiaoEnvironment CiaoTool").split()
 
-import io, six
-
-from ... import PKError, cli
+from ... import PKError
 from ...cli import multitool
 from ...io import Path
 from .. import Environment, prepend_environ_path, user_data_path
 
 
-class CiaoEnvironment (Environment):
+class CiaoEnvironment(Environment):
     _installpath = None
     _parampath = None
 
-    def __init__ (self, installdir=None, paramdir=None):
+    def __init__(self, installdir=None, paramdir=None):
         if installdir is None:
-            installdir = self._default_installdir ()
+            installdir = self._default_installdir()
         if paramdir is None:
-            paramdir = user_data_path ('cxcds_param')
-
-        self._installpath = Path (installdir).absolute ()
-        self._parampath = Path (paramdir).absolute ()
+            paramdir = user_data_path("cxcds_param")
 
+        self._installpath = Path(installdir).absolute()
+        self._parampath = Path(paramdir).absolute()
 
-    def _default_installdir (self):
+    def _default_installdir(self):
         import os
-        d = os.environ.get ('PWKIT_CIAO')
+
+        d = os.environ.get("PWKIT_CIAO")
         if d is None:
-            raise PKError ('CIAO installation directory must be specified '
-                           'in the $PWKIT_CIAO environment variable')
+            raise PKError(
+                "CIAO installation directory must be specified "
+                "in the $PWKIT_CIAO environment variable"
+            )
         return d
 
-
-    def modify_environment (self, env):
+    def modify_environment(self, env):
         p = self._installpath
 
-        env['ASCDS_INSTALL'] = str (p)
-        env['ASCDS_CONTRIB'] = str (p / 'contrib')
-        env['ASCDS_BIN'] = str (p / 'bin')
-        env['ASCDS_LIB'] = str (p / 'lib')
-        env['ASCDS_IMAGER_PATH'] = str (p / 'ots' / 'bin')
-        env['ASCDS_WORK_PATH'] = str ('/tmp') # needed by at least specextract
-        env['CIAO_XPA'] = b'CIAO'
-        env['CIAO_PYTHON'] = b'CIAO'
-        env['CIAO_APP_PYTHON'] = b'CIAO'
-        env['CIAO_IPYTHON'] = b'CIAO'
-        env['CIAO_APP_IPYTHON'] = b'CIAO'
-        env['CIAO_PYTHON_EXE'] = str (p / 'ots' / 'bin' / 'python')
-        env['CIAO_SCRIPT_LANG'] = b'python'
-        env['XPA_METHOD'] = b'local'
-        env['CALDB'] = str (p / 'CALDB')
-        env['CALDBCONFIG'] = str (p / 'CALDB' / 'software' / 'tools' / 'caldb.config')
-        env['CALDBALIAS'] = str (p / 'CALDB' / 'software' / 'tools' / 'alias_config.fits')
-        env['ASCDS_CALIB'] = str (p / 'data')
-        env['ASCDS_CIAO'] = b'ciao'
+        env["ASCDS_INSTALL"] = str(p)
+        env["ASCDS_CONTRIB"] = str(p / "contrib")
+        env["ASCDS_BIN"] = str(p / "bin")
+        env["ASCDS_LIB"] = str(p / "lib")
+        env["ASCDS_IMAGER_PATH"] = str(p / "ots" / "bin")
+        env["ASCDS_WORK_PATH"] = str("/tmp")  # needed by at least specextract
+        env["CIAO_XPA"] = b"CIAO"
+        env["CIAO_PYTHON"] = b"CIAO"
+        env["CIAO_APP_PYTHON"] = b"CIAO"
+        env["CIAO_IPYTHON"] = b"CIAO"
+        env["CIAO_APP_IPYTHON"] = b"CIAO"
+        env["CIAO_PYTHON_EXE"] = str(p / "ots" / "bin" / "python")
+        env["CIAO_SCRIPT_LANG"] = b"python"
+        env["XPA_METHOD"] = b"local"
+        env["CALDB"] = str(p / "CALDB")
+        env["CALDBCONFIG"] = str(p / "CALDB" / "software" / "tools" / "caldb.config")
+        env["CALDBALIAS"] = str(
+            p / "CALDB" / "software" / "tools" / "alias_config.fits"
+        )
+        env["ASCDS_CALIB"] = str(p / "data")
+        env["ASCDS_CIAO"] = b"ciao"
 
         # Obsvis:
-        env['OBSVIS_PKG_PATH'] = str (p / 'lib' / 'tcltk' / 'packages' / 'obsvis')
+        env["OBSVIS_PKG_PATH"] = str(p / "lib" / "tcltk" / "packages" / "obsvis")
 
         # Sherpa:
-        env['CIAO_HEADAS'] = str (p / 'ots' / 'spectral')
-        env['XSPEC_HELP_FILE'] = str (p / 'doc' / 'xspec.hlp')
+        env["CIAO_HEADAS"] = str(p / "ots" / "spectral")
+        env["XSPEC_HELP_FILE"] = str(p / "doc" / "xspec.hlp")
 
         # Proposal tools:
-        env['DATA_ROOT'] = str (p / 'config')
-        env['JCMLIBDATA'] = str (p / 'config' / 'jcm_data')
-        env['ASCDS_PROP_NHBASE'] = env['JCMLIBDATA']
-        env['JCMPATH'] = env['JCMLIBDATA']
-        env['ASCDS_PROP_DATE_DATA'] = env['JCMLIBDATA']
-        env['ASCDS_PROP_PREC_DATA'] = env['JCMLIBDATA']
-
-        env['PFILES'] = '%s;%s:%s' % (self._parampath,
-                                      p / 'contrib' / 'param',
-                                      p / 'param')
-
-        prepend_environ_path (env, 'PATH', str (p / 'contrib' / 'bin'))
-        prepend_environ_path (env, 'PATH', str (p / 'ots' / 'bin'))
-        prepend_environ_path (env, 'PATH', str (p / 'bin'))
+        env["DATA_ROOT"] = str(p / "config")
+        env["JCMLIBDATA"] = str(p / "config" / "jcm_data")
+        env["ASCDS_PROP_NHBASE"] = env["JCMLIBDATA"]
+        env["JCMPATH"] = env["JCMLIBDATA"]
+        env["ASCDS_PROP_DATE_DATA"] = env["JCMLIBDATA"]
+        env["ASCDS_PROP_PREC_DATA"] = env["JCMLIBDATA"]
+
+        env["PFILES"] = "%s;%s:%s" % (
+            self._parampath,
+            p / "contrib" / "param",
+            p / "param",
+        )
+
+        prepend_environ_path(env, "PATH", str(p / "contrib" / "bin"))
+        prepend_environ_path(env, "PATH", str(p / "ots" / "bin"))
+        prepend_environ_path(env, "PATH", str(p / "bin"))
 
         return env
 
-    def _preexec (self, env, **kwargs):
-        self._parampath.ensure_dir (parents=True)
+    def _preexec(self, env, **kwargs):
+        self._parampath.ensure_dir(parents=True)
 
 
 # Command-line interface
 
 from .. import DefaultExecCommand, DefaultShellCommand
 
-class BgbandCommand (multitool.Command):
-    name = 'bgband'
-    argspec = '<evt> <srcreg> <bkgreg> <elo1> <ehi1> [... <eloN> <ehiN>]'
-    summary = 'Compute basic background statistics for a source in energy bands.'
-
-    def invoke (self, args, envclass=None, **kwargs):
-        if len (args) < 5:
-            raise multitool.UsageError ('bgband takes at least two arguments')
-        if len (args) % 2 == 0:
-            raise multitool.UsageError ('bgband expects an odd number of arguments')
+
+class BgbandCommand(multitool.Command):
+    name = "bgband"
+    argspec = "<evt> <srcreg> <bkgreg> <elo1> <ehi1> [... <eloN> <ehiN>]"
+    summary = "Compute basic background statistics for a source in energy bands."
+
+    def invoke(self, args, envclass=None, **kwargs):
+        if len(args) < 5:
+            raise multitool.UsageError("bgband takes at least two arguments")
+        if len(args) % 2 == 0:
+            raise multitool.UsageError("bgband expects an odd number of arguments")
 
         evt = args[0]
         srcreg = args[1]
         bkgreg = args[2]
-        ebins = [(float (args[i]), float (args[i+1])) for i in range (3, len (args), 2)]
+        ebins = [(float(args[i]), float(args[i + 1])) for i in range(3, len(args), 2)]
 
-        env = envclass ()
+        env = envclass()
         from .analysis import compute_bgband
-        df = compute_bgband (evt, srcreg, bkgreg, ebins, env)
-        print (df.to_string (index=False, justify='left'))
+
+        df = compute_bgband(evt, srcreg, bkgreg, ebins, env)
+        print(df.to_string(index=False, justify="left"))
 
 
-class CiaoTool (multitool.Multitool):
-    cli_name = 'pkenvtool ciao'
-    summary = 'Run tools in the CIAO environment.'
-
-    def invoke_command (self, cmd, args, **kwargs):
-        return super (CiaoTool, self).invoke_command (cmd, args,
-                                                      envname='ciao',
-                                                      envclass=CiaoEnvironment,
-                                                      module=__package__,
-                                                      **kwargs)
-
-
-def commandline (argv):
-    from six import itervalues
-    tool = CiaoTool ()
-    tool.populate (itervalues (globals ()))
-    tool.commandline (argv)
+class CiaoTool(multitool.Multitool):
+    cli_name = "pkenvtool ciao"
+    summary = "Run tools in the CIAO environment."
+
+    def invoke_command(self, cmd, args, **kwargs):
+        return super(CiaoTool, self).invoke_command(
+            cmd,
+            args,
+            envname="ciao",
+            envclass=CiaoEnvironment,
+            module=__package__,
+            **kwargs
+        )
+
+
+def commandline(argv):
+    tool = CiaoTool()
+    tool.populate(globals().values())
+    tool.commandline(argv)
```

### Comparing `pwkit-1.1.1/pwkit/environments/ciao/analysis.py` & `pwkit-1.2.0/pwkit/environments/ciao/analysis.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/ciao/data.py` & `pwkit-1.2.0/pwkit/environments/ciao/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 
 TODO: SAS, CIAO, HEASoft, etc all use very similar data formats; more code
 should be shared.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''
+__all__ = str(
+    """
 BaseCIAOData
 GTIData
 Events
 OIFData
 ChandraDataSet
-''').split ()
+"""
+).split()
 
-import numpy as np, pandas as pd
-from six.moves import range
+import numpy as np
 from astropy.time import Time
-from ... import astutil
 from ...cli import warn
 from ...io import Path
 from ...numutil import fits_recarray_to_data_frame
 
 
-def tight_bounds (minval, maxval):
+def tight_bounds(minval, maxval):
     if minval > maxval:
         maxval, minval = minval, maxval
 
     span = maxval - minval
     if span <= 0:
-        span = abs (maxval)
+        span = abs(maxval)
         if span == 0:
             span = 1
 
     span *= 0.05
     return minval - span, maxval + span
 
 
-class BaseCIAOData (object):
+class BaseCIAOData(object):
     telescope = None
     "Telescope name: likely 'CHANDRA'"
 
     instrument = None
     "Instrument used: likely 'ACIS'"
 
     obsid = None
@@ -61,113 +61,114 @@
     """Offset Mission Elapsed Time (seconds) value ; default is
     the first data timestamp in the data set.
 
     """
     mjd0 = None
     "Offset MJD; default mjd0 = floor (t0 / 86400 + mjdref)."
 
-    def __init__ (self, path, mjd0=None, t0=None):
+    def __init__(self, path, mjd0=None, t0=None):
         self.mjd0 = mjd0
         self.t0 = t0
 
-        with Path (path).read_fits () as hdulist:
-            self._process_main (hdulist, hdulist[0].header)
+        with Path(path).read_fits() as hdulist:
+            self._process_main(hdulist, hdulist[0].header)
             assert self.mjdref is not None
             assert np.isfinite(self.mjdref)
             assert self.t0 is not None
             assert np.isfinite(self.t0)
             assert self.mjd0 is not None
             assert np.isfinite(self.mjd0)
 
             for hdu in hdulist[1:]:
-                self._process_hdu (hdu)
-
+                self._process_hdu(hdu)
 
-    def _process_main (self, hdulist, header):
-        self.telescope = header.get ('TELESCOP')
-        self.instrument = header.get ('INSTRUME')
-        self.obsid = header.get ('OBS_ID')
-        if 'DATE-OBS' in header:
-            self.obs_start = Time (header['DATE-OBS'], format='isot')
-        if 'DATE-END' in header:
-            self.obs_stop = Time (header['DATE-END'], format='isot')
+    def _process_main(self, hdulist, header):
+        self.telescope = header.get("TELESCOP")
+        self.instrument = header.get("INSTRUME")
+        self.obsid = header.get("OBS_ID")
+        if "DATE-OBS" in header:
+            self.obs_start = Time(header["DATE-OBS"], format="isot")
+        if "DATE-END" in header:
+            self.obs_stop = Time(header["DATE-END"], format="isot")
 
-        if 'MJDREF' in header:
-            self.mjdref = header['MJDREF']
+        if "MJDREF" in header:
+            self.mjdref = header["MJDREF"]
             # TODO: use TIMEZERO correctly?
-            self.timesys = header['TIMESYS']
-        elif 'MJDREFI' in header:
-            self.mjdref = float(header['MJDREFI'])
-            if 'MJDREFF' in header:
-                self.mjdref += header['MJDREFF']
-            self.timesys = header['TIMESYS']
+            self.timesys = header["TIMESYS"]
+        elif "MJDREFI" in header:
+            self.mjdref = float(header["MJDREFI"])
+            if "MJDREFF" in header:
+                self.mjdref += header["MJDREFF"]
+            self.timesys = header["TIMESYS"]
 
-    def _process_hdu (self, hdu):
-        warn ('ignoring HDU named %s', hdu.name)
+    def _process_hdu(self, hdu):
+        warn("ignoring HDU named %s", hdu.name)
 
 
-class GTIData (BaseCIAOData):
+class GTIData(BaseCIAOData):
     gti = None
     """Dict mapping CCD number to DataFrames of GTI info. Index: integers.
     Columns:
 
         start_met  - GTI start time in MET seconds
         stop_met   - GTI stop time in MET seconds
         start_mjd  - GTI start time as MJD
         stop_mjd   - GTI stop time as MJD
         start_dks  - GTI start time as delta-kiloseconds
         stop_dks   - GTI stop time as delta-kiloseconds
         start_dmjd - GTI start time as `mjd - mjd0`
         stop_dmjd  - GTI stop time as `mjd - mjd0`
 
     """
-    def _process_main (self, hdulist, header):
-        super (GTIData, self)._process_main (hdulist, header)
-        self.gti = {}
 
+    def _process_main(self, hdulist, header):
+        super(GTIData, self)._process_main(hdulist, header)
+        self.gti = {}
 
-    def _process_hdu (self, hdu):
-        if hdu.name in ('GTI', 'STDGTI'):
-            ccd = hdu.header.get('CCD_ID', 0)
-            gti = self.gti[ccd] = fits_recarray_to_data_frame (hdu.data)
-            gti.rename (columns={'start': 'start_met', 'stop': 'stop_met'},
-                        inplace=True)
-            gti['start_mjd'] = gti.start_met / 86400 + self.mjdref
-            gti['start_dks'] = 1e-3 * (gti.start_met - self.t0)
-            gti['start_dmjd'] = gti.start_mjd - self.mjd0
-            gti['stop_mjd'] = gti.stop_met / 86400 + self.mjdref
-            gti['stop_dks'] = 1e-3 * (gti.stop_met - self.t0)
-            gti['stop_dmjd'] = gti.stop_mjd - self.mjd0
+    def _process_hdu(self, hdu):
+        if hdu.name in ("GTI", "STDGTI"):
+            ccd = hdu.header.get("CCD_ID", 0)
+            gti = self.gti[ccd] = fits_recarray_to_data_frame(hdu.data)
+            gti.rename(columns={"start": "start_met", "stop": "stop_met"}, inplace=True)
+            gti["start_mjd"] = gti.start_met / 86400 + self.mjdref
+            gti["start_dks"] = 1e-3 * (gti.start_met - self.t0)
+            gti["start_dmjd"] = gti.start_mjd - self.mjd0
+            gti["stop_mjd"] = gti.stop_met / 86400 + self.mjdref
+            gti["stop_dks"] = 1e-3 * (gti.stop_met - self.t0)
+            gti["stop_dmjd"] = gti.stop_mjd - self.mjd0
         else:
-            super (GTIData, self)._process_hdu (hdu)
-
+            super(GTIData, self)._process_hdu(hdu)
 
-    def _plot_add_gtis (self, p, ccdnum, tunit='dmjd'):
+    def _plot_add_gtis(self, p, ccdnum, tunit="dmjd"):
         import omega as om
 
         gti = self.gti[ccdnum]
         ngti = gti.shape[0]
         if ngti == 0:
             return
 
-        gti0 = gti.at[0,'start_'+tunit]
-        gti1 = gti.at[ngti-1,'stop_'+tunit]
+        gti0 = gti.at[0, "start_" + tunit]
+        gti1 = gti.at[ngti - 1, "stop_" + tunit]
         smallofs = (gti1 - gti0) * 0.03
 
         start = gti0 - smallofs
 
-        for i in range (ngti):
-            p.add (om.rect.XBand (start, gti.at[i,'start_'+tunit], keyText=None), zheight=-1, dsn=1)
-            start = gti.at[i,'stop_'+tunit]
+        for i in range(ngti):
+            p.add(
+                om.rect.XBand(start, gti.at[i, "start_" + tunit], keyText=None),
+                zheight=-1,
+                dsn=1,
+            )
+            start = gti.at[i, "stop_" + tunit]
 
-        p.add (om.rect.XBand (start, start + smallofs, keyText=None), zheight=-1, dsn=1)
-        p.setBounds (gti0 - smallofs, gti1 + smallofs)
+        p.add(om.rect.XBand(start, start + smallofs, keyText=None), zheight=-1, dsn=1)
+        p.setBounds(gti0 - smallofs, gti1 + smallofs)
 
 
-class Events (GTIData):
+class Events(GTIData):
     events = None
     """DataFrame of event data. Columns are:
 
     ccd_id
       CCD on which the event happened.
     chipx, chipy
       Row/column on each individual chip.
@@ -206,52 +207,56 @@
     dmjd
       Event time as MJD-MJD0 (added in software).
 
     """
     exposure = None
     """The total effective exposure time, in seconds."""
 
-    def _process_main (self, hdulist, header):
-        super (Events, self)._process_main (hdulist, header)
+    def _process_main(self, hdulist, header):
+        super(Events, self)._process_main(hdulist, header)
 
-        hdu = hdulist['EVENTS']
-        self.exposure = hdu.header.get('exposure')
-        self.events = fits_recarray_to_data_frame (hdu.data)
+        hdu = hdulist["EVENTS"]
+        self.exposure = hdu.header.get("exposure")
+        self.events = fits_recarray_to_data_frame(hdu.data)
 
         if self.t0 is None:
-            self.t0 = self.events.time.min ()
+            self.t0 = self.events.time.min()
             if not np.isfinite(self.t0):
                 # Can happen if there are zero events!
-                self.t0 = 51544.5 # J2000 epoch as MJD
+                self.t0 = 51544.5  # J2000 epoch as MJD
 
         if self.mjd0 is None:
-            self.mjd0 = np.floor (self.t0 / 86400 + self.mjdref)
-
-        self.events['mjd'] = self.events.time / 86400 + self.mjdref
-        self.events['dks'] = 1e-3 * (self.events.time - self.t0)
-        self.events['dmjd'] = self.events.mjd - self.mjd0
+            self.mjd0 = np.floor(self.t0 / 86400 + self.mjdref)
 
+        self.events["mjd"] = self.events.time / 86400 + self.mjdref
+        self.events["dks"] = 1e-3 * (self.events.time - self.t0)
+        self.events["dmjd"] = self.events.mjd - self.mjd0
 
-    def _process_hdu (self, hdu):
+    def _process_hdu(self, hdu):
         "We've hacked the load order a bit to get t0 and mjd0 in _process_main()."
 
-        if hdu.name == 'EVENTS':
+        if hdu.name == "EVENTS":
             pass
         else:
-            super (Events, self)._process_hdu (hdu)
-
+            super(Events, self)._process_hdu(hdu)
 
-    def _plot_binned_event_energies(self, bbinfo, energy_scale=1., time_key='dmjd',
-                                    target_max_per_bin=100, **kwargs):
+    def _plot_binned_event_energies(
+        self,
+        bbinfo,
+        energy_scale=1.0,
+        time_key="dmjd",
+        target_max_per_bin=100,
+        **kwargs
+    ):
         import omega as om
         from scipy.stats.mstats_extras import mjci
 
         p = om.RectPlot()
         time = self.events[time_key]
-        energy = self.events['energy'] * energy_scale
+        energy = self.events["energy"] * energy_scale
 
         for ledge, redge in zip(bbinfo.ledges, bbinfo.redges):
             subset = self.events[(time >= ledge) & (time < redge)]
             n = subset.shape[0]
 
             if n == 0:
                 continue
@@ -268,123 +273,135 @@
                 if subsubset.shape[0] == 0:
                     continue
 
                 subsubenergy = energy[matched]
                 med_energy = subsubenergy.median()
                 u_med_energy = mjci(subsubenergy.data, prob=0.5).item()
                 p.addXY([t0, t1], [med_energy, med_energy], None, **kwargs)
-                p.addXY([tmid, tmid], [med_energy - u_med_energy, med_energy + u_med_energy],
-                        None, **kwargs)
+                p.addXY(
+                    [tmid, tmid],
+                    [med_energy - u_med_energy, med_energy + u_med_energy],
+                    None,
+                    **kwargs
+                )
 
         return p
 
-
-    def plot_lightcurve (self, ccd_id=None, bin_energies=False):
+    def plot_lightcurve(self, ccd_id=None, bin_energies=False):
         import omega as om
         from ...bblocks import tt_bblock
 
         if ccd_id is None:
-            if len (self.gti) != 1:
-                raise Exception ('must specify ccd_id')
+            if len(self.gti) != 1:
+                raise Exception("must specify ccd_id")
             ccd_id = list(self.gti.keys())[0]
 
-        kev = self.events['energy'] * 1e-3
-        vb = om.layout.VBox (2)
+        kev = self.events["energy"] * 1e-3
+        vb = om.layout.VBox(2)
 
         if kev.size == 0:
             vb[0] = om.RectPlot()
             vb[1] = om.RectPlot()
-            tmin = self.gti[ccd_id]['start_dmjd'].min()
-            tmax = self.gti[ccd_id]['stop_dmjd'].max()
+            tmin = self.gti[ccd_id]["start_dmjd"].min()
+            tmax = self.gti[ccd_id]["stop_dmjd"].max()
             if np.isnan(tmin):
-                tmin, tmax = -1., 1.
-            emin, emax = -1., 1.
-            rmin, rmax = -1., 1.
+                tmin, tmax = -1.0, 1.0
+            emin, emax = -1.0, 1.0
+            rmin, rmax = -1.0, 1.0
         else:
-            bbinfo = tt_bblock (
-                self.gti[ccd_id]['start_dmjd'],
-                self.gti[ccd_id]['stop_dmjd'],
-                self.events['dmjd'],
-                intersect_with_bins = True,
+            bbinfo = tt_bblock(
+                self.gti[ccd_id]["start_dmjd"],
+                self.gti[ccd_id]["stop_dmjd"],
+                self.events["dmjd"],
+                intersect_with_bins=True,
             )
             cps = bbinfo.rates / 86400
 
-            tmin, tmax = tight_bounds (bbinfo.ledges[0], bbinfo.redges[-1])
-            emin, emax = tight_bounds (kev.min (), kev.max ())
-            rmin, rmax = tight_bounds (cps.min (), cps.max ())
-
-            vb[0] = om.RectPlot ()
-            csp = om.rect.ContinuousSteppedPainter (keyText='%d events' % (self.events.shape[0]))
-            csp.setFloats (np.concatenate ((bbinfo.ledges, bbinfo.redges[-1:])),
-                           np.concatenate ((cps, [0])))
-            vb[0].add (csp)
+            tmin, tmax = tight_bounds(bbinfo.ledges[0], bbinfo.redges[-1])
+            emin, emax = tight_bounds(kev.min(), kev.max())
+            rmin, rmax = tight_bounds(cps.min(), cps.max())
+
+            vb[0] = om.RectPlot()
+            csp = om.rect.ContinuousSteppedPainter(
+                keyText="%d events" % (self.events.shape[0])
+            )
+            csp.setFloats(
+                np.concatenate((bbinfo.ledges, bbinfo.redges[-1:])),
+                np.concatenate((cps, [0])),
+            )
+            vb[0].add(csp)
 
             if bin_energies:
                 vb[1] = self._plot_binned_event_energies(
-                    bbinfo,
-                    energy_scale = 1e-3,
-                    dsn = 0
+                    bbinfo, energy_scale=1e-3, dsn=0
                 )
             else:
-                vb[1] = om.quickXY (self.events['dmjd'], kev, None, lines=0)
+                vb[1] = om.quickXY(self.events["dmjd"], kev, None, lines=0)
 
-        vb[0].setBounds (tmin, tmax, rmin, rmax)
-        vb[0].setYLabel ('Count rate (ct/s)')
+        vb[0].setBounds(tmin, tmax, rmin, rmax)
+        vb[0].setYLabel("Count rate (ct/s)")
         vb[0].bpainter.paintLabels = False
-        self._plot_add_gtis (vb[0], ccd_id)
+        self._plot_add_gtis(vb[0], ccd_id)
 
-        vb[1].setBounds (tmin, tmax, emin, emax)
-        vb[1].setLabels ('MJD - %d' % self.mjd0, 'Energy (keV)')
-        self._plot_add_gtis (vb[1], ccd_id)
+        vb[1].setBounds(tmin, tmax, emin, emax)
+        vb[1].setLabels("MJD - %d" % self.mjd0, "Energy (keV)")
+        self._plot_add_gtis(vb[1], ccd_id)
         return vb
 
-
-    def print_lightcurve (self, ccd_id=None, header=True):
+    def print_lightcurve(self, ccd_id=None, header=True):
         from ...bblocks import tt_bblock
 
         if ccd_id is None:
-            if len (self.gti) != 1:
-                raise Exception ('must specify ccd_id')
+            if len(self.gti) != 1:
+                raise Exception("must specify ccd_id")
             ccd_id = list(self.gti.keys())[0]
 
-        kev = self.events['energy'] * 1e-3
+        kev = self.events["energy"] * 1e-3
 
-        bbinfo = tt_bblock (
-            self.gti[ccd_id]['start_dmjd'],
-            self.gti[ccd_id]['stop_dmjd'],
-            self.events['dmjd'],
-            intersect_with_bins = True,
+        bbinfo = tt_bblock(
+            self.gti[ccd_id]["start_dmjd"],
+            self.gti[ccd_id]["stop_dmjd"],
+            self.events["dmjd"],
+            intersect_with_bins=True,
         )
         cps = bbinfo.rates / 86400
         tprev = None
 
         if header:
-            print('%7s  %8s  %8s  %5s  %7s  %4s' % ('Gap', 'Tstart', 'Tstop', 'Nevt', 'Ct/s', 'keV'))
+            print(
+                "%7s  %8s  %8s  %5s  %7s  %4s"
+                % ("Gap", "Tstart", "Tstop", "Nevt", "Ct/s", "keV")
+            )
 
         for i in range(bbinfo.rates.size):
             tstart = bbinfo.ledges[i]
             tstop = bbinfo.redges[i]
             rate = cps[i]
 
             if tprev is None:
-                gapstr = ''
+                gapstr = ""
             elif tstart == tprev:
-                gapstr = '--'
+                gapstr = "--"
             else:
-                gapstr = '%7.5f' % (tstart - tprev)
+                gapstr = "%7.5f" % (tstart - tprev)
 
-            subset = self.events[(self.events['dmjd'] >= tstart) & (self.events['dmjd'] < tstop)]
+            subset = self.events[
+                (self.events["dmjd"] >= tstart) & (self.events["dmjd"] < tstop)
+            ]
             n = subset.shape[0]
-            kev = subset['energy'].median() * 1e-3
+            kev = subset["energy"].median() * 1e-3
 
-            print('%7s  %8.5f  %8.5f  %5d  %7.4f  %4.1f' % (gapstr, tstart, tstop, n, rate, kev))
+            print(
+                "%7s  %8.5f  %8.5f  %5d  %7.4f  %4.1f"
+                % (gapstr, tstart, tstop, n, rate, kev)
+            )
             tprev = tstop
 
 
-class OIFData (BaseCIAOData):
+class OIFData(BaseCIAOData):
     contents = None
     """DataFrame giving information about the various files in a Chandra dataset.
     Columns are:
 
     member_content
       E.g. "OIF", "BADPIX", "BIAS0", "mtl"; there are duplicates.
     member_date-end
@@ -406,22 +423,23 @@
     member_uri_type
       All "URL" in my example.
     member_version
       Processing version number? Mostly 1 in my example.
     member_xtension
       Extension type? "PRIMARY" or "BINTABLE" in my example.
     """
-    def _process_hdu (self, hdu):
-        if hdu.name == 'GROUPING':
-            self.contents = fits_recarray_to_data_frame (hdu.data)
+
+    def _process_hdu(self, hdu):
+        if hdu.name == "GROUPING":
+            self.contents = fits_recarray_to_data_frame(hdu.data)
         else:
-            super (OIFData, self)._process_hdu (hdu)
+            super(OIFData, self)._process_hdu(hdu)
 
 
-class ChandraDataSet (object):
+class ChandraDataSet(object):
     path = None
     "A `pwkit.io.Path` pointing to the data set top level."
 
     timesys = None
     "Time reference system used; e.g. 'TT'."
 
     mjdref = None
@@ -435,79 +453,83 @@
     mjd0 = None
     "Offset MJD; default mjd0 = floor (t0 / 86400 + mjdref)."
 
     _toc = None
     "Table of Contents of data files within this dataset."
 
     _content_to_factory = {
-        'oif': OIFData,
-        'badpix': BaseCIAOData,
-        'fov': BaseCIAOData,
-        'hiresimg': BaseCIAOData,
-        'evt2': Events,
-        'loresimg': BaseCIAOData,
-        'orbitephem1': BaseCIAOData,
-        'aspsol': BaseCIAOData,
-        'evt1': Events,
-        'gti': BaseCIAOData,
-        'msk': BaseCIAOData,
-        'mtl': BaseCIAOData,
-        'expstats': BaseCIAOData,
-        'pbk': BaseCIAOData,
-        'aspqual': BaseCIAOData,
-        'angleephem': BaseCIAOData,
-        'lunarephem1': BaseCIAOData,
-        'solarephem1': BaseCIAOData,
+        "oif": OIFData,
+        "badpix": BaseCIAOData,
+        "fov": BaseCIAOData,
+        "hiresimg": BaseCIAOData,
+        "evt2": Events,
+        "loresimg": BaseCIAOData,
+        "orbitephem1": BaseCIAOData,
+        "aspsol": BaseCIAOData,
+        "evt1": Events,
+        "gti": BaseCIAOData,
+        "msk": BaseCIAOData,
+        "mtl": BaseCIAOData,
+        "expstats": BaseCIAOData,
+        "pbk": BaseCIAOData,
+        "aspqual": BaseCIAOData,
+        "angleephem": BaseCIAOData,
+        "lunarephem1": BaseCIAOData,
+        "solarephem1": BaseCIAOData,
     }
 
-    def __init__ (self, path):
-        self.path = Path (path)
-        self._toc = {'oif': (self.path / 'oif.fits', OIFData)}
+    def __init__(self, path):
+        self.path = Path(path)
+        self._toc = {"oif": (self.path / "oif.fits", OIFData)}
 
-        if not self._toc['oif'][0].exists ():
+        if not self._toc["oif"][0].exists():
             # This is nominally racy against the load(), but should be convenient.
-            raise ValueError ('%r does not appear to point to a Chandra data set (no oif.fits inside)'
-                              % (path, ))
+            raise ValueError(
+                "%r does not appear to point to a Chandra data set (no oif.fits inside)"
+                % (path,)
+            )
 
-        with self.lookup ('oif').read_fits () as hdul:
-            self.timesys = hdul['GROUPING'].header['TIMESYS']
-            self.mjdref = hdul['GROUPING'].header['MJDREF']
-            self.t0 = hdul['GROUPING'].header['TSTART']
-            self.mjd0 = np.floor (self.t0 / 86400 + self.mjdref)
-            contents = fits_recarray_to_data_frame (hdul['GROUPING'].data)
+        with self.lookup("oif").read_fits() as hdul:
+            self.timesys = hdul["GROUPING"].header["TIMESYS"]
+            self.mjdref = hdul["GROUPING"].header["MJDREF"]
+            self.t0 = hdul["GROUPING"].header["TSTART"]
+            self.mjd0 = np.floor(self.t0 / 86400 + self.mjdref)
+            contents = fits_recarray_to_data_frame(hdul["GROUPING"].data)
 
-        for idx, row in contents.iterrows ():
-            content = row.member_content.strip ().lower ()
+        for idx, row in contents.iterrows():
+            content = row.member_content.strip().lower()
 
-            if content == 'oif':
-                continue # already dealt with
+            if content == "oif":
+                continue  # already dealt with
 
-            if content in ('bias0', 'obcsol'):
+            if content in ("bias0", "obcsol"):
                 # XXX: multiple files; not sure what to do about them
                 continue
 
-            factory = self._content_to_factory.get (content)
+            factory = self._content_to_factory.get(content)
             if factory is None:
-                warn ('unexpected member_content %r in %s:oif.fits', content, self.path)
+                warn("unexpected member_content %r in %s:oif.fits", content, self.path)
                 continue
 
-            p = row.member_location.strip ()
-            if p.startswith ('./'):
+            p = row.member_location.strip()
+            if p.startswith("./"):
                 p = p[2:]
             p = self.path / p
 
-            if not p.exists ():
-                p = p.with_name (p.name + '.gz')
-                if not p.exists ():
-                    warn ('missing member %r (from %s:oif.fits)', row.member_location, self.path)
+            if not p.exists():
+                p = p.with_name(p.name + ".gz")
+                if not p.exists():
+                    warn(
+                        "missing member %r (from %s:oif.fits)",
+                        row.member_location,
+                        self.path,
+                    )
                     continue
 
             self._toc[content] = (p, factory)
 
-
-    def lookup (self, itemname):
+    def lookup(self, itemname):
         return self._toc[itemname][0]
 
-
-    def load (self, itemname, **kwargs):
+    def load(self, itemname, **kwargs):
         path, factory = self._toc[itemname]
-        return factory (path, t0=self.t0, mjd0=self.mjd0, **kwargs)
+        return factory(path, t0=self.t0, mjd0=self.mjd0, **kwargs)
```

### Comparing `pwkit-1.1.1/pwkit/environments/heasoft.py` & `pwkit-1.2.0/pwkit/environments/heasoft.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/environments/jupyter/__init__.py` & `pwkit-1.2.0/pwkit/environments/jupyter/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,179 +3,181 @@
 # Licensed under the MIT License.
 
 """jupyter - extensions for the Jupyter/IPython project
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('JupyterTool commandline').split ()
+__all__ = str("JupyterTool commandline").split()
 
-from ... import PKError, cli
+from ... import cli
 from ...io import Path
 from ...cli import multitool
 
 import logging, sys
 from notebook import notebookapp
 
-class BgNotebookApp (notebookapp.NotebookApp):
-    def initialize (self, argv=None):
-        self.port = 0 # => auto-choose port
-        self.open_browser = False
-        super (BgNotebookApp, self).initialize (argv)
 
+class BgNotebookApp(notebookapp.NotebookApp):
+    def initialize(self, argv=None):
+        self.port = 0  # => auto-choose port
+        self.open_browser = False
+        super(BgNotebookApp, self).initialize(argv)
 
-    def _log_level_default (self):
+    def _log_level_default(self):
         return logging.ERROR
 
-
-    def init_webapp (self):
-        super (BgNotebookApp, self).init_webapp ()
+    def init_webapp(self):
+        super(BgNotebookApp, self).init_webapp()
         # Update fields to reflect the port that was actually chosen.
-        sock = list (self.http_server._sockets.values ())[0]
-        self.port = sock.getsockname ()[1]
+        sock = list(self.http_server._sockets.values())[0]
+        self.port = sock.getsockname()[1]
 
 
-def get_server_cwd ():
-    return Path ('~').expand (user=True)
+def get_server_cwd():
+    return Path("~").expand(user=True)
 
 
-def get_server_info ():
-    servercwd = get_server_cwd ()
+def get_server_info():
+    servercwd = get_server_cwd()
 
-    for info in notebookapp.list_running_servers ():
-        if Path (info['notebook_dir']) == servercwd:
+    for info in notebookapp.list_running_servers():
+        if Path(info["notebook_dir"]) == servercwd:
             return info
 
     return None
 
 
 # Command-line interface
 
-class BgNotebookCommand (multitool.Command):
-    name = 'bg-notebook'
-    argspec = ''
-    summary = 'Start a standardized notebook server in the background if needed.'
+
+class BgNotebookCommand(multitool.Command):
+    name = "bg-notebook"
+    argspec = ""
+    summary = "Start a standardized notebook server in the background if needed."
     help_if_no_args = False
-    more_help = '''\
+    more_help = """\
 A new server will only be started if necessary. Regardless of whether a server
 was started or not, the only thing that will be printed is the base URL at
 which the server may be accessed. Unlike the standard setup, the port on which
 the server listens will probably not be 8888, because we ask the OS to
-determine it automatically. '''
+determine it automatically. """
 
-    def invoke (self, args, **kwargs):
+    def invoke(self, args, **kwargs):
         import os
 
-        if len (args):
-            raise multitool.UsageError ('mynotebook takes no arguments')
+        if len(args):
+            raise multitool.UsageError("mynotebook takes no arguments")
 
         # See if there's a running server that we can suggest.
-        servercwd = get_server_cwd ()
+        servercwd = get_server_cwd()
 
-        for info in notebookapp.list_running_servers ():
-            if Path (info['notebook_dir']) == servercwd:
-                print (info['url'])
+        for info in notebookapp.list_running_servers():
+            if Path(info["notebook_dir"]) == servercwd:
+                print(info["url"])
                 return
 
         # OK, need to start a server
 
-        info = cli.fork_detached_process ()
-        if info.whoami == 'original':
-            url = info.pipe.readline ().strip ()
-            if not len (url):
-                cli.die ('notebook server (PID %d) appears to have crashed', info.forkedpid)
-            print (url.decode ('ascii'))
+        info = cli.fork_detached_process()
+        if info.whoami == "original":
+            url = info.pipe.readline().strip()
+            if not len(url):
+                cli.die(
+                    "notebook server (PID %d) appears to have crashed", info.forkedpid
+                )
+            print(url.decode("ascii"))
         else:
             # We're the child. Set up to run as a background daemon as much as
             # possible, then indicate to the parent that things look OK. NOTE:
             # notebook's `argv` should not include what's traditionally called
             # `argv[0]`.
 
-            os.chdir (str (servercwd))
+            os.chdir(str(servercwd))
 
-            app = BgNotebookApp.instance ()
-            app.initialize (argv=[])
+            app = BgNotebookApp.instance()
+            app.initialize(argv=[])
 
-            info.pipe.write (app.display_url.encode ('ascii'))
-            info.pipe.write (b'\n')
-            info.pipe.close ()
+            info.pipe.write(app.display_url.encode("ascii"))
+            info.pipe.write(b"\n")
+            info.pipe.close()
 
-            with open (os.devnull, 'rb') as devnull:
-                os.dup2 (devnull.fileno (), 0)
+            with open(os.devnull, "rb") as devnull:
+                os.dup2(devnull.fileno(), 0)
 
-            with open (os.devnull, 'wb') as devnull:
+            with open(os.devnull, "wb") as devnull:
                 for fd in 1, 2:
-                    os.dup2 (devnull.fileno (), fd)
+                    os.dup2(devnull.fileno(), fd)
 
             # Enter the main loop, never to leave again.
-            app.start ()
+            app.start()
 
 
-class GetNotebookPidCommand (multitool.Command):
-    name = 'get-notebook-pid'
-    argspec = ''
-    summary = 'Print the PID of the currently running notebook server, if any.'
+class GetNotebookPidCommand(multitool.Command):
+    name = "get-notebook-pid"
+    argspec = ""
+    summary = "Print the PID of the currently running notebook server, if any."
     help_if_no_args = False
-    more_help = '''\
+    more_help = """\
 If no server is currently running, a message is printed to standard error but
-nothing is printed to stdout. Furthermore the exit code in this case is 1.'''
+nothing is printed to stdout. Furthermore the exit code in this case is 1."""
 
-    def invoke (self, args, **kwargs):
-        if len (args):
-            raise multitool.UsageError ('get-notebook-pid takes no arguments')
+    def invoke(self, args, **kwargs):
+        if len(args):
+            raise multitool.UsageError("get-notebook-pid takes no arguments")
 
-        info = get_server_info ()
+        info = get_server_info()
         if info is None:
-            print ('(no notebook server is currently running)', file=sys.stderr)
-            sys.exit (1)
+            print("(no notebook server is currently running)", file=sys.stderr)
+            sys.exit(1)
 
-        print (info['pid'])
+        print(info["pid"])
 
 
-class KillNotebookCommand (multitool.Command):
-    name = 'kill-notebook'
-    argspec = ''
-    summary = 'Kill the currently running notebook server, if any.'
+class KillNotebookCommand(multitool.Command):
+    name = "kill-notebook"
+    argspec = ""
+    summary = "Kill the currently running notebook server, if any."
     help_if_no_args = False
-    more_help = '''\
+    more_help = """\
 If no server is currently running, a warning is printed to standard error, and
-the exit code is 1.'''
+the exit code is 1."""
 
-    def invoke (self, args, **kwargs):
-        if len (args):
-            raise multitool.UsageError ('kill-notebook takes no arguments')
+    def invoke(self, args, **kwargs):
+        if len(args):
+            raise multitool.UsageError("kill-notebook takes no arguments")
 
-        info = get_server_info ()
+        info = get_server_info()
         if info is None:
-            print ('(no notebook server is currently running)', file=sys.stderr)
-            sys.exit (1)
+            print("(no notebook server is currently running)", file=sys.stderr)
+            sys.exit(1)
 
         # Not sure what Jupyter does when it gets SIGTERM, but to be safe let's
         # shut down everything
         from requests import request
         from notebook.utils import url_path_join as ujoin
 
-        def command (verb, *paths):
-            resp = request (verb, ujoin (info['url'], *paths))
-            resp.raise_for_status ()
+        def command(verb, *paths):
+            resp = request(verb, ujoin(info["url"], *paths))
+            resp.raise_for_status()
             return resp
 
-        for sessinfo in command ('GET', 'api/sessions').json ():
-            command ('DELETE', 'api/sessions', sessinfo['id'])
+        for sessinfo in command("GET", "api/sessions").json():
+            command("DELETE", "api/sessions", sessinfo["id"])
 
-        for kerninfo in command ('GET', 'api/kernels').json ():
-            command ('DELETE', 'api/kernels', kerninfo['id'])
+        for kerninfo in command("GET", "api/kernels").json():
+            command("DELETE", "api/kernels", kerninfo["id"])
 
         import os, signal
-        os.kill (info['pid'], signal.SIGTERM)
+
+        os.kill(info["pid"], signal.SIGTERM)
 
 
-class JupyterTool (multitool.Multitool):
-    cli_name = 'pkenvtool jupyter'
-    summary = 'Helpers for the Jupyter environment.'
+class JupyterTool(multitool.Multitool):
+    cli_name = "pkenvtool jupyter"
+    summary = "Helpers for the Jupyter environment."
 
 
-def commandline (argv):
-    from six import itervalues
-    tool = JupyterTool ()
-    tool.populate (itervalues (globals ()))
-    tool.commandline (argv)
+def commandline(argv):
+    tool = JupyterTool()
+    tool.populate(globals().values())
+    tool.commandline(argv)
```

### Comparing `pwkit-1.1.1/pwkit/environments/sas/__init__.py` & `pwkit-1.2.0/pwkit/environments/sas/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -88,22 +88,22 @@
 
 See the ``make-*-aliases`` commands for tools that generate symlinks with saner
 names.
 
 """
 from __future__ import absolute_import, division, print_function
 
-__all__ = ''.split()
+__all__ = "".split()
 
-import io, os.path, six
+import os.path
 
 from ... import PKError, cli
 from ...cli import multitool
 from ...io import Path
-from .. import Environment, prepend_environ_path, user_data_path
+from .. import Environment, prepend_environ_path
 
 
 class SasEnvironment(Environment):
     _odfdir = None
     _revnum = None
     _obsid = None
     _sumsas = None
@@ -111,232 +111,235 @@
     _heaenv = None
 
     def __init__(self, manifest, installdir=None, heaenv=None):
         if installdir is None:
             installdir = self._default_installdir()
         if heaenv is None:
             from .. import heasoft
+
             heaenv = heasoft.HeasoftEnvironment()
 
         self._installdir = os.path.abspath(installdir)
         self._heaenv = heaenv
 
         # TODO: I used to read the manifest file to infer both the revolution
         # number and obsid, but in the case of 0673000145, the obsid mentioned
         # in the manifest is different! (But close: 0673000101.) So now I glob
         # the containing directory for that.
 
         manifest = Path(manifest)
 
         for line in manifest.read_lines():
-            if not line.startswith('File '):
+            if not line.startswith("File "):
                 continue
 
-            bits = line.split()[1].split('_')
+            bits = line.split()[1].split("_")
             if len(bits) < 3:
                 continue
 
-            self._revnum = bits[0] # note: kept as a string; not an int
+            self._revnum = bits[0]  # note: kept as a string; not an int
             break
 
         self._odfdir = Path(manifest).resolve().parent
 
-        for p in self._odfdir.glob('%s_*_*.FIT' % self._revnum):
-            bits = p.name.split('_')
+        for p in self._odfdir.glob("%s_*_*.FIT" % self._revnum):
+            bits = p.name.split("_")
             self._obsid = bits[1]
             break
 
-        self._sumsas = self._odfdir / ('%s_%s_SCX00000SUM.SAS' % (self._revnum, self._obsid))
-
+        self._sumsas = self._odfdir / (
+            "%s_%s_SCX00000SUM.SAS" % (self._revnum, self._obsid)
+        )
 
     def _default_installdir(self):
-        d = os.environ.get('PWKIT_SAS')
+        d = os.environ.get("PWKIT_SAS")
         if d is None:
-            raise PKError('SAS installation directory must be specified '
-                          'in the $PWKIT_SAS environment variable')
+            raise PKError(
+                "SAS installation directory must be specified "
+                "in the $PWKIT_SAS environment variable"
+            )
         return d
 
-
     def modify_environment(self, env):
         self._heaenv.modify_environment(env)
 
         def path(*args):
             return os.path.join(self._installdir, *args)
 
-        env['SAS_DIR'] = path()
-        env['SAS_PATH'] = env['SAS_DIR']
-        env['SAS_CCFPATH'] = path('ccf')
-        env['SAS_ODF'] = str(self._sumsas) # but see _preexec
-        env['SAS_CCF'] = str(self._odfdir / 'ccf.cif')
-
-        prepend_environ_path(env, 'PATH', path('bin'))
-        prepend_environ_path(env, 'LD_LIBRARY_PATH', path('libextra'))
-        prepend_environ_path(env, 'LD_LIBRARY_PATH', path('lib'))
-        prepend_environ_path(env, 'PERL5LIB', path('lib', 'perl5'))
-
-        env['SAS_BROWSER'] = 'firefox' # yay hardcoding
-        env['SAS_IMAGEVIEWER'] = 'ds9'
-        env['SAS_SUPPRESS_WARNING'] = '1'
-        env['SAS_VERBOSITY'] = '4'
+        env["SAS_DIR"] = path()
+        env["SAS_PATH"] = env["SAS_DIR"]
+        env["SAS_CCFPATH"] = path("ccf")
+        env["SAS_ODF"] = str(self._sumsas)  # but see _preexec
+        env["SAS_CCF"] = str(self._odfdir / "ccf.cif")
+
+        prepend_environ_path(env, "PATH", path("bin"))
+        prepend_environ_path(env, "LD_LIBRARY_PATH", path("libextra"))
+        prepend_environ_path(env, "LD_LIBRARY_PATH", path("lib"))
+        prepend_environ_path(env, "PERL5LIB", path("lib", "perl5"))
+
+        env["SAS_BROWSER"] = "firefox"  # yay hardcoding
+        env["SAS_IMAGEVIEWER"] = "ds9"
+        env["SAS_SUPPRESS_WARNING"] = "1"
+        env["SAS_VERBOSITY"] = "4"
 
         # These can be helpful:
-        env['PWKIT_SAS_REVNUM'] = self._revnum
-        env['PWKIT_SAS_OBSID'] = self._obsid
+        env["PWKIT_SAS_REVNUM"] = self._revnum
+        env["PWKIT_SAS_OBSID"] = self._obsid
 
         return env
 
-
     def _preexec(self, env, printbuilds=True):
         from ...cli import wrapout
 
         # Need to compile the CCF info?
 
-        cif = env['SAS_CCF']
+        cif = env["SAS_CCF"]
         if not os.path.exists(cif):
             if printbuilds:
-                print('[building %s]' % cif)
+                print("[building %s]" % cif)
 
-            env['SAS_ODF'] = str(self._odfdir)
-            log = self._odfdir / 'cifbuild.log'
+            env["SAS_ODF"] = str(self._odfdir)
+            log = self._odfdir / "cifbuild.log"
 
-            with log.open('wb') as f:
+            with log.open("wb") as f:
                 w = wrapout.Wrapper(f)
                 w.use_colors = True
-                if w.launch('cifbuild', ['cifbuild'], env=env, cwd=str(self._odfdir)):
-                    raise PKError('failed to build CIF; see %s', log)
+                if w.launch("cifbuild", ["cifbuild"], env=env, cwd=str(self._odfdir)):
+                    raise PKError("failed to build CIF; see %s", log)
 
             if not os.path.exists(cif):
                 # cifbuild can exit with status 0 whilst still having failed
-                raise PKError('failed to build CIF; see %s', log)
+                raise PKError("failed to build CIF; see %s", log)
 
-            env['SAS_ODF'] = str(self._sumsas)
+            env["SAS_ODF"] = str(self._sumsas)
 
         # Need to generate SUM.SAS file?
 
         if not self._sumsas.exists():
             if printbuilds:
-                print('[building %s]' % self._sumsas)
+                print("[building %s]" % self._sumsas)
 
-            env['SAS_ODF'] = str(self._odfdir)
-            log = self._odfdir / 'odfingest.log'
+            env["SAS_ODF"] = str(self._odfdir)
+            log = self._odfdir / "odfingest.log"
 
-            with log.open('wb') as f:
+            with log.open("wb") as f:
                 w = wrapout.Wrapper(f)
                 w.use_colors = True
-                if w.launch('odfingest', ['odfingest'], env=env, cwd=str(self._odfdir)):
-                    raise PKError('failed to build CIF; see %s', log)
+                if w.launch("odfingest", ["odfingest"], env=env, cwd=str(self._odfdir)):
+                    raise PKError("failed to build CIF; see %s", log)
 
-            env['SAS_ODF'] = str(self._sumsas)
+            env["SAS_ODF"] = str(self._sumsas)
 
 
 # Command-line interface
 
+
 class Exec(multitool.Command):
-    name = 'exec'
-    argspec = '<manifest> <command> [args...]'
-    summary = 'Run a program in SAS.'
-    more_help = '''Due to the way SAS works, the path to a MANIFEST.nnnnn file in an ODF
+    name = "exec"
+    argspec = "<manifest> <command> [args...]"
+    summary = "Run a program in SAS."
+    more_help = """Due to the way SAS works, the path to a MANIFEST.nnnnn file in an ODF
 directory must be specified, and all operations work on the specified data
-set.'''
+set."""
 
     def invoke(self, args, **kwargs):
         if len(args) < 2:
-            raise multitool.UsageError('exec requires at least 2 arguments')
+            raise multitool.UsageError("exec requires at least 2 arguments")
 
         manifest = args[0]
         progargv = args[1:]
 
         env = SasEnvironment(manifest)
         env.execvpe(progargv)
 
 
 class MakeEPICAliases(multitool.Command):
-    name = 'make-epic-aliases'
-    argspec = '<srcdir> <destdir>'
-    summary = 'Generate user-friendly aliases to XMM-Newton EPIC data files.'
-    more_help = '''destdir should already not exist and will be created. <srcdir> should
-be the ODF directory, containing a file named MANIFEST.<numbers> and many others.'''
+    name = "make-epic-aliases"
+    argspec = "<srcdir> <destdir>"
+    summary = "Generate user-friendly aliases to XMM-Newton EPIC data files."
+    more_help = """destdir should already not exist and will be created. <srcdir> should
+be the ODF directory, containing a file named MANIFEST.<numbers> and many others."""
 
     INSTRUMENT = slice(16, 18)
-    EXPFLAG = slice(18, 19) # 'S': sched, 'U': unsched; 'X': N/A
+    EXPFLAG = slice(18, 19)  # 'S': sched, 'U': unsched; 'X': N/A
     EXPNO = slice(19, 22)
     CCDNO = slice(22, 24)
     DTYPE = slice(24, 27)
     EXTENSION = slice(28, None)
 
     instrmap = {
-        'M1': 'mos1',
-        'M2': 'mos2',
-        'PN': 'pn',
-        'RM': 'radmon',
+        "M1": "mos1",
+        "M2": "mos2",
+        "PN": "pn",
+        "RM": "radmon",
     }
 
     extmap = {
-        'FIT': 'fits',
+        "FIT": "fits",
     }
 
     dtypemap = {
-        'aux': 'aux',
-        'bue': 'burst',
-        'ccx': 'counting_cycle',
-        'cte': 'compressed_timing',
-        'dii': 'diagnostic',
-        'dli': 'discarded_lines',
-        'ecx': 'hk_extraheating_config', # or radiation mon count rate
-        'esx': 'spectra', # radiation monitor spectra, that is
-        'hbh': 'hk_hbr_buffer',
-        'hch': 'hk_hbr_config',
-        'hdi': 'high_rate_offset_data',
-        'hth': 'hk_hbr_threshold',
-        'ime': 'imaging',
-        'noi': 'noise',
-        'odi': 'offset_data',
-        'ove': 'offset_variance',
-        'pah': 'hk_additional',
-        'peh': 'hk_periodic',
-        'pmh': 'hk_main',
-        'pth': 'hk_bright_pixels',
-        'rie': 'reduced_imaging',
-        'tmh': 'hk_thermal_limits',
-        'tie': 'timing',
+        "aux": "aux",
+        "bue": "burst",
+        "ccx": "counting_cycle",
+        "cte": "compressed_timing",
+        "dii": "diagnostic",
+        "dli": "discarded_lines",
+        "ecx": "hk_extraheating_config",  # or radiation mon count rate
+        "esx": "spectra",  # radiation monitor spectra, that is
+        "hbh": "hk_hbr_buffer",
+        "hch": "hk_hbr_config",
+        "hdi": "high_rate_offset_data",
+        "hth": "hk_hbr_threshold",
+        "ime": "imaging",
+        "noi": "noise",
+        "odi": "offset_data",
+        "ove": "offset_variance",
+        "pah": "hk_additional",
+        "peh": "hk_periodic",
+        "pmh": "hk_main",
+        "pth": "hk_bright_pixels",
+        "rie": "reduced_imaging",
+        "tmh": "hk_thermal_limits",
+        "tie": "timing",
     }
 
     def invoke(self, args, **kwargs):
         if len(args) != 2:
-            raise multitool.UsageError('make-epic-aliases requires exactly 2 arguments')
+            raise multitool.UsageError("make-epic-aliases requires exactly 2 arguments")
 
         srcdir = Path(args[0])
         destdir = Path(args[1])
 
         srcpaths = [x for x in srcdir.iterdir() if len(x.name) > 28]
 
         # Sorted list of exposure numbers.
 
-        expnos = dict((i, set()) for i in six.iterkeys(self.instrmap))
+        expnos = dict((i, set()) for i in self.instrmap.keys())
 
         for p in srcpaths:
             instr = p.name[self.INSTRUMENT]
             if instr not in self.instrmap:
                 continue
 
             expno = int(p.name[self.EXPNO])
             dtype = p.name[self.DTYPE]
 
-            if expno > 0 and dtype not in ('DLI', 'ODI'):
+            if expno > 0 and dtype not in ("DLI", "ODI"):
                 expnos[instr].add(expno)
 
         expseqs = {}
 
-        for k, v in six.iteritems(expnos):
+        for k, v in expnos.items():
             expseqs[self.instrmap[k]] = dict((n, i) for i, n in enumerate(sorted(v)))
 
         # Do it.
 
         stems = set()
-        destdir.mkdir() # intentionally crash if exists; easiest approach
+        destdir.mkdir()  # intentionally crash if exists; easiest approach
 
         for p in srcpaths:
             instr = p.name[self.INSTRUMENT]
             if instr not in self.instrmap:
                 continue
 
             eflag = p.name[self.EXPFLAG]
@@ -346,92 +349,92 @@
             ext = p.name[self.EXTENSION]
 
             instr = self.instrmap[instr]
             expno = int(expno)
             dtype = self.dtypemap[dtype.lower()]
             ext = self.extmap[ext]
 
-            if expno > 0 and dtype not in ('discarded_lines', 'offset_data'):
+            if expno > 0 and dtype not in ("discarded_lines", "offset_data"):
                 expno = expseqs[instr][expno]
 
-            if instr == 'radmon' and dtype == 'hk_extraheating_config':
-                dtype = 'rates'
+            if instr == "radmon" and dtype == "hk_extraheating_config":
+                dtype = "rates"
 
-            if instr == 'radmon' or dtype == 'aux':
-                stem = '%s_e%03d_%s.%s' % (instr, expno, dtype, ext)
-            elif ccdno == '00':
-                stem = '%s_%s.%s' % (instr, dtype, ext)
-            elif dtype in ('discarded_lines', 'offset_data'):
-                stem = '%s_%s_e%03d_c%s.%s' % (instr, dtype, expno, ccdno, ext)
+            if instr == "radmon" or dtype == "aux":
+                stem = "%s_e%03d_%s.%s" % (instr, expno, dtype, ext)
+            elif ccdno == "00":
+                stem = "%s_%s.%s" % (instr, dtype, ext)
+            elif dtype in ("discarded_lines", "offset_data"):
+                stem = "%s_%s_e%03d_c%s.%s" % (instr, dtype, expno, ccdno, ext)
             else:
-                stem = '%s_e%03d_c%s_%s.%s' % (instr, expno, ccdno, dtype, ext)
+                stem = "%s_e%03d_c%s_%s.%s" % (instr, expno, ccdno, dtype, ext)
 
             if stem in stems:
-                cli.die('short identifier clash: %r', stem)
+                cli.die("short identifier clash: %r", stem)
             stems.add(stem)
 
             (destdir / stem).rellink_to(p)
 
 
 class MakeOMAliases(multitool.Command):
-    name = 'make-om-aliases'
-    argspec = '<srcdir> <destdir>'
-    summary = 'Generate user-friendly aliases to XMM-Newton OM data files.'
-    more_help = 'destdir should already not exist and will be created.'
+    name = "make-om-aliases"
+    argspec = "<srcdir> <destdir>"
+    summary = "Generate user-friendly aliases to XMM-Newton OM data files."
+    more_help = "destdir should already not exist and will be created."
 
-    PROD_TYPE = slice(0, 1) # 'P': final product; 'F': intermediate
+    PROD_TYPE = slice(0, 1)  # 'P': final product; 'F': intermediate
     OBSID = slice(1, 11)
-    EXPFLAG = slice(11, 12) # 'S': sched, 'U': unsched; 'X': N/A
-    EXPNO = slice(14, 17) # (12-14 is the string 'OM')
+    EXPFLAG = slice(11, 12)  # 'S': sched, 'U': unsched; 'X': N/A
+    EXPNO = slice(14, 17)  # (12-14 is the string 'OM')
     DTYPE = slice(17, 23)
     WINNUM = slice(23, 24)
     SRCNUM = slice(24, 27)
     EXTENSION = slice(28, None)
 
     extmap = {
-        'ASC': 'txt',
-        'FIT': 'fits',
-        'PDF': 'pdf',
-        'PS': 'ps',
+        "ASC": "txt",
+        "FIT": "fits",
+        "PDF": "pdf",
+        "PS": "ps",
     }
 
     dtypemap = {
-        'image_': 'image_ccd',
-        'simage': 'image_sky',
-        'swsrli': 'source_list',
-        'timesr': 'lightcurve',
-        'tshplt': 'tracking_plot',
-        'tstrts': 'tracking_stars',
+        "image_": "image_ccd",
+        "simage": "image_sky",
+        "swsrli": "source_list",
+        "timesr": "lightcurve",
+        "tshplt": "tracking_plot",
+        "tstrts": "tracking_stars",
     }
 
     def invoke(self, args, **kwargs):
         if len(args) != 2:
-            raise multitool.UsageError('make-om-aliases requires exactly 2 arguments')
+            raise multitool.UsageError("make-om-aliases requires exactly 2 arguments")
 
         from fnmatch import fnmatch
+
         srcdir, destdir = args
 
-        srcfiles = [x for x in os.listdir(srcdir)
-                    if x[0] == 'P' and len(x) > 28]
+        srcfiles = [x for x in os.listdir(srcdir) if x[0] == "P" and len(x) > 28]
 
         # Sorted list of exposure numbers.
 
         expnos = set()
 
         for f in srcfiles:
-            if not fnmatch(f, 'P*IMAGE_*.FIT'):
+            if not fnmatch(f, "P*IMAGE_*.FIT"):
                 continue
             expnos.add(f[self.EXPNO])
 
         expseqs = dict((n, i) for i, n in enumerate(sorted(expnos)))
 
         # Do it.
 
         idents = set()
-        os.mkdir(destdir) # intentionally crash if exists; easiest approach
+        os.mkdir(destdir)  # intentionally crash if exists; easiest approach
 
         for f in srcfiles:
             ptype = f[self.PROD_TYPE]
             obsid = f[self.OBSID]
             eflag = f[self.EXPFLAG]
             expno = f[self.EXPNO]
             dtype = f[self.DTYPE]
@@ -440,92 +443,92 @@
             ext = f[self.EXTENSION]
 
             seq = expseqs[expno]
             dtype = self.dtypemap[dtype.lower()]
             ext = self.extmap[ext]
 
             # There's only one clash, and it's easy:
-            if dtype == 'lightcurve' and ext == 'pdf':
+            if dtype == "lightcurve" and ext == "pdf":
                 continue
 
             ident = (seq, dtype)
             if ident in idents:
-                cli.die('short identifier clash: %r', ident)
+                cli.die("short identifier clash: %r", ident)
             idents.add(ident)
 
             oldpath = os.path.join(srcdir, f)
-            newpath = os.path.join(destdir, '%s.%02d.%s' % (dtype, seq, ext))
+            newpath = os.path.join(destdir, "%s.%02d.%s" % (dtype, seq, ext))
             os.symlink(os.path.relpath(oldpath, destdir), newpath)
 
 
 class MakeRGSAliases(multitool.Command):
-    name = 'make-rgs-aliases'
-    argspec = '<srcdir> <destdir>'
-    summary = 'Generate user-friendly aliases to XMM-Newton RGS data files.'
-    more_help = '''destdir should already not exist and will be created. <srcdir> should
-be the ODF directory, containing a file named MANIFEST.<numbers> and many others.'''
+    name = "make-rgs-aliases"
+    argspec = "<srcdir> <destdir>"
+    summary = "Generate user-friendly aliases to XMM-Newton RGS data files."
+    more_help = """destdir should already not exist and will be created. <srcdir> should
+be the ODF directory, containing a file named MANIFEST.<numbers> and many others."""
 
     INSTRUMENT = slice(16, 18)
-    EXPFLAG = slice(18, 19) # 'S': sched, 'U': unsched; 'X': N/A
+    EXPFLAG = slice(18, 19)  # 'S': sched, 'U': unsched; 'X': N/A
     EXPNO = slice(19, 22)
     CCDNO = slice(22, 24)
     DTYPE = slice(24, 27)
     EXTENSION = slice(28, None)
 
     instrmap = {
-        'R1': 'rgs1',
-        'R2': 'rgs2',
+        "R1": "rgs1",
+        "R2": "rgs2",
     }
 
     extmap = {
-        'FIT': 'fits',
+        "FIT": "fits",
     }
 
     dtypemap = {
-        'aux': 'aux',
-        'd1h': 'hk_dpp1',
-        'd2h': 'hk_dpp2',
-        'dii': 'diagnostic',
-        'hte': 'high_time_res',
-        'ofx': 'offset',
-        'pch': 'hk_ccd_temp',
-        'pfh': 'hk_periodic',
-        'spe': 'spectra',
+        "aux": "aux",
+        "d1h": "hk_dpp1",
+        "d2h": "hk_dpp2",
+        "dii": "diagnostic",
+        "hte": "high_time_res",
+        "ofx": "offset",
+        "pch": "hk_ccd_temp",
+        "pfh": "hk_periodic",
+        "spe": "spectra",
     }
 
     def invoke(self, args, **kwargs):
         if len(args) != 2:
-            raise multitool.UsageError('make-rgs-aliases requires exactly 2 arguments')
+            raise multitool.UsageError("make-rgs-aliases requires exactly 2 arguments")
 
         srcdir = Path(args[0])
         destdir = Path(args[1])
         srcpaths = [x for x in srcdir.iterdir() if len(x.name) > 28]
 
         # Sorted list of exposure numbers.
 
-        expnos = dict((i, set()) for i in six.iterkeys(self.instrmap))
+        expnos = dict((i, set()) for i in self.instrmap.keys())
 
         for p in srcpaths:
             instr = p.name[self.INSTRUMENT]
             if instr not in self.instrmap:
                 continue
 
             expno = int(p.name[self.EXPNO])
             if expno > 0 and expno < 900:
                 expnos[instr].add(expno)
 
         expseqs = {}
 
-        for k, v in six.iteritems(expnos):
+        for k, v in expnos.items():
             expseqs[self.instrmap[k]] = dict((n, i) for i, n in enumerate(sorted(v)))
 
         # Do it.
 
         stems = set()
-        destdir.mkdir() # intentionally crash if exists; easiest approach
+        destdir.mkdir()  # intentionally crash if exists; easiest approach
 
         for p in srcpaths:
             instr = p.name[self.INSTRUMENT]
             if instr not in self.instrmap:
                 continue
 
             eflag = p.name[self.EXPFLAG]
@@ -538,166 +541,175 @@
             expno = int(expno)
             dtype = self.dtypemap[dtype.lower()]
             ext = self.extmap[ext]
 
             if expno > 0 and expno < 900:
                 expno = expseqs[instr][expno]
 
-            if ccdno == '00' and dtype != 'aux':
-                stem = '%s_%s.%s' % (instr, dtype, ext)
-            elif dtype == 'aux':
-                stem = '%s_e%03d_%s.%s' % (instr, expno, dtype, ext)
-            elif dtype == 'diagnostic':
-                stem = '%s_%s_e%03d_c%s.%s' % (instr, dtype, expno, ccdno, ext)
+            if ccdno == "00" and dtype != "aux":
+                stem = "%s_%s.%s" % (instr, dtype, ext)
+            elif dtype == "aux":
+                stem = "%s_e%03d_%s.%s" % (instr, expno, dtype, ext)
+            elif dtype == "diagnostic":
+                stem = "%s_%s_e%03d_c%s.%s" % (instr, dtype, expno, ccdno, ext)
             else:
-                stem = '%s_e%03d_c%s_%s.%s' % (instr, expno, ccdno, dtype, ext)
+                stem = "%s_e%03d_c%s_%s.%s" % (instr, expno, ccdno, dtype, ext)
 
             if stem in stems:
-                cli.die('short identifier clash: %r', stem)
+                cli.die("short identifier clash: %r", stem)
             stems.add(stem)
 
             (destdir / stem).rellink_to(p)
 
 
 class MakeSCAliases(multitool.Command):
-    name = 'make-sc-aliases'
-    argspec = '<srcdir> <destdir>'
-    summary = 'Generate user-friendly aliases to XMM-Newton spacecraft (SC) data files.'
-    more_help = '''destdir should already not exist and will be created. <srcdir> should
-be the ODF directory, containing a file named MANIFEST.<numbers> and many others.'''
+    name = "make-sc-aliases"
+    argspec = "<srcdir> <destdir>"
+    summary = "Generate user-friendly aliases to XMM-Newton spacecraft (SC) data files."
+    more_help = """destdir should already not exist and will be created. <srcdir> should
+be the ODF directory, containing a file named MANIFEST.<numbers> and many others."""
 
     INSTRUMENT = slice(16, 18)
-    EXPFLAG = slice(18, 19) # 'S': sched, 'U': unsched; 'X': N/A
+    EXPFLAG = slice(18, 19)  # 'S': sched, 'U': unsched; 'X': N/A
     EXPNO = slice(19, 22)
     CCDNO = slice(22, 24)
     DTYPE = slice(24, 27)
     EXTENSION = slice(28, None)
 
     extmap = {
-        'ASC': 'txt',
-        'FIT': 'fits',
-        'SAS': 'txt',
+        "ASC": "txt",
+        "FIT": "fits",
+        "SAS": "txt",
     }
 
     dtypemap = {
-        'ats': 'attitude',
-        'das': 'dummy_attitude',
-        'pos': 'pred_orbit',
-        'p1s': 'phk_hk1',
-        'p2s': 'phk_hk2',
-        'p3s': 'phk_att1',
-        'p4s': 'phk_att2',
-        'p5s': 'phk_sid0',
-        'p6s': 'phk_sid1',
-        'p7s': 'phk_sid4',
-        'p8s': 'phk_sid5',
-        'p9s': 'phk_sid6',
-        'ras': 'raw_attitude',
-        'ros': 'recon_orbit',
-        'sum': 'summary',
-        'tcs': 'raw_time_corr',
-        'tcx': 'recon_time_corr',
+        "ats": "attitude",
+        "das": "dummy_attitude",
+        "pos": "pred_orbit",
+        "p1s": "phk_hk1",
+        "p2s": "phk_hk2",
+        "p3s": "phk_att1",
+        "p4s": "phk_att2",
+        "p5s": "phk_sid0",
+        "p6s": "phk_sid1",
+        "p7s": "phk_sid4",
+        "p8s": "phk_sid5",
+        "p9s": "phk_sid6",
+        "ras": "raw_attitude",
+        "ros": "recon_orbit",
+        "sum": "summary",
+        "tcs": "raw_time_corr",
+        "tcx": "recon_time_corr",
     }
 
     def invoke(self, args, **kwargs):
         if len(args) != 2:
-            raise multitool.UsageError('make-sc-aliases requires exactly 2 arguments')
+            raise multitool.UsageError("make-sc-aliases requires exactly 2 arguments")
 
         srcdir = Path(args[0])
         destdir = Path(args[1])
 
         srcfiles = [x for x in srcdir.iterdir() if len(x.name) > 28]
 
         # Do it.
 
         idents = set()
-        destdir.mkdir() # intentionally crash if exists; easiest approach
+        destdir.mkdir()  # intentionally crash if exists; easiest approach
 
         for p in srcfiles:
             instr = p.name[self.INSTRUMENT]
-            if instr != 'SC':
+            if instr != "SC":
                 continue
 
             # none of these are actually useful for SC files:
-            #eflag = p.name[self.EXPFLAG]
-            #expno = p.name[self.EXPNO]
-            #ccdno = p.name[self.CCDNO]
+            # eflag = p.name[self.EXPFLAG]
+            # expno = p.name[self.EXPNO]
+            # ccdno = p.name[self.CCDNO]
             dtype = p.name[self.DTYPE]
             ext = p.name[self.EXTENSION]
 
             # One conflict, easy to resolve
-            if dtype == 'SUM' and ext == 'ASC':
+            if dtype == "SUM" and ext == "ASC":
                 continue
 
             dtype = self.dtypemap[dtype.lower()]
             ext = self.extmap[ext]
 
             ident = dtype
             if ident in idents:
-                cli.die('short identifier clash: %r', ident)
+                cli.die("short identifier clash: %r", ident)
             idents.add(ident)
 
-            (destdir / (dtype + '.' + ext)).rellink_to(p)
+            (destdir / (dtype + "." + ext)).rellink_to(p)
 
 
 class Shell(multitool.Command):
     # XXX we hardcode bash! and we copy/paste from environments/__init__.py
-    name = 'shell'
-    argspec = '<manifest>'
-    summary = 'Start an interactive shell in the SAS environment.'
+    name = "shell"
+    argspec = "<manifest>"
+    summary = "Start an interactive shell in the SAS environment."
     help_if_no_args = False
-    more_help = '''Due to the way SAS works, the path to a MANIFEST.nnnnn file in an ODF
+    more_help = """Due to the way SAS works, the path to a MANIFEST.nnnnn file in an ODF
 directory must be specified, and all operations work on the specified data
-set.'''
+set."""
 
     def invoke(self, args, **kwargs):
         if len(args) != 1:
-            raise multitool.UsageError('shell expects exactly 1 argument')
+            raise multitool.UsageError("shell expects exactly 1 argument")
 
         env = SasEnvironment(args[0])
 
         from tempfile import NamedTemporaryFile
-        with NamedTemporaryFile(delete=False, mode='wt') as f:
-            print('''[ -e ~/.bashrc ] && source ~/.bashrc
+
+        with NamedTemporaryFile(delete=False, mode="wt") as f:
+            print(
+                """[ -e ~/.bashrc ] && source ~/.bashrc
 PS1="SAS(%s) $PS1"
-rm %s''' % (env._obsid, f.name), file=f)
+rm %s"""
+                % (env._obsid, f.name),
+                file=f,
+            )
 
-        env.execvpe(['bash', '--rcfile', f.name, '-i'])
+        env.execvpe(["bash", "--rcfile", f.name, "-i"])
 
 
 class UpdateCcf(multitool.Command):
-    name = 'update-ccf'
-    argspec = ''
+    name = "update-ccf"
+    argspec = ""
     summary = 'Update the SAS "current calibration files".'
-    more_help = 'This executes an rsync command to make sure the files are up-to-date.'
+    more_help = "This executes an rsync command to make sure the files are up-to-date."
     help_if_no_args = False
 
     def invoke(self, args, **kwargs):
         if len(args):
-            raise multitool.UsageError('update-ccf expects no arguments')
+            raise multitool.UsageError("update-ccf expects no arguments")
 
-        sasdir = os.environ.get('PWKIT_SAS')
+        sasdir = os.environ.get("PWKIT_SAS")
         if sasdir is None:
-            cli.die('environment variable $PWKIT_SAS must be set')
+            cli.die("environment variable $PWKIT_SAS must be set")
 
-        os.chdir(os.path.join(sasdir, 'ccf'))
-        os.execvp('rsync', ['rsync',
-                            '-av',
-                            '--delete',
-                            '--delete-after',
-                            '--force',
-                            '--include=*.CCF',
-                            '--exclude=*/',
-                            'xmm.esac.esa.int::XMM_VALID_CCF',
-                            '.'])
+        os.chdir(os.path.join(sasdir, "ccf"))
+        os.execvp(
+            "rsync",
+            [
+                "rsync",
+                "-av",
+                "--delete",
+                "--delete-after",
+                "--force",
+                "--include=*.CCF",
+                "--exclude=*/",
+                "xmm.esac.esa.int::XMM_VALID_CCF",
+                ".",
+            ],
+        )
 
 
 class SasTool(multitool.Multitool):
-    cli_name = 'pkenvtool sas'
-    summary = 'Run tools in the SAS environment.'
+    cli_name = "pkenvtool sas"
+    summary = "Run tools in the SAS environment."
 
 
 def commandline(argv):
-    from six import itervalues
     tool = SasTool()
-    tool.populate(itervalues(globals()))
+    tool.populate(globals().values())
     tool.commandline(argv)
```

### Comparing `pwkit-1.1.1/pwkit/environments/sas/data.py` & `pwkit-1.2.0/pwkit/environments/sas/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 # Licensed under the MIT License.
 
 """pwkit.environments.sas.data - loading up SAS data sets
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('BaseSASData Events GTIData Lightcurve RegionData').split ()
+__all__ = str("BaseSASData Events GTIData Lightcurve RegionData").split()
 
 import numpy as np, pandas as pd
-from six.moves import range
 from astropy.time import Time
 from ... import astutil, cli
 from ...io import Path
 from ...numutil import fits_recarray_to_data_frame
 
 
-class BaseSASData (object):
+class BaseSASData(object):
     telescope = None
     "Telescope name: likely 'XMM'"
 
     instrument = None
     "Instrument used: likely 'EMOS1', 'EMOS2', 'EPN'"
 
     obsid = None
@@ -87,146 +86,146 @@
     """Pixel-to-world scale factors of the Y/X projection as a 2-element ndarray,
     in radians per pixel. Order is [y,x].
 
     """
     calindex = None
     "DataFrame of calibration table info. Schema to be investigated."
 
-    def __init__ (self, path, mjd0=None, t0=None):
+    def __init__(self, path, mjd0=None, t0=None):
         self.mjd0 = mjd0
         self.t0 = t0
 
-        with Path (path).read_fits () as hdulist:
-            self._process_main (hdulist, hdulist[0].header)
+        with Path(path).read_fits() as hdulist:
+            self._process_main(hdulist, hdulist[0].header)
             assert self.mjdref is not None
             assert self.t0 is not None
             assert self.mjd0 is not None
 
             for hdu in hdulist[1:]:
-                self._process_hdu (hdu)
+                self._process_hdu(hdu)
 
-
-    def _process_main (self, hdulist, header):
-        self.telescope = header.get ('TELESCOP')
-        self.instrument = header.get ('INSTRUME')
-        self.obsid = header.get ('OBS_ID')
-        self.expid = header.get ('EXP_ID')
-        self.revnum = header.get ('REVOLUT')
-        self.filter = header.get ('FILTER')
-        self.targ_name = header.get ('OBJECT')
-        if 'DATE-OBS' in header:
-            self.obs_start = Time (header['DATE-OBS'], format='isot')
-        if 'DATE-END' in header:
-            self.obs_stop = Time (header['DATE-END'], format='isot')
-        if 'RA_OBJ' in header:
-            self.targ_ra = header['RA_OBJ'] * astutil.D2R
-            self.targ_dec = header['DEC_OBJ'] * astutil.D2R
-
-        if 'RADECSYS' in header:
-            if header['REFYCUNI'] != 'deg' or header['REFXCUNI'] != 'deg':
-                raise ValueError ('expect projection to be in degree units')
-
-            self.proj_csys = header['RADECSYS']
-            self.proj_equinox = header['EQUINOX']
-            self.proj_types = [header['REFYCTYP'], header['REFXCTYP']]
-            self.proj_crpix = np.asarray ([header['REFYCRPX'], header['REFXCRPX']])
-            self.proj_crval = np.asarray ([header['REFYCRVL'], header['REFXCRVL']])
+    def _process_main(self, hdulist, header):
+        self.telescope = header.get("TELESCOP")
+        self.instrument = header.get("INSTRUME")
+        self.obsid = header.get("OBS_ID")
+        self.expid = header.get("EXP_ID")
+        self.revnum = header.get("REVOLUT")
+        self.filter = header.get("FILTER")
+        self.targ_name = header.get("OBJECT")
+        if "DATE-OBS" in header:
+            self.obs_start = Time(header["DATE-OBS"], format="isot")
+        if "DATE-END" in header:
+            self.obs_stop = Time(header["DATE-END"], format="isot")
+        if "RA_OBJ" in header:
+            self.targ_ra = header["RA_OBJ"] * astutil.D2R
+            self.targ_dec = header["DEC_OBJ"] * astutil.D2R
+
+        if "RADECSYS" in header:
+            if header["REFYCUNI"] != "deg" or header["REFXCUNI"] != "deg":
+                raise ValueError("expect projection to be in degree units")
+
+            self.proj_csys = header["RADECSYS"]
+            self.proj_equinox = header["EQUINOX"]
+            self.proj_types = [header["REFYCTYP"], header["REFXCTYP"]]
+            self.proj_crpix = np.asarray([header["REFYCRPX"], header["REFXCRPX"]])
+            self.proj_crval = np.asarray([header["REFYCRVL"], header["REFXCRVL"]])
             self.proj_crval *= astutil.D2R
-            self.proj_cdelt = np.asarray ([header['REFYCDLT'], header['REFXCDLT']])
+            self.proj_cdelt = np.asarray([header["REFYCDLT"], header["REFXCDLT"]])
             self.proj_cdelt *= astutil.D2R
 
-
-    def _process_hdu (self, hdu):
-        if hdu.name == 'CALINDEX':
-            self.calindex = fits_recarray_to_data_frame (hdu.data)
+    def _process_hdu(self, hdu):
+        if hdu.name == "CALINDEX":
+            self.calindex = fits_recarray_to_data_frame(hdu.data)
         else:
-            cli.warn ('ignoring HDU named %s', hdu.name)
+            cli.warn("ignoring HDU named %s", hdu.name)
 
 
-class GTIData (BaseSASData):
+class GTIData(BaseSASData):
     gti = None
     """Dict mapping CCD number to DataFrames of GTI info. Index: integers.
     Columns:
 
         start_met  - GTI start time in MET seconds
         stop_met   - GTI stop time in MET seconds
         start_mjd  - GTI start time as MJD
         stop_mjd   - GTI stop time as MJD
         start_dks  - GTI start time as delta-kiloseconds
         stop_dks   - GTI stop time as delta-kiloseconds
         start_dmjd - GTI start time as `mjd - mjd0`
         stop_dmjd  - GTI stop time as `mjd - mjd0`
 
     """
-    def _process_main (self, hdulist, header):
-        super (GTIData, self)._process_main (hdulist, header)
-        self.gti = {}
 
+    def _process_main(self, hdulist, header):
+        super(GTIData, self)._process_main(hdulist, header)
+        self.gti = {}
 
-    def _process_hdu (self, hdu):
-        if hdu.name.startswith ('STDGTI'):
-            ccd = int (hdu.name[6:])
-            gti = self.gti[ccd] = fits_recarray_to_data_frame (hdu.data)
-            gti.rename (columns={'start': 'start_met', 'stop': 'stop_met'},
-                        inplace=True)
-            gti['start_mjd'] = gti.start_met / 86400 + self.mjdref
-            gti['start_dks'] = 1e-3 * (gti.start_met - self.t0)
-            gti['start_dmjd'] = gti.start_mjd - self.mjd0
-            gti['stop_mjd'] = gti.stop_met / 86400 + self.mjdref
-            gti['stop_dks'] = 1e-3 * (gti.stop_met - self.t0)
-            gti['stop_dmjd'] = gti.stop_mjd - self.mjd0
+    def _process_hdu(self, hdu):
+        if hdu.name.startswith("STDGTI"):
+            ccd = int(hdu.name[6:])
+            gti = self.gti[ccd] = fits_recarray_to_data_frame(hdu.data)
+            gti.rename(columns={"start": "start_met", "stop": "stop_met"}, inplace=True)
+            gti["start_mjd"] = gti.start_met / 86400 + self.mjdref
+            gti["start_dks"] = 1e-3 * (gti.start_met - self.t0)
+            gti["start_dmjd"] = gti.start_mjd - self.mjd0
+            gti["stop_mjd"] = gti.stop_met / 86400 + self.mjdref
+            gti["stop_dks"] = 1e-3 * (gti.stop_met - self.t0)
+            gti["stop_dmjd"] = gti.stop_mjd - self.mjd0
         else:
-            super (GTIData, self)._process_hdu (hdu)
-
+            super(GTIData, self)._process_hdu(hdu)
 
-    def _plot_add_gtis (self, p, ccdnum, tunit='dmjd'):
+    def _plot_add_gtis(self, p, ccdnum, tunit="dmjd"):
         import omega as om
 
         gti = self.gti[ccdnum]
         ngti = gti.shape[0]
-        gti0 = gti.at[0,'start_'+tunit]
-        gti1 = gti.at[ngti-1,'stop_'+tunit]
+        gti0 = gti.at[0, "start_" + tunit]
+        gti1 = gti.at[ngti - 1, "stop_" + tunit]
         smallofs = (gti1 - gti0) * 0.03
 
         start = gti0 - smallofs
 
-        for i in range (ngti):
-            p.add (om.rect.XBand (start, gti.at[i,'start_'+tunit], keyText=None), zheight=-1, dsn=1)
-            start = gti.at[i,'stop_'+tunit]
+        for i in range(ngti):
+            p.add(
+                om.rect.XBand(start, gti.at[i, "start_" + tunit], keyText=None),
+                zheight=-1,
+                dsn=1,
+            )
+            start = gti.at[i, "stop_" + tunit]
 
-        p.add (om.rect.XBand (start, start + smallofs, keyText=None), zheight=-1, dsn=1)
-        p.setBounds (gti0 - smallofs, gti1 + smallofs)
+        p.add(om.rect.XBand(start, start + smallofs, keyText=None), zheight=-1, dsn=1)
+        p.setBounds(gti0 - smallofs, gti1 + smallofs)
 
 
-class RegionData (BaseSASData):
+class RegionData(BaseSASData):
     regions = None
     """Dict mapping identifier to DataFrames of selection region info. Identifiers
     are like "00106" in SAS but I don't understand their significance.
     DataFrame index: integers. Columns:
         shape     - region shape as string: 'CIRCLE', ...
         x         - region center in X
         y         - region center in Y
         r         - circle radius (meaning for other shapes?)
         component - ?
 
     """
-    def _process_main (self, hdulist, header):
-        super (RegionData, self)._process_main (hdulist, header)
-        self.regions = {}
 
+    def _process_main(self, hdulist, header):
+        super(RegionData, self)._process_main(hdulist, header)
+        self.regions = {}
 
-    def _process_hdu (self, hdu):
-        if hdu.name.startswith ('REG'):
+    def _process_hdu(self, hdu):
+        if hdu.name.startswith("REG"):
             ident = hdu.name[3:]
-            self.regions[ident] = fits_recarray_to_data_frame (hdu.data)
+            self.regions[ident] = fits_recarray_to_data_frame(hdu.data)
         else:
-            super (RegionData, self)._process_hdu (hdu)
+            super(RegionData, self)._process_hdu(hdu)
 
 
-class Events (GTIData, RegionData):
+class Events(GTIData, RegionData):
     filter = None
     "Filter used as a string; e.g. 'Medium'."
 
     elapsed = None
     "Time elapsed over all events, in seconds."
 
     ccd_info = None
@@ -255,153 +254,155 @@
           mjd      - event time as MJD
           dks      - event time as delta-kiloseconds
           dmjd     - event time as `mjd - mjd0`
     """
     offsets = None
     """DataFrame of "offsets". Some kind of CCD meta-info."""
 
-    #exposure = None
+    # exposure = None
     # Commented out; exposure tables are quite large and I don't know if they're
     # useful for anything.
 
     badpix = None
     """Dict mapping CCD number to DataFrames of bad-pixel info. Index: integers.
     Columns: badflag, rawx, rawy, type, yextent.
 
     """
-    def _process_main (self, hdulist, header):
-        super (Events, self)._process_main (hdulist, header)
 
-        ccd_nums = set ()
+    def _process_main(self, hdulist, header):
+        super(Events, self)._process_main(hdulist, header)
+
+        ccd_nums = set()
         for hdu in hdulist[1:]:
-            if hdu.name.startswith ('EXPOSU'):
-                ccd_nums.add (int (hdu.name[6:]))
+            if hdu.name.startswith("EXPOSU"):
+                ccd_nums.add(int(hdu.name[6:]))
 
-        ccd_nums = sorted (ccd_nums)
+        ccd_nums = sorted(ccd_nums)
 
-        #self.exposure = {}
+        # self.exposure = {}
         self.badpix = {}
-        self.ccd_info = pd.DataFrame ({}, index=ccd_nums)
+        self.ccd_info = pd.DataFrame({}, index=ccd_nums)
 
-        hdu = hdulist['EVENTS']
-        self.events = fits_recarray_to_data_frame (hdu.data)
-        self.mjdref = hdu.header['MJDREF']
+        hdu = hdulist["EVENTS"]
+        self.events = fits_recarray_to_data_frame(hdu.data)
+        self.mjdref = hdu.header["MJDREF"]
 
         if self.t0 is None:
-            self.t0 = self.events.time.min ()
+            self.t0 = self.events.time.min()
 
         if self.mjd0 is None:
-            self.mjd0 = np.floor (self.t0 / 86400 + self.mjdref)
+            self.mjd0 = np.floor(self.t0 / 86400 + self.mjdref)
 
-        self.events['mjd'] = self.events.time / 86400 + self.mjdref
-        self.events['dks'] = 1e-3 * (self.events.time - self.t0)
-        self.events['dmjd'] = self.events.mjd - self.mjd0
-        self.timesys = hdu.header['TIMESYS']
-        self.elapsed = hdu.header['TELAPSE']
-        self.ccd_info['ontime'] = np.nan
-        self.ccd_info['livetime'] = np.nan
+        self.events["mjd"] = self.events.time / 86400 + self.mjdref
+        self.events["dks"] = 1e-3 * (self.events.time - self.t0)
+        self.events["dmjd"] = self.events.mjd - self.mjd0
+        self.timesys = hdu.header["TIMESYS"]
+        self.elapsed = hdu.header["TELAPSE"]
+        self.ccd_info["ontime"] = np.nan
+        self.ccd_info["livetime"] = np.nan
 
         for ccd in ccd_nums:
-            self.ccd_info.at[ccd,'ontime'] = hdu.header['ONTIME%02d' % ccd]
-            self.ccd_info.at[ccd,'livetime'] = hdu.header['LIVETI%02d' % ccd]
-
+            self.ccd_info.at[ccd, "ontime"] = hdu.header["ONTIME%02d" % ccd]
+            self.ccd_info.at[ccd, "livetime"] = hdu.header["LIVETI%02d" % ccd]
 
-    def _process_hdu (self, hdu):
-        if hdu.name == 'EVENTS':
+    def _process_hdu(self, hdu):
+        if hdu.name == "EVENTS":
             pass
-        elif hdu.name == 'OFFSETS':
-            self.offsets = fits_recarray_to_data_frame (hdu.data)
-        elif hdu.name.startswith ('EXPOSU'):
+        elif hdu.name == "OFFSETS":
+            self.offsets = fits_recarray_to_data_frame(hdu.data)
+        elif hdu.name.startswith("EXPOSU"):
             # These data are very large, and their purpose is unclear to me.
             pass
-            #ccd = int (hdu.name[6:])
-            #exp = self.exposure[ccd] = fits_recarray_to_data_frame (hdu.data)
-            #exp['mjd'] = exp.time / 86400 + self.mjdref
-            #exp['dks'] = 1e-3 * (exp.time - self.t0)
-        elif hdu.name.startswith ('BADPIX'):
-            ccd = int (hdu.name[6:])
-            self.badpix[ccd] = fits_recarray_to_data_frame (hdu.data)
+            # ccd = int (hdu.name[6:])
+            # exp = self.exposure[ccd] = fits_recarray_to_data_frame (hdu.data)
+            # exp['mjd'] = exp.time / 86400 + self.mjdref
+            # exp['dks'] = 1e-3 * (exp.time - self.t0)
+        elif hdu.name.startswith("BADPIX"):
+            ccd = int(hdu.name[6:])
+            self.badpix[ccd] = fits_recarray_to_data_frame(hdu.data)
         else:
-            super (Events, self)._process_hdu (hdu)
+            super(Events, self)._process_hdu(hdu)
 
-
-    def plot_pi_time (self, ccdnum):
+    def plot_pi_time(self, ccdnum):
         import omega as om
 
-        p = om.quickDF (self.events[self.events.ccdnr == ccdnum][['dmjd', 'pi']],
-                        self.targ_name,
-                        lines=False)
-        self._plot_add_gtis (p, ccdnum)
-        p.setLabels ('MJD - %.0f' % self.mjd0, 'PI')
+        p = om.quickDF(
+            self.events[self.events.ccdnr == ccdnum][["dmjd", "pi"]],
+            self.targ_name,
+            lines=False,
+        )
+        self._plot_add_gtis(p, ccdnum)
+        p.setLabels("MJD - %.0f" % self.mjd0, "PI")
         return p
 
-
-    def plot_lightcurve (self, ccd_id=None, bin_energies=False):
+    def plot_lightcurve(self, ccd_id=None, bin_energies=False):
         # XXX CIAO COPY/PASTE DOES THIS EVEN WORK???
         import omega as om
         from ...bblocks import tt_bblock
         from ..ciao.data import tight_bounds
 
         if ccd_id is None:
-            if len (self.gti) != 1:
-                raise Exception ('must specify ccd_id')
+            if len(self.gti) != 1:
+                raise Exception("must specify ccd_id")
             ccd_id = list(self.gti.keys())[0]
 
-        kev = self.events['pi'] * 1e-3 # XXXXXXX
-        vb = om.layout.VBox (2)
+        kev = self.events["pi"] * 1e-3  # XXXXXXX
+        vb = om.layout.VBox(2)
 
         if kev.size == 0:
             vb[0] = om.RectPlot()
             vb[1] = om.RectPlot()
-            tmin = self.gti[ccd_id]['start_dmjd'].min()
-            tmax = self.gti[ccd_id]['stop_dmjd'].max()
+            tmin = self.gti[ccd_id]["start_dmjd"].min()
+            tmax = self.gti[ccd_id]["stop_dmjd"].max()
             if np.isnan(tmin):
-                tmin, tmax = -1., 1.
-            emin, emax = -1., 1.
-            rmin, rmax = -1., 1.
+                tmin, tmax = -1.0, 1.0
+            emin, emax = -1.0, 1.0
+            rmin, rmax = -1.0, 1.0
         else:
-            bbinfo = tt_bblock (
-                self.gti[ccd_id]['start_dmjd'],
-                self.gti[ccd_id]['stop_dmjd'],
-                self.events['dmjd'].sort_values(),
-                intersect_with_bins = True,
+            bbinfo = tt_bblock(
+                self.gti[ccd_id]["start_dmjd"],
+                self.gti[ccd_id]["stop_dmjd"],
+                self.events["dmjd"].sort_values(),
+                intersect_with_bins=True,
             )
             cps = bbinfo.rates / 86400
 
-            tmin, tmax = tight_bounds (bbinfo.ledges[0], bbinfo.redges[-1])
-            emin, emax = tight_bounds (kev.min (), kev.max ())
-            rmin, rmax = tight_bounds (cps.min (), cps.max ())
-
-            vb[0] = om.RectPlot ()
-            csp = om.rect.ContinuousSteppedPainter (keyText='%d events' % (self.events.shape[0]))
-            csp.setFloats (np.concatenate ((bbinfo.ledges, bbinfo.redges[-1:])),
-                           np.concatenate ((cps, [0])))
-            vb[0].add (csp)
+            tmin, tmax = tight_bounds(bbinfo.ledges[0], bbinfo.redges[-1])
+            emin, emax = tight_bounds(kev.min(), kev.max())
+            rmin, rmax = tight_bounds(cps.min(), cps.max())
+
+            vb[0] = om.RectPlot()
+            csp = om.rect.ContinuousSteppedPainter(
+                keyText="%d events" % (self.events.shape[0])
+            )
+            csp.setFloats(
+                np.concatenate((bbinfo.ledges, bbinfo.redges[-1:])),
+                np.concatenate((cps, [0])),
+            )
+            vb[0].add(csp)
 
             if bin_energies:
                 vb[1] = self._plot_binned_event_energies(
-                    bbinfo,
-                    energy_scale = 1e-3,
-                    dsn = 0
+                    bbinfo, energy_scale=1e-3, dsn=0
                 )
             else:
-                vb[1] = om.quickXY (self.events['dmjd'], kev, None, lines=0)
+                vb[1] = om.quickXY(self.events["dmjd"], kev, None, lines=0)
 
-        vb[0].setBounds (tmin, tmax, rmin, rmax)
-        vb[0].setYLabel ('Count rate (ct/s)')
+        vb[0].setBounds(tmin, tmax, rmin, rmax)
+        vb[0].setYLabel("Count rate (ct/s)")
         vb[0].bpainter.paintLabels = False
-        self._plot_add_gtis (vb[0], ccd_id)
+        self._plot_add_gtis(vb[0], ccd_id)
 
-        vb[1].setBounds (tmin, tmax, emin, emax)
-        vb[1].setLabels ('MJD - %d' % self.mjd0, 'Energy (keV)')
-        self._plot_add_gtis (vb[1], ccd_id)
+        vb[1].setBounds(tmin, tmax, emin, emax)
+        vb[1].setLabels("MJD - %d" % self.mjd0, "Energy (keV)")
+        self._plot_add_gtis(vb[1], ccd_id)
         return vb
 
 
-class Lightcurve (GTIData, RegionData):
+class Lightcurve(GTIData, RegionData):
     filter = None
     "Filter used as a string; e.g. 'Medium'."
 
     binsize = None
     "The bin size used when creating the light curve, in seconds."
 
     start_met = start_mjd = start_dks = start_dmjd = None
@@ -435,69 +436,68 @@
         rate       - event rate in counts per second
         u_rate     - uncertainty on `rate`.
 
     I'm pretty sure that `u_rate` may not be just the straight Poisson noise
     since there may be GTI gaps.
 
     """
-    def _process_main (self, hdulist, header):
-        super (Lightcurve, self)._process_main (hdulist, header)
+
+    def _process_main(self, hdulist, header):
+        super(Lightcurve, self)._process_main(hdulist, header)
 
         # Early loading of bulk data
 
-        hdu = hdulist['RATE']
-        self.lc = fits_recarray_to_data_frame (hdu.data)
-        self.lc.rename (columns={'error': 'u_rate'}, inplace=True)
+        hdu = hdulist["RATE"]
+        self.lc = fits_recarray_to_data_frame(hdu.data)
+        self.lc.rename(columns={"error": "u_rate"}, inplace=True)
 
         # Straighten out timekeeping
 
-        self.mjdref = float (hdu.header['MJDREF'])
-        self.timesys = hdu.header.get ('TIMESYS')
+        self.mjdref = float(hdu.header["MJDREF"])
+        self.timesys = hdu.header.get("TIMESYS")
 
         if self.t0 is None:
-            self.t0 = self.lc.time.min ()
+            self.t0 = self.lc.time.min()
 
         if self.mjd0 is None:
-            self.mjd0 = np.floor (self.t0 / 86400 + self.mjdref)
+            self.mjd0 = np.floor(self.t0 / 86400 + self.mjdref)
 
         # Fill in the rest
 
-        self.filter = hdu.header.get ('FILTER')
-        self.binsize = hdu.header.get ('TIMEDEL')
-        self.start_met = hdu.header['TSTART']
+        self.filter = hdu.header.get("FILTER")
+        self.binsize = hdu.header.get("TIMEDEL")
+        self.start_met = hdu.header["TSTART"]
         self.start_mjd = self.start_met / 86400 + self.mjdref
         self.start_dks = 1e-3 * (self.start_met - self.t0)
         self.start_dmjd = self.start_mjd - self.mjd0
-        self.stop_met = hdu.header['TSTOP']
+        self.stop_met = hdu.header["TSTOP"]
         self.stop_mjd = self.stop_met / 86400 + self.mjdref
         self.stop_dks = 1e-3 * (self.stop_met - self.t0)
         self.stop_dmjd = self.stop_mjd - self.mjd0
-        self.energy_min = hdu.header.get ('CHANMIN')
-        self.energy_max = hdu.header.get ('CHANMAX')
-        self.energy_type = hdu.header.get ('CHANTYPE')
-        self.exposure = hdu.header.get ('EXPOSURE')
-
-        self.lc['counts'] = self.lc.rate * self.binsize
-        self.lc['mjd'] = self.lc.time / 86400 + self.mjdref
-        self.lc['dks'] = 1e-3 * (self.lc.time - self.t0)
-        self.lc['dmjd'] = self.lc.mjd - self.mjd0
-        self.lc['left_dmjd'] = self.lc.dmjd - 0.5 * self.binsize / 86400
-        self.lc['right_dmjd'] = self.lc.dmjd + 0.5 * self.binsize / 86400
+        self.energy_min = hdu.header.get("CHANMIN")
+        self.energy_max = hdu.header.get("CHANMAX")
+        self.energy_type = hdu.header.get("CHANTYPE")
+        self.exposure = hdu.header.get("EXPOSURE")
+
+        self.lc["counts"] = self.lc.rate * self.binsize
+        self.lc["mjd"] = self.lc.time / 86400 + self.mjdref
+        self.lc["dks"] = 1e-3 * (self.lc.time - self.t0)
+        self.lc["dmjd"] = self.lc.mjd - self.mjd0
+        self.lc["left_dmjd"] = self.lc.dmjd - 0.5 * self.binsize / 86400
+        self.lc["right_dmjd"] = self.lc.dmjd + 0.5 * self.binsize / 86400
 
-
-    def _process_hdu (self, hdu):
-        if hdu.name == 'RATE':
+    def _process_hdu(self, hdu):
+        if hdu.name == "RATE":
             pass
         else:
-            super (Lightcurve, self)._process_hdu (hdu)
-
+            super(Lightcurve, self)._process_hdu(hdu)
 
-    def plot_curve (self, ccdnum=None):
+    def plot_curve(self, ccdnum=None):
         import omega as om
 
-        p = om.quickDF (self.lc[['dmjd', 'rate', 'u_rate']].dropna (),
-                        self.targ_name,
-                        lines=False)
+        p = om.quickDF(
+            self.lc[["dmjd", "rate", "u_rate"]].dropna(), self.targ_name, lines=False
+        )
         if ccdnum is not None:
-            self._plot_add_gtis (p, ccdnum)
-        p.setLabels ('MJD - %.0f' % self.mjd0, 'Count rate')
+            self._plot_add_gtis(p, ccdnum)
+        p.setLabels("MJD - %.0f" % self.mjd0, "Count rate")
         return p
```

### Comparing `pwkit-1.1.1/pwkit/fk10.py` & `pwkit-1.2.0/pwkit/fk10.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/immodel.py` & `pwkit-1.2.0/pwkit/immodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,536 +8,544 @@
 wanting this code so I should put it somewhere more generic. Such as here.
 Also, given the history, there are a lot more bells and whistles in the code
 than the currently exposed UI really needs.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''FitComponent Fitter GaussianComponent beam_volume
-                  fit_one_source''').split ()
+__all__ = str(
+    """FitComponent Fitter GaussianComponent beam_volume
+                  fit_one_source"""
+).split()
 
 
-import sys, numpy as np
-from six.moves import range
+import numpy as np
 
 from . import ellipses, lmmin
 from .astutil import *
 
 
 NX = 4
-X_DX, X_DY, X_LAT, X_LON = range (NX)
+X_DX, X_DY, X_LAT, X_LON = range(NX)
 
 
-class FitComponent (object):
+class FitComponent(object):
     npar = 0
     issource = False
 
     pofs = None
     setvalue = None
     setlimit = None
 
-    def model (self, pars, x, y):
+    def model(self, pars, x, y):
         pass
 
-    def deriv (self, pars, x, jac):
+    def deriv(self, pars, x, jac):
         pass
 
-    def lat_lon_bounds (self, pars, smallval):
+    def lat_lon_bounds(self, pars, smallval):
         """return is (minlat, minlon, latwidth, lonwidth)"""
         return (None, None, None, None)
 
-    def prep_problem (self):
+    def prep_problem(self):
         pass
 
-    def postprocess (self, pars, perr, cov):
+    def postprocess(self, pars, perr, cov):
         pass
 
 
-class GaussianComponent (FitComponent):
+class GaussianComponent(FitComponent):
     npar = 6
     issource = True
 
-    def model (self, pars, x, y):
+    def model(self, pars, x, y):
         amp, slat, slon, p, q, th = pars
         lat = x[X_LAT]
         lon = x[X_LON]
 
-        sn = np.sin (th)
-        cs = np.cos (th)
+        sn = np.sin(th)
+        cs = np.cos(th)
         a = -0.5 * (cs * cs * p + sn * sn * q)
         b = sn * cs * (q - p)
         c = -0.5 * (sn * sn * p + cs * cs * q)
 
         dlat = lat - slat
-        dlon = (lon - slon) * np.cos (lat)
+        dlon = (lon - slon) * np.cos(lat)
         f = a * dlat**2 + b * dlat * dlon + c * dlon**2
-        y += amp * np.exp (f)
+        y += amp * np.exp(f)
 
-
-    def deriv (self, pars, x, jac):
+    def deriv(self, pars, x, jac):
         # Need to compute the whole source function to get the
         # amplitude derivative.
 
         amp, slat, slon, p, q, th = pars
         lat = x[X_LAT]
         lon = x[X_LON]
 
-        sn = np.sin (th)
-        cs = np.cos (th)
+        sn = np.sin(th)
+        cs = np.cos(th)
         a = -0.5 * (cs * cs * p + sn * sn * q)
         b = sn * cs * (q - p)
         c = -0.5 * (sn * sn * p + cs * cs * q)
         dlat = lat - slat
-        dlon = (lon - slon) * np.cos (lat)
+        dlon = (lon - slon) * np.cos(lat)
         f = a * dlat**2 + b * dlat * dlon + c * dlon**2
 
         # Now, back to the Jacobian ...  I got this right on the first
         # try!
 
-        jac[0] = np.exp (f)
+        jac[0] = np.exp(f)
         v = amp * jac[0]
-        jac[1] = v * (-2*a*dlat - b*dlon)
-        jac[2] = v * (-2*c*dlon - b*dlat) * np.cos (lat)
-        jac[3] = v * (-0.5 * ((cs*dlat)**2 + (sn*dlon)**2) + cs*sn*dlat*dlon)
-        jac[4] = v * (-0.5 * ((sn*dlat)**2 + (cs*dlon)**2) - cs*sn*dlat*dlon)
-        jac[5] = v * (p - q) * (cs*sn*(dlat**2-dlon**2) -
-                                dlat*dlon*(cs**2 - sn**2))
-
+        jac[1] = v * (-2 * a * dlat - b * dlon)
+        jac[2] = v * (-2 * c * dlon - b * dlat) * np.cos(lat)
+        jac[3] = v * (
+            -0.5 * ((cs * dlat) ** 2 + (sn * dlon) ** 2) + cs * sn * dlat * dlon
+        )
+        jac[4] = v * (
+            -0.5 * ((sn * dlat) ** 2 + (cs * dlon) ** 2) - cs * sn * dlat * dlon
+        )
+        jac[5] = (
+            v
+            * (p - q)
+            * (cs * sn * (dlat**2 - dlon**2) - dlat * dlon * (cs**2 - sn**2))
+        )
 
-    def lat_lon_bounds (self, pars, smallval):
+    def lat_lon_bounds(self, pars, smallval):
         amp, slat, slon, p, q, th = pars
         smaj = p**-0.5
         smin = q**-0.5
-        s = np.sin (th)
-        c = np.cos (th)
+        s = np.sin(th)
+        c = np.cos(th)
 
-        siglat = np.sqrt ((c * smaj)**2 + (s * smin)**2)
-        siglon = np.sqrt ((s * smaj)**2 + (c * smin)**2)
+        siglat = np.sqrt((c * smaj) ** 2 + (s * smin) ** 2)
+        siglon = np.sqrt((s * smaj) ** 2 + (c * smin) ** 2)
 
-        if abs (amp) <= 90 * smallval:
+        if abs(amp) <= 90 * smallval:
             # 90 is about the cutoff for a 3 sigma attenuation
             n = 3
         else:
-            n = np.sqrt (2 * np.log (abs (amp) / smallval))
+            n = np.sqrt(2 * np.log(abs(amp) / smallval))
 
         dlat = n * siglat
-        dlon = n * siglon / np.cos (slat)
+        dlon = n * siglon / np.cos(slat)
         return [slat - dlat, slon - dlon, 2 * dlat, 2 * dlon]
 
-
-    def prep_problem (self):
+    def prep_problem(self):
         # this corresponds to a FWHM of ~135 degrees ...
-        self.setlimit (3, lower=1)
-        self.setlimit (4, lower=1)
+        self.setlimit(3, lower=1)
+        self.setlimit(4, lower=1)
 
-
-    def postprocess (self, pars, perr, cov):
+    def postprocess(self, pars, perr, cov):
         self.f_pkflux = pars[0]
         self.e_pkflux = perr[0]
         self.f_dec = pars[1]
         self.e_dec = perr[1]
         self.f_ra = pars[2]
         self.e_ra = perr[2]
-        self.f_rmajor = pars[3]**-0.5 * S2F
+        self.f_rmajor = pars[3] ** -0.5 * S2F
         self.e_rmajor = 0.5 * self.f_rmajor**3 * perr[3] * S2F
-        self.f_rminor = pars[4]**-0.5 * S2F
+        self.f_rminor = pars[4] ** -0.5 * S2F
         self.e_rminor = 0.5 * self.f_rminor**3 * perr[4] * S2F
-        self.f_pa = orientcen (pars[5])
+        self.f_pa = orientcen(pars[5])
         self.e_pa = perr[5]
 
         # Uncertainty in the position as a 1-sigma ellipse
         if perr[1] == 0 and perr[2] == 0:
-            self.eell_pos = (0, 0, 0) # presume a fixed position
+            self.eell_pos = (0, 0, 0)  # presume a fixed position
         else:
-            s = ellipses.sigmascale (1)
-            pmaj, pmin, ppa = ellipses.bivell (perr[1], perr[2], cov[1,2])
+            s = ellipses.sigmascale(1)
+            pmaj, pmin, ppa = ellipses.bivell(perr[1], perr[2], cov[1, 2])
             self.eell_pos = (pmaj * s, pmin * s, ppa)
 
         if self.f_rminor > self.f_rmajor:
             self.f_rminor, self.f_rmajor = self.f_rmajor, self.f_rminor
             self.e_rminor, self.e_rmajor = self.e_rmajor, self.e_rminor
 
             if self.f_pa > 0:
                 self.f_pa -= halfpi
             else:
                 self.f_pa += halfpi
 
-
-    def postproc_total_flux (self, im):
-        self.f_totflux = self.f_pkflux * self.f_rmajor * self.f_rminor \
-            / (im.bmaj * im.bmin)
-        x = ((self.e_pkflux / self.f_pkflux)**2 +
-             (self.e_rmajor / self.f_rmajor)**2 +
-             (self.e_rminor / self.f_rminor)**2)
-        self.e_totflux = abs (self.f_totflux) * np.sqrt (x)
-
-
-    def deconvolve (self, im):
-        return gaussian_deconvolve (self.f_rmajor, self.f_rminor, self.f_pa,
-                                    im.bmaj, im.bmin, im.bpa)
-
-
-    def setup (self, flux, lat, lon, maj, min, pa, fixpos=False, fixshape=False):
-        self.setvalue (0, flux)
-        self.setvalue (1, lat, fixed=fixpos)
-        self.setvalue (2, lon, fixed=fixpos)
-        self.setvalue (3, (maj * F2S)**-2, fixed=fixshape)
-        self.setvalue (4, (min * F2S)**-2, fixed=fixshape)
-        self.setvalue (5, pa, fixed=fixshape)
+    def postproc_total_flux(self, im):
+        self.f_totflux = (
+            self.f_pkflux * self.f_rmajor * self.f_rminor / (im.bmaj * im.bmin)
+        )
+        x = (
+            (self.e_pkflux / self.f_pkflux) ** 2
+            + (self.e_rmajor / self.f_rmajor) ** 2
+            + (self.e_rminor / self.f_rminor) ** 2
+        )
+        self.e_totflux = abs(self.f_totflux) * np.sqrt(x)
+
+    def deconvolve(self, im):
+        return gaussian_deconvolve(
+            self.f_rmajor, self.f_rminor, self.f_pa, im.bmaj, im.bmin, im.bpa
+        )
+
+    def setup(self, flux, lat, lon, maj, min, pa, fixpos=False, fixshape=False):
+        self.setvalue(0, flux)
+        self.setvalue(1, lat, fixed=fixpos)
+        self.setvalue(2, lon, fixed=fixpos)
+        self.setvalue(3, (maj * F2S) ** -2, fixed=fixshape)
+        self.setvalue(4, (min * F2S) ** -2, fixed=fixshape)
+        self.setvalue(5, pa, fixed=fixshape)
+
+    def setup_point(self, flux, lat, lon, im, fixpos=False, fixshape=False):
+        self.setup(
+            flux, lat, lon, im.bmaj, im.bmin, im.bpa, fixpos=fixpos, fixshape=fixshape
+        )
 
 
-    def setup_point (self, flux, lat, lon, im, fixpos=False, fixshape=False):
-        self.setup (flux, lat, lon, im.bmaj, im.bmin, im.bpa,
-                    fixpos=fixpos, fixshape=fixshape)
-
-
-def beam_volume (im):
+def beam_volume(im):
     delta = 1e-6
     latax, lonax = im._latax, im._lonax
 
-    p = 0.5 * (np.asfarray (im.shape) - 1)
-    w1 = im.toworld (p)
+    p = 0.5 * (np.asfarray(im.shape) - 1)
+    w1 = im.toworld(p)
     p[latax] += delta
-    w2 = im.toworld (p)
+    w2 = im.toworld(p)
     latcell = (w2[latax] - w1[latax]) / delta
     p[latax] -= delta
     p[lonax] += delta
-    w2 = im.toworld (p)
-    loncell = (w2[lonax] - w1[lonax]) / delta * np.cos (w2[latax])
-    bmrad2 = 2 * np.pi * im.bmaj * im.bmin / (8 * np.log (2))
+    w2 = im.toworld(p)
+    loncell = (w2[lonax] - w1[lonax]) / delta * np.cos(w2[latax])
+    bmrad2 = 2 * np.pi * im.bmaj * im.bmin / (8 * np.log(2))
     cellrad2 = latcell * loncell
-    return np.abs (bmrad2 / cellrad2)
+    return np.abs(bmrad2 / cellrad2)
 
 
-class Fitter (object):
-    def __init__ (self):
+class Fitter(object):
+    def __init__(self):
         self.npar = 0
-        self.guess = np.zeros ((0, ))
+        self.guess = np.zeros((0,))
         self.components = []
-        self.prob = lmmin.Problem ()
-
+        self.prob = lmmin.Problem()
 
-    def add (self, component):
+    def add(self, component):
         component.pofs = self.npar
 
-        def setvalue (cidx, val, fixed=False):
+        def setvalue(cidx, val, fixed=False):
             if cidx < 0 or cidx >= component.npar:
-                raise ValueError ('cidx')
-            self.prob.p_value (cidx + component.pofs, val, fixed=fixed)
+                raise ValueError("cidx")
+            self.prob.p_value(cidx + component.pofs, val, fixed=fixed)
             self.guess[cidx + component.pofs] = val
 
-        def setlimit (cidx, lower=-np.inf, upper=np.inf):
+        def setlimit(cidx, lower=-np.inf, upper=np.inf):
             if cidx < 0 or cidx >= component.npar:
-                raise ValueError ('cidx')
-            self.prob.p_limit (cidx + component.pofs, lower, upper)
+                raise ValueError("cidx")
+            self.prob.p_limit(cidx + component.pofs, lower, upper)
 
         component.setvalue = setvalue
         component.setlimit = setlimit
 
-        newguess = np.zeros ((self.npar + component.npar, ))
-        newguess[:self.npar] = self.guess
+        newguess = np.zeros((self.npar + component.npar,))
+        newguess[: self.npar] = self.guess
         self.guess = newguess
 
-        self.components.append (component)
+        self.components.append(component)
         self.npar += component.npar
-        self.prob.set_npar (self.npar)
+        self.prob.set_npar(self.npar)
         return component
 
-
-    def setup_problem (self, im, fullimdata, noise, smallvalfactor,
-                       stamphalfsize=None):
-        if not len (self.components):
-            raise RuntimeError ('no components added to fitter')
+    def setup_problem(self, im, fullimdata, noise, smallvalfactor, stamphalfsize=None):
+        if not len(self.components):
+            raise RuntimeError("no components added to fitter")
 
         self.im = im
         self.fullimdata = fullimdata
         self.noise = noise
 
         # We're going to have to scale up our error estimates because noise is
         # heavily correlated between pixels. I don't pretend to know the
         # details but this is apparently the factor we need:
 
-        self.imerrscale = np.sqrt (beam_volume (im))
+        self.imerrscale = np.sqrt(beam_volume(im))
 
         # Determine rough lat/lon bounds of emission. We have to be careful
         # because we're on a sphere and angles may wrap.
 
-        wbounds = [None] * 4 # latmin, lonmin, latmax, lonmax
+        wbounds = [None] * 4  # latmin, lonmin, latmax, lonmax
 
         for comp in self.components:
-            p = self.guess[comp.pofs:comp.pofs+comp.npar]
-            cbounds = comp.lat_lon_bounds (p, noise * smallvalfactor)
+            p = self.guess[comp.pofs : comp.pofs + comp.npar]
+            cbounds = comp.lat_lon_bounds(p, noise * smallvalfactor)
 
-            for i in range (2):
+            for i in range(2):
                 cb = cbounds[i]
 
                 if cb is None:
                     continue
 
                 if wbounds[i] is None:
                     wbounds[i] = cb
-                    wbounds[i+2] = cb + cbounds[i+2]
+                    wbounds[i + 2] = cb + cbounds[i + 2]
                     continue
 
-                if i == 0: # latitude -- easier
-                    wbounds[i] = min (wbounds[i], cb)
-                    wbounds[i+2] = max (wbounds[i+2], cb + cbounds[i+2])
-                else: # longitude -- worry about wraps
-                    delta = angcen (cb - wbounds[i])
+                if i == 0:  # latitude -- easier
+                    wbounds[i] = min(wbounds[i], cb)
+                    wbounds[i + 2] = max(wbounds[i + 2], cb + cbounds[i + 2])
+                else:  # longitude -- worry about wraps
+                    delta = angcen(cb - wbounds[i])
                     if delta < 0:
                         wbounds[i] += delta
 
-                    delta = angcen (cb + cbounds[i+2] - wbounds[i+2])
+                    delta = angcen(cb + cbounds[i + 2] - wbounds[i + 2])
                     if delta > 0:
-                        wbounds[i+2] += delta
+                        wbounds[i + 2] += delta
 
         # could handle this in various ways instead of bailing
         if wbounds[0] is None:
-            raise RuntimeError ('no lat bounds')
+            raise RuntimeError("no lat bounds")
         if wbounds[1] is None:
-            raise RuntimeError ('no lon bounds')
+            raise RuntimeError("no lon bounds")
 
         # Now map these into a rectangle of pixels, with clipping and all of
         # that good stuff. TODO: if we don't have enough pixels to
         # successfully solve the problem, increase the bounds until we can.
 
         pbounds = [np.inf, -np.inf, np.inf, -np.inf]
 
-        def adjust (lat, lon):
-            py, px = im.topixel ([lat, lon])
-            px = int (np.floor (px))
-            py = int (np.floor (py))
-            pbounds[0] = min (pbounds[0], px)
-            pbounds[1] = max (pbounds[1], px + 1)
-            pbounds[2] = min (pbounds[2], py)
-            pbounds[3] = max (pbounds[3], py + 1)
-
-        adjust (wbounds[0], wbounds[1])
-        adjust (wbounds[0], wbounds[3])
-        adjust (wbounds[2], wbounds[1])
-        adjust (wbounds[2], wbounds[3])
+        def adjust(lat, lon):
+            py, px = im.topixel([lat, lon])
+            px = int(np.floor(px))
+            py = int(np.floor(py))
+            pbounds[0] = min(pbounds[0], px)
+            pbounds[1] = max(pbounds[1], px + 1)
+            pbounds[2] = min(pbounds[2], py)
+            pbounds[3] = max(pbounds[3], py + 1)
+
+        adjust(wbounds[0], wbounds[1])
+        adjust(wbounds[0], wbounds[3])
+        adjust(wbounds[2], wbounds[1])
+        adjust(wbounds[2], wbounds[3])
 
         if stamphalfsize is not None:
             # Hackishness for the 3-pixel parabolic fits a la
             # Bannister+ 2011.
             xmid = (pbounds[0] + pbounds[1]) // 2
             ymid = (pbounds[2] + pbounds[3]) // 2
             pbounds[:2] = xmid - stamphalfsize, xmid + stamphalfsize
             pbounds[2:] = ymid - stamphalfsize, ymid + stamphalfsize
 
-        x0 = self.x0 = max (pbounds[0], 0)
-        x1 = min (pbounds[1] + 1, im.shape[1]) # to Python range style
-        y0 = self.y0 = max (pbounds[2], 0)
-        y1 = min (pbounds[3] + 1, im.shape[0])
+        x0 = self.x0 = max(pbounds[0], 0)
+        x1 = min(pbounds[1] + 1, im.shape[1])  # to Python range style
+        y0 = self.y0 = max(pbounds[2], 0)
+        y1 = min(pbounds[3] + 1, im.shape[0])
 
         if x0 >= im.shape[1] or x1 < 0 or y0 >= im.shape[0] or y1 < 0:
-            raise RuntimeError ('trying to fit a component outside the image')
+            raise RuntimeError("trying to fit a component outside the image")
 
         patchw = x1 - x0
         patchh = y1 - y0
 
         assert patchw > 0
         assert patchh > 0
 
         # Extract the postage stamp and set up our X values.
 
-        data = self.data = self.fullimdata[y0:y1,x0:x1]
-        x = np.empty ((NX, patchh, patchw))
-        x[X_DY], x[X_DX] = np.indices (data.shape)
+        data = self.data = self.fullimdata[y0:y1, x0:x1]
+        x = np.empty((NX, patchh, patchw))
+        x[X_DY], x[X_DX] = np.indices(data.shape)
         x[X_DX] -= 0.5 * (patchw - 1)
         x[X_DY] -= 0.5 * (patchh - 1)
 
-        for i in range (patchh):
-            for j in range (patchw):
-                x[X_LAT,i,j], x[X_LON,i,j] = self.im.toworld ([i + y0, j + x0])
+        for i in range(patchh):
+            for j in range(patchw):
+                x[X_LAT, i, j], x[X_LON, i, j] = self.im.toworld([i + y0, j + x0])
 
-        x = self.x = x.reshape ((NX, patchh * patchw))
+        x = self.x = x.reshape((NX, patchh * patchw))
 
         # The functions.
 
         for c in self.components:
-            c.prep_problem ()
+            c.prep_problem()
 
-        def model (pars, outputs, sourcesonly=False):
-            outputs.fill (0)
+        def model(pars, outputs, sourcesonly=False):
+            outputs.fill(0)
 
             for c in self.components:
                 if sourcesonly and not c.issource:
                     continue
 
-                p = pars[c.pofs:c.pofs+c.npar]
-                c.model (p, x, outputs)
+                p = pars[c.pofs : c.pofs + c.npar]
+                c.model(p, x, outputs)
 
-        def deriv (pars, jac):
+        def deriv(pars, jac):
             for c in self.components:
-                p = pars[c.pofs:c.pofs+c.npar]
-                subjac = jac[c.pofs:c.pofs+c.npar]
-                c.deriv (p, x, subjac)
+                p = pars[c.pofs : c.pofs + c.npar]
+                subjac = jac[c.pofs : c.pofs + c.npar]
+                c.deriv(p, x, subjac)
 
         self.model = model
         self.deriv = deriv
-        self.prob.set_residual_func (data.flatten (),
-                                     np.ones (data.size) / self.noise,
-                                     model, deriv)
+        self.prob.set_residual_func(
+            data.flatten(), np.ones(data.size) / self.noise, model, deriv
+        )
         return self
 
-
-    def solve (self):
-        self.soln = self.prob.solve (self.guess)
+    def solve(self):
+        self.soln = self.prob.solve(self.guess)
         return self
 
-
-    def postprocess (self):
+    def postprocess(self):
         pars = self.soln.params
         perr = self.soln.perror
         cov = self.soln.covar
 
         # Apply that correction for correlated pixels. (It seems like a good
         # idea to do it as far upstream as possible, which seems to be here.)
 
         perr *= self.imerrscale
 
         # Goodness-of-fit metrics
 
         self.rchisq = self.soln.fnorm / self.soln.ndof
         n = self.data.size
         k = n - self.soln.ndof
-        self.aicc = self.soln.fnorm + 2. * k * n / (n - k - 1)
-        self.residrms = np.sqrt (self.soln.fnorm / self.data.size) * self.noise
+        self.aicc = self.soln.fnorm + 2.0 * k * n / (n - k - 1)
+        self.residrms = np.sqrt(self.soln.fnorm / self.data.size) * self.noise
 
         for c in self.components:
-            spar = pars[c.pofs:c.pofs+c.npar]
-            serr = perr[c.pofs:c.pofs+c.npar]
-            scov = cov[c.pofs:c.pofs+c.npar,c.pofs:c.pofs+c.npar]
-            c.postprocess (spar, serr, scov)
+            spar = pars[c.pofs : c.pofs + c.npar]
+            serr = perr[c.pofs : c.pofs + c.npar]
+            scov = cov[c.pofs : c.pofs + c.npar, c.pofs : c.pofs + c.npar]
+            c.postprocess(spar, serr, scov)
 
         return self
 
-
-    def subsources (self, imdata):
+    def subsources(self, imdata):
         # XXX not currently used.
-        postage = np.empty (self.data.size)
-        self.model (self.soln.params, postage, sourcesonly=True)
+        postage = np.empty(self.data.size)
+        self.model(self.soln.params, postage, sourcesonly=True)
         h, w = self.data.shape
         x0, y0 = self.x0, self.y0
-        imdata[y0:y0+h,x0:x0+w] -= postage.reshape ((h, w))
+        imdata[y0 : y0 + h, x0 : x0 + w] -= postage.reshape((h, w))
 
-
-    def display (self, run_main=True):
+    def display(self, run_main=True):
         from .ndshow_gtk3 import cycle
 
         arrays = [self.data[::-1,]]
-        descs = ['Data']
+        descs = ["Data"]
 
-        model = np.empty (self.data.size)
-        self.model (self.soln.params, model, sourcesonly=False)
-        arrays.append (model.reshape (self.data.shape)[::-1,])
-        descs.append ('Model')
+        model = np.empty(self.data.size)
+        self.model(self.soln.params, model, sourcesonly=False)
+        arrays.append(model.reshape(self.data.shape)[::-1,])
+        descs.append("Model")
 
-        arrays.append (arrays[0] - arrays[1])
-        descs.append ('Residual')
+        arrays.append(arrays[0] - arrays[1])
+        descs.append("Residual")
 
-        cycle (arrays, descs, run_main=run_main, yflip=True)
+        cycle(arrays, descs, run_main=run_main, yflip=True)
         return self
 
 
-def _guess_background_point_flux (im, imdata, xmid, ymid, patchhalfsize=16):
+def _guess_background_point_flux(im, imdata, xmid, ymid, patchhalfsize=16):
     imh, imw = imdata.shape
 
-    x0 = max (xmid - patchhalfsize, 0)
-    x1 = min (xmid + patchhalfsize + 1, imw)
-    y0 = max (ymid - patchhalfsize, 0)
-    y1 = min (ymid + patchhalfsize + 1, imh)
-
-    d = imdata[y0:y1,x0:x1]
-    dmed = np.median (d)
-    dmax = np.max (d)
+    x0 = max(xmid - patchhalfsize, 0)
+    x1 = min(xmid + patchhalfsize + 1, imw)
+    y0 = max(ymid - patchhalfsize, 0)
+    y1 = min(ymid + patchhalfsize + 1, imh)
+
+    d = imdata[y0:y1, x0:x1]
+    dmed = np.median(d)
+    dmax = np.max(d)
     return dmed, dmax - dmed
 
 
-def fit_one_source (im, xmid, ymid, forcepoint=False,
-                    patchhalfsize=16, noise=1e-3, smallvalfactor=0.5, report_func=None, display=False):
-    imdata = im.read ()
-    bgguess, ptguess = _guess_background_point_flux (im, imdata, xmid, ymid,
-                                                     patchhalfsize)
-    lat, lon = im.toworld ([ymid, xmid])
-
-    fg = Fitter ()
-    fg.add (GaussianComponent ()).setup_point (ptguess, lat, lon,
-                                               im, fixshape=False)
-    fg.setup_problem (im, imdata, noise, smallvalfactor)
-    fg.solve ().postprocess ()
-
-    dmaj, dmin, dpa, status = fg.components[-1].deconvolve (im)
-
-    fp = Fitter ()
-    fp.add (GaussianComponent ()).setup_point (ptguess, lat, lon,
-                                               im, fixshape=True)
-    fp.setup_problem (im, imdata, noise, smallvalfactor)
-    fp.solve ().postprocess ()
+def fit_one_source(
+    im,
+    xmid,
+    ymid,
+    forcepoint=False,
+    patchhalfsize=16,
+    noise=1e-3,
+    smallvalfactor=0.5,
+    report_func=None,
+    display=False,
+):
+    imdata = im.read()
+    bgguess, ptguess = _guess_background_point_flux(
+        im, imdata, xmid, ymid, patchhalfsize
+    )
+    lat, lon = im.toworld([ymid, xmid])
+
+    fg = Fitter()
+    fg.add(GaussianComponent()).setup_point(ptguess, lat, lon, im, fixshape=False)
+    fg.setup_problem(im, imdata, noise, smallvalfactor)
+    fg.solve().postprocess()
+
+    dmaj, dmin, dpa, status = fg.components[-1].deconvolve(im)
+
+    fp = Fitter()
+    fp.add(GaussianComponent()).setup_point(ptguess, lat, lon, im, fixshape=True)
+    fp.setup_problem(im, imdata, noise, smallvalfactor)
+    fp.solve().postprocess()
 
     if forcepoint:
         f = fp
-        kind = 'point'
-        reason = 'forced'
-    elif status != 'ok':
+        kind = "point"
+        reason = "forced"
+    elif status != "ok":
         f = fp
-        kind = 'point'
+        kind = "point"
         if fg.rchisq < 0.95 * fp.rchisq:
-            reason = 'couldnt_deconvolve'
+            reason = "couldnt_deconvolve"
         else:
-            reason = 'better_fit'
+            reason = "better_fit"
     elif fg.rchisq < 0.95 * fp.rchisq:
         f = fg
-        kind = 'gaussian'
-        reason = 'better_fit'
+        kind = "gaussian"
+        reason = "better_fit"
     else:
         f = fp
-        kind = 'point'
-        reason = 'better_fit'
+        kind = "point"
+        reason = "better_fit"
 
     s = f.residrms / noise
     c = f.components[-1]
-    c.postproc_total_flux (im)
-    fy, fx = im.topixel ([c.f_dec, c.f_ra])
+    c.postproc_total_flux(im)
+    fy, fx = im.topixel([c.f_dec, c.f_ra])
     if im.pclat is not None:
-        d = sphdist (c.f_dec, c.f_ra, im.pclat, im.pclon)
+        d = sphdist(c.f_dec, c.f_ra, im.pclat, im.pclon)
 
     if report_func is not None:
         report = report_func
     else:
-        def report (key, fmt, value):
-            print (key, '=', fmt % value, sep='')
 
-    report ('preferred_shape', '%s', kind)
-    report ('preferred_shape_reason', '%s', reason)
-    report ('rel_rchisq_point', '%.2f', fp.rchisq / f.rchisq)
-    report ('rel_rchisq_gauss', '%.2f', fg.rchisq / f.rchisq)
-    report ('resid_rms_mjy', '%.4f', f.residrms * 1e3)
-    report ('ndof', '%d', f.soln.ndof)
-    report ('ndata', '%d', f.data.size)
-    report ('nparam', '%d', f.data.size - f.soln.ndof)
-    report ('ra_sexg', '%s', fmthours (c.f_ra))
-    report ('dec_sexg', '%s', fmtdeglat (c.f_dec))
-    report ('x_pix', '%.1f', fx)
-    report ('y_pix', '%.1f', fy)
+        def report(key, fmt, value):
+            print(key, "=", fmt % value, sep="")
+
+    report("preferred_shape", "%s", kind)
+    report("preferred_shape_reason", "%s", reason)
+    report("rel_rchisq_point", "%.2f", fp.rchisq / f.rchisq)
+    report("rel_rchisq_gauss", "%.2f", fg.rchisq / f.rchisq)
+    report("resid_rms_mjy", "%.4f", f.residrms * 1e3)
+    report("ndof", "%d", f.soln.ndof)
+    report("ndata", "%d", f.data.size)
+    report("nparam", "%d", f.data.size - f.soln.ndof)
+    report("ra_sexg", "%s", fmthours(c.f_ra))
+    report("dec_sexg", "%s", fmtdeglat(c.f_dec))
+    report("x_pix", "%.1f", fx)
+    report("y_pix", "%.1f", fy)
 
     if im.pclat is not None:
-        report ('pnt_ctr_distance', '%.3f', d * R2A)
+        report("pnt_ctr_distance", "%.3f", d * R2A)
 
-    report ('pos_err_major_arcsec', '%.3f', s * c.eell_pos[0] * R2A)
-    report ('pos_err_minor_arcsec', '%.3f', s * c.eell_pos[1] * R2A)
-    report ('pos_err_pa_deg', '%.1f', c.eell_pos[2] * R2D)
-    report ('tot_flux_mjy', '%.4f', c.f_totflux * 1e3)
-    report ('tot_flux_err_mjy', '%.4f', s * c.e_totflux * 1e3)
-    report ('tot_flux_err_frac', '%.3f', s * c.e_totflux / c.f_totflux)
-
-    if kind == 'gaussian':
-        report ('shape_pa_err_deg', '%.1f', s * c.e_pa * R2D)
-        report ('dshape_major_arcsec', '%.3f', dmaj * R2A)
-        report ('dshape_minor_arcsec', '%.3f', dmin * R2A)
-        report ('dshape_pa_deg', '%.2f', dpa * R2D)
-        report ('dshape_area_ratio', '%.3f',
-                c.f_rmajor * c.f_rminor / (im.bmaj * im.bmin))
+    report("pos_err_major_arcsec", "%.3f", s * c.eell_pos[0] * R2A)
+    report("pos_err_minor_arcsec", "%.3f", s * c.eell_pos[1] * R2A)
+    report("pos_err_pa_deg", "%.1f", c.eell_pos[2] * R2D)
+    report("tot_flux_mjy", "%.4f", c.f_totflux * 1e3)
+    report("tot_flux_err_mjy", "%.4f", s * c.e_totflux * 1e3)
+    report("tot_flux_err_frac", "%.3f", s * c.e_totflux / c.f_totflux)
+
+    if kind == "gaussian":
+        report("shape_pa_err_deg", "%.1f", s * c.e_pa * R2D)
+        report("dshape_major_arcsec", "%.3f", dmaj * R2A)
+        report("dshape_minor_arcsec", "%.3f", dmin * R2A)
+        report("dshape_pa_deg", "%.2f", dpa * R2D)
+        report(
+            "dshape_area_ratio", "%.3f", c.f_rmajor * c.f_rminor / (im.bmaj * im.bmin)
+        )
 
     if display:
-        f.display ()
+        f.display()
```

### Comparing `pwkit-1.1.1/pwkit/inifile.py` & `pwkit-1.2.0/pwkit/inifile.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,106 +22,110 @@
 mutate_in_place
   Rewrite an ini file specififed by its path name, in place.
 
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''FileChunk InifileError mutate_in_place mutate_stream
-                  mutate read_stream read write_stream write''').split ()
+__all__ = str(
+    """FileChunk InifileError mutate_in_place mutate_stream
+                  mutate read_stream read write_stream write"""
+).split()
 
-import io, os, re, six
-from six.moves import range
+import io, os, re
 from . import Holder, PKError
 
-sectionre = re.compile (r'^\[(.*)]\s*$')
-keyre = re.compile (r'^(\S+)\s*=(.*)$') # leading space chomped later
-escre = re.compile (r'^(\S+)\s*=\s*"(.*)"\s*$')
+sectionre = re.compile(r"^\[(.*)]\s*$")
+keyre = re.compile(r"^(\S+)\s*=(.*)$")  # leading space chomped later
+escre = re.compile(r'^(\S+)\s*=\s*"(.*)"\s*$')
 
 
-class InifileError (PKError):
+class InifileError(PKError):
     pass
 
 
-def read_stream (stream):
+def read_stream(stream):
     """Python 3 compat note: we're assuming `stream` gives bytes not unicode."""
 
     section = None
     key = None
     data = None
 
     for fullline in stream:
-        line = fullline.split ('#', 1)[0]
+        line = fullline.split("#", 1)[0]
 
-        m = sectionre.match (line)
+        m = sectionre.match(line)
         if m is not None:
             # New section
             if section is not None:
                 if key is not None:
-                    section.set_one (key, data.strip ())
+                    section.set_one(key, data.strip())
                     key = data = None
                 yield section
 
-            section = Holder ()
-            section.section = m.group (1)
+            section = Holder()
+            section.section = m.group(1)
             continue
 
-        if len (line.strip ()) == 0:
+        if len(line.strip()) == 0:
             if key is not None:
-                section.set_one (key, data.strip ())
+                section.set_one(key, data.strip())
                 key = data = None
             continue
 
-        m = escre.match (fullline)
+        m = escre.match(fullline)
         if m is not None:
             if section is None:
-                raise InifileError ('key seen without section!')
+                raise InifileError("key seen without section!")
             if key is not None:
-                section.set_one (key, data.strip ())
-            key = m.group (1)
-            data = m.group (2).replace (r'\"', '"').replace (r'\n', '\n').replace (r'\\', '\\')
-            section.set_one (key, data)
+                section.set_one(key, data.strip())
+            key = m.group(1)
+            data = (
+                m.group(2).replace(r"\"", '"').replace(r"\n", "\n").replace(r"\\", "\\")
+            )
+            section.set_one(key, data)
             key = data = None
             continue
 
-        m = keyre.match (line)
+        m = keyre.match(line)
         if m is not None:
             if section is None:
-                raise InifileError ('key seen without section!')
+                raise InifileError("key seen without section!")
             if key is not None:
-                section.set_one (key, data.strip ())
-            key = m.group (1)
-            data = m.group (2)
-            if not len (data):
-                data = ' '
-            elif not data[-1].isspace ():
-                data += ' '
+                section.set_one(key, data.strip())
+            key = m.group(1)
+            data = m.group(2)
+            if not len(data):
+                data = " "
+            elif not data[-1].isspace():
+                data += " "
             continue
 
-        if line[0].isspace () and key is not None:
-            data += line.strip () + ' '
+        if line[0].isspace() and key is not None:
+            data += line.strip() + " "
             continue
 
-        raise InifileError ('unparsable line: ' + line[:-1])
+        raise InifileError("unparsable line: " + line[:-1])
 
     if section is not None:
         if key is not None:
-            section.set_one (key, data.strip ())
+            section.set_one(key, data.strip())
         yield section
 
 
-def read (stream_or_path):
-    if isinstance (stream_or_path, six.string_types):
-        return read_stream (io.open (stream_or_path, 'rt'))
-    return read_stream (stream_or_path)
+def read(stream_or_path):
+    if isinstance(stream_or_path, str):
+        return read_stream(io.open(stream_or_path, "rt"))
+    return read_stream(stream_or_path)
 
 
 # Writing
 
-def write_stream (stream, holders, defaultsection=None):
+
+def write_stream(stream, holders, defaultsection=None):
     """Very simple writing in ini format. The simple stringification of each value
     in each Holder is printed, and no escaping is performed. (This is most
     relevant for multiline values or ones containing pound signs.) `None` values are
     skipped.
 
     Arguments:
 
@@ -135,32 +139,32 @@
       `section` field.
 
     """
     anybefore = False
 
     for h in holders:
         if anybefore:
-            print ('', file=stream)
+            print("", file=stream)
 
-        s = h.get ('section', defaultsection)
+        s = h.get("section", defaultsection)
         if s is None:
-            raise ValueError ('cannot determine section name for item <%s>' % h)
-        print ('[%s]' % s, file=stream)
+            raise ValueError("cannot determine section name for item <%s>" % h)
+        print("[%s]" % s, file=stream)
 
-        for k in sorted (x for x in six.iterkeys (h.__dict__) if x != 'section'):
-            v = h.get (k)
+        for k in sorted(x for x in h.__dict__.keys() if x != "section"):
+            v = h.get(k)
             if v is None:
                 continue
 
-            print ('%s = %s' % (k, v), file=stream)
+            print("%s = %s" % (k, v), file=stream)
 
         anybefore = True
 
 
-def write (stream_or_path, holders, **kwargs):
+def write(stream_or_path, holders, **kwargs):
     """Very simple writing in ini format. The simple stringification of each value
     in each Holder is printed, and no escaping is performed. (This is most
     relevant for multiline values or ones containing pound signs.) `None` values are
     skipped.
 
     Arguments:
 
@@ -170,168 +174,168 @@
       An iterable of objects to write. Their fields will be
       written as sections.
     defaultsection=None
       Section name to use if a holder doesn't contain a
       `section` field.
 
     """
-    if isinstance (stream_or_path, six.string_types):
-        return write_stream (io.open (stream_or_path, 'wt'), holders, **kwargs)
+    if isinstance(stream_or_path, str):
+        return write_stream(io.open(stream_or_path, "wt"), holders, **kwargs)
     else:
-        return write_stream (stream_or_path, holders, **kwargs)
+        return write_stream(stream_or_path, holders, **kwargs)
 
 
 # Parsing plus inline modification, preserving the file as much as possible.
 #
 # I'm pretty sure that this code gets the corner cases right, but it hasn't
 # been thoroughly tested, and it's a little hairy ...
 
-class FileChunk (object):
-    def __init__ (self):
-        self.data = Holder ()
-        self._lines = []
-
 
-    def _addLine (self, line, assoc):
-        self._lines.append ((assoc, line))
+class FileChunk(object):
+    def __init__(self):
+        self.data = Holder()
+        self._lines = []
 
+    def _addLine(self, line, assoc):
+        self._lines.append((assoc, line))
 
-    def set (self, name, value):
-        newline = ((u'%s = %s' % (name, value)) + os.linesep).encode ('utf8')
+    def set(self, name, value):
+        newline = (("%s = %s" % (name, value)) + os.linesep).encode("utf8")
         first = True
 
-        for i in range (len (self._lines)):
+        for i in range(len(self._lines)):
             assoc, line = self._lines[i]
 
             if assoc != name:
                 continue
 
             if first:
                 self._lines[i] = (assoc, newline)
                 first = False
             else:
                 # delete the line
                 self._lines[i] = (None, None)
 
         if first:
             # Need to append the line to the last block
-            for i in range (len (self._lines) - 1, -1, -1):
+            for i in range(len(self._lines) - 1, -1, -1):
                 if self._lines[i][0] is not None:
                     break
 
-            self._lines.insert (i + 1, (name, newline))
-
+            self._lines.insert(i + 1, (name, newline))
 
-    def emit (self, stream):
+    def emit(self, stream):
         for assoc, line in self._lines:
             if line is None:
                 continue
-            stream.write (line)
+            stream.write(line)
 
 
-def mutate_stream (instream, outstream):
+def mutate_stream(instream, outstream):
     """Python 3 compat note: we're assuming `stream` gives bytes not unicode."""
 
     chunk = None
     key = None
     data = None
     misclines = []
 
     for fullline in instream:
-        line = fullline.split ('#', 1)[0]
+        line = fullline.split("#", 1)[0]
 
-        m = sectionre.match (line)
+        m = sectionre.match(line)
         if m is not None:
             # New chunk
             if chunk is not None:
                 if key is not None:
-                    chunk.data.set_one (key, data.strip ())
+                    chunk.data.set_one(key, data.strip())
                     key = data = None
                 yield chunk
-                chunk.emit (outstream)
+                chunk.emit(outstream)
 
-            chunk = FileChunk ()
+            chunk = FileChunk()
             for miscline in misclines:
-                chunk._addLine (miscline, None)
+                chunk._addLine(miscline, None)
             misclines = []
-            chunk.data.section = m.group (1)
-            chunk._addLine (fullline, None)
+            chunk.data.section = m.group(1)
+            chunk._addLine(fullline, None)
             continue
 
-        if len (line.strip ()) == 0:
+        if len(line.strip()) == 0:
             if key is not None:
-                chunk.data.set_one (key, data.strip ())
+                chunk.data.set_one(key, data.strip())
                 key = data = None
             if chunk is not None:
-                chunk._addLine (fullline, None)
+                chunk._addLine(fullline, None)
             else:
-                misclines.append (fullline)
+                misclines.append(fullline)
             continue
 
-        m = escre.match (fullline)
+        m = escre.match(fullline)
         if m is not None:
             if chunk is None:
-                raise InifileError ('key seen without section!')
+                raise InifileError("key seen without section!")
             if key is not None:
-                chunk.data.set_one (key, data.strip ())
-            key = m.group (1)
-            data = m.group (2).replace (r'\"', '"').replace (r'\n', '\n').replace (r'\\', '\\')
-            chunk.data.set_one (key, data)
-            chunk._addLine (fullline, key)
+                chunk.data.set_one(key, data.strip())
+            key = m.group(1)
+            data = (
+                m.group(2).replace(r"\"", '"').replace(r"\n", "\n").replace(r"\\", "\\")
+            )
+            chunk.data.set_one(key, data)
+            chunk._addLine(fullline, key)
             key = data = None
             continue
 
-        m = keyre.match (line)
+        m = keyre.match(line)
         if m is not None:
             if chunk is None:
-                raise InifileError ('key seen without section!')
+                raise InifileError("key seen without section!")
             if key is not None:
-                chunk.data.set_one (key, data.strip ())
-            key = m.group (1)
-            data = m.group (2)
-            if not data[-1].isspace ():
-                data += ' '
-            chunk._addLine (fullline, key)
+                chunk.data.set_one(key, data.strip())
+            key = m.group(1)
+            data = m.group(2)
+            if not data[-1].isspace():
+                data += " "
+            chunk._addLine(fullline, key)
             continue
 
-        if line[0].isspace () and key is not None:
-            data += line.strip () + ' '
-            chunk._addLine (fullline, key)
+        if line[0].isspace() and key is not None:
+            data += line.strip() + " "
+            chunk._addLine(fullline, key)
             continue
 
-        raise InifileError ('unparsable line: ' + line[:-1])
+        raise InifileError("unparsable line: " + line[:-1])
 
     if chunk is not None:
         if key is not None:
-            chunk.data.set_one (key, data.strip ())
+            chunk.data.set_one(key, data.strip())
         yield chunk
-        chunk.emit (outstream)
+        chunk.emit(outstream)
 
 
-def mutate (instream_or_path, outstream_or_path, outmode='wb'):
-    if isinstance (instream_or_path, six.string_types):
-        instream_or_path = io.open (instream_or_path, 'rb')
+def mutate(instream_or_path, outstream_or_path, outmode="wb"):
+    if isinstance(instream_or_path, str):
+        instream_or_path = io.open(instream_or_path, "rb")
 
-    if isinstance (outstream_or_path, six.string_types):
-        outstream_or_path = io.open (outstream_or_path, outmode)
+    if isinstance(outstream_or_path, str):
+        outstream_or_path = io.open(outstream_or_path, outmode)
 
-    return mutate_stream (instream_or_path, outstream_or_path)
+    return mutate_stream(instream_or_path, outstream_or_path)
 
 
-def mutate_in_place (inpath):
+def mutate_in_place(inpath):
     from sys import exc_info
     from os import rename, unlink
 
-    tmppath = inpath + '.new'
+    tmppath = inpath + ".new"
 
-    with io.open (inpath, 'rb') as instream:
+    with io.open(inpath, "rb") as instream:
         try:
-            with io.open (tmppath, 'wb') as outstream:
-                for item in mutate_stream (instream, outstream):
+            with io.open(tmppath, "wb") as outstream:
+                for item in mutate_stream(instream, outstream):
                     yield item
-                rename (tmppath, inpath)
+                rename(tmppath, inpath)
         except:
             try:
-                os.unlink (tmppath)
+                os.unlink(tmppath)
             except Exception:
                 pass
             raise
```

### Comparing `pwkit-1.1.1/pwkit/io.py` & `pwkit-1.2.0/pwkit/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 files. The most generic such tools are located in this module. The most
 important tool is the :class:`Path` class for object-oriented navigation of
 the filesystem.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''djoin ensure_dir ensure_symlink make_path_func rellink
-                  pathlines pathwords try_open words Path''').split ()
+__all__ = str(
+    """djoin ensure_dir ensure_symlink make_path_func rellink
+                  pathlines pathwords try_open words Path"""
+).split()
 
 import io, os, pathlib
-import six
 
-from . import PKError, text_type
-
-if six.PY2:
-    path_type = six.binary_type
-else:
-    path_type = six.text_type
+from . import PKError
 
 
 # Python 2/3 bytes/unicode compat helpers
 
+path_type = str
+
+
 def _get_bytes_stream(base):
-    if hasattr(base, 'buffer'): # Python 3
+    if hasattr(base, "buffer"):  # Python 3
         return base.buffer
-    if hasattr(base, 'stream'): # after pwkit.cli.unicode_stdio() is invoked.
+    if hasattr(base, "stream"):  # after pwkit.cli.unicode_stdio() is invoked.
         return base.stream
-    return base # Hopefully ...
+    return base  # Hopefully ...
+
 
 def get_stdout_bytes():
     """Get a reference to the standard output stream that accepts bytes, not
     unicode characters.
 
     Returns: a file-like object hooked up to the process’ standard output.
 
@@ -48,16 +48,18 @@
     Python 2 or Python 3, or whether :func:`pwkit.cli.unicode_stdio` has been
     called, the right way to get access to the underlying byte-based stream is
     different. This function encapsulates these checks and works across all of
     these cases.
 
     """
     import sys
+
     return _get_bytes_stream(sys.stdout)
 
+
 def get_stderr_bytes():
     """Get a reference to the standard error stream that accepts bytes, not
     unicode characters.
 
     Returns: a file-like object hooked up to the process’ standard error.
 
     Usually, you want to write text to a process's standard error stream
@@ -69,206 +71,216 @@
     Python 2 or Python 3, or whether :func:`pwkit.cli.unicode_stdio` has been
     called, the right way to get access to the underlying byte-based stream is
     different. This function encapsulates these checks and works across all of
     these cases.
 
     """
     import sys
+
     return _get_bytes_stream(sys.stderr)
 
 
 # Reading text.
 
-def try_open (*args, **kwargs):
+
+def try_open(*args, **kwargs):
     """Simply a wrapper for io.open(), unless an IOError with errno=2 (ENOENT) is
     raised, in which case None is retured.
 
     """
     try:
-        return io.open (*args, **kwargs)
+        return io.open(*args, **kwargs)
     except IOError as e:
         if e.errno == 2:
             return None
         raise
 
 
-def words (linegen):
+def words(linegen):
     for line in linegen:
-        a = line.split ('#', 1)[0].strip ().split ()
-        if len (a):
+        a = line.split("#", 1)[0].strip().split()
+        if len(a):
             yield a
 
 
-def pathwords (path, mode='rt', noexistok=False, **kwargs):
+def pathwords(path, mode="rt", noexistok=False, **kwargs):
     try:
-        with io.open (path, mode, **kwargs) as f:
+        with io.open(path, mode, **kwargs) as f:
             for line in f:
-                a = line.split ('#', 1)[0].strip ().split ()
-                if len (a):
+                a = line.split("#", 1)[0].strip().split()
+                if len(a):
                     yield a
     except IOError as e:
         if e.errno != 2 or not noexistok:
             raise
 
 
-def pathlines (path, mode='rt', noexistok=False, **kwargs):
+def pathlines(path, mode="rt", noexistok=False, **kwargs):
     try:
-        with io.open (path, mode, **kwargs) as f:
+        with io.open(path, mode, **kwargs) as f:
             for line in f:
                 yield line
     except IOError as e:
         if e.errno != 2 or not noexistok:
             raise
 
 
 # Path manipulations -- should largely be superseded by the Path object
 
-def make_path_func (*baseparts):
+
+def make_path_func(*baseparts):
     """Return a function that joins paths onto some base directory."""
     from os.path import join
-    base = join (*baseparts)
-    def path_func (*args):
-        return join (base, *args)
+
+    base = join(*baseparts)
+
+    def path_func(*args):
+        return join(base, *args)
+
     return path_func
 
 
-def djoin (*args):
+def djoin(*args):
     """'dotless' join, for nicer paths."""
     from os.path import join
 
     i = 0
-    alen = len (args)
+    alen = len(args)
 
-    while i < alen and (args[i] == '' or args[i] == '.'):
+    while i < alen and (args[i] == "" or args[i] == "."):
         i += 1
 
     if i == alen:
-        return '.'
+        return "."
 
-    return join (*args[i:])
+    return join(*args[i:])
 
 
 # Doing stuff on the filesystem.
 
-def rellink (source, dest):
+
+def rellink(source, dest):
     """Create a symbolic link to path *source* from path *dest*. If either
     *source* or *dest* is an absolute path, the link from *dest* will point to
     the absolute path of *source*. Otherwise, the link to *source* from *dest*
     will be a relative link.
 
     """
     from os.path import isabs, dirname, relpath, abspath
 
-    if isabs (source):
-        os.symlink (source, dest)
-    elif isabs (dest):
-        os.symlink (abspath (source), dest)
+    if isabs(source):
+        os.symlink(source, dest)
+    elif isabs(dest):
+        os.symlink(abspath(source), dest)
     else:
-        os.symlink (relpath (source, dirname (dest)), dest)
+        os.symlink(relpath(source, dirname(dest)), dest)
 
 
-def ensure_dir (path, parents=False):
+def ensure_dir(path, parents=False):
     """Returns a boolean indicating whether the directory already existed. Will
     attempt to create parent directories if *parents* is True.
 
     """
     if parents:
         from os.path import dirname
-        parent = dirname (path)
-        if len (parent) and parent != path:
-            ensure_dir (parent, True)
+
+        parent = dirname(path)
+        if len(parent) and parent != path:
+            ensure_dir(parent, True)
 
     try:
-        os.mkdir (path)
+        os.mkdir(path)
     except OSError as e:
-        if e.errno == 17: # EEXIST
+        if e.errno == 17:  # EEXIST
             return True
         raise
     return False
 
 
-def ensure_symlink (src, dst):
+def ensure_symlink(src, dst):
     """Ensure the existence of a symbolic link pointing to src named dst. Returns
     a boolean indicating whether the symlink already existed.
 
     """
     try:
-        os.symlink (src, dst)
+        os.symlink(src, dst)
     except OSError as e:
-        if e.errno == 17: # EEXIST
+        if e.errno == 17:  # EEXIST
             return True
         raise
     return False
 
 
 # Extended Path object. pathlib.Path objects have fancy __new__ semantics that
 # we need to jump through some hoops for.
 
-_ParentPath = pathlib.WindowsPath if os.name == 'nt' else pathlib.PosixPath
+_ParentPath = pathlib.WindowsPath if os.name == "nt" else pathlib.PosixPath
+
 
-class Path (_ParentPath):
+class Path(_ParentPath):
     """This is an extended version of the :class:`pathlib.Path` class.
     (:mod:`pathlib` is built into Python 3.x and is available as a backport to
     Python 2.x.) It represents a path on the filesystem.
 
     """
+
     # Manipulations
 
-    def expand (self, user=False, vars=False, glob=False, resolve=False):
+    def expand(self, user=False, vars=False, glob=False, resolve=False):
         """Return a new :class:`Path` with various expansions performed. All
-	expansions are disabled by default but can be enabled by passing in
-	true values in the keyword arguments.
+        expansions are disabled by default but can be enabled by passing in
+        true values in the keyword arguments.
 
-	user : bool (default False)
-	  Expand ``~`` and ``~user`` home-directory constructs. If a username is
-	  unmatched or ``$HOME`` is unset, no change is made. Calls
-	  :func:`os.path.expanduser`.
-	vars : bool (default False)
-	  Expand ``$var`` and ``${var}`` environment variable constructs. Unknown
-	  variables are not substituted. Calls :func:`os.path.expandvars`.
-	glob : bool (default False)
-	  Evaluate the path as a :mod:`glob` expression and use the matched path.
-	  If the glob does not match anything, do not change anything. If the
-	  glob matches more than one path, raise an :exc:`IOError`.
-	resolve : bool (default False)
-	  Call :meth:`resolve` on the return value before returning it.
+        user : bool (default False)
+          Expand ``~`` and ``~user`` home-directory constructs. If a username is
+          unmatched or ``$HOME`` is unset, no change is made. Calls
+          :func:`os.path.expanduser`.
+        vars : bool (default False)
+          Expand ``$var`` and ``${var}`` environment variable constructs. Unknown
+          variables are not substituted. Calls :func:`os.path.expandvars`.
+        glob : bool (default False)
+          Evaluate the path as a :mod:`glob` expression and use the matched path.
+          If the glob does not match anything, do not change anything. If the
+          glob matches more than one path, raise an :exc:`IOError`.
+        resolve : bool (default False)
+          Call :meth:`resolve` on the return value before returning it.
 
         """
         from os import path
         from glob import glob
 
-        text = text_type (self)
+        text = str(self)
         if user:
-            text = path.expanduser (text)
+            text = path.expanduser(text)
         if vars:
-            text = path.expandvars (text)
+            text = path.expandvars(text)
         if glob:
-            results = glob (text)
-            if len (results) == 1:
+            results = glob(text)
+            if len(results) == 1:
                 text = results[0]
-            elif len (results) > 1:
-                raise IOError ('glob of %r should\'ve returned 0 or 1 matches; got %d'
-                               % (text, len (results)))
+            elif len(results) > 1:
+                raise IOError(
+                    "glob of %r should've returned 0 or 1 matches; got %d"
+                    % (text, len(results))
+                )
 
-        other = self.__class__ (text)
+        other = self.__class__(text)
         if resolve:
-            other = other.resolve ()
+            other = other.resolve()
 
         return other
 
-
-    def format (self, *args, **kwargs):
+    def format(self, *args, **kwargs):
         """Return a new path formed by calling :meth:`str.format` on the
         textualization of this path.
 
         """
-        return self.__class__ (str (self).format (*args, **kwargs))
+        return self.__class__(str(self).format(*args, **kwargs))
 
-
-    def get_parent (self, mode='naive'):
+    def get_parent(self, mode="naive"):
         """Get the path of this path’s parent directory.
 
         Unlike the :attr:`parent` attribute, this function can correctly
         ascend into parent directories if *self* is ``"."`` or a sequence of
         ``".."``. The precise way in which it handles these kinds of paths,
         however, depends on the *mode* parameter:
 
@@ -283,62 +295,60 @@
           a sequence of ``".."`` is the same sequence with another ``".."``. Note
           that this manipulation is still strictly textual, so results when called
           on paths like ``"foo/../bar/../other"`` will likely not be what you want.
           Furthermore, ``p.get_parent(mode="naive")`` never yields a path equal to
           ``p``, so some kinds of loops will execute infinitely.
 
         """
-        if mode == 'textual':
+        if mode == "textual":
             return self.parent
 
-        if mode == 'resolved':
-            return self.resolve ().parent
+        if mode == "resolved":
+            return self.resolve().parent
 
-        if mode == 'naive':
+        if mode == "naive":
             from os.path import pardir
 
-            if not len (self.parts):
-                return self.__class__ (pardir)
-            if all (p == pardir for p in self.parts):
+            if not len(self.parts):
+                return self.__class__(pardir)
+            if all(p == pardir for p in self.parts):
                 return self / pardir
             return self.parent
 
-        raise ValueError ('unhandled get_parent() mode %r' % (mode, ))
-
+        raise ValueError("unhandled get_parent() mode %r" % (mode,))
 
-    def make_relative (self, other):
+    def make_relative(self, other):
         """Return a new path that is the equivalent of this one relative to the path
         *other*. Unlike :meth:`relative_to`, this will not throw an error if *self* is
         not a sub-path of *other*; instead, it will use ``..`` to build a relative
         path. This can result in invalid relative paths if *other* contains a
         directory symbolic link.
 
         If *self* is an absolute path, it is returned unmodified.
 
         """
-        if self.is_absolute ():
+        if self.is_absolute():
             return self
 
         from os.path import relpath
-        other = self.__class__ (other)
-        return self.__class__ (relpath (text_type (self), text_type (other)))
 
+        other = self.__class__(other)
+        return self.__class__(relpath(str(self), str(other)))
 
     # Filesystem interrogation
 
-    def readlink (self):
+    def readlink(self):
         """Assuming that this path is a symbolic link, read its contents and
         return them as another :class:`Path` object. An "invalid argument"
         OSError will be raised if this path does not point to a symbolic link.
 
         """
-        return self.__class__ (os.readlink (path_type (self)))
-
+        return self.__class__(os.readlink(path_type(self)))
 
-    def scandir (self):
+    def scandir(self):
         """Iteratively scan this path, assuming it’s a directory. This requires and
         uses the :mod:`scandir` module.
 
         `scandir` is different than `iterdir` because it generates `DirEntry`
         items rather than Path instances. DirEntry objects have their
         properties filled from the directory info itself, so querying them
         avoids syscalls that would be necessary with iterdir().
@@ -346,25 +356,24 @@
         The generated values are :class:`scandir.DirEntry` objects which have
         some information pre-filled. These objects have methods ``inode()``,
         ``is_dir()``, ``is_file()``, ``is_symlink()``, and ``stat()``. They
         have attributes ``name`` (the basename of the entry) and ``path`` (its
         full path).
 
         """
-        if hasattr (os, 'scandir'):
+        if hasattr(os, "scandir"):
             scandir = os.scandir
         else:
             from scandir import scandir
 
-        return scandir (path_type (self))
-
+        return scandir(path_type(self))
 
     # Filesystem modification
 
-    def copy_to (self, dest, preserve='mode'):
+    def copy_to(self, dest, preserve="mode"):
         """Copy this path — as a file — to another *dest*.
 
         The *preserve* argument specifies which meta-properties of the file
         should be preserved:
 
         ``none``
           Only copy the file data.
@@ -378,32 +387,32 @@
         Returns the final destination path.
 
         """
         # shutil.copyfile() doesn't let the destination be a directory, so we
         # have to manage that possibility ourselves.
 
         import shutil
-        dest = Path (dest)
 
-        if dest.is_dir ():
+        dest = Path(dest)
+
+        if dest.is_dir():
             dest = dest / self.name
 
-        if preserve == 'none':
-            shutil.copyfile (str(self), str(dest))
-        elif preserve == 'mode':
-            shutil.copy (str(self), str(dest))
-        elif preserve == 'all':
-            shutil.copy2 (str(self), str(dest))
+        if preserve == "none":
+            shutil.copyfile(str(self), str(dest))
+        elif preserve == "mode":
+            shutil.copy(str(self), str(dest))
+        elif preserve == "all":
+            shutil.copy2(str(self), str(dest))
         else:
-            raise ValueError ('unrecognized "preserve" value %r' % (preserve,))
+            raise ValueError('unrecognized "preserve" value %r' % (preserve,))
 
         return dest
 
-
-    def ensure_dir (self, mode=0o777, parents=False):
+    def ensure_dir(self, mode=0o777, parents=False):
         """Ensure that this path exists as a directory.
 
         This function calls :meth:`mkdir` on this path, but does not raise an
         exception if it already exists. It does raise an exception if this
         path exists but is not a directory. If the directory is created,
         *mode* is used to set the permissions of the resulting directory, with
         the important caveat that the current :func:`os.umask` is applied.
@@ -413,111 +422,107 @@
         If *parents* is true, parent directories will be created in the same
         manner.
 
         """
         if parents:
             p = self.parent
             if p == self:
-                return False # can never create root; avoids loop when parents=True
-            p.ensure_dir (mode, True)
+                return False  # can never create root; avoids loop when parents=True
+            p.ensure_dir(mode, True)
 
         made_it = False
 
         try:
-            self.mkdir (mode)
+            self.mkdir(mode)
             made_it = True
         except OSError as e:
-            if e.errno == 17: # EEXIST?
-                return False # that's fine
-            raise # other exceptions are not fine
+            if e.errno == 17:  # EEXIST?
+                return False  # that's fine
+            raise  # other exceptions are not fine
 
-        if not self.is_dir ():
+        if not self.is_dir():
             import errno
-            raise OSError (errno.ENOTDIR, 'Not a directory', str(self))
 
-        return made_it
+            raise OSError(errno.ENOTDIR, "Not a directory", str(self))
 
+        return made_it
 
-    def ensure_parent (self, mode=0o777, parents=False):
+    def ensure_parent(self, mode=0o777, parents=False):
         """Ensure that this path's *parent* directory exists.
 
         Returns a boolean whether the parent directory was created. Will
         attempt to create superior parent directories if *parents* is true.
 
         """
-        return self.parent.ensure_dir (mode, parents)
-
+        return self.parent.ensure_dir(mode, parents)
 
-    class _PathTempfileContextManager (object):
-        def __init__ (self, reference, want, resolution, suffix, kwargs):
+    class _PathTempfileContextManager(object):
+        def __init__(self, reference, want, resolution, suffix, kwargs):
             self.reference = reference
             self.want = want
             self.resolution = resolution
             self.suffix = suffix
             self.kwargs = kwargs
 
-        def __enter__ (self):
+        def __enter__(self):
             from tempfile import NamedTemporaryFile
 
             # Pretty hacky: we know that we've been called from
             # create_tempfile() when `reference` is a class.
 
-            if isinstance (self.reference, type):
+            if isinstance(self.reference, type):
                 dir = None
-                prefix = 'tmp'
+                prefix = "tmp"
                 refcls = self.reference
             else:
                 dir = str(self.reference.parent)
-                prefix = (self.reference.name + '.')
+                prefix = self.reference.name + "."
                 refcls = self.reference.__class__
 
-            self.handle = NamedTemporaryFile (
-                dir = dir,
-                prefix = prefix,
-                suffix = self.suffix,
-                delete = False,
-                **self.kwargs
+            self.handle = NamedTemporaryFile(
+                dir=dir, prefix=prefix, suffix=self.suffix, delete=False, **self.kwargs
             )
 
-            self.temppath = refcls (self.handle.name)
+            self.temppath = refcls(self.handle.name)
             self.handle.path = self.temppath
 
-            if self.want == 'handle':
+            if self.want == "handle":
                 return self.handle
 
-            if self.want == 'path':
-                self.handle.close ()
+            if self.want == "path":
+                self.handle.close()
                 self.handle = None
                 return self.temppath
 
-            assert False, 'not reached'
+            assert False, "not reached"
 
-        def __exit__ (self, etype, evalue, etb):
+        def __exit__(self, etype, evalue, etb):
             if self.handle is not None:
-                self.handle.close ()
+                self.handle.close()
 
             if etype is not None:
                 # On error, keep the tempfile
                 return False
 
-            if self.resolution == 'unlink':
-                self.temppath.unlink ()
-            elif self.resolution == 'try_unlink':
-                self.temppath.try_unlink ()
-            elif self.resolution == 'keep':
+            if self.resolution == "unlink":
+                self.temppath.unlink()
+            elif self.resolution == "try_unlink":
+                self.temppath.try_unlink()
+            elif self.resolution == "keep":
                 pass
-            elif self.resolution == 'overwrite':
-                self.temppath.rename (self.reference)
+            elif self.resolution == "overwrite":
+                self.temppath.rename(self.reference)
             else:
-                assert False, 'not reached'
+                assert False, "not reached"
 
             return False
 
-
-    def make_tempfile (self, want='handle', resolution='try_unlink', suffix='', **kwargs):
+    def make_tempfile(
+        self, want="handle", resolution="try_unlink", suffix="", **kwargs
+    ):
         """Get a context manager that creates and cleans up a uniquely-named temporary
         file with a name similar to this path.
 
         This function returns a context manager that creates a secure
         temporary file with a path similar to *self*. In particular, if
         ``str(self)`` is something like ``foo/bar``, the path of the temporary
         file will be something like ``foo/bar.ame8_2``.
@@ -563,136 +568,143 @@
         The *suffix* argument is appended to the temporary file name after the
         random portion. It defaults to the empty string. If you want it to
         operate as a typical filename suffix, include a leading ``"."``.
 
         Other **kwargs** are passed to :class:`tempfile.NamedTemporaryFile`.
 
         """
-        if want not in ('handle', 'path'):
-            raise ValueError ('unrecognized make_tempfile() "want" mode %r' % (want,))
-        if resolution not in ('unlink', 'try_unlink', 'keep', 'overwrite'):
-            raise ValueError ('unrecognized make_tempfile() "resolution" mode %r' % (resolution,))
-        return Path._PathTempfileContextManager (self, want, resolution, suffix, kwargs)
-
+        if want not in ("handle", "path"):
+            raise ValueError('unrecognized make_tempfile() "want" mode %r' % (want,))
+        if resolution not in ("unlink", "try_unlink", "keep", "overwrite"):
+            raise ValueError(
+                'unrecognized make_tempfile() "resolution" mode %r' % (resolution,)
+            )
+        return Path._PathTempfileContextManager(self, want, resolution, suffix, kwargs)
 
     @classmethod
-    def create_tempfile (cls, want='handle', resolution='try_unlink', suffix='', **kwargs):
-        if want not in ('handle', 'path'):
-            raise ValueError ('unrecognized create_tempfile() "want" mode %r' % (want,))
-        if resolution not in ('unlink', 'try_unlink', 'keep'):
-            raise ValueError ('unrecognized create_tempfile() "resolution" mode %r' % (resolution,))
-        return cls._PathTempfileContextManager (cls, want, resolution, suffix, kwargs)
-
+    def create_tempfile(
+        cls, want="handle", resolution="try_unlink", suffix="", **kwargs
+    ):
+        if want not in ("handle", "path"):
+            raise ValueError('unrecognized create_tempfile() "want" mode %r' % (want,))
+        if resolution not in ("unlink", "try_unlink", "keep"):
+            raise ValueError(
+                'unrecognized create_tempfile() "resolution" mode %r' % (resolution,)
+            )
+        return cls._PathTempfileContextManager(cls, want, resolution, suffix, kwargs)
 
-    def rellink_to (self, target, force=False):
+    def rellink_to(self, target, force=False):
         """Make this path a symlink pointing to the given *target*, generating the
-	proper relative path using :meth:`make_relative`. This gives different
-	behavior than :meth:`symlink_to`. For instance, ``Path
-	('a/b').symlink_to ('c')`` results in ``a/b`` pointing to the path
-	``c``, whereas :meth:`rellink_to` results in it pointing to ``../c``.
-	This can result in broken relative paths if (continuing the example)
-	``a`` is a symbolic link to a directory.
-
-	If either *target* or *self* is absolute, the symlink will point at
-	the absolute path to *target*. The intention is that if you’re trying
-	to link ``/foo/bar`` to ``bee/boo``, it probably makes more sense for
-	the link to point to ``/path/to/.../bee/boo`` rather than
-	``../../../../bee/boo``.
+        proper relative path using :meth:`make_relative`. This gives different
+        behavior than :meth:`symlink_to`. For instance, ``Path
+        ('a/b').symlink_to ('c')`` results in ``a/b`` pointing to the path
+        ``c``, whereas :meth:`rellink_to` results in it pointing to ``../c``.
+        This can result in broken relative paths if (continuing the example)
+        ``a`` is a symbolic link to a directory.
+
+        If either *target* or *self* is absolute, the symlink will point at
+        the absolute path to *target*. The intention is that if you’re trying
+        to link ``/foo/bar`` to ``bee/boo``, it probably makes more sense for
+        the link to point to ``/path/to/.../bee/boo`` rather than
+        ``../../../../bee/boo``.
 
-	If *force* is true, :meth:`try_unlink` will be called on *self* before
-	the link is made, forcing its re-creation.
+        If *force* is true, :meth:`try_unlink` will be called on *self* before
+        the link is made, forcing its re-creation.
 
         """
-        target = self.__class__ (target)
+        target = self.__class__(target)
 
         if force:
-            self.try_unlink ()
-
-        if self.is_absolute ():
-            target = target.absolute () # force absolute link
+            self.try_unlink()
 
-        return self.symlink_to (target.make_relative (self.parent))
+        if self.is_absolute():
+            target = target.absolute()  # force absolute link
 
+        return self.symlink_to(target.make_relative(self.parent))
 
-    def rmtree (self, errors='warn'):
+    def rmtree(self, errors="warn"):
         """Recursively delete this directory and its contents. The *errors* keyword
         specifies how errors are handled:
 
         "warn" (the default)
           Print a warning to standard error.
         "ignore"
           Ignore errors.
 
         """
         import shutil
 
-        if errors == 'ignore':
+        if errors == "ignore":
             ignore_errors = True
             onerror = None
-        elif errors == 'warn':
+        elif errors == "warn":
             ignore_errors = False
             from .cli import warn
 
-            def onerror (func, path, exc_info):
-                warn ('couldn\'t rmtree %s: in %s of %s: %s', self, func.__name__,
-                      path, exc_info[1])
+            def onerror(func, path, exc_info):
+                warn(
+                    "couldn't rmtree %s: in %s of %s: %s",
+                    self,
+                    func.__name__,
+                    path,
+                    exc_info[1],
+                )
+
         else:
-            raise ValueError ('unexpected "errors" keyword %r' % (errors,))
+            raise ValueError('unexpected "errors" keyword %r' % (errors,))
 
-        shutil.rmtree (text_type (self), ignore_errors=ignore_errors, onerror=onerror)
+        shutil.rmtree(str(self), ignore_errors=ignore_errors, onerror=onerror)
         return self
 
-
-    def try_unlink (self):
+    def try_unlink(self):
         """Try to unlink this path. If it doesn't exist, no error is returned. Returns
         a boolean indicating whether the path was really unlinked.
 
         """
         try:
-            self.unlink ()
+            self.unlink()
             return True
         except OSError as e:
             if e.errno == 2:
-                return False # ENOENT
+                return False  # ENOENT
             raise
 
-
     # Data I/O
 
-    def try_open (self, null_if_noexist=False, **kwargs):
+    def try_open(self, null_if_noexist=False, **kwargs):
         """Call :meth:`Path.open` on this path (passing *kwargs*) and return the
         result. If the file doesn't exist, the behavior depends on
         *null_if_noexist*. If it is false (the default), ``None`` is returned.
         Otherwise, :data:`os.devnull` is opened and returned.
 
         """
         try:
-            return self.open (**kwargs)
+            return self.open(**kwargs)
         except IOError as e:
             if e.errno == 2:
                 if null_if_noexist:
                     import io, os
-                    return io.open (os.devnull, **kwargs)
+
+                    return io.open(os.devnull, **kwargs)
                 return None
             raise
 
-
-    def as_hdf_store (self, mode='r', **kwargs):
+    def as_hdf_store(self, mode="r", **kwargs):
         """Return the path as an opened :class:`pandas.HDFStore` object. Note that the
         :class:`HDFStore` constructor unconditionally prints messages to
         standard output when opening and closing files, so use of this
         function will pollute your program’s standard output. The *kwargs* are
         forwarded to the :class:`HDFStore` constructor.
 
         """
         from pandas import HDFStore
-        return HDFStore (text_type (self), mode=mode, **kwargs)
 
+        return HDFStore(str(self), mode=mode, **kwargs)
 
-    def read_astropy_ascii (self, **kwargs):
+    def read_astropy_ascii(self, **kwargs):
         """Open as an ASCII table, returning a :class:`astropy.table.Table` object.
         Keyword arguments are passed to :func:`astropy.io.ascii.open`; valid
         ones likely include:
 
         - ``names = <list>`` (column names)
         - ``format`` ('basic', 'cds', 'csv', 'ipac', ...)
         - ``guess = True`` (guess table format)
@@ -704,18 +716,18 @@
         - ``converters = <dict>``
         - ``include_names = <list>`` (names of columns to include)
         - ``exclude_names = <list>`` (names of columns to exclude; applied after include)
         - ``fill_values = <dict>`` (filler values)
 
         """
         from astropy.io import ascii
-        return ascii.read (text_type (self), **kwargs)
 
+        return ascii.read(str(self), **kwargs)
 
-    def read_fits (self, **kwargs):
+    def read_fits(self, **kwargs):
         """Open as a FITS file, returning a :class:`astropy.io.fits.HDUList` object.
         Keyword arguments are passed to :func:`astropy.io.fits.open`; valid
         ones likely include:
 
         - ``mode = 'readonly'`` (or "update", "append", "denywrite", "ostream")
         - ``memmap = None``
         - ``save_backup = False``
@@ -726,18 +738,18 @@
         - ``disable_image_compression = False``
         - ``do_not_scale_image_data = False``
         - ``ignore_blank = False``
         - ``scale_back = False``
 
         """
         from astropy.io import fits
-        return fits.open (text_type (self), **kwargs)
 
+        return fits.open(str(self), **kwargs)
 
-    def read_fits_bintable (self, hdu=1, drop_nonscalar_ok=True, **kwargs):
+    def read_fits_bintable(self, hdu=1, drop_nonscalar_ok=True, **kwargs):
         """Open as a FITS file, read in a binary table, and return it as a
         :class:`pandas.DataFrame`, converted with
         :func:`pkwit.numutil.fits_recarray_to_data_frame`. The *hdu* argument
         specifies which HDU to read, with its default 1 indicating the first
         FITS extension. The *drop_nonscalar_ok* argument specifies if
         non-scalar table values (which are inexpressible in
         :class:`pandas.DataFrame`s) should be silently ignored (``True``) or
@@ -746,29 +758,28 @@
         :meth:`Path.read_fits`) although the open mode is hardcoded to be
         ``"readonly"``.
 
         """
         from astropy.io import fits
         from .numutil import fits_recarray_to_data_frame as frtdf
 
-        with fits.open (text_type (self), mode='readonly', **kwargs) as hdulist:
-            return frtdf (hdulist[hdu].data, drop_nonscalar_ok=drop_nonscalar_ok)
-
+        with fits.open(str(self), mode="readonly", **kwargs) as hdulist:
+            return frtdf(hdulist[hdu].data, drop_nonscalar_ok=drop_nonscalar_ok)
 
-    def read_hdf (self, key, **kwargs):
+    def read_hdf(self, key, **kwargs):
         """Open as an HDF5 file using :mod:`pandas` and return the item stored under
         the key *key*. *kwargs* are passed to :func:`pandas.read_hdf`.
 
         """
         # This one needs special handling because of the "key" and path input.
         import pandas
-        return pandas.read_hdf (text_type (self), key, **kwargs)
 
+        return pandas.read_hdf(str(self), key, **kwargs)
 
-    def read_inifile (self, noexistok=False, typed=False):
+    def read_inifile(self, noexistok=False, typed=False):
         """Open assuming an “ini-file” format and return a generator yielding data
         records using either :func:`pwkit.inifile.read_stream` (if *typed* is
         false) or :func:`pwkit.tinifile.read_stream` (if it’s true). The
         latter version is designed to work with numerical data using the
         :mod:`pwkit.msmt` subsystem. If *noexistok* is true, a nonexistent
         file will result in no items being generated rather than an
         :exc:`IOError` being raised.
@@ -776,174 +787,171 @@
         """
         if typed:
             from .tinifile import read_stream
         else:
             from .inifile import read_stream
 
         try:
-            with self.open ('rb') as f:
-                for item in read_stream (f):
+            with self.open("rb") as f:
+                for item in read_stream(f):
                     yield item
         except IOError as e:
             if e.errno != 2 or not noexistok:
                 raise
 
-
-    def read_json (self, mode='rt', **kwargs):
+    def read_json(self, mode="rt", **kwargs):
         """Use the :mod:`json` module to read in this file as a JSON-formatted data
         structure. Keyword arguments are passed to :func:`json.load`. Returns the
         read-in data structure.
 
         """
         import json
 
-        with self.open (mode=mode) as f:
-            return json.load (f, **kwargs)
+        with self.open(mode=mode) as f:
+            return json.load(f, **kwargs)
 
-
-    def read_lines (self, mode='rt', noexistok=False, **kwargs):
+    def read_lines(self, mode="rt", noexistok=False, **kwargs):
         """Generate a sequence of lines from the file pointed to by this path, by
         opening as a regular file and iterating over it. The lines therefore
         contain their newline characters. If *noexistok*, a nonexistent file
         will result in an empty sequence rather than an exception. *kwargs*
         are passed to :meth:`Path.open`.
 
         """
         try:
-            with self.open (mode=mode, **kwargs) as f:
+            with self.open(mode=mode, **kwargs) as f:
                 for line in f:
                     yield line
         except IOError as e:
             if e.errno != 2 or not noexistok:
                 raise
 
-
-    def read_numpy (self, **kwargs):
+    def read_numpy(self, **kwargs):
         """Read this path into a :class:`numpy.ndarray` using :func:`numpy.load`.
         *kwargs* are passed to :func:`numpy.load`; they likely are:
 
-	mmap_mode : None, 'r+', 'r', 'w+', 'c'
+        mmap_mode : None, 'r+', 'r', 'w+', 'c'
           Load the array using memory-mapping
-	allow_pickle : bool = True
+        allow_pickle : bool = True
           Whether Pickle-format data are allowed; potential security hazard.
-	fix_imports : bool = True
-	  Try to fix Python 2->3 import renames when loading Pickle-format data.
-	encoding : 'ASCII', 'latin1', 'bytes'
-	  The encoding to use when reading Python 2 strings in Pickle-format data.
+        fix_imports : bool = True
+          Try to fix Python 2->3 import renames when loading Pickle-format data.
+        encoding : 'ASCII', 'latin1', 'bytes'
+          The encoding to use when reading Python 2 strings in Pickle-format data.
 
         """
         import numpy as np
-        with self.open ('rb') as f:
-            return np.load (f, **kwargs)
 
+        with self.open("rb") as f:
+            return np.load(f, **kwargs)
 
-    def read_numpy_text (self, dfcols=None, **kwargs):
+    def read_numpy_text(self, dfcols=None, **kwargs):
         """Read this path into a :class:`numpy.ndarray` as a text file using
         :func:`numpy.loadtxt`. In normal conditions the returned array is
         two-dimensional, with the first axis spanning the rows in the file and
         the second axis columns (but see the *unpack* and *dfcols* keywords).
 
         If *dfcols* is not None, the return value is a
         :class:`pandas.DataFrame` constructed from the array. *dfcols* should
         be an iterable of column names, one for each of the columns returned
         by the :func:`numpy.loadtxt` call. For convenience, if *dfcols* is a
         single string, it will by turned into an iterable by a call to
         :func:`str.split`.
 
         The remaining *kwargs* are passed to :func:`numpy.loadtxt`; they likely are:
 
-	dtype : data type
-	  The data type of the resulting array.
-	comments : str
-	  If specific, a character indicating the start of a comment.
-	delimiter : str
-	  The string that separates values. If unspecified, any span of whitespace works.
-	converters : dict
-	  A dictionary mapping zero-based column *number* to a function that will
-	  turn the cell text into a number.
-	skiprows : int (default=0)
-	  Skip this many lines at the top of the file
-	usecols : sequence
-	  Which columns keep, by number, starting at zero.
-	unpack : bool (default=False)
-	  If true, the return value is transposed to be of shape ``(cols, rows)``.
-	ndmin : int (default=0)
-	  The returned array will have at least this many dimensions; otherwise
-	  mono-dimensional axes will be squeezed.
+        dtype : data type
+          The data type of the resulting array.
+        comments : str
+          If specific, a character indicating the start of a comment.
+        delimiter : str
+          The string that separates values. If unspecified, any span of whitespace works.
+        converters : dict
+          A dictionary mapping zero-based column *number* to a function that will
+          turn the cell text into a number.
+        skiprows : int (default=0)
+          Skip this many lines at the top of the file
+        usecols : sequence
+          Which columns keep, by number, starting at zero.
+        unpack : bool (default=False)
+          If true, the return value is transposed to be of shape ``(cols, rows)``.
+        ndmin : int (default=0)
+          The returned array will have at least this many dimensions; otherwise
+          mono-dimensional axes will be squeezed.
 
         """
         import numpy as np
 
         if dfcols is not None:
-            kwargs['unpack'] = True
+            kwargs["unpack"] = True
 
-        retval = np.loadtxt (text_type (self), **kwargs)
+        retval = np.loadtxt(str(self), **kwargs)
 
         if dfcols is not None:
             import pandas as pd
-            if isinstance (dfcols, six.string_types):
-                dfcols = dfcols.split ()
-            retval = pd.DataFrame (dict (zip (dfcols, retval)))
 
-        return retval
+            if isinstance(dfcols, str):
+                dfcols = dfcols.split()
+            retval = pd.DataFrame(dict(zip(dfcols, retval)))
 
+        return retval
 
-    def read_pandas (self, format='table', **kwargs):
+    def read_pandas(self, format="table", **kwargs):
         """Read using :mod:`pandas`. The function ``pandas.read_FORMAT`` is called
         where ``FORMAT`` is set from the argument *format*. *kwargs* are
         passed to this function. Supported formats likely include
         ``clipboard``, ``csv``, ``excel``, ``fwf``, ``gbq``, ``html``,
         ``json``, ``msgpack``, ``pickle``, ``sql``, ``sql_query``,
         ``sql_table``, ``stata``, ``table``. Note that ``hdf`` is not
         supported because it requires a non-keyword argument; see
         :meth:`Path.read_hdf`.
 
         """
         import pandas
 
-        reader = getattr (pandas, 'read_' + format, None)
-        if not callable (reader):
-            raise PKError ('unrecognized Pandas format %r: no function pandas.read_%s',
-                           format, format)
-
-        with self.open ('rb') as f:
-            return reader (f, **kwargs)
+        reader = getattr(pandas, "read_" + format, None)
+        if not callable(reader):
+            raise PKError(
+                "unrecognized Pandas format %r: no function pandas.read_%s",
+                format,
+                format,
+            )
 
+        with self.open("rb") as f:
+            return reader(f, **kwargs)
 
-    def read_pickle (self):
+    def read_pickle(self):
         """Open the file, unpickle one object from it using :mod:`pickle`, and return
         it.
 
         """
-        gen = self.read_pickles ()
-        value = gen.next ()
-        gen.close ()
+        gen = self.read_pickles()
+        value = gen.next()
+        gen.close()
         return value
 
-
-    def read_pickles (self):
+    def read_pickles(self):
         """Generate a sequence of objects by opening the path and unpickling items
         until EOF is reached.
 
         """
         try:
             import cPickle as pickle
         except ImportError:
             import pickle
 
-        with self.open (mode='rb') as f:
+        with self.open(mode="rb") as f:
             while True:
                 try:
-                    obj = pickle.load (f)
+                    obj = pickle.load(f)
                 except EOFError:
                     break
                 yield obj
 
-
-    def read_tabfile (self, **kwargs):
+    def read_tabfile(self, **kwargs):
         """Read this path as a table of typed measurements via
         :func:`pwkit.tabfile.read`. Returns a generator for a sequence of
         :class:`pwkit.Holder` objects, one for each row in the table, with
         attributes for each of the columns.
 
         tabwidth : int (default=8)
             The tab width to assume. Defaults to 8 and should not be changed unless
@@ -954,92 +962,95 @@
             If true, a nonexistent file will result in no items being generated, as
             opposed to an :exc:`IOError`.
         kwargs : keywords
             Additional arguments are passed to :func:`io.open`.
 
         """
         from .tabfile import read
-        return read (text_type (self), **kwargs)
 
+        return read(str(self), **kwargs)
 
     def read_text(self, encoding=None, errors=None, newline=None):
         """Read this path as one large chunk of text.
 
         This function reads in the entire file as one big piece of text and
         returns it. The *encoding*, *errors*, and *newline* keywords are
         passed to :meth:`open`.
 
         This is not a good way to read files unless you know for sure that they
         are small.
 
         """
-        with self.open (mode='rt', encoding=encoding, errors=errors, newline=newline) as f:
+        with self.open(
+            mode="rt", encoding=encoding, errors=errors, newline=newline
+        ) as f:
             return f.read()
 
-
     def read_toml(self, encoding=None, errors=None, newline=None, **kwargs):
         """Read this path as a TOML document.
 
         The `TOML <https://github.com/toml-lang/toml>`_ parsing is done with
         the :mod:`pytoml` module. The *encoding*, *errors*, and *newline*
         keywords are passed to :meth:`open`. The remaining *kwargs* are passed
         to :meth:`toml.load`.
 
         Returns the decoded data structure.
 
         """
         import pytoml
 
-        with self.open (mode='rt', encoding=encoding, errors=errors, newline=newline) as f:
-            return pytoml.load (f, **kwargs)
-
+        with self.open(
+            mode="rt", encoding=encoding, errors=errors, newline=newline
+        ) as f:
+            return pytoml.load(f, **kwargs)
 
-    def read_yaml (self, encoding=None, errors=None, newline=None, **kwargs):
+    def read_yaml(self, encoding=None, errors=None, newline=None, **kwargs):
         """Read this path as a YAML document.
 
         The YAML parsing is done with the :mod:`yaml` module. The *encoding*,
         *errors*, and *newline* keywords are passed to :meth:`open`. The
         remaining *kwargs* are passed to :meth:`yaml.load`.
 
         Returns the decoded data structure.
 
         """
         import yaml
 
-        with self.open (mode='rt', encoding=encoding, errors=errors, newline=newline) as f:
-            return yaml.load (f, **kwargs)
+        with self.open(
+            mode="rt", encoding=encoding, errors=errors, newline=newline
+        ) as f:
+            return yaml.load(f, **kwargs)
 
-
-    def write_pickle (self, obj):
+    def write_pickle(self, obj):
         """Dump *obj* to this path using :mod:`cPickle`."""
-        self.write_pickles ((obj, ))
-
+        self.write_pickles((obj,))
 
-    def write_pickles (self, objs):
+    def write_pickles(self, objs):
         """*objs* must be iterable. Write each of its values to this path in sequence
         using :mod:`cPickle`.
 
         """
         try:
             import cPickle as pickle
         except ImportError:
             import pickle
 
-        with self.open (mode='wb') as f:
+        with self.open(mode="wb") as f:
             for obj in objs:
-                pickle.dump (obj, f)
-
+                pickle.dump(obj, f)
 
-    def write_yaml (self, data, encoding=None, errors=None, newline=None, **kwargs):
+    def write_yaml(self, data, encoding=None, errors=None, newline=None, **kwargs):
         """Read *data* to this path as a YAML document.
 
         The *encoding*, *errors*, and *newline* keywords are passed to
         :meth:`open`. The remaining *kwargs* are passed to :meth:`yaml.dump`.
 
         """
         import yaml
 
-        with self.open (mode='wt', encoding=encoding, errors=errors, newline=newline) as f:
-            return yaml.dump (data, stream=f, **kwargs)
+        with self.open(
+            mode="wt", encoding=encoding, errors=errors, newline=newline
+        ) as f:
+            return yaml.dump(data, stream=f, **kwargs)
 
 
 del _ParentPath
```

### Comparing `pwkit-1.1.1/pwkit/kbn_conf.py` & `pwkit-1.2.0/pwkit/kbn_conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,42 +18,41 @@
 vec_kbn_conf - Vectorized version of `kbn_conf`.
 
 TODO: tests!
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('kbn_conf vec_kbn_conf').split ()
+__all__ = str("kbn_conf vec_kbn_conf").split()
 
-from six.moves import range
 from numpy import exp, log, vectorize
 from scipy.special import gammaln
 from scipy.integrate import quad
 from scipy.optimize import newton
 
 
-def _cconst (N, B):
-    s = 0.
-    lnb = log (B)
+def _cconst(N, B):
+    s = 0.0
+    lnb = log(B)
 
-    for n in range (N + 1):
-        s += exp (-B + n * lnb - gammaln (n + 1))
+    for n in range(N + 1):
+        s += exp(-B + n * lnb - gammaln(n + 1))
 
-    return 1. / s
+    return 1.0 / s
 
 
-def _fcnb (C, N, B, S):
-    return C * exp (-(S + B) + N * log (S + B) - gammaln (N + 1))
+def _fcnb(C, N, B, S):
+    return C * exp(-(S + B) + N * log(S + B) - gammaln(N + 1))
 
 
-def _fnb (N, B, S):
-    return _fcnb (_cconst (N, B), N, B, S)
+def _fnb(N, B, S):
+    return _fcnb(_cconst(N, B), N, B, S)
 
 
-def kbn_conf (N, B, CL):
+def kbn_conf(N, B, CL):
     """Given a (integer) number of observed Poisson events `N` and a (real)
     expected number of background events `B` and a confidence limit `CL`
     (between 0 and 1), return the confidence interval on the source event
     rate.
 
     Returns: (Smin, Smax)
 
@@ -75,60 +74,64 @@
 
     """
 
     tol = 1e-6
 
     origN = N
     try:
-        N = int (N)
+        N = int(N)
         assert N == origN
     except Exception:
-        raise ValueError ('N must be an integer')
+        raise ValueError("N must be an integer")
 
-    CL = float (CL)
-    if CL <= 0. or CL >= 1.:
-        raise ValueError ('CL must be between 0 and 1, noninclusive')
+    CL = float(CL)
+    if CL <= 0.0 or CL >= 1.0:
+        raise ValueError("CL must be between 0 and 1, noninclusive")
 
-    B = float (B)
+    B = float(B)
     if B < 0:
-        raise ValueError ('B must be nonnegative')
+        raise ValueError("B must be nonnegative")
 
     # OK, arg-checking is out of the way. Precompute some things ...
 
-    C = _cconst (N, B)
-    f = lambda s: _fcnb (C, N, B, s)
+    C = _cconst(N, B)
+    f = lambda s: _fcnb(C, N, B, s)
 
     # The goal is find Smin and Smax such that the integral of _fnb between
     # Smin and Smax is CL, and _fnb (Smin) = _fnb (Smax). Follow the
     # suggestion in Kraft, Burrows, & Nousek (1991) and start at the
     # maximum-probability value, integrating outwards trying to maintain the
     # constraints. We have to be careful because smin cannot go below zero,
     # and to ignore the enormous typo ("local maximum at S = B + N"!) in the
     # paper!
 
-    smin = smax = max (N - B, 0.)
-    fmin = f (smin)
-    fmax = f (smax)
-    conf = 0.
+    smin = smax = max(N - B, 0.0)
+    fmin = f(smin)
+    fmax = f(smax)
+    conf = 0.0
 
     while conf < CL:
-        if smin == 0. or fmin < fmax:
-            stepsize = max (0.2 * abs (CL - conf) / CL / fmax, tol)
-            conf += quad (f, smax, smax + stepsize)[0]
+        if smin == 0.0 or fmin < fmax:
+            stepsize = max(0.2 * abs(CL - conf) / CL / fmax, tol)
+            conf += quad(f, smax, smax + stepsize)[0]
             smax += stepsize
-            fmax = f (smax)
+            fmax = f(smax)
         else:
-            stepsize = max (min (0.2 * abs (CL - conf) / CL / fmin, 0.1 * smin), tol)
+            stepsize = max(min(0.2 * abs(CL - conf) / CL / fmin, 0.1 * smin), tol)
             if smin - stepsize < tol:
-                conf += quad (f, 0, smin)[0]
-                smin = 0.
+                conf += quad(f, 0, smin)[0]
+                smin = 0.0
             else:
-                conf += quad (f, smin - stepsize, smin)[0]
+                conf += quad(f, smin - stepsize, smin)[0]
                 smin -= stepsize
-            fmin = f (smin)
+            fmin = f(smin)
 
     return smin, smax
 
 
-vec_kbn_conf = vectorize (kbn_conf, otypes=[float, float], doc="""Vectorized form of `kbn_conf`.
+vec_kbn_conf = vectorize(
+    kbn_conf,
+    otypes=[float, float],
+    doc="""Vectorized form of `kbn_conf`.
 
-All three inputs must be broadcastable to a common shape.""")
+All three inputs must be broadcastable to a common shape.""",
+)
```

### Comparing `pwkit-1.1.1/pwkit/kwargv.py` & `pwkit-1.2.0/pwkit/kwargv.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,19 +94,17 @@
 See the :class:`KeywordInfo` documentation for specification of additional
 keyword properties that may be specified. The ``Custom`` name is simply an
 alias for :class:`KeywordInfo`.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str('Custom KwargvError ParseError KeywordInfo ParseKeywords basic').split()
+__all__ = str("Custom KwargvError ParseError KeywordInfo ParseKeywords basic").split()
 
-import six
-from six.moves import range
-from . import Holder, PKError, text_type
+from . import Holder, PKError
 
 
 class KwargvError(PKError):
     """Raised when invalid arguments have been provided."""
 
 
 class ParseError(KwargvError):
@@ -124,60 +122,61 @@
     instance. If *args* is ``None``, ``sys.argv[1:]`` is used. Raises
     :exc:`KwargvError` on invalid arguments (i.e., ones without an equals sign
     or a leading plus sign).
 
     """
     if args is None:
         import sys
+
         args = sys.argv[1:]
 
     parsed = Holder()
 
     for arg in args:
-        if arg[0] == '+':
-            for kw in arg[1:].split(','):
+        if arg[0] == "+":
+            for kw in arg[1:].split(","):
                 parsed.set_one(kw, True)
             # avoid analogous -a,b,c syntax because it gets confused with -a --help, etc.
         else:
-            t = arg.split('=', 1)
+            t = arg.split("=", 1)
             if len(t) < 2:
                 raise KwargvError('don\'t know what to do with argument "%s"', arg)
             if not len(t[1]):
                 raise KwargvError('empty value for keyword argument "%s"', t[0])
             parsed.set_one(t[0], t[1])
 
     return parsed
 
 
 # The fancy, full-featured system.
 
+
 class KeywordInfo(object):
-    """Properties that a keyword argument may have.
+    """Properties that a keyword argument may have."""
 
-    """
     parser = None
     """A callable used to convert the argument text to a Python value.
     This attribute is assigned automatically upon setup."""
 
     default = None
     """The default value for the keyword if it’s left unspecified."""
 
     required = False
     """Whether an error should be raised if the keyword is not seen while
     parsing."""
 
-    sep = ','
+    sep = ","
     """The textual separator between items for list-valued keywords."""
 
     maxvals = None
     """The maximum number of values allowed. This only applies for flexible lists;
     fixed lists have predetermined sizes.
 
     """
-    minvals = 0 # note: maxvals and minvals are used in different ways
+    minvals = 0  # note: maxvals and minvals are used in different ways
     """The minimum number of values allowed in a flexible list, *if the keyword is
     specified at all*. If you want ``minvals = 1``, use ``required = True``.
 
     """
     scale = None
     """If not ``None``, multiply numeric values by this number after parsing."""
 
@@ -225,51 +224,51 @@
         # Slightly black magic. Grayish magic. This lets us be used as
         # a decorator on "fixup" functions to modify or range-check
         # the parsed argument value.
         self.fixupfunc = fixupfunc
         return self
 
 
-Custom = KeywordOptions # sugar for users
+Custom = KeywordOptions  # sugar for users
 
 
 def _parse_bool(s):
     s = s.lower()
 
-    if s in 'y yes t true on 1'.split():
+    if s in "y yes t true on 1".split():
         return True
-    if s in 'n no f false off 0'.split():
+    if s in "n no f false off 0".split():
         return False
     raise ParseError('don\'t know how to interpret "%s" as a boolean' % s)
 
 
 def _val_to_parser(v):
     if isinstance(v, bool):
         return _parse_bool
-    if isinstance(v, (int, float, text_type)):
+    if isinstance(v, (int, float, str)):
         return v.__class__
-    raise ValueError('can\'t figure out how to parse %r' % v)
+    raise ValueError("can't figure out how to parse %r" % v)
 
 
 def _val_or_func_to_parser(v):
     if v is bool:
         return _parse_bool
     if callable(v):
         return v
     return _val_to_parser(v)
 
 
 def _val_or_func_to_default(v):
     if callable(v):
         return None
-    if isinstance(v, (int, float, bool, text_type)):
+    if isinstance(v, (int, float, bool, str)):
         return v
     raise ValueError
 
-    ('can\'t figure out a default for %r' % v)
+    ("can't figure out a default for %r" % v)
 
 
 def _handle_flex_list(ki, ks):
     assert len(ks) == 1
     elemparser = ks[0]
     # I don't think 'foo = [0]' will be useful ...
     assert callable(elemparser)
@@ -287,47 +286,54 @@
 
     def fixlistparse(val):
         items = val.split(ki.sep)
         ngot = len(items)
 
         if ngot < ki.minvals:
             if ki.minvals == ntot:
-                raise ParseError('expected exactly %d values, but only got %d',
-                                 ntot, ngot)
-            raise ParseError('expected between %d and %d values, but only got %d',
-                             ki.minvals, ntot, ngot)
+                raise ParseError(
+                    "expected exactly %d values, but only got %d", ntot, ngot
+                )
+            raise ParseError(
+                "expected between %d and %d values, but only got %d",
+                ki.minvals,
+                ntot,
+                ngot,
+            )
         if ngot > ntot:
-            raise ParseError('expected between %d and %d values, but got %d',
-                             ki.minvals, ntot, ngot)
+            raise ParseError(
+                "expected between %d and %d values, but got %d", ki.minvals, ntot, ngot
+            )
 
-        result = list(defaults) # make a copy
+        result = list(defaults)  # make a copy
         for i in range(ngot):
             result[i] = parsers[i](items[i])
         return result
 
-    return fixlistparse, list(defaults) # make a copy
+    return fixlistparse, list(defaults)  # make a copy
 
 
 class ParseKeywords(Holder):
     """The template class for defining your keyword arguments. A subclass of
     :class:`pwkit.Holder`. Declare attributes in a subclass following the
     scheme described above, then call the :meth:`ParseKeywords.parse` method.
 
     """
+
     def __init__(self):
         kwspecs = self.__class__.__dict__
         kwinfos = {}
 
         # Process our keywords, as specified by the class attributes, into a
         # form more friendly for parsing, and check for things we don't
         # understand. 'kw' is the keyword name exposed to the user; 'attrname'
         # is the name of the attribute to set on the resulting object.
 
-        for kw, ks in six.iteritems(kwspecs):
-            if kw[0] == '_':
+        for kw, ks in kwspecs.items():
+            if kw[0] == "_":
                 continue
 
             ki = KeywordInfo()
             ko = None
             attrname = kw
 
             if isinstance(ks, KeywordOptions):
@@ -351,15 +357,15 @@
                 parser = _val_to_parser(ks)
                 default = _val_or_func_to_default(ks)
 
             ki._attrname = attrname
             ki.parser = parser
             ki.default = default
 
-            if ko is not None: # override with user-specified options
+            if ko is not None:  # override with user-specified options
                 ki.__dict__.update(ko.__dict__)
 
             if ki.required:
                 # makes sense, and prevents trying to call fixupfunc on
                 # weird default values of fixed lists.
                 ki.default = None
             elif ki.repeatable:
@@ -368,66 +374,80 @@
                 # kinda gross structure here, oh well.
                 ki.default = ki.fixupfunc(ki.default)
 
             kwinfos[kw] = ki
 
         # Apply defaults, save parse info, done
 
-        for kw, ki in six.iteritems(kwinfos):
+        for kw, ki in kwinfos.items():
             self.set_one(ki._attrname, ki.default)
 
         self._kwinfos = kwinfos
 
-
     def parse(self, args=None):
         """Parse textual keywords as described by this class’s attributes, and update
         this instance’s attributes with the parsed values. *args* is a list of
         strings; if ``None``, it defaults to ``sys.argv[1:]``. Returns *self*
         for convenience. Raises :exc:`KwargvError` if invalid keywords are
         encountered.
 
         See also :meth:`ParseKeywords.parse_or_die`.
 
         """
         if args is None:
             import sys
+
             args = sys.argv[1:]
 
         seen = set()
 
         for arg in args:
-            t = arg.split('=', 1)
+            t = arg.split("=", 1)
             if len(t) < 2:
                 raise KwargvError('don\'t know what to do with argument "%s"', arg)
 
             kw, val = t
             ki = self._kwinfos.get(kw)
 
             if ki is None:
                 raise KwargvError('unrecognized keyword argument "%s"', kw)
 
             if not len(val):
                 raise KwargvError('empty value for keyword argument "%s"', kw)
 
             try:
                 pval = ki.parser(val)
-            except ParseError as e :
-                raise KwargvError('cannot parse value "%s" for keyword '
-                                  'argument "%s": %s', val, kw, e)
+            except ParseError as e:
+                raise KwargvError(
+                    'cannot parse value "%s" for keyword ' 'argument "%s": %s',
+                    val,
+                    kw,
+                    e,
+                )
             except Exception as e:
                 if ki.printexc:
-                    raise KwargvError('cannot parse value "%s" for keyword '
-                                      'argument "%s": %s', val, kw, e)
-                raise KwargvError('cannot parse value "%s" for keyword '
-                                  'argument "%s"', val, kw)
+                    raise KwargvError(
+                        'cannot parse value "%s" for keyword ' 'argument "%s": %s',
+                        val,
+                        kw,
+                        e,
+                    )
+                raise KwargvError(
+                    'cannot parse value "%s" for keyword ' 'argument "%s"', val, kw
+                )
 
             if ki.maxvals is not None and len(pval) > ki.maxvals:
-                raise KwargvError('keyword argument "%s" may have at most %d'
-                                  ' values, but got %s ("%s")', kw,
-                                  ki.maxvals, len(pval), val)
+                raise KwargvError(
+                    'keyword argument "%s" may have at most %d'
+                    ' values, but got %s ("%s")',
+                    kw,
+                    ki.maxvals,
+                    len(pval),
+                    val,
+                )
 
             if ki.scale is not None:
                 pval = pval * ki.scale
 
             if ki.fixupfunc is not None:
                 pval = ki.fixupfunc(pval)
 
@@ -441,29 +461,30 @@
                 else:
                     cur.append(pval)
                     pval = cur
 
             seen.add(kw)
             self.set_one(ki._attrname, pval)
 
-        for kw, ki in six.iteritems(self._kwinfos):
+        for kw, ki in self._kwinfos.items():
             if kw not in seen:
                 if ki.required:
-                    raise KwargvError('required keyword argument "%s" was not provided', kw)
+                    raise KwargvError(
+                        'required keyword argument "%s" was not provided', kw
+                    )
 
                 # If there's a fixup, process it even if the keyword wasn't
                 # provided. This lets code use "interesting" defaults with
                 # types that you might prefer to use when launching a task
                 # programmatically; e.g. a default output stream that is
                 # `sys.stdout`, not "-".
                 if ki.fixupfunc is not None:
                     self.set_one(ki._attrname, ki.fixupfunc(None))
 
-        return self # convenience
-
+        return self  # convenience
 
     def parse_or_die(self, args=None):
         """Like :meth:`ParseKeywords.parse`, but calls :func:`pkwit.cli.die` if a
         :exc:`KwargvError` is raised, printing the exception text. Returns
         *self* for convenience.
 
         """
@@ -471,9 +492,9 @@
 
         try:
             return self.parse(args)
         except KwargvError as e:
             die(e)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     print(basic())
```

### Comparing `pwkit-1.1.1/pwkit/latex.py` & `pwkit-1.2.0/pwkit/latex.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,39 +45,37 @@
 
 
 XXX: Barely tested!
 
 """
 from __future__ import absolute_import, division, print_function
 
-__all__ = '''
+__all__ = """
 AlignedNumberFormatter
 BasicFormatter
 BoolFormatter
 LimitFormatter
 MaybeNumberFormatter
 Referencer
 TableBuilder
 UncertFormatter
 WideHeader
 latexify_l3col
 latexify_n2col
 latexify_u3col
-latexify'''.split()
+latexify""".split()
 
 import string
-import six
-from six.moves import range
-from . import Holder, PKError, binary_type, msmt, reraise_context, text_type
+from . import Holder, PKError, reraise_context
 
 
 def _reftext(key):
-    if key[0] == '*':
+    if key[0] == "*":
         return key[1:]
-    return '\\citet{%s}' % key
+    return "\\citet{%s}" % key
 
 
 class Referencer(object):
     """Accumulate a numbered list of bibtex references. Methods:
 
     refkey(bibkey)
       Return a string that should be used to give
@@ -94,173 +92,175 @@
     thisworkmarker
       special symbol used to denote "this work"; defaults to star.
 
     Bibtex keys beginning with asterisks have the rest of their value used for
     the citation text, rather than "\citet{<key>}".
 
     """
-    thisworktext = 'this work'
-    thisworkmarker = '$\\star$'
+
+    thisworktext = "this work"
+    thisworkmarker = "$\\star$"
 
     def __init__(self):
         self.bibkeys = []
         self.seenthiswork = False
 
-
     def refkey(self, bibkey):
         if bibkey is None:
-            return ''
+            return ""
 
-        if bibkey == 'thiswork':
+        if bibkey == "thiswork":
             self.seenthiswork = True
             return self.thisworkmarker
 
         try:
             idx = self.bibkeys.index(bibkey)
         except ValueError:
             idx = len(self.bibkeys)
             self.bibkeys.append(bibkey)
 
-        return text_type(idx + 1)
-
+        return str(idx + 1)
 
     def dump(self):
-        s = ', '.join('[%d] %s' % (i + 1, _reftext(self.bibkeys[i]))
-                       for i in range(len(self.bibkeys)))
+        s = ", ".join(
+            "[%d] %s" % (i + 1, _reftext(self.bibkeys[i]))
+            for i in range(len(self.bibkeys))
+        )
 
         if self.seenthiswork:
-            s = ('[%s]: %s, ' % (self.thisworkmarker, self.thisworktext)) + s
+            s = ("[%s]: %s, " % (self.thisworkmarker, self.thisworktext)) + s
 
         return s
 
 
 # Generic infrastructure for converting Python objects to LaTeX.
 #
 # Note that it's important that these functions all accept miscellaneous
 # kwargs arguments, so that TableBuilder invocations can pass along special
 # control keywords that are only specific to certain cells, without causing
 # crashes elsewhere.
 
-_printable_ascii = frozenset(string.printable.encode('ascii'))
+_printable_ascii = frozenset(string.printable.encode("ascii"))
 
-def latexify(obj, **kwargs):
-    """Render an object in LaTeX appropriately.
 
-    """
-    if hasattr(obj, '__pk_latex__'):
+def latexify(obj, **kwargs):
+    """Render an object in LaTeX appropriately."""
+    if hasattr(obj, "__pk_latex__"):
         return obj.__pk_latex__(**kwargs)
 
-    if isinstance(obj, text_type):
+    if isinstance(obj, str):
         from .unicode_to_latex import unicode_to_latex
+
         return unicode_to_latex(obj)
 
     if isinstance(obj, bool):
         # isinstance(True, int) = True, so gotta handle this first.
-        raise ValueError('no well-defined LaTeXification of bool %r' % obj)
+        raise ValueError("no well-defined LaTeXification of bool %r" % obj)
 
     if isinstance(obj, float):
-        nplaces = kwargs.get('nplaces')
+        nplaces = kwargs.get("nplaces")
         if nplaces is None:
-            return '$%f$' % obj
-        return '$%.*f$' % (nplaces, obj)
+            return "$%f$" % obj
+        return "$%.*f$" % (nplaces, obj)
 
     if isinstance(obj, int):
-        return '$%d$' % obj
+        return "$%d$" % obj
 
-    if isinstance(obj, binary_type):
+    if isinstance(obj, bytes):
         if all(c in _printable_ascii for c in obj):
-            return obj.decode('ascii')
-        raise ValueError('no safe LaTeXification of binary string %r' % obj)
+            return obj.decode("ascii")
+        raise ValueError("no safe LaTeXification of binary string %r" % obj)
 
-    raise ValueError('can\'t LaTeXify %r' % obj)
+    raise ValueError("can't LaTeXify %r" % obj)
 
 
 def latexify_n2col(x, nplaces=None, **kwargs):
     """Render a number into LaTeX in a 2-column format, where the columns split
     immediately to the left of the decimal point. This gives nice alignment of
     numbers in a table.
 
     """
     if nplaces is not None:
-        t = '%.*f' % (nplaces, x)
+        t = "%.*f" % (nplaces, x)
     else:
-        t = '%f' % x
+        t = "%f" % x
 
-    if '.' not in t:
-        return '$%s$ &' % t
+    if "." not in t:
+        return "$%s$ &" % t
 
-    left, right = t.split('.')
-    return '$%s$ & $.%s$' % (left, right)
+    left, right = t.split(".")
+    return "$%s$ & $.%s$" % (left, right)
 
 
 def latexify_u3col(obj, **kwargs):
     """Convert an object to special LaTeX for uncertainty tables.
 
     This conversion is meant for uncertain values in a table. The return value
     should span three columns. The first column ends just before the decimal
     point in the main number value, if it has one. It has no separation from
     the second column. The second column goes from the decimal point until
     just before the "plus-or-minus" indicator. The third column goes from the
     "plus-or-minus" until the end. If the item being formatted does not fit this
     schema, it can be wrapped in something like '\multicolumn{3}{c}{...}'.
 
     """
-    if hasattr(obj, '__pk_latex_u3col__'):
+    if hasattr(obj, "__pk_latex_u3col__"):
         return obj.__pk_latex_u3col__(**kwargs)
 
     # TODO: there are reasonable ways to format many basic types, but I'm not
     # going to implement them until I need to.
 
-    raise ValueError('can\'t LaTeXify %r in 3-column uncertain format' % obj)
+    raise ValueError("can't LaTeXify %r in 3-column uncertain format" % obj)
 
 
 def latexify_l3col(obj, **kwargs):
     """Convert an object to special LaTeX for limit tables.
 
     This conversion is meant for limit values in a table. The return value
     should span three columns. The first column is the limit indicator: <, >,
     ~, etc. The second column is the whole part of the value, up until just
     before the decimal point. The third column is the decimal point and the
     fractional part of the value, if present. If the item being formatted does
     not fit this schema, it can be wrapped in something like
     '\multicolumn{3}{c}{...}'.
 
     """
-    if hasattr(obj, '__pk_latex_l3col__'):
+    if hasattr(obj, "__pk_latex_l3col__"):
         return obj.__pk_latex_l3col__(**kwargs)
 
     if isinstance(obj, bool):
         # isinstance(True, int) = True, so gotta handle this first.
-        raise ValueError('no well-defined l3col LaTeXification of bool %r' % obj)
+        raise ValueError("no well-defined l3col LaTeXification of bool %r" % obj)
 
     if isinstance(obj, float):
-        return '&' + latexify_n2col(obj, **kwargs)
+        return "&" + latexify_n2col(obj, **kwargs)
 
     if isinstance(obj, int):
-        return '& $%d$ &' % obj
-
-    raise ValueError('can\'t LaTeXify %r in 3-column limit format' % obj)
+        return "& $%d$ &" % obj
 
+    raise ValueError("can't LaTeXify %r in 3-column limit format" % obj)
 
 
 # Building nice deluxetables.
 
+
 class WideHeader(object):
     """Information needed for constructing wide table headers.
 
     nlogcols - Number of logical columns consumed by this header.
     content  - The LaTeX to insert for this header's content.
     align    - The alignment of this header; default 'c'.
 
     Rendered as \multicolumn{nlatex}{align}{content}, where `nlatex` is the
     number of LaTeX columns spanned by this header -- which may be larger than
     `nlogcols` if certain logical columns span multiple LaTeX columns.
 
     """
-    def __init__(self, nlogcols, content, align='c'):
+
+    def __init__(self, nlogcols, content, align="c"):
         self.nlogcols = nlogcols
         self.align = align
         self.content = content
 
 
 class TableBuilder(object):
     """Build and then emit a nice deluxetable.
@@ -318,33 +318,35 @@
     are handled specially.
 
     If \\tablewidth{} is not provided, the table is set at full width, not its
     natural width, which is a lame default. The default `widthspec` lets us
     auto-widen while providing a clear avenue to customizing the width.
 
     """
-    environment = 'deluxetable'
+
+    environment = "deluxetable"
     label = None
-    note = ''
-    preamble = ''
-    refs = ''
-    title = 'Untitled table'
-    widthspec = '0em'
+    note = ""
+    preamble = ""
+    refs = ""
+    title = "Untitled table"
+    widthspec = "0em"
     numbercols = True
     final_double_backslash = False
 
     def __init__(self, label):
         self._colinfo = []
         self._hclines = []
         self._notes = {}
         self._notecounter = 0
         self.label = latexify(label)
 
-
-    def addcol(self, headings, datafunc, formatter=None, colspec=None, numbering='(%d)'):
+    def addcol(
+        self, headings, datafunc, formatter=None, colspec=None, numbering="(%d)"
+    ):
         """Define a logical column. Arguments:
 
         headings
           A string, or list of strings and WideHeaders. The headings are stacked
           vertically in the table header section.
         datafunc
           Return LaTeX for this cell. Call spec should be
@@ -357,49 +359,54 @@
           If non-False, a format for writing this column's number; if False,
           no number is written.
 
         """
         if formatter is None:
             formatter = BasicFormatter()
 
-        if isinstance(headings, six.string_types):
-            headings = (headings, )
+        if isinstance(headings, str):
+            headings = (headings,)
 
         try:
-            code = six.get_function_code(datafunc)
+            code = datafunc.__code__
             nargs = code.co_argcount
         except AttributeError:
-            if hasattr(datafunc, '__call__'):
+            if hasattr(datafunc, "__call__"):
                 # This is pretty hacky ...
-                nargs = six.get_function_code(datafunc.__call__).co_argcount - 1
+                nargs = datafunc.__call__.__code__.co_argcount - 1
             else:
-                raise ValueError('cannot find code object for datafunc')
+                raise ValueError("cannot find code object for datafunc")
 
         if nargs == 3:
-            wrapped = datafunc # (item, formatter, builder)
+            wrapped = datafunc  # (item, formatter, builder)
         elif nargs == 2:
             wrapped = lambda i, f, b: datafunc(i, f)
         elif nargs == 1:
             wrapped = lambda i, f, b: datafunc(i)
-        elif nargs == 0: # why not
+        elif nargs == 0:  # why not
             wrapped = lambda i, f, b: datafunc()
         else:
-            raise ValueError('datafunc must accept between 0 and 3 args; it takes %d' % nargs)
-
-        ci = Holder(headings=[latexify(h) for h in headings], formatter=formatter,
-                    wdatafunc=wrapped, colspec=colspec, numbering=numbering)
+            raise ValueError(
+                "datafunc must accept between 0 and 3 args; it takes %d" % nargs
+            )
+
+        ci = Holder(
+            headings=[latexify(h) for h in headings],
+            formatter=formatter,
+            wdatafunc=wrapped,
+            colspec=colspec,
+            numbering=numbering,
+        )
         self._colinfo.append(ci)
         return self
 
-
     def addnote(self, key, text):
         self._notes[key] = [None, text]
         return self
 
-
     def addhcline(self, headerrowidx, logcolidx, latexdeltastart, latexdeltaend):
         """Adds a horizontal line below a limited range of columns in the header section.
         Arguments:
 
         headerrowidx    - The 0-based row number *below* which the line will be
                           drawn; i.e. 0 means that the line will be drawn below
                           the first row of header cells.
@@ -415,36 +422,33 @@
                           if you want to underline two LaTeX columns,
                           latexdeltaend = latexdeltastart + 2.
 
         """
         self._hclines.append((headerrowidx, logcolidx, latexdeltastart, latexdeltaend))
         return self
 
-
     def notemark(self, key):
         noteinfo = self._notes.get(key)
         if noteinfo is None:
             raise ValueError('unrecognized note key "%s"' % key)
 
         if noteinfo[0] is None:
             if self._notecounter > 25:
-                raise PKError('maximum number of table notes exceeded')
+                raise PKError("maximum number of table notes exceeded")
 
             noteinfo[0] = self._notecounter
             self._notecounter += 1
 
-        return '\\tablenotemark{%c}' % chr(ord('a') + noteinfo[0])
-
+        return "\\tablenotemark{%c}" % chr(ord("a") + noteinfo[0])
 
     def emit(self, stream, items):
-        from six import itervalues
         write = stream.write
         colinfo = self._colinfo
 
-        colspec = ''
+        colspec = ""
         ncols = 0
         nheadrows = 0
         curlatexcol = 1
 
         for ci in colinfo:
             ci.nlcol, colspecpart, ci.headprefix = ci.formatter.colinfo(self)
             ci.latexcol = curlatexcol
@@ -452,278 +456,289 @@
             if ci.colspec is not None:
                 # This is more about convenience for columns that don't have
                 # fancy alignment requirements, rather than about allowing
                 # overriding.
                 colspecpart = latexify(ci.colspec)
 
             if colspecpart is None:
-                colspecpart = 'c' * ci.nlcol
+                colspecpart = "c" * ci.nlcol
 
             ncols += ci.nlcol
             colspec += colspecpart
             nheadrows = max(nheadrows, len(ci.headings))
             curlatexcol += ci.nlcol
 
-        write('% TableBuilder table\n')
-        write('\\begin{')
+        write("% TableBuilder table\n")
+        write("\\begin{")
         write(self.environment)
-        write('}{')
+        write("}{")
         write(colspec)
-        write('}\n%custom preamble\n')
+        write("}\n%custom preamble\n")
         write(self.preamble)
-        write('\n%hardcoded preamble\n\\tablecolumns{')
-        write(text_type(ncols))
-        write('}\n\\tablewidth{')
+        write("\n%hardcoded preamble\n\\tablecolumns{")
+        write(str(ncols))
+        write("}\n\\tablewidth{")
         write(self.widthspec)
-        write('}\n\\tablecaption{')
+        write("}\n\\tablecaption{")
         write(self.title)
-        write('\\label{')
+        write("\\label{")
         write(self.label)
-        write('}}\n\\tablehead{\n')
+        write("}}\n\\tablehead{\n")
 
-        cr = ''
+        cr = ""
 
         for i in range(nheadrows):
             write(cr)
 
             for hidx, cidx, lds, lde in self._hclines:
                 # Note super inefficiency. Who cares?
                 if hidx == i - 1:
                     latexcolbase = colinfo[cidx].latexcol
-                    write(' \\cline{')
-                    write(text_type(latexcolbase + lds))
-                    write('-')
-                    write(text_type(latexcolbase + lde - 1))
-                    write('} ')
+                    write(" \\cline{")
+                    write(str(latexcolbase + lds))
+                    write("-")
+                    write(str(latexcolbase + lde - 1))
+                    write("} ")
 
-            sep = ''
+            sep = ""
             nlefttoskip = 0
 
             for cidx, ci in enumerate(colinfo):
                 write(sep)
 
                 if nlefttoskip < 1:
                     if len(ci.headings) <= i:
-                        write(' & ' * (ci.nlcol - 1))
+                        write(" & " * (ci.nlcol - 1))
                     else:
                         h = ci.headings[i]
 
                         if isinstance(h, WideHeader):
                             nlefttoskip = h.nlogcols
 
                             nlatex = 0
                             for j in range(h.nlogcols):
                                 nlatex += colinfo[cidx + j].nlcol
 
-                            write('\\multicolumn{')
-                            write(text_type(nlatex))
-                            write('}{')
+                            write("\\multicolumn{")
+                            write(str(nlatex))
+                            write("}{")
                             write(h.align)
-                            write('}{')
+                            write("}{")
                             write(h.content)
-                            write('}')
+                            write("}")
                         else:
                             write(ci.headprefix)
-                            write('{')
+                            write("{")
                             write(h)
-                            write('}')
+                            write("}")
 
                 nlefttoskip -= 1
 
                 if nlefttoskip > 0:
-                    sep = ' '
+                    sep = " "
                 else:
-                    sep = ' & '
+                    sep = " & "
 
-            cr = ' \\\\\n'
+            cr = " \\\\\n"
 
         if self.numbercols:
             colnum = 1
-            sep = ''
-            write(' \\\\ \\\\\n')
+            sep = ""
+            write(" \\\\ \\\\\n")
 
             for ci in colinfo:
                 write(sep)
-                write('\\multicolumn{')
-                write(text_type(ci.nlcol))
-                write('}{c}{')
+                write("\\multicolumn{")
+                write(str(ci.nlcol))
+                write("}{c}{")
                 if ci.numbering is False:
                     pass
-                elif '%d' in ci.numbering:
+                elif "%d" in ci.numbering:
                     write(ci.numbering % colnum)
                     colnum += 1
                 else:
                     write(ci.numbering)
-                write('}')
-                sep = ' & '
+                write("}")
+                sep = " & "
 
-        write('\n}\n\\startdata\n')
+        write("\n}\n\\startdata\n")
 
-        cr = ''
+        cr = ""
 
         for item in items:
             write(cr)
-            sep = ''
+            sep = ""
 
-            rp = getattr(item, 'tb_row_preamble', None)
+            rp = getattr(item, "tb_row_preamble", None)
             if rp is not None:
                 write(rp)
 
             for ci in colinfo:
                 write(sep)
                 formatted = ci.wdatafunc(item, ci.formatter, self)
                 try:
                     write(formatted)
                 except Exception:
-                    reraise_context('while writing %r (from %r with %r)',
-                                    formatted, item, ci.formatter)
-                sep = ' & '
+                    reraise_context(
+                        "while writing %r (from %r with %r)",
+                        formatted,
+                        item,
+                        ci.formatter,
+                    )
+                sep = " & "
 
-            cr = ' \\\\\n'
+            cr = " \\\\\n"
 
         if self.final_double_backslash:
-            write(' \\\\')
-        write('\n\\enddata\n')
+            write(" \\\\")
+        write("\n\\enddata\n")
 
         if self.note is not None and len(self.note):
-            write('\\tablecomments{')
+            write("\\tablecomments{")
             write(self.note)
-            write('}\n')
+            write("}\n")
 
         if self.refs is not None and len(self.refs):
-            write('\\tablerefs{')
+            write("\\tablerefs{")
             write(self.refs)
-            write('}\n')
+            write("}\n")
 
-        for noteinfo in sorted((ni for ni in itervalues(self._notes)
-                                 if ni[0] is not None), key=lambda ni: ni[0]):
-            write('\\tablenotetext{')
-            write(chr(ord('a') + noteinfo[0]))
-            write('}{')
+        for noteinfo in sorted(
+            (ni for ni in self._notes.values() if ni[0] is not None),
+            key=lambda ni: ni[0],
+        ):
+            write("\\tablenotetext{")
+            write(chr(ord("a") + noteinfo[0]))
+            write("}{")
             write(noteinfo[1])
-            write('}\n')
+            write("}\n")
 
-        write('\\end{')
+        write("\\end{")
         write(self.environment)
-        write('}\n% end TableBuilder table\n')
+        write("}\n% end TableBuilder table\n")
 
 
 class BasicFormatter(object):
     """Base class for formatting table cells in a TableBuilder.
 
     Generally a formatter will also provide methods for turning input data
     into fancified LaTeX output that can be used by the column's "data
     function".
 
     """
+
     def colinfo(self, builder):
         """Return (nlcol, colspec, headprefix), where:
 
         nlcol      - The number of LaTeX columns encompassed by this logical
                      column.
         colspec    - Its LaTeX column specification (None to force user to
                      specify).
         headprefix - Prefix applied before heading items in {} (e.g.,
                      "\\colhead").
 
         """
-        return 1, None, '\\colhead'
-
+        return 1, None, "\\colhead"
 
 
 class BoolFormatter(BasicFormatter):
     """Format booleans. Attributes `truetext` and `falsetext` set what shows up
     for true and false values, respectively.
 
     """
-    truetext = '$\\bullet$'
-    falsetext = ''
+
+    truetext = "$\\bullet$"
+    falsetext = ""
 
     def colinfo(self, builder):
-        return 1, 'c', '\\colhead'
+        return 1, "c", "\\colhead"
 
     def format(self, value):
         if value:
             return self.truetext
         return self.falsetext
 
 
 class MaybeNumberFormatter(BasicFormatter):
     """Format Python objects. If it's a number, format it as such, without any
     fancy column alignment, but with a specifiable number of decimal places.
     Otherwise, call latexify() on it.
 
     """
-    def __init__(self, nplaces=1, align='c'):
+
+    def __init__(self, nplaces=1, align="c"):
         self.nplaces = nplaces
         self.align = align
 
     def colinfo(self, builder):
-        return 1, self.align, '\\colhead'
+        return 1, self.align, "\\colhead"
 
     def format(self, datum, nplaces=None):
         if datum is None:
-            return ''
+            return ""
 
         try:
             v = float(datum)
         except TypeError:
             return latexify(datum)
         else:
             if nplaces is None:
                 nplaces = self.nplaces
-            return '$%.*f$' % (nplaces, v)
+            return "$%.*f$" % (nplaces, v)
 
 
 class AlignedNumberFormatter(BasicFormatter):
     """Format numbers. Allows the number of decimal places to be specified, and
     aligns the numbers at the decimal point.
 
     """
+
     def __init__(self, nplaces=1):
         self.nplaces = nplaces
 
     def colinfo(self, builder):
-        return 2, 'r@{}l', '\\multicolumn{2}{c}'
+        return 2, "r@{}l", "\\multicolumn{2}{c}"
 
     def format(self, datum, nplaces=None):
         if datum is None:
-            return ' & '
+            return " & "
         if nplaces is None:
             nplaces = self.nplaces
 
         return latexify_n2col(float(datum), nplaces=nplaces)
 
 
 class UncertFormatter(BasicFormatter):
     """Format measurements (cf. pwkit.msmt) with detailed uncertainty information,
     possibly including asymmetric uncertainties. Because of the latter
     possibility, table rows have to be made extra-high to maintain evenness.
 
     """
-    strut = r'\rule{0pt}{3ex}'
+
+    strut = r"\rule{0pt}{3ex}"
 
     def colinfo(self, builder):
-        return 3, r'r@{}l@{\,}l', r'\multicolumn{3}{c}'
+        return 3, r"r@{}l@{\,}l", r"\multicolumn{3}{c}"
 
     def format(self, datum, **kwargs):
         if datum is None:
-            return ' & & ' + self.strut
+            return " & & " + self.strut
         return latexify_u3col(datum, **kwargs) + self.strut
 
 
 class LimitFormatter(BasicFormatter):
     """Format measurements (cf pwkit.msmt) with nice-looking limit information.
     Specific uncertainty information is discarded. The default formats do not
     involve fancy subscripts or superscripts, so row struts are not needed ...
     by default.
 
     """
-    strut = ''
+
+    strut = ""
 
     def colinfo(self, builder):
-        return 3, r'r@{\,}r@{}l', r'\multicolumn{3}{c}'
+        return 3, r"r@{\,}r@{}l", r"\multicolumn{3}{c}"
 
     def format(self, datum, **kwargs):
         if datum is None:
-            return ' & & ' + self.strut
+            return " & & " + self.strut
         return latexify_l3col(datum, **kwargs) + self.strut
```

### Comparing `pwkit-1.1.1/pwkit/lmmin.py` & `pwkit-1.2.0/pwkit/lmmin.py`

 * *Files 13% similar despite different names*

```diff
@@ -212,208 +212,213 @@
 information regarding provenance, license, and academic references,
 see comments in the module source code.)
 
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = '''enorm_fast enorm_mpfit_careful enorm_minpack Problem Solution
-ResidualProblem check_derivative'''.split()
+__all__ = """enorm_fast enorm_mpfit_careful enorm_minpack Problem Solution
+ResidualProblem check_derivative""".split()
 
 
-from six.moves import range
 import numpy as np
 
 # Quickie testing infrastructure
 
 _testfuncs = []
 
-def test(f): # a decorator
+
+def test(f):  # a decorator
     _testfuncs.append(f)
     return f
 
+
 def _runtests(namefilt=None):
     for f in _testfuncs:
         if namefilt is not None and f.__name__ != namefilt:
             continue
         n = f.__name__
-        if n[0] == '_':
+        if n[0] == "_":
             n = n[1:]
-        print(n, '...')
+        print(n, "...")
         f()
 
+
 from numpy.testing import assert_array_almost_equal as Taaae
 from numpy.testing import assert_almost_equal as Taae
 
+
 def _timer_helper(n=100):
     for i in range(n):
         for f in _testfuncs:
             f()
 
 
 # Parameter Info attributes that can be specified
 #
 # Each parameter can be described by five floats:
 
-PI_F_VALUE = 0 # specified initial value
-PI_F_LLIMIT = 1 # lower bound on param value (can be -inf)
-PI_F_ULIMIT = 2 # upper bound (can be +inf)
-PI_F_STEP = 3 # fixed parameter step size to use (abs or rel), 0. for unspecified
-PI_F_MAXSTEP = 4 # maximum step to take
+PI_F_VALUE = 0  # specified initial value
+PI_F_LLIMIT = 1  # lower bound on param value (can be -inf)
+PI_F_ULIMIT = 2  # upper bound (can be +inf)
+PI_F_STEP = 3  # fixed parameter step size to use (abs or rel), 0. for unspecified
+PI_F_MAXSTEP = 4  # maximum step to take
 PI_NUM_F = 5
 
 # Four bits of data
-PI_M_SIDE = 0x3 # sidedness of derivative - two bits
-PI_M_FIXED = 0x4 # fixed value
-PI_M_RELSTEP = 0x8 # whether the specified stepsize is relative
+PI_M_SIDE = 0x3  # sidedness of derivative - two bits
+PI_M_FIXED = 0x4  # fixed value
+PI_M_RELSTEP = 0x8  # whether the specified stepsize is relative
 
 # And one object
-PI_O_TIEFUNC = 0 # fixed to be a function of other parameters
+PI_O_TIEFUNC = 0  # fixed to be a function of other parameters
 PI_NUM_O = 1
 
 # Codes for the automatic derivative sidedness
 DSIDE_AUTO = 0x0
-DSIDE_POS  = 0x1
-DSIDE_NEG  = 0x2
-DSIDE_TWO  = 0x3
+DSIDE_POS = 0x1
+DSIDE_NEG = 0x2
+DSIDE_TWO = 0x3
 
 _dside_names = {
-    'auto': DSIDE_AUTO,
-    'pos': DSIDE_POS,
-    'neg': DSIDE_NEG,
-    'two': DSIDE_TWO,
+    "auto": DSIDE_AUTO,
+    "pos": DSIDE_POS,
+    "neg": DSIDE_NEG,
+    "two": DSIDE_TWO,
 }
 
 
 anynotfinite = lambda x: not np.all(np.isfinite(x))
 
 # Euclidean norm-calculating functions. The naive implementation is
 # fast but can be sensitive to under/overflows. The "mpfit_careful"
 # version is slower but tries to be more robust. The "minpack"
 # version, which does indeed emulate the MINPACK implementation, also
 # tries to be careful. I've used this last implementation a little
 # bit but haven't compared it to the others thoroughly.
 
 enorm_fast = lambda v, finfo: np.sqrt(np.dot(v, v))
 
+
 def enorm_mpfit_careful(v, finfo):
     # "This is hopefully a compromise between speed and robustness.
     # Need to do this because of the possibility of over- or under-
     # flow."
 
     mx = max(abs(v.max()), abs(v.min()))
 
     if mx == 0:
-        return v[0] * 0. # preserve type (?)
+        return v[0] * 0.0  # preserve type (?)
     if not np.isfinite(mx):
-        raise ValueError('tried to compute norm of a vector with nonfinite values')
+        raise ValueError("tried to compute norm of a vector with nonfinite values")
     if mx > finfo.max / v.size or mx < finfo.tiny * v.size:
         return mx * np.sqrt(np.dot(v / mx, v / mx))
 
     return np.sqrt(np.dot(v, v))
 
 
 def enorm_minpack(v, finfo):
     rdwarf = 3.834e-20
     rgiant = 1.304e19
     agiant = rgiant / v.size
 
-    s1 = s2 = s3 = x1max = x3max = 0.
+    s1 = s2 = s3 = x1max = x3max = 0.0
 
     for i in range(v.size):
         xabs = abs(v[i])
 
         if xabs > rdwarf and xabs < agiant:
             s2 += xabs**2
         elif xabs <= rdwarf:
             if xabs <= x3max:
-                if xabs != 0.:
-                    s3 += (xabs / x3max)**2
+                if xabs != 0.0:
+                    s3 += (xabs / x3max) ** 2
             else:
-                s3 = 1 + s3 * (x3max / xabs)**2
+                s3 = 1 + s3 * (x3max / xabs) ** 2
                 x3max = xabs
         else:
             if xabs <= x1max:
-                s1 += (xabs / x1max)**2
+                s1 += (xabs / x1max) ** 2
             else:
-                s1 = 1. + s1 * (x1max / xabs)**2
+                s1 = 1.0 + s1 * (x1max / xabs) ** 2
                 x1max = xabs
 
-    if s1 != 0.:
+    if s1 != 0.0:
         return x1max * np.sqrt(s1 + (s2 / x1max) / x1max)
 
-    if s2 == 0.:
+    if s2 == 0.0:
         return x3max * np.sqrt(s3)
 
     if s2 >= x3max:
         return np.sqrt(s2 * (1 + (x3max / s2) * (x3max * s3)))
 
     return np.sqrt(x3max * ((s2 / x3max) + (x3max * s3)))
 
 
 # Q-R factorization.
 
+
 def _qr_factor_packed(a, enorm, finfo):
     """Compute the packed pivoting Q-R factorization of a matrix.
 
-Parameters:
-a     - An n-by-m matrix, m >= n. This will be *overwritten*
-        by this function as described below!
-enorm - A Euclidian-norm-computing function.
-finfo - A Numpy finfo object.
-
-Returns:
-pmut   - An n-element permutation vector
-rdiag  - An n-element vector of the diagonal of R
-acnorm - An n-element vector of the norms of the rows
-         of the input matrix 'a'.
-
-Computes the transposed Q-R factorization of the matrix 'a', with
-pivoting, in a packed form, in-place. The packed information can be
-used to construct matrices Q and R such that
-
-  A P = R Q or, in Python,
-  np.dot(r, q) = a[pmut]
-
-where q is m-by-m and q q^T = ident and r is n-by-m and is lower
-triangular. The function _qr_factor_full can compute these
-matrices. The packed form of output is all that is used by the main LM
-fitting algorithm.
-
-"Pivoting" refers to permuting the rows of 'a' to have their norms in
-nonincreasing order. The return value 'pmut' maps the unpermuted rows
-of 'a' to permuted rows. That is, the norms of the rows of a[pmut] are
-in nonincreasing order.
-
-The parameter 'a' is overwritten by this function. Its new value
-should still be interpreted as an n-by-m array. It comes in two
-parts. Its strict lower triangular part contains the struct lower
-triangular part of R. (The diagonal of R is returned in 'rdiag' and
-the strict upper trapezoidal part of R is zero.) The upper trapezoidal
-part of 'a' contains Q as factorized into a series of Householder
-transformation vectors. Q can be reconstructed as the matrix product
-of n Householder matrices, where the i'th Householder matrix is
-defined by
-
-H_i = I - 2 (v^T v) / (v v^T)
-
-where 'v' is the pmut[i]'th row of 'a' with its strict lower
-triangular part set to zero. See _qr_factor_full for more information.
-
-'rdiag' contains the diagonal part of the R matrix, taking into
-account the permutation of 'a'. The strict lower triangular part of R
-is stored in 'a' *with permutation*, so that the i'th row of R has
-rdiag[i] as its diagonal and a[pmut[i],:i] as its upper part. See
-_qr_factor_full for more information.
+    Parameters:
+    a     - An n-by-m matrix, m >= n. This will be *overwritten*
+            by this function as described below!
+    enorm - A Euclidian-norm-computing function.
+    finfo - A Numpy finfo object.
+
+    Returns:
+    pmut   - An n-element permutation vector
+    rdiag  - An n-element vector of the diagonal of R
+    acnorm - An n-element vector of the norms of the rows
+             of the input matrix 'a'.
+
+    Computes the transposed Q-R factorization of the matrix 'a', with
+    pivoting, in a packed form, in-place. The packed information can be
+    used to construct matrices Q and R such that
+
+      A P = R Q or, in Python,
+      np.dot(r, q) = a[pmut]
+
+    where q is m-by-m and q q^T = ident and r is n-by-m and is lower
+    triangular. The function _qr_factor_full can compute these
+    matrices. The packed form of output is all that is used by the main LM
+    fitting algorithm.
+
+    "Pivoting" refers to permuting the rows of 'a' to have their norms in
+    nonincreasing order. The return value 'pmut' maps the unpermuted rows
+    of 'a' to permuted rows. That is, the norms of the rows of a[pmut] are
+    in nonincreasing order.
+
+    The parameter 'a' is overwritten by this function. Its new value
+    should still be interpreted as an n-by-m array. It comes in two
+    parts. Its strict lower triangular part contains the struct lower
+    triangular part of R. (The diagonal of R is returned in 'rdiag' and
+    the strict upper trapezoidal part of R is zero.) The upper trapezoidal
+    part of 'a' contains Q as factorized into a series of Householder
+    transformation vectors. Q can be reconstructed as the matrix product
+    of n Householder matrices, where the i'th Householder matrix is
+    defined by
+
+    H_i = I - 2 (v^T v) / (v v^T)
+
+    where 'v' is the pmut[i]'th row of 'a' with its strict lower
+    triangular part set to zero. See _qr_factor_full for more information.
+
+    'rdiag' contains the diagonal part of the R matrix, taking into
+    account the permutation of 'a'. The strict lower triangular part of R
+    is stored in 'a' *with permutation*, so that the i'th row of R has
+    rdiag[i] as its diagonal and a[pmut[i],:i] as its upper part. See
+    _qr_factor_full for more information.
 
-'acnorm' contains the norms of the rows of the original input
-matrix 'a' without permutation.
+    'acnorm' contains the norms of the rows of the original input
+    matrix 'a' without permutation.
 
-The form of this transformation and the method of pivoting first
-appeared in Linpack."""
+    The form of this transformation and the method of pivoting first
+    appeared in Linpack."""
 
     machep = finfo.eps
     n, m = a.shape
 
     if m < n:
         raise ValueError('"a" must be at least as tall as it is wide')
 
@@ -442,97 +447,95 @@
             temp = a[i].copy()
             a[i] = a[kmax]
             a[kmax] = temp
 
         # Compute the Householder transformation to reduce the i'th
         # row of A to a multiple of the i'th unit vector.
 
-        ainorm = enorm(a[i,i:], finfo)
+        ainorm = enorm(a[i, i:], finfo)
 
         if ainorm == 0:
             rdiag[i] = 0
             continue
 
-        if a[i,i] < 0:
+        if a[i, i] < 0:
             # Doing this apparently improves FP precision somehow.
             ainorm = -ainorm
 
-        a[i,i:] /= ainorm
-        a[i,i] += 1
+        a[i, i:] /= ainorm
+        a[i, i] += 1
 
         # Apply the transformation to the remaining rows and update
         # the norms.
 
         for j in range(i + 1, n):
-            a[j,i:] -= a[i,i:] * np.dot(a[i,i:], a[j,i:]) / a[i,i]
+            a[j, i:] -= a[i, i:] * np.dot(a[i, i:], a[j, i:]) / a[i, i]
 
             if rdiag[j] != 0:
-                rdiag[j] *= np.sqrt(max(1 - (a[j,i] / rdiag[j])**2, 0))
+                rdiag[j] *= np.sqrt(max(1 - (a[j, i] / rdiag[j]) ** 2, 0))
 
-                if 0.05 * (rdiag[j] / wa[j])**2 <= machep:
+                if 0.05 * (rdiag[j] / wa[j]) ** 2 <= machep:
                     # What does this do???
-                    wa[j] = rdiag[j] = enorm(a[j,i+1:], finfo)
+                    wa[j] = rdiag[j] = enorm(a[j, i + 1 :], finfo)
 
         rdiag[i] = -ainorm
 
     return pmut, rdiag, acnorm
 
 
 def _manual_qr_factor_packed(a, dtype=float):
     # This testing function gives sensible defaults to _qr_factor_packed
     # and makes a copy of its input to make comparisons easier.
 
     a = np.array(a, dtype)
-    pmut, rdiag, acnorm = _qr_factor_packed(a, enorm_mpfit_careful,
-                                            np.finfo(dtype))
+    pmut, rdiag, acnorm = _qr_factor_packed(a, enorm_mpfit_careful, np.finfo(dtype))
     return a, pmut, rdiag, acnorm
 
 
 def _qr_factor_full(a, dtype=float):
     """Compute the QR factorization of a matrix, with pivoting.
 
-Parameters:
-a     - An n-by-m arraylike, m >= n.
-dtype - (optional) The data type to use for computations.
-        Default is float.
-
-Returns:
-q    - An m-by-m orthogonal matrix (q q^T = ident)
-r    - An n-by-m upper triangular matrix
-pmut - An n-element permutation vector
-
-The returned values will satisfy the equation
-
-np.dot(r, q) == a[:,pmut]
-
-The outputs are computed indirectly via the function
-_qr_factor_packed. If you need to compute q and r matrices in
-production code, there are faster ways to do it. This function is for
-testing _qr_factor_packed.
-
-The permutation vector pmut is a vector of the integers 0 through
-n-1. It sorts the rows of 'a' by their norms, so that the
-pmut[i]'th row of 'a' has the i'th biggest norm."""
+    Parameters:
+    a     - An n-by-m arraylike, m >= n.
+    dtype - (optional) The data type to use for computations.
+            Default is float.
+
+    Returns:
+    q    - An m-by-m orthogonal matrix (q q^T = ident)
+    r    - An n-by-m upper triangular matrix
+    pmut - An n-element permutation vector
+
+    The returned values will satisfy the equation
+
+    np.dot(r, q) == a[:,pmut]
+
+    The outputs are computed indirectly via the function
+    _qr_factor_packed. If you need to compute q and r matrices in
+    production code, there are faster ways to do it. This function is for
+    testing _qr_factor_packed.
+
+    The permutation vector pmut is a vector of the integers 0 through
+    n-1. It sorts the rows of 'a' by their norms, so that the
+    pmut[i]'th row of 'a' has the i'th biggest norm."""
 
     n, m = a.shape
 
     # Compute the packed Q and R matrix information.
 
-    packed, pmut, rdiag, acnorm = \
-        _manual_qr_factor_packed(a, dtype)
+    packed, pmut, rdiag, acnorm = _manual_qr_factor_packed(a, dtype)
 
     # Now we unpack. Start with the R matrix, which is easy: we just
     # have to piece it together from the strict lower triangle of 'a'
     # and the diagonal in 'rdiag'.
 
     r = np.zeros((n, m))
 
     for i in range(n):
-        r[i,:i] = packed[i,:i]
-        r[i,i] = rdiag[i]
+        r[i, :i] = packed[i, :i]
+        r[i, i] = rdiag[i]
 
     # Now the Q matrix. It is the concatenation of n Householder
     # transformations, each of which is defined by a row in the upper
     # trapezoidal portion of 'a'. We extract the appropriate vector,
     # construct the matrix for the Householder transform, and build up
     # the Q matrix.
 
@@ -550,200 +553,201 @@
 
 
 @test
 def _qr_examples():
     # This is the sample given in the comments of Craig Markwardt's
     # IDL MPFIT implementation.
 
-    a = np.asarray([[9., 2, 6], [4, 8, 7]])
+    a = np.asarray([[9.0, 2, 6], [4, 8, 7]])
     packed, pmut, rdiag, acnorm = _manual_qr_factor_packed(a)
 
-    Taaae(packed, [[1.35218036, 0.70436073, 0.61631563],
-                   [-8.27623852, 1.96596229, 0.25868293]])
+    Taaae(
+        packed,
+        [[1.35218036, 0.70436073, 0.61631563], [-8.27623852, 1.96596229, 0.25868293]],
+    )
     assert pmut[0] == 1
     assert pmut[1] == 0
     Taaae(rdiag, [-11.35781669, 7.24595584])
     Taaae(acnorm, [11.0, 11.35781669])
 
     q, r, pmut = _qr_factor_full(a)
     Taaae(np.dot(r, q), a[pmut])
 
     # This is the sample given in Wikipedia. I know, shameful!
 
-    a = np.asarray([[12., 6, -4],
-                    [-51, 167, 24],
-                    [4, -68, -41]])
+    a = np.asarray([[12.0, 6, -4], [-51, 167, 24], [4, -68, -41]])
     packed, pmut, rdiag, acnorm = _manual_qr_factor_packed(a)
-    Taaae(packed, [[ 1.28935268, -0.94748818, -0.13616597],
-                   [-71.16941178,  1.36009392, 0.93291606],
-                   [1.66803309, -2.18085468, 2.]])
+    Taaae(
+        packed,
+        [
+            [1.28935268, -0.94748818, -0.13616597],
+            [-71.16941178, 1.36009392, 0.93291606],
+            [1.66803309, -2.18085468, 2.0],
+        ],
+    )
     assert pmut[0] == 1
     assert pmut[1] == 2
     assert pmut[2] == 0
     Taaae(rdiag, [176.25549637, 35.43888862, 13.72812946])
-    Taaae(acnorm, [14., 176.25549637, 79.50471684])
+    Taaae(acnorm, [14.0, 176.25549637, 79.50471684])
 
     q, r, pmut = _qr_factor_full(a)
     Taaae(np.dot(r, q), a[pmut])
 
     # A sample I constructed myself analytically. I made the Q
     # from rotation matrices and chose R pretty dumbly to get a
     # nice-ish matrix following the columnar norm constraint.
 
     r3 = np.sqrt(3)
-    a = np.asarray([[-3 * r3, 7, -2],
-                    [3 * r3, 9, -6]])
+    a = np.asarray([[-3 * r3, 7, -2], [3 * r3, 9, -6]])
     q, r, pmut = _qr_factor_full(a)
 
-    r *= np.sign(q[0,0])
+    r *= np.sign(q[0, 0])
     for i in range(3):
         # Normalize signs.
-        q[i] *= (-1)**i * np.sign(q[i,0])
+        q[i] *= (-1) ** i * np.sign(q[i, 0])
 
     assert pmut[0] == 1
     assert pmut[1] == 0
 
-    Taaae(q, 0.25 * np.asarray([[r3, 3, -2],
-                                [-2*r3, 2, 0],
-                                [1, r3, 2*r3]]))
-    Taaae(r, np.asarray([[12, 0, 0],
-                         [4, 8, 0]]))
+    Taaae(q, 0.25 * np.asarray([[r3, 3, -2], [-2 * r3, 2, 0], [1, r3, 2 * r3]]))
+    Taaae(r, np.asarray([[12, 0, 0], [4, 8, 0]]))
     Taaae(np.dot(r, q), a[pmut])
 
 
 # QR solution.
 
+
 def _qrd_solve(r, pmut, ddiag, bqt, sdiag):
     """Solve an equation given a QR factored matrix and a diagonal.
 
-Parameters:
-r     - **input-output** n-by-n array. The full lower triangle contains
-        the full lower triangle of R. On output, the strict upper
-        triangle contains the transpose of the strict lower triangle of
-        S.
-pmut  - n-vector describing the permutation matrix P.
-ddiag - n-vector containing the diagonal of the matrix D in the base
-        problem (see below).
-bqt   - n-vector containing the first n elements of B Q^T.
-sdiag - output n-vector. It is filled with the diagonal of S. Should
-        be preallocated by the caller -- can result in somewhat greater
-        efficiency if the vector is reused from one call to the next.
-
-Returns:
-x     - n-vector solving the equation.
-
-Compute the n-vector x such that
-
-A^T x = B, D x = 0
-
-where A is an n-by-m matrix, B is an m-vector, and D is an n-by-n
-diagonal matrix. We are given information about pivoted QR
-factorization of A with permutation, such that
-
-A P = R Q
-
-where P is a permutation matrix, Q has orthogonal rows, and R is lower
-triangular with nonincreasing diagonal elements. Q is m-by-m, R is
-n-by-m, and P is n-by-n. If x = P z, then we need to solve
-
-R z = B Q^T,
-P^T D P z = 0 (why the P^T? and do these need to be updated for the transposition?)
-
-If the system is rank-deficient, these equations are solved as well as
-possible in a least-squares sense. For the purposes of the LM
-algorithm we also compute the lower triangular n-by-n matrix S such
-that
+    Parameters:
+    r     - **input-output** n-by-n array. The full lower triangle contains
+            the full lower triangle of R. On output, the strict upper
+            triangle contains the transpose of the strict lower triangle of
+            S.
+    pmut  - n-vector describing the permutation matrix P.
+    ddiag - n-vector containing the diagonal of the matrix D in the base
+            problem (see below).
+    bqt   - n-vector containing the first n elements of B Q^T.
+    sdiag - output n-vector. It is filled with the diagonal of S. Should
+            be preallocated by the caller -- can result in somewhat greater
+            efficiency if the vector is reused from one call to the next.
+
+    Returns:
+    x     - n-vector solving the equation.
+
+    Compute the n-vector x such that
+
+    A^T x = B, D x = 0
+
+    where A is an n-by-m matrix, B is an m-vector, and D is an n-by-n
+    diagonal matrix. We are given information about pivoted QR
+    factorization of A with permutation, such that
+
+    A P = R Q
+
+    where P is a permutation matrix, Q has orthogonal rows, and R is lower
+    triangular with nonincreasing diagonal elements. Q is m-by-m, R is
+    n-by-m, and P is n-by-n. If x = P z, then we need to solve
+
+    R z = B Q^T,
+    P^T D P z = 0 (why the P^T? and do these need to be updated for the transposition?)
+
+    If the system is rank-deficient, these equations are solved as well as
+    possible in a least-squares sense. For the purposes of the LM
+    algorithm we also compute the lower triangular n-by-n matrix S such
+    that
 
-P^T (A^T A + D D) P = S^T S. (transpose?)
-"""
+    P^T (A^T A + D D) P = S^T S. (transpose?)"""
 
     n, m = r.shape
 
     # "Copy r and bqt to preserve input and initialize s.  In
     # particular, save the diagonal elements of r in x."  Recall that
     # on input only the full lower triangle of R is meaningful, so we
     # can mirror that into the upper triangle without issues.
 
     for i in range(n):
-        r[i,i:] = r[i:,i]
+        r[i, i:] = r[i:, i]
 
     x = r.diagonal().copy()
     zwork = bqt.copy()
 
     # "Eliminate the diagonal matrix d using a Givens rotation."
 
     for i in range(n):
         # "Prepare the row of D to be eliminated, locating the
         # diagonal element using P from the QR factorization."
 
         li = pmut[i]
         if ddiag[li] == 0:
-            sdiag[i] = r[i,i]
-            r[i,i] = x[i]
+            sdiag[i] = r[i, i]
+            r[i, i] = x[i]
             continue
 
         sdiag[i:] = 0
         sdiag[i] = ddiag[li]
 
         # "The transformations to eliminate the row of d modify only a
         # single element of (q transpose)*b beyond the first n, which
         # is initially zero."
 
-        bqtpi = 0.
+        bqtpi = 0.0
 
         for j in range(i, n):
             # "Determine a Givens rotation which eliminates the
             # appropriate element in the current row of D."
 
             if sdiag[j] == 0:
                 continue
 
-            if abs(r[j,j]) < abs(sdiag[j]):
-                cot = r[j,j] / sdiag[j]
+            if abs(r[j, j]) < abs(sdiag[j]):
+                cot = r[j, j] / sdiag[j]
                 sin = 0.5 / np.sqrt(0.25 + 0.25 * cot**2)
                 cos = sin * cot
             else:
-                tan = sdiag[j] / r[j,j]
+                tan = sdiag[j] / r[j, j]
                 cos = 0.5 / np.sqrt(0.25 + 0.25 * tan**2)
                 sin = cos * tan
 
             # "Compute the modified diagonal element of r and the
             # modified element of ((q transpose)*b,0)."
-            r[j,j] = cos * r[j,j] + sin * sdiag[j]
+            r[j, j] = cos * r[j, j] + sin * sdiag[j]
             temp = cos * zwork[j] + sin * bqtpi
             bqtpi = -sin * zwork[j] + cos * bqtpi
             zwork[j] = temp
 
             # "Accumulate the transformation in the row of s."
             if j + 1 < n:
-                temp = cos * r[j,j+1:] + sin * sdiag[j+1:]
-                sdiag[j+1:] = -sin * r[j,j+1:] + cos * sdiag[j+1:]
-                r[j,j+1:] = temp
+                temp = cos * r[j, j + 1 :] + sin * sdiag[j + 1 :]
+                sdiag[j + 1 :] = -sin * r[j, j + 1 :] + cos * sdiag[j + 1 :]
+                r[j, j + 1 :] = temp
 
         # Save the diagonal of S and restore the diagonal of R
         # from its saved location in x.
-        sdiag[i] = r[i,i]
-        r[i,i] = x[i]
+        sdiag[i] = r[i, i]
+        r[i, i] = x[i]
 
     # "Solve the triangular system for z.  If the system is singular
     # then obtain a least squares solution."
 
     nsing = n
 
     for i in range(n):
-        if sdiag[i] == 0.:
+        if sdiag[i] == 0.0:
             nsing = i
             zwork[i:] = 0
             break
 
     if nsing > 0:
-        zwork[nsing-1] /= sdiag[nsing-1] # Degenerate case
+        zwork[nsing - 1] /= sdiag[nsing - 1]  # Degenerate case
         # "Reverse loop"
         for i in range(nsing - 2, -1, -1):
-            s = np.dot(zwork[i+1:nsing], r[i,i+1:nsing])
+            s = np.dot(zwork[i + 1 : nsing], r[i, i + 1 : nsing])
             zwork[i] = (zwork[i] - s) / sdiag[i]
 
     # "Permute the components of z back to components of x."
     x[pmut] = zwork
     return x
 
 
@@ -761,168 +765,166 @@
     if not build_s:
         return x, swork, sdiag
 
     # Rebuild s.
 
     swork = swork.T
     for i in range(r.shape[1]):
-        swork[i,i:] = 0
-        swork[i,i] = sdiag[i]
+        swork[i, i:] = 0
+        swork[i, i] = sdiag[i]
 
     return x, swork
 
 
 def _qrd_solve_full(a, b, ddiag, dtype=float):
     """Solve the equation A^T x = B, D x = 0.
 
-Parameters:
-a     - an n-by-m array, m >= n
-b     - an m-vector
-ddiag - an n-vector giving the diagonal of D. (The rest of D is 0.)
-
-Returns:
-x    - n-vector solving the equation.
-s    - the n-by-n supplementary matrix s.
-pmut - n-element permutation vector defining the permutation matrix P.
-
-The equations are solved in a least-squares sense if the system is
-rank-deficient.  D is a diagonal matrix and hence only its diagonal is
-in fact supplied as an argument. The matrix s is full lower triangular
-and solves the equation
-
-P^T (A A^T + D D) P = S^T S (needs transposition?)
-
-where P is the permutation matrix defined by the vector pmut; it puts
-the rows of 'a' in order of nonincreasing rank, so that a[pmut]
-has its rows sorted that way.
-"""
+    Parameters:
+    a     - an n-by-m array, m >= n
+    b     - an m-vector
+    ddiag - an n-vector giving the diagonal of D. (The rest of D is 0.)
+
+    Returns:
+    x    - n-vector solving the equation.
+    s    - the n-by-n supplementary matrix s.
+    pmut - n-element permutation vector defining the permutation matrix P.
+
+    The equations are solved in a least-squares sense if the system is
+    rank-deficient.  D is a diagonal matrix and hence only its diagonal is
+    in fact supplied as an argument. The matrix s is full lower triangular
+    and solves the equation
+
+    P^T (A A^T + D D) P = S^T S (needs transposition?)
+
+    where P is the permutation matrix defined by the vector pmut; it puts
+    the rows of 'a' in order of nonincreasing rank, so that a[pmut]
+    has its rows sorted that way."""
 
     a = np.asarray(a, dtype)
     b = np.asarray(b, dtype)
     ddiag = np.asarray(ddiag, dtype)
 
     n, m = a.shape
     assert m >= n
-    assert b.shape == (m, )
-    assert ddiag.shape == (n, )
+    assert b.shape == (m,)
+    assert ddiag.shape == (n,)
 
     # The computation is straightforward.
 
     q, r, pmut = _qr_factor_full(a)
     bqt = np.dot(b, q.T)
-    x, s = _manual_qrd_solve(r[:,:n], pmut, ddiag, bqt,
-                             dtype=dtype, build_s=True)
+    x, s = _manual_qrd_solve(r[:, :n], pmut, ddiag, bqt, dtype=dtype, build_s=True)
 
     return x, s, pmut
 
 
 @test
 def _qrd_solve_alone():
     # Testing out just the QR solution function without
     # also the QR factorization bits.
 
     # The very simplest case.
     r = np.eye(2)
     pmut = np.asarray([0, 1])
-    diag = np.asarray([0., 0])
-    bqt = np.asarray([3., 5])
+    diag = np.asarray([0.0, 0])
+    bqt = np.asarray([3.0, 5])
     x, s = _manual_qrd_solve(r, pmut, diag, bqt, build_s=True)
-    Taaae(x, [3., 5])
+    Taaae(x, [3.0, 5])
     Taaae(s, np.eye(2))
 
     # Now throw in a diagonal matrix ...
-    diag = np.asarray([2., 3.])
+    diag = np.asarray([2.0, 3.0])
     x, s = _manual_qrd_solve(r, pmut, diag, bqt, build_s=True)
     Taaae(x, [0.6, 0.5])
     Taaae(s, np.sqrt(np.diag([5, 10])))
 
     # And a permutation. We permute A but maintain
     # B, effectively saying x1 = 5, x2 = 3, so
     # we need to permute diag as well to scale them
     # by the amounts that yield nice X values.
     pmut = np.asarray([1, 0])
-    diag = np.asarray([3., 2.])
+    diag = np.asarray([3.0, 2.0])
     x, s = _manual_qrd_solve(r, pmut, diag, bqt, build_s=True)
     Taaae(x, [0.5, 0.6])
     Taaae(s, np.sqrt(np.diag([5, 10])))
 
 
 # Calculation of the Levenberg-Marquardt parameter
 
+
 def _lm_solve(r, pmut, ddiag, bqt, delta, par0, enorm, finfo):
     """Compute the Levenberg-Marquardt parameter and solution vector.
 
-Parameters:
-r     - IN/OUT n-by-m matrix, m >= n. On input, the full lower triangle is
-        the full lower  triangle of R and the strict upper triangle is
-        ignored.  On output, the strict upper triangle has been
-        obliterated. The value of 'm' here is not relevant so long as it
-        is at least n.
-pmut  - n-vector, defines permutation of R
-ddiag - n-vector, diagonal elements of D
-bqt   - n-vector, first elements of B Q^T
-delta - positive scalar, specifies scale of enorm(Dx)
-par0  - positive scalar, initial estimate of the LM parameter
-enorm - norm-computing function
-finfo - info about chosen floating-point representation
-
-Returns:
-par   - positive scalar, final estimate of LM parameter
-x     - n-vector, least-squares solution of LM equation (see below)
-
-This routine computes the Levenberg-Marquardt parameter 'par' and a LM
-solution vector 'x'. Given an n-by-n matrix A, an n-by-n nonsingular
-diagonal matrix D, an m-vector B, and a positive number delta, the
-problem is to determine values such that 'x' is the least-squares
-solution to
-
- A x = B
- sqrt(par) * D x = 0
-
-and either
-
- (1) par = 0, dxnorm - delta <= 0.1 delta or
- (2) par > 0 and |dxnorm - delta| <= 0.1 delta
-
-where dxnorm = enorm(D x).
-
-This routine is not given A, B, or D directly. If we define the
-column-pivoted transposed QR factorization of A such that
-
- A P = R Q
-
-where P is a permutation matrix, Q has orthogonal rows, and R is a
-lower triangular matrix with diagonal elements of nonincreasing
-magnitude, this routine is given the full lower triangle of R, a
-vector defining P ('pmut'), and the first n components of B Q^T
-('bqt'). These values are essentially passed verbatim to _qrd_solve().
+    Parameters:
+    r     - IN/OUT n-by-m matrix, m >= n. On input, the full lower triangle is
+            the full lower  triangle of R and the strict upper triangle is
+            ignored.  On output, the strict upper triangle has been
+            obliterated. The value of 'm' here is not relevant so long as it
+            is at least n.
+    pmut  - n-vector, defines permutation of R
+    ddiag - n-vector, diagonal elements of D
+    bqt   - n-vector, first elements of B Q^T
+    delta - positive scalar, specifies scale of enorm(Dx)
+    par0  - positive scalar, initial estimate of the LM parameter
+    enorm - norm-computing function
+    finfo - info about chosen floating-point representation
+
+    Returns:
+    par   - positive scalar, final estimate of LM parameter
+    x     - n-vector, least-squares solution of LM equation (see below)
+
+    This routine computes the Levenberg-Marquardt parameter 'par' and a LM
+    solution vector 'x'. Given an n-by-n matrix A, an n-by-n nonsingular
+    diagonal matrix D, an m-vector B, and a positive number delta, the
+    problem is to determine values such that 'x' is the least-squares
+    solution to
+
+     A x = B
+     sqrt(par) * D x = 0
+
+    and either
+
+     (1) par = 0, dxnorm - delta <= 0.1 delta or
+     (2) par > 0 and |dxnorm - delta| <= 0.1 delta
+
+    where dxnorm = enorm(D x).
+
+    This routine is not given A, B, or D directly. If we define the
+    column-pivoted transposed QR factorization of A such that
+
+     A P = R Q
+
+    where P is a permutation matrix, Q has orthogonal rows, and R is a
+    lower triangular matrix with diagonal elements of nonincreasing
+    magnitude, this routine is given the full lower triangle of R, a
+    vector defining P ('pmut'), and the first n components of B Q^T
+    ('bqt'). These values are essentially passed verbatim to _qrd_solve().
 
-This routine iterates to estimate par. Usually only a few iterations
-are needed, but no more than 10 are performed.
-"""
+    This routine iterates to estimate par. Usually only a few iterations
+    are needed, but no more than 10 are performed."""
     dwarf = finfo.tiny
     n, m = r.shape
     x = np.empty_like(bqt)
     sdiag = np.empty_like(bqt)
 
     # "Compute and store x in the Gauss-Newton direction. If the
     # Jacobian is rank-deficient, obtain a least-squares solution."
 
     nnonsingular = n
     wa1 = bqt.copy()
 
     for i in range(n):
-        if r[i,i] == 0:
+        if r[i, i] == 0:
             nnonsingular = i
             wa1[i:] = 0
             break
 
     for j in range(nnonsingular - 1, -1, -1):
-        wa1[j] /= r[j,j]
-        wa1[:j] -= r[j,:j] * wa1[j]
+        wa1[j] /= r[j, j]
+        wa1[:j] -= r[j, :j] * wa1[j]
 
     x[pmut] = wa1
 
     # Initial function evaluation. Check if the Gauss-Newton direction
     # was good enough.
 
     wa2 = ddiag * x
@@ -931,30 +933,30 @@
 
     if normdiff <= 0.1 * delta:
         return 0, x
 
     # If the Jacobian is not rank deficient, the Newton step provides
     # a lower bound for the zero of the function.
 
-    par_lower = 0.
+    par_lower = 0.0
 
     if nnonsingular == n:
         wa1 = ddiag[pmut] * wa2[pmut] / dxnorm
-        wa1[0] /= r[0,0] # "Degenerate case"
+        wa1[0] /= r[0, 0]  # "Degenerate case"
 
         for j in range(1, n):
-            wa1[j] = (wa1[j] - np.dot(wa1[:j], r[j,:j])) / r[j,j]
+            wa1[j] = (wa1[j] - np.dot(wa1[:j], r[j, :j])) / r[j, j]
 
         temp = enorm(wa1, finfo)
         par_lower = normdiff / delta / temp**2
 
     # We can always find an upper bound.
 
     for j in range(n):
-        wa1[j] = np.dot(bqt[:j+1], r[j,:j+1]) / ddiag[pmut[j]]
+        wa1[j] = np.dot(bqt[: j + 1], r[j, : j + 1]) / ddiag[pmut[j]]
 
     gnorm = enorm(wa1, finfo)
     par_upper = gnorm / delta
     if par_upper == 0:
         par_upper = dwarf / min(delta, 0.1)
 
     # Now iterate our way to victory.
@@ -969,205 +971,205 @@
         itercount += 1
 
         if par == 0:
             par = max(dwarf, par_upper * 0.001)
 
         temp = np.sqrt(par)
         wa1 = temp * ddiag
-        x = _qrd_solve(r[:,:n], pmut, wa1, bqt, sdiag) # sdiag is an output arg here
+        x = _qrd_solve(r[:, :n], pmut, wa1, bqt, sdiag)  # sdiag is an output arg here
         wa2 = ddiag * x
         dxnorm = enorm(wa2, finfo)
         olddiff = normdiff
         normdiff = dxnorm - delta
 
         if abs(normdiff) < 0.1 * delta:
-            break # converged
+            break  # converged
         if par_lower == 0 and normdiff <= olddiff and olddiff < 0:
-            break # overshot, I guess?
+            break  # overshot, I guess?
         if itercount == 10:
-            break # this is taking too long
+            break  # this is taking too long
 
         # Compute and apply the Newton correction
 
         wa1 = ddiag[pmut] * wa2[pmut] / dxnorm
 
         for j in range(n - 1):
             wa1[j] /= sdiag[j]
-            wa1[j+1:n] -= r[j,j+1:n] * wa1[j]
-        wa1[n-1] /= sdiag[n-1] # degenerate case
+            wa1[j + 1 : n] -= r[j, j + 1 : n] * wa1[j]
+        wa1[n - 1] /= sdiag[n - 1]  # degenerate case
 
-        par_delta = normdiff / delta / enorm(wa1, finfo)**2
+        par_delta = normdiff / delta / enorm(wa1, finfo) ** 2
 
         if normdiff > 0:
             par_lower = max(par_lower, par)
         elif normdiff < 0:
             par_upper = min(par_upper, par)
 
         par = max(par_lower, par + par_delta)
 
     return par, x
 
 
 def _lm_solve_full(a, b, ddiag, delta, par0, dtype=float):
     """Compute the Levenberg-Marquardt parameter and solution vector.
 
-Parameters:
-a     - n-by-m matrix, m >= n (only the n-by-n component is used)
-b     - n-by-n matrix
-ddiag - n-vector, diagonal elements of D
-delta - positive scalar, specifies scale of enorm(Dx)
-par0  - positive scalar, initial estimate of the LM parameter
-
-Returns:
-par    - positive scalar, final estimate of LM parameter
-x      - n-vector, least-squares solution of LM equation
-dxnorm - positive scalar, enorm(D x)
-relnormdiff - scalar, (dxnorm - delta) / delta, maybe abs-ified
-
-This routine computes the Levenberg-Marquardt parameter 'par' and a LM
-solution vector 'x'. Given an n-by-n matrix A, an n-by-n nonsingular
-diagonal matrix D, an m-vector B, and a positive number delta, the
-problem is to determine values such that 'x' is the least-squares
-solution to
-
- A x = B
- sqrt(par) * D x = 0
+    Parameters:
+    a     - n-by-m matrix, m >= n (only the n-by-n component is used)
+    b     - n-by-n matrix
+    ddiag - n-vector, diagonal elements of D
+    delta - positive scalar, specifies scale of enorm(Dx)
+    par0  - positive scalar, initial estimate of the LM parameter
+
+    Returns:
+    par    - positive scalar, final estimate of LM parameter
+    x      - n-vector, least-squares solution of LM equation
+    dxnorm - positive scalar, enorm(D x)
+    relnormdiff - scalar, (dxnorm - delta) / delta, maybe abs-ified
+
+    This routine computes the Levenberg-Marquardt parameter 'par' and a LM
+    solution vector 'x'. Given an n-by-n matrix A, an n-by-n nonsingular
+    diagonal matrix D, an m-vector B, and a positive number delta, the
+    problem is to determine values such that 'x' is the least-squares
+    solution to
+
+     A x = B
+     sqrt(par) * D x = 0
 
-and either
+    and either
 
- (1) par = 0, dxnorm - delta <= 0.1 delta or
- (2) par > 0 and |dxnorm - delta| <= 0.1 delta
+     (1) par = 0, dxnorm - delta <= 0.1 delta or
+     (2) par > 0 and |dxnorm - delta| <= 0.1 delta
 
-where dxnorm = enorm(D x).
-"""
+    where dxnorm = enorm(D x)."""
     a = np.asarray(a, dtype)
     b = np.asarray(b, dtype)
     ddiag = np.asarray(ddiag, dtype)
 
     n, m = a.shape
     assert m >= n
-    assert b.shape == (m, )
-    assert ddiag.shape == (n, )
+    assert b.shape == (m,)
+    assert ddiag.shape == (n,)
 
     q, r, pmut = _qr_factor_full(a)
     bqt = np.dot(b, q.T)
-    par, x = _lm_solve(r, pmut, ddiag, bqt, delta, par0,
-                       enorm_mpfit_careful, np.finfo(dtype))
+    par, x = _lm_solve(
+        r, pmut, ddiag, bqt, delta, par0, enorm_mpfit_careful, np.finfo(dtype)
+    )
     dxnorm = enorm_mpfit_careful(ddiag * x, np.finfo(dtype))
     relnormdiff = (dxnorm - delta) / delta
 
     if par > 0:
         relnormdiff = abs(relnormdiff)
 
     return par, x, dxnorm, relnormdiff
 
 
 def _calc_covariance(r, pmut, tol=1e-14):
     """Calculate the covariance matrix of the fitted parameters
 
-Parameters:
-r    - n-by-n matrix, the full upper triangle of R
-pmut - n-vector, defines the permutation of R
-tol  - scalar, relative column scale for determining rank
-       deficiency. Default 1e-14.
-
-Returns:
-cov  - n-by-n matrix, the covariance matrix C
-
-Given an n-by-n matrix A, the corresponding covariance matrix
-is
-
-  C = inverse(A^T A)
-
-This routine is given information relating to the pivoted transposed
-QR factorization of A, which is defined by matrices such that
-
- A P = R Q
-
-where P is a permutation matrix, Q has orthogonal rows, and R is a
-lower triangular matrix with diagonal elements of nonincreasing
-magnitude. In particular we take the full lower triangle of R ('r')
-and a vector describing P ('pmut'). The covariance matrix is then
-
- C = P inverse(R^T R) P^T
-
-If A is nearly rank-deficient, it may be desirable to compute the
-covariance matrix corresponding to the linearly-independent columns of
-A. We use a tolerance, 'tol', to define the numerical rank of A. If j
-is the largest integer such that |R[j,j]| > tol*|R[0,0]|, then we
-compute the covariance matrix for the first j columns of R. For k > j,
-the corresponding covariance entries (pmut[k]) are set to zero.
-"""
+    Parameters:
+    r    - n-by-n matrix, the full upper triangle of R
+    pmut - n-vector, defines the permutation of R
+    tol  - scalar, relative column scale for determining rank
+           deficiency. Default 1e-14.
+
+    Returns:
+    cov  - n-by-n matrix, the covariance matrix C
+
+    Given an n-by-n matrix A, the corresponding covariance matrix
+    is
+
+      C = inverse(A^T A)
+
+    This routine is given information relating to the pivoted transposed
+    QR factorization of A, which is defined by matrices such that
+
+     A P = R Q
+
+    where P is a permutation matrix, Q has orthogonal rows, and R is a
+    lower triangular matrix with diagonal elements of nonincreasing
+    magnitude. In particular we take the full lower triangle of R ('r')
+    and a vector describing P ('pmut'). The covariance matrix is then
+
+     C = P inverse(R^T R) P^T
+
+    If A is nearly rank-deficient, it may be desirable to compute the
+    covariance matrix corresponding to the linearly-independent columns of
+    A. We use a tolerance, 'tol', to define the numerical rank of A. If j
+    is the largest integer such that |R[j,j]| > tol*|R[0,0]|, then we
+    compute the covariance matrix for the first j columns of R. For k > j,
+    the corresponding covariance entries (pmut[k]) are set to zero."""
     # This routine could save an allocation by operating on r in-place,
     # which might be worthwhile for large n, and is what the original
     # Fortran does.
 
     n = r.shape[1]
     assert r.shape[0] >= n
     r = r.copy()
 
     # Form the inverse of R in the full lower triangle of R.
 
     jrank = -1
-    abstol = tol * abs(r[0,0])
+    abstol = tol * abs(r[0, 0])
 
     for i in range(n):
-        if abs(r[i,i]) <= abstol:
+        if abs(r[i, i]) <= abstol:
             break
 
-        r[i,i] **= -1
+        r[i, i] **= -1
 
         for j in range(i):
-            temp = r[i,i] * r[i,j]
-            r[i,j] = 0.
-            r[i,:j+1] -= temp * r[j,:j+1]
+            temp = r[i, i] * r[i, j]
+            r[i, j] = 0.0
+            r[i, : j + 1] -= temp * r[j, : j + 1]
 
         jrank = i
 
     # Form the full lower triangle of the inverse(R^T R) in the full
     # lower triangle of R.
 
     for i in range(jrank + 1):
         for j in range(i):
-            r[j,:j+1] += r[i,j] * r[i,:j+1]
-        r[i,:i+1] *= r[i,i]
+            r[j, : j + 1] += r[i, j] * r[i, : j + 1]
+        r[i, : i + 1] *= r[i, i]
 
     # Form the full upper triangle of the covariance matrix in the
     # strict upper triangle of R and in wa.
 
     wa = np.empty(n)
-    wa.fill(r[0,0])
+    wa.fill(r[0, 0])
 
     for i in range(n):
         pi = pmut[i]
         sing = i > jrank
 
         for j in range(i + 1):
             if sing:
-                r[i,j] = 0.
+                r[i, j] = 0.0
 
             pj = pmut[j]
             if pj > pi:
-                r[pi,pj] = r[i,j]
+                r[pi, pj] = r[i, j]
             elif pj < pi:
-                r[pj,pi] = r[i,j]
+                r[pj, pi] = r[i, j]
 
-        wa[pi] = r[i,i]
+        wa[pi] = r[i, i]
 
     # Symmetrize.
 
     for i in range(n):
-        r[i,:i+1] = r[:i+1,i]
-        r[i,i] = wa[i]
+        r[i, : i + 1] = r[: i + 1, i]
+        r[i, i] = wa[i]
 
     return r
 
 
 # The actual user interface to the problem-solving machinery:
 
+
 class Solution(object):
     """A parameter solution from the Levenberg-Marquard algorithm. Attributes:
 
     ndof   - The number of degrees of freedom in the problem.
     prob   - The `Problem`.
     status - A set of strings indicating which stop condition(s) arose.
     niter  - The number of iterations needed to obtain the solution.
@@ -1179,14 +1181,15 @@
     fjac   - The final Jacobian.
     nfev   - The number of function evaluations needed to obtain the solution.
     njev   - The number of Jacobian evaluations needed to obtain the solution.
 
     The presence of 'ftol', 'gtol', or 'xtol' in `status` suggests success.
 
     """
+
     ndof = None
     prob = None
     status = None
     niter = None
     perror = None
     params = None
     covar = None
@@ -1257,14 +1260,15 @@
       Set the function to a standard model-fitting style.
     solve
       Run the algorithm.
     solve_scipy
       Run the algorithm using the Scipy implementation (for testing).
 
     """
+
     _yfunc = None
     _jfunc = None
     _npar = None
     _nout = None
 
     _pinfof = None
     _pinfoo = None
@@ -1277,274 +1281,264 @@
     # Public fields, settable by user at will
 
     solclass = None
 
     ftol = 1e-10
     xtol = 1e-10
     gtol = 1e-10
-    damp = 0.
-    factor = 100.
+    damp = 0.0
+    factor = 100.0
     epsilon = None
 
     maxiter = 200
     normfunc = None
 
     diag = None
 
     debug_calls = False
     debug_jac = False
 
-
-    def __init__(self, npar=None, nout=None, yfunc=None, jfunc=None,
-                  solclass=Solution):
+    def __init__(self, npar=None, nout=None, yfunc=None, jfunc=None, solclass=Solution):
         if npar is not None:
             self.set_npar(npar)
         if yfunc is not None:
             self.set_func(nout, yfunc, jfunc)
 
         if not issubclass(solclass, Solution):
-            raise ValueError('solclass')
+            raise ValueError("solclass")
 
         self.solclass = solclass
 
-
     # The parameters and their metadata -- can be configured without
     # setting nout or the functions.
 
     def set_npar(self, npar):
         try:
             npar = int(npar)
             assert npar > 0
         except Exception:
-            raise ValueError('npar must be a positive integer')
+            raise ValueError("npar must be a positive integer")
 
         if self._npar is not None and self._npar == npar:
             return self
 
         newinfof = p = np.ndarray((PI_NUM_F, npar), dtype=float)
         p[PI_F_VALUE] = np.nan
         p[PI_F_LLIMIT] = -np.inf
         p[PI_F_ULIMIT] = np.inf
-        p[PI_F_STEP] = 0.
+        p[PI_F_STEP] = 0.0
         p[PI_F_MAXSTEP] = np.inf
 
         newinfoo = p = np.ndarray((PI_NUM_O, npar), dtype=np.object)
         p[PI_O_TIEFUNC] = None
 
         newinfob = p = np.ndarray(npar, dtype=int)
         p[:] = 0
 
         if self._npar is not None:
             overlap = min(self._npar, npar)
-            newinfof[:,:overlap] = self._pinfof[:,:overlap]
-            newinfoo[:,:overlap] = self._pinfoo[:,:overlap]
+            newinfof[:, :overlap] = self._pinfof[:, :overlap]
+            newinfoo[:, :overlap] = self._pinfoo[:, :overlap]
             newinfob[:overlap] = self._pinfob[:overlap]
 
         self._pinfof = newinfof
         self._pinfoo = newinfoo
         self._pinfob = newinfob
         # Return self for easy chaining of calls.
         self._npar = npar
         return self
 
-
     def _setBit(self, idx, mask, cond):
         p = self._pinfob
         p[idx] = (p[idx] & ~mask) | np.where(cond, mask, 0x0)
 
-
     def _getBits(self, mask):
         return np.where(self._pinfob & mask, True, False)
 
-
     def p_value(self, idx, value, fixed=False):
         if anynotfinite(value):
-            raise ValueError('value')
+            raise ValueError("value")
 
-        self._pinfof[PI_F_VALUE,idx] = value
+        self._pinfof[PI_F_VALUE, idx] = value
         self._setBit(idx, PI_M_FIXED, fixed)
         return self
 
-
     def p_limit(self, idx, lower=-np.inf, upper=np.inf):
         if np.any(lower > upper):
-            raise ValueError('lower/upper')
+            raise ValueError("lower/upper")
 
-        self._pinfof[PI_F_LLIMIT,idx] = lower
-        self._pinfof[PI_F_ULIMIT,idx] = upper
+        self._pinfof[PI_F_LLIMIT, idx] = lower
+        self._pinfof[PI_F_ULIMIT, idx] = upper
 
         # Try to be clever here -- setting lower = upper
         # marks the parameter as fixed.
 
         w = np.where(lower == upper)
         if len(w) and w[0].size:
             self.p_value(w, np.atleast_1d(lower)[w], True)
 
         return self
 
-
     def p_step(self, idx, step, maxstep=np.inf, isrel=False):
         if np.any(np.isinf(step)):
-            raise ValueError('step')
+            raise ValueError("step")
         if np.any((step > maxstep) & ~isrel):
-            raise ValueError('step > maxstep')
+            raise ValueError("step > maxstep")
 
-        self._pinfof[PI_F_STEP,idx] = step
-        self._pinfof[PI_F_MAXSTEP,idx] = maxstep
+        self._pinfof[PI_F_STEP, idx] = step
+        self._pinfof[PI_F_MAXSTEP, idx] = maxstep
         self._setBit(idx, PI_M_RELSTEP, isrel)
         return self
 
-
     def p_side(self, idx, sidedness):
         """Acceptable values for *sidedness* are "auto", "pos",
         "neg", and "two"."""
         dsideval = _dside_names.get(sidedness)
         if dsideval is None:
             raise ValueError('unrecognized sidedness "%s"' % sidedness)
 
         p = self._pinfob
         p[idx] = (p[idx] & ~PI_M_SIDE) | dsideval
         return self
 
-
     def p_tie(self, idx, tiefunc):
         t1 = np.atleast_1d(tiefunc)
         if not np.all([x is None or callable(x) for x in t1]):
-            raise ValueError('tiefunc')
+            raise ValueError("tiefunc")
 
-        self._pinfoo[PI_O_TIEFUNC,idx] = tiefunc
+        self._pinfoo[PI_O_TIEFUNC, idx] = tiefunc
         return self
 
-
     def _check_param_config(self):
         if self._npar is None:
-            raise ValueError('no npar yet')
+            raise ValueError("no npar yet")
 
         p = self._pinfof
 
         if np.any(np.isinf(p[PI_F_VALUE])):
             # note: this allows NaN param values, in which case we'll
             # check in solve() that it's been given valid parameters
             # as arguments.
-            raise ValueError('some specified initial values infinite')
+            raise ValueError("some specified initial values infinite")
 
         if np.any(np.isinf(p[PI_F_STEP])):
-            raise ValueError('some specified parameter steps infinite')
+            raise ValueError("some specified parameter steps infinite")
 
         if np.any((p[PI_F_STEP] > p[PI_F_MAXSTEP]) & ~self._getBits(PI_M_RELSTEP)):
-            raise ValueError('some specified steps bigger than specified maxsteps')
+            raise ValueError("some specified steps bigger than specified maxsteps")
 
         if np.any(p[PI_F_LLIMIT] > p[PI_F_ULIMIT]):
-            raise ValueError('some param lower limits > upper limits')
+            raise ValueError("some param lower limits > upper limits")
 
         for i in range(p.shape[1]):
-            v = p[PI_F_VALUE,i]
+            v = p[PI_F_VALUE, i]
 
             if np.isnan(v):
-                continue # unspecified param ok; but comparisons will issue warnings
-            if v < p[PI_F_LLIMIT,i]:
-                raise ValueError('parameter #%d value below its lower limit' % i)
-            if v > p[PI_F_ULIMIT,i]:
-                raise ValueError('parameter #%d value above its upper limit' % i)
+                continue  # unspecified param ok; but comparisons will issue warnings
+            if v < p[PI_F_LLIMIT, i]:
+                raise ValueError("parameter #%d value below its lower limit" % i)
+            if v > p[PI_F_ULIMIT, i]:
+                raise ValueError("parameter #%d value above its upper limit" % i)
 
         p = self._pinfoo
 
         if not np.all([x is None or callable(x) for x in p[PI_O_TIEFUNC]]):
-            raise ValueError('some tied values not None or callable')
+            raise ValueError("some tied values not None or callable")
 
         # And compute some useful arrays. A tied parameter counts as fixed.
 
         tied = np.asarray([x is not None for x in self._pinfoo[PI_O_TIEFUNC]])
         self._anytied = np.any(tied)
         self._ifree = np.where(~(self._getBits(PI_M_FIXED) | tied))[0]
 
-
     def get_nfree(self):
         self._check_param_config()
         return self._ifree.size
 
-
     # Now, the function and the constraint values
 
     def set_func(self, nout, yfunc, jfunc):
         try:
             nout = int(nout)
             assert nout > 0
             # Do not check that nout >= npar here, since
             # the user may wish to fix parameters, which
             # could make the problem tractable after all.
         except:
-            raise ValueError('nout')
+            raise ValueError("nout")
 
         if not callable(yfunc):
-            raise ValueError('yfunc')
+            raise ValueError("yfunc")
 
         if jfunc is None:
             self._get_jacobian = self._get_jacobian_automatic
         else:
             if not callable(jfunc):
-                raise ValueError('jfunc')
+                raise ValueError("jfunc")
             self._get_jacobian = self._get_jacobian_explicit
 
         self._nout = nout
         self._yfunc = yfunc
         self._jfunc = jfunc
         self._nfev = 0
         self._njev = 0
         return self
 
-
     def set_residual_func(self, yobs, errinv, yfunc, jfunc, reckless=False):
         from numpy import subtract, multiply
 
         self._check_param_config()
         npar = self._npar
 
         if anynotfinite(errinv):
-            raise ValueError('some inverse errors are nonfinite')
+            raise ValueError("some inverse errors are nonfinite")
 
         # FIXME: handle yobs.ndim != 1 and/or yobs being complex
 
         if reckless:
+
             def ywrap(pars, nresids):
-                yfunc(pars, nresids) # model Y values => nresids
-                subtract(yobs, nresids, nresids) # abs. residuals => nresids
+                yfunc(pars, nresids)  # model Y values => nresids
+                subtract(yobs, nresids, nresids)  # abs. residuals => nresids
                 multiply(nresids, errinv, nresids)
+
             def jwrap(pars, jac):
                 jfunc(pars, jac)
                 multiply(jac, -1, jac)
-                jac *= errinv # broadcasts how we want
+                jac *= errinv  # broadcasts how we want
+
         else:
+
             def ywrap(pars, nresids):
                 yfunc(pars, nresids)
                 if anynotfinite(nresids):
-                    raise RuntimeError('function returned nonfinite values')
+                    raise RuntimeError("function returned nonfinite values")
                 subtract(yobs, nresids, nresids)
                 multiply(nresids, errinv, nresids)
+
             def jwrap(pars, jac):
                 jfunc(pars, jac)
                 if anynotfinite(jac):
-                    raise RuntimeError('jacobian returned nonfinite values')
+                    raise RuntimeError("jacobian returned nonfinite values")
                 multiply(jac, -1, jac)
                 jac *= errinv
 
         if jfunc is None:
             jwrap = None
 
         return self.set_func(yobs.size, ywrap, jwrap)
 
-
     def _fixup_check(self, dtype):
         self._check_param_config()
 
         if self._nout is None:
-            raise ValueError('no nout yet')
+            raise ValueError("no nout yet")
 
         if self._nout < self._npar - self._ifree.size:
-            raise RuntimeError('too many free parameters')
+            raise RuntimeError("too many free parameters")
 
         # Coerce parameters to desired types
 
         self.ftol = float(self.ftol)
         self.xtol = float(self.xtol)
         self.gtol = float(self.gtol)
         self.damp = float(self.damp)
@@ -1558,62 +1552,60 @@
         self.maxiter = int(self.maxiter)
         self.debug_calls = bool(self.debug_calls)
         self.debug_jac = bool(self.debug_jac)
 
         if self.diag is not None:
             self.diag = np.atleast_1d(np.asarray(self.diag, dtype=float))
 
-            if self.diag.shape != (self._npar, ):
-                raise ValueError('diag')
-            if np.any(self.diag <= 0.):
-                raise ValueError('diag')
+            if self.diag.shape != (self._npar,):
+                raise ValueError("diag")
+            if np.any(self.diag <= 0.0):
+                raise ValueError("diag")
 
         if self.normfunc is None:
             self.normfunc = enorm_mpfit_careful
         elif not callable(self.normfunc):
-            raise ValueError('normfunc must be a callable or None')
+            raise ValueError("normfunc must be a callable or None")
 
         # Bounds and type checks
 
         if not issubclass(self.solclass, Solution):
-            raise ValueError('solclass')
+            raise ValueError("solclass")
 
-        if self.ftol < 0.:
-            raise ValueError('ftol')
+        if self.ftol < 0.0:
+            raise ValueError("ftol")
 
-        if self.xtol < 0.:
-            raise ValueError('xtol')
+        if self.xtol < 0.0:
+            raise ValueError("xtol")
 
-        if self.gtol < 0.:
-            raise ValueError('gtol')
+        if self.gtol < 0.0:
+            raise ValueError("gtol")
 
-        if self.damp < 0.:
-            raise ValueError('damp')
+        if self.damp < 0.0:
+            raise ValueError("damp")
 
         if self.maxiter < 1:
-            raise ValueError('maxiter')
+            raise ValueError("maxiter")
 
-        if self.factor <= 0.:
-            raise ValueError('factor')
+        if self.factor <= 0.0:
+            raise ValueError("factor")
 
         # Consistency checks
 
         if self._jfunc is not None and self.damp > 0:
-            raise ValueError('damping factor not allowed when using '
-                             'explicit derivatives')
-
+            raise ValueError(
+                "damping factor not allowed when using " "explicit derivatives"
+            )
 
     def get_ndof(self):
-        self._fixup_check(float) # dtype is irrelevant here
+        self._fixup_check(float)  # dtype is irrelevant here
         return self._nout - self._ifree.size
 
-
     def copy(self):
-        n = Problem(self._npar, self._nout, self._yfunc, self._jfunc,
-                    self.solclass)
+        n = Problem(self._npar, self._nout, self._yfunc, self._jfunc, self.solclass)
 
         if self._pinfof is not None:
             n._pinfof = self._pinfof.copy()
             n._pinfoo = self._pinfoo.copy()
             n._pinfob = self._pinfob.copy()
 
         if self.diag is not None:
@@ -1628,40 +1620,38 @@
         n.maxiter = self.maxiter
         n.normfunc = self.normfunc
         n.debug_calls = self.debug_calls
         n.debug_jac = self.debug_jac
 
         return n
 
-
     # Actual implementation code!
 
     def _ycall(self, params, vec):
         if self._anytied:
             self._apply_ties(params)
 
         self._nfev += 1
 
         if self.debug_calls:
-            print('Call: #%4d f(%s) ->' % (self._nfev, params), end='')
+            print("Call: #%4d f(%s) ->" % (self._nfev, params), end="")
         self._yfunc(params, vec)
         if self.debug_calls:
             print(vec)
 
         if self.damp > 0:
             np.tanh(vec / self.damp, vec)
 
-
     def solve(self, initial_params=None, dtype=float):
         from numpy import any, clip, dot, isfinite, sqrt, where
 
         self._fixup_check(dtype)
         ifree = self._ifree
         ycall = self._ycall
-        n = ifree.size # number of free params; we try to allow n = 0
+        n = ifree.size  # number of free params; we try to allow n = 0
 
         # Set up initial values. These can either be specified via the
         # arguments to this function, or set implicitly with calls to
         # p_value() and p_limit(). Former overrides the latter. (The
         # intent of this flexibility is that if you compose a problem
         # out of several independent pieces, the caller of solve()
         # might not know good initial guesses for all of the
@@ -1670,71 +1660,75 @@
 
         if initial_params is not None:
             initial_params = np.atleast_1d(np.asarray(initial_params, dtype=dtype))
         else:
             initial_params = self._pinfof[PI_F_VALUE]
 
         if initial_params.size != self._npar:
-            raise ValueError('expected exactly %d parameters, got %d'
-                             % (self._npar, initial_params.size))
+            raise ValueError(
+                "expected exactly %d parameters, got %d"
+                % (self._npar, initial_params.size)
+            )
 
-        initial_params = initial_params.copy() # make sure not to modify arg
+        initial_params = initial_params.copy()  # make sure not to modify arg
         w = where(self._pinfob & PI_M_FIXED)
-        initial_params[w] = self._pinfof[PI_F_VALUE,w]
+        initial_params[w] = self._pinfof[PI_F_VALUE, w]
 
         if anynotfinite(initial_params):
-            raise ValueError('some nonfinite initial parameter values')
+            raise ValueError("some nonfinite initial parameter values")
 
         dtype = initial_params.dtype
         finfo = np.finfo(dtype)
         params = initial_params.copy()
-        x = params[ifree] # x is the free subset of our parameters
+        x = params[ifree]  # x is the free subset of our parameters
 
         # Steps for numerical derivatives
         isrel = self._getBits(PI_M_RELSTEP)
         dside = self._pinfob & PI_M_SIDE
-        maxstep = self._pinfof[PI_F_MAXSTEP,ifree]
+        maxstep = self._pinfof[PI_F_MAXSTEP, ifree]
         whmaxstep = where(isfinite(maxstep))
         anymaxsteps = whmaxstep[0].size > 0
 
         # Which parameters have limits?
 
-        hasulim = isfinite(self._pinfof[PI_F_ULIMIT,ifree])
-        ulim = self._pinfof[PI_F_ULIMIT,ifree]
-        hasllim = isfinite(self._pinfof[PI_F_LLIMIT,ifree])
-        llim = self._pinfof[PI_F_LLIMIT,ifree]
+        hasulim = isfinite(self._pinfof[PI_F_ULIMIT, ifree])
+        ulim = self._pinfof[PI_F_ULIMIT, ifree]
+        hasllim = isfinite(self._pinfof[PI_F_LLIMIT, ifree])
+        llim = self._pinfof[PI_F_LLIMIT, ifree]
         anylimits = any(hasulim) or any(hasllim)
 
         # Init fnorm
 
         enorm = self.normfunc
-        fnorm1 = -1.
+        fnorm1 = -1.0
         fvec = np.ndarray(self._nout, dtype)
         fullfjac = np.zeros((self._npar, self._nout), finfo.dtype)
         fjac = fullfjac[:n]
         ycall(params, fvec)
         fnorm = enorm(fvec, finfo)
 
         # Initialize Levenberg-Marquardt parameter and
         # iteration counter.
 
-        par = 0.
+        par = 0.0
         niter = 1
-        fqt = x * 0.
+        fqt = x * 0.0
         status = set()
 
         # Outer loop top.
 
         while True:
             params[ifree] = x
 
             if self._anytied:
                 self._apply_ties(params)
 
-            self._get_jacobian(params, fvec, fullfjac, ulim, dside, maxstep, isrel, finfo)
+            self._get_jacobian(
+                params, fvec, fullfjac, ulim, dside, maxstep, isrel, finfo
+            )
 
             if anylimits:
                 # Check for parameters pegged at limits
                 whlpeg = where(hasllim & (x == llim))[0]
                 nlpeg = len(whlpeg)
                 whupeg = where(hasulim & (x == ulim))[0]
                 nupeg = len(whupeg)
@@ -1758,87 +1752,86 @@
             if niter == 1:
                 # If "diag" unspecified, scale according to norms of rows
                 # of the initial jacobian
                 if self.diag is not None:
                     diag = self.diag.copy()
                 else:
                     diag = wa2.copy()
-                    diag[where(diag == 0)] = 1.
+                    diag[where(diag == 0)] = 1.0
 
                 # Calculate norm of scaled x, initialize step bound delta
                 xnorm = enorm(diag * x, finfo)
                 delta = self.factor * xnorm
-                if delta == 0.:
+                if delta == 0.0:
                     delta = self.factor
 
             # Compute fvec * (q.T), store the first n components in fqt
 
             wa4 = fvec.copy()
 
             for j in range(n):
-                temp3 = fjac[j,j]
+                temp3 = fjac[j, j]
                 if temp3 != 0:
-                    fj = fjac[j,j:]
+                    fj = fjac[j, j:]
                     wj = wa4[j:]
                     wa4[j:] = wj - fj * dot(wj, fj) / temp3
-                fjac[j,j] = wa1[j]
+                fjac[j, j] = wa1[j]
                 fqt[j] = wa4[j]
 
             # Only the n-by-n part of fjac is important now, and this
             # test will probably be cheap since usually n << m.
 
-            if anynotfinite(fjac[:,:n]):
-                raise RuntimeError('nonfinite terms in Jacobian matrix')
+            if anynotfinite(fjac[:, :n]):
+                raise RuntimeError("nonfinite terms in Jacobian matrix")
 
             # Calculate the norm of the scaled gradient
 
-            gnorm = 0.
+            gnorm = 0.0
             if fnorm != 0:
                 for j in range(n):
                     l = pmut[j]
                     if wa2[l] != 0:
-                        s = dot(fqt[:j+1], fjac[j,:j+1]) / fnorm
+                        s = dot(fqt[: j + 1], fjac[j, : j + 1]) / fnorm
                         gnorm = max(gnorm, abs(s / wa2[l]))
 
             # Test for convergence of gradient norm
 
             if gnorm <= self.gtol:
-                status.add('gtol')
+                status.add("gtol")
                 break
 
             if self.diag is None:
                 diag = np.maximum(diag, wa2)
 
             # Inner loop
             while True:
                 # Get Levenberg-Marquardt parameter. fjac is modified in-place
-                par, wa1 = _lm_solve(fjac, pmut, diag, fqt, delta, par,
-                                     enorm, finfo)
+                par, wa1 = _lm_solve(fjac, pmut, diag, fqt, delta, par, enorm, finfo)
                 # "Store the direction p and x+p. Calculate the norm of p"
                 wa1 *= -1
-                alpha = 1.
+                alpha = 1.0
 
                 if not anylimits and not anymaxsteps:
                     # No limits applied, so just move to new position
                     wa2 = x + wa1
                 else:
                     if anylimits:
                         if nlpeg:
-                            wa1[whlpeg] = clip(wa1[whlpeg], 0., max(wa1))
+                            wa1[whlpeg] = clip(wa1[whlpeg], 0.0, max(wa1))
                         if nupeg:
-                            wa1[whupeg] = clip(wa1[whupeg], min(wa1), 0.)
+                            wa1[whupeg] = clip(wa1[whupeg], min(wa1), 0.0)
 
                         dwa1 = abs(wa1) > finfo.eps
-                        whl = where((dwa1 != 0.) & hasllim & ((x + wa1) < llim))
+                        whl = where((dwa1 != 0.0) & hasllim & ((x + wa1) < llim))
 
                         if len(whl[0]):
                             t = (llim[whl] - x[whl]) / wa1[whl]
                             alpha = min(alpha, t.min())
 
-                        whu = where((dwa1 != 0.) & hasulim & ((x + wa1) > ulim))
+                        whu = where((dwa1 != 0.0) & hasulim & ((x + wa1) > ulim))
 
                         if len(whu[0]):
                             t = (ulim[whu] - x[whu]) / wa1[whu]
                             alpha = min(alpha, t.min())
 
                     if anymaxsteps:
                         nwa1 = wa1 * alpha
@@ -1871,35 +1864,35 @@
                 # Evaluate func at x + p and calculate norm
 
                 ycall(params, wa4)
                 fnorm1 = enorm(wa4, finfo)
 
                 # Compute scaled actual reductions
 
-                actred = -1.
+                actred = -1.0
                 if 0.1 * fnorm1 < fnorm:
-                    actred = 1 - (fnorm1 / fnorm)**2
+                    actred = 1 - (fnorm1 / fnorm) ** 2
 
                 # Compute scaled predicted reduction and scaled directional
                 # derivative
 
                 for j in range(n):
                     wa3[j] = 0
-                    wa3[:j+1] = wa3[:j+1] + fjac[j,:j+1] * wa1[pmut[j]]
+                    wa3[: j + 1] = wa3[: j + 1] + fjac[j, : j + 1] * wa1[pmut[j]]
 
                 # "Remember, alpha is the fraction of the full LM step actually
                 # taken."
 
                 temp1 = enorm(alpha * wa3, finfo) / fnorm
                 temp2 = sqrt(alpha * par) * pnorm / fnorm
                 prered = temp1**2 + 2 * temp2**2
                 dirder = -(temp1**2 + temp2**2)
 
                 # Compute ratio of the actual to the predicted reduction.
-                ratio = 0.
+                ratio = 0.0
                 if prered != 0:
                     ratio = actred / prered
 
                 # Update the step bound
 
                 if ratio <= 0.25:
                     if actred >= 0:
@@ -1924,49 +1917,49 @@
                     xnorm = enorm(wa2, finfo)
                     fnorm = fnorm1
                     niter += 1
 
                 # Check for convergence
 
                 if abs(actred) <= self.ftol and prered <= self.ftol and ratio <= 2:
-                    status.add('ftol')
+                    status.add("ftol")
 
                 if delta <= self.xtol * xnorm:
-                    status.add('xtol')
+                    status.add("xtol")
 
                 # Check for termination, "stringent tolerances"
 
                 if niter >= self.maxiter:
-                    status.add('maxiter')
+                    status.add("maxiter")
 
                 if abs(actred) <= finfo.eps and prered <= finfo.eps and ratio <= 2:
-                    status.add('feps')
+                    status.add("feps")
 
                 if delta <= finfo.eps * xnorm:
-                    status.add('xeps')
+                    status.add("xeps")
 
                 if gnorm <= finfo.eps:
-                    status.add('geps')
+                    status.add("geps")
 
                 # Repeat loop if iteration
                 # unsuccessful. "Unsuccessful" means that the ratio of
                 # actual to predicted norm reduction is less than 1e-4
                 # and none of the stopping criteria were met.
                 if ratio >= 0.0001 or len(status):
                     break
 
             if len(status):
                 break
 
             if anynotfinite(wa1):
-                raise RuntimeError('overflow in wa1')
+                raise RuntimeError("overflow in wa1")
             if anynotfinite(wa2):
-                raise RuntimeError('overflow in wa2')
+                raise RuntimeError("overflow in wa2")
             if anynotfinite(x):
-                raise RuntimeError('overflow in x')
+                raise RuntimeError("overflow in x")
 
         # End outer loop. Finalize params, fvec, and fnorm
 
         if n == 0:
             params = initial_params.copy()
         else:
             params[ifree] = x
@@ -1984,19 +1977,19 @@
 
         if n > 0:
             sz = fjac.shape
 
             if sz[0] < n or sz[1] < n or len(pmut) < n:
                 covar = None
             else:
-                cv = _calc_covariance(fjac[:,:n], pmut[:n])
+                cv = _calc_covariance(fjac[:, :n], pmut[:n])
                 cv.shape = (n, n)
 
-                for i in range(n): # can't do 2D fancy indexing
-                    covar[ifree[i],ifree] = cv[i]
+                for i in range(n):  # can't do 2D fancy indexing
+                    covar[ifree[i], ifree] = cv[i]
 
         # Errors in parameters from the diagonal of covar.
 
         perror = None
 
         if covar is not None:
             perror = np.zeros(self._npar, dtype)
@@ -2016,49 +2009,49 @@
         soln.fnorm = fnorm
         soln.fvec = fvec
         soln.fjac = fjac
         soln.nfev = self._nfev
         soln.njev = self._njev
         return soln
 
-
-    def _get_jacobian_explicit(self, params, fvec, fjacfull, ulimit,
-                               dside, maxstep, isrel, finfo):
+    def _get_jacobian_explicit(
+        self, params, fvec, fjacfull, ulimit, dside, maxstep, isrel, finfo
+    ):
         self._njev += 1
 
         if self.debug_calls:
-            print('Call: #%4d j(%s) ->' % (self._njev, params), end='')
+            print("Call: #%4d j(%s) ->" % (self._njev, params), end="")
         self._jfunc(params, fjacfull)
         if self.debug_calls:
             print(fjacfull)
 
         # Condense down to contain only the rows relevant to the free
         # parameters. We actually copy the data here instead of using fancy
         # indexing since this condensed matrix will be used a lot.
 
         ifree = self._ifree
 
         if ifree.size < self._npar:
             for i in range(ifree.size):
                 fjacfull[i] = fjacfull[ifree[i]]
 
-
-    def _get_jacobian_automatic(self, params, fvec, fjacfull, ulimit,
-                                dside, maxstep, isrel, finfo):
+    def _get_jacobian_automatic(
+        self, params, fvec, fjacfull, ulimit, dside, maxstep, isrel, finfo
+    ):
         eps = np.sqrt(max(self.epsilon, finfo.eps))
         ifree = self._ifree
         x = params[ifree]
         m = len(fvec)
         n = len(x)
         h = eps * np.abs(x)
 
         # Apply any fixed steps, absolute and relative.
-        stepi = self._pinfof[PI_F_STEP,ifree]
+        stepi = self._pinfof[PI_F_STEP, ifree]
         wh = np.where(stepi > 0)
-        h[wh] = stepi[wh] * np.where(isrel[ifree[wh]], x[wh], 1.)
+        h[wh] = stepi[wh] * np.where(isrel[ifree[wh]], x[wh], 1.0)
 
         # Clamp stepsizes to maxstep.
         np.minimum(h, maxstep, h)
 
         # Make sure no zero step values
         h[np.where(h == 0)] = eps
 
@@ -2068,15 +2061,15 @@
         mask = (dside == DSIDE_NEG)[ifree]
         if ulimit is not None:
             mask |= x > ulimit - h
         wh = np.where(mask)
         h[wh] = -h[wh]
 
         if self.debug_jac:
-            print('Jac-:', h)
+            print("Jac-:", h)
 
         # Compute derivative for each parameter
 
         fp = np.empty(self._nout, dtype=finfo.dtype)
         fm = np.empty(self._nout, dtype=finfo.dtype)
 
         for i in range(n):
@@ -2091,134 +2084,150 @@
                 # Two-sided ... extra func call
                 xp[ifree[i]] = params[ifree[i]] - h[i]
                 self._ycall(xp, fm)
                 fjacfull[i] = (fp - fm) / (2 * h[i])
 
         if self.debug_jac:
             for i in range(n):
-                print('Jac :', fjacfull[i])
-
+                print("Jac :", fjacfull[i])
 
     def _manual_jacobian(self, params, dtype=float):
         self._fixup_check(dtype)
 
         ifree = self._ifree
 
         params = np.atleast_1d(np.asarray(params, dtype))
         fvec = np.empty(self._nout, dtype)
         fjacfull = np.empty((self._npar, self._nout), dtype)
-        ulimit = self._pinfof[PI_F_ULIMIT,ifree]
+        ulimit = self._pinfof[PI_F_ULIMIT, ifree]
         dside = self._pinfob & PI_M_SIDE
-        maxstep = self._pinfof[PI_F_MAXSTEP,ifree]
+        maxstep = self._pinfof[PI_F_MAXSTEP, ifree]
         isrel = self._getBits(PI_M_RELSTEP)
         finfo = np.finfo(dtype)
 
         # Before we can evaluate the Jacobian, we need to get the initial
         # value of the function at the specified position. Note that in the
         # real algorithm, _apply_ties is always called before _get_jacobian.
 
         self._ycall(params, fvec)
         self._get_jacobian(params, fvec, fjacfull, ulimit, dside, maxstep, isrel, finfo)
-        return fjacfull[:ifree.size]
-
+        return fjacfull[: ifree.size]
 
     def _apply_ties(self, params):
         funcs = self._pinfoo[PI_O_TIEFUNC]
 
         for i in range(self._npar):
             if funcs[i] is not None:
                 params[i] = funcs[i](params)
 
-
     def solve_scipy(self, initial_params=None, dtype=float, strict=True):
         from numpy import any, clip, dot, isfinite, sqrt, where
+
         self._fixup_check(dtype)
 
         if strict:
             if self._ifree.size != self._npar:
-                raise RuntimeError('can only use scipy layer with no ties '
-                                   'or fixed params')
-            if any(isfinite(self._pinfof[PI_F_ULIMIT]) | isfinite(self._pinfof[PI_F_LLIMIT])):
-                raise RuntimeError('can only use scipy layer with no '
-                                   'parameter limits')
+                raise RuntimeError(
+                    "can only use scipy layer with no ties " "or fixed params"
+                )
+            if any(
+                isfinite(self._pinfof[PI_F_ULIMIT])
+                | isfinite(self._pinfof[PI_F_LLIMIT])
+            ):
+                raise RuntimeError(
+                    "can only use scipy layer with no " "parameter limits"
+                )
 
         from scipy.optimize import leastsq
 
         if initial_params is not None:
             initial_params = np.atleast_1d(np.asarray(initial_params, dtype=dtype))
         else:
             initial_params = self._pinfof[PI_F_VALUE]
 
         if initial_params.size != self._npar:
-            raise ValueError('expected exactly %d parameters, got %d'
-                             % (self._npar, initial_params.size))
+            raise ValueError(
+                "expected exactly %d parameters, got %d"
+                % (self._npar, initial_params.size)
+            )
 
         if anynotfinite(initial_params):
-            raise ValueError('some nonfinite initial parameter values')
+            raise ValueError("some nonfinite initial parameter values")
 
         dtype = initial_params.dtype
         finfo = np.finfo(dtype)
 
         def sofunc(pars):
             y = np.empty(self._nout, dtype=dtype)
             self._yfunc(pars, y)
             return y
 
         if self._jfunc is None:
             sojac = None
         else:
+
             def sojac(pars):
                 j = np.empty((self._npar, self._nout), dtype=dtype)
                 self._jfunc(pars, j)
                 return j.T
 
-        t = leastsq(sofunc, initial_params, Dfun=sojac, full_output=1,
-                    ftol=self.ftol, xtol=self.xtol, gtol=self.gtol,
-                    maxfev=self.maxiter, # approximate
-                    epsfcn=self.epsilon, factor=self.factor, diag=self.diag,
-                    warning=False)
+        t = leastsq(
+            sofunc,
+            initial_params,
+            Dfun=sojac,
+            full_output=1,
+            ftol=self.ftol,
+            xtol=self.xtol,
+            gtol=self.gtol,
+            maxfev=self.maxiter,  # approximate
+            epsfcn=self.epsilon,
+            factor=self.factor,
+            diag=self.diag,
+            warning=False,
+        )
 
         covar = t[1]
         perror = None
 
         if covar is not None:
             perror = np.zeros(self._npar, dtype)
             d = covar.diagonal()
             wh = where(d >= 0)
             perror[wh] = sqrt(d[wh])
 
         soln = self.solclass(self)
         soln.ndof = self.get_ndof()
-        soln.status = set(('scipy', ))
+        soln.status = set(("scipy",))
         soln.scipy_mesg = t[3]
         soln.scipy_ier = t[4]
-        soln.niter = t[2]['nfev'] # approximate
+        soln.niter = t[2]["nfev"]  # approximate
         soln.params = t[0]
         soln.covar = covar
         soln.perror = perror
-        soln.fvec = t[2]['fvec']
-        soln.fnorm = enorm_minpack(soln.fvec, finfo)**2
-        soln.fjac = t[2]['fjac'].T
-        soln.nfev = t[2]['nfev']
-        soln.njev = 0 # could compute when given explicit derivative ...
+        soln.fvec = t[2]["fvec"]
+        soln.fnorm = enorm_minpack(soln.fvec, finfo) ** 2
+        soln.fjac = t[2]["fjac"].T
+        soln.nfev = t[2]["nfev"]
+        soln.njev = 0  # could compute when given explicit derivative ...
         return soln
 
 
 def check_derivative(npar, nout, yfunc, jfunc, guess):
     explicit = np.empty((npar, nout))
     jfunc(guess, explicit)
 
     p = Problem(npar, nout, yfunc, None)
     auto = p._manual_jacobian(guess)
 
     return explicit, auto
 
 
-def ResidualProblem(npar, yobs, errinv, yfunc, jfunc,
-                    solclass=Solution, reckless=False):
+def ResidualProblem(
+    npar, yobs, errinv, yfunc, jfunc, solclass=Solution, reckless=False
+):
     p = Problem(solclass=solclass)
     p.set_npar(npar)
     p.set_residual_func(yobs, errinv, yfunc, jfunc, reckless=reckless)
     return p
 
 
 # Test!
@@ -2234,30 +2243,32 @@
     def f(pars, ymodel):
         multiply(x, pars[0], ymodel)
         add(ymodel, pars[1], ymodel)
 
     p = ResidualProblem(2, y, 100, f, None)
     return p.solve([2.5, 1.5])
 
+
 @test
 def _simple_automatic_jac():
     def f(pars, vec):
         np.exp(pars, vec)
 
     p = Problem(1, 1, f, None)
     j = p._manual_jacobian(0)
-    Taaae(j, [[1.]])
+    Taaae(j, [[1.0]])
     j = p._manual_jacobian(1)
     Taaae(j, [[np.e]])
 
     p = Problem(3, 3, f, None)
     x = np.asarray([0, 1, 2])
     j = p._manual_jacobian(x)
     Taaae(j, np.diag(np.exp(x)))
 
+
 @test
 def _jac_sidedness():
     # Make a function with a derivative discontinuity so we can test
     # the sidedness settings.
 
     def f(pars, vec):
         p = pars[0]
@@ -2266,59 +2277,60 @@
             vec[:] = p
         else:
             vec[:] = -p
 
     p = Problem(1, 1, f, None)
 
     # Default: positive unless against upper limit.
-    Taaae(p._manual_jacobian(0), [[1.]])
+    Taaae(p._manual_jacobian(0), [[1.0]])
 
     # DSIDE_AUTO should be the default.
-    p.p_side(0, 'auto')
-    Taaae(p._manual_jacobian(0), [[1.]])
+    p.p_side(0, "auto")
+    Taaae(p._manual_jacobian(0), [[1.0]])
 
     # DSIDE_POS should be equivalent here.
-    p.p_side(0, 'pos')
-    Taaae(p._manual_jacobian(0), [[1.]])
+    p.p_side(0, "pos")
+    Taaae(p._manual_jacobian(0), [[1.0]])
 
     # DSIDE_NEG should get the other side of the discont.
-    p.p_side(0, 'neg')
-    Taaae(p._manual_jacobian(0), [[-1.]])
+    p.p_side(0, "neg")
+    Taaae(p._manual_jacobian(0), [[-1.0]])
 
     # DSIDE_AUTO should react to an upper limit and take
     # a negative-step derivative.
-    p.p_side(0, 'auto')
+    p.p_side(0, "auto")
     p.p_limit(0, upper=0)
-    Taaae(p._manual_jacobian(0), [[-1.]])
+    Taaae(p._manual_jacobian(0), [[-1.0]])
+
 
 @test
 def _jac_stepsizes():
     def f(expstep, pars, vec):
         p = pars[0]
 
-        if p != 1.:
+        if p != 1.0:
             Taae(p, expstep)
 
         vec[:] = 1
 
     # Fixed stepsize of 1.
-    p = Problem(1, 1, lambda p, v: f(2., p, v), None)
-    p.p_step(0, 1.)
+    p = Problem(1, 1, lambda p, v: f(2.0, p, v), None)
+    p.p_step(0, 1.0)
     p._manual_jacobian(1)
 
     # Relative stepsize of 0.1
     p = Problem(1, 1, lambda p, v: f(1.1, p, v), None)
     p.p_step(0, 0.1, isrel=True)
     p._manual_jacobian(1)
 
     # Fixed stepsize must be less than max stepsize.
     try:
         p = Problem(2, 2, f, None)
         p.p_step((0, 1), (1, 1), (1, 0.5))
-        assert False, 'Invalid arguments accepted'
+        assert False, "Invalid arguments accepted"
     except ValueError:
         pass
 
     # Maximum stepsize, made extremely small to be enforced
     # in default circumstances.
     p = Problem(1, 1, lambda p, v: f(1 + 1e-11, p, v), None)
     p.p_step(0, 0.0, 1e-11)
@@ -2328,14 +2340,15 @@
     p = Problem(1, 1, lambda p, v: f(1.1, p, v), None)
     p.p_step(0, 0.5, 0.1, True)
     p._manual_jacobian(1)
 
 
 # lmder1 / lmdif1 test cases
 
+
 def _lmder1_test(nout, func, jac, guess):
     finfo = np.finfo(float)
     tol = np.sqrt(finfo.eps)
     guess = np.asfarray(guess)
 
     y = np.empty(nout)
     func(guess, y)
@@ -2344,24 +2357,25 @@
     p.xtol = p.ftol = tol
     p.gtol = 0
     p.maxiter = 100 * (guess.size + 1)
     s = p.solve(guess)
     func(s.params, y)
     fnorm2 = enorm_mpfit_careful(y, finfo)
 
-    print('  n, m:', guess.size, nout)
-    print('  fnorm1:', fnorm1)
-    print('  fnorm2:', fnorm2)
-    print('  nfev, njev:', s.nfev, s.njev)
-    print('  status:', s.status)
-    print('  params:', s.params)
+    print("  n, m:", guess.size, nout)
+    print("  fnorm1:", fnorm1)
+    print("  fnorm2:", fnorm2)
+    print("  nfev, njev:", s.nfev, s.njev)
+    print("  status:", s.status)
+    print("  params:", s.params)
 
 
-def _lmder1_driver(nout, func, jac, guess, target_fnorm1,
-                   target_fnorm2, target_params, decimal=10):
+def _lmder1_driver(
+    nout, func, jac, guess, target_fnorm1, target_fnorm2, target_params, decimal=10
+):
     finfo = np.finfo(float)
     tol = np.sqrt(finfo.eps)
     guess = np.asfarray(guess)
 
     y = np.empty(nout)
     func(guess, y)
     fnorm1 = enorm_mpfit_careful(y, finfo)
@@ -2374,163 +2388,214 @@
     s = p.solve(guess)
 
     if target_params is not None:
         # assert_array_almost_equal goes to a fixed number of decimal
         # places regardless of the scale of the number, so it breaks
         # when we work with very large values.
         from numpy.testing import assert_array_almost_equal as aaae
+
         scale = np.maximum(np.abs(target_params), 1)
         try:
             aaae(s.params / scale, target_params / scale, decimal=decimal)
         except AssertionError:
-            assert False, '''Arrays are not almost equal to %d (scaled) decimals
+            assert False, """Arrays are not almost equal to %d (scaled) decimals
 
 x: %s
-y: %s''' % (decimal, s.params, target_params)
+y: %s""" % (
+                decimal,
+                s.params,
+                target_params,
+            )
 
     func(s.params, y)
     fnorm2 = enorm_mpfit_careful(y, finfo)
     Taae(fnorm2, target_fnorm2)
 
 
 def _lmder1_linear_full_rank(n, m, factor, target_fnorm1, target_fnorm2):
     """A full-rank linear function (lmder test #1)"""
 
     def func(params, vec):
         s = params.sum()
-        temp = 2. * s / m + 1
+        temp = 2.0 * s / m + 1
         vec[:] = -temp
-        vec[:params.size] += params
+        vec[: params.size] += params
 
     def jac(params, jac):
         # jac.shape = (n, m) by LMDER standards
-        jac.fill(-2. / m)
+        jac.fill(-2.0 / m)
         for i in range(n):
-            jac[i,i] += 1
+            jac[i, i] += 1
 
     guess = np.ones(n) * factor
 
-    #_lmder1_test(m, func, jac, guess)
-    _lmder1_driver(m, func, jac, guess,
-                   target_fnorm1, target_fnorm2,
-                   [-1] * n)
+    # _lmder1_test(m, func, jac, guess)
+    _lmder1_driver(m, func, jac, guess, target_fnorm1, target_fnorm2, [-1] * n)
+
 
 @test
 def _lmder1_linear_full_rank_1():
-    _lmder1_linear_full_rank(5, 10, 1, 5., 0.2236068e+01)
+    _lmder1_linear_full_rank(5, 10, 1, 5.0, 0.2236068e01)
+
 
 @test
 def _lmder1_linear_full_rank_2():
-    _lmder1_linear_full_rank(5, 50, 1, 0.806225774e+01, 0.670820393e+01)
+    _lmder1_linear_full_rank(5, 50, 1, 0.806225774e01, 0.670820393e01)
 
 
 # To investigate: the following four linear rank-1 tests have something weird
 # going on. The parameters returned by the optimizer agree with the Fortran
 # implementation for one of my machines (an AMD64) and disagree for another (a
 # 32-bit Intel). Furthermore, the same **Fortran** implementation gives
 # different parameter results on the two machines. I take this as an
 # indication that there's something weird about these tests such that the
 # precise parameter values are unpredictable. I've hacked the tests
 # accordingly to not check the parameter results.
 
+
 def _lmder1_linear_rank1(n, m, factor, target_fnorm1, target_fnorm2, target_params):
     """A rank-1 linear function (lmder test #2)"""
 
     def func(params, vec):
         s = 0
         for j in range(n):
             s += (j + 1) * params[j]
         for i in range(m):
             vec[i] = (i + 1) * s - 1
 
     def jac(params, jac):
         for i in range(n):
             for j in range(m):
-                jac[i,j] = (i + 1) * (j + 1)
+                jac[i, j] = (i + 1) * (j + 1)
 
     guess = np.ones(n) * factor
 
-    #_lmder1_test(m, func, jac, guess)
-    _lmder1_driver(m, func, jac, guess,
-                   target_fnorm1, target_fnorm2, None) #target_params)
+    # _lmder1_test(m, func, jac, guess)
+    _lmder1_driver(
+        m, func, jac, guess, target_fnorm1, target_fnorm2, None
+    )  # target_params)
+
 
 @test
 def _lmder1_linear_rank1_1():
-    _lmder1_linear_rank1(5, 10, 1,
-                         0.2915218688e+03, 0.1463850109e+01,
-                         [-0.167796818e+03, -0.8339840901e+02, 0.2211100431e+03,
-                          -0.4119920451e+02, -0.327593636e+02])
+    _lmder1_linear_rank1(
+        5,
+        10,
+        1,
+        0.2915218688e03,
+        0.1463850109e01,
+        [
+            -0.167796818e03,
+            -0.8339840901e02,
+            0.2211100431e03,
+            -0.4119920451e02,
+            -0.327593636e02,
+        ],
+    )
+
 
 @test
 def _lmder1_linear_rank1_2():
-    _lmder1_linear_rank1(5, 50, 1,
-                         0.310160039334e+04, 0.34826301657e+01,
-                         [-0.2029999900022674e+02, -0.9649999500113370e+01,
-                          -0.1652451975264496e+03, -0.4324999750056676e+01,
-                          0.1105330585100652e+03])
+    _lmder1_linear_rank1(
+        5,
+        50,
+        1,
+        0.310160039334e04,
+        0.34826301657e01,
+        [
+            -0.2029999900022674e02,
+            -0.9649999500113370e01,
+            -0.1652451975264496e03,
+            -0.4324999750056676e01,
+            0.1105330585100652e03,
+        ],
+    )
 
 
 def _lmder1_linear_r1zcr(n, m, factor, target_fnorm1, target_fnorm2, target_params):
     """A rank-1 linear function with zero columns and rows (lmder test #3)"""
 
     def func(params, vec):
         s = 0
         for j in range(1, n - 1):
             s += (j + 1) * params[j]
         for i in range(m):
             vec[i] = i * s - 1
-        vec[m-1] = -1
+        vec[m - 1] = -1
 
     def jac(params, jac):
         jac.fill(0)
 
         for i in range(1, n - 1):
             for j in range(1, m - 1):
-                jac[i,j] = j * (i + 1)
+                jac[i, j] = j * (i + 1)
 
     guess = np.ones(n) * factor
 
-    #_lmder1_test(m, func, jac, guess)
-    _lmder1_driver(m, func, jac, guess,
-                   target_fnorm1, target_fnorm2, None) #target_params)
+    # _lmder1_test(m, func, jac, guess)
+    _lmder1_driver(
+        m, func, jac, guess, target_fnorm1, target_fnorm2, None
+    )  # target_params)
+
 
 @test
 def _lmder1_linear_r1zcr_1():
-    _lmder1_linear_r1zcr(5, 10, 1,
-                         0.1260396763e+03, 0.1909727421e+01,
-                         [0.1000000000e+01, -0.2103615324e+03, 0.3212042081e+02,
-                          0.8113456825e+02, 0.1000000000e+01])
+    _lmder1_linear_r1zcr(
+        5,
+        10,
+        1,
+        0.1260396763e03,
+        0.1909727421e01,
+        [
+            0.1000000000e01,
+            -0.2103615324e03,
+            0.3212042081e02,
+            0.8113456825e02,
+            0.1000000000e01,
+        ],
+    )
+
 
 @test
 def _lmder1_linear_r1zcr_2():
-    _lmder1_linear_r1zcr(5, 50, 1,
-                         0.17489499707e+04, 0.3691729402e+01,
-                         [0.1000000000e+01, 0.3321494859e+03, -0.4396851914e+03,
-                          0.1636968826e+03, 0.1000000000e+01])
+    _lmder1_linear_r1zcr(
+        5,
+        50,
+        1,
+        0.17489499707e04,
+        0.3691729402e01,
+        [
+            0.1000000000e01,
+            0.3321494859e03,
+            -0.4396851914e03,
+            0.1636968826e03,
+            0.1000000000e01,
+        ],
+    )
+
 
 @test
 def _lmder1_rosenbrock():
     """Rosenbrock function (lmder test #4)"""
 
     def func(params, vec):
-        vec[0] = 10 * (params[1] - params[0]**2)
+        vec[0] = 10 * (params[1] - params[0] ** 2)
         vec[1] = 1 - params[0]
 
     def jac(params, jac):
-        jac[0,0] = -20 * params[0]
-        jac[0,1] = -1
-        jac[1,0] = 10
-        jac[1,1] = 0
+        jac[0, 0] = -20 * params[0]
+        jac[0, 1] = -1
+        jac[1, 0] = 10
+        jac[1, 1] = 0
 
     guess = np.asfarray([-1.2, 1])
-    norm1s = [0.491934955050e+01, 0.134006305822e+04, 0.1430000511923e+06]
+    norm1s = [0.491934955050e01, 0.134006305822e04, 0.1430000511923e06]
 
     for i in range(3):
-        _lmder1_driver(2, func, jac, guess * 10**i,
-                       norm1s[i], 0, [1, 1])
+        _lmder1_driver(2, func, jac, guess * 10**i, norm1s[i], 0, [1, 1])
 
 
 @test
 def _lmder1_helical_valley():
     """Helical valley function (lmder test #5)"""
     tpi = 2 * np.pi
 
@@ -2538,68 +2603,86 @@
         if params[0] == 0:
             tmp1 = np.copysign(0.25, params[1])
         elif params[0] > 0:
             tmp1 = np.arctan(params[1] / params[0]) / tpi
         else:
             tmp1 = np.arctan(params[1] / params[0]) / tpi + 0.5
 
-        tmp2 = np.sqrt(params[0]**2 + params[1]**2)
+        tmp2 = np.sqrt(params[0] ** 2 + params[1] ** 2)
 
         vec[0] = 10 * (params[2] - 10 * tmp1)
         vec[1] = 10 * (tmp2 - 1)
         vec[2] = params[2]
 
     def jac(params, jac):
-        temp = params[0]**2 + params[1]**2
+        temp = params[0] ** 2 + params[1] ** 2
         tmp1 = tpi * temp
         tmp2 = np.sqrt(temp)
-        jac[0,0] = 100 * params[1] / tmp1
-        jac[0,1] = 10 * params[0] / tmp2
-        jac[0,2] = 0
-        jac[1,0] = -100 * params[0] / tmp1
-        jac[1,1] = 10 * params[1] / tmp2
-        jac[2,0] = 10
-        jac[2,1] = 0
-        jac[1,2] = 0
-        jac[2,2] = 1
+        jac[0, 0] = 100 * params[1] / tmp1
+        jac[0, 1] = 10 * params[0] / tmp2
+        jac[0, 2] = 0
+        jac[1, 0] = -100 * params[0] / tmp1
+        jac[1, 1] = 10 * params[1] / tmp2
+        jac[2, 0] = 10
+        jac[2, 1] = 0
+        jac[1, 2] = 0
+        jac[2, 2] = 1
 
     guess = np.asfarray([-1, 0, 0])
 
-    _lmder1_driver(3, func, jac, guess,
-                   50., 0.993652310343e-16,
-                   [0.100000000000e+01, -0.624330159679e-17, 0.000000000000e+00])
-    _lmder1_driver(3, func, jac, guess * 10,
-                   0.102956301410e+03, 0.104467885065e-18,
-                   [0.100000000000e+01, 0.656391080516e-20, 0.000000000000e+00])
-    _lmder1_driver(3, func, jac, guess * 100,
-                   0.991261822124e+03, 0.313877781195e-28,
-                   [0.100000000000e+01, -0.197215226305e-29, 0.000000000000e+00])
+    _lmder1_driver(
+        3,
+        func,
+        jac,
+        guess,
+        50.0,
+        0.993652310343e-16,
+        [0.100000000000e01, -0.624330159679e-17, 0.000000000000e00],
+    )
+    _lmder1_driver(
+        3,
+        func,
+        jac,
+        guess * 10,
+        0.102956301410e03,
+        0.104467885065e-18,
+        [0.100000000000e01, 0.656391080516e-20, 0.000000000000e00],
+    )
+    _lmder1_driver(
+        3,
+        func,
+        jac,
+        guess * 100,
+        0.991261822124e03,
+        0.313877781195e-28,
+        [0.100000000000e01, -0.197215226305e-29, 0.000000000000e00],
+    )
 
 
 def _lmder1_powell_singular():
     """Powell's singular function (lmder test #6). Don't run this as a
     test, since it just zooms to zero parameters.  The precise results
     depend a lot on nitty-gritty rounding and tolerances and things."""
 
     def func(params, vec):
         vec[0] = params[0] + 10 * params[1]
         vec[1] = np.sqrt(5) * (params[2] - params[3])
-        vec[2] = (params[1] - 2 * params[2])**2
-        vec[3] = np.sqrt(10) * (params[0] - params[3])**2
+        vec[2] = (params[1] - 2 * params[2]) ** 2
+        vec[3] = np.sqrt(10) * (params[0] - params[3]) ** 2
 
     def jac(params, jac):
         jac.fill(0)
-        jac[0,0] = 1
-        jac[0,3] = 2 * np.sqrt(10) * (params[0] - params[3])
-        jac[1,0] = 10
-        jac[1,2] = 2 * (params[1] - 2 * params[2])
-        jac[2,1] = np.sqrt(5)
-        jac[2,2] = -2 * jac[2,1]
-        jac[3,1] = -np.sqrt(5)
-        jac[3,3] = -jac[3,0]
+        jac[0, 0] = 1
+        jac[0, 3] = 2 * np.sqrt(10) * (params[0] - params[3])
+        jac[1, 0] = 10
+        jac[1, 2] = 2 * (params[1] - 2 * params[2])
+        jac[2, 1] = np.sqrt(5)
+        jac[2, 2] = -2 * jac[2, 1]
+        jac[3, 1] = -np.sqrt(5)
+        jac[3, 3] = -jac[3, 0]
 
     guess = np.asfarray([3, -1, 0, 1])
 
     _lmder1_test(4, func, jac, guess)
     _lmder1_test(4, func, jac, guess * 10)
     _lmder1_test(4, func, jac, guess * 100)
 
@@ -2610,82 +2693,149 @@
 
     def func(params, vec):
         vec[0] = -13 + params[0] + ((5 - params[1]) * params[1] - 2) * params[1]
         vec[1] = -29 + params[0] + ((1 + params[1]) * params[1] - 14) * params[1]
 
     def jac(params, jac):
         jac[0] = 1
-        jac[1,0] = params[1] * (10 - 3 * params[1]) - 2
-        jac[1,1] = params[1] * (2 + 3 * params[1]) - 14
+        jac[1, 0] = params[1] * (10 - 3 * params[1]) - 2
+        jac[1, 1] = params[1] * (2 + 3 * params[1]) - 14
 
     guess = np.asfarray([0.5, -2])
 
-    _lmder1_driver(2, func, jac, guess,
-                   0.200124960962e+02, 0.699887517585e+01,
-                   [0.114124844655e+02, -0.896827913732e+00])
-    _lmder1_driver(2, func, jac, guess * 10,
-                   0.124328339489e+05, 0.699887517449e+01,
-                   [0.114130046615e+02, -0.896796038686e+00])
-    _lmder1_driver(2, func, jac, guess * 100,
-                   0.11426454595762e+08, 0.699887517243e+01,
-                   [0.114127817858e+02, -0.896805107492e+00])
+    _lmder1_driver(
+        2,
+        func,
+        jac,
+        guess,
+        0.200124960962e02,
+        0.699887517585e01,
+        [0.114124844655e02, -0.896827913732e00],
+    )
+    _lmder1_driver(
+        2,
+        func,
+        jac,
+        guess * 10,
+        0.124328339489e05,
+        0.699887517449e01,
+        [0.114130046615e02, -0.896796038686e00],
+    )
+    _lmder1_driver(
+        2,
+        func,
+        jac,
+        guess * 100,
+        0.11426454595762e08,
+        0.699887517243e01,
+        [0.114127817858e02, -0.896805107492e00],
+    )
 
 
 @test
 def _lmder1_bard():
     """Bard function (lmder1 test #8)"""
 
-    y1 = np.asfarray([0.14, 0.18, 0.22, 0.25, 0.29,
-                      0.32, 0.35, 0.39, 0.37, 0.58,
-                      0.73, 0.96, 1.34, 2.10, 4.39])
+    y1 = np.asfarray(
+        [
+            0.14,
+            0.18,
+            0.22,
+            0.25,
+            0.29,
+            0.32,
+            0.35,
+            0.39,
+            0.37,
+            0.58,
+            0.73,
+            0.96,
+            1.34,
+            2.10,
+            4.39,
+        ]
+    )
 
     def func(params, vec):
         for i in range(15):
             tmp2 = 15 - i
 
             if i > 7:
                 tmp3 = tmp2
             else:
                 tmp3 = i + 1
 
-            vec[i] = y1[i] - (params[0] + (i + 1) / (params[1] * tmp2 + params[2] * tmp3))
+            vec[i] = y1[i] - (
+                params[0] + (i + 1) / (params[1] * tmp2 + params[2] * tmp3)
+            )
 
     def jac(params, jac):
         for i in range(15):
             tmp2 = 15 - i
 
             if i > 7:
                 tmp3 = tmp2
             else:
                 tmp3 = i + 1
 
-            tmp4 = (params[1] * tmp2 + params[2] * tmp3)**2
-            jac[0,i] = -1
-            jac[1,i] = (i + 1) * tmp2 / tmp4
-            jac[2,i] = (i + 1) * tmp3 / tmp4
+            tmp4 = (params[1] * tmp2 + params[2] * tmp3) ** 2
+            jac[0, i] = -1
+            jac[1, i] = (i + 1) * tmp2 / tmp4
+            jac[2, i] = (i + 1) * tmp3 / tmp4
 
     guess = np.asfarray([1, 1, 1])
 
-    _lmder1_driver(15, func, jac, guess,
-                   0.6456136295159668e+01, 0.9063596033904667e-01,
-                   [0.8241057657583339e-01, 0.1133036653471504e+01, 0.2343694638941154e+01])
-    _lmder1_driver(15, func, jac, guess * 10,
-                   0.3614185315967845e+02, 0.4174768701385386e+01,
-                   [0.8406666738183293e+00, -0.1588480332595655e+09, -0.1643786716535352e+09])
-    _lmder1_driver(15, func, jac, guess * 100,
-                   0.3841146786373992e+03, 0.4174768701359691e+01,
-                   [0.8406666738676455e+00, -0.1589461672055184e+09, -0.1644649068577712e+09])
+    _lmder1_driver(
+        15,
+        func,
+        jac,
+        guess,
+        0.6456136295159668e01,
+        0.9063596033904667e-01,
+        [0.8241057657583339e-01, 0.1133036653471504e01, 0.2343694638941154e01],
+    )
+    _lmder1_driver(
+        15,
+        func,
+        jac,
+        guess * 10,
+        0.3614185315967845e02,
+        0.4174768701385386e01,
+        [0.8406666738183293e00, -0.1588480332595655e09, -0.1643786716535352e09],
+    )
+    _lmder1_driver(
+        15,
+        func,
+        jac,
+        guess * 100,
+        0.3841146786373992e03,
+        0.4174768701359691e01,
+        [0.8406666738676455e00, -0.1589461672055184e09, -0.1644649068577712e09],
+    )
 
 
 @test
 def _lmder1_kowalik_osborne():
     """Kowalik & Osborne function (lmder1 test #9)"""
     v = np.asfarray([4, 2, 1, 0.5, 0.25, 0.167, 0.125, 0.1, 0.0833, 0.0714, 0.0625])
-    y2 = np.asfarray([0.1957, 0.1947, 0.1735, 0.16, 0.0844, 0.0627, 0.0456,
-                      0.0342, 0.0323, 0.0235, 0.0246])
+    y2 = np.asfarray(
+        [
+            0.1957,
+            0.1947,
+            0.1735,
+            0.16,
+            0.0844,
+            0.0627,
+            0.0456,
+            0.0342,
+            0.0323,
+            0.0235,
+            0.0246,
+        ]
+    )
 
     def func(params, vec):
         tmp1 = v * (v + params[1])
         tmp2 = v * (v + params[2]) + params[3]
         vec[:] = y2 - params[0] * tmp1 / tmp2
 
     def jac(params, jac):
@@ -2694,39 +2844,76 @@
         jac[0] = -tmp1 / tmp2
         jac[1] = -v * params[0] / tmp2
         jac[2] = jac[0] * jac[1]
         jac[3] = jac[2] / v
 
     guess = np.asfarray([0.25, 0.39, 0.415, 0.39])
 
-    _lmder1_driver(11, func, jac, guess,
-                   0.7289151028829448e-01, 0.1753583772112895e-01,
-                   [0.1928078104762493e+00, 0.1912626533540709e+00,
-                    0.1230528010469309e+00, 0.1360532211505167e+00])
-    _lmder1_driver(11, func, jac, guess * 10,
-                   0.2979370075552020e+01, 0.3205219291793696e-01,
-                   [0.7286754737686598e+06, -0.1407588031293926e+02,
-                    -0.3297779778419661e+08, -0.2057159419780170e+08])
+    _lmder1_driver(
+        11,
+        func,
+        jac,
+        guess,
+        0.7289151028829448e-01,
+        0.1753583772112895e-01,
+        [
+            0.1928078104762493e00,
+            0.1912626533540709e00,
+            0.1230528010469309e00,
+            0.1360532211505167e00,
+        ],
+    )
+    _lmder1_driver(
+        11,
+        func,
+        jac,
+        guess * 10,
+        0.2979370075552020e01,
+        0.3205219291793696e-01,
+        [
+            0.7286754737686598e06,
+            -0.1407588031293926e02,
+            -0.3297779778419661e08,
+            -0.2057159419780170e08,
+        ],
+    )
 
     # This last test seems to rely on hitting maxfev in the solver.
     # Our stopping criterion is a bit different, so we go a bit farther.
     # I'm going to hope that's why our results are different.
-    #_lmder1_driver(11, func, jac, guess * 100,
+    # _lmder1_driver(11, func, jac, guess * 100,
     #               0.2995906170160365e+02, 0.1753583967605901e-01,
     #               [0.1927984063846549e+00, 0.1914736844615448e+00,
     #                0.1230924753714115e+00, 0.1361509629062244e+00])
 
 
 @test
 def _lmder1_meyer():
     """Meyer function (lmder1 test #10)"""
 
-    y3 = np.asarray([3.478e4, 2.861e4, 2.365e4, 1.963e4, 1.637e4, 1.372e4, 1.154e4,
-                     9.744e3, 8.261e3, 7.03e3, 6.005e3, 5.147e3, 4.427e3, 3.82e3,
-                     3.307e3, 2.872e3])
+    y3 = np.asarray(
+        [
+            3.478e4,
+            2.861e4,
+            2.365e4,
+            1.963e4,
+            1.637e4,
+            1.372e4,
+            1.154e4,
+            9.744e3,
+            8.261e3,
+            7.03e3,
+            6.005e3,
+            5.147e3,
+            4.427e3,
+            3.82e3,
+            3.307e3,
+            2.872e3,
+        ]
+    )
 
     def func(params, vec):
         temp = 5 * (np.arange(16) + 1) + 45 + params[2]
         tmp1 = params[1] / temp
         tmp2 = np.exp(tmp1)
         vec[:] = params[0] * tmp2 - y3
 
@@ -2736,31 +2923,36 @@
         tmp2 = np.exp(tmp1)
         jac[0] = tmp2
         jac[1] = params[0] * tmp2 / temp
         jac[2] = -tmp1 * jac[1]
 
     guess = np.asfarray([0.02, 4000, 250])
 
-    _lmder1_driver(16, func, jac, guess,
-                   0.4115346655430312e+05, 0.9377945146518742e+01,
-                   [0.5609636471026614e-02, 0.6181346346286591e+04,
-                    0.3452236346241440e+03])
+    _lmder1_driver(
+        16,
+        func,
+        jac,
+        guess,
+        0.4115346655430312e05,
+        0.9377945146518742e01,
+        [0.5609636471026614e-02, 0.6181346346286591e04, 0.3452236346241440e03],
+    )
     # This one depends on maxiter semantics.
-    #_lmder1_driver(16, func, jac, guess * 10,
+    # _lmder1_driver(16, func, jac, guess * 10,
     #               0.4168216891308465e+07, 0.7929178717795005e+03,
     #               [0.1423670741579940e-10, 0.3369571334325413e+05,
     #                0.9012685279538006e+03])
 
 
 @test
 def _lmder1_watson():
     """Watson function (lmder1 test #11)"""
 
     def func(params, vec):
-        div = (np.arange(29) + 1.) / 29
+        div = (np.arange(29) + 1.0) / 29
         s1 = 0
         dx = 1
 
         for j in range(1, params.size):
             s1 += j * dx * params[j]
             dx *= div
 
@@ -2769,92 +2961,215 @@
 
         for j in range(params.size):
             s2 += dx * params[j]
             dx *= div
 
         vec[:29] = s1 - s2**2 - 1
         vec[29] = params[0]
-        vec[30] = params[1] - params[0]**2 - 1
+        vec[30] = params[1] - params[0] ** 2 - 1
 
     def jac(params, jac):
         jac.fill(0)
-        div = (np.arange(29) + 1.) / 29
+        div = (np.arange(29) + 1.0) / 29
         s2 = 0
         dx = 1
 
         for j in range(params.size):
             s2 += dx * params[j]
             dx *= div
 
         temp = 2 * div * s2
-        dx = 1. / div
+        dx = 1.0 / div
 
         for j in range(params.size):
-            jac[j,:29] = dx * (j - temp)
+            jac[j, :29] = dx * (j - temp)
             dx *= div
 
-        jac[0,29] = 1
-        jac[0,30] = -2 * params[0]
-        jac[1,30] = 1
-
-    _lmder1_driver(31, func, jac, np.zeros(6),
-                   0.5477225575051661e+01, 0.4782959390976008e-01,
-                   [-0.1572496150837816e-01, 0.1012434882329655e+01,
-                    -0.2329917223876733e+00, 0.1260431011028184e+01,
-                    -0.1513730313944205e+01, 0.9929972729184200e+00])
-    _lmder1_driver(31, func, jac, np.zeros(6) + 10,
-                   0.6433125789500264e+04, 0.4782959390969513e-01,
-                   [-0.1572519013866769e-01, 0.1012434858601051e+01,
-                    -0.2329915458438287e+00, 0.1260429320891626e+01,
-                    -0.1513727767065747e+01, 0.9929957342632802e+00])
-    _lmder1_driver(31, func, jac, np.zeros(6) + 100,
-                   0.6742560406052133e+06, 0.4782959391154397e-01,
-                   [-0.1572470197125856e-01, 0.1012434909256583e+01,
-                    -0.2329919227616415e+00, 0.1260432929295546e+01,
-                    -0.1513733204527065e+01, 0.9929990192232198e+00])
-    _lmder1_driver(31, func, jac, np.zeros(9),
-                   0.5477225575051661e+01, 0.1183114592124197e-02,
-                   [-0.1530706441667223e-04, 0.9997897039345969e+00, 0.1476396349109780e-01,
-                    0.1463423301459916e+00, 0.1000821094548170e+01, -0.2617731120705071e+01,
-                    0.4104403139433541e+01, -0.3143612262362414e+01, 0.1052626403787590e+01],
-                   decimal=8) # good enough for me
-    _lmder1_driver(31, func, jac, np.zeros(9) + 10,
-                   0.1208812706930700e+05, 0.1183114592125130e-02,
-                   [-0.1530713348492787e-04, 0.9997897039412339e+00, 0.1476396297862168e-01,
-                    0.1463423348188364e+00, 0.1000821073213860e+01, -0.2617731070847222e+01,
-                    0.4104403076555641e+01, -0.3143612221786855e+01, 0.1052626393225894e+01],
-                   decimal=7) # ditto
-    _lmder1_driver(31, func, jac, np.zeros(9) + 100,
-                   0.1269109290438338e+07, 0.1183114592123836e-02,
-                   [-0.1530695233521759e-04, 0.9997897039583713e+00, 0.1476396251853923e-01,
-                    0.1463423410963262e+00, 0.1000821047291639e+01, -0.2617731015736446e+01,
-                    0.4104403014272860e+01, -0.3143612186025031e+01, 0.1052626385167739e+01],
-                   decimal=7)
+        jac[0, 29] = 1
+        jac[0, 30] = -2 * params[0]
+        jac[1, 30] = 1
+
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(6),
+        0.5477225575051661e01,
+        0.4782959390976008e-01,
+        [
+            -0.1572496150837816e-01,
+            0.1012434882329655e01,
+            -0.2329917223876733e00,
+            0.1260431011028184e01,
+            -0.1513730313944205e01,
+            0.9929972729184200e00,
+        ],
+    )
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(6) + 10,
+        0.6433125789500264e04,
+        0.4782959390969513e-01,
+        [
+            -0.1572519013866769e-01,
+            0.1012434858601051e01,
+            -0.2329915458438287e00,
+            0.1260429320891626e01,
+            -0.1513727767065747e01,
+            0.9929957342632802e00,
+        ],
+    )
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(6) + 100,
+        0.6742560406052133e06,
+        0.4782959391154397e-01,
+        [
+            -0.1572470197125856e-01,
+            0.1012434909256583e01,
+            -0.2329919227616415e00,
+            0.1260432929295546e01,
+            -0.1513733204527065e01,
+            0.9929990192232198e00,
+        ],
+    )
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(9),
+        0.5477225575051661e01,
+        0.1183114592124197e-02,
+        [
+            -0.1530706441667223e-04,
+            0.9997897039345969e00,
+            0.1476396349109780e-01,
+            0.1463423301459916e00,
+            0.1000821094548170e01,
+            -0.2617731120705071e01,
+            0.4104403139433541e01,
+            -0.3143612262362414e01,
+            0.1052626403787590e01,
+        ],
+        decimal=8,
+    )  # good enough for me
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(9) + 10,
+        0.1208812706930700e05,
+        0.1183114592125130e-02,
+        [
+            -0.1530713348492787e-04,
+            0.9997897039412339e00,
+            0.1476396297862168e-01,
+            0.1463423348188364e00,
+            0.1000821073213860e01,
+            -0.2617731070847222e01,
+            0.4104403076555641e01,
+            -0.3143612221786855e01,
+            0.1052626393225894e01,
+        ],
+        decimal=7,
+    )  # ditto
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(9) + 100,
+        0.1269109290438338e07,
+        0.1183114592123836e-02,
+        [
+            -0.1530695233521759e-04,
+            0.9997897039583713e00,
+            0.1476396251853923e-01,
+            0.1463423410963262e00,
+            0.1000821047291639e01,
+            -0.2617731015736446e01,
+            0.4104403014272860e01,
+            -0.3143612186025031e01,
+            0.1052626385167739e01,
+        ],
+        decimal=7,
+    )
     # I've hacked params[0] below to agree with the Python since most everything else
     # is a lot closer. Fortran value is -0.6602660013963822D-08.
-    _lmder1_driver(31, func, jac, np.zeros(12),
-                   0.5477225575051661e+01, 0.2173104025358612e-04,
-                   [-0.66380604e-08, 0.1000001644118327e+01, -0.5639321469801545e-03,
-                    0.3478205400507559e+00, -0.1567315002442332e+00, 0.1052815158255932e+01,
-                    -0.3247271095194506e+01, 0.7288434783750497e+01, -0.1027184809861398e+02,
-                    0.9074113537157828e+01, -0.4541375419181941e+01, 0.1012011879750439e+01],
-                   decimal=7)
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(12),
+        0.5477225575051661e01,
+        0.2173104025358612e-04,
+        [
+            -0.66380604e-08,
+            0.1000001644118327e01,
+            -0.5639321469801545e-03,
+            0.3478205400507559e00,
+            -0.1567315002442332e00,
+            0.1052815158255932e01,
+            -0.3247271095194506e01,
+            0.7288434783750497e01,
+            -0.1027184809861398e02,
+            0.9074113537157828e01,
+            -0.4541375419181941e01,
+            0.1012011879750439e01,
+        ],
+        decimal=7,
+    )
     # These last two don't need any hacking or decimal < 10 ...
-    _lmder1_driver(31, func, jac, np.zeros(12) + 10,
-                   0.1922075897909507e+05, 0.2173104025185086e-04,
-                   [-0.6637102230174097e-08, 0.1000001644117873e+01, -0.5639322083473270e-03,
-                    0.3478205404869979e+00, -0.1567315039556524e+00, 0.1052815176545732e+01,
-                    -0.3247271151521395e+01, 0.7288434894306651e+01, -0.1027184823696385e+02,
-                    0.9074113643837332e+01, -0.4541375465336661e+01, 0.1012011888308566e+01],
-                   decimal=7)
-    _lmder1_driver(31, func, jac, np.zeros(12) + 100,
-                   0.2018918044623666e+07, 0.2173104025398453e-04,
-                   [-0.6638060464852487e-08, 0.1000001644117862e+01, -0.5639322103249589e-03,
-                    0.3478205405035875e+00, -0.1567315040913747e+00, 0.1052815177180306e+01,
-                    -0.3247271153370249e+01, 0.7288434897753017e+01, -0.1027184824108129e+02,
-                    0.9074113646884637e+01, -0.4541375466608216e+01, 0.1012011888536897e+01])
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(12) + 10,
+        0.1922075897909507e05,
+        0.2173104025185086e-04,
+        [
+            -0.6637102230174097e-08,
+            0.1000001644117873e01,
+            -0.5639322083473270e-03,
+            0.3478205404869979e00,
+            -0.1567315039556524e00,
+            0.1052815176545732e01,
+            -0.3247271151521395e01,
+            0.7288434894306651e01,
+            -0.1027184823696385e02,
+            0.9074113643837332e01,
+            -0.4541375465336661e01,
+            0.1012011888308566e01,
+        ],
+        decimal=7,
+    )
+    _lmder1_driver(
+        31,
+        func,
+        jac,
+        np.zeros(12) + 100,
+        0.2018918044623666e07,
+        0.2173104025398453e-04,
+        [
+            -0.6638060464852487e-08,
+            0.1000001644117862e01,
+            -0.5639322103249589e-03,
+            0.3478205405035875e00,
+            -0.1567315040913747e00,
+            0.1052815177180306e01,
+            -0.3247271153370249e01,
+            0.7288434897753017e01,
+            -0.1027184824108129e02,
+            0.9074113646884637e01,
+            -0.4541375466608216e01,
+            0.1012011888536897e01,
+        ],
+    )
 
 
 # Finally ...
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     _runtests()
```

### Comparing `pwkit-1.1.1/pwkit/lsqmdl.py` & `pwkit-1.2.0/pwkit/lsqmdl.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,43 @@
 
 This module provides tools for fitting models to data using least-squares
 optimization.
 
 """
 from __future__ import absolute_import, division, print_function
 
-__all__ = 'ModelBase Model ComposedModel PolynomialModel ScaleModel'.split()
+__all__ = "ModelBase Model ComposedModel PolynomialModel ScaleModel".split()
 
 import numpy as np
+
 try:
     # numpy 1.7
     import numpy.polynomial.polynomial as npoly
 except ImportError:
     import numpy.polynomial as npoly
 
-from six import get_function_code
-from six.moves import range, reduce
-from . import binary_type, text_type
-
 
 class Parameter(object):
     """Information about a parameter in a least-squares model.
 
     These data may only be obtained after solving least-squares problem. These
     objects reference information from their parent objects, so changing the
     parent will alter the apparent contents of these objects.
 
     """
+
     def __init__(self, owner, index):
         self._owner = owner
         self._index = index
 
     def __repr__(self):
         return '<Parameter "%s" (#%d) of %s>' % (self.name, self._index, self._owner)
 
     @property
-    def index(self): # make this read-only
+    def index(self):  # make this read-only
         "The parameter's index in the Model's arrays."
         return self._index
 
     @property
     def name(self):
         "The parameter's name."
         return self._owner.pnames[self._index]
@@ -59,14 +57,15 @@
         "The uncertainty in :attr:`value`."
         return self._owner.puncerts[self._index]
 
     @property
     def uval(self):
         "Accesses :attr:`value` and :attr:`uncert` as a :class:`pwkit.msmt.Uval`."
         from .msmt import Uval
+
         return Uval.from_norm(self.value, self.uncert)
 
 
 class ModelBase(object):
     """An abstract base class holding data and a model for least-squares fitting.
 
     The models implemented in this module all derive from this class and so
@@ -76,14 +75,15 @@
     object with either the parameter's numerical index or its name. I.e.::
 
       m = Model(...).solve(...)
       p = m['slope']
       print(p.name, p.value, p.uncert, p.uval)
 
     """
+
     data = None
     "The data to be modeled; an *n*-dimensional Numpy array."
 
     invsigma = None
     "Data weights: 1/σ for each data point."
 
     params = None
@@ -118,141 +118,142 @@
 
     resids = None
     "After fitting, the residuals: ``resids = data - mdata``."
 
     def __init__(self, data, invsigma=None):
         self.set_data(data, invsigma)
 
-
     def set_data(self, data, invsigma=None):
         """Set the data to be modeled.
 
         Returns *self*.
 
         """
         self.data = np.array(data, dtype=float, ndmin=1)
 
         if invsigma is None:
             self.invsigma = np.ones(self.data.shape)
         else:
             i = np.array(invsigma, dtype=float)
-            self.invsigma = np.broadcast_arrays(self.data, i)[1] # allow scalar invsigma
+            self.invsigma = np.broadcast_arrays(self.data, i)[
+                1
+            ]  # allow scalar invsigma
 
         if self.invsigma.shape != self.data.shape:
-            raise ValueError('data values and inverse-sigma values must have same shape')
+            raise ValueError(
+                "data values and inverse-sigma values must have same shape"
+            )
 
         return self
 
-
     def print_soln(self):
         """Print information about the model solution."""
-        lmax = reduce(max,(len(x) for x in self.pnames), len('r chi sq'))
+        lmax = reduce(max, (len(x) for x in self.pnames), len("r chi sq"))
 
         if self.puncerts is None:
             for pn, val in zip(self.pnames, self.params):
-                print('%s: %14g' % (pn.rjust(lmax), val))
+                print("%s: %14g" % (pn.rjust(lmax), val))
         else:
             for pn, val, err in zip(self.pnames, self.params, self.puncerts):
-                frac = abs(100. * err / val)
-                print('%s: %14g +/- %14g (%.2f%%)' % (pn.rjust(lmax), val, err, frac))
+                frac = abs(100.0 * err / val)
+                print("%s: %14g +/- %14g (%.2f%%)" % (pn.rjust(lmax), val, err, frac))
 
         if self.rchisq is not None:
-            print('%s: %14g' % ('r chi sq'.rjust(lmax), self.rchisq))
+            print("%s: %14g" % ("r chi sq".rjust(lmax), self.rchisq))
         elif self.chisq is not None:
-            print('%s: %14g' % ('chi sq'.rjust(lmax), self.chisq))
+            print("%s: %14g" % ("chi sq".rjust(lmax), self.chisq))
         else:
-            print('%s: unknown/undefined' % ('r chi sq'.rjust(lmax)))
+            print("%s: unknown/undefined" % ("r chi sq".rjust(lmax)))
         return self
 
-
     def make_frozen_func(self, params):
         """Return a data-generating model function frozen at the specified parameters.
 
         As with the :attr:`mfunc` attribute, the resulting function may or may
         not take arguments depending on the particular kind of model being
         evaluated.
 
         """
         raise NotImplementedError()
 
-
     def __getitem__(self, key):
-        if isinstance(key, binary_type):
+        if isinstance(key, bytes):
             # If you're not using the unicode_literals __future__, things get
             # annoying really quickly without this.
-            key = text_type(key)
+            key = str(key)
 
         if isinstance(key, int):
             idx = key
             if idx < 0 or idx >= len(self.pnames):
-                raise ValueError('illegal parameter number %d' % key)
-        elif isinstance(key, text_type):
+                raise ValueError("illegal parameter number %d" % key)
+        elif isinstance(key, str):
             try:
                 idx = self.pnames.index(key)
             except ValueError:
                 raise ValueError('no such parameter named "%s"' % key)
         else:
-            raise ValueError('illegal parameter key %r' % key)
+            raise ValueError("illegal parameter key %r" % key)
 
         return Parameter(self, idx)
 
-
-    def plot(self, modelx, dlines=False, xmin=None, xmax=None,
-             ymin=None, ymax=None, **kwargs):
+    def plot(
+        self, modelx, dlines=False, xmin=None, xmax=None, ymin=None, ymax=None, **kwargs
+    ):
         """Plot the data and model (requires `omega`).
 
         This assumes that `data` is 1D and that `mfunc` takes one argument
         that should be treated as the X variable.
 
         """
         import omega as om
 
         modelx = np.asarray(modelx)
         if modelx.shape != self.data.shape:
-            raise ValueError('modelx and data arrays must have same shape')
+            raise ValueError("modelx and data arrays must have same shape")
 
         modely = self.mfunc(modelx)
-        sigmas = self.invsigma**-1 # TODO: handle invsigma = 0
+        sigmas = self.invsigma**-1  # TODO: handle invsigma = 0
 
         vb = om.layout.VBox(2)
-        vb.pData = om.quickXYErr(modelx, self.data, sigmas,
-                                 'Data', lines=dlines, **kwargs)
+        vb.pData = om.quickXYErr(
+            modelx, self.data, sigmas, "Data", lines=dlines, **kwargs
+        )
 
         vb[0] = vb.pData
-        vb[0].addXY(modelx, modely, 'Model')
-        vb[0].setYLabel('Y')
+        vb[0].addXY(modelx, modely, "Model")
+        vb[0].setYLabel("Y")
         vb[0].rebound(False, True)
         vb[0].setBounds(xmin, xmax, ymin, ymax)
 
         vb[1] = vb.pResid = om.RectPlot()
         vb[1].defaultField.xaxis = vb[1].defaultField.xaxis
         vb[1].addXYErr(modelx, self.resids, sigmas, None, lines=False)
-        vb[1].setLabels('X', 'Residuals')
+        vb[1].setLabels("X", "Residuals")
         vb[1].rebound(False, True)
         # ignore Y values since residuals are on different scale:
         vb[1].setBounds(xmin, xmax)
 
         vb.setWeight(0, 3)
         return vb
 
-
     def show_cov(self):
         "Show the parameter covariance matrix with `pwkit.ndshow_gtk3`."
         # would be nice: labels with parameter names (hard because this is
         # ndshow, not omegaplot)
         from .ndshow_gtk3 import view
-        view(self.covar, title='Covariance Matrix')
 
+        view(self.covar, title="Covariance Matrix")
 
     def show_corr(self):
         "Show the parameter correlation matrix with `pwkit.ndshow_gtk3`."
         from .ndshow_gtk3 import view
+
         d = np.diag(self.covar) ** -0.5
-        corr = self.covar * d[np.newaxis,:] * d[:,np.newaxis]
-        view(corr, title='Correlation Matrix')
+        corr = self.covar * d[np.newaxis, :] * d[:, np.newaxis]
+        view(corr, title="Correlation Matrix")
 
 
 class Model(ModelBase):
     """Models data with a generic nonlinear optimizer
 
     Basic usage is::
 
@@ -276,28 +277,29 @@
       m = Model(func, data, uncerts) # WRONG
 
     If you have zero uncertainty on a measurement, you must wind a way to
     express that constraint without including that measurement as part of the
     ``data`` vector.
 
     """
+
     lm_prob = None
     """A :class:`pwkit.lmmin.Problem` instance describing the problem to be solved.
 
     After setting up the data-generating function, you can access this item to
     tune the solver.
 
     """
+
     def __init__(self, simple_func, data, invsigma=None, args=()):
         if simple_func is not None:
             self.set_simple_func(simple_func, args)
         if data is not None:
             self.set_data(data, invsigma)
 
-
     def set_func(self, func, pnames, args=()):
         """Set the model function to use an efficient but tedious calling convention.
 
         The function should obey the following convention::
 
             def func(param_vec, *args):
                 modeled_data = { do something using param_vec }
@@ -313,52 +315,50 @@
 
         self.func = func
         self._args = args
         self.pnames = list(pnames)
         self.lm_prob = Problem(len(self.pnames))
         return self
 
-
     def set_simple_func(self, func, args=()):
         """Set the model function to use a simple but somewhat inefficient calling
         convention.
 
         The function should obey the following convention::
 
             def func(param0, param1, ..., paramN, *args):
                 modeled_data = { do something using the parameters }
                 return modeled_data
 
         Returns *self*.
 
         """
-        code = get_function_code(func)
+        code = func.__code__
         npar = code.co_argcount - len(args)
         pnames = code.co_varnames[:npar]
 
         def wrapper(params, *args):
             return func(*(tuple(params) + args))
 
         return self.set_func(wrapper, pnames, args)
 
-
     def make_frozen_func(self, params):
         """Returns a model function frozen to the specified parameter values.
 
         Any remaining arguments are left free and must be provided when the
         function is called.
 
         For this model, the returned function is the application of
         :func:`functools.partial` to the :attr:`func` property of this object.
 
         """
         params = np.array(params, dtype=float, ndmin=1)
         from functools import partial
-        return partial(self.func, params)
 
+        return partial(self.func, params)
 
     def solve(self, guess):
         """Solve for the parameters, using an initial guess.
 
         This uses the Levenberg-Marquardt optimizer described in
         :mod:`pwkit.lmmin`.
 
@@ -368,17 +368,17 @@
         guess = np.array(guess, dtype=float, ndmin=1)
         f = self.func
         args = self._args
 
         def lmfunc(params, vec):
             vec[:] = f(params, *args).flatten()
 
-        self.lm_prob.set_residual_func(self.data.flatten(),
-                                       self.invsigma.flatten(),
-                                       lmfunc, None)
+        self.lm_prob.set_residual_func(
+            self.data.flatten(), self.invsigma.flatten(), lmfunc, None
+        )
         self.lm_soln = soln = self.lm_prob.solve(guess)
 
         self.params = soln.params
         self.puncerts = soln.perror
         self.covar = soln.covar
         self.mfunc = self.make_frozen_func(soln.params)
 
@@ -409,98 +409,94 @@
     uncertainties.
 
     Methods:
 
     as_nonlinear - Return a (lmmin-based) `Model` equivalent to self.
 
     """
+
     def __init__(self, maxexponent, x, data, invsigma=None):
         self.maxexponent = maxexponent
         self.x = np.array(x, dtype=float, ndmin=1, copy=False, subok=True)
         self.set_data(data, invsigma)
 
-
     def make_frozen_func(self, params):
         return lambda x: npoly.polyval(x, params)
 
-
     def solve(self):
-        self.pnames = ['a%d' % i for i in range(self.maxexponent + 1)]
-        self.params = npoly.polyfit(self.x, self.data, self.maxexponent,
-                                    w=self.invsigma)
-        self.puncerts = None # does anything provide this? could farm out to lmmin ...
+        self.pnames = ["a%d" % i for i in range(self.maxexponent + 1)]
+        self.params = npoly.polyfit(
+            self.x, self.data, self.maxexponent, w=self.invsigma
+        )
+        self.puncerts = None  # does anything provide this? could farm out to lmmin ...
         self.covar = None
         self.mfunc = self.make_frozen_func(self.params)
         self.mdata = self.mfunc(self.x)
         self.resids = self.data - self.mdata
 
-        self.chisq = ((self.resids * self.invsigma)**2).sum()
+        self.chisq = ((self.resids * self.invsigma) ** 2).sum()
         if self.x.size > self.maxexponent + 1:
             self.rchisq = self.chisq / (self.x.size - (self.maxexponent + 1))
 
         return self
 
-
     def as_nonlinear(self, params=None):
         """Return a `Model` equivalent to this object. The nonlinear solver is less
         efficient, but lets you freeze parameters, compute uncertainties, etc.
 
         If the `params` argument is provided, solve() will be called on the
         returned object with those parameters. If it is `None` and this object
         has parameters in `self.params`, those will be use. Otherwise, solve()
         will not be called on the returned object.
 
         """
         if params is None:
             params = self.params
 
         nlm = Model(None, self.data, self.invsigma)
-        nlm.set_func(lambda p, x: npoly.polyval(x, p),
-                     self.pnames,
-                     args=(self.x,))
+        nlm.set_func(lambda p, x: npoly.polyval(x, p), self.pnames, args=(self.x,))
 
         if params is not None:
             nlm.solve(params)
         return nlm
 
 
 class ScaleModel(ModelBase):
     """Solve `data = m * x` for `m`."""
 
     def __init__(self, x, data, invsigma=None):
         self.x = np.array(x, dtype=float, ndmin=1, copy=False, subok=True)
         self.set_data(data, invsigma)
 
-
     def make_frozen_func(self, params):
         return lambda x: params[0] * x
 
-
     def solve(self):
         w2 = self.invsigma**2
         sxx = np.dot(self.x**2, w2)
         sxy = np.dot(self.x * self.data, w2)
         m = sxy / sxx
-        uc_m = 1. / np.sqrt(sxx)
+        uc_m = 1.0 / np.sqrt(sxx)
 
-        self.pnames = ['m']
+        self.pnames = ["m"]
         self.params = np.asarray([m])
         self.puncerts = np.asarray([uc_m])
         self.covar = self.puncerts.reshape((1, 1))
         self.mfunc = lambda x: m * x
         self.mdata = m * self.x
         self.resids = self.data - self.mdata
-        self.chisq = ((self.resids * self.invsigma)**2).sum()
+        self.chisq = ((self.resids * self.invsigma) ** 2).sum()
         self.rchisq = self.chisq / (self.x.size - 1)
         return self
 
 
 # lmmin-based model-fitting when the model is broken down into composable
 # components.
 
+
 class ModelComponent(object):
     npar = 0
     name = None
     pnames = ()
     nmodelargs = 0
 
     setguess = None
@@ -549,68 +545,67 @@
         size has to be a function of the "free" parameters to the model
         function that are implicit/fixed during the fitting process. Given these "free"
         parameters, _outputshape returns the shape that the output will have."""
         raise NotImplementedError()
 
     def mfunc(self, *args):
         if len(args) != self.nmodelargs:
-            raise TypeError('model function expected %d arguments, got %d' %
-                            (self.nmodelargs, len(args)))
+            raise TypeError(
+                "model function expected %d arguments, got %d"
+                % (self.nmodelargs, len(args))
+            )
 
         result = np.zeros(self._outputshape(*args))
         self._accum_mfunc(result, *args)
         return result
 
 
 class ComposedModel(ModelBase):
     def __init__(self, component, data, invsigma=None):
         if component is not None:
             self.set_component(component)
         if data is not None:
             self.set_data(data, invsigma)
 
-
     def _component_setguess(self, vals, ofs=0):
         vals = np.asarray(vals)
         if ofs < 0 or ofs + vals.size > self.component.npar:
-            raise ValueError('ofs %d, vals.size %d, npar %d' %
-                             (ofs, vals.size, self.component.npar))
-        self.force_guess[ofs:ofs+vals.size] = vals
-
+            raise ValueError(
+                "ofs %d, vals.size %d, npar %d" % (ofs, vals.size, self.component.npar)
+            )
+        self.force_guess[ofs : ofs + vals.size] = vals
 
     def _component_setvalue(self, cidx, val, fixed=False):
         if cidx < 0 or cidx >= self.component.npar:
-            raise ValueError('cidx %d, npar %d' % (cidx, self.component.npar))
+            raise ValueError("cidx %d, npar %d" % (cidx, self.component.npar))
         self.lm_prob.p_value(cidx, val, fixed=fixed)
         self.force_guess[cidx] = val
 
-
     def _component_setlimit(self, cidx, lower=-np.inf, upper=np.inf):
         if cidx < 0 or cidx >= self.component.npar:
-            raise ValueError('cidx %d, npar %d' % (cidx, self.component.npar))
+            raise ValueError("cidx %d, npar %d" % (cidx, self.component.npar))
         self.lm_prob.p_limit(cidx, lower, upper)
 
-
     def set_component(self, component):
         self.component = component
 
         component.setguess = self._component_setguess
         component.setvalue = self._component_setvalue
         component.setlimit = self._component_setlimit
         component.finalize_setup()
 
         from .lmmin import Problem
+
         self.lm_prob = Problem(component.npar)
         self.force_guess = np.empty(component.npar)
         self.force_guess.fill(np.nan)
         self.pnames = list(component._param_names())
 
         component.prep_params()
 
-
     def solve(self, guess=None):
         if guess is None:
             guess = self.force_guess
         else:
             guess = np.array(guess, dtype=float, ndmin=1, copy=True)
 
             for i in range(self.force_guess.size):
@@ -619,16 +614,17 @@
 
         def model(pars, outputs):
             outputs.fill(0)
             self.component.model(pars, outputs)
 
         self.lm_model = model
         self.lm_deriv = self.component.deriv
-        self.lm_prob.set_residual_func(self.data, self.invsigma, model,
-                                       self.component.deriv)
+        self.lm_prob.set_residual_func(
+            self.data, self.invsigma, model, self.component.deriv
+        )
         self.lm_soln = soln = self.lm_prob.solve(guess)
 
         self.params = soln.params
         self.puncerts = soln.perror
         self.covar = soln.covar
 
         # fvec = resids * invsigma = (data - mdata) * invsigma
@@ -639,82 +635,85 @@
         self.chisq = (self.lm_soln.fvec**2).sum()
         if soln.ndof > 0:
             self.rchisq = self.chisq / soln.ndof
 
         self.component.extract(soln.params, soln.perror, soln.covar)
         return self
 
-
     def make_frozen_func(self):
         return self.component.mfunc
 
-
     def mfunc(self, *args):
         return self.component.mfunc(*args)
 
-
     def debug_derivative(self, guess):
         """returns (explicit, auto)"""
         from .lmmin import check_derivative
-        return check_derivative(self.component.npar, self.data.size,
-                                self.lm_model, self.lm_deriv, guess)
+
+        return check_derivative(
+            self.component.npar, self.data.size, self.lm_model, self.lm_deriv, guess
+        )
 
 
 # Now specific components useful in the above framework. The general strategy
 # is to err on the side of having additional parameters in the individual
 # classes, and the user can call setvalue() to fix them if they're not needed.
 
+
 class AddConstantComponent(ModelComponent):
     npar = 1
-    pnames = ('value', )
+    pnames = ("value",)
     nmodelargs = 0
 
     def model(self, pars, mdata):
         mdata += pars[0]
 
     def deriv(self, pars, jac):
-        jac[0] = 1.
+        jac[0] = 1.0
 
     def _outputshape(self):
-        return()
+        return ()
 
     def extract(self, pars, perr, cov):
         def _accum_mfunc(res):
             res += pars[0]
+
         self._accum_mfunc = _accum_mfunc
 
         self.covar = cov
         self.f_value = pars[0]
         self.u_value = perr[0]
 
 
 class AddValuesComponent(ModelComponent):
     """XXX terminology between this and AddConstant is mushy."""
+
     nmodelargs = 0
 
     def __init__(self, nvals, name=None):
         super(AddValuesComponent, self).__init__(name)
         self.npar = nvals
 
     def _param_names(self):
         for i in range(self.npar):
-            yield 'v%d' % i
+            yield "v%d" % i
 
     def model(self, pars, mdata):
         mdata += pars
 
     def deriv(self, pars, jac):
-        jac[:,:] = np.eye(self.npar)
+        jac[:, :] = np.eye(self.npar)
 
     def _outputshape(self):
-        return(self.npar,)
+        return (self.npar,)
 
     def extract(self, pars, perr, cov):
         def _accum_mfunc(res):
             res += pars
+
         self._accum_mfunc = _accum_mfunc
 
         self.covar = cov
         self.f_vals = pars
         self.u_vals = perr
 
 
@@ -724,15 +723,15 @@
     def __init__(self, maxexponent, x, name=None):
         super(AddPolynomialComponent, self).__init__(name)
         self.npar = maxexponent + 1
         self.x = np.array(x, dtype=float, ndmin=1, copy=False, subok=True)
 
     def _param_names(self):
         for i in range(self.npar):
-            yield 'c%d' % i
+            yield "c%d" % i
 
     def model(self, pars, mdata):
         mdata += npoly.polyval(self.x, pars)
 
     def deriv(self, pars, jac):
         w = np.ones_like(self.x)
 
@@ -742,14 +741,15 @@
 
     def _outputshape(self, x):
         return x.shape
 
     def extract(self, pars, perr, cov):
         def _accum_mfunc(res, x):
             res += npoly.polyval(x, pars)
+
         self._accum_mfunc = _accum_mfunc
 
         self.covar = cov
         self.f_coeffs = pars
         self.u_coeffs = perr
 
 
@@ -762,151 +762,140 @@
     n = max(n1, n2)
     res = [1] * n
 
     for i in range(n):
         if i >= n1:
             c1 = 1
         else:
-            c1 = s1[n1-1-i]
+            c1 = s1[n1 - 1 - i]
 
         if i >= n2:
             c2 = 1
         else:
-            c2 = s2[n2-1-i]
+            c2 = s2[n2 - 1 - i]
 
         if c1 == 1:
             rc = c2
         elif c2 == 1 or c1 == c2:
             rc = c1
         else:
-            raise ValueError('array shapes %r and %r are not compatible' % (s1, s2))
+            raise ValueError("array shapes %r and %r are not compatible" % (s1, s2))
 
-        res[n-1-i] = rc
+        res[n - 1 - i] = rc
 
     return tuple(res)
 
 
 class SeriesComponent(ModelComponent):
     """Apply a set of subcomponents in series, isolating each from the other. This
     is only valid if every subcomponent except the first is additive --
     otherwise, the Jacobian won't be right."""
 
     def __init__(self, components=(), name=None):
         super(SeriesComponent, self).__init__(name)
         self.components = list(components)
 
-
     def add(self, component):
         """This helps, but direct manipulation of self.components should be
         supported."""
         self.components.append(component)
         return self
 
-
     def _param_names(self):
         for c in self.components:
-            pfx = c.name + '.' if c.name is not None else ''
+            pfx = c.name + "." if c.name is not None else ""
             for p in c._param_names():
                 yield pfx + p
 
-
     def _offset_setguess(self, ofs, npar, vals, subofs=0):
         vals = np.asarray(vals)
         if subofs < 0 or subofs + vals.size > npar:
-            raise ValueError('subofs %d, vals.size %d, npar %d' %
-                             (subofs, vals.size, npar))
+            raise ValueError(
+                "subofs %d, vals.size %d, npar %d" % (subofs, vals.size, npar)
+            )
         return self.setguess(vals, ofs + subofs)
 
-
     def _offset_setvalue(self, ofs, npar, cidx, value, fixed=False):
         if cidx < 0 or cidx >= npar:
-            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+            raise ValueError("cidx %d, npar %d" % (cidx, npar))
         return self.setvalue(ofs + cidx, value, fixed)
 
-
     def _offset_setlimit(self, ofs, npar, cidx, lower=-np.inf, upper=np.inf):
         if cidx < 0 or cidx >= npar:
-            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+            raise ValueError("cidx %d, npar %d" % (cidx, npar))
         return self.setlimit(ofs + cidx, lower, upper)
 
-
     def finalize_setup(self):
         from functools import partial
 
         ofs = 0
         self.nmodelargs = 0
 
         for i, c in enumerate(self.components):
             if c.name is None:
-                c.name = 'c%d' % i
+                c.name = "c%d" % i
 
             c.setguess = partial(self._offset_setguess, ofs, c.npar)
             c.setvalue = partial(self._offset_setvalue, ofs, c.npar)
             c.setlimit = partial(self._offset_setlimit, ofs, c.npar)
             c.finalize_setup()
             ofs += c.npar
             self.nmodelargs += c.nmodelargs
 
         self.npar = ofs
 
-
     def prep_params(self):
         for c in self.components:
             c.prep_params()
 
-
     def model(self, pars, mdata):
         ofs = 0
 
         for c in self.components:
-            p = pars[ofs:ofs+c.npar]
+            p = pars[ofs : ofs + c.npar]
             c.model(p, mdata)
             ofs += c.npar
 
-
     def deriv(self, pars, jac):
         ofs = 0
 
         for c in self.components:
-            p = pars[ofs:ofs+c.npar]
-            j = jac[ofs:ofs+c.npar]
+            p = pars[ofs : ofs + c.npar]
+            j = jac[ofs : ofs + c.npar]
             c.deriv(p, j)
             ofs += c.npar
 
-
     def extract(self, pars, perr, cov):
         ofs = 0
 
         for c in self.components:
             n = c.npar
 
-            spar = pars[ofs:ofs+n]
-            serr = perr[ofs:ofs+n]
-            scov = cov[ofs:ofs+n,ofs:ofs+n]
+            spar = pars[ofs : ofs + n]
+            serr = perr[ofs : ofs + n]
+            scov = cov[ofs : ofs + n, ofs : ofs + n]
             c.extract(spar, serr, scov)
             ofs += n
 
-
     def _outputshape(self, *args):
         s = ()
         ofs = 0
 
         for c in self.components:
-            cargs = args[ofs:ofs+c.nmodelargs]
+            cargs = args[ofs : ofs + c.nmodelargs]
             s = _broadcast_shapes(s, c._outputshape(*cargs))
             ofs += c.nmodelargs
 
         return s
 
-
     def _accum_mfunc(self, res, *args):
         ofs = 0
 
         for c in self.components:
-            cargs = args[ofs:ofs+c.nmodelargs]
+            cargs = args[ofs : ofs + c.nmodelargs]
             c._accum_mfunc(res, *cargs)
             ofs += c.nmodelargs
 
 
 class MatMultComponent(ModelComponent):
     """Given a component yielding k**2 data points and k additional components,
     each yielding n data points. The result is [A]×[B], where A is the square
@@ -918,251 +907,228 @@
 
     def __init__(self, k, name=None):
         super(MatMultComponent, self).__init__(name)
         self.k = k
         self.acomponent = None
         self.bcomponents = [None] * k
 
-
     def _param_names(self):
-        pfx = self.acomponent.name + '.' if self.acomponent.name is not None else ''
+        pfx = self.acomponent.name + "." if self.acomponent.name is not None else ""
         for p in self.acomponent._param_names():
             yield pfx + p
 
         for c in self.bcomponents:
-            pfx = c.name + '.' if c.name is not None else ''
+            pfx = c.name + "." if c.name is not None else ""
             for p in c._param_names():
                 yield pfx + p
 
-
     def _offset_setguess(self, ofs, npar, vals, subofs=0):
         vals = np.asarray(vals)
         if subofs < 0 or subofs + vals.size > npar:
-            raise ValueError('subofs %d, vals.size %d, npar %d' %
-                             (subofs, vals.size, npar))
+            raise ValueError(
+                "subofs %d, vals.size %d, npar %d" % (subofs, vals.size, npar)
+            )
         return self.setguess(vals, ofs + subofs)
 
-
     def _offset_setvalue(self, ofs, npar, cidx, value, fixed=False):
         if cidx < 0 or cidx >= npar:
-            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+            raise ValueError("cidx %d, npar %d" % (cidx, npar))
         return self.setvalue(ofs + cidx, value, fixed)
 
-
     def _offset_setlimit(self, ofs, npar, cidx, lower=-np.inf, upper=np.inf):
         if cidx < 0 or cidx >= npar:
-            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+            raise ValueError("cidx %d, npar %d" % (cidx, npar))
         return self.setlimit(ofs + cidx, lower, upper)
 
-
     def finalize_setup(self):
         from functools import partial
 
         c = self.acomponent
 
         if c.name is None:
-            c.name = 'a'
+            c.name = "a"
 
         c.setguess = partial(self._offset_setguess, 0, c.npar)
         c.setvalue = partial(self._offset_setvalue, 0, c.npar)
         c.setlimit = partial(self._offset_setlimit, 0, c.npar)
         c.finalize_setup()
         ofs = c.npar
         self.nmodelargs = c.nmodelargs
 
         for i, c in enumerate(self.bcomponents):
             if c.name is None:
-                c.name = 'b%d' % i
+                c.name = "b%d" % i
 
             c.setguess = partial(self._offset_setguess, ofs, c.npar)
             c.setvalue = partial(self._offset_setvalue, ofs, c.npar)
             c.setlimit = partial(self._offset_setlimit, ofs, c.npar)
             c.finalize_setup()
             ofs += c.npar
             self.nmodelargs += c.nmodelargs
 
         self.npar = ofs
 
-
     def prep_params(self):
         self.acomponent.prep_params()
 
         for c in self.bcomponents:
             c.prep_params()
 
-
     def _sep_model(self, pars, nd):
         k = self.k
         ma = np.zeros((k, k))
         mb = np.zeros((k, nd))
 
         c = self.acomponent
-        c.model(pars[:c.npar], ma.reshape(k**2))
+        c.model(pars[: c.npar], ma.reshape(k**2))
 
         pofs = c.npar
 
         for i, c in enumerate(self.bcomponents):
-            p = pars[pofs:pofs+c.npar]
+            p = pars[pofs : pofs + c.npar]
             c.model(p, mb[i])
             pofs += c.npar
 
         return ma, mb
 
-
     def model(self, pars, mdata):
         k = self.k
         nd = mdata.size // k
         ma, mb = self._sep_model(pars, nd)
         np.dot(ma, mb, mdata.reshape((k, nd)))
 
-
     def deriv(self, pars, jac):
         k = self.k
         nd = jac.shape[1] // k
         npar = self.npar
 
         ma, mb = self._sep_model(pars, nd)
         ja = np.zeros((npar, k, k))
         jb = np.zeros((npar, k, nd))
 
         c = self.acomponent
-        c.deriv(pars[:c.npar], ja[:c.npar].reshape((c.npar, k**2)))
+        c.deriv(pars[: c.npar], ja[: c.npar].reshape((c.npar, k**2)))
         pofs = c.npar
 
         for i, c in enumerate(self.bcomponents):
-            p = pars[pofs:pofs+c.npar]
-            c.deriv(p, jb[pofs:pofs+c.npar,i,:])
+            p = pars[pofs : pofs + c.npar]
+            c.deriv(p, jb[pofs : pofs + c.npar, i, :])
             pofs += c.npar
 
         for i in range(self.npar):
             jac[i] = (np.dot(ja[i], mb) + np.dot(ma, jb[i])).reshape(k * nd)
 
-
     def extract(self, pars, perr, cov):
         c = self.acomponent
-        c.extract(pars[:c.npar], perr[:c.npar], cov[:c.npar,:c.npar])
+        c.extract(pars[: c.npar], perr[: c.npar], cov[: c.npar, : c.npar])
         ofs = c.npar
 
         for c in self.bcomponents:
             n = c.npar
 
-            spar = pars[ofs:ofs+n]
-            serr = perr[ofs:ofs+n]
-            scov = cov[ofs:ofs+n,ofs:ofs+n]
+            spar = pars[ofs : ofs + n]
+            serr = perr[ofs : ofs + n]
+            scov = cov[ofs : ofs + n, ofs : ofs + n]
             c.extract(spar, serr, scov)
             ofs += n
 
-
     def _outputshape(self, *args):
         aofs = self.acomponent.nmodelargs
         sb = ()
 
         for c in self.bcomponents:
-            a = args[aofs:aofs+c.nmodelargs]
+            a = args[aofs : aofs + c.nmodelargs]
             sb = _broadcast_shapes(sb, c._outputshape(*a))
             aofs += c.nmodelargs
 
         return (self.k,) + sb
 
-
     def _accum_mfunc(self, res, *args):
         k = self.k
         nd = res.shape[1]
 
         ma = np.zeros((k, k))
         mb = np.zeros((k, nd))
 
         c = self.acomponent
-        c._accum_mfunc(ma.reshape(k**2), *(args[:c.nmodelargs]))
+        c._accum_mfunc(ma.reshape(k**2), *(args[: c.nmodelargs]))
         aofs = c.nmodelargs
 
         for i, c in enumerate(self.bcomponents):
-            a = args[aofs:aofs+c.nmodelargs]
+            a = args[aofs : aofs + c.nmodelargs]
             c._accum_mfunc(mb[i], *a)
             aofs += c.nmodelargs
 
         np.dot(ma, mb, res)
 
 
 class ScaleComponent(ModelComponent):
     npar = 1
 
     def __init__(self, subcomp=None, name=None):
         super(ScaleComponent, self).__init__(name)
         self.setsubcomp(subcomp)
 
-
     def setsubcomp(self, subcomp):
         self.subcomp = subcomp
         return self
 
-
     def _param_names(self):
-        yield 'factor'
+        yield "factor"
 
-        pfx = self.subcomp.name + '.' if self.subcomp.name is not None else ''
+        pfx = self.subcomp.name + "." if self.subcomp.name is not None else ""
         for p in self.subcomp._param_names():
             yield pfx + p
 
-
     def _sub_setguess(self, npar, cidx, vals, ofs=0):
         vals = np.asarray(vals)
         if ofs < 0 or ofs + vals.size > npar:
-            raise ValueError('ofs %d, vals.size %d, npar %d' %
-                             (ofs, vals.size, npar))
+            raise ValueError("ofs %d, vals.size %d, npar %d" % (ofs, vals.size, npar))
         return self.setguess(vals, ofs + 1)
 
-
     def _sub_setvalue(self, npar, cidx, value, fixed=False):
         if cidx < 0 or cidx >= npar:
-            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+            raise ValueError("cidx %d, npar %d" % (cidx, npar))
         return self.setvalue(1 + cidx, value, fixed)
 
-
     def _sub_setlimit(self, npar, cidx, lower=-np.inf, upper=np.inf):
         if cidx < 0 or cidx >= npar:
-            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+            raise ValueError("cidx %d, npar %d" % (cidx, npar))
         return self.setlimit(1 + cidx, lower, upper)
 
-
     def finalize_setup(self):
         if self.subcomp.name is None:
-            self.subcomp.name = 'c'
+            self.subcomp.name = "c"
 
         from functools import partial
+
         self.subcomp.setvalue = partial(self._sub_setvalue, self.subcomp.npar)
         self.subcomp.setlimit = partial(self._sub_setvalue, self.subcomp.npar)
         self.subcomp.finalize_setup()
 
         self.npar = self.subcomp.npar + 1
         self.nmodelargs = self.subcomp.nmodelargs
 
-
     def prep_params(self):
         self.subcomp.prep_params()
 
-
     def model(self, pars, mdata):
         self.subcomp.model(pars[1:], mdata)
         mdata *= pars[0]
 
-
     def deriv(self, pars, jac):
         self.subcomp.model(pars[1:], jac[0])
         self.subcomp.deriv(pars[1:], jac[1:])
         jac[1:] *= pars[0]
 
-
     def extract(self, pars, perr, cov):
         self.f_factor = pars[0]
         self.u_factor = perr[0]
         self.c_factor = cov[0]
 
-        self.subcomp.extract(pars[1:], perr[1:], cov[1:,1:])
-
+        self.subcomp.extract(pars[1:], perr[1:], cov[1:, 1:])
 
     def _outputshape(self, *args):
         return self.subcomp._outputshape(*args)
 
-
     def _accum_mfunc(self, res, *args):
         self.subcomp._accum_mfunc(res, *args)
```

### Comparing `pwkit-1.1.1/pwkit/method_decorator.py` & `pwkit-1.2.0/pwkit/method_decorator.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/msmt.py` & `pwkit-1.2.0/pwkit/msmt.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,63 +69,66 @@
 uval_dtype                 - The Numpy dtype of Uval data (often ignored!)
 uval_nsamples              - Number of samples used when constructing Uvals
 uval_unary_math            - Dict of unary math functions operating on Uvals.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str('''LimitError Lval Textual Uval absolute arccos arcsin arctan cos errinfo
+__all__ = str(
+    """LimitError Lval Textual Uval absolute arccos arcsin arctan cos errinfo
     expm1 exp fmtinfo isfinite is_measurement liminfo limtype log10 log1p log2
     log negative reciprocal repval sin sqrt square tan unwrap add divide floor_divide
     multiply power subtract true_divide typealign find_gamma_params
     pk_scoreatpercentile sample_double_norm sample_gamma lval_unary_math
     parsers scalar_unary_math textual_unary_math UQUANT_UNCERT
-    uval_default_repval_method uval_dtype uval_nsamples uval_unary_math''').split()
+    uval_default_repval_method uval_dtype uval_nsamples uval_unary_math"""
+).split()
 
-import operator, six
-from six.moves import range
+import operator
 
 import numpy as np
 
-from . import PKError, text_type, unicode_to_str
+from . import PKError, unicode_to_str
 
 
 uval_nsamples = 1024
 uval_dtype = np.double
-uval_default_repval_method = 'pct'
+uval_default_repval_method = "pct"
 
 
 # This is a copy of scipy.stats' scoreatpercentile() function with simplified
 # functionality. This way we don't depend on scipy, and we can count on the
 # ability to handle vector `per`, which earlier versions incorrectly didn't.
 # I'm also tempted to make percentiles be in [0, 1], not [0, 100], but
 # gratuitous incompatibilities seem unwise.
 
+
 def pk_scoreatpercentile(a, per):
     asort = np.sort(a)
     vper = np.atleast_1d(per)
 
     if np.any((vper < 0) | (vper > 100)):
-        raise ValueError('`per` must be in the range [0, 100]')
+        raise ValueError("`per` must be in the range [0, 100]")
 
-    fidx = vper / 100. * (asort.size - 1)
+    fidx = vper / 100.0 * (asort.size - 1)
     # clipping iidx here gets the right behavior for per = 100:
     iidx = np.minimum(fidx.astype(int), asort.size - 2)
     res = (iidx + 1 - fidx) * asort[iidx] + (fidx - iidx) * asort[iidx + 1]
 
     if np.isscalar(per):
         return res[0]
     return res
 
 
 # Double-normal distribution -- that is, pasting together two normal
 # distributions with unequal left and right variances. Skew-normal distributions
 # are mathematically purer but turn out to be just obnoxiously hard to work with.
 # Double-normals are ad-hoc but also much more tractable.
 
+
 def sample_double_norm(mean, std_upper, std_lower, size):
     """Note that this function requires Scipy."""
     from scipy.special import erfinv
 
     # There's probably a better way to do this. We first draw percentiles
     # uniformly between 0 and 1. We want the peak of the distribution to occur
     # at `mean`. However, if we assign 50% of the samples to the lower half
@@ -135,18 +138,18 @@
     # fraction `cutoff` (defined below) going to the lower half. Having
     # partitioned them this way, we can then use the standard Gaussian
     # quantile function to go from percentiles to sample values -- except that
     # we must remap from [0, cutoff] to [0, 0.5] and from [cutoff, 1] to [0.5,
     # 1].
 
     samples = np.empty(size)
-    percentiles = np.random.uniform(0., 1., size)
+    percentiles = np.random.uniform(0.0, 1.0, size)
     cutoff = std_lower / (std_lower + std_upper)
 
-    w = (percentiles < cutoff)
+    w = percentiles < cutoff
     percentiles[w] *= 0.5 / cutoff
     samples[w] = mean + np.sqrt(2) * std_lower * erfinv(2 * percentiles[w] - 1)
 
     w = ~w
     percentiles[w] = 1 - (1 - percentiles[w]) * 0.5 / (1 - cutoff)
     samples[w] = mean + np.sqrt(2) * std_upper * erfinv(2 * percentiles[w] - 1)
 
@@ -155,52 +158,55 @@
 
 # Utilities for gamma distributions. We want these for values that are
 # presented as being (skew)normal but must be positive. If the uncertainty is
 # not much smaller than the value, the samples can cross zero in significant
 # numbers and lead to all sorts of bad behavior in some kinds of computation
 # (e.g., taking logarithms, which we do a lot).
 
+
 def sample_gamma(alpha, beta, size):
     """This is mostly about recording the conversion between Numpy/Scipy
     conventions and Wikipedia conventions. Some equations:
 
     mean = alpha / beta
     variance = alpha / beta**2
     mode = (alpha - 1) / beta [if alpha > 1; otherwise undefined]
     skewness = 2 / sqrt(alpha)
     """
 
     if alpha <= 0:
-        raise ValueError('alpha must be positive; got %e' % alpha)
+        raise ValueError("alpha must be positive; got %e" % alpha)
     if beta <= 0:
-        raise ValueError('beta must be positive; got %e' % beta)
-    return np.random.gamma(alpha, scale=1./beta, size=size)
+        raise ValueError("beta must be positive; got %e" % beta)
+    return np.random.gamma(alpha, scale=1.0 / beta, size=size)
 
 
 def find_gamma_params(mode, std):
     """Given a modal value and a standard deviation, compute corresponding
     parameters for the gamma distribution.
 
     Intended to be used to replace normal distributions when the value must be
     positive and the uncertainty is comparable to the best value. Conversion
     equations determined from the relations given in the sample_gamma()
     docs.
 
     """
     if mode < 0:
-        raise ValueError('input mode must be positive for gamma; got %e' % mode)
+        raise ValueError("input mode must be positive for gamma; got %e" % mode)
 
     var = std**2
     beta = (mode + np.sqrt(mode**2 + 4 * var)) / (2 * var)
     j = 2 * var / mode**2
     alpha = (j + 1 + np.sqrt(2 * j + 1)) / j
 
     if alpha <= 1:
-        raise ValueError('couldn\'t compute self-consistent gamma parameters: '
-                         'mode=%e std=%e alpha=%e beta=%e' % (mode, std, alpha, beta))
+        raise ValueError(
+            "couldn't compute self-consistent gamma parameters: "
+            "mode=%e std=%e alpha=%e beta=%e" % (mode, std, alpha, beta)
+        )
 
     return alpha, beta
 
 
 # Scalar math.
 #
 # What's going on here is that we want to provide a library of standard math
@@ -211,74 +217,79 @@
 # function to invoke. This declutters things and also lets the implementations
 # of math operators take advantage of the unary functions, as is done
 # extensively in the Lval implementation.
 #
 # For scalars, we just delegate to Numpy.
 
 scalar_unary_math = {
-    'absolute': np.absolute,
-    'arccos': np.arccos,
-    'arcsin': np.arcsin,
-    'arctan': np.arctan,
-    'cos': np.cos,
-    'expm1': np.expm1,
-    'exp': np.exp,
-    'isfinite': np.isfinite,
-    'log10': np.log10,
-    'log1p': np.log1p,
-    'log2': np.log2,
-    'log': np.log,
-    'negative': np.negative,
-    'reciprocal': lambda x: 1. / x, # numpy reciprocal barfs on ints. I don't want that.
-    'sin': np.sin,
-    'sqrt': np.sqrt,
-    'square': np.square,
-    'tan': np.tan,
+    "absolute": np.absolute,
+    "arccos": np.arccos,
+    "arcsin": np.arcsin,
+    "arctan": np.arctan,
+    "cos": np.cos,
+    "expm1": np.expm1,
+    "exp": np.exp,
+    "isfinite": np.isfinite,
+    "log10": np.log10,
+    "log1p": np.log1p,
+    "log2": np.log2,
+    "log": np.log,
+    "negative": np.negative,
+    "reciprocal": lambda x: 1.0
+    / x,  # numpy reciprocal barfs on ints. I don't want that.
+    "sin": np.sin,
+    "sqrt": np.sqrt,
+    "square": np.square,
+    "tan": np.tan,
 }
 
 
 # The fundamental "Uval" class.
 #
 # These have a more extensive math/operator library than Lval and Textual
 # since it's so easy to implement things.
 
+
 def _to_uval_info(value):
     if isinstance(value, Uval):
         return value.d
-    return float(value) # broadcasting FTW
+    return float(value)  # broadcasting FTW
 
 
 def _make_uval_operator(opfunc):
     def uvalopfunc(uval, other):
         try:
             otherd = _to_uval_info(other)
         except Exception:
             return NotImplemented
         return Uval(opfunc(uval.d, otherd))
+
     return uvalopfunc
 
 
 def _make_uval_rev_operator(opfunc):
     def uvalopfunc(uval, other):
         try:
             otherd = _to_uval_info(other)
         except Exception:
             return NotImplemented
         return Uval(opfunc(otherd, uval.d))
+
     return uvalopfunc
 
 
 def _make_uval_inpl_operator(opfunc):
     def uvalopfunc(uval, other):
         try:
             otherd = _to_uval_info(other)
         except Exception:
             return NotImplemented
         uval.d = opfunc(uval.d, otherd)
         return uval
+
     return uvalopfunc
 
 
 class Uval(object):
     """An empirical uncertain value, represented by samples.
 
     Constructors are:
@@ -298,75 +309,75 @@
     - :meth:`format`
     - :meth:`debug_distribution`
 
     Supported operations are:
     ``unicode() str() repr() [latexification]  + -(sub) * // / % ** += -= *= //= %= /= **= -(neg) ~ abs()``
 
     """
-    __slots__ = ('d', )
+
+    __slots__ = ("d",)
 
     # Initialization.
 
     def __init__(self, data):
         self.d = data
 
     @staticmethod
     def from_other(o):
         if isinstance(o, Uval):
             return Uval(o.d.copy())
         if np.isscalar(o):
             return Uval.from_fixed(o)
-        raise ValueError('cannot convert %r to a Uval' % o)
+        raise ValueError("cannot convert %r to a Uval" % o)
 
     @staticmethod
     def from_fixed(v):
         return Uval(np.zeros(uval_nsamples, dtype=uval_dtype) + v)
 
     @staticmethod
     def from_norm(mean, std):
         if std < 0:
-            raise ValueError('std must be positive')
+            raise ValueError("std must be positive")
         return Uval(np.random.normal(mean, std, uval_nsamples))
 
     @staticmethod
     def from_unif(lower_incl, upper_excl):
         if upper_excl <= lower_incl:
-            raise ValueError('upper_excl must be greater than lower_incl')
+            raise ValueError("upper_excl must be greater than lower_incl")
         return Uval(np.random.uniform(lower_incl, upper_excl, uval_nsamples))
 
     @staticmethod
     def from_double_norm(mean, std_upper, std_lower):
         if std_upper <= 0:
-            raise ValueError('double-norm upper stddev must be positive')
+            raise ValueError("double-norm upper stddev must be positive")
         if std_lower <= 0:
-            raise ValueError('double-norm lower stddev must be positive')
+            raise ValueError("double-norm lower stddev must be positive")
         return Uval(sample_double_norm(mean, std_upper, std_lower, uval_nsamples))
 
     @staticmethod
     def from_gamma(alpha, beta):
         if alpha <= 0:
-            raise ValueError('gamma parameter `alpha` must be positive')
+            raise ValueError("gamma parameter `alpha` must be positive")
         if beta <= 0:
-            raise ValueError('gamma parameter `beta` must be positive')
+            raise ValueError("gamma parameter `beta` must be positive")
         return Uval(sample_gamma(alpha, beta, uval_nsamples))
 
     @staticmethod
     def from_pcount(nevents):
         """We assume a Poisson process. nevents is the number of events in
         some interval. The distribution of values is the distribution of the
         Poisson rate parameter given this observed number of events, where the
         "rate" is in units of events per interval of the same duration. The
         max-likelihood value is nevents, but the mean value is nevents + 1.
         The gamma distribution is obtained by assuming an improper, uniform
         prior for the rate between 0 and infinity."""
         if nevents < 0:
-            raise ValueError('Poisson parameter `nevents` must be nonnegative')
+            raise ValueError("Poisson parameter `nevents` must be nonnegative")
         return Uval(np.random.gamma(nevents + 1, size=uval_nsamples))
 
-
     # Interrogation. Would be nice to have a way to estimate the
     # distribution's mode -- when a scientist writes V = X +- Y, I think they
     # usually think of X as the maximum likelihood value, which is the modal
     # value. Maybe a kernel density estimator do this sensibly? Anyway, I
     # don't think we're in a position to unilaterally declare what the "best"
     # representative value is, so we provide options and let the caller
     # decide.
@@ -384,199 +395,199 @@
         The "pct" method returns the 50th, 15.866th, and 84.134th percentile
         values.
 
         The "gauss" method computes the mean μ and standard deviation σ of the
         samples and returns [μ, μ+σ, μ-σ].
 
         """
-        if method == 'pct':
-            return pk_scoreatpercentile(self.d, [50., 84.134, 15.866])
-        if method == 'gauss':
+        if method == "pct":
+            return pk_scoreatpercentile(self.d, [50.0, 84.134, 15.866])
+        if method == "gauss":
             m, s = self.d.mean(), self.d.std()
             return np.asarray([m, m + s, m - s])
         raise ValueError('unknown representative-value method "%s"' % method)
 
-
     # Textualization.
 
     def text_pieces(self, method, uplaces=2, use_exponent=True):
         """Return (main, dhigh, dlow, sharedexponent), all as strings. The
         delta terms do not have sign indicators. Any item except the first
         may be None.
 
         `method` is passed to Uval.repvals() to compute representative
         statistical limits.
 
         """
         md, hi, lo = self.repvals(method)
 
         if hi == lo:
-            return '%g' % lo, None, None, None
+            return "%g" % lo, None, None, None
 
         if not np.isfinite([lo, md, hi]).all():
-            raise ValueError('got nonfinite values when formatting Uval')
+            raise ValueError("got nonfinite values when formatting Uval")
 
         # Deltas. Round to limited # of places because we don't actually know
         # the fourth moment of the thing we're trying to describe.
 
         from numpy import abs, ceil, floor, log10
 
         dh = hi - md
         dl = md - lo
 
         if dh <= 0:
-            raise ValueError('strange problem formatting Uval; '
-                             'hi=%g md=%g dh=%g' % (hi, md, dh))
+            raise ValueError(
+                "strange problem formatting Uval; " "hi=%g md=%g dh=%g" % (hi, md, dh)
+            )
         if dl <= 0:
-            raise ValueError('strange problem formatting Uval; '
-                             'lo=%g md=%g dl=%g' % (lo, md, dl))
+            raise ValueError(
+                "strange problem formatting Uval; " "lo=%g md=%g dl=%g" % (lo, md, dl)
+            )
 
         p = int(ceil(log10(dh)))
-        rdh = round(dh * 10**(-p), uplaces) * 10**p
+        rdh = round(dh * 10 ** (-p), uplaces) * 10**p
         p = int(ceil(log10(dl)))
-        rdl = round(dl * 10**(-p), uplaces) * 10**p
+        rdl = round(dl * 10 ** (-p), uplaces) * 10**p
 
         # The least significant place to worry about is the L.S.P. of one of
         # the deltas, which we can find relative to its M.S.P. Any precision
         # in the datum beyond this point is false.
 
         lsp = int(ceil(log10(min(rdh, rdl)))) - uplaces
 
         # We should round the datum since it might be something like
         # 0.999+-0.1 and we're about to try to decide what its most
         # significant place is. Might get -1 rather than 0.
 
         rmd = round(md, -lsp)
 
-        if rmd == -0.: # 0 = -0, too, but no problem there.
-            rmd = 0.
+        if rmd == -0.0:  # 0 = -0, too, but no problem there.
+            rmd = 0.0
 
         # The most significant place to worry about is the M.S.P. of any of
         # the datum or the deltas. rdl and rdl must be positive, but not
         # necessarily rmd.
 
         msp = int(floor(log10(max(abs(rmd), rdh, rdl))))
 
         # If we're not very large or very small, or it's been explicitly
         # disabled, don't use scientific notation.
 
         if (msp > -3 and msp < 3) or not use_exponent:
-            srmd = '%.*f' % (-lsp, rmd)
-            srdh = '%.*f' % (-lsp, rdh)
-            srdl = '%.*f' % (-lsp, rdl)
+            srmd = "%.*f" % (-lsp, rmd)
+            srdh = "%.*f" % (-lsp, rdh)
+            srdl = "%.*f" % (-lsp, rdl)
             return srmd, srdh, srdl, None
 
         # Use scientific notation. Adjust values, then format.
 
         armd = rmd * 10**-msp
         ardh = rdh * 10**-msp
         ardl = rdl * 10**-msp
         prec = msp - lsp
 
-        sarmd = '%.*f' % (prec, armd)
-        sardh = '%.*f' % (prec, ardh)
-        sardl = '%.*f' % (prec, ardl)
+        sarmd = "%.*f" % (prec, armd)
+        sardh = "%.*f" % (prec, ardh)
+        sardl = "%.*f" % (prec, ardl)
         return sarmd, sardh, sardl, str(msp)
 
-
     def format(self, method, parenexp=True, uplaces=2, use_exponent=True):
-        main, dh, dl, exp = self.text_pieces(method, uplaces=uplaces, use_exponent=use_exponent)
+        main, dh, dl, exp = self.text_pieces(
+            method, uplaces=uplaces, use_exponent=use_exponent
+        )
 
         if exp is not None and not parenexp:
-            main += 'e' + exp
+            main += "e" + exp
             if dh is not None:
-                dh += 'e' + exp
+                dh += "e" + exp
             if dl is not None:
-                dl += 'e' + exp
+                dl += "e" + exp
 
         if dh is None:
-            pmterm = ''
+            pmterm = ""
         elif dh == dl:
-            pmterm = 'pm' + dh
+            pmterm = "pm" + dh
         else:
-            pmterm = ''.join(['p', dh, 'm', dl])
+            pmterm = "".join(["p", dh, "m", dl])
 
         if exp is not None and parenexp:
-            return '(%s%s)e%s' % (main, pmterm, exp)
+            return "(%s%s)e%s" % (main, pmterm, exp)
 
         return main + pmterm
 
-
     def __unicode__(self):
         try:
             return self.format(uval_default_repval_method)
         except ValueError:
-            return '{bad samples}'
+            return "{bad samples}"
 
     __str__ = unicode_to_str
 
-
     def __repr__(self):
         formatted = self.format(uval_default_repval_method)
         v = pk_scoreatpercentile(self.d, [0, 2.5, 50, 97.5, 100])
-        return '<Uval %s [min=%g l95=%g med=%g u95=%g max=%g]>' % \
-            ((formatted, ) + tuple(v))
-
+        return "<Uval %s [min=%g l95=%g med=%g u95=%g max=%g]>" % (
+            (formatted,) + tuple(v)
+        )
 
     def __pk_fmtinfo__(self):
-        return 'u', self.format('pct', parenexp=False), True
-
+        return "u", self.format("pct", parenexp=False), True
 
     def __pk_latex__(self, method=None, uplaces=1, use_exponent=True, **kwargs):
         if method is None:
             method = uval_default_repval_method
-        main, dh, dl, exp = self.text_pieces(method, uplaces=uplaces, use_exponent=use_exponent)
+        main, dh, dl, exp = self.text_pieces(
+            method, uplaces=uplaces, use_exponent=use_exponent
+        )
 
         if dh is None:
-            return r'$%s$' % main
+            return r"$%s$" % main
 
         if dh == dl:
-            pmterm = r'\pm %s' % dh
+            pmterm = r"\pm %s" % dh
         else:
-            pmterm = r'^{%s}_{%s}' % (dh, dl)
+            pmterm = r"^{%s}_{%s}" % (dh, dl)
 
         if exp is None:
-            return '$%s %s$' % (main, pmterm)
-
-        return r'$(%s %s) \times 10^{%s}$' % (main, pmterm, exp)
+            return "$%s %s$" % (main, pmterm)
 
+        return r"$(%s %s) \times 10^{%s}$" % (main, pmterm, exp)
 
     def __pk_latex_l3col__(self, method=None, **kwargs):
         if method is None:
             method = uval_default_repval_method
         v = self.repvals(method)[0]
 
         from .latex import latexify_n2col
-        return b'$\\sim$ & ' + latexify_n2col(v, **kwargs)
 
+        return b"$\\sim$ & " + latexify_n2col(v, **kwargs)
 
     def __pk_latex_u3col__(self, method=None, uplaces=1, use_exponent=True, **kwargs):
         if method is None:
             method = uval_default_repval_method
-        main, dh, dl, exp = self.text_pieces(method, uplaces=uplaces, use_exponent=use_exponent)
+        main, dh, dl, exp = self.text_pieces(
+            method, uplaces=uplaces, use_exponent=use_exponent
+        )
 
         if dh is None:
-            return r'\multicolumn{3}{c}{$%s$}' % main
+            return r"\multicolumn{3}{c}{$%s$}" % main
 
         if dh == dl:
-            pmterm = r'$\pm\,%s$' % dh
+            pmterm = r"$\pm\,%s$" % dh
         else:
-            pmterm = r'$\pm\,^{%s}_{%s}$' % (dh, dl)
+            pmterm = r"$\pm\,^{%s}_{%s}$" % (dh, dl)
 
-        if '.' not in main:
-            mainterm = r'$%s$ & ' % main
+        if "." not in main:
+            mainterm = r"$%s$ & " % main
         else:
-            mainterm = r'$%s$ & $.%s$' % tuple(main.split('.'))
+            mainterm = r"$%s$ & $.%s$" % tuple(main.split("."))
 
         if exp is None:
-            return mainterm + ' & ' + pmterm
-
-        return ''.join(['$($', mainterm, ' & ', pmterm,
-                        r'$) \times 10^{%s}$' % exp])
+            return mainterm + " & " + pmterm
 
+        return "".join(["$($", mainterm, " & ", pmterm, r"$) \times 10^{%s}$" % exp])
 
     # math -- http://docs.python.org/2/reference/datamodel.html#emulating-numeric-types
 
     __add__ = _make_uval_operator(operator.add)
     __sub__ = _make_uval_operator(operator.sub)
     __mul__ = _make_uval_operator(operator.mul)
     __floordiv__ = _make_uval_operator(operator.floordiv)
@@ -621,27 +632,27 @@
         return self
 
     def __invert__(self):
         self.d = ~self.d
         return self
 
     def __nonzero__(self):
-        raise TypeError('uncertain value cannot be reduced to a boolean scalar')
+        raise TypeError("uncertain value cannot be reduced to a boolean scalar")
 
     def __complex__(self):
-        raise TypeError('uncertain value cannot be reduced to a complex scalar')
+        raise TypeError("uncertain value cannot be reduced to a complex scalar")
 
     def __int__(self):
-        raise TypeError('uncertain value cannot be reduced to an integer scalar')
+        raise TypeError("uncertain value cannot be reduced to an integer scalar")
 
     def __long__(self):
-        raise TypeError('uncertain value cannot be reduced to a long-integer scalar')
+        raise TypeError("uncertain value cannot be reduced to a long-integer scalar")
 
     def __float__(self):
-        raise TypeError('uncertain value cannot be reduced to a float scalar')
+        raise TypeError("uncertain value cannot be reduced to a float scalar")
 
     # skipped: oct, hex, index, coerce
 
     def __lt__(self, other):
         raise TypeError('uncertain value does not have a well-defined "<" comparison')
 
     def __le__(self, other):
@@ -656,66 +667,70 @@
     def __gt__(self, other):
         raise TypeError('uncertain value does not have a well-defined ">" comparison')
 
     def __ge__(self, other):
         raise TypeError('uncertain value does not have a well-defined ">=" comparison')
 
     def __cmp__(self, other):
-        raise TypeError('uncertain value does not have a well-defined __cmp__ comparison')
+        raise TypeError(
+            "uncertain value does not have a well-defined __cmp__ comparison"
+        )
 
     __hash__ = None
 
-
     def debug_distribution(self):
         import omega as om
 
         v = pk_scoreatpercentile(self.d, [50, 0, 0.270, 2.5, 97.5, 99.730, 100])
         median = v[0]
         v = v[1:]
 
-        print('median=%g mean=%g'
-              % (median, self.d.mean()))
-        print('   abs: min=%g l3σ=%g l95%%=%g .. u95%%=%g u3σ=%g max=%g'
-              % tuple(v))
-        print('   rel: min=%g l3σ=%g l95%%=%g .. u95%%=%g u3σ=%g max=%g'
-              % tuple(v - median))
-        print('   scl: min=%.2f l3σ=%.2f l95%%=%.2f .. u95%%=%.2f u3σ=%.2f max=%.2f'
-              % tuple((v - median) / np.abs(median)))
+        print("median=%g mean=%g" % (median, self.d.mean()))
+        print("   abs: min=%g l3σ=%g l95%%=%g .. u95%%=%g u3σ=%g max=%g" % tuple(v))
+        print(
+            "   rel: min=%g l3σ=%g l95%%=%g .. u95%%=%g u3σ=%g max=%g"
+            % tuple(v - median)
+        )
+        print(
+            "   scl: min=%.2f l3σ=%.2f l95%%=%.2f .. u95%%=%.2f u3σ=%.2f max=%.2f"
+            % tuple((v - median) / np.abs(median))
+        )
         return om.quickHist(self.d, bins=25)
 
 
 def _make_uval_unary_math(scalarfunc):
     def uval_unary_math(v):
         return Uval(scalarfunc(_to_uval_info(v)))
+
     return uval_unary_math
 
 
 def _uval_unary_isfinite(v):
     return np.all(np.isfinite(_to_uval_info(v)))
 
 
 uval_unary_math = {
-    'absolute': _make_uval_unary_math(np.absolute),
-    'arccos': _make_uval_unary_math(np.arccos),
-    'arcsin': _make_uval_unary_math(np.arcsin),
-    'arctan': _make_uval_unary_math(np.arctan),
-    'cos': _make_uval_unary_math(np.cos),
-    'expm1': _make_uval_unary_math(np.expm1),
-    'exp': _make_uval_unary_math(np.exp),
-    'isfinite': _uval_unary_isfinite,
-    'log10': _make_uval_unary_math(np.log10),
-    'log1p': _make_uval_unary_math(np.log1p),
-    'log2': _make_uval_unary_math(np.log2),
-    'log': _make_uval_unary_math(np.log),
-    'negative': _make_uval_unary_math(np.negative),
-    'reciprocal': _make_uval_unary_math(lambda x: 1. / x),
-    'sin': _make_uval_unary_math(np.sin),
-    'sqrt': _make_uval_unary_math(np.sqrt),
-    'square': _make_uval_unary_math(np.square),
-    'tan': _make_uval_unary_math(np.tan),
+    "absolute": _make_uval_unary_math(np.absolute),
+    "arccos": _make_uval_unary_math(np.arccos),
+    "arcsin": _make_uval_unary_math(np.arcsin),
+    "arctan": _make_uval_unary_math(np.arctan),
+    "cos": _make_uval_unary_math(np.cos),
+    "expm1": _make_uval_unary_math(np.expm1),
+    "exp": _make_uval_unary_math(np.exp),
+    "isfinite": _uval_unary_isfinite,
+    "log10": _make_uval_unary_math(np.log10),
+    "log1p": _make_uval_unary_math(np.log1p),
+    "log2": _make_uval_unary_math(np.log2),
+    "log": _make_uval_unary_math(np.log),
+    "negative": _make_uval_unary_math(np.negative),
+    "reciprocal": _make_uval_unary_math(lambda x: 1.0 / x),
+    "sin": _make_uval_unary_math(np.sin),
+    "sqrt": _make_uval_unary_math(np.sqrt),
+    "square": _make_uval_unary_math(np.square),
+    "tan": _make_uval_unary_math(np.tan),
 }
 
 
 # Now, limiting values. I tried to do this within the context of the Uval
 # system, but it just never worked in a way that gave the results that people
 # would naively expect. Lvals are one level "above" Uvals: Lvals know about
 # Uvals, but not the other way around.
@@ -729,76 +744,76 @@
 # Practical math with limits requires both possibilities. In particular, we
 # sometimes want to take reciprocals or logs of numbers known to be positive,
 # and sometimes we'll want to exponentiate numbers that are known to be logs.
 # After several false starts, the system I've devised below seems to allow
 # sane operation in the majority of cases.
 
 _lval_pos_sigils = {
-    'exact': '',
-    'uncertain': '~',
-    'toinf': '>',
-    'tozero': '<',
-    'pastzero': '<<',
-    'undef': '!',
+    "exact": "",
+    "uncertain": "~",
+    "toinf": ">",
+    "tozero": "<",
+    "pastzero": "<<",
+    "undef": "!",
 }
 
 _lval_kmap_reciprocal = {
-    'toinf': 'tozero',
-    'tozero': 'toinf',
-    'pastzero': 'undef',
+    "toinf": "tozero",
+    "tozero": "toinf",
+    "pastzero": "undef",
 }
 
 _lval_kmap_add_unconditional = {
-    ('exact', 'exact'): 'exact',
-    ('exact', 'tozero'): 'undef',
-    ('exact', 'uncertain'): 'uncertain',
-    ('tozero', 'uncertain'): 'undef',
-    ('uncertain', 'uncertain'): 'uncertain',
+    ("exact", "exact"): "exact",
+    ("exact", "tozero"): "undef",
+    ("exact", "uncertain"): "uncertain",
+    ("tozero", "uncertain"): "undef",
+    ("uncertain", "uncertain"): "uncertain",
 }
 
 _lval_kmap_mul = {
-    ('exact', 'exact'): 'exact',
-    ('exact', 'pastzero'): 'pastzero',
-    ('exact', 'toinf'): 'toinf',
-    ('exact', 'tozero'): 'tozero',
-    ('exact', 'uncertain'): 'uncertain',
-    ('pastzero', 'pastzero'): 'undef',
-    ('pastzero', 'toinf'): 'undef',
-    ('pastzero', 'tozero'): 'pastzero',
-    ('pastzero', 'uncertain'): 'pastzero',
-    ('toinf', 'toinf'): 'toinf',
+    ("exact", "exact"): "exact",
+    ("exact", "pastzero"): "pastzero",
+    ("exact", "toinf"): "toinf",
+    ("exact", "tozero"): "tozero",
+    ("exact", "uncertain"): "uncertain",
+    ("pastzero", "pastzero"): "undef",
+    ("pastzero", "toinf"): "undef",
+    ("pastzero", "tozero"): "pastzero",
+    ("pastzero", "uncertain"): "pastzero",
+    ("toinf", "toinf"): "toinf",
     # ('toinf', 'tozero'): special case -> >0
-    ('toinf', 'uncertain'): 'toinf',
-    ('tozero', 'tozero'): 'tozero',
-    ('tozero', 'uncertain'): 'tozero',
-    ('uncertain', 'uncertain'): 'uncertain',
+    ("toinf", "uncertain"): "toinf",
+    ("tozero", "tozero"): "tozero",
+    ("tozero", "uncertain"): "tozero",
+    ("uncertain", "uncertain"): "uncertain",
 }
 
 _lval_kmap_pow_zero_to_one = {
-    'pastzero': 'toinf',
-    'toinf': 'tozero',
-    'tozero': 'undef', # this yields a value in [v**l, 1], which is inexpressible.
+    "pastzero": "toinf",
+    "toinf": "tozero",
+    "tozero": "undef",  # this yields a value in [v**l, 1], which is inexpressible.
 }
 
 _lval_kmap_pow_above_one = {
-    'pastzero': 'tozero',
-    'toinf': 'toinf',
-    'tozero': 'undef', # this yields a value in [1, v**l], which is inexpressible.
+    "pastzero": "tozero",
+    "toinf": "toinf",
+    "tozero": "undef",  # this yields a value in [1, v**l], which is inexpressible.
 }
 
-_lval_kmap_exp = _lval_kmap_pow_above_one # same behavior
+_lval_kmap_exp = _lval_kmap_pow_above_one  # same behavior
 
 _lval_kmap_log = {
-    'tozero': 'pastzero',
+    "tozero": "pastzero",
 }
 
 
 class LimitError(PKError):
     def __init__(self):
-        super(LimitError, self).__init__('forbidden operation on a limit value')
+        super(LimitError, self).__init__("forbidden operation on a limit value")
 
 
 def _ordpair(v1, v2):
     if v1 > v2:
         return (v2, v1)
     return (v1, v2)
 
@@ -807,142 +822,142 @@
     """Compute the appropriate Lval "kind" for the limit of value `x` towards
     `polarity`. Either 'toinf' or 'pastzero' depending on the sign of `x` and
     the infinity direction of polarity.
 
     """
     if x < 0:
         if polarity < 0:
-            return Lval('toinf', x)
-        return Lval('pastzero', x)
+            return Lval("toinf", x)
+        return Lval("pastzero", x)
     elif polarity > 0:
-        return Lval('toinf', x)
-    return Lval('pastzero', x)
+        return Lval("toinf", x)
+    return Lval("pastzero", x)
 
 
 class Lval(object):
     """A container for either precise values or upper/lower limits. Constructed as
     ``Lval(kind, value)``, where *kind* is ``"exact"``, ``"uncertain"``,
     ``"toinf"``, ``"tozero"``, ``"pastzero"``, or ``"undef"``. Most easily
     constructed via :meth:`Textual.parse`. Can also be constructed with
     :meth:`Lval.from_other`.
 
     Supported operations are
     ``unicode() str() repr() -(neg) abs() + - * / ** += -= *= /= **=``.
 
     """
-    __slots__ = ('kind', 'value')
+
+    __slots__ = ("kind", "value")
 
     def __init__(self, kind, value):
         if kind not in _lval_pos_sigils:
-            raise ValueError('unrecognized Lval kind %r' % kind)
+            raise ValueError("unrecognized Lval kind %r" % kind)
         if not np.isscalar(value):
-            raise ValueError('Lvals must be scalars; got %r' % value)
+            raise ValueError("Lvals must be scalars; got %r" % value)
         self.kind = kind
         self.value = value
 
     @staticmethod
     def from_other(o):
         if isinstance(o, Lval):
             from copy import copy
+
             return Lval(o.kind, copy(o.value))
         if isinstance(o, Uval):
-            return Lval('uncertain', o.repvals(uval_default_repval_method)[0])
+            return Lval("uncertain", o.repvals(uval_default_repval_method)[0])
         if np.isscalar(o):
-            return Lval('exact', float(o))
-        raise ValueError('cannot convert %r to an Lval' % o)
+            return Lval("exact", float(o))
+        raise ValueError("cannot convert %r to an Lval" % o)
 
     # Textualization.
 
     def __unicode__(self):
         s = _lval_pos_sigils[self.kind]
         if self.value < 0:
-            if s == '>':
-                s = '<'
+            if s == ">":
+                s = "<"
             else:
-                s = s.replace('<', '>')
-        return '%s%g' % (s, self.value)
+                s = s.replace("<", ">")
+        return "%s%g" % (s, self.value)
 
     __str__ = unicode_to_str
 
     def __repr__(self):
-        return 'Lval(%r, %r)' % (self.kind, self.value)
+        return "Lval(%r, %r)" % (self.kind, self.value)
 
     def __pk_fmtinfo__(self):
         # Only certain kinds of Lval can successfully be roundtripped through
         # text. Positive 'tozero' values need the 'P' flag; negative tozeros
         # are inexpressible.
-        if self.kind == 'undef' or (self.kind == 'tozero' and self.value < 0):
-            raise ValueError('no fmtinfo textualization of %r is possible' % self)
+        if self.kind == "undef" or (self.kind == "tozero" and self.value < 0):
+            raise ValueError("no fmtinfo textualization of %r is possible" % self)
 
-        if self.kind == 'tozero':
-            return 'Pu', '<%g' % self.value, True
+        if self.kind == "tozero":
+            return "Pu", "<%g" % self.value, True
 
-        s = _lval_pos_sigils[self.kind][0] # note: truncating << pastzero mode.
+        s = _lval_pos_sigils[self.kind][0]  # note: truncating << pastzero mode.
         if self.value < 0:
-            if s == '>': # toinf, but we're negative.
-                s = '<'
-            else: # tozero disallowed, so we must be pastzero
-                s = '>'
-
-        return 'u', '%s%g' % (s, self.value), True
+            if s == ">":  # toinf, but we're negative.
+                s = "<"
+            else:  # tozero disallowed, so we must be pastzero
+                s = ">"
 
+        return "u", "%s%g" % (s, self.value), True
 
     def __pk_latex__(self, undefok=False, **kwargs):
         from .latex import latexify
+
         base = latexify(self.value, **kwargs)
 
-        if self.kind == 'undef':
+        if self.kind == "undef":
             if undefok:
-                return b''
-            raise ValueError('tried to LaTeXify undefined Lval')
+                return b""
+            raise ValueError("tried to LaTeXify undefined Lval")
 
-        if self.kind == 'exact':
-            return b'' + base
+        if self.kind == "exact":
+            return b"" + base
 
-        if self.kind == 'uncertain':
-            return b'$\\sim$' + base
+        if self.kind == "uncertain":
+            return b"$\\sim$" + base
 
-        s = _lval_pos_sigils[self.kind][0] # note: truncating << pastzero mode.
+        s = _lval_pos_sigils[self.kind][0]  # note: truncating << pastzero mode.
         if self.value < 0:
-            if s == '>':
-                s = '<'
+            if s == ">":
+                s = "<"
             else:
-                s = '>'
-
-        return b'$%s$%s' % (s, base)
+                s = ">"
 
+        return b"$%s$%s" % (s, base)
 
     def __pk_latex_l3col__(self, undefok=False, **kwargs):
         from .latex import latexify_n2col
+
         base = latexify_n2col(self.value, **kwargs)
 
-        if self.kind == 'undef':
+        if self.kind == "undef":
             if undefok:
-                return b' & & '
-            raise ValueError('tried to LaTeXify undefined Lval')
+                return b" & & "
+            raise ValueError("tried to LaTeXify undefined Lval")
 
-        if self.kind == 'exact':
-            return b'& ' + base
+        if self.kind == "exact":
+            return b"& " + base
 
-        if self.kind == 'uncertain':
-            return b'$\\sim$ & ' + base
+        if self.kind == "uncertain":
+            return b"$\\sim$ & " + base
 
-        s = _lval_pos_sigils[self.kind][0] # note: truncating << pastzero mode.
+        s = _lval_pos_sigils[self.kind][0]  # note: truncating << pastzero mode.
         if self.value < 0:
-            if s == '>':
-                s = '<'
+            if s == ">":
+                s = "<"
             else:
-                s = '>'
-
-        return b'$%s$ & %s' % (s, base)
+                s = ">"
 
+        return b"$%s$ & %s" % (s, base)
 
     def __pk_latex_u3col__(self, **kwargs):
-        return br'\multicolumn{3}{c}{%s}' % self.__pk_latex__(**kwargs)
-
+        return rb"\multicolumn{3}{c}{%s}" % self.__pk_latex__(**kwargs)
 
     # Math. We start with addition. It gets complicated!
 
     def __neg__(self):
         return _lval_unary_negative(self)
 
     def __abs__(self):
@@ -951,82 +966,81 @@
     def _polarity(self):
         # -2  --  limit towards -infinity
         # -1  --  limit from a negative value to zero
         # 0   --  not a limit
         # +1  --  limit from a positive value to zero
         # +2  --  limit towards +infinity
 
-        assert self.kind != 'undef'
+        assert self.kind != "undef"
 
-        if self.kind in ('uncertain', 'exact'):
+        if self.kind in ("uncertain", "exact"):
             return 0
 
         if self.value < 0:
-            if self.kind == 'toinf':
+            if self.kind == "toinf":
                 return -2
-            if self.kind == 'tozero':
+            if self.kind == "tozero":
                 return -1
             return +2
 
-        if self.kind == 'toinf':
+        if self.kind == "toinf":
             return +2
-        if self.kind == 'tozero':
+        if self.kind == "tozero":
             return +1
         return -2
 
-
     def __add__(self, other):
         v1 = self
         v2 = Lval.from_other(other)
         tot = v1.value + v2.value
 
         # Rule 1: undef trumps all.
-        if v1.kind == 'undef' or v2.kind == 'undef':
-            return Lval('undef', tot)
+        if v1.kind == "undef" or v2.kind == "undef":
+            return Lval("undef", tot)
 
         # Rule(s) 2: some combinations with exact/uncert values require no
         # checking of the kind or polarity.
         k = _lval_kmap_add_unconditional.get(_ordpair(v1.kind, v2.kind))
         if k is not None:
             return Lval(k, tot)
 
         # Rule 3: if values have same sign and same kind, we can add
         # without needing to worry about changing the kind.
         s1, s2 = np.sign(v1.value), np.sign(v2.value)
         if s1 == 0:
-            s1 = 1.
+            s1 = 1.0
         if s2 == 0:
-            s2 = 1.
+            s2 = 1.0
 
         if s1 == s2 and v1.kind == v2.kind:
             return Lval(v1.kind, tot)
 
         # Undefs and exact-ish pairs were dealt with in Rules 1 and 2; to-zero
         # and exact-ish were dealt with in Rule 2, and same-sign-same-kind was
         # dealt with in Rule 3. Therefore if we have two to-zeros, they must
         # be of opposite polarity. Rule 4: this goes to undef.
 
         p1, p2 = v1._polarity(), v2._polarity()
 
         if max(abs(p1), abs(p2)) == 1:
             assert p1 == -p2
-            return Lval('undef', tot)
+            return Lval("undef", tot)
 
         # The only remaining possibility is a combination of a limit to
         # infinity and something else. Make sure that p1 holds an infinity
         # limit.
 
         if abs(p1) < 2:
             v1, v2 = v2, v1
             s1, s2 = s2, s1
             p1, p2 = p2, p1
 
         # Rule 5: to-infs of opposite signs go to undef.
         if p2 == -p1:
-            return Lval('undef', tot)
+            return Lval("undef", tot)
 
         # Rule 6: to-infs of same sign are add-and-normalize.
         if p1 == p2:
             return _lval_add_towards_polarity(tot, p1)
 
         # Rule 7: to-inf and to-zero of same polarity give the to-inf.
         # Rule 8: to-inf and to-zero of opposite polarity are add-and-normalize.
@@ -1035,15 +1049,15 @@
                 return v1
             return _lval_add_towards_polarity(tot, p1)
 
         # Rule 9: to-inf and constant-ish are add-and-normalize.
         if p2 == 0:
             return _lval_add_towards_polarity(tot, p1)
 
-        assert False, 'not reached'
+        assert False, "not reached"
 
     __radd__ = __add__
 
     def __sub__(self, other):
         other = Lval.from_other(other)
         other = -other
         return self + other
@@ -1078,21 +1092,21 @@
 
         if v2.value < 0:
             negative = not negative
             v2 = -v2
 
         prod = v1.value * v2.value
 
-        if v1.kind == 'undef' or v2.kind == 'undef':
-            return Lval('undef', prod)
+        if v1.kind == "undef" or v2.kind == "undef":
+            return Lval("undef", prod)
 
         ordkind = _ordpair(v1.kind, v2.kind)
 
-        if ordkind ==('toinf', 'tozero'):
-            rv = Lval('toinf', 0.)
+        if ordkind == ("toinf", "tozero"):
+            rv = Lval("toinf", 0.0)
         else:
             rv = Lval(_lval_kmap_mul[ordkind], prod)
 
         if negative:
             return -rv
         return rv
 
@@ -1127,199 +1141,197 @@
 
     __itruediv__ = __idiv__
 
     # Exponentiation.
 
     def __pow__(self, other, modulo=None):
         if modulo is not None:
-            raise ValueError('powmod behavior forbidden with Lvals')
+            raise ValueError("powmod behavior forbidden with Lvals")
 
         try:
             v = float(other)
         except TypeError:
-            raise ValueError('Lvals can only be exponentiated by exact values')
+            raise ValueError("Lvals can only be exponentiated by exact values")
 
-        if self.kind == 'undef':
+        if self.kind == "undef":
             # It's not worth trying to get a reasonable value in this case.
-            return Lval('undef', np.nan)
+            return Lval("undef", np.nan)
 
         if v == 0:
-            return Lval('exact', 1.)
+            return Lval("exact", 1.0)
 
-        reciprocate = (v < 0)
+        reciprocate = v < 0
         if reciprocate:
             v = -v
 
         i = int(v)
 
         if v != i:
             # For us, fractional powers are only defined on positive numbers,
             # which gives us a fairly small number of valid cases to worry
             # about.
-            if self.value <= 0 or self.kind == 'pastzero':
-                return Lval('undef', np.nan)
+            if self.value <= 0 or self.kind == "pastzero":
+                return Lval("undef", np.nan)
             rv = Lval(self.kind, self.value**v)
         else:
             # We can deal with integer exponentiation as a series of
             # multiplies. Not the most efficient, but reduces the chance for
             # bugs.
             rv = Lval.from_other(self)
             for _ in range(i - 1):
                 rv *= self
 
         if reciprocate:
             rv = _lval_unary_reciprocal(rv)
         return rv
 
-
     def __rpow__(self, other, modulo=None):
         if modulo is not None:
-            raise ValueError('powmod behavior forbidden with Lvals')
+            raise ValueError("powmod behavior forbidden with Lvals")
 
-        if self.kind == 'undef':
-            return Lval('undef', np.nan)
+        if self.kind == "undef":
+            return Lval("undef", np.nan)
 
-        if self.kind == 'exact':
+        if self.kind == "exact":
             # In this very special case, we can delegate.
-            return other ** self.value
+            return other**self.value
 
         # In all other cases, we're exponentiating by a fractional value,
         # so we're only valid for nonnegative numbers.
 
         try:
             v = float(other)
         except TypeError:
-            raise ValueError('Lvals can only exponentiate exact values')
+            raise ValueError("Lvals can only exponentiate exact values")
 
         if v < 0:
-            raise ValueError('Lvals can only exponentiate nonnegative values')
+            raise ValueError("Lvals can only exponentiate nonnegative values")
 
-        reciprocate = (self.value < 0)
-        exponent = self # NOTE: no use of 'self' from here on out!
+        reciprocate = self.value < 0
+        exponent = self  # NOTE: no use of 'self' from here on out!
         if reciprocate:
             exponent = -exponent
 
         if v == 0:
-            if exponent.kind == 'pastzero':
-                return Lval('undef', np.nan)
+            if exponent.kind == "pastzero":
+                return Lval("undef", np.nan)
             # We ignore the fact that 0**0 = 1.
-            rv = Lval('exact', 0.)
+            rv = Lval("exact", 0.0)
         elif v < 1:
             k = _lval_kmap_pow_zero_to_one.get(exponent.kind, exponent.kind)
             rv = Lval(k, v**exponent.value)
         else:
             k = _lval_kmap_pow_above_one.get(exponent.kind, exponent.kind)
             rv = Lval(k, v**exponent.value)
 
         if reciprocate:
             rv = _lval_unary_reciprocal(rv)
         return rv
 
-
     def __ipow__(self, other, modulo=None):
         tmp = pow(self, other, modulo)
         self.kind, self.value = tmp.kind, tmp.value
         return self
 
-
     __hash__ = None
 
 
 def _make_lval_unary_math_nolimits(scalarfunc):
     def lval_unary_math_nolimits(v):
         v = Lval.from_other(v)
-        if v.kind == 'upper' or v.kind == 'lower':
+        if v.kind == "upper" or v.kind == "lower":
             raise LimitError()
         return Lval(v.kind, scalarfunc(value))
+
     return lval_unary_math_nolimits
 
 
 def _lval_unary_absolute(v):
     v = Lval.from_other(v)
 
-    if v.kind == 'pastzero':
-        return Lval('toinf', 0.) # can't argue with this!
+    if v.kind == "pastzero":
+        return Lval("toinf", 0.0)  # can't argue with this!
     return Lval(v.kind, abs(v.value))
 
 
 def _lval_unary_exp(v):
     v = Lval.from_other(v)
 
-    reciprocate = (v.value < 0)
+    reciprocate = v.value < 0
     if reciprocate:
         v = -v
 
     rv = Lval(_lval_kmap_exp.get(v.kind, v.kind), np.exp(v.value))
     if reciprocate:
         rv = _lval_unary_reciprocal(rv)
     return rv
 
 
 def _lval_unary_isfinite(v):
     v = Lval.from_other(v)
 
-    if v.kind == 'undef':
+    if v.kind == "undef":
         return False
     return np.isfinite(v.value)
 
 
 def _make_lval_unary_log(scalarfunc):
     def lval_unary_log(v):
         v = Lval.from_other(v)
-        if v.value <= 0 or v.kind in ('undef', 'pastzero'):
-            return Lval('undef', np.nan)
-        return Lval(_lval_kmap_log.get(v.kind, v.kind),
-                    scalarfunc(v.value))
+        if v.value <= 0 or v.kind in ("undef", "pastzero"):
+            return Lval("undef", np.nan)
+        return Lval(_lval_kmap_log.get(v.kind, v.kind), scalarfunc(v.value))
+
     return lval_unary_log
 
 
 def _lval_unary_negative(v):
     # In this convenient case, the `kind` doesn't change.
     v = Lval.from_other(v)
     return Lval(v.kind, -v.value)
 
 
 def _lval_unary_reciprocal(v):
     v = Lval.from_other(v)
     if v.value == 0:
-        return Lval('undef', np.nan)
-    return Lval(_lval_kmap_reciprocal.get(v.kind, v.kind), 1. / v.value)
+        return Lval("undef", np.nan)
+    return Lval(_lval_kmap_reciprocal.get(v.kind, v.kind), 1.0 / v.value)
 
 
 def _lval_unary_sqrt(v):
     v = Lval.from_other(v)
-    return v ** 0.5
+    return v**0.5
 
 
 def _lval_unary_square(v):
     v = Lval.from_other(v)
     return v * v
 
 
 lval_unary_math = {
     # The 'nolimits' entries could be improved with special-cased
     # implementations, but I'm not going to write them until the need arises.
-    'absolute': _lval_unary_absolute,
-    'arccos': _make_lval_unary_math_nolimits(np.arccos),
-    'arcsin': _make_lval_unary_math_nolimits(np.arcsin),
-    'arctan': _make_lval_unary_math_nolimits(np.arctan),
-    'cos': _make_lval_unary_math_nolimits(np.cos),
-    'expm1': _make_lval_unary_math_nolimits(np.expm1),
-    'exp': _lval_unary_exp,
-    'isfinite': _lval_unary_isfinite,
-    'log10': _make_lval_unary_log(np.log10),
-    'log1p': _make_lval_unary_math_nolimits(np.log1p),
-    'log2': _make_lval_unary_log(np.log2),
-    'log': _make_lval_unary_log(np.log),
-    'negative': _lval_unary_negative,
-    'reciprocal': _lval_unary_reciprocal,
-    'sin': _make_lval_unary_math_nolimits(np.sin),
-    'sqrt': _lval_unary_sqrt,
-    'square': _lval_unary_square,
-    'tan': _make_lval_unary_math_nolimits(np.tan),
+    "absolute": _lval_unary_absolute,
+    "arccos": _make_lval_unary_math_nolimits(np.arccos),
+    "arcsin": _make_lval_unary_math_nolimits(np.arcsin),
+    "arctan": _make_lval_unary_math_nolimits(np.arctan),
+    "cos": _make_lval_unary_math_nolimits(np.cos),
+    "expm1": _make_lval_unary_math_nolimits(np.expm1),
+    "exp": _lval_unary_exp,
+    "isfinite": _lval_unary_isfinite,
+    "log10": _make_lval_unary_log(np.log10),
+    "log1p": _make_lval_unary_math_nolimits(np.log1p),
+    "log2": _make_lval_unary_log(np.log2),
+    "log": _make_lval_unary_log(np.log),
+    "negative": _lval_unary_negative,
+    "reciprocal": _lval_unary_reciprocal,
+    "sin": _make_lval_unary_math_nolimits(np.sin),
+    "sqrt": _lval_unary_sqrt,
+    "square": _lval_unary_square,
+    "tan": _make_lval_unary_math_nolimits(np.tan),
 }
 
 
 # Finally, measurements represented in textual form. Textual forms can
 # represent exact values, Uvals, or Lvals.
 
 UQUANT_UNCERT = 0.2
@@ -1333,24 +1345,24 @@
 are 20% uncertain and give them to multiple decimal places. I'd rather be
 conservative with these values than overly optimistic.
 
 Code to do the appropriate parsing is in the Python uncertainties package, in
 its __init__.py:parse_error_in_parentheses().
 
 """
-_tkinds = frozenset(('none', 'log10', 'positive'))
-_dkinds = frozenset(('exact', 'symm', 'asymm', 'uncertain', 'upper', 'lower', 'unif'))
-_noextra_dkinds = frozenset(('exact', 'uncertain', 'upper', 'lower'))
-_yesextra_dkinds = frozenset(('symm', 'asymm'))
+_tkinds = frozenset(("none", "log10", "positive"))
+_dkinds = frozenset(("exact", "symm", "asymm", "uncertain", "upper", "lower", "unif"))
+_noextra_dkinds = frozenset(("exact", "uncertain", "upper", "lower"))
+_yesextra_dkinds = frozenset(("symm", "asymm"))
 
 
 def _split_decimal_col(floattext):
-    if '.' not in floattext:
-        return '$%s$ & ' % floattext
-    return '$%s$ & $.%s$ ' % tuple(floattext.split('.'))
+    if "." not in floattext:
+        return "$%s$ & " % floattext
+    return "$%s$ & $.%s$ " % tuple(floattext.split("."))
 
 
 class Textual(object):
     """A measurement recorded in textual form.
 
     Textual.from_exact(text, tkind='none') - `text` is passed to float()
     Textual.parse(text, tkind='none')      - `text` as described below.
@@ -1366,193 +1378,189 @@
     repval(limitsok=False) - Get single scalar "representative" value.
     limtype()              - -1 if upper limit; +1 if lower; 0 otherwise.
 
     Supported operations: unicode() str() repr() [latexification] -(neg) abs()
     + - * / **
 
     """
-    __slots__ = ('tkind', 'dkind', 'data')
+
+    __slots__ = ("tkind", "dkind", "data")
 
     def __init__(self, tkind, dkind, data):
         if tkind not in _tkinds:
             raise ValueError('unrecognized transformation kind "%s"' % tkind)
         if dkind not in _dkinds:
             raise ValueError('unrecognized distribution kind "%s"' % dkind)
         # FIXME: could/should check `data`.
 
         self.tkind = tkind
         self.dkind = dkind
         self.data = data
 
-
     @staticmethod
-    def from_exact(text, tkind='none'):
-        float(text) # check float-parseability.
-        return Textual(tkind, 'exact', text)
-
+    def from_exact(text, tkind="none"):
+        float(text)  # check float-parseability.
+        return Textual(tkind, "exact", text)
 
     @staticmethod
-    def parse(text, tkind='none'):
+    def parse(text, tkind="none"):
         # freestanding float() calls below are used to check
         # float-parseability of strings.
         # XXX: we do not check sanity when tkind is 'positive'!
 
-        if text[0] == '~':
-            dkind = 'uncertain'
+        if text[0] == "~":
+            dkind = "uncertain"
             data = text[1:]
             float(data)
-        elif text[0] == '<':
-            dkind = 'upper'
+        elif text[0] == "<":
+            dkind = "upper"
             data = text[1:]
             float(data)
-        elif text[0] == '>':
-            dkind = 'lower'
+        elif text[0] == ">":
+            dkind = "lower"
             data = text[1:]
             float(data)
-        elif 'to' in text:
-            lower, upper = text.split('to')
+        elif "to" in text:
+            lower, upper = text.split("to")
             f_lower = float(lower)
             f_upper = float(upper)
 
             if f_lower > f_upper:
                 upper, lower = lower, upper
                 f_upper, f_lower = f_lower, f_upper
 
-            if f_lower < 0 and tkind == 'positive':
-                raise ValueError('uniform interval is forced positive, but '
-                                 'got "%s"' % text)
+            if f_lower < 0 and tkind == "positive":
+                raise ValueError(
+                    "uniform interval is forced positive, but " 'got "%s"' % text
+                )
 
-            dkind = 'unif'
+            dkind = "unif"
             data = (lower, upper)
-        elif 'pm' in text:
-            val, uncert = text.split('pm')
+        elif "pm" in text:
+            val, uncert = text.split("pm")
             float(val)
             f_uncert = float(uncert)
-            if f_uncert <= 0.:
+            if f_uncert <= 0.0:
                 raise ValueError('uncertainty values must be positive; got "%s"' % text)
 
-            dkind = 'symm'
+            dkind = "symm"
             data = (val, uncert)
-        elif 'p' in text:
-            val, rhs = text.split('p', 1)
-            high, low = rhs.split('m', 1)
-            float(val) # checks parseability
+        elif "p" in text:
+            val, rhs = text.split("p", 1)
+            high, low = rhs.split("m", 1)
+            float(val)  # checks parseability
             f_high = float(high)
             f_low = float(low)
 
             if f_high <= 0:
-                raise ValueError('asymmetrical upper uncertainty must be positive')
+                raise ValueError("asymmetrical upper uncertainty must be positive")
             if f_low <= 0:
-                raise ValueError('asymmetrical lower uncertainty must be positive')
+                raise ValueError("asymmetrical lower uncertainty must be positive")
 
-            dkind = 'asymm'
+            dkind = "asymm"
             data = (val, high, low)
         else:
-            try: # plain float treated as unquantified
-                dkind = 'uncertain'
+            try:  # plain float treated as unquantified
+                dkind = "uncertain"
                 data = text
                 float(data)
             except ValueError:
-                raise ValueError('don\'t know how to parse measurement text: %s' % text)
+                raise ValueError("don't know how to parse measurement text: %s" % text)
 
         return Textual(tkind, dkind, data)
 
-
     # Textualization -- keep this up here since this is so closely tied to
     # construction via parse(). Note that unparse() loses the `tkind` info.
 
     def unparse(self):
-        if self.dkind == 'exact':
+        if self.dkind == "exact":
             return self.data
-        elif self.dkind == 'uncertain':
-            return '~' + self.data
-        elif self.dkind == 'symm':
-            return self.data[0] + 'pm' + self.data[1]
-        elif self.dkind == 'asymm':
-            return self.data[0] + 'p' + self.data[1] + 'm' + self.data[2]
-        elif self.dkind == 'upper':
-            return '<' + self.data
-        elif self.dkind == 'lower':
-            return '>' + self.data
-        elif self.dkind == 'unif':
-            return self.data[0] + 'to' + self.data[1]
-
+        elif self.dkind == "uncertain":
+            return "~" + self.data
+        elif self.dkind == "symm":
+            return self.data[0] + "pm" + self.data[1]
+        elif self.dkind == "asymm":
+            return self.data[0] + "p" + self.data[1] + "m" + self.data[2]
+        elif self.dkind == "upper":
+            return "<" + self.data
+        elif self.dkind == "lower":
+            return ">" + self.data
+        elif self.dkind == "unif":
+            return self.data[0] + "to" + self.data[1]
 
     def __repr__(self):
-        if self.tkind == 'none':
-            ttext = ''
+        if self.tkind == "none":
+            ttext = ""
         else:
-            ttext = ', %r' % (self.tkind, )
-
-        if self.dkind == 'exact':
-            return 'Textual.from_exact (%r%s)' % (self.data, ttext)
-        return 'Textual.parse(%r%s)' % (self.unparse(), ttext)
+            ttext = ", %r" % (self.tkind,)
 
+        if self.dkind == "exact":
+            return "Textual.from_exact (%r%s)" % (self.data, ttext)
+        return "Textual.parse(%r%s)" % (self.unparse(), ttext)
 
     def __unicode__(self):
-        if self.tkind == 'none':
+        if self.tkind == "none":
             return self.unparse()
-        return self.unparse() + ':' + self.tkind
+        return self.unparse() + ":" + self.tkind
 
     __str__ = unicode_to_str
 
     def __pk_fmtinfo__(self):
         t = self.unparse()
 
-        if self.tkind == 'log10':
-            ttag = 'L'
-        elif self.tkind == 'positive':
-            ttag = 'P'
+        if self.tkind == "log10":
+            ttag = "L"
+        elif self.tkind == "positive":
+            ttag = "P"
         else:
-            ttag = ''
+            ttag = ""
 
-        if self.dkind == 'exact':
-            dtag = 'f'
+        if self.dkind == "exact":
+            dtag = "f"
         else:
-            dtag = 'u'
+            dtag = "u"
 
         return ttag + dtag, t, False
 
-
     # "Unwrapping" -- conversion into either a scalar, Uval, or Lval. The
     # ability to apply various data transforms complicates this process.
 
     def _unwrap_pos(self):
         dkind = self.dkind
 
         # Deal with the easy cases ...
 
-        if dkind == 'exact':
+        if dkind == "exact":
             return float(self.data)
 
-        if dkind == 'upper':
+        if dkind == "upper":
             # Important case here: since we're positivized, the appropriate
             # Lval kind is 'tozero' rather than 'pastzero'. This allows
             # the caller to safely take the log or the reciprocal.
-            return Lval('tozero', float(self.data))
+            return Lval("tozero", float(self.data))
 
-        if dkind == 'lower':
-            return Lval('toinf', float(self.data))
+        if dkind == "lower":
+            return Lval("toinf", float(self.data))
 
-        if dkind == 'unif':
+        if dkind == "unif":
             # Limits should have been checked upon construction.
             lower, upper = map(float, self.data)
             return Uval.from_unif(lower, upper)
 
         # We have to get careful with the Uvals.
 
-        if dkind == 'symm':
+        if dkind == "symm":
             val = float(self.data[0])
             uncert = float(self.data[1])
             v = Uval.from_norm(val, uncert)
-        elif dkind == 'uncertain':
+        elif dkind == "uncertain":
             val = float(self.data)
             uncert = UQUANT_UNCERT * abs(val)
             v = Uval.from_norm(val, uncert)
-        elif dkind == 'asymm':
+        elif dkind == "asymm":
             val, dhigh, dlow = map(float, self.data)
             v = Uval.from_double_norm(val, dhigh, dlow)
 
         nnonpos = np.where(v.d <= 0)[0].size
 
         if nnonpos == 0:
             return v
@@ -1563,186 +1571,181 @@
             v.d = np.abs(v.d)
             return v
 
         # There are enough negative values that we're not comfortable with
         # drawing from a (double) normal distribution. Draw from a gamma
         # distribution instead.
 
-        if dkind == 'asymm':
+        if dkind == "asymm":
             # The gamma distribution only has two parameters, so what else can
             # we do?
             uncert = 0.5 * (dhigh + dlow)
 
         alpha, beta = find_gamma_params(val, uncert)
         return Uval.from_gamma(alpha, beta)
 
-
     def _unwrap_log(self):
         dkind = self.dkind
 
-        if dkind == 'exact':
-            return 10**float(self.data)
+        if dkind == "exact":
+            return 10 ** float(self.data)
 
-        if dkind == 'upper':
+        if dkind == "upper":
             # As with positive Textuals, it's important that we can return
             # a tozero limit here.
-            return Lval('tozero', 10 ** float(self.data))
+            return Lval("tozero", 10 ** float(self.data))
 
-        if dkind == 'lower':
-            return Lval('toinf', 10 ** float(self.data))
+        if dkind == "lower":
+            return Lval("toinf", 10 ** float(self.data))
 
-        if dkind == 'uncertain':
+        if dkind == "uncertain":
             # Assume UQUANT_UNCERT in (10**x), not in x itself
-            val = 10**float(self.data)
+            val = 10 ** float(self.data)
             return Uval.from_norm(val, UQUANT_UNCERT * abs(val))
 
-        if dkind == 'unif':
+        if dkind == "unif":
             # We'll yield a uniform distribution in log10(x), not x. I think
             # this is more desirable if someone writes "foo:Lu = 3.5to4.5".
             lower, upper = map(float, self.data)
-            return 10**Uval.from_unif(lower, upper)
+            return 10 ** Uval.from_unif(lower, upper)
 
-        if dkind == 'symm':
+        if dkind == "symm":
             val = float(self.data[0])
             uncert = float(self.data[1])
-            return 10**Uval.from_norm(val, uncert)
+            return 10 ** Uval.from_norm(val, uncert)
 
-        assert dkind == 'asymm'
+        assert dkind == "asymm"
         val, dhigh, dlow = map(float, self.data)
-        return 10**Uval.from_double_norm(val, dhigh, dlow)
-
+        return 10 ** Uval.from_double_norm(val, dhigh, dlow)
 
     def unwrap(self):
-        if self.tkind == 'log10':
+        if self.tkind == "log10":
             return self._unwrap_log()
-        if self.tkind == 'positive':
+        if self.tkind == "positive":
             return self._unwrap_pos()
 
         # No transformations applied:
         dkind = self.dkind
 
-        if dkind == 'exact':
+        if dkind == "exact":
             return float(self.data)
 
-        if dkind == 'upper':
+        if dkind == "upper":
             # Limits of magnitude-type quantities should always be of tkind
             # 'log10' or 'positive', so that we can return a 'tozero' Lval
             # rather than 'pastzero'. This is important for taking reciprocals
             # and/or logarithms.
             v = float(self.data)
             if v < 0:
-                return Lval('toinf', v)
-            return Lval('pastzero', v)
+                return Lval("toinf", v)
+            return Lval("pastzero", v)
 
-        if dkind == 'lower':
+        if dkind == "lower":
             v = float(self.data)
             if v < 0:
-                return Lval('pastzero', v)
-            return Lval('toinf', v)
+                return Lval("pastzero", v)
+            return Lval("toinf", v)
 
-        if dkind == 'unif':
+        if dkind == "unif":
             lower, upper = map(float, self.data)
             return Uval.from_unif(lower, upper)
 
-        if dkind == 'uncertain':
+        if dkind == "uncertain":
             val = float(self.data)
             return Uval.from_norm(val, UQUANT_UNCERT * abs(val))
 
-        if dkind == 'symm':
+        if dkind == "symm":
             val = float(self.data[0])
             uncert = float(self.data[1])
             return Uval.from_norm(val, uncert)
 
-        assert dkind == 'asymm'
+        assert dkind == "asymm"
         val, dhigh, dlow = map(float, self.data)
         return Uval.from_double_norm(val, dhigh, dlow)
 
-
     # Other numerical helpers.
 
     def repval(self, limitsok=False):
         """Get a best-effort representative value as a float. This can be
         DANGEROUS because it discards limit information, which is rarely wise."""
 
-        if not limitsok and self.dkind in ('lower', 'upper'):
+        if not limitsok and self.dkind in ("lower", "upper"):
             raise LimitError()
 
-        if self.dkind == 'unif':
+        if self.dkind == "unif":
             lower, upper = map(float, self.data)
             v = 0.5 * (lower + upper)
         elif self.dkind in _noextra_dkinds:
             v = float(self.data)
         elif self.dkind in _yesextra_dkinds:
             v = float(self.data[0])
         else:
-            raise RuntimeError('can\'t happen')
+            raise RuntimeError("can't happen")
 
-        if self.tkind == 'log10':
+        if self.tkind == "log10":
             return 10**v
         return v
 
-
     def limtype(self):
         """Return -1 if this value is an upper limit, 1 if it is a lower
         limit, 0 otherwise."""
 
-        if self.dkind == 'upper':
+        if self.dkind == "upper":
             return -1
-        if self.dkind == 'lower':
+        if self.dkind == "lower":
             return 1
         return 0
 
-
     # Latexification.
 
     def __pk_latex__(self):
-        if self.dkind == 'exact':
-            return r'$%s$' % self.data
-        if self.dkind == 'uncertain':
-            return r'$\sim$$%s$' % self.data
-        if self.dkind == 'symm':
-            return r'$%s \pm %s$' % self.data
-        if self.dkind == 'asymm':
-            return r'$%s^{+%s}_{-%s}$' % self.data
-        if self.dkind == 'upper':
-            return r'$<$$%s$' % self.data
-        if self.dkind == 'lower':
-            return r'$>$$%s$' % self.data
-        if self.dkind == 'unif':
-            return r'$%s$--$%s$' % self.data
-
+        if self.dkind == "exact":
+            return r"$%s$" % self.data
+        if self.dkind == "uncertain":
+            return r"$\sim$$%s$" % self.data
+        if self.dkind == "symm":
+            return r"$%s \pm %s$" % self.data
+        if self.dkind == "asymm":
+            return r"$%s^{+%s}_{-%s}$" % self.data
+        if self.dkind == "upper":
+            return r"$<$$%s$" % self.data
+        if self.dkind == "lower":
+            return r"$>$$%s$" % self.data
+        if self.dkind == "unif":
+            return r"$%s$--$%s$" % self.data
 
     def __pk_latex_u3col__(self):
-        if self.dkind == 'exact':
-            return r'\multicolumn{3}{c}{$%s$}' % self.data
-        if self.dkind == 'uncertain':
-            return r'\multicolumn{3}{c}{$\sim$$%s$}' % self.data
-        if self.dkind == 'symm':
-            return r'%s & $\pm\,%s$' % \
-                (_split_decimal_col(self.data[0]), self.data[1])
-        if self.dkind == 'asymm':
-            return r'%s & $\pm\,^{%s}_{%s}$' % \
-                (_split_decimal_col(self.data[0]), self.data[1], self.data[2])
-        if self.dkind == 'upper':
-            return r'\multicolumn{3}{c}{$<$$%s$}' % self.data
-        if self.dkind == 'lower':
-            return r'\multicolumn{3}{c}{$>$$%s$}' % self.data
-        if self.dkind == 'unif':
-            return r'\multicolumn{3}{c}{$%s$--$%s$}' % self.data
-
+        if self.dkind == "exact":
+            return r"\multicolumn{3}{c}{$%s$}" % self.data
+        if self.dkind == "uncertain":
+            return r"\multicolumn{3}{c}{$\sim$$%s$}" % self.data
+        if self.dkind == "symm":
+            return r"%s & $\pm\,%s$" % (_split_decimal_col(self.data[0]), self.data[1])
+        if self.dkind == "asymm":
+            return r"%s & $\pm\,^{%s}_{%s}$" % (
+                _split_decimal_col(self.data[0]),
+                self.data[1],
+                self.data[2],
+            )
+        if self.dkind == "upper":
+            return r"\multicolumn{3}{c}{$<$$%s$}" % self.data
+        if self.dkind == "lower":
+            return r"\multicolumn{3}{c}{$>$$%s$}" % self.data
+        if self.dkind == "unif":
+            return r"\multicolumn{3}{c}{$%s$--$%s$}" % self.data
 
     # Unary math -- we do the same thing as _make_textual_unary_math_generic()
     # below. Unlike Uval and Lval, algebra on Textuals is emphatically not
     # closed -- the result is always a non-Textual.
 
     def __neg__(self):
-        return _dispatch_unary_math('negative', False, self.unwrap())
+        return _dispatch_unary_math("negative", False, self.unwrap())
 
     def __abs__(self):
-        return _dispatch_unary_math('absolute', False, self.unwrap())
+        return _dispatch_unary_math("absolute", False, self.unwrap())
 
     # Binary math -- we delegate to the functions that are defined below.
 
     def __add__(self, other):
         return add(self, other)
 
     def __sub__(self, other):
@@ -1755,15 +1758,15 @@
         return divide(self, other)
 
     def __truediv__(self, other):
         return true_divide(self, other)
 
     def __pow__(self, other, module=None):
         if modulo is not None:
-            raise ValueError('powmod behavior forbidden with Textuals')
+            raise ValueError("powmod behavior forbidden with Textuals")
         return power(self, other)
 
     def __radd__(self, other):
         return add(other, self)
 
     def __rsub__(self, other):
         return subtract(other, self)
@@ -1775,90 +1778,92 @@
         return divide(other, self)
 
     def __rtruediv__(self, other):
         return true_divide(other, self)
 
     def __rpow__(self, other, module=None):
         if modulo is not None:
-            raise ValueError('powmod behavior forbidden with Textuals')
+            raise ValueError("powmod behavior forbidden with Textuals")
         return power(other, self)
 
 
 def _dispatch_unary_math(name, check_textual, value):
     if np.isscalar(value):
         table = scalar_unary_math
     elif isinstance(value, Uval):
         table = uval_unary_math
     elif isinstance(value, Lval):
         table = lval_unary_math
     elif check_textual and isinstance(value, Textual):
         table = textual_unary_math
     else:
-        raise ValueError('cannot treat %r as a scalar for %s' % (value, name))
+        raise ValueError("cannot treat %r as a scalar for %s" % (value, name))
 
     func = table.get(name)
     if func is None:
-        raise ValueError('no implementation of %s for %r' % (name, value))
+        raise ValueError("no implementation of %s for %r" % (name, value))
     return func(value)
 
 
 def _make_textual_unary_math_generic(name):
     # N.B.: unlike Uval and Lval functions, this assumes that `v` is in fact a
     # Textual.
     def textual_unary_math_generic(val):
         return _dispatch_unary_math(name, False, val.unwrap())
+
     return textual_unary_math_generic
 
 
 def _textual_unary_log10(val):
-    if val.tkind == 'log10':
-        return Textual('none', val.dkind, val.data)
-    return _dispatch_unary_math('log10', False, val.unwrap())
+    if val.tkind == "log10":
+        return Textual("none", val.dkind, val.data)
+    return _dispatch_unary_math("log10", False, val.unwrap())
 
 
 textual_unary_math = {
-    'absolute': _make_textual_unary_math_generic('absolute'),
-    'arccos': _make_textual_unary_math_generic('arccos'),
-    'arcsin': _make_textual_unary_math_generic('arcsin'),
-    'arctan': _make_textual_unary_math_generic('arctan'),
-    'cos': _make_textual_unary_math_generic('cos'),
-    'expm1': _make_textual_unary_math_generic('expm1'),
-    'exp': _make_textual_unary_math_generic('exp'),
-    'isfinite': lambda v: True, # legal Textuals can never yield inf or nan
-    'log10': _textual_unary_log10,
-    'log1p': _make_textual_unary_math_generic('log1p'),
-    'log2': _make_textual_unary_math_generic('log2'),
-    'log': _make_textual_unary_math_generic('log'),
-    'negative': _make_textual_unary_math_generic('negative'),
-    'reciprocal': _make_textual_unary_math_generic('reciprocal'),
-    'sin': _make_textual_unary_math_generic('sin'),
-    'sqrt': _make_textual_unary_math_generic('sqrt'),
-    'square':  _make_textual_unary_math_generic('square'),
-    'tan': _make_textual_unary_math_generic('tan'),
+    "absolute": _make_textual_unary_math_generic("absolute"),
+    "arccos": _make_textual_unary_math_generic("arccos"),
+    "arcsin": _make_textual_unary_math_generic("arcsin"),
+    "arctan": _make_textual_unary_math_generic("arctan"),
+    "cos": _make_textual_unary_math_generic("cos"),
+    "expm1": _make_textual_unary_math_generic("expm1"),
+    "exp": _make_textual_unary_math_generic("exp"),
+    "isfinite": lambda v: True,  # legal Textuals can never yield inf or nan
+    "log10": _textual_unary_log10,
+    "log1p": _make_textual_unary_math_generic("log1p"),
+    "log2": _make_textual_unary_math_generic("log2"),
+    "log": _make_textual_unary_math_generic("log"),
+    "negative": _make_textual_unary_math_generic("negative"),
+    "reciprocal": _make_textual_unary_math_generic("reciprocal"),
+    "sin": _make_textual_unary_math_generic("sin"),
+    "sqrt": _make_textual_unary_math_generic("sqrt"),
+    "square": _make_textual_unary_math_generic("square"),
+    "tan": _make_textual_unary_math_generic("tan"),
 }
 
 
 # Now, a library of metadata-esque functions that will handle anything you
 # throw at them: scalars, Uvals, Lvals, and Textuals.
 
+
 def is_measurement(obj):
     return np.isscalar(obj) or isinstance(obj, (Uval, Lval, Textual))
 
 
 def unwrap(msmt):
     """Convert the value into the most basic representation that we can do
     math on: float if possible, then Uval, then Lval."""
 
     if np.isscalar(msmt):
         return float(msmt)
     if isinstance(msmt, (Uval, Lval)):
         return msmt
     if isinstance(msmt, Textual):
         return msmt.unwrap()
-    raise ValueError('don\'t know how to treat %r as a measurement' % msmt)
+    raise ValueError("don't know how to treat %r as a measurement" % msmt)
 
 
 def typealign(origmsmt1, origmsmt2):
     msmt1 = origmsmt1
     if isinstance(msmt1, Textual):
         msmt1 = msmt1.unwrap()
     msmt2 = origmsmt2
@@ -1873,62 +1878,63 @@
         return msmt1, Uval.from_other(msmt2)
     if isinstance(msmt2, Uval):
         return Uval.from_other(msmt1), msmt2
 
     try:
         return float(msmt1), float(msmt2)
     except Exception:
-        raise ValueError('cannot treat %r and %r as numeric types'
-                         % (origmsmt1, origmsmt2))
+        raise ValueError(
+            "cannot treat %r and %r as numeric types" % (origmsmt1, origmsmt2)
+        )
 
 
 def repval(msmt, limitsok=False):
     """Get a best-effort representative value as a float. This is DANGEROUS
     because it discards limit information, which is rarely wise. m_liminfo()
     or m_unwrap() are recommended instead."""
 
     if np.isscalar(msmt):
         return float(msmt)
     if isinstance(msmt, Uval):
         return msmt.repvals(uval_default_repval_method)[0]
     if isinstance(msmt, Lval):
-        if not limitsok and msmt.kind in('tozero', 'toinf', 'pastzero'):
+        if not limitsok and msmt.kind in ("tozero", "toinf", "pastzero"):
             raise LimitError()
         return msmt.value
     if isinstance(msmt, Textual):
         return msmt.repval(limitsok=limitsok)
 
-    raise ValueError('don\'t know how to treat %r as a measurement' % msmt)
+    raise ValueError("don't know how to treat %r as a measurement" % msmt)
 
 
 def limtype(msmt):
     """Return -1 if this value is some kind of upper limit, 1 if this value
     is some kind of lower limit, 0 otherwise."""
 
     if np.isscalar(msmt):
         return 0
     if isinstance(msmt, Uval):
         return 0
     if isinstance(msmt, Lval):
-        if msmt.kind == 'undef':
-            raise ValueError('no simple limit type for Lval %r' % msmt)
+        if msmt.kind == "undef":
+            raise ValueError("no simple limit type for Lval %r" % msmt)
 
         # Quasi-hack here: limits of ('tozero', [positive number]) are
         # reported as upper limits. In a plot full of fluxes this would be
         # what makes sense, but note that this would be misleading if the
         # quantity in question was something that could go negative.
         p = msmt._polarity()
         if p == -2 or p == 1:
             return -1
         if p == 2 or p == -1:
             return 1
         return 0
     if isinstance(msmt, Textual):
         return msmt.limtype()
-    raise ValueError('don\'t know how to treat %r as a measurement' % msmt)
+    raise ValueError("don't know how to treat %r as a measurement" % msmt)
 
 
 def liminfo(msmt):
     """Return (limtype, repval). `limtype` is -1 for upper limits, 1 for lower
     limits, and 0 otherwise; repval is a best-effort representative scalar value
     for this measurement."""
 
@@ -1948,15 +1954,15 @@
     if isinstance(msmt, Uval):
         rep, plus1, minus1 = msmt.repvals(uval_default_repval_method)
         return 0, rep, plus1, minus1
 
     if isinstance(msmt, Lval):
         return limtype(msmt), msmt.value, msmt.value, msmt.value
 
-    raise ValueError('don\'t know how to treat %r as a measurement' % msmt)
+    raise ValueError("don't know how to treat %r as a measurement" % msmt)
 
 
 # Unary numerical functions.
 #
 # Here we just have to look up the appropriate table of unary math operations
 # and delegate. The implemented functions are those in the scalar_unary_math
 # dict.
@@ -1967,32 +1973,35 @@
 # deg2rad degrees fabs fix floor frexp hypot i0 imag ldexp modf rad2deg
 # radians real rint round_ sign signbit sinc sinh tanh trunc unwrap
 #
 # Skipped core Python unary operators:
 #
 # abs coerce complex hex index int invert float long neg nonzero oct pos
 
+
 def _make_wrapped_unary_math(name):
     def unary_mathfunc(val):
         rv = _dispatch_unary_math(name, True, val)
-        if not _dispatch_unary_math('isfinite', True, rv):
-            raise ValueError('out-of-bounds input %r to %s' % (val, name))
+        if not _dispatch_unary_math("isfinite", True, rv):
+            raise ValueError("out-of-bounds input %r to %s" % (val, name))
         return rv
+
     return unary_mathfunc
 
 
 def _init_unary_math():
     g = globals()
 
-    for name in six.iterkeys(scalar_unary_math):
-        if name == 'isfinite':
-            g[name] = lambda v: _dispatch_unary_math('isfinite', True, v)
+    for name in scalar_unary_math.keys():
+        if name == "isfinite":
+            g[name] = lambda v: _dispatch_unary_math("isfinite", True, v)
         else:
             g[name] = _make_wrapped_unary_math(name)
 
+
 _init_unary_math()
 
 
 # Binary numerical functions.
 #
 # Here we have to coerce the arguments to the ~"highest-level" type that's
 # relevant. Then we can delegate to the class's __op__ functions. Note that
@@ -2004,50 +2013,56 @@
 #
 # fmod maximum minimum mod=remainder logaddexp2 logaddexp
 #
 # Skipped core Python binary operators:
 #
 # and cmp eq ge gt le lshift lt ne or rshift xor
 
+
 def _make_wrapped_binary_math(opfunc):
     def binary_mathfunc(val1, val2):
         a1, a2 = typealign(val1, val2)
         return opfunc(a1, a2)
+
     return binary_mathfunc
 
 
 add = _make_wrapped_binary_math(operator.add)
 floor_divide = _make_wrapped_binary_math(operator.floordiv)
 multiply = _make_wrapped_binary_math(operator.mul)
 power = _make_wrapped_binary_math(operator.pow)
 subtract = _make_wrapped_binary_math(operator.sub)
 true_divide = _make_wrapped_binary_math(operator.truediv)
-divide = true_divide # are we supposed to respect Py2 plain-div semantics?
+divide = true_divide  # are we supposed to respect Py2 plain-div semantics?
 
 
 # Parsing and formatting of measurements and other quantities.
 
+
 def _parse_bool(text):
     if not len(text):
         return False
-    if text == 'y':
+    if text == "y":
         return True
-    raise ValueError('illegal bool textualization: expect empty or "y"; '
-                     'got "%s"' % text)
+    raise ValueError(
+        'illegal bool textualization: expect empty or "y"; ' 'got "%s"' % text
+    )
 
 
 def _maybe(subparse):
     def parser(text):
         if not len(text):
             return None
         return subparse(text)
+
     return parser
 
 
-_ttkinds = {'': 'none', 'L': 'log10', 'P': 'positive'}
+_ttkinds = {"": "none", "L": "log10", "P": "positive"}
+
 
 def _maybe_parse_exact(text, tkind):
     if not len(text):
         return None
     return Textual.from_exact(text, _ttkinds[tkind])
 
 
@@ -2055,46 +2070,47 @@
     if not len(text):
         return None
     return Textual.parse(text, _ttkinds[tkind])
 
 
 parsers = {
     # maps 'type tag string' to 'parsing function'.
-    'x': None,
-    'b': _parse_bool,
-    'i': _maybe(int),
-    's': _maybe(text_type),
-    'f': lambda t: _maybe_parse_exact(t, ''),
-    'Lf': lambda t: _maybe_parse_exact(t, 'L'),
-    'Pf': lambda t: _maybe_parse_exact(t, 'P'),
-    'u': lambda t: _maybe_parse_uncert(t, ''),
-    'Lu': lambda t: _maybe_parse_uncert(t, 'L'),
-    'Pu': lambda t: _maybe_parse_uncert(t, 'P'),
+    "x": None,
+    "b": _parse_bool,
+    "i": _maybe(int),
+    "s": _maybe(str),
+    "f": lambda t: _maybe_parse_exact(t, ""),
+    "Lf": lambda t: _maybe_parse_exact(t, "L"),
+    "Pf": lambda t: _maybe_parse_exact(t, "P"),
+    "u": lambda t: _maybe_parse_uncert(t, ""),
+    "Lu": lambda t: _maybe_parse_uncert(t, "L"),
+    "Pu": lambda t: _maybe_parse_uncert(t, "P"),
 }
 
+
 def fmtinfo(value):
     """Returns (typetag, text, is_imprecise). Unlike other functions that operate
     on measurements, this also operates on bools, ints, and strings.
 
     """
     if value is None:
-        raise ValueError('cannot format None!')
+        raise ValueError("cannot format None!")
 
-    if isinstance(value, text_type):
-        return '', value, False
+    if isinstance(value, str):
+        return "", value, False
 
     if isinstance(value, bool):
         # Note: isinstance(True, int) = True, so this must come before the next case.
         if value:
-            return 'b', 'y', False
-        return 'b', '', False
+            return "b", "y", False
+        return "b", "", False
 
-    if isinstance(value, six.integer_types):
-        return 'i', text_type(value), False
+    if isinstance(value, int):
+        return "i", str(value), False
 
     if isinstance(value, float):
-        return 'f', text_type(value), True
+        return "f", str(value), True
 
-    if hasattr(value, '__pk_fmtinfo__'):
+    if hasattr(value, "__pk_fmtinfo__"):
         return value.__pk_fmtinfo__()
 
-    raise ValueError('don\'t know how to format %r as a measurement' % value)
+    raise ValueError("don't know how to format %r as a measurement" % value)
```

### Comparing `pwkit-1.1.1/pwkit/ndshow_gtk2.py` & `pwkit-1.2.0/pwkit/ndshow_gtk3.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2012-2014 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2012-2015 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
-"""pwkit.ndshow_gtk2 - visualize data arrays with the Gtk+2 toolkit.
+"""pwkit.ndshow_gtk3 - visualize data arrays with the Gtk+3 toolkit.
 
 Functions:
 
 view     - Show a GUI visualizing a 2D array.
 cycle    - Show a GUI cycling through planes of a 3D array.
 
 Classes:
@@ -16,90 +16,104 @@
 Cycler   - A GUI window for cycling through planes of a 3D array.
 
 
 UI features of the viewport:
 
 - click-drag to pan
 - scrollwheel to zoom in/out (Ctrl to do so more aggressively)
--   (Shift to change color scale adjustment sensitivity)
+  (Shift to change color scale adjustment sensitivity)
 - double-click to recenter
 - shift-click-drag to adjust color scale (prototype)
 
 Added by the toplevel window viewer:
 
 - Ctrl-A to autoscale data to fit window
 - Ctrl-E to center the data in the window
 - Ctrl-F to fullscreen the window
 - Escape to un-fullscreen it
 - Ctrl-W to close the window
 - Ctrl-1 to set scale to unity
 - Ctrl-S to save the data to "data.png" under the current rendering options
   (but not zoomed to the current view of the data).
+- z/Z to zoom in and out - for when trackpad scrolling motion doesn't work
 
 Added by cycler:
 
 - Ctrl-K to move to next plane
 - Ctrl-J to move to previous plane
 - Ctrl-C to toggle automatic cycling
 
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 __all__ = str("Cycler Viewer Viewport cycle view").split()
 
-import cairo, glib, gtk, numpy as np, sys, time
+import sys
+import numpy as np
+import cairo
+
+# There is a gi.repository.cairo but it barely exposes any API, and it seems
+# like you're not really supposed to use it.
+import gi
+
+gi.require_version("Gdk", "3.0")
+gi.require_version("Gtk", "3.0")
+from gi.repository import GLib, GObject, Gdk, Gtk
 
 from . import PKError
 from .data_gui_helpers import Clipper, ColorMapper
 
 
 DRAG_TYPE_NONE = 0
 DRAG_TYPE_PAN = 1
 DRAG_TYPE_TUNER = 2
 
 DEFAULT_WIN_WIDTH = 800
 DEFAULT_WIN_HEIGHT = 600
 
 
-class Viewport(gtk.DrawingArea):
-    bgpattern = None
+class Viewport(Gtk.DrawingArea):
+    __gtype_name__ = "Viewport"
 
-    getshape = None
-    settuning = None
-    getsurface = None
-    onmotion = None
-    drawoverlay = None
+    bgpattern = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    getshape = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    settuning = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    getsurface = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    onmotion = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    drawoverlay = GObject.Property(type=GObject.TYPE_PYOBJECT)
 
-    centerx = 0
-    centery = 0
+    centerx = GObject.Property(type=GObject.TYPE_FLOAT, default=0.0)
+    centery = GObject.Property(type=GObject.TYPE_FLOAT, default=0.0)
     # The data pixel coordinate of the central pixel of the displayed window.
 
-    scale = None
+    scale = GObject.Property(type=GObject.TYPE_FLOAT, default=-1.0)
     # From data space to viewer space: e.g., scale = 2 means that each data
     # pixel occupies 2 pixels on-screen.
 
-    needtune = True
-    tunerx = 0
-    tunery = 1.0
-    tunerscale = 200
-
-    drag_type = DRAG_TYPE_NONE
-    drag_win_x0 = drag_win_y0 = None
-    drag_dc_x0 = drag_dc_y0 = None
+    needtune = GObject.Property(type=GObject.TYPE_BOOLEAN, default=True)
+    tunerx = GObject.Property(type=GObject.TYPE_FLOAT, default=0.0)
+    tunery = GObject.Property(type=GObject.TYPE_FLOAT, default=1.0)
+    tunerscale = GObject.Property(type=GObject.TYPE_FLOAT, default=200.0)
+
+    drag_type = GObject.Property(type=GObject.TYPE_INT, default=DRAG_TYPE_NONE)
+    drag_win_x0 = GObject.Property(type=GObject.TYPE_FLOAT, default=0.0)
+    drag_win_y0 = GObject.Property(type=GObject.TYPE_FLOAT, default=0.0)
+    drag_dc_x0 = GObject.Property(type=GObject.TYPE_FLOAT, default=0.0)
+    drag_dc_y0 = GObject.Property(type=GObject.TYPE_FLOAT, default=0.0)
 
     def __init__(self):
         super(Viewport, self).__init__()
         self.add_events(
-            gtk.gdk.POINTER_MOTION_MASK
-            | gtk.gdk.BUTTON_PRESS_MASK
-            | gtk.gdk.BUTTON_RELEASE_MASK
-            | gtk.gdk.SCROLL_MASK
+            Gdk.EventMask.POINTER_MOTION_MASK
+            | Gdk.EventMask.BUTTON_PRESS_MASK
+            | Gdk.EventMask.BUTTON_RELEASE_MASK
+            | Gdk.EventMask.SCROLL_MASK
         )
-        self.connect("expose-event", self._on_expose)
+        self.connect("draw", self._on_draw)
         self.connect("scroll-event", self._on_scroll)
         self.connect("button-press-event", self._on_button_press)
         self.connect("button-release-event", self._on_button_release)
         self.connect("motion-notify-event", self._on_motion_notify)
 
         self.bgpattern = cairo.SolidPattern(0.1, 0.1, 0.1)
 
@@ -131,21 +145,19 @@
     def set_overlay_drawer(self, drawoverlay):
         if drawoverlay is not None and not callable(drawoverlay):
             raise ValueError()
         self.drawoverlay = drawoverlay
         return self
 
     def autoscale(self):
-        if self.allocation is None:
-            raise PKError("must be called after allocation")
         if self.getshape is None:
             raise PKError("must be called after setting shape-getter")
 
-        aw = self.allocation.width
-        ah = self.allocation.height
+        aw = self.get_allocated_width()
+        ah = self.get_allocated_height()
 
         dw, dh = self.getshape()
 
         wratio = float(aw) / dw
         hratio = float(ah) / dh
 
         self.scale = min(wratio, hratio)
@@ -179,50 +191,52 @@
         surface.write_to_png(filename)
 
     def write_view_as_png(self, filename):
         if self.getshape is None:
             raise PKError("must be called after setting shape-getter")
         if self.getsurface is None:
             raise PKError("must be called after setting surface-getter")
-        if self.allocation is None:
-            raise PKError("must be called after allocation")
 
-        width = self.allocation.width
-        height = self.allocation.height
+        width = self.get_allocated_width()
+        height = self.get_allocated_height()
 
         stride = cairo.ImageSurface.format_stride_for_width(cairo.FORMAT_ARGB32, width)
         assert stride % 4 == 0  # stride is in bytes
         viewdata = np.empty((height, stride // 4), dtype=np.uint32)
         viewsurface = cairo.ImageSurface.create_for_data(
             viewdata, cairo.FORMAT_ARGB32, width, height, stride
         )
         ctxt = cairo.Context(viewsurface)
         self._draw_in_context(ctxt, width, height)
         viewsurface.write_to_png(filename)
 
     def get_pointer_data_coords(self):
-        if self.allocation is None:
-            raise PKError("must be called after allocation")
-        if self.scale is None:
+        if self.scale < 0.0:
             self.autoscale()
 
         x, y = self.get_pointer()
-        dx = x - 0.5 * self.allocation.width
-        dy = y - 0.5 * self.allocation.height
+        dx = x - 0.5 * self.get_allocated_width()
+        dy = y - 0.5 * self.get_allocated_height()
         datax = self.centerx + dx / self.scale
         datay = self.centery + dy / self.scale
         return datax, datay
 
-    def _draw_in_context(self, ctxt, width, height):
+    def _on_draw(self, widget, ctxt):
+        if self.getshape is None or self.getsurface is None:
+            return False
+
+        width = self.get_allocated_width()
+        height = self.get_allocated_height()
+
         if self.getshape is None or self.getsurface is None:
             raise PKError(
                 "must be called after setting shape-getter " "and surface-getter"
             )
 
-        if self.scale is None:
+        if self.scale < 0.0:
             self.autoscale()
         if self.needtune:
             self.settuning(self.tunerx, self.tunery)
             self.needtune = False
 
         # Our data coordinates have integral pixel values being in the
         # centers of pixels; Cairo uses edges. That's the origin of the
@@ -246,96 +260,89 @@
         pat.set_filter(cairo.FILTER_NEAREST)
         ctxt.paint()
         ctxt.restore()
 
         if self.drawoverlay is not None:
             self.drawoverlay(ctxt, width, height, -xoffset, -yoffset, self.scale)
 
-    def _on_expose(self, alsoself, event):
-        if self.getshape is None or self.getsurface is None:
-            return False
-
-        self._draw_in_context(
-            self.window.cairo_create(), self.allocation.width, self.allocation.height
-        )
-        return True
+        return False
 
     def _on_scroll(self, alsoself, event):
-        modmask = gtk.accelerator_get_default_mod_mask()
+        modmask = Gtk.accelerator_get_default_mod_mask()
 
-        if (event.state & modmask) in (0, gtk.gdk.CONTROL_MASK):
+        if (event.state & modmask) in (0, Gdk.ModifierType.CONTROL_MASK):
             oldscale = self.scale
             newscale = self.scale
 
-            if event.state & modmask == gtk.gdk.CONTROL_MASK:
+            if event.state & modmask == Gdk.ModifierType.CONTROL_MASK:
                 factor = 1.2
             else:
                 factor = 1.05
 
-            if event.direction == gtk.gdk.SCROLL_UP:
+            if event.direction == Gdk.ScrollDirection.UP:
                 newscale *= factor
 
-            if event.direction == gtk.gdk.SCROLL_DOWN:
+            if event.direction == Gdk.ScrollDirection.DOWN:
                 newscale /= factor
 
             if newscale == oldscale:
                 return False
 
             self.scale = newscale
             self.queue_draw()
             return True
 
-        if (event.state & modmask) == gtk.gdk.SHIFT_MASK:
+        if (event.state & modmask) == Gdk.ModifierType.SHIFT_MASK:
             oldscale = self.tunerscale
             newscale = self.tunerscale
 
-            if event.direction == gtk.gdk.SCROLL_UP:
+            if event.direction == Gdk.ScrollDirection.UP:
                 newscale *= 1.05
 
-            if event.direction == gtk.gdk.SCROLL_DOWN:
+            if event.direction == Gdk.ScrollDirection.DOWN:
                 newscale /= 1.05
 
             if newscale == oldscale:
                 return False
 
             self.tunerscale = newscale
             return True
 
         return False
 
     def _on_button_press(self, alsoself, event):
-        modmask = gtk.accelerator_get_default_mod_mask()
+        modmask = Gtk.accelerator_get_default_mod_mask()
 
-        if event.type == gtk.gdk.BUTTON_PRESS and event.button == 1:
+        if event.type == Gdk.EventType.BUTTON_PRESS and event.button == 1:
             self.grab_add()
             self.drag_win_x0 = event.x
             self.drag_win_y0 = event.y
 
             if (event.state & modmask) == 0:
                 self.drag_type = DRAG_TYPE_PAN
                 self.drag_dc_x0 = self.centerx
                 self.drag_dc_y0 = self.centery
                 return True
 
-            if (event.state & modmask) == gtk.gdk.SHIFT_MASK:
+            if (event.state & modmask) == Gdk.ModifierType.SHIFT_MASK:
                 self.drag_type = DRAG_TYPE_TUNER
                 self.drag_dc_x0 = self.tunerx
                 self.drag_dc_y0 = self.tunery
                 return True
 
             return False
 
-        if event.type == gtk.gdk._2BUTTON_PRESS and event.button == 1:
-            dx = event.x - 0.5 * self.allocation.width
-            dy = event.y - 0.5 * self.allocation.height
+        if event.type == Gdk.EventType._2BUTTON_PRESS and event.button == 1:
+            dx = event.x - 0.5 * self.get_allocated_width()
+            dy = event.y - 0.5 * self.get_allocated_height()
 
             if (event.state & modmask) == 0:
                 self.centerx += dx / self.scale
                 self.centery += dy / self.scale
-            elif (event.state & modmask) == gtk.gdk.SHIFT_MASK:
+            elif (event.state & modmask) == Gdk.ModifierType.SHIFT_MASK:
                 self.tunerx += dx / self.tunerscale
                 self.tunery += dy / self.tunerscale
                 self.needtune = True
             else:
                 return False
 
             self.queue_draw()
@@ -344,15 +351,15 @@
             self.grab_remove()
             self.drag_type = DRAG_TYPE_NONE
             return True
 
         return False
 
     def _on_button_release(self, alsoself, event):
-        if event.type == gtk.gdk.BUTTON_RELEASE and event.button == 1:
+        if event.type == Gdk.EventType.BUTTON_RELEASE and event.button == 1:
             if self.drag_type == DRAG_TYPE_NONE:
                 return False
 
             self.grab_remove()
             dx = self.drag_win_x0 - event.x
             dy = self.drag_win_y0 - event.y
 
@@ -362,26 +369,26 @@
             elif self.drag_type == DRAG_TYPE_TUNER:
                 self.tunerx = self.drag_dc_x0 - dx / self.tunerscale
                 self.tunery = self.drag_dc_y0 - dy / self.tunerscale
                 self.needtune = True
             else:
                 return False
 
-            self.drag_win_x0 = self.drag_win_y0 = None
-            self.drag_dc_x0 = self.drag_dc_y0 = None
+            self.drag_win_x0 = self.drag_win_y0 = 0.0
+            self.drag_dc_x0 = self.drag_dc_y0 = 0.0
             self.drag_type = DRAG_TYPE_NONE
             self.queue_draw()
             return True
 
         return False
 
     def _on_motion_notify(self, alsoself, event):
         if self.onmotion is not None:
-            dx = event.x - 0.5 * self.allocation.width
-            dy = event.y - 0.5 * self.allocation.height
+            dx = event.x - 0.5 * self.get_allocated_width()
+            dy = event.y - 0.5 * self.get_allocated_height()
             datax = self.centerx + dx / self.scale
             datay = self.centery + dy / self.scale
             self.onmotion(datax, datay)
 
         if self.drag_type == DRAG_TYPE_NONE:
             return False
         elif self.drag_type == DRAG_TYPE_PAN:
@@ -404,25 +411,25 @@
     def __init__(
         self,
         title="Array Viewer",
         default_width=DEFAULT_WIN_WIDTH,
         default_height=DEFAULT_WIN_HEIGHT,
     ):
         self.viewport = Viewport()
-        self.win = gtk.Window(gtk.WINDOW_TOPLEVEL)
+        self.win = Gtk.Window(type=Gtk.WindowType.TOPLEVEL)
         self.win.set_title(title)
         self.win.set_default_size(default_width, default_height)
         self.win.connect("key-press-event", self._on_key_press)
 
-        vb = gtk.VBox()
+        vb = Gtk.VBox()
         vb.pack_start(self.viewport, True, True, 2)
-        hb = gtk.HBox()
+        hb = Gtk.HBox()
         vb.pack_start(hb, False, True, 2)
 
-        self.status_label = gtk.Label()
+        self.status_label = Gtk.Label()
         self.status_label.set_alignment(0, 0.5)
         hb.pack_start(self.status_label, True, True, 2)
 
         self.status_label.set_markup("Temp")
 
         self.win.add(vb)
 
@@ -446,17 +453,17 @@
         return self
 
     def set_overlay_drawer(self, drawoverlay):
         self.viewport.set_overlay_drawer(drawoverlay)
         return self
 
     def _on_key_press(self, widget, event):
-        kn = gtk.gdk.keyval_name(event.keyval)
-        modmask = gtk.accelerator_get_default_mod_mask()
-        isctrl = (event.state & modmask) == gtk.gdk.CONTROL_MASK
+        kn = Gdk.keyval_name(event.keyval)
+        modmask = Gtk.accelerator_get_default_mod_mask()
+        isctrl = (event.state & modmask) == Gdk.ModifierType.CONTROL_MASK
 
         if kn == "a" and isctrl:
             self.viewport.autoscale()
             return True
 
         if kn == "e" and isctrl:
             self.viewport.center()
@@ -482,25 +489,46 @@
         if kn == "s" and isctrl:
             print("Writing data.png ...", end="")
             sys.stdout.flush()
             self.viewport.write_data_as_png("data.png")
             print("done")
             return True
 
+        if kn == "z":
+            if isctrl:
+                self.viewport.scale *= 1.2
+            else:
+                self.viewport.scale *= 1.05
+            self.viewport.queue_draw()
+            return True
+
+        if kn == "Z":
+            if isctrl:
+                self.viewport.scale /= 1.2
+            else:
+                self.viewport.scale /= 1.05
+            self.viewport.queue_draw()
+            return True
+
         return False
 
 
 def view(
     array,
     title="Array Viewer",
     colormap="black_to_blue",
     toworld=None,
     drawoverlay=None,
     yflip=False,
+    tostatus=None,
+    run_main=True,
 ):
+    if toworld is not None and tostatus is not None:
+        raise ValueError('only one of "toworld" and "tostatus" may be given')
+
     clipper = Clipper()
     clipper.alloc_buffer(array)
     clipper.set_tile_size()
     clipper.default_bounds(array)
     processed = clipper.buffer
 
     mapper = ColorMapper(colormap)
@@ -540,61 +568,51 @@
 
     # I originally had the is_masked call inside fmtstatus and somehow it
     # ended up causing large lags in the label updates. Can't be that
     # CPU-intensive, right??
 
     nomask = not np.ma.is_masked(array) or array.mask is np.ma.nomask
 
-    if toworld is None:
+    if tostatus is None:
+        if toworld is None:
+            tostatus = lambda t: ""
+        else:
+            from .astutil import fmthours, fmtdeglat
 
-        def fmtstatus(x, y):
-            s = ""
-            row = int(np.floor(y + 0.5))
-            col = int(np.floor(x + 0.5))
-            if row >= 0 and col >= 0 and row < h and col < w:
-                if nomask or not array.mask[row, col]:
-                    s += "%g " % array[row, col]
-            if yflip:
-                y = h - 1 - y
-                row = h - 1 - row
-            return s + "[%d,%d] x=%.1f y=%.1f" % (row, col, x, y)
+            def tostatus(y_and_x):
+                lat, lon = toworld(y_and_x)
+                return "lat=%s lon=%s" % (fmtdeglat(lat), fmthours(lon))
 
-    else:
-        from .astutil import fmthours, fmtdeglat
+    def fmtstatus(x, y):
+        s = ""
+        row = int(np.floor(y + 0.5))
+        col = int(np.floor(x + 0.5))
+        if row >= 0 and col >= 0 and row < h and col < w:
+            if nomask or not array.mask[row, col]:
+                s += "%g " % array[row, col]
+        if yflip:
+            y = h - 1 - y
+            row = h - 1 - row
 
-        def fmtstatus(x, y):
-            s = ""
-            row = int(np.floor(y + 0.5))
-            col = int(np.floor(x + 0.5))
-            if row >= 0 and col >= 0 and row < h and col < w:
-                if nomask or not array.mask[row, col]:
-                    s += "%g " % array[row, col]
-            if yflip:
-                y = h - 1 - y
-                row = h - 1 - row
-            lat, lon = toworld([y, x])
-            s += "[%d,%d] x=%.1f y=%.1f lat=%s lon=%s" % (
-                row,
-                col,
-                x,
-                y,
-                fmtdeglat(lat),
-                fmthours(lon),
-            )
-            return s
+        s += "[%d,%d] x=%.1f y=%.1f %s" % (row, col, x, y, tostatus(np.array([y, x])))
+        return s
 
     viewer = Viewer(title=title)
     viewer.set_shape_getter(getshape)
     viewer.set_tuning_setter(settuning)
     viewer.set_surface_getter(getsurface)
     viewer.set_status_formatter(fmtstatus)
     viewer.set_overlay_drawer(drawoverlay)
     viewer.win.show_all()
-    viewer.win.connect("destroy", gtk.main_quit)
-    gtk.main()
+
+    if run_main:
+        viewer.win.connect("destroy", Gtk.main_quit)
+        Gtk.main()
+    else:
+        viewer.win.connect("destroy", lambda e: viewer.win.destroy())
 
 
 class Cycler(Viewer):
     getn = None
     getshapei = None
     getdesci = None
     settuningi = None
@@ -610,34 +628,34 @@
         default_width=DEFAULT_WIN_WIDTH,
         default_height=DEFAULT_WIN_HEIGHT,
         cadence=0.6,
     ):
         self.cadence = cadence
 
         self.viewport = Viewport()
-        self.win = gtk.Window(gtk.WINDOW_TOPLEVEL)
+        self.win = Gtk.Window(type=Gtk.WindowType.TOPLEVEL)
         self.win.set_title(title)
         self.win.set_default_size(default_width, default_height)
         self.win.connect("key-press-event", self._on_key_press)
         self.win.connect("realize", self._on_realize)
         self.win.connect("unrealize", self._on_unrealize)
 
-        vb = gtk.VBox()
+        vb = Gtk.VBox()
         vb.pack_start(self.viewport, True, True, 2)
-        hb = gtk.HBox()
+        hb = Gtk.HBox()
         vb.pack_start(hb, False, True, 2)
-        self.status_label = gtk.Label()
+        self.status_label = Gtk.Label()
         self.status_label.set_alignment(0, 0.5)
         hb.pack_start(self.status_label, True, True, 2)
-        self.plane_label = gtk.Label()
+        self.plane_label = Gtk.Label()
         self.plane_label.set_alignment(0, 0.5)
         hb.pack_start(self.plane_label, True, True, 2)
-        self.desc_label = gtk.Label()
+        self.desc_label = Gtk.Label()
         hb.pack_start(self.desc_label, True, True, 2)
-        self.cycle_tbutton = gtk.ToggleButton("Cycle")
+        self.cycle_tbutton = Gtk.ToggleButton(label="Cycle")
         hb.pack_start(self.cycle_tbutton, False, True, 2)
         self.win.add(vb)
 
         self.viewport.set_shape_getter(self._get_shape)
         self.viewport.set_surface_getter(self._get_surface)
         self.viewport.set_tuning_setter(self._set_tuning)
 
@@ -668,14 +686,16 @@
 
     def _set_tuning(self, tunerx, tunery):
         if self.i is None:
             self.set_current(0)
         self.settuningi(self.i, tunerx, tunery)
         self.needtune.fill(True)
         self.needtune[self.i] = False
+        self.last_tunerx = tunerx
+        self.last_tunery = tunery
 
     def set_tuning_setter(self, settuningi):
         if not callable(settuningi):
             raise ValueError("not callable")
         self.settuningi = settuningi
         self.viewport.set_tuning_setter(self._set_tuning)  # force retune
         return self
@@ -729,31 +749,31 @@
             self.viewport.onmotion(datax, datay)
 
         self.viewport.queue_draw()
 
     def _on_realize(self, widget):
         if self.sourceid is not None:
             return
-        self.sourceid = glib.timeout_add(int(self.cadence * 1000), self._do_cycle)
+        self.sourceid = GLib.timeout_add(int(self.cadence * 1000), self._do_cycle)
 
     def _on_unrealize(self, widget):
         if self.sourceid is None:
             return
-        glib.source_remove(self.sourceid)
+        GLib.source_remove(self.sourceid)
         self.sourceid = None
 
     def _do_cycle(self):
         if self.cycle_tbutton.get_active():
             self.set_current(self.i + 1)
         return True
 
     def _on_key_press(self, widget, event):
-        kn = gtk.gdk.keyval_name(event.keyval)
-        modmask = gtk.accelerator_get_default_mod_mask()
-        isctrl = (event.state & modmask) == gtk.gdk.CONTROL_MASK
+        kn = Gdk.keyval_name(event.keyval)
+        modmask = Gtk.accelerator_get_default_mod_mask()
+        isctrl = (event.state & modmask) == Gdk.ModifierType.CONTROL_MASK
 
         if kn == "j" and isctrl:
             self.set_current(self.i - 1)
             return True
 
         if kn == "k" and isctrl:
             self.set_current(self.i + 1)
@@ -763,19 +783,65 @@
             self.cycle_tbutton.set_active(not self.cycle_tbutton.get_active())
             return True
 
         return super(Cycler, self)._on_key_press(widget, event)
 
 
 def cycle(
-    arrays, descs=None, cadence=0.6, toworlds=None, drawoverlay=None, yflip=False
+    arrays,
+    descs=None,
+    cadence=0.6,
+    toworlds=None,
+    drawoverlay=None,
+    yflip=False,
+    tostatuses=None,
+    run_main=True,
+    save_after_viewing=None,
 ):
+    """Interactively display a series of 2D data arrays.
+
+    arrays
+      An iterable of 2D arrays (a 3D array works).
+    descs
+      An iterable of text descriptions, one for each array
+    cadence
+      The time delay before the next array is shown, in seconds.
+    tostatuses
+      An iterable of functions that convert cursor positions to a textual
+      status output corresponding to that position. FIXME details needed.
+    toworlds
+      An iterable of functions that convert cursor positions to a
+      latitude/longitude pair that is displayed in the status output.
+      The `tostatuses` keyword is a more generic version of this.
+      FIXME details needed.
+    drawoverlay
+      An optional function that draws an overlay on the display after
+      the underlying data image is presented. FIXME details needed.
+    yflip
+      If true, have the numerical *y* coordinates have 0 refer to the
+      bottom of the image. Note that the data array is still drawn such
+      that its first row appears at the top!
+    run_main
+      If true, run the Gtk mainloop explicitly so that the function does
+      not return until the window is closed. If false, no mainloop is run.
+      If the application happens to already be running a mainloop in the
+      background, the window will appear and the user will be able to
+      interact with it while this thread continues executing.
+    save_after_viewing
+      If set to a string containing an integer percent-formatting specifier,
+      the data will be written to a series of PNG files after the window is
+      closed.
+
+    """
     n = len(arrays)
     amin = amax = h = w = None
 
+    if toworlds is not None and tostatuses is not None:
+        raise ValueError('only one of "toworlds" and "tostatuses" may be given')
+
     if descs is None:
         descs = [""] * n
 
     for array in arrays:
         thish, thisw = array.shape
         thismin, thismax = array.min(), array.max()
 
@@ -823,64 +889,82 @@
 
     def getshapei(i):
         return w, h
 
     def getdesci(i):
         return descs[i]
 
-    clipped = np.zeros((h, w), dtype=np.int32)  # scratch array
+    clipped = np.zeros((h, w), dtype=np.int32)  # scratch arrays -- two needed
+    clipped2 = np.zeros((h, w), dtype=np.uint32)  # to make numpy ufunc casting happy
 
     def settuningi(i, tunerx, tunery):
         np.bitwise_and(imgdata[i], 0xFF000000, imgdata[i])
 
         fmin = int(0x0FFFFFF0 * tunerx)
         fmax = int(0x0FFFFFF0 * tunery)
 
         if fmin == fmax:
-            np.add(imgdata[i], 255 * (fixed[i] > fmin), imgdata[i])
+            np.add(imgdata[i], 255 * (fixed[i] > fmin).astype(np.uint32), imgdata[i])
         else:
             np.clip(fixed[i], fmin, fmax, clipped)
             np.subtract(clipped, fmin, clipped)
-            np.multiply(clipped, 255.0 / (fmax - fmin), clipped)
-            np.add(imgdata[i], clipped, imgdata[i])
+            np.multiply(clipped, 255.0 / (fmax - fmin), clipped2, casting="unsafe")
+            np.add(imgdata[i], clipped2, imgdata[i])
 
         np.multiply(imgdata[i], antimask[i], imgdata[i])
 
     def getsurfacei(i, xoffset, yoffset, width, height):
         return surfaces[i], xoffset, yoffset
 
     # see comment in view()
     nomasks = [not np.ma.is_masked(a) or a.mask is np.ma.nomask for a in arrays]
 
-    if toworlds is None:
-        toworlds = [None] * n
+    if tostatuses is None:
+        if toworlds is None:
+            tostatuses = [None] * n
+        else:
+            from .astutil import fmthours, fmtdeglat
+
+            def make_status_func(toworld):
+                def status(y_and_x):
+                    lat, lon = toworld(y_and_x)
+                    return "lat=%s lon=%s" % (fmtdeglat(lat), fmthours(lon))
 
-    from .astutil import fmthours, fmtdeglat
+            tostatuses = [make_status_func(toworlds[i]) for i in range(n)]
 
     def fmtstatusi(i, x, y):
         s = ""
         row = int(np.floor(y + 0.5))
         col = int(np.floor(x + 0.5))
         if row >= 0 and col >= 0 and row < h and col < w:
             if nomasks[i] or not arrays[i].mask[row, col]:
                 s += "%g " % arrays[i][row, col]
         if yflip:
             y = h - 1 - y
             row = h - 1 - row
         s += "[%d,%d] x=%.1f y=%.1f" % (row, col, x, y)
-        if toworlds[i] is not None:
-            lat, lon = toworlds[i]([y, x])
-            s += " lat=%s lon=%s" % (fmtdeglat(lat), fmthours(lon))
+        if tostatuses[i] is not None:
+            s += " " + tostatuses[i](np.array([y, x]))
         return s
 
     cycler = Cycler()
     cycler.set_n_getter(getn)
     cycler.set_shape_getter(getshapei)
     cycler.set_desc_getter(getdesci)
     cycler.set_tuning_setter(settuningi)
     cycler.set_surface_getter(getsurfacei)
     cycler.set_status_formatter(fmtstatusi)
     cycler.set_overlay_drawer(drawoverlay)
     cycler.win.show_all()
-    cycler.win.connect("destroy", gtk.main_quit)
 
-    gtk.main()
+    if run_main:
+        cycler.win.connect("destroy", Gtk.main_quit)
+        Gtk.main()
+    else:
+        cycler.win.connect("destroy", lambda e: cycler.win.destroy())
+
+    if save_after_viewing is not None:
+        for i in range(n):
+            filename = save_after_viewing % (i,)
+            settuningi(i, cycler.last_tunerx, cycler.last_tunery)
+            surface, xoffset, yoffset = getsurfacei(i, 0, 0, w, h)
+            surface.write_to_png(filename)
```

### Comparing `pwkit-1.1.1/pwkit/ninja_syntax.py` & `pwkit-1.2.0/pwkit/ninja_syntax.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/numutil.py` & `pwkit-1.2.0/pwkit/numutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 __all__ = """broadcastize dfsmooth fits_recarray_to_data_frame make_step_lcont
            make_step_rcont make_tophat_ee make_tophat_ei make_tophat_ie
            make_tophat_ii parallel_newton parallel_quad rms unit_tophat_ee
            unit_tophat_ei unit_tophat_ie unit_tophat_ii usmooth weighted_mean
            weighted_mean_df weighted_variance""".split()
 
 import functools
-from six.moves import range
 import numpy as np
 
 from .method_decorator import method_decorator
 
 
 def _broadcastize_spec_to_scalar_filter(s):
     if s is None:
@@ -153,29 +152,26 @@
     :meth:`astropy.table.table.Table.from_pandas`. It converts a Pandas
     :class:`pandas.DataFrame` object to an Astropy
     :class:`astropy.table.Table`.
 
     """
     from astropy.utils import OrderedDict
     from astropy.table import Table, Column, MaskedColumn
-    from astropy.extern import six
 
     out = OrderedDict()
 
     for name in dataframe.columns:
         column = dataframe[name]
         mask = np.array(column.isnull())
         data = np.array(column)
 
         if data.dtype.kind == "O":
             # If all elements of an object array are string-like or np.nan
             # then coerce back to a native numpy str/unicode array.
-            string_types = six.string_types
-            if six.PY3:
-                string_types += (bytes,)
+            string_types = (str, bytes)
             nan = np.nan
             if all(isinstance(x, string_types) or x is nan for x in data):
                 # Force any missing (null) values to b''.  Numpy will
                 # upcast to str/unicode as needed.
                 data[mask] = b""
 
                 # When the numpy object array is represented as a list then
```

### Comparing `pwkit-1.1.1/pwkit/parallel.py` & `pwkit-1.2.0/pwkit/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,21 +42,19 @@
 instances support a "partially-Pickling" `map`-like function
 :meth:`ParallelHelper.get_ppmap` that works around Pickle-related limitations
 in the :mod:`multiprocessing` library.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str('make_parallel_helper').split()
+__all__ = str("make_parallel_helper").split()
 
 import functools, signal
 from multiprocessing.pool import Pool
 from multiprocessing import Process, Queue, TimeoutError
-import six
-from six.moves import range
 
 
 def _initializer_wrapper(actual_initializer, *rest):
     """We ignore SIGINT. It's up to our parent to kill us in the typical condition
     of this arising from ``^C`` on a terminal. If someone is manually killing
     us with that signal, well... nothing will happen.
 
@@ -92,21 +90,22 @@
 
     - `<https://github.com/jreese/multiprocessing-keyboardinterrupt/>`_
 
     This version is a drop-in replacement for multiprocessing.Pool ... as long
     as the map() method is the only one that needs to be interrupt-friendly.
 
     """
+
     wait_timeout = 3600
 
     def __init__(self, processes=None, initializer=None, initargs=(), **kwargs):
         new_initializer = functools.partial(_initializer_wrapper, initializer)
-        super(InterruptiblePool, self).__init__(processes, new_initializer,
-                                                initargs, **kwargs)
-
+        super(InterruptiblePool, self).__init__(
+            processes, new_initializer, initargs, **kwargs
+        )
 
     def map(self, func, iterable, chunksize=None):
         """Equivalent of `map` built-in, without swallowing KeyboardInterrupt.
 
         func
           The function to apply to the items.
         iterable
@@ -154,29 +153,30 @@
     useless in production code. The "partially-Pickling map" works around this
     by using a different method that allows some arguments to the map
     operation to avoid being pickled. (Instead, they are directly inherited by
     :func:`os.fork`-ed subprocesses.) See the docs for :func:`serial_ppmap` for
     usage information.
 
     """
+
     def get_map(self):
         """Get a *context manager* that yields a function with the same call signature
         as the standard library function :func:`map`. Its results are the
         same, but it may evaluate the mapped function in parallel across
         multiple threads or processes --- the calling function should not have
         to particularly care about the details. Example usage is::
 
             with phelp.get_map() as map:
                 results_arr = map(my_function, my_args)
 
         The passed function and its arguments must be Pickle-able. The alternate
         method :meth:`get_ppmap` relaxes this restriction somewhat.
 
         """
-        raise NotImplementedError('get_map() not available')
+        raise NotImplementedError("get_map() not available")
 
     def get_ppmap(self):
         """Get a *context manager* that yields a "partially-pickling map function". It
         can be used to perform a parallelized :func:`map` operation with some
         un-pickle-able arguments.
 
         The yielded function has the signature of :func:`serial_ppmap`. Its
@@ -208,26 +208,29 @@
           ``ppmap``.
 
         This variant of the standard :func:`map` function exists to allow the
         parallel-processing system to work around :mod:`pickle`-related
         limitations in the :mod:`multiprocessing` library.
 
         """
-        raise NotImplementedError('get_ppmap() not available')
+        raise NotImplementedError("get_ppmap() not available")
 
 
 class VacuousContextManager(object):
     """A context manager that just returns a static value and doesn't do anything
     clever with exceptions.
 
     """
+
     def __init__(self, value):
         self.value = value
+
     def __enter__(self):
         return self.value
+
     def __exit__(self, etype, evalue, etb):
         return False
 
 
 def serial_ppmap(func, fixed_arg, var_arg_iter):
     """A serial implementation of the "partially-pickling map" function returned
     by the :meth:`ParallelHelper.get_ppmap` interface. Its arguments are:
@@ -291,69 +294,74 @@
 class MultiprocessingPoolHelper(ParallelHelper):
     """A :class:`ParallelHelper` that parallelizes computations using Python's
     :class:`multiprocessing.Pool` with a configurable number of processes.
     Actually, we use a wrapped version of :class:`multiprocessing.Pool` that
     handles :exc:`KeyboardInterrupt` exceptions more helpfully.
 
     """
+
     class InterruptiblePoolContextManager(object):
         def __init__(self, methodname, methodkwargs={}, **kwargs):
             self.methodname = methodname
             self.methodkwargs = methodkwargs
             self.kwargs = kwargs
 
         def __enter__(self):
             from functools import partial
+
             self.pool = InterruptiblePool(**self.kwargs)
             func = getattr(self.pool, self.methodname)
             return partial(func, **self.methodkwargs)
 
         def __exit__(self, etype, evalue, etb):
             self.pool.terminate()
             self.pool.join()
             return False
 
-
     def __init__(self, chunksize=None, **pool_kwargs):
         self.chunksize = chunksize
         self.pool_kwargs = pool_kwargs
 
     def get_map(self):
-        return self.InterruptiblePoolContextManager('map',
-                                                    {'chunksize': self.chunksize},
-                                                    **self.pool_kwargs)
-
+        return self.InterruptiblePoolContextManager(
+            "map", {"chunksize": self.chunksize}, **self.pool_kwargs
+        )
 
     def _ppmap(self, func, fixed_arg, var_arg_iter):
         """The multiprocessing implementation of the partially-Pickling "ppmap"
         function. This doesn't use a Pool like map() does, because the whole
         problem is that Pool chokes on un-Pickle-able values. Strongly derived
         from code posted on StackExchange by "klaus se":
         `<http://stackoverflow.com/a/16071616/3760486>`_.
 
         This implementation could definitely be improved -- that's basically
         what the Pool class is all about -- but this gets us off the ground
         for those cases where the Pickle limitation is important.
 
         XXX This deadlocks if a child process crashes!!! XXX
         """
-        n_procs = self.pool_kwargs.get('processes')
+        n_procs = self.pool_kwargs.get("processes")
         if n_procs is None:
             # Logic copied from multiprocessing.pool.Pool.__init__()
             try:
                 from multiprocessing import cpu_count
+
                 n_procs = cpu_count()
             except NotImplementedError:
                 n_procs = 1
 
         in_queue = Queue(1)
         out_queue = Queue()
-        procs = [Process(target=multiprocessing_ppmap_worker,
-                         args=(in_queue, out_queue, func, fixed_arg))
-                 for _ in range(n_procs)]
+        procs = [
+            Process(
+                target=multiprocessing_ppmap_worker,
+                args=(in_queue, out_queue, func, fixed_arg),
+            )
+            for _ in range(n_procs)
+        ]
 
         for p in procs:
             p.daemon = True
             p.start()
 
         i = -1
 
@@ -429,26 +437,28 @@
     be worked around somewhat with the special
     :meth:`ParallelHelper.get_ppmap` variant. This returns a
     "partially-Pickling" map operation --- with a different calling signature
     --- that allows un-Pickle-able values to be used. See the documentation
     for :func:`serial_ppmap` for usage information.
 
     """
-    if parallel_arg is True: # note: (True == 1) is True
+    if parallel_arg is True:  # note: (True == 1) is True
         return MultiprocessingPoolHelper(**kwargs)
 
     if parallel_arg is False or parallel_arg == 1:
         return SerialHelper(**kwargs)
 
     if parallel_arg > 0 and parallel_arg < 1:
         from multiprocessing import cpu_count
+
         n = int(round(parallel_arg * cpu_count()))
         return MultiprocessingPoolHelper(processes=n, **kwargs)
 
     if isinstance(parallel_arg, ParallelHelper):
         return parallel_arg
 
-    if isinstance(parallel_arg, six.integer_types):
+    if isinstance(parallel_arg, int):
         return MultiprocessingPoolHelper(processes=parallel_arg, **kwargs)
 
-    raise ValueError('don\'t understand make_parallel_helper() argument %r'
-                     % parallel_arg)
+    raise ValueError(
+        "don't understand make_parallel_helper() argument %r" % parallel_arg
+    )
```

### Comparing `pwkit-1.1.1/pwkit/pdm.py` & `pwkit-1.2.0/pwkit/pdm.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,55 +16,57 @@
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 # TODO: automatic rule for nbin?
 # TODO: ditto for nr periods to try?
 # TODO: confidence in peak value or something
 
-__all__ = str ('PDMResult pdm').split ()
+__all__ = str("PDMResult pdm").split()
 
 import numpy as np
 from collections import namedtuple
-from six.moves import range
 
 from .numutil import weighted_variance
 from .parallel import make_parallel_helper
 
-PDMResult = namedtuple ('PDMResult', 'thetas imin pmin mc_tmins '
-                        'mc_pvalue mc_pmins mc_puncert'.split ())
+PDMResult = namedtuple(
+    "PDMResult", "thetas imin pmin mc_tmins " "mc_pvalue mc_pmins mc_puncert".split()
+)
 
 
-def one_theta (t, x, wt, period, nbin, nshift, v_all):
+def one_theta(t, x, wt, period, nbin, nshift, v_all):
     phase0 = t / period
-    numer = denom = 0.
+    numer = denom = 0.0
 
-    for i in range (nshift):
-        phase = (phase0 + float (i) / (nshift * nbin)) % 1.
-        binloc = np.floor (phase * nbin).astype (int)
+    for i in range(nshift):
+        phase = (phase0 + float(i) / (nshift * nbin)) % 1.0
+        binloc = np.floor(phase * nbin).astype(int)
 
-        for j in range (nbin):
-            wh = np.where (binloc == j)[0]
+        for j in range(nbin):
+            wh = np.where(binloc == j)[0]
             if wh.size < 3:
                 continue
 
-            numer += weighted_variance (x[wh], wt[wh]) * (wh.size - 1)
+            numer += weighted_variance(x[wh], wt[wh]) * (wh.size - 1)
             denom += wh.size - 1
 
     return numer / (denom * v_all)
 
 
-def _map_one_theta (args):
+def _map_one_theta(args):
     """Needed for the parallel map() call in pdm() due to the gross way in which
     Python multiprocessing works.
 
     """
-    return one_theta (*args)
+    return one_theta(*args)
 
 
-def pdm (t, x, u, periods, nbin, nshift=8, nsmc=256, numc=256, weights=False, parallel=True):
+def pdm(
+    t, x, u, periods, nbin, nshift=8, nsmc=256, numc=256, weights=False, parallel=True
+):
     """Perform phase dispersion minimization.
 
     t : 1D array
       time coordinate
     x : 1D array, same size as *t*
       observed value
     u : 1D array, same size as *t*
@@ -109,94 +111,101 @@
       standard deviation of `mc_pmins`; approximate uncertainty
       on `pmin`.
 
     We don't do anything clever, so runtime scales at least as
     ``t.size * periods.size * nbin * nshift * (nsmc + numc + 1)``.
 
     """
-    t = np.asfarray (t)
-    x = np.asfarray (x)
-    u = np.asfarray (u)
-    periods = np.asfarray (periods)
-    t, x, u, periods = np.atleast_1d (t, x, u, periods)
-    nbin = int (nbin)
-    nshift = int (nshift)
-    nsmc = int (nsmc)
-    numc = int (numc)
-    phelp = make_parallel_helper (parallel)
+    t = np.asfarray(t)
+    x = np.asfarray(x)
+    u = np.asfarray(u)
+    periods = np.asfarray(periods)
+    t, x, u, periods = np.atleast_1d(t, x, u, periods)
+    nbin = int(nbin)
+    nshift = int(nshift)
+    nsmc = int(nsmc)
+    numc = int(numc)
+    phelp = make_parallel_helper(parallel)
 
     if t.ndim != 1:
-        raise ValueError ('`t` must be <= 1D')
+        raise ValueError("`t` must be <= 1D")
 
     if x.shape != t.shape:
-        raise ValueError ('`t` and `x` arguments must be the same size')
+        raise ValueError("`t` and `x` arguments must be the same size")
 
     if u.shape != t.shape:
-        raise ValueError ('`t` and `u` arguments must be the same size')
+        raise ValueError("`t` and `u` arguments must be the same size")
 
     if periods.ndim != 1:
-        raise ValueError ('`periods` must be <= 1D')
+        raise ValueError("`periods` must be <= 1D")
 
     if nbin < 2:
-        raise ValueError ('`nbin` must be at least 2')
+        raise ValueError("`nbin` must be at least 2")
 
     if nshift < 1:
-        raise ValueError ('`nshift` must be at least 1')
+        raise ValueError("`nshift` must be at least 1")
 
     if nsmc < 0:
-        raise ValueError ('`nsmc` must be nonnegative')
+        raise ValueError("`nsmc` must be nonnegative")
 
     if numc < 0:
-        raise ValueError ('`numc` must be nonnegative')
+        raise ValueError("`numc` must be nonnegative")
 
     # We can finally get started!
 
     if weights:
         wt = u
-        u = wt ** -0.5
+        u = wt**-0.5
     else:
-        wt = u ** -2
+        wt = u**-2
 
-    v_all = weighted_variance (x, wt)
+    v_all = weighted_variance(x, wt)
 
-    with phelp.get_map () as map:
-        get_thetas = lambda args: np.asarray (map (_map_one_theta, args))
-        thetas = get_thetas ((t, x, wt, p, nbin, nshift, v_all)
-                             for p in periods)
-        imin = thetas.argmin ()
+    with phelp.get_map() as map:
+        get_thetas = lambda args: np.asarray(map(_map_one_theta, args))
+        thetas = get_thetas((t, x, wt, p, nbin, nshift, v_all) for p in periods)
+        imin = thetas.argmin()
         pmin = periods[imin]
 
         # Now do the Monte Carlo jacknifing so that the caller can have some idea
         # as to the significance of the minimal value of `thetas`.
 
-        mc_thetas = np.empty (periods.shape)
-        mc_tmins = np.empty (nsmc)
+        mc_thetas = np.empty(periods.shape)
+        mc_tmins = np.empty(nsmc)
 
-        for i in range (nsmc):
-            shuf = np.random.permutation (x.size)
+        for i in range(nsmc):
+            shuf = np.random.permutation(x.size)
             # Note that what we do here is very MapReduce-y. I'm not aware of
             # an easy way to implement this computation in that model, though.
-            mc_thetas = get_thetas ((t, x[shuf], wt[shuf], p, nbin, nshift, v_all)
-                                    for p in periods)
-            mc_tmins[i] = mc_thetas.min ()
+            mc_thetas = get_thetas(
+                (t, x[shuf], wt[shuf], p, nbin, nshift, v_all) for p in periods
+            )
+            mc_tmins[i] = mc_thetas.min()
 
-        mc_tmins.sort ()
-        mc_pvalue = mc_tmins.searchsorted (thetas[imin]) / nsmc
+        mc_tmins.sort()
+        mc_pvalue = mc_tmins.searchsorted(thetas[imin]) / nsmc
 
         # Now add noise to assess the uncertainty of the period.
 
-        mc_pmins = np.empty (numc)
+        mc_pmins = np.empty(numc)
 
-        for i in range (numc):
-            noised = np.random.normal (x, u)
-            mc_thetas = get_thetas ((t, noised, wt, p, nbin, nshift, v_all)
-                                    for p in periods)
-            mc_pmins[i] = periods[mc_thetas.argmin ()]
+        for i in range(numc):
+            noised = np.random.normal(x, u)
+            mc_thetas = get_thetas(
+                (t, noised, wt, p, nbin, nshift, v_all) for p in periods
+            )
+            mc_pmins[i] = periods[mc_thetas.argmin()]
 
-        mc_pmins.sort ()
-        mc_puncert = mc_pmins.std ()
+        mc_pmins.sort()
+        mc_puncert = mc_pmins.std()
 
     # All done.
 
-    return PDMResult (thetas=thetas, imin=imin, pmin=pmin, mc_tmins=mc_tmins,
-                      mc_pvalue=mc_pvalue, mc_pmins=mc_pmins,
-                      mc_puncert=mc_puncert)
+    return PDMResult(
+        thetas=thetas,
+        imin=imin,
+        pmin=pmin,
+        mc_tmins=mc_tmins,
+        mc_pvalue=mc_pvalue,
+        mc_pmins=mc_pmins,
+        mc_puncert=mc_puncert,
+    )
```

### Comparing `pwkit-1.1.1/pwkit/phoenix.py` & `pwkit-1.2.0/pwkit/phoenix.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/radio_cal_models.py` & `pwkit-1.2.0/pwkit/radio_cal_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,225 +25,253 @@
   activates "flux" mode, where a three-item string is
   printed that can be passed to MIRIAD tasks that accept a
   model flux and spectral index argument.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('cas_a commandline init_cas_a models spindexes').split ()
+__all__ = str("cas_a commandline init_cas_a models spindexes").split()
 
 
-import six
 import numpy as np
 
 from . import PKError
 
 models = {}
 spindexes = {}
 
 
-def cas_a (freq_mhz, year):
+def cas_a(freq_mhz, year):
     """Return the flux of Cas A given a frequency and the year of observation.
     Based on the formula given in Baars et al., 1977.
 
     Parameters:
 
     freq - Observation frequency in MHz.
     year - Year of observation. May be floating-point.
 
     Returns: s, flux in Jy.
 
     """
     # The snu rule is right out of Baars et al. The dnu is corrected
     # for the frequency being measured in MHz, not GHz.
 
-    snu = 10. ** (5.745 - 0.770 * np.log10 (freq_mhz)) # Jy
-    dnu = 0.01 * (0.07 - 0.30 * np.log10 (freq_mhz)) # percent per yr.
-    loss = (1 - dnu) ** (year - 1980.)
+    snu = 10.0 ** (5.745 - 0.770 * np.log10(freq_mhz))  # Jy
+    dnu = 0.01 * (0.07 - 0.30 * np.log10(freq_mhz))  # percent per yr.
+    loss = (1 - dnu) ** (year - 1980.0)
     return snu * loss
 
 
-def init_cas_a (year):
+def init_cas_a(year):
     """Insert an entry for Cas A into the table of models. Need to specify the
     year of the observations to account for the time variation of Cas A's
     emission.
 
     """
-    year = float (year)
-    models['CasA'] = lambda f: cas_a (f, year)
+    year = float(year)
+    models["CasA"] = lambda f: cas_a(f, year)
 
 
 # Other models from Baars et al. 1977 -- data from Table 5 in that paper. Some
 # of these will be overwritten by VLA models below.
 
-def _add_generic_baars (src, a, b, c, fmin, fmax):
-    def fluxdens (freq_mhz):
-        if np.any (freq_mhz < fmin) or np.any (freq_mhz > fmax):
-            raise PKError ('going beyond frequency limits of model: want '
-                           '%f, but validity is [%f, %f]', freq_mhz, fmin, fmax)
-        lf = np.log10 (freq_mhz)
-        return 10.**(a + b * lf + c * lf**2)
-
-    def spindex (freq_mhz):
-        if np.any (freq_mhz < fmin) or np.any (freq_mhz > fmax):
-            raise PKError ('going beyond frequency limits of model: want '
-                           '%f, but validity is [%f, %f]', freq_mhz, fmin, fmax)
-        return b + 2 * c * np.log10 (freq_mhz)
+
+def _add_generic_baars(src, a, b, c, fmin, fmax):
+    def fluxdens(freq_mhz):
+        if np.any(freq_mhz < fmin) or np.any(freq_mhz > fmax):
+            raise PKError(
+                "going beyond frequency limits of model: want "
+                "%f, but validity is [%f, %f]",
+                freq_mhz,
+                fmin,
+                fmax,
+            )
+        lf = np.log10(freq_mhz)
+        return 10.0 ** (a + b * lf + c * lf**2)
+
+    def spindex(freq_mhz):
+        if np.any(freq_mhz < fmin) or np.any(freq_mhz > fmax):
+            raise PKError(
+                "going beyond frequency limits of model: want "
+                "%f, but validity is [%f, %f]",
+                freq_mhz,
+                fmin,
+                fmax,
+            )
+        return b + 2 * c * np.log10(freq_mhz)
 
     models[src] = fluxdens
     spindexes[src] = spindex
 
 
 baars_parameters = {
-    '3c48': (2.345, 0.071, -0.138, 405., 15000.),
-    '3c123': (2.921, -0.002, -0.124, 405., 15000.),
-    '3c147': (1.766, 0.447, -0.184, 405., 15000.),
-    '3c161': (1.633, 0.498, -0.194, 405., 10700.),
-    '3c218': (4.497, -0.910, 0.0, 405., 10700.),
-    '3c227': (3.460, -0.827, 0.0, 405, 15000.),
-    '3c249.1': (1.230, 0.288, -0.176, 405., 15000.),
-    '3c286': (1.480, 0.292, -0.124, 405., 15000.),
-    '3c295': (1.485, 0.759, -0.255, 405., 15000.),
-    '3c348': (4.963, -1.052, 0., 405., 10700.),
-    '3c353': (2.944, -0.034, -0.109, 405., 10700.),
-    'DR21': (1.81, -0.122, 0., 7000., 31000.),
-    'NGC7027': (1.32, -0.127, 0., 10000., 31000.)
+    "3c48": (2.345, 0.071, -0.138, 405.0, 15000.0),
+    "3c123": (2.921, -0.002, -0.124, 405.0, 15000.0),
+    "3c147": (1.766, 0.447, -0.184, 405.0, 15000.0),
+    "3c161": (1.633, 0.498, -0.194, 405.0, 10700.0),
+    "3c218": (4.497, -0.910, 0.0, 405.0, 10700.0),
+    "3c227": (3.460, -0.827, 0.0, 405, 15000.0),
+    "3c249.1": (1.230, 0.288, -0.176, 405.0, 15000.0),
+    "3c286": (1.480, 0.292, -0.124, 405.0, 15000.0),
+    "3c295": (1.485, 0.759, -0.255, 405.0, 15000.0),
+    "3c348": (4.963, -1.052, 0.0, 405.0, 10700.0),
+    "3c353": (2.944, -0.034, -0.109, 405.0, 10700.0),
+    "DR21": (1.81, -0.122, 0.0, 7000.0, 31000.0),
+    "NGC7027": (1.32, -0.127, 0.0, 10000.0, 31000.0),
 }
 
-def _init_generic_baars ():
-    for src, info in six.iteritems (baars_parameters):
-        _add_generic_baars (src, *info)
 
-_init_generic_baars ()
+def _init_generic_baars():
+    for src, info in baars_parameters.items():
+        _add_generic_baars(src, *info)
+
+
+_init_generic_baars()
 
 
 # VLA models of calibrators: see
 # http://www.vla.nrao.edu/astro/calib/manual/baars.html These are the 1999.2
 # values. This makes them pretty out of date, but still a lot more recent than
 # Baars.
 
-def _add_vla_model (src, a, b, c, d):
-    def fluxdens (freq_mhz):
-        if np.any (freq_mhz < 300) or np.any (freq_mhz > 50000):
-            raise PKError ('going beyond frequency limits of model: want '
-                           '%f, but validity is [300, 50000]', freq_mhz)
-        lghz = np.log10 (freq_mhz) - 3
-        return 10.**(a + b * lghz + c * lghz**2 + d * lghz**3)
-
-    def spindex (freq_mhz):
-        if np.any (freq_mhz < 300) or np.any (freq_mhz > 50000):
-            raise PKError ('going beyond frequency limits of model: want '
-                           '%f, but validity is [300, 50000]', freq_mhz)
-        lghz = np.log10 (freq_mhz) - 3
+
+def _add_vla_model(src, a, b, c, d):
+    def fluxdens(freq_mhz):
+        if np.any(freq_mhz < 300) or np.any(freq_mhz > 50000):
+            raise PKError(
+                "going beyond frequency limits of model: want "
+                "%f, but validity is [300, 50000]",
+                freq_mhz,
+            )
+        lghz = np.log10(freq_mhz) - 3
+        return 10.0 ** (a + b * lghz + c * lghz**2 + d * lghz**3)
+
+    def spindex(freq_mhz):
+        if np.any(freq_mhz < 300) or np.any(freq_mhz > 50000):
+            raise PKError(
+                "going beyond frequency limits of model: want "
+                "%f, but validity is [300, 50000]",
+                freq_mhz,
+            )
+        lghz = np.log10(freq_mhz) - 3
         return b + 2 * c * lghz + 3 * d * lghz**2
 
     models[src] = fluxdens
     spindexes[src] = spindex
 
 
 vla_parameters = {
-    '3c48': (1.31752, -0.74090, -0.16708, +0.01525),
-    '3c138': (1.00761, -0.55629, -0.11134, -0.01460),
-    '3c147': (1.44856, -0.67252, -0.21124, +0.04077),
-    '3c286': (1.23734, -0.43276, -0.14223, +0.00345),
-    '3c295': (1.46744, -0.77350, -0.25912, +0.00752)
+    "3c48": (1.31752, -0.74090, -0.16708, +0.01525),
+    "3c138": (1.00761, -0.55629, -0.11134, -0.01460),
+    "3c147": (1.44856, -0.67252, -0.21124, +0.04077),
+    "3c286": (1.23734, -0.43276, -0.14223, +0.00345),
+    "3c295": (1.46744, -0.77350, -0.25912, +0.00752),
 }
 
-def _init_vla ():
-    for src, info in six.iteritems (vla_parameters):
-        _add_vla_model (src, *info)
 
-_init_vla ()
+def _init_vla():
+    for src, info in vla_parameters.items():
+        _add_vla_model(src, *info)
+
+
+_init_vla()
 
 
 # Crappier power-law modeling based on VLA Calibrator Manual catalog. It is
 # not clear whether values in the catalog should be taken to supersede those
 # given in the analytic models above, for those five sources that have
 # analytic models. The catalog entries do not seem to necessarily be more
 # recent than the analytic models.
 
-def add_from_vla_obs (src, Lband, Cband):
+
+def add_from_vla_obs(src, Lband, Cband):
     """Add an entry into the models table for a source based on L-band and
     C-band flux densities.
 
     """
     if src in models:
-        raise PKError ('already have a model for ' + src)
+        raise PKError("already have a model for " + src)
 
-    fL = np.log10 (1425)
-    fC = np.log10 (4860)
+    fL = np.log10(1425)
+    fC = np.log10(4860)
 
-    lL = np.log10 (Lband)
-    lC = np.log10 (Cband)
+    lL = np.log10(Lband)
+    lC = np.log10(Cband)
 
     A = (lL - lC) / (fL - fC)
     B = lL - A * fL
 
-    def fluxdens (freq_mhz):
-        return 10. ** (A * np.log10 (freq_mhz) + B)
+    def fluxdens(freq_mhz):
+        return 10.0 ** (A * np.log10(freq_mhz) + B)
 
-    def spindex (freq_mhz):
+    def spindex(freq_mhz):
         return A
 
     models[src] = fluxdens
     spindexes[src] = spindex
 
 
-add_from_vla_obs ('3c84', 23.9, 23.3)
+add_from_vla_obs("3c84", 23.9, 23.3)
 
 
 # If we're executed as a program, print out a flux given a source name.
 
-def commandline (argv):
+
+def commandline(argv):
     from . import cli
 
-    cli.unicode_stdio ()
-    cli.check_usage (__doc__, argv, usageifnoargs='long')
-    flux_mode = cli.pop_option ('f', argv)
+    cli.unicode_stdio()
+    cli.check_usage(__doc__, argv, usageifnoargs="long")
+    flux_mode = cli.pop_option("f", argv)
     source = argv[1]
 
-    if source == 'CasA':
-        if len (argv) != 4:
-            cli.wrong_usage (__doc__, 'must give exactly three arguments '
-                             'when modeling Cas A')
+    if source == "CasA":
+        if len(argv) != 4:
+            cli.wrong_usage(
+                __doc__, "must give exactly three arguments " "when modeling Cas A"
+            )
 
         try:
-            init_cas_a (float (argv[3]))
+            init_cas_a(float(argv[3]))
         except Exception as e:
-            cli.die ('unable to parse year "%s": %s', argv[3], e)
-    elif len (argv) != 3:
-        cli.wrong_usage (__doc__, 'must give exactly two arguments unless '
-                         'modeling Cas A')
+            cli.die('unable to parse year "%s": %s', argv[3], e)
+    elif len(argv) != 3:
+        cli.wrong_usage(
+            __doc__, "must give exactly two arguments unless " "modeling Cas A"
+        )
 
     try:
-        freq = float (argv[2])
+        freq = float(argv[2])
     except Exception as e:
-        cli.die ('unable to parse frequency "%s": %s', argv[2], e)
+        cli.die('unable to parse frequency "%s": %s', argv[2], e)
 
     if source not in models:
-        cli.die ('unknown source "%s"; known sources are: CasA, %s', source,
-                 ', '.join (sorted (models.keys ())))
+        cli.die(
+            'unknown source "%s"; known sources are: CasA, %s',
+            source,
+            ", ".join(sorted(models.keys())),
+        )
 
     try:
-        flux = models[source] (freq)
+        flux = models[source](freq)
     except Exception as e:
         # Catch, e.g, going beyond frequency limits.
-        cli.die ('error finding flux of %s at %f MHz: %s', source, freq, e)
+        cli.die("error finding flux of %s at %f MHz: %s", source, freq, e)
 
     if not flux_mode:
-        print ('%g' % (flux, ))
+        print("%g" % (flux,))
         return 0
 
     try:
-        spindex = spindexes[source] (freq)
+        spindex = spindexes[source](freq)
     except Exception as e:
-        cli.warn ('error finding spectral index of %s at %f MHz: %s',
-                  source, freq, e)
+        cli.warn("error finding spectral index of %s at %f MHz: %s", source, freq, e)
         spindex = 0
 
-    print ('%g,%g,%g' % (flux, freq * 1e-3, spindex))
+    print("%g,%g,%g" % (flux, freq * 1e-3, spindex))
     return 0
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from sys import argv, exit
-    exit (commandline (argv))
+
+    exit(commandline(argv))
```

### Comparing `pwkit-1.1.1/pwkit/sherpa.py` & `pwkit-1.2.0/pwkit/sherpa.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/simpleenum.py` & `pwkit-1.2.0/pwkit/simpleenum.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit/slurp.py` & `pwkit-1.2.0/pwkit/slurp.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 # Copyright 2015 Peter Williams <peter@newton.cx> and collaborators
 # Licensed under the MIT License.
 
 """pwkit.slurp - run a program and capture its output."""
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('Event Redirection Slurper').split ()
+__all__ = str("Event Redirection Slurper").split()
 
-import fcntl, os, signal, six, subprocess, sys
+import fcntl, os, signal, subprocess
 from select import select, error as selecterror
 
 from . import Holder
 
 try:
-    from subprocss import DEVNULL as _DEVNULL
+    from subprocess import DEVNULL as _DEVNULL
 except ImportError:
     _DEVNULL = subprocess.STDOUT - 1
 
+
 @Holder
-class Event (object):
-    Stdout = 'stdout'
-    Stderr = 'stderr'
-    ForwardedSignal = 'forwarded-signal'
-    Timeout = 'timeout'
+class Event(object):
+    Stdout = "stdout"
+    Stderr = "stderr"
+    ForwardedSignal = "forwarded-signal"
+    Timeout = "timeout"
 
 
 @Holder
-class Redirection (object):
+class Redirection(object):
     Pipe = subprocess.PIPE
     Stdout = subprocess.STDOUT
     DevNull = _DEVNULL
 
 
 signals_for_child = [
     signal.SIGHUP,
@@ -39,80 +40,92 @@
     signal.SIGQUIT,
     signal.SIGTERM,
     signal.SIGUSR1,
     signal.SIGUSR2,
 ]
 
 
-class SlurperIterator (object):
-    def __init__ (self, parent):
+class SlurperIterator(object):
+    def __init__(self, parent):
         self.parent = parent
 
-    def __iter__ (self):
+    def __iter__(self):
         return self
 
-    def __next__ (self): # Python 3
-        if not len (self.parent._files):
-            raise StopIteration ()
-        return self.parent._next_lowlevel ()
+    def __next__(self):  # Python 3
+        if not len(self.parent._files):
+            raise StopIteration()
+        return self.parent._next_lowlevel()
 
-    next = __next__ # Python 2
+    next = __next__  # Python 2
 
 
-def _decode_streams (event_source, which_events, encoding):
+def _decode_streams(event_source, which_events, encoding):
     from codecs import getincrementaldecoder
+
     decoders = {}
 
     for etype, edata in event_source:
         if etype not in which_events:
             yield etype, edata
             continue
 
-        dec = decoders.get (etype)
+        dec = decoders.get(etype)
         if dec is None:
-            dec = decoders[etype] = getincrementaldecoder (encoding) ()
+            dec = decoders[etype] = getincrementaldecoder(encoding)()
 
-        final = not len (edata)
-        result = dec.decode (edata, final)
-        if len (result):
-            yield etype, result # no false EOF indicators
+        final = not len(edata)
+        result = dec.decode(edata, final)
+        if len(result):
+            yield etype, result  # no false EOF indicators
 
         if final:
-            yield etype, edata # make sure we have an EOF signal
+            yield etype, edata  # make sure we have an EOF signal
 
 
-def _linebreak_streams (event_source, which_events):
+def _linebreak_streams(event_source, which_events):
     partials = {}
 
     for etype, edata in event_source:
         if etype not in which_events:
             yield etype, edata
             continue
 
-        if not len (edata):
+        if not len(edata):
             # EOF on this stream.
-            trailer = partials.get (etype, edata)
-            if len (trailer):
+            trailer = partials.get(etype, edata)
+            if len(trailer):
                 yield etype, trailer
             yield etype, edata
             continue
 
-        lines = (partials.get (etype, edata * 0) + edata).split (edata.__class__ (b'\n'))
+        lines = (partials.get(etype, edata * 0) + edata).split(edata.__class__(b"\n"))
         for line in lines[:-1]:
             yield etype, line
         partials[etype] = lines[-1]
 
 
-class Slurper (object):
+class Slurper(object):
     _chunksize = 1024
 
-    def __init__ (self, argv=None, env=None, cwd=None, propagate_signals=True,
-                  timeout=10, linebreak=False, encoding=None,
-                  stdin=Redirection.DevNull, stdout=Redirection.Pipe,
-                  stderr=Redirection.Pipe, executable=None, subproc_factory=None):
+    def __init__(
+        self,
+        argv=None,
+        env=None,
+        cwd=None,
+        propagate_signals=True,
+        timeout=10,
+        linebreak=False,
+        encoding=None,
+        stdin=Redirection.DevNull,
+        stdout=Redirection.Pipe,
+        stderr=Redirection.Pipe,
+        executable=None,
+        subproc_factory=None,
+    ):
         if subproc_factory is None:
             subproc_factory = subprocess.Popen
 
         self.subproc_factory = subproc_factory
         self.proc = None
         self.argv = argv
         self.env = env
@@ -122,105 +135,102 @@
         self.linebreak = linebreak
         self.encoding = encoding
         self.stdin = stdin
         self.stdout = stdout
         self.stderr = stderr
         self.executable = executable
 
-
-    def __enter__ (self):
+    def __enter__(self):
         self._prev_handlers = {}
         self._other_events = []
         self._file_event_types = {}
         self._files = []
 
         stdin = self.stdin
         if stdin == Redirection.DevNull:
-            stdin = open (os.devnull, 'r')
+            stdin = open(os.devnull, "r")
 
         stdout = self.stdout
         if stdout == Redirection.DevNull:
-            stdout = open (os.devnull, 'w')
+            stdout = open(os.devnull, "w")
 
         stderr = self.stderr
         if stderr == Redirection.DevNull:
-            stderr = open (os.devnull, 'w')
+            stderr = open(os.devnull, "w")
 
-        self.proc = self.subproc_factory (
+        self.proc = self.subproc_factory(
             self.argv,
             env=self.env,
             executable=self.executable,
             cwd=self.cwd,
             stdin=stdin,
             stdout=stdout,
             stderr=stderr,
             shell=False,
         )
 
         if self.propagate_signals:
-            def handle (signum, frame):
-                self.proc.send_signal (signum)
-                self._other_events.insert (0, (Event.ForwardedSignal, signum))
+
+            def handle(signum, frame):
+                self.proc.send_signal(signum)
+                self._other_events.insert(0, (Event.ForwardedSignal, signum))
 
             for signum in signals_for_child:
-                self._prev_handlers[signum] = signal.signal (signum, handle)
+                self._prev_handlers[signum] = signal.signal(signum, handle)
 
         if stdout == Redirection.Pipe:
-            self._file_event_types[self.proc.stdout.fileno ()] = Event.Stdout
-            self._files.append (self.proc.stdout)
+            self._file_event_types[self.proc.stdout.fileno()] = Event.Stdout
+            self._files.append(self.proc.stdout)
 
         if stderr == Redirection.Pipe:
-            self._file_event_types[self.proc.stderr.fileno ()] = Event.Stderr
-            self._files.append (self.proc.stderr)
+            self._file_event_types[self.proc.stderr.fileno()] = Event.Stderr
+            self._files.append(self.proc.stderr)
 
         for fd in self._files:
-            fl = fcntl.fcntl (fd.fileno (), fcntl.F_GETFL)
-            fcntl.fcntl (fd.fileno (), fcntl.F_SETFL, fl | os.O_NONBLOCK)
+            fl = fcntl.fcntl(fd.fileno(), fcntl.F_GETFL)
+            fcntl.fcntl(fd.fileno(), fcntl.F_SETFL, fl | os.O_NONBLOCK)
 
         return self
 
-
-    def _next_lowlevel (self):
-        if len (self._other_events):
-            return self._other_events.pop ()
+    def _next_lowlevel(self):
+        if len(self._other_events):
+            return self._other_events.pop()
 
         while True:
             try:
-                rd, wr, er = select (self._files, [], [], self.timeout)
+                rd, wr, er = select(self._files, [], [], self.timeout)
                 break
             except selecterror as e:
                 # if EINTR or EAGAIN, try again; we won't get EINTR unless
                 # we're forwarding signals, since otherwise it'll show up as a
                 # KeyboardInterrupt. "e.args[0]" is the only way to get errno.
                 if e.args[0] not in (4, 11):
                     raise
 
         for fd in rd:
-            chunk = fd.read (self._chunksize)
-            if not len (chunk):
-                self._files.remove (fd)
-            return (self._file_event_types[fd.fileno ()], chunk)
+            chunk = fd.read(self._chunksize)
+            if not len(chunk):
+                self._files.remove(fd)
+            return (self._file_event_types[fd.fileno()], chunk)
 
         return (Event.Timeout, None)
 
-
-    def __iter__ (self):
-        result = SlurperIterator (self)
+    def __iter__(self):
+        result = SlurperIterator(self)
 
         if self.encoding is not None:
-            which = frozenset ((Event.Stdout, Event.Stderr))
-            result = _decode_streams (result, which, self.encoding)
+            which = frozenset((Event.Stdout, Event.Stderr))
+            result = _decode_streams(result, which, self.encoding)
 
         if self.linebreak:
-            which = frozenset ((Event.Stdout, Event.Stderr))
-            result = _linebreak_streams (result, which)
+            which = frozenset((Event.Stdout, Event.Stderr))
+            result = _linebreak_streams(result, which)
 
         return result
 
+    def __exit__(self, etype, evalue, etb):
+        self.proc.wait()
 
-    def __exit__ (self, etype, evalue, etb):
-        self.proc.wait ()
-
-        for signum, prev_handler in six.iteritems (self._prev_handlers):
-            signal.signal (signum, prev_handler)
+        for signum, prev_handler in self._prev_handlers.items():
+            signal.signal(signum, prev_handler)
 
         return False
```

### Comparing `pwkit-1.1.1/pwkit/synphot.py` & `pwkit-1.2.0/pwkit/synphot.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,18 +511,16 @@
 
 
 def get_std_registry():
     """Get a Registry object pre-filled with information for standard
     telescopes.
 
     """
-    from six import itervalues
-
     reg = Registry()
-    for fn in itervalues(builtin_registrars):
+    for fn in builtin_registrars.values():
         fn(reg)
     return reg
 
 
 # Now, builtin information for a variety of telescopes. Document these
 # aggressively! I have these in alphabetical order. 2MASS is first.
```

### Comparing `pwkit-1.1.1/pwkit/tabfile.py` & `pwkit-1.2.0/pwkit/tabfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,39 +14,38 @@
 of the form "colname = value" set a column name that gets the same value for
 every item in the table. The header line is prefixed with an @ sign.
 Subsequent lines are data rows.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('read vizread write').split ()
+__all__ = str("read vizread write").split()
 
-import six
 from . import Holder, PKError, io, msmt, reraise_context
 
 
-def _getparser (lname):
-    a = lname.rsplit (':', 1)
-    if len (a) == 1:
-        a.append ('s')
+def _getparser(lname):
+    a = lname.rsplit(":", 1)
+    if len(a) == 1:
+        a.append("s")
     return a[0], msmt.parsers[a[1]]
 
 
-def _trimmedlines (path, **kwargs):
-    for line in io.pathlines (path, **kwargs):
-        line = line[:-1] # trailing newline
-        line = line.split ('#', 1)[0]
-        if not len (line):
+def _trimmedlines(path, **kwargs):
+    for line in io.pathlines(path, **kwargs):
+        line = line[:-1]  # trailing newline
+        line = line.split("#", 1)[0]
+        if not len(line):
             continue
-        if line.isspace ():
+        if line.isspace():
             continue
         yield line
 
 
-def read (path, tabwidth=8, **kwargs):
+def read(path, tabwidth=8, **kwargs):
     """Read a typed tabular text file into a stream of Holders.
 
     Arguments:
 
     path
       The path of the file to read.
     tabwidth=8
@@ -61,87 +60,87 @@
     Returns a generator for a stream of `pwkit.Holder`s, each of which will
     contain ints, strings, or some kind of measurement (cf `pwkit.msmt`).
 
     """
     datamode = False
     fixedcols = {}
 
-    for text in _trimmedlines (path, **kwargs):
-        text = text.expandtabs (tabwidth)
+    for text in _trimmedlines(path, **kwargs):
+        text = text.expandtabs(tabwidth)
 
         if datamode:
             # table row
-            h = Holder ()
-            h.set (**fixedcols)
+            h = Holder()
+            h.set(**fixedcols)
             for name, cslice, parser in info:
                 try:
-                    v = parser (text[cslice].strip ())
+                    v = parser(text[cslice].strip())
                 except:
-                    reraise_context ('while parsing "%s"', text[cslice].strip ())
-                h.set_one (name, v)
+                    reraise_context('while parsing "%s"', text[cslice].strip())
+                h.set_one(name, v)
             yield h
-        elif text[0] != '@':
+        elif text[0] != "@":
             # fixed column
-            padnamekind, padval = text.split ('=', 1)
-            name, parser = _getparser (padnamekind.strip ())
-            fixedcols[name] = parser (padval.strip ())
+            padnamekind, padval = text.split("=", 1)
+            name, parser = _getparser(padnamekind.strip())
+            fixedcols[name] = parser(padval.strip())
         else:
             # column specification
-            n = len (text)
+            n = len(text)
             assert n > 1
             start = 0
             info = []
 
             while start < n:
                 end = start + 1
-                while end < n and (not text[end].isspace ()):
+                while end < n and (not text[end].isspace()):
                     end += 1
 
                 if start == 0:
-                    namekind = text[start+1:end] # eat leading @
+                    namekind = text[start + 1 : end]  # eat leading @
                 else:
                     namekind = text[start:end]
 
-                while end < n and text[end].isspace ():
+                while end < n and text[end].isspace():
                     end += 1
 
-                name, parser = _getparser (namekind)
-                if parser is None: # allow columns to be ignored
+                name, parser = _getparser(namekind)
+                if parser is None:  # allow columns to be ignored
                     skippedlast = True
                 else:
                     skippedlast = False
-                    info.append ((name, slice (start, end), parser))
+                    info.append((name, slice(start, end), parser))
                 start = end
 
             datamode = True
 
             if not skippedlast:
                 # make our last column go as long as the line goes
                 # (e.g. for "comments" columns)
                 # but if the real last column is ":x"-type, then info[-1]
                 # doesn't run up to the end of the line, so do nothing in that case.
                 lname, lslice, lparser = info[-1]
-                info[-1] = lname, slice (lslice.start, None), lparser
+                info[-1] = lname, slice(lslice.start, None), lparser
 
 
-def _tabpad (text, width, tabwidth=8):
+def _tabpad(text, width, tabwidth=8):
     # note: assumes we're starting tab-aligned
-    l = len (text)
+    l = len(text)
     assert l <= width
 
     if l == width:
         return text
 
     n = width - l
     ntab = n // tabwidth
     nsp = n - ntab * tabwidth
-    return ''.join ((text, ' ' * nsp, '\t' * ntab))
+    return "".join((text, " " * nsp, "\t" * ntab))
 
 
-def write (stream, items, fieldnames, tabwidth=8):
+def write(stream, items, fieldnames, tabwidth=8):
     """Write a typed tabular text file to the specified stream.
 
     Arguments:
 
     stream
       The destination stream.
     items
@@ -153,85 +152,94 @@
       If the latter, it will be split into a list with .split().
     tabwidth=8
       The tab width to use. Please don't monkey with it.
 
     Returns nothing.
 
     """
-    if isinstance (fieldnames, six.string_types):
-        fieldnames = fieldnames.split ()
+    if isinstance(fieldnames, str):
+        fieldnames = fieldnames.split()
 
-    maxlens = [0] * len (fieldnames)
+    maxlens = [0] * len(fieldnames)
 
     # We have to make two passes, so listify:
-    items = list (items)
+    items = list(items)
 
     # pass 1: get types and maximum lengths for each record. Pad by 1 to
     # ensure there's at least one space between all columns.
 
-    coltypes = [None] * len (fieldnames)
+    coltypes = [None] * len(fieldnames)
 
     for i in items:
-        for idx, fn in enumerate (fieldnames):
-            val = i.get (fn)
+        for idx, fn in enumerate(fieldnames):
+            val = i.get(fn)
             if val is None:
                 continue
 
-            typetag, text, inexact = msmt.fmtinfo (val)
-            maxlens[idx] = max (maxlens[idx], len (text) + 1)
+            typetag, text, inexact = msmt.fmtinfo(val)
+            maxlens[idx] = max(maxlens[idx], len(text) + 1)
 
             if coltypes[idx] is None:
                 coltypes[idx] = typetag
                 continue
 
             if coltypes[idx] == typetag:
                 continue
 
-            if coltypes[idx][-1] == 'f' and typetag[-1] == 'u':
+            if coltypes[idx][-1] == "f" and typetag[-1] == "u":
                 # Can upcast floats to uvals
                 if coltypes[idx][:-1] == typetag[:-1]:
-                    coltypes[idx] = coltypes[idx][:-1] + 'u'
+                    coltypes[idx] = coltypes[idx][:-1] + "u"
                     continue
 
-            if coltypes[idx][-1] == 'u' and typetag[-1] == 'f':
+            if coltypes[idx][-1] == "u" and typetag[-1] == "f":
                 if coltypes[idx][:-1] == typetag[:-1]:
                     continue
 
-            raise PKError ('irreconcilable column types: %s and %s', coltypes[idx], typetag)
+            raise PKError(
+                "irreconcilable column types: %s and %s", coltypes[idx], typetag
+            )
 
     # Compute column headers and their widths
 
-    headers = list (fieldnames)
-    headers[0] = '@' + headers[0]
+    headers = list(fieldnames)
+    headers[0] = "@" + headers[0]
 
-    for idx, fn in enumerate (fieldnames):
-        if coltypes[idx] != '':
-            headers[idx] += ':' + coltypes[idx]
+    for idx, fn in enumerate(fieldnames):
+        if coltypes[idx] != "":
+            headers[idx] += ":" + coltypes[idx]
 
-        maxlens[idx] = max (maxlens[idx], len (headers[idx]))
+        maxlens[idx] = max(maxlens[idx], len(headers[idx]))
 
     widths = [tabwidth * ((k + tabwidth - 1) // tabwidth) for k in maxlens]
 
     # pass 2: write out
 
-    print (''.join (_tabpad (h, widths[idx], tabwidth)
-                    for (idx, h) in enumerate (headers)), file=stream)
+    print(
+        "".join(_tabpad(h, widths[idx], tabwidth) for (idx, h) in enumerate(headers)),
+        file=stream,
+    )
 
-    def ustr (i, f):
-        v = i.get (f)
+    def ustr(i, f):
+        v = i.get(f)
         if v is None:
-            return ''
-        return msmt.fmtinfo (v)[1]
+            return ""
+        return msmt.fmtinfo(v)[1]
 
     for i in items:
-        print (''.join (_tabpad (ustr (i, fn), widths[idx], tabwidth)
-                        for (idx, fn) in enumerate (fieldnames)), file=stream)
+        print(
+            "".join(
+                _tabpad(ustr(i, fn), widths[idx], tabwidth)
+                for (idx, fn) in enumerate(fieldnames)
+            ),
+            file=stream,
+        )
 
 
-def vizread (descpath, descsection, tabpath, tabwidth=8, **kwargs):
+def vizread(descpath, descsection, tabpath, tabwidth=8, **kwargs):
     """Read a headerless tabular text file into a stream of Holders.
 
     Arguments:
 
     descpath
       The path of the table description ini file.
     descsection
@@ -257,41 +265,41 @@
     b, i, f, u, Lu, Pu).
 
     """
     from .inifile import read as iniread
 
     cols = []
 
-    for i in iniread (descpath):
+    for i in iniread(descpath):
         if i.section != descsection:
             continue
 
-        for field, desc in six.iteritems (i.__dict__):
-            if field == 'section':
+        for field, desc in i.__dict__.items():
+            if field == "section":
                 continue
 
-            a = desc.split ()
-            idx0 = int (a[0]) - 1
+            a = desc.split()
+            idx0 = int(a[0]) - 1
 
-            if len (a) == 1:
-                cols.append ((field, slice (idx0, idx0 + 1), msmt.parsers['s']))
+            if len(a) == 1:
+                cols.append((field, slice(idx0, idx0 + 1), msmt.parsers["s"]))
                 continue
 
-            if len (a) == 2:
-                parser = msmt.parsers['s']
+            if len(a) == 2:
+                parser = msmt.parsers["s"]
             else:
                 parser = msmt.parsers[a[2]]
 
-            cols.append ((field, slice (idx0, int (a[1])), parser))
+            cols.append((field, slice(idx0, int(a[1])), parser))
 
-    for text in _trimmedlines (tabpath, **kwargs):
-        text = text.expandtabs (tabwidth)
+    for text in _trimmedlines(tabpath, **kwargs):
+        text = text.expandtabs(tabwidth)
 
-        h = Holder ()
+        h = Holder()
         for name, cslice, parser in cols:
             try:
-                v = parser (text[cslice].strip ())
+                v = parser(text[cslice].strip())
             except:
-                reraise_context ('while parsing "%s"', text[cslice].strip ())
-            h.set_one (name, v)
+                reraise_context('while parsing "%s"', text[cslice].strip())
+            h.set_one(name, v)
 
         yield h
```

### Comparing `pwkit-1.1.1/pwkit/tinifile.py` & `pwkit-1.2.0/pwkit/tinifile.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,123 +14,130 @@
   Lower-level version; only operates on streams, not path names.
 write_stream
   Lower-level version; only operates on streams, not path names.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('read_stream read write_stream write').split ()
-
-import six
+__all__ = str("read_stream read write_stream write").split()
 
 from . import Holder, inifile, msmt
 
 
-def _parse_one (old):
+def _parse_one(old):
     new = {}
 
-    for name, value in six.iteritems (old.__dict__):
-        if name == 'section':
+    for name, value in old.__dict__.items():
+        if name == "section":
             new[name] = value
             continue
 
-        a = name.rsplit (':', 1)
-        if len (a) == 1:
-            a.append ('s')
+        a = name.rsplit(":", 1)
+        if len(a) == 1:
+            a.append("s")
         shname, typetag = a
-        new[shname] = msmt.parsers[typetag] (value)
+        new[shname] = msmt.parsers[typetag](value)
 
-    return Holder (**new)
+    return Holder(**new)
 
 
-def read_stream (stream, **kwargs):
-    for unparsed in inifile.read_stream (stream, **kwargs):
-        yield _parse_one (unparsed)
+def read_stream(stream, **kwargs):
+    for unparsed in inifile.read_stream(stream, **kwargs):
+        yield _parse_one(unparsed)
 
 
-def read (stream_or_path, **kwargs):
-    for unparsed in inifile.read (stream_or_path, **kwargs):
-        yield _parse_one (unparsed)
+def read(stream_or_path, **kwargs):
+    for unparsed in inifile.read(stream_or_path, **kwargs):
+        yield _parse_one(unparsed)
 
 
-def _format_many (holders, defaultsection, extrapos, digest):
+def _format_many(holders, defaultsection, extrapos, digest):
     # We need to handle defaultsection here, and not just leave it to inifile,
     # so that we can get consistent digest computation.
 
     for old in holders:
-        s = old.get ('section', defaultsection)
+        s = old.get("section", defaultsection)
         if s is None:
-            raise ValueError ('cannot determine section name for item <%s>' % old)
-        new = {'section': s}
+            raise ValueError("cannot determine section name for item <%s>" % old)
+        new = {"section": s}
 
         if digest is not None:
-            digest.update ('s')
-            digest.update (s)
+            digest.update("s")
+            digest.update(s)
 
-        for name in sorted (x for x in six.iterkeys (old.__dict__) if x != 'section'):
-            value = old.get (name)
+        for name in sorted(x for x in old.__dict__.keys() if x != "section"):
+            value = old.get(name)
             if value is None:
                 continue
 
-            typetag, ftext, is_imprecise = msmt.fmtinfo (value)
+            typetag, ftext, is_imprecise = msmt.fmtinfo(value)
             lname = name
-            if len (typetag):
-                if is_imprecise and name in extrapos and typetag in ('u', 'f'):
-                    typetag = 'P' + typetag
-                lname += ':' + typetag
-            itext = ' # imprecise' if is_imprecise else ''
+            if len(typetag):
+                if is_imprecise and name in extrapos and typetag in ("u", "f"):
+                    typetag = "P" + typetag
+                lname += ":" + typetag
+            itext = " # imprecise" if is_imprecise else ""
             new[lname] = ftext + itext
 
             if digest is not None:
-                digest.update ('k')
-                digest.update (name)
-                digest.update (typetag)
-                digest.update ('v')
+                digest.update("k")
+                digest.update(name)
+                digest.update(typetag)
+                digest.update("v")
                 if is_imprecise:
-                    digest.update ('<impreciseval>')
+                    digest.update("<impreciseval>")
                 else:
-                    digest.update (ftext)
+                    digest.update(ftext)
 
-        yield Holder (**new)
+        yield Holder(**new)
 
 
-def write_stream (stream, holders, defaultsection=None, extrapos=(), sha1sum=False, **kwargs):
+def write_stream(
+    stream, holders, defaultsection=None, extrapos=(), sha1sum=False, **kwargs
+):
     """`extrapos` is basically a hack for multi-step processing. We have some flux
     measurements that are computed from luminosities and distances. The flux
     value is therefore an unwrapped Uval, which doesn't retain memory of any
     positivity constraint it may have had. Therefore, if we write out such a
     value using this routine, we may get something like `fx:u = 1pm1`, and the
     next time it's read in we'll get negative fluxes. Fields listed in
     `extrapos` will have a "P" constraint added if they are imprecise and
     their typetag is just "f" or "u".
 
     """
     if sha1sum:
         import hashlib
-        sha1 = hashlib.sha1 ()
+
+        sha1 = hashlib.sha1()
     else:
         sha1 = None
 
-    inifile.write_stream (stream,
-                          _format_many (holders, defaultsection, extrapos, sha1),
-                          defaultsection=defaultsection,
-                          **kwargs)
+    inifile.write_stream(
+        stream,
+        _format_many(holders, defaultsection, extrapos, sha1),
+        defaultsection=defaultsection,
+        **kwargs
+    )
 
     if sha1sum:
-        return sha1.digest ()
+        return sha1.digest()
 
 
-def write (stream_or_path, holders, defaultsection=None, extrapos=(),
-           sha1sum=False, **kwargs):
+def write(
+    stream_or_path, holders, defaultsection=None, extrapos=(), sha1sum=False, **kwargs
+):
     if sha1sum:
         import hashlib
-        sha1 = hashlib.sha1 ()
+
+        sha1 = hashlib.sha1()
     else:
         sha1 = None
 
-    inifile.write (stream_or_path,
-                   _format_many (holders, defaultsection, extrapos, sha1),
-                   defaultsection=defaultsection,
-                   **kwargs)
+    inifile.write(
+        stream_or_path,
+        _format_many(holders, defaultsection, extrapos, sha1),
+        defaultsection=defaultsection,
+        **kwargs
+    )
 
     if sha1sum:
-        return sha1.digest ()
+        return sha1.digest()
```

### Comparing `pwkit-1.1.1/pwkit/ucd_physics.py` & `pwkit-1.2.0/pwkit/ucd_physics.py`

 * *Files identical despite different names*

### Comparing `pwkit-1.1.1/pwkit.egg-info/PKG-INFO` & `pwkit-1.2.0/pwkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwkit
-Version: 1.1.1
+Version: 1.2.0
 Summary: Miscellaneous scientific and astronomical tools
 Home-page: https://github.com/pkgw/pwkit/
 Author: Peter Williams
 Author-email: peter@newton.cx
 License: MIT
 Keywords: astronomy science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pwkit-1.1.1/pwkit.egg-info/SOURCES.txt` & `pwkit-1.2.0/pwkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 docs/source/io/pwkit-tabfile.rst
 docs/source/io/pwkit-tinifile.rst
 docs/source/io/pwkit-unicode_to_latex.rst
 docs/source/io/slurp.rst
 docs/source/pwkit/colormaps.rst
 docs/source/pwkit/contours.rst
 docs/source/pwkit/data_gui_helpers.rst
-docs/source/pwkit/ndshow_gtk2.rst
 docs/source/pwkit/ndshow_gtk3.rst
 docs/source/pwkit/cli/astrotool.rst
 docs/source/pwkit/cli/imtool.rst
 docs/source/pwkit/cli/latexdriver.rst
 docs/source/pwkit/cli/wrapout.rst
 docs/source/pwkit/environments/casa/scripting.rst
 docs/source/pwkit/environments/casa/spwglue.rst
@@ -105,15 +104,14 @@
 pwkit/kbn_conf.py
 pwkit/kwargv.py
 pwkit/latex.py
 pwkit/lmmin.py
 pwkit/lsqmdl.py
 pwkit/method_decorator.py
 pwkit/msmt.py
-pwkit/ndshow_gtk2.py
 pwkit/ndshow_gtk3.py
 pwkit/ninja_syntax.py
 pwkit/numutil.py
 pwkit/parallel.py
 pwkit/pdm.py
 pwkit/phoenix.py
 pwkit/radio_cal_models.py
```

### Comparing `pwkit-1.1.1/setup.py` & `pwkit-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 """
     )
     return "".join(lines)
 
 
 setup(
     name="pwkit",  # cranko project-name
-    version="1.1.1",  # cranko project-version
+    version="1.2.0",  # cranko project-version
     # This package actually *is* zip-safe, but I've run into issues with
     # installing it as a Zip: in particular, the install sometimes fails with
     # "bad local file header", and reloading a module after a reinstall in
     # IPython gives an ImportError with the same message. These are annoying
     # enough and I don't really care so we just install it as flat files.
     zip_safe=False,
     packages=[
@@ -59,15 +59,14 @@
     # We want to go easy on the requires; some modules are going to require
     # more stuff, but others don't need much of anything. But, it's pretty
     # much impossible to do science without Numpy. We may actually require
     # version 1.8 but for now I'll optimistically hope that we can get away
     # with 1.6.
     install_requires=[
         "numpy >= 1.6",
-        "six >= 1.9",
     ],
     extras_require={
         "docs": [
             "mock",
             "numpydoc",
             "sphinx",
             "sphinx_rtd_theme",
```


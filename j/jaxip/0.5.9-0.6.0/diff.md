# Comparing `tmp/jaxip-0.5.9.tar.gz` & `tmp/jaxip-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.5.9.tar", last modified: Wed May 17 19:33:14 2023, max compression
+gzip compressed data, was "jaxip-0.6.0.tar", last modified: Sun Jun 18 10:02:54 2023, max compression
```

## Comparing `jaxip-0.5.9.tar` & `jaxip-0.6.0.tar`

### file list

```diff
@@ -1,141 +1,147 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.069933 jaxip-0.5.9/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.9/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.9/CONTRIBUTING.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.9/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.9/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.9/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-05-17 19:33:14.069933 jaxip-0.5.9/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4745 2023-05-17 19:30:18.000000 jaxip-0.5.9/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.049933 jaxip-0.5.9/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.9/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.045933 jaxip-0.5.9/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.045933 jaxip-0.5.9/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.045933 jaxip-0.5.9/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.9/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.9/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.9/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.9/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6394 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.9/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       71 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.9/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.9/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.9/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.5.9/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.9/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      662 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.models.nn.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      941 2023-05-17 19:29:09.000000 jaxip-0.5.9/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.9/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-17 19:29:09.000000 jaxip-0.5.9/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.9/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.5.9/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.9/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.5.9/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.057933 jaxip-0.5.9/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/atoms/_box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/atoms/_neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3724 2023-05-09 21:10:18.000000 jaxip-0.5.9/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.9/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3015 2023-05-09 21:10:18.000000 jaxip-0.5.9/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    16813 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.057933 jaxip-0.5.9/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/datasets/dataset.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6445 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/datasets/runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1039 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/datasets/transformer.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.057933 jaxip-0.5.9/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.061933 jaxip-0.5.9/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.9/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.5.9/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7689 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/descriptor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.061933 jaxip-0.5.9/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.5.9/jaxip/models/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/models/model.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.065933 jaxip-0.5.9/jaxip/models/nn/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.5.9/jaxip/models/nn/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.5.9/jaxip/models/nn/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.5.9/jaxip/models/nn/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2911 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/models/nn/network.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.065933 jaxip-0.5.9/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1973 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1831 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/atomic_potential.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.065933 jaxip-0.5.9/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9155 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9364 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      545 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    18966 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11352 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3585 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/pytree.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.5.9/jaxip/types.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.9/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.065933 jaxip-0.5.9/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.9/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.9/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.9/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.057933 jaxip-0.5.9/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3091 2023-05-17 19:33:14.000000 jaxip-0.5.9/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-17 19:33:14.069933 jaxip-0.5.9/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.9/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.069933 jaxip-0.5.9/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.069933 jaxip-0.5.9/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.9/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.9/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.9/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.9/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.9/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.9/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.9/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-17 19:26:08.000000 jaxip-0.5.9/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-17 19:26:08.000000 jaxip-0.5.9/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-05-07 11:23:30.000000 jaxip-0.5.9/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4116 2023-05-08 16:51:03.000000 jaxip-0.5.9/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3472 2023-05-17 19:30:18.000000 jaxip-0.5.9/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.9/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.9/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.9/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-17 19:26:08.000000 jaxip-0.5.9/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-17 19:26:08.000000 jaxip-0.5.9/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.381492 jaxip-0.6.0/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.6.0/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.6.0/CONTRIBUTING.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      650 2023-06-18 10:02:01.000000 jaxip-0.6.0/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.6.0/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.6.0/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-06-18 10:02:54.381492 jaxip-0.6.0/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4745 2023-05-17 19:30:18.000000 jaxip-0.6.0/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.6.0/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.349491 jaxip-0.6.0/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.349491 jaxip-0.6.0/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-06-18 09:34:19.000000 jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:34:19.000000 jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:34:19.000000 jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.349491 jaxip-0.6.0/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-06-18 09:20:05.000000 jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:20:05.000000 jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-06-18 09:20:05.000000 jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.6.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.6.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.6.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.6.0/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-06-18 10:02:01.000000 jaxip-0.6.0/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.6.0/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       71 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.6.0/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.357491 jaxip-0.6.0/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.6.0/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.6.0/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.6.0/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.6.0/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      662 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-05-17 19:30:18.000000 jaxip-0.6.0/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-06-18 10:02:01.000000 jaxip-0.6.0/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      560 2023-06-18 10:02:01.000000 jaxip-0.6.0/docs/jaxip.simulation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-10 20:36:05.000000 jaxip-0.6.0/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.6.0/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-06-18 09:19:55.000000 jaxip-0.6.0/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.6.0/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.6.0/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.6.0/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.365491 jaxip-0.6.0/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.6.0/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.369491 jaxip-0.6.0/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/atoms/_box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/atoms/_neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3918 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3015 2023-05-09 21:10:18.000000 jaxip-0.6.0/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    17216 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.369491 jaxip-0.6.0/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/datasets/dataset.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6445 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/datasets/runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1039 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/datasets/transformer.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.6.0/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.6.0/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7689 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/descriptors/descriptor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.6.0/jaxip/models/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/models/model.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.6.0/jaxip/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.6.0/jaxip/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.6.0/jaxip/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2911 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.373491 jaxip-0.6.0/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1973 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1831 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.377491 jaxip-0.6.0/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9155 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9364 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      545 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    18966 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11352 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3585 2023-05-17 19:30:18.000000 jaxip-0.6.0/jaxip/pytree.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.377491 jaxip-0.6.0/jaxip/simulation/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      163 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/simulation/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     8913 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/simulation/md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      832 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/simulation/thermostat.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.6.0/jaxip/types.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.6.0/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.377491 jaxip-0.6.0/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.6.0/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.6.0/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.6.0/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.6.0/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.369491 jaxip-0.6.0/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3217 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-06-18 10:02:54.000000 jaxip-0.6.0/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-06-18 10:02:54.385491 jaxip-0.6.0/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.6.0/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.381492 jaxip-0.6.0/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-06-18 10:02:54.381492 jaxip-0.6.0/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.6.0/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.6.0/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.6.0/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.6.0/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.6.0/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.6.0/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.6.0/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-06-18 09:42:24.000000 jaxip-0.6.0/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-06-18 09:42:24.000000 jaxip-0.6.0/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-05-07 11:23:30.000000 jaxip-0.6.0/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4858 2023-06-18 10:02:01.000000 jaxip-0.6.0/tests/test_md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4116 2023-05-08 16:51:03.000000 jaxip-0.6.0/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3472 2023-05-17 19:30:18.000000 jaxip-0.6.0/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.6.0/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.6.0/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5463 2023-06-18 10:02:01.000000 jaxip-0.6.0/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-06-18 09:42:24.000000 jaxip-0.6.0/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-06-18 09:42:24.000000 jaxip-0.6.0/tests/weights.008.pkl
```

### Comparing `jaxip-0.5.9/CONTRIBUTING.rst` & `jaxip-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/HISTORY.rst` & `jaxip-0.6.0/HISTORY.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+0.6.0 (2023-06-18)
+-------------------
+* Add molecular dynamics (MD) simulator
+
+
 0.5.0 (2023-03-02)
 -------------------
 * Implemented Kalman filter trainer 
 
 
 0.4.0 (2023-01-03)
 -------------------
```

### Comparing `jaxip-0.5.9/LICENSE` & `jaxip-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/PKG-INFO` & `jaxip-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.5.9
+Version: 0.6.0
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `jaxip-0.5.9/README.rst` & `jaxip-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/Makefile` & `jaxip-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png` & `jaxip-0.6.0/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_38_0.png` & `jaxip-0.6.0/docs/_build/html/_images/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/conf.py` & `jaxip-0.6.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 # html_theme = "alabaster"
-html_theme = "sphinx_rtd_theme"  # "pydata_sphinx_theme"
+html_theme = "sphinx_rtd_theme"
+# html_theme = "pydata_sphinx_theme"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
     # "search_bar_position": "sidebar",
```

### Comparing `jaxip-0.5.9/docs/images/flowchart.drawio.png` & `jaxip-0.6.0/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/images/water.png` & `jaxip-0.6.0/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/installation.rst` & `jaxip-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/jaxip.atoms.rst` & `jaxip-0.6.0/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/jaxip.datasets.rst` & `jaxip-0.6.0/docs/jaxip.datasets.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.6.0/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/jaxip.descriptors.rst` & `jaxip-0.6.0/docs/jaxip.descriptors.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/jaxip.models.nn.rst` & `jaxip-0.6.0/docs/jaxip.models.nn.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/jaxip.potentials.nnp.rst` & `jaxip-0.6.0/docs/jaxip.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/jaxip.rst` & `jaxip-0.6.0/docs/jaxip.rst`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
    :maxdepth: 4
 
    jaxip.atoms
    jaxip.datasets
    jaxip.descriptors
    jaxip.models
    jaxip.potentials
+   jaxip.simulation
    jaxip.utils
 
 Submodules
 ----------
 
 jaxip.config module
 -------------------
```

### Comparing `jaxip-0.5.9/docs/jaxip.utils.rst` & `jaxip-0.6.0/docs/jaxip.utils.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/make.bat` & `jaxip-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/theory.rst` & `jaxip-0.6.0/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/docs/usage.rst` & `jaxip-0.6.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/__init__.py` & `jaxip-0.6.0/jaxip/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/atoms/_neighbor.py` & `jaxip-0.6.0/jaxip/atoms/_neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/atoms/_structure.py` & `jaxip-0.6.0/jaxip/atoms/_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/atoms/box.py` & `jaxip-0.6.0/jaxip/atoms/box.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,9 +115,16 @@
     @property
     def length(self) -> Optional[Array]:
         """Return length of cell in x, y, and z-directions."""
         if self.lattice is not None:
             return self.lattice.diagonal()
         return None
 
+    @property
+    def volume(self) -> Optional[Array]:
+        """Return volume of the box."""
+        if self.lattice is not None:
+            return jnp.prod(self.length)
+        return None
+
 
 register_jax_pytree_node(Box)
```

### Comparing `jaxip-0.5.9/jaxip/atoms/neighbor.py` & `jaxip-0.6.0/jaxip/atoms/neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/atoms/structure.py` & `jaxip-0.6.0/jaxip/atoms/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,16 @@
 
         # Extract atom info from the ASE atoms instance
         data = {
             "element": [
                 ElementMap.atomic_number_to_element(n)
                 for n in atoms.get_atomic_numbers()
             ],
-            "lattice": np.asarray(atoms.get_cell()),
-            "position": atoms.get_positions(),
+            "lattice": np.asarray(atoms.get_cell() * units.FROM_ANGSTROM),
+            "position": atoms.get_positions() * units.FROM_ANGSTROM,
         }
         for key, attr in zip(
             ("charge", "energy"),
             ("charges", "potential_energies"),
         ):
             try:
                 data[key] = getattr(atoms, f"get_{attr}")()
@@ -303,14 +303,25 @@
         return self.box.lattice
 
     @property
     def elements(self) -> tuple[Element, ...]:
         atom_type_host = jax.device_get(self.atom_type)
         return tuple(sorted({str(self.element_map(int(at))) for at in atom_type_host}))
 
+    @property
+    def mass(self) -> Array:
+        """Return an array of atomic masses."""
+        to_element = self.element_map.atom_type_to_element
+        elements = (to_element[int(at)] for at in self.atom_type)
+        return jnp.array(
+            tuple(
+                ElementMap.element_to_atomic_mass(element) for element in elements
+            )
+        )
+
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}"
             f"(natoms={self.natoms}, elements={self.elements}, dtype={self.dtype})"
         )
 
     def select(self, element: Element) -> Array:
@@ -381,17 +392,17 @@
         :return: ASE representation of the structure
         :rtype: AseAtoms
         """
         logger.info("Creating a representation of the structure in form of ASE atoms")
         return AseAtoms(
             symbols=[self.element_map(int(at)) for at in self.atom_type],
             positions=[
-                units.BOHR_TO_ANGSTROM * np.asarray(pos) for pos in self.position
+                units.TO_ANGSTROM * np.asarray(pos) for pos in self.position
             ],
-            cell=units.BOHR_TO_ANGSTROM * np.asarray(self.box.lattice)
+            cell=units.TO_ANGSTROM * np.asarray(self.box.lattice)
             if self.box
             else None,
             pbc=True if self.box else False,
             charges=[np.asarray(ch) for ch in self.charge],
         )
 
     # --------------------------------------------------------------------------------------
```

### Comparing `jaxip-0.5.9/jaxip/config.py` & `jaxip-0.6.0/jaxip/config.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/datasets/runner.py` & `jaxip-0.6.0/jaxip/datasets/runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/datasets/transformer.py` & `jaxip-0.6.0/jaxip/datasets/transformer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.6.0/jaxip/descriptors/acsf/_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.6.0/jaxip/descriptors/acsf/acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/descriptors/acsf/angular.py` & `jaxip-0.6.0/jaxip/descriptors/acsf/angular.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/descriptors/acsf/cutoff.py` & `jaxip-0.6.0/jaxip/descriptors/acsf/cutoff.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/descriptors/acsf/radial.py` & `jaxip-0.6.0/jaxip/descriptors/acsf/radial.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.6.0/jaxip/descriptors/acsf/symmetry.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/descriptors/descriptor.py` & `jaxip-0.6.0/jaxip/descriptors/descriptor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/descriptors/scaler.py` & `jaxip-0.6.0/jaxip/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/logger.py` & `jaxip-0.6.0/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/models/nn/activation.py` & `jaxip-0.6.0/jaxip/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/models/nn/initializer.py` & `jaxip-0.6.0/jaxip/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/models/nn/network.py` & `jaxip-0.6.0/jaxip/models/nn/network.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/_energy.py` & `jaxip-0.6.0/jaxip/potentials/_energy.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/_force.py` & `jaxip-0.6.0/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/atomic_potential.py` & `jaxip-0.6.0/jaxip/potentials/atomic_potential.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.6.0/jaxip/potentials/nnp/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.6.0/jaxip/potentials/nnp/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/nnp/metrics.py` & `jaxip-0.6.0/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/nnp/nnp.py` & `jaxip-0.6.0/jaxip/potentials/nnp/nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/nnp/potential.py` & `jaxip-0.6.0/jaxip/potentials/nnp/potential.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/potentials/nnp/settings.py` & `jaxip-0.6.0/jaxip/potentials/nnp/settings.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/pytree.py` & `jaxip-0.6.0/jaxip/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/types.py` & `jaxip-0.6.0/jaxip/types.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/utils/attribute.py` & `jaxip-0.6.0/jaxip/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/utils/batch.py` & `jaxip-0.6.0/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/utils/compare.py` & `jaxip-0.6.0/jaxip/utils/compare.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/utils/profiler.py` & `jaxip-0.6.0/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip/utils/tokenize.py` & `jaxip-0.6.0/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/jaxip.egg-info/PKG-INFO` & `jaxip-0.6.0/jaxip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.5.9
+Version: 0.6.0
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `jaxip-0.5.9/jaxip.egg-info/SOURCES.txt` & `jaxip-0.6.0/jaxip.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/jaxip.descriptors.acsf.rst
 docs/jaxip.descriptors.rst
 docs/jaxip.models.nn.rst
 docs/jaxip.models.rst
 docs/jaxip.potentials.nnp.rst
 docs/jaxip.potentials.rst
 docs/jaxip.rst
+docs/jaxip.simulation.rst
 docs/jaxip.utils.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/theory.rst
 docs/usage.rst
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
@@ -89,26 +90,30 @@
 jaxip/potentials/nnp/__init__.py
 jaxip/potentials/nnp/gradient_descent.py
 jaxip/potentials/nnp/kalman_filter.py
 jaxip/potentials/nnp/metrics.py
 jaxip/potentials/nnp/nnp.py
 jaxip/potentials/nnp/potential.py
 jaxip/potentials/nnp/settings.py
+jaxip/simulation/__init__.py
+jaxip/simulation/md.py
+jaxip/simulation/thermostat.py
 jaxip/utils/__init__.py
 jaxip/utils/attribute.py
 jaxip/utils/batch.py
 jaxip/utils/compare.py
 jaxip/utils/profiler.py
 jaxip/utils/tokenize.py
 tests/__init__.py
 tests/h2o.data
 tests/h2o.json
 tests/scaling.001.data
 tests/scaling.008.data
 tests/test_acsf.py
+tests/test_md.py
 tests/test_nn.py
 tests/test_nnp.py
 tests/test_runner.py
 tests/test_scaler.py
 tests/test_structure.py
 tests/weights.001.pkl
 tests/weights.008.pkl
```

### Comparing `jaxip-0.5.9/setup.py` & `jaxip-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.6.0/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.6.0/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.6.0/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.6.0/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/h2o.data` & `jaxip-0.6.0/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/h2o.json` & `jaxip-0.6.0/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/test_acsf.py` & `jaxip-0.6.0/tests/test_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/test_nn.py` & `jaxip-0.6.0/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/test_nnp.py` & `jaxip-0.6.0/tests/test_nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/test_runner.py` & `jaxip-0.6.0/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/test_scaler.py` & `jaxip-0.6.0/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/test_structure.py` & `jaxip-0.6.0/tests/test_structure.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         [11.4260918, 11.4260918, 11.4260918],
     ],
     "total_energy": [-0.21838404],
     "comment": ["r = 1.01000000E+00, E = -2.18384040E-01, dEdr = -1.97905715E+01"],
     "total_charge": [],
     "lattice": [],
     "atom_type": [1, 1],
+    "mass": [36785.88642640456] * 2,
 }
 
 H2O_DATA: Dict[str, Any] = {
     "lattice": [
         [11.8086403654, 0.0, 0.0],
         [0.0, 11.8086403654, 0.0],
         [0.0, 0.0, 11.8086403654],
@@ -87,20 +88,21 @@
         [-0.1172658121, -0.1885000212, -0.5958629059],
         [-0.1934543148, 0.5415107499, 0.4505828542],
         [0.0216973013, -0.0334599566, 0.508882732],
     ],
     "total_energy": [-32.1390027258],
     "total_charge": [8.0e-07],
     "atom_type": [2, 1, 1, 2, 1, 1, 2, 1, 1, 2, 1, 1],
+    "mass": [29164.39033379815, 1837.4714329938454, 1837.4714329938454] * 4,
 }
 
 
 class TestStructure:
     lj: Structure = Structure.create_from_dict(
-        LJ_DATA, dtype=jnp.float32
+        LJ_DATA, dtype=jnp.float32  # type: ignore
     )  # type: ignore
     h2o: Structure = Structure.create_from_dict(H2O_DATA, r_cutoff=11.0)
     atom_attributes: Tuple[str, ...] = tuple(
         ["position", "force", "energy", "total_energy", "charge", "total_charge"]
     )
 
     @pytest.mark.parametrize(
@@ -136,19 +138,33 @@
                 assert jnp.allclose(getattr(structure, attr), expected[i])
 
     @pytest.mark.parametrize(
         "structure, expected",
         [
             (
                 lj,
-                (2, ("Ne",), None, jnp.float32, None),
+                (
+                    2,
+                    ("Ne",),
+                    None,
+                    jnp.float32,
+                    None,
+                    jnp.asarray(LJ_DATA["mass"]),
+                ),
             ),
             (
                 h2o,
-                (12, ("H", "O"), 11.0, _dtype.FLOATX, jnp.asarray(H2O_DATA["lattice"])),
+                (
+                    12,
+                    ("H", "O"),
+                    11.0,
+                    _dtype.FLOATX,
+                    jnp.asarray(H2O_DATA["lattice"]),
+                    jnp.asarray(H2O_DATA["mass"]),
+                ),
             ),
         ],
     )
     def test_general_attributes(
         self,
         structure: Structure,
         expected: Tuple,
@@ -157,7 +173,8 @@
         assert structure.elements == expected[1]
         assert structure.r_cutoff == expected[2]
         assert structure.dtype == expected[3]
         if structure.lattice is None:
             assert structure.lattice is expected[4]
         else:
             assert jnp.allclose(structure.lattice, expected[4])
+        assert jnp.allclose(structure.mass, expected[5])
```

### Comparing `jaxip-0.5.9/tests/weights.001.pkl` & `jaxip-0.6.0/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.9/tests/weights.008.pkl` & `jaxip-0.6.0/tests/weights.008.pkl`

 * *Files identical despite different names*


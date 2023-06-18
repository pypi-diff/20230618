# Comparing `tmp/hgutilities-1.0.6.tar.gz` & `tmp/hgutilities-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.6.tar", last modified: Wed Jun 14 09:11:27 2023, max compression
+gzip compressed data, was "hgutilities-1.0.7.tar", last modified: Sun Jun 18 20:15:22 2023, max compression
```

## Comparing `hgutilities-1.0.6.tar` & `hgutilities-1.0.7.tar`

### file list

```diff
@@ -1,106 +1,201 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.709352 hgutilities-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.581107 hgutilities-1.0.6/.github/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.592109 hgutilities-1.0.6/.github/workflows/
--rw-rw-rw-   0        0        0     1123 2023-06-14 09:06:29.000000 hgutilities-1.0.6/.github/workflows/python-publish.yml
--rw-rw-rw-   0        0        0    35823 2023-06-14 09:06:29.000000 hgutilities-1.0.6/LICENSE.md
--rw-rw-rw-   0        0        0     7982 2023-06-14 09:11:27.709352 hgutilities-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     7224 2023-06-14 09:06:29.000000 hgutilities-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.593108 hgutilities-1.0.6/hgutilities/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.609334 hgutilities-1.0.6/hgutilities/Documentation/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/Documentation/__init__.py
--rw-rw-rw-   0        0        0     2505 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/Documentation/hgutilities.txt
--rw-rw-rw-   0        0        0      163 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.612334 hgutilities-1.0.6/hgutilities/defaults/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.623333 hgutilities-1.0.6/hgutilities/defaults/Documentation/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/__init__.py
--rw-rw-rw-   0        0        0      633 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/defaults.txt
--rw-rw-rw-   0        0        0      715 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/docs.txt
--rw-rw-rw-   0        0        0      361 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/inherit.txt
--rw-rw-rw-   0        0        0      625 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/loaddefaults.txt
--rw-rw-rw-   0        0        0      537 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/processkwargs.txt
--rw-rw-rw-   0        0        0      239 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/__init__.py
--rw-rw-rw-   0        0        0     2962 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/docs.py
--rw-rw-rw-   0        0        0      671 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/inherit.py
--rw-rw-rw-   0        0        0     1562 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/loaddefaults.py
--rw-rw-rw-   0        0        0     2571 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/processkwargs.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.630146 hgutilities-1.0.6/hgutilities/plotting/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.636146 hgutilities-1.0.6/hgutilities/plotting/Default Settings/
--rw-rw-rw-   0        0        0      193 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Default Settings/Animate.txt
--rw-rw-rw-   0        0        0      608 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Default Settings/Figure.txt
--rw-rw-rw-   0        0        0      330 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Default Settings/Figures.txt
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Default Settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.652907 hgutilities-1.0.6/hgutilities/plotting/Documentation/
--rw-rw-rw-   0        0        0      598 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/Animate.txt
--rw-rw-rw-   0        0        0      424 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/Figure.txt
--rw-rw-rw-   0        0        0      579 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/Figures.txt
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/__init__.py
--rw-rw-rw-   0        0        0      811 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/create_animations.txt
--rw-rw-rw-   0        0        0      628 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/create_figures.txt
--rw-rw-rw-   0        0        0     1180 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/plotting.txt
--rw-rw-rw-   0        0        0    11039 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/README.md
--rw-rw-rw-   0        0        0     1132 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/__init__.py
--rw-rw-rw-   0        0        0     2673 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/animate.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.655905 hgutilities-1.0.6/hgutilities/plotting/datatypes/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.674744 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/
--rw-rw-rw-   0        0        0      283 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Bar.txt
--rw-rw-rw-   0        0        0      183 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Bars.txt
--rw-rw-rw-   0        0        0      738 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
--rw-rw-rw-   0        0        0      441 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Data.txt
--rw-rw-rw-   0        0        0     1135 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Line.txt
--rw-rw-rw-   0        0        0      191 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Lines.txt
--rw-rw-rw-   0        0        0      355 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Pie.txt
--rw-rw-rw-   0        0        0      582 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Surface.txt
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.697356 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/
--rw-rw-rw-   0        0        0      677 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Bar.txt
--rw-rw-rw-   0        0        0      887 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Bars.txt
--rw-rw-rw-   0        0        0      374 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Colormap.txt
--rw-rw-rw-   0        0        0      782 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Data.txt
--rw-rw-rw-   0        0        0      674 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Line.txt
--rw-rw-rw-   0        0        0     1232 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Lines.txt
--rw-rw-rw-   0        0        0      670 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Pie.txt
--rw-rw-rw-   0        0        0      872 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Surface.txt
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/__init__.py
--rw-rw-rw-   0        0        0      229 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/bar.py
--rw-rw-rw-   0        0        0     1025 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/bars.py
--rw-rw-rw-   0        0        0      872 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/colorplot.py
--rw-rw-rw-   0        0        0      255 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/data.py
--rw-rw-rw-   0        0        0      232 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/line.py
--rw-rw-rw-   0        0        0     1677 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/lines.py
--rw-rw-rw-   0        0        0      387 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/pie.py
--rw-rw-rw-   0        0        0     1014 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/surface.py
--rw-rw-rw-   0        0        0     5536 2023-06-14 09:00:42.000000 hgutilities-1.0.6/hgutilities/plotting/figure.py
--rw-rw-rw-   0        0        0     2609 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/figures.py
--rw-rw-rw-   0        0        0      398 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotfunctions.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.700353 hgutilities-1.0.6/hgutilities/plotting/plottypes/
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.701352 hgutilities-1.0.6/hgutilities/plotting/plottypes/Documentation/
--rw-rw-rw-   0        0        0      508 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/Documentation/Plot.txt
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/Documentation/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/__init__.py
--rw-rw-rw-   0        0        0     3301 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plot.py
--rw-rw-rw-   0        0        0     3444 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotbars.py
--rw-rw-rw-   0        0        0     2671 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotcolorplot.py
--rw-rw-rw-   0        0        0     6829 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotlines.py
--rw-rw-rw-   0        0        0     1284 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotpie.py
--rw-rw-rw-   0        0        0     3786 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotsurface.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.706352 hgutilities-1.0.6/hgutilities/plotting/plotutils/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-06-14 09:00:40.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/figuresize.py
--rw-rw-rw-   0        0        0     4561 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/griddimensions.py
--rw-rw-rw-   0        0        0     4541 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/plotshape.py
--rw-rw-rw-   0        0        0     1330 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/savefigure.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.709352 hgutilities-1.0.6/hgutilities/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/__init__.py
--rw-rw-rw-   0        0        0      195 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/dicts.py
--rw-rw-rw-   0        0        0     1456 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/groups.py
--rw-rw-rw-   0        0        0      961 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/paths.py
--rw-rw-rw-   0        0        0      697 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/plots.py
-drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.605673 hgutilities-1.0.6/hgutilities.egg-info/
--rw-rw-rw-   0        0        0     7982 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3707 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 09:11:27.709352 hgutilities-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1491 2023-06-14 09:09:51.000000 hgutilities-1.0.6/setup.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.867899 hgutilities-1.0.7/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.766529 hgutilities-1.0.7/.eggs/
+-rw-r-----   0 henry     (1000) henry     (1000)      211 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/README.txt
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.759081 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.771250 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/
+-rw-r-----   0 henry     (1000) henry     (1000)     1023 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE
+-rw-r-----   0 henry     (1000) henry     (1000)    24836 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     2575 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD
+-rw-r-----   0 henry     (1000) henry     (1000)       92 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/WHEEL
+-rw-r-----   0 henry     (1000) henry     (1000)     1734 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      102 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       15 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/zip-safe
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.783253 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/
+-rw-r-----   0 henry     (1000) henry     (1000)     5891 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)       98 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__main__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.790547 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     7516 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4963 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1634 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2634 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    10366 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3086 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5165 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     6554 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5593 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    10226 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)    24841 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2845 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2696 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.792491 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.794539 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      252 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/__init__.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4755 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1190 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2838 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py
+-rw-r-----   0 henry     (1000) henry     (1000)      530 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1067 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py
+-rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1575 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py
+-rw-r-----   0 henry     (1000) henry     (1000)     7237 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1867 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3100 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4287 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2293 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py
+-rw-r-----   0 henry     (1000) henry     (1000)     9599 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1776 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6128 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4166 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3620 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py
+-rw-r-----   0 henry     (1000) henry     (1000)      585 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py
+-rw-r-----   0 henry     (1000) henry     (1000)     5117 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py
+-rw-r-----   0 henry     (1000) henry     (1000)    17034 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.760212 hgutilities-1.0.7/.github/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.795112 hgutilities-1.0.7/.github/workflows/
+-rw-r-----   0 henry     (1000) henry     (1000)     1084 2023-06-18 19:06:03.000000 hgutilities-1.0.7/.github/workflows/python-publish.yml
+-rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-18 19:06:03.000000 hgutilities-1.0.7/LICENSE.md
+-rw-r-----   0 henry     (1000) henry     (1000)     7811 2023-06-18 20:15:22.867430 hgutilities-1.0.7/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     7148 2023-06-18 19:06:03.000000 hgutilities-1.0.7/README.md
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.795606 hgutilities-1.0.7/hgutilities/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.799137 hgutilities-1.0.7/hgutilities/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2483 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/Documentation/hgutilities.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.799663 hgutilities-1.0.7/hgutilities/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      368 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/__pycache__/__init__.cpython-310.pyc
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.802340 hgutilities-1.0.7/hgutilities/defaults/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.805851 hgutilities-1.0.7/hgutilities/defaults/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      614 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/Documentation/defaults.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/Documentation/docs.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      353 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/Documentation/inherit.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      608 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/Documentation/loaddefaults.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      524 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/Documentation/processkwargs.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      239 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.808755 hgutilities-1.0.7/hgutilities/defaults/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      448 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3821 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      765 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2281 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3202 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2962 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/docs.py
+-rw-r-----   0 henry     (1000) henry     (1000)      671 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/inherit.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1562 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/loaddefaults.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2571 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/defaults/processkwargs.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.812069 hgutilities-1.0.7/hgutilities/plotting/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.814338 hgutilities-1.0.7/hgutilities/plotting/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)      195 2023-06-18 19:27:52.000000 hgutilities-1.0.7/hgutilities/plotting/Default Settings/Animate.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      830 2023-06-18 19:56:12.000000 hgutilities-1.0.7/hgutilities/plotting/Default Settings/Figure.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      361 2023-06-18 19:56:18.000000 hgutilities-1.0.7/hgutilities/plotting/Default Settings/Figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.818905 hgutilities-1.0.7/hgutilities/plotting/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/Documentation/Animate.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      414 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/Documentation/Figure.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      564 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/Documentation/Figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)      791 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/Documentation/create_animations.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      612 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/Documentation/create_figures.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1155 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/Documentation/plotting.txt
+-rw-r-----   0 henry     (1000) henry     (1000)    11039 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/README.md
+-rw-r-----   0 henry     (1000) henry     (1000)     1132 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.821802 hgutilities-1.0.7/hgutilities/plotting/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)     1137 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4083 2023-06-18 19:35:30.000000 hgutilities-1.0.7/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     7866 2023-06-18 20:03:47.000000 hgutilities-1.0.7/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3949 2023-06-18 19:32:07.000000 hgutilities-1.0.7/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      574 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2936 2023-06-18 19:35:17.000000 hgutilities-1.0.7/hgutilities/plotting/animate.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.827030 hgutilities-1.0.7/hgutilities/plotting/datatypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.832551 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/
+-rw-r-----   0 henry     (1000) henry     (1000)      283 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Bar.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      183 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Bars.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      738 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      570 2023-06-18 20:07:01.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Data.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1135 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Line.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Lines.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      355 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Pie.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      582 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Surface.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.838024 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      664 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Bar.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      869 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Bars.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      365 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Colormap.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Data.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      659 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Line.txt
+-rw-r-----   0 henry     (1000) henry     (1000)     1210 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Lines.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Pie.txt
+-rw-r-----   0 henry     (1000) henry     (1000)      859 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Surface.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.843473 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1564 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1304 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      731 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      590 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2260 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      813 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1657 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/bar.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1025 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/bars.py
+-rw-r-----   0 henry     (1000) henry     (1000)      872 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/colorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)      255 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/data.py
+-rw-r-----   0 henry     (1000) henry     (1000)      232 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/line.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1677 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/lines.py
+-rw-r-----   0 henry     (1000) henry     (1000)      387 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/pie.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1014 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/datatypes/surface.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6189 2023-06-18 20:02:49.000000 hgutilities-1.0.7/hgutilities/plotting/figure.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2899 2023-06-18 19:31:35.000000 hgutilities-1.0.7/hgutilities/plotting/figures.py
+-rw-r-----   0 henry     (1000) henry     (1000)      398 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plotfunctions.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.847570 hgutilities-1.0.7/hgutilities/plotting/plottypes/
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.848802 hgutilities-1.0.7/hgutilities/plotting/plottypes/Documentation/
+-rw-r-----   0 henry     (1000) henry     (1000)      508 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/Documentation/Plot.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/Documentation/__init__.py
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.853297 hgutilities-1.0.7/hgutilities/plotting/plottypes/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4394 2023-06-18 20:09:09.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3938 2023-06-18 20:06:55.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2030 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4726 2023-06-18 20:06:55.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1377 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     3246 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     4015 2023-06-18 20:11:52.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/plot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3530 2023-06-18 20:06:50.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/plotbars.py
+-rw-r-----   0 henry     (1000) henry     (1000)     2671 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/plotcolorplot.py
+-rw-r-----   0 henry     (1000) henry     (1000)     6917 2023-06-18 20:06:26.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/plotlines.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1284 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/plotpie.py
+-rw-r-----   0 henry     (1000) henry     (1000)     3786 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plottypes/plotsurface.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.856547 hgutilities-1.0.7/hgutilities/plotting/plotutils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.859321 hgutilities-1.0.7/hgutilities/plotting/plotutils/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1177 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     5394 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1505 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      719 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/figuresize.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4561 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/griddimensions.py
+-rw-r-----   0 henry     (1000) henry     (1000)     4541 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/plotshape.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1429 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/plotting/plotutils/savefigure.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.862325 hgutilities-1.0.7/hgutilities/utils/
+-rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/utils/__init__.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.865166 hgutilities-1.0.7/hgutilities/utils/__pycache__/
+-rw-r-----   0 henry     (1000) henry     (1000)      184 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      511 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     2048 2023-06-18 19:09:39.000000 hgutilities-1.0.7/hgutilities/utils/__pycache__/groups.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)     1422 2023-06-18 19:09:38.000000 hgutilities-1.0.7/hgutilities/utils/__pycache__/paths.cpython-310.pyc
+-rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/utils/dicts.py
+-rw-r-----   0 henry     (1000) henry     (1000)     1830 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/utils/groups.py
+-rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/utils/paths.py
+-rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-18 19:06:03.000000 hgutilities-1.0.7/hgutilities/utils/plots.py
+drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-18 20:15:22.798163 hgutilities-1.0.7/hgutilities.egg-info/
+-rw-r-----   0 henry     (1000) henry     (1000)     7811 2023-06-18 20:15:22.000000 hgutilities-1.0.7/hgutilities.egg-info/PKG-INFO
+-rw-r-----   0 henry     (1000) henry     (1000)     9254 2023-06-18 20:15:22.000000 hgutilities-1.0.7/hgutilities.egg-info/SOURCES.txt
+-rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-18 20:15:22.000000 hgutilities-1.0.7/hgutilities.egg-info/dependency_links.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-18 20:15:22.000000 hgutilities-1.0.7/hgutilities.egg-info/requires.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-18 20:15:22.000000 hgutilities-1.0.7/hgutilities.egg-info/top_level.txt
+-rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-18 20:15:22.868023 hgutilities-1.0.7/setup.cfg
+-rw-r-----   0 henry     (1000) henry     (1000)     1453 2023-06-18 20:14:33.000000 hgutilities-1.0.7/setup.py
```

### Comparing `hgutilities-1.0.6/LICENSE.md` & `hgutilities-1.0.7/LICENSE.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `hgutilities-1.0.6/PKG-INFO` & `hgutilities-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: hgutilities
-Version: 1.0.6
-Summary: A triple of tools used for plotting, handling key-words, and utilities
-Author: Henry Ginn
-Author-email: <henryginn137@gmail.com>
-Keywords: python,matplotlib,plotting,default,keywords,utils
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
-- add README to defaults subpackage
+Metadata-Version: 2.1
+Name: hgutilities
+Version: 1.0.7
+Summary: A triple of tools used for plotting, handling key-words, and utilities
+Author: Henry Ginn
+Author-email: <henryginn137@gmail.com>
+Keywords: python,matplotlib,plotting,default,keywords,utils
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
```

### Comparing `hgutilities-1.0.6/README.md` & `hgutilities-1.0.7/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
 - add README to defaults subpackage
```

### Comparing `hgutilities-1.0.6/hgutilities/Documentation/hgutilities.txt` & `hgutilities-1.0.7/hgutilities/Documentation/hgutilities.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-This is a collection of useful tools I use regularly.
-
-There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-Defaults:
-This part of the package aims to make passing in keyword value pairs into classes easier. A list of keywords with their default values are stored in files and are loaded in upon creation of the class. When keywords are passed into a class, they can be fed into this sub-package along with the object instance where they are processed. Classes also inherit default values from parent classes. Tools for documentation and inheriting attributes from one object to another are also included.
-
-Plotting:
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of the plotting part of the package is to make the creation of such figures easier.
-
-Utils:
-The aim of the utils part of this package is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed and it has been left undocumented. Where suitable spellings and names are consistent with matplotlib.
-
-For further documentation see the following:
-hgutils.defaults, hgutils.plotting
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This is a collection of useful tools I use regularly.
+
+There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+Defaults:
+This part of the package aims to make passing in keyword value pairs into classes easier. A list of keywords with their default values are stored in files and are loaded in upon creation of the class. When keywords are passed into a class, they can be fed into this sub-package along with the object instance where they are processed. Classes also inherit default values from parent classes. Tools for documentation and inheriting attributes from one object to another are also included.
+
+Plotting:
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of the plotting part of the package is to make the creation of such figures easier.
+
+Utils:
+The aim of the utils part of this package is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed and it has been left undocumented. Where suitable spellings and names are consistent with matplotlib.
+
+For further documentation see the following:
+hgutils.defaults, hgutils.plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.6/hgutilities/defaults/Documentation/docs.txt` & `hgutilities-1.0.7/hgutilities/defaults/Documentation/docs.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-The purpose of this function is to prevent bloated doc strings
-at the start of modules, classes, and functions by storing the
-doc strings in text files.
-
-By placing "defaults.docs()" in a package __init__.py file, all the
-modules, classes, and functions that were imported within that file
-that are part of the package will have their doc strings set. The
-doc strings are set from text files stored in folders called
-"Documentation", and these folders are in the same directory as
-the script for the corresponding module, class, or function.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+The purpose of this function is to prevent bloated doc strings
+at the start of modules, classes, and functions by storing the
+doc strings in text files.
+
+By placing "defaults.docs()" in a package __init__.py file, all the
+modules, classes, and functions that were imported within that file
+that are part of the package will have their doc strings set. The
+doc strings are set from text files stored in folders called
+"Documentation", and these folders are in the same directory as
+the script for the corresponding module, class, or function.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.6/hgutilities/defaults/Documentation/loaddefaults.txt` & `hgutilities-1.0.7/hgutilities/defaults/Documentation/loaddefaults.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Load
-
-Takes key-word value pairs in a json file and sets them as
-class attributes. The file will have the same name as the class
-and should be located in a folder called "Default Settings" in
-the same folder as the script where the class is defined.
-
-After a class, (e.g. "MyClass") has been defined, calling
-"Defaults.load(MyClass)" will load from the file if it exists.
-
-Any keyword-value pairs defined in parent classes will be
-inherited.
-
-For further documentation see the following:
-kwargs
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+Load
+
+Takes key-word value pairs in a json file and sets them as
+class attributes. The file will have the same name as the class
+and should be located in a folder called "Default Settings" in
+the same folder as the script where the class is defined.
+
+After a class, (e.g. "MyClass") has been defined, calling
+"Defaults.load(MyClass)" will load from the file if it exists.
+
+Any keyword-value pairs defined in parent classes will be
+inherited.
+
+For further documentation see the following:
+kwargs
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.6/hgutilities/defaults/Documentation/processkwargs.txt` & `hgutilities-1.0.7/hgutilities/defaults/Documentation/processkwargs.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Allows the user to easily set the key-words passed in to classes
-as object attributes.
-
-Calling "defaults.kwargs(self, **kwargs)" or
-"defaults.kwargs(self, kwargs)" will take any key-word value pairs
-in the kwargs dict and assign them as object variables. If these
-key-words had default values set, they will be overruled by the new
-values passed in.
-
-For further documentation see the following:
-load, inherit
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+Allows the user to easily set the key-words passed in to classes
+as object attributes.
+
+Calling "defaults.kwargs(self, **kwargs)" or
+"defaults.kwargs(self, kwargs)" will take any key-word value pairs
+in the kwargs dict and assign them as object variables. If these
+key-words had default values set, they will be overruled by the new
+values passed in.
+
+For further documentation see the following:
+load, inherit
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.6/hgutilities/defaults/docs.py` & `hgutilities-1.0.7/hgutilities/defaults/docs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/defaults/inherit.py` & `hgutilities-1.0.7/hgutilities/defaults/inherit.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/defaults/loaddefaults.py` & `hgutilities-1.0.7/hgutilities/defaults/loaddefaults.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.7/hgutilities/defaults/processkwargs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/Default Settings/Figure.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Data.txt`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3888888888888889%*

 * *Differences: {"'axes'": 'True',*

 * * "'legend'": 'False',*

 * * "'legend_loc'": 'None',*

 * * "'projection'": 'None',*

 * * "'x_ha'": "'center'",*

 * * "'x_rotation'": 'None',*

 * * "'x_va'": "'top'",*

 * * "'y_ha'": "'right'",*

 * * "'y_rotation'": 'None',*

 * * "'y_va'": "'center'",*

 * * 'delete': "['dark', 'maximise', 'dpi', 'figure_size', 'subplots', 'w_pad', 'h_pad', 'hspace', "*

 * *           "'wspace', 'x_axis_rotation', 'y_axis_rotation', 'z_axis_rotation']"}*

```diff
@@ -1,28 +1,26 @@
 {
+    "axes": true,
     "axis_color": null,
     "axis_fontname": null,
     "axis_fontsize": null,
     "axis_labelpad": null,
     "axis_loc": null,
-    "dark": false,
-    "dpi": null,
-    "figure_size": null,
-    "h_pad": 0.3,
-    "hspace": null,
-    "maximise": true,
-    "subplots": null,
+    "legend": false,
+    "legend_loc": null,
+    "projection": null,
     "title": null,
     "title_color": null,
     "title_fontname": null,
     "title_fontsize": null,
     "title_horizontalalignment": null,
     "title_loc": null,
     "title_pad": null,
     "title_verticalalignment": null,
     "title_y": null,
-    "w_pad": 0.3,
-    "wspace": null,
-    "x_axis_rotation": 0,
-    "y_axis_rotation": 0,
-    "z_axis_rotation": 0
+    "x_ha": "center",
+    "x_rotation": null,
+    "x_va": "top",
+    "y_ha": "right",
+    "y_rotation": null,
+    "y_va": "center"
 }
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/Documentation/Animate.txt` & `hgutilities-1.0.7/hgutilities/plotting/Documentation/Animate.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-A subclass of Figures, this is responsible for creating
-short animations.
-
-create_animations is an interface for this class.
-
-Takes in a list of Data objects. These are just like
-regular Data objects, but the dependent variable should
-instead be an iterable where each element gives the values
-for a single frame.
-
-Currently this is only implemented for Surface objects.
-
-Animate.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+A subclass of Figures, this is responsible for creating
+short animations.
+
+create_animations is an interface for this class.
+
+Takes in a list of Data objects. These are just like
+regular Data objects, but the dependent variable should
+instead be an iterable where each element gives the values
+for a single frame.
+
+Currently this is only implemented for Surface objects.
+
+Animate.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/Documentation/create_animations.txt` & `hgutilities-1.0.7/hgutilities/plotting/Documentation/create_animations.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-This function will take in a list of data objects
-and produce an animation. These Data objects are just
-like regular Data objects, but the dependent variable
-should instead be an iterable where each element gives
-the values for a single frame.
-
-This is an interface for the Animate class, and to
-see a list of optional key-word arguments you can
-look at Animate.defaults, Figures.defaults and
-Figure.defaults.
-
-This also returns the Figures object produced if
-the user wants to work with it directly, but this
-is not encouraged, and should only be necessary if
-a feature has not been implemented.
-
-For further documentation see the following:
-Animate, Figures, and Data classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This function will take in a list of data objects
+and produce an animation. These Data objects are just
+like regular Data objects, but the dependent variable
+should instead be an iterable where each element gives
+the values for a single frame.
+
+This is an interface for the Animate class, and to
+see a list of optional key-word arguments you can
+look at Animate.defaults, Figures.defaults and
+Figure.defaults.
+
+This also returns the Figures object produced if
+the user wants to work with it directly, but this
+is not encouraged, and should only be necessary if
+a feature has not been implemented.
+
+For further documentation see the following:
+Animate, Figures, and Data classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/Documentation/create_figures.txt` & `hgutilities-1.0.7/hgutilities/plotting/Documentation/create_figures.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-This function will take in a list of data objects
-and produce a set of figures showing them.
-
-This is an interface for the Figures class, and to
-see a list of optional key-word arguments you can
-look at Figures.defaults and Figure.defaults.
-
-This also returns the Figures object produced if
-the user wants to work with it directly, but this
-is not encouraged, and should only be necessary if
-a feature has not been implemented.
-
-For further documentation see the following:
-Figures and Data classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This function will take in a list of data objects
+and produce a set of figures showing them.
+
+This is an interface for the Figures class, and to
+see a list of optional key-word arguments you can
+look at Figures.defaults and Figure.defaults.
+
+This also returns the Figures object produced if
+the user wants to work with it directly, but this
+is not encouraged, and should only be necessary if
+a feature has not been implemented.
+
+For further documentation see the following:
+Figures and Data classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/Documentation/plotting.txt` & `hgutilities-1.0.7/hgutilities/plotting/Documentation/plotting.txt`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-This package is an interface for matplotlib and is designed to make
-creation and processing of figures with subplots easier. The data and
-settings are specified, and they are arranged on figures where the user
-can control the maximum number of subplots on each figure and prescribe
-a target aspect ratio. If the subplots do not fit on one figure, they
-will be spread over multiple figures. The number of figures is no more
-than the ceiling of the total number of plots divided by the maximum
-number of plots per figure.
-
-While this package offers a lot of flexibility, it is mainly intended for
-convenient production of figures. For publication quality plots, it is
-recommended that the full flexibility of matplotlib or other plotting
-packages should be used instead. This package performs best for purposes
-such as analysing data and making powerpoints to be shared among
-colleages and students.
-
-Functions defined here:
-
-create_figures
-create_animations
-
-For further documentation see the following:
-Data and Figures classes and functions from the above list
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+This package is an interface for matplotlib and is designed to make
+creation and processing of figures with subplots easier. The data and
+settings are specified, and they are arranged on figures where the user
+can control the maximum number of subplots on each figure and prescribe
+a target aspect ratio. If the subplots do not fit on one figure, they
+will be spread over multiple figures. The number of figures is no more
+than the ceiling of the total number of plots divided by the maximum
+number of plots per figure.
+
+While this package offers a lot of flexibility, it is mainly intended for
+convenient production of figures. For publication quality plots, it is
+recommended that the full flexibility of matplotlib or other plotting
+packages should be used instead. This package performs best for purposes
+such as analysing data and making powerpoints to be shared among
+colleages and students.
+
+Functions defined here:
+
+create_figures
+create_animations
+
+For further documentation see the following:
+Data and Figures classes and functions from the above list
+https://github.com/HenryGinn/HGUtils
+https://github.com/HenryGinn/HGUtils/tree/main/Plotting
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/README.md` & `hgutilities-1.0.7/hgutilities/plotting/README.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/__init__.py` & `hgutilities-1.0.7/hgutilities/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/animate.py` & `hgutilities-1.0.7/hgutilities/plotting/animate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import PIL
 import io
+import os
+import __main__
 
-from matplotlib.pyplot import savefig
-from matplotlib.pyplot import show
+import matplotlib.pyplot as plt
+import numpy as np
 
 from .figures import Figures
 from .. import defaults
 
 class Animate(Figures):
     
     def __init__(self, data_objects, **kwargs):
@@ -17,14 +19,15 @@
         self.process_data_objects()
         self.set_figure_objects(**kwargs)
         self.prepare_animation_settings()
         self.animate_data_objects()
 
     def prepare_animation_settings(self):
         self.output = None
+        self.set_path()
         self.set_animation_axis_limits()
         self.set_figure_animation_settings()
 
     def set_animation_axis_limits(self):
         for figure_obj in self.figure_objects:
             figure_obj.set_animation_axis_limits()
 
@@ -34,45 +37,54 @@
             figure_obj.figure_size = self.figure_size
 
     def animate_data_objects(self):
         for figure_obj in self.figure_objects:
             self.animate_figure(figure_obj)
 
     def animate_figure(self, figure_obj):
-        frame_count = figure_obj.get_frame_count()
+        self.frame_count = figure_obj.get_frame_count()
         self.set_all_data_values(figure_obj)
-        frames = self.get_frames(figure_obj, frame_count)
-        self.save_animation(frames)
+        self.create_animation(figure_obj)
 
     def set_all_data_values(self, figure_obj):
         figure_obj.all_data_values = [data_obj.get_data_values()
                                       for data_obj in figure_obj.data_objects]
 
-    def get_frames(self, figure_obj, frame_count):
+    def create_animation(self, figure_obj):
+        frames = self.get_frames(figure_obj)
+        self.save_animation(frames)
+
+    def get_frames(self, figure_obj):
         frames = [self.get_frame(figure_obj, index)
-                  for index in range(frame_count)]
+                  for index in range(self.frame_count)]
         return frames
 
     def get_frame(self, figure_obj, index):
         buffer = self.get_buffer(figure_obj, index)
-        image = self.get_image(buffer, figure_obj)
+        image = self.get_image(buffer, figure_obj).copy()
+        plt.close()
         return image
 
     def get_buffer(self, figure_obj, index):
         figure_obj.set_data_value(index)
         figure_obj.create_figure()
         buffer = io.BytesIO()
         return buffer
 
     def get_image(self, buffer, figure_obj):
-        savefig(buffer, dpi=figure_obj.fig.dpi)
+        plt.savefig(buffer, dpi=figure_obj.fig.dpi)
         buffer.seek(0)
         image = PIL.Image.open(buffer)
         image = image.resize(figure_obj.figure_size_pixels)
         return image
 
     def save_animation(self, frames):
-        animation_path = f"{self.animation_name}.{self.format}"
-        frames[0].save(animation_path, loop=self.loop, save_all=True,
+        path = self.get_animation_path()
+        frames[0].save(path, loop=self.loop, save_all=True,
                        append_images=frames[1:], duration=self.duration)
 
+    def get_animation_path(self):
+        name = f"{self.animation_name}.{self.format}"
+        path = os.path.join(self.path, name)
+        return path
+
 defaults.load(Animate)
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Line.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Line.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Surface.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Default Settings/Surface.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Bar.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Bar.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Contains information about a single data series on a bar chart.
-Anything that affects the entire chart should be specied upon creation
-of Bars objects. Almost all features of matplotlib bar charts are
-supported, and the key-word arguments are the same. Care must be
-taken to enter the key-word arguments in relevant object (Bars
-properties not entered into Bar properties and vice versa).
-
-Bar.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
+Contains information about a single data series on a bar chart.
+Anything that affects the entire chart should be specied upon creation
+of Bars objects. Almost all features of matplotlib bar charts are
+supported, and the key-word arguments are the same. Care must be
+taken to enter the key-word arguments in relevant object (Bars
+properties not entered into Bar properties and vice versa).
+
+Bar.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Bars.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Bars.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-This is a subclass of Data used to create bar charts.
-It takes in a bar object, or an iterable of bar objects,
-and keyword arguments thar are relevant only to the entire
-plot. If you wanted every data series to be the same color,
-you would need to specify that for each bar object, but if
-you wanted a log scale, you would specify that at this level.
-If it does not make sense for two distinct data series to
-have different values for a property, then it should be a
-property of this object. For more detail, look at the
-default values for Bars and Bar objects.
-
-Bars.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Bar, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
+This is a subclass of Data used to create bar charts.
+It takes in a bar object, or an iterable of bar objects,
+and keyword arguments thar are relevant only to the entire
+plot. If you wanted every data series to be the same color,
+you would need to specify that for each bar object, but if
+you wanted a log scale, you would specify that at this level.
+If it does not make sense for two distinct data series to
+have different values for a property, then it should be a
+property of this object. For more detail, look at the
+default values for Bars and Bar objects.
+
+Bars.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Bar, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Line.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Line.txt`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Contains information about a single data series
-on a line or scatter graph. Anything that affects
-the entire chart should be specified upon creation
-of Lines objects. Properties such as line color,
-line style, line thickness, and errors in x or y
-should be specified here.If a line is given a label
-then this label will be used in the chart legend.
-
-Line.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Lines, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+Contains information about a single data series
+on a line or scatter graph. Anything that affects
+the entire chart should be specified upon creation
+of Lines objects. Properties such as line color,
+line style, line thickness, and errors in x or y
+should be specified here.If a line is given a label
+then this label will be used in the chart legend.
+
+Line.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Lines, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Lines.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Lines.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-This is used to create line and scatter graphs and takes in a Line
-object or an iterable of line objects. The scope of this object is the
-entire plot, and data about individual lines should be specified by
-Line objects. Properties such as whether the plot has a legend, what
-the title and axis labels are, and the plot type are relevant at this
-level. If it does not make sense for two distinct data series to have
-different values for a property, then it should be a property of this
-object. For more detail, look at the default values for Lines and Line objects.
-
-The plot_type key-word controls which matplotlib plotting function is
-used to create the plot. The options are "plot", "semilogx", "semilogy",
-"loglog", "scatter", and "errorbar". If values for xerr and yerr are
-given for any line object, this will not be detected. The keyword
-plot_type="errorbar" needs to be passed in explicitily.
-
-lines.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Line, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+This is used to create line and scatter graphs and takes in a Line
+object or an iterable of line objects. The scope of this object is the
+entire plot, and data about individual lines should be specified by
+Line objects. Properties such as whether the plot has a legend, what
+the title and axis labels are, and the plot type are relevant at this
+level. If it does not make sense for two distinct data series to have
+different values for a property, then it should be a property of this
+object. For more detail, look at the default values for Lines and Line objects.
+
+The plot_type key-word controls which matplotlib plotting function is
+used to create the plot. The options are "plot", "semilogx", "semilogy",
+"loglog", "scatter", and "errorbar". If values for xerr and yerr are
+given for any line object, this will not be detected. The keyword
+plot_type="errorbar" needs to be passed in explicitily.
+
+lines.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Line, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Pie.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Pie.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-This is a Data subclass used to create pie charts. A pie chart can only
-display one data series, and so this takes in a list of values and
-labels directly unlike the Lines and Bars classes. Almost all
-matplotlib pie chart keyword arguments are accepted, and information
-about the plot legend should also be passed in, either upon creation
-or set directly.
-
-Pie.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Data and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pie.html
+This is a Data subclass used to create pie charts. A pie chart can only
+display one data series, and so this takes in a list of values and
+labels directly unlike the Lines and Bars classes. Almost all
+matplotlib pie chart keyword arguments are accepted, and information
+about the plot legend should also be passed in, either upon creation
+or set directly.
+
+Pie.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Data and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pie.html
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Surface.txt` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/Documentation/Surface.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-This is a Data subclass used to create surfaces in 3D. It takes in x, y, and z values, all of which are 2D arrays of the same shape. Only one data series can be shown on each plot. All keyword arguments are the same as the matplotlib keyword arguments. This accepts the following arguments for the plot_type keyword, all of which are the names of the corresponding matplotlib plotting function:
-
-plot_surface: standard surface plotter
-plot_wireframe: shows the surface as a wire frame
-contour: shows the level sets of a function
-
-Surface.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Data and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface.html
+This is a Data subclass used to create surfaces in 3D. It takes in x, y, and z values, all of which are 2D arrays of the same shape. Only one data series can be shown on each plot. All keyword arguments are the same as the matplotlib keyword arguments. This accepts the following arguments for the plot_type keyword, all of which are the names of the corresponding matplotlib plotting function:
+
+plot_surface: standard surface plotter
+plot_wireframe: shows the surface as a wire frame
+contour: shows the level sets of a function
+
+Surface.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Data and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface.html
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/bars.py` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/bars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/colorplot.py` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/colorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/lines.py` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/lines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/datatypes/surface.py` & `hgutilities-1.0.7/hgutilities/plotting/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/figure.py` & `hgutilities-1.0.7/hgutilities/plotting/figure.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .plottypes.plotbars import PlotBars
 from .plottypes.plotpie import PlotPie
 from .plottypes.plotcolorplot import PlotColorplot
 from .plottypes.plotsurface import PlotSurface
 from .plotutils.griddimensions import get_grid_dimensions
 from .plotutils.savefigure import save_figure
 from .plotutils.figuresize import maximise_figure
+from ..utils.dicts import remove_none_values
 
 class Figure():
     
     @classmethod
     def set_plot_classes(cls):
         cls.plot_classes = {"Lines": PlotLines,
                             "Bars": PlotBars,
@@ -74,21 +75,32 @@
     
     def remove_extra_axes(self):
         extra_axes_count = len(self.axes) - self.count
         for ax, _ in zip(self.axes[::-1], range(extra_axes_count)):
             ax.remove()
 
     def add_figure_peripherals(self):
+        self.set_suptitle_fontdict()
         self.set_suptitle()
         self.set_universal_legend()
         self.set_figure_size()
 
+    def set_suptitle_fontdict(self):
+        kwargs = {"fontname": self.suptitle_fontname,
+                  "fontsize": self.suptitle_fontsize,
+                  "color": self.suptitle_color,
+                  "verticalalignment": self.suptitle_verticalalignment,
+                  "horizontalalignment": self.suptitle_horizontalalignment}
+        self.suptitle_fontdict = remove_none_values(kwargs)
+
     def set_suptitle(self):
-        if self.figures_obj.title is not None:
-            self.fig.suptitle(f"{self.figures_obj.title}")
+        if self.figures_obj.suptitle is not None:
+            self.fig.suptitle(f"{self.figures_obj.suptitle}",
+                              **self.suptitle_fontdict, loc=self.suptitle_loc,
+                              y=self.suptitle_y, pad=self.suptitle_pad)
 
     def set_universal_legend(self):
         if self.figures_obj.universal_legend:
             self.do_universal_legend()
 
     def do_universal_legend(self):
         ax = self.axes[-1]
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/figures.py` & `hgutilities-1.0.7/hgutilities/plotting/figures.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,20 +41,28 @@
     def create_figures(self, **kwargs):
         self.process_data_objects()
         self.process_output_mode()
         self.plot_data_objects(**kwargs)
 
     def process_output_mode(self):
         if self.output == "Save":
-            self.create_plots_folder()
+            self.set_path()
 
-    def create_plots_folder(self):
+    def set_path(self, plots_folder_name="Plots"):
+        self.set_default_path()
+        self.split_on_plots_folder(plots_folder_name)
+
+    def set_default_path(self):
         if self.path is None:
             self.path = os.path.split(__main__.__file__)[0]
-        make_folder(self.path)
+
+    def split_on_plots_folder(self, plots_folder_name):
+        if self.plots_folder:
+            self.path = os.path.join(self.path, plots_folder_name)
+            make_folder(self.path)
 
     def process_data_objects(self):
         self.subplots = get_group_size(self.subplots, self.data_objects)
         group_indexes = get_group_indexes(self.data_obj_count, self.subplots)
         self.data_object_groups = [self.data_objects[indexes]
                                     for indexes in group_indexes]
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plottypes/plot.py` & `hgutilities-1.0.7/hgutilities/plotting/plottypes/plot.py`

 * *Files 19% similar despite different names*

```diff
@@ -85,8 +85,24 @@
                                **self.axis_fontdict)
 
     def add_z_label(self):
         if self.data_obj.z_label is not None:
             self.ax.set_zlabel(self.data_obj.z_label,
                                **self.axis_fontdict)
 
+    def set_tick_labels(self):
+        self.set_x_tick_labels()
+        self.set_y_tick_labels()
+
+    def set_x_tick_labels(self):
+        if hasattr(self.ax, "set_xticks"):
+            self.ax.set_xticks(self.ax.get_xticks(), self.ax.get_xticklabels(),
+                               rotation=self.data_obj.x_rotation, ha=self.data_obj.x_ha,
+                               va=self.data_obj.x_va)
+
+    def set_y_tick_labels(self):
+        if hasattr(self.ax, "set_yticks"):
+            self.ax.set_yticks(self.ax.get_yticks(), self.ax.get_yticklabels(),
+                               rotation=self.data_obj.y_rotation, ha=self.data_obj.y_ha,
+                               va=self.data_obj.y_va)
+
 defaults.load(Plot)
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plottypes/plotbars.py` & `hgutilities-1.0.7/hgutilities/plotting/plottypes/plotbars.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
     def initialise_from_bars_obj(self):
         self.bar_objects = self.bars_obj.bar_objects
         self.between_group_spacing = self.bars_obj.between_group_spacing
         self.within_group_spacing = self.bars_obj.within_group_spacing
 
     def plot_data(self):
+        self.plot_bars()
+        self.set_tick_labels()
+
+    def plot_bars(self):
         self.preprocess_bars()
         for index, bar_obj in enumerate(self.bars_obj.bar_objects):
             self.plot_bar_obj(index, bar_obj)
 
     def preprocess_bars(self):
         self.group_width = 1 - self.between_group_spacing
         self.set_bar_proportions()
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plottypes/plotcolorplot.py` & `hgutilities-1.0.7/hgutilities/plotting/plottypes/plotcolorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plottypes/plotlines.py` & `hgutilities-1.0.7/hgutilities/plotting/plottypes/plotlines.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
     def __init__(self, figure_obj, ax, lines_obj, **kwargs):
         Plot.__init__(self, figure_obj, ax, lines_obj, **kwargs)
         self.lines_obj = lines_obj
         defaults.kwargs(self, kwargs)
 
     def plot_data(self):
+        self.plot_lines()
+        self.set_tick_labels()
+
+    def plot_lines(self):
         plot_type_function = self.get_plot_type_function()
         plot_function = getattr(self.ax, self.lines_obj.plot_type)
         for line_obj in self.lines_obj.line_objects:
             plot_type_function(self, plot_function, line_obj)
 
     def get_plot_type_function(self):
         plot_type = self.lines_obj.plot_type
```

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plottypes/plotpie.py` & `hgutilities-1.0.7/hgutilities/plotting/plottypes/plotpie.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plottypes/plotsurface.py` & `hgutilities-1.0.7/hgutilities/plotting/plottypes/plotsurface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plotutils/figuresize.py` & `hgutilities-1.0.7/hgutilities/plotting/plotutils/figuresize.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plotutils/griddimensions.py` & `hgutilities-1.0.7/hgutilities/plotting/plotutils/griddimensions.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/plotting/plotutils/plotshape.py` & `hgutilities-1.0.7/hgutilities/plotting/plotutils/plotshape.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.6/hgutilities/utils/paths.py` & `hgutilities-1.0.7/hgutilities/utils/paths.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import os
-import json
-
-def make_file(file_path):
-    if not os.path.exists(file_path):
-        folder_path = os.path.split(file_path)[0]
-        make_folder(folder_path)
-        make_empty_file(file_path)
-
-def make_empty_file(file_path):
-    with open(file_path, "w") as file:
-        pass
-
-def make_folder(folder_path):
-    if not os.path.exists(folder_path):
-        parent_folder_path = os.path.split(folder_path)[0]
-        make_folder(parent_folder_path)
-        os.mkdir(folder_path)
-
-def make_folder_path(path):
-    if os.path.isfile(path):
-        path = os.path.split(path)[0]
-    make_file(path)
-
-def load_json(path, ignore_empty_or_none=True):
-    if ignore_empty_or_none:
-        if not os.path.exists(path) or os.stat(path).st_size == 0:
-            return {}
-    return do_load_json(path)
-
-def do_load_json(path):
-    with open(path, "r") as file:
-        file_contents = json.load(file)
-    return file_contents
+import os
+import json
+
+def make_file(file_path):
+    if not os.path.exists(file_path):
+        folder_path = os.path.split(file_path)[0]
+        make_folder(folder_path)
+        make_empty_file(file_path)
+
+def make_empty_file(file_path):
+    with open(file_path, "w") as file:
+        pass
+
+def make_folder(folder_path):
+    if not os.path.exists(folder_path):
+        parent_folder_path = os.path.split(folder_path)[0]
+        make_folder(parent_folder_path)
+        os.mkdir(folder_path)
+
+def make_folder_path(path):
+    if os.path.isfile(path):
+        path = os.path.split(path)[0]
+    make_file(path)
+
+def load_json(path, ignore_empty_or_none=True):
+    if ignore_empty_or_none:
+        if not os.path.exists(path) or os.stat(path).st_size == 0:
+            return {}
+    return do_load_json(path)
+
+def do_load_json(path):
+    with open(path, "r") as file:
+        file_contents = json.load(file)
+    return file_contents
```

### Comparing `hgutilities-1.0.6/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.7/hgutilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: hgutilities
-Version: 1.0.6
-Summary: A triple of tools used for plotting, handling key-words, and utilities
-Author: Henry Ginn
-Author-email: <henryginn137@gmail.com>
-Keywords: python,matplotlib,plotting,default,keywords,utils
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
-- add README to defaults subpackage
+Metadata-Version: 2.1
+Name: hgutilities
+Version: 1.0.7
+Summary: A triple of tools used for plotting, handling key-words, and utilities
+Author: Henry Ginn
+Author-email: <henryginn137@gmail.com>
+Keywords: python,matplotlib,plotting,default,keywords,utils
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
```

### Comparing `hgutilities-1.0.6/setup.py` & `hgutilities-1.0.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = "1.0.6"
-DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
-LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
-                    "Plotting: a front end for matplotlib to easily create subplots.\n"
-                    "Utils: a collection of generally useful functions")
-
-# Setting up
-setup(
-    name="hgutilities",
-    version=VERSION,
-    author="Henry Ginn",
-    author_email="<henryginn137@gmail.com>",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    setup_requires=['setuptools_scm'],
-    include_package_data=True,
-    install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
-    keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Operating System :: Unix",
-        "Operating System :: Microsoft :: Windows",
-    ]
-)
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+VERSION = "1.0.7"
+DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
+LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
+                    "Plotting: a front end for matplotlib to easily create subplots.\n"
+                    "Utils: a collection of generally useful functions")
+
+# Setting up
+setup(
+    name="hgutilities",
+    version=VERSION,
+    author="Henry Ginn",
+    author_email="<henryginn137@gmail.com>",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    setup_requires=['setuptools_scm'],
+    include_package_data=True,
+    install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
+    keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Operating System :: Unix",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```


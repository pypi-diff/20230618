# Comparing `tmp/dune-iga-0.1.6.dev20230616150758.tar.gz` & `tmp/dune-iga-0.1.6.dev20230618094642.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-iga-0.1.6.dev20230616150758.tar", last modified: Fri Jun 16 15:07:58 2023, max compression
+gzip compressed data, was "dune-iga-0.1.6.dev20230618094642.tar", last modified: Sun Jun 18 09:46:42 2023, max compression
```

## Comparing `dune-iga-0.1.6.dev20230616150758.tar` & `dune-iga-0.1.6.dev20230618094642.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.850531 dune-iga-0.1.6.dev20230616150758/
--rw-r--r--   0 root         (0) root         (0)     1025 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.clang-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.830531 dune-iga-0.1.6.dev20230616150758/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.834531 dune-iga-0.1.6.dev20230616150758/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1384 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.github/workflows/createRelease.yml
--rw-r--r--   0 root         (0) root         (0)     1758 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2245 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     1728 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.github/workflows/reuseLint.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.834531 dune-iga-0.1.6.dev20230616150758/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3200 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.834531 dune-iga-0.1.6.dev20230616150758/.reuse/
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.834531 dune-iga-0.1.6.dev20230616150758/LICENSES/
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-16 15:07:58.850531 dune-iga-0.1.6.dev20230616150758/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.834531 dune-iga-0.1.6.dev20230616150758/cmake/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.834531 dune-iga-0.1.6.dev20230616150758/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/FormatTarget/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/FormatTarget/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.834531 dune-iga-0.1.6.dev20230616150758/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      753 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      843 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/modules/AddClipperLibFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      826 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/modules/AddEarCutFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      824 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/modules/AddnLohmannJsonFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/cmake/modules/DuneIgaMacros.cmake
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.834531 dune-iga-0.1.6.dev20230616150758/dune/
--rw-r--r--   0 root         (0) root         (0)      219 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.838531 dune-iga-0.1.6.dev20230616150758/dune/iga/
--rw-r--r--   0 root         (0) root         (0)      808 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9152 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/bsplinealgorithms.hh
--rw-r--r--   0 root         (0) root         (0)     2017 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/controlpoint.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.838531 dune-iga-0.1.6.dev20230616150758/dune/iga/geometry/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/geometry/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6122 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/geometry/closestpointprojection.hh
--rw-r--r--   0 root         (0) root         (0)     2825 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/geometry/geohelper.hh
--rw-r--r--   0 root         (0) root         (0)     2785 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/gridcapabilities.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.838531 dune-iga-0.1.6.dev20230616150758/dune/iga/io/
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/io/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.838531 dune-iga-0.1.6.dev20230616150758/dune/iga/io/ibra/
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/io/ibra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    10369 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/io/ibra/ibrageometry.hh
--rw-r--r--   0 root         (0) root         (0)     7806 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/io/ibra/ibrareader.hh
--rw-r--r--   0 root         (0) root         (0)     8239 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/io/igadatacollector.hh
--rw-r--r--   0 root         (0) root         (0)    30655 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsalgorithms.hh
--rw-r--r--   0 root         (0) root         (0)    29306 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsbasis.hh
--rw-r--r--   0 root         (0) root         (0)    18305 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgeometry.hh
--rw-r--r--   0 root         (0) root         (0)    11629 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgrid.hh
--rw-r--r--   0 root         (0) root         (0)    13111 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgridentity.hh
--rw-r--r--   0 root         (0) root         (0)     3063 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgridindexsets.hh
--rw-r--r--   0 root         (0) root         (0)     3957 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgridleafiterator.hh
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgridtraits.hh
--rw-r--r--   0 root         (0) root         (0)     1285 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsidset.hh
--rw-r--r--   0 root         (0) root         (0)     7882 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsintersection.hh
--rw-r--r--   0 root         (0) root         (0)     9302 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsleafgridview.hh
--rw-r--r--   0 root         (0) root         (0)     9447 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbslocalgeometry.hh
--rw-r--r--   0 root         (0) root         (0)    36685 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbspatch.hh
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbspatchdata.hh
--rw-r--r--   0 root         (0) root         (0)     9061 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/nurbspatchgeometry.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.842531 dune-iga-0.1.6.dev20230616150758/dune/iga/test/
--rw-r--r--   0 root         (0) root         (0)     1347 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.842531 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)     5772 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/element.ibra
--rw-r--r--   0 root         (0) root         (0)     7222 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/element_trim.ibra
--rw-r--r--   0 root         (0) root         (0)     7396 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra
--rw-r--r--   0 root         (0) root         (0)     7665 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/infty_pwh.ibra
--rw-r--r--   0 root         (0) root         (0)     6209 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/nurbs_1.ibra
--rw-r--r--   0 root         (0) root         (0)     6704 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/pipe_trim.ibra
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/plate_quarter.ibra
--rw-r--r--   0 root         (0) root         (0)    10170 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/schale_trim.ibra
--rw-r--r--   0 root         (0) root         (0)    12176 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/shell-hole.ibra
--rw-r--r--   0 root         (0) root         (0)     7146 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/shell.ibra
--rw-r--r--   0 root         (0) root         (0)     7688 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/surface-hole.ibra
--rw-r--r--   0 root         (0) root         (0)    60433 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/surface-multihole.ibra
--rw-r--r--   0 root         (0) root         (0)    45902 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/gridTests.cc
--rw-r--r--   0 root         (0) root         (0)    17532 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/test/trimmedGridTests.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.842531 dune-iga-0.1.6.dev20230616150758/dune/iga/trim/
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/trim/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4636 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/trim/nurbstrimboundary.hh
--rw-r--r--   0 root         (0) root         (0)    37350 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/trim/nurbstrimmer.hh
--rw-r--r--   0 root         (0) root         (0)    14597 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/trim/trimmedelementrepresentation.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.842531 dune-iga-0.1.6.dev20230616150758/dune/iga/utils/
--rw-r--r--   0 root         (0) root         (0)      328 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2224 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/utils/fillquadraturerule.hh
--rw-r--r--   0 root         (0) root         (0)     2372 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/utils/igahelpers.hh
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/utils/linearalgebra.hh
--rw-r--r--   0 root         (0) root         (0)    22061 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/utils/mdnet.hh
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/iga/utils/typetraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.842531 dune-iga-0.1.6.dev20230616150758/dune/python/
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.846531 dune-iga-0.1.6.dev20230616150758/dune/python/iga/
--rw-r--r--   0 root         (0) root         (0)      290 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/iga/boundarypatch.hh
--rw-r--r--   0 root         (0) root         (0)     6370 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/iga/grid.hh
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/iga/gridenums.hh
--rw-r--r--   0 root         (0) root         (0)     4441 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/iga/nurbspatchdata.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.846531 dune-iga-0.1.6.dev20230616150758/dune/python/test/
--rw-r--r--   0 root         (0) root         (0)      461 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5171 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/test/poisson.py
--rw-r--r--   0 root         (0) root         (0)     5241 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/test/readGrid.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune/python/test/setpath.py.in
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune-iga.pc.in
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/dune.module
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.846531 dune-iga-0.1.6.dev20230616150758/python/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.846531 dune-iga-0.1.6.dev20230616150758/python/dune/
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.846531 dune-iga-0.1.6.dev20230616150758/python/dune/iga/
--rw-r--r--   0 root         (0) root         (0)      675 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/__init__.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/_boundarypatch.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/_iga.cc
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/_igagrids.py
--rw-r--r--   0 root         (0) root         (0)     3110 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/_nurbsAlgorithms.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/_nurbspatchdata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.846531 dune-iga-0.1.6.dev20230616150758/python/dune/iga/basis/
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/python/dune/iga/basis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.846531 dune-iga-0.1.6.dev20230616150758/python/dune_iga.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-16 15:07:58.000000 dune-iga-0.1.6.dev20230616150758/python/dune_iga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3671 2023-06-16 15:07:58.000000 dune-iga-0.1.6.dev20230616150758/python/dune_iga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 15:07:58.000000 dune-iga-0.1.6.dev20230616150758/python/dune_iga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-16 15:07:58.000000 dune-iga-0.1.6.dev20230616150758/python/dune_iga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-16 15:07:58.000000 dune-iga-0.1.6.dev20230616150758/python/dune_iga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 15:07:58.850531 dune-iga-0.1.6.dev20230616150758/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      889 2023-06-16 15:07:58.000000 dune-iga-0.1.6.dev20230616150758/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.846531 dune-iga-0.1.6.dev20230616150758/src/
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 15:07:58.850531 dune-iga-0.1.6.dev20230616150758/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)      228 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/src/auxiliaryFiles/kirchhoff_plate.parset
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/src/auxiliaryFiles/linear2dsolid.parset
--rw-r--r--   0 root         (0) root         (0)     7688 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/src/auxiliaryFiles/surface-hole.ibra
--rw-r--r--   0 root         (0) root         (0)     6609 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/src/kirchhoff_plate.cc
--rw-r--r--   0 root         (0) root         (0)    13589 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/src/kirchhoffplate.hh
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/src/linear2dsolid.cc
--rw-r--r--   0 root         (0) root         (0)    15691 2023-06-16 15:07:50.000000 dune-iga-0.1.6.dev20230616150758/src/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.935542 dune-iga-0.1.6.dev20230618094642/
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.clang-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.907542 dune-iga-0.1.6.dev20230618094642/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.915542 dune-iga-0.1.6.dev20230618094642/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1758 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.github/workflows/reuseLint.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.915542 dune-iga-0.1.6.dev20230618094642/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3200 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.915542 dune-iga-0.1.6.dev20230618094642/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.915542 dune-iga-0.1.6.dev20230618094642/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-18 09:46:42.935542 dune-iga-0.1.6.dev20230618094642/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.915542 dune-iga-0.1.6.dev20230618094642/cmake/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.915542 dune-iga-0.1.6.dev20230618094642/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/FormatTarget/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/FormatTarget/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.919542 dune-iga-0.1.6.dev20230618094642/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      753 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      843 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/modules/AddClipperLibFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      826 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/modules/AddEarCutFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      824 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/modules/AddnLohmannJsonFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/cmake/modules/DuneIgaMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.919542 dune-iga-0.1.6.dev20230618094642/dune/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.923542 dune-iga-0.1.6.dev20230618094642/dune/iga/
+-rw-r--r--   0 root         (0) root         (0)      808 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9152 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/bsplinealgorithms.hh
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/controlpoint.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.923542 dune-iga-0.1.6.dev20230618094642/dune/iga/geometry/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/geometry/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6122 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/geometry/closestpointprojection.hh
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/geometry/geohelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/gridcapabilities.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.923542 dune-iga-0.1.6.dev20230618094642/dune/iga/io/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/io/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.927542 dune-iga-0.1.6.dev20230618094642/dune/iga/io/ibra/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/io/ibra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    10369 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/io/ibra/ibrageometry.hh
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/io/ibra/ibrareader.hh
+-rw-r--r--   0 root         (0) root         (0)     8239 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/io/igadatacollector.hh
+-rw-r--r--   0 root         (0) root         (0)    30655 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsalgorithms.hh
+-rw-r--r--   0 root         (0) root         (0)    29306 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsbasis.hh
+-rw-r--r--   0 root         (0) root         (0)    18305 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgeometry.hh
+-rw-r--r--   0 root         (0) root         (0)    11629 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgrid.hh
+-rw-r--r--   0 root         (0) root         (0)    13111 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgridentity.hh
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgridindexsets.hh
+-rw-r--r--   0 root         (0) root         (0)     3957 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgridleafiterator.hh
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgridtraits.hh
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsidset.hh
+-rw-r--r--   0 root         (0) root         (0)     7979 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsintersection.hh
+-rw-r--r--   0 root         (0) root         (0)     9302 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsleafgridview.hh
+-rw-r--r--   0 root         (0) root         (0)     9447 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbslocalgeometry.hh
+-rw-r--r--   0 root         (0) root         (0)    36685 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbspatch.hh
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbspatchdata.hh
+-rw-r--r--   0 root         (0) root         (0)     9061 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/nurbspatchgeometry.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.927542 dune-iga-0.1.6.dev20230618094642/dune/iga/test/
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.927542 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)     5772 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/element.ibra
+-rw-r--r--   0 root         (0) root         (0)     7222 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/element_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)     7396 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/infty_pwh.ibra
+-rw-r--r--   0 root         (0) root         (0)     6209 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/nurbs_1.ibra
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/pipe_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/plate_quarter.ibra
+-rw-r--r--   0 root         (0) root         (0)    10170 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/schale_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)    12176 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/shell-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)     7146 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/shell.ibra
+-rw-r--r--   0 root         (0) root         (0)     7688 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/surface-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)    60433 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/surface-multihole.ibra
+-rw-r--r--   0 root         (0) root         (0)    45902 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/gridTests.cc
+-rw-r--r--   0 root         (0) root         (0)    17532 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/test/trimmedGridTests.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.931542 dune-iga-0.1.6.dev20230618094642/dune/iga/trim/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/trim/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/trim/nurbstrimboundary.hh
+-rw-r--r--   0 root         (0) root         (0)    37350 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/trim/nurbstrimmer.hh
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/trim/trimmedelementrepresentation.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.931542 dune-iga-0.1.6.dev20230618094642/dune/iga/utils/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/utils/fillquadraturerule.hh
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/utils/igahelpers.hh
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/utils/linearalgebra.hh
+-rw-r--r--   0 root         (0) root         (0)    22274 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/utils/mdnet.hh
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/iga/utils/typetraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.931542 dune-iga-0.1.6.dev20230618094642/dune/python/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.931542 dune-iga-0.1.6.dev20230618094642/dune/python/iga/
+-rw-r--r--   0 root         (0) root         (0)      290 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/iga/boundarypatch.hh
+-rw-r--r--   0 root         (0) root         (0)     6540 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/iga/grid.hh
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/iga/gridenums.hh
+-rw-r--r--   0 root         (0) root         (0)     5102 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/iga/nurbspatchdata.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.931542 dune-iga-0.1.6.dev20230618094642/dune/python/test/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5171 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/test/poisson.py
+-rw-r--r--   0 root         (0) root         (0)     5499 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/test/readGrid.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune/python/test/setpath.py.in
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune-iga.pc.in
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/dune.module
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.931542 dune-iga-0.1.6.dev20230618094642/python/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.931542 dune-iga-0.1.6.dev20230618094642/python/dune/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.935542 dune-iga-0.1.6.dev20230618094642/python/dune/iga/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/_boundarypatch.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/_iga.cc
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/_igagrids.py
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/_nurbsAlgorithms.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/_nurbspatchdata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.935542 dune-iga-0.1.6.dev20230618094642/python/dune/iga/basis/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/python/dune/iga/basis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.935542 dune-iga-0.1.6.dev20230618094642/python/dune_iga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-18 09:46:42.000000 dune-iga-0.1.6.dev20230618094642/python/dune_iga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3671 2023-06-18 09:46:42.000000 dune-iga-0.1.6.dev20230618094642/python/dune_iga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 09:46:42.000000 dune-iga-0.1.6.dev20230618094642/python/dune_iga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-18 09:46:42.000000 dune-iga-0.1.6.dev20230618094642/python/dune_iga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-18 09:46:42.000000 dune-iga-0.1.6.dev20230618094642/python/dune_iga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 09:46:42.935542 dune-iga-0.1.6.dev20230618094642/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-18 09:46:42.000000 dune-iga-0.1.6.dev20230618094642/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.935542 dune-iga-0.1.6.dev20230618094642/src/
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 09:46:42.935542 dune-iga-0.1.6.dev20230618094642/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/src/auxiliaryFiles/kirchhoff_plate.parset
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/src/auxiliaryFiles/linear2dsolid.parset
+-rw-r--r--   0 root         (0) root         (0)     7688 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/src/auxiliaryFiles/surface-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)     6609 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/src/kirchhoff_plate.cc
+-rw-r--r--   0 root         (0) root         (0)    13589 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/src/kirchhoffplate.hh
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/src/linear2dsolid.cc
+-rw-r--r--   0 root         (0) root         (0)    15691 2023-06-18 09:46:35.000000 dune-iga-0.1.6.dev20230618094642/src/linearElastic.hh
```

### Comparing `dune-iga-0.1.6.dev20230616150758/.clang-format` & `dune-iga-0.1.6.dev20230618094642/.clang-format`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/.github/workflows/createRelease.yml` & `dune-iga-0.1.6.dev20230618094642/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/.github/workflows/debian-coverage.yml` & `dune-iga-0.1.6.dev20230618094642/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/.github/workflows/debian.yml` & `dune-iga-0.1.6.dev20230618094642/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/.github/workflows/releasePythonPackage.yml` & `dune-iga-0.1.6.dev20230618094642/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/.github/workflows/scripts/release.py` & `dune-iga-0.1.6.dev20230618094642/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/.github/workflows/style.yml` & `dune-iga-0.1.6.dev20230618094642/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/CMakeLists.txt` & `dune-iga-0.1.6.dev20230618094642/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/LICENSES/CC0-1.0.txt` & `dune-iga-0.1.6.dev20230618094642/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/LICENSES/LGPL-3.0-or-later.txt` & `dune-iga-0.1.6.dev20230618094642/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/PKG-INFO` & `dune-iga-0.1.6.dev20230618094642/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-iga
-Version: 0.1.6.dev20230616150758
+Version: 0.1.6.dev20230618094642
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

### Comparing `dune-iga-0.1.6.dev20230616150758/README.md` & `dune-iga-0.1.6.dev20230618094642/README.md`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/cmake/FormatTarget/CMakeLists.txt` & `dune-iga-0.1.6.dev20230618094642/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/cmake/FormatTarget/CPM.cmake` & `dune-iga-0.1.6.dev20230618094642/cmake/FormatTarget/CPM.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/cmake/modules/AddAutoDiffFlags.cmake` & `dune-iga-0.1.6.dev20230618094642/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/cmake/modules/AddClipperLibFlags.cmake` & `dune-iga-0.1.6.dev20230618094642/cmake/modules/AddClipperLibFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/cmake/modules/AddEarCutFlags.cmake` & `dune-iga-0.1.6.dev20230618094642/cmake/modules/AddEarCutFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/cmake/modules/AddEigenFlags.cmake` & `dune-iga-0.1.6.dev20230618094642/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/cmake/modules/AddnLohmannJsonFlags.cmake` & `dune-iga-0.1.6.dev20230618094642/cmake/modules/AddnLohmannJsonFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/config.h.cmake` & `dune-iga-0.1.6.dev20230618094642/config.h.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/CMakeLists.txt` & `dune-iga-0.1.6.dev20230618094642/dune/iga/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/bsplinealgorithms.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/bsplinealgorithms.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/controlpoint.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/controlpoint.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/geometry/closestpointprojection.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/geometry/closestpointprojection.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/geometry/geohelper.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/geometry/geohelper.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/gridcapabilities.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/gridcapabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/io/ibra/ibrageometry.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/io/ibra/ibrageometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/io/ibra/ibrareader.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/io/ibra/ibrareader.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/io/igadatacollector.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/io/igadatacollector.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsalgorithms.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsalgorithms.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsbasis.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsbasis.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgeometry.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgrid.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgrid.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgridentity.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgridentity.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgridindexsets.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgridindexsets.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgridleafiterator.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgridleafiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsgridtraits.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsgridtraits.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsidset.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsidset.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsintersection.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsintersection.hh`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,20 @@
 
     /** \brief Same as outerNormal() but with unit length */
     [[nodiscard]] GlobalCoordinate unitOuterNormal(const LocalCoordinate& xi) const {
       auto N = this->outerNormal(xi);
       return N / N.two_norm();
     }
 
-    [[nodiscard]] GlobalCoordinate centerUnitOuterNormal() const { return unitOuterNormal(0.5); }
+    [[nodiscard]] GlobalCoordinate centerUnitOuterNormal() const {
+      if constexpr (mydimension == 0)
+        return unitOuterNormal({});
+      else
+        return unitOuterNormal(0.5);
+    }
 
     /** \brief Same as outerNormal() but with the length of the integration element */
     [[nodiscard]] GlobalCoordinate integrationOuterNormal(const LocalCoordinate& xi) const {
       return this->unitOuterNormal(xi) * this->geometry().integrationElement(xi);
     }
 
     /** \brief Returns the consecutive index if this intersection lies on the boundary */
```

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbsleafgridview.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbsleafgridview.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbslocalgeometry.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbslocalgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbspatch.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbspatch.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbspatchdata.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbspatchdata.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/nurbspatchgeometry.h` & `dune-iga-0.1.6.dev20230618094642/dune/iga/nurbspatchgeometry.h`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/CMakeLists.txt` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/element.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/element.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/element_trim.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/element_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/infty_pwh.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/infty_pwh.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/nurbs_1.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/nurbs_1.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/pipe_trim.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/pipe_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/plate_quarter.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/plate_quarter.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/schale_trim.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/schale_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/shell-hole.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/shell-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/shell.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/shell.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/surface-hole.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/surface-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/auxiliaryFiles/surface-multihole.ibra` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/auxiliaryFiles/surface-multihole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/gridTests.cc` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/gridTests.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/test/trimmedGridTests.cc` & `dune-iga-0.1.6.dev20230618094642/dune/iga/test/trimmedGridTests.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/trim/nurbstrimboundary.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/trim/nurbstrimboundary.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/trim/nurbstrimmer.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/trim/nurbstrimmer.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/trim/trimmedelementrepresentation.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/trim/trimmedelementrepresentation.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/utils/concepts.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/utils/fillquadraturerule.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/utils/fillquadraturerule.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/utils/igahelpers.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/utils/igahelpers.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/utils/linearalgebra.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/utils/linearalgebra.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/iga/utils/mdnet.hh` & `dune-iga-0.1.6.dev20230618094642/dune/iga/utils/mdnet.hh`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,19 @@
     }
 
     explicit MultiDimensionNet(const std::vector<std::vector<ValueType>>& vals) {
       std::array<int, netdim> dimsize = {static_cast<int>(vals.size()), static_cast<int>(vals.begin()->size())};
       *this                           = MultiDimensionNet{dimsize, vals};
     }
 
+    explicit MultiDimensionNet(const std::vector<ValueType>& vals) {
+      std::array<int, 1> dimsize = {static_cast<int>(vals.size())};
+      *this                      = MultiDimensionNet{dimsize, vals};
+    }
+
     /** \brief constructor for a net of a certain strideSizes with values unknown.
      *
      *  \param[in] dimSize array of the strideSizes of each dimension
      */
     explicit MultiDimensionNet(const std::array<int, netdim>& dimSize) : dimSize_(dimSize) {
       int size_ = 1;
       for (auto ds : dimSize)
```

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/python/iga/boundarypatch.hh` & `dune-iga-0.1.6.dev20230618094642/dune/python/iga/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/python/iga/grid.hh` & `dune-iga-0.1.6.dev20230618094642/dune/python/iga/grid.hh`

 * *Files 2% similar despite different names*

```diff
@@ -75,34 +75,41 @@
       pybind11::module module, pybind11::class_<NURBSGrid, options...> cls) {
     using pybind11::operator""_a;
 
     static constexpr std::integral auto dimension      = NURBSGrid::dimension;
     static constexpr std::integral auto dimensionworld = NURBSGrid::dimensionworld;
     using ctype                                        = typename NURBSGrid::ctype;
 
-    module.def("reader", [](const pybind11::dict& args_) { return Dune::Python::IGA::reader<NURBSGrid>(args_); });
+    if constexpr (dimension == 2)
+      module.def("reader", [](const pybind11::dict& args_) { return Dune::Python::IGA::reader<NURBSGrid>(args_); });
 
     Dune::Python::registerHierarchicalGrid(module, cls);
     using LeafGridView = typename NURBSGrid::LeafGridView;
     auto clsLeafView   = insertClass<LeafGridView>(module, "LeafGrid", GenerateTypeName(cls, "LeafGridView"));
     if (clsLeafView.second) registerGridView(module, clsLeafView.first);
 
 #if HAVE_DUNE_VTK
-    pybind11::module::import("dune.vtk");
+    if constexpr (dimension == 2) {
+      pybind11::module::import("dune.vtk");
 
-    using TrimmedWriterType
-        = Dune::VtkUnstructuredGridWriter<LeafGridView, Dune::Vtk::DiscontinuousIgaDataCollector<LeafGridView>>;
-    auto clsLeafViewWriter = insertClass<TrimmedWriterType>(module, "TrimmedVtkWriter",
-                                                            GenerateTypeName(clsLeafView.first, "TrimmedVtkWriter"));
-    if (clsLeafViewWriter.second) Dune::Vtk::registerVtkWriter<TrimmedWriterType>(module, clsLeafViewWriter.first);
-
-    clsLeafView.first.def("trimmedVtkWriter", [](const LeafGridView& self, int subSample=0) {
-      auto dataCollector = std::make_shared<Dune::Vtk::DiscontinuousIgaDataCollector<LeafGridView>>(self,subSample);
-      return new Dune::VtkUnstructuredGridWriter(dataCollector, Vtk::FormatTypes::ASCII);
-    },pybind11::arg("subSample")=0);
+      using TrimmedWriterType
+          = Dune::VtkUnstructuredGridWriter<LeafGridView, Dune::Vtk::DiscontinuousIgaDataCollector<LeafGridView>>;
+      auto clsLeafViewWriter = insertClass<TrimmedWriterType>(module, "TrimmedVtkWriter",
+                                                              GenerateTypeName(clsLeafView.first, "TrimmedVtkWriter"));
+      if (clsLeafViewWriter.second) Dune::Vtk::registerVtkWriter<TrimmedWriterType>(module, clsLeafViewWriter.first);
+
+      clsLeafView.first.def(
+          "trimmedVtkWriter",
+          [](const LeafGridView& self, int subSample = 0) {
+            auto dataCollector
+                = std::make_shared<Dune::Vtk::DiscontinuousIgaDataCollector<LeafGridView>>(self, subSample);
+            return new Dune::VtkUnstructuredGridWriter(dataCollector, Vtk::FormatTypes::ASCII);
+          },
+          pybind11::arg("subSample") = 0);
+    }
 #endif
 
     using ControlPointNetType = typename NURBSGrid::ControlPointNetType;
     using NURBSPatchDataType  = typename NURBSGrid::NURBSPatchDataType;
 
     cls.def(pybind11::init(
         [](const std::array<std::vector<double>, dimension>& knotSpans, const ControlPointNetType& controlPoints,
```

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/python/iga/nurbspatchdata.hh` & `dune-iga-0.1.6.dev20230618094642/dune/python/iga/nurbspatchdata.hh`

 * *Files 16% similar despite different names*

```diff
@@ -41,23 +41,33 @@
   void registerMultiDimensionNet(pybind11::handle scope, pybind11::class_<MultiDimensionNet, options...> cls) {
     using pybind11::operator""_a;
 
     using ValueType              = typename MultiDimensionNet::value_type;
     constexpr std::size_t netDim = MultiDimensionNet::netDim;
 
     cls.def(pybind11::init());
-    cls.def(pybind11::init(
-        [](const std::vector<std::vector<ValueType>>& values) { return new MultiDimensionNet(values); }));
+    if constexpr (netDim == 2)
+      cls.def(pybind11::init(
+          [](const std::vector<std::vector<ValueType>>& values) { return new MultiDimensionNet(values); }));
+    else if constexpr (netDim == 1)
+      cls.def(pybind11::init([](const std::vector<ValueType>& values) { return new MultiDimensionNet(values); }));
+    else if constexpr (netDim == 3)
+      cls.def(pybind11::init([](const std::vector<std::vector<std::vector<ValueType>>>& values) {
+        return new MultiDimensionNet(values);
+      }));
 
     cls.def("__len__", &MultiDimensionNet::size);
     cls.def("strideSizes", &MultiDimensionNet::strideSizes);
     cls.def("set", &MultiDimensionNet::set);
+    cls.def("directGet", [](MultiDimensionNet& self, int directIndex) { return self.directGet(directIndex); });
     cls.def("get",
             [](MultiDimensionNet& self, const std::array<int, netDim>& multIndex) { return self.get(multIndex); });
     cls.def_property_readonly_static("netDim", [](pybind11::object /* self */) { return MultiDimensionNet::netDim; });
+    cls.def_property_readonly_static("valueType",
+                                     [](pybind11::object /* self */) { return Dune::className<ValueType>(); });
   }
 
   template <class NURBSPatchData, class... options>
   void registerNurbsPatchData(pybind11::handle scope, pybind11::class_<NURBSPatchData, options...> cls) {
     using pybind11::operator""_a;
 
     using GlobalCoordinateType     = typename NURBSPatchData::GlobalCoordinateType;
```

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/python/test/poisson.py` & `dune-iga-0.1.6.dev20230618094642/dune/python/test/poisson.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/python/test/readGrid.py` & `dune-iga-0.1.6.dev20230618094642/dune/python/test/readGrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 
 from dune.iga import reader as readeriga
 from dune.iga.basis import defaultGlobalBasis, Power, Lagrange, Nurbs
 from dune.common import FieldVector
 from dune.grid import gridFunction
 
 if __name__ == "__main__":
+    # one dimensional test
+    cp = ControlPoint((0, 0, 0), 1)
+    cp2 = ControlPoint((0, 0, 3), 1)
+    netC = (((cp, cp2)))
+    net = ControlPointNet(netC)
+    nurbsPatchData = NurbsPatchData(((0, 0, 1, 1)), net, (1))
+    gridView = IGAGrid(nurbsPatchData)
     reader = (readeriga.json, "../../iga/test/auxiliaryFiles/element_trim.ibra")
     refinements = 5
     gridView = IGAGrid(reader, dimgrid=2, dimworld=2)
     gridView.hierarchicalGrid.globalRefine(refinements)
     fv = FieldVector(
         10 * [0.1]
     )  # this is here due to https://gitlab.dune-project.org/core/dune-common/-/issues/340
```

### Comparing `dune-iga-0.1.6.dev20230616150758/dune/python/test/setpath.py.in` & `dune-iga-0.1.6.dev20230618094642/dune/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/python/dune/iga/CMakeLists.txt` & `dune-iga-0.1.6.dev20230618094642/python/dune/iga/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/python/dune/iga/_boundarypatch.py` & `dune-iga-0.1.6.dev20230618094642/python/dune/iga/_boundarypatch.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/python/dune/iga/_igagrids.py` & `dune-iga-0.1.6.dev20230618094642/python/dune/iga/_igagrids.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/python/dune/iga/_nurbsAlgorithms.py` & `dune-iga-0.1.6.dev20230618094642/python/dune/iga/_nurbsAlgorithms.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/python/dune/iga/_nurbspatchdata.py` & `dune-iga-0.1.6.dev20230618094642/python/dune/iga/_nurbspatchdata.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,40 +20,57 @@
 
     return module.ControlPoint(fv, weight)
 
 
 def ControlPointNet(controlPoints):
     generator = SimpleGenerator("MultiDimensionNet", "Dune::Python")
 
-    element_type = f"Dune::IGA::MultiDimensionNet<{len(controlPoints)},{controlPoints[0][0].cppTypeName}>"
+    try:
+        controlPointType= controlPoints[0][0][0].cppTypeName
+        netDim=3
+    except:
+        try:
+            controlPointType= controlPoints[0][0].cppTypeName
+            netDim=2
+        except:
+            try:
+                controlPointType= controlPoints[0].cppTypeName
+                netDim=1
+            except:
+                raise Exception("Controlpoint type not deducable from list")
+    element_type = f"Dune::IGA::MultiDimensionNet<{netDim},{controlPointType}>"
 
     includes = []
     includes += ["dune/python/iga/nurbspatchdata.hh"]
     moduleName = "NurbsPatchData_" + hashIt(element_type)
     module = generator.load(
         includes=includes, typeName=element_type, moduleName=moduleName
     )
 
     return module.MultiDimensionNet(controlPoints)
 
 
 def NurbsPatchData(knotSpans, controlPointNet, degree):
     generator = SimpleGenerator("NurbsPatchData", "Dune::Python")
 
-    worldDim = len(controlPointNet.get((0, 0)).coords)
+    worldDim = len(controlPointNet.directGet( 0).coords)
     dim = controlPointNet.netDim
     element_type = f"Dune::IGA::NURBSPatchData<{dim},{worldDim},double>"
 
     includes = []
     includes += ["dune/python/iga/nurbspatchdata.hh"]
     moduleName = "NurbsPatchData_" + hashIt(element_type)
     module = generator.load(
         includes=includes, typeName=element_type, moduleName=moduleName
     )
 
+    if isinstance(knotSpans,tuple):
+        knotSpans= list([list(knotSpans),])
+    if isinstance(degree,int):
+        degree=(degree,)
     return module.NurbsPatchData(knotSpans, controlPointNet, degree)
 
 
 def NurbsPatchDataDefault(dim, worldDim):
     generator = SimpleGenerator("NurbsPatchData", "Dune::Python")
 
     element_type = f"Dune::IGA::NURBSPatchData<{dim},{worldDim},double>"
```

### Comparing `dune-iga-0.1.6.dev20230616150758/python/dune/iga/basis/__init__.py` & `dune-iga-0.1.6.dev20230618094642/python/dune/iga/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/python/dune_iga.egg-info/PKG-INFO` & `dune-iga-0.1.6.dev20230618094642/python/dune_iga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-iga
-Version: 0.1.6.dev20230616150758
+Version: 0.1.6.dev20230618094642
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

### Comparing `dune-iga-0.1.6.dev20230616150758/python/dune_iga.egg-info/SOURCES.txt` & `dune-iga-0.1.6.dev20230618094642/python/dune_iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/setup.py` & `dune-iga-0.1.6.dev20230618094642/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 # build _iga
 # cd /tmp/dune-iga
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/dune-iga
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-duneigaVersion = "0.1.6.dev20230616150758"
+duneigaVersion = "0.1.6.dev20230618094642"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = duneigaVersion
 
 setup(**metadata)
```

### Comparing `dune-iga-0.1.6.dev20230616150758/src/CMakeLists.txt` & `dune-iga-0.1.6.dev20230618094642/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/src/auxiliaryFiles/surface-hole.ibra` & `dune-iga-0.1.6.dev20230618094642/src/auxiliaryFiles/surface-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/src/kirchhoff_plate.cc` & `dune-iga-0.1.6.dev20230618094642/src/kirchhoff_plate.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/src/kirchhoffplate.hh` & `dune-iga-0.1.6.dev20230618094642/src/kirchhoffplate.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/src/linear2dsolid.cc` & `dune-iga-0.1.6.dev20230618094642/src/linear2dsolid.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.6.dev20230616150758/src/linearElastic.hh` & `dune-iga-0.1.6.dev20230618094642/src/linearElastic.hh`

 * *Files identical despite different names*


# Comparing `tmp/tensorboardX-2.6.tar.gz` & `tmp/tensorboardX-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorboardX-2.6.tar", last modified: Sun Feb 12 17:54:18 2023, max compression
+gzip compressed data, was "tensorboardX-2.6.1.tar", last modified: Sun Jun 18 16:42:12 2023, max compression
```

## Comparing `tensorboardX-2.6.tar` & `tensorboardX-2.6.1.tar`

### file list

```diff
@@ -1,73 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 17:54:18.579210 tensorboardX-2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-02-12 17:54:16.000000 tensorboardX-2.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-12 17:54:16.000000 tensorboardX-2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-12 17:54:16.000000 tensorboardX-2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-02-12 17:54:18.579210 tensorboardX-2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-02-12 17:54:16.000000 tensorboardX-2.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-02-12 17:54:16.000000 tensorboardX-2.6/compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-12 17:54:18.579210 tensorboardX-2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-02-12 17:54:16.000000 tensorboardX-2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 17:54:18.575210 tensorboardX-2.6/tensorboardX/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-12 17:54:18.000000 tensorboardX-2.6/tensorboardX/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 17:54:18.575210 tensorboardX-2.6/tensorboardX/beholder/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/beholder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/beholder/beholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/beholder/file_system_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/beholder/shared_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/beholder/video_writing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/caffe2_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/comet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/crc32c.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/event_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/global_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/onnx_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/openvino_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 17:54:18.579210 tensorboardX-2.6/tensorboardX/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/api.proto
--rw-r--r--   0 runner    (1001) docker     (123)    48501 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/attr_value.proto
--rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/attr_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/event.proto
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/graph.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/graph_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/layout.proto
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/layout_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/node_def.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/node_def_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/plugin_hparams.proto
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/plugin_hparams_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/plugin_mesh.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/plugin_mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/plugin_pr_curve.proto
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/plugin_pr_curve_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/plugin_text.proto
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/plugin_text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/resource_handle.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/resource_handle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/summary.proto
--rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/summary_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/tensor.proto
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/tensor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/tensor_shape.proto
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/tensor_shape_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/types.proto
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/versions.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/proto/versions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/record_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24447 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/torchvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/visdom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    52124 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-02-12 17:54:16.000000 tensorboardX-2.6/tensorboardX/x2num.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 17:54:18.575210 tensorboardX-2.6/tensorboardX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-02-12 17:54:18.000000 tensorboardX-2.6/tensorboardX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-02-12 17:54:18.000000 tensorboardX-2.6/tensorboardX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 17:54:18.000000 tensorboardX-2.6/tensorboardX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 17:54:18.000000 tensorboardX-2.6/tensorboardX.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-12 17:54:18.000000 tensorboardX-2.6/tensorboardX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-12 17:54:18.000000 tensorboardX-2.6/tensorboardX.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.525844 tensorboardX-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/ISSUE_TEMPLATE/feature-requests-or-general-questions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/workflows/build-pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-18 16:42:12.525844 tensorboardX-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/compile.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.509843 tensorboardX-2.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.505843 tensorboardX-2.6.1/docs/_static/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.509843 tensorboardX-2.6.1/docs/_static/img/tensorboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    48135 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_histogram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64086 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_hparam.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47119 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76694 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_images.png
+-rw-r--r--   0 runner    (1001) docker     (123)   571509 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_mesh.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45941 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146137 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalar_global.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99156 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/add_scalars.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160926 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/_static/img/tensorboard/hier_tags.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/tensorboard.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/tutorial_zh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/docs/utils.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/run_pytest.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.513843 tensorboardX-2.6.1/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)   490837 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/Demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/audio.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1373389 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/comet.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    65080 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/distribution.png
+-rw-r--r--   0 runner    (1001) docker     (123)   181800 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/embedding.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71618 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/graph.png
+-rw-r--r--   0 runner    (1001) docker     (123)   257734 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/histogram.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1077074 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)   119007 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/scalar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38551 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/screenshots/text.png
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-18 16:42:12.525844 tensorboardX-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.517844 tensorboardX-2.6.1/tensorboardX/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.517844 tensorboardX-2.6.1/tensorboardX/beholder/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/beholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/file_system_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/shared_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/beholder/video_writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/caffe2_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/comet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/crc32c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/event_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/global_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/onnx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/openvino_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.517844 tensorboardX-2.6.1/tensorboardX/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/api.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/attr_value.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/attr_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/event.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/graph.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/graph_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/layout.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/layout_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/node_def.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/node_def_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_hparams.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_hparams_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_mesh.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_pr_curve.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_pr_curve_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_text.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/plugin_text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/resource_handle.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/resource_handle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/summary.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/summary_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/tensor.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/tensor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/tensor_shape.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/tensor_shape_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/types.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/versions.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/proto/versions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/record_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24447 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/torchvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/visdom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52414 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tensorboardX/x2num.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.517844 tensorboardX-2.6.1/tensorboardX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 16:42:12.000000 tensorboardX-2.6.1/tensorboardX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.521844 tensorboardX-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/event_file_writer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:12.525844 tensorboardX-2.6.1/tests/expect/
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/caffe_mnist.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/caffe_overfeat.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_caffe2.test_simple_cnnmodel.expect
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_caffe2.test_simple_model.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_pr_curve.test_pr_purve.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_pr_curve.test_pr_purve_raw.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_audio.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_custom_scalars.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_float32_image.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_histogram_auto.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_histogram_doane.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_histogram_fd.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_hparams.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_hparams_bool.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_hparams_string.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_3_channel_batched.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_boxes.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_four_channel.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_four_channel_batched.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_one_channel.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_with_one_channel_batched.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_image_without_channel.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_mesh.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_text.expect
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_uint8_image.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect/test_summary.test_video.expect
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/expect_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26454 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/mnist-8.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/record_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_beholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_chainer_np.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_crc32c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_multiprocess_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_onnx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_openvino_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_pr_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_pytorch_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_pytorch_np.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_record_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_summary_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_visdom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-18 16:42:05.000000 tensorboardX-2.6.1/tests/test_writer.py
```

### Comparing `tensorboardX-2.6/HISTORY.rst` & `tensorboardX-2.6.1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 History
 =======
+2.6.1 (2023-06-18)
+-------------------
+* Expose use_strict_trace parameter in add_graph (#694)
+* Upgrade to protobuf 4
+* Fix git based package versioning
+* Fix GCS Connection Error #606 (#686)
+
 2.6 (2023-02-12)
 -------------------
 * Fixed several deprecation warnings
 * Update dependencies
 
 2.5.1 (2022-06-05)
 -------------------
```

### Comparing `tensorboardX-2.6/LICENSE` & `tensorboardX-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/PKG-INFO` & `tensorboardX-2.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorboardX
-Version: 2.6
+Version: 2.6.1
 Summary: TensorBoardX lets you watch Tensors Flow without Tensorflow
 Home-page: https://github.com/lanpa/tensorboardX
 Author: Tzu-Wei Huang
 Author-email: huang.dexter@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 
 History
 =======
+2.6.1 (2023-06-18)
+-------------------
+* Expose use_strict_trace parameter in add_graph (#694)
+* Upgrade to protobuf 4
+* Fix git based package versioning
+* Fix GCS Connection Error #606 (#686)
+
 2.6 (2023-02-12)
 -------------------
 * Fixed several deprecation warnings
 * Update dependencies
 
 2.5.1 (2022-06-05)
 -------------------
```

### Comparing `tensorboardX-2.6/README.md` & `tensorboardX-2.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # tensorboardX
 
-[![Build Status](https://travis-ci.org/lanpa/tensorboardX.svg?branch=master)](https://travis-ci.org/lanpa/tensorboardX)
 [![PyPI version](https://badge.fury.io/py/tensorboardX.svg)](https://badge.fury.io/py/tensorboardX)
 [![Documentation Status](https://readthedocs.org/projects/tensorboardx/badge/?version=latest)](https://tensorboardx.readthedocs.io/en/latest/?badge=latest)
-[![Documentation Status](https://codecov.io/gh/lanpa/tensorboardX/branch/master/graph/badge.svg)](https://codecov.io/gh/lanpa/tensorboardX/)
+[![Coverage Status](https://codecov.io/gh/lanpa/tensorboardX/branch/master/graph/badge.svg)](https://codecov.io/gh/lanpa/tensorboardX/)
 
 Write TensorBoard events with simple function call.
 
 The current release (v2.5) is tested on anaconda3, with PyTorch 1.11.0 / torchvision 0.12 / tensorboard 2.9.0.
 
 * Support `scalar`, `image`, `figure`, `histogram`, `audio`, `text`, `graph`, `onnx_graph`, `embedding`, `pr_curve`, `mesh`, `hyper-parameters`
   and `video` summaries.
@@ -98,15 +97,15 @@
 
 ## Screenshots
 
 <img src="screenshots/Demo.gif">
 
 ## Using TensorboardX with Comet
 
-TensorboardX now supports logging directly to [Comet](https://www.comet.ml/site/data-scientists/?utm_campaign=tensorboardx-integration&utm_source=github&utm_medium=readme). Comet is a **free** cloud based solution that allows you to automatically track, compare and explain your experiments. It adds a lot of functionality on top of tensorboard such as dataset management, diffing experiments, seeing the code that generated the results and more.
+TensorboardX now supports logging directly to [Comet](https://www.comet.com/site/products/ml-experiment-tracking/?utm_source=tensorboardx&utm_medium=partner&utm_campaign=partner_tensorboardx_2023). Comet is a **free** cloud based solution that allows you to automatically track, compare and explain your experiments. It adds a lot of functionality on top of tensorboard such as dataset management, diffing experiments, seeing the code that generated the results and more.
 
 This works out of the box and just require an additional line of code. See a full code example in this [Colab Notebook](https://colab.research.google.com/drive/1cTO3tgZ03nuJQ8kOjZhEiwbB-45tV4lm?usp=sharing)
 
 <p align="center">
 <img src="screenshots/comet.gif" width="750" height="400">
 </p>
```

### Comparing `tensorboardX-2.6/compile.sh` & `tensorboardX-2.6.1/compile.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/bash
 
 # Exit on error
 # set -e
 
-DESIRED_PROTO_VERSION="3.8.0"
+DESIRED_PROTO_VERSION="22.3"
 
 # call protoc direclty, if version is not the desired one, download the desired vesrion.
 
 
 if [ -f "protoc/bin/protoc" ]; then
   PROTOC_BIN="protoc/bin/protoc"
 else
```

### Comparing `tensorboardX-2.6/tensorboardX/beholder/__init__.py` & `tensorboardX-2.6.1/tensorboardX/beholder/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/beholder/beholder.py` & `tensorboardX-2.6.1/tensorboardX/beholder/beholder.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/beholder/file_system_tools.py` & `tensorboardX-2.6.1/tensorboardX/beholder/file_system_tools.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/beholder/shared_config.py` & `tensorboardX-2.6.1/tensorboardX/beholder/shared_config.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/beholder/video_writing.py` & `tensorboardX-2.6.1/tensorboardX/beholder/video_writing.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/caffe2_graph.py` & `tensorboardX-2.6.1/tensorboardX/caffe2_graph.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/comet_utils.py` & `tensorboardX-2.6.1/tensorboardX/comet_utils.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/crc32c.py` & `tensorboardX-2.6.1/tensorboardX/crc32c.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/embedding.py` & `tensorboardX-2.6.1/tensorboardX/embedding.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/event_file_writer.py` & `tensorboardX-2.6.1/tensorboardX/event_file_writer.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/global_writer.py` & `tensorboardX-2.6.1/tensorboardX/global_writer.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/onnx_graph.py` & `tensorboardX-2.6.1/tensorboardX/onnx_graph.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/openvino_graph.py` & `tensorboardX-2.6.1/tensorboardX/openvino_graph.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/api.proto` & `tensorboardX-2.6.1/tensorboardX/proto/api.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/attr_value.proto` & `tensorboardX-2.6.1/tensorboardX/proto/attr_value.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/event.proto` & `tensorboardX-2.6.1/tensorboardX/proto/event.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/graph.proto` & `tensorboardX-2.6.1/tensorboardX/proto/graph.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/layout.proto` & `tensorboardX-2.6.1/tensorboardX/proto/layout.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/node_def.proto` & `tensorboardX-2.6.1/tensorboardX/proto/node_def.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/plugin_hparams.proto` & `tensorboardX-2.6.1/tensorboardX/proto/plugin_hparams.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/plugin_mesh.proto` & `tensorboardX-2.6.1/tensorboardX/proto/plugin_mesh.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/plugin_pr_curve.proto` & `tensorboardX-2.6.1/tensorboardX/proto/plugin_pr_curve.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/plugin_text.proto` & `tensorboardX-2.6.1/tensorboardX/proto/plugin_text.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/resource_handle.proto` & `tensorboardX-2.6.1/tensorboardX/proto/resource_handle.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/summary.proto` & `tensorboardX-2.6.1/tensorboardX/proto/summary.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/tensor.proto` & `tensorboardX-2.6.1/tensorboardX/proto/tensor.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/tensor_shape.proto` & `tensorboardX-2.6.1/tensorboardX/proto/tensor_shape.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/types.proto` & `tensorboardX-2.6.1/tensorboardX/proto/types.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/proto/versions.proto` & `tensorboardX-2.6.1/tensorboardX/proto/versions.proto`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/record_writer.py` & `tensorboardX-2.6.1/tensorboardX/record_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -145,15 +145,18 @@
     def write(self, val):
         self.buffer.write(val)
 
     def flush(self):
         upload_buffer = copy.copy(self.buffer)
         upload_buffer.seek(0)
 
-        self.blob.upload_from_string(upload_buffer.getvalue())
+        # work with blob generation, so that uploading will automatically retry in case of connection errors
+        blob_generation = self.blob.generation
+        self.blob.upload_from_string(data=upload_buffer.getvalue(),
+                                     if_generation_match=blob_generation)
 
     def close(self):
         self.flush()
 
 
 class GCSRecordWriterFactory(object):
     """Factory for event protocol buffer files to Google Cloud Storage."""
```

### Comparing `tensorboardX-2.6/tensorboardX/summary.py` & `tensorboardX-2.6.1/tensorboardX/summary.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/torchvis.py` & `tensorboardX-2.6.1/tensorboardX/torchvis.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/utils.py` & `tensorboardX-2.6.1/tensorboardX/utils.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/visdom_writer.py` & `tensorboardX-2.6.1/tensorboardX/visdom_writer.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX/writer.py` & `tensorboardX-2.6.1/tensorboardX/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -919,26 +919,29 @@
         self._get_file_writer().add_openvino_graph(load_openvino_graph(xmlname))
         self._get_comet_logger().log_asset(xmlname)
 
     def add_graph(
             self,
             model,
             input_to_model=None,
-            verbose=False):
+            verbose=False,
+            use_strict_trace=True):
         """Add graph data to summary. The graph is actually processed by `torch.utils.tensorboard.add_graph()`
 
         Args:
             model (torch.nn.Module): Model to draw.
             input_to_model (torch.Tensor or list of torch.Tensor): A variable or a tuple of
                 variables to be fed.
             verbose (bool): Whether to print graph structure in console.
-
+            use_strict_trace (bool): Whether to pass keyword argument `strict` to
+                `torch.jit.trace`. Pass False when you want the tracer to
+                record your mutable container types (list, dict)
         """
         from torch.utils.tensorboard._pytorch_graph import graph
-        self._get_file_writer().add_graph(graph(model, input_to_model, verbose))
+        self._get_file_writer().add_graph(graph(model, input_to_model, verbose, use_strict_trace=use_strict_trace))
 
     @staticmethod
     def _encode(rawstr):
         # I'd use urllib but, I'm unsure about the differences from python3 to python2, etc.
         retval = rawstr
         retval = retval.replace("%", "%%%02x" % (ord("%")))
         retval = retval.replace("/", "%%%02x" % (ord("/")))
```

### Comparing `tensorboardX-2.6/tensorboardX/x2num.py` & `tensorboardX-2.6.1/tensorboardX/x2num.py`

 * *Files identical despite different names*

### Comparing `tensorboardX-2.6/tensorboardX.egg-info/PKG-INFO` & `tensorboardX-2.6.1/tensorboardX.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorboardX
-Version: 2.6
+Version: 2.6.1
 Summary: TensorBoardX lets you watch Tensors Flow without Tensorflow
 Home-page: https://github.com/lanpa/tensorboardX
 Author: Tzu-Wei Huang
 Author-email: huang.dexter@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 
 History
 =======
+2.6.1 (2023-06-18)
+-------------------
+* Expose use_strict_trace parameter in add_graph (#694)
+* Upgrade to protobuf 4
+* Fix git based package versioning
+* Fix GCS Connection Error #606 (#686)
+
 2.6 (2023-02-12)
 -------------------
 * Fixed several deprecation warnings
 * Update dependencies
 
 2.5.1 (2022-06-05)
 -------------------
```


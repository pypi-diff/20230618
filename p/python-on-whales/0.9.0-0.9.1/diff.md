# Comparing `tmp/python-on-whales-0.9.0.tar.gz` & `tmp/python-on-whales-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-on-whales-0.9.0.tar", last modified: Mon Jan  4 10:44:54 2021, max compression
+gzip compressed data, was "python-on-whales-0.9.1.tar", last modified: Tue Jan  5 09:08:20 2021, max compression
```

## Comparing `python-on-whales-0.9.0.tar` & `python-on-whales-0.9.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.864242 python-on-whales-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)       43 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    11087 2021-01-04 10:44:54.864242 python-on-whales-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     9321 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.856242 python-on-whales-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.860242 python-on-whales-0.9.0/docs/template/
--rw-r--r--   0 runner    (1001) docker     (116)     3797 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_client.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.860242 python-on-whales-0.9.0/docs/template/docker_objects/
--rw-r--r--   0 runner    (1001) docker     (116)      710 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_objects/builders.md
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_objects/configs.md
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_objects/containers.md
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_objects/images.md
--rw-r--r--   0 runner    (1001) docker     (116)     1198 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_objects/networks.md
--rw-r--r--   0 runner    (1001) docker     (116)      984 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_objects/nodes.md
--rw-r--r--   0 runner    (1001) docker     (116)     1126 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_objects/services.md
--rw-r--r--   0 runner    (1001) docker     (116)     1121 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/docker_objects/volumes.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.860242 python-on-whales-0.9.0/docs/template/sub-commands/
--rw-r--r--   0 runner    (1001) docker     (116)      934 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/sub-commands/compose.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.860242 python-on-whales-0.9.0/docs/template/user_guide/
--rw-r--r--   0 runner    (1001) docker     (116)     3833 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/user_guide/docker_run.md
--rw-r--r--   0 runner    (1001) docker     (116)     6442 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/docs/template/user_guide/generic_resources.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.860242 python-on-whales-0.9.0/python_on_whales/
--rw-r--r--   0 runner    (1001) docker     (116)      535 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7021 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/client_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     1523 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/command_line_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.864242 python-on-whales-0.9.0/python_on_whales/components/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1455 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/app.py
--rw-r--r--   0 runner    (1001) docker     (116)    19366 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/buildx.py
--rw-r--r--   0 runner    (1001) docker     (116)     3408 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/compose.py
--rw-r--r--   0 runner    (1001) docker     (116)     5176 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    64773 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/container.py
--rw-r--r--   0 runner    (1001) docker     (116)     4550 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/context.py
--rw-r--r--   0 runner    (1001) docker     (116)    16099 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/image.py
--rw-r--r--   0 runner    (1001) docker     (116)      480 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (116)     7198 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/network.py
--rw-r--r--   0 runner    (1001) docker     (116)     7235 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/node.py
--rw-r--r--   0 runner    (1001) docker     (116)     3457 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/secret.py
--rw-r--r--   0 runner    (1001) docker     (116)     7244 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     4545 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/stack.py
--rw-r--r--   0 runner    (1001) docker     (116)     4975 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/swarm.py
--rw-r--r--   0 runner    (1001) docker     (116)     7819 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/system.py
--rw-r--r--   0 runner    (1001) docker     (116)      520 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/trust.py
--rw-r--r--   0 runner    (1001) docker     (116)     9508 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/components/volume.py
--rw-r--r--   0 runner    (1001) docker     (116)     9033 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/docker_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     6141 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/download_binaries.py
--rw-r--r--   0 runner    (1001) docker     (116)      424 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     7632 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/python_on_whales/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.860242 python-on-whales-0.9.0/python_on_whales.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    11087 2021-01-04 10:44:54.000000 python-on-whales-0.9.0/python_on_whales.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1716 2021-01-04 10:44:54.000000 python-on-whales-0.9.0/python_on_whales.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-04 10:44:54.000000 python-on-whales-0.9.0/python_on_whales.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       84 2021-01-04 10:44:54.000000 python-on-whales-0.9.0/python_on_whales.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2021-01-04 10:44:54.000000 python-on-whales-0.9.0/python_on_whales.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-04 10:44:54.000000 python-on-whales-0.9.0/python_on_whales.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-04 10:44:54.864242 python-on-whales-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      815 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-04 10:44:54.864242 python-on-whales-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       26 2021-01-04 10:44:42.000000 python-on-whales-0.9.0/tests/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    11087 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     9321 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.129936 python-on-whales-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.129936 python-on-whales-0.9.1/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (116)     3797 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_client.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/docs/template/docker_objects/
+-rw-r--r--   0 runner    (1001) docker     (116)      710 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_objects/builders.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1096 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_objects/configs.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_objects/containers.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1322 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_objects/images.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1198 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_objects/networks.md
+-rw-r--r--   0 runner    (1001) docker     (116)      984 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_objects/nodes.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1126 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_objects/services.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1121 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/docker_objects/volumes.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/docs/template/sub-commands/
+-rw-r--r--   0 runner    (1001) docker     (116)      934 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/sub-commands/compose.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/docs/template/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (116)     3833 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/user_guide/docker_run.md
+-rw-r--r--   0 runner    (1001) docker     (116)     6442 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/docs/template/user_guide/generic_resources.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/python_on_whales/
+-rw-r--r--   0 runner    (1001) docker     (116)      535 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7021 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1523 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/command_line_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/python_on_whales/components/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1455 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/app.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19366 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/buildx.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3408 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/compose.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5176 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    64773 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/container.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4599 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/context.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16099 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/image.py
+-rw-r--r--   0 runner    (1001) docker     (116)      480 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7198 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/network.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7235 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/node.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3457 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/secret.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7254 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/service.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4545 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/stack.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4975 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/swarm.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7819 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/system.py
+-rw-r--r--   0 runner    (1001) docker     (116)      520 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/trust.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9508 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/components/volume.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9033 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/docker_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6141 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/download_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (116)      424 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7632 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/python_on_whales/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/python_on_whales.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    11087 2021-01-05 09:08:19.000000 python-on-whales-0.9.1/python_on_whales.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1716 2021-01-05 09:08:20.000000 python-on-whales-0.9.1/python_on_whales.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-05 09:08:19.000000 python-on-whales-0.9.1/python_on_whales.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       84 2021-01-05 09:08:19.000000 python-on-whales-0.9.1/python_on_whales.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       39 2021-01-05 09:08:19.000000 python-on-whales-0.9.1/python_on_whales.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2021-01-05 09:08:19.000000 python-on-whales-0.9.1/python_on_whales.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       39 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      815 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-05 09:08:20.133936 python-on-whales-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)       26 2021-01-05 09:08:09.000000 python-on-whales-0.9.1/tests/test-requirements.txt
```

### Comparing `python-on-whales-0.9.0/PKG-INFO` & `python-on-whales-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-on-whales
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Docker client for Python, designed to be fun and intuivive!
 Home-page: UNKNOWN
 License: MIT
 Description: <img src="https://raw.githubusercontent.com/gabrieldemarmiesse/python-on-whales/master/img/full.png" alt="logo" class="responsive" style="width: 80%; height: auto;">
         
         A Docker client for Python, designed to be fun and intuivive!
         
@@ -168,15 +168,15 @@
         | sub-command  | Function implemented  |
         |---|---|
         | app | 0/15  |
         | buildx  | 9/11 |
         | compose  | 0/24 |
         | config  | 4/4 |
         | container | 21/24 |
-        | context  | 3/8 |
+        | context  | 4/6 |
         | image  | 12/13 |
         | manifest  | 0/4 |
         | network  | 7/7 |
         | node  | 6/7 |
         | secret  | 4/4 |
         | service  | 6/9 |
         | stack  | 4/5 |
```

### Comparing `python-on-whales-0.9.0/README.md` & `python-on-whales-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 | sub-command  | Function implemented  |
 |---|---|
 | app | 0/15  |
 | buildx  | 9/11 |
 | compose  | 0/24 |
 | config  | 4/4 |
 | container | 21/24 |
-| context  | 3/8 |
+| context  | 4/6 |
 | image  | 12/13 |
 | manifest  | 0/4 |
 | network  | 7/7 |
 | node  | 6/7 |
 | secret  | 4/4 |
 | service  | 6/9 |
 | stack  | 4/5 |
```

### Comparing `python-on-whales-0.9.0/docs/template/docker_client.md` & `python-on-whales-0.9.1/docs/template/docker_client.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/docker_objects/builders.md` & `python-on-whales-0.9.1/docs/template/docker_objects/builders.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/docker_objects/configs.md` & `python-on-whales-0.9.1/docs/template/docker_objects/configs.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/docker_objects/containers.md` & `python-on-whales-0.9.1/docs/template/docker_objects/containers.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/docker_objects/images.md` & `python-on-whales-0.9.1/docs/template/docker_objects/images.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/docker_objects/networks.md` & `python-on-whales-0.9.1/docs/template/docker_objects/networks.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/docker_objects/nodes.md` & `python-on-whales-0.9.1/docs/template/docker_objects/nodes.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/docker_objects/services.md` & `python-on-whales-0.9.1/docs/template/docker_objects/services.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/docker_objects/volumes.md` & `python-on-whales-0.9.1/docs/template/docker_objects/volumes.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/sub-commands/compose.md` & `python-on-whales-0.9.1/docs/template/sub-commands/compose.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/user_guide/docker_run.md` & `python-on-whales-0.9.1/docs/template/user_guide/docker_run.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/docs/template/user_guide/generic_resources.md` & `python-on-whales-0.9.1/docs/template/user_guide/generic_resources.md`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/__init__.py` & `python-on-whales-0.9.1/python_on_whales/__init__.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/client_config.py` & `python-on-whales-0.9.1/python_on_whales/client_config.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/command_line_entrypoint.py` & `python-on-whales-0.9.1/python_on_whales/command_line_entrypoint.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/app.py` & `python-on-whales-0.9.1/python_on_whales/components/app.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/buildx.py` & `python-on-whales-0.9.1/python_on_whales/components/buildx.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/compose.py` & `python-on-whales-0.9.1/python_on_whales/components/compose.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/config.py` & `python-on-whales-0.9.1/python_on_whales/components/config.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/container.py` & `python-on-whales-0.9.1/python_on_whales/components/container.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/context.py` & `python-on-whales-0.9.1/python_on_whales/components/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,34 +98,27 @@
 
 
 class ContextCLI(DockerCLICaller):
     def create(self):
         """Not yet implemented"""
         raise NotImplementedError
 
-    def export(self):
-        """Not yet implemented"""
-        raise NotImplementedError
-
-    def import_(self):
-        """Not yet implemented"""
-        raise NotImplementedError
-
     @overload
     def inspect(self, x: Union[None, str]) -> Context:
         ...
 
     @overload
     def inspect(self, x: List[str]) -> List[Context]:
         ...
 
     def inspect(
         self, x: Union[None, str, List[str]] = None
     ) -> Union[Context, List[Context]]:
-        """Not yet implemented"""
+        """Returns the context object. If no argument is provided, returns the
+        current context."""
         if isinstance(x, str) or x is None:
             return Context(self.client_config, x)
         else:
             return [Context(self.client_config, ref) for ref in x]
 
     def list(self) -> List[Context]:
         """List all Docker contexts available
@@ -151,10 +144,15 @@
         full_cmd += to_list(x)
         run(full_cmd)
 
     def update(self):
         """Not yet implemented"""
         raise NotImplementedError
 
-    def use(self):
-        """Not yet implemented"""
-        raise NotImplementedError
+    def use(self, context: ValidContext):
+        """Set the default context
+
+        # Arguments
+            context: The context to set as default
+        """
+        full_cmd = self.docker_cmd + ["context", "use", context]
+        run(full_cmd)
```

### Comparing `python-on-whales-0.9.0/python_on_whales/components/image.py` & `python-on-whales-0.9.1/python_on_whales/components/image.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/network.py` & `python-on-whales-0.9.1/python_on_whales/components/network.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/node.py` & `python-on-whales-0.9.1/python_on_whales/components/node.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/secret.py` & `python-on-whales-0.9.1/python_on_whales/components/secret.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/service.py` & `python-on-whales-0.9.1/python_on_whales/components/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     ports: Optional[List[EndpointPortConfig]]
     virtual_ips: Optional[List[VirtualIP]]
 
 
 class ServiceUpdateStatus(DockerCamelModel):
     state: str
     started_at: str
-    completed_at: str
+    completed_at: Optional[str]
     message: str
 
 
 class ServiceInspectResult(DockerCamelModel):
     id: str = Field(alias="ID")
     version: ServiceVersion
     created_at: datetime
```

### Comparing `python-on-whales-0.9.0/python_on_whales/components/stack.py` & `python-on-whales-0.9.1/python_on_whales/components/stack.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/swarm.py` & `python-on-whales-0.9.1/python_on_whales/components/swarm.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/system.py` & `python-on-whales-0.9.1/python_on_whales/components/system.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/trust.py` & `python-on-whales-0.9.1/python_on_whales/components/trust.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/components/volume.py` & `python-on-whales-0.9.1/python_on_whales/components/volume.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/docker_client.py` & `python-on-whales-0.9.1/python_on_whales/docker_client.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/download_binaries.py` & `python-on-whales-0.9.1/python_on_whales/download_binaries.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales/utils.py` & `python-on-whales-0.9.1/python_on_whales/utils.py`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/python_on_whales.egg-info/PKG-INFO` & `python-on-whales-0.9.1/python_on_whales.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-on-whales
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Docker client for Python, designed to be fun and intuivive!
 Home-page: UNKNOWN
 License: MIT
 Description: <img src="https://raw.githubusercontent.com/gabrieldemarmiesse/python-on-whales/master/img/full.png" alt="logo" class="responsive" style="width: 80%; height: auto;">
         
         A Docker client for Python, designed to be fun and intuivive!
         
@@ -168,15 +168,15 @@
         | sub-command  | Function implemented  |
         |---|---|
         | app | 0/15  |
         | buildx  | 9/11 |
         | compose  | 0/24 |
         | config  | 4/4 |
         | container | 21/24 |
-        | context  | 3/8 |
+        | context  | 4/6 |
         | image  | 12/13 |
         | manifest  | 0/4 |
         | network  | 7/7 |
         | node  | 6/7 |
         | secret  | 4/4 |
         | service  | 6/9 |
         | stack  | 4/5 |
```

### Comparing `python-on-whales-0.9.0/python_on_whales.egg-info/SOURCES.txt` & `python-on-whales-0.9.1/python_on_whales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-on-whales-0.9.0/setup.py` & `python-on-whales-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def get_long_description() -> str:
     return (CURRENT_DIR / "README.md").read_text(encoding="utf8")
 
 
 setup(
     name="python-on-whales",
-    version="0.9.0",
+    version="0.9.1",
     description="A Docker client for Python, designed to be fun and intuivive!",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     install_requires=(CURRENT_DIR / "requirements.txt").read_text().splitlines(),
     packages=find_packages(),
     include_package_data=True,  # will read the MANIFEST.in
     license="MIT",
```


# Comparing `tmp/compas_ui-0.9.1.tar.gz` & `tmp/compas_ui-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_ui-0.9.1.tar", last modified: Thu Dec  1 20:16:47 2022, max compression
+gzip compressed data, was "compas_ui-0.9.3.tar", last modified: Sun Jun 18 20:07:56 2023, max compression
```

## Comparing `compas_ui-0.9.1.tar` & `compas_ui-0.9.3.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.762864 compas_ui-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2022-12-01 20:16:22.000000 compas_ui-0.9.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (122)     3806 2022-12-01 20:16:22.000000 compas_ui-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-12-01 20:16:22.000000 compas_ui-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      407 2022-12-01 20:16:22.000000 compas_ui-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2022-12-01 20:16:47.762864 compas_ui-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-12-01 20:16:22.000000 compas_ui-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      677 2022-12-01 20:16:22.000000 compas_ui-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-12-01 20:16:22.000000 compas_ui-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      207 2022-12-01 20:16:47.762864 compas_ui-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2022-12-01 20:16:22.000000 compas_ui-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.742863 compas_ui-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.746863 compas_ui-0.9.1/src/compas_ui/
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.746863 compas_ui-0.9.1/src/compas_ui/artists/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/artists/curveartist.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/artists/meshartist.py
--rw-r--r--   0 runner    (1001) docker     (122)      474 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/artists/primitiveartist.py
--rw-r--r--   0 runner    (1001) docker     (122)     9113 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.750863 compas_ui-0.9.1/src/compas_ui/objects/
--rw-r--r--   0 runner    (1001) docker     (122)     1066 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/curveobject.py
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/groupobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/lineobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/meshobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     4213 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/networkobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     5675 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/object.py
--rw-r--r--   0 runner    (1001) docker     (122)     4832 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/objects/volmeshobject.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.750863 compas_ui-0.9.1/src/compas_ui/rhino/
--rw-r--r--   0 runner    (1001) docker     (122)      300 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.750863 compas_ui-0.9.1/src/compas_ui/rhino/artists/
--rw-r--r--   0 runner    (1001) docker     (122)      750 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/artists/curveartist.py
--rw-r--r--   0 runner    (1001) docker     (122)      258 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/artists/lineartist.py
--rw-r--r--   0 runner    (1001) docker     (122)      272 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/artists/meshartist.py
--rw-r--r--   0 runner    (1001) docker     (122)      195 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1200 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/command.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.754863 compas_ui-0.9.1/src/compas_ui/rhino/forms/
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      843 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/about.py
--rw-r--r--   0 runner    (1001) docker     (122)     2924 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/attributes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/conda.py
--rw-r--r--   0 runner    (1001) docker     (122)     7654 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/defaultattributes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2990 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     1341 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     9655 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/meshdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     8140 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/scene.py
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/searchpaths.py
--rw-r--r--   0 runner    (1001) docker     (122)     7225 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1121 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/splash.py
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/forms/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     5027 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/install_plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)      879 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/mouse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.754863 compas_ui-0.9.1/src/compas_ui/rhino/objects/
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15975 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/objects/_modify.py
--rw-r--r--   0 runner    (1001) docker     (122)     3521 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/objects/curveobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     3458 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/objects/lineobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    14395 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/objects/meshobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/objects/networkobject.py
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/objects/object.py
--rw-r--r--   0 runner    (1001) docker     (122)     9441 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/objects/volmeshobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    13876 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/rui.py
--rw-r--r--   0 runner    (1001) docker     (122)      893 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.742863 compas_ui-0.9.1/src/compas_ui/rhino/ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.742863 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.754863 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS__toolbar_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      205 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_cloud_restart_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      207 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_cloud_shutdown_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_cloud_start_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      499 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_conda_envs_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      203 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_load_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      229 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_mesh_create_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      187 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_redo_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      187 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_save_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      191 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_saveas_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      448 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_scene_clear_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      205 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_scene_objects_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      203 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_scene_update_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_searchpaths_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      338 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_settings_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      187 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_undo_cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/__plugin__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.758864 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/
--rw-r--r--   0 runner    (1001) docker     (122)   827523 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-restart.png
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-shutdown.png
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-start.png
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_environments.png
--rw-r--r--   0 runner    (1001) docker     (122)     2267 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_init.png
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_load.png
--rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_redo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_save.png
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-clear.png
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-objects.png
--rw-r--r--   0 runner    (1001) docker     (122)     1659 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-settings.png
--rw-r--r--   0 runner    (1001) docker     (122)      562 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-update.png
--rw-r--r--   0 runner    (1001) docker     (122)    11134 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_settings.png
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_ui-14.png
--rw-r--r--   0 runner    (1001) docker     (122)    14927 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_ui.png
--rw-r--r--   0 runner    (1001) docker     (122)      502 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_undo.png
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      906 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1128 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (122)      463 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/config.json
--rw-r--r--   0 runner    (1001) docker     (122)      207 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/rui.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/ui.json
--rw-r--r--   0 runner    (1001) docker     (122)     5350 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/scene.py
--rw-r--r--   0 runner    (1001) docker     (122)     6383 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/session.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.758864 compas_ui-0.9.1/src/compas_ui/singleton/
--rw-r--r--   0 runner    (1001) docker     (122)      460 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/singleton/meta.py
--rw-r--r--   0 runner    (1001) docker     (122)       95 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/singleton/singleton_ipy.py
--rw-r--r--   0 runner    (1001) docker     (122)       95 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/singleton/singleton_py3.py
--rw-r--r--   0 runner    (1001) docker     (122)    12492 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.762864 compas_ui-0.9.1/src/compas_ui/values/
--rw-r--r--   0 runner    (1001) docker     (122)      413 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/boolvalue.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/colorvalue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1442 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/dictvalue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1510 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/floatvalue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/intvalue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/listvalue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1429 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      166 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/strvalue.py
--rw-r--r--   0 runner    (1001) docker     (122)     2264 2022-12-01 20:16:22.000000 compas_ui-0.9.1/src/compas_ui/values/value.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:16:47.746863 compas_ui-0.9.1/src/compas_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2022-12-01 20:16:47.000000 compas_ui-0.9.1/src/compas_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5012 2022-12-01 20:16:47.000000 compas_ui-0.9.1/src/compas_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:16:47.000000 compas_ui-0.9.1/src/compas_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:16:47.000000 compas_ui-0.9.1/src/compas_ui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2022-12-01 20:16:47.000000 compas_ui-0.9.1/src/compas_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-12-01 20:16:47.000000 compas_ui-0.9.1/src/compas_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.100868 compas_ui-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-18 20:07:37.000000 compas_ui-0.9.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-18 20:07:37.000000 compas_ui-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 20:07:37.000000 compas_ui-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-18 20:07:37.000000 compas_ui-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 20:07:56.100868 compas_ui-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-18 20:07:37.000000 compas_ui-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-18 20:07:37.000000 compas_ui-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 20:07:37.000000 compas_ui-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-18 20:07:56.100868 compas_ui-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-18 20:07:37.000000 compas_ui-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.080868 compas_ui-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.084868 compas_ui-0.9.3/src/compas_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.084868 compas_ui-0.9.3/src/compas_ui/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/artists/curveartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/artists/meshartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/artists/primitiveartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.088868 compas_ui-0.9.3/src/compas_ui/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/curveobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/groupobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/lineobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/meshobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/networkobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/objects/volmeshobject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.088868 compas_ui-0.9.3/src/compas_ui/rhino/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.088868 compas_ui-0.9.3/src/compas_ui/rhino/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/artists/curveartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/artists/lineartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/artists/meshartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.092868 compas_ui-0.9.3/src/compas_ui/rhino/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/defaultattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/meshdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/searchpaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/splash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/forms/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/install_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/mouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.092868 compas_ui-0.9.3/src/compas_ui/rhino/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/objects/_modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/objects/curveobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/objects/lineobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/objects/meshobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/objects/networkobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/objects/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/objects/volmeshobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/rui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.080868 compas_ui-0.9.3/src/compas_ui/rhino/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.080868 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.096868 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS__toolbar_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_cloud_restart_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_cloud_shutdown_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_cloud_start_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_conda_envs_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_load_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_mesh_create_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_redo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_save_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_saveas_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_scene_clear_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_scene_objects_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_scene_update_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_searchpaths_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_settings_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS_undo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/__plugin__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.100868 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   827523 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-restart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-shutdown.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-start.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_environments.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_load.png
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_redo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_save.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-clear.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-update.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_ui-14.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_ui.png
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/rui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.100868 compas_ui-0.9.3/src/compas_ui/singleton/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/singleton/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/singleton/singleton_ipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/singleton/singleton_py3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.100868 compas_ui-0.9.3/src/compas_ui/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/boolvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/colorvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/dictvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/floatvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/intvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/listvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/strvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-18 20:07:37.000000 compas_ui-0.9.3/src/compas_ui/values/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:07:56.084868 compas_ui-0.9.3/src/compas_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-18 20:07:56.000000 compas_ui-0.9.3/src/compas_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-18 20:07:56.000000 compas_ui-0.9.3/src/compas_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:07:56.000000 compas_ui-0.9.3/src/compas_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:07:56.000000 compas_ui-0.9.3/src/compas_ui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 20:07:56.000000 compas_ui-0.9.3/src/compas_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 20:07:56.000000 compas_ui-0.9.3/src/compas_ui.egg-info/top_level.txt
```

### Comparing `compas_ui-0.9.1/CHANGELOG.md` & `compas_ui-0.9.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,156 +1,169 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.9.1] 2022-12-01
+## Unreleased
 
 ### Added
 
 ### Changed
 
 ### Removed
 
 
-## [0.9.0] 2022-12-01
+## [0.9.3] 2023-06-18
 
 ### Added
 
 ### Changed
 
 ### Removed
 
 
-## [0.8.4] 2022-11-18
+## [0.9.2] 2023-06-18
 
 ### Added
 
 ### Changed
 
+- Fixed a scene object form bug.
+
 ### Removed
 
+## [0.9.1] 2022-12-01
 
-## [0.8.3] 2022-11-17
+### Added
+
+### Changed
+
+### Removed
+
+## [0.9.0] 2022-12-01
 
 ### Added
 
 ### Changed
 
 ### Removed
 
+## [0.8.4] 2022-11-18
+
+### Added
 
-## [0.8.2] 2022-11-17
+### Changed
+
+### Removed
+
+## [0.8.3] 2022-11-17
 
 ### Added
 
 ### Changed
 
 ### Removed
 
+## [0.8.2] 2022-11-17
+
+### Added
+
+### Changed
+
+### Removed
 
 ## [0.8.1] 2022-11-17
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.8.0] 2022-11-17
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.7.1] 2022-11-09
 
 ### Added
 
 * Added `compas_ui.rhino.install.after_rhino_install`.
 
 ### Changed
 
 ### Removed
 
 * Removed `compas_ui.rhino.install.main`.
 
-
 ## [0.7.0] 2022-10-25
 
 ### Added
 
 ### Changed
 
 * Use `black` as formatter.
 * Updated all github workflows to v2
 
 ### Removed
 
-
 ## [0.6.2] 2022-09-24
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.6.1] 2022-09-23
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.6.0] 2022-09-23
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.5.3] 2022-09-23
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.5.2] 2022-09-23
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.5.1] 2022-09-22
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.5.0] 2022-09-21
 
 ### Added
 
 * Added `compas_ui.rhino.forms.AboutForm`.
 * Added `compas_ui.rhino.forms.CondaEnvsForm`.
 * Added `compas_ui.rhino.forms.FileForm`.
@@ -168,29 +181,27 @@
 ### Changed
 
 * Change on `SceneObjectsForm` is reflected realtime.
 * Locked `sphinx` to `4.5`
 
 ### Removed
 
-
 ## [0.4.1] 2022-03-23
 
 ### Added
 
 * Added `App.pick_file_save` and `App.pick_file_open`.
 
 ### Changed
 
 * Use `TreeView` and `CustomCell` for `SettingsForm`.
 * Changed clien size of browser form.
 
 ### Removed
 
-
 ## [0.4.0] 2022-03-22
 
 ### Added
 
 * `SingletonMetaClass` for Python 3+.
 * `SingletonMetaClass` for IronPython 2.7.
 * `App` singleton as main entry point.
@@ -211,25 +222,22 @@
 * `RhinoNetworkObject` as plugin for `NetworkObject` in the Rhino context.
 * `RhinoVolMeshObject` as plugin for `VolMeshObject` in the Rhino context.
 
 ### Changed
 
 ### Removed
 
-
 ## [0.3.0] 2022-02-25
 
 ### Added
 
 ### Changed
 
 ### Removed
 
-
 ## [0.2.0] 2022-02-25
 
 ### Added
 
 ### Changed
 
 ### Removed
-
```

### Comparing `compas_ui-0.9.1/LICENSE` & `compas_ui-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/PKG-INFO` & `compas_ui-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_ui
-Version: 0.9.1
+Version: 0.9.3
 Summary: COMPAS UI provides basic functionality to build a user interface for a COMPAS app.
 Home-page: https://github.com/blockresearchgroup/compas_ui
 Author: tom van mele
 Author-email: van.mele@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_ui-0.9.1/pyproject.toml` & `compas_ui-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/setup.py` & `compas_ui-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,24 @@
 from setuptools import setup
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 def read(*names, **kwargs):
-    return io.open(
-        path.join(here, *names), encoding=kwargs.get("encoding", "utf8")
-    ).read()
+    return io.open(path.join(here, *names), encoding=kwargs.get("encoding", "utf8")).read()
 
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="compas_ui",
-    version="0.9.1",
+    version="0.9.3",
     description="COMPAS UI provides basic functionality to build a user interface for a COMPAS app.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/blockresearchgroup/compas_ui",
     author="tom van mele",
     author_email="van.mele@arch.ethz.ch",
     license="MIT license",
```

### Comparing `compas_ui-0.9.1/src/compas_ui/__init__.py` & `compas_ui-0.9.3/src/compas_ui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import os
 
 
 __author__ = ["tom van mele"]
 __copyright__ = "ETH Zurich - Block Research Group"
 __license__ = "MIT License"
 __email__ = "van.mele@arch.ethz.ch"
-__version__ = "0.9.1"
+__version__ = "0.9.3"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `compas_ui-0.9.1/src/compas_ui/artists/meshartist.py` & `compas_ui-0.9.3/src/compas_ui/artists/meshartist.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/controller.py` & `compas_ui-0.9.3/src/compas_ui/controller.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/objects/__init__.py` & `compas_ui-0.9.3/src/compas_ui/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/objects/curveobject.py` & `compas_ui-0.9.3/src/compas_ui/objects/curveobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import uuid
 from .object import Object
 from compas_ui.values import Settings
 
 
 class CurveObject(Object):
-
     SETTINGS = Settings()
 
     def __init__(self, *args, **kwargs):
         super(CurveObject, self).__init__(*args, **kwargs)
 
     @property
     def state(self):
```

### Comparing `compas_ui-0.9.1/src/compas_ui/objects/groupobject.py` & `compas_ui-0.9.3/src/compas_ui/objects/groupobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/objects/lineobject.py` & `compas_ui-0.9.3/src/compas_ui/objects/lineobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import uuid
 from .object import Object
 from compas_ui.values import Settings
 
 
 class LineObject(Object):
-
     SETTINGS = Settings()
 
     def __init__(self, *args, **kwargs):
         super(LineObject, self).__init__(*args, **kwargs)
 
     @property
     def state(self):
```

### Comparing `compas_ui-0.9.1/src/compas_ui/objects/meshobject.py` & `compas_ui-0.9.3/src/compas_ui/objects/meshobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/objects/networkobject.py` & `compas_ui-0.9.3/src/compas_ui/objects/networkobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/objects/object.py` & `compas_ui-0.9.3/src/compas_ui/objects/object.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/objects/volmeshobject.py` & `compas_ui-0.9.3/src/compas_ui/objects/volmeshobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/artists/__init__.py` & `compas_ui-0.9.3/src/compas_ui/rhino/artists/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/command.py` & `compas_ui-0.9.3/src/compas_ui/rhino/command.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/__init__.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/about.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/about.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/attributes.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/attributes.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/conda.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/conda.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/defaultattributes.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/defaultattributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import Rhino.UI
 import Eto.Drawing
 import Eto.Forms
 
 
 class AddDefaultAttributeForm(Eto.Forms.Dialog[bool]):
     def __init__(self, width=300, height=140):
-
         self.Title = "Add Default Attribute"
         self.Padding = Eto.Drawing.Padding(0)
         self.Resizable = True
         self.MinimumSize = Eto.Drawing.Size(0.5 * width, 0.5 * height)
         self.ClientSize = Eto.Drawing.Size(width, height)
 
         layout = Eto.Forms.DynamicLayout()
@@ -77,15 +76,14 @@
             "default_vertex_attributes",
             "default_edge_attributes",
             "default_face_attributes",
         ],
         width=500,
         height=500,
     ):
-
         self.Title = title
         self.Padding = Eto.Drawing.Padding(0)
         self.Resizable = True
         self.MinimumSize = Eto.Drawing.Size(0.5 * width, 0.5 * height)
         self.ClientSize = Eto.Drawing.Size(width, height)
         self.item = item
         self.default_attributes_names = default_attributes_names
@@ -217,15 +215,14 @@
                 self.table.ReloadData()
 
     def show(self):
         return self.ShowModal(Rhino.UI.RhinoEtoApp.MainWindow)
 
 
 if __name__ == "__main__":
-
     from compas.datastructures import Mesh
     import compas
 
     mesh = Mesh.from_obj(compas.get("faces.obj"))
 
     form = DefaultAttributesForm(mesh)
     form.show()
```

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/error.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/error.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/filesystem.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/filesystem.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/info.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/info.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/meshdata.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/meshdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         title="Mesh Data",
         width=800,
         height=800,
         excluded_vertex_attr=None,
         excluded_edge_attr=None,
         excluded_face_attr=None,
     ):
-
         self.mesh = mesh
         self.excluded_vertex_attr = excluded_vertex_attr
         self.excluded_edge_attr = excluded_edge_attr
         self.excluded_face_attr = excluded_face_attr
 
         self.Title = title
         self.Padding = Eto.Drawing.Padding(0)
```

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/scene.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/scene.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/searchpaths.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/searchpaths.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/settings.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,22 @@
 
 class CustomCell(Eto.Forms.CustomCell):
     def OnGetIdentifier(self, args):
         return str(args.Item.GetValue(0))
 
     def OnCreateCell(self, args):
         item = args.Item
+
+        if item is None:
+            return Eto.Forms.Label()
+
         value = item.GetValue(1)
         valueobj = item.GetValue(2)
 
         if isinstance(valueobj, Value):
-
             if valueobj.value_type == bool:
                 control = Eto.Forms.CheckBox()
                 control.Checked = value
 
                 def on_checked(sender, e):
                     item.SetValue(1, control.Checked)
 
@@ -71,27 +74,26 @@
                 def on_value_changed(sender, e):
                     color = Eto.Drawing.Color(control.Value)
                     item.SetValue(1, Color(color.R, color.G, color.B))
 
                 control.ValueChanged += on_value_changed
 
             else:
-                control = Eto.Forms.Label(str(valueobj))
+                control = Eto.Forms.Label(Text=str(valueobj))
 
         else:
             control = Eto.Forms.Label()
 
         control.Size = Eto.Drawing.Size(100, 25)
 
         return control
 
 
 class SettingsForm(Eto.Forms.Dialog[bool]):
     def __init__(self, settings, title="Settings", width=500, height=500, use_tab=False):
-
         self._names = None
         self._values = None
         self.settings = settings
         self.use_tab = use_tab
 
         self.Title = title
         self.Padding = Eto.Drawing.Padding(0)
```

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/splash.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/splash.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import Rhino.UI
 import Eto.Drawing
 import Eto.Forms
 
 
 class SplashForm(Eto.Forms.Dialog[bool]):
     def __init__(self, title, url, width=800, height=450):
-
         self.Title = title
         self.Padding = Eto.Drawing.Padding(0)
         self.Resizable = False
         self.ClientSize = Eto.Drawing.Size(width, height)
         self.WindowStyle = getattr(Eto.Forms.WindowStyle, "None")
 
         webview = Eto.Forms.WebView()
```

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/forms/toolbar.py` & `compas_ui-0.9.3/src/compas_ui/rhino/forms/toolbar.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/install.py` & `compas_ui-0.9.3/src/compas_ui/rhino/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,10 +39,9 @@
 
 @plugin(category="install", tryfirst=True)
 def installable_rhino_packages():
     return ["compas_ui"]
 
 
 if __name__ == "__main__":
-
     print("This installation procedure is deprecated.")
     print("Use `python -m compas_rhino.install` instead.")
```

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/install_plugin.py` & `compas_ui-0.9.3/src/compas_ui/rhino/install_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 def get_version_from_args():
     args = compas_rhino.INSTALLATION_ARGUMENTS
     return compas_rhino._check_rhino_version(args.version)
 
 
 def get_package_plugins(package_name):
-
     plugin_paths = []
 
     package = import_module(package_name)
     package_dir = os.path.dirname(package.__file__)
     package_plugins_path = os.path.join(package_dir, "rhino", "ui")
     if os.path.exists(package_plugins_path):
         for plugin_name in os.listdir(package_plugins_path):
@@ -104,15 +103,14 @@
             print("PlugIn {} RUI file generation failed.".format(plugin_name))
             print(e)
 
     return "python plugin {} installed".format(plugin_fullname)
 
 
 def clean_up(plugins):
-
     version = get_version_from_args()
 
     # Clean up the plugin directory
     symlinks_to_remove = []
     python_plugins_path = compas_rhino._get_rhino_pythonplugins_path(version)
     if not os.path.exists(python_plugins_path):
         os.mkdir(python_plugins_path)
```

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/mouse.py` & `compas_ui-0.9.3/src/compas_ui/rhino/mouse.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/objects/__init__.py` & `compas_ui-0.9.3/src/compas_ui/rhino/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/objects/_modify.py` & `compas_ui-0.9.3/src/compas_ui/rhino/objects/_modify.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/objects/curveobject.py` & `compas_ui-0.9.3/src/compas_ui/rhino/objects/curveobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/objects/lineobject.py` & `compas_ui-0.9.3/src/compas_ui/rhino/objects/lineobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/objects/meshobject.py` & `compas_ui-0.9.3/src/compas_ui/rhino/objects/meshobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/objects/networkobject.py` & `compas_ui-0.9.3/src/compas_ui/rhino/objects/networkobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/objects/object.py` & `compas_ui-0.9.3/src/compas_ui/rhino/objects/object.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/objects/volmeshobject.py` & `compas_ui-0.9.3/src/compas_ui/rhino/objects/volmeshobject.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/rui.py` & `compas_ui-0.9.3/src/compas_ui/rhino/rui.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,14 @@
         guid = uuid.uuid4()
         s_item = TPL_TOOLBARGROUPITEM.format(guid, tb_name, tb_guid)
         e_item = ET.fromstring(s_item)
         root.append(e_item)
 
 
 if __name__ == "__main__":
-
     import argparse
 
     parser = argparse.ArgumentParser(description="COMPAS Rhino UI compiler.")
 
     parser.add_argument("ipath", help="Path to the config file (input).")
     parser.add_argument("opath", help="Path to the rui file (output).")
```

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/scene.py` & `compas_ui-0.9.3/src/compas_ui/rhino/scene.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS__toolbar_cmd.py` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/COMPAS__toolbar_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 
 HERE = os.path.dirname(__file__)
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()  # noqa: F841
 
     config = [
         {
             "command": "COMPAS_load",
             "icon": os.path.join(HERE, "assets", "COMPAS_load.png"),
         },
```

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS.jpg` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS.jpg`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-restart.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-restart.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-shutdown.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-shutdown.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-start.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_cloud-start.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_environments.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_environments.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_init.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_init.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_load.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_load.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_save.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_save.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-clear.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-clear.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-objects.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-objects.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-settings.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-settings.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-update.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_scene-update.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_settings.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_settings.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_ui-14.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_ui-14.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_ui.png` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/COMPAS_ui.png`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/favicon.ico` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/index.html` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/index.html`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/assets/styles.css` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/assets/styles.css`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/rhino/ui/COMPAS/dev/ui.json` & `compas_ui-0.9.3/src/compas_ui/rhino/ui/COMPAS/dev/ui.json`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/scene.py` & `compas_ui-0.9.3/src/compas_ui/scene.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/session.py` & `compas_ui-0.9.3/src/compas_ui/session.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/ui.py` & `compas_ui-0.9.3/src/compas_ui/ui.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/values/colorvalue.py` & `compas_ui-0.9.3/src/compas_ui/values/colorvalue.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/values/dictvalue.py` & `compas_ui-0.9.3/src/compas_ui/values/dictvalue.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/values/floatvalue.py` & `compas_ui-0.9.3/src/compas_ui/values/floatvalue.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/values/intvalue.py` & `compas_ui-0.9.3/src/compas_ui/values/intvalue.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/values/listvalue.py` & `compas_ui-0.9.3/src/compas_ui/values/listvalue.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/values/settings.py` & `compas_ui-0.9.3/src/compas_ui/values/settings.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui/values/value.py` & `compas_ui-0.9.3/src/compas_ui/values/value.py`

 * *Files identical despite different names*

### Comparing `compas_ui-0.9.1/src/compas_ui.egg-info/PKG-INFO` & `compas_ui-0.9.3/src/compas_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas-ui
-Version: 0.9.1
+Version: 0.9.3
 Summary: COMPAS UI provides basic functionality to build a user interface for a COMPAS app.
 Home-page: https://github.com/blockresearchgroup/compas_ui
 Author: tom van mele
 Author-email: van.mele@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_ui-0.9.1/src/compas_ui.egg-info/SOURCES.txt` & `compas_ui-0.9.3/src/compas_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*


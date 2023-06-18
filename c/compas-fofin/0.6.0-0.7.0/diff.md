# Comparing `tmp/compas_fofin-0.6.0.tar.gz` & `tmp/compas_fofin-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_fofin-0.6.0.tar", last modified: Wed Nov  9 22:44:51 2022, max compression
+gzip compressed data, was "compas_fofin-0.7.0.tar", last modified: Sun Jun 18 20:10:17 2023, max compression
```

## Comparing `compas_fofin-0.6.0.tar` & `compas_fofin-0.7.0.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.549471 compas_fofin-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-11-09 22:44:51.549471 compas_fofin-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-11-09 22:44:51.549471 compas_fofin-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.541471 compas_fofin-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.541471 compas_fofin-0.6.0/src/compas_fofin/
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin/artists/
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/artists/cablemeshartist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/artists/constraintartist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin/datastructures/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/datastructures/cablemesh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin/objects/
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3106 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/objects/cablemeshobject.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/objects/circleconstraintobject.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/objects/constraintobject.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/objects/curveconstraintobject.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/objects/lineconstraintobject.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin/rhino/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin/rhino/artists/
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5066 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/artists/cablemeshartist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/artists/circleconstraintartist.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/artists/curveconstraintartist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/artists/lineconstraintartist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin/rhino/conduits/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/conduits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6565 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/conduits/cablemeshconduit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin/rhino/conversions/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/conversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/conversions/curves.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/install.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin/rhino/objects/
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21017 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/objects/cablemeshobject.py
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/objects/circleconstraintobject.py
--rw-r--r--   0 runner    (1001) docker     (121)     3712 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/objects/curveconstraintobject.py
--rw-r--r--   0 runner    (1001) docker     (121)     3691 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/objects/lineconstraintobject.py
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/register.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.541471 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.541471 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.549471 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF__toolbar_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_anchors_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_constraints_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_edges_delete_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_box_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_cylinder_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_mesh_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_meshgrid_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_surface_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_edges_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_nodes_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_nodes_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3681 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_scale_q_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_solve_fd_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_update_constraints_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_toolbar_cablemesh_create_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__plugin__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.549471 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_cablemesh_constrain_nodes_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_cablemesh_unconstrain_nodes_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_toolbar_load_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_toolbar_save_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4317 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/_FF_cablemesh_scale_q_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_load_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_save_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_solve_dr_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_constraint_add_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.549471 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/
--rw-r--r--   0 runner    (1001) docker     (121)   668934 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF.png
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_anchors.png
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_constrain_nodes.png
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_create.png
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_edges_delete.png
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_modify_edges.png
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_modify_nodes.png
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_move_nodes.png
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_scale_q.png
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_solve_fd.png
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_update_constraints.png
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_ui.png
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/config.json
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/rui.py
--rw-r--r--   0 runner    (1001) docker     (121)     6796 2022-11-09 22:44:37.000000 compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/ui.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 22:44:51.545471 compas_fofin-0.6.0/src/compas_fofin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-11-09 22:44:51.000000 compas_fofin-0.6.0/src/compas_fofin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4639 2022-11-09 22:44:51.000000 compas_fofin-0.6.0/src/compas_fofin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 22:44:51.000000 compas_fofin-0.6.0/src/compas_fofin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 22:44:51.000000 compas_fofin-0.6.0/src/compas_fofin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-09 22:44:51.000000 compas_fofin-0.6.0/src/compas_fofin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-09 22:44:51.000000 compas_fofin-0.6.0/src/compas_fofin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.951169 compas_fofin-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-18 20:10:17.951169 compas_fofin-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-18 20:10:17.955169 compas_fofin-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.943169 compas_fofin-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.943169 compas_fofin-0.7.0/src/compas_fofin/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/artists/cablemeshartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/artists/constraintartist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/datastructures/cablemesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/objects/cablemeshobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/objects/circleconstraintobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/objects/constraintobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/objects/curveconstraintobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/objects/lineconstraintobject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin/rhino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin/rhino/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/artists/cablemeshartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/artists/circleconstraintartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/artists/curveconstraintartist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/artists/lineconstraintartist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin/rhino/conduits/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/conduits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/conduits/cablemeshconduit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin/rhino/conversions/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/conversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/conversions/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin/rhino/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20929 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/objects/cablemeshobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/objects/circleconstraintobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/objects/curveconstraintobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/objects/lineconstraintobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.943169 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.943169 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.951169 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF__toolbar_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_anchors_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_constraints_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_edges_delete_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_box_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_cylinder_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_mesh_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_meshgrid_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_surface_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_edges_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_nodes_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_nodes_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_scale_q_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_solve_fd_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_update_constraints_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_toolbar_cablemesh_create_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__plugin__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.951169 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_cablemesh_constrain_nodes_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_cablemesh_unconstrain_nodes_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_toolbar_load_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_toolbar_save_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/_FF_cablemesh_scale_q_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_load_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_save_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_solve_dr_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_constraint_add_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.951169 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   668934 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF.png
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_anchors.png
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_constrain_nodes.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_create.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_edges_delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_modify_edges.png
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_modify_nodes.png
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_move_nodes.png
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_scale_q.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_solve_fd.png
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_update_constraints.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_ui.png
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/rui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-18 20:10:03.000000 compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/ui.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:10:17.947169 compas_fofin-0.7.0/src/compas_fofin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-18 20:10:17.000000 compas_fofin-0.7.0/src/compas_fofin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-18 20:10:17.000000 compas_fofin-0.7.0/src/compas_fofin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:10:17.000000 compas_fofin-0.7.0/src/compas_fofin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:10:17.000000 compas_fofin-0.7.0/src/compas_fofin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 20:10:17.000000 compas_fofin-0.7.0/src/compas_fofin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 20:10:17.000000 compas_fofin-0.7.0/src/compas_fofin.egg-info/top_level.txt
```

### Comparing `compas_fofin-0.6.0/CHANGELOG.md` & `compas_fofin-0.7.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## Unreleased
+
+### Added
+
+### Changed
+
+### Removed
+
+
+## [0.7.0] 2023-06-18
+
+### Added
+
+### Changed
+
+* Updated CI/CD setups.
+
+### Removed
+
+
 ## [0.6.0] 2022-11-09
 
 ### Added
 
 * Added `compas_fofin.rhino.install.after_rhino_install`.
 
 ### Changed
```

### Comparing `compas_fofin-0.6.0/LICENSE` & `compas_fofin-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/PKG-INFO` & `compas_fofin-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: compas_fofin
-Version: 0.6.0
+Version: 0.7.0
 Summary: Form Finding bundle for COMPAS
 Home-page: https://github.com/BlockResearchGroup/compas-FoFin
 Author: tom van mele
 Author-email: van.mele@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # COMPAS FoFin
 
 Form Finding bundle for COMPAS
```

### Comparing `compas_fofin-0.6.0/setup.py` & `compas_fofin-0.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="compas_fofin",
-    version='0.6.0',
+    version='0.7.0',
     description="Form Finding bundle for COMPAS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BlockResearchGroup/compas-FoFin",
     author="tom van mele",
     author_email="van.mele@arch.ethz.ch",
     license="MIT license",
@@ -42,28 +42,28 @@
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Unix",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     keywords=[],
     project_urls={},
     packages=["compas_fofin"],
     package_dir={"": "src"},
     package_data={},
     data_files=[],
     include_package_data=True,
     zip_safe=False,
     install_requires=requirements,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     extras_require=optional_requirements,
     entry_points={
         "console_scripts": [],
     },
     ext_modules=[],
 )
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/__init__.py` & `compas_fofin-0.7.0/src/compas_fofin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # import compas
 
 
 __author__ = ["tom van mele"]
 __copyright__ = "Block Research Group - ETH Zurich"
 __license__ = "MIT License"
 __email__ = "van.mele@arch.ethz.ch"
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/artists/cablemeshartist.py` & `compas_fofin-0.7.0/src/compas_fofin/artists/cablemeshartist.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/artists/constraintartist.py` & `compas_fofin-0.7.0/src/compas_fofin/artists/constraintartist.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/datastructures/__init__.py` & `compas_fofin-0.7.0/src/compas_fofin/datastructures/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,10 +18,8 @@
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
 
 from .cablemesh import CableMesh  # noqa: F401
 
 
-__all__ = [
-    'CableMesh'
-]
+__all__ = ["CableMesh"]
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/datastructures/cablemesh.py` & `compas_fofin-0.7.0/src/compas_fofin/datastructures/cablemesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,15 @@
     def vertex_load(self, vertex):
         return Vector(*self.vertex_attributes(vertex, ["px", "py", "pz"]))
 
     def edge_line(self, edge):
         return Line(self.vertex_coordinates(edge[0]), self.vertex_coordinates(edge[1]))
 
     def edge_vector(self, edge):
-        return Vector.from_start_end(
-            self.vertex_coordinates(edge[0]), self.vertex_coordinates(edge[1])
-        )
+        return Vector.from_start_end(self.vertex_coordinates(edge[0]), self.vertex_coordinates(edge[1]))
 
     def edge_force(self, edge):
         vector = self.edge_vector()
         vector.unitize()
         vector.scale(self.edge_attribute(edge, "_f"))
         return vector
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/objects/__init__.py` & `compas_fofin-0.7.0/src/compas_fofin/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/objects/cablemeshobject.py` & `compas_fofin-0.7.0/src/compas_fofin/objects/cablemeshobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,47 +13,49 @@
 
 class CableMeshObject(MeshObject):
     """Base object for representing a cable mesh in a scene."""
 
     # TODO: Move this to a settings object
     # TODO: For every setting use a setting object
 
-    SETTINGS = Settings({
-        "layer": StrValue("FF"),
-        "show.vertices:free": BoolValue(False),
-        "show.vertices:is_anchor": BoolValue(True),
-        "show.edges": BoolValue(True),
-        "show.faces": BoolValue(False),
-        "show.faces:all": BoolValue(False),
-        "show.reactions": BoolValue(True),
-        "show.loads": BoolValue(True),
-        "show.selfweight": BoolValue(True),
-        "show.pipes:forcedensities": BoolValue(False),
-        "show.pipes:forces": BoolValue(True),
-        "show.constraints": BoolValue(True),
-        "color.vertices": ColorValue(Color.black()),
-        "color.vertices:is_anchor": ColorValue(Color.red()),
-        "color.vertices:is_fixed": ColorValue(Color.blue()),
-        "color.vertices:is_constrained": ColorValue(Color.cyan()),
-        "color.edges": ColorValue(Color.black()),
-        "color.faces": ColorValue(Color.white().darkened(25)),
-        "color.tension": ColorValue(Color.red()),
-        "color.compression": ColorValue(Color.blue()),
-        "color.reactions": ColorValue(Color.green().darkened(50)),
-        "color.loads": ColorValue(Color.green().darkened(50)),
-        "color.selfweight": ColorValue(Color.white()),
-        "color.invalid": ColorValue(Color.black()),
-        "color.pipes": ColorValue(Color.white().darkened(50)),
-        "scale.reactions": FloatValue(0.300),
-        "scale.loads": FloatValue(1.0),
-        "scale.selfweight": FloatValue(1.0),
-        "pipe_thickness.min": FloatValue(0.0),
-        "pipe_thickness.max": FloatValue(10.0),
-        "tol.externalforces": FloatValue(1e-3),
-    })
+    SETTINGS = Settings(
+        {
+            "layer": StrValue("FF"),
+            "show.vertices:free": BoolValue(False),
+            "show.vertices:is_anchor": BoolValue(True),
+            "show.edges": BoolValue(True),
+            "show.faces": BoolValue(False),
+            "show.faces:all": BoolValue(False),
+            "show.reactions": BoolValue(True),
+            "show.loads": BoolValue(True),
+            "show.selfweight": BoolValue(True),
+            "show.pipes:forcedensities": BoolValue(False),
+            "show.pipes:forces": BoolValue(True),
+            "show.constraints": BoolValue(True),
+            "color.vertices": ColorValue(Color.black()),
+            "color.vertices:is_anchor": ColorValue(Color.red()),
+            "color.vertices:is_fixed": ColorValue(Color.blue()),
+            "color.vertices:is_constrained": ColorValue(Color.cyan()),
+            "color.edges": ColorValue(Color.black()),
+            "color.faces": ColorValue(Color.white().darkened(25)),
+            "color.tension": ColorValue(Color.red()),
+            "color.compression": ColorValue(Color.blue()),
+            "color.reactions": ColorValue(Color.green().darkened(50)),
+            "color.loads": ColorValue(Color.green().darkened(50)),
+            "color.selfweight": ColorValue(Color.white()),
+            "color.invalid": ColorValue(Color.black()),
+            "color.pipes": ColorValue(Color.white().darkened(50)),
+            "scale.reactions": FloatValue(0.300),
+            "scale.loads": FloatValue(1.0),
+            "scale.selfweight": FloatValue(1.0),
+            "pipe_thickness.min": FloatValue(0.0),
+            "pipe_thickness.max": FloatValue(10.0),
+            "tol.externalforces": FloatValue(1e-3),
+        }
+    )
 
     def __init__(self, *args, **kwargs):
         super(CableMeshObject, self).__init__(*args, **kwargs)
         self._is_valid = False
         self._group_free = None
         self._group_fixed = None
         self._group_anchors = None
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/objects/constraintobject.py` & `compas_fofin-0.7.0/src/compas_fofin/objects/constraintobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import uuid
 from compas_ui.objects import Object
 from compas_ui.values import Settings
 
 
 class ConstraintObject(Object):
-
     SETTINGS = Settings()
 
     def __init__(self, *args, **kwargs):
         super(ConstraintObject, self).__init__(*args, **kwargs)
 
     @property
     def state(self):
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/objects/lineconstraintobject.py` & `compas_fofin-0.7.0/src/compas_fofin/objects/lineconstraintobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import print_function
 
 from compas_ui.objects import Object
 from compas_ui.values import Settings
 
 
 class LineConstraintObject(Object):
-
     SETTINGS = Settings()
 
     def __init__(self, *args, **kwargs):
         super(LineConstraintObject, self).__init__(*args, **kwargs)
 
     @property
     def line(self):
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/artists/__init__.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/artists/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from .lineconstraintartist import RhinoLineConstraintArtist
 from .circleconstraintartist import RhinoCircleConstraintArtist
 from .curveconstraintartist import RhinoCurveConstraintArtist
 
 
 @plugin(category="factories", requires=["Rhino"])
 def register_artists():
-
     RhinoArtist.register(CurveConstraint, RhinoCurveConstraintArtist, context="Rhino")
     RhinoArtist.register(LineConstraint, RhinoLineConstraintArtist, context="Rhino")
     RhinoArtist.register(CircleConstraint, RhinoCircleConstraintArtist, context="Rhino")
     RhinoArtist.register(CableMesh, RhinoCableMeshArtist, context="Rhino")
 
     print("FoFin Rhino Artists registered.")
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/artists/cablemeshartist.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/artists/cablemeshartist.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/artists/circleconstraintartist.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/artists/circleconstraintartist.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/artists/curveconstraintartist.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/artists/curveconstraintartist.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/artists/lineconstraintartist.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/artists/lineconstraintartist.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/conduits/cablemeshconduit.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/conduits/cablemeshconduit.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,17 +171,15 @@
 
     def PostDrawObjects(self, e):
         for edge in self.edges:
             u, v = edge
             sp = self.xyz[u]
             ep = self.xyz[v]
             thickness = int(abs(self.values[edge]))
-            e.Display.DrawLine(
-                Point3d(*sp), Point3d(*ep), Color.FromArgb(*self.color[edge]), thickness
-            )
+            e.Display.DrawLine(Point3d(*sp), Point3d(*ep), Color.FromArgb(*self.color[edge]), thickness)
 
 
 class EdgeConduit(BaseConduit):
     """Display conduit for CableMesh edges as lines.
 
     Parameters
     ----------
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/conversions/curves.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/conversions/curves.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/objects/__init__.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/objects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from .lineconstraintobject import RhinoLineConstraintObject
 from .circleconstraintobject import RhinoCircleConstraintObject
 from .curveconstraintobject import RhinoCurveConstraintObject
 
 
 @plugin(category="ui", requires=["Rhino"])
 def register_objects():
-
     RhinoObject.register(CurveConstraint, RhinoCurveConstraintObject, context="Rhino")
     RhinoObject.register(LineConstraint, RhinoLineConstraintObject, context="Rhino")
     RhinoObject.register(CircleConstraint, RhinoCircleConstraintObject, context="Rhino")
     RhinoObject.register(CableMesh, RhinoCableMeshObject, context="Rhino")
 
     print("FoFin Rhino Objects registered.")
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/objects/cablemeshobject.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/objects/cablemeshobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,17 +153,15 @@
         if not self._conduit_forces:
             self._conduit_forces = PipeConduit(xyz={}, edges=[], values={}, color={})
         return self._conduit_forces
 
     @property
     def conduit_forcedensities(self):
         if not self._conduit_forcedensities:
-            self._conduit_forcedensities = PipeConduit(
-                xyz={}, edges=[], values={}, color={}
-            )
+            self._conduit_forcedensities = PipeConduit(xyz={}, edges=[], values={}, color={})
         return self._conduit_forcedensities
 
     @property
     def conduit_edges(self):
         if not self._conduit_edges:
             vertex_index = self.mesh.key_index()
             edges = self.mesh.edges_where(_is_edge=True)
@@ -351,23 +349,18 @@
     # Vertices
     # --------
     # Draw the vertices and add them to the vertex group.
     # Free vertices and anchored vertices are drawn separately.
     # ======================================================================
 
     def _draw_vertices(self):
-
         free = list(self.mesh.vertices_where(is_anchor=False))
         fixed = list(self.mesh.vertices_where(is_fixed=True))
         anchored = list(self.mesh.vertices_where(is_anchor=True))
-        constrained = list(
-            self.mesh.vertices_where_predicate(
-                lambda key, attr: attr["constraint"] is not None
-            )
-        )
+        constrained = list(self.mesh.vertices_where_predicate(lambda key, attr: attr["constraint"] is not None))
 
         color_free = self.settings["color.vertices"]
         color_fixed = self.settings["color.vertices:is_fixed"]
         color_anchored = self.settings["color.vertices:is_anchor"]
         color_constrained = self.settings["color.vertices:is_constrained"]
 
         color = {vertex: color_free for vertex in free}
@@ -405,15 +398,14 @@
     # ======================================================================
     # Edges
     # -----
     # Draw the edges and add them to the edge group.
     # ======================================================================
 
     def _draw_edges(self):
-
         edges = list(self.mesh.edges_where(_is_edge=True))
         color = {edge: self.settings["color.edges"] for edge in edges}
 
         if self.is_valid:
             edge_q = {edge: self.mesh.edge_attribute(edge, "q") for edge in edges}
             for edge in edges:
                 if edge_q[edge] < 0.0:
@@ -435,15 +427,14 @@
     # ======================================================================
     # Faces
     # -----
     # Draw the faces and add them to the face group.
     # ======================================================================
 
     def _draw_faces(self):
-
         if self.settings["show.faces:all"]:
             faces = list(self.mesh.faces())
         else:
             faces = list(self.mesh.faces_where(is_loaded=True))
 
         if faces:
             color = {face: self.settings["color.faces"] for face in faces}
@@ -462,15 +453,14 @@
     # ======================================================================
     # Constraints
     # -----------
     # Draw the constraints if they are not alreay in the model.
     # ======================================================================
 
     def _draw_constraints(self):
-
         old_new = {}
 
         for vertex in self.mesh.vertices():
             constraint = self.mesh.vertex_attribute(vertex, "constraint")
             if constraint is not None:
                 guid = constraint._rhino_guid
 
@@ -539,15 +529,14 @@
             self.conduit_selfweight.tol = self.settings["tol.externalforces"]
             self.conduit_selfweight.enable()
 
     def _draw_force_overlays(self):
         self.conduit_forces.disable()
 
         if self.is_valid and self.settings["show.pipes:forces"]:
-
             xyz = {v: self.mesh.vertex_coordinates(v) for v in self.mesh.vertices()}
             edges = list(self.mesh.edges_where(_is_edge=True))
             forces = self.mesh.edges_attribute("_f", keys=edges)
 
             fmin = min(forces)
             fmax = max(forces)
             frange = (fmax - fmin) or 1
@@ -576,15 +565,14 @@
             self.conduit_forces.color = color
             self.conduit_forces.enable()
 
     def _draw_q_overlays(self):
         self.conduit_forcedensities.disable()
 
         if self.is_valid and self.settings["show.pipes:forcedensities"]:
-
             xyz = {v: self.mesh.vertex_coordinates(v) for v in self.mesh.vertices()}
             edges = list(self.mesh.edges_where(_is_edge=True))
             qs = self.mesh.edges_attribute("q", keys=edges)
 
             qmin = min(qs)
             qmax = max(qs)
             qrange = (qmax - qmin) or 1
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/objects/circleconstraintobject.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/objects/circleconstraintobject.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/objects/curveconstraintobject.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/objects/curveconstraintobject.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/objects/lineconstraintobject.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/objects/lineconstraintobject.py`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/register.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         "solver.tol.displacements": FloatValue(1e-3),
     }
 )
 
 
 @plugin(category="ui")
 def register(ui):
-
     plugin_name = "FoFin"
     plugin_path = os.path.join(HERE, "ui", plugin_name)
     if not os.path.isdir(plugin_path):
         raise Exception("Cannot find the plugin: {}".format(plugin_path))
 
     ui.registry["FoFin"] = SETTINGS
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF__toolbar_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF__toolbar_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 
 HERE = os.path.dirname(__file__)
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()  # noqa: F841
 
     config = [
         {
             "command": "FF_toolbar_cablemesh_create",
             "icon": os.path.join(HERE, "assets", "FF_cablemesh_create.png"),
         },
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_anchors_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_anchors_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 __commandname__ = "FF_cablemesh_anchors"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_constraints_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_constraints_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 
 __commandname__ = "FF_cablemesh_constraints"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, RhinoCableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
@@ -63,15 +62,14 @@
             return
 
         obj = compas_rhino.find_object(guid)
         if not obj:
             return
 
         if obj.ObjectType == Rhino.DocObjects.ObjectType.Curve:
-
             constraint = None
             for vertex in mesh.vertices():
                 temp = mesh.vertex_attribute(vertex, "constraint")
                 if temp is not None:
                     if temp._rhino_guid == str(guid):
                         constraint = temp
                         break
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_edges_delete_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_edges_delete_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 
 
 __commandname__ = "FF_cablemesh_edges_delete"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
     cablemesh.is_valid = False
     ui.scene.update()
 
     edges = ui.controller.mesh_select_edges(cablemesh)
 
     if edges:
         fkeys = set()
-        for (u, v) in edges:
+        for u, v in edges:
             fkeys.update(cablemesh.mesh.edge_faces(u, v))
         for fkey in fkeys:
             if fkey:
                 cablemesh.mesh.delete_face(fkey)
 
         cablemesh.mesh.remove_unused_vertices()
         ui.scene.update()
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_box_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_box_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 __commandname__ = "FF_cablemesh_from_box"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     guid = compas_rhino.select_object("Select a box")
     if not guid:
         return
 
     k = ui.get_integer("Resolution", minval=1, maxval=6, default=2)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_cylinder_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_cylinder_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 __commandname__ = "FF_cablemesh_from_cylinder"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     guid = compas_rhino.select_object("Select a cylinder")
     if not guid:
         return
 
     U = ui.get_integer(
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_mesh_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_mesh_cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 
 __commandname__ = "FF_cablemesh_from_mesh"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     guid = compas_rhino.select_mesh()
     if not guid:
         return
 
     mesh = RhinoMesh.from_guid(guid).to_compas(cls=CableMesh)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_meshgrid_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_meshgrid_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 
 __commandname__ = "FF_cablemesh_from_meshgrid"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     nx = ui.get_integer(
         "Number of faces in the X direction",
         minval=1,
         maxval=1000,
         default=10,
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_surface_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_surface_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 __commandname__ = "FF_cablemesh_from_surface"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     guid = compas_rhino.select_surface()
     if not guid:
         return
 
     U = ui.get_integer(
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_edges_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_edges_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,28 @@
 
 
 __commandname__ = "FF_cablemesh_modify_edges"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
     cablemesh.is_valid = False
     ui.scene.update()
 
     edges = ui.controller.mesh_select_edges(cablemesh)
 
     if edges:
-
-        public = [
-            name
-            for name in cablemesh.mesh.default_edge_attributes.keys()
-            if not name.startswith("_")
-        ]
+        public = [name for name in cablemesh.mesh.default_edge_attributes.keys() if not name.startswith("_")]
         cablemesh.modify_edges(edges, names=public)
 
     ui.scene.update()
     ui.record()
 
     compas_rhino.rs.UnselectAllObjects()
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_nodes_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_nodes_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,40 +8,35 @@
 
 
 __commandname__ = "FF_cablemesh_modify_nodes"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
-    cablemesh.settings["show.vertices:anchors"] = True
+    cablemesh.settings["show.vertices:is_anchor"] = True
     cablemesh.settings["show.vertices:free"] = True
 
     cablemesh.is_valid = False
 
     ui.scene.update()
 
     nodes = ui.controller.mesh_select_vertices(cablemesh)
 
     if nodes:
-        public = [
-            name
-            for name in cablemesh.mesh.default_vertex_attributes.keys()
-            if not name.startswith("_")
-        ]
+        public = [name for name in cablemesh.mesh.default_vertex_attributes.keys() if not name.startswith("_")]
         cablemesh.modify_vertices(nodes, names=public)
 
-    cablemesh.settings["show.vertices:anchors"] = True
+    cablemesh.settings["show.vertices:is_anchor"] = True
     cablemesh.settings["show.vertices:free"] = False
 
     ui.scene.update()
     ui.record()
 
     compas_rhino.rs.UnselectAllObjects()
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_update_constraints_cmd.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
 
+import compas_rhino
+
 from compas_ui.ui import UI
 from compas_fofin.objects import CableMeshObject
 
 
-__commandname__ = "FF_cablemesh_move"
+__commandname__ = "FF_cablemesh_update_constraints"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
-    if cablemesh.move():
-        ui.scene.update()
-        ui.record()
-
-    # provide the option to move in
-    # - global coordinate space
-    # - object coordinate space
-    # - ...
+    cablemesh.update_constraints()
+
+    compas_rhino.rs.UnselectAllObjects()
+    cablemesh.is_valid = False
+    ui.scene.update()
+    ui.record()
 
 
 if __name__ == "__main__":
     RunCommand(True)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_nodes_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_nodes_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 __commandname__ = "FF_cablemesh_move_nodes"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_scale_q_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_scale_q_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 __commandname__ = "FF_cablemesh_scale_q"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
@@ -32,22 +31,18 @@
     selected = ui.controller.mesh_select_edges(cablemesh)
     if not selected:
         return
 
     Q = cablemesh.mesh.edges_attribute("q", keys=selected)
 
     if mode == "Value":
-
         scale = ui.get_real("Scaling factor", minval=-1e2, maxval=+1e2, default=1.0)
 
     elif mode == "Interactive":
-
-        fd_create = ui.proxy.function(
-            "compas_fd.fd.mesh_fd_constrained_cache_create", cache=True
-        )
+        fd_create = ui.proxy.function("compas_fd.fd.mesh_fd_constrained_cache_create", cache=True)
         fd_call = ui.proxy.function("compas_fd.fd.mesh_fd_constrained_cache_call")
         fd_delete = ui.proxy.function("compas_fd.fd.mesh_fd_constrained_cache_delete")
 
         cached_data = fd_create(
             cablemesh.mesh,
             selected,
             kmax=ui.registry["FoFin"]["solver.kmax"],
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_solve_fd_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_solve_fd_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import Eto.Forms
 
 __commandname__ = "FF_cablemesh_solve_fd"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_update_constraints_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_cablemesh_unconstrain_nodes_cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
 
 import compas_rhino
-
 from compas_ui.ui import UI
 from compas_fofin.objects import CableMeshObject
 
 
-__commandname__ = "FF_cablemesh_update_constraints"
+__commandname__ = "FF_cablemesh_unconstrain_nodes"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
-    cablemesh.update_constraints()
+    nodes = ui.controller.mesh_select_vertices(cablemesh)
+
+    if nodes:
+        for node in nodes:
+            cablemesh.mesh.unset_vertex_attribute(node, "constraint")
+
+        cablemesh.is_valid = False
+        ui.scene.update()
+        ui.record()
 
     compas_rhino.rs.UnselectAllObjects()
-    cablemesh.is_valid = False
-    ui.scene.update()
-    ui.record()
 
 
 if __name__ == "__main__":
     RunCommand(True)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_toolbar_cablemesh_create_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_toolbar_cablemesh_create_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 
 __commandname__ = "FF_toolbar_cablemesh_create"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()  # noqa: F841
 
     options = ["FromMeshgrid", "FromMesh", "FromSurface", "FromBox", "FromCylinder"]
     option = compas_rhino.rs.GetString("Create Cablemesh", strings=options)
 
     if not option:
         return
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_cablemesh_constrain_nodes_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_cablemesh_constrain_nodes_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 
 __commandname__ = "FF_cablemesh_constrain_nodes"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, RhinoCableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
@@ -38,20 +37,18 @@
         return
 
     obj = compas_rhino.find_object(guid)
     if not obj:
         return
 
     if obj.ObjectType == Rhino.DocObjects.ObjectType.Curve:
-
         curve = curveobject_to_compas(obj)
         constraint = Constraint(curve)
 
     elif obj.ObjectType == Rhino.DocObjects.ObjectType.Surface:
-
         guid = compas_rhino.select_surface(message="Select surface constraint")
         if not guid:
             return
 
         surface = RhinoSurface.from_guid(guid).to_compas()
         constraint = Constraint(surface)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_cablemesh_unconstrain_nodes_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_save_cmd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
 
-import compas_rhino
+import compas
 from compas_ui.ui import UI
 from compas_fofin.objects import CableMeshObject
 
 
-__commandname__ = "FF_cablemesh_unconstrain_nodes"
+__commandname__ = "FF_cablemesh_data_save"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
-    nodes = ui.controller.mesh_select_vertices(cablemesh)
-
-    if nodes:
-        for node in nodes:
-            cablemesh.mesh.unset_vertex_attribute(node, "constraint")
-
-        cablemesh.is_valid = False
-        ui.scene.update()
-        ui.record()
+    mesh = cablemesh.mesh
 
-    compas_rhino.rs.UnselectAllObjects()
+    path = ui.pick_file_save("FoFin.data")
+    if path:
+        compas.json_dump(mesh, path)
 
 
 if __name__ == "__main__":
     RunCommand(True)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_toolbar_load_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_toolbar_load_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 
 from compas_ui.ui import UI
 
 import FF_load_cmd
 import FF_cablemesh_data_load_cmd
 
 
-__commandname__ = 'FF_toolbar_load'
+__commandname__ = "FF_toolbar_load"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     options = ["LoadSession", "LoadMeshData"]
     option = compas_rhino.rs.GetString("Create Cablemesh:", strings=options)
 
     if not option:
         return
 
     if option == "LoadSession":
         FF_load_cmd.RunCommand(True)
 
     elif option == "LoadMeshData":
         FF_cablemesh_data_load_cmd.RunCommand(True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     RunCommand(True)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_toolbar_save_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/FF_toolbar_save_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 from compas_ui.ui import UI
 
 import FF_save_cmd
 import FF_saveas_cmd
 import FF_cablemesh_data_save_cmd
 
 
-__commandname__ = 'FF_toolbar_save'
+__commandname__ = "FF_toolbar_save"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     options = ["SaveSession", "SaveSessionAs", "SaveMeshData"]
     option = compas_rhino.rs.GetString("Create Cablemesh:", strings=options)
 
     if not option:
         return
 
     if option == "SaveSession":
@@ -29,9 +28,9 @@
     elif option == "SaveSessionAs":
         FF_saveas_cmd.RunCommand(True)
 
     elif option == "SaveMeshData":
         FF_cablemesh_data_save_cmd.RunCommand(True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     RunCommand(True)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/_FF_cablemesh_scale_q_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/_FF_cablemesh_scale_q_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     else:
         mesh.data = result.data
         return mesh
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
@@ -64,19 +63,17 @@
 
     Q = cablemesh.mesh.edges_attribute("q", keys=selected)
     cached_Q = ui.proxy.cache(Q)
 
     kmax = 10
 
     if mode == "Value":
-
         scale = ui.get_real("Scaling factor?", minval=-1e2, maxval=+1e2, default=1.0)
 
     elif mode == "Interactive":
-
         gp = Rhino.Input.Custom.GetPoint()
         gp.SetCommandPrompt("Base point for scaling.")
 
         gp.Get()
         if gp.CommandResult() != Rhino.Commands.Result.Success:
             return False
 
@@ -101,20 +98,24 @@
             v2 = r2 - o
             l2 = v2.SquareLength
 
             sign = +1 if Rhino.Geometry.Vector3d.Multiply(v1, v2) > 0 else -1
             scale = sign * l2 / l1
             print(scale)
 
-            result = fd_cached_proxy(cached_mesh, scale, selected, cached_Q,
-                                     kmax,
-                                     ui.registry["FoFin"]["solver.damping"],
-                                     ui.registry["FoFin"]["solver.tol.residuals"],
-                                     ui.registry["FoFin"]["solver.tol.displacements"],
-                                     )
+            result = fd_cached_proxy(
+                cached_mesh,
+                scale,
+                selected,
+                cached_Q,
+                kmax,
+                ui.registry["FoFin"]["solver.damping"],
+                ui.registry["FoFin"]["solver.tol.residuals"],
+                ui.registry["FoFin"]["solver.tol.displacements"],
+            )
 
             if not result:
                 print("Force-density method equilibrium failed!")
                 return False
 
             cablemesh.mesh.data = result.data
             cablemesh.is_valid = True
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_cmd.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 __commandname__ = "FF_cablemesh_data"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_load_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_load_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 __commandname__ = "FF_cablemesh_data_load"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_data_save_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_cmd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import print_function
 from __future__ import absolute_import
 from __future__ import division
 
-import compas
+import compas_rhino
 from compas_ui.ui import UI
 from compas_fofin.objects import CableMeshObject
 
 
-__commandname__ = "FF_cablemesh_data_save"
+__commandname__ = "FF_cablemesh_modify"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
 
-    mesh = cablemesh.mesh
+    cablemesh.is_valid = False
+    ui.scene.update()
+
+    cablemesh.modify()
+
+    ui.scene.update()
+    ui.record()
 
-    path = ui.pick_file_save("FoFin.data")
-    if path:
-        compas.json_dump(mesh, path)
+    compas_rhino.rs.UnselectAllObjects()
 
 
 if __name__ == "__main__":
     RunCommand(True)
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_solve_dr_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_cablemesh_solve_dr_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 __commandname__ = "FF_cablemesh_solve_dr"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     cablemesh = ui.scene.active_object
 
     if not isinstance(cablemesh, CableMeshObject):
         raise Exception("The active object is not a CableMesh.")
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_constraint_add_cmd.py` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/__temp/__FF_constraint_add_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 
 __commandname__ = "FF_constraint_add"
 
 
 @UI.error()
 def RunCommand(is_interactive):
-
     ui = UI()
 
     ctypes = ["Line", "Curve", "Surface"]
     ctype = ui.get_string("Node constraint type?", options=ctypes)
     if not ctype:
         return
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF.png` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF.png`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_constrain_nodes.png` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_constrain_nodes.png`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_modify_edges.png` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_modify_edges.png`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_modify_nodes.png` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_modify_nodes.png`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_scale_q.png` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_scale_q.png`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_solve_fd.png` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_solve_fd.png`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_update_constraints.png` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_cablemesh_update_constraints.png`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_ui.png` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/FF_ui.png`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/index.html` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/index.html`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/styles.css` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/assets/styles.css`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/config.json` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/config.json`

 * *Files identical despite different names*

### Comparing `compas_fofin-0.6.0/src/compas_fofin/rhino/ui/FoFin/dev/ui.json` & `compas_fofin-0.7.0/src/compas_fofin/rhino/ui/FoFin/dev/ui.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.989572192513369%*

 * *Differences: {"'commands'": "{insert: [(7, OrderedDict([('name', 'FF_cablemesh_modify'), ('menu_text', 'Mesh "*

 * *               "Attributes'), ('tooltip', 'Modify Mesh Attributes')]))]}",*

 * * "'menus'": "{0: {'items': {insert: [(5, OrderedDict([('type', 'separator')])), (6, "*

 * *            "OrderedDict([('command', 'FF_cablemesh_modify')]))]}}}"}*

```diff
@@ -29,14 +29,19 @@
             "name": "FF_cablemesh_from_meshgrid"
         },
         {
             "menu_text": "Cablemesh From Surface",
             "name": "FF_cablemesh_from_surface"
         },
         {
+            "menu_text": "Mesh Attributes",
+            "name": "FF_cablemesh_modify",
+            "tooltip": "Modify Mesh Attributes"
+        },
+        {
             "icon": 9,
             "menu_text": "Edge Attributes",
             "name": "FF_cablemesh_modify_edges",
             "tooltip": "Modify Edge Attributes"
         },
         {
             "icon": 6,
@@ -136,14 +141,20 @@
                 {
                     "command": "FF_cablemesh_solve_fd"
                 },
                 {
                     "type": "separator"
                 },
                 {
+                    "command": "FF_cablemesh_modify"
+                },
+                {
+                    "type": "separator"
+                },
+                {
                     "items": [
                         {
                             "command": "FF_cablemesh_move_nodes"
                         },
                         {
                             "command": "FF_cablemesh_constraints"
                         },
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin.egg-info/PKG-INFO` & `compas_fofin-0.7.0/src/compas_fofin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: compas-fofin
-Version: 0.6.0
+Version: 0.7.0
 Summary: Form Finding bundle for COMPAS
 Home-page: https://github.com/BlockResearchGroup/compas-FoFin
 Author: tom van mele
 Author-email: van.mele@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # COMPAS FoFin
 
 Form Finding bundle for COMPAS
```

### Comparing `compas_fofin-0.6.0/src/compas_fofin.egg-info/SOURCES.txt` & `compas_fofin-0.7.0/src/compas_fofin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 src/compas_fofin/__init__.py
 src/compas_fofin.egg-info/PKG-INFO
 src/compas_fofin.egg-info/SOURCES.txt
 src/compas_fofin.egg-info/dependency_links.txt
@@ -46,14 +47,15 @@
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_constraints_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_edges_delete_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_box_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_cylinder_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_mesh_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_meshgrid_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_from_surface_cmd.py
+src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_edges_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_modify_nodes_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_move_nodes_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_scale_q_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_solve_fd_cmd.py
 src/compas_fofin/rhino/ui/FoFin/dev/FF_cablemesh_update_constraints_cmd.py
```


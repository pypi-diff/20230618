# Comparing `tmp/multipie-1.1.8.tar.gz` & `tmp/multipie-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multipie-1.1.8.tar", last modified: Fri Jun 16 02:53:50 2023, max compression
+gzip compressed data, was "multipie-1.1.9.tar", last modified: Fri Jun 16 10:31:13 2023, max compression
```

## Comparing `multipie-1.1.8.tar` & `multipie-1.1.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.404238 multipie-1.1.8/
--rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.1.8/LICENSE
--rw-------   0 hiro       (501) staff       (20)       81 2023-05-15 22:16:08.000000 multipie-1.1.8/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-16 02:53:50.404336 multipie-1.1.8/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1727 2023-05-25 21:40:12.000000 multipie-1.1.8/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.371873 multipie-1.1.8/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)     2299 2023-06-16 01:54:52.000000 multipie-1.1.8/multipie/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.387759 multipie-1.1.8/multipie/binary_data/
--rw-r--r--   0 hiro       (501) staff       (20)  5479250 2023-05-15 16:10:42.000000 multipie-1.1.8/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.1.8/multipie/binary_data/CharacterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-05-15 16:00:43.000000 multipie-1.1.8/multipie/binary_data/ClebschGordanPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-05-15 15:37:02.000000 multipie-1.1.8/multipie/binary_data/HarmonicsPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-05-15 16:01:10.000000 multipie-1.1.8/multipie/binary_data/ResponseTensorPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.1.8/multipie/binary_data/SymmetryOperationGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.1.8/multipie/binary_data/VirtualClusterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   380153 2023-05-15 15:37:10.000000 multipie-1.1.8/multipie/binary_data/WyckoffGSet.pkl
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.388351 multipie-1.1.8/multipie/character/
--rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/character/character_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/character/character_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.388661 multipie-1.1.8/multipie/clebsch_gordan/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/clebsch_gordan/clebsch_gordan_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
--rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.1.8/multipie/const.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.396946 multipie-1.1.8/multipie/data/
--rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_atomic_multipoles.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_cartesian_to_ch_harmoncis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_character_table.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_compatibility_relation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_harmonics_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_no_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_product_decomp.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_symmetry_operation_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_symmetry_operation_sg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      883 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_tag_harmonics_alias.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_tag_point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_tag_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1380 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_transform_matrix.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_virtual_cluster_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15108 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_wyckoff_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   157758 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/data/data_wyckoff_sg.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.397450 multipie-1.1.8/multipie/group/
--rwxr-xr-x   0 hiro       (501) staff       (20)    30142 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/group/point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    22542 2023-06-12 13:15:36.000000 multipie-1.1.8/multipie/group/space_group.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.398414 multipie-1.1.8/multipie/harmonics/
--rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/harmonics/harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/harmonics/harmonics_complex_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/harmonics/harmonics_complex_pg_set.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/harmonics/harmonics_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/harmonics/harmonics_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.398553 multipie-1.1.8/multipie/harmonics/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/harmonics/util/equivalent_operator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.399239 multipie-1.1.8/multipie/model/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2198 2023-06-06 22:09:12.000000 multipie-1.1.8/multipie/model/construct_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3459 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/model/create_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    31907 2023-06-16 02:46:38.000000 multipie-1.1.8/multipie/model/material_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/model/multipie_manager.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    18219 2023-06-16 02:02:17.000000 multipie-1.1.8/multipie/model/symmetry_adapted_model.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.399686 multipie-1.1.8/multipie/model/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/model/util/atomic_matrix_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    26198 2023-06-16 02:40:39.000000 multipie-1.1.8/multipie/model/util/create_pdf.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    25021 2023-06-07 14:42:34.000000 multipie-1.1.8/multipie/model/util/symmetry_adapted_model_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.370377 multipie-1.1.8/multipie/multipole/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.400041 multipie-1.1.8/multipie/multipole/base/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/multipole/base/base_atomic_multipole_dataset.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/multipole/base/base_atomic_multipole_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.401106 multipie-1.1.8/multipie/multipole/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    14715 2023-05-31 07:36:18.000000 multipie-1.1.8/multipie/multipole/util/atomic_orbital_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     6736 2023-06-01 08:23:27.000000 multipie-1.1.8/multipie/multipole/util/atomic_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/multipole/util/multipole_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/multipole/util/pauli.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/multipole/util/spin_orbital_basis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4751 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/multipole/util/structure_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/multipole/util/z_samb_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.401392 multipie-1.1.8/multipie/response_tensor/
--rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/response_tensor/response_tensor_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/response_tensor/response_tensor_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.401539 multipie-1.1.8/multipie/response_tensor/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/response_tensor/util/response_tensor_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.401839 multipie-1.1.8/multipie/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.1.8/multipie/scripts/create_binary.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1601 2023-06-04 14:31:58.000000 multipie-1.1.8/multipie/scripts/create_samb.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.402268 multipie-1.1.8/multipie/symmetry_operation/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/symmetry_operation/symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    14936 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/symmetry_operation/symmetry_operation_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/symmetry_operation/symmetry_operation_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.402424 multipie-1.1.8/multipie/symmetry_operation/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     5488 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/symmetry_operation/util/symmetry_operation_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.403559 multipie-1.1.8/multipie/tag/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_list.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_multipole.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_response_tensor.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/tag/tag_wyckoff.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.403834 multipie-1.1.8/multipie/virtual_cluster/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/virtual_cluster/virtual_cluster_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/virtual_cluster/virtual_cluster_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.404097 multipie-1.1.8/multipie/wyckoff/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3252 2023-05-15 15:10:01.000000 multipie-1.1.8/multipie/wyckoff/wyckoff_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.1.8/multipie/wyckoff/wyckoff_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 02:53:50.373060 multipie-1.1.8/multipie.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     3339 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)      116 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        9 2023-06-16 02:53:50.000000 multipie-1.1.8/multipie.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      888 2023-06-16 02:53:50.405012 multipie-1.1.8/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.1.8/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.515001 multipie-1.1.9/
+-rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.1.9/LICENSE
+-rw-------   0 hiro       (501) staff       (20)       81 2023-05-15 22:16:08.000000 multipie-1.1.9/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-16 10:31:13.515089 multipie-1.1.9/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1727 2023-05-25 21:40:12.000000 multipie-1.1.9/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.464007 multipie-1.1.9/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)     2299 2023-06-16 10:25:10.000000 multipie-1.1.9/multipie/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.498067 multipie-1.1.9/multipie/binary_data/
+-rw-r--r--   0 hiro       (501) staff       (20)  5479250 2023-05-15 16:10:42.000000 multipie-1.1.9/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.1.9/multipie/binary_data/CharacterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-05-15 16:00:43.000000 multipie-1.1.9/multipie/binary_data/ClebschGordanPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-05-15 15:37:02.000000 multipie-1.1.9/multipie/binary_data/HarmonicsPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-05-15 16:01:10.000000 multipie-1.1.9/multipie/binary_data/ResponseTensorPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.1.9/multipie/binary_data/SymmetryOperationGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.1.9/multipie/binary_data/VirtualClusterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   380153 2023-05-15 15:37:10.000000 multipie-1.1.9/multipie/binary_data/WyckoffGSet.pkl
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.499007 multipie-1.1.9/multipie/character/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/character/character_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/character/character_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.499270 multipie-1.1.9/multipie/clebsch_gordan/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/clebsch_gordan/clebsch_gordan_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.1.9/multipie/const.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.507282 multipie-1.1.9/multipie/data/
+-rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_atomic_multipoles.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_cartesian_to_ch_harmoncis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_character_table.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_compatibility_relation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_harmonics_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_no_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_product_decomp.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_symmetry_operation_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_symmetry_operation_sg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      883 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_tag_harmonics_alias.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_tag_point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_tag_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1380 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_transform_matrix.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_virtual_cluster_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15108 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_wyckoff_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   157758 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/data/data_wyckoff_sg.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.507719 multipie-1.1.9/multipie/group/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    30142 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/group/point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22542 2023-06-12 13:15:36.000000 multipie-1.1.9/multipie/group/space_group.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.508677 multipie-1.1.9/multipie/harmonics/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/harmonics/harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/harmonics/harmonics_complex_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/harmonics/harmonics_complex_pg_set.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/harmonics/harmonics_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/harmonics/harmonics_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.508817 multipie-1.1.9/multipie/harmonics/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/harmonics/util/equivalent_operator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.509502 multipie-1.1.9/multipie/model/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2198 2023-06-06 22:09:12.000000 multipie-1.1.9/multipie/model/construct_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3459 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/model/create_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    31907 2023-06-16 02:46:38.000000 multipie-1.1.9/multipie/model/material_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/model/multipie_manager.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    18292 2023-06-16 10:24:29.000000 multipie-1.1.9/multipie/model/symmetry_adapted_model.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.509918 multipie-1.1.9/multipie/model/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/model/util/atomic_matrix_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    26198 2023-06-16 02:40:39.000000 multipie-1.1.9/multipie/model/util/create_pdf.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    25021 2023-06-07 14:42:34.000000 multipie-1.1.9/multipie/model/util/symmetry_adapted_model_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.462093 multipie-1.1.9/multipie/multipole/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.510193 multipie-1.1.9/multipie/multipole/base/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/multipole/base/base_atomic_multipole_dataset.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/multipole/base/base_atomic_multipole_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.511535 multipie-1.1.9/multipie/multipole/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14715 2023-05-31 07:36:18.000000 multipie-1.1.9/multipie/multipole/util/atomic_orbital_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     6736 2023-06-01 08:23:27.000000 multipie-1.1.9/multipie/multipole/util/atomic_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/multipole/util/multipole_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/multipole/util/pauli.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/multipole/util/spin_orbital_basis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4751 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/multipole/util/structure_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/multipole/util/z_samb_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.512015 multipie-1.1.9/multipie/response_tensor/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/response_tensor/response_tensor_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/response_tensor/response_tensor_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.512209 multipie-1.1.9/multipie/response_tensor/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/response_tensor/util/response_tensor_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.512558 multipie-1.1.9/multipie/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.1.9/multipie/scripts/create_binary.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1601 2023-06-04 14:31:58.000000 multipie-1.1.9/multipie/scripts/create_samb.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.512991 multipie-1.1.9/multipie/symmetry_operation/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/symmetry_operation/symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14936 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/symmetry_operation/symmetry_operation_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/symmetry_operation/symmetry_operation_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.513141 multipie-1.1.9/multipie/symmetry_operation/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     5488 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/symmetry_operation/util/symmetry_operation_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.514343 multipie-1.1.9/multipie/tag/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/tag/tag.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/tag/tag_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/tag/tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/tag/tag_list.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/tag/tag_multipole.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/tag/tag_response_tensor.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/tag/tag_symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/tag/tag_wyckoff.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.514614 multipie-1.1.9/multipie/virtual_cluster/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/virtual_cluster/virtual_cluster_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/virtual_cluster/virtual_cluster_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.514859 multipie-1.1.9/multipie/wyckoff/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3252 2023-05-15 15:10:01.000000 multipie-1.1.9/multipie/wyckoff/wyckoff_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.1.9/multipie/wyckoff/wyckoff_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-06-16 10:31:13.465067 multipie-1.1.9/multipie.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2222 2023-06-16 10:31:13.000000 multipie-1.1.9/multipie.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     3339 2023-06-16 10:31:13.000000 multipie-1.1.9/multipie.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-06-16 10:31:13.000000 multipie-1.1.9/multipie.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      116 2023-06-16 10:31:13.000000 multipie-1.1.9/multipie.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-06-16 10:31:13.000000 multipie-1.1.9/multipie.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        9 2023-06-16 10:31:13.000000 multipie-1.1.9/multipie.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      888 2023-06-16 10:31:13.515485 multipie-1.1.9/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.1.9/setup.py
```

### Comparing `multipie-1.1.8/LICENSE` & `multipie-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/PKG-INFO` & `multipie-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.1.8
+Version: 1.1.9
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.8
```

### Comparing `multipie-1.1.8/README.md` & `multipie-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/__init__.py` & `multipie-1.1.9/multipie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 __top_dir__ = os.path.normpath(os.path.dirname(__file__) + "/../") + "/"
 __bin_dir__ = __top_dir__ + "multipie/binary_data/"
 
 
 # ==================================================
 from gcoreutils.string_util import class_name
 from gcoreutils.binary_manager import BinaryManager
```

### Comparing `multipie-1.1.8/multipie/binary_data/BaseAtomicMultipoleDataset.pkl` & `multipie-1.1.9/multipie/binary_data/BaseAtomicMultipoleDataset.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/binary_data/CharacterPGSet.pkl` & `multipie-1.1.9/multipie/binary_data/CharacterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/binary_data/ClebschGordanPGSet.pkl` & `multipie-1.1.9/multipie/binary_data/ClebschGordanPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/binary_data/HarmonicsPGSet.pkl` & `multipie-1.1.9/multipie/binary_data/HarmonicsPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/binary_data/ResponseTensorPGSet.pkl` & `multipie-1.1.9/multipie/binary_data/ResponseTensorPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/binary_data/SymmetryOperationGSet.pkl` & `multipie-1.1.9/multipie/binary_data/SymmetryOperationGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/binary_data/VirtualClusterPGSet.pkl` & `multipie-1.1.9/multipie/binary_data/VirtualClusterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/binary_data/WyckoffGSet.pkl` & `multipie-1.1.9/multipie/binary_data/WyckoffGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/character/character_pg.py` & `multipie-1.1.9/multipie/character/character_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/character/character_pg_set.py` & `multipie-1.1.9/multipie/character/character_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/clebsch_gordan/clebsch_gordan_pg.py` & `multipie-1.1.9/multipie/clebsch_gordan/clebsch_gordan_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/clebsch_gordan/clebsch_gordan_pg_set.py` & `multipie-1.1.9/multipie/clebsch_gordan/clebsch_gordan_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/const.py` & `multipie-1.1.9/multipie/const.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_atomic_multipoles.py` & `multipie-1.1.9/multipie/data/data_atomic_multipoles.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_cartesian_to_ch_harmoncis.py` & `multipie-1.1.9/multipie/data/data_cartesian_to_ch_harmoncis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_character_table.py` & `multipie-1.1.9/multipie/data/data_character_table.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_compatibility_relation.py` & `multipie-1.1.9/multipie/data/data_compatibility_relation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_harmonics.py` & `multipie-1.1.9/multipie/data/data_harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_harmonics_real.py` & `multipie-1.1.9/multipie/data/data_harmonics_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_no_space_group.py` & `multipie-1.1.9/multipie/data/data_no_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_product_decomp.py` & `multipie-1.1.9/multipie/data/data_product_decomp.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_symmetry_operation_pg.py` & `multipie-1.1.9/multipie/data/data_symmetry_operation_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_symmetry_operation_sg.py` & `multipie-1.1.9/multipie/data/data_symmetry_operation_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_tag_harmonics_alias.py` & `multipie-1.1.9/multipie/data/data_tag_harmonics_alias.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_tag_irrep.py` & `multipie-1.1.9/multipie/data/data_tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_tag_point_group.py` & `multipie-1.1.9/multipie/data/data_tag_point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_tag_space_group.py` & `multipie-1.1.9/multipie/data/data_tag_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_transform_matrix.py` & `multipie-1.1.9/multipie/data/data_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_virtual_cluster_real.py` & `multipie-1.1.9/multipie/data/data_virtual_cluster_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_wyckoff_pg.py` & `multipie-1.1.9/multipie/data/data_wyckoff_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/data/data_wyckoff_sg.py` & `multipie-1.1.9/multipie/data/data_wyckoff_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/group/point_group.py` & `multipie-1.1.9/multipie/group/point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/group/space_group.py` & `multipie-1.1.9/multipie/group/space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/harmonics/harmonics.py` & `multipie-1.1.9/multipie/harmonics/harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/harmonics/harmonics_complex_pg.py` & `multipie-1.1.9/multipie/harmonics/harmonics_complex_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/harmonics/harmonics_complex_pg_set.py` & `multipie-1.1.9/multipie/harmonics/harmonics_complex_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/harmonics/harmonics_pg.py` & `multipie-1.1.9/multipie/harmonics/harmonics_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/harmonics/harmonics_pg_set.py` & `multipie-1.1.9/multipie/harmonics/harmonics_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/harmonics/util/equivalent_operator.py` & `multipie-1.1.9/multipie/harmonics/util/equivalent_operator.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/model/construct_model.py` & `multipie-1.1.9/multipie/model/construct_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/model/create_model.py` & `multipie-1.1.9/multipie/model/create_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/model/material_model.py` & `multipie-1.1.9/multipie/model/material_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/model/multipie_manager.py` & `multipie-1.1.9/multipie/model/multipie_manager.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/model/symmetry_adapted_model.py` & `multipie-1.1.9/multipie/model/symmetry_adapted_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,16 +204,17 @@
             if molecule:
                 if len(atomic_data) > 0:
                     atomic_info, atomic_data, z_data = redefine_index(atomic_info, atomic_data, z_data, molecule=True)
                 if len(uniform_data) > 0:
                     uniform_info, uniform_data, z_data = redefine_index(
                         uniform_info, uniform_data, z_data, molecule=True
                     )
-            if not molecule:
+            else:
                 if len(atomic_data) > 0:
+                    _, _, z_data = redefine_index(atomic_info, atomic_data, z_data)
                     atomic_info, atomic_data, zk_data = redefine_index(atomic_info, atomic_data, zk_data)
                 if len(uniform_data) > 0:
                     uniform_info, uniform_data, zk_data = redefine_index(uniform_info, uniform_data, zk_data)
                 if len(structure_data) > 0:
                     structure_info, structure_data, zk_data = redefine_index(structure_info, structure_data, zk_data)
 
         # harmonics
```

### Comparing `multipie-1.1.8/multipie/model/util/create_pdf.py` & `multipie-1.1.9/multipie/model/util/create_pdf.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/model/util/symmetry_adapted_model_util.py` & `multipie-1.1.9/multipie/model/util/symmetry_adapted_model_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/base/base_atomic_multipole_dataset.py` & `multipie-1.1.9/multipie/multipole/base/base_atomic_multipole_dataset.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/base/base_atomic_multipole_set.py` & `multipie-1.1.9/multipie/multipole/base/base_atomic_multipole_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/util/atomic_orbital_util.py` & `multipie-1.1.9/multipie/multipole/util/atomic_orbital_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/util/atomic_samb_util.py` & `multipie-1.1.9/multipie/multipole/util/atomic_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/util/multipole_util.py` & `multipie-1.1.9/multipie/multipole/util/multipole_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/util/pauli.py` & `multipie-1.1.9/multipie/multipole/util/pauli.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/util/spin_orbital_basis.py` & `multipie-1.1.9/multipie/multipole/util/spin_orbital_basis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/util/structure_samb_util.py` & `multipie-1.1.9/multipie/multipole/util/structure_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/multipole/util/z_samb_util.py` & `multipie-1.1.9/multipie/multipole/util/z_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/response_tensor/response_tensor_pg.py` & `multipie-1.1.9/multipie/response_tensor/response_tensor_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/response_tensor/response_tensor_pg_set.py` & `multipie-1.1.9/multipie/response_tensor/response_tensor_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/response_tensor/util/response_tensor_util.py` & `multipie-1.1.9/multipie/response_tensor/util/response_tensor_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/scripts/create_binary.py` & `multipie-1.1.9/multipie/scripts/create_binary.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/scripts/create_samb.py` & `multipie-1.1.9/multipie/scripts/create_samb.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/symmetry_operation/symmetry_operation.py` & `multipie-1.1.9/multipie/symmetry_operation/symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/symmetry_operation/symmetry_operation_g.py` & `multipie-1.1.9/multipie/symmetry_operation/symmetry_operation_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/symmetry_operation/symmetry_operation_g_set.py` & `multipie-1.1.9/multipie/symmetry_operation/symmetry_operation_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/symmetry_operation/util/symmetry_operation_util.py` & `multipie-1.1.9/multipie/symmetry_operation/util/symmetry_operation_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/tag/tag.py` & `multipie-1.1.9/multipie/tag/tag.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/tag/tag_group.py` & `multipie-1.1.9/multipie/tag/tag_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/tag/tag_irrep.py` & `multipie-1.1.9/multipie/tag/tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/tag/tag_list.py` & `multipie-1.1.9/multipie/tag/tag_list.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/tag/tag_multipole.py` & `multipie-1.1.9/multipie/tag/tag_multipole.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/tag/tag_response_tensor.py` & `multipie-1.1.9/multipie/tag/tag_response_tensor.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/tag/tag_symmetry_operation.py` & `multipie-1.1.9/multipie/tag/tag_symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/tag/tag_wyckoff.py` & `multipie-1.1.9/multipie/tag/tag_wyckoff.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/virtual_cluster/virtual_cluster_pg.py` & `multipie-1.1.9/multipie/virtual_cluster/virtual_cluster_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/virtual_cluster/virtual_cluster_pg_set.py` & `multipie-1.1.9/multipie/virtual_cluster/virtual_cluster_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/wyckoff/wyckoff_g.py` & `multipie-1.1.9/multipie/wyckoff/wyckoff_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie/wyckoff/wyckoff_g_set.py` & `multipie-1.1.9/multipie/wyckoff/wyckoff_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/multipie.egg-info/PKG-INFO` & `multipie-1.1.9/multipie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.1.8
+Version: 1.1.9
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.8
```

### Comparing `multipie-1.1.8/multipie.egg-info/SOURCES.txt` & `multipie-1.1.9/multipie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multipie-1.1.8/setup.cfg` & `multipie-1.1.9/setup.cfg`

 * *Files identical despite different names*


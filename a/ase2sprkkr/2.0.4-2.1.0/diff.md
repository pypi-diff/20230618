# Comparing `tmp/ase2sprkkr-2.0.4.tar.gz` & `tmp/ase2sprkkr-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ase2sprkkr-2.0.4.tar", last modified: Wed Jun  7 21:15:52 2023, max compression
+gzip compressed data, was "ase2sprkkr-2.1.0.tar", last modified: Sun Jun 18 19:58:15 2023, max compression
```

## Comparing `ase2sprkkr-2.0.4.tar` & `ase2sprkkr-2.1.0.tar`

### file list

```diff
@@ -1,159 +1,178 @@
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/
--rw-rw-r--   0 logik     (1000) logik     (1000)     1074 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.4/LICENCE
--rw-rw-r--   0 logik     (1000) logik     (1000)      110 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/MANIFEST.in
--rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/PKG-INFO
--rw-rw-r--   0 logik     (1000) logik     (1000)     4356 2023-03-30 16:14:13.000000 ase2sprkkr-2.0.4/README.md
--rw-rw-r--   0 logik     (1000) logik     (1000)      104 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.4/pyproject.toml
--rw-rw-r--   0 logik     (1000) logik     (1000)      731 2023-06-07 21:15:52.907179 ase2sprkkr-2.0.4/setup.cfg
--rw-rw-r--   0 logik     (1000) logik     (1000)      256 2023-06-07 19:13:11.000000 ase2sprkkr-2.0.4/setup.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.891179 ase2sprkkr-2.0.4/src/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2021-02-10 09:12:38.000000 ase2sprkkr-2.0.4/src/MANIFEST.in
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.891179 ase2sprkkr-2.0.4/src/ase2sprkkr/
--rw-rw-r--   0 logik     (1000) logik     (1000)      817 2023-06-07 17:36:39.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8263 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      286 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/pbc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1311 2023-02-20 17:22:04.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/symbols.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2373 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/visualise.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/asr/
--rw-rw-r--   0 logik     (1000) logik     (1000)       43 2023-06-07 20:32:19.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/asr/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/
--rw-rw-r--   0 logik     (1000) logik     (1000)       86 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4892 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/es_finder.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8391 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/spglib.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/common/
--rw-rw-r--   0 logik     (1000) logik     (1000)       66 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1097 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/alternative_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5389 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    17525 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration_containers.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    42000 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     9642 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/decorators.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1348 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/directory.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      512 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/doc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1114 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/formats.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2858 2022-12-05 17:02:51.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/grammar.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    46421 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/grammar_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1608 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/misc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2221 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/no_output.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    14102 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/options.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6382 2022-09-04 15:14:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/process_output_reader.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2893 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/test_common.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8125 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/test_grammar_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6798 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/unique_values.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/
--rw-rw-r--   0 logik     (1000) logik     (1000)       78 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/
--rw-rw-r--   0 logik     (1000) logik     (1000)      369 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5030 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/arpes.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      690 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/dos.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      659 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/phagen.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      746 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/scf.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    10422 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/sections.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/
--rw-rw-r--   0 logik     (1000) logik     (1000)      726 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/arpes.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      210 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/dos.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      266 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/phagen.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      276 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/scf.in
--rw-rw-r--   0 logik     (1000) logik     (1000)    13368 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/input_parameters.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4541 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/input_parameters_definitions.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2046 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/test_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    12452 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/test_input_parameters.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/
--rw-rw-r--   0 logik     (1000) logik     (1000)       67 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2128 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/output_definitions.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/
--rw-rw-r--   0 logik     (1000) logik     (1000)       50 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      295 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/default.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8303 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/scf.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1649 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/task_result.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-11 17:30:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      985 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/test_output.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/physics/
--rw-rw-r--   0 logik     (1000) logik     (1000)      101 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/physics/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     9561 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/physics/lattice_data.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1865 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/physics/winger_seitz_radii.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/
--rw-rw-r--   0 logik     (1000) logik     (1000)       84 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2989 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/custom_potential_section.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/
--rw-rw-r--   0 logik     (1000) logik     (1000)      334 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3186 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/potential.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/
--rw-rw-r--   0 logik     (1000) logik     (1000)      531 2022-03-11 17:30:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      900 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7295 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/lattice.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      998 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2748 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/occupation.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1326 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/reference_system.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2012 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      833 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/types.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/
--rw-rw-r--   0 logik     (1000) logik     (1000)   265591 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/FePt.new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     3894 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/FePt.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)    22581 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/GeTe.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)   263365 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/Li_scf.new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     9591 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/fp_basscale0.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)   395148 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/fp_new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     5137 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potential_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5236 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potential_sections.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4062 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potentials.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1156 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_2D.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2135 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_custom_section.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3880 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_potential.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1334 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_structure.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/
--rw-rw-r--   0 logik     (1000) logik     (1000)      112 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6553 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/atomic_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5136 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/atoms_region.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3799 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    33787 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/calculator.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4381 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/configuration.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2210 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/io_data.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7669 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/occupations.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      912 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/radial_meshes.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      328 2022-03-14 23:18:04.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/reference_systems.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5323 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    13056 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sprkkr_atoms.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      802 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5647 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/structure.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7511 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sysfile.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      676 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6989 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_calculator.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1965 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3824 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2537 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sysfile.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/
--rw-rw-r--   0 logik     (1000) logik     (1000)       55 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/__init__.py
--rwxrwxr-x   0 logik     (1000) logik     (1000)     2632 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/a2s_visualise_in_struct.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      750 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/test_tools.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      150 2023-06-07 21:12:07.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/version.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/
--rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/PKG-INFO
--rw-rw-r--   0 logik     (1000) logik     (1000)     5307 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/SOURCES.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)        1 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/dependency_links.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)       31 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/requires.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)       18 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/top_level.txt
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/sprkkr/
--rw-rw-r--   0 logik     (1000) logik     (1000)       40 2023-06-07 19:12:36.000000 ase2sprkkr-2.0.4/src/sprkkr/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/tests/
--rw-rw-r--   0 logik     (1000) logik     (1000)     2838 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.4/tests/test.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      468 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.4/tests/test_inputfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1074 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.0/LICENCE
+-rw-rw-r--   0 logik     (1000) logik     (1000)      110 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/MANIFEST.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/PKG-INFO
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4356 2023-03-30 16:14:13.000000 ase2sprkkr-2.1.0/README.md
+-rw-rw-r--   0 logik     (1000) logik     (1000)      104 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.0/pyproject.toml
+-rw-rw-r--   0 logik     (1000) logik     (1000)      779 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/setup.cfg
+-rw-rw-r--   0 logik     (1000) logik     (1000)      256 2023-06-07 19:13:11.000000 ase2sprkkr-2.1.0/setup.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2021-02-10 09:12:38.000000 ase2sprkkr-2.1.0/src/MANIFEST.in
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      890 2023-06-18 15:04:21.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8263 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      286 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/pbc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2370 2023-06-17 14:04:22.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/symbols.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2373 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/visualise.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr/asr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      279 2023-06-08 07:39:18.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/asr/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       86 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4892 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/es_finder.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8391 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/spglib.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/common/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       66 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1097 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/alternative_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5389 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    18435 2023-06-18 18:27:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration_containers.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    43224 2023-06-18 18:16:18.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    10044 2023-06-18 12:13:29.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/decorators.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1348 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/directory.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      512 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/doc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1114 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/formats.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2906 2023-06-18 18:17:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/generated_configuration_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2858 2022-12-05 17:02:51.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1490 2023-06-16 20:05:37.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    16245 2023-06-18 19:18:28.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/arrays.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    10886 2023-06-18 11:03:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/basic.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1734 2023-06-18 19:18:28.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/data.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)        1 2023-06-15 07:45:04.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/functions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    16998 2023-06-18 19:18:28.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/grammar_type.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3624 2023-06-18 18:25:56.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/mixed.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1608 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/misc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2221 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/no_output.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    16385 2023-06-18 19:48:21.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/options.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6382 2022-09-04 15:14:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/process_output_reader.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3395 2023-06-18 12:18:11.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/test_common.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8125 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/test_grammar_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      927 2023-06-17 12:20:25.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/tools.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6798 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/unique_values.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       78 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      369 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5645 2023-06-18 19:34:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/arpes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      690 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/dos.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2279 2023-06-18 11:00:14.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/gilbert.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      659 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/phagen.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      746 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/scf.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    10536 2023-06-18 19:33:50.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/sections.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      726 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/arpes.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      210 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/dos.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      266 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/phagen.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      276 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/scf.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)    13384 2023-06-18 14:47:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/input_parameters.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4541 2023-06-18 11:35:58.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/input_parameters_definitions.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2162 2023-06-18 19:55:56.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/test_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    12772 2023-06-18 18:40:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/test_input_parameters.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       67 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2128 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_definitions.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2036 2023-06-16 20:42:06.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3489 2023-06-18 19:18:42.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files/spc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3413 2023-06-16 19:09:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files_definitions.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       50 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      968 2023-06-18 13:35:35.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/arpes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      295 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/default.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8303 2023-06-18 07:50:22.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/scf.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1649 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/task_result.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-11 17:30:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1034 2023-06-18 19:18:42.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/test_files.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      985 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/test_output.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/physics/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      101 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/physics/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     9561 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/physics/lattice_data.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1865 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/physics/winger_seitz_radii.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       84 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2989 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/custom_potential_section.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      334 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3186 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/potential.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      531 2022-03-11 17:30:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      900 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7295 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/lattice.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      998 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2748 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/occupation.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1326 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/reference_system.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2012 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      833 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/types.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/
+-rw-rw-r--   0 logik     (1000) logik     (1000)   265591 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/FePt.new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3894 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/FePt.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)    22581 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/GeTe.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)   263365 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/Li_scf.new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     9591 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/fp_basscale0.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)   395148 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/fp_new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5137 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potential_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5236 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potential_sections.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4062 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potentials.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1156 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_2D.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2135 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_custom_section.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3880 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_potential.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1334 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_structure.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      112 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6553 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/atomic_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5136 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/atoms_region.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3799 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    37563 2023-06-18 19:18:42.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/calculator.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4381 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/configuration.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2210 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/io_data.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7669 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/occupations.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      912 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/radial_meshes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      328 2022-03-14 23:18:04.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/reference_systems.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5323 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    13056 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sprkkr_atoms.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      802 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5647 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/structure.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7511 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sysfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1394 2023-06-18 13:46:33.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_arpes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      676 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6989 2023-06-18 14:32:45.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_calculator.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1965 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3824 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2537 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sysfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       55 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/__init__.py
+-rwxrwxr-x   0 logik     (1000) logik     (1000)     1997 2023-06-18 12:07:20.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/a2s_plot_output.py
+-rwxrwxr-x   0 logik     (1000) logik     (1000)     2632 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/a2s_visualise_in_struct.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      750 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/test_tools.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      150 2023-06-18 19:19:01.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/version.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/src/ase2sprkkr/visualise/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-06-18 14:02:55.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/visualise/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6607 2023-06-17 12:11:09.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/visualise/plot.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/PKG-INFO
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6096 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/SOURCES.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)        1 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/dependency_links.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)       35 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/requires.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)       11 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/top_level.txt
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/tests/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2838 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.0/tests/test.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      468 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.0/tests/test_inputfile.py
```

### Comparing `ase2sprkkr-2.0.4/LICENCE` & `ase2sprkkr-2.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/PKG-INFO` & `ase2sprkkr-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ase2sprkkr
-Version: 2.0.4
+Version: 2.1.0
 Summary: ASE (atomic simulation environment) interface to SPRKKR
 Home-page: https://ase2sprkkr.github.io/ase2sprkkr/
 Author: Matyáš Novák & Jano Minár
 Author-email: ase2kkr@ntc.zcu.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ase2sprkkr-2.0.4/README.md` & `ase2sprkkr-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/setup.cfg` & `ase2sprkkr-2.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 [options.package_data]
 * = src/**/*.in
 
 [options]
 package_dir = 
 	= src
 packages = find:
-scripts = src/ase2sprkkr/tools/a2s_visualise_in_struct.py
+scripts = 
+	src/ase2sprkkr/tools/a2s_visualise_in_struct.py
+	src/ase2sprkkr/tools/a2s_plot_output.py
 python_requires = >=3.7
 install_requires = 
 	ase
+	asr
 	spglib
 	pyparsing
 	mendeleev
 
 [options.packages.find]
 where = src
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/__init__.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 """ Potential file object for SPRKKR calcualtions """
 from .potentials.potentials import Potential
 
 """ An extension of ASE atoms object """
 from .sprkkr.sprkkr_atoms import SPRKKRAtoms
 
+""" SPRKKR Output File """
+from .outputs.output_files import OutputFile
+
 """ Version of the package """
 from .version import __version__
 
 def _init():
    import ase
    from ase.calculators.calculator import register_calculator_class
    register_calculator_class('sprkkr', SPRKKR)
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/ase/build.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/ase/build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/ase/visualise.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/ase/visualise.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/es_finder.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/es_finder.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/spglib.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/spglib.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/alternative_types.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/alternative_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration_containers.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration_containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,29 @@
       """ Create the container and its members, according to the definition """
       super().__init__(definition, container)
       """
       The members of the container, in a form of ``{obj.name : obj}``
       """
       self._init_members_from_the_definition()
 
+  def copy(self, copy_values:bool=False):
+      """ Create a copy of the container
+
+      Parameters
+      ----------
+      copy_values
+        If true, the copy of values is done, so their modifications do not affects the container.
+        (e.g. for numpy arrays)
+      """
+      d=self._definition
+      vals=self.as_dict(copy=copy_values)
+      out =d.result_class(definition=d)
+      out.set(vals, unknown='add')
+      return out
+
   def _init_members_from_the_definition(self):
       self._members = OrderedDict()
       """
       Non-hidden members of the containers, accesible via sanitized names.
       I.e. via names with whitespaces and other special characters replaced by underscore.
       These sanitized names are then used as names for "attributes" of this container, to
       make the members accesible via ``<container>.<member>`` notation.
@@ -96,29 +111,35 @@
       """
       return itertools.chain(self._interactive_members.keys(), super().__dir__())
 
   def __contains__(self, name):
       """ The check for existence of a member with the given name."""
       return name in self._members
 
-  def clear(self, do_not_check_required=False):
+  def clear(self, do_not_check_required=False, call_hooks=True, generated=None):
       """
       Erase all values (or reset to default) from all options in the container
       (ad subcontainers)
 
       Parameters
       ----------
       do_not_check_required: bool
-      Do not check validity of the values after clearing. If ``False`` (default)
-      is passed as this argument, the required option without a default value
-      (or a section containing such value) throw an exception, which prevents the
-      clearing (neverthenless, previous values in the section will be cleared anyway).
+        Do not check validity of the values after clearing. If ``False`` (default)
+        is passed as this argument, the required option without a default value
+        (or a section containing such value) throw an exception, which prevents the
+        clearing (neverthenless, previous values in the section will be cleared anyway).
+
+      call_hooks: bool
+        If False, the cleared values do not raise theirs hooks
+
+      generated: bool
+        If True
       """
       for i in self._members.values():
-          i.clear(do_not_check_required)
+          i.clear(do_not_check_required, call_hooks=call_hooks, generated=False if generated is None else generated)
 
   def get(self, name=None, unknown='find'):
       """
       Get the value, either of self or of a child of a given name.
 
       Parameters
       ----------
@@ -147,15 +168,15 @@
       else:
          val = None
       if not val:
          raise ValueError(f"No {name} member of {self}")
       return val.get()
 
 
-  def set(self, values:Union[Dict[str,Any],str,None]={}, value=None, *, unknown='find', **kwargs):
+  def set(self, values:Union[Dict[str,Any],str,None]={}, value=None, *, unknown='find', error=None, **kwargs):
       """
       Set the value(s) of parameter(s). Usage:
 
       > input_parameters.set({'NITER': 5, 'NE': [10]})
       or
       > input_parameters.set(NITER=5, NE=[10])
 
@@ -182,28 +203,30 @@
          values = { values : value }
       elif value is not None:
          raise ValueError("If value argument of Container.set method is given,"
          " the values have to be string name of the value")
 
       def set_value(name, value):
         if '.' in name:
-          section, name = name.split('.')
-          self._members[section].set({name:value})
+          section, name = name.split('.', 1)
+          self._members[section].set({name:value}, unknown=unknown, error=error)
         if name not in self._members:
            if unknown == 'find':
               option = self._find_value(name)
               if option:
-                 option.set(value)
+                 option.set(value, error=error)
                  return
+           if unknown == 'ignore':
+               return
            if not unknown == 'add':
               raise KeyError("No option with name {} in {}".format(name, str(self)))
               return
            self.add(name, value)
         else:
-           self._members[name].set(value, unknown=unknown)
+           self._members[name].set(value, unknown=unknown, error=error)
 
       if values:
         try:
            items = values.items()
         except AttributeError:
           raise ValueError('Only a dictionary can be assigned to a section.')
         for i,v in items:
@@ -250,31 +273,34 @@
           self._interactive_members[iname] == member:
             del self._interactive_members[iname]
 
   def __iter__(self):
       """ Iterate over all members of the container """
       yield from self._members.values()
 
-  def as_dict(self, only_changed:Union[bool,str]='basic'):
+  def as_dict(self, only_changed:Union[bool,str]='basic', generated:bool=False, copy=False):
       """
       Return the content of the container as a dictionary.
       Nested containers will be transformed to dictionaries as well.
 
       Parameters
       ----------
       only_changed
         Return only changed values, or all of them?
         If True, return only the values, that differ from the defaults.
         If False, return all the values.
         The default value 'basic' means, return all non-expert values
         and all changed expert values.
+
+      generated: bool
+        Add generated values
       """
       out = OrderedDict()
       for i in self:
-          value = i.as_dict(only_changed)
+          value = i.as_dict(only_changed, generated, copy)
           if value is not None:
               out[i.name] = value
       return out or None
 
   def to_string(self):
       """
       Return the configuration (problem definition) in a string.
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration_definitions.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 e.g. an :py:class:`Option<ase2sprkkr.common.options.Option>` or
 :py:class:`Section<ase2sprkkr.common.configuration_containers.Section>`
 ), or write such object to a file.
 """
 
 from ..common.grammar_types  import type_from_type, type_from_value, GrammarType
 from ..common.grammar  import delimitedList, end_of_file, generate_grammar
-import pyparsing as pp
 from ..common.misc import OrderedDict
 from .configuration_containers import Section
 from .options import Option, DangerousValue
+from .decorators import cache
+
 import numpy as np
+import pyparsing as pp
 import inspect
-from .decorators import cache
 import itertools
 import builtins
 from typing import Dict, Union
 
 #:This serves just for dealing with various pyparsing versions
 _parse_all_name = 'parse_all' if \
   'parse_all' in inspect.getfullargspec(pp.Or.parseString).args \
@@ -84,15 +85,15 @@
    the behavior.
    """
 
    def __init__(self, name, alternative_names=None,
                 is_optional=False, is_hidden=False, is_expert=False,
                 name_in_grammar=None, info=None, description=None,
                 write_alternative_name:bool=False,
-                result_class=None
+                result_class=None,
                 ):
        """
        Parameters
        ----------
         name: str
           Name of the value/section
 
@@ -279,25 +280,30 @@
    def can_be_repeated(self):
        """ If True, the item can be repeated in the parsed file.
        This behavior have currently the values with is_numbered_array property = True.
        This function is to be redefined in descendants
        """
        return False
 
+   is_generated = False
+   """ Generated values are computed on the fly from the other data """
+
 class ValueDefinition(BaseDefinition):
 
   result_class = Option
 
   name_in_grammar = None
 
   def __init__(self, name, type=None, default_value=None, alternative_names=None,
                fixed_value=None, required=None, info=None, description=None,
                is_hidden=False, is_optional=None, is_expert=False, is_numbered_array:bool=False,
+               is_always_added:bool=None,
                name_in_grammar=None, name_format=None, expert=None,
-               write_alternative_name:bool=False, result_class=None):
+               write_alternative_name:bool=False, result_class=None,
+               ):
     """
     Definition of a configuration value.
 
     Parameters
     ----------
     name: str
       Name of the configuration value
@@ -343,14 +349,18 @@
       default value.
 
     is_numbered_array
       Such values can contains (sparse) arrays. In the resulting ouput, the
       members of the array are in the form NAME1=..., NAME2=..., ... The default
       value for missing number can appear in the form NAME=...
 
+    is_always_added
+      If False, add the value, only if its value is not the default value.
+      Default None means False for expert values, True for the others.
+
     name_in_grammar: bool or None
       The value in the conf file is prefixed by <name><name_value_delimiter>
       If None, the default type value (type.name_in_grammar) is used
 
     name_format: str or None
       The way how the name is written
 
@@ -371,14 +381,19 @@
        else:
           default_value=expert
        is_expert = True
        required = False
     elif type is None:
        raise TypeError("The data-type of the configuration value is required.")
 
+    if is_always_added is None:
+       self.is_always_added = not is_expert
+    else:
+       self.is_always_added = is_always_added
+
     if fixed_value is None:
        self.is_fixed = False
     else:
        default_value = fixed_value
        self.is_fixed = True
 
     if default_value is None and not isinstance(type, (GrammarType, builtins.type)):
@@ -423,14 +438,18 @@
     self.required = self.default_value is not None if required is None else required
     self.name_format = name_format
 
   type_from_type_map = {}
   """ Redefine this in descendants, if you need to create different types that the defaults to be
   'guessed' from the default values """
 
+  def enrich(self, option):
+      """ The Option can be enriched by the definition, e.g. the docsting can be extended. """
+      self.type.enrich(option)
+
   @property
   def formated_name(self):
     name = next(iter(self.alternative_names)) if self.write_alternative_name else self.name
     if self.name_format:
        return "{:{}}".format(name, self.name_format)
     return name
 
@@ -460,16 +479,18 @@
        out+=f" ≝ {value}"
 
     flags = []
     if self.is_optional:
        flags.append('optional')
     if self.is_hidden:
        flags.append('hidden')
-    if self.is_hidden:
+    if self.is_expert:
        flags.append('expert')
+    if self.is_expert == self.is_always_added:
+       flags.append('always add' if self.is_expert else 'add non-default')
     if self.is_numbered_array:
        flags.append('array')
     if self.is_fixed:
        flags.append('read_only')
     if flags:
        flags = ', '.join(flags)
        out+= f"  ({flags})"
@@ -507,15 +528,15 @@
   def validate(self, value, why='set'):
     if value is None:
        if self.required:
           raise ValueError(f"The value is required for {self.name}, cannot set it to None")
        return True
     if self.is_fixed and not np.array_equal(self.default_value, value):
        raise ValueError(f'The value of {self.name} is required to be {self.default_value}, cannot set it to {value}')
-    self.type.validate(value, self.name, why='set')
+    self.type.validate(value, self.name, why=why)
 
   def convert_and_validate(self, value, why='set'):
     value = self.type.convert(value)
     self.validate(value, why)
     return value
 
   @property
@@ -670,14 +691,28 @@
        out = super()._get_copy_args()
        if self.is_fixed:
            out['fixed_value'] = out['default_value']
        return out
 
   _copy_excluded_args = BaseDefinition._copy_excluded_args + ['fixed_value']
 
+  def copy_value(self, value, all_values=False):
+      """ Creates copy of the value
+
+      Parameters
+      ----------
+      values
+        The value to copy
+
+      all_values
+        Wheter, for a numbered array, a whole dict is supplied
+      """
+      if not all_values or not self.is_numbered_array:
+          return self.type.copy_value(value)
+      return { k:self.type.copy_value(v) for v in values }
 
 def add_excluded_names_condition(element, names):
     """ Add the condition to the element, that
     its value is not any of given names """
     if not names:
        return
     names = set((i.upper() for i in names))
@@ -899,17 +934,19 @@
          """ This function iterates over the items of the container, joining all the without name_in_grammar with the previous ones. """
 
          def repeated_grammars():
              """ If the item can be repeated, do it here - we don't know, whether there is a fixed order in any way
              (e.g. the item is followed by the items without name in grammar)
              """
              for i in self._members.values():
+                 if i.is_generated:
+                     continue
                  g = i._grammar(allow_dangerous)
                  if i.can_be_repeated():
-                    g = delimitedList(g, delimiter)
+                     g = delimitedList(g, delimiter)
                  yield i,g
 
          it = iter(repeated_grammars())
          head_item, grammar_chain = next(it)
 
          for item, grammar in it:
              if item.name_in_grammar:
@@ -932,15 +969,15 @@
            first = pp.Empty().addCondition(lambda loc, toks: loc == init.location)
            if custom_value:
               cvs = pp.ZeroOrMore(custom_value + delimiter).setName('<custom...>')
               after = delimiter + cvs
            else:
               after = pp.Forward() << delimiter
            after.addCondition(lambda loc, toks: loc != init.location)
-           inter = first | after
+           inter = (first | after).setName('?')
 
            def sequence():
                for head,g in grammars():
                    g = inter + g
                    if head.is_optional:
                       g = pp.Optional(g)
                    yield g
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/decorators.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def __init__(self, method=None):
         self.fget = method
 
     def __get__(self, instance, cls=None):
         return self.fget(cls)
 
 
-def add_to_signature(func, prepend=False, self_name='self'):
+def add_to_signature(func, prepend=False, excluding=None):
   """
   Add the arguments in the ``func`` function to the list of arguments
   of the resulting function (as keyword_only arguments)
   The modified function has to have its arguments defined as
   in the following example:
 
   .. code-block::
@@ -138,26 +138,28 @@
 
   Parameters
   ----------
   func
     A function, whose parameters will be added to the resulting function signature.
 
   prepend
-    If true, the new positional arguments will be the first.
-    If false, they will be after the parents positional arguments.
-    The same-named arguments just alter the properties of the "old"
-    arguments, retaining their position.
-
-  self_name
-    Name of the self-parameter (for object method), that should be the first, even
-    if ``prepend`` is True.
-    Default self, set to None if you do not want special handling of self parameter
-    (i.e. if your function has the first argument named *self* and it is not a method).
+    If True, the new positional arguments will be the first.
+    If False, they will be after the parents positional arguments.
 
+    The same-named arguments can be given as keyword-only - then
+    they just alter the properties of the "old" arguments, retaining their position.
+    If they are given as regular ones, they takes their new position, too.
+
+  excluding
+    Do not add this arguments
   """
+  if not excluding:
+     excluding=[]
+  elif isinstance(excluding, str):
+     excluding=[ excluding ]
 
   signature = inspect.signature(func)
   pars = list( signature.parameters.values())
   P = inspect.Parameter
 
   arg_ar = arg_kw = None
   for i in pars:
@@ -175,45 +177,52 @@
 
       used = set()
       def use(i):
           nonlocal used
           used.add(i.name)
           return i
 
-      old_pars = [ use(new_pars[i.name]) if i.name in new_pars else i for i in pars ]
-      add_pars = [ i for i in new_pars.values() if i.name not in used ]
+      if prepend:
+        old_names = set((i.name for i in pars if i.name not in excluding))
+        old_pars = [ use(i) for i in new_pars.values() \
+                     if i.kind != P.KEYWORD_ONLY or i.name not in old_names ]
+        def add_pars():
+            for i in pars:
+                if i in excluding:
+                   continue
+                if i.name not in new_pars:
+                   yield i
+                else:
+                   n=new_pars[i.name]
+                   if n.kind != P.KEYWORD_ONLY:
+                       continue
+                   #keyword only parameters retain the old position, taken new default and annotation
+                   P(i.name, i.kind, default=n.default, annotation=n.annotation)
+                   yield n
+        add_pars = [ i for i in add_pars() ]
+      else:
+        old_pars = [ use(new_pars[i.name]) if i.name in new_pars else i for i in pars if i.name not in excluding ]
+        add_pars = [ i for i in new_pars.values() if i.name not in used ]
 
       #the easy and fast way - only keyword arguments are present, the function can be called as is,
       #just make its signature pretty
       for i in add_pars:
         if i.kind != P.KEYWORD_ONLY:
            break
       else:
         result = list(heapq.merge(old_pars, add_pars, key = lambda x: x.kind))
         result = new_sig.replace(parameters = result)
         mod_func.__signature__ = result
         return mod_func
 
-      #the hard way, the arguments have to be rearranged
-      if prepend:
-         if old_pars and old_pars[0].name == self_name:
-            self = old_pars[0]
-            del old_pars[0]
-         else:
-            self = None
-         result = heapq.merge(add_pars, old_pars, key = lambda x: x.kind)
-         if self:
-            result = itertools.chain((self,), result)
-      else:
-         result = heapq.merge(old_pars, add_pars, key = lambda x: x.kind)
-         self = None
-
+      result = heapq.merge(old_pars, add_pars, key = lambda x: x.kind)
       result = list(result)
       result=new_sig.replace(parameters = result)
 
+
       @functools.wraps(mod_func)
       def wrapper(*args, **kwargs):
           ba=result.bind(*args, **kwargs)
           ba.apply_defaults()
           nargs = []
           nkwargs = {}
           for k,v in ba.arguments.items():
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/directory.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/directory.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/doc.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/doc.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/formats.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/formats.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/grammar.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/init_tests.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/misc.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/misc.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/no_output.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/no_output.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/options.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,33 +81,38 @@
           The container, that owns the object
 
       value: mixed
           The value of the option.
       """
       super().__init__(definition, container)
       self._hook = None
-      self._definition.type.enrich(self)
+      self._definition.enrich(self)
       self._value = value
 
   def __call__(self, all_values:bool=False):
       """
       Return the value of the option.
 
       Parameters
       ----------
       all_values: For numbered_array (see :class:`ConfigurationDefinition.is_numbered_array <ConfigurationDefinition>`,
       pass True as this argument to obtain array of all values. If False (the default) is given,
       only the 'wildcard' value (i.e. the one without array index, which is used for the all values
       not explicitly specified) is returned.
       """
+      if self._definition.is_generated:
+         return self._definition.getter(self)
+
       value = self._unpack_value(self._value)
       if value is not None:
           if self._definition.is_numbered_array and not all_values:
               return value.get('def', self.default_value)
           return value
+      if hasattr(self, '_result'):
+          return self.result
       if self._definition.is_numbered_array and all_values and self.default_value is not None:
           return { 'def' : self.default_value }
       return self.default_value
 
   def is_dangerous(self):
       """ Return, whether the option is set to a dangerous value, i.e. a value
       that bypass the validation. """
@@ -135,90 +140,117 @@
       """ Return default value for the option.
       The function is here, and not in the definition, since the default value can be given
       by callable, that accepts the Option as argument. This possibility is used in ase2sprkkr,
       when the default values of some options are generated from the underlined Atoms object
       """
       return self._definition.get_value(self)
 
-  def set(self, value, *, unknown=None):
+  def set(self, value, *, unknown=None, error=None):
       """
       Set the value of the option.
 
       Parameters
       ----------
       value: mixed
         The new value of the option.
 
       unknown: str or None
         A dummy argument to make the method compatibile with
         ase2sprkkr.sprkkr.common.configuration_containers.ConfigurationContainer.set()
+
+      error:
       """
+      if self._definition.is_generated:
+          return self._definition.setter(self, value)
+
       if value is None:
-          return self.clear()
+          try:
+              return self.clear()
+          except ValueError:
+              if not error=='ignore': raise
+              return
       elif self._definition.is_numbered_array:
         if isinstance(value, dict):
            self.clear(do_not_check_required=value, call_hooks=False)
            for k,v in value.items():
-               self._set_item(k, v)
+               self._set_item(k, v, error)
         else:
-           self._set_item('def', value)
-      elif isinstance(value, DangerousValue):
-         self._value = value
+           self._set_item('def', value, error)
       else:
-        self._value = self._definition.convert_and_validate(value)
+         try:
+             self._value = self._pack_value(value)
+         except ValueError:
+             if not error=='ignore': raise
       self._post_set()
 
   def _post_set(self):
       """ Thus should be called after all modifications """
       if hasattr(self,'_result'):
         del self._result
       if self._hook:
         self._hook(self)
 
   def _check_array_access(self):
       """ Check, whether the option is numbered array and thus it can be accessed as array using [] """
-      if not self._definition.is_numbered_array:
+      if not self._definition.is_numbered_array and not self._definition.type.array_access:
           raise TypeException('It is not allowed to access {self._get_path()} as array')
 
   def __setitem__(self, name, value):
       """ Set an item of a numbered array. If the Option is not a numbered array, throw an Exception. """
+      if self._definition.is_generated:
+          self._definition.setter(self, value, name)
+          return
+
       self._check_array_access()
 
-      if isinstance(name, (list, tuple)):
-          for n in name:
-            self._set_item(n, value)
-      elif isinstance(name, slice):
-         if slice.stop is None:
-             raise KeyError("To get/set values in a numbered array using slice, you have to specify the end index of the slice")
-         for n in range(name.stop)[name]:
-             self._set_item(n, value)
+      if not self._definition.is_numbered_array:
+          self()[name]=value
+          self.validate(why='set')
       else:
-         self._set_item(name, value)
+        if isinstance(name, (list, tuple)):
+            for n in name:
+              self._set_item(n, value)
+        elif isinstance(name, slice):
+           if slice.stop is None:
+               raise KeyError("To get/set values in a numbered array using slice, you have to specify the end index of the slice")
+           for n in range(name.stop)[name]:
+               self._set_item(n, value)
+        else:
+           self._set_item(name, value)
       self._post_set()
 
-  def _set_item(self, name, value):
+  def _set_item(self, name, value, error=None):
       """ Set a single item of a numbered array. For internal use - so no sanity checks """
       if self._value is None:
          self._value = {}
       if name != 'def':
          try:
             name = as_integer(name)
          except TypeError as e:
             raise KeyError('Numbered array indexes can be only integers, lists or slices') from e
 
       if value is None:
          del self._value[name]
          if not self._value:
             self._value = None
       else:
-         self._value[name] = self._pack_value(value)
+         try:
+            self._value[name] = self._pack_value(value)
+         except ValueError:
+            if error!='ignore': raise
 
   def __getitem__(self, name):
       """ Get an item of a numbered array. If the Option is not a numbered array, throw an Exception. """
+      if self._definition.is_generated:
+          self._definition.getter(self, name)
+          return
       self._check_array_access()
+      if not self._definition.is_numbered_array:
+          return self()[name]
+
       if isinstance(name, (list, tuple)):
           return [ self._getitem(n) for n in name ]
       elif isinstance(name, slice):
          if slice.stop is None:
              raise KeyError("To get/set values in a numbered array using slice, you have to specify the end index of the slice")
          return [ self._getitem(n) for n in range(name.stop)[name] ]
       return self._getitem(name)
@@ -247,14 +279,17 @@
          pass
       else:
          value = self._definition.convert_and_validate(value)
       return value
 
   def __hasitem__(self, name):
       self._check_array_access()
+      if not self._definition.is_numbered_array:
+          return name in self()
+
       if self._value is None:
          return False
       value = self._unpack_value(self._value)
       return name in value
 
   def get(self):
       """ Return the value of self """
@@ -281,91 +316,127 @@
   def result(self, value):
       self._result = value
 
   def clear_result(self):
       if hasattr(self, '_result'):
           del self._result
 
-  def clear(self, do_not_check_required=False,call_hooks=True):
+  def clear(self, do_not_check_required=False, call_hooks=True, generated=True):
       """ Clear the value: set it to None """
-      if not self._definition.type.has_value:
-         return
-      if self._definition.default_value is None and not do_not_check_required and self._definition.required:
-         raise ValueError(f'Option {self._get_path()} must have a value')
-      self._value = None
-      self.clear_result()
+      if self._definition.is_generated:
+          if not generated:
+             return
+          self._definition.setter(self, None)
+      else:
+          if not self._definition.type.has_value:
+             return
+          if self._definition.default_value is None and not do_not_check_required and self._definition.required:
+             raise ValueError(f'Option {self._get_path()} must have a value')
+          self._value = None
+          self.clear_result()
       if call_hooks:
         self._post_set()
 
   def is_changed(self) -> bool:
       """ True, if the value is set and the value differs from the default """
       return self.value_and_changed()[1]
 
+  def is_set(self) -> bool:
+      """ True, if the value is set (even equal to the default value) """
+      return self._value is not None
+
   def _save_to_file(self, file):
       """ Write the name-value pair to the given file, if the value
       is set. """
       d = self._definition
+      if d.is_generated:
+         return
 
       if not d.type.has_value:
          return d.write(file, None)
       elif self.is_dangerous():
          value = self._value
       else:
          value = self.result
-         if value is None or (d.is_expert and self.is_it_the_default_value(value)):
+         if value is None or (not d.is_always_added and self.is_it_the_default_value(value)):
           return
       return d.write(file, value)
 
   def validate(self, why='save'):
-      if self.is_dangerous():
-          return True
       d = self._definition
+      if d.is_generated or self.is_dangerous():
+         return
+
       if d.type.has_value:
-        value = self()
-        if value is None:
-           if not d.is_optional:
-               name = self._get_root_container()
-               raise Exception(f'Value {self._get_path()} is None and it is not an optional value. Therefore, I cannot save the {name}')
+
+        def vali(value):
+          if value is None:
+             if not d.is_optional:
+                 name = self._get_root_container()
+                 raise Exception(f'Value {self._get_path()} is None and it is not an optional value. Therefore, I cannot save the {name}')
+          else:
+             d.validate(value, why)
+
+        if why == 'set':
+           vali(self())
         else:
-           d.type.validate(value, why)
+           value = self.result
+           if d.is_numbered_array:
+              for i in value.values():
+                  vali(i)
+           else:
+              vali(value)
+
 
   @property
   def name(self):
       return self._definition.name
 
-  def as_dict(self, only_changed: Union[bool,str]='basic'):
+  def as_dict(self, only_changed: Union[bool,str]='basic', generated:bool=False, copy:bool=False):
       d = self._definition
-      if only_changed and (only_changed!='basic' or d.is_expert):
+      if d.is_generated and not generated:
+           return None
+      if only_changed and (only_changed!='basic' or d.is_always_added):
            v,c = self.value_and_changed()
-           return v if c else None
-      return self(all_values=True)
+           if not c:
+                return None
+      else:
+           v = self(all_values=True)
+      if copy:
+           v = self._definition.copy_value(v, all_values=True)
+      return v
 
   def value_and_changed(self):
       """ Return value and whether the value was changed
 
           Returns
           -------
           value:mixed
             The value of the options (return all values for 'numbered array')
 
           changed:bool
             Whether the value is the same as the default value or not
       """
+      if self._definition.is_generated:
+          return self(), False
+
       value = self._unpack_value(self._value)
       if value is not None:
          return value, not self.is_it_the_default_value(value)
       if self._definition.is_numbered_array:
          return {'def' : self.default_value}, False
       else:
          return self.default_value, False
 
   def is_it_the_default_value(self, value):
       """ Return, whether the given value is the default value. For
       numbered array, only the wildcard value can be set and this value
       have to be the same as the default. """
+      if self._definition.is_generated:
+          return True
 
       default = self.default_value
       d = self._definition
       if d.is_numbered_array:
           return 'def' in value and len(value) == 1 and \
                   d.type.is_the_same_value(value['def'], default)
       else:
@@ -376,28 +447,37 @@
       if self._definition.name == name:
          return self
 
   def get_path(self):
       return self._get_path()
 
   def __repr__(self):
-      v = self._value
-      if v is None:
+      if self._definition.is_generated:
+         v = self()
+         o = ' (generated)'
+      else:
+         v = self._value
+         o = None
+
+      if o is None and v is None:
          v = self.default_value
-         if v:
+         if v is not None:
             o=' (default)'
-            v=' = '+str(v)
-         else:
-            o='out'
-            v=''
+
+      if v is None:
+        if o:
+           o='out' + o
+        else:
+           o='out'
+        v=''
       else:
-          v=' = ' + str(v)
-          o=''
+         v=' = '+str(v)
 
-      return f"<Option {self._get_path()} of type {self._definition.type} with{o} value{v}>"
+      type = '(generated)' if self._definition.is_generated else f'of type {self._definition.type}'
+      return f"<Option {self._get_path()} {type} with{o} value{v}>"
 
 class CustomOption(Option):
   """ An user-added option (configuration value). It can be removed from the section. """
 
   def remove(self):
       """ Remove me from my "parent" section """
       self._container.remove_member(self._definition.name)
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/process_output_reader.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/process_output_reader.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/init_tests.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/test_common.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/test_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,26 +30,34 @@
 
     @add_to_signature(f, prepend=True)
     def ff(c, *args, **kwargs):
         return c,f(*args,**kwargs)
 
     self.assertEqual( ('c',('a',2, {'d':'d', 'e':'e'})),
                        ff('c', 'a', d='d', e='e'))
-
     def f(c=1, d=5):
         return c,d
 
     @add_to_signature(f, prepend=True)
     def ff(a=2, d='d', *args, **kwargs):
         return a,  f(d=d, *args, **kwargs)
 
+    self.assertEqual( ('a', (1, 'c')),
+                      ff('a', 'c')
+                    )
+
+    @add_to_signature(f, prepend=True)
+    def ff(a=2, *args, d='d', **kwargs):
+        return a,  f(d=d, *args, **kwargs)
+
     self.assertEqual( ('a', ('c', 'd')),
                       ff('a', 'c')
                     )
 
+
     def f(*args):
        return args
 
     @add_to_signature(f)
     def ff(a,*args):
        return a, f(*args)
 
@@ -75,14 +83,24 @@
 
     @add_to_signature(lambda:None)
     def ff(a, *args, c, **kwargs):
         return a,c
     self.assertEqual((2,1), ff(2,c=1) )
 
 
+    def f(a=1, b=2):
+        return a,b
+
+    @add_to_signature(f, excluding='b')
+    def ff(c=1, *args, **kwargs):
+        return c,*f(b=5, *args, **kwargs)
+    self.assertEqual((7,3,5), ff(3,7))
+    self.assertEqual((7,3,5), ff(3,c=7))
+    self.assertEqual((7,3,5), ff(a=3,c=7))
+
 
   def test_asyncio_file_reader(self):
     with tempfile.TemporaryFile(mode='w+b') as tfile:
       tfile.write(b"""First line\nSecond line\nHi, this is a very long file!! really!!! 12345123456789""")
       tfile.seek(0)
       ar = AsyncioFileReader(tfile, buffersize=5)
       self.assertAsyncEqual(b"First line\n", ar.readline())
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/test_grammar_types.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/test_grammar_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/common/unique_values.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/common/unique_values.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/arpes.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/arpes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ ARPES task input parameters definition """
 from ...common.grammar_types  import *
 from .sections import *
 from ..input_parameters_definitions import \
     InputParametersDefinition as InputParameters, \
     InputValueDefinition as V, \
     InputSectionDefinition as Section
+from ...sprkkr.sprkkr_grammar_types import Site
 
 input_parameters = InputParameters(
     'arpes', [
     CONTROL('ARPES'),
     TAU,
     ENERGY.copy([
         V('EMINEV', -10., info='Minimum of the energy window in eV with respect to the Fermi level'),
@@ -19,24 +20,27 @@
       ],
       remove = ['EMIN'],
       defaults = { 'GRID' : 1, 'NE' : 300 }
     ),
 
     SITES.copy(defaults = {'NL' : 4 }),
 
-    TASK('ARPES').copy([
-      V('STRVER', 0),
-      V('IQ_AT_SURF', 2),
+    Section('TASK', [
+      V('TASK', DefKeyword({
+        'ARPES' : 'Angle resolved photoemission spectroscopy',
+        'AIPES' : 'Angle integrated photoemission spectroscopy',
+        'SPLEED' : 'Spin polarized LEED (experimental feature)',
+        'BAND'  : 'band structure calculations (experimental feature)'
+      }), name_in_grammar=False, info='Type of the calculation'),
+      V('IQ_AT_SURF', Site.I, 1),
       V('MILLER_HKL', SetOf(int, length=3), [0,0,1]),
-      V('NTMP', 1),
-      V('TMPMIN', 11.),
-      V('CTMPMAX', 11.),
-      V('CTMPMAX', 11.),
-      V('VIBRA', flag, True),
-      V('CNVIBRA', 14),
+      V('CRYS_VEC', True, info='Miller indices with respect to crystalographic primitive vectors'),
+
+      V('STRVER', 1, is_expert=True, is_always_added=True, info="Set to 0 to supply the ARPES input file 'struc.inp' manually (and do not generate it)."),
+      V('INPVER', 1, is_expert=True, is_always_added=True, info='Set to 0 to use an old input.inp from old rslab'),
     ]),
 
     Section('SPEC_PH', [
       V('THETA', 45.),
       V('PHI', 0.),
       V('POL_P', DefKeyword('P', 'S', 'C+', 'C-'), info='Polarization of the light'),
       V('EPHOT', 6675., info='Photon energy in eV'),
@@ -64,15 +68,15 @@
           1: 'variable'
           }), is_expert=True, required=False, info='Photon azimuth angle type'),
       V('THETA_FIX', float, is_expert=True, info='Light and electrons are at fixed polarization angle')
     ]),
 
     Section('SPEC_EL', [
       V('THETA', Range(float), 45., info='Scattering angle'),
-      V('PHI', Range(float), 0, info='Scattering angle'),
+      V('PHI', Range(float), 0., info='Scattering angle'),
       V('NT', 1, info='Number of angular values for a rotation in polar coordinate.'),
       V('NP', 1, info='Number of angular values for a rotation in azimuth coordinate.'),
       V('POL_E', DefKeyword('PZ')),
       V('SPOL', int, required=False),
       V('PSPIN', SetOf(float, length=3), required=False),
       #expert
       V('TYP', Keyword({0: "i(e) diagram",
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/dos.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/dos.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/phagen.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/phagen.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/scf.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/scf.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/sections.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/sections.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
   Return
   ------
   CONTROL: InputSectionDefinition
   """
 
   return Section('CONTROL',[
-      V('DATASET', str, 'case', required = True, info="The custom field for the description of the problem."),
+      V('DATASET', str, 'case', required = True, info="The custom field for the description of the problem - the output files will have called 'DATASET.<ext>'."),
       V('ADSI', DefKeyword(ADSI), required = True, info="Type of the computation."),
       V('POTFIL', str, required=True, info="The potential file (see SPRKKR documentation for its format). It isn't necessary to set it, it will be set by the calculator."),
       V('KRWS', int, required=False),
       V('PRINT', Integer(min=0, max=5), default_value=0, info="Verbosity of the output (0-5). Do not affect the results in any way, just the amount of the printed output."),
       V('NONMAG', False, info="Set this flag, if it is known that the system considered is non-magnetic. This leads to a higher symmetry and a faster calculation. ")
   ])
 
@@ -167,26 +167,29 @@
   V('SOC', 1.0, info='Scale the strength of the spin-orbit coupling for atom type.', is_numbered_array=True),
   ], is_expert=True, is_optional=True, info=
       """If not specified otherwise the programs of the SPRKKR-package assume that a magnetic system should be treated in a fully relativistic way. By setting the parameter SP-SREL a slightly faster scalar relativistic calculation can be done instead for a magnetic system.""",
 )
 """MODE Section definition"""
 
 
-def TASK(TASK):
+def TASK(task, add = []):
   """ Create the definition of the CONTROL section of the task input file.
 
   Parameters
   ----------
   TASK: string
     the default value for the TASK parameter of the resulting section
 
   Return
   ------
   TASK: InputSectionDefinition
   """
+  if isinstance(task, str):
+     task = DefKeyword(task)
+
   return Section('TASK', [
-    V('TASK', DefKeyword(TASK), name_in_grammar=False)
-  ])
+    V('TASK', task, name_in_grammar=False)
+  ] + add)
 
 __all__ = [
     'CONTROL', 'TAU', 'ENERGY', 'SCF', 'SITES', 'TASK', 'STRCONST', 'CPA', 'MODE'
 ]
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/arpes.in` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/arpes.in`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/input_parameters.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/input_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,11 +370,11 @@
   def change_task(self, task):
       """ Change the task to the given task. Retain the value of the options,
       that are present in the new task.
       """
       vals = self.to_dict()
       self._definition = self.task_definition(task)
       self._init_members_from_the_definition()
-      self.set(vals, unknown = 'ignore')
+      self.set(vals, unknown = 'ignore', error='ignore')
 
 #at least, to avoid a circular import
 from ..sprkkr import calculator
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/input_parameters_definitions.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/input_parameters_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/init_tests.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/test_definitions.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/test_definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,17 @@
           name = i[:-3]
           check(t, name)
           t = InputParameters.from_file(filename)
           check(t, name)
 
           if name == 'scf':
              self.assertFalse('MODE' in t.to_string())
+          if name == 'arpes':
+             for i in [ 'AIPES', 'SPLEED', 'BAND' ]:
+                 t.TASK.TASK = i
 
         except Exception as e:
           raise Exception(f'Parsing of "{i}" failed with the reason: \n {e}').with_traceback(e.__traceback__)
 
       td = InputParameters.definitions['PHAGEN']
       td['TASK']['TASK'].default_value = 'scf'
       t = td.read_from_file(os.path.join(path,'phagen.in'))
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/test_input_parameters.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/test_input_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,14 +275,23 @@
     self.assertTrue(isinstance(ips.ENERGY.NXXX, CustomOption))
     ips.ENERGY.NXXX.set(5)
     self.assertEqual(ips.ENERGY.NXXX(), 5)
     ips.ENERGY.NXXX.remove()
     self.assertFalse(hasattr(ips.ENERGY, 'NXXX'))
 
     self.assertEqual(ips['ENERGY'].NE(), np.array((300,200)))
+    cps = ips.copy(copy_values=True)
+    cps.ENERGY.NE[0]=100
+    self.assertEqual(ips['ENERGY'].NE(), np.array((300,200)))
+    dps = cps.copy()
+    dps.ENERGY.NE[0]=150
+    self.assertEqual(cps['ENERGY'].NE(), np.array((150,200)))
+    cps.ENERGY.NE[0]=180
+    self.assertEqual(dps['ENERGY'].NE(), np.array((180,200)))
+
     self.assertEqual(ips['SITES'].NL(), 2)
     self.assertEqual(ips.find('NL').get_path(), 'SITES.NL')
     ips.find('NL').set(3)
     self.assertEqual(ips['SITES'].NL(), 3)
     self.assertTrue(isinstance(ips['XSITES'], CustomSection))
 
     output = io.StringIO()
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/output_definitions.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/scf.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/scf.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/task_result.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/task_result.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/init_tests.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/test_output.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/test_output.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/physics/lattice_data.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/physics/lattice_data.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/physics/winger_seitz_radii.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/physics/winger_seitz_radii.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/custom_potential_section.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/custom_potential_section.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/potential.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/potential.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/__init__.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/lattice.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/lattice.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/occupation.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/occupation.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/reference_system.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/reference_system.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/sites.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/types.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/FePt.new.pot` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/FePt.new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/FePt.pot` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/FePt.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/GeTe.pot` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/GeTe.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/Li_scf.new.pot` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/Li_scf.new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/fp_basscale0.pot` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/fp_basscale0.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/fp_new.pot` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/fp_new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potential_definitions.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potential_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potential_sections.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potential_sections.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potentials.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potentials.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/init_tests.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_2D.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_2D.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_custom_section.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_custom_section.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_potential.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_potential.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_structure.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_structure.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/atomic_types.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/atomic_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/atoms_region.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/atoms_region.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/build.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/calculator.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,21 @@
 import os, sys
 from ase.calculators.calculator import Calculator, all_changes
 
 from .sprkkr_atoms import SPRKKRAtoms
 from ..potentials.potentials import Potential
 from ..common.decorators import add_to_signature
 from ..common.directory import Directory
+from ..ase.symbols import filename_from_symbols
 import shutil
 import copy
 import subprocess
 from typing import Union, Any, Dict, Optional
+from pathlib import Path
+import re
 
 class SPRKKR(Calculator):
     """
     ASE calculator for SPR-KKR.
 
     :cvar ase2sprkkr.input_parameters.input_parameters.InputParameters InputParameters: (just for an easier access to the class)
     :cvar ase2sprkkr.potentials.potentials.Potential Potential: (dto.)
@@ -39,15 +42,15 @@
     implemented_properties = ['energy']
 
     def __init__(self, restart=None,
                  label=None, atoms=None, directory='.',
                  input_file=True, output_file=True, potential_file=True,
                  print_output='info',
                  mpi=False,
-                 input_parameters=None, options={}, potential=True,
+                 input_parameters=None, options={}, potential=None,
                  executable_postfix=True,
                  empty_spheres : str|bool = False,
                  **kwargs):
         """
         Parameters
         ----------
         label: str or None
@@ -96,29 +99,34 @@
 
         options: dict
           Further parameters for input parameters
 
         potential: sprkkr.potential.Potential or str or bool or None
           The (default) potential to be used in calculations.
           If a string is given, the potential will be read from the given filename.
-          True means to generate the potential from atoms (the default value).
+          True means to generate the potential from atoms.
           False means that the potential will be given by the input_parameters.
-          None means that the potential is required to be supplied, when calculate or save_input
-          methods are called.
+          None (the default value) means that the potential is required to be supplied,
+          when calculate or save_input
+          methods are called (either directly, or via atoms, input_parameters etc.)
 
         executable_postfix: str or bool
           String to be added to the runned executable. In some environments, the version
           and the hostname is added to the name of sprkkr executables.
           True: use SPRKKR_EXECUTABLE_SUFFIX environment variable
           False: do not append anything (the same as '')
 
         empty_spheres
           Whether to add empty spheres to the structure or not.
           Default 'auto' means add if no empty sphere is present.
-       """
+        """
+
+        if kwargs:
+            print(f"Warning - unknown arguments in the SPRKKR calculator: {kwargs}")
+
         if potential and not isinstance(potential, bool):
            if isinstance(potential, str):
                potential = Potential.from_file(potential, atoms = atoms)
            if atoms:
                raise ValueError('You can not specify both atoms and potential. '
                                 'If you specify one of them, the other will be generated from it.')
            atoms = potential.atoms
@@ -338,15 +346,15 @@
         return open(filename, mode)
 
     def save_input(self, atoms=None, input_parameters=None, potential=None,
                   input_file=None, potential_file=None, output_file=False,
                   directory:Union[str,bool,Directory,None]=None, create_subdirs:bool=False,
                   empty_spheres: Optional[str|bool] = None,
                   mpi=None,
-                  options={},
+                  options={}, task=None,
                   return_files=False,
                   ):
         """
         Save input and potential files for a calculation.
 
         Parameters
         ----------
@@ -365,15 +373,16 @@
                whose name is given by input_file argument.
 
         potential: sprkkr.potential.potentials.Potential or str or None or False
             If it is None, the self.potential value is used instead (see the later options)
             If False, the potential filename is specified in the input_parameters.
             If True,  create the potential according to the atoms and write to the resulting <potential_file> file.
             If str, then it is the filename of the potential, that is left unchanged on input
-            If None, use the potential value of the calcualtor.
+            If it is None, use the potential value of the calcualtor. If this is None too,
+            the potential is set to True if atoms are set, to False otherwise.
 
         input_file: str or bool or None
             Filename or template (see FilenameTemplator class) where to save the input file,
             None means to use the default value from the Calculator.
             See the __init__ method for the meaning of other options.
 
         potential_file: str or bool or None
@@ -405,14 +414,19 @@
             None means use for this parameter the default value from the calculator.
 
         options: dict
             Options to set to the input_parameters. If input_parameters are given by a filename,
             they are readed from the file, altered by the options and then the modified input file
             (in a temporary file) will be used.
 
+        task: None
+            Change the task (ARPES, DOS, etc...) before the calculation.
+            Instead of setting input_parameters, this way retain the compatible settings in the
+            input parameters.
+
         return_files: boolean
             Return open files object instead of just string filenames.
 
 
         Returns
         -------
         input_parameters: InputParameters
@@ -427,151 +441,213 @@
         output_filename: str or file
             Output file. See return_files
 
         """
 
         def makepath(path, must_exist):
            if '/' not in path and directory:
-              path = os.path.join(directory, path)
+              path = os.path.join(str(directory), path)
            if must_exist and not os.path.isfile(path):
               raise ValueError(must_exist.format(path=path))
            return path
 
         def from_input_name(template, replacement, default):
             if template is not True:
                return template
-            if input_file.name:
-               if input_file.name.endswith('.inp'):
-                  return input_file.name[:-4] + replacement
+            if not save_input and input_file.name:
+               name = os.path.basename(input_file.name)
+               if name.endswith('.inp'):
+                  return name[:-4] + replacement
                if input_file.name.endswith('.in'):
-                  return input_file.name[:-3] + replacement
+                  return name[:-3] + replacement
+               return name + replacement
             return default
 
-        templator = FilenameTemplator(self)
-
-        with Directory.new(directory, default=self._directory) as directory:
-          directory = directory.path
-
-          """ Resolve potential argument - whether is in fact given or not"""
-          if potential is None:
-             potential = self.potential
-
-          """ Get the input file """
-          save_input = True
-          if input_parameters:
-             if isinstance(input_parameters, str):
-                if InputParameters.is_it_a_input_parameters_name(input_parameters):
-                   input_parameters = InputParameters.create_input_parameters(input_parameters)
-                else:
-                   if not options and not potential and not input_file:
-                     save_input = False
-                     input_file = makepath(input_parameters, "'{path}' is not a task file nor a known name of input_parameters.")
-                   input_parameters = InputParameters.from_file(input_parameters)
-          else:
-             input_parameters = self.input_parameters
-          templator.input_parameters = input_parameters
-
-          input_file = input_file or self.input_file
-          if input_file is True:
-              input_file = (self.label or '') + '%a_%t.inp'
-
-          input_file = self._open_file(input_file, directory,
-                                       templator, input_parameters.is_mpi(self.mpi if mpi is None else mpi),
-                                      allow_temporary=return_files,
-                                      create_subdirs=create_subdirs,
-                                      mode = 'w+' if save_input else 'r'
-                                      )
-
-
-          """ Get the potential file """
-          # potential_file - the file containing the potential (possibly a template)
-          # potential - potential object (to be updated by atoms)
-
-          potential = potential if potential is not None else self.potential
-
-          #this is a bit tricky - both of them must not be defined - however, there is a mess with default values
-          if ((potential and potential is not True) == bool(atoms)) and (atoms or not self._atoms):
-              raise ValueError("You can not provide both a potential and atoms object to the SPRKKR calculate method, "
-                               "just one from them is generated from the another.")
-
-          atoms = atoms or self._atoms
-
-          if potential is True:
-               if not atoms:
-                   raise ValueError("Potential set to <True> which means to generate the potential from the ASE-atoms object. "
-                                    "However, this object has not been supplied")
-               potential=Potential.from_atoms(atoms)
-          elif potential is False:
-                if potential_file is not None:
-                    raise ValueError("When potential is True, the value of POTENTIAL option from the input (parameters) file will be used "
-                                     " as the potential file. Thus, specifing the <potential_file> argument is not allowed.")
-                potential = None
-          elif potential is None:
-             raise ValueError("The potential can not be <None>. However, consider supplying either <True> as the potential to generate"
-                               " it from the atoms object, or False to use the POTENTIAL option from the input (parameters) file")
-          elif isinstance(potential, str):
-                if potential_file:
+        def resolve_potential_and_atoms(potential, atoms, potential_file):
+            """ Get the potential file and the atoms object.
+            potential_file - the file containing the potential (possibly a template)
+            potential - potential object (to be updated by atoms)
+            """
+            save_input = None
+            potential = potential if potential is not None else self.potential
+            if potential is None:
+               potential = bool(atoms or self._atoms)
+            #this is a bit tricky - both of them must not be defined - however, there is a mess with default values
+            pot_specified = False
+            if potential.__class__ is bool:
+               pot_specified = not potential
+            else:
+               pot_specified = potential
+            if (pot_specified == bool(atoms)) and (atoms or not self._atoms):
+                raise ValueError("You can not provide both a potential and atoms object to the SPRKKR calculate method, "
+                                 "just one from them is generated from the another.")
+
+            atoms = atoms or self._atoms
+
+            if potential is True:
+                 if not atoms:
+                     raise ValueError("Potential set to <True> which means to generate the potential from the ASE-atoms object. "
+                                      "However, this object has not been supplied")
+                 potential=Potential.from_atoms(atoms)
+            elif potential is False:
+                  if potential_file is not None:
+                      raise ValueError("When potential is False, the value of POTENTIAL option from the input (parameters) file will be used "
+                                       " as the potential file. Thus, specifing the <potential_file> argument is not allowed.")
+                  potential = None
+            elif potential is None:
+               raise ValueError("The potential can not be <None>. However, consider supplying either <True> as the potential to generate"
+                                 " it from the atoms object, or <False> to use the POTENTIAL option from the input (parameters) file")
+            elif isinstance(potential, str):
+               if potential_file:
                    potential = Potential.from_file(potential)
-                else:
-                   potential_file = makepath(potential, "'{path}' is not a potential file")
-                   potential = None
+               else:
+                   #Set the potential file and clear the potential. Thus,
+                   #the potential will not be saved
+                   potential_file = potential
+                   potential = False
+                   save_input = True
+
+            if isinstance(potential, Potential):
+              atoms = potential.atoms
+            elif atoms:
+              atoms = SPRKKRAtoms.promote_ase_atoms(atoms)
+
+            return potential, atoms, potential_file, save_input
+
+
+        def resolve_input_parameters(input_parameters, input_file, save_input):
+            if input_parameters is None:
+                input_parameters=self.input_parameters
+            if input_parameters:
+               if isinstance(input_parameters, str):
+                  if InputParameters.is_it_a_input_parameters_name(input_parameters):
+                     input_parameters = InputParameters.create_input_parameters(input_parameters)
+                  else:
+                     if not save_input and not options and not task and not potential and not input_file:
+                       save_input = False
+                       input_file = makepath(input_parameters, "'{path}' is not a task file nor a known name of input_parameters.")
+                     input_parameters = InputParameters.from_file(input_parameters)
+            else:
+               input_parameters = self.input_parameters
 
-          if isinstance(potential, Potential):
-            atoms = potential.atoms
-          else:
-            atoms = SPRKKRAtoms.promote_ase_atoms(atoms)
+            if not input_parameters.CONTROL.POTFIL() and not potential and not potential_file:
+                raise ValueError("Potential in the input parameters is not set and no Atoms nor Potential object have been given.")
+            if save_input is None:
+                save_input = True
+            return input_parameters, input_file, save_input
+
+
+        def resolve_empty_spheres(empty_spheres):
+            if empty_spheres is None:
+               empty_spheres = self.empty_spheres
+            if empty_spheres == 'auto':
+               empty_spheres = True
+               for site in atoms.sites:
+                   if site.is_vacuum():
+                      empty_spheres = False
+            if empty_spheres:
+               from ..bindings.es_finder import add_empty_spheres
+               add_empty_spheres(atoms)
 
-          if empty_spheres is None:
-             empty_spheres = self.empty_spheres
-          if empty_spheres == 'auto':
-             empty_spheres = True
-             for site in atoms.sites:
-                 if site.is_vacuum():
-                    empty_spheres = False
-          if empty_spheres:
-             from ..bindings.es_finder import add_empty_spheres
-             add_empty_spheres(atoms)
 
-          if potential:
-             if potential_file is None:
-                 potential_file = self.potential_file
-             pf = from_input_name(potential_file, '.pot', '%a.pot')
+        def save_potential_file():
+             pf = from_input_name(potential_file or self.potential_file, '.pot', '%a.pot')
              pf = self._open_file(pf, directory, templator, True,
                                               allow_temporary=return_files,
                                               create_subdirs=create_subdirs)
              potential.save_to_file(pf, atoms)
              pf.close()
-             potential_file = pf.name
+             return pf.name
 
-          """ update input_parameters by the potential """
-          if save_input:
+
+        def open_input_file():
+            ifile = input_file or self.input_file
+            if ifile is True:
+                ifile = '%l%_%a_%t.inp'
+
+            return self._open_file(ifile, directory,
+                                         templator,
+                                        input_parameters.is_mpi(self.mpi if mpi is None else mpi),
+                                        allow_temporary=return_files,
+                                        create_subdirs=create_subdirs,
+                                        mode = 'w+' if save_input else 'r'
+                                        )
+
+        def save_input_file():
+            """ update input_parameters by the potential """
+            if task:
+              input_parameters.change_task(task)
             if options:
               input_parameters.set(options, unknown = 'find')
             if potential_file:
               #use the relative potential file name to avoid too-long-
               #-potential-file-name problem
-              dirr = os.path.dirname( input_file.name ) if input_file.name else directory
-              input_parameters.CONTROL.POTFIL = os.path.relpath( potential_file, dirr )
-            else:
-              potential_file = input_parameters.CONTROL.POTFIL()
+              #dirr = os.path.dirname( input_file.name ) if input_file.name else directory
+              input_parameters.CONTROL.POTFIL = os.path.abspath(potential_file)
+              input_parameters.CONTROL.POTFIL.result = os.path.relpath(potential_file, directory)
+            if not input_parameters.CONTROL.DATASET.is_set():
+              input_parameters.CONTROL.DATASET.result = Path(input_file.name).stem
             input_parameters.save_to_file(input_file, atoms)
             input_file.seek(0)
-          #This branch can occur if the potential have been explicitly set to False,
-          #which means not to create the potential (and take it from the input_parameters)
-          else:
-              potential_file = input_parameters.CONTROL.POTFIL
 
-          if output_file is not False:
-            """ Get the output file """
-            output_file = output_file or self.output_file
-            output_file = from_input_name(output_file, '.out', '%a_%t.out')
-            output_file = self._open_file(output_file, directory, templator, False, mode='wb',
+
+        def open_output_file():
+            """ Get and open the output file """
+            ofile = output_file or self.output_file
+            ofile = from_input_name(ofile, '.out', '%a_%t.out')
+            return self._open_file(ofile, directory, templator, False, mode='wb',
                                               allow_temporary=return_files,
                                               create_subdirs=create_subdirs)
 
+        def symbols():
+            """ Return a best guess for the names of the output file """
+            if atoms:
+                return filename_from_symbols(atoms.symbols)
+            for i in 'POTFIL', 'DATASET':
+                i=input_parameters.CONTROL[i]
+                if i.is_set():
+                   return Path(i()).stem
+            for i in (input_file, potential_file, self.input_file, self.potential_file):
+                if isinstance(i, str):
+                   i=Path(i).stem
+                   if not '%' in i: #thus i is not template
+                       return i
+            return 'sprkkr'
+
+        def taskname():
+            if task: return task
+            if input_parameters: return input_parameters.task_name
+            return 'SPRKKR'
+
+        #ALL auxiliary procedures defined
+        #HERE starts the execution
+
+        potential, atoms, potential_file, save_input = \
+                    resolve_potential_and_atoms(potential, atoms, potential_file)
+        input_parameters, input_file, save_input = \
+                    resolve_input_parameters(input_parameters, input_file, save_input)
+        resolve_empty_spheres(empty_spheres)
+
+        templator = FilenameTemplator(self, taskname, symbols)
+        with Directory.new(directory, default=self._directory) as directory:
+          directory = directory.path
+          input_file=open_input_file()
+          if potential:
+              potential_file = save_potential_file()
+          if save_input:
+              save_input_file()
+          else:
+              #This branch can occur if the potential have been explicitly set to False,
+              #which means not to create the potential (and take it from the input_parameters)
+              dirr = os.path.dirname( input_file.name ) if input_file.name else directory
+              potential_file = os.path.join(dirr, input_parameters.CONTROL.POTFIL.result)
+          if output_file is not False:
+              output_file = open_output_file()
+
+          #All is saved and opened - return the values
           if not return_files:
             for f in input_file, output_file:
                 if hasattr(f,'close'):
                    f.close()
             input_file = input_file.name
             if output_file:
                output_file = output_file.name
@@ -582,15 +658,15 @@
              return input_parameters, input_file, potential_file
 
     def run(self, atoms=None, input_parameters=None,
                   potential=None, input_file=None, potential_file=None, output_file=None,
                   directory:Union[str,bool,Directory,None]=None, create_subdirs:bool=False,
                   empty_spheres : Optional[str|bool] = None,
                   mpi : bool=None,
-                  options={},
+                  options={}, task=None,
                   print_output=None, executable_postfix=None):
         """
         Do the calculation, return various results.
 
         Parameters
         ----------
 
@@ -623,15 +699,15 @@
         with Directory.new(directory, default=self._directory) as directory:
 
           input_parameters, input_file, _, output_file = self.save_input(
                               atoms=atoms, input_parameters=input_parameters,
                               potential=potential, output_file=output_file,
                               empty_spheres=empty_spheres,
                               mpi=mpi,
-                              options=options,
+                              options=options, task=task,
                               return_files=True,
                               directory=directory)
 
           with directory.chdir():
             return input_parameters.run_process(self, input_file, output_file, print_output if print_output is not None else self.print_output,
                                      executable_postfix = executable_postfix,
                                      mpi=self.mpi if mpi is None else mpi
@@ -639,15 +715,15 @@
 
     def calculate(self, atoms=None, properties=['energy'], system_changes=all_changes,
                   input_parameters=None, potential=None,
                   input_file=None, potential_file=None, output_file=None,
                   directory:Union[str,bool,Directory,None]=None, create_subdirs:bool=False,
                   empty_spheres : Optional[str|bool] = None,
                   mpi : bool=None,
-                  options={},
+                  options={}, task=None,
                   print_output=None, executable_postfix=None):
         """
         ASE-interface method for the calculation.  This method runs the appropriate task(s)
         for the requested properties (currently always the SCF one) and updates the
         calculator object with the results.
 
         See
@@ -687,15 +763,15 @@
         #super().calculate(atoms, properties, system_changes)
         out = self.run(
                   atoms, input_parameters, potential,
                   input_file, potential_file, output_file,
                   directory, create_subdirs,
                   empty_spheres,
                   mpi,
-                  options,
+                  options, task,
                   print_output, executable_postfix
         )
         if hasattr(out, 'energy'):
             self.results.update({
               'energy' : out.energy,
             })
         return out
@@ -736,43 +812,52 @@
     @property
     def potential_object(self):
         """ Convert self.potential to a Potential object """
         if isinstance(self.potential, str):
           self.potential = Potential.from_file(self.potential)
         return self.potential
 
+    def change_task(self, task):
+        """ Just a shortcut to ``input_parameters.change_task`` """
+        self.input_parameters.change_task(task)
+
 
 class FilenameTemplator:
     """ Class that replaces the placeholders in filenames with propper values,
         see the replacements property of the class.
         The used values are remembered so all the processed filenames use
         the same value (e.g. counter, datetime etc...)
     """
 
-    def __init__(self, calculator):
+    def __init__(self, calculator, task, symbols):
         self.data = {}
         self.calculator = calculator
-        self.input_parameters = None
+        self.task = task
+        self.symbols = symbols
 
-    def _get(self, name, default, calculator):
+    def _get(self, name, default):
         if not name in self.data:
-            self.data[name] = default(self, calculator)
+            self.data[name] = default(self)
         return self.data[name]
 
     replacements = {
-          "%d" : lambda self, calc: datetime.today().strftime('%Y-%m-%d_%H:%M'),
-          "%t" : lambda self, calc: self.input_parameters.task_name if self.input_parameters else 'SPRKKR',
-          "%a" : lambda self, calc: str(calc.atoms.symbols) if calc.atoms else 'custom',
-          "%c" : lambda self, calc: calc._advance_counter()
+          "%d" : lambda self: datetime.today().strftime('%Y-%m-%d_%H:%M'),
+          "%t" : lambda self: self.task(),
+          "%a" : lambda self: self.symbols(),
+          "%l" : lambda self: self.calculator.label or '',
+          "%c" : lambda self: self.calculator._advance_counter()
         }
 
     def __call__(self, template):
         for i,v in self.replacements.items():
           if i in template:
-             template = template.replace(i, self._get(i, v, self.calculator))
+             template = template.replace(i, self._get(i, v))
+        template = re.sub('^%_','',template)
+        template = re.sub('%_(%_)*','_',template)
+        template = template.replace('%_', '_')
         return template
 
 #at least, to avoid a circular import
 from ..input_parameters.input_parameters import InputParameters
 
 #is there a better way to not document an inner classes?
 if os.path.basename(sys.argv[0]) != 'sphinx-build':
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/configuration.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/configuration.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/io_data.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/io_data.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/occupations.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/occupations.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/radial_meshes.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/radial_meshes.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sites.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sprkkr_atoms.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sprkkr_atoms.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/structure.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/structure.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sysfile.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sysfile.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/init_tests.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_build.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_calculator.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_calculator.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sites.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sysfile.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sysfile.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/tools/a2s_visualise_in_struct.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/tools/a2s_visualise_in_struct.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/init_tests.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/test_tools.py` & `ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/PKG-INFO` & `ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ase2sprkkr
-Version: 2.0.4
+Version: 2.1.0
 Summary: ASE (atomic simulation environment) interface to SPRKKR
 Home-page: https://ase2sprkkr.github.io/ase2sprkkr/
 Author: Matyáš Novák & Jano Minár
 Author-email: ase2kkr@ntc.zcu.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/SOURCES.txt` & `ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -26,51 +26,65 @@
 src/ase2sprkkr/common/configuration.py
 src/ase2sprkkr/common/configuration_containers.py
 src/ase2sprkkr/common/configuration_definitions.py
 src/ase2sprkkr/common/decorators.py
 src/ase2sprkkr/common/directory.py
 src/ase2sprkkr/common/doc.py
 src/ase2sprkkr/common/formats.py
+src/ase2sprkkr/common/generated_configuration_definitions.py
 src/ase2sprkkr/common/grammar.py
-src/ase2sprkkr/common/grammar_types.py
 src/ase2sprkkr/common/init_tests.py
 src/ase2sprkkr/common/misc.py
 src/ase2sprkkr/common/no_output.py
 src/ase2sprkkr/common/options.py
 src/ase2sprkkr/common/process_output_reader.py
+src/ase2sprkkr/common/tools.py
 src/ase2sprkkr/common/unique_values.py
+src/ase2sprkkr/common/grammar_types/__init__.py
+src/ase2sprkkr/common/grammar_types/arrays.py
+src/ase2sprkkr/common/grammar_types/basic.py
+src/ase2sprkkr/common/grammar_types/data.py
+src/ase2sprkkr/common/grammar_types/functions.py
+src/ase2sprkkr/common/grammar_types/grammar_type.py
+src/ase2sprkkr/common/grammar_types/mixed.py
 src/ase2sprkkr/common/test/__init__.py
 src/ase2sprkkr/common/test/init_tests.py
 src/ase2sprkkr/common/test/test_common.py
 src/ase2sprkkr/common/test/test_grammar_types.py
 src/ase2sprkkr/input_parameters/__init__.py
 src/ase2sprkkr/input_parameters/input_parameters.py
 src/ase2sprkkr/input_parameters/input_parameters_definitions.py
 src/ase2sprkkr/input_parameters/definitions/__init__.py
 src/ase2sprkkr/input_parameters/definitions/arpes.py
 src/ase2sprkkr/input_parameters/definitions/dos.py
+src/ase2sprkkr/input_parameters/definitions/gilbert.py
 src/ase2sprkkr/input_parameters/definitions/phagen.py
 src/ase2sprkkr/input_parameters/definitions/scf.py
 src/ase2sprkkr/input_parameters/definitions/sections.py
 src/ase2sprkkr/input_parameters/examples/arpes.in
 src/ase2sprkkr/input_parameters/examples/dos.in
 src/ase2sprkkr/input_parameters/examples/phagen.in
 src/ase2sprkkr/input_parameters/examples/scf.in
 src/ase2sprkkr/input_parameters/test/__init__.py
 src/ase2sprkkr/input_parameters/test/init_tests.py
 src/ase2sprkkr/input_parameters/test/test_definitions.py
 src/ase2sprkkr/input_parameters/test/test_input_parameters.py
 src/ase2sprkkr/outputs/__init__.py
 src/ase2sprkkr/outputs/output_definitions.py
+src/ase2sprkkr/outputs/output_files_definitions.py
 src/ase2sprkkr/outputs/task_result.py
+src/ase2sprkkr/outputs/output_files/__init__.py
+src/ase2sprkkr/outputs/output_files/spc.py
 src/ase2sprkkr/outputs/readers/__init__.py
+src/ase2sprkkr/outputs/readers/arpes.py
 src/ase2sprkkr/outputs/readers/default.py
 src/ase2sprkkr/outputs/readers/scf.py
 src/ase2sprkkr/outputs/test/__init__.py
 src/ase2sprkkr/outputs/test/init_tests.py
+src/ase2sprkkr/outputs/test/test_files.py
 src/ase2sprkkr/outputs/test/test_output.py
 src/ase2sprkkr/physics/__init__.py
 src/ase2sprkkr/physics/lattice_data.py
 src/ase2sprkkr/physics/winger_seitz_radii.py
 src/ase2sprkkr/potentials/__init__.py
 src/ase2sprkkr/potentials/custom_potential_section.py
 src/ase2sprkkr/potentials/potential_definitions.py
@@ -111,20 +125,23 @@
 src/ase2sprkkr/sprkkr/sites.py
 src/ase2sprkkr/sprkkr/sprkkr_atoms.py
 src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py
 src/ase2sprkkr/sprkkr/structure.py
 src/ase2sprkkr/sprkkr/sysfile.py
 src/ase2sprkkr/sprkkr/test/__init__.py
 src/ase2sprkkr/sprkkr/test/init_tests.py
+src/ase2sprkkr/sprkkr/test/test_arpes.py
 src/ase2sprkkr/sprkkr/test/test_build.py
 src/ase2sprkkr/sprkkr/test/test_calculator.py
 src/ase2sprkkr/sprkkr/test/test_sites.py
 src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py
 src/ase2sprkkr/sprkkr/test/test_sysfile.py
 src/ase2sprkkr/tools/__init__.py
+src/ase2sprkkr/tools/a2s_plot_output.py
 src/ase2sprkkr/tools/a2s_visualise_in_struct.py
 src/ase2sprkkr/tools/test/__init__.py
 src/ase2sprkkr/tools/test/init_tests.py
 src/ase2sprkkr/tools/test/test_tools.py
-src/sprkkr/__init__.py
+src/ase2sprkkr/visualise/__init__.py
+src/ase2sprkkr/visualise/plot.py
 tests/test.py
 tests/test_inputfile.py
```

### Comparing `ase2sprkkr-2.0.4/tests/test.py` & `ase2sprkkr-2.1.0/tests/test.py`

 * *Files identical despite different names*


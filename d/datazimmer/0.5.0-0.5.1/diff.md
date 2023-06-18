# Comparing `tmp/datazimmer-0.5.0.tar.gz` & `tmp/datazimmer-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazimmer-0.5.0.tar", last modified: Sun May  7 14:13:03 2023, max compression
+gzip compressed data, was "datazimmer-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `datazimmer-0.5.0.tar` & `datazimmer-0.5.1.tar`

### file list

```diff
@@ -1,146 +1,148 @@
--rw-r--r--   0        0        0     1003 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.github/workflows/compatibility_test.yml
--rw-r--r--   0        0        0     1299 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      565 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1795 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.gitignore
--rw-r--r--   0        0        0      288 2023-05-07 14:12:58.174204 datazimmer-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0      491 2023-05-07 14:12:58.174204 datazimmer-0.5.0/CITATION.cff
--rw-r--r--   0        0        0     1077 2023-05-07 14:12:58.174204 datazimmer-0.5.0/LICENSE
--rw-r--r--   0        0        0     3122 2023-05-07 14:12:58.174204 datazimmer-0.5.0/README.md
--rw-r--r--   0        0        0     3754 2023-05-07 14:12:58.174204 datazimmer-0.5.0/conftest.py
--rw-r--r--   0        0        0      634 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/__init__.py
--rw-r--r--   0        0        0     3363 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/aswan_integration.py
--rw-r--r--   0        0        0     7997 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/config_loading.py
--rw-r--r--   0        0        0      102 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/exceptions.py
--rw-r--r--   0        0        0      624 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/get_runtime.py
--rw-r--r--   0        0        0     2420 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/gh_actions.py
--rw-r--r--   0        0        0        0 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/__init__.py
--rw-r--r--   0        0        0     6235 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/atoms.py
--rw-r--r--   0        0        0     1344 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/complete_id.py
--rw-r--r--   0        0        0     1744 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/datascript.py
--rw-r--r--   0        0        0     4537 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/high_level.py
--rw-r--r--   0        0        0     4798 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/metadata/scrutable.py
--rw-r--r--   0        0        0     3334 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/naming.py
--rw-r--r--   0        0        0      526 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/persistent_state.py
--rw-r--r--   0        0        0     8281 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/pipeline_element.py
--rw-r--r--   0        0        0     7718 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/project_runtime.py
--rw-r--r--   0        0        0      935 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/raw_data.py
--rw-r--r--   0        0        0     6107 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/registry.py
--rw-r--r--   0        0        0      713 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/reporting.py
--rw-r--r--   0        0        0        0 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/sql/__init__.py
--rw-r--r--   0        0        0       87 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/sql/draw.py
--rw-r--r--   0        0        0     9253 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/sql/loader.py
--rw-r--r--   0        0        0        0 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/__init__.py
--rw-r--r--   0        0        0     4692 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/create_dogshow.py
--rw-r--r--   0        0        0      845 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_commands.py
--rw-r--r--   0        0        0      346 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_config.py
--rw-r--r--   0        0        0     4264 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_full_integration.py
--rw-r--r--   0        0        0      465 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_registry.py
--rw-r--r--   0        0        0      294 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_runtime.py
--rw-r--r--   0        0        0     1799 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_scrutable.py
--rw-r--r--   0        0        0      152 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_sql.py
--rw-r--r--   0        0        0      235 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_util.py
--rw-r--r--   0        0        0      943 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/test_validation.py
--rw-r--r--   0        0        0      939 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/tests/util.py
--rw-r--r--   0        0        0    10122 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/typer_commands.py
--rw-r--r--   0        0        0     3260 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/utils.py
--rw-r--r--   0        0        0     2877 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/validation_functions.py
--rw-r--r--   0        0        0    10327 2023-05-07 14:12:58.174204 datazimmer-0.5.0/datazimmer/zenodo.py
--rw-r--r--   0        0        0      114 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.AbstractEntity.rst
--rw-r--r--   0        0        0      123 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.CompositeTypeBase.rst
--rw-r--r--   0        0        0      746 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.DzAswan.rst
--rw-r--r--   0        0        0      739 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.EntityClass.rst
--rw-r--r--   0        0        0       87 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.Index.rst
--rw-r--r--   0        0        0       96 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.Nullable.rst
--rw-r--r--   0        0        0      444 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.PersistentState.rst
--rw-r--r--   0        0        0      592 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.ReportFile.rst
--rw-r--r--   0        0        0      565 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.ScruTable.rst
--rw-r--r--   0        0        0       99 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.SourceUrl.rst
--rw-r--r--   0        0        0      107 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.dump_dfs_to_tables.rst
--rw-r--r--   0        0        0      104 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.get_raw_data_path.rst
--rw-r--r--   0        0        0       77 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.parse_df.rst
--rw-r--r--   0        0        0       77 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.register.rst
--rw-r--r--   0        0        0      113 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.register_data_loader.rst
--rw-r--r--   0        0        0      113 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/api/datazimmer.register_env_creator.rst
--rw-r--r--   0        0        0       39 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/autosumm.rst
--rw-r--r--   0        0        0     2402 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      263 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/index.rst
--rw-r--r--   0        0        0       77 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-001-intro.rst
--rw-r--r--   0        0        0     4171 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-002-glossary.rst
--rw-r--r--   0        0        0      616 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-003-mock-projects.rst
--rw-r--r--   0        0        0     1269 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-004-rules-conventions.rst
--rw-r--r--   0        0        0      284 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/notebooks/doc-005-cli.rst
--rw-r--r--   0        0        0      102 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/main.rst
--rw-r--r--   0        0        0       45 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.0.rst
--rw-r--r--   0        0        0       46 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.1.rst
--rw-r--r--   0        0        0       27 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.2.rst
--rw-r--r--   0        0        0       15 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.3.rst
--rw-r--r--   0        0        0       15 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.4.rst
--rw-r--r--   0        0        0       15 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.1.5.rst
--rw-r--r--   0        0        0       34 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.1.rst
--rw-r--r--   0        0        0       31 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.2.rst
--rw-r--r--   0        0        0       31 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.3.rst
--rw-r--r--   0        0        0       31 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.4.rst
--rw-r--r--   0        0        0       29 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.5.rst
--rw-r--r--   0        0        0       39 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.6.rst
--rw-r--r--   0        0        0       34 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.2.7.rst
--rw-r--r--   0        0        0       45 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.0.rst
--rw-r--r--   0        0        0       32 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.1.rst
--rw-r--r--   0        0        0       48 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.10.rst
--rw-r--r--   0        0        0       47 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.2.rst
--rw-r--r--   0        0        0       39 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.3.rst
--rw-r--r--   0        0        0       33 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.4.rst
--rw-r--r--   0        0        0       34 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.5.rst
--rw-r--r--   0        0        0       32 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.6.rst
--rw-r--r--   0        0        0       32 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.7.rst
--rw-r--r--   0        0        0       31 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.8.rst
--rw-r--r--   0        0        0       35 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.3.9.rst
--rw-r--r--   0        0        0       37 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.0.rst
--rw-r--r--   0        0        0       32 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.1.rst
--rw-r--r--   0        0        0       70 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.10.rst
--rw-r--r--   0        0        0       55 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.11.rst
--rw-r--r--   0        0        0       45 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.12.rst
--rw-r--r--   0        0        0       68 2023-05-07 14:12:58.174204 datazimmer-0.5.0/docs/release_notes/v0.4.13.rst
--rw-r--r--   0        0        0       68 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.14.rst
--rw-r--r--   0        0        0       42 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.15.rst
--rw-r--r--   0        0        0       52 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.2.rst
--rw-r--r--   0        0        0       66 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.3.rst
--rw-r--r--   0        0        0       53 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.4.rst
--rw-r--r--   0        0        0       45 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.5.rst
--rw-r--r--   0        0        0       41 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.6.rst
--rw-r--r--   0        0        0       71 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.7.rst
--rw-r--r--   0        0        0       47 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.8.rst
--rw-r--r--   0        0        0       53 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.4.9.rst
--rw-r--r--   0        0        0       64 2023-05-07 14:12:58.178204 datazimmer-0.5.0/docs/release_notes/v0.5.0.rst
--rw-r--r--   0        0        0      159 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/confs.yaml
--rw-r--r--   0        0        0     1773 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/data/photo.csv
--rw-r--r--   0        0        0      655 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/minimal.py
--rw-r--r--   0        0        0     9861 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb
--rw-r--r--   0        0        0       57 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/__init__.py
--rw-r--r--   0        0        0     2304 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py
--rw-r--r--   0        0        0     1566 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py
--rw-r--r--   0        0        0     3192 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py
--rw-r--r--   0        0        0      307 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0      674 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py
--rw-r--r--   0        0        0      261 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0     2533 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py
--rw-r--r--   0        0        0      120 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dograce/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0       65 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/__init__.py
--rw-r--r--   0        0        0      421 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/meta.py
--rw-r--r--   0        0        0      945 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py
--rw-r--r--   0        0        0     1093 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py
--rw-r--r--   0        0        0     2415 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py
--rw-r--r--   0        0        0      810 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py
--rw-r--r--   0        0        0      575 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0     2940 2023-05-07 14:12:58.178204 datazimmer-0.5.0/dogshow/todo/complex_success.py
--rw-r--r--   0        0        0      612 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-001-intro.ipynb
--rw-r--r--   0        0        0     5328 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-002-glossary.ipynb
--rw-r--r--   0        0        0     1877 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-003-mock-projects.ipynb
--rw-r--r--   0        0        0     1928 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-004-rules-conventions.ipynb
--rw-r--r--   0        0        0     1235 2023-05-07 14:12:58.178204 datazimmer-0.5.0/notebooks/doc-005-cli.ipynb
--rw-r--r--   0        0        0     1121 2023-05-07 14:12:58.178204 datazimmer-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datazimmer-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1003 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.github/workflows/compatibility_test.yml
+-rw-r--r--   0        0        0     1299 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      565 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1795 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.gitignore
+-rw-r--r--   0        0        0      288 2023-06-18 14:15:24.928776 datazimmer-0.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0      491 2023-06-18 14:15:24.928776 datazimmer-0.5.1/CITATION.cff
+-rw-r--r--   0        0        0     1077 2023-06-18 14:15:24.928776 datazimmer-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3122 2023-06-18 14:15:24.928776 datazimmer-0.5.1/README.md
+-rw-r--r--   0        0        0     4074 2023-06-18 14:15:24.928776 datazimmer-0.5.1/conftest.py
+-rw-r--r--   0        0        0      634 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/aswan_integration.py
+-rw-r--r--   0        0        0     7923 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/config_loading.py
+-rw-r--r--   0        0        0     2112 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/dvc_util.py
+-rw-r--r--   0        0        0      144 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/exceptions.py
+-rw-r--r--   0        0        0      624 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/get_runtime.py
+-rw-r--r--   0        0        0     2434 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/gh_actions.py
+-rw-r--r--   0        0        0        0 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/__init__.py
+-rw-r--r--   0        0        0     6235 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/atoms.py
+-rw-r--r--   0        0        0     1422 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/complete_id.py
+-rw-r--r--   0        0        0     1744 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/datascript.py
+-rw-r--r--   0        0        0     4537 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/high_level.py
+-rw-r--r--   0        0        0     4798 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/metadata/scrutable.py
+-rw-r--r--   0        0        0     3456 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/naming.py
+-rw-r--r--   0        0        0      526 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/persistent_state.py
+-rw-r--r--   0        0        0     8463 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/pipeline_element.py
+-rw-r--r--   0        0        0     7648 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/project_runtime.py
+-rw-r--r--   0        0        0      935 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/raw_data.py
+-rw-r--r--   0        0        0     6177 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/registry.py
+-rw-r--r--   0        0        0      863 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/reporting.py
+-rw-r--r--   0        0        0        0 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/sql/__init__.py
+-rw-r--r--   0        0        0       87 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/sql/draw.py
+-rw-r--r--   0        0        0     9259 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/sql/loader.py
+-rw-r--r--   0        0        0        0 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/__init__.py
+-rw-r--r--   0        0        0     4692 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/create_dogshow.py
+-rw-r--r--   0        0        0      845 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_commands.py
+-rw-r--r--   0        0        0      346 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_config.py
+-rw-r--r--   0        0        0     4366 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_full_integration.py
+-rw-r--r--   0        0        0      465 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_registry.py
+-rw-r--r--   0        0        0      294 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_runtime.py
+-rw-r--r--   0        0        0     1799 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_scrutable.py
+-rw-r--r--   0        0        0      152 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_sql.py
+-rw-r--r--   0        0        0      235 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_util.py
+-rw-r--r--   0        0        0      943 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/test_validation.py
+-rw-r--r--   0        0        0      939 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/tests/util.py
+-rw-r--r--   0        0        0    10109 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/typer_commands.py
+-rw-r--r--   0        0        0     3260 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/utils.py
+-rw-r--r--   0        0        0     2957 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/validation_functions.py
+-rw-r--r--   0        0        0    10327 2023-06-18 14:15:24.928776 datazimmer-0.5.1/datazimmer/zenodo.py
+-rw-r--r--   0        0        0      114 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.AbstractEntity.rst
+-rw-r--r--   0        0        0      123 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.CompositeTypeBase.rst
+-rw-r--r--   0        0        0      746 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.DzAswan.rst
+-rw-r--r--   0        0        0      739 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.EntityClass.rst
+-rw-r--r--   0        0        0       87 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.Index.rst
+-rw-r--r--   0        0        0       96 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.Nullable.rst
+-rw-r--r--   0        0        0      444 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.PersistentState.rst
+-rw-r--r--   0        0        0      592 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.ReportFile.rst
+-rw-r--r--   0        0        0      565 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.ScruTable.rst
+-rw-r--r--   0        0        0       99 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.SourceUrl.rst
+-rw-r--r--   0        0        0      107 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.dump_dfs_to_tables.rst
+-rw-r--r--   0        0        0      104 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.get_raw_data_path.rst
+-rw-r--r--   0        0        0       77 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.parse_df.rst
+-rw-r--r--   0        0        0       77 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.register.rst
+-rw-r--r--   0        0        0      113 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.register_data_loader.rst
+-rw-r--r--   0        0        0      113 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/api/datazimmer.register_env_creator.rst
+-rw-r--r--   0        0        0       39 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/autosumm.rst
+-rw-r--r--   0        0        0     2402 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0      263 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/index.rst
+-rw-r--r--   0        0        0       77 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-001-intro.rst
+-rw-r--r--   0        0        0     4171 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-002-glossary.rst
+-rw-r--r--   0        0        0      616 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-003-mock-projects.rst
+-rw-r--r--   0        0        0     1269 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-004-rules-conventions.rst
+-rw-r--r--   0        0        0      284 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/notebooks/doc-005-cli.rst
+-rw-r--r--   0        0        0      102 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/main.rst
+-rw-r--r--   0        0        0       45 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.0.rst
+-rw-r--r--   0        0        0       46 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.1.rst
+-rw-r--r--   0        0        0       27 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.2.rst
+-rw-r--r--   0        0        0       15 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.3.rst
+-rw-r--r--   0        0        0       15 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.4.rst
+-rw-r--r--   0        0        0       15 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.1.5.rst
+-rw-r--r--   0        0        0       34 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.1.rst
+-rw-r--r--   0        0        0       31 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.2.rst
+-rw-r--r--   0        0        0       31 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.3.rst
+-rw-r--r--   0        0        0       31 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.4.rst
+-rw-r--r--   0        0        0       29 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.5.rst
+-rw-r--r--   0        0        0       39 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.6.rst
+-rw-r--r--   0        0        0       34 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.2.7.rst
+-rw-r--r--   0        0        0       45 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.0.rst
+-rw-r--r--   0        0        0       32 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.1.rst
+-rw-r--r--   0        0        0       48 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.10.rst
+-rw-r--r--   0        0        0       47 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.2.rst
+-rw-r--r--   0        0        0       39 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.3.rst
+-rw-r--r--   0        0        0       33 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.4.rst
+-rw-r--r--   0        0        0       34 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.5.rst
+-rw-r--r--   0        0        0       32 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.6.rst
+-rw-r--r--   0        0        0       32 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.7.rst
+-rw-r--r--   0        0        0       31 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.8.rst
+-rw-r--r--   0        0        0       35 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.3.9.rst
+-rw-r--r--   0        0        0       37 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.4.0.rst
+-rw-r--r--   0        0        0       32 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.4.1.rst
+-rw-r--r--   0        0        0       70 2023-06-18 14:15:24.928776 datazimmer-0.5.1/docs/release_notes/v0.4.10.rst
+-rw-r--r--   0        0        0       55 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.11.rst
+-rw-r--r--   0        0        0       45 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.12.rst
+-rw-r--r--   0        0        0       68 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.13.rst
+-rw-r--r--   0        0        0       68 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.14.rst
+-rw-r--r--   0        0        0       42 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.15.rst
+-rw-r--r--   0        0        0       52 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.2.rst
+-rw-r--r--   0        0        0       66 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.3.rst
+-rw-r--r--   0        0        0       53 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.4.rst
+-rw-r--r--   0        0        0       45 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.5.rst
+-rw-r--r--   0        0        0       41 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.6.rst
+-rw-r--r--   0        0        0       71 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.7.rst
+-rw-r--r--   0        0        0       47 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.8.rst
+-rw-r--r--   0        0        0       53 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.4.9.rst
+-rw-r--r--   0        0        0       64 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.5.0.rst
+-rw-r--r--   0        0        0       50 2023-06-18 14:15:24.932776 datazimmer-0.5.1/docs/release_notes/v0.5.1.rst
+-rw-r--r--   0        0        0      159 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/confs.yaml
+-rw-r--r--   0        0        0     1773 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/data/photo.csv
+-rw-r--r--   0        0        0      655 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/minimal.py
+-rw-r--r--   0        0        0     9861 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb
+-rw-r--r--   0        0        0       57 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/__init__.py
+-rw-r--r--   0        0        0     2304 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py
+-rw-r--r--   0        0        0     1566 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py
+-rw-r--r--   0        0        0     3192 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py
+-rw-r--r--   0        0        0      307 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0      674 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py
+-rw-r--r--   0        0        0      261 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py
+-rw-r--r--   0        0        0      120 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dograce/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/meta.py
+-rw-r--r--   0        0        0      945 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py
+-rw-r--r--   0        0        0     1093 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py
+-rw-r--r--   0        0        0     2415 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py
+-rw-r--r--   0        0        0      810 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py
+-rw-r--r--   0        0        0      575 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0     2940 2023-06-18 14:15:24.932776 datazimmer-0.5.1/dogshow/todo/complex_success.py
+-rw-r--r--   0        0        0      612 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-001-intro.ipynb
+-rw-r--r--   0        0        0     5328 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-002-glossary.ipynb
+-rw-r--r--   0        0        0     1877 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-003-mock-projects.ipynb
+-rw-r--r--   0        0        0     1928 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-004-rules-conventions.ipynb
+-rw-r--r--   0        0        0     1235 2023-06-18 14:15:24.932776 datazimmer-0.5.1/notebooks/doc-005-cli.ipynb
+-rw-r--r--   0        0        0     1102 2023-06-18 14:15:24.932776 datazimmer-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4486 1970-01-01 00:00:00.000000 datazimmer-0.5.1/PKG-INFO
```

### Comparing `datazimmer-0.5.0/.github/workflows/compatibility_test.yml` & `datazimmer-0.5.1/.github/workflows/compatibility_test.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/.github/workflows/test.yml` & `datazimmer-0.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/.github/workflows/twine_release.yml` & `datazimmer-0.5.1/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/.gitignore` & `datazimmer-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/LICENSE` & `datazimmer-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/README.md` & `datazimmer-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/conftest.py` & `datazimmer-0.5.1/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,33 +5,41 @@
 from tempfile import TemporaryDirectory
 
 import boto3
 import moto
 import pytest
 from aswan.constants import DEFAULT_REMOTE_ENV_VAR, DEPOT_ROOT_ENV_VAR
 from aswan.depot.remote import HEX_ENV, PW_ENV
-from dvc.config import Config as DvcConfig
 from zimmauth import ZimmAuth
 from zimmauth.core import LOCAL_HOST_NAMES_ENV_VAR
 
 from datazimmer.config_loading import RunConfig
 from datazimmer.naming import (
     AUTH_HEX_ENV_VAR,
     AUTH_PASS_ENV_VAR,
     DEFAULT_ENV_NAME,
     MAIN_MODULE_NAME,
+    META_MODULE_NAME,
 )
 from datazimmer.tests.create_dogshow import dogshow_root
 from datazimmer.tests.util import dz_ctx
-from datazimmer.typer_commands import cleanup, init
+from datazimmer.typer_commands import init, setup_dvc
 from datazimmer.utils import cd_into, gen_rmtree
 
 CORE_PY = dogshow_root / "minimal.py"
 
 
+def pytest_sessionstart(session):
+    """
+    Called after the Session object has been created and
+    before performing collection and entering the run test loop.
+    """
+    setup_dvc()
+
+
 def pytest_addoption(parser):
     # test / explore / live
     parser.addoption("--mode", action="store", default="test")
 
 
 @pytest.fixture(scope="session")
 def empty_template():
@@ -54,14 +62,17 @@
 
 
 @pytest.fixture
 def in_template(empty_template: Path):
     with cd_into(empty_template):
         sys.path.insert(0, empty_template.as_posix())
         yield empty_template
+        for k in list(sys.modules.keys()):
+            if k.startswith(META_MODULE_NAME) or k.startswith(MAIN_MODULE_NAME):
+                sys.modules.pop(k)
         sys.path.pop(0)
 
 
 @pytest.fixture
 def running_template(in_template):
     _env = DEFAULT_ENV_NAME
     with RunConfig(write_env=_env, read_env=_env, profile=True):
@@ -77,18 +88,18 @@
         conn.create_bucket(Bucket="bucket-2", **_bconf)
         conn.create_bucket(Bucket="bucket-3", **_bconf)
         yield conn
 
 
 @pytest.fixture
 def proper_env():
-    gpath = Path(DvcConfig().files.get("global"))
+    gpath = Path.home() / ".config" / "dvc" / "config"
 
     old_conf = None
-    if gpath.name and gpath.exists():
+    if gpath.exists():
         old_conf = gpath.read_text()
 
     tmp_dir = TemporaryDirectory()
     tmp_path = Path(tmp_dir.name)
     rem_path, local_path = tmp_path / "aswan-remote", tmp_path / "aswan-local"
     rem_path.mkdir()
     local_path.mkdir()
```

### Comparing `datazimmer-0.5.0/datazimmer/__init__.py` & `datazimmer-0.5.1/datazimmer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 from .persistent_state import PersistentState
 from .pipeline_element import register, register_data_loader, register_env_creator
 from .project_runtime import dump_dfs_to_tables
 from .raw_data import get_raw_data_path
 from .reporting import ReportFile
 from .typer_commands import app
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
```

### Comparing `datazimmer-0.5.0/datazimmer/aswan_integration.py` & `datazimmer-0.5.1/datazimmer/aswan_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from importlib import import_module
 from typing import TYPE_CHECKING
 
-from dvc.repo import Repo
 from structlog import get_logger
 
 from .config_loading import Config, RunConfig, get_aswan_leaf_param_id
+from .dvc_util import get_locked_param
 from .metadata.complete_id import CompleteIdBase
-from .naming import BASE_CONF_PATH, get_stage_name
+from .naming import get_stage_name
 from .utils import get_creation_module_name
 
 logger = get_logger("aswan_integration")
 
 if TYPE_CHECKING:
     from aswan import ANY_HANDLER_T  # pragma: no cover
 
@@ -73,24 +73,12 @@
         pass  # pragma: no cover
 
     def get_aswan_status(self):
         conf = RunConfig.load()
         if conf.reset_aswan:
             return
         stage_name = get_stage_name(self._ns, conf.write_env)
-        possible_deps = []
-        repo = Repo()
-
         aswan_id = get_aswan_leaf_param_id(self.name)
-
-        for stage in repo.index.stages:
-            # imported stage has no name attribute
-            if getattr(stage, "name", "") == stage_name:
-                possible_deps = stage.deps
-
-        for dep in possible_deps:
-            if dep.def_path == BASE_CONF_PATH.as_posix():
-                info = dep.hash_info.value if dep.hash_info else {}
-                return info.get(aswan_id)
+        get_locked_param(stage_name, aswan_id)
 
     def _reg_from_module(self):
         self.project.register_module(import_module(type(self).__module__))
```

### Comparing `datazimmer-0.5.0/datazimmer/config_loading.py` & `datazimmer-0.5.1/datazimmer/config_loading.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 from abc import ABCMeta
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Type, TypeVar, Union
 
 import yaml
-from dvc.repo import Repo
 from parquetranger import TableRepo
 from structlog import get_logger
 from zimmauth import ZimmAuth
 
+from .dvc_util import get_default_remote
 from .exceptions import ProjectSetupException
 from .metadata.complete_id import CompleteId
 from .naming import (
     AUTH_HEX_ENV_VAR,
     AUTH_PASS_ENV_VAR,
     BASE_CONF_PATH,
     DEFAULT_ENV_NAME,
@@ -36,21 +36,17 @@
 class ProjectEnv:
     name: str = DEFAULT_ENV_NAME
     remote: Optional[str] = None
     parent: Optional[str] = None
     params: dict = field(default_factory=dict)
     import_envs: dict = field(default_factory=dict)
 
-    def __post_init__(self):
-        if self.remote is None:
-            try:
-                repo = Repo()
-                self.remote = repo.config["core"]["remote"]
-            except KeyError:
-                pass
+    @property
+    def true_remote(self):
+        return self.remote or get_default_remote()
 
 
 @dataclass
 class ImportedProject:
     name: str
     data_namespaces: list = None
     version: str = ""
@@ -158,16 +154,18 @@
     def load(cls):
         dic = cls._load_raw()
         ldic = {k: _to_list(dic.pop(k, {}), v) for k, v in _DC_ATTRIBUTES.items()}
         return cls(**dic, **ldic)
 
     @property
     def sorted_envs(self):
-        _remote = self.get_env(self.default_env).remote
-        return sorted(self.envs, key=lambda env: (env.remote == _remote, env.remote))
+        _remote = self.get_env(self.default_env).true_remote
+        return sorted(
+            self.envs, key=lambda env: (env.true_remote == _remote, env.true_remote)
+        )
 
     @property
     def env_names(self):
         return [e.name for e in self.envs]
 
     def _update_raw(self, dic: dict):
         BASE_CONF_PATH.write_text(yaml.dump(self._load_raw() | dic, sort_keys=False))
```

### Comparing `datazimmer-0.5.0/datazimmer/get_runtime.py` & `datazimmer-0.5.1/datazimmer/get_runtime.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/gh_actions.py` & `datazimmer-0.5.1/datazimmer/gh_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     path.parent.mkdir(exist_ok=True, parents=True)
     path.write_text(yaml.safe_dump(dic, sort_keys=False).replace("'on':", "on:"))
 
 
 def write_project_cron(cron):
     from . import typer_commands as tc
 
-    funs = tc.build_meta, tc.update, (tc.run, "--commit"), tc.publish_data
+    funs = tc.setup_dvc, tc.build_meta, tc.update, (tc.run, "--commit"), tc.publish_data
     cron_dic = _get_cron_dic(cron, "zimmer-project", *funs)
     write_action(cron_dic, _GHA / "zimmer_schedule.yml")
 
 
 def write_aswan_crons(projects: list["DzAswan"]):
     from . import typer_commands as tc
```

### Comparing `datazimmer-0.5.0/datazimmer/metadata/atoms.py` & `datazimmer-0.5.1/datazimmer/metadata/atoms.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/metadata/complete_id.py` & `datazimmer-0.5.1/datazimmer/metadata/complete_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional
 
+from ..exceptions import NotADzObject
 from ..naming import MAIN_MODULE_NAME, META_MODULE_NAME, from_mod_name
 
 
 @dataclass
 class CompleteId:
     """bedrock id with a namespace prefix
 
@@ -42,7 +43,8 @@
     @classmethod
     def from_module_name(cls, module_name, project=None):
         _splitted = module_name.split(".")
         if _splitted[0] == META_MODULE_NAME:
             return cls(from_mod_name(_splitted[1]), _splitted[2])
         elif (_splitted[0] == MAIN_MODULE_NAME) and (len(_splitted) > 1):
             return cls(project, _splitted[1])
+        raise NotADzObject(module_name)
```

### Comparing `datazimmer-0.5.0/datazimmer/metadata/datascript.py` & `datazimmer-0.5.1/datazimmer/metadata/datascript.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/metadata/high_level.py` & `datazimmer-0.5.1/datazimmer/metadata/high_level.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/metadata/scrutable.py` & `datazimmer-0.5.1/datazimmer/metadata/scrutable.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/naming.py` & `datazimmer-0.5.1/datazimmer/naming.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         self._info_dir = self.dir / "info"
 
         package_name = get_package_name(name)
 
         self.index_dir = self.dir / "index"
         self.info_yaml = self.info_yaml_of(name, version)
         self.publish_paths = self._relpos([self.index_dir, self.info_yaml])
-        self.dist_gitpath = f"index/{package_name}-{version}.tar.gz"
+        self.tarfile_name = f"{package_name}-{version}.tar.gz"
+        self.wheel_name = f"{package_name}-{version}-py3-none-any.whl"
+        self.dist_gitpath = f"index/{self.tarfile_name}"
 
     def info_yaml_of(self, name, version: Optional[str] = None) -> Path:
         if version:
             return self._info_dir / f"{name}-{version}.yaml"
         return self.get_latest_yaml_path(name)
 
     def get_latest_yaml_path(self, name):
```

### Comparing `datazimmer-0.5.0/datazimmer/persistent_state.py` & `datazimmer-0.5.1/datazimmer/persistent_state.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/pipeline_element.py` & `datazimmer-0.5.1/datazimmer/pipeline_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass, field
 from functools import partial
 from pathlib import Path
 from typing import Any, Optional
 
 from structlog import get_logger
 
+from . import dvc_util as dvcu
 from .aswan_integration import DzAswan
 from .config_loading import (
     CONF_KEYS,
     ENV_KEYS,
     Config,
     RunConfig,
     get_aswan_leaf_param_id,
@@ -67,41 +68,46 @@
         conf.read_env = self.read_env or env
         conf.write_env = env
         conf.dump()
         _, kwargs = self._get_params(env)
         with _profile(conf.profile, self.stage_name(env)):
             return self.runner(**kwargs)
 
-    def add_stages(self, dvc_repo):
+    def add_stages(self):
         from . import typer_commands as tc
 
         # relpath = inspect.getfile(self.runner)
         # lineno = inspect.findsource(self.runner)[1]
 
         for write_env in self.write_envs:
             _true_read_env = self.read_env or write_env
             _parser = partial(_parse_list, env=write_env)
             param_ids, _ = self._get_params(write_env)
 
-            dvc_repo.stage.add(
+            dvcu.add_stage(
                 cmd=cli_run((tc.run_step, self.ns, write_env)),
                 name=self.stage_name(write_env),
                 outs_no_cache=_parser(self.outputs_nocache),
                 outs=_parser(self.outputs),
                 outs_persist=_parser(self.outputs_persist),
                 deps=_parse_list([self.runner, *self.dependencies], _true_read_env),
-                params=[{BASE_CONF_PATH.as_posix(): param_ids}] if param_ids else None,
-                force=True,
+                params=[
+                    f"{BASE_CONF_PATH.as_posix()}:{pid}" for pid in (param_ids or [])
+                ],
             )
             yield self.stage_name(write_env)
 
     def get_no_cache_outs(self, env):
         for e in [env] if env else self.write_envs:
             yield _parse_list(self.outputs_nocache, e)
 
+    def get_all_outs(self, env):
+        for ol in [self.outputs_nocache, self.outputs, self.outputs_persist]:
+            yield _parse_list(ol, env)
+
     def stage_name(self, env):
         return get_stage_name(self.ns, env)
 
     @property
     def ns(self):
         return CompleteIdBase.from_cls(self.runner).namespace
```

### Comparing `datazimmer-0.5.0/datazimmer/project_runtime.py` & `datazimmer-0.5.1/datazimmer/project_runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from dataclasses import dataclass
 from functools import partial
 from importlib import import_module
 from pathlib import Path
 from pkgutil import walk_packages
 from typing import TYPE_CHECKING, TypeVar
 
-from dvc.repo import Repo
 from structlog import get_logger
 
 from .config_loading import Config
-from .exceptions import ProjectSetupException
+from .dvc_util import import_dvc
+from .exceptions import NotADzObject, ProjectSetupException
 from .metadata.atoms import EntityClass
 from .metadata.complete_id import CompleteIdBase
 from .metadata.high_level import NamespaceMetadata, ProjectMetadata
 from .metadata.scrutable import ScruTable
 from .naming import (
     MAIN_MODULE_NAME,
     META_MODULE_NAME,
@@ -53,23 +53,28 @@
         while self._module_dic.keys() != self._collected_modules:
             self._collect_metas()
         self._fill_projects()
         self.metadata = self.metadata_dic[self.name]
         self.data_to_load: list[DataEnvironmentToLoad] = self._get_data_envs()
 
     def load_all_data(self, env=None):
-        dvc_repo = Repo()
         posixes = []
         for data_env in self.data_to_load:
             gen_rmtree(data_env.path)  # brave thing...
             data_env.path.parent.mkdir(exist_ok=True, parents=True)
             pull = (env is None) or (
                 data_env.env == self.config.resolve_ns_env(data_env.project, env)
             )
-            data_env.load_data(dvc_repo, pull)
+            import_dvc(
+                uri=data_env.uri,
+                path=data_env.posix,
+                out=data_env.posix,
+                rev=data_env.tag,
+                no_exec=not pull,
+            )
             posixes.append(data_env.posix)
         return posixes
 
     def get_table_for_entity(
         self, ec: EntityClass, base_table: ScruTable, feat_elems
     ) -> ScruTable:
         fixed = base_table.key_map.get(feat_elems)
@@ -129,21 +134,22 @@
         for ns_module_id, module in list(self._module_dic.items()):
             if ns_module_id in self._collected_modules:
                 continue
             self._parse_module(module)
             self._collected_modules.add(ns_module_id)
 
     def _parse_module(self, module):
-        base_id = CompleteIdBase.from_module_name(module.__name__, self.name)
-        if base_id is None:
+        try:
+            base_id = CompleteIdBase.from_module_name(module.__name__, self.name)
+        except NotADzObject:
             return
+
         if base_id not in self._ns_meta_dic.keys():
             self._ns_meta_dic[base_id] = NamespaceMetadata(base_id.namespace)
         ns_meta = self._ns_meta_dic[base_id]
-
         for obj in map(partial(getattr, module), dir(module)):
             if inspect.ismodule(obj) and _dz_module(obj.__name__):
                 self._walk_module(obj)
                 continue
             mod_name = getattr(obj, "__module__", "")  # set for relevant instances
             if _dz_module(mod_name):
                 if mod_name != module.__name__:
@@ -180,24 +186,14 @@
     def posix(self):
         return self.path.as_posix()
 
     @property
     def path(self):
         return get_data_path(self.project, self.ns, self.env)
 
-    def load_data(self, dvc_repo: Repo, pull=False):
-        dvc_repo.imp(
-            url=self.uri,
-            path=self.posix,
-            out=self.posix,
-            rev=self.tag,
-            fname=None,
-            no_exec=not pull,
-        )
-
 
 def dump_dfs_to_tables(
     df_structable_pairs: list[tuple["pd.DataFrame", "ScruTable"]],
     parse=True,
     skip_empty=False,
     **kwargs,
 ):
```

### Comparing `datazimmer-0.5.0/datazimmer/raw_data.py` & `datazimmer-0.5.1/datazimmer/raw_data.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/registry.py` & `datazimmer-0.5.1/datazimmer/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import sys
 from functools import partial
 from pathlib import Path
 from shutil import copy, copytree
-from subprocess import PIPE, CalledProcessError, check_call, check_output
+from subprocess import CalledProcessError, check_call, check_output
 from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING
 
 import toml
 import yaml
 from flit.build import main
 from structlog import get_logger
@@ -117,17 +117,19 @@
                 "requires-python": PYV,
                 "dependencies": self.requires + reqs_from_txt,
             },
             "tool": {"flit": {"module": {"name": f"{META_MODULE_NAME}.{mod_name}"}}},
         }
         pack_paths.toml_path.write_text(toml.dumps(proj_conf))
         ns = main(pack_paths.toml_path)
-        copy(ns.sdist.file, self.paths.index_dir)
-        copy(ns.wheel.file, self.paths.index_dir)
-        return ns.sdist.file
+        for _src, _dst in [
+            (ns.sdist.file, self.paths.tarfile_name),
+            (ns.wheel.file, self.paths.wheel_name),
+        ]:
+            copy(_src, self.paths.index_dir / _dst)
 
     def _install_no_server(self, packages: list):
         addr = self.paths.index_dir.as_posix()
         comm = [sys.executable, "-m", "pip", "install", f"--find-links={addr}"]
         extras = ["--no-cache", "--no-build-isolation"]
         backup_ind = ["--extra-index-url", "https://pypi.org/simple"]
         check_call(comm + backup_ind + extras + packages)  # TODO: , stdout=PIPE)
@@ -143,15 +145,15 @@
     def _get_tags(self):
         tagpref = VERSION_SEPARATOR.join([VERSION_PREFIX, self.conf.version])
         return list(command_out_w_prefix(["git", "tag"], tagpref))
 
     def _is_released(self):
         try:
             comm = ["git", "cat-file", "-e", f"origin/main:{self.paths.dist_gitpath}"]
-            check_call(comm, cwd=self.posix, stdout=PIPE, stderr=PIPE)
+            check_call(comm, cwd=self.posix)  # KMN , stdout=PIPE, stderr=PIPE
             msg = f"can't package {self.name}-{self.conf.version} - already released"
             logger.warning(msg)
             return True
         except CalledProcessError:
             return False
```

### Comparing `datazimmer-0.5.0/datazimmer/reporting.py` & `datazimmer-0.5.1/datazimmer/reporting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from pathlib import Path
 
 from .config_loading import RunConfig
+from .exceptions import ProjectSetupException
 
 REPORT_DIR = Path("reports")
 
 report_file = REPORT_DIR / "report.html"
 
 
 @dataclass
@@ -24,8 +25,12 @@
         self.current_path.write_text(text)
 
     def write_bytes(self, blob):
         self.current_path.write_bytes(blob)
 
     @property
     def current_path(self) -> Path:
-        return self.env_path(RunConfig.load().write_env)
+        try:
+            wenv = RunConfig.load().write_env
+        except ProjectSetupException:
+            wenv = "ext-run"
+        return self.env_path(wenv)
```

### Comparing `datazimmer-0.5.0/datazimmer/sql/loader.py` & `datazimmer-0.5.1/datazimmer/sql/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     def validate_data(self):
         for table in self.ns_meta.tables:
             self._validate_table(table)
 
     def _load_table(self, table: ScruTable, session):
         ins = self.sql_meta.tables[table.id_.sql_id].insert()
-        logger.info("loading", table=table.name)
+        logger.info("loading", table=table.id_.sql_id)
         for df in table.dfs:
             self._partition(df.reset_index() if table.index else df, ins, session)
 
     def _validate_table(self, table: ScruTable):
         dt_map = {}
         table_id = table.id_.sql_id
         logger.info("validating table", table=table_id)
```

### Comparing `datazimmer-0.5.0/datazimmer/tests/create_dogshow.py` & `datazimmer-0.5.1/datazimmer/tests/create_dogshow.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/tests/test_commands.py` & `datazimmer-0.5.1/datazimmer/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/tests/test_full_integration.py` & `datazimmer-0.5.1/datazimmer/tests/test_full_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from pathlib import Path
 
 import nbformat
 from nbconvert.preprocessors import ExecutePreprocessor
 
 from datazimmer.config_loading import Config
+from datazimmer.dvc_util import run_dvc
 from datazimmer.naming import meta_version_from_tag
 from datazimmer.typer_commands import (
     build_meta,
     deposit_to_zenodo,
     draw,
     import_raw,
     load_external_data,
@@ -43,14 +44,15 @@
             run_project_test(ds, constr)
         ds_cc.check_sdists()
 
 
 def run_project_test(dog_context, constr):
     with dog_context as (name, versions, raw_imports, zen_pattern):
         print("%" * 40, "\n" * 8, name, "\n" * 8, "%" * 40, sep="\n")
+        run_dvc("config", "cache.type", "copy")
         conf = Config.load()
         _complete(constr, raw_imports, zen_pattern)
         for testv in versions:
             modify_to_version(testv)
             if testv == conf.version:
                 # should warn and just try install
                 run_in_process(build_meta)
@@ -86,15 +88,15 @@
     run_in_process(draw)
     run_in_process(_run_notebooks)
     for imp in raw_imports:
         run_in_process(import_raw, imp, commit=True)
     run_in_process(load_external_data, git_commit=True)
     run_in_process(run_aswan_project)
     run_in_process(run, commit=True, reset_aswan=reset_aswan)
-    run_in_process(validate, constr)
+    run_in_process(validate, constr, verbose=True)
     run_in_process(publish_data)
     if zen_pattern:
         key_path = Path("kp.key")
         key_path.write_text(((b"MTEx" * 11)[:-1] + b"=").hex())
         run_in_process(
             deposit_to_zenodo,
             test=True,
```

### Comparing `datazimmer-0.5.0/datazimmer/tests/test_scrutable.py` & `datazimmer-0.5.1/datazimmer/tests/test_scrutable.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/tests/test_validation.py` & `datazimmer-0.5.1/datazimmer/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/tests/util.py` & `datazimmer-0.5.1/datazimmer/tests/util.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/typer_commands.py` & `datazimmer-0.5.1/datazimmer/typer_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from dataclasses import asdict
 from itertools import chain
 from pathlib import Path
 from subprocess import check_call
 from typing import TYPE_CHECKING
 
 import typer
-from dvc.repo import Repo
 from structlog import get_logger
 
+from . import dvc_util as dvcu
 from .config_loading import CONF_KEYS, Config, RunConfig, UserConfig
+from .dvc_util import setup_dvc
 from .exceptions import ProjectSetupException
 from .get_runtime import get_runtime
 from .gh_actions import write_aswan_crons, write_project_cron
 from .metadata.high_level import ProjectMetadata
 from .naming import (
     BASE_CONF_PATH,
     MAIN_MODULE_NAME,
@@ -25,26 +26,27 @@
     env_from_tag,
     get_tag,
     meta_version_from_tag,
 )
 from .raw_data import IMPORTED_RAW_DATA_DIR, RAW_DATA_DIR, RAW_ENV_NAME
 from .registry import Registry
 from .sql.draw import dump_graph
-from .sql.loader import tmp_constr
+from .sql.loader import SqlLoader, tmp_constr
 from .utils import cd_into, command_out_w_prefix, gen_rmtree, get_git_diffs, git_run
 from .validation_functions import validate
 from .zenodo import CITATION_FILE, ZenApi
 
 if TYPE_CHECKING:  # pragma: no cover
     from .project_runtime import ProjectRuntime
 
 logger = get_logger(ctx="CLI command")
 app = typer.Typer()
 
 app.command()(validate)
+app.command()(setup_dvc)
 
 
 @app.command()
 def run_step(name: str, env: str):
     get_runtime().run_step(name, env)
 
 
@@ -81,36 +83,42 @@
 @app.command()
 def update(registry: bool = True, code: bool = True, dvc: bool = True):
     if registry:
         Registry(Config.load()).update()
     if code:
         git_run(pull=True)
     if dvc:
-        Repo().pull()
+        dvcu.pull()
 
 
 @app.command()
 def draw(v: bool = False):
     with tmp_constr(v) as constr:
         dump_graph(constr)
 
 
 @app.command()
+def sql_load(env: str = None, constr: str = "sqlite:///data.db"):
+    loader = SqlLoader(constr)
+    loader.setup_schema()
+    loader.load_data(env or Config.load().default_env)
+
+
+@app.command()
 def set_whoami(first_name: str, last_name: str, orcid: str):
     UserConfig(first_name, last_name, orcid).dump()
 
 
 @app.command()
 def import_raw(project: str, tag: str = "", commit: bool = False):
-    dvc_repo = Repo()
     reg = get_runtime().registry
     v = meta_version_from_tag(tag) if tag else None
     uri = ProjectMetadata(**reg.get_project_meta_base(project, v)).uri
     IMPORTED_RAW_DATA_DIR.mkdir(exist_ok=True)
-    dvc_repo.imp(
+    dvcu.import_dvc(
         uri,
         path=RAW_DATA_DIR.as_posix(),
         out=(IMPORTED_RAW_DATA_DIR / project).as_posix(),
         rev=tag or None,
     )
     if commit:
         _dvc_commit(paths=[f"{IMPORTED_RAW_DATA_DIR}/*"], msg=f"import raw {project}")
@@ -118,35 +126,34 @@
 
 @app.command()
 def publish_data():
     build_meta()
     # TODO: ensure that this build gets published
     _validate_empty_vc("publishing data")
     runtime = get_runtime()
-    dvc_repo = Repo()
     data_version = runtime.metadata.next_data_v
     vtags = []
 
     def _tag(env_name, env_remote):
         vtag = get_tag(runtime.config.version, data_version, env_name)
         _commit_dvc_default(env_remote)
         check_call(["git", "tag", vtag])
         vtags.append(vtag)
 
-    default_remote = runtime.config.get_env(runtime.config.default_env).remote
+    default_remote = runtime.config.get_env(runtime.config.default_env).true_remote
     if RAW_DATA_DIR.exists():
-        dvc_repo.add(RAW_DATA_DIR.as_posix())
-        dvc_repo.push(targets=RAW_DATA_DIR.as_posix(), remote=default_remote)
+        dvcu.add(RAW_DATA_DIR.as_posix())
+        dvcu.push(targets=[RAW_DATA_DIR.as_posix()], remote=default_remote)
         _dvc_commit([RAW_DATA_DIR], "save raw data")
         _tag(RAW_ENV_NAME, default_remote)
     for env in runtime.config.sorted_envs:
         targets = runtime.step_names_of_env(env.name)
         logger.info("pushing targets", targets=targets, env=env.name)
-        dvc_repo.push(targets=targets, remote=env.remote)
-        _tag(env.name, env.remote)
+        dvcu.push(targets=targets, remote=env.true_remote)
+        _tag(env.name, env.true_remote)
     git_run(push=True, pull=True)
     for tag_to_push in vtags:
         check_call(["git", "push", "origin", tag_to_push])
     runtime.registry.publish()
 
 
 @app.command()
@@ -232,60 +239,51 @@
         asw_project(global_run=True).run()
     if publish:
         git_run(add=(BASE_CONF_PATH,), msg="asw-run", push=True, pull=True, check=True)
 
 
 @app.command()
 def run(
-    stage: bool = True,
     profile: bool = False,
     env: str = None,
     commit: bool = False,
     reset_aswan: bool = False,
 ):
     # TODO: add validation that all scrutables belong somewhere as an output
-    dvc_repo = Repo(config={"core": {"autostage": stage}})
+    # used to have autostage thing
     runtime = get_runtime()
     stage_names = []
     no_cache_outputs = []
     for step in runtime.metadata.complete.pipeline_elements:
         no_cache_outputs.extend(chain(*step.get_no_cache_outs(env)))
-        stage_names.extend(step.add_stages(dvc_repo))
-
-    for dvc_stage in dvc_repo.stages:
-        if (
-            dvc_stage.is_data_source
-            or dvc_stage.is_import
-            or (dvc_stage.name in stage_names)
-        ):
+        stage_names.extend(step.add_stages())
+    data_sources = []  # TODO
+    for dvc_stage_name in dvcu.list_stages():
+        if dvc_stage_name in (stage_names + data_sources):
             continue
-        logger.info("removing dvc stage", stage=dvc_stage.name)
-        dvc_repo.remove(dvc_stage.name)
-        dvc_repo.lock.lock()
-        dvc_stage.remove_outs(force=True)
-        dvc_repo.lock.unlock()
+        logger.info("removing dvc stage", stage=dvc_stage_name)
+        dvcu.remove(dvc_stage_name)
     if not stage_names:
         return
     targets = runtime.step_names_of_env(env) if env else None
     rconf = RunConfig(profile=profile, reset_aswan=reset_aswan)
     with rconf:
         logger.info("running repro", targets=targets, **asdict(rconf))
-        runs = dvc_repo.reproduce(targets=targets, pull=True)
+        runs = dvcu.reproduce(targets=targets)
     git_run(add=["dvc.yaml", "dvc.lock", BASE_CONF_PATH, *no_cache_outputs])
     if commit:
         now = dt.datetime.now().isoformat(" ", "minutes")
         git_run(msg=f"at {now} ran: {runs}", check=True)
     return runs
 
 
 def _iter_dvc_paths(runtime: "ProjectRuntime", env):
-    dvc_repo = Repo()
-    for step in runtime.step_names_of_env(env):
-        for out in list(dvc_repo.stage.collect(step))[0].outs:
-            op = Path(out.fs_path)
+    for step in runtime.metadata.complete.pipeline_elements:
+        for out_path in chain(*step.get_all_outs(env)):
+            op = Path(out_path)
             yield op.relative_to(Path.cwd()) if op.is_absolute() else op
 
 
 def _get_current_tag_of_env(env: str):
     tag_comm = ["git", "tag", "--points-at", "HEAD"]
     for tag in command_out_w_prefix(tag_comm, VERSION_PREFIX):
         tag_env = env_from_tag(tag)
```

### Comparing `datazimmer-0.5.0/datazimmer/utils.py` & `datazimmer-0.5.1/datazimmer/utils.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/datazimmer/validation_functions.py` & `datazimmer-0.5.1/datazimmer/validation_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,21 @@
 from .sql.draw import dump_graph
 from .sql.loader import SqlLoader
 from .utils import cd_into, git_run
 
 logger = get_logger(ctx="validation")
 
 
-def validate(con: str = CONSTR, env: str = "", draw: bool = False, batch: int = 20000):
+def validate(
+    con: str = CONSTR,
+    env: str = "",
+    draw: bool = False,
+    batch: int = 20000,
+    verbose: bool = False,
+):
     """asserts a few things about a dataset
 
     - configuration files are present
     - metadata is properly exported from datascript
     - metadata fits what is in the data files
     - is properly uploaded -> can be imported to a project
 
@@ -46,20 +52,20 @@
         env_names.add(_env.name)
     if _env in ctx.config.envs:
         if _env.parent:
             assert _env.parent in env_names
 
     venv = env or ctx.config.default_env
     _log("reading data to sql db", env=venv)
-    sql_validation(con, venv, draw, batch_size=batch)
+    sql_validation(con, venv, draw, batch_size=batch, verbose=verbose)
 
 
-def sql_validation(constr, env, draw=False, batch_size=2000):
+def sql_validation(constr, env, draw=False, batch_size=2000, verbose=False):
     # TODO: check if postgres validates FKs, but sqlite does not
-    loader = SqlLoader(constr, echo=False, batch_size=batch_size)
+    loader = SqlLoader(constr, echo=verbose, batch_size=batch_size)
     _log = logger.new(step="sql", constr=constr, batch_size=batch_size, env=env).info
     try:
         _log("schema setup")
         loader.setup_schema()
         draw and dump_graph(constr)
         _log("loading to db")
         loader.load_data(env)
```

### Comparing `datazimmer-0.5.0/datazimmer/zenodo.py` & `datazimmer-0.5.1/datazimmer/zenodo.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/docs/api/datazimmer.DzAswan.rst` & `datazimmer-0.5.1/docs/api/datazimmer.DzAswan.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/docs/api/datazimmer.EntityClass.rst` & `datazimmer-0.5.1/docs/api/datazimmer.EntityClass.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/docs/api/datazimmer.ReportFile.rst` & `datazimmer-0.5.1/docs/api/datazimmer.ReportFile.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/docs/api/datazimmer.ScruTable.rst` & `datazimmer-0.5.1/docs/api/datazimmer.ScruTable.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/docs/conf.py` & `datazimmer-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/docs/notebooks/doc-002-glossary.rst` & `datazimmer-0.5.1/docs/notebooks/doc-002-glossary.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/docs/notebooks/doc-003-mock-projects.rst` & `datazimmer-0.5.1/docs/notebooks/doc-003-mock-projects.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/docs/notebooks/doc-004-rules-conventions.rst` & `datazimmer-0.5.1/docs/notebooks/doc-004-rules-conventions.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/data/photo.csv` & `datazimmer-0.5.1/dogshow/data/photo.csv`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/minimal.py` & `datazimmer-0.5.1/dogshow/minimal.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb` & `datazimmer-0.5.1/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py` & `datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py` & `datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py` & `datazimmer-0.5.1/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py` & `datazimmer-0.5.1/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py` & `datazimmer-0.5.1/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py` & `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py` & `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py` & `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py` & `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml` & `datazimmer-0.5.1/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/dogshow/todo/complex_success.py` & `datazimmer-0.5.1/dogshow/todo/complex_success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/notebooks/doc-001-intro.ipynb` & `datazimmer-0.5.1/notebooks/doc-001-intro.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/notebooks/doc-002-glossary.ipynb` & `datazimmer-0.5.1/notebooks/doc-002-glossary.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/notebooks/doc-003-mock-projects.ipynb` & `datazimmer-0.5.1/notebooks/doc-003-mock-projects.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/notebooks/doc-004-rules-conventions.ipynb` & `datazimmer-0.5.1/notebooks/doc-004-rules-conventions.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/notebooks/doc-005-cli.ipynb` & `datazimmer-0.5.1/notebooks/doc-005-cli.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.0/pyproject.toml` & `datazimmer-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 requires-python = ">=3.10"
 scripts = {datazimmer = "datazimmer:app", dz = "datazimmer:app"}
 dependencies = [
     "flit",
     "wheel>=0.37.0",
     "pip>=22.0.0",
     "setuptools>=60.0.0",
-    "dvc[s3,ssh]",
     "parquetranger>=0.2.3",
     "pandas>=2.0.1",
     "colassigner>=0.2.2",
     "sqlalchemy>=2.0.0",
     "pyyaml",
     "structlog",
     "toml",
```

### Comparing `datazimmer-0.5.0/PKG-INFO` & `datazimmer-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: datazimmer
-Version: 0.5.0
+Version: 0.5.1
 Summary: sscu-budapest utilities for scientific data engineering
 Author-email: Social Science Computing Unit Budapest <borza.endre@krtk.hu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: flit
 Requires-Dist: wheel>=0.37.0
 Requires-Dist: pip>=22.0.0
 Requires-Dist: setuptools>=60.0.0
-Requires-Dist: dvc[s3,ssh]
 Requires-Dist: parquetranger>=0.2.3
 Requires-Dist: pandas>=2.0.1
 Requires-Dist: colassigner>=0.2.2
 Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: pyyaml
 Requires-Dist: structlog
 Requires-Dist: toml
```


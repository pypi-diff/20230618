# Comparing `tmp/molecule_generation-0.3.0.tar.gz` & `tmp/molecule_generation-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/molecule_generation-0.3.0.tar", last modified: Wed Oct 19 00:00:22 2022, max compression
+gzip compressed data, was "molecule_generation-0.4.0.tar", last modified: Sun Jun 18 21:12:02 2023, max compression
```

## Comparing `molecule_generation-0.3.0.tar` & `molecule_generation-0.4.0.tar`

### file list

```diff
@@ -1,139 +1,144 @@
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      381 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/.flake8
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/.github/
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/.github/workflows/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1487 2022-10-15 13:28:58.000000 molecule_generation-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      114 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/.gitignore
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     2982 2022-10-18 23:42:33.000000 molecule_generation-0.3.0/CHANGELOG.md
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      444 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1141 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/LICENSE
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    16812 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/PKG-INFO
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    16085 2022-10-15 13:28:58.000000 molecule_generation-0.3.0/README.md
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     2780 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/SECURITY.md
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      494 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/SUPPORT.md
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      130 2022-10-15 13:28:58.000000 molecule_generation-0.3.0/environment.yml
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      312 2022-10-15 13:28:58.000000 molecule_generation-0.3.0/molecule_generation/__init__.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/chem/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/chem/__init__.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    11953 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/chem/atom_feature_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    25603 2022-10-08 23:11:22.000000 molecule_generation-0.3.0/molecule_generation/chem/molecule_dataset_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     8370 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/chem/motif_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     3559 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/chem/rdkit_helpers.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     2870 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/chem/topology_features.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     7349 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/chem/valence_constraints.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/cli/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/cli/__init__.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1159 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/cli/cli.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1630 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/cli/encode.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    13710 2022-10-08 23:11:22.000000 molecule_generation-0.3.0/molecule_generation/cli/preprocess.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1330 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/cli/sample.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    14195 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/cli/train.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1154 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/cli/visualise.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/dataset/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/dataset/__init__.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     9382 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/dataset/in_memory_trace_dataset.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     6276 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/dataset/jsonl_abstract_trace_dataset.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      564 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/dataset/jsonl_cgvae_trace_dataset.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     8455 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/dataset/jsonl_graph_properties_dataset.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     3431 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/dataset/jsonl_moler_trace_dataset.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    25561 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/dataset/trace_dataset.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     8952 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/dataset/trace_sample.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/layers/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/layers/__init__.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    39463 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/layers/cgvae_decoder.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     6743 2022-10-15 13:28:58.000000 molecule_generation-0.3.0/molecule_generation/layers/graph_property_predictor.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    97249 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/layers/moler_decoder.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/models/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/models/__init__.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    29407 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/models/cgvae.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    12869 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/models/moler_base_model.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     3676 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/models/moler_generator.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    24647 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/models/moler_vae.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/preprocessing/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/preprocessing/__init__.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    21996 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/preprocessing/cgvae_generation_trace.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    23228 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/preprocessing/data_conversion_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     6108 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/preprocessing/generation_order.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     2746 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/preprocessing/graph_sample.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    42258 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/preprocessing/moler_generation_trace.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     8379 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/preprocessing/preprocess.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/__init__.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/dataset/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     5513 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/dataset/test_jsonl_cgvae_trace_dataset_preprocessing.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     5688 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/dataset/test_jsonl_moler_trace_dataset_preprocessing.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/integration/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    15086 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/integration/test_data_moler_integration.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/layers/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     6853 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/layers/test_cgvae_decoder.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     4058 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/layers/test_moler_decoder.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/models/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     3223 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/models/test_gnn_vae.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     3396 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/models/test_moler_vae.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/preprocessing/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     8721 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/preprocessing/test_data_conversion_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1356 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/preprocessing/test_generate_test_dataset.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     8138 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/preprocessing/test_generation_trace.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      509 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/10_test_smiles.smiles
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/__init__.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1177 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/metadata.pkl.gz
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/test_0/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)   127920 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/test_0/test_0.pkl.gz
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/train_0/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)   127917 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/train_0/train_0.pkl.gz
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/valid_0/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)   128126 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/valid_0/valid_0.pkl.gz
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     2902 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/generate_test_dataset.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1203 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/metadata.pkl.gz
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/test_0/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)   144364 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/test_0/test_0.pkl.gz
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/train_0/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)   144184 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/train_0/train_0.pkl.gz
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/valid_0/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)   144003 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/valid_0/valid_0.pkl.gz
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/test/utils/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     9738 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/utils/test_beam_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1964 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/utils/test_decoder_batching.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     3675 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/utils/test_motif_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1164 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/utils/test_topology_constraints.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     5785 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/test/utils/test_valence_constraints.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/utils/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/__init__.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    13433 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/beam_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     8303 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/cgvae_visualisation_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1354 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/cli_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      532 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/data_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     4406 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/decoder_batching.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     6240 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/epoch_metrics_logger.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     3057 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/model_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    30904 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/moler_decoding_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    12034 2022-10-08 23:11:22.000000 molecule_generation-0.3.0/molecule_generation/utils/moler_inference_server.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    14767 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/moler_visualisation_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      523 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/multiprocessing_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     3603 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/preprocessing_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    11911 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/property_models.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1768 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/sequential_worker_pool.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    12158 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/sharded_data_reader.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      661 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/utils/training_utils.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      231 2022-10-15 13:28:58.000000 molecule_generation-0.3.0/molecule_generation/version.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation/visualisation/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/visualisation/__init__.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     4561 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/visualisation/cgvae_visualiser_cli.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    12917 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/visualisation/cgvae_visualiser_html.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     4778 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/visualisation/moler_visualiser_cli.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    15574 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/visualisation/moler_visualiser_html.py
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     6704 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/molecule_generation/wrapper.py
-drwxr-xr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation.egg-info/
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)    16812 2022-10-19 00:00:21.000000 molecule_generation-0.3.0/molecule_generation.egg-info/PKG-INFO
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     5036 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/molecule_generation.egg-info/SOURCES.txt
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)        1 2022-10-19 00:00:21.000000 molecule_generation-0.3.0/molecule_generation.egg-info/dependency_links.txt
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)       73 2022-10-19 00:00:21.000000 molecule_generation-0.3.0/molecule_generation.egg-info/entry_points.txt
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)      123 2022-10-19 00:00:21.000000 molecule_generation-0.3.0/molecule_generation.egg-info/requires.txt
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)       20 2022-10-19 00:00:21.000000 molecule_generation-0.3.0/molecule_generation.egg-info/top_level.txt
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)       57 2022-10-08 23:11:09.000000 molecule_generation-0.3.0/pyproject.toml
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)       38 2022-10-19 00:00:22.000000 molecule_generation-0.3.0/setup.cfg
--rw-r--r--   0 krmaziar  (1000) krmaziar  (1000)     1574 2022-10-15 13:28:58.000000 molecule_generation-0.3.0/setup.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.401428 molecule_generation-0.4.0/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      381 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/.flake8
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.377427 molecule_generation-0.4.0/.github/
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.381427 molecule_generation-0.4.0/.github/workflows/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1496 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/.github/workflows/ci.yml
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      114 2022-05-06 11:40:18.000000 molecule_generation-0.4.0/.gitignore
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3623 2023-06-16 17:31:40.000000 molecule_generation-0.4.0/CHANGELOG.md
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      444 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1141 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/LICENSE
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    16966 2023-06-18 21:12:02.401428 molecule_generation-0.4.0/PKG-INFO
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    16188 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/README.md
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     2780 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/SECURITY.md
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      494 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/SUPPORT.md
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      174 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/environment-py37.yml
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      173 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/environment-py38.yml
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      173 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/environment-py39.yml
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      136 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/environment.yml
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.381427 molecule_generation-0.4.0/molecule_generation/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      312 2022-12-05 11:20:37.000000 molecule_generation-0.4.0/molecule_generation/__init__.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.385427 molecule_generation-0.4.0/molecule_generation/chem/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/chem/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    11953 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/chem/atom_feature_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    25602 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/chem/molecule_dataset_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     8368 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/chem/motif_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3559 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/chem/rdkit_helpers.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3343 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/molecule_generation/chem/topology_features.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     7348 2023-03-17 17:35:42.000000 molecule_generation-0.4.0/molecule_generation/chem/valence_constraints.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.385427 molecule_generation-0.4.0/molecule_generation/cli/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/cli/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1159 2022-05-20 13:36:16.000000 molecule_generation-0.4.0/molecule_generation/cli/cli.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1630 2022-05-06 11:40:18.000000 molecule_generation-0.4.0/molecule_generation/cli/encode.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    13710 2022-08-31 12:52:22.000000 molecule_generation-0.4.0/molecule_generation/cli/preprocess.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1330 2022-07-27 11:16:50.000000 molecule_generation-0.4.0/molecule_generation/cli/sample.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    14195 2022-08-25 09:30:12.000000 molecule_generation-0.4.0/molecule_generation/cli/train.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1154 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/cli/visualise.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.385427 molecule_generation-0.4.0/molecule_generation/dataset/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/dataset/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     9382 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/dataset/in_memory_trace_dataset.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     6276 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/dataset/jsonl_abstract_trace_dataset.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      564 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/dataset/jsonl_cgvae_trace_dataset.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     8455 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/dataset/jsonl_graph_properties_dataset.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3431 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/dataset/jsonl_moler_trace_dataset.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    25561 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/dataset/trace_dataset.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     8952 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/dataset/trace_sample.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.389428 molecule_generation-0.4.0/molecule_generation/layers/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/layers/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    39463 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/layers/cgvae_decoder.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     6743 2022-12-05 11:20:37.000000 molecule_generation-0.4.0/molecule_generation/layers/graph_property_predictor.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    97241 2023-04-28 16:27:05.000000 molecule_generation-0.4.0/molecule_generation/layers/moler_decoder.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.389428 molecule_generation-0.4.0/molecule_generation/models/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/models/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    29406 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/models/cgvae.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    12867 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/models/moler_base_model.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3674 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/models/moler_generator.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    24644 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/models/moler_vae.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.389428 molecule_generation-0.4.0/molecule_generation/preprocessing/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/preprocessing/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    21996 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/preprocessing/cgvae_generation_trace.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    23228 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/preprocessing/data_conversion_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     6108 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/preprocessing/generation_order.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     2746 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/preprocessing/graph_sample.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    42258 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/preprocessing/moler_generation_trace.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     8379 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/preprocessing/preprocess.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.389428 molecule_generation-0.4.0/molecule_generation/test/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      354 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/molecule_generation/test/conftest.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.389428 molecule_generation-0.4.0/molecule_generation/test/dataset/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     5278 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/molecule_generation/test/dataset/test_jsonl_cgvae_trace_dataset_preprocessing.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     5453 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/molecule_generation/test/dataset/test_jsonl_moler_trace_dataset_preprocessing.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.389428 molecule_generation-0.4.0/molecule_generation/test/integration/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     2336 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/molecule_generation/test/integration/test_cli.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    15101 2023-05-12 09:50:19.000000 molecule_generation-0.4.0/molecule_generation/test/integration/test_data_moler_integration.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/layers/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     6853 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/layers/test_cgvae_decoder.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     4058 2022-07-27 11:16:50.000000 molecule_generation-0.4.0/molecule_generation/test/layers/test_moler_decoder.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/models/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3223 2023-05-26 13:19:44.000000 molecule_generation-0.4.0/molecule_generation/test/models/test_gnn_vae.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3396 2023-05-26 13:19:44.000000 molecule_generation-0.4.0/molecule_generation/test/models/test_moler_vae.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/preprocessing/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     8721 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/preprocessing/test_data_conversion_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1356 2023-06-14 12:22:51.000000 molecule_generation-0.4.0/molecule_generation/test/preprocessing/test_generate_test_dataset.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     8138 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/preprocessing/test_generation_trace.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      509 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/10_test_smiles.smiles
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/__init__.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1177 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/metadata.pkl.gz
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/test_0/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)   127920 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/test_0/test_0.pkl.gz
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/train_0/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)   127917 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/train_0/train_0.pkl.gz
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/valid_0/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)   128126 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/valid_0/valid_0.pkl.gz
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     2902 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/generate_test_dataset.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1203 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/metadata.pkl.gz
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/test_0/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)   144364 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/test_0/test_0.pkl.gz
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/train_0/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)   144184 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/train_0/train_0.pkl.gz
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.393427 molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/valid_0/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)   144003 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/valid_0/valid_0.pkl.gz
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.397428 molecule_generation-0.4.0/molecule_generation/test/utils/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     9738 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/utils/test_beam_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1964 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/utils/test_decoder_batching.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3675 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/utils/test_motif_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1164 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/test/utils/test_topology_constraints.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     5782 2023-03-17 17:35:42.000000 molecule_generation-0.4.0/molecule_generation/test/utils/test_valence_constraints.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.397428 molecule_generation-0.4.0/molecule_generation/utils/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    13433 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/beam_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     8303 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/cgvae_visualisation_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1354 2022-05-20 13:36:16.000000 molecule_generation-0.4.0/molecule_generation/utils/cli_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      532 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/data_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     4405 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/utils/decoder_batching.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     6239 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/utils/epoch_metrics_logger.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3057 2022-07-27 11:16:50.000000 molecule_generation-0.4.0/molecule_generation/utils/model_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    30904 2023-06-14 13:20:45.000000 molecule_generation-0.4.0/molecule_generation/utils/moler_decoding_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    12922 2023-05-12 09:50:19.000000 molecule_generation-0.4.0/molecule_generation/utils/moler_inference_server.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    14766 2023-03-16 13:40:03.000000 molecule_generation-0.4.0/molecule_generation/utils/moler_visualisation_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      523 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/multiprocessing_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     3603 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/preprocessing_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    11911 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/property_models.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1768 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/sequential_worker_pool.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    12158 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/sharded_data_reader.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      661 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/utils/training_utils.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      231 2022-12-05 11:20:37.000000 molecule_generation-0.4.0/molecule_generation/version.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.401428 molecule_generation-0.4.0/molecule_generation/visualisation/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        0 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/visualisation/__init__.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     4561 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/visualisation/cgvae_visualiser_cli.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    12917 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/molecule_generation/visualisation/cgvae_visualiser_html.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     4778 2022-07-27 11:16:50.000000 molecule_generation-0.4.0/molecule_generation/visualisation/moler_visualiser_cli.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    15574 2022-07-27 11:16:50.000000 molecule_generation-0.4.0/molecule_generation/visualisation/moler_visualiser_html.py
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     7317 2023-05-12 09:50:19.000000 molecule_generation-0.4.0/molecule_generation/wrapper.py
+drwxrwxr-x   0 krmaziar  (1000) krmaziar  (1000)        0 2023-06-18 21:12:02.385427 molecule_generation-0.4.0/molecule_generation.egg-info/
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)    16966 2023-06-18 21:12:02.000000 molecule_generation-0.4.0/molecule_generation.egg-info/PKG-INFO
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     5185 2023-06-18 21:12:02.000000 molecule_generation-0.4.0/molecule_generation.egg-info/SOURCES.txt
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)        1 2023-06-18 21:12:02.000000 molecule_generation-0.4.0/molecule_generation.egg-info/dependency_links.txt
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)       73 2023-06-18 21:12:02.000000 molecule_generation-0.4.0/molecule_generation.egg-info/entry_points.txt
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)      123 2023-06-18 21:12:02.000000 molecule_generation-0.4.0/molecule_generation.egg-info/requires.txt
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)       20 2023-06-18 21:12:02.000000 molecule_generation-0.4.0/molecule_generation.egg-info/top_level.txt
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)       57 2022-04-11 10:09:56.000000 molecule_generation-0.4.0/pyproject.toml
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)       38 2023-06-18 21:12:02.401428 molecule_generation-0.4.0/setup.cfg
+-rw-rw-r--   0 krmaziar  (1000) krmaziar  (1000)     1624 2023-06-15 16:44:37.000000 molecule_generation-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `molecule_generation-0.3.0/CHANGELOG.md` & `molecule_generation-0.4.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,64 @@
 # Changelog
-All notable changes to the project will be documented in this file.
 
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+All notable changes to the project are documented in this file.
+
+The format follows [Common Changelog](https://common-changelog.org/),
+and the project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.4.0] - 2023-06-16
+
+### Added
+- Add an option for `decode` to return the entire generation trace ([#51](https://github.com/microsoft/molecule-generation/pull/51))
+
+### Changed
+- Reformat with `black==23.1.0` and pin it in CI to avoid further unexpected updates ([#50](https://github.com/microsoft/molecule-generation/pull/50))
+
+### Fixed
+- Remove deprecated `numpy` types to make `molecule_generation` work with `numpy>=1.24.0` ([#49](https://github.com/microsoft/molecule-generation/pull/49))
+- Patch `GetSSSR` for compatibility with `rdkit>=2022.09.1` ([#58](https://github.com/microsoft/molecule-generation/pull/58))
+
 ## [0.3.0] - 2022-10-18
 
 ### Added
-- Support for fine-tuning a pretrained model on new data ([#30](https://github.com/microsoft/molecule-generation/pull/30))
-- `__version__` attribute to make the package version easily accessible at runtime ([#35](https://github.com/microsoft/molecule-generation/pull/35))
+- Add support for fine-tuning a pretrained model on new data ([#30](https://github.com/microsoft/molecule-generation/pull/30))
+- Add a `__version__` attribute to make the package version easily accessible at runtime ([#35](https://github.com/microsoft/molecule-generation/pull/35))
 
 ### Changed
-- Dropped the exact version requirements for `python` and `tensorflow` in order to support entire ranges of versions, including modern ones ([#35](https://github.com/microsoft/molecule-generation/pull/35))
+- Drop the exact version requirements for `python` and `tensorflow` to support entire ranges of versions ([#35](https://github.com/microsoft/molecule-generation/pull/35))
 
 ### Removed
-- Unused `GraphMultitaskModel` which ended up in the open-source release by accident ([#34](https://github.com/microsoft/molecule-generation/pull/34))
+- Drop unused `GraphMultitaskModel` which ended up in the open-source release by accident ([#34](https://github.com/microsoft/molecule-generation/pull/34))
 
 ### Fixed
-- Made the inference server check the status of child processes every 10 seconds, so that it can exit gracefully in case of errors instead of hanging ([#33](https://github.com/microsoft/molecule-generation/pull/33))
+- Make the inference server check the status of child processes every 10 seconds, so that it can exit gracefully in case of errors instead of hanging ([#33](https://github.com/microsoft/molecule-generation/pull/33))
 
 ## [0.2.0] - 2022-07-01
 
 ### Added
-- `MoLeRGenerator`, which uses the MoLeR decoder (without the encoder) as an autoregressive policy ([#6](https://github.com/microsoft/molecule-generation/pull/6))
-- `load_model_from_directory`, which can load any model by automatically picking the right wrapper class (either `VaeWrapper` or `GeneratorWrapper`) ([#24](https://github.com/microsoft/molecule-generation/pull/24))
-- An option for `encode` to return not only the mean latent code but also the variance ([#26](https://github.com/microsoft/molecule-generation/pull/26))
+- Add `MoLeRGenerator`, which uses the MoLeR decoder (without the encoder) as an autoregressive policy ([#6](https://github.com/microsoft/molecule-generation/pull/6))
+- Add `load_model_from_directory`, which can load any model by automatically picking the right wrapper class ([#24](https://github.com/microsoft/molecule-generation/pull/24))
+- Implement an option for `encode` to return not only the mean latent code but also the variance ([#26](https://github.com/microsoft/molecule-generation/pull/26))
 
 ### Changed
-- Improved how the MoLeR visualisers handle node selection steps ([#10](https://github.com/microsoft/molecule-generation/pull/10))
-- Refactored how MoLeR keeps track of generation steps during decoding and included partial molecules in the step info classes ([#27](https://github.com/microsoft/molecule-generation/pull/27))
+- Improve how the MoLeR visualisers handle node selection steps ([#10](https://github.com/microsoft/molecule-generation/pull/10))
+- Refactor how MoLeR keeps track of generation steps during decoding and include partial molecules in the step info classes ([#27](https://github.com/microsoft/molecule-generation/pull/27))
 
 ### Fixed
-- One-off errors in the latent-based visualisation mode ([#10](https://github.com/microsoft/molecule-generation/pull/10))
-- Constrained the version of `protobuf` to avoid pulling in a breaking release ([#25](https://github.com/microsoft/molecule-generation/pull/25))
+- Fix one-off errors in the latent-based visualisation mode ([#10](https://github.com/microsoft/molecule-generation/pull/10))
+- Constrain `protobuf` version to avoid pulling in a breaking release ([#25](https://github.com/microsoft/molecule-generation/pull/25))
 
 ## [0.1.0] - 2022-04-11
 
-This is the first public release, matching what was used for [the original paper](https://arxiv.org/abs/2103.03864).
+:seedling: First public release, matching what was used for [the original paper](https://arxiv.org/abs/2103.03864).
 
 ### Added
-- Full implementation of MoLeR as introduced in the paper
-- Reference implementation of CGVAE, not yet supported by the high-level model API
+- Add full implementation of MoLeR as introduced in the paper
+- Add reference implementation of CGVAE, not yet supported by the high-level model API
 
-[Unreleased]: https://github.com/microsoft/molecule-generation/compare/v0.3.0...HEAD
+[Unreleased]: https://github.com/microsoft/molecule-generation/compare/v0.4.0...HEAD
 [0.1.0]: https://github.com/microsoft/molecule-generation/releases/tag/v0.1.0
 [0.2.0]: https://github.com/microsoft/molecule-generation/releases/tag/v0.2.0
 [0.3.0]: https://github.com/microsoft/molecule-generation/releases/tag/v0.3.0
+[0.4.0]: https://github.com/microsoft/molecule-generation/releases/tag/v0.4.0
```

### Comparing `molecule_generation-0.3.0/LICENSE` & `molecule_generation-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/PKG-INFO` & `molecule_generation-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 Metadata-Version: 2.1
 Name: molecule_generation
-Version: 0.3.0
+Version: 0.4.0
 Summary: Implementations of deep generative models of molecules.
 Home-page: https://github.com/microsoft/molecule-generation/
 Author: Krzysztof Maziarz
 Author-email: krzysztof.maziarz@microsoft.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MoLeR: A Model for Molecule Generation
 
 [![CI](https://github.com/microsoft/molecule-generation/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/microsoft/molecule-generation/actions/workflows/ci.yml)
 [![license](https://img.shields.io/github/license/microsoft/molecule-generation.svg)](https://github.com/microsoft/molecule-generation/blob/main/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/molecule-generation.svg)](https://pypi.org/project/molecule-generation/)
+[![python](https://img.shields.io/pypi/pyversions/molecule_generation)](https://www.python.org/downloads/)
 [![code style](https://img.shields.io/badge/code%20style-black-202020.svg)](https://github.com/ambv/black)
 
-This repository contains training and inference code for the MoLeR model introduced in [Learning to Extend Molecular Scaffolds with Structural Motifs](https://arxiv.org/abs/2103.03864). We also include our implementation of CGVAE, but it currently lacks integration with the high-level model interface, and is provided mostly for reference.
+This repository contains training and inference code for the MoLeR model introduced in [Learning to Extend Molecular Scaffolds with Structural Motifs](https://arxiv.org/abs/2103.03864). We also include our implementation of CGVAE, but without integration with the high-level model interface.
 
 ## Quick start
 
-The `molecule_generation` package can be installed via `pip`, but it additionally depends on `rdkit` and (if one wants to use a GPU) on correctly setting up CUDA libraries. One approach to get both is through our minimalistic `conda` environment:
+`molecule_generation` can be installed via `pip`, but it additionally depends on `rdkit` and (if one wants to use a GPU) on setting up CUDA libraries. One can get both through `conda`:
 
 ```bash
 conda env create -f environment.yml
 conda activate moler-env
 ```
 
-This environment pins the versions of `python`, `rdkit` and `tensorflow` for reproducibility, but `molecule_generation` is compatible with a range of versions of these dependencies.
+Our package was tested with `python>=3.7`, `tensorflow>=2.1.0` and `rdkit>=2020.09.1`; see the `environment*.yml` files for the exact configurations tested in CI.
 
-To then install the latest release of `molecule_generation`, simply run
+To then install the latest release of `molecule_generation`, run
 ```bash
 pip install molecule-generation
 ```
 
-Alternatively, running `pip install -e .` within the root folder installs the latest state of the code, including changes that were merged into `main` but not yet released.
-
-Note that in the instructions above we pinned the `rdkit` version, as this is the version the code has been tested with. However, our code is likely to work with other modern version of `rdkit` as well.
-Finally, if `tensorflow` installation doesn't work out-of-the-box for your particular system, you may need to refer to [the tensorflow website](https://www.tensorflow.org/install) for guidelines.
+Alternatively, `pip install -e .` within the root folder installs the latest state of the code, including changes that were merged into `main` but not yet released.
 
 A MoLeR checkpoint trained using the default hyperparameters is available [here](https://figshare.com/ndownloader/files/34642724). This file needs to be saved in a fresh folder `MODEL_DIR` (e.g., `/tmp/MoLeR_checkpoint`) and be renamed to have the `.pkl` ending (e.g., to `GNN_Edge_MLP_MoLeR__2022-02-24_07-16-23_best.pkl`). Then you can sample 10 molecules by running
 
 ```bash
 molecule_generation sample MODEL_DIR 10
 ```
 
-See the next sections for how to train your own model and run more advanced inference.
+See below for how to train your own model and run more advanced inference.
+
+### Troubleshooting
+
+> Q: I am in China and so the figshare checkpoint link does not work for me.
+>
+> A: You can try [this link](https://pan.baidu.com/s/1lkiWK9-d5MvNyzqRrusGXA?pwd=4hij) instead.
+
+> Q: My particular combination of dependency versions does not work.
+>
+> A: Please submit an issue and default to using one of the pinned configurations from `environment-py*.yml` in the meantime.
+
+> Q: Installing `tensorflow` on my system does not work.
+>
+> A: Please refer to [the tensorflow website](https://www.tensorflow.org/install) for guidelines.
 
 ## Workflow
 
 Working with MoLeR can be roughly divided into four stages:
 - *data preprocessing*, where a plain text list of SMILES strings is turned into `*.pkl` files containing descriptions of the molecular graphs and generation traces;
 - *training*, where MoLeR is trained on the preprocessed data until convergence;
 - *inference*, where one loads the model and performs batched encoding, decoding or sampling; and (optionally)
```

### Comparing `molecule_generation-0.3.0/README.md` & `molecule_generation-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 # MoLeR: A Model for Molecule Generation
 
 [![CI](https://github.com/microsoft/molecule-generation/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/microsoft/molecule-generation/actions/workflows/ci.yml)
 [![license](https://img.shields.io/github/license/microsoft/molecule-generation.svg)](https://github.com/microsoft/molecule-generation/blob/main/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/molecule-generation.svg)](https://pypi.org/project/molecule-generation/)
+[![python](https://img.shields.io/pypi/pyversions/molecule_generation)](https://www.python.org/downloads/)
 [![code style](https://img.shields.io/badge/code%20style-black-202020.svg)](https://github.com/ambv/black)
 
-This repository contains training and inference code for the MoLeR model introduced in [Learning to Extend Molecular Scaffolds with Structural Motifs](https://arxiv.org/abs/2103.03864). We also include our implementation of CGVAE, but it currently lacks integration with the high-level model interface, and is provided mostly for reference.
+This repository contains training and inference code for the MoLeR model introduced in [Learning to Extend Molecular Scaffolds with Structural Motifs](https://arxiv.org/abs/2103.03864). We also include our implementation of CGVAE, but without integration with the high-level model interface.
 
 ## Quick start
 
-The `molecule_generation` package can be installed via `pip`, but it additionally depends on `rdkit` and (if one wants to use a GPU) on correctly setting up CUDA libraries. One approach to get both is through our minimalistic `conda` environment:
+`molecule_generation` can be installed via `pip`, but it additionally depends on `rdkit` and (if one wants to use a GPU) on setting up CUDA libraries. One can get both through `conda`:
 
 ```bash
 conda env create -f environment.yml
 conda activate moler-env
 ```
 
-This environment pins the versions of `python`, `rdkit` and `tensorflow` for reproducibility, but `molecule_generation` is compatible with a range of versions of these dependencies.
+Our package was tested with `python>=3.7`, `tensorflow>=2.1.0` and `rdkit>=2020.09.1`; see the `environment*.yml` files for the exact configurations tested in CI.
 
-To then install the latest release of `molecule_generation`, simply run
+To then install the latest release of `molecule_generation`, run
 ```bash
 pip install molecule-generation
 ```
 
-Alternatively, running `pip install -e .` within the root folder installs the latest state of the code, including changes that were merged into `main` but not yet released.
-
-Note that in the instructions above we pinned the `rdkit` version, as this is the version the code has been tested with. However, our code is likely to work with other modern version of `rdkit` as well.
-Finally, if `tensorflow` installation doesn't work out-of-the-box for your particular system, you may need to refer to [the tensorflow website](https://www.tensorflow.org/install) for guidelines.
+Alternatively, `pip install -e .` within the root folder installs the latest state of the code, including changes that were merged into `main` but not yet released.
 
 A MoLeR checkpoint trained using the default hyperparameters is available [here](https://figshare.com/ndownloader/files/34642724). This file needs to be saved in a fresh folder `MODEL_DIR` (e.g., `/tmp/MoLeR_checkpoint`) and be renamed to have the `.pkl` ending (e.g., to `GNN_Edge_MLP_MoLeR__2022-02-24_07-16-23_best.pkl`). Then you can sample 10 molecules by running
 
 ```bash
 molecule_generation sample MODEL_DIR 10
 ```
 
-See the next sections for how to train your own model and run more advanced inference.
+See below for how to train your own model and run more advanced inference.
+
+### Troubleshooting
+
+> Q: I am in China and so the figshare checkpoint link does not work for me.
+>
+> A: You can try [this link](https://pan.baidu.com/s/1lkiWK9-d5MvNyzqRrusGXA?pwd=4hij) instead.
+
+> Q: My particular combination of dependency versions does not work.
+>
+> A: Please submit an issue and default to using one of the pinned configurations from `environment-py*.yml` in the meantime.
+
+> Q: Installing `tensorflow` on my system does not work.
+>
+> A: Please refer to [the tensorflow website](https://www.tensorflow.org/install) for guidelines.
 
 ## Workflow
 
 Working with MoLeR can be roughly divided into four stages:
 - *data preprocessing*, where a plain text list of SMILES strings is turned into `*.pkl` files containing descriptions of the molecular graphs and generation traces;
 - *training*, where MoLeR is trained on the preprocessed data until convergence;
 - *inference*, where one loads the model and performs batched encoding, decoding or sampling; and (optionally)
```

### Comparing `molecule_generation-0.3.0/SECURITY.md` & `molecule_generation-0.4.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/chem/atom_feature_utils.py` & `molecule_generation-0.4.0/molecule_generation/chem/atom_feature_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/chem/molecule_dataset_utils.py` & `molecule_generation-0.4.0/molecule_generation/chem/molecule_dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -657,15 +657,14 @@
                 try:
                     datapoint["descriptors"].append(descr_calc_fn(rdkit_mol))
                 except Exception:
                     datapoint["failed_to_convert_from_smiles"] = datapoint["SMILES"]
 
         # Compute molecule-based scores with RDKit:
         if include_molecule_stats:
-
             datapoint["properties"] = {
                 "sa_score": compute_sa_score(rdkit_mol),
                 "clogp": MolLogP(rdkit_mol),
                 "mol_weight": ExactMolWt(rdkit_mol),
                 "qed": qed(rdkit_mol),
                 "bertz": BertzCT(rdkit_mol),
             }
```

### Comparing `molecule_generation-0.3.0/molecule_generation/chem/motif_utils.py` & `molecule_generation-0.4.0/molecule_generation/chem/motif_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     """
     fragments = fragment_into_candidate_motifs(
         molecule, cut_leaf_edges=motif_vocabulary.settings.cut_leaf_edges
     )
 
     motifs_found = []
 
-    for (motif, atom_annotations) in fragments:
+    for motif, atom_annotations in fragments:
         smiles = Chem.MolToSmiles(motif)
 
         if smiles in motif_vocabulary.vocabulary:
             motifs_found.append(MotifAnnotation(motif_type=smiles, atoms=atom_annotations))
 
     return motifs_found
```

### Comparing `molecule_generation-0.3.0/molecule_generation/chem/rdkit_helpers.py` & `molecule_generation-0.4.0/molecule_generation/chem/rdkit_helpers.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/chem/topology_features.py` & `molecule_generation-0.4.0/molecule_generation/chem/topology_features.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 """Functions to constrain edge choices based on molecule topology."""
 import logging
 from typing import Collection
 
 import numpy as np
+import rdkit
+from packaging.version import parse as parse_version
 from rdkit.Chem import BondType, GetSSSR, RWMol
 
 logger = logging.getLogger(__name__)
 
 
+def get_SSSR_size(mol: RWMol) -> int:
+    """Get the size of the smallest set of smallest rings as computed by `rdkit`."""
+    # Starting with version 2022.09.1 `GetSSSR` returns the SSSR itself, prior to that it returns
+    # the *size* of the SSSR.
+    if parse_version(rdkit.__version__) >= parse_version("2022.09.1"):
+        return len(GetSSSR(mol))
+    else:
+        return GetSSSR(mol)
+
+
 def calculate_topology_features(edges: Collection, mol: RWMol) -> np.ndarray:
     """Constrain edges based on how many loops would be in a resulting molecule.
 
     Args:
         edges: a collection of shape (E, 2) representing edges that we might want to add to the molecule supplied. Each
             edge must have element 0 containing the source atom index of the edge, and element 1 containing the target
             atom index.
@@ -28,21 +40,21 @@
     """
     # Make sure sensible default values are here in case RDKit throws an error.
     num_rings_created_by_edge = np.zeros(shape=(len(edges),), dtype=np.float32)
     num_tri_ring_edges_created_by_edge = np.zeros_like(num_rings_created_by_edge)
     mol_copy = RWMol(mol)
     try:
         # Must be calculated before GetRingInfo is called, to ensure ring info is initialised.
-        num_rings_in_base_mol = GetSSSR(mol_copy)
+        num_rings_in_base_mol = get_SSSR_size(mol_copy)
         num_base_tri_ring_edges = _calculate_num_tri_rings(mol_copy)
 
         for edge_idx, edge in enumerate(edges):
             test_mol = RWMol(mol)
             test_mol.AddBond(int(edge[0]), int(edge[1]), BondType.SINGLE)
-            num_rings_with_new_edge = GetSSSR(test_mol)
+            num_rings_with_new_edge = get_SSSR_size(test_mol)
             num_tri_ring_edges = _calculate_num_tri_rings(test_mol)
 
             num_tri_ring_edges_created_by_edge[edge_idx] = (
                 num_tri_ring_edges - num_base_tri_ring_edges
             )
             num_rings_created_by_edge[edge_idx] = num_rings_with_new_edge - num_rings_in_base_mol
```

### Comparing `molecule_generation-0.3.0/molecule_generation/chem/valence_constraints.py` & `molecule_generation-0.4.0/molecule_generation/chem/valence_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         A bool mask of the same length as candidate_target_nodes (as np array), indicating which
         of these choices are valid.
     """
     assert len(adjacency_lists) == 3, "We can only deal with 3 edge types for now."
 
     # Early exit for degenerate case:
     if len(candidate_target_nodes) == 0:
-        return np.zeros(shape=(0,), dtype=np.bool)
+        return np.zeros(shape=(0,), dtype=bool)
 
     node_idx_to_valency_map = _calculate_valency_map(adjacency_lists, node_types)
     node_idx_to_max_valency_map = _calculate_max_valency(node_types)
     node_idx_to_open_map = node_idx_to_valency_map < node_idx_to_max_valency_map
     edge_to_open_node = node_idx_to_open_map[candidate_target_nodes]
     focus_node_is_open = node_idx_to_open_map[start_node]
     return np.logical_and(edge_to_open_node, focus_node_is_open)
@@ -146,15 +146,15 @@
             functions above.
         node_types: a list of node type information. Shape = [num_nodes]
 
     Returns:
         A numpy array of shape (num_nodes,). The ith element of the array corresponds to the valency
         of the node whose index is i.
     """
-    node_idx_to_valency_map = np.zeros(shape=len(node_types), dtype=np.int)
+    node_idx_to_valency_map = np.zeros(shape=len(node_types), dtype=np.int32)
     for edge_type_idx, adjacency_list in enumerate(adjacency_lists):
         if len(adjacency_list) == 0:
             continue
         node_idx, count = np.unique(adjacency_list[:, 0], return_counts=True)
         count *= edge_type_idx + 1  # adjust for valency of edge type.
         node_idx_to_valency_map[node_idx] += count
     return node_idx_to_valency_map
```

### Comparing `molecule_generation-0.3.0/molecule_generation/cli/cli.py` & `molecule_generation-0.4.0/molecule_generation/cli/cli.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/cli/encode.py` & `molecule_generation-0.4.0/molecule_generation/cli/encode.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/cli/preprocess.py` & `molecule_generation-0.4.0/molecule_generation/cli/preprocess.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/cli/sample.py` & `molecule_generation-0.4.0/molecule_generation/cli/sample.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/cli/train.py` & `molecule_generation-0.4.0/molecule_generation/cli/train.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/cli/visualise.py` & `molecule_generation-0.4.0/molecule_generation/cli/visualise.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/dataset/in_memory_trace_dataset.py` & `molecule_generation-0.4.0/molecule_generation/dataset/in_memory_trace_dataset.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/dataset/jsonl_abstract_trace_dataset.py` & `molecule_generation-0.4.0/molecule_generation/dataset/jsonl_abstract_trace_dataset.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/dataset/jsonl_cgvae_trace_dataset.py` & `molecule_generation-0.4.0/molecule_generation/dataset/jsonl_cgvae_trace_dataset.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/dataset/jsonl_graph_properties_dataset.py` & `molecule_generation-0.4.0/molecule_generation/dataset/jsonl_graph_properties_dataset.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/dataset/jsonl_moler_trace_dataset.py` & `molecule_generation-0.4.0/molecule_generation/dataset/jsonl_moler_trace_dataset.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/dataset/trace_dataset.py` & `molecule_generation-0.4.0/molecule_generation/dataset/trace_dataset.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/dataset/trace_sample.py` & `molecule_generation-0.4.0/molecule_generation/dataset/trace_sample.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/layers/cgvae_decoder.py` & `molecule_generation-0.4.0/molecule_generation/layers/cgvae_decoder.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/layers/graph_property_predictor.py` & `molecule_generation-0.4.0/molecule_generation/layers/graph_property_predictor.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/layers/moler_decoder.py` & `molecule_generation-0.4.0/molecule_generation/layers/moler_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,14 @@
             atom_featurisers=self._atom_featurisers,
             motif_vocabulary=self._motif_vocabulary,
             uses_categorical_features=self.uses_categorical_features,
             **kwargs,
         )
 
     def compute_metrics(self, *, batch_features, batch_labels, task_output) -> MoLeRDecoderMetrics:
-
         node_classification_loss = self.compute_node_type_selection_loss(
             node_type_logits=task_output.node_type_logits,
             node_type_multihot_labels=batch_labels["correct_node_type_choices"],
         )
 
         first_node_classification_loss = self.compute_first_node_type_selection_loss(
             first_node_type_logits=task_output.first_node_type_logits,
@@ -1124,15 +1123,14 @@
         initial_molecules: Optional[List[Optional[Chem.Mol]]] = None,
         mol_ids: Optional[Iterable[Any]] = None,
         store_generation_traces: bool = False,
         max_num_steps: int = 120,
         beam_size: int = 1,
         sampling_mode: DecoderSamplingMode = DecoderSamplingMode.GREEDY,
     ) -> List[MoLeRDecoderState]:
-
         """Decoding procedure for MoLeR.
 
         This method can handle generation of many graphs in parallel and implements greedy
         decoding. Roughly, the following algorithm is implemented:
 
         while True:
             new_atom_or_motif = pick_atom_or_motif(G, sampled_input_representation)
@@ -1426,15 +1424,15 @@
                 )
 
                 for decoder_state, attachment_point_picks, attachment_point_logits in zip(
                     require_attachment_point_states,
                     attachment_pick_results,
                     attachment_pick_logits,
                 ):
-                    for (attachment_point_pick, attachment_point_logprob) in attachment_point_picks:
+                    for attachment_point_pick, attachment_point_logprob in attachment_point_picks:
                         attachment_point_choice_info = None
                         if store_generation_traces:
                             attachment_point_choice_info = MoleculeGenerationAttachmentPointChoiceInfo(
                                 partial_molecule_adjacency_lists=decoder_state.adjacency_lists,
                                 motif_nodes=decoder_state.atoms_to_mark_as_visited,
                                 candidate_attachment_points=decoder_state.candidate_attachment_points,
                                 candidate_idx_to_prob=tf.nn.softmax(attachment_point_logits),
@@ -1456,15 +1454,15 @@
             # Step 3: Pick fresh bonds and populate the next round of decoding steps:
             require_bond_states = restrict_to_beam_size_per_mol(require_bond_states, beam_size)
             bond_pick_results = self._decoder_pick_new_bond_types(
                 decoder_states=require_bond_states,
                 store_generation_traces=store_generation_traces,
                 sampling_mode=sampling_mode,
             )
-            for (decoder_state, (bond_picks, edge_choice_info)) in zip(
+            for decoder_state, (bond_picks, edge_choice_info) in zip(
                 require_bond_states, bond_pick_results
             ):
                 if len(bond_picks) == 0:
                     # There were no valid options for this bonds, so we treat this as if
                     # predicting no more bonds with probability 1.0:
                     # print(I {decoder_state.molecule_id} {decoder_state.logprob:12f}: No more allowed bonds to node {decoder_state.focus_atom}")
                     new_decoder_states.append(
@@ -1472,15 +1470,15 @@
                             decoder_state,
                             focus_node_finished_logprob=0,
                             edge_choice_info=edge_choice_info,
                         )
                     )
                     continue
 
-                for (bond_pick, bond_pick_logprob) in bond_picks:
+                for bond_pick, bond_pick_logprob in bond_picks:
                     # If the decoder says we need no more bonds for the current focus node,
                     # we mark this and put the decoder state back for the next expansion round:
                     if bond_pick is None:
                         # print(I {decoder_state.molecule_id} {decoder_state.logprob:12f}: Finished connecting bonds to node {decoder_state.focus_atom} - p={bond_pick_logprob:5f}")
                         new_decoder_states.append(
                             MoLeRDecoderState.new_with_focus_marked_as_visited(
                                 decoder_state,
```

### Comparing `molecule_generation-0.3.0/molecule_generation/models/cgvae.py` & `molecule_generation-0.4.0/molecule_generation/models/cgvae.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,14 @@
         self,
         data_iterator: Iterable[Tuple[Dict[str, tf.Tensor], Dict[str, tf.Tensor]]],
         quiet: bool = False,
         training: bool = True,
         max_num_steps: Optional[int] = None,  # Run until dataset ends if None
         aml_run: Optional = None,
     ) -> Tuple[float, float, List[Any]]:
-
         with EpochMetricsLogger(
             window_size=self._logged_loss_smoothing_window_size,
             quiet=quiet,
             aml_run=aml_run,
             training=training,
         ) as metrics_logger:
             for step, (batch_features, batch_labels) in enumerate(data_iterator):
```

### Comparing `molecule_generation-0.3.0/molecule_generation/models/moler_base_model.py` & `molecule_generation-0.4.0/molecule_generation/models/moler_base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
 
         # Skip call to GraphTaskModel.build, in case we don't want to build an
         # encoder GNN.
 
     def _compute_decoder_loss_and_metrics(
         self, batch_features, task_output, batch_labels
     ) -> Tuple[tf.Tensor, MoLeRDecoderMetrics]:
-
         decoder_metrics = self.decoder.compute_metrics(
             batch_features=batch_features, batch_labels=batch_labels, task_output=task_output
         )
 
         total_loss = (
             self._params["node_classification_loss_weight"]
             * decoder_metrics.node_classification_loss
@@ -196,15 +195,14 @@
             )
 
         return total_loss, decoder_metrics
 
     def _get_decoder_output(
         self, *, batch_features, molecule_representations, training
     ) -> MoLeRDecoderOutput:
-
         partial_adjacency_lists: Tuple[tf.Tensor, ...] = tuple(
             batch_features[f"partial_adjacency_list_{edge_type_idx}"]
             for edge_type_idx in range(self._num_edge_types)
         )  # Each element has shape (E, 2)
         decoder_output = self._decoder_layer(
             MoLeRDecoderInput(
                 node_features=batch_features["partial_node_features"],
```

### Comparing `molecule_generation-0.3.0/molecule_generation/models/moler_generator.py` & `molecule_generation-0.4.0/molecule_generation/models/moler_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         self,
         batch_features: Dict[str, tf.Tensor],
         final_node_representations: Optional[
             Any
         ],  # Ignored: here for consistency of interface with moler_vae
         training: bool,
     ) -> MoLeRGeneratorOutput:
-
         molecule_representations = tf.zeros(
             (batch_features["num_partial_graphs_in_batch"], self.latent_dim)
         )
         decoder_output = self._get_decoder_output(
             batch_features=batch_features,
             molecule_representations=molecule_representations,
             training=training,
@@ -79,15 +78,14 @@
     def build(self, input_shapes: Dict[str, Any]):
         super().build(input_shapes=input_shapes)
         # Skip call to GraphTaskModel.build, since we don't want to build an
         # encoder GNN for this model
         self.built = True
 
     def compute_epoch_metrics(self, task_results: List[Any]) -> Tuple[float, str]:
-
         average_loss = self._dict_average(task_results, "loss")
         result_string = f"\n" f"Avg weighted sum. of graph losses: {average_loss: 7.4f}\n"
 
         graph_generation_losses = self._get_graph_generation_losses(task_results)
         result_string += self._format_graph_generation_losses(graph_generation_losses)
 
         return average_loss, result_string
```

### Comparing `molecule_generation-0.3.0/molecule_generation/models/moler_vae.py` & `molecule_generation-0.4.0/molecule_generation/models/moler_vae.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,14 @@
                     dropout_rate=prop_predictor_hypers["dropout_rate"],
                     property_stddev=prop_stddev,
                 )
             else:
                 raise ValueError(f"Unknown property type {prop_type}")
 
     def build(self, input_shapes: Dict[str, Any]):
-
         # Build decoder
         super().build(input_shapes=input_shapes)
 
         # Compute some sizes and shapes we'll re-use a few times:
         final_node_representation_dim = self._params["gnn_hidden_dim"]
         if self._params["use_intermediate_gnn_results"]:
             # In this case, we have one initial representation + results for all layers:
@@ -409,15 +408,14 @@
 
     def compute_vae_metrics(
         self,
         batch_features: Dict[str, tf.Tensor],
         task_output: MoLeRVaeOutput,
         batch_labels: Dict[str, tf.Tensor],
     ) -> MoLeRMetrics:
-
         total_loss, decoder_metrics = self._compute_decoder_loss_and_metrics(
             batch_features=batch_features, task_output=task_output, batch_labels=batch_labels
         )
 
         kl_divergence_summand = (
             tf.square(task_output.graph_representation_mean)
             + tf.exp(task_output.graph_representation_log_variance)
@@ -471,15 +469,14 @@
     def _get_graph_generation_losses(self, task_results: List[Any]) -> List[Tuple[str, str]]:
         graph_generation_losses = super()._get_graph_generation_losses(task_results)
         average_kl_divergence = self._dict_average(task_results, "kl_divergence")
         graph_generation_losses.append(("Avg KL divergence:", f"{average_kl_divergence: 7.4f}\n"))
         return graph_generation_losses
 
     def compute_epoch_metrics(self, task_results: List[Any]) -> Tuple[float, str]:
-
         # Compute results for the individual property predictors.
         # Weigh their respective contributions using the loss weight.
         prop_to_task_results: Dict[str, List[Dict[str, Any]]] = {
             prop_name: [] for prop_name in self._property_predictors.keys()
         }
         for task_result in task_results:
             for prop_name, prop_result in task_result["property_to_metrics"].items():
```

### Comparing `molecule_generation-0.3.0/molecule_generation/preprocessing/cgvae_generation_trace.py` & `molecule_generation-0.4.0/molecule_generation/preprocessing/cgvae_generation_trace.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/preprocessing/data_conversion_utils.py` & `molecule_generation-0.4.0/molecule_generation/preprocessing/data_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/preprocessing/generation_order.py` & `molecule_generation-0.4.0/molecule_generation/preprocessing/generation_order.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/preprocessing/graph_sample.py` & `molecule_generation-0.4.0/molecule_generation/preprocessing/graph_sample.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/preprocessing/moler_generation_trace.py` & `molecule_generation-0.4.0/molecule_generation/preprocessing/moler_generation_trace.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/preprocessing/preprocess.py` & `molecule_generation-0.4.0/molecule_generation/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/dataset/test_jsonl_cgvae_trace_dataset_preprocessing.py` & `molecule_generation-0.4.0/molecule_generation/test/dataset/test_jsonl_cgvae_trace_dataset_preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,50 +11,40 @@
 from molecule_generation.chem.atom_feature_utils import get_default_atom_featurisers
 from molecule_generation.preprocessing.preprocess import preprocess_jsonl_files
 from molecule_generation.chem.molecule_dataset_utils import featurise_smiles_datapoints
 from molecule_generation.utils.preprocessing_utils import save_data, write_jsonl_gz_data
 
 
 @pytest.fixture
-def smiles_list():
-    smiles_file = os.path.join(
-        os.path.dirname(__file__), "..", "test_datasets", "10_test_smiles.smiles"
-    )
-    with open(smiles_file) as f:
-        data = f.readlines()
-    return data
-
-
-@pytest.fixture
 def interrim_dir():
     save_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "tmp")
     os.mkdir(save_dir)
     yield save_dir
     # Tear down:
     if os.path.exists(save_dir):
         shutil.rmtree(save_dir)
 
 
-def test_write_smiles_to_jsonl(smiles_list, interrim_dir):
-    smiles_dict = [{"SMILES": x.strip()} for x in smiles_list]
+def test_write_smiles_to_jsonl(test_smiles, interrim_dir):
+    smiles_dict = [{"SMILES": x.strip()} for x in test_smiles]
     data = featurise_smiles_datapoints(
         train_data=smiles_dict,
         valid_data=smiles_dict,
         test_data=smiles_dict,
         atom_feature_extractors=get_default_atom_featurisers(),
         temporary_save_directory=RichPath.create(interrim_dir),
     )
     save_path_name = os.path.join(interrim_dir, "train.jsonl.gz")
     num_written = write_jsonl_gz_data(save_path_name, data=data.train_data)
     assert num_written == 10
 
 
-def test_read_and_write_jsonl_files(smiles_list, interrim_dir):
+def test_read_and_write_jsonl_files(test_smiles, interrim_dir):
     # Prepare the jsonl.gz files
-    smiles_dict = [{"SMILES": x.strip()} for x in smiles_list]
+    smiles_dict = [{"SMILES": x.strip()} for x in test_smiles]
     data = featurise_smiles_datapoints(
         train_data=smiles_dict,
         valid_data=smiles_dict,
         test_data=smiles_dict,
         atom_feature_extractors=get_default_atom_featurisers(),
     )
     save_data(data, output_dir=interrim_dir)
```

### Comparing `molecule_generation-0.3.0/molecule_generation/test/dataset/test_jsonl_moler_trace_dataset_preprocessing.py` & `molecule_generation-0.4.0/molecule_generation/test/dataset/test_jsonl_moler_trace_dataset_preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,50 +11,40 @@
 from molecule_generation.chem.atom_feature_utils import get_default_atom_featurisers
 from molecule_generation.preprocessing.preprocess import preprocess_jsonl_files
 from molecule_generation.chem.molecule_dataset_utils import featurise_smiles_datapoints
 from molecule_generation.utils.preprocessing_utils import save_data, write_jsonl_gz_data
 
 
 @pytest.fixture
-def smiles_list():
-    smiles_file = os.path.join(
-        os.path.dirname(__file__), "..", "test_datasets", "10_test_smiles.smiles"
-    )
-    with open(smiles_file) as f:
-        data = f.readlines()
-    return data
-
-
-@pytest.fixture
 def interrim_dir():
     save_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "tmp")
     os.mkdir(save_dir)
     yield save_dir
     # Tear down:
     if os.path.exists(save_dir):
         shutil.rmtree(save_dir)
 
 
-def test_write_smiles_to_jsonl(smiles_list, interrim_dir):
-    smiles_dict = [{"SMILES": x.strip()} for x in smiles_list]
+def test_write_smiles_to_jsonl(test_smiles, interrim_dir):
+    smiles_dict = [{"SMILES": x.strip()} for x in test_smiles]
     data = featurise_smiles_datapoints(
         train_data=smiles_dict,
         valid_data=smiles_dict,
         test_data=smiles_dict,
         atom_feature_extractors=get_default_atom_featurisers(),
         temporary_save_directory=RichPath.create(interrim_dir),
     )
     save_path_name = os.path.join(interrim_dir, "train.jsonl.gz")
     num_written = write_jsonl_gz_data(save_path_name, data=data.train_data)
     assert num_written == 10
 
 
-def test_read_and_write_jsonl_files(smiles_list, interrim_dir):
+def test_read_and_write_jsonl_files(test_smiles, interrim_dir):
     # Prepare the jsonl.gz files
-    smiles_dict = [{"SMILES": x.strip()} for x in smiles_list]
+    smiles_dict = [{"SMILES": x.strip()} for x in test_smiles]
     data = featurise_smiles_datapoints(
         train_data=smiles_dict,
         valid_data=smiles_dict,
         test_data=smiles_dict,
         atom_feature_extractors=get_default_atom_featurisers(),
     )
     save_data(data, output_dir=interrim_dir)
```

### Comparing `molecule_generation-0.3.0/molecule_generation/test/integration/test_data_moler_integration.py` & `molecule_generation-0.4.0/molecule_generation/test/integration/test_data_moler_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     # Clear the Keras session so that unique naming does not mess up weight loading.
     tf.keras.backend.clear_session()
 
     caffeine_smiles = "CN1C=NC2=C1C(=O)N(C(=O)N2C)C"
 
     with MoLeRInferenceServer(get_model_path(tmp_test_directory)) as moler:
         embedding = moler.encode([caffeine_smiles])
-        smiles = [s for s, _ in moler.decode(embedding)]
+        smiles = [s for s, _, _ in moler.decode(embedding)]
 
     assert len(smiles) == 1
 
 
 def test_can_decode_smiles_with_scaffold_trained_model(capsys, tmp_test_directory):
     # Clear the Keras session so that unique naming does not mess up weight loading.
     tf.keras.backend.clear_session()
@@ -349,15 +349,15 @@
     scaffold_mol = Chem.MolFromSmiles("CCC1C(O)C(O)C=CC1C(C)NC")  # 14 atoms
     scaffold_smarts = Chem.MolToSmarts(scaffold_mol)
     num_atoms_in_substructure = scaffold_mol.GetNumAtoms()
 
     with MoLeRInferenceServer(get_model_path(tmp_test_directory)) as moler:
         # Initial Molecules = [Scaffold]
         embedding = moler.encode([base_smiles])
-        smiles = [s for s, _ in moler.decode(embedding, init_mols=[scaffold_mol])]
+        smiles = [s for s, _, _ in moler.decode(embedding, init_mols=[scaffold_mol])]
 
     assert len(smiles) == 1
 
     # Check if the scaffold still exists in all of the samples:
     for sample in smiles:
         mol = Chem.MolFromSmiles(sample)
         substructure_match = get_substructure_match(mol, scaffold_smarts)
@@ -372,25 +372,25 @@
     scaffold_mol = Chem.MolFromSmiles("CCC1C(O)C(O)C=CC1C(C)NC")  # 14 atoms
     scaffold_smarts = Chem.MolToSmarts(scaffold_mol)
     num_atoms_in_substructure = scaffold_mol.GetNumAtoms()
 
     with MoLeRInferenceServer(get_model_path(tmp_test_directory)) as moler:
         # Initial Molecules = [Scaffold, None]
         embeddings = moler.encode([base_smiles, base_smiles])
-        smiles = [s for s, _ in moler.decode(embeddings, init_mols=[scaffold_mol, None])]
+        smiles = [s for s, _, _ in moler.decode(embeddings, init_mols=[scaffold_mol, None])]
 
         assert len(smiles) == 2
 
         substructure_match = get_substructure_match(Chem.MolFromSmiles(smiles[0]), scaffold_smarts)
         assert len(substructure_match) == num_atoms_in_substructure
 
         # Initial Molecules = [None, None]
         embeddings = moler.encode([base_smiles, base_smiles])
-        smiles = [s for s, _ in moler.decode(embeddings, init_mols=[None, None])]
+        smiles = [s for s, _, _ in moler.decode(embeddings, init_mols=[None, None])]
 
         assert len(smiles) == 2
 
         # Initial Molecules = None
         embeddings = moler.encode([base_smiles, base_smiles])
-        smiles = [s for s, _ in moler.decode(embeddings)]
+        smiles = [s for s, _, _ in moler.decode(embeddings)]
 
         assert len(smiles) == 2
```

### Comparing `molecule_generation-0.3.0/molecule_generation/test/layers/test_cgvae_decoder.py` & `molecule_generation-0.4.0/molecule_generation/test/layers/test_cgvae_decoder.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/layers/test_moler_decoder.py` & `molecule_generation-0.4.0/molecule_generation/test/layers/test_moler_decoder.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/models/test_gnn_vae.py` & `molecule_generation-0.4.0/molecule_generation/test/models/test_gnn_vae.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/models/test_moler_vae.py` & `molecule_generation-0.4.0/molecule_generation/test/models/test_moler_vae.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/preprocessing/test_data_conversion_utils.py` & `molecule_generation-0.4.0/molecule_generation/test/preprocessing/test_data_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/preprocessing/test_generate_test_dataset.py` & `molecule_generation-0.4.0/molecule_generation/test/preprocessing/test_generate_test_dataset.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/preprocessing/test_generation_trace.py` & `molecule_generation-0.4.0/molecule_generation/test/preprocessing/test_generation_trace.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/metadata.pkl.gz` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/metadata.pkl.gz`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/test_0/test_0.pkl.gz` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/test_0/test_0.pkl.gz`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/train_0/train_0.pkl.gz` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/train_0/train_0.pkl.gz`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/cgvae_traces/valid_0/valid_0.pkl.gz` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/cgvae_traces/valid_0/valid_0.pkl.gz`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/generate_test_dataset.py` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/generate_test_dataset.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/metadata.pkl.gz` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/metadata.pkl.gz`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/test_0/test_0.pkl.gz` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/test_0/test_0.pkl.gz`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/train_0/train_0.pkl.gz` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/train_0/train_0.pkl.gz`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/test_datasets/moler_traces/valid_0/valid_0.pkl.gz` & `molecule_generation-0.4.0/molecule_generation/test/test_datasets/moler_traces/valid_0/valid_0.pkl.gz`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/utils/test_beam_utils.py` & `molecule_generation-0.4.0/molecule_generation/test/utils/test_beam_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/utils/test_decoder_batching.py` & `molecule_generation-0.4.0/molecule_generation/test/utils/test_decoder_batching.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/utils/test_motif_utils.py` & `molecule_generation-0.4.0/molecule_generation/test/utils/test_motif_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/utils/test_topology_constraints.py` & `molecule_generation-0.4.0/molecule_generation/test/utils/test_topology_constraints.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/test/utils/test_valence_constraints.py` & `molecule_generation-0.4.0/molecule_generation/test/utils/test_valence_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         candidate_target_nodes=edge_choices[:, 1],
         adjacency_lists=adjacency_lists,
         node_types=node_types,
     )
 
     # Then:
     expected_edge_choices = np.zeros(shape=(0, 2), dtype=np.int32)
-    expected_open_edges = np.zeros(shape=(0,), dtype=np.bool)
+    expected_open_edges = np.zeros(shape=(0,), dtype=bool)
     np.testing.assert_array_equal(edge_choices, expected_edge_choices)
     np.testing.assert_array_equal(target_candidate_mask, expected_open_edges)
 
 
 def test_constrain_edge_choices_based_on_valence_if_focus_node_is_full():
     # Given molecule of all carbons:
     #
```

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/beam_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/beam_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/cgvae_visualisation_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/cgvae_visualisation_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/cli_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/data_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/decoder_batching.py` & `molecule_generation-0.4.0/molecule_generation/utils/decoder_batching.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     atom_featurisers: List[AtomTypeFeatureExtractor],
     motif_vocabulary: Optional[MotifVocabulary],
     uses_categorical_features: bool,
     decoder_states: List[MoLeRDecoderState],
     init_batch_callback: Callable[[Dict[str, Any]], None],
     add_state_to_batch_callback: Callable[[Dict[str, Any], MoLeRDecoderState], None],
 ) -> Generator[Tuple[Dict[str, Any], List[MoLeRDecoderState]], None, None]:
-
     graph_id_offset = 0
 
     def _get_empty_batch() -> Dict[str, Any]:
         new_batch = {
             "nodes_in_batch": 0,
             "graphs_in_batch": 0,
             "molecule_representations": [],
```

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/epoch_metrics_logger.py` & `molecule_generation-0.4.0/molecule_generation/utils/epoch_metrics_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 class EpochMetricsLogger:
     """Logs metrics for an epoch of training"""
 
     def __init__(
         self, *, window_size: int = 100, quiet: bool, aml_run: Optional, training: bool
     ) -> None:
-
         self._window_size = window_size
         self._quiet = quiet
         self._aml_run = aml_run
         self._training = training
 
         # Initialise everything in case you don't want to use this as a contextmanager
         self._start_logging()
```

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/model_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/moler_decoding_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/moler_decoding_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/moler_inference_server.py` & `molecule_generation-0.4.0/molecule_generation/utils/moler_inference_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from rdkit import Chem
 
 from molecule_generation.dataset.in_memory_trace_dataset import DataFold, InMemoryTraceDataset
 from molecule_generation.models.moler_generator import MoLeRGenerator
 from molecule_generation.models.moler_vae import MoLeRVae
 from molecule_generation.preprocessing.data_conversion_utils import remove_non_max_frags
 from molecule_generation.utils.model_utils import load_vae_model_and_dataset
-from molecule_generation.utils.moler_decoding_utils import DecoderSamplingMode, MoLeRDecoderState
+from molecule_generation.utils.moler_decoding_utils import (
+    DecoderSamplingMode,
+    MoLeRDecoderState,
+    MoleculeGenerationChoiceInfo,
+)
 
 Pathlike = Union[str, pathlib.Path]
 
 
 class MoLeRRequestType(enum.Enum):
     TERMINATE = enum.auto()
     ENCODE = enum.auto()
@@ -58,15 +62,15 @@
         data_fold=DataFold.TEST, use_worker_threads=False
     ):
         final_node_representations = model.compute_final_node_representations(
             batch_features, training=False
         )
 
         # Get means and log variances, both with shape [NumGraphsInBatch, LatentDim].
-        (graph_rep_mean, graph_rep_logvar, _,) = model.compute_latent_molecule_representations(
+        (graph_rep_mean, graph_rep_logvar, _) = model.compute_latent_molecule_representations(
             final_node_representations=final_node_representations,
             num_graphs=batch_features["num_graphs_in_batch"],
             node_to_graph_map=batch_features["node_to_graph_map"],
             partial_graph_to_original_graph_map=batch_features[
                 "partial_graph_to_original_graph_map"
             ],
             training=False,
@@ -80,37 +84,53 @@
     return result
 
 
 def _decode_from_latents(
     model: Union[MoLeRVae, MoLeRGenerator],
     latent_representations: np.ndarray,
     include_latent_samples: bool = False,
+    include_generation_steps: bool = False,
     init_mols: List[Any] = None,
     beam_size: int = 1,
     sampling_mode: DecoderSamplingMode = DecoderSamplingMode.GREEDY,
-) -> Iterator[Tuple[str, Optional[np.ndarray]]]:
+) -> Iterator[Tuple[str, Optional[np.ndarray], Optional[List[MoleculeGenerationChoiceInfo]]]]:
     decoder_states = model.decoder.decode(
         graph_representations=latent_representations,
         initial_molecules=init_mols,
+        store_generation_traces=include_generation_steps,
         beam_size=beam_size,
         sampling_mode=sampling_mode,
     )
 
     decoder_states_by_id: DefaultDict[Any, List[MoLeRDecoderState]] = defaultdict(list)
     for decoder_state in decoder_states:
         decoder_states_by_id[decoder_state.molecule_id].append(decoder_state)
 
     for per_sampled_latent_results in sorted(decoder_states_by_id.items(), key=lambda kv: kv[0]):
         best_decoder_state = max(per_sampled_latent_results[1], key=lambda s: s.logprob)
         mol = remove_non_max_frags(Chem.RWMol(best_decoder_state.molecule))
+
         input_mol_representation = None
         if include_latent_samples:
             input_mol_representation = best_decoder_state.molecule_representation
 
-        yield (Chem.MolToSmiles(mol, isomericSmiles=False), input_mol_representation)
+        generation_steps = None
+        if include_generation_steps:
+            generation_steps = best_decoder_state.generation_steps
+
+            # Before returning, we slightly clean up the molecules in the trace. In particular, this
+            # fixes implicit hydrogen count for the partial molecules.
+            for step in generation_steps:
+                Chem.SanitizeMol(step.molecule)
+
+        yield (
+            Chem.MolToSmiles(mol, isomericSmiles=False),
+            input_mol_representation,
+            generation_steps,
+        )
 
 
 def _moler_worker_process(
     model_path: str,
     request_queue,
     output_queue,
 ):
@@ -127,22 +147,24 @@
                 dataset, moler_model, smiles_list, include_log_variances=include_log_variances
             )
             output_queue.put((uid, encoded_mols))
         elif request == MoLeRRequestType.DECODE:
             (
                 latent_representations,
                 include_latent_samples,
+                include_generation_steps,
                 init_mols,
                 beam_size,
                 sampling_mode,
             ) = arguments
             decoder_results = _decode_from_latents(
                 moler_model,
                 latent_representations,
                 include_latent_samples,
+                include_generation_steps,
                 init_mols,
                 beam_size,
                 sampling_mode,
             )
             output_queue.put((uid, list(decoder_results)))
         else:
             raise ValueError(f"Unknown worker request {request}!")
@@ -282,18 +304,19 @@
 
         return self.try_collect_results(num_results)
 
     def decode(
         self,
         latent_representations: np.ndarray,
         include_latent_samples: bool = False,
+        include_generation_steps: bool = False,
         init_mols: List[Any] = None,
         beam_size: int = 1,
         sampling_mode: DecoderSamplingMode = DecoderSamplingMode.GREEDY,
-    ) -> List[Tuple[str, Optional[np.ndarray]]]:
+    ) -> List[Tuple[str, Optional[np.ndarray], Optional[List[MoleculeGenerationChoiceInfo]]]]:
         self.init_workers()
 
         # Choose chunk size such that all workers have something to do.
         chunk_size = min(
             self._max_num_samples_per_chunk, len(latent_representations) // self._num_workers + 1
         )
 
@@ -313,14 +336,15 @@
             self._request_queue.put(
                 (
                     MoLeRRequestType.DECODE,
                     num_results,
                     (
                         latents_chunk,
                         include_latent_samples,
+                        include_generation_steps,
                         list(next(init_mol_chunks)),
                         beam_size,
                         sampling_mode,
                     ),
                 )
             )
             num_results += 1
```

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/moler_visualisation_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/moler_visualisation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,14 @@
                             predictions.node_type_logits[node_choice_idx, :]
                         ).numpy(),
                     ),
                     choice_descr="next addition to partial molecule",
                 )
 
     def visualise_from_samples(self, molecule_representation: np.ndarray):
-
         property_data: Dict[str, PropertyPredictionInformation] = {}
 
         for prop_name in self.supported_property_names:
             property_data[prop_name] = PropertyPredictionInformation(
                 prediction=self.vae._property_predictors[prop_name](
                     [molecule_representation], training=False
                 ).numpy(),
```

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/multiprocessing_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/preprocessing_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/property_models.py` & `molecule_generation-0.4.0/molecule_generation/utils/property_models.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/sequential_worker_pool.py` & `molecule_generation-0.4.0/molecule_generation/utils/sequential_worker_pool.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/sharded_data_reader.py` & `molecule_generation-0.4.0/molecule_generation/utils/sharded_data_reader.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/utils/training_utils.py` & `molecule_generation-0.4.0/molecule_generation/utils/training_utils.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/visualisation/cgvae_visualiser_cli.py` & `molecule_generation-0.4.0/molecule_generation/visualisation/cgvae_visualiser_cli.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/visualisation/cgvae_visualiser_html.py` & `molecule_generation-0.4.0/molecule_generation/visualisation/cgvae_visualiser_html.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/visualisation/moler_visualiser_cli.py` & `molecule_generation-0.4.0/molecule_generation/visualisation/moler_visualiser_cli.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/visualisation/moler_visualiser_html.py` & `molecule_generation-0.4.0/molecule_generation/visualisation/moler_visualiser_html.py`

 * *Files identical despite different names*

### Comparing `molecule_generation-0.3.0/molecule_generation/wrapper.py` & `molecule_generation-0.4.0/molecule_generation/wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 import numpy as np
 import tensorflow as tf
 from rdkit import Chem
 
 from molecule_generation.models.moler_generator import MoLeRGenerator
 from molecule_generation.models.moler_vae import MoLeRVae
-from molecule_generation.utils.moler_decoding_utils import DecoderSamplingMode
+from molecule_generation.utils.moler_decoding_utils import (
+    DecoderSamplingMode,
+    MoleculeGenerationChoiceInfo,
+)
 from molecule_generation.utils.model_utils import get_model_class, get_model_parameters
 
 
 Pathlike = Union[str, pathlib.Path]
 
 
 class ModelWrapper(ContextManager):
@@ -111,41 +114,48 @@
             smiles_list, include_log_variances=include_log_variances
         )
 
     def decode(
         self,
         latents: List[np.ndarray],  # type: ignore
         scaffolds: Optional[List[Optional[str]]] = None,
-    ) -> List[str]:
+        include_generation_steps: bool = False,
+    ) -> Union[List[str], List[Tuple[str, MoleculeGenerationChoiceInfo]]]:
         """Decode molecules from latent vectors, potentially conditioned on scaffolds.
 
         Args:
             latents: List of latent vectors to decode.
             scaffolds: List of scaffold molecules, one per each vector. Each scaffold in
                 the list can be `None` (denoting lack of scaffold) or the whole list can
                 be `None`, which is synonymous with `[None, ..., None]`.
+            include_generation_steps: Whether to also track and return various metadata about the
+                full generation trace.
 
         Returns:
-            List of SMILES strings.
+            List of results. Each result is just a SMILES string if `include_generation_steps` is
+            `False`, and a pair containing the SMILES string and the generation trace otherwise.
         """
         if scaffolds is not None:
             scaffolds = [
                 Chem.MolFromSmiles(scaffold) if scaffold is not None else None
                 for scaffold in scaffolds
             ]
 
-        return [
-            smiles_str
-            for smiles_str, _ in self._inference_server.decode(
-                latent_representations=np.stack(latents),
-                include_latent_samples=False,
-                init_mols=scaffolds,
-                beam_size=self.beam_size,
-            )
-        ]
+        results = self._inference_server.decode(
+            latent_representations=np.stack(latents),
+            include_latent_samples=False,
+            include_generation_steps=include_generation_steps,
+            init_mols=scaffolds,
+            beam_size=self.beam_size,
+        )
+
+        if include_generation_steps:
+            return [(smiles_str, steps) for smiles_str, _, steps in results]
+        else:
+            return [smiles_str for smiles_str, _, _ in results]
 
     def sample(self, num_samples: int) -> List[str]:
         """Sample SMILES strings from the model.
 
         Args:
             num_samples: Number of samples to return.
```

### Comparing `molecule_generation-0.3.0/molecule_generation.egg-info/PKG-INFO` & `molecule_generation-0.4.0/molecule_generation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 Metadata-Version: 2.1
 Name: molecule-generation
-Version: 0.3.0
+Version: 0.4.0
 Summary: Implementations of deep generative models of molecules.
 Home-page: https://github.com/microsoft/molecule-generation/
 Author: Krzysztof Maziarz
 Author-email: krzysztof.maziarz@microsoft.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MoLeR: A Model for Molecule Generation
 
 [![CI](https://github.com/microsoft/molecule-generation/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/microsoft/molecule-generation/actions/workflows/ci.yml)
 [![license](https://img.shields.io/github/license/microsoft/molecule-generation.svg)](https://github.com/microsoft/molecule-generation/blob/main/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/molecule-generation.svg)](https://pypi.org/project/molecule-generation/)
+[![python](https://img.shields.io/pypi/pyversions/molecule_generation)](https://www.python.org/downloads/)
 [![code style](https://img.shields.io/badge/code%20style-black-202020.svg)](https://github.com/ambv/black)
 
-This repository contains training and inference code for the MoLeR model introduced in [Learning to Extend Molecular Scaffolds with Structural Motifs](https://arxiv.org/abs/2103.03864). We also include our implementation of CGVAE, but it currently lacks integration with the high-level model interface, and is provided mostly for reference.
+This repository contains training and inference code for the MoLeR model introduced in [Learning to Extend Molecular Scaffolds with Structural Motifs](https://arxiv.org/abs/2103.03864). We also include our implementation of CGVAE, but without integration with the high-level model interface.
 
 ## Quick start
 
-The `molecule_generation` package can be installed via `pip`, but it additionally depends on `rdkit` and (if one wants to use a GPU) on correctly setting up CUDA libraries. One approach to get both is through our minimalistic `conda` environment:
+`molecule_generation` can be installed via `pip`, but it additionally depends on `rdkit` and (if one wants to use a GPU) on setting up CUDA libraries. One can get both through `conda`:
 
 ```bash
 conda env create -f environment.yml
 conda activate moler-env
 ```
 
-This environment pins the versions of `python`, `rdkit` and `tensorflow` for reproducibility, but `molecule_generation` is compatible with a range of versions of these dependencies.
+Our package was tested with `python>=3.7`, `tensorflow>=2.1.0` and `rdkit>=2020.09.1`; see the `environment*.yml` files for the exact configurations tested in CI.
 
-To then install the latest release of `molecule_generation`, simply run
+To then install the latest release of `molecule_generation`, run
 ```bash
 pip install molecule-generation
 ```
 
-Alternatively, running `pip install -e .` within the root folder installs the latest state of the code, including changes that were merged into `main` but not yet released.
-
-Note that in the instructions above we pinned the `rdkit` version, as this is the version the code has been tested with. However, our code is likely to work with other modern version of `rdkit` as well.
-Finally, if `tensorflow` installation doesn't work out-of-the-box for your particular system, you may need to refer to [the tensorflow website](https://www.tensorflow.org/install) for guidelines.
+Alternatively, `pip install -e .` within the root folder installs the latest state of the code, including changes that were merged into `main` but not yet released.
 
 A MoLeR checkpoint trained using the default hyperparameters is available [here](https://figshare.com/ndownloader/files/34642724). This file needs to be saved in a fresh folder `MODEL_DIR` (e.g., `/tmp/MoLeR_checkpoint`) and be renamed to have the `.pkl` ending (e.g., to `GNN_Edge_MLP_MoLeR__2022-02-24_07-16-23_best.pkl`). Then you can sample 10 molecules by running
 
 ```bash
 molecule_generation sample MODEL_DIR 10
 ```
 
-See the next sections for how to train your own model and run more advanced inference.
+See below for how to train your own model and run more advanced inference.
+
+### Troubleshooting
+
+> Q: I am in China and so the figshare checkpoint link does not work for me.
+>
+> A: You can try [this link](https://pan.baidu.com/s/1lkiWK9-d5MvNyzqRrusGXA?pwd=4hij) instead.
+
+> Q: My particular combination of dependency versions does not work.
+>
+> A: Please submit an issue and default to using one of the pinned configurations from `environment-py*.yml` in the meantime.
+
+> Q: Installing `tensorflow` on my system does not work.
+>
+> A: Please refer to [the tensorflow website](https://www.tensorflow.org/install) for guidelines.
 
 ## Workflow
 
 Working with MoLeR can be roughly divided into four stages:
 - *data preprocessing*, where a plain text list of SMILES strings is turned into `*.pkl` files containing descriptions of the molecular graphs and generation traces;
 - *training*, where MoLeR is trained on the preprocessed data until convergence;
 - *inference*, where one loads the model and performs batched encoding, decoding or sampling; and (optionally)
```

### Comparing `molecule_generation-0.3.0/molecule_generation.egg-info/SOURCES.txt` & `molecule_generation-0.4.0/molecule_generation.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 .gitignore
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE
 README.md
 SECURITY.md
 SUPPORT.md
+environment-py37.yml
+environment-py38.yml
+environment-py39.yml
 environment.yml
 pyproject.toml
 setup.py
 .github/workflows/ci.yml
 molecule_generation/__init__.py
 molecule_generation/version.py
 molecule_generation/wrapper.py
@@ -54,16 +57,18 @@
 molecule_generation/preprocessing/cgvae_generation_trace.py
 molecule_generation/preprocessing/data_conversion_utils.py
 molecule_generation/preprocessing/generation_order.py
 molecule_generation/preprocessing/graph_sample.py
 molecule_generation/preprocessing/moler_generation_trace.py
 molecule_generation/preprocessing/preprocess.py
 molecule_generation/test/__init__.py
+molecule_generation/test/conftest.py
 molecule_generation/test/dataset/test_jsonl_cgvae_trace_dataset_preprocessing.py
 molecule_generation/test/dataset/test_jsonl_moler_trace_dataset_preprocessing.py
+molecule_generation/test/integration/test_cli.py
 molecule_generation/test/integration/test_data_moler_integration.py
 molecule_generation/test/layers/test_cgvae_decoder.py
 molecule_generation/test/layers/test_moler_decoder.py
 molecule_generation/test/models/test_gnn_vae.py
 molecule_generation/test/models/test_moler_vae.py
 molecule_generation/test/preprocessing/test_data_conversion_utils.py
 molecule_generation/test/preprocessing/test_generate_test_dataset.py
```

### Comparing `molecule_generation-0.3.0/setup.py` & `molecule_generation-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,10 +33,11 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
```


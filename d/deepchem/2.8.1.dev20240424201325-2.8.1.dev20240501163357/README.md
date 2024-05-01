# Comparing `tmp/deepchem-2.8.1.dev20240424201325.tar.gz` & `tmp/deepchem-2.8.1.dev20240501163357.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.8.1.dev20240424201325.tar", last modified: Wed Apr 24 20:13:26 2024, max compression
+gzip compressed data, was "deepchem-2.8.1.dev20240501163357.tar", last modified: Wed May  1 16:33:57 2024, max compression
```

## Comparing `deepchem-2.8.1.dev20240424201325.tar` & `deepchem-2.8.1.dev20240501163357.tar`

### file list

```diff
@@ -1,390 +1,390 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.322665 deepchem-2.8.1.dev20240424201325/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-24 20:13:26.326665 deepchem-2.8.1.dev20240424201325/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.270665 deepchem-2.8.1.dev20240424201325/deepchem/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.270665 deepchem-2.8.1.dev20240424201325/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84152 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)   118030 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.270665 deepchem-2.8.1.dev20240424201325/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.274665 deepchem-2.8.1.dev20240424201325/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/binding_pocket_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/bio_seq_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.274665 deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)    27676 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20248 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    22111 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    38890 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.274665 deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    28058 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    14808 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.278665 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.278665 deepchem-2.8.1.dev20240424201325/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.278665 deepchem-2.8.1.dev20240424201325/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22429 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.282665 deepchem-2.8.1.dev20240424201325/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17151 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.282665 deepchem-2.8.1.dev20240424201325/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/metalearning/maml.py
--rw-r--r--   0 runner    (1001) docker     (127)    16233 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/metalearning/torch_maml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.282665 deepchem-2.8.1.dev20240424201325/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.286665 deepchem-2.8.1.dev20240424201325/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17354 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.286665 deepchem-2.8.1.dev20240424201325/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/dft/dftxc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.286665 deepchem-2.8.1.dev20240424201325/deepchem/models/dft/hamilton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/dft/hamilton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/dft/hamilton/orbparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.286665 deepchem-2.8.1.dev20240424201325/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    57408 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.286665 deepchem-2.8.1.dev20240424201325/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28179 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    56651 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (127)   144759 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.286665 deepchem-2.8.1.dev20240424201325/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    62329 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    27252 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    25969 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.290665 deepchem-2.8.1.dev20240424201325/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.294665 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/acnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31166 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/dtnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    29583 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (127)    16557 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    58182 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gan.py
--rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14944 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    51159 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28998 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    39504 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (127)    38435 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23111 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    35955 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)   238616 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17126 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18343 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (127)    17860 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (127)    24055 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    27274 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/seqtoseq.py
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/text_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    53816 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/weavemodel_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.298665 deepchem-2.8.1.dev20240424201325/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.302665 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)   165414 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.302665 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    36564 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.306665 deepchem-2.8.1.dev20240424201325/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.306665 deepchem-2.8.1.dev20240424201325/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.306665 deepchem-2.8.1.dev20240424201325/deepchem/rl/torch_rl/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/torch_rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34135 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/torch_rl/torch_a2c.py
--rw-r--r--   0 runner    (1001) docker     (127)    32978 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/rl/torch_rl/torch_ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.306665 deepchem-2.8.1.dev20240424201325/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64330 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.306665 deepchem-2.8.1.dev20240424201325/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    91191 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.310665 deepchem-2.8.1.dev20240424201325/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/attribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/debug_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.310665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/api/getxc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/api/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/data/datastruct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/df/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/df/base_df.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/grid/base_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14735 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/grid/radial_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15817 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/base_hamilton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/intor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/intor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/intor/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/orbparams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/qccalc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/qccalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/qccalc/base_qccalc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/qccalc/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/qccalc/scf_qccalc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/system/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/system/base_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.314665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.318665 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/xc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/xc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35724 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/xc/base_xc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/xc/libxc.py
--rw-r--r--   0 runner    (1001) docker     (127)    40477 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/xc/libxc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/dftutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.318665 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)    23731 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/editable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/grad.py
--rw-r--r--   0 runner    (1001) docker     (127)    50928 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/linop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.318665 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/minimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/rootfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/rootsolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/pure_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    45298 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/solve.py
--rw-r--r--   0 runner    (1001) docker     (127)    37426 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/symeig.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/equivariance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19262 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/periodic_table_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65661 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/safeops_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.322665 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_attribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31537 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_dft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31918 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_differentiation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_equivariance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_periodic_table_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_safe_ops_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:26.270665 deepchem-2.8.1.dev20240424201325/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-24 20:13:26.000000 deepchem-2.8.1.dev20240424201325/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-24 20:13:26.000000 deepchem-2.8.1.dev20240424201325/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:13:26.000000 deepchem-2.8.1.dev20240424201325/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-24 20:13:26.000000 deepchem-2.8.1.dev20240424201325/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 20:13:26.000000 deepchem-2.8.1.dev20240424201325/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 20:13:26.326665 deepchem-2.8.1.dev20240424201325/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-24 20:13:17.000000 deepchem-2.8.1.dev20240424201325/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.416983 deepchem-2.8.1.dev20240501163357/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-01 16:33:57.416983 deepchem-2.8.1.dev20240501163357/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.360983 deepchem-2.8.1.dev20240501163357/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.360983 deepchem-2.8.1.dev20240501163357/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84152 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118030 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.364983 deepchem-2.8.1.dev20240501163357/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.364983 deepchem-2.8.1.dev20240501163357/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/binding_pocket_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/bio_seq_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.364983 deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27676 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20248 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22111 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38890 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.368983 deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28058 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14808 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.372983 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.372983 deepchem-2.8.1.dev20240501163357/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.372983 deepchem-2.8.1.dev20240501163357/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22429 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.372983 deepchem-2.8.1.dev20240501163357/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17151 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.372983 deepchem-2.8.1.dev20240501163357/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/metalearning/maml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16233 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/metalearning/torch_maml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.372983 deepchem-2.8.1.dev20240501163357/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.376983 deepchem-2.8.1.dev20240501163357/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17354 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.380983 deepchem-2.8.1.dev20240501163357/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/dft/dftxc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.380983 deepchem-2.8.1.dev20240501163357/deepchem/models/dft/hamilton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/dft/hamilton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/dft/hamilton/orbparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23457 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.380983 deepchem-2.8.1.dev20240501163357/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57408 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.380983 deepchem-2.8.1.dev20240501163357/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28179 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57000 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144759 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.380983 deepchem-2.8.1.dev20240501163357/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62329 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27252 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17830 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25969 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.380983 deepchem-2.8.1.dev20240501163357/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.388983 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/acnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31166 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/dtnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29583 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22218 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58182 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14944 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51159 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28998 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39504 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38435 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23460 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35955 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238616 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17126 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17860 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24055 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27274 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/seqtoseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/text_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54165 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/weavemodel_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.388983 deepchem-2.8.1.dev20240501163357/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14702 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.396983 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165414 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.396983 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36564 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.396983 deepchem-2.8.1.dev20240501163357/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.400982 deepchem-2.8.1.dev20240501163357/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25374 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.400982 deepchem-2.8.1.dev20240501163357/deepchem/rl/torch_rl/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/torch_rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34135 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/torch_rl/torch_a2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32978 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/rl/torch_rl/torch_ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.400982 deepchem-2.8.1.dev20240501163357/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64330 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.400982 deepchem-2.8.1.dev20240501163357/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91191 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.404982 deepchem-2.8.1.dev20240501163357/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/attribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/debug_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.404982 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.404982 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/api/getxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/api/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/data/datastruct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/df/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/df/base_df.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/grid/base_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14735 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/grid/radial_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15817 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/base_hamilton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/intor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/intor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/intor/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/orbparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/qccalc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/qccalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/qccalc/base_qccalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/qccalc/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/qccalc/scf_qccalc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/system/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/system/base_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.408983 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/xc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/xc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35724 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/xc/base_xc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/xc/libxc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40477 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/xc/libxc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/dftutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.412983 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23731 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/editable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/grad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50928 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/linop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.412983 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16460 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/rootfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/rootsolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/pure_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45298 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37426 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/symeig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14881 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/equivariance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19262 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/periodic_table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65661 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/safeops_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.416983 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_attribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31537 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_dft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31918 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_differentiation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_equivariance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_periodic_table_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_safe_ops_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-01 16:33:47.000000 deepchem-2.8.1.dev20240501163357/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:33:57.360983 deepchem-2.8.1.dev20240501163357/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-01 16:33:57.000000 deepchem-2.8.1.dev20240501163357/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-05-01 16:33:57.000000 deepchem-2.8.1.dev20240501163357/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:33:57.000000 deepchem-2.8.1.dev20240501163357/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-01 16:33:57.000000 deepchem-2.8.1.dev20240501163357/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 16:33:57.000000 deepchem-2.8.1.dev20240501163357/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-01 16:33:57.420982 deepchem-2.8.1.dev20240501163357/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-01 16:33:48.000000 deepchem-2.8.1.dev20240501163357/setup.py
```

### Comparing `deepchem-2.8.1.dev20240424201325/LICENSE` & `deepchem-2.8.1.dev20240501163357/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/PKG-INFO` & `deepchem-2.8.1.dev20240501163357/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.8.1.dev20240424201325
+Version: 2.8.1.dev20240501163357
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.8.1.dev20240424201325/README.md` & `deepchem-2.8.1.dev20240501163357/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/data/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/data/data_loader.py` & `deepchem-2.8.1.dev20240501163357/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/data/datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/data/pytorch_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/data/supports.py` & `deepchem-2.8.1.dev20240501163357/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/dock/binding_pocket.py` & `deepchem-2.8.1.dev20240501163357/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/dock/docking.py` & `deepchem-2.8.1.dev20240501163357/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/dock/pose_generation.py` & `deepchem-2.8.1.dev20240501163357/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/dock/pose_scoring.py` & `deepchem-2.8.1.dev20240501163357/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/atomic_conformation.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/base_classes.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/bert_tokenizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/binding_pocket_features.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/bio_seq_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/bio_seq_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/dft_data.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/graph_data.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/graph_features.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/mol_graphs.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/reaction_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.8.1.dev20240501163357/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/hyper/base_classes.py` & `deepchem-2.8.1.dev20240501163357/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/hyper/gaussian_process.py` & `deepchem-2.8.1.dev20240501163357/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/hyper/grid_search.py` & `deepchem-2.8.1.dev20240501163357/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/hyper/random_search.py` & `deepchem-2.8.1.dev20240501163357/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/metalearning/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/metalearning/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/metalearning/maml.py` & `deepchem-2.8.1.dev20240501163357/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/metalearning/torch_maml.py` & `deepchem-2.8.1.dev20240501163357/deepchem/metalearning/torch_maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/metrics/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/metrics/genomic_metrics.py` & `deepchem-2.8.1.dev20240501163357/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/metrics/metric.py` & `deepchem-2.8.1.dev20240501163357/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/metrics/score_function.py` & `deepchem-2.8.1.dev20240501163357/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/IRV.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/atomic_conv.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/callbacks.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/chemnet_layers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/chemnet_models.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/dft/dftxc.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/dft/hamilton/orbparams.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/dft/hamilton/orbparams.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/dft/nnxc.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/dft/scf.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/fcnet.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/gan.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/graph_models.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/jax_models/jax_model.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/jax_models/layers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/keras_model.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/keras_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,16 +391,16 @@
             the variables to train.  If None (the default), all trainable variables in
             the model are used.
         loss: function
             a function of the form f(outputs, labels, weights) that computes the loss
             for each batch.  If None (the default), the model's standard loss function
             is used.
         callbacks: function or list of functions
-            one or more functions of the form f(model, step) that will be invoked after
-            every step.  This can be used to perform validation, logging, etc.
+            one or more functions of the form f(model, step, **kwargs) that will be invoked
+            after every step.  This can be used to perform validation, logging, etc.
         all_losses: Optional[List[float]], optional (default None)
             If specified, all logged losses are appended into this list. Note that
             you can call `fit()` repeatedly with the same list and losses will
             continue to be appended.
 
         Returns
         -------
@@ -468,15 +468,21 @@
                 last_avg_loss = avg_loss
                 avg_loss = 0.0
                 averaged_batches = 0
 
             if checkpoint_interval > 0 and current_step % checkpoint_interval == checkpoint_interval - 1:
                 manager.save()
             for c in callbacks:
-                c(self, current_step)
+                try:
+                    # NOTE In DeepChem > 2.8.0, callback signature is updated to allow
+                    # variable arguments.
+                    c(self, current_step, iteration_loss=batch_loss)
+                except TypeError:
+                    # DeepChem <= 2.8.0, the callback should have this signature.
+                    c(self, current_step)
             if self.tensorboard and should_log:
                 self._log_scalar_to_tensorboard('loss', batch_loss,
                                                 current_step)
             if (self.wandb_logger is not None) and should_log:
                 all_data = dict({'train/loss': batch_loss})
                 self.wandb_logger.log_data(all_data, step=current_step)
```

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/layers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/losses.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/models.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/molgan.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/multitask.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/normalizing_flows.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/optimizers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/progressive_multitask.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/robust_multitask.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/scscore.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/seqtoseq.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/text_cnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from deepchem.models.torch_models.grover import GroverModel, GroverPretrain, GroverFinetune
 from deepchem.models.torch_models.readout import GroverReadout
 from deepchem.models.torch_models.dtnn import DTNN, DTNNModel
 from deepchem.models.torch_models.seqtoseq import SeqToSeq, SeqToSeqModel
 from deepchem.models.torch_models.acnn import AtomConvModel
 from deepchem.models.torch_models.progressive_multitask import ProgressiveMultitask, ProgressiveMultitaskModel
 from deepchem.models.torch_models.text_cnn import TextCNNModel
-from deepchem.models.torch_models.flows import Flow, Affine, MaskedAffineFlow, ActNorm
+from deepchem.models.torch_models.flows import Flow, Affine, MaskedAffineFlow, ActNorm, ClampExp, ConstScaleLayer, MLP_flow
 from deepchem.models.torch_models.unet import UNet, UNetModel
 try:
     from deepchem.models.torch_models.dmpnn import DMPNN, DMPNNModel
     from deepchem.models.torch_models.gnn import GNN, GNNHead, GNNModular
     from deepchem.models.torch_models.pna_gnn import AtomEncoder, BondEncoder, PNALayer, PNAGNN, PNA
     from deepchem.models.torch_models.gnn3d import Net3D, InfoMax3DModular
     from deepchem.models.torch_models.weavemodel_pytorch import Weave, WeaveModel
```

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/acnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/acnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/attention.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/chemberta.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/cnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/dtnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/dtnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/ferminet.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/flows.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/flows.py`

 * *Files 16% similar despite different names*

```diff
@@ -436,7 +436,193 @@
         if not self.data_dep_init_done:  # type: ignore
             assert self.scale is not None and self.shift is not None
             s_init = torch.log(z.std(dim=self.batch_dims, keepdim=True) + 1e-6)
             self.scale.data = s_init.data
             self.shift.data = z.mean(dim=self.batch_dims, keepdim=True).data
             self.data_dep_init_done = torch.tensor(1.0)
         return super().inverse(z)
+
+
+class ClampExp(nn.Module):
+    """
+    A non Linearity layer that clamps the input tensor by taking the minimum of the
+    exponential of the input multiplied by a lambda parameter and 1.
+
+    .. math:: f(x) = min(exp(\lambda * x), 1)
+
+    Example
+    -------
+    >>> import torch
+    >>> from deepchem.models.torch_models.flows import ClampExp
+    >>> lambda_param = 1.0
+    >>> clamp_exp = ClampExp(lambda_param)
+    >>> input = torch.tensor([-1 ,0.5, 0.6, 0.7])
+    >>> clamp_exp(input)
+    tensor([0.3679, 1.0000, 1.0000, 1.0000])
+    """
+
+    def __init__(self, lambda_param: float = 1.0) -> None:
+        """
+        Initializes the ClampExp layer
+
+        Parameters
+        ----------
+        lambda_param : float
+            Lambda parameter for the ClampExp layer
+        """
+
+        self.lambda_param = lambda_param
+        super(ClampExp, self).__init__()
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        Forward pass of the ClampExp layer
+
+        Parameters
+        ----------
+        x : torch.Tensor
+            Input tensor
+
+        Returns
+        -------
+        torch.Tensor
+            Transformed tensor according to ClampExp layer with the shape of 'x'.
+        """
+        one = torch.tensor(1.0, device=x.device, dtype=x.dtype)
+        return torch.min(torch.exp(self.lambda_param * x), one)
+
+
+class ConstScaleLayer(nn.Module):
+    """
+    This layer scales the input tensor by a fixed factor
+
+    Example
+    -------
+    >>> import torch
+    >>> from deepchem.models.torch_models.flows import ConstScaleLayer
+    >>> scale = 2.0
+    >>> const_scale = ConstScaleLayer(scale)
+    >>> input = torch.tensor([1, 2, 3])
+    >>> const_scale(input)
+    tensor([2., 4., 6.])
+    """
+
+    def __init__(self, scale: float = 1.0):
+        """
+        Initializes the ConstScaleLayer
+
+        Parameters
+        ----------
+        scale : float
+            Scaling factor
+        """
+        super().__init__()
+        self.scale = torch.tensor(scale)
+
+    def forward(self, input: torch.Tensor) -> torch.Tensor:
+        """Forward pass of the ConstScaleLayer
+
+        Parameters
+        ----------
+        input : torch.Tensor
+            Input tensor
+
+        Returns
+        -------
+        torch.Tensor
+            Scaled tensor
+        """
+        return input * self.scale
+
+
+class MLP_flow(nn.Module):
+    """
+    A Multi-Layer Perceptron (MLP) model for normalizing flows that is
+    used as a part of a Normalizing Flow model.
+    It is a modified version of the MLP model from `deepchem/deepchem/models/torch_models/layers.py`
+    to handle multiple layers
+
+    Example
+    -------
+    >>> import torch
+    >>> from deepchem.models.torch_models.flows import MLP_flow
+    >>> layers = [2, 4, 4, 2]
+    >>> mlp_flow = MLP_flow(layers)
+    >>> input = torch.tensor([1., 2.])
+    >>> output = mlp_flow(input)
+    >>> output.shape
+    torch.Size([2])
+    """
+
+    def __init__(
+        self,
+        layers: list,
+        leaky: float = 0.0,
+        score_scale: Optional[float] = None,
+        output_fn=None,
+        output_scale: Optional[float] = None,
+        init_zeros: bool = False,
+        dropout: Optional[float] = None,
+    ):
+        """
+        Initializes the MLP_flow model
+
+        Parameters
+        ----------
+        layers : list
+            List of layer sizes from start to end
+        leaky : float, optional default 0.0
+            Slope of the leaky part of the ReLU, if 0.0, standard ReLU is used
+        score_scale : float, optional
+            Factor to apply to the scores, i.e. output before output_fn
+        output_fn : str, optional
+            Function to be applied to the output, either None, "sigmoid", "relu", "tanh", or "clampexp"
+        output_scale : float, optional
+            Rescale outputs if output_fn is specified, i.e. scale * output_fn(out / scale)
+        init_zeros : bool, optional
+            Flag, if true, weights and biases of last layer are initialized with zeros
+            (helpful for deep models, see arXiv 1807.03039)
+        dropout : float, optional
+            If specified, dropout is done before last layer; if None, no dropout is done
+        """
+        super().__init__()
+        net = nn.ModuleList([])
+        for k in range(len(layers) - 2):
+            net.append(nn.Linear(layers[k], layers[k + 1]))
+            net.append(nn.LeakyReLU(leaky))
+        if dropout is not None:
+            net.append(nn.Dropout(p=dropout))
+        net.append(nn.Linear(layers[-2], layers[-1]))
+        if init_zeros:
+            nn.init.zeros_(net[-1].weight)
+            nn.init.zeros_(net[-1].bias)
+        if output_fn is not None:
+            if score_scale is not None:
+                net.append(ConstScaleLayer(score_scale))
+            if output_fn == "sigmoid":
+                net.append(nn.Sigmoid())
+            elif output_fn == "relu":
+                net.append(nn.ReLU())
+            elif output_fn == "tanh":
+                net.append(nn.Tanh())
+            elif output_fn == "clampexp":
+                net.append(ClampExp())
+            else:
+                NotImplementedError("This output function is not implemented.")
+            if output_scale is not None:
+                net.append(ConstScaleLayer(output_scale))
+        self.net = nn.Sequential(*net)
+
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        """Forward pass of the MLP_flow model
+
+        Parameters
+        ----------
+        x : torch.Tensor
+            Input tensor
+
+        Returns
+        -------
+        torch.Tensor
+            Transformed tensor according to the MLP_flow model with the shape of 'x'
+        """
+        return self.net(x)
```

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gan.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gat.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gcn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/grover.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/hf_models.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/hf_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,16 +273,16 @@
             the variables to train.  If None (the default), all trainable variables in
             the model are used.
         loss: function
             a function of the form f(outputs, labels, weights) that computes the loss
             for each batch.  If None (the default), the model's standard loss function
             is used.
         callbacks: function or list of functions
-            one or more functions of the form f(model, step) that will be invoked after
-            every step.  This can be used to perform validation, logging, etc.
+            one or more functions of the form f(model, step, **kwargs) that will be invoked
+            after every step.  This can be used to perform validation, logging, etc.
         all_losses: Optional[List[float]], optional (default None)
             If specified, all logged losses are appended into this list. Note that
             you can call `fit()` repeatedly with the same list and losses will
             continue to be appended.
 
         Returns
         -------
@@ -354,15 +354,21 @@
                 last_avg_loss = avg_loss
                 avg_loss = 0.0
                 averaged_batches = 0
 
             if checkpoint_interval > 0 and current_step % checkpoint_interval == checkpoint_interval - 1:
                 self.save_checkpoint(max_checkpoints_to_keep)
             for c in callbacks:
-                c(self, current_step)
+                try:
+                    # NOTE In DeepChem > 2.8.0, callback signature is updated to allow
+                    # variable arguments.
+                    c(self, current_step, iteration_loss=batch_loss)
+                except TypeError:
+                    # DeepChem <= 2.8.0, the callback should have this signature.
+                    c(self, current_step)
             if self.tensorboard and should_log:
                 self._log_scalar_to_tensorboard('loss', batch_loss,
                                                 current_step)
             if (self.wandb_logger is not None) and should_log:
                 all_data = dict({'train/loss': batch_loss})
                 self.wandb_logger.log_data(all_data, step=current_step)
```

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/infograph.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/layers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/lcnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/mat.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/megnet.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/modular.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/modular.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,16 @@
             the variables to train.  If None (the default), all trainable variables in
             the model are used.
         loss: function
             a function of the form f(outputs, labels, weights) that computes the loss
             for each batch.  If None (the default), the model's standard loss function
             is used.
         callbacks: function or list of functions
-            one or more functions of the form f(model, step) that will be invoked after
-            every step.  This can be used to perform validation, logging, etc.
+            one or more functions of the form f(model, step, **kwargs) that will be invoked
+            after every step.  This can be used to perform validation, logging, etc.
         all_losses: Optional[List[float]], optional (default None)
             If specified, all logged losses are appended into this list. Note that
             you can call `fit()` repeatedly with the same list and losses will
             continue to be appended.
 
         Returns
         -------
@@ -248,15 +248,21 @@
                 # Capture the last avg_loss in case of return since we're resetting to 0 now
                 last_avg_loss = avg_loss
                 avg_loss = 0.0
                 averaged_batches = 0
             if checkpoint_interval > 0 and current_step % checkpoint_interval == checkpoint_interval - 1:
                 self.save_checkpoint(max_checkpoints_to_keep)
             for c in callbacks:
-                c(self, current_step)
+                try:
+                    # NOTE In DeepChem > 2.8.0, callback signature is updated to allow
+                    # variable arguments.
+                    c(self, current_step, iteration_loss=batch_loss)
+                except TypeError:
+                    # DeepChem <= 2.8.0, the callback should have this signature.
+                    c(self, current_step)
             if self.tensorboard and should_log:
                 self._log_scalar_to_tensorboard('loss', batch_loss,
                                                 current_step)
             if (self.wandb_logger is not None) and should_log:
                 all_data = dict({'train/loss': batch_loss})
                 self.wandb_logger.log_data(all_data, step=current_step)
```

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/molgan.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/mpnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/pagtn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/progressive_multitask.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/readout.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/scscore.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/seqtoseq.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/text_cnn.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/torch_model.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/torch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
             the variables to train.  If None (the default), all trainable variables in
             the model are used.
         loss: function
             a function of the form f(outputs, labels, weights) that computes the loss
             for each batch.  If None (the default), the model's standard loss function
             is used.
         callbacks: function or list of functions
-            one or more functions of the form f(model, step) that will be invoked after
+            one or more functions of the form f(model, step, **kwargs) that will be invoked after
             every step.  This can be used to perform validation, logging, etc.
         all_losses: Optional[List[float]], optional (default None)
             If specified, all logged losses are appended into this list. Note that
             you can call `fit()` repeatedly with the same list and losses will
             continue to be appended.
 
         Returns
@@ -461,15 +461,21 @@
                 last_avg_loss = avg_loss
                 avg_loss = 0.0
                 averaged_batches = 0
 
             if checkpoint_interval > 0 and current_step % checkpoint_interval == checkpoint_interval - 1:
                 self.save_checkpoint(max_checkpoints_to_keep)
             for c in callbacks:
-                c(self, current_step)
+                try:
+                    # NOTE In DeepChem > 2.8.0, callback signature is updated to allow
+                    # variable arguments.
+                    c(self, current_step, iteration_loss=batch_loss)
+                except TypeError:
+                    # DeepChem <= 2.8.0, the callback should have this signature.
+                    c(self, current_step)
             if self.tensorboard and should_log:
                 self._log_scalar_to_tensorboard('loss', batch_loss,
                                                 current_step)
             if (self.wandb_logger is not None) and should_log:
                 all_data = dict({'train/loss': batch_loss})
                 self.wandb_logger.log_data(all_data, step=current_step)
```

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/unet.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/unet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/torch_models/weavemodel_pytorch.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/torch_models/weavemodel_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/trainer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/trainer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/models/wandblogger.py` & `deepchem-2.8.1.dev20240501163357/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/check_availability.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/defaults.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/dnasim.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/run_benchmark.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.8.1.dev20240501163357/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/rl/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/rl/a2c.py` & `deepchem-2.8.1.dev20240501163357/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.8.1.dev20240501163357/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/rl/envs/tictactoe.py` & `deepchem-2.8.1.dev20240501163357/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/rl/ppo.py` & `deepchem-2.8.1.dev20240501163357/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/rl/torch_rl/torch_a2c.py` & `deepchem-2.8.1.dev20240501163357/deepchem/rl/torch_rl/torch_a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/rl/torch_rl/torch_ppo.py` & `deepchem-2.8.1.dev20240501163357/deepchem/rl/torch_rl/torch_ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/splits/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/splits/splitters.py` & `deepchem-2.8.1.dev20240501163357/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/splits/task_splitter.py` & `deepchem-2.8.1.dev20240501163357/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/trans/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/trans/duplicate.py` & `deepchem-2.8.1.dev20240501163357/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/trans/transformers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/attribute_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/attribute_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/batch_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/conformers.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/data_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/debug_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/api/getxc.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/api/getxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/api/parser.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/api/parser.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/config.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/config.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/data/datastruct.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/data/datastruct.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/df/base_df.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/df/base_df.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/grid/base_grid.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/grid/base_grid.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/grid/radial_grid.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/grid/radial_grid.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/base_hamilton.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/base_hamilton.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/intor/lattice.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/intor/lattice.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/hamilton/orbparams.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/hamilton/orbparams.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/qccalc/base_qccalc.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/qccalc/base_qccalc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/qccalc/hf.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/qccalc/hf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/qccalc/scf_qccalc.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/qccalc/scf_qccalc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/system/base_system.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/system/base_system.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/xc/base_xc.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/xc/base_xc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/xc/libxc.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/xc/libxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dft_utils/xc/libxc_wrapper.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dft_utils/xc/libxc_wrapper.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/dftutils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/__init__.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/bcast.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/bcast.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/editable_module.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/editable_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/grad.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/grad.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/linop.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/linop.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/misc.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/misc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/equilibrium.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/equilibrium.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/jacobian.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/jacobian.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/minimizer.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/minimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/rootfinder.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/rootfinder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/optimize/rootsolver.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/optimize/rootsolver.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/pure_function.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/pure_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/solve.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/solve.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/differentiation_utils/symeig.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/differentiation_utils/symeig.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/docking_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/electron_sampler.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/equivariance_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/equivariance_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/evaluate.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/fake_data_generator.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/fragment_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/genomics_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/geometry_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/graph_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/grover.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/hash_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/misc_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/noncovalent_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/pdbqt_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/periodic_table_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/periodic_table_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/pytorch_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/rdkit_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/safeops_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/safeops_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/save.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/sequence_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_attribute_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_attribute_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_batch_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_batch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_data_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_dft_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_dft_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_dftutils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_differentiation_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_differentiation_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_equivariance_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_equivariance_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_evaluate.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_grover.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_periodic_table_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_periodic_table_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_pytorch_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_safe_ops_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_safe_ops_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/typing.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/vina_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem/utils/voxel_utils.py` & `deepchem-2.8.1.dev20240501163357/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem.egg-info/PKG-INFO` & `deepchem-2.8.1.dev20240501163357/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.8.1.dev20240424201325
+Version: 2.8.1.dev20240501163357
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.8.1.dev20240424201325/deepchem.egg-info/SOURCES.txt` & `deepchem-2.8.1.dev20240501163357/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/setup.cfg` & `deepchem-2.8.1.dev20240501163357/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.8.1.dev20240424201325/setup.py` & `deepchem-2.8.1.dev20240501163357/setup.py`

 * *Files identical despite different names*


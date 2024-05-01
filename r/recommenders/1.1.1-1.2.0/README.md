# Comparing `tmp/recommenders-1.1.1.tar.gz` & `tmp/recommenders-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recommenders-1.1.1.tar", last modified: Wed Jul 20 05:25:55 2022, max compression
+gzip compressed data, was "recommenders-1.2.0.tar", last modified: Wed May  1 11:35:42 2024, max compression
```

## Comparing `recommenders-1.1.1.tar` & `recommenders-1.2.0.tar`

### file list

```diff
@@ -1,256 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.261056 recommenders-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     6144 2022-07-20 05:25:49.000000 recommenders-1.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-07-20 05:25:49.000000 recommenders-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-20 05:25:49.000000 recommenders-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12371 2022-07-20 05:25:55.261056 recommenders-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    26287 2022-07-20 05:25:49.000000 recommenders-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-20 05:25:49.000000 recommenders-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.201051 recommenders-1.1.1/recommenders/
--rw-r--r--   0 runner    (1001) docker     (121)     9353 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17699 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/amazon_reviews.py
--rw-r--r--   0 runner    (1001) docker     (121)     2591 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/cosmos_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/covid_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6125 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/criteo.py
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    15300 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/mind.py
--rw-r--r--   0 runner    (1001) docker     (121)    25389 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/movielens.py
--rw-r--r--   0 runner    (1001) docker     (121)    17415 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/pandas_df_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10271 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/python_splitters.py
--rw-r--r--   0 runner    (1001) docker     (121)    10125 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/spark_splitters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7142 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     7060 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/split_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6979 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/datasets/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    55764 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/evaluation/python_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)    37456 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/evaluation/spark_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/models/cornac/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/cornac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/cornac/cornac_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/models/deeprec/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/models/deeprec/DataModel/
--rw-r--r--   0 runner    (1001) docker     (121)     7713 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/DataModel/ImplicitCF.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/DataModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17496 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/deeprec_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/models/deeprec/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4835 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/io/dkn_item2item_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)    15611 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/io/dkn_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8838 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/io/iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12102 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/io/nextitnet_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)    19373 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/io/sequential_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/models/deeprec/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28259 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    20302 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/dkn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/dkn_item2item.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.209052 recommenders-1.1.1/recommenders/models/deeprec/models/graphrec/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/graphrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15626 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/graphrec/lightgcn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.213052 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/asvd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4100 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/caser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/gru4rec.py
--rw-r--r--   0 runner    (1001) docker     (121)     8153 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/nextitnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    25194 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/rnn_cell_implement.py
--rw-r--r--   0 runner    (1001) docker     (121)    13250 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/sequential_base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5543 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/sli_rec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/sum.py
--rw-r--r--   0 runner    (1001) docker     (121)    13157 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/sequential/sum_cells.py
--rw-r--r--   0 runner    (1001) docker     (121)    22126 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/deeprec/models/xDeepFM.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.213052 recommenders-1.1.1/recommenders/models/fastai/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/fastai/fastai_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.217053 recommenders-1.1.1/recommenders/models/geoimc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/geoimc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/geoimc/geoimc_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     8650 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/geoimc/geoimc_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/geoimc/geoimc_predict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/geoimc/geoimc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.217053 recommenders-1.1.1/recommenders/models/lightfm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/lightfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9414 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/lightfm/lightfm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.217053 recommenders-1.1.1/recommenders/models/lightgbm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8188 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/lightgbm/lightgbm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.217053 recommenders-1.1.1/recommenders/models/ncf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/ncf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22412 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/ncf/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    16083 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/ncf/ncf_singlenode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.221053 recommenders-1.1.1/recommenders/models/newsrec/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.221053 recommenders-1.1.1/recommenders/models/newsrec/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23911 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/io/mind_all_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)    15793 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/io/mind_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.221053 recommenders-1.1.1/recommenders/models/newsrec/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14186 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    10522 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7902 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/models/lstur.py
--rw-r--r--   0 runner    (1001) docker     (121)    14156 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/models/naml.py
--rw-r--r--   0 runner    (1001) docker     (121)     7789 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/models/npa.py
--rw-r--r--   0 runner    (1001) docker     (121)     6738 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/models/nrms.py
--rw-r--r--   0 runner    (1001) docker     (121)     8715 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/newsrec/newsrec_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.225053 recommenders-1.1.1/recommenders/models/rbm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/rbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27615 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/rbm/rbm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.225053 recommenders-1.1.1/recommenders/models/rlrmc/
--rw-r--r--   0 runner    (1001) docker     (121)    11351 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/rlrmc/RLRMCalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5809 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/rlrmc/RLRMCdataset.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/rlrmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9912 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/rlrmc/conjugate_gradient_ms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.225053 recommenders-1.1.1/recommenders/models/sar/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/sar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22607 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/sar/sar_singlenode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.225053 recommenders-1.1.1/recommenders/models/sasrec/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/sasrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28071 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/sasrec/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/sasrec/sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)    10145 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/sasrec/ssept.py
--rw-r--r--   0 runner    (1001) docker     (121)     3800 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/sasrec/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.225053 recommenders-1.1.1/recommenders/models/surprise/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/surprise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3960 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/surprise/surprise_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.229054 recommenders-1.1.1/recommenders/models/tfidf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/tfidf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14957 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/tfidf/tfidf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.229054 recommenders-1.1.1/recommenders/models/vae/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/vae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18660 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/vae/multinomial_vae.py
--rw-r--r--   0 runner    (1001) docker     (121)    17523 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/vae/standard_vae.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.229054 recommenders-1.1.1/recommenders/models/vowpal_wabbit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/vowpal_wabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8375 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/vowpal_wabbit/vw.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.229054 recommenders-1.1.1/recommenders/models/wide_deep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/wide_deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7641 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/models/wide_deep/wide_deep_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.229054 recommenders-1.1.1/recommenders/tuning/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.233054 recommenders-1.1.1/recommenders/tuning/nni/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/tuning/nni/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6099 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/tuning/nni/ncf_training.py
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/tuning/nni/ncf_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5095 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/tuning/nni/nni_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6736 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/tuning/nni/svd_training.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/tuning/parameter_sweep.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.237054 recommenders-1.1.1/recommenders/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/gpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3060 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/notebook_memory_management.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     8238 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11815 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-07-20 05:25:49.000000 recommenders-1.1.1/recommenders/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.205052 recommenders-1.1.1/recommenders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12371 2022-07-20 05:25:55.000000 recommenders-1.1.1/recommenders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8833 2022-07-20 05:25:55.000000 recommenders-1.1.1/recommenders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 05:25:55.000000 recommenders-1.1.1/recommenders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-07-20 05:25:55.000000 recommenders-1.1.1/recommenders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-07-20 05:25:55.000000 recommenders-1.1.1/recommenders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-20 05:25:55.261056 recommenders-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-07-20 05:25:49.000000 recommenders-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.201051 recommenders-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.237054 recommenders-1.1.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.237054 recommenders-1.1.1/tests/integration/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19106 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/examples/test_notebooks_gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/examples/test_notebooks_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (121)     8732 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/examples/test_notebooks_python.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.237054 recommenders-1.1.1/tests/integration/recommenders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/recommenders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.241055 recommenders-1.1.1/tests/integration/recommenders/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/recommenders/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/recommenders/datasets/test_criteo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/recommenders/datasets/test_mind.py
--rw-r--r--   0 runner    (1001) docker     (121)     8291 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/integration/recommenders/datasets/test_movielens.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.241055 recommenders-1.1.1/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.241055 recommenders-1.1.1/tests/smoke/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8843 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/examples/test_notebooks_gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/examples/test_notebooks_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (121)     6359 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/examples/test_notebooks_python.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.241055 recommenders-1.1.1/tests/smoke/recommenders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.241055 recommenders-1.1.1/tests/smoke/recommenders/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/dataset/test_criteo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4240 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/dataset/test_mind.py
--rw-r--r--   0 runner    (1001) docker     (121)     6950 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/dataset/test_movielens.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.245055 recommenders-1.1.1/tests/smoke/recommenders/recommender/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/recommender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10065 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/recommender/test_deeprec_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/recommender/test_deeprec_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8984 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/recommender/test_newsrec_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5180 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/smoke/recommenders/recommender/test_newsrec_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.245055 recommenders-1.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.245055 recommenders-1.1.1/tests/unit/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/examples/test_notebooks_gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)     4139 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/examples/test_notebooks_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/examples/test_notebooks_python.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.245055 recommenders-1.1.1/tests/unit/recommenders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.249055 recommenders-1.1.1/tests/unit/recommenders/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/test_covid_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5081 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/test_movielens.py
--rw-r--r--   0 runner    (1001) docker     (121)     9707 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/test_pandas_df_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    15667 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/test_python_splitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7513 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/test_spark_splitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4017 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/datasets/test_wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.249055 recommenders-1.1.1/tests/unit/recommenders/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23921 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/evaluation/test_python_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6504 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/evaluation/test_python_evaluation_time_performance.py
--rw-r--r--   0 runner    (1001) docker     (121)    20963 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/evaluation/test_spark_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.253056 recommenders-1.1.1/tests/unit/recommenders/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_cornac_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9968 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_deeprec_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_deeprec_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4502 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_geoimc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_lightfm_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7948 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_ncf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5789 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_ncf_singlenode.py
--rw-r--r--   0 runner    (1001) docker     (121)     5171 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_newsrec_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_newsrec_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7238 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_rbm.py
--rw-r--r--   0 runner    (1001) docker     (121)    14889 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_sar_singlenode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6950 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_sasrec_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4323 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_surprise_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3765 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_tfidf_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2999 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_vowpal_wabbit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4088 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/models/test_wide_deep_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.257056 recommenders-1.1.1/tests/unit/recommenders/tuning/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/tuning/test_ncf_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7437 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/tuning/test_nni_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/tuning/test_sweep.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:55.261056 recommenders-1.1.1/tests/unit/recommenders/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/test_general_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/test_gpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/test_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/test_notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/test_python_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7355 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/test_tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-07-20 05:25:49.000000 recommenders-1.1.1/tests/unit/recommenders/utils/test_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.780128 recommenders-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-01 11:35:37.000000 recommenders-1.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-01 11:35:37.000000 recommenders-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 11:35:37.000000 recommenders-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-01 11:35:42.780128 recommenders-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21088 2024-05-01 11:35:37.000000 recommenders-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-01 11:35:37.000000 recommenders-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.748128 recommenders-1.2.0/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.752128 recommenders-1.2.0/recommenders/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17682 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/amazon_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/cosmos_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/covid_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/criteo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25508 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/movielens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/pandas_df_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/python_splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/spark_splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/datasets/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.752128 recommenders-1.2.0/recommenders/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61915 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/evaluation/python_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37328 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/evaluation/spark_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.752128 recommenders-1.2.0/recommenders/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.752128 recommenders-1.2.0/recommenders/models/cornac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/cornac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/cornac/cornac_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.752128 recommenders-1.2.0/recommenders/models/deeprec/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.752128 recommenders-1.2.0/recommenders/models/deeprec/DataModel/
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/DataModel/ImplicitCF.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/DataModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17458 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/deeprec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.752128 recommenders-1.2.0/recommenders/models/deeprec/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/io/dkn_item2item_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15594 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/io/dkn_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/io/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/io/nextitnet_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19356 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/io/sequential_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.752128 recommenders-1.2.0/recommenders/models/deeprec/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28242 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20285 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/dkn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/dkn_item2item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.756128 recommenders-1.2.0/recommenders/models/deeprec/models/graphrec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/graphrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/graphrec/lightgcn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.756128 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/asvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/caser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/nextitnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25947 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/rnn_cell_implement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/sequential_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/sli_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/sequential/sum_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22109 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/deeprec/models/xDeepFM.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.756128 recommenders-1.2.0/recommenders/models/fastai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/fastai/fastai_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.756128 recommenders-1.2.0/recommenders/models/geoimc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/geoimc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/geoimc/geoimc_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/geoimc/geoimc_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/geoimc/geoimc_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/geoimc/geoimc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.756128 recommenders-1.2.0/recommenders/models/lightfm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/lightfm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/lightfm/lightfm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.756128 recommenders-1.2.0/recommenders/models/lightgbm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/lightgbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/lightgbm/lightgbm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.756128 recommenders-1.2.0/recommenders/models/ncf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/ncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22528 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/ncf/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16066 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/ncf/ncf_singlenode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.760128 recommenders-1.2.0/recommenders/models/newsrec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.760128 recommenders-1.2.0/recommenders/models/newsrec/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23895 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/io/mind_all_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/io/mind_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.760128 recommenders-1.2.0/recommenders/models/newsrec/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/models/lstur.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/models/naml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/models/npa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/models/nrms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/newsrec/newsrec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.760128 recommenders-1.2.0/recommenders/models/rbm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/rbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27627 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/rbm/rbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.760128 recommenders-1.2.0/recommenders/models/rlrmc/
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/rlrmc/RLRMCalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/rlrmc/RLRMCdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/rlrmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/rlrmc/conjugate_gradient_ms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.760128 recommenders-1.2.0/recommenders/models/sar/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/sar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22622 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/sar/sar_singlenode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.760128 recommenders-1.2.0/recommenders/models/sasrec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/sasrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28049 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/sasrec/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/sasrec/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/sasrec/ssept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/sasrec/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.764128 recommenders-1.2.0/recommenders/models/surprise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/surprise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/surprise/surprise_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.764128 recommenders-1.2.0/recommenders/models/tfidf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/tfidf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14944 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/tfidf/tfidf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.764128 recommenders-1.2.0/recommenders/models/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/vae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/vae/multinomial_vae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/vae/standard_vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.764128 recommenders-1.2.0/recommenders/models/vowpal_wabbit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/vowpal_wabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/vowpal_wabbit/vw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.764128 recommenders-1.2.0/recommenders/models/wide_deep/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/wide_deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/models/wide_deep/wide_deep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.764128 recommenders-1.2.0/recommenders/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.764128 recommenders-1.2.0/recommenders/tuning/nni/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/tuning/nni/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/tuning/nni/ncf_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/tuning/nni/ncf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/tuning/nni/nni_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/tuning/nni/svd_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/tuning/parameter_sweep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/recommenders/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/gpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/notebook_memory_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-01 11:35:37.000000 recommenders-1.2.0/recommenders/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.748128 recommenders-1.2.0/recommenders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-01 11:35:42.000000 recommenders-1.2.0/recommenders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-01 11:35:42.000000 recommenders-1.2.0/recommenders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:35:42.000000 recommenders-1.2.0/recommenders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-01 11:35:42.000000 recommenders-1.2.0/recommenders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 11:35:42.000000 recommenders-1.2.0/recommenders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:35:42.780128 recommenders-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-01 11:35:37.000000 recommenders-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.744128 recommenders-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/ci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/tests/ci/azureml_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/ci/azureml_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/ci/azureml_tests/run_groupwise_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18194 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/ci/azureml_tests/submit_groupwise_azureml_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36977 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/ci/azureml_tests/test_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/tests/data_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/tests/data_validation/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/examples/test_mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/examples/test_wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/tests/data_validation/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/recommenders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/tests/data_validation/recommenders/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/recommenders/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/recommenders/datasets/test_covid_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/recommenders/datasets/test_criteo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/recommenders/datasets/test_mind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13630 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/recommenders/datasets/test_movielens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/data_validation/recommenders/datasets/test_wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.768128 recommenders-1.2.0/tests/functional/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/functional/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17379 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/functional/examples/test_notebooks_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/functional/examples/test_notebooks_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/functional/examples/test_notebooks_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/integration/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/integration/recommenders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/integration/recommenders/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/integration/recommenders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/integration/recommenders/utils/test_k8s_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/performance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/performance/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/performance/recommenders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/performance/recommenders/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/performance/recommenders/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/performance/recommenders/evaluation/test_python_evaluation_time_performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/regression/test_compatibility_tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/responsible_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/responsible_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/responsible_ai/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/responsible_ai/recommenders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/responsible_ai/recommenders/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/responsible_ai/recommenders/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/responsible_ai/recommenders/datasets/test_criteo_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/responsible_ai/recommenders/datasets/test_movielens_privacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/security/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/security/test_dependency_security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/smoke/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/examples/test_notebooks_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/examples/test_notebooks_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/examples/test_notebooks_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.772128 recommenders-1.2.0/tests/smoke/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/recommenders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.776128 recommenders-1.2.0/tests/smoke/recommenders/recommender/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/recommenders/recommender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/recommenders/recommender/test_deeprec_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/recommenders/recommender/test_deeprec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/recommenders/recommender/test_newsrec_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/smoke/recommenders/recommender/test_newsrec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.776128 recommenders-1.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.776128 recommenders-1.2.0/tests/unit/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/examples/test_notebooks_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/examples/test_notebooks_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/examples/test_notebooks_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.776128 recommenders-1.2.0/tests/unit/recommenders/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.776128 recommenders-1.2.0/tests/unit/recommenders/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/datasets/test_download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/datasets/test_pandas_df_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15649 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/datasets/test_python_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/datasets/test_spark_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/datasets/test_sparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.776128 recommenders-1.2.0/tests/unit/recommenders/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/evaluation/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/evaluation/test_python_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/evaluation/test_spark_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.780128 recommenders-1.2.0/tests/unit/recommenders/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_cornac_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_deeprec_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_deeprec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_geoimc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_lightfm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_ncf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_ncf_singlenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_newsrec_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_newsrec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_rbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_sar_singlenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_sasrec_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_surprise_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_tfidf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_vowpal_wabbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/models/test_wide_deep_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.780128 recommenders-1.2.0/tests/unit/recommenders/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/tuning/test_ncf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/tuning/test_nni_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/tuning/test_sweep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:42.780128 recommenders-1.2.0/tests/unit/recommenders/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/utils/test_general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/utils/test_gpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/utils/test_notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/utils/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/utils/test_python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/utils/test_tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-01 11:35:37.000000 recommenders-1.2.0/tests/unit/recommenders/utils/test_timer.py
```

### Comparing `recommenders-1.1.1/AUTHORS.md` & `recommenders-1.2.0/AUTHORS.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+<!--
+Copyright (c) Recommenders contributors.
+Licensed under the MIT License.
+-->
+
 Contributors to Recommenders 
 ============================
 Recommenders is developed and maintained by a community of people interested in exploring recommendation algorithms and how best to deploy them in industry settings. The goal is to accelerate the workflow of any individual or organization working on recommender systems. Everyone is encouraged to contribute at any level to add and improve the implemented algorithms, notebooks and utilities.
 
 <p align="center">
-  <img src="https://contributors-img.web.app/image?repo=microsoft/recommenders" width = 500/>
+  <img src="https://contributors-img.web.app/image?repo=recommenders-team/recommenders" width = 500/>
 </p>
 
 Maintainers (sorted alphabetically)
 ---------------------------------------
 Maintainers are actively supporting the project and have made substantial contributions to the repository.<br>
 They have admin access to the repo and provide support reviewing issues and pull requests.
 
@@ -28,14 +33,16 @@
    * Recommendation algorithms review, development and optimization.
    * Reco utils review, development and optimization.
    * Github statistics.
    * Continuous integration build / test setup.
 * **[Scott Graham](https://github.com/gramhagen)**
    * Improving documentation
    * VW notebook
+* **[Simon Zhao](https://github.com/simonyansenzhao)**
+   * SARplus algorithm upgrade
 * **[Tao Wu](https://github.com/wutaomsft)**
    * Improving documentation
 
 
 Contributors  (sorted alphabetically)
 -------------------------------------
 [Full List of Contributors](https://github.com/Microsoft/Recommenders/graphs/contributors)
@@ -116,16 +123,14 @@
 * **[Quoc-Tuan Truong](https://github.com/tqtg)**
    * BPR notebook using [Cornac](https://github.com/PreferredAI/cornac) framework
    * BiVAE notebook using [Cornac](https://github.com/PreferredAI/cornac) framework
 * **[Robert Alexander](https://github.com/roalexan)**
    * Windows test pipelines
 * **[Satyadev Ntv](https://github.com/satyadevntv)**
    * GeoIMC algorithm
-* **[Simon Zhao](https://github.com/simonzhaoms)**
-   * SARplus algorithm upgrade
 * **[Yan Zhang](https://github.com/YanZhangADS)**
    * Diversity metrics including coverage, novelty, diversity, and serendipity
    * Diversity metrics evaluation sample notebook
 * **[Yassine Khelifi](https://github.com/datashinobi)**
    * SAR notebook quickstart
 * **[Zhenhui Xu](https://github.com/motefly)**
    * Reco utils of LightGBM
```

### Comparing `recommenders-1.1.1/LICENSE` & `recommenders-1.2.0/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
     MIT License
 
-    Copyright (c) Microsoft Corporation. All rights reserved.
+    Copyright (c) 2018-present Microsoft Corporation.
+    Copyright (c) 2023-present Recommenders contributors.
 
     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to deal
     in the Software without restriction, including without limitation the rights
     to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:
```

### Comparing `recommenders-1.1.1/PKG-INFO` & `recommenders-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: recommenders
-Version: 1.1.1
-Summary: Microsoft Recommenders - Python utilities for building recommender systems
-Home-page: https://github.com/microsoft/recommenders
-Author: RecoDev Team at Microsoft
-Author-email: RecoDevTeam@service.microsoft.com
+Version: 1.2.0
+Summary: Recommenders - Python utilities for building recommendation systems
+Home-page: https://github.com/recommenders-team/recommenders
+Author: Recommenders contributors
+Author-email: recommenders-technical-discuss@lists.lfaidata.foundation
 License: UNKNOWN
-Project-URL: Documentation, https://microsoft-recommenders.readthedocs.io/en/stable/
-Project-URL: Wiki, https://github.com/microsoft/recommenders/wiki
-Description: # Recommender Utilities
+Project-URL: Documentation, https://recommenders-team.github.io/recommenders/intro.html
+Project-URL: Wiki, https://github.com/recommenders-team/recommenders/wiki
+Description: <!--
+        Copyright (c) Recommenders contributors.
+        Licensed under the MIT License.
+        -->
+        
+        # Recommender Utilities
         
         This package contains functions to simplify common tasks used when developing and evaluating recommender systems. A short description of the submodules is provided below. For more details about what functions are available and how to use them, please review the doc-strings provided with the code or the [online documentation](https://readthedocs.org/projects/microsoft-recommenders/).
         
         # Installation
         
         ## Pre-requisites
         Some dependencies require compilation during pip installation. On Linux this can be supported by adding build-essential dependencies:
         ```bash
         sudo apt-get install -y build-essential libpython<version>
         ``` 
-        where `<version>` should be the Python version (e.g. `3.6`).
+        where `<version>` should be the Python version (e.g. `3.8`).
         
         On Windows you will need [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)
         
         For more details about the software requirements that must be pre-installed on each supported platform, see the [setup guide](https://github.com/microsoft/recommenders/blob/main/SETUP.md).   
         
         ## Basic installation
         
@@ -149,15 +154,15 @@
         The models submodule contains implementations of various algorithms that can be used in addition to external packages to evaluate and develop new recommender system approaches. A description of all the algorithms can be found on [this table](../README.md#algorithms). The following is a list of the algorithm utilities:
         
         * Cornac
         * DeepRec
           *  Convolutional Sequence Embedding Recommendation (CASER)
           *  Deep Knowledge-Aware Network (DKN)
           *  Extreme Deep Factorization Machine (xDeepFM)
-          *  GRU4Rec
+          *  GRU
           *  LightGCN
           *  Next Item Recommendation (NextItNet)
           *  Short-term and Long-term Preference Integrated Recommender (SLi-Rec)
           *  Multi-Interest-Aware Sequential User Modeling (SUM)
         * FastAI
         * GeoIMC
         * LightFM
@@ -197,23 +202,19 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.6, <3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: examples
 Provides-Extra: gpu
 Provides-Extra: spark
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: experimental
-Provides-Extra: nni
```

### Comparing `recommenders-1.1.1/README.md` & `recommenders-1.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,121 +1,99 @@
-# Recommenders
+<!--
+Copyright (c) Recommenders contributors.
+Licensed under the MIT License.
+-->
 
-[![Documentation Status](https://readthedocs.org/projects/microsoft-recommenders/badge/?version=latest)](https://microsoft-recommenders.readthedocs.io/en/latest/?badge=latest)
+# Recommenders
 
-## What's New (July, 2022)
+[![Documentation status](https://github.com/recommenders-team/recommenders/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/recommenders-team/recommenders/actions/workflows/pages/pages-build-deployment)
 
-We have a new release [Recommenders 1.1.1](https://github.com/microsoft/recommenders/releases/tag/1.1.1)! 
+<img src="https://raw.githubusercontent.com/recommenders-team/artwork/main/color/recommenders_color.svg" width="800">
 
-We have introduced a new way of testing our repository using [AzureML](https://azure.microsoft.com/en-us/services/machine-learning/). With AzureML we are able to distribute our tests to different machines and run them in parallel. This allows us to test our repository on a wider range of machines and provides us with a much faster test cycle. Our total computation time went from around 9h to 35min, and we were able to reduce the costs by half. See more details [here](tests/README.md).
+## What's New (May, 2024)
 
-We also made other improvements like faster evaluation metrics and improving SAR algorithm. 
+We have a new release [Recommenders 1.2.0](https://github.com/microsoft/recommenders/releases/tag/1.2.0)!
 
-Starting with release 0.6.0, Recommenders has been available on PyPI and can be installed using pip! 
+So many changes since our last release. We have full tests on Python 3.8 to 3.11 (around 1800 tests), upgraded performance in many algorithms, reviewed notebooks, and many more improvements.
 
-Here you can find the PyPi page: https://pypi.org/project/recommenders/
+## Introduction
 
-Here you can find the package documentation: https://microsoft-recommenders.readthedocs.io/en/latest/
+Recommenders objective is to assist researchers, developers and enthusiasts in prototyping, experimenting with and bringing to production a range of classic and state-of-the-art recommendation systems.
 
-## Introduction
+Recommenders is a project under the [Linux Foundation of AI and Data](https://lfaidata.foundation/projects/). 
 
 This repository contains examples and best practices for building recommendation systems, provided as Jupyter notebooks. The examples detail our learnings on five key tasks:
 
-- [Prepare Data](examples/01_prepare_data): Preparing and loading data for each recommender algorithm
-- [Model](examples/00_quick_start): Building models using various classical and deep learning recommender algorithms such as Alternating Least Squares ([ALS](https://spark.apache.org/docs/latest/api/python/_modules/pyspark/ml/recommendation.html#ALS)) or eXtreme Deep Factorization Machines ([xDeepFM](https://arxiv.org/abs/1803.05170)).
-- [Evaluate](examples/03_evaluate): Evaluating algorithms with offline metrics
-- [Model Select and Optimize](examples/04_model_select_and_optimize): Tuning and optimizing hyperparameters for recommender models
-- [Operationalize](examples/05_operationalize): Operationalizing models in a production environment on Azure
+- [Prepare Data](examples/01_prepare_data): Preparing and loading data for each recommendation algorithm.
+- [Model](examples/00_quick_start): Building models using various classical and deep learning recommendation algorithms such as Alternating Least Squares ([ALS](https://spark.apache.org/docs/latest/api/python/_modules/pyspark/ml/recommendation.html#ALS)) or eXtreme Deep Factorization Machines ([xDeepFM](https://arxiv.org/abs/1803.05170)).
+- [Evaluate](examples/03_evaluate): Evaluating algorithms with offline metrics.
+- [Model Select and Optimize](examples/04_model_select_and_optimize): Tuning and optimizing hyperparameters for recommendation models.
+- [Operationalize](examples/05_operationalize): Operationalizing models in a production environment on Azure.
 
 Several utilities are provided in [recommenders](recommenders) to support common tasks such as loading datasets in the format expected by different algorithms, evaluating model outputs, and splitting training/test data. Implementations of several state-of-the-art algorithms are included for self-study and customization in your own applications. See the [Recommenders documentation](https://readthedocs.org/projects/microsoft-recommenders/).
 
 For a more detailed overview of the repository, please see the documents on the [wiki page](https://github.com/microsoft/recommenders/wiki/Documents-and-Presentations).
 
-## Getting Started
-
-Please see the [setup guide](SETUP.md) for more details on setting up your machine locally, on a [Data Science Virtual Machine (DSVM)](https://azure.microsoft.com/en-gb/services/virtual-machines/data-science-virtual-machines/) or on [Azure Databricks](SETUP.md#setup-guide-for-azure-databricks).
-
-The installation of the recommenders package has been tested with 
-- Python versions 3.6 - 3.9 and [venv](https://docs.python.org/3/library/venv.html), [virtualenv](https://virtualenv.pypa.io/en/latest/index.html#) or [conda](https://docs.conda.io/projects/conda/en/latest/glossary.html?highlight=environment#conda-environment)
-
-and currently does not support version 3.10 and above. It is recommended to install the package and its dependencies inside a clean environment (such as [conda](https://docs.conda.io/projects/conda/en/latest/glossary.html?highlight=environment#conda-environment), [venv](https://docs.python.org/3/library/venv.html) or [virtualenv](https://virtualenv.pypa.io/en/latest/index.html#)).
-
-To set up on your local machine:
-
-* To install core utilities, CPU-based algorithms, and dependencies:
-
-    1. Ensure software required for compilation and Python libraries
-       is installed.
-
-       + On Linux this can be supported by adding:
-
-         ```bash
-         sudo apt-get install -y build-essential libpython<version>
-         ``` 
-
-         where `<version>` should be the Python version (e.g. `3.6`).
-
-       + On Windows you will need [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/).
-
-    2. Create a conda or virtual environment.  See the
-       [setup guide](SETUP.md) for more details.
-
-    3. Within the created environment, install the package from
-       [PyPI](https://pypi.org):
-
-       ```bash
-       pip install --upgrade pip
-       pip install --upgrade setuptools
-       pip install recommenders[examples]
-       ```
-
-    4. Register your (conda or virtual) environment with Jupyter:
+For some of the practical scenarios where recommendation systems have been applied, see [scenarios](scenarios). 
 
-       ```bash
-       python -m ipykernel install --user --name my_environment_name --display-name "Python (reco)"
-       ```
-
-    5. Start the Jupyter notebook server
-
-       ```bash
-       jupyter notebook
-       ```
-
-    6. Run the [SAR Python CPU MovieLens](examples/00_quick_start/sar_movielens.ipynb)
-       notebook under the `00_quick_start` folder.  Make sure to
-       change the kernel to "Python (reco)".
-
-* For additional options to install the package (support for GPU,
-  Spark etc.) see [this guide](recommenders/README.md).
-
-**NOTE** - The [Alternating Least Squares (ALS)](examples/00_quick_start/als_movielens.ipynb) notebooks require a PySpark environment to run. Please follow the steps in the [setup guide](SETUP.md#dependencies-setup) to run these notebooks in a PySpark environment. For the deep learning algorithms, it is recommended to use a GPU machine and to follow the steps in the [setup guide](SETUP.md#dependencies-setup) to set up Nvidia libraries.
+## Getting Started
 
-**NOTE for DSVM Users** - Please follow the steps in the [Dependencies setup - Set PySpark environment variables on Linux or MacOS](SETUP.md#dependencies-setup) and [Troubleshooting for the DSVM](SETUP.md#troubleshooting-for-the-dsvm) sections if you encounter any issue.
+We recommend [conda](https://docs.conda.io/projects/conda/en/latest/glossary.html?highlight=environment#conda-environment) for environment management, and [VS Code](https://code.visualstudio.com/) for development. To install the recommenders package and run an example notebook on Linux/WSL:
 
-**DOCKER** - Another easy way to try the recommenders repository and get started quickly is to build [docker images](tools/docker/README.md) suitable for different environments. 
+```bash
+# 1. Install gcc if it is not installed already. On Ubuntu, this could done by using the command
+# sudo apt install gcc
+
+# 2. Create and activate a new conda environment
+conda create -n <environment_name> python=3.9
+conda activate <environment_name>
+
+# 3. Install the core recommenders package. It can run all the CPU notebooks.
+pip install recommenders
+
+# 4. create a Jupyter kernel
+python -m ipykernel install --user --name <environment_name> --display-name <kernel_name>
+
+# 5. Clone this repo within VSCode or using command line:
+git clone https://github.com/recommenders-team/recommenders.git
+
+# 6. Within VSCode:
+#   a. Open a notebook, e.g., examples/00_quick_start/sar_movielens.ipynb;  
+#   b. Select Jupyter kernel <kernel_name>;
+#   c. Run the notebook.
+```
+
+For more information about setup on other platforms (e.g., Windows and macOS) and different configurations (e.g., GPU, Spark and experimental features), see the [Setup Guide](SETUP.md).
+
+In addition to the core package, several extras are also provided, including:
++ `[gpu]`: Needed for running GPU models.
++ `[spark]`: Needed for running Spark models.
++ `[dev]`: Needed for development for the repo.
++ `[all]`: `[gpu]`|`[spark]`|`[dev]`
++ `[experimental]`: Models that are not thoroughly tested and/or may require additional steps in installation.
 
 ## Algorithms
 
-The table below lists the recommender algorithms currently available in the repository. Notebooks are linked under the Example column as Quick start, showcasing an easy to run example of the algorithm, or as Deep dive, explaining in detail the math and implementation of the algorithm.
+The table below lists the recommendation algorithms currently available in the repository. Notebooks are linked under the Example column as Quick start, showcasing an easy to run example of the algorithm, or as Deep dive, explaining in detail the math and implementation of the algorithm.
 
 | Algorithm | Type | Description | Example |
 |-----------|------|-------------|---------|
 | Alternating Least Squares (ALS) | Collaborative Filtering | Matrix factorization algorithm for explicit or implicit feedback in large datasets, optimized for scalability and distributed computing capability. It works in the PySpark environment. | [Quick start](examples/00_quick_start/als_movielens.ipynb) / [Deep dive](examples/02_model_collaborative_filtering/als_deep_dive.ipynb) |
 | Attentive Asynchronous Singular Value Decomposition (A2SVD)<sup>*</sup> | Collaborative Filtering | Sequential-based algorithm that aims to capture both long and short-term user preferences using attention mechanism. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/sequential_recsys_amazondataset.ipynb) |
 | Cornac/Bayesian Personalized Ranking (BPR) | Collaborative Filtering | Matrix factorization algorithm for predicting item ranking with implicit feedback. It works in the CPU environment. | [Deep dive](examples/02_model_collaborative_filtering/cornac_bpr_deep_dive.ipynb) |
 | Cornac/Bilateral Variational Autoencoder (BiVAE) | Collaborative Filtering | Generative model for dyadic data (e.g., user-item interactions). It works in the CPU/GPU environment. | [Deep dive](examples/02_model_collaborative_filtering/cornac_bivae_deep_dive.ipynb) |
 | Convolutional Sequence Embedding Recommendation (Caser) | Collaborative Filtering | Algorithm based on convolutions that aim to capture both user’s general preferences and sequential patterns. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/sequential_recsys_amazondataset.ipynb) |
 | Deep Knowledge-Aware Network (DKN)<sup>*</sup> | Content-Based Filtering | Deep learning algorithm incorporating a knowledge graph and article embeddings for providing news or article recommendations. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/dkn_MIND.ipynb) / [Deep dive](examples/02_model_content_based_filtering/dkn_deep_dive.ipynb) |
-| Extreme Deep Factorization Machine (xDeepFM)<sup>*</sup> | Hybrid | Deep learning based algorithm for implicit and explicit feedback with user/item features. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/xdeepfm_criteo.ipynb) |
+| Extreme Deep Factorization Machine (xDeepFM)<sup>*</sup> | Collaborative Filtering | Deep learning based algorithm for implicit and explicit feedback with user/item features. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/xdeepfm_criteo.ipynb) |
 | FastAI Embedding Dot Bias (FAST) | Collaborative Filtering | General purpose algorithm with embeddings and biases for users and items. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/fastai_movielens.ipynb) |
-| LightFM/Hybrid Matrix Factorization | Hybrid | Hybrid matrix factorization algorithm for both implicit and explicit feedbacks. It works in the CPU environment. | [Quick start](examples/02_model_hybrid/lightfm_deep_dive.ipynb) |
+| LightFM/Factorization Machine | Collaborative Filtering | Factorization Machine algorithm for both implicit and explicit feedbacks. It works in the CPU environment. | [Quick start](examples/02_model_collaborative_filtering/lightfm_deep_dive.ipynb) |
 | LightGBM/Gradient Boosting Tree<sup>*</sup> | Content-Based Filtering | Gradient Boosting Tree algorithm for fast training and low memory usage in content-based problems. It works in the CPU/GPU/PySpark environments. | [Quick start in CPU](examples/00_quick_start/lightgbm_tinycriteo.ipynb) / [Deep dive in PySpark](examples/02_model_content_based_filtering/mmlspark_lightgbm_criteo.ipynb) |
 | LightGCN | Collaborative Filtering | Deep learning algorithm which simplifies the design of GCN for predicting implicit feedback. It works in the CPU/GPU environment. | [Deep dive](examples/02_model_collaborative_filtering/lightgcn_deep_dive.ipynb) |
-| GeoIMC<sup>*</sup> | Hybrid | Matrix completion algorithm that has into account user and item features using Riemannian conjugate gradients optimization and following a geometric approach. It works in the CPU environment. | [Quick start](examples/00_quick_start/geoimc_movielens.ipynb) |
-| GRU4Rec | Collaborative Filtering | Sequential-based algorithm that aims to capture both long and short-term user preferences using recurrent neural networks. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/sequential_recsys_amazondataset.ipynb) |
+| GeoIMC<sup>*</sup> | Collaborative Filtering | Matrix completion algorithm that has into account user and item features using Riemannian conjugate gradients optimization and following a geometric approach. It works in the CPU environment. | [Quick start](examples/00_quick_start/geoimc_movielens.ipynb) |
+| GRU | Collaborative Filtering | Sequential-based algorithm that aims to capture both long and short-term user preferences using recurrent neural networks. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/sequential_recsys_amazondataset.ipynb) |
 | Multinomial VAE | Collaborative Filtering | Generative model for predicting user/item interactions. It works in the CPU/GPU environment. | [Deep dive](examples/02_model_collaborative_filtering/multi_vae_deep_dive.ipynb) |
 | Neural Recommendation with Long- and Short-term User Representations (LSTUR)<sup>*</sup> | Content-Based Filtering | Neural recommendation algorithm for recommending news articles with long- and short-term user interest modeling. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/lstur_MIND.ipynb) |
 | Neural Recommendation with Attentive Multi-View Learning (NAML)<sup>*</sup> | Content-Based Filtering | Neural recommendation algorithm for recommending news articles with attentive multi-view learning. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/naml_MIND.ipynb) |
 | Neural Collaborative Filtering (NCF) | Collaborative Filtering | Deep learning algorithm with enhanced performance for user/item implicit feedback. It works in the CPU/GPU environment.| [Quick start](examples/00_quick_start/ncf_movielens.ipynb) / [Deep dive](examples/02_model_collaborative_filtering/ncf_deep_dive.ipynb) |
 | Neural Recommendation with Personalized Attention (NPA)<sup>*</sup> | Content-Based Filtering | Neural recommendation algorithm for recommending news articles with personalized attention network. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/npa_MIND.ipynb) |
 | Neural Recommendation with Multi-Head Self-Attention (NRMS)<sup>*</sup> | Content-Based Filtering | Neural recommendation algorithm for recommending news articles with multi-head self-attention. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/nrms_MIND.ipynb) |
 | Next Item Recommendation (NextItNet) | Collaborative Filtering | Algorithm based on dilated convolutions and residual network that aims to capture sequential patterns. It considers both user/item interactions and features.  It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/sequential_recsys_amazondataset.ipynb) |
@@ -126,16 +104,16 @@
 | Short-term and Long-term Preference Integrated Recommender (SLi-Rec)<sup>*</sup> | Collaborative Filtering | Sequential-based algorithm that aims to capture both long and short-term user preferences using attention mechanism, a time-aware controller and a content-aware controller. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/sequential_recsys_amazondataset.ipynb) |
 | Multi-Interest-Aware Sequential User Modeling (SUM)<sup>*</sup> | Collaborative Filtering | An enhanced memory network-based sequential user model which aims to capture users' multiple interests. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/sequential_recsys_amazondataset.ipynb) |
 | Sequential Recommendation Via Personalized Transformer (SSEPT) | Collaborative Filtering | Transformer based algorithm for sequential recommendation with User embedding. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/sasrec_amazon.ipynb) |
 | Standard VAE | Collaborative Filtering | Generative Model for predicting user/item interactions.  It works in the CPU/GPU environment. | [Deep dive](examples/02_model_collaborative_filtering/standard_vae_deep_dive.ipynb) |
 | Surprise/Singular Value Decomposition (SVD) | Collaborative Filtering | Matrix factorization algorithm for predicting explicit rating feedback in small datasets. It works in the CPU/GPU environment. | [Deep dive](examples/02_model_collaborative_filtering/surprise_svd_deep_dive.ipynb) |
 | Term Frequency - Inverse Document Frequency (TF-IDF) | Content-Based Filtering | Simple similarity-based algorithm for content-based recommendations with text datasets. It works in the CPU environment. | [Quick  start](examples/00_quick_start/tfidf_covid.ipynb) |
 | Vowpal Wabbit (VW)<sup>*</sup> | Content-Based Filtering | Fast online learning algorithms, great for scenarios where user features / context are constantly changing. It uses the CPU for online learning. | [Deep dive](examples/02_model_content_based_filtering/vowpal_wabbit_deep_dive.ipynb) |
-| Wide and Deep | Hybrid | Deep learning algorithm that can memorize feature interactions and generalize user features. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/wide_deep_movielens.ipynb) |
-| xLearn/Factorization Machine (FM) & Field-Aware FM (FFM) | Hybrid | Quick and memory efficient algorithm to predict labels with user/item features. It works in the CPU/GPU environment. | [Deep dive](examples/02_model_hybrid/fm_deep_dive.ipynb) |
+| Wide and Deep | Collaborative Filtering | Deep learning algorithm that can memorize feature interactions and generalize user features. It works in the CPU/GPU environment. | [Quick start](examples/00_quick_start/wide_deep_movielens.ipynb) |
+| xLearn/Factorization Machine (FM) & Field-Aware FM (FFM) | Collaborative Filtering | Quick and memory efficient algorithm to predict labels with user/item features. It works in the CPU/GPU environment. | [Deep dive](examples/02_model_collaborative_filtering/fm_deep_dive.ipynb) |
 
 **NOTE**: <sup>*</sup> indicates algorithms invented/contributed by Microsoft.
 
 Independent or incubating algorithms and utilities are candidates for the [contrib](contrib) folder. This will house contributions which may not easily fit into the core repository or need time to refactor or mature the code and add necessary tests.
 
 | Algorithm | Type | Description | Example |
 |-----------|------|-------------|---------|
@@ -148,60 +126,39 @@
 | Algo | MAP | nDCG@k | Precision@k | Recall@k | RMSE | MAE | R<sup>2</sup> | Explained Variance |
 | --- | --- | --- | --- | --- | --- | --- | --- | --- |
 | [ALS](examples/00_quick_start/als_movielens.ipynb) | 0.004732 |	0.044239 |	0.048462 |	0.017796 | 0.965038 |	0.753001 |	0.255647 |	0.251648 |
 | [BiVAE](examples/02_model_collaborative_filtering/cornac_bivae_deep_dive.ipynb) | 0.146126	| 0.475077 |	0.411771 |	0.219145 | N/A |	N/A |	N/A |	N/A |
 | [BPR](examples/02_model_collaborative_filtering/cornac_bpr_deep_dive.ipynb) | 0.132478	| 0.441997 |	0.388229 |	0.212522 | N/A |	N/A |	N/A |	N/A |
 | [FastAI](examples/00_quick_start/fastai_movielens.ipynb) | 0.025503 |	0.147866 |	0.130329 |	0.053824 | 0.943084 |	0.744337 |	0.285308 |	0.287671 |
 | [LightGCN](examples/02_model_collaborative_filtering/lightgcn_deep_dive.ipynb) | 0.088526 | 0.419846 | 0.379626 | 0.144336 | N/A | N/A | N/A | N/A |
-| [NCF](examples/02_model_hybrid/ncf_deep_dive.ipynb) | 0.107720	| 0.396118 |	0.347296 |	0.180775 | N/A | N/A | N/A | N/A |
+| [NCF](examples/02_model_collaborative_filtering/ncf_deep_dive.ipynb) | 0.107720	| 0.396118 |	0.347296 |	0.180775 | N/A | N/A | N/A | N/A |
 | [SAR](examples/00_quick_start/sar_movielens.ipynb) | 0.110591 |	0.382461 | 	0.330753 | 0.176385 | 1.253805 | 1.048484 |	-0.569363 |	0.030474 |
 | [SVD](examples/02_model_collaborative_filtering/surprise_svd_deep_dive.ipynb) | 0.012873	| 0.095930 |	0.091198 |	0.032783 | 0.938681 | 0.742690 | 0.291967 | 0.291971 |
 
-## Code of Conduct
-
-This project adheres to [Microsoft's Open Source Code of Conduct](CODE_OF_CONDUCT.md) in order to foster a welcoming and inspiring community for all.
-
 ## Contributing
 
 This project welcomes contributions and suggestions. Before contributing, please see our [contribution guidelines](CONTRIBUTING.md).
 
-## Build Status
-
-These tests are the nightly builds, which compute the smoke and integration tests. `main` is our principal branch and `staging` is our development branch. We use `pytest` for testing python utilities in [recommenders](recommenders) and `papermill` for the [notebooks](examples). For more information about the testing pipelines, please see the [test documentation](tests/README.md).
+This project adheres to [Microsoft's Open Source Code of Conduct](CODE_OF_CONDUCT.md) in order to foster a welcoming and inspiring community for all.
 
-### DSVM Build Status
+## Build Status
 
-The following tests run on a Linux DSVM daily. 
+These tests are the nightly builds, which compute the asynchronous tests. `main` is our principal branch and `staging` is our development branch. We use [pytest](https://docs.pytest.org/) for testing python utilities in [recommenders](recommenders) and the Recommenders [notebook executor](recommenders/utils/notebook_utils.py) for the [notebooks](examples). 
 
-| Build Type | Branch | Status |  | Branch | Status |
-| --- | --- | --- | --- | --- | --- |
-| **Linux CPU** | main | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/linux-tests/dsvm_nightly_linux_cpu?branchName=main)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=162&branchName=main) | | staging | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/linux-tests/dsvm_nightly_linux_cpu?branchName=staging)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=162&branchName=staging) |
-| **Linux GPU** | main | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/linux-tests/dsvm_nightly_linux_gpu?branchName=main)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=163&branchName=main) | | staging | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/linux-tests/dsvm_nightly_linux_gpu?branchName=staging)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=163&branchName=staging) |
-| **Linux Spark** | main | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/linux-tests/dsvm_nightly_linux_pyspark?branchName=main)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=164&branchName=main) | | staging | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/linux-tests/dsvm_nightly_linux_pyspark?branchName=staging)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=164&branchName=staging) |
-<!--
-| **Windows CPU** | main | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/windows-tests/dsvm_nightly_win_cpu?branchName=main)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=101&branchName=main) | | staging | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/windows-tests/dsvm_nightly_win_cpu?branchName=staging)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=101&branchName=staging) |
-| **Windows GPU** | main | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/windows-tests/dsvm_nightly_win_gpu?branchName=main)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=102&branchName=main) | | staging | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/windows-tests/dsvm_nightly_win_gpu?branchName=staging)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=102&branchName=staging) |
-| **Windows Spark** | main | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/windows-tests/dsvm_nightly_win_pyspark?branchName=main)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=103&branchName=main) | | staging | [![Build Status](https://dev.azure.com/best-practices/recommenders/_apis/build/status/windows-tests/dsvm_nightly_win_pyspark?branchName=staging)](https://dev.azure.com/best-practices/recommenders/_build/latest?definitionId=103&branchName=staging) |
--->
+For more information about the testing pipelines, please see the [test documentation](tests/README.md).
 
 ### AzureML Nightly Build Status
 
-Smoke and integration tests are run daily on AzureML.
+The nightly build tests are run daily on AzureML.
 
 | Build Type | Branch | Status |  | Branch | Status |
 | --- | --- | --- | --- | --- | --- |
 | **Linux CPU** | main | [![azureml-cpu-nightly](https://github.com/microsoft/recommenders/actions/workflows/azureml-cpu-nightly.yml/badge.svg?branch=main)](https://github.com/microsoft/recommenders/actions/workflows/azureml-cpu-nightly.yml?query=branch%3Amain) | | staging | [![azureml-cpu-nightly](https://github.com/microsoft/recommenders/actions/workflows/azureml-cpu-nightly.yml/badge.svg?branch=staging)](https://github.com/microsoft/recommenders/actions/workflows/azureml-cpu-nightly.yml?query=branch%3Astaging) |
 | **Linux GPU** | main | [![azureml-gpu-nightly](https://github.com/microsoft/recommenders/actions/workflows/azureml-gpu-nightly.yml/badge.svg?branch=main)](https://github.com/microsoft/recommenders/actions/workflows/azureml-gpu-nightly.yml?query=branch%3Amain) | | staging | [![azureml-gpu-nightly](https://github.com/microsoft/recommenders/actions/workflows/azureml-gpu-nightly.yml/badge.svg?branch=staging)](https://github.com/microsoft/recommenders/actions/workflows/azureml-gpu-nightly.yml?query=branch%3Astaging) |
 | **Linux Spark** | main | [![azureml-spark-nightly](https://github.com/microsoft/recommenders/actions/workflows/azureml-spark-nightly.yml/badge.svg?branch=main)](https://github.com/microsoft/recommenders/actions/workflows/azureml-spark-nightly.yml?query=branch%3Amain) | | staging | [![azureml-spark-nightly](https://github.com/microsoft/recommenders/actions/workflows/azureml-spark-nightly.yml/badge.svg?branch=staging)](https://github.com/microsoft/recommenders/actions/workflows/azureml-spark-nightly.yml?query=branch%3Astaging) |
 
-## Related projects
-
-- [Microsoft AI Github](https://github.com/microsoft/ai): Find other Best Practice projects, and Azure AI design patterns in our central repository.
-- [NLP best practices](https://github.com/microsoft/nlp-recipes): Best practices and examples on NLP.
-- [Computer vision best practices](https://github.com/microsoft/computervision-recipes): Best practices and examples on computer vision.
-- [Forecasting best practices](https://github.com/microsoft/forecasting): Best practices and examples on time series forecasting.
-
-## Reference papers
+## References
 
+- D. Li, J. Lian, L. Zhang, K. Ren, D. Lu, T. Wu, X. Xie, "Recommender Systems: Frontiers and Practices", Springer, Beijing, 2024. [Available on this link](https://www.amazon.com/Recommender-Systems-Frontiers-Practices-Dongsheng/dp/9819989639/).
 - A. Argyriou, M. González-Fierro, and L. Zhang, "Microsoft Recommenders: Best Practices for Production-Ready Recommendation Systems", *WWW 2020: International World Wide Web Conference Taipei*, 2020. Available online: https://dl.acm.org/doi/abs/10.1145/3366424.3382692
-- L. Zhang, T. Wu, X. Xie, A. Argyriou, M. González-Fierro and J. Lian, "Building Production-Ready Recommendation System at Scale", *ACM SIGKDD Conference on Knowledge Discovery and Data Mining 2019 (KDD 2019)*, 2019.
 - S. Graham,  J.K. Min, T. Wu, "Microsoft recommenders: tools to accelerate developing recommender systems", *RecSys '19: Proceedings of the 13th ACM Conference on Recommender Systems*, 2019. Available online: https://dl.acm.org/doi/10.1145/3298689.3346967
+- L. Zhang, T. Wu, X. Xie, A. Argyriou, M. González-Fierro and J. Lian, "Building Production-Ready Recommendation System at Scale", *ACM SIGKDD Conference on Knowledge Discovery and Data Mining 2019 (KDD 2019)*, 2019.
```

### Comparing `recommenders-1.1.1/recommenders/README.md` & `recommenders-1.2.0/recommenders/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+<!--
+Copyright (c) Recommenders contributors.
+Licensed under the MIT License.
+-->
+
 # Recommender Utilities
 
 This package contains functions to simplify common tasks used when developing and evaluating recommender systems. A short description of the submodules is provided below. For more details about what functions are available and how to use them, please review the doc-strings provided with the code or the [online documentation](https://readthedocs.org/projects/microsoft-recommenders/).
 
 # Installation
 
 ## Pre-requisites
 Some dependencies require compilation during pip installation. On Linux this can be supported by adding build-essential dependencies:
 ```bash
 sudo apt-get install -y build-essential libpython<version>
 ``` 
-where `<version>` should be the Python version (e.g. `3.6`).
+where `<version>` should be the Python version (e.g. `3.8`).
 
 On Windows you will need [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)
 
 For more details about the software requirements that must be pre-installed on each supported platform, see the [setup guide](https://github.com/microsoft/recommenders/blob/main/SETUP.md).   
 
 ## Basic installation
 
@@ -139,15 +144,15 @@
 The models submodule contains implementations of various algorithms that can be used in addition to external packages to evaluate and develop new recommender system approaches. A description of all the algorithms can be found on [this table](../README.md#algorithms). The following is a list of the algorithm utilities:
 
 * Cornac
 * DeepRec
   *  Convolutional Sequence Embedding Recommendation (CASER)
   *  Deep Knowledge-Aware Network (DKN)
   *  Extreme Deep Factorization Machine (xDeepFM)
-  *  GRU4Rec
+  *  GRU
   *  LightGCN
   *  Next Item Recommendation (NextItNet)
   *  Short-term and Long-term Preference Integrated Recommender (SLi-Rec)
   *  Multi-Interest-Aware Sequential User Modeling (SUM)
 * FastAI
 * GeoIMC
 * LightFM
```

### Comparing `recommenders-1.1.1/recommenders/datasets/amazon_reviews.py` & `recommenders-1.2.0/recommenders/datasets/amazon_reviews.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import shutil
 import pandas as pd
 import gzip
 import random
```

### Comparing `recommenders-1.1.1/recommenders/datasets/cosmos_cli.py` & `recommenders-1.2.0/recommenders/datasets/cosmos_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 import pydocumentdb.errors as errors
 
 
 def find_collection(client, dbid, id):
     """Find whether or not a CosmosDB collection exists.
```

### Comparing `recommenders-1.1.1/recommenders/datasets/covid_utils.py` & `recommenders-1.2.0/recommenders/datasets/covid_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import pandas as pd
 import requests
```

### Comparing `recommenders-1.1.1/recommenders/datasets/criteo.py` & `recommenders-1.2.0/recommenders/datasets/criteo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 import pandas as pd
 import os
 import tarfile
 
@@ -153,15 +153,34 @@
     if path is None:
         folder = os.path.dirname(compressed_file)
         extracted_dir = os.path.join(folder, "dac")
     else:
         extracted_dir = path
 
     with tarfile.open(compressed_file) as tar:
-        tar.extractall(extracted_dir)
+
+        def is_within_directory(directory, target):
+
+            abs_directory = os.path.abspath(directory)
+            abs_target = os.path.abspath(target)
+
+            prefix = os.path.commonprefix([abs_directory, abs_target])
+
+            return prefix == abs_directory
+
+        def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+
+            for member in tar.getmembers():
+                member_path = os.path.join(path, member.name)
+                if not is_within_directory(path, member_path):
+                    raise Exception("Attempted Path Traversal in Tar File")
+
+            tar.extractall(path, members, numeric_owner=numeric_owner)
+
+        safe_extract(tar, extracted_dir)
 
     filename_selector = {"sample": "dac_sample.txt", "full": "train.txt"}
     return os.path.join(extracted_dir, filename_selector[size])
 
 
 def get_spark_schema(header=DEFAULT_HEADER):
     """Get Spark schema from header.
```

### Comparing `recommenders-1.1.1/recommenders/datasets/download_utils.py` & `recommenders-1.2.0/recommenders/datasets/download_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import logging
 import requests
 import math
 import zipfile
```

### Comparing `recommenders-1.1.1/recommenders/datasets/mind.py` & `recommenders-1.2.0/recommenders/datasets/mind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import random
 import logging
 import json
 import numpy as np
@@ -248,15 +248,16 @@
 
     Args:
         dest_path (str): Destination directory path for the downloaded file
 
     Returns:
         str: File path where Glove was extracted.
     """
-    url = "http://nlp.stanford.edu/data/glove.6B.zip"
+    # url = "http://nlp.stanford.edu/data/glove.6B.zip"
+    url = "https://huggingface.co/stanfordnlp/glove/resolve/main/glove.6B.zip"
     filepath = maybe_download(url=url, work_directory=dest_path)
     glove_path = os.path.join(dest_path, "glove")
     unzip_file(filepath, glove_path, clean_zip_file=False)
     return glove_path
 
 
 def generate_embeddings(
```

### Comparing `recommenders-1.1.1/recommenders/datasets/movielens.py` & `recommenders-1.2.0/recommenders/datasets/movielens.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import re
 import random
 import shutil
 import warnings
@@ -194,15 +194,15 @@
             title_col='Title',
             genres_col='Genres',
             year_col='Year'
         )
     """
     size = size.lower()
     if size not in DATA_FORMAT and size not in MOCK_DATA_FORMAT:
-        raise ValueError(ERROR_MOVIE_LENS_SIZE)
+        raise ValueError(f"Size: {size}. " + ERROR_MOVIE_LENS_SIZE)
 
     if header is None:
         header = DEFAULT_HEADER
     elif len(header) < 2:
         raise ValueError(ERROR_HEADER)
     elif len(header) > 4:
         warnings.warn(WARNING_MOVIE_LENS_HEADER)
@@ -272,15 +272,15 @@
         year_col (str): Movie release year column name. If None, the column will not be loaded.
 
     Returns:
         pandas.DataFrame: Movie information data, such as title, genres, and release year.
     """
     size = size.lower()
     if size not in DATA_FORMAT:
-        raise ValueError(ERROR_MOVIE_LENS_SIZE)
+        raise ValueError(f"Size: {size}. " + ERROR_MOVIE_LENS_SIZE)
 
     with download_path(local_cache_path) as path:
         filepath = os.path.join(path, "ml-{}.zip".format(size))
         _, item_datapath = _maybe_download_and_extract(size, filepath)
         item_df = _load_item_df(
             size, item_datapath, movie_col, title_col, genres_col, year_col
         )
@@ -417,15 +417,15 @@
         )
 
         # On DataBricks, pass the dbutils argument as follows:
         spark_df = load_spark_df(spark, dbutils=dbutils)
     """
     size = size.lower()
     if size not in DATA_FORMAT and size not in MOCK_DATA_FORMAT:
-        raise ValueError(ERROR_MOVIE_LENS_SIZE)
+        raise ValueError(f"Size: {size}. " + ERROR_MOVIE_LENS_SIZE)
 
     if size in MOCK_DATA_FORMAT:
         # generate fake data
         return MockMovielensSchema.get_spark_df(
             spark,
             keep_title_col=(title_col is not None),
             keep_genre_col=(genres_col is not None),
@@ -546,15 +546,15 @@
     """Downloads MovieLens datafile.
 
     Args:
         size (str): Size of the data to load. One of ("100k", "1m", "10m", "20m").
         dest_path (str): File path for the downloaded file
     """
     if size not in DATA_FORMAT:
-        raise ValueError(ERROR_MOVIE_LENS_SIZE)
+        raise ValueError(f"Size: {size}. " + ERROR_MOVIE_LENS_SIZE)
 
     url = "https://files.grouplens.org/datasets/movielens/ml-" + size + ".zip"
     dirs, file = os.path.split(dest_path)
     maybe_download(url, file, work_directory=dirs)
 
 
 def extract_movielens(size, rating_path, item_path, zip_path):
@@ -592,18 +592,26 @@
     Dataset schema and generation is configured using pandera.
     Please see https://pandera.readthedocs.io/en/latest/schema_models.html
     for more information.
     """
 
     # Some notebooks will do a cross join with userID and itemID,
     # a sparse range for these IDs can slow down the notebook tests
-    userID: Series[int] = Field(in_range={"min_value": 1, "max_value": 50}, alias=DEFAULT_USER_COL)
-    itemID: Series[int] = Field(in_range={"min_value": 1, "max_value": 50}, alias=DEFAULT_ITEM_COL)
-    rating: Series[float] = Field(in_range={"min_value": 1, "max_value": 5}, alias=DEFAULT_RATING_COL)
-    timestamp: Series[int] = Field(in_range={"min_value": 0, "max_value": 1e9}, alias=DEFAULT_TIMESTAMP_COL)
+    userID: Series[int] = Field(
+        in_range={"min_value": 1, "max_value": 50}, alias=DEFAULT_USER_COL
+    )
+    itemID: Series[int] = Field(
+        in_range={"min_value": 1, "max_value": 50}, alias=DEFAULT_ITEM_COL
+    )
+    rating: Series[float] = Field(
+        in_range={"min_value": 1, "max_value": 5}, alias=DEFAULT_RATING_COL
+    )
+    timestamp: Series[int] = Field(
+        in_range={"min_value": 0, "max_value": 1e9}, alias=DEFAULT_TIMESTAMP_COL
+    )
     title: Series[str] = Field(eq="foo", alias=DEFAULT_TITLE_COL)
     genre: Series[str] = Field(eq="genreA|0", alias=DEFAULT_GENRE_COL)
 
     @classmethod
     def get_df(
         cls,
         size: int = 3,
```

### Comparing `recommenders-1.1.1/recommenders/datasets/pandas_df_utils.py` & `recommenders-1.2.0/recommenders/datasets/pandas_df_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import logging
 import pandas as pd
 import numpy as np
 from functools import lru_cache, wraps
 
@@ -83,15 +83,15 @@
     ]
 
 
 class LibffmConverter:
     """Converts an input dataframe to another dataframe in libffm format. A text file of the converted
     Dataframe is optionally generated.
 
-    .. note::
+    Note:
 
         The input dataframe is expected to represent the feature data in the following schema:
 
         .. code-block:: python
 
             |field-1|field-2|...|field-n|rating|
             |feature-1-1|feature-2-1|...|feature-n-1|1|
@@ -356,27 +356,22 @@
 
 
 def has_columns(df, columns):
     """Check if DataFrame has necessary columns
 
     Args:
         df (pandas.DataFrame): DataFrame
-        columns (list(str): columns to check for
+        columns (iterable(str)): columns to check for
 
     Returns:
         bool: True if DataFrame has specified columns.
     """
-
-    result = True
-    for column in columns:
-        if column not in df.columns:
-            logger.error("Missing column: {} in DataFrame".format(column))
-            result = False
-
-    return result
+    if not isinstance(columns, set):
+        columns = set(columns)
+    return columns.issubset(df.columns)
 
 
 def has_same_base_dtype(df_1, df_2, columns=None):
     """Check if specified columns have the same base dtypes across both DataFrames
 
     Args:
         df_1 (pandas.DataFrame): first DataFrame
```

### Comparing `recommenders-1.1.1/recommenders/datasets/python_splitters.py` & `recommenders-1.2.0/recommenders/datasets/python_splitters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split as sk_split
 
 from recommenders.utils.constants import (
     DEFAULT_ITEM_COL,
@@ -83,44 +83,41 @@
             data,
             min_rating=min_rating,
             filter_by=filter_by,
             col_user=col_user,
             col_item=col_item,
         )
 
-    # Split by each group and aggregate splits together.
-    splits = []
+    if is_random:
+        np.random.seed(seed)
+        data["random"] = np.random.rand(data.shape[0])
+        order_by = "random"
+    else:
+        order_by = col_timestamp
 
-    # If it is for chronological splitting, the split will be performed in a random way.
-    df_grouped = (
-        data.sort_values(col_timestamp).groupby(split_by_column)
-        if is_random is False
-        else data.groupby(split_by_column)
-    )
-
-    for _, group in df_grouped:
-        group_splits = split_pandas_data_with_ratios(
-            group, ratio, shuffle=is_random, seed=seed
-        )
+    data = data.sort_values([split_by_column, order_by])
 
-        # Concatenate the list of split dataframes.
-        concat_group_splits = pd.concat(group_splits)
+    groups = data.groupby(split_by_column)
 
-        splits.append(concat_group_splits)
+    data["count"] = groups[split_by_column].transform("count")
+    data["rank"] = groups.cumcount() + 1
 
-    # Concatenate splits for all the groups together.
-    splits_all = pd.concat(splits)
+    if is_random:
+        data = data.drop("random", axis=1)
 
-    # Take split by split_index
-    splits_list = [
-        splits_all[splits_all["split_index"] == x].drop("split_index", axis=1)
-        for x in range(len(ratio))
-    ]
+    splits = []
+    prev_threshold = None
+    for threshold in np.cumsum(ratio):
+        condition = data["rank"] <= round(threshold * data["count"])
+        if prev_threshold is not None:
+            condition &= data["rank"] > round(prev_threshold * data["count"])
+        splits.append(data[condition].drop(["rank", "count"], axis=1))
+        prev_threshold = threshold
 
-    return splits_list
+    return splits
 
 
 def python_chrono_split(
     data,
     ratio=0.75,
     min_rating=1,
     filter_by="user",
```

### Comparing `recommenders-1.1.1/recommenders/datasets/spark_splitters.py` & `recommenders-1.2.0/recommenders/datasets/spark_splitters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 
 try:
     from pyspark.sql import functions as F, Window
     from pyspark.storagelevel import StorageLevel
```

### Comparing `recommenders-1.1.1/recommenders/datasets/sparse.py` & `recommenders-1.2.0/recommenders/datasets/sparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import pandas as pd
 import numpy as np
 import itertools
 
 from scipy.sparse import coo_matrix
```

### Comparing `recommenders-1.1.1/recommenders/datasets/split_utils.py` & `recommenders-1.2.0/recommenders/datasets/split_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import math
 import logging
 
 from recommenders.utils.constants import DEFAULT_ITEM_COL, DEFAULT_USER_COL
@@ -134,16 +134,15 @@
     else:
         raise ValueError("name should be either 'user' or 'item'.")
 
 
 def split_pandas_data_with_ratios(data, ratios, seed=42, shuffle=False):
     """Helper function to split pandas DataFrame with given ratios
 
-    .. note::
-
+    Note:
         Implementation referenced from `this source <https://stackoverflow.com/questions/38250710/how-to-split-data-into-3-sets-train-validation-and-test>`_.
 
     Args:
         data (pandas.DataFrame): Pandas data frame to be split.
         ratios (list of floats): list of ratios for split. The ratios have to sum to 1.
         seed (int): random seed.
         shuffle (bool): whether data will be shuffled when being split.
```

### Comparing `recommenders-1.1.1/recommenders/datasets/wikidata.py` & `recommenders-1.2.0/recommenders/datasets/wikidata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import pandas as pd
 import requests
 import logging
 from retrying import retry
 
@@ -59,15 +59,15 @@
     )
 
     try:
         response = session.get(API_URL_WIKIPEDIA, params=params)
         page_id = response.json()["query"]["search"][0]["pageid"]
     except Exception:
         # TODO: distinguish between connection error and entity not found
-        logger.error("ENTITY NOT FOUND")
+        logger.warning("ENTITY NOT FOUND")
         return "entityNotFound"
 
     params = dict(
         action="query",
         prop="pageprops",
         ppprop="wikibase_item",
         pageids=[page_id],
@@ -77,15 +77,15 @@
     try:
         response = session.get(API_URL_WIKIPEDIA, params=params)
         entity_id = response.json()["query"]["pages"][str(page_id)]["pageprops"][
             "wikibase_item"
         ]
     except Exception:
         # TODO: distinguish between connection error and entity not found
-        logger.error("ENTITY NOT FOUND")
+        logger.warning("ENTITY NOT FOUND")
         return "entityNotFound"
 
     return entity_id
 
 
 @retry(wait_random_min=1000, wait_random_max=5000, stop_max_attempt_number=5)
 def query_entity_links(entity_id, session=None):
@@ -135,15 +135,15 @@
     session = get_session(session=session)
 
     try:
         data = session.get(
             API_URL_WIKIDATA, params=dict(query=query, format="json")
         ).json()
     except Exception as e:  # noqa: F841
-        logger.error("ENTITY NOT FOUND")
+        logger.warning("ENTITY NOT FOUND")
         return {}
 
     return data
 
 
 def read_linked_entities(data):
     """Obtain lists of liken entities (IDs and names) from dictionary
@@ -196,15 +196,15 @@
 
     session = get_session(session=session)
 
     try:
         r = session.get(API_URL_WIKIDATA, params=dict(query=query, format="json"))
         description = r.json()["results"]["bindings"][0]["o"]["value"]
     except Exception as e:  # noqa: F841
-        logger.error("DESCRIPTION NOT FOUND")
+        logger.warning("DESCRIPTION NOT FOUND")
         return "descriptionNotFound"
 
     return description
 
 
 def search_wikidata(names, extras=None, describe=True, verbose=False):
     """Create DataFrame of Wikidata search results
```

### Comparing `recommenders-1.1.1/recommenders/evaluation/python_evaluation.py` & `recommenders-1.2.0/recommenders/evaluation/python_evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import pandas as pd
 from functools import wraps
 from sklearn.metrics import (
     mean_squared_error,
@@ -28,14 +28,40 @@
 from recommenders.datasets.pandas_df_utils import (
     has_columns,
     has_same_base_dtype,
     lru_cache_df,
 )
 
 
+class ColumnMismatchError(Exception):
+    """Exception raised when there is a mismatch in columns.
+
+    This exception is raised when an operation involving columns
+    encounters a mismatch or inconsistency.
+
+    Attributes:
+        message (str): Explanation of the error.
+    """
+
+    pass
+
+
+class ColumnTypeMismatchError(Exception):
+    """Exception raised when there is a mismatch in column types.
+
+    This exception is raised when an operation involving column types
+    encounters a mismatch or inconsistency.
+
+    Attributes:
+        message (str): Explanation of the error.
+    """
+
+    pass
+
+
 def _check_column_dtypes(func):
     """Checks columns of DataFrame inputs
 
     This includes the checks on:
 
     * whether the input columns exist in the input DataFrames
     * whether the data types of col_user as well as col_item are matched in the two input DataFrames.
@@ -49,48 +75,53 @@
 
     @wraps(func)
     def check_column_dtypes_wrapper(
         rating_true,
         rating_pred,
         col_user=DEFAULT_USER_COL,
         col_item=DEFAULT_ITEM_COL,
-        col_rating=DEFAULT_RATING_COL,
         col_prediction=DEFAULT_PREDICTION_COL,
         *args,
-        **kwargs
+        **kwargs,
     ):
         """Check columns of DataFrame inputs
 
         Args:
             rating_true (pandas.DataFrame): True data
             rating_pred (pandas.DataFrame): Predicted data
             col_user (str): column name for user
             col_item (str): column name for item
             col_rating (str): column name for rating
             col_prediction (str): column name for prediction
         """
+        # Some ranking metrics don't have the rating column, so we don't need to check.
+        expected_true_columns = {col_user, col_item}
+        if "col_rating" in kwargs:
+            expected_true_columns.add(kwargs["col_rating"])
+        if not has_columns(rating_true, expected_true_columns):
+            raise ColumnMismatchError("Missing columns in true rating DataFrame")
+
+        if not has_columns(rating_pred, {col_user, col_item, col_prediction}):
+            raise ColumnMismatchError("Missing columns in predicted rating DataFrame")
 
-        if not has_columns(rating_true, [col_user, col_item, col_rating]):
-            raise ValueError("Missing columns in true rating DataFrame")
-        if not has_columns(rating_pred, [col_user, col_item, col_prediction]):
-            raise ValueError("Missing columns in predicted rating DataFrame")
         if not has_same_base_dtype(
             rating_true, rating_pred, columns=[col_user, col_item]
         ):
-            raise ValueError("Columns in provided DataFrames are not the same datatype")
+            raise ColumnTypeMismatchError(
+                "Columns in provided DataFrames are not the same datatype"
+            )
 
         return func(
             rating_true=rating_true,
             rating_pred=rating_pred,
             col_user=col_user,
             col_item=col_item,
-            col_rating=col_rating,
             col_prediction=col_prediction,
             *args,
-            **kwargs
+            **kwargs,
         )
 
     return check_column_dtypes_wrapper
 
 
 @_check_column_dtypes
 @lru_cache_df(maxsize=1)
@@ -346,28 +377,27 @@
 @_check_column_dtypes
 @lru_cache_df(maxsize=1)
 def merge_ranking_true_pred(
     rating_true,
     rating_pred,
     col_user,
     col_item,
-    col_rating,
     col_prediction,
     relevancy_method,
     k=DEFAULT_K,
     threshold=DEFAULT_THRESHOLD,
+    **_,
 ):
     """Filter truth and prediction data frames on common users
 
     Args:
         rating_true (pandas.DataFrame): True DataFrame
         rating_pred (pandas.DataFrame): Predicted DataFrame
         col_user (str): column name for user
         col_item (str): column name for item
-        col_rating (str): column name for rating
         col_prediction (str): column name for prediction
         relevancy_method (str): method for determining relevancy ['top_k', 'by_threshold', None]. None means that the
             top k items are directly provided, so there is no need to compute the relevancy operation.
         k (int): number of top k items per user (optional)
         threshold (float): threshold of top items per user (optional)
 
     Returns:
@@ -416,19 +446,19 @@
 
 
 def precision_at_k(
     rating_true,
     rating_pred,
     col_user=DEFAULT_USER_COL,
     col_item=DEFAULT_ITEM_COL,
-    col_rating=DEFAULT_RATING_COL,
     col_prediction=DEFAULT_PREDICTION_COL,
     relevancy_method="top_k",
     k=DEFAULT_K,
     threshold=DEFAULT_THRESHOLD,
+    **_,
 ):
     """Precision at K.
 
     Note:
         We use the same formula to calculate precision@k as that in Spark.
         More details can be found at
         http://spark.apache.org/docs/2.1.1/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.precisionAt
@@ -436,31 +466,28 @@
         user in rating_pred is less than k.
 
     Args:
         rating_true (pandas.DataFrame): True DataFrame
         rating_pred (pandas.DataFrame): Predicted DataFrame
         col_user (str): column name for user
         col_item (str): column name for item
-        col_rating (str): column name for rating
         col_prediction (str): column name for prediction
         relevancy_method (str): method for determining relevancy ['top_k', 'by_threshold', None]. None means that the
             top k items are directly provided, so there is no need to compute the relevancy operation.
         k (int): number of top k items per user
         threshold (float): threshold of top items per user (optional)
 
     Returns:
         float: precision at k (min=0, max=1)
     """
-
     df_hit, df_hit_count, n_users = merge_ranking_true_pred(
         rating_true=rating_true,
         rating_pred=rating_pred,
         col_user=col_user,
         col_item=col_item,
-        col_rating=col_rating,
         col_prediction=col_prediction,
         relevancy_method=relevancy_method,
         k=k,
         threshold=threshold,
     )
 
     if df_hit.shape[0] == 0:
@@ -470,67 +497,124 @@
 
 
 def recall_at_k(
     rating_true,
     rating_pred,
     col_user=DEFAULT_USER_COL,
     col_item=DEFAULT_ITEM_COL,
-    col_rating=DEFAULT_RATING_COL,
     col_prediction=DEFAULT_PREDICTION_COL,
     relevancy_method="top_k",
     k=DEFAULT_K,
     threshold=DEFAULT_THRESHOLD,
+    **_,
 ):
     """Recall at K.
 
     Args:
         rating_true (pandas.DataFrame): True DataFrame
         rating_pred (pandas.DataFrame): Predicted DataFrame
         col_user (str): column name for user
         col_item (str): column name for item
-        col_rating (str): column name for rating
         col_prediction (str): column name for prediction
         relevancy_method (str): method for determining relevancy ['top_k', 'by_threshold', None]. None means that the
             top k items are directly provided, so there is no need to compute the relevancy operation.
         k (int): number of top k items per user
         threshold (float): threshold of top items per user (optional)
 
     Returns:
         float: recall at k (min=0, max=1). The maximum value is 1 even when fewer than
         k items exist for a user in rating_true.
     """
-
     df_hit, df_hit_count, n_users = merge_ranking_true_pred(
         rating_true=rating_true,
         rating_pred=rating_pred,
         col_user=col_user,
         col_item=col_item,
-        col_rating=col_rating,
         col_prediction=col_prediction,
         relevancy_method=relevancy_method,
         k=k,
         threshold=threshold,
     )
 
     if df_hit.shape[0] == 0:
         return 0.0
 
     return (df_hit_count["hit"] / df_hit_count["actual"]).sum() / n_users
 
 
+def r_precision_at_k(
+    rating_true,
+    rating_pred,
+    col_user=DEFAULT_USER_COL,
+    col_item=DEFAULT_ITEM_COL,
+    col_prediction=DEFAULT_PREDICTION_COL,
+    relevancy_method="top_k",
+    k=DEFAULT_K,
+    threshold=DEFAULT_THRESHOLD,
+    **_,
+):
+    """R-precision at K.
+
+    R-precision can be defined as the precision@R for each user, where R is the
+    numer of relevant items for the query. Its also equivalent to the recall at
+    the R-th position.
+    
+    Note:
+        As R can be high, in this case, the k indicates the maximum possible R.
+        If every user has more than k true items, then r-precision@k is equal to
+        precision@k. You might need to raise the k value to get meaningful results.
+
+    Args:
+        rating_true (pandas.DataFrame): True DataFrame
+        rating_pred (pandas.DataFrame): Predicted DataFrame
+        col_user (str): column name for user
+        col_item (str): column name for item
+        col_prediction (str): column name for prediction
+        relevancy_method (str): method for determining relevancy ['top_k', 'by_threshold', None]. None means that the
+            top k items are directly provided, so there is no need to compute the relevancy operation.
+        k (int): number of top k items per user
+        threshold (float): threshold of top items per user (optional)
+
+    Returns:
+        float: recall at k (min=0, max=1). The maximum value is 1 even when fewer than
+        k items exist for a user in rating_true.
+    """
+    df_hit, df_hit_count, n_users = merge_ranking_true_pred(
+        rating_true=rating_true,
+        rating_pred=rating_pred,
+        col_user=col_user,
+        col_item=col_item,
+        col_prediction=col_prediction,
+        relevancy_method=relevancy_method,
+        k=k,
+        threshold=threshold,
+    )
+
+    if df_hit.shape[0] == 0:
+        return 0.0
+
+    df_merged = df_hit.merge(df_hit_count[[col_user, 'actual']])
+    df_merged = df_merged[df_merged['rank'] <= df_merged['actual']]
+
+    return (df_merged.groupby(col_user).size() / df_hit_count.set_index(col_user)['actual']).mean()
+
+
 def ndcg_at_k(
     rating_true,
     rating_pred,
     col_user=DEFAULT_USER_COL,
     col_item=DEFAULT_ITEM_COL,
     col_rating=DEFAULT_RATING_COL,
     col_prediction=DEFAULT_PREDICTION_COL,
     relevancy_method="top_k",
     k=DEFAULT_K,
     threshold=DEFAULT_THRESHOLD,
+    score_type="binary",
+    discfun_type="loge",
+    **_,
 ):
     """Normalized Discounted Cumulative Gain (nDCG).
 
     Info: https://en.wikipedia.org/wiki/Discounted_cumulative_gain
 
     Args:
         rating_true (pandas.DataFrame): True DataFrame
@@ -539,116 +623,219 @@
         col_item (str): column name for item
         col_rating (str): column name for rating
         col_prediction (str): column name for prediction
         relevancy_method (str): method for determining relevancy ['top_k', 'by_threshold', None]. None means that the
             top k items are directly provided, so there is no need to compute the relevancy operation.
         k (int): number of top k items per user
         threshold (float): threshold of top items per user (optional)
+        score_type (str): type of relevance scores ['binary', 'raw', 'exp']. With the default option 'binary', the
+            relevance score is reduced to either 1 (hit) or 0 (miss). Option 'raw' uses the raw relevance score.
+            Option 'exp' uses (2 ** RAW_RELEVANCE - 1) as the relevance score
+        discfun_type (str): type of discount function ['loge', 'log2'] used to calculate DCG.
 
     Returns:
         float: nDCG at k (min=0, max=1).
     """
-
-    df_hit, df_hit_count, n_users = merge_ranking_true_pred(
+    df_hit, _, _ = merge_ranking_true_pred(
         rating_true=rating_true,
         rating_pred=rating_pred,
         col_user=col_user,
         col_item=col_item,
-        col_rating=col_rating,
         col_prediction=col_prediction,
         relevancy_method=relevancy_method,
         k=k,
         threshold=threshold,
     )
 
     if df_hit.shape[0] == 0:
         return 0.0
 
-    # calculate discounted gain for hit items
-    df_dcg = df_hit.copy()
-    # relevance in this case is always 1
-    df_dcg["dcg"] = 1 / np.log1p(df_dcg["rank"])
-    # sum up discount gained to get discount cumulative gain
-    df_dcg = df_dcg.groupby(col_user, as_index=False, sort=False).agg({"dcg": "sum"})
-    # calculate ideal discounted cumulative gain
-    df_ndcg = pd.merge(df_dcg, df_hit_count, on=[col_user])
-    df_ndcg["idcg"] = df_ndcg["actual"].apply(
-        lambda x: sum(1 / np.log1p(range(1, min(x, k) + 1)))
+    df_dcg = df_hit.merge(rating_pred, on=[col_user, col_item]).merge(
+        rating_true, on=[col_user, col_item], how="outer", suffixes=("_left", None)
+    )
+
+    if score_type == "binary":
+        df_dcg["rel"] = 1
+    elif score_type == "raw":
+        df_dcg["rel"] = df_dcg[col_rating]
+    elif score_type == "exp":
+        df_dcg["rel"] = 2 ** df_dcg[col_rating] - 1
+    else:
+        raise ValueError("score_type must be one of 'binary', 'raw', 'exp'")
+
+    if discfun_type == "loge":
+        discfun = np.log
+    elif discfun_type == "log2":
+        discfun = np.log2
+    else:
+        raise ValueError("discfun_type must be one of 'loge', 'log2'")
+
+    # Calculate the actual discounted gain for each record
+    df_dcg["dcg"] = df_dcg["rel"] / discfun(1 + df_dcg["rank"])
+
+    # Calculate the ideal discounted gain for each record
+    df_idcg = df_dcg.sort_values([col_user, col_rating], ascending=False)
+    df_idcg["irank"] = df_idcg.groupby(col_user, as_index=False, sort=False)[
+        col_rating
+    ].rank("first", ascending=False)
+    df_idcg["idcg"] = df_idcg["rel"] / discfun(1 + df_idcg["irank"])
+
+    # Calculate the actual DCG for each user
+    df_user = df_dcg.groupby(col_user, as_index=False, sort=False).agg({"dcg": "sum"})
+
+    # Calculate the ideal DCG for each user
+    df_user = df_user.merge(
+        df_idcg.groupby(col_user, as_index=False, sort=False)
+        .head(k)
+        .groupby(col_user, as_index=False, sort=False)
+        .agg({"idcg": "sum"}),
+        on=col_user,
     )
 
     # DCG over IDCG is the normalized DCG
-    return (df_ndcg["dcg"] / df_ndcg["idcg"]).sum() / n_users
+    df_user["ndcg"] = df_user["dcg"] / df_user["idcg"]
+    return df_user["ndcg"].mean()
 
 
-def map_at_k(
+@lru_cache_df(maxsize=1)
+def _get_reciprocal_rank(
     rating_true,
     rating_pred,
     col_user=DEFAULT_USER_COL,
     col_item=DEFAULT_ITEM_COL,
-    col_rating=DEFAULT_RATING_COL,
     col_prediction=DEFAULT_PREDICTION_COL,
     relevancy_method="top_k",
     k=DEFAULT_K,
     threshold=DEFAULT_THRESHOLD,
 ):
-    """Mean Average Precision at k
+    df_hit, df_hit_count, n_users = merge_ranking_true_pred(
+        rating_true=rating_true,
+        rating_pred=rating_pred,
+        col_user=col_user,
+        col_item=col_item,
+        col_prediction=col_prediction,
+        relevancy_method=relevancy_method,
+        k=k,
+        threshold=threshold,
+    )
+
+    if df_hit.shape[0] == 0:
+        return None, n_users
+
+    # calculate reciprocal rank of items for each user and sum them up
+    df_hit_sorted = df_hit.copy()
+    df_hit_sorted["rr"] = (
+        df_hit_sorted.groupby(col_user).cumcount() + 1
+    ) / df_hit_sorted["rank"]
+    df_hit_sorted = df_hit_sorted.groupby(col_user).agg({"rr": "sum"}).reset_index()
+
+    return pd.merge(df_hit_sorted, df_hit_count, on=col_user), n_users
+
+
+def map(
+    rating_true,
+    rating_pred,
+    col_user=DEFAULT_USER_COL,
+    col_item=DEFAULT_ITEM_COL,
+    col_prediction=DEFAULT_PREDICTION_COL,
+    relevancy_method="top_k",
+    k=DEFAULT_K,
+    threshold=DEFAULT_THRESHOLD,
+    **_,
+):
+    """Mean Average Precision for top k prediction items
 
     The implementation of MAP is referenced from Spark MLlib evaluation metrics.
     https://spark.apache.org/docs/2.3.0/mllib-evaluation-metrics.html#ranking-systems
 
     A good reference can be found at:
     http://web.stanford.edu/class/cs276/handouts/EvaluationNew-handout-6-per.pdf
 
     Note:
-        1. The evaluation function is named as 'MAP is at k' because the evaluation class takes top k items for
-        the prediction items. The naming is different from Spark.
-
-        2. The MAP is meant to calculate Avg. Precision for the relevant items, so it is normalized by the number of
+        The MAP is meant to calculate Avg. Precision for the relevant items, so it is normalized by the number of
         relevant items in the ground truth data, instead of k.
 
     Args:
         rating_true (pandas.DataFrame): True DataFrame
         rating_pred (pandas.DataFrame): Predicted DataFrame
         col_user (str): column name for user
         col_item (str): column name for item
-        col_rating (str): column name for rating
         col_prediction (str): column name for prediction
         relevancy_method (str): method for determining relevancy ['top_k', 'by_threshold', None]. None means that the
             top k items are directly provided, so there is no need to compute the relevancy operation.
         k (int): number of top k items per user
         threshold (float): threshold of top items per user (optional)
 
     Returns:
-        float: MAP at k (min=0, max=1).
+        float: MAP (min=0, max=1)
     """
-
-    df_hit, df_hit_count, n_users = merge_ranking_true_pred(
+    df_merge, n_users = _get_reciprocal_rank(
         rating_true=rating_true,
         rating_pred=rating_pred,
         col_user=col_user,
         col_item=col_item,
-        col_rating=col_rating,
         col_prediction=col_prediction,
         relevancy_method=relevancy_method,
         k=k,
         threshold=threshold,
     )
 
-    if df_hit.shape[0] == 0:
+    if df_merge is None:
         return 0.0
+    else:
+        return (df_merge["rr"] / df_merge["actual"]).sum() / n_users
 
-    # calculate reciprocal rank of items for each user and sum them up
-    df_hit_sorted = df_hit.copy()
-    df_hit_sorted["rr"] = (
-        df_hit_sorted.groupby(col_user).cumcount() + 1
-    ) / df_hit_sorted["rank"]
-    df_hit_sorted = df_hit_sorted.groupby(col_user).agg({"rr": "sum"}).reset_index()
 
-    df_merge = pd.merge(df_hit_sorted, df_hit_count, on=col_user)
-    return (df_merge["rr"] / df_merge["actual"]).sum() / n_users
+def map_at_k(
+    rating_true,
+    rating_pred,
+    col_user=DEFAULT_USER_COL,
+    col_item=DEFAULT_ITEM_COL,
+    col_prediction=DEFAULT_PREDICTION_COL,
+    relevancy_method="top_k",
+    k=DEFAULT_K,
+    threshold=DEFAULT_THRESHOLD,
+    **_,
+):
+    """Mean Average Precision at k
+
+    The implementation of MAP@k is referenced from Spark MLlib evaluation metrics.
+    https://github.com/apache/spark/blob/b938ff9f520fd4e4997938284ffa0aba9ea271fc/mllib/src/main/scala/org/apache/spark/mllib/evaluation/RankingMetrics.scala#L99
+
+    Args:
+        rating_true (pandas.DataFrame): True DataFrame
+        rating_pred (pandas.DataFrame): Predicted DataFrame
+        col_user (str): column name for user
+        col_item (str): column name for item
+        col_prediction (str): column name for prediction
+        relevancy_method (str): method for determining relevancy ['top_k', 'by_threshold', None]. None means that the
+            top k items are directly provided, so there is no need to compute the relevancy operation.
+        k (int): number of top k items per user
+        threshold (float): threshold of top items per user (optional)
+
+    Returns:
+        float: MAP@k (min=0, max=1)
+    """
+    df_merge, n_users = _get_reciprocal_rank(
+        rating_true=rating_true,
+        rating_pred=rating_pred,
+        col_user=col_user,
+        col_item=col_item,
+        col_prediction=col_prediction,
+        relevancy_method=relevancy_method,
+        k=k,
+        threshold=threshold,
+    )
+
+    if df_merge is None:
+        return 0.0
+    else:
+        return (
+            df_merge["rr"] / df_merge["actual"].apply(lambda x: min(x, k))
+        ).sum() / n_users
 
 
 def get_top_k_items(
     dataframe, col_user=DEFAULT_USER_COL, col_rating=DEFAULT_RATING_COL, k=DEFAULT_K
 ):
     """Get the input customer-item-rating tuple in the format of Pandas
     DataFrame, output a Pandas DataFrame in the dense format of top k items
@@ -690,16 +877,18 @@
 metrics = {
     rmse.__name__: rmse,
     mae.__name__: mae,
     rsquared.__name__: rsquared,
     exp_var.__name__: exp_var,
     precision_at_k.__name__: precision_at_k,
     recall_at_k.__name__: recall_at_k,
+    r_precision_at_k.__name__: r_precision_at_k,
     ndcg_at_k.__name__: ndcg_at_k,
     map_at_k.__name__: map_at_k,
+    map.__name__: map,
 }
 
 
 # diversity metrics
 def _check_column_dtypes_diversity_serendipity(func):
     """Checks columns of DataFrame inputs
 
@@ -726,15 +915,15 @@
         item_sim_measure=DEFAULT_ITEM_SIM_MEASURE,
         col_item_features=DEFAULT_ITEM_FEATURES_COL,
         col_user=DEFAULT_USER_COL,
         col_item=DEFAULT_ITEM_COL,
         col_sim=DEFAULT_SIMILARITY_COL,
         col_relevance=None,
         *args,
-        **kwargs
+        **kwargs,
     ):
         """Check columns of DataFrame inputs
 
         Args:
             train_df (pandas.DataFrame): Data set with historical data for users and items they
                 have interacted with; contains col_user, col_item. Assumed to not contain any duplicate rows.
             reco_df (pandas.DataFrame): Recommender's prediction output, containing col_user, col_item,
@@ -793,15 +982,15 @@
             item_feature_df=item_feature_df,
             item_sim_measure=item_sim_measure,
             col_user=col_user,
             col_item=col_item,
             col_sim=col_sim,
             col_relevance=col_relevance,
             *args,
-            **kwargs
+            **kwargs,
         )
 
     return check_column_dtypes_diversity_serendipity_wrapper
 
 
 def _check_column_dtypes_novelty_coverage(func):
     """Checks columns of DataFrame inputs
@@ -822,15 +1011,15 @@
     @wraps(func)
     def check_column_dtypes_novelty_coverage_wrapper(
         train_df,
         reco_df,
         col_user=DEFAULT_USER_COL,
         col_item=DEFAULT_ITEM_COL,
         *args,
-        **kwargs
+        **kwargs,
     ):
         """Check columns of DataFrame inputs
 
         Args:
             train_df (pandas.DataFrame): Data set with historical data for users and items they
                 have interacted with; contains col_user, col_item. Assumed to not contain any duplicate rows.
                 Interaction here follows the *item choice model* from Castells et al.
@@ -858,15 +1047,15 @@
 
         return func(
             train_df=train_df,
             reco_df=reco_df,
             col_user=col_user,
             col_item=col_item,
             *args,
-            **kwargs
+            **kwargs,
         )
 
     return check_column_dtypes_novelty_coverage_wrapper
 
 
 @lru_cache_df(maxsize=1)
 def _get_pairwise_items(
@@ -895,15 +1084,14 @@
     item_feature_df=None,
     item_sim_measure=DEFAULT_ITEM_SIM_MEASURE,
     col_item_features=DEFAULT_ITEM_FEATURES_COL,
     col_user=DEFAULT_USER_COL,
     col_item=DEFAULT_ITEM_COL,
     col_sim=DEFAULT_SIMILARITY_COL,
 ):
-
     if item_sim_measure == "item_cooccurrence_count":
         # calculate item-item similarity based on item co-occurrence count
         df_cosine_similarity = _get_cooccurrence_similarity(
             train_df, col_user, col_item, col_sim
         )
     elif item_sim_measure == "item_feature_vector":
         # calculdf_cosine_similarity = ate item-item similarity based on item feature vectors
```

### Comparing `recommenders-1.1.1/recommenders/evaluation/spark_evaluation.py` & `recommenders-1.2.0/recommenders/evaluation/spark_evaluation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 
 try:
     from pyspark.mllib.evaluation import RegressionMetrics, RankingMetrics
     from pyspark.sql import Window, DataFrame
@@ -146,26 +146,28 @@
             float: R squared.
         """
         return self.metrics.r2
 
     def exp_var(self):
         """Calculate explained variance.
 
-        .. note::
+        Note:
            Spark MLLib's implementation is buggy (can lead to values > 1), hence we use var().
 
         Returns:
             float: Explained variance (min=0, max=1).
         """
-        var1 = self.y_pred_true.selectExpr("variance(label - prediction)").collect()[0][
-            0
-        ]
+        var1 = self.y_pred_true.selectExpr("variance(label-prediction)").collect()[0][0]
         var2 = self.y_pred_true.selectExpr("variance(label)").collect()[0][0]
-        # numpy divide is more tolerant to var2 being zero
-        return 1 - np.divide(var1, var2)
+
+        if var1 is None or var2 is None:
+            return -np.inf
+        else:
+            # numpy divide is more tolerant to var2 being zero
+            return 1 - np.divide(var1, var2)
 
 
 class SparkRankingEvaluation:
     """Spark Ranking Evaluator"""
 
     def __init__(
         self,
@@ -181,15 +183,15 @@
     ):
         """Initialization.
         This is the Spark version of ranking metrics evaluator.
         The methods of this class, calculate ranking metrics such as precision@k, recall@k, ndcg@k, and mean average
         precision.
 
         The implementations of precision@k, ndcg@k, and mean average precision are referenced from Spark MLlib, which
-        can be found at `here <https://spark.apache.org/docs/2.3.0/mllib-evaluation-metrics.html#ranking-systems>`_.
+        can be found at `the link <https://spark.apache.org/docs/2.3.0/mllib-evaluation-metrics.html#ranking-systems>`_.
 
         Args:
             rating_true (pyspark.sql.DataFrame): DataFrame of true rating data (in the
                 format of customerID-itemID-rating tuple).
             rating_pred (pyspark.sql.DataFrame): DataFrame of predicted rating data (in
                 the format of customerID-itemID-rating tuple).
             col_user (str): column name for user.
@@ -197,15 +199,15 @@
             col_rating (str): column name for rating.
             col_prediction (str): column name for prediction.
             k (int): number of items to recommend to each user.
             relevancy_method (str): method for determining relevant items. Possible
                 values are "top_k", "by_time_stamp", and "by_threshold".
             threshold (float): threshold for determining the relevant recommended items.
                 This is used for the case that predicted ratings follow a known
-                distribution. NOTE: this option is only activated if relevancy_method is
+                distribution. NOTE: this option is only activated if `relevancy_method` is
                 set to "by_threshold".
         """
         self.rating_true = rating_true
         self.rating_pred = rating_pred
         self.col_user = col_user
         self.col_item = col_item
         self.col_rating = col_rating
@@ -298,87 +300,80 @@
         ).drop(self.col_user)
 
         return RankingMetrics(self._items_for_user_all.rdd)
 
     def precision_at_k(self):
         """Get precision@k.
 
-        .. note::
+        Note:
             More details can be found
-            `here <http://spark.apache.org/docs/2.1.1/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.precisionAt>`_.
+            `on the precisionAt PySpark documentation <http://spark.apache.org/docs/3.0.0/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.precisionAt>`_.
 
         Return:
             float: precision at k (min=0, max=1)
         """
-        precision = self._metrics.precisionAt(self.k)
-
-        return precision
+        return self._metrics.precisionAt(self.k)
 
     def recall_at_k(self):
         """Get recall@K.
 
-        .. note::
+        Note:
             More details can be found
-            `here <http://spark.apache.org/docs/2.1.1/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.meanAveragePrecision>`_.
+            `on the recallAt PySpark documentation <http://spark.apache.org/docs/3.0.0/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.recallAt>`_.
 
         Return:
             float: recall at k (min=0, max=1).
         """
-        df_hit = self._items_for_user_all.withColumn(
-            "hit", F.array_intersect(DEFAULT_PREDICTION_COL, "ground_truth")
-        )
-        df_hit = df_hit.withColumn("num_hit", F.size("hit"))
-        df_hit = df_hit.withColumn("num_actual", F.size("ground_truth"))
-        df_hit = df_hit.withColumn("per_hit", df_hit["num_hit"] / df_hit["num_actual"])
-        recall = df_hit.select(F.mean("per_hit")).collect()[0][0]
-
-        return recall
+        return self._metrics.recallAt(self.k)
 
     def ndcg_at_k(self):
         """Get Normalized Discounted Cumulative Gain (NDCG)
 
-        .. note::
+        Note:
             More details can be found
-            `here <http://spark.apache.org/docs/2.1.1/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.ndcgAt>`_.
+            `on the ndcgAt PySpark documentation <http://spark.apache.org/docs/3.0.0/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.ndcgAt>`_.
 
         Return:
             float: nDCG at k (min=0, max=1).
         """
-        ndcg = self._metrics.ndcgAt(self.k)
+        return self._metrics.ndcgAt(self.k)
+
+    def map(self):
+        """Get mean average precision.
 
-        return ndcg
+        Return:
+            float: MAP (min=0, max=1).
+        """
+        return self._metrics.meanAveragePrecision
 
     def map_at_k(self):
         """Get mean average precision at k.
 
-        .. note::
-            More details can be found
-            `here <http://spark.apache.org/docs/2.1.1/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.meanAveragePrecision>`_.
+        Note:
+            More details `on the meanAveragePrecision PySpark documentation <http://spark.apache.org/docs/3.0.0/api/python/pyspark.mllib.html#pyspark.mllib.evaluation.RankingMetrics.meanAveragePrecision>`_.
 
         Return:
             float: MAP at k (min=0, max=1).
         """
-        maprecision = self._metrics.meanAveragePrecision
-
-        return maprecision
+        return self._metrics.meanAveragePrecisionAt(self.k)
 
 
 def _get_top_k_items(
     dataframe,
     col_user=DEFAULT_USER_COL,
     col_item=DEFAULT_ITEM_COL,
     col_rating=DEFAULT_RATING_COL,
     col_prediction=DEFAULT_PREDICTION_COL,
     k=DEFAULT_K,
 ):
     """Get the input customer-item-rating tuple in the format of Spark
     DataFrame, output a Spark DataFrame in the dense format of top k items
     for each user.
 
-    .. note::
+    Note:
         if it is implicit rating, just append a column of constants to be ratings.
 
     Args:
         dataframe (pyspark.sql.DataFrame): DataFrame of rating data (in the format of
         customerID-itemID-rating tuple).
         col_user (str): column name for user.
         col_item (str): column name for item.
@@ -464,15 +459,15 @@
         dataframe (pyspark.sql.DataFrame): A Spark DataFrame of customerID-itemID-rating-timeStamp
             tuples.
         col_user (str): column name for user.
         col_item (str): column name for item.
         col_rating (str): column name for rating.
         col_timestamp (str): column name for timestamp.
         col_prediction (str): column name for prediction.
-        k: number of relevent items to be filtered by the function.
+        k: number of relevant items to be filtered by the function.
 
     Return:
         pyspark.sql.DataFrame: DataFrame of customerID-itemID-rating tuples with only relevant items.
     """
     window_spec = Window.partitionBy(col_user).orderBy(col(col_timestamp).desc())
 
     items_for_user = (
@@ -526,15 +521,15 @@
 
             Y.C. Zhang, D.Ó. Séaghdha, D. Quercia and T. Jambor, Auralist: introducing
             serendipity into music recommendation, WSDM 2012
 
             P. Castells, S. Vargas, and J. Wang, Novelty and diversity metrics for recommender systems:
             choice, discovery and relevance, ECIR 2011
 
-            Eugene Yan, Serendipity: Accuracy’s unpopular best friend in Recommender Systems,
+            Eugene Yan, Serendipity: Accuracy's unpopular best friend in Recommender Systems,
             eugeneyan.com, April 2020
 
         Args:
             train_df (pyspark.sql.DataFrame): Data set with historical data for users and items they
                 have interacted with; contains col_user, col_item. Assumed to not contain any duplicate rows.
                 Interaction here follows the *item choice model* from Castells et al.
             reco_df (pyspark.sql.DataFrame): Recommender's prediction output, containing col_user, col_item,
@@ -582,25 +577,24 @@
             required_schema = StructType(
                 (
                     StructField(self.col_item, IntegerType()),
                     StructField(self.col_item_features, VectorUDT()),
                 )
             )
             if self.item_feature_df is not None:
-
                 if str(required_schema) != str(item_feature_df.schema):
                     raise Exception(
-                        "Incorrect schema! item_feature_df should have schema:"
-                        + str(required_schema)
+                        "Incorrect schema! item_feature_df should have schema "
+                        f"{str(required_schema)} but have {str(item_feature_df.schema)}"
                     )
             else:
                 raise Exception(
                     "item_feature_df not specified! item_feature_df must be provided "
                     "if choosing to use item_feature_vector to calculate item similarity. "
-                    "item_feature_df should have schema:" + str(required_schema)
+                    f"item_feature_df should have schema {str(required_schema)}"
                 )
 
         # check if reco_df contains any user_item pairs that are already shown in train_df
         count_intersection = (
             self.train_df.select(self.col_user, self.col_item)
             .intersect(self.reco_df.select(self.col_user, self.col_item))
             .count()
@@ -622,15 +616,14 @@
                 ),
                 (F.col(self.col_user) == F.col("_user")) & (F.col("i1") <= F.col("i2")),
             )
             .select(self.col_user, "i1", "i2")
         )
 
     def _get_cosine_similarity(self, n_partitions=200):
-
         if self.item_sim_measure == "item_cooccurrence_count":
             # calculate item-item similarity based on item co-occurrence count
             self._get_cooccurrence_similarity(n_partitions)
         elif self.item_sim_measure == "item_feature_vector":
             # calculate item-item similarity based on item feature vectors
             self._get_item_feature_similarity(n_partitions)
         else:
```

### Comparing `recommenders-1.1.1/recommenders/models/cornac/cornac_utils.py` & `recommenders-1.2.0/recommenders/models/cornac/cornac_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import pandas as pd
 import numpy as np
 
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/DataModel/ImplicitCF.py` & `recommenders-1.2.0/recommenders/models/deeprec/DataModel/ImplicitCF.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import random
 import numpy as np
 import pandas as pd
 import scipy.sparse as sp
 
@@ -66,15 +66,19 @@
             test (pandas.DataFrame): Test data with at least columns (col_user, col_item, col_rating).
                 test can be None, if so, we only process the training data.
 
         Returns:
             list: train and test pandas.DataFrame Dataset, which have been reindexed and filtered.
 
         """
-        df = train if test is None else train.append(test)
+        df = (
+            train
+            if test is None
+            else pd.concat([train, test], axis=0, ignore_index=True)
+        )
 
         if self.user_idx is None:
             user_idx = df[[self.col_user]].drop_duplicates().reindex()
             user_idx[self.col_user + "_idx"] = np.arange(len(user_idx))
             self.n_users = len(user_idx)
             self.user_idx = user_idx
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/deeprec_utils.py` & `recommenders-1.2.0/recommenders/models/deeprec/deeprec_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 import os
 from sklearn.metrics import (
     roc_auc_score,
     log_loss,
@@ -180,15 +180,15 @@
             "layer_sizes",
             "cross_layer_sizes",
             "activation",
             "loss",
             "data_format",
             "dropout",
         ]
-    if f_config["model_type"] in ["gru4rec", "GRU4REC", "GRU4Rec"]:
+    if f_config["model_type"] in ["gru", "GRU"]:
         required_parameters = [
             "item_embedding_dim",
             "cate_embedding_dim",
             "max_seq_length",
             "loss",
             "method",
             "user_vocab",
@@ -502,15 +502,15 @@
 
     Returns:
         np.ndarray: dcg scores.
     """
     k = min(np.shape(y_true)[-1], k)
     order = np.argsort(y_score)[::-1]
     y_true = np.take(y_true, order[:k])
-    gains = 2 ** y_true - 1
+    gains = 2**y_true - 1
     discounts = np.log2(np.arange(len(y_true)) + 2)
     return np.sum(gains / discounts)
 
 
 def cal_metric(labels, preds, metrics):
     """Calculate metrics.
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/io/dkn_item2item_iterator.py` & `recommenders-1.2.0/recommenders/models/deeprec/io/dkn_item2item_iterator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 import tensorflow as tf
 from recommenders.models.deeprec.io.dkn_iterator import DKNTextIterator
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/io/dkn_iterator.py` & `recommenders-1.2.0/recommenders/models/deeprec/io/dkn_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 import numpy as np
 
 from recommenders.models.deeprec.io.iterator import BaseIterator
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/io/iterator.py` & `recommenders-1.2.0/recommenders/models/deeprec/io/iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import tensorflow as tf
 import abc
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/io/nextitnet_iterator.py` & `recommenders-1.2.0/recommenders/models/deeprec/io/nextitnet_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 import numpy as np
 import random
 
 from recommenders.models.deeprec.io.sequential_iterator import SequentialIterator
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/io/sequential_iterator.py` & `recommenders-1.2.0/recommenders/models/deeprec/io/sequential_iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 import numpy as np
 import random
 
 from recommenders.models.deeprec.io.iterator import BaseIterator
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/base_model.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 from os.path import join
 import abc
 import time
 import os
 import numpy as np
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/dkn.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/dkn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import tensorflow as tf
 
 from recommenders.models.deeprec.models.base_model import BaseModel
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/dkn_item2item.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/dkn_item2item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-
 import numpy as np
 import tensorflow as tf
 from recommenders.models.deeprec.models.dkn import DKN
 from recommenders.models.deeprec.deeprec_utils import cal_metric
 
-
-r"""
+"""
 This new model adapts DKN's structure for item-to-item recommendations.
 The tutorial can be found at: https://github.com/microsoft/recommenders/blob/main/examples/07_tutorials/KDD2020-tutorial/step4_run_dkn_item2item.ipynb
  """
 
 
 class DKNItem2Item(DKN):
     """Class for item-to-item recommendations using DKN.
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/graphrec/lightgcn.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/graphrec/lightgcn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 import time
 import os
 import sys
 import numpy as np
@@ -295,37 +295,21 @@
         """
         topk_scores = self.recommend_k_items(
             self.data.test, top_k=self.top_k, use_id=True
         )
         ret = []
         for metric in self.metrics:
             if metric == "map":
-                ret.append(
-                    map_at_k(
-                        self.data.test, topk_scores, relevancy_method=None, k=self.top_k
-                    )
-                )
+                ret.append(map_at_k(self.data.test, topk_scores, k=self.top_k))
             elif metric == "ndcg":
-                ret.append(
-                    ndcg_at_k(
-                        self.data.test, topk_scores, relevancy_method=None, k=self.top_k
-                    )
-                )
+                ret.append(ndcg_at_k(self.data.test, topk_scores, k=self.top_k))
             elif metric == "precision":
-                ret.append(
-                    precision_at_k(
-                        self.data.test, topk_scores, relevancy_method=None, k=self.top_k
-                    )
-                )
+                ret.append(precision_at_k(self.data.test, topk_scores, k=self.top_k))
             elif metric == "recall":
-                ret.append(
-                    recall_at_k(
-                        self.data.test, topk_scores, relevancy_method=None, k=self.top_k
-                    )
-                )
+                ret.append(recall_at_k(self.data.test, topk_scores, k=self.top_k))
         return ret
 
     def score(self, user_ids, remove_seen=True):
         """Score all items for test users.
 
         Args:
             user_ids (np.array): Users to test.
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/asvd.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/asvd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 from recommenders.models.deeprec.models.sequential.sequential_base_model import (
     SequentialBaseModel,
 )
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/caser.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/caser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 from recommenders.models.deeprec.models.sequential.sequential_base_model import (
     SequentialBaseModel,
 )
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/gru4rec.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/gru.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 from keras.layers.legacy_rnn.rnn_cell_impl import GRUCell, LSTMCell
 from recommenders.models.deeprec.models.sequential.sequential_base_model import (
     SequentialBaseModel,
 )
 from tensorflow.compat.v1.nn import dynamic_rnn
 
-__all__ = ["GRU4RecModel"]
+__all__ = ["GRUModel"]
 
 
-class GRU4RecModel(SequentialBaseModel):
-    """GRU4Rec Model
+class GRUModel(SequentialBaseModel):
+    """GRU Model
 
     :Citation:
 
-        B. Hidasi, A. Karatzoglou, L. Baltrunas, D. Tikk, "Session-based Recommendations
-        with Recurrent Neural Networks", ICLR (Poster), 2016.
+        Kyunghyun Cho, Bart van Merrienboer, Caglar Gulcehre, Dzmitry Bahdanau, 
+        Fethi Bougares, Holger Schwenk, and Yoshua Bengio. Learning Phrase 
+        Representations using RNN Encoder-Decoder for Statistical Machine Translation. 
+        arXiv preprint arXiv:1406.1078. 2014.
     """
 
     def _build_seq_graph(self):
-        """The main function to create GRU4Rec model.
+        """The main function to create GRU model.
 
         Returns:
-            object:the output of GRU4Rec section.
+            object:the output of GRU section.
         """
-        with tf.compat.v1.variable_scope("gru4rec"):
+        with tf.compat.v1.variable_scope("gru"):
             # final_state = self._build_lstm()
             final_state = self._build_gru()
             model_output = tf.concat([final_state, self.target_item_embedding], 1)
             tf.compat.v1.summary.histogram("model_output", model_output)
             return model_output
 
     def _build_lstm(self):
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/nextitnet.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/nextitnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 from recommenders.models.deeprec.models.sequential.sequential_base_model import (
     SequentialBaseModel,
 )
 
@@ -12,16 +12,15 @@
 class NextItNetModel(SequentialBaseModel):
     """NextItNet Model
 
     :Citation:
         Yuan, Fajie, et al. "A Simple Convolutional Generative Network
         for Next Item Recommendation", in Web Search and Data Mining, 2019.
 
-    .. note::
-
+    Note:
         It requires strong sequence with dataset.
     """
 
     def _build_seq_graph(self):
         """The main function to create nextitnet model.
 
         Returns:
@@ -41,15 +40,14 @@
             true_fn=lambda: self.cate_history_embedding[
                 :: self.hparams.train_num_ngs + 1
             ],
             false_fn=lambda: self.cate_history_embedding,
         )
 
         with tf.compat.v1.variable_scope("nextitnet", reuse=tf.compat.v1.AUTO_REUSE):
-
             dilate_input = tf.concat(
                 [item_history_embedding, cate_history_embedding], 2
             )
 
             for layer_id, dilation in enumerate(hparams.dilations):
                 dilate_input = tf.cond(
                     pred=is_training,
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/rnn_cell_implement.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/rnn_cell_implement.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         num_unit_shards=None,
         num_proj_shards=None,
         forget_bias=1.0,
         state_is_tuple=True,
         activation=None,
         reuse=None,
     ):
-
         super(Time4LSTMCell, self).__init__(_reuse=reuse)
         if not state_is_tuple:
             logging.warn(
                 "%s: Using a concatenated state is slower and will soon be "
                 "deprecated.  Use state_is_tuple=True.",
                 self,
             )
@@ -123,14 +122,25 @@
         return self._state_size
 
     @property
     def output_size(self):
         return self._output_size
 
     def call(self, inputs, state):
+        """Call method for the Time4LSTMCell.
+
+        Args:
+            inputs: A 2D Tensor of shape [batch_size, input_size].
+            state: A 2D Tensor of shape [batch_size, state_size].
+
+        Returns:
+            A tuple containing:
+            - A 2D Tensor of shape [batch_size, output_size].
+            - A 2D Tensor of shape [batch_size, state_size].
+        """
         time_now_score = tf.expand_dims(inputs[:, -1], -1)
         time_last_score = tf.expand_dims(inputs[:, -2], -1)
         inputs = inputs[:, :-2]
         num_proj = self._num_units if self._num_proj is None else self._num_proj
         sigmoid = math_ops.sigmoid
 
         if self._state_is_tuple:
@@ -310,15 +320,14 @@
         num_unit_shards=None,
         num_proj_shards=None,
         forget_bias=1.0,
         state_is_tuple=True,
         activation=None,
         reuse=None,
     ):
-
         super(Time4ALSTMCell, self).__init__(_reuse=reuse)
         if not state_is_tuple:
             logging.warn(
                 "%s: Using a concatenated state is slower and will soon be "
                 "deprecated.  Use state_is_tuple=True.",
                 self,
             )
@@ -378,14 +387,25 @@
         return self._state_size
 
     @property
     def output_size(self):
         return self._output_size
 
     def call(self, inputs, state):
+        """Call method for the Time4ALSTMCell.
+
+        Args:
+            inputs: A 2D Tensor of shape [batch_size, input_size].
+            state: A 2D Tensor of shape [batch_size, state_size].
+
+        Returns:
+            A tuple containing:
+            - A 2D Tensor of shape [batch_size, output_size].
+            - A 2D Tensor of shape [batch_size, state_size].
+        """
         att_score = tf.expand_dims(inputs[:, -1], -1)
         time_now_score = tf.expand_dims(inputs[:, -2], -1)
         time_last_score = tf.expand_dims(inputs[:, -3], -1)
         inputs = inputs[:, :-3]
         num_proj = self._num_units if self._num_proj is None else self._num_proj
         sigmoid = math_ops.sigmoid
 
@@ -577,17 +597,17 @@
         output_size,
         build_bias,
         bias_initializer=None,
         kernel_initializer=None,
     ):
         self._build_bias = build_bias
 
-        if args is None or (nest.is_sequence(args) and not args):
+        if args is None or (nest.is_nested(args) and not args):
             raise ValueError("`args` must be specified")
-        if not nest.is_sequence(args):
+        if not nest.is_nested(args):
             args = [args]
             self._is_sequence = False
         else:
             self._is_sequence = True
 
         # Calculate the total size of arguments on dimension 1.
         total_arg_size = 0
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/sequential_base_model.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/sequential_base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 import os
 import abc
 import numpy as np
 import tensorflow as tf
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/sli_rec.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/sli_rec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 from recommenders.models.deeprec.models.sequential.sequential_base_model import (
     SequentialBaseModel,
 )
 from tensorflow.compat.v1.nn import dynamic_rnn
@@ -123,14 +123,14 @@
             last_hidden_nn_layer = tf.concat(
                 [att_inputs, queries, att_inputs - queries, att_inputs * queries], -1
             )
             att_fnc_output = self._fcn_net(
                 last_hidden_nn_layer, hparams.att_fcn_layer_sizes, scope="att_fcn"
             )
             att_fnc_output = tf.squeeze(att_fnc_output, -1)
-            mask_paddings = tf.ones_like(att_fnc_output) * (-(2 ** 32) + 1)
+            mask_paddings = tf.ones_like(att_fnc_output) * (-(2**32) + 1)
             att_weights = tf.nn.softmax(
                 tf.compat.v1.where(boolean_mask, att_fnc_output, mask_paddings),
                 name="att_weights",
             )
             output = user_embedding * tf.expand_dims(att_weights, -1)
             return output
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/sum.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/sum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 from tensorflow.compat.v1.nn import dynamic_rnn
 from recommenders.models.deeprec.models.sequential.sequential_base_model import (
     SequentialBaseModel,
 )
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/sequential/sum_cells.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/sequential/sum_cells.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import tensorflow as tf
 from keras.layers.legacy_rnn.rnn_cell_impl import LayerRNNCell
 from tensorflow.python.eager import context
 from tensorflow.python.keras import activations
```

### Comparing `recommenders-1.1.1/recommenders/models/deeprec/models/xDeepFM.py` & `recommenders-1.2.0/recommenders/models/deeprec/models/xDeepFM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import tensorflow as tf
 
 from recommenders.models.deeprec.models.base_model import BaseModel
```

### Comparing `recommenders-1.1.1/recommenders/models/fastai/fastai_utils.py` & `recommenders-1.2.0/recommenders/models/fastai/fastai_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 import numpy as np
 import pandas as pd
 import fastai
 import fastprogress
+import torch
 from fastprogress.fastprogress import force_console_behavior
 
 from recommenders.utils import constants as cc
 
 
 def cartesian_product(*arrays):
     """Compute the Cartesian product in fastai algo. This is a helper function.
@@ -47,37 +48,45 @@
         prediction_col (str): Prediction column name.
         top_k (int): Number of top items to recommend.
 
     Returns:
         pandas.DataFrame: Result of recommendation
     """
     # replace values not known to the model with NaN
-    total_users, total_items = learner.data.train_ds.x.classes.values()
+    total_users, total_items = learner.dls.classes.values()
     test_df.loc[~test_df[user_col].isin(total_users), user_col] = np.nan
     test_df.loc[~test_df[item_col].isin(total_items), item_col] = np.nan
 
     # map ids to embedding ids
-    u = learner.get_idx(test_df[user_col], is_item=False)
-    m = learner.get_idx(test_df[item_col], is_item=True)
+    u = learner._get_idx(test_df[user_col], is_item=False)
+    m = learner._get_idx(test_df[item_col], is_item=True)
 
     # score the pytorch model
-    pred = learner.model.forward(u, m)
+    x = torch.column_stack((u, m))
+
+    if torch.cuda.is_available():
+        x = x.to("cuda")
+        learner.model = learner.model.to("cuda")
+
+    pred = learner.model.forward(x).detach().cpu().numpy()
     scores = pd.DataFrame(
         {user_col: test_df[user_col], item_col: test_df[item_col], prediction_col: pred}
     )
     scores = scores.sort_values([user_col, prediction_col], ascending=[True, False])
+
     if top_k is not None:
         top_scores = scores.groupby(user_col).head(top_k).reset_index(drop=True)
     else:
         top_scores = scores
+
     return top_scores
 
 
 def hide_fastai_progress_bar():
     """Hide fastai progress bar"""
     fastprogress.fastprogress.NO_BAR = True
     fastprogress.fastprogress.WRITER_FN = str
     master_bar, progress_bar = force_console_behavior()
-    fastai.basic_train.master_bar, fastai.basic_train.progress_bar = (
+    fastai.callback.progress.master_bar, fastai.callback.progress.progress_bar = (
         master_bar,
         progress_bar,
     )
```

### Comparing `recommenders-1.1.1/recommenders/models/geoimc/geoimc_algorithm.py` & `recommenders-1.2.0/recommenders/models/geoimc/geoimc_algorithm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 """
 Module maintaining the IMC problem.
 """
 
 import numpy as np
@@ -76,15 +76,15 @@
             the cost needs to be evaluated.
             residual_global (csr_matrix): Residual matrix.
         """
         U = params[0]
         B = params[1]
         V = params[2]
 
-        regularizer = 0.5 * self.lambda1 * np.sum(B ** 2)
+        regularizer = 0.5 * self.lambda1 * np.sum(B**2)
 
         IMCProblem._computeLoss_csrmatrix(
             self.X.dot(U.dot(B)),
             V.T.dot(self.Z.T),
             self.Y.data,
             self.Y.indices,
             self.Y.indptr,
```

### Comparing `recommenders-1.1.1/recommenders/models/geoimc/geoimc_data.py` & `recommenders-1.2.0/recommenders/models/geoimc/geoimc_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import logging
 import pandas as pd
 import numpy as np
 from scipy.sparse import coo_matrix, isspmatrix_csr
 from sklearn.model_selection import train_test_split
```

### Comparing `recommenders-1.1.1/recommenders/models/geoimc/geoimc_predict.py` & `recommenders-1.2.0/recommenders/models/geoimc/geoimc_predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 from scipy.linalg import sqrtm
 
 from recommenders.utils.python_utils import binarize as conv_binary
```

### Comparing `recommenders-1.1.1/recommenders/models/geoimc/geoimc_utils.py` & `recommenders-1.2.0/recommenders/models/geoimc/geoimc_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 from sklearn.decomposition import PCA
 
 
 def length_normalize(matrix):
@@ -10,15 +10,15 @@
 
     Args:
         matrix (np.ndarray): Input matrix that needs to be normalized
 
     Returns:
         Normalized matrix
     """
-    norms = np.sqrt(np.sum(matrix ** 2, axis=1))
+    norms = np.sqrt(np.sum(matrix**2, axis=1))
     norms[norms == 0] = 1
     return matrix / norms[:, np.newaxis]
 
 
 def mean_center(matrix):
     """Performs mean centering across axis 0
```

### Comparing `recommenders-1.1.1/recommenders/models/lightfm/lightfm_utils.py` & `recommenders-1.2.0/recommenders/models/lightfm/lightfm_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import pandas as pd
 import numpy as np
 import seaborn as sns
 
 from lightfm.evaluation import precision_at_k, recall_at_k
```

### Comparing `recommenders-1.1.1/recommenders/models/lightgbm/lightgbm_utils.py` & `recommenders-1.2.0/recommenders/models/lightgbm/lightgbm_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import logging
 import numpy as np
 import category_encoders as ce
 from tqdm import tqdm
 import collections
```

### Comparing `recommenders-1.1.1/recommenders/models/ncf/dataset.py` & `recommenders-1.2.0/recommenders/models/ncf/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Copyright (c) Recommenders contributors.
+# Licensed under the MIT License.
+
 import os
 from collections import OrderedDict
 import random
 import numpy as np
 import pandas as pd
 import csv
 import logging
@@ -187,15 +190,17 @@
         """
         records = []
         key_col = self.col_user if by_user else self.col_test_batch
 
         # fast forward in file to user/test batch
         while (self.line_num == 0) or (self.row[key_col] != key):
             if self.end_of_file:
-                raise MissingUserException("User {} not in file {}".format(key, self.filename))
+                raise MissingUserException(
+                    "User {} not in file {}".format(key, self.filename)
+                )
             next(self)
         # collect user/test batch data
         while self.row[key_col] == key:
             row = self.row
             if self.col_test_batch in row:
                 del row[self.col_test_batch]
             records.append(row)
```

### Comparing `recommenders-1.1.1/recommenders/models/ncf/ncf_singlenode.py` & `recommenders-1.2.0/recommenders/models/ncf/ncf_singlenode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import numpy as np
 import tensorflow as tf
 import tf_slim as slim
 from time import time
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/io/mind_all_iterator.py` & `recommenders-1.2.0/recommenders/models/newsrec/io/mind_all_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 import numpy as np
 import pickle
 
 from recommenders.models.deeprec.io.iterator import BaseIterator
@@ -142,15 +142,15 @@
         with tf.io.gfile.GFile(behaviors_file, "r") as rd:
             impr_index = 0
             for line in rd:
                 uid, time, history, impr = line.strip("\n").split(self.col_spliter)[-4:]
 
                 history = [self.nid2index[i] for i in history.split()]
                 history = [0] * (self.his_size - len(history)) + history[
-                    : self.his_size
+                    -self.his_size :
                 ]
 
                 impr_news = [self.nid2index[i.split("-")[0]] for i in impr.split()]
                 label = [int(i.split("-")[1]) for i in impr.split()]
                 uindex = self.uid2index[uid] if uid in self.uid2index else 0
 
                 self.histories.append(history)
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/io/mind_iterator.py` & `recommenders-1.2.0/recommenders/models/newsrec/io/mind_iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 import numpy as np
 import pickle
 
 from recommenders.models.deeprec.io.iterator import BaseIterator
@@ -115,15 +115,15 @@
         with tf.io.gfile.GFile(behaviors_file, "r") as rd:
             impr_index = 0
             for line in rd:
                 uid, time, history, impr = line.strip("\n").split(self.col_spliter)[-4:]
 
                 history = [self.nid2index[i] for i in history.split()]
                 history = [0] * (self.his_size - len(history)) + history[
-                    : self.his_size
+                    -self.his_size :
                 ]
 
                 impr_news = [self.nid2index[i.split("-")[0]] for i in impr.split()]
                 label = [int(i.split("-")[1]) for i in impr.split()]
                 uindex = self.uid2index[uid] if uid in self.uid2index else 0
 
                 self.histories.append(history)
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/models/base_model.py` & `recommenders-1.2.0/recommenders/models/newsrec/models/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import abc
 import time
 import numpy as np
 from tqdm import tqdm
 import tensorflow as tf
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/models/layers.py` & `recommenders-1.2.0/recommenders/models/newsrec/models/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow.compat.v1.keras as keras
 from tensorflow.compat.v1.linalg import einsum
 from tensorflow.compat.v1.keras import layers
 from tensorflow.compat.v1.keras import backend as K
 
@@ -52,15 +52,15 @@
             shape=(dim, 1),
             initializer=keras.initializers.glorot_uniform(seed=self.seed),
             trainable=True,
         )
         super(AttLayer2, self).build(input_shape)  # be sure you call this somewhere!
 
     def call(self, inputs, mask=None, **kwargs):
-        """Core implemention of soft attention
+        """Core implementation of soft attention.
 
         Args:
             inputs (object): input tensor.
 
         Returns:
             object: weighted sum of input tensors.
         """
@@ -80,27 +80,27 @@
         )
 
         attention_weight = K.expand_dims(attention_weight)
         weighted_input = inputs * attention_weight
         return K.sum(weighted_input, axis=1)
 
     def compute_mask(self, input, input_mask=None):
-        """Compte output mask value
+        """Compte output mask value.
 
         Args:
             input (object): input tensor.
             input_mask: input mask
 
         Returns:
             object: output mask.
         """
         return None
 
     def compute_output_shape(self, input_shape):
-        """Compute shape of output tensor
+        """Compute shape of output tensor.
 
         Args:
             input_shape (tuple): shape of input tensor.
 
         Returns:
             tuple: shape of output tensor.
         """
@@ -108,15 +108,15 @@
 
 
 class SelfAttention(layers.Layer):
     """Multi-head self attention implement.
 
     Args:
         multiheads (int): The number of heads.
-        head_dim (object): Dimention of each head.
+        head_dim (object): Dimension of each head.
         mask_right (boolean): whether to mask right words.
 
     Returns:
         object: Weighted sum after attention.
     """
 
     def __init__(self, multiheads, head_dim, seed=0, mask_right=False, **kwargs):
@@ -309,23 +309,31 @@
         bool tensor: True for values not equal to zero.
     """
 
     def __init__(self, **kwargs):
         super(ComputeMasking, self).__init__(**kwargs)
 
     def call(self, inputs, **kwargs):
+        """Call method for ComputeMasking.
+
+        Args:
+            inputs (object): input tensor.
+
+        Returns:
+            bool tensor: True for values not equal to zero.
+        """
         mask = K.not_equal(inputs, 0)
         return K.cast(mask, K.floatx())
 
     def compute_output_shape(self, input_shape):
         return input_shape
 
 
 class OverwriteMasking(layers.Layer):
-    """Set values at spasific positions to zero.
+    """Set values at specific positions to zero.
 
     Args:
         inputs (list): value tensor and mask tensor.
 
     Returns:
         object: tensor after setting values to zero.
     """
@@ -333,11 +341,19 @@
     def __init__(self, **kwargs):
         super(OverwriteMasking, self).__init__(**kwargs)
 
     def build(self, input_shape):
         super(OverwriteMasking, self).build(input_shape)
 
     def call(self, inputs, **kwargs):
+        """Call method for OverwriteMasking.
+
+        Args:
+            inputs (list): value tensor and mask tensor.
+
+        Returns:
+            object: tensor after setting values to zero.
+        """
         return inputs[0] * K.expand_dims(inputs[1])
 
     def compute_output_shape(self, input_shape):
         return input_shape[0]
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/models/lstur.py` & `recommenders-1.2.0/recommenders/models/newsrec/models/lstur.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow.compat.v1.keras as keras
 from tensorflow.compat.v1.keras import layers
 
 
 from recommenders.models.newsrec.models.base_model import BaseModel
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/models/naml.py` & `recommenders-1.2.0/recommenders/models/newsrec/models/naml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import tensorflow.keras as keras
 from tensorflow.keras import layers
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/models/npa.py` & `recommenders-1.2.0/recommenders/models/newsrec/models/npa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow.keras as keras
 from tensorflow.keras import layers
 
 
 from recommenders.models.newsrec.models.base_model import BaseModel
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/models/nrms.py` & `recommenders-1.2.0/recommenders/models/newsrec/models/nrms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow.keras as keras
 from tensorflow.keras import layers
 
 
 from recommenders.models.newsrec.models.base_model import BaseModel
```

### Comparing `recommenders-1.1.1/recommenders/models/newsrec/newsrec_utils.py` & `recommenders-1.2.0/recommenders/models/newsrec/newsrec_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 from recommenders.models.deeprec.deeprec_utils import (
     flat_config,
     HParams,
     load_yaml,
```

### Comparing `recommenders-1.1.1/recommenders/models/rbm/rbm.py` & `recommenders-1.2.0/recommenders/models/rbm/rbm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import tensorflow as tf
 import logging
 import os
 from pathlib import Path
@@ -115,15 +115,16 @@
         self.possible_ratings = possible_ratings
 
         # create a lookup table to map integer indices to float ratings
         self.ratings_lookup_table = tf.lookup.StaticHashTable(
             tf.lookup.KeyValueTensorInitializer(
                 tf.constant(list(range(len(self.possible_ratings))), dtype=tf.int32),
                 tf.constant(list(self.possible_ratings), dtype=tf.float32),
-            ), default_value=0
+            ),
+            default_value=0,
         )
 
         self.generate_graph()
         self.init_metrics()
         self.init_gpu()
         init_graph = tf.compat.v1.global_variables_initializer()
 
@@ -187,22 +188,18 @@
         f = tf.convert_to_tensor(
             value=g / g.sum(), dtype=tf.float32
         )  # normalize and convert to tensor
 
         samp = tf.nn.relu(tf.sign(pr - f))  # apply rejection method
 
         # get integer index of the rating to be sampled
-        v_argmax = tf.cast(
-            tf.argmax(input=samp, axis=2), "int32"
-        )
+        v_argmax = tf.cast(tf.argmax(input=samp, axis=2), "int32")
 
         # lookup the rating using integer index
-        v_samp = tf.cast(
-            self.ratings_lookup_table.lookup(v_argmax), "float32"
-        )
+        v_samp = tf.cast(self.ratings_lookup_table.lookup(v_argmax), "float32")
 
         return v_samp
 
     def multinomial_distribution(self, phi):
         """Probability that unit v has value l given phi: P(v=l|phi)
 
         Args:
@@ -244,15 +241,17 @@
 
         F = bias + f  # free energy density per training example
 
         return F
 
     def placeholder(self):
         """Initialize the placeholders for the visible units"""
-        self.vu = tf.compat.v1.placeholder(shape=[None, self.n_visible], dtype="float32")
+        self.vu = tf.compat.v1.placeholder(
+            shape=[None, self.n_visible], dtype="float32"
+        )
 
     def init_parameters(self):
         """Initialize the parameters of the model.
 
         This is a single layer model with two biases. So we have a rectangular matrix w_{ij} and
         two bias vectors to initialize.
 
@@ -463,15 +462,17 @@
         self.v = self.iter.get_next()
 
     def init_metrics(self):
         """Initialize metrics"""
 
         if self.with_metrics:  # if true (default) returns evaluation metrics
             self.rmse = tf.sqrt(
-                tf.compat.v1.losses.mean_squared_error(self.v, self.v_k, weights=tf.where(self.v > 0, 1, 0))
+                tf.compat.v1.losses.mean_squared_error(
+                    self.v, self.v_k, weights=tf.where(self.v > 0, 1, 0)
+                )
             )
 
     def generate_graph(self):
         """Call the different RBM modules to generate the computational graph"""
 
         log.info("Creating the computational graph")
 
@@ -694,15 +695,15 @@
         """
 
         v_, _ = self.eval_out()  # evaluate the ratings and the associated probabilities
         vp = self.sess.run(v_, feed_dict={self.vu: x})
 
         return vp
 
-    def save(self, file_path='./rbm_model.ckpt'):
+    def save(self, file_path="./rbm_model.ckpt"):
         """Save model parameters to `file_path`
 
         This function saves the current tensorflow session to a specified path.
 
         Args:
             file_path (str): output file path for the RBM model checkpoint
                 we will create a new directory if not existing.
@@ -714,15 +715,15 @@
         # create the directory if it does not exist
         os.makedirs(dir_name, exist_ok=True)
 
         # save trained model
         saver = tf.compat.v1.train.Saver()
         saver.save(self.sess, os.path.join(dir_name, file_name))
 
-    def load(self, file_path='./rbm_model.ckpt'):
+    def load(self, file_path="./rbm_model.ckpt"):
         """Load model parameters for further use.
 
         This function loads a saved tensorflow session.
 
         Args:
             file_path (str): file path for RBM model checkpoint
         """
```

### Comparing `recommenders-1.1.1/recommenders/models/rlrmc/RLRMCalgorithm.py` & `recommenders-1.2.0/recommenders/models/rlrmc/RLRMCalgorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import logging
 
 from pymanopt import Problem
 from recommenders.models.rlrmc.conjugate_gradient_ms import ConjugateGradientMS
@@ -184,28 +184,28 @@
         stats.setdefault("time", []).append(time_iter)
         stats.setdefault("objective", []).append(cost)
         stats.setdefault("gradnorm", []).append(gradnorm)
         U1 = weights[0]
         U2 = weights[1]
         B = weights[2]
         U1_dot_B = np.dot(U1, B)
-        train_mse = np.mean(residual_global ** 2)
+        train_mse = np.mean(residual_global**2)
         train_rmse = sqrt(train_mse)
         stats.setdefault("trainRMSE", []).append(train_rmse)
         # Prediction
         if entries_validation_csr_data is not None:
             RLRMCalgorithm._computeLoss_csrmatrix(
                 U1_dot_B,
                 U2.T,
                 entries_validation_csr_data,
                 entries_validation_csr_indices,
                 entries_validation_csr_indptr,
                 residual_validation_global,
             )
-            validation_mse = np.mean(residual_validation_global ** 2)
+            validation_mse = np.mean(residual_validation_global**2)
             validation_rmse = sqrt(validation_mse)
             stats.setdefault("validationRMSE", []).append(validation_rmse)
             logger.info(
                 "Train RMSE: %.4f, Validation RMSE: %.4f, Total time: %.2f"
                 % (train_rmse, validation_rmse, time_iter)
             )
         else:
@@ -229,15 +229,15 @@
             U1_dot_B,
             U2.T,
             entries_train_csr_data,
             entries_train_csr_indices,
             entries_train_csr_indptr,
             residual_global,
         )
-        objective = 0.5 * np.sum((residual_global) ** 2) + 0.5 * self.C * np.sum(B ** 2)
+        objective = 0.5 * np.sum((residual_global) ** 2) + 0.5 * self.C * np.sum(B**2)
         return objective
 
     # computes the gradient of the objective function at a given point
     def _egrad(
         self,
         weights,
         entries_train_csr_indices,
```

### Comparing `recommenders-1.1.1/recommenders/models/rlrmc/RLRMCdataset.py` & `recommenders-1.2.0/recommenders/models/rlrmc/RLRMCdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
 
 from recommenders.utils.constants import (
@@ -64,16 +64,15 @@
 
         Returns:
             list: train and validation pandas.DataFrame Dataset, which have been reindexed.
 
         """
         # Data processing and reindexing code is adopted from https://github.com/Microsoft/Recommenders/blob/main/recommenders/models/ncf/dataset.py
         # If validation dataset is None
-        df = train if validation is None else train.append(validation)
-        df = df if test is None else df.append(test)
+        df = pd.concat([train, validation, test])
 
         # Reindex user and item index
         if self.user_idx is None:
             # Map user id
             user_idx = df[[self.col_user]].drop_duplicates().reindex()
             user_idx[self.col_user + "_idx"] = np.arange(len(user_idx))
             self.n_users = len(user_idx)
```

### Comparing `recommenders-1.1.1/recommenders/models/rlrmc/conjugate_gradient_ms.py` & `recommenders-1.2.0/recommenders/models/rlrmc/conjugate_gradient_ms.py`

 * *Files identical despite different names*

### Comparing `recommenders-1.1.1/recommenders/models/sar/sar_singlenode.py` & `recommenders-1.2.0/recommenders/models/sar/sar_singlenode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
+
 import numpy as np
 import pandas as pd
 import logging
 from scipy import sparse
 
 from recommenders.utils.python_utils import (
     cosine_similarity,
@@ -83,15 +84,17 @@
             SIM_JACCARD,
             SIM_LIFT,
             SIM_MUTUAL_INFORMATION,
             SIM_LEXICOGRAPHERS_MUTUAL_INFORMATION,
         ]
         if similarity_type not in available_similarity_types:
             raise ValueError(
-                'Similarity type must be one of ["' + '" | "'.join(available_similarity_types) + '"]'
+                'Similarity type must be one of ["'
+                + '" | "'.join(available_similarity_types)
+                + '"]'
             )
         self.similarity_type = similarity_type
         self.time_decay_half_life = (
             time_decay_coefficient * 24 * 60 * 60
         )  # convert to seconds
         self.time_decay_flag = timedecay_formula
         self.time_now = time_now
@@ -219,17 +222,16 @@
         # set values for the total count of users and items
         self.n_users = len(self.user2index)
         self.n_items = len(self.index2item)
 
     def fit(self, df):
         """Main fit method for SAR.
 
-        .. note::
-
-        Please make sure that `df` has no duplicates.
+        Note:
+            Please make sure that `df` has no duplicates.
 
         Args:
             df (pandas.DataFrame): User item rating dataframe (without duplicates).
         """
         select_columns = [self.col_user, self.col_item, self.col_rating]
         if self.time_decay_flag:
             select_columns += [self.col_timestamp]
```

### Comparing `recommenders-1.1.1/recommenders/models/sasrec/model.py` & `recommenders-1.2.0/recommenders/models/sasrec/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
+
 import random
 import numpy as np
 from tqdm import tqdm
 import tensorflow as tf
 
 from recommenders.utils.timer import Timer
 
@@ -68,28 +69,28 @@
         # Key Masking
         key_masks = tf.sign(tf.abs(tf.reduce_sum(keys, axis=-1)))  # (N, T_k)
         key_masks = tf.tile(key_masks, [self.num_heads, 1])  # (h*N, T_k)
         key_masks = tf.tile(
             tf.expand_dims(key_masks, 1), [1, tf.shape(queries)[1], 1]
         )  # (h*N, T_q, T_k)
 
-        paddings = tf.ones_like(outputs) * (-(2 ** 32) + 1)
+        paddings = tf.ones_like(outputs) * (-(2**32) + 1)
         # outputs, (h*N, T_q, T_k)
         outputs = tf.where(tf.equal(key_masks, 0), paddings, outputs)
 
         # Future blinding (Causality)
         diag_vals = tf.ones_like(outputs[0, :, :])  # (T_q, T_k)
         tril = tf.linalg.LinearOperatorLowerTriangular(
             diag_vals
         ).to_dense()  # (T_q, T_k)
         masks = tf.tile(
             tf.expand_dims(tril, 0), [tf.shape(outputs)[0], 1, 1]
         )  # (h*N, T_q, T_k)
 
-        paddings = tf.ones_like(masks) * (-(2 ** 32) + 1)
+        paddings = tf.ones_like(masks) * (-(2**32) + 1)
         # outputs, (h*N, T_q, T_k)
         outputs = tf.where(tf.equal(masks, 0), paddings, outputs)
 
         # Activation
         outputs = tf.nn.softmax(outputs)  # (h*N, T_q, T_k)
 
         # Query Masking, query_masks (N, T_q)
@@ -443,15 +444,15 @@
         Returns:
             tf.Tensor, tf.Tensor:
             - Sequence embeddings.
             - Positional embeddings.
         """
 
         seq_embeddings = self.item_embedding_layer(input_seq)
-        seq_embeddings = seq_embeddings * (self.embedding_dim ** 0.5)
+        seq_embeddings = seq_embeddings * (self.embedding_dim**0.5)
 
         # FIXME
         positional_seq = tf.expand_dims(tf.range(tf.shape(input_seq)[1]), 0)
         positional_seq = tf.tile(positional_seq, [tf.shape(input_seq)[0], 1])
         positional_embeddings = self.positional_embedding_layer(positional_seq)
 
         return seq_embeddings, positional_embeddings
```

### Comparing `recommenders-1.1.1/recommenders/models/sasrec/sampler.py` & `recommenders-1.2.0/recommenders/models/sasrec/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 # Original codes are from
 # https://github.com/kang205/SASRec/blob/master/sampler.py
+
 import numpy as np
 from multiprocessing import Process, Queue
 
 
 def random_neq(left, right, s):
     t = np.random.randint(left, right)
     while t in s:
```

### Comparing `recommenders-1.1.1/recommenders/models/sasrec/ssept.py` & `recommenders-1.2.0/recommenders/models/sasrec/ssept.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
+
 import tensorflow as tf
 from recommenders.models.sasrec.model import SASREC, Encoder, LayerNormalization
 
 
 class SSEPT(SASREC):
     """
     SSE-PT Model
@@ -96,15 +97,15 @@
         mask = tf.expand_dims(tf.cast(tf.not_equal(input_seq, 0), tf.float32), -1)
         seq_embeddings, positional_embeddings = self.embedding(input_seq)
 
         # User Encoding
         # u0_latent = self.user_embedding_layer(users[0])
         # u0_latent = u0_latent * (self.embedding_dim ** 0.5)
         u_latent = self.user_embedding_layer(users)
-        u_latent = u_latent * (self.user_embedding_dim ** 0.5)  # (b, 1, h)
+        u_latent = u_latent * (self.user_embedding_dim**0.5)  # (b, 1, h)
         # return users
 
         # replicate the user embedding for all the items
         u_latent = tf.tile(u_latent, [1, tf.shape(input_seq)[1], 1])  # (b, s, h)
 
         seq_embeddings = tf.reshape(
             tf.concat([seq_embeddings, u_latent], 2),
@@ -176,20 +177,20 @@
         input_seq = inputs["input_seq"]
         candidate = inputs["candidate"]
 
         mask = tf.expand_dims(tf.cast(tf.not_equal(input_seq, 0), tf.float32), -1)
         seq_embeddings, positional_embeddings = self.embedding(input_seq)  # (1, s, h)
 
         u0_latent = self.user_embedding_layer(user)
-        u0_latent = u0_latent * (self.user_embedding_dim ** 0.5)  # (1, 1, h)
+        u0_latent = u0_latent * (self.user_embedding_dim**0.5)  # (1, 1, h)
         u0_latent = tf.squeeze(u0_latent, axis=0)  # (1, h)
         test_user_emb = tf.tile(u0_latent, [1 + self.num_neg_test, 1])  # (101, h)
 
         u_latent = self.user_embedding_layer(user)
-        u_latent = u_latent * (self.user_embedding_dim ** 0.5)  # (b, 1, h)
+        u_latent = u_latent * (self.user_embedding_dim**0.5)  # (b, 1, h)
         u_latent = tf.tile(u_latent, [1, tf.shape(input_seq)[1], 1])  # (b, s, h)
 
         seq_embeddings = tf.reshape(
             tf.concat([seq_embeddings, u_latent], 2),
             [tf.shape(input_seq)[0], -1, self.hidden_units],
         )
         seq_embeddings += positional_embeddings  # (b, s, h1 + h2)
```

### Comparing `recommenders-1.1.1/recommenders/models/sasrec/util.py` & `recommenders-1.2.0/recommenders/models/sasrec/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
+
 from collections import defaultdict
 
 
 class SASRecDataSet:
     """
     A class for creating SASRec specific dataset used during
     train, validation and testing.
@@ -30,19 +31,21 @@
         self.user_test = {}
         self.col_sep = kwargs.get("col_sep", " ")
         self.filename = kwargs.get("filename", None)
 
         if self.filename:
             with open(self.filename, "r") as fr:
                 sample = fr.readline()
-            ncols = sample.strip().split(self.col_sep)
+            ncols = len(sample.strip().split(self.col_sep))
             if ncols == 3:
                 self.with_time = True
-            else:
+            elif ncols == 2:
                 self.with_time = False
+            else:
+                raise ValueError(f"3 or 2 columns must be in dataset. Given {ncols} columns")
 
     def split(self, **kwargs):
         self.filename = kwargs.get("filename", self.filename)
         if not self.filename:
             raise ValueError("Filename is required")
 
         if self.with_time:
```

### Comparing `recommenders-1.1.1/recommenders/models/surprise/surprise_utils.py` & `recommenders-1.2.0/recommenders/models/surprise/surprise_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import pandas as pd
 import numpy as np
 
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
```

### Comparing `recommenders-1.1.1/recommenders/models/tfidf/tfidf_utils.py` & `recommenders-1.2.0/recommenders/models/tfidf/tfidf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.metrics.pairwise import linear_kernel
 from transformers import BertTokenizer
 import re
@@ -111,24 +111,24 @@
         df[new_col_name] = df[new_col_name].map(
             lambda x: self.__clean_text(x, for_BERT)
         )
 
         return df
 
     def tokenize_text(
-        self, df_clean, text_col="cleaned_text", ngram_range=(1, 3), min_df=0
+        self, df_clean, text_col="cleaned_text", ngram_range=(1, 3), min_df=0.0
     ):
         """Tokenize the input text.
         For more details on the TfidfVectorizer, see https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html
 
         Args:
             df_clean (pandas.DataFrame): Dataframe with cleaned text in the new column.
             text_col (str): Name of column containing the cleaned text.
             ngram_range (tuple of int): The lower and upper boundary of the range of n-values for different n-grams to be extracted.
-            min_df (int): When building the vocabulary ignore terms that have a document frequency strictly lower than the given threshold.
+            min_df (float): When building the vocabulary ignore terms that have a document frequency strictly lower than the given threshold.
 
         Returns:
             TfidfVectorizer, pandas.Series:
             - Scikit-learn TfidfVectorizer object defined in `.tokenize_text()`.
             - Each row contains tokens for respective documents separated by spaces.
         """
         vectors = df_clean[text_col]
```

### Comparing `recommenders-1.1.1/recommenders/models/vae/multinomial_vae.py` & `recommenders-1.2.0/recommenders/models/vae/multinomial_vae.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from recommenders.evaluation.python_evaluation import ndcg_at_k
 
@@ -316,15 +316,15 @@
         self.h_decoded = self.h_decoder(self.z)
         self.h_decoded_ = self.dropout_decoder(self.h_decoded)
         self.x_decoded = self.x_bar(self.h_decoded_)
 
         # Training
         self.model = Model(self.x, self.x_decoded)
         self.model.compile(
-            optimizer=tf.keras.optimizers.Adam(learning_rate=0.001),
+            optimizer=tf.keras.optimizers.legacy.Adam(learning_rate=0.001),
             loss=self._get_vae_loss,
         )
 
     def _get_vae_loss(self, x, x_bar):
         """Calculate negative ELBO (NELBO)."""
         log_softmax_var = tf.nn.log_softmax(x_bar)
         self.neg_ll = -tf.reduce_mean(
```

### Comparing `recommenders-1.1.1/recommenders/models/vae/standard_vae.py` & `recommenders-1.2.0/recommenders/models/vae/standard_vae.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 import tensorflow as tf
 from tensorflow.keras.layers import *
@@ -287,15 +287,15 @@
         self.h_decoded = self.h_decoder(self.z)
         self.h_decoded_ = self.dropout_decoder(self.h_decoded)
         self.x_decoded = self.x_bar(self.h_decoded_)
 
         # Training
         self.model = Model(self.x, self.x_decoded)
         self.model.compile(
-            optimizer=tf.keras.optimizers.Adam(learning_rate=0.001),
+            optimizer=tf.keras.optimizers.legacy.Adam(learning_rate=0.001),
             loss=self._get_vae_loss,
         )
 
     def _get_vae_loss(self, x, x_bar):
         """Calculate negative ELBO (NELBO)."""
         # Reconstruction error: logistic log likelihood
         reconst_loss = self.original_dim * binary_crossentropy(x, x_bar)
```

### Comparing `recommenders-1.1.1/recommenders/models/vowpal_wabbit/vw.py` & `recommenders-1.2.0/recommenders/models/vowpal_wabbit/vw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 """
 This file provides a wrapper to run Vowpal Wabbit from the command line through python.
 It is not recommended to use this approach in production, there are python bindings that can be installed from the
 repository or pip or the command line can be used. This is merely to demonstrate vw usage in the example notebooks.
 """
```

### Comparing `recommenders-1.1.1/recommenders/models/wide_deep/wide_deep_utils.py` & `recommenders-1.2.0/recommenders/models/wide_deep/wide_deep_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import tensorflow as tf
 
 from recommenders.utils.constants import DEFAULT_USER_COL, DEFAULT_ITEM_COL
 from recommenders.utils.tf_utils import MODEL_DIR
 
@@ -105,19 +105,19 @@
 
     Returns:
         list: Deep feature columns.
     """
     deep_columns = [
         # User embedding
         tf.feature_column.embedding_column(
-            categorical_column=user_ids, dimension=user_dim, max_norm=user_dim ** 0.5
+            categorical_column=user_ids, dimension=user_dim, max_norm=user_dim**0.5
         ),
         # Item embedding
         tf.feature_column.embedding_column(
-            categorical_column=item_ids, dimension=item_dim, max_norm=item_dim ** 0.5
+            categorical_column=item_ids, dimension=item_dim, max_norm=item_dim**0.5
         ),
     ]
     # Item feature
     if item_feat_col is not None:
         deep_columns.append(
             tf.feature_column.numeric_column(
                 item_feat_col, shape=item_feat_shape, dtype=tf.float32
@@ -157,19 +157,23 @@
         log_every_n_iter (int): Log the training loss for every n steps.
         save_checkpoints_steps (int): Model checkpoint frequency.
         seed (int): Random seed.
 
     Returns:
         tf.estimator.Estimator: Model
     """
-    # TensorFlow training log frequency setup
+    gpu_config = tf.compat.v1.ConfigProto()
+    gpu_config.gpu_options.allow_growth = True  # dynamic memory allocation
+
+    # TensorFlow training setup
     config = tf.estimator.RunConfig(
         tf_random_seed=seed,
         log_step_count_steps=log_every_n_iter,
         save_checkpoints_steps=save_checkpoints_steps,
+        session_config=gpu_config,
     )
 
     if len(wide_columns) > 0 and len(deep_columns) == 0:
         model = tf.compat.v1.estimator.LinearRegressor(
             model_dir=model_dir,
             config=config,
             feature_columns=wide_columns,
```

### Comparing `recommenders-1.1.1/recommenders/tuning/nni/ncf_training.py` & `recommenders-1.2.0/recommenders/tuning/nni/ncf_training.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import argparse
 import json
 import logging
 import numpy as np
 import os
```

### Comparing `recommenders-1.1.1/recommenders/tuning/nni/ncf_utils.py` & `recommenders-1.2.0/recommenders/tuning/nni/ncf_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import pandas as pd
 
 from recommenders.utils.constants import DEFAULT_K
```

### Comparing `recommenders-1.1.1/recommenders/tuning/nni/nni_utils.py` & `recommenders-1.2.0/recommenders/tuning/nni/nni_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import ast
 import json
 import os
 import requests
 import subprocess
```

### Comparing `recommenders-1.1.1/recommenders/tuning/nni/svd_training.py` & `recommenders-1.2.0/recommenders/tuning/nni/svd_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import argparse
 import json
 import logging
 import os
 import numpy as np
```

### Comparing `recommenders-1.1.1/recommenders/tuning/parameter_sweep.py` & `recommenders-1.2.0/recommenders/tuning/parameter_sweep.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 #
 # Utility functions for parameter sweep.
 
 from itertools import product
```

### Comparing `recommenders-1.1.1/recommenders/utils/constants.py` & `recommenders-1.2.0/recommenders/utils/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors. All rights reserved.
 # Licensed under the MIT License.
 
 # Default column names
 DEFAULT_USER_COL = "userID"
 DEFAULT_ITEM_COL = "itemID"
 DEFAULT_RATING_COL = "rating"
 DEFAULT_LABEL_COL = "label"
```

### Comparing `recommenders-1.1.1/recommenders/utils/general_utils.py` & `recommenders-1.2.0/recommenders/utils/general_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import psutil
 
 
 def invert_dictionary(dictionary):
     """Invert a dictionary
 
-    .. note::
+    Note:
 
         If the dictionary has unique keys and unique values, the inversion would be perfect. However, if there are
         repeated values, the inversion can take different keys
 
     Args:
         dictionary (dict): A dictionary
```

### Comparing `recommenders-1.1.1/recommenders/utils/k8s_utils.py` & `recommenders-1.2.0/recommenders/utils/k8s_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 from math import ceil, floor
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `recommenders-1.1.1/recommenders/utils/notebook_memory_management.py` & `recommenders-1.2.0/recommenders/utils/notebook_memory_management.py`

 * *Files identical despite different names*

### Comparing `recommenders-1.1.1/recommenders/utils/plot.py` & `recommenders-1.2.0/recommenders/utils/plot.py`

 * *Files identical despite different names*

### Comparing `recommenders-1.1.1/recommenders/utils/python_utils.py` & `recommenders-1.2.0/recommenders/utils/python_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import logging
 import numpy as np
 from scipy import sparse
 
 
@@ -58,15 +58,15 @@
     """
 
     diag_rows, diag_cols = _get_row_and_column_matrix(cooccurrence.diagonal())
 
     with np.errstate(invalid="ignore", divide="ignore"):
         result = cooccurrence / (diag_rows + diag_cols - cooccurrence)
 
-    return np.array(result)
+    return np.array(result) if isinstance(result, np.ndarray) else result.toarray()
 
 
 def lift(cooccurrence):
     """Helper method to calculate the Lift of a matrix of
     co-occurrences. In comparison with basic co-occurrence and Jaccard
     similarity, lift favours discoverability and serendipity, as
     opposed to co-occurrence that favours the most popular items, and
@@ -81,15 +81,15 @@
     """
 
     diag_rows, diag_cols = _get_row_and_column_matrix(cooccurrence.diagonal())
 
     with np.errstate(invalid="ignore", divide="ignore"):
         result = cooccurrence / (diag_rows * diag_cols)
 
-    return np.array(result)
+    return np.array(result) if isinstance(result, np.ndarray) else result.toarray()
 
 
 def mutual_information(cooccurrence):
     """Helper method to calculate the Mutual Information of a matrix of
     co-occurrences.
 
     Mutual information is a measurement of the amount of information
@@ -102,15 +102,15 @@
         numpy.ndarray: The matrix of mutual information between any two items.
 
     """
 
     with np.errstate(invalid="ignore", divide="ignore"):
         result = np.log2(cooccurrence.shape[0] * lift(cooccurrence))
 
-    return np.array(result)
+    return np.array(result) if isinstance(result, np.ndarray) else result.toarray()
 
 
 def lexicographers_mutual_information(cooccurrence):
     """Helper method to calculate the Lexicographers Mutual Information of
     a matrix of co-occurrences.
 
     Due to the bias of mutual information for low frequency items,
@@ -124,15 +124,15 @@
         numpy.ndarray: The matrix of lexicographers mutual information between any two items.
 
     """
 
     with np.errstate(invalid="ignore", divide="ignore"):
         result = cooccurrence * mutual_information(cooccurrence)
 
-    return np.array(result)
+    return np.array(result) if isinstance(result, np.ndarray) else result.toarray()
 
 
 def cosine_similarity(cooccurrence):
     """Helper method to calculate the Cosine similarity of a matrix of
     co-occurrences.
 
     Cosine similarity can be interpreted as the angle between the i-th
@@ -147,15 +147,15 @@
     """
 
     diag_rows, diag_cols = _get_row_and_column_matrix(cooccurrence.diagonal())
 
     with np.errstate(invalid="ignore", divide="ignore"):
         result = cooccurrence / np.sqrt(diag_rows * diag_cols)
 
-    return np.array(result)
+    return np.array(result) if isinstance(result, np.ndarray) else result.toarray()
 
 
 def inclusion_index(cooccurrence):
     """Helper method to calculate the Inclusion Index of a matrix of
     co-occurrences.
 
     Inclusion index measures the overlap between items.
@@ -169,15 +169,15 @@
     """
 
     diag_rows, diag_cols = _get_row_and_column_matrix(cooccurrence.diagonal())
 
     with np.errstate(invalid="ignore", divide="ignore"):
         result = cooccurrence / np.minimum(diag_rows, diag_cols)
 
-    return np.array(result)
+    return np.array(result) if isinstance(result, np.ndarray) else result.toarray()
 
 
 def get_top_k_scored_items(scores, top_k, sort_top_k=False):
     """Extract top K items from a matrix of scores for each user-item pair, optionally sort results per user.
 
     Args:
         scores (numpy.ndarray): Score matrix (users x items).
@@ -230,15 +230,15 @@
 
 
 def rescale(data, new_min=0, new_max=1, data_min=None, data_max=None):
     """Rescale/normalize the data to be within the range `[new_min, new_max]`
     If data_min and data_max are explicitly provided, they will be used
     as the old min/max values instead of taken from the data.
 
-    .. note::
+    Note:
         This is same as the `scipy.MinMaxScaler` with the exception that we can override
         the min/max of the old scale.
 
     Args:
         data (numpy.ndarray): 1d scores vector or 2d score matrix (users x items).
         new_min (int|float): The minimum of the newly scaled data.
         new_max (int|float): The maximum of the newly scaled data.
```

### Comparing `recommenders-1.1.1/recommenders/utils/spark_utils.py` & `recommenders-1.2.0/recommenders/utils/spark_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 
 
 try:
     from pyspark.sql import SparkSession  # noqa: F401
@@ -26,15 +26,15 @@
     repositories=None,
 ):
     """Start Spark if not started
 
     Args:
         app_name (str): set name of the application
         url (str): URL for spark master
-        memory (str): size of memory for spark driver
+        memory (str): size of memory for spark driver. This will be ignored if spark.driver.memory is set in config.
         config (dict): dictionary of configuration options
         packages (list): list of packages to install
         jars (list): list of jar files to add
         repositories (list): list of maven repositories
 
     Returns:
         object: Spark context.
@@ -61,9 +61,13 @@
                 '"{}"'.format(raw_value) if isinstance(raw_value, str) else raw_value
             )
             spark_opts.append('config("{key}", {value})'.format(key=key, value=value))
 
     if config is None or "spark.driver.memory" not in config:
         spark_opts.append('config("spark.driver.memory", "{}")'.format(memory))
 
+    # Set larger stack size
+    spark_opts.append('config("spark.executor.extraJavaOptions", "-Xss4m")')
+    spark_opts.append('config("spark.driver.extraJavaOptions", "-Xss4m")')
+
     spark_opts.append("getOrCreate()")
     return eval(".".join(spark_opts))
```

### Comparing `recommenders-1.1.1/recommenders/utils/tf_utils.py` & `recommenders-1.2.0/recommenders/utils/tf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import itertools
 import numpy as np
 import tensorflow as tf
 from tensorflow_estimator.python.estimator.export.export import (
     build_supervised_input_receiver_fn_from_input_fn,
@@ -57,16 +57,15 @@
 
 def pandas_input_fn(
     df, y_col=None, batch_size=128, num_epochs=1, shuffle=False, seed=None
 ):
     """Pandas input function for TensorFlow high-level API Estimator.
     This function returns a `tf.data.Dataset` function.
 
-    .. note::
-
+    Note:
         `tf.estimator.inputs.pandas_input_fn` cannot handle array/list column properly.
         For more information, see https://www.tensorflow.org/api_docs/python/tf/estimator/inputs/numpy_input_fn
 
     Args:
         df (pandas.DataFrame): Data containing features.
         y_col (str): Label column name if df has it.
         batch_size (int): Batch size for the input function.
@@ -195,15 +194,15 @@
     model_dir=None,
     batch_size=256,
     eval_fns=None,
     **eval_kwargs
 ):
     """Evaluation log hook for TensorFlow high-level API Estimator.
 
-    .. note::
+    Note:
        TensorFlow Estimator model uses the last checkpoint weights for evaluation or prediction.
        In order to get the most up-to-date evaluation results while training,
        set model's `save_checkpoints_steps` to be equal or greater than hook's `every_n_iter`.
 
     Args:
         estimator (tf.estimator.Estimator): Model to evaluate.
         logger (Logger): Custom logger to log the results.
@@ -212,15 +211,15 @@
         y_col (str): Label column name in true_df
         eval_df (pd.DataFrame): Evaluation data without label column.
         every_n_iter (int): Evaluation frequency (steps).
         model_dir (str): Model directory to save the summaries to. If None, does not record.
         batch_size (int): Number of samples fed into the model at a time.
             Note, the batch size doesn't affect on evaluation results.
         eval_fns (iterable of functions): List of evaluation functions that have signature of
-            (true_df, prediction_df, **eval_kwargs)->(float). If None, loss is calculated on true_df.
+            `(true_df, prediction_df, **eval_kwargs)`->`float`. If None, loss is calculated on `true_df`.
         eval_kwargs: Evaluation function's keyword arguments.
             Note, prediction column name should be 'prediction'
 
     Returns:
         tf.train.SessionRunHook: Session run hook to evaluate the model while training.
     """
```

### Comparing `recommenders-1.1.1/recommenders/utils/timer.py` & `recommenders-1.2.0/recommenders/utils/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 from timeit import default_timer
 
 
 class Timer(object):
     """Timer class.
```

### Comparing `recommenders-1.1.1/recommenders.egg-info/PKG-INFO` & `recommenders-1.2.0/recommenders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: recommenders
-Version: 1.1.1
-Summary: Microsoft Recommenders - Python utilities for building recommender systems
-Home-page: https://github.com/microsoft/recommenders
-Author: RecoDev Team at Microsoft
-Author-email: RecoDevTeam@service.microsoft.com
+Version: 1.2.0
+Summary: Recommenders - Python utilities for building recommendation systems
+Home-page: https://github.com/recommenders-team/recommenders
+Author: Recommenders contributors
+Author-email: recommenders-technical-discuss@lists.lfaidata.foundation
 License: UNKNOWN
-Project-URL: Documentation, https://microsoft-recommenders.readthedocs.io/en/stable/
-Project-URL: Wiki, https://github.com/microsoft/recommenders/wiki
-Description: # Recommender Utilities
+Project-URL: Documentation, https://recommenders-team.github.io/recommenders/intro.html
+Project-URL: Wiki, https://github.com/recommenders-team/recommenders/wiki
+Description: <!--
+        Copyright (c) Recommenders contributors.
+        Licensed under the MIT License.
+        -->
+        
+        # Recommender Utilities
         
         This package contains functions to simplify common tasks used when developing and evaluating recommender systems. A short description of the submodules is provided below. For more details about what functions are available and how to use them, please review the doc-strings provided with the code or the [online documentation](https://readthedocs.org/projects/microsoft-recommenders/).
         
         # Installation
         
         ## Pre-requisites
         Some dependencies require compilation during pip installation. On Linux this can be supported by adding build-essential dependencies:
         ```bash
         sudo apt-get install -y build-essential libpython<version>
         ``` 
-        where `<version>` should be the Python version (e.g. `3.6`).
+        where `<version>` should be the Python version (e.g. `3.8`).
         
         On Windows you will need [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)
         
         For more details about the software requirements that must be pre-installed on each supported platform, see the [setup guide](https://github.com/microsoft/recommenders/blob/main/SETUP.md).   
         
         ## Basic installation
         
@@ -149,15 +154,15 @@
         The models submodule contains implementations of various algorithms that can be used in addition to external packages to evaluate and develop new recommender system approaches. A description of all the algorithms can be found on [this table](../README.md#algorithms). The following is a list of the algorithm utilities:
         
         * Cornac
         * DeepRec
           *  Convolutional Sequence Embedding Recommendation (CASER)
           *  Deep Knowledge-Aware Network (DKN)
           *  Extreme Deep Factorization Machine (xDeepFM)
-          *  GRU4Rec
+          *  GRU
           *  LightGCN
           *  Next Item Recommendation (NextItNet)
           *  Short-term and Long-term Preference Integrated Recommender (SLi-Rec)
           *  Multi-Interest-Aware Sequential User Modeling (SUM)
         * FastAI
         * GeoIMC
         * LightFM
@@ -197,23 +202,19 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.6, <3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: examples
 Provides-Extra: gpu
 Provides-Extra: spark
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: experimental
-Provides-Extra: nni
```

### Comparing `recommenders-1.1.1/recommenders.egg-info/SOURCES.txt` & `recommenders-1.2.0/recommenders.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 recommenders/models/deeprec/models/dkn_item2item.py
 recommenders/models/deeprec/models/xDeepFM.py
 recommenders/models/deeprec/models/graphrec/__init__.py
 recommenders/models/deeprec/models/graphrec/lightgcn.py
 recommenders/models/deeprec/models/sequential/__init__.py
 recommenders/models/deeprec/models/sequential/asvd.py
 recommenders/models/deeprec/models/sequential/caser.py
-recommenders/models/deeprec/models/sequential/gru4rec.py
+recommenders/models/deeprec/models/sequential/gru.py
 recommenders/models/deeprec/models/sequential/nextitnet.py
 recommenders/models/deeprec/models/sequential/rnn_cell_implement.py
 recommenders/models/deeprec/models/sequential/sequential_base_model.py
 recommenders/models/deeprec/models/sequential/sli_rec.py
 recommenders/models/deeprec/models/sequential/sum.py
 recommenders/models/deeprec/models/sequential/sum_cells.py
 recommenders/models/fastai/__init__.py
@@ -123,57 +123,78 @@
 recommenders/utils/notebook_memory_management.py
 recommenders/utils/notebook_utils.py
 recommenders/utils/plot.py
 recommenders/utils/python_utils.py
 recommenders/utils/spark_utils.py
 recommenders/utils/tf_utils.py
 recommenders/utils/timer.py
+tests/ci/__init__.py
+tests/ci/azureml_tests/__init__.py
+tests/ci/azureml_tests/run_groupwise_pytest.py
+tests/ci/azureml_tests/submit_groupwise_azureml_pytest.py
+tests/ci/azureml_tests/test_groups.py
+tests/data_validation/__init__.py
+tests/data_validation/examples/__init__.py
+tests/data_validation/examples/test_mind.py
+tests/data_validation/examples/test_wikidata.py
+tests/data_validation/recommenders/__init__.py
+tests/data_validation/recommenders/datasets/__init__.py
+tests/data_validation/recommenders/datasets/test_covid_utils.py
+tests/data_validation/recommenders/datasets/test_criteo.py
+tests/data_validation/recommenders/datasets/test_mind.py
+tests/data_validation/recommenders/datasets/test_movielens.py
+tests/data_validation/recommenders/datasets/test_wikidata.py
+tests/functional/__init__.py
+tests/functional/examples/__init__.py
+tests/functional/examples/test_notebooks_gpu.py
+tests/functional/examples/test_notebooks_pyspark.py
+tests/functional/examples/test_notebooks_python.py
 tests/integration/__init__.py
-tests/integration/examples/__init__.py
-tests/integration/examples/test_notebooks_gpu.py
-tests/integration/examples/test_notebooks_pyspark.py
-tests/integration/examples/test_notebooks_python.py
 tests/integration/recommenders/__init__.py
-tests/integration/recommenders/datasets/__init__.py
-tests/integration/recommenders/datasets/test_criteo.py
-tests/integration/recommenders/datasets/test_mind.py
-tests/integration/recommenders/datasets/test_movielens.py
+tests/integration/recommenders/utils/__init__.py
+tests/integration/recommenders/utils/test_k8s_utils.py
+tests/performance/__init__.py
+tests/performance/recommenders/__init__.py
+tests/performance/recommenders/evaluation/__init__.py
+tests/performance/recommenders/evaluation/test_python_evaluation_time_performance.py
+tests/regression/__init__.py
+tests/regression/test_compatibility_tf.py
+tests/responsible_ai/__init__.py
+tests/responsible_ai/recommenders/__init__.py
+tests/responsible_ai/recommenders/datasets/__init__.py
+tests/responsible_ai/recommenders/datasets/test_criteo_privacy.py
+tests/responsible_ai/recommenders/datasets/test_movielens_privacy.py
+tests/security/__init__.py
+tests/security/test_dependency_security.py
 tests/smoke/__init__.py
 tests/smoke/examples/__init__.py
 tests/smoke/examples/test_notebooks_gpu.py
 tests/smoke/examples/test_notebooks_pyspark.py
 tests/smoke/examples/test_notebooks_python.py
 tests/smoke/recommenders/__init__.py
-tests/smoke/recommenders/dataset/__init__.py
-tests/smoke/recommenders/dataset/test_criteo.py
-tests/smoke/recommenders/dataset/test_mind.py
-tests/smoke/recommenders/dataset/test_movielens.py
 tests/smoke/recommenders/recommender/__init__.py
 tests/smoke/recommenders/recommender/test_deeprec_model.py
 tests/smoke/recommenders/recommender/test_deeprec_utils.py
 tests/smoke/recommenders/recommender/test_newsrec_model.py
 tests/smoke/recommenders/recommender/test_newsrec_utils.py
 tests/unit/__init__.py
 tests/unit/examples/__init__.py
 tests/unit/examples/test_notebooks_gpu.py
 tests/unit/examples/test_notebooks_pyspark.py
 tests/unit/examples/test_notebooks_python.py
 tests/unit/recommenders/__init__.py
 tests/unit/recommenders/datasets/__init__.py
-tests/unit/recommenders/datasets/test_covid_utils.py
-tests/unit/recommenders/datasets/test_dataset.py
-tests/unit/recommenders/datasets/test_movielens.py
+tests/unit/recommenders/datasets/test_download_utils.py
 tests/unit/recommenders/datasets/test_pandas_df_utils.py
 tests/unit/recommenders/datasets/test_python_splitter.py
 tests/unit/recommenders/datasets/test_spark_splitter.py
 tests/unit/recommenders/datasets/test_sparse.py
-tests/unit/recommenders/datasets/test_wikidata.py
 tests/unit/recommenders/evaluation/__init__.py
+tests/unit/recommenders/evaluation/conftest.py
 tests/unit/recommenders/evaluation/test_python_evaluation.py
-tests/unit/recommenders/evaluation/test_python_evaluation_time_performance.py
 tests/unit/recommenders/evaluation/test_spark_evaluation.py
 tests/unit/recommenders/models/__init__.py
 tests/unit/recommenders/models/test_cornac_utils.py
 tests/unit/recommenders/models/test_deeprec_model.py
 tests/unit/recommenders/models/test_deeprec_utils.py
 tests/unit/recommenders/models/test_geoimc.py
 tests/unit/recommenders/models/test_lightfm_utils.py
@@ -191,13 +212,12 @@
 tests/unit/recommenders/tuning/__init__.py
 tests/unit/recommenders/tuning/test_ncf_utils.py
 tests/unit/recommenders/tuning/test_nni_utils.py
 tests/unit/recommenders/tuning/test_sweep.py
 tests/unit/recommenders/utils/__init__.py
 tests/unit/recommenders/utils/test_general_utils.py
 tests/unit/recommenders/utils/test_gpu_utils.py
-tests/unit/recommenders/utils/test_k8s_utils.py
 tests/unit/recommenders/utils/test_notebook_utils.py
 tests/unit/recommenders/utils/test_plot.py
 tests/unit/recommenders/utils/test_python_utils.py
 tests/unit/recommenders/utils/test_tf_utils.py
 tests/unit/recommenders/utils/test_timer.py
```

### Comparing `recommenders-1.1.1/setup.py` & `recommenders-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 from os import environ
 from pathlib import Path
 from setuptools import setup, find_packages
 import site
 import sys
 import time
 
-# workround for enabling editable user pip installs
+# Workaround for enabling editable user pip installs
 site.ENABLE_USER_SITE = "--user" in sys.argv[1:]
 
-# version
+# Version
 here = Path(__file__).absolute().parent
 version_data = {}
 with open(here.joinpath("recommenders", "__init__.py"), "r") as f:
     exec(f.read(), version_data)
 version = version_data.get("__version__", "0.0")
 
 # Get the long description from the README file
@@ -23,121 +23,105 @@
     LONG_DESCRIPTION = f.read()
 
 HASH = environ.get("HASH", None)
 if HASH is not None:
     version += ".post" + str(int(time.time()))
 
 install_requires = [
-    "numpy>=1.19",  # 1.19 required by tensorflow 2.6
-    "pandas>1.0.3,<2",
-    "scipy>=1.0.0,<2",
-    "tqdm>=4.31.1,<5",
-    "matplotlib>=2.2.2,<4",
-    "scikit-learn>=0.22.1,<1.0.3",
-    "numba>=0.38.1,<1",
-    "lightfm>=1.15,<2",
-    "lightgbm>=2.2.1",
-    "memory_profiler>=0.54.0,<1",
-    "nltk>=3.4,<4",
-    "seaborn>=0.8.1,<1",
-    "transformers>=2.5.0,<5",
-    "bottleneck>=1.2.1,<2",
-    "category_encoders>=1.3.0,<2",
-    "jinja2>=2,<3.1",
-    "pyyaml>=5.4.1,<6",
-    "requests>=2.0.0,<3",
-    "cornac>=1.1.2,<2",
-    "retrying>=1.3.3",
-    "pandera[strategies]>=0.6.5",  # For generating fake datasets
-    "scikit-surprise>=1.0.6"
+    "category-encoders>=2.6.0,<3",  # requires packaging
+    "cornac>=1.15.2,<2",  # requires packaging, tqdm
+    "hyperopt>=0.2.7,<1",
+    "lightfm>=1.17,<2",  # requires requests
+    "lightgbm>=4.0.0,<5",
+    "locust>=2.12.2,<3",  # requires jinja2
+    "memory-profiler>=0.61.0,<1",
+    "nltk>=3.8.1,<4",  # requires tqdm
+    "notebook>=7.0.0,<8",  # requires ipykernel, jinja2, jupyter, nbconvert, nbformat, packaging, requests
+    "numba>=0.57.0,<1",
+    "pandas>2.0.0,<3.0.0",  # requires numpy
+    "pandera[strategies]>=0.6.5,<0.18;python_version<='3.8'",  # For generating fake datasets
+    "pandera[strategies]>=0.15.0;python_version>='3.9'",
+    "retrying>=1.3.4,<2",
+    "scikit-learn>=1.2.0,<2",  # requires scipy, and introduce breaking change affects feature_extraction.text.TfidfVectorizer.min_df
+    "scikit-surprise>=1.1.3",
+    "scipy>=1.10.1",
+    "seaborn>=0.13.0,<1",  # requires matplotlib, packaging
+    "transformers>=4.27.0,<5",  # requires packaging, pyyaml, requests, tqdm
 ]
 
 # shared dependencies
 extras_require = {
-    "examples": [
-        "azure.mgmt.cosmosdb>=0.8.0,<1",
-        "hyperopt>=0.1.2,<1",
-        "ipykernel>=4.6.1,<7",
-        "jupyter>=1,<2",
-        "locust>=1,<2",
-        "papermill>=2.1.2,<3",
-        "scrapbook>=0.5.0,<1.0.0",
-    ],
     "gpu": [
-        "nvidia-ml-py3>=7.352.0",
-        # TensorFlow compiled with CUDA 11.2, cudnn 8.1
-        "tensorflow~=2.6.1;python_version=='3.6'",
-        "tensorflow~=2.7.0;python_version>='3.7'",
-        "tf-slim>=1.1.0",
-        "torch>=1.8",  # for CUDA 11 support
-        "fastai>=1.0.46,<2",
+        "fastai>=2.7.11,<3",
+        "nvidia-ml-py>=11.525.84",
+        "tensorflow>=2.8.4,!=2.9.0.*,!=2.9.1,!=2.9.2,!=2.10.0.*,<2.16",  # Fixed TF due to constant security problems and breaking changes #2073
+        "tf-slim>=1.1.0",  # No python_requires in its setup.py
+        "torch>=2.0.1,<3",
     ],
     "spark": [
-        "databricks_cli>=0.8.6,<1",
-        "pyarrow>=0.12.1,<7.0.0",
-        "pyspark>=2.4.5,<4.0.0",
+        "pyarrow>=10.0.1",
+        "pyspark>=3.3.0,<=4",
     ],
     "dev": [
-        "black>=18.6b4,<21",
-        "pytest>=3.6.4",
-        "pytest-cov>=2.12.1",
-        "pytest-mock>=3.6.1",  # for access to mock fixtures in pytest
-        "pytest-rerunfailures>=10.2",  # to mark flaky tests
+        "black>=23.3.0",
+        "pytest>=7.2.1",
+        "pytest-cov>=4.1.0",
+        "pytest-mock>=3.10.0",  # for access to mock fixtures in pytest
     ],
 }
-# for the brave of heart
+# For the brave of heart
 extras_require["all"] = list(set(sum([*extras_require.values()], [])))
 
-# the following dependencies need additional testing
+# The following dependencies need additional testing
 extras_require["experimental"] = [
     # xlearn requires cmake to be pre-installed
     "xlearn==0.40a1",
     # VW C++ binary needs to be installed manually for some code to work
     "vowpalwabbit>=8.9.0,<9",
-]
-extras_require["nni"] = [
     # nni needs to be upgraded
     "nni==1.5",
+    "pymanopt>=0.2.5",
 ]
 
 # The following dependency can be installed as below, however PyPI does not allow direct URLs.
 # Temporary fix for pymanopt, only this commit works with TF2
 # "pymanopt@https://github.com/pymanopt/pymanopt/archive/fb36a272cdeecb21992cfd9271eb82baafeb316d.zip",
 
 setup(
     name="recommenders",
     version=version,
-    description="Microsoft Recommenders - Python utilities for building recommender systems",
+    description="Recommenders - Python utilities for building recommendation systems",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    url="https://github.com/microsoft/recommenders",
+    url="https://github.com/recommenders-team/recommenders",
     project_urls={
-        "Documentation": "https://microsoft-recommenders.readthedocs.io/en/stable/",
-        "Wiki": "https://github.com/microsoft/recommenders/wiki",
+        "Documentation": "https://recommenders-team.github.io/recommenders/intro.html",
+        "Wiki": "https://github.com/recommenders-team/recommenders/wiki",
     },
-    author="RecoDev Team at Microsoft",
-    author_email="RecoDevTeam@service.microsoft.com",
+    author="Recommenders contributors",
+    author_email="recommenders-technical-discuss@lists.lfaidata.foundation",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: POSIX :: Linux",
-        "Operating System :: MacOS",
     ],
     extras_require=extras_require,
     keywords="recommendations recommendation recommenders recommender system engine "
     "machine learning python spark gpu",
     install_requires=install_requires,
     package_dir={"recommenders": "recommenders"},
-    python_requires=">=3.6, <3.10",
-    packages=find_packages(where=".", exclude=["contrib", "docs", "examples", "scenarios", "tests", "tools"]),
-    setup_requires=["numpy>=1.15"]
+    python_requires=">=3.6",
+    packages=find_packages(
+        where=".",
+        exclude=["contrib", "docs", "examples", "scenarios", "tests", "tools"],
+    ),
+    setup_requires=["numpy>=1.19"],
 )
```

### Comparing `recommenders-1.1.1/tests/integration/examples/test_notebooks_gpu.py` & `recommenders-1.2.0/tests/functional/examples/test_notebooks_gpu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import pytest
 
-try:
-    import papermill as pm
-    import scrapbook as sb
-except ImportError:
-    pass  # disable error while collecting tests for non-notebook environments
-
-
 from recommenders.utils.gpu_utils import get_number_gpus
+from recommenders.utils.notebook_utils import execute_notebook, read_notebook
 
 
-TOL = 0.5
+TOL = 0.1
 ABS_TOL = 0.05
 
 
 @pytest.mark.gpu
-@pytest.mark.integration
 def test_gpu_vm():
     assert get_number_gpus() >= 1
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, epochs, expected_values, seed",
     [
         (
             "1m",
             10,
             {
@@ -40,37 +32,34 @@
                 "recall": 0.0557367,
             },
             42,
         ),
         # ("10m", 5, {"map": 0.024821, "ndcg": 0.153396, "precision": 0.143046, "recall": 0.056590})# takes too long
     ],
 )
-def test_ncf_integration(
+def test_ncf_functional(
     notebooks, output_notebook, kernel_name, size, epochs, expected_values, seed
 ):
     notebook_path = notebooks["ncf"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
             TOP_K=10, MOVIELENS_DATA_SIZE=size, EPOCHS=epochs, BATCH_SIZE=512, SEED=seed
         ),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, epochs, batch_size, expected_values, seed",
     [
         (
             "100k",
             10,
             512,
@@ -84,48 +73,45 @@
                 "precision2": 0.179533,
                 "recall2": 0.106434,
             },
             42,
         )
     ],
 )
-def test_ncf_deep_dive_integration(
+def test_ncf_deep_dive_functional(
     notebooks,
     output_notebook,
     kernel_name,
     size,
     epochs,
     batch_size,
     expected_values,
     seed,
 ):
     notebook_path = notebooks["ncf_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
             TOP_K=10,
             MOVIELENS_DATA_SIZE=size,
             EPOCHS=epochs,
             BATCH_SIZE=batch_size,
             SEED=seed,
         ),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, epochs, expected_values",
     [
         (
             "1m",
             10,
             {
@@ -138,148 +124,141 @@
                 "rsquared": 0.379963,
                 "exp_var": 0.382842,
             },
         ),
         # ("10m", 5, ), # it gets an OOM on pred = learner.model.forward(u, m)
     ],
 )
-def test_fastai_integration(
+def test_fastai_functional(
     notebooks, output_notebook, kernel_name, size, epochs, expected_values
 ):
     notebook_path = notebooks["fastai"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE=size, EPOCHS=epochs),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
-    "syn_epochs, criteo_epochs, expected_values, seed",
+    "epochs, expected_values, seed",
     [
         (
-            15,
-            10,
-            {
-                "res_syn": {"auc": 0.9716, "logloss": 0.699},
-                "res_real": {"auc": 0.749, "logloss": 0.4926},
-            },
+            5,
+            {"auc": 0.742, "logloss": 0.4964},
             42,
         )
     ],
 )
-def test_xdeepfm_integration(
+def test_xdeepfm_functional(
     notebooks,
     output_notebook,
     kernel_name,
-    syn_epochs,
-    criteo_epochs,
+    epochs,
     expected_values,
     seed,
 ):
     notebook_path = notebooks["xdeepfm_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
-            EPOCHS_FOR_SYNTHETIC_RUN=syn_epochs,
-            EPOCHS_FOR_CRITEO_RUN=criteo_epochs,
-            BATCH_SIZE_SYNTHETIC=1024,
-            BATCH_SIZE_CRITEO=1024,
+            EPOCHS=epochs,
+            BATCH_SIZE=1024,
             RANDOM_SEED=seed,
         ),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
-        assert results[key]["auc"] == pytest.approx(value["auc"], rel=TOL, abs=ABS_TOL)
-        assert results[key]["logloss"] == pytest.approx(
-            value["logloss"], rel=TOL, abs=ABS_TOL
-        )
+        assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
-    "size, steps, expected_values, seed",
+    "size, steps, batch_size, expected_values, seed",
     [
         (
-            "1m",
+            "100k",
             10000,
+            32,
             {
                 "rmse": 0.924958,
                 "mae": 0.741425,
-                "rsquared": 0.316534,
-                "exp_var": 0.322202,
+                "rsquared": 0.262963,
+                "exp_var": 0.268413,
                 "ndcg_at_k": 0.118114,
-                "map_at_k": 0.0139213,
+                "map": 0.0139213,
                 "precision_at_k": 0.107087,
                 "recall_at_k": 0.0328638,
             },
             42,
         )
     ],
 )
-def test_wide_deep_integration(
-    notebooks, output_notebook, kernel_name, size, steps, expected_values, seed, tmp
+def test_wide_deep_functional(
+    notebooks,
+    output_notebook,
+    kernel_name,
+    size,
+    steps,
+    batch_size,
+    expected_values,
+    seed,
+    tmp,
 ):
     notebook_path = notebooks["wide_deep"]
 
     params = {
         "MOVIELENS_DATA_SIZE": size,
         "STEPS": steps,
+        "BATCH_SIZE": batch_size,
         "EVALUATE_WHILE_TRAINING": False,
         "MODEL_DIR": tmp,
         "EXPORT_DIR_BASE": tmp,
         "RATING_METRICS": ["rmse", "mae", "rsquared", "exp_var"],
-        "RANKING_METRICS": ["ndcg_at_k", "map_at_k", "precision_at_k", "recall_at_k"],
+        "RANKING_METRICS": ["ndcg_at_k", "map", "precision_at_k", "recall_at_k"],
         "RANDOM_SEED": seed,
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "yaml_file, data_path, epochs, batch_size, expected_values, seed",
     [
         (
             "recommenders/models/deeprec/config/sli_rec.yaml",
             os.path.join("tests", "resources", "deeprec", "slirec"),
             10,
             400,
-            {"res_syn": {"auc": 0.7183, "logloss": 0.6045}},
+            {
+                "auc": 0.7183
+            },  # Don't do logloss check as SLi-Rec uses ranking loss, not a point-wise loss
             42,
         )
     ],
 )
-def test_slirec_quickstart_integration(
+def test_slirec_quickstart_functional(
     notebooks,
     output_notebook,
     kernel_name,
     yaml_file,
     data_path,
     epochs,
     batch_size,
@@ -291,53 +270,42 @@
     params = {
         "yaml_file": yaml_file,
         "data_path": data_path,
         "EPOCHS": epochs,
         "BATCH_SIZE": batch_size,
         "RANDOM_SEED": seed,
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    for key, value in expected_values.items():
-        assert results[key]["auc"] == pytest.approx(value["auc"], rel=TOL, abs=ABS_TOL)
-
-        ## disable logloss check, because so far SLi-Rec uses ranking loss, not a point-wise loss
-        # assert results[key]["logloss"] == pytest.approx(
-        #     value["logloss"], rel=TOL, abs=ABS_TOL
-        # )
+    assert results["auc"] == pytest.approx(expected_values["auc"], rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "epochs, batch_size, seed, MIND_type, expected_values",
     [
         (
             5,
             64,
             42,
             "demo",
             {
-                "res_syn": {
-                    "group_auc": 0.6217,
-                    "mean_mrr": 0.2783,
-                    "ndcg@5": 0.3024,
-                    "ndcg@10": 0.3719,
-                }
+                "group_auc": 0.6217,
+                "mean_mrr": 0.2783,
+                "ndcg@5": 0.3024,
+                "ndcg@10": 0.3719,
             },
         )
     ],
 )
-def test_nrms_quickstart_integration(
+def test_nrms_quickstart_functional(
     notebooks,
     output_notebook,
     kernel_name,
     epochs,
     batch_size,
     seed,
     MIND_type,
@@ -347,59 +315,53 @@
 
     params = {
         "epochs": epochs,
         "batch_size": batch_size,
         "seed": seed,
         "MIND_type": MIND_type,
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    for key, value in expected_values.items():
-        assert results[key]["group_auc"] == pytest.approx(
-            value["group_auc"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["mean_mrr"] == pytest.approx(
-            value["mean_mrr"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["ndcg@5"] == pytest.approx(
-            value["ndcg@5"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["ndcg@10"] == pytest.approx(
-            value["ndcg@10"], rel=TOL, abs=ABS_TOL
-        )
+    assert results["group_auc"] == pytest.approx(
+        expected_values["group_auc"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["mean_mrr"] == pytest.approx(
+        expected_values["mean_mrr"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["ndcg@5"] == pytest.approx(
+        expected_values["ndcg@5"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["ndcg@10"] == pytest.approx(
+        expected_values["ndcg@10"], rel=TOL, abs=ABS_TOL
+    )
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "epochs, batch_size, seed, MIND_type, expected_values",
     [
         (
             5,
             64,
             42,
             "demo",
             {
-                "res_syn": {
-                    "group_auc": 0.6436,
-                    "mean_mrr": 0.2990,
-                    "ndcg@5": 0.3297,
-                    "ndcg@10": 0.3933,
-                }
+                "group_auc": 0.6436,
+                "mean_mrr": 0.2990,
+                "ndcg@5": 0.3297,
+                "ndcg@10": 0.3933,
             },
         )
     ],
 )
-def test_naml_quickstart_integration(
+def test_naml_quickstart_functional(
     notebooks,
     output_notebook,
     kernel_name,
     batch_size,
     epochs,
     seed,
     MIND_type,
@@ -409,59 +371,53 @@
 
     params = {
         "epochs": epochs,
         "batch_size": batch_size,
         "seed": seed,
         "MIND_type": MIND_type,
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    for key, value in expected_values.items():
-        assert results[key]["group_auc"] == pytest.approx(
-            value["group_auc"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["mean_mrr"] == pytest.approx(
-            value["mean_mrr"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["ndcg@5"] == pytest.approx(
-            value["ndcg@5"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["ndcg@10"] == pytest.approx(
-            value["ndcg@10"], rel=TOL, abs=ABS_TOL
-        )
+    assert results["group_auc"] == pytest.approx(
+        expected_values["group_auc"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["mean_mrr"] == pytest.approx(
+        expected_values["mean_mrr"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["ndcg@5"] == pytest.approx(
+        expected_values["ndcg@5"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["ndcg@10"] == pytest.approx(
+        expected_values["ndcg@10"], rel=TOL, abs=ABS_TOL
+    )
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "epochs, batch_size, seed, MIND_type, expected_values",
     [
         (
             5,
             64,
             42,
             "demo",
             {
-                "res_syn": {
-                    "group_auc": 0.6444,
-                    "mean_mrr": 0.2983,
-                    "ndcg@5": 0.3287,
-                    "ndcg@10": 0.3938,
-                }
+                "group_auc": 0.6444,
+                "mean_mrr": 0.2983,
+                "ndcg@5": 0.3287,
+                "ndcg@10": 0.3938,
             },
         )
     ],
 )
-def test_lstur_quickstart_integration(
+def test_lstur_quickstart_functional(
     notebooks,
     output_notebook,
     kernel_name,
     epochs,
     batch_size,
     seed,
     MIND_type,
@@ -471,59 +427,53 @@
 
     params = {
         "epochs": epochs,
         "batch_size": batch_size,
         "seed": seed,
         "MIND_type": MIND_type,
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    for key, value in expected_values.items():
-        assert results[key]["group_auc"] == pytest.approx(
-            value["group_auc"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["mean_mrr"] == pytest.approx(
-            value["mean_mrr"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["ndcg@5"] == pytest.approx(
-            value["ndcg@5"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["ndcg@10"] == pytest.approx(
-            value["ndcg@10"], rel=TOL, abs=ABS_TOL
-        )
+    assert results["group_auc"] == pytest.approx(
+        expected_values["group_auc"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["mean_mrr"] == pytest.approx(
+        expected_values["mean_mrr"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["ndcg@5"] == pytest.approx(
+        expected_values["ndcg@5"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["ndcg@10"] == pytest.approx(
+        expected_values["ndcg@10"], rel=TOL, abs=ABS_TOL
+    )
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "epochs, batch_size, seed, MIND_type, expected_values",
     [
         (
             5,
             64,
             42,
             "demo",
             {
-                "res_syn": {
-                    "group_auc": 0.6035,
-                    "mean_mrr": 0.2765,
-                    "ndcg@5": 0.2977,
-                    "ndcg@10": 0.3637,
-                }
+                "group_auc": 0.6035,
+                "mean_mrr": 0.2765,
+                "ndcg@5": 0.2977,
+                "ndcg@10": 0.3637,
             },
         )
     ],
 )
-def test_npa_quickstart_integration(
+def test_npa_quickstart_functional(
     notebooks,
     output_notebook,
     kernel_name,
     epochs,
     batch_size,
     seed,
     MIND_type,
@@ -533,39 +483,35 @@
 
     params = {
         "epochs": epochs,
         "batch_size": batch_size,
         "seed": seed,
         "MIND_type": MIND_type,
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    for key, value in expected_values.items():
-        assert results[key]["group_auc"] == pytest.approx(
-            value["group_auc"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["mean_mrr"] == pytest.approx(
-            value["mean_mrr"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["ndcg@5"] == pytest.approx(
-            value["ndcg@5"], rel=TOL, abs=ABS_TOL
-        )
-        assert results[key]["ndcg@10"] == pytest.approx(
-            value["ndcg@10"], rel=TOL, abs=ABS_TOL
-        )
+    assert results["group_auc"] == pytest.approx(
+        expected_values["group_auc"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["mean_mrr"] == pytest.approx(
+        expected_values["mean_mrr"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["ndcg@5"] == pytest.approx(
+        expected_values["ndcg@5"], rel=TOL, abs=ABS_TOL
+    )
+    assert results["ndcg@10"] == pytest.approx(
+        expected_values["ndcg@10"], rel=TOL, abs=ABS_TOL
+    )
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "yaml_file, data_path, size, epochs, batch_size, expected_values, seed",
     [
         (
             "recommenders/models/deeprec/config/lightgcn.yaml",
             os.path.join("tests", "resources", "deeprec", "lightgcn"),
             "100k",
@@ -577,149 +523,163 @@
                 "precision": 0.308165,
                 "recall": 0.163034,
             },
             42,
         )
     ],
 )
-def test_lightgcn_deep_dive_integration(
+def test_lightgcn_deep_dive_functional(
     notebooks,
     output_notebook,
     kernel_name,
     yaml_file,
     data_path,
     size,
     epochs,
     batch_size,
     expected_values,
     seed,
 ):
     notebook_path = notebooks["lightgcn_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
             TOP_K=10,
             MOVIELENS_DATA_SIZE=size,
             EPOCHS=epochs,
             BATCH_SIZE=batch_size,
             SEED=seed,
             yaml_file=yaml_file,
             user_file=os.path.join(data_path, r"user_embeddings"),
             item_file=os.path.join(data_path, r"item_embeddings"),
         ),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
-def test_dkn_quickstart_integration(notebooks, output_notebook, kernel_name):
+def test_dkn_quickstart_functional(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["dkn_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(epochs=5, batch_size=500),
+        parameters=dict(EPOCHS=5, BATCH_SIZE=200),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    assert results["res"]["auc"] == pytest.approx(0.5651, rel=TOL, abs=ABS_TOL)
-    assert results["res"]["mean_mrr"] == pytest.approx(0.1639, rel=TOL, abs=ABS_TOL)
-    assert results["res"]["ndcg@5"] == pytest.approx(0.1735, rel=TOL, abs=ABS_TOL)
-    assert results["res"]["ndcg@10"] == pytest.approx(0.2301, rel=TOL, abs=ABS_TOL)
+    assert results["auc"] == pytest.approx(0.5651, rel=TOL, abs=ABS_TOL)
+    assert results["mean_mrr"] == pytest.approx(0.1639, rel=TOL, abs=ABS_TOL)
+    assert results["ndcg@5"] == pytest.approx(0.1735, rel=TOL, abs=ABS_TOL)
+    assert results["ndcg@10"] == pytest.approx(0.2301, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, expected_values",
     [
         ("1m", dict(map=0.081794, ndcg=0.400983, precision=0.367997, recall=0.138352)),
         # 10m works but takes too long
     ],
 )
-def test_cornac_bivae_integration(
+def test_cornac_bivae_functional(
     notebooks, output_notebook, kernel_name, size, expected_values
 ):
     notebook_path = notebooks["cornac_bivae_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(MOVIELENS_DATA_SIZE=size),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.gpu
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
-    "data_dir, num_epochs, batch_size, model_name, expected_values, seed",
+    "data_dir, num_epochs, batch_size, model_name, expected_values",
     [
         (
             os.path.join("tests", "recsys_data", "RecSys", "SASRec-tf2", "data"),
             1,
             128,
             "sasrec",
-            {"ndcg@10": 0.2626, "Hit@10": 0.4244},
-            42,
+            {"ndcg@10": 0.2297, "Hit@10": 0.3789},
         ),
         (
             os.path.join("tests", "recsys_data", "RecSys", "SASRec-tf2", "data"),
             1,
             128,
             "ssept",
-            {"ndcg@10": 0.2626, "Hit@10": 0.4244},
-            42,
+            {"ndcg@10": 0.2245, "Hit@10": 0.3743},
         ),
     ],
 )
-def test_sasrec_quickstart_integration(
+def test_sasrec_quickstart_functional(
     notebooks,
     output_notebook,
     kernel_name,
     data_dir,
     num_epochs,
     batch_size,
     model_name,
     expected_values,
-    seed,
 ):
     notebook_path = notebooks["sasrec_quickstart"]
     params = {
         "data_dir": data_dir,
         "num_epochs": num_epochs,
         "batch_size": batch_size,
         "model_name": model_name,
-        "seed": seed,
     }
-
-    print("Executing notebook ... ")
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=params,
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
+
+
+@pytest.mark.gpu
+@pytest.mark.notebooks
+@pytest.mark.parametrize(
+    "size, algos, expected_values_ndcg",
+    [
+        (
+            ["100k"],
+            ["ncf", "fastai", "bivae", "lightgcn"],
+            [0.382793, 0.147583, 0.471722, 0.412664],
+        ),
+    ],
+)
+def test_benchmark_movielens_gpu(
+    notebooks, output_notebook, kernel_name, size, algos, expected_values_ndcg
+):
+    notebook_path = notebooks["benchmark_movielens"]
+    execute_notebook(
+        notebook_path,
+        output_notebook,
+        kernel_name=kernel_name,
+        parameters=dict(data_sizes=size, algorithms=algos),
+    )
+    results = read_notebook(output_notebook)
+
+    assert len(results) == 4
+    for i, value in enumerate(algos):
+        assert results[value] == pytest.approx(
+            expected_values_ndcg[i], rel=TOL, abs=ABS_TOL
+        )
```

### Comparing `recommenders-1.1.1/tests/integration/examples/test_notebooks_pyspark.py` & `recommenders-1.2.0/tests/functional/examples/test_notebooks_pyspark.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+import os
 import sys
 import pytest
 
-try:
-    import papermill as pm
-    import scrapbook as sb
-except ImportError:
-    pass  # disable error while collecting tests for non-notebook environments
+from recommenders.utils.notebook_utils import execute_notebook, read_notebook
 
 
 TOL = 0.05
 ABS_TOL = 0.05
 
 
 # This is a flaky test that can fail unexpectedly
 @pytest.mark.flaky(reruns=5, reruns_delay=2)
 @pytest.mark.spark
 @pytest.mark.notebooks
-@pytest.mark.integration
-def test_als_pyspark_integration(notebooks, output_notebook, kernel_name):
+def test_als_pyspark_functional(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["als_pyspark"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE="1m"),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     assert results["map"] == pytest.approx(0.00201, rel=TOL, abs=ABS_TOL)
     assert results["ndcg"] == pytest.approx(0.02516, rel=TOL, abs=ABS_TOL)
     assert results["precision"] == pytest.approx(0.03172, rel=TOL, abs=ABS_TOL)
     assert results["recall"] == pytest.approx(0.009302, rel=TOL, abs=ABS_TOL)
     assert results["rmse"] == pytest.approx(0.8621, rel=TOL, abs=ABS_TOL)
     assert results["mae"] == pytest.approx(0.68023, rel=TOL, abs=ABS_TOL)
@@ -42,23 +36,52 @@
     assert results["rsquared"] == pytest.approx(0.4038, rel=TOL, abs=ABS_TOL)
 
 
 # This is a flaky test that can fail unexpectedly
 @pytest.mark.flaky(reruns=5, reruns_delay=2)
 @pytest.mark.spark
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.skip(reason="It takes too long in the current test machine")
 @pytest.mark.skipif(sys.platform == "win32", reason="Not implemented on Windows")
-def test_mmlspark_lightgbm_criteo_integration(notebooks, output_notebook, kernel_name):
+def test_mmlspark_lightgbm_criteo_functional(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["mmlspark_lightgbm_criteo"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(DATA_SIZE="full", NUM_ITERATIONS=50),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     assert results["auc"] == pytest.approx(0.68895, rel=TOL, abs=ABS_TOL)
+
+
+@pytest.mark.spark
+@pytest.mark.notebooks
+@pytest.mark.parametrize(
+    "size, algos, expected_values_ndcg",
+    [
+        (["100k"], ["als"], [0.035812]),
+    ],
+)
+def test_benchmark_movielens_pyspark(
+    notebooks, output_notebook, kernel_name, size, algos, expected_values_ndcg
+):
+    notebook_path = notebooks["benchmark_movielens"]
+
+    os.environ["PYSPARK_PYTHON"] = sys.executable
+    os.environ["PYSPARK_DRIVER_PYTHON"] = sys.executable
+    os.environ.pop("SPARK_HOME", None)
+
+    execute_notebook(
+        notebook_path,
+        output_notebook,
+        kernel_name=kernel_name,
+        parameters=dict(data_sizes=size, algorithms=algos),
+    )
+    results = read_notebook(output_notebook)
+
+    assert len(results) == 1
+    for i, value in enumerate(algos):
+        assert results[value] == pytest.approx(
+            expected_values_ndcg[i], rel=TOL, abs=ABS_TOL
+        )
```

### Comparing `recommenders-1.1.1/tests/integration/examples/test_notebooks_python.py` & `recommenders-1.2.0/tests/functional/examples/test_notebooks_python.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import sys
 import pytest
 
-try:
-    import papermill as pm
-    import scrapbook as sb
-except ImportError:
-    pass  # disable error while collecting tests for non-notebook environments
+from recommenders.utils.notebook_utils import execute_notebook, read_notebook
 
 
 TOL = 0.05
 ABS_TOL = 0.05
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, expected_values",
     [
         (
             "1m",
             {
                 "map": 0.060579,
@@ -36,34 +30,31 @@
                 "ndcg": 0.319625,
                 "precision": 0.275756,
                 "recall": 0.154014,
             },
         ),
     ],
 )
-def test_sar_single_node_integration(
+def test_sar_single_node_functional(
     notebooks, output_notebook, kernel_name, size, expected_values
 ):
     notebook_path = notebooks["sar_single_node"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE=size),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, expected_values",
     [
         (
             "1m",
             {
                 "map": 0.033914,
@@ -71,34 +62,31 @@
                 "precision": 0.211923,
                 "recall": 0.064663,
             },
         ),
         # ("10m", {"map": , "ndcg": , "precision": , "recall": }), # OOM on test machine
     ],
 )
-def test_baseline_deep_dive_integration(
+def test_baseline_deep_dive_functional(
     notebooks, output_notebook, kernel_name, size, expected_values
 ):
     notebook_path = notebooks["baseline_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE=size),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, expected_values",
     [
         (
             "1m",
             dict(
                 rmse=0.89,
@@ -110,34 +98,31 @@
                 precision=0.093,
                 recall=0.025,
             ),
         ),
         # 10m works but takes too long
     ],
 )
-def test_surprise_svd_integration(
+def test_surprise_svd_functional(
     notebooks, output_notebook, kernel_name, size, expected_values
 ):
     notebook_path = notebooks["surprise_svd_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(MOVIELENS_DATA_SIZE=size),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, expected_values",
     [
         (
             "1m",
             dict(
                 rmse=0.959885,
@@ -149,38 +134,35 @@
                 precision=0.061142,
                 recall=0.017789,
             ),
         )
     ],
 )
 @pytest.mark.skip(reason="VW pip package has installation incompatibilities")
-def test_vw_deep_dive_integration(
+def test_vw_deep_dive_functional(
     notebooks, output_notebook, kernel_name, size, expected_values
 ):
     notebook_path = notebooks["vowpal_wabbit_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(MOVIELENS_DATA_SIZE=size, TOP_K=10),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.skip(reason="NNI pip package has installation incompatibilities")
 def test_nni_tuning_svd(notebooks, output_notebook, kernel_name, tmp):
     notebook_path = notebooks["nni_tuning_svd"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
             MOVIELENS_DATA_SIZE="100k",
             SURPRISE_READER="ml-100k",
             TMP_DIR=tmp,
@@ -189,123 +171,119 @@
             WAITING_TIME=20,
             MAX_RETRIES=50,
         ),
     )
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
-@pytest.mark.skip(reason="Wikidata API is unstable")
-def test_wikidata_integration(notebooks, output_notebook, kernel_name, tmp):
-    notebook_path = notebooks["wikidata_knowledge_graph"]
-    pm.execute_notebook(
-        notebook_path,
-        output_notebook,
-        kernel_name=kernel_name,
-        parameters=dict(
-            MOVIELENS_DATA_SIZE="100k", MOVIELENS_SAMPLE=True, MOVIELENS_SAMPLE_SIZE=5
-        ),
-    )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
-
-    # NOTE: The return number should be always 5, but sometimes we get less because wikidata is unstable
-    assert results["length_result"] >= 1
-
-
-@pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, expected_values",
     [
         ("1m", dict(map=0.081390, ndcg=0.406627, precision=0.373228, recall=0.132444)),
         # 10m works but takes too long
     ],
 )
-def test_cornac_bpr_integration(
+def test_cornac_bpr_functional(
     notebooks, output_notebook, kernel_name, size, expected_values
 ):
     notebook_path = notebooks["cornac_bpr_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(MOVIELENS_DATA_SIZE=size),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.parametrize(
     "size, epochs, expected_values",
     [
         (
             "100k",
-            10,
+            3,
             dict(
                 eval_precision=0.131601,
                 eval_recall=0.038056,
                 eval_precision2=0.145599,
                 eval_recall2=0.051338,
             ),
         ),
     ],
 )
-def test_lightfm_integration(
+@pytest.mark.skip(reason="LightFM notebook takes too long to run. Review issue #1707")
+def test_lightfm_functional(
     notebooks, output_notebook, kernel_name, size, epochs, expected_values
 ):
     notebook_path = notebooks["lightfm_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(MOVIELENS_DATA_SIZE=size, NO_EPOCHS=epochs),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.experimental
 @pytest.mark.parametrize(
     "expected_values",
     [({"rmse": 0.4969, "mae": 0.4761})],
 )
-def test_geoimc_integration(notebooks, output_notebook, kernel_name, expected_values):
+@pytest.mark.skip(reason="geoimc doesn't work with any officially released pymanopt package")
+def test_geoimc_functional(notebooks, output_notebook, kernel_name, expected_values):
     notebook_path = notebooks["geoimc_quickstart"]
-    pm.execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
+    results = read_notebook(output_notebook)
 
     for key, value in expected_values.items():
         assert results[key] == pytest.approx(value, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.integration
 @pytest.mark.experimental
-def test_xlearn_fm_integration(notebooks, output_notebook, kernel_name):
+@pytest.mark.skip(reason="xLearn pip package has installation incompatibilities")
+def test_xlearn_fm_functional(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["xlearn_fm_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(LEARNING_RATE=0.2, EPOCH=10),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     assert results["auc_score"] == pytest.approx(0.75, rel=TOL, abs=ABS_TOL)
+
+
+@pytest.mark.notebooks
+@pytest.mark.parametrize(
+    "size, algos, expected_values_ndcg",
+    [
+        (["100k"], ["svd", "sar", "bpr"], [0.094444, 0.393818, 0.444990]),
+    ],
+)
+def test_benchmark_movielens_cpu(
+    notebooks, output_notebook, kernel_name, size, algos, expected_values_ndcg
+):
+    notebook_path = notebooks["benchmark_movielens"]
+    execute_notebook(
+        notebook_path,
+        output_notebook,
+        kernel_name=kernel_name,
+        parameters=dict(data_sizes=size, algorithms=algos),
+    )
+    results = read_notebook(output_notebook)
+
+    assert len(results) == 3
+    for i, value in enumerate(algos):
+        assert results[value] == pytest.approx(
+            expected_values_ndcg[i], rel=TOL, abs=ABS_TOL
+        )
```

### Comparing `recommenders-1.1.1/tests/smoke/examples/test_notebooks_gpu.py` & `recommenders-1.2.0/tests/smoke/examples/test_notebooks_gpu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,258 +1,216 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 import pytest
 
-try:
-    import papermill as pm
-    import scrapbook as sb
-except ImportError:
-    pass  # disable error while collecting tests for non-notebook environments
-
 from recommenders.utils.gpu_utils import get_number_gpus
+from recommenders.utils.notebook_utils import execute_notebook, read_notebook
 
 
 TOL = 0.5
 ABS_TOL = 0.05
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_gpu_vm():
     assert get_number_gpus() >= 1
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_ncf_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["ncf"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE="100k", EPOCHS=1, BATCH_SIZE=256),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     assert results["map"] == pytest.approx(0.0409234, rel=TOL, abs=ABS_TOL)
     assert results["ndcg"] == pytest.approx(0.1773, rel=TOL, abs=ABS_TOL)
     assert results["precision"] == pytest.approx(0.160127, rel=TOL, abs=ABS_TOL)
     assert results["recall"] == pytest.approx(0.0879193, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_ncf_deep_dive_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["ncf_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(
-            TOP_K=10, MOVIELENS_DATA_SIZE="100k", EPOCHS=1, BATCH_SIZE=1024
-        ),
+        parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE="100k", EPOCHS=1, BATCH_SIZE=1024),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     # There is too much variability to do an approx equal, just adding top values
     assert results["map"] == pytest.approx(0.0370396, rel=TOL, abs=ABS_TOL)
     assert results["ndcg"] == pytest.approx(0.29423, rel=TOL, abs=ABS_TOL)
     assert results["precision"] == pytest.approx(0.144539, rel=TOL, abs=ABS_TOL)
     assert results["recall"] == pytest.approx(0.0730272, rel=TOL, abs=ABS_TOL)
     assert results["map2"] == pytest.approx(0.028952, rel=TOL, abs=ABS_TOL)
     assert results["ndcg2"] == pytest.approx(0.143744, rel=TOL, abs=ABS_TOL)
     assert results["precision2"] == pytest.approx(0.127041, rel=TOL, abs=ABS_TOL)
     assert results["recall2"] == pytest.approx(0.0584491, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_fastai_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["fastai"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE="100k", EPOCHS=1),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     assert results["rmse"] == pytest.approx(0.959352, rel=TOL, abs=ABS_TOL)
     assert results["mae"] == pytest.approx(0.766504, rel=TOL, abs=ABS_TOL)
     assert results["rsquared"] == pytest.approx(0.287902, rel=TOL, abs=ABS_TOL)
     assert results["exp_var"] == pytest.approx(0.289008, rel=TOL, abs=ABS_TOL)
     assert results["map"] == pytest.approx(0.024379, rel=TOL, abs=ABS_TOL)
     assert results["ndcg"] == pytest.approx(0.148380, rel=TOL, abs=ABS_TOL)
     assert results["precision"] == pytest.approx(0.138494, rel=TOL, abs=ABS_TOL)
     assert results["recall"] == pytest.approx(0.058747, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_xdeepfm_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["xdeepfm_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
-            EPOCHS_FOR_SYNTHETIC_RUN=1,
-            EPOCHS_FOR_CRITEO_RUN=1,
-            BATCH_SIZE_SYNTHETIC=128,
-            BATCH_SIZE_CRITEO=512,
+            EPOCHS=1,
+            BATCH_SIZE=512,
             RANDOM_SEED=42,
         ),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
-
-    assert results["res_syn"]["auc"] == pytest.approx(0.5043, rel=TOL, abs=ABS_TOL)
-    assert results["res_syn"]["logloss"] == pytest.approx(0.7046, rel=TOL, abs=ABS_TOL)
-    assert results["res_real"]["auc"] == pytest.approx(0.7251, rel=TOL, abs=ABS_TOL)
-    assert results["res_real"]["logloss"] == pytest.approx(0.508, rel=TOL, abs=ABS_TOL)
+    results = read_notebook(output_notebook)
+
+    assert results["auc"] == pytest.approx(0.7251, rel=TOL, abs=ABS_TOL)
+    assert results["logloss"] == pytest.approx(0.508, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_wide_deep_smoke(notebooks, output_notebook, kernel_name, tmp):
     notebook_path = notebooks["wide_deep"]
 
     params = {
         "MOVIELENS_DATA_SIZE": "100k",
         "STEPS": 1000,
         "EVALUATE_WHILE_TRAINING": False,
         "MODEL_DIR": tmp,
         "EXPORT_DIR_BASE": tmp,
         "RATING_METRICS": ["rmse", "mae"],
         "RANKING_METRICS": ["ndcg_at_k", "precision_at_k"],
         "RANDOM_SEED": 42,
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     assert results["rmse"] == pytest.approx(1.06034, rel=TOL, abs=ABS_TOL)
     assert results["mae"] == pytest.approx(0.876228, rel=TOL, abs=ABS_TOL)
     assert results["ndcg_at_k"] == pytest.approx(0.181513, rel=TOL, abs=ABS_TOL)
     assert results["precision_at_k"] == pytest.approx(0.158961, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_naml_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["naml_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(epochs=1, seed=42, MIND_type="demo"),
+        parameters=dict(epochs=1, batch_size=64, seed=42, MIND_type="demo"),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    assert results["res_syn"]["group_auc"] == pytest.approx(
+    assert results["group_auc"] == pytest.approx(
         0.5801, rel=TOL, abs=ABS_TOL
     )
-    assert results["res_syn"]["mean_mrr"] == pytest.approx(0.2512, rel=TOL, abs=ABS_TOL)
+    assert results["mean_mrr"] == pytest.approx(0.2512, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_nrms_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["nrms_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(epochs=1, seed=42, MIND_type="demo"),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    assert results["res_syn"]["group_auc"] == pytest.approx(
+    assert results["group_auc"] == pytest.approx(
         0.5768, rel=TOL, abs=ABS_TOL
     )
-    assert results["res_syn"]["mean_mrr"] == pytest.approx(0.2457, rel=TOL, abs=ABS_TOL)
+    assert results["mean_mrr"] == pytest.approx(0.2457, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_npa_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["npa_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(epochs=1, seed=42, MIND_type="demo"),
+        parameters=dict(epochs=1, batch_size=64, seed=42, MIND_type="demo"),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    assert results["res_syn"]["group_auc"] == pytest.approx(
+    assert results["group_auc"] == pytest.approx(
         0.5861, rel=TOL, abs=ABS_TOL
     )
-    assert results["res_syn"]["mean_mrr"] == pytest.approx(0.255, rel=TOL, abs=ABS_TOL)
+    assert results["mean_mrr"] == pytest.approx(0.255, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_lstur_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["lstur_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(epochs=1, seed=40, MIND_type="demo"),
+        parameters=dict(epochs=1, batch_size=64, seed=40, MIND_type="demo"),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
-    assert results["res_syn"]["group_auc"] == pytest.approx(
+    assert results["group_auc"] == pytest.approx(
         0.5977, rel=TOL, abs=ABS_TOL
     )
-    assert results["res_syn"]["mean_mrr"] == pytest.approx(0.2618, rel=TOL, abs=ABS_TOL)
+    assert results["mean_mrr"] == pytest.approx(0.2618, rel=TOL, abs=ABS_TOL)
 
 
 @pytest.mark.notebooks
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_cornac_bivae_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["cornac_bivae_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(MOVIELENS_DATA_SIZE="100k"),
     )
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     assert results["map"] == pytest.approx(0.146552, rel=TOL, abs=ABS_TOL)
     assert results["ndcg"] == pytest.approx(0.474124, rel=TOL, abs=ABS_TOL)
     assert results["precision"] == pytest.approx(0.412527, rel=TOL, abs=ABS_TOL)
     assert results["recall"] == pytest.approx(0.225064, rel=TOL, abs=ABS_TOL)
```

### Comparing `recommenders-1.1.1/tests/smoke/examples/test_notebooks_pyspark.py` & `recommenders-1.2.0/tests/smoke/examples/test_notebooks_pyspark.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,55 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import sys
 import pytest
 
-try:
-    import papermill as pm
-    import scrapbook as sb
-except ImportError:
-    pass  # disable error while collecting tests for non-notebook environments
+from recommenders.utils.notebook_utils import execute_notebook, read_notebook
 
 
 TOL = 0.05
 ABS_TOL = 0.05
 
 
 # This is a flaky test that can fail unexpectedly
 @pytest.mark.flaky(reruns=5, reruns_delay=2)
-@pytest.mark.smoke
 @pytest.mark.spark
 @pytest.mark.notebooks
 def test_als_pyspark_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["als_pyspark"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE="100k"),
     )
 
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
 
     assert results["map"] == pytest.approx(0.0052, rel=TOL, abs=ABS_TOL)
     assert results["ndcg"] == pytest.approx(0.0463, rel=TOL, abs=ABS_TOL)
     assert results["precision"] == pytest.approx(0.0487, rel=TOL, abs=ABS_TOL)
     assert results["recall"] == pytest.approx(0.0177, rel=TOL, abs=ABS_TOL)
     assert results["rmse"] == pytest.approx(0.9636, rel=TOL, abs=ABS_TOL)
     assert results["mae"] == pytest.approx(0.7508, rel=TOL, abs=ABS_TOL)
     assert results["exp_var"] == pytest.approx(0.2672, rel=TOL, abs=ABS_TOL)
     assert results["rsquared"] == pytest.approx(0.2611, rel=TOL, abs=ABS_TOL)
 
 
 # This is a flaky test that can fail unexpectedly
 @pytest.mark.flaky(reruns=5, reruns_delay=2)
-@pytest.mark.smoke
 @pytest.mark.spark
 @pytest.mark.notebooks
 @pytest.mark.skipif(sys.platform == "win32", reason="Not implemented on Windows")
 def test_mmlspark_lightgbm_criteo_smoke(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["mmlspark_lightgbm_criteo"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(DATA_SIZE="sample", NUM_ITERATIONS=50),
     )
 
-    results = sb.read_notebook(output_notebook).scraps.dataframe.set_index("name")[
-        "data"
-    ]
+    results = read_notebook(output_notebook)
     assert results["auc"] == pytest.approx(0.65, rel=TOL, abs=ABS_TOL)
```

### Comparing `recommenders-1.1.1/tests/smoke/recommenders/dataset/test_mind.py` & `recommenders-1.2.0/tests/data_validation/recommenders/datasets/test_mind.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import pytest
 import os
+import pytest
 import requests
+
 from recommenders.datasets.mind import download_mind, extract_mind
 
 
-@pytest.mark.smoke
 @pytest.mark.parametrize(
     "url, content_length, etag",
     [
         (
             "https://recodatasets.z20.web.core.windows.net/newsrec/MINDdemo_train.zip",
             "17372879",
             '"0x8D8B8AD5B233930"',
@@ -60,49 +60,96 @@
 )
 def test_mind_url(url, content_length, etag):
     url_headers = requests.head(url).headers
     assert url_headers["Content-Length"] == content_length
     assert url_headers["ETag"] == etag
 
 
-@pytest.mark.smoke
-@pytest.mark.parametrize("size", [("demo"), ("small")])
-def test_extract_mind(size, tmp):
-    train_zip, valid_zip = download_mind(size, dest_path=tmp)
+def test_download_mind_demo(tmp):
+    train_path, valid_path = download_mind(size="demo", dest_path=tmp)
+    statinfo = os.stat(train_path)
+    assert statinfo.st_size == 17372879
+    statinfo = os.stat(valid_path)
+    assert statinfo.st_size == 10080022
+
+
+def test_download_mind_small(tmp):
+    train_path, valid_path = download_mind(size="small", dest_path=tmp)
+    statinfo = os.stat(train_path)
+    assert statinfo.st_size == 52952752
+    statinfo = os.stat(valid_path)
+    assert statinfo.st_size == 30945572
+
+
+def test_extract_mind_demo(tmp):
+    train_zip, valid_zip = download_mind(size="demo", dest_path=tmp)
+    train_path, valid_path = extract_mind(train_zip, valid_zip, clean_zip_file=False)
+
+    statinfo = os.stat(os.path.join(train_path, "behaviors.tsv"))
+    assert statinfo.st_size == 14707247
+    statinfo = os.stat(os.path.join(train_path, "entity_embedding.vec"))
+    assert statinfo.st_size == 16077470
+    statinfo = os.stat(os.path.join(train_path, "news.tsv"))
+    assert statinfo.st_size == 23120370
+    statinfo = os.stat(os.path.join(train_path, "relation_embedding.vec"))
+    assert statinfo.st_size == 1044588
+    statinfo = os.stat(os.path.join(valid_path, "behaviors.tsv"))
+    assert statinfo.st_size == 4434762
+    statinfo = os.stat(os.path.join(valid_path, "entity_embedding.vec"))
+    assert statinfo.st_size == 11591565
+    statinfo = os.stat(os.path.join(valid_path, "news.tsv"))
+    assert statinfo.st_size == 15624320
+    statinfo = os.stat(os.path.join(valid_path, "relation_embedding.vec"))
+    assert statinfo.st_size == 1044588
+
+
+def test_extract_mind_small(tmp):
+    train_zip, valid_zip = download_mind(size="small", dest_path=tmp)
     train_path, valid_path = extract_mind(train_zip, valid_zip, clean_zip_file=False)
 
-    if size == "demo":
-        statinfo = os.stat(os.path.join(train_path, "behaviors.tsv"))
-        assert statinfo.st_size == 14707247
-        statinfo = os.stat(os.path.join(train_path, "entity_embedding.vec"))
-        assert statinfo.st_size == 16077470
-        statinfo = os.stat(os.path.join(train_path, "news.tsv"))
-        assert statinfo.st_size == 23120370
-        statinfo = os.stat(os.path.join(train_path, "relation_embedding.vec"))
-        assert statinfo.st_size == 1044588
-        statinfo = os.stat(os.path.join(valid_path, "behaviors.tsv"))
-        assert statinfo.st_size == 4434762
-        statinfo = os.stat(os.path.join(valid_path, "entity_embedding.vec"))
-        assert statinfo.st_size == 11591565
-        statinfo = os.stat(os.path.join(valid_path, "news.tsv"))
-        assert statinfo.st_size == 15624320
-        statinfo = os.stat(os.path.join(valid_path, "relation_embedding.vec"))
-        assert statinfo.st_size == 1044588
-    elif size == "small":
-        statinfo = os.stat(os.path.join(train_path, "behaviors.tsv"))
-        assert statinfo.st_size == 92019716
-        statinfo = os.stat(os.path.join(train_path, "entity_embedding.vec"))
-        assert statinfo.st_size == 25811015
-        statinfo = os.stat(os.path.join(train_path, "news.tsv"))
-        assert statinfo.st_size == 41202121
-        statinfo = os.stat(os.path.join(train_path, "relation_embedding.vec"))
-        assert statinfo.st_size == 1044588
-        statinfo = os.stat(os.path.join(valid_path, "behaviors.tsv"))
-        assert statinfo.st_size == 42838544
-        statinfo = os.stat(os.path.join(valid_path, "entity_embedding.vec"))
-        assert statinfo.st_size == 21960998
-        statinfo = os.stat(os.path.join(valid_path, "news.tsv"))
-        assert statinfo.st_size == 33519092
-        statinfo = os.stat(os.path.join(valid_path, "relation_embedding.vec"))
-        assert statinfo.st_size == 1044588
-    else:
-        assert False
+    statinfo = os.stat(os.path.join(train_path, "behaviors.tsv"))
+    assert statinfo.st_size == 92019716
+    statinfo = os.stat(os.path.join(train_path, "entity_embedding.vec"))
+    assert statinfo.st_size == 25811015
+    statinfo = os.stat(os.path.join(train_path, "news.tsv"))
+    assert statinfo.st_size == 41202121
+    statinfo = os.stat(os.path.join(train_path, "relation_embedding.vec"))
+    assert statinfo.st_size == 1044588
+    statinfo = os.stat(os.path.join(valid_path, "behaviors.tsv"))
+    assert statinfo.st_size == 42838544
+    statinfo = os.stat(os.path.join(valid_path, "entity_embedding.vec"))
+    assert statinfo.st_size == 21960998
+    statinfo = os.stat(os.path.join(valid_path, "news.tsv"))
+    assert statinfo.st_size == 33519092
+    statinfo = os.stat(os.path.join(valid_path, "relation_embedding.vec"))
+    assert statinfo.st_size == 1044588
+
+
+def test_download_mind_large(tmp_path):
+    train_path, valid_path = download_mind(size="large", dest_path=tmp_path)
+    statinfo = os.stat(train_path)
+    assert statinfo.st_size == 530196631
+    statinfo = os.stat(valid_path)
+    assert statinfo.st_size == 103456245
+
+
+def test_extract_mind_large(tmp):
+    train_zip, valid_zip = download_mind(size="large", dest_path=tmp)
+    train_path, valid_path = extract_mind(train_zip, valid_zip)
+
+    statinfo = os.stat(os.path.join(train_path, "behaviors.tsv"))
+    assert statinfo.st_size == 1373844151
+    statinfo = os.stat(os.path.join(train_path, "entity_embedding.vec"))
+    assert statinfo.st_size == 40305151
+    statinfo = os.stat(os.path.join(train_path, "news.tsv"))
+    assert statinfo.st_size == 84881998
+    statinfo = os.stat(os.path.join(train_path, "relation_embedding.vec"))
+    assert statinfo.st_size == 1044588
+
+    statinfo = os.stat(os.path.join(valid_path, "behaviors.tsv"))
+    assert statinfo.st_size == 230662527
+    statinfo = os.stat(os.path.join(valid_path, "entity_embedding.vec"))
+    assert statinfo.st_size == 31958202
+    statinfo = os.stat(os.path.join(valid_path, "news.tsv"))
+    assert statinfo.st_size == 59055351
+    statinfo = os.stat(os.path.join(valid_path, "relation_embedding.vec"))
+    assert statinfo.st_size == 1044588
```

### Comparing `recommenders-1.1.1/tests/smoke/recommenders/recommender/test_deeprec_model.py` & `recommenders-1.2.0/tests/smoke/recommenders/recommender/test_deeprec_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import pytest
 
+from recommenders.datasets import movielens
+from recommenders.datasets.python_splitters import python_stratified_split
+
 try:
     import tensorflow as tf
     from recommenders.models.deeprec.deeprec_utils import (
         download_deeprec_resources,
         prepare_hparams,
     )
     from recommenders.models.deeprec.models.base_model import BaseModel
     from recommenders.models.deeprec.models.xDeepFM import XDeepFMModel
     from recommenders.models.deeprec.models.dkn import DKN
     from recommenders.models.deeprec.io.iterator import FFMTextIterator
     from recommenders.models.deeprec.io.dkn_iterator import DKNTextIterator
     from recommenders.models.deeprec.io.sequential_iterator import SequentialIterator
     from recommenders.models.deeprec.models.sequential.sli_rec import SLI_RECModel
-    from recommenders.models.deeprec.models.sequential.sum import SUMModel
     from recommenders.datasets.amazon_reviews import (
         download_and_extract,
         data_preprocessing,
     )
     from recommenders.models.deeprec.models.graphrec.lightgcn import LightGCN
     from recommenders.models.deeprec.DataModel.ImplicitCF import ImplicitCF
-    from recommenders.datasets import movielens
-    from recommenders.datasets.python_splitters import python_stratified_split
+
 except ImportError:
     pass  # disable error while collecting tests for non-gpu environments
 
+try:
+    from recommenders.models.deeprec.models.sequential.sum import SUMModel
+except ImportError:
+    pass  # disable error while collecting tests for SUMModel
+
 
-@pytest.mark.smoke
 @pytest.mark.gpu
-@pytest.mark.deeprec
 def test_FFM_iterator(deeprec_resource_path):
     data_path = os.path.join(deeprec_resource_path, "xdeepfm")
     yaml_file = os.path.join(data_path, "xDeepFM.yaml")
     data_file = os.path.join(data_path, "sample_FFM_data.txt")
 
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
@@ -48,17 +52,15 @@
     hparams = prepare_hparams(yaml_file)
     iterator = FFMTextIterator(hparams, tf.Graph())
     assert iterator is not None
     for res in iterator.load_data_from_file(data_file):
         assert isinstance(res, tuple)
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
-@pytest.mark.deeprec
 def test_model_xdeepfm(deeprec_resource_path):
     data_path = os.path.join(deeprec_resource_path, "xdeepfm")
     yaml_file = os.path.join(data_path, "xDeepFM.yaml")
     data_file = os.path.join(data_path, "sample_FFM_data.txt")
     output_file = os.path.join(data_path, "output.txt")
 
     if not os.path.exists(yaml_file):
@@ -75,17 +77,15 @@
     model = XDeepFMModel(hparams, input_creator)
 
     assert model.run_eval(data_file) is not None
     assert isinstance(model.fit(data_file, data_file), BaseModel)
     assert model.predict(data_file, output_file) is not None
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
-@pytest.mark.deeprec
 def test_model_dkn(deeprec_resource_path):
     data_path = os.path.join(deeprec_resource_path, "dkn")
     yaml_file = os.path.join(data_path, r"dkn.yaml")
     train_file = os.path.join(data_path, r"train_mind_demo.txt")
     valid_file = os.path.join(data_path, r"valid_mind_demo.txt")
     news_feature_file = os.path.join(data_path, r"doc_feature.txt")
     user_history_file = os.path.join(data_path, r"user_history.txt")
@@ -112,18 +112,15 @@
     input_creator = DKNTextIterator
     model = DKN(hparams, input_creator)
 
     assert isinstance(model.fit(train_file, valid_file), BaseModel)
     assert model.run_eval(valid_file) is not None
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
-@pytest.mark.deeprec
-@pytest.mark.sequential
 def test_model_slirec(deeprec_resource_path, deeprec_config_path):
     data_path = os.path.join(deeprec_resource_path, "slirec")
     yaml_file = os.path.join(deeprec_config_path, "sli_rec.yaml")
     train_file = os.path.join(data_path, r"train_data")
     valid_file = os.path.join(data_path, r"valid_data")
     test_file = os.path.join(data_path, r"test_data")
     output_file = os.path.join(data_path, "output.txt")
@@ -178,18 +175,15 @@
     assert model.run_eval(valid_file, num_ngs=valid_num_ngs) is not None
     assert isinstance(
         model.fit(train_file, valid_file, valid_num_ngs=valid_num_ngs), BaseModel
     )
     assert model.predict(test_file, output_file) is not None
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
-@pytest.mark.deeprec
-@pytest.mark.sequential
 def test_model_sum(deeprec_resource_path, deeprec_config_path):
     data_path = os.path.join(deeprec_resource_path, "slirec")
     yaml_file = os.path.join(deeprec_config_path, "sum.yaml")
     train_file = os.path.join(data_path, r"train_data")
     valid_file = os.path.join(data_path, r"valid_data")
     test_file = os.path.join(data_path, r"test_data")
     output_file = os.path.join(data_path, "output.txt")
@@ -244,17 +238,15 @@
     assert model.run_eval(valid_file, num_ngs=valid_num_ngs) is not None
     assert isinstance(
         model.fit(train_file, valid_file, valid_num_ngs=valid_num_ngs), BaseModel
     )
     assert model.predict(valid_file, output_file) is not None
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
-@pytest.mark.deeprec
 def test_model_lightgcn(deeprec_resource_path, deeprec_config_path):
     data_path = os.path.join(deeprec_resource_path, "dkn")
     yaml_file = os.path.join(deeprec_config_path, "lightgcn.yaml")
     user_file = os.path.join(data_path, r"user_embeddings.csv")
     item_file = os.path.join(data_path, r"item_embeddings.csv")
 
     df = movielens.load_pandas_df(size="100k")
```

### Comparing `recommenders-1.1.1/tests/smoke/recommenders/recommender/test_deeprec_utils.py` & `recommenders-1.2.0/tests/smoke/recommenders/recommender/test_deeprec_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import pytest
 
 try:
     import tensorflow as tf
@@ -19,15 +19,14 @@
         DKNItem2itemTextIterator,
     )
     from recommenders.models.deeprec.io.sequential_iterator import SequentialIterator
 except ImportError:
     pass  # disable error while collecting tests for non-gpu environments
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_DKN_iterator(deeprec_resource_path):
     data_path = os.path.join(deeprec_resource_path, "dkn")
     data_file = os.path.join(data_path, r"train_mind_demo.txt")
     news_feature_file = os.path.join(data_path, r"doc_feature.txt")
     user_history_file = os.path.join(data_path, r"user_history.txt")
     wordEmb_file = os.path.join(data_path, "word_embeddings_100.npy")
@@ -78,15 +77,14 @@
     ):
         assert isinstance(res, dict)
         test_round -= 1
         if test_round <= 0:
             break
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_Sequential_Iterator(deeprec_resource_path, deeprec_config_path):
     data_path = os.path.join(deeprec_resource_path, "slirec")
     yaml_file = os.path.join(deeprec_config_path, "sli_rec.yaml")
     train_file = os.path.join(data_path, r"train_data")
 
     if not os.path.exists(train_file):
```

### Comparing `recommenders-1.1.1/tests/smoke/recommenders/recommender/test_newsrec_model.py` & `recommenders-1.2.0/tests/smoke/recommenders/recommender/test_newsrec_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import pytest
 
 try:
     from recommenders.models.newsrec.newsrec_utils import prepare_hparams
@@ -13,41 +13,40 @@
     from recommenders.models.newsrec.models.lstur import LSTURModel
     from recommenders.models.newsrec.io.mind_iterator import MINDIterator
     from recommenders.models.newsrec.io.mind_all_iterator import MINDAllIterator
 except ImportError:
     pass  # disable error while collecting tests for non-gpu environments
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_model_nrms(mind_resource_path):
-    train_news_file = os.path.join(mind_resource_path, "train", r"news.tsv")
-    train_behaviors_file = os.path.join(mind_resource_path, "train", r"behaviors.tsv")
-    valid_news_file = os.path.join(mind_resource_path, "valid", r"news.tsv")
-    valid_behaviors_file = os.path.join(mind_resource_path, "valid", r"behaviors.tsv")
+    train_news_file = os.path.join(mind_resource_path, "train", "news.tsv")
+    train_behaviors_file = os.path.join(mind_resource_path, "train", "behaviors.tsv")
+    valid_news_file = os.path.join(mind_resource_path, "valid", "news.tsv")
+    valid_behaviors_file = os.path.join(mind_resource_path, "valid", "behaviors.tsv")
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"nrms.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "nrms.yaml")
 
     if not os.path.exists(train_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "train"),
             "MINDdemo_train.zip",
         )
     if not os.path.exists(valid_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "valid"),
             "MINDdemo_dev.zip",
         )
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
@@ -65,43 +64,42 @@
         model.fit(
             train_news_file, train_behaviors_file, valid_news_file, valid_behaviors_file
         ),
         BaseModel,
     )
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_model_naml(mind_resource_path):
-    train_news_file = os.path.join(mind_resource_path, "train", r"news.tsv")
-    train_behaviors_file = os.path.join(mind_resource_path, "train", r"behaviors.tsv")
-    valid_news_file = os.path.join(mind_resource_path, "valid", r"news.tsv")
-    valid_behaviors_file = os.path.join(mind_resource_path, "valid", r"behaviors.tsv")
+    train_news_file = os.path.join(mind_resource_path, "train", "news.tsv")
+    train_behaviors_file = os.path.join(mind_resource_path, "train", "behaviors.tsv")
+    valid_news_file = os.path.join(mind_resource_path, "valid", "news.tsv")
+    valid_behaviors_file = os.path.join(mind_resource_path, "valid", "behaviors.tsv")
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding_all.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict_all.pkl")
     vertDict_file = os.path.join(mind_resource_path, "utils", "vert_dict.pkl")
     subvertDict_file = os.path.join(mind_resource_path, "utils", "subvert_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"naml.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "naml.yaml")
 
     if not os.path.exists(train_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "train"),
             "MINDdemo_train.zip",
         )
     if not os.path.exists(valid_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "valid"),
             "MINDdemo_dev.zip",
         )
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
@@ -119,41 +117,40 @@
         model.fit(
             train_news_file, train_behaviors_file, valid_news_file, valid_behaviors_file
         ),
         BaseModel,
     )
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_model_lstur(mind_resource_path):
-    train_news_file = os.path.join(mind_resource_path, "train", r"news.tsv")
-    train_behaviors_file = os.path.join(mind_resource_path, "train", r"behaviors.tsv")
-    valid_news_file = os.path.join(mind_resource_path, "valid", r"news.tsv")
-    valid_behaviors_file = os.path.join(mind_resource_path, "valid", r"behaviors.tsv")
+    train_news_file = os.path.join(mind_resource_path, "train", "news.tsv")
+    train_behaviors_file = os.path.join(mind_resource_path, "train", "behaviors.tsv")
+    valid_news_file = os.path.join(mind_resource_path, "valid", "news.tsv")
+    valid_behaviors_file = os.path.join(mind_resource_path, "valid", "behaviors.tsv")
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"lstur.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "lstur.yaml")
 
     if not os.path.exists(train_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "train"),
             "MINDdemo_train.zip",
         )
     if not os.path.exists(valid_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "valid"),
             "MINDdemo_dev.zip",
         )
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
@@ -171,41 +168,40 @@
         model.fit(
             train_news_file, train_behaviors_file, valid_news_file, valid_behaviors_file
         ),
         BaseModel,
     )
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_model_npa(mind_resource_path):
-    train_news_file = os.path.join(mind_resource_path, "train", r"news.tsv")
-    train_behaviors_file = os.path.join(mind_resource_path, "train", r"behaviors.tsv")
-    valid_news_file = os.path.join(mind_resource_path, "valid", r"news.tsv")
-    valid_behaviors_file = os.path.join(mind_resource_path, "valid", r"behaviors.tsv")
+    train_news_file = os.path.join(mind_resource_path, "train", "news.tsv")
+    train_behaviors_file = os.path.join(mind_resource_path, "train", "behaviors.tsv")
+    valid_news_file = os.path.join(mind_resource_path, "valid", "news.tsv")
+    valid_behaviors_file = os.path.join(mind_resource_path, "valid", "behaviors.tsv")
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"lstur.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "lstur.yaml")
 
     if not os.path.exists(train_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "train"),
             "MINDdemo_train.zip",
         )
     if not os.path.exists(valid_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "valid"),
             "MINDdemo_dev.zip",
         )
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
```

### Comparing `recommenders-1.1.1/tests/smoke/recommenders/recommender/test_newsrec_utils.py` & `recommenders-1.2.0/tests/smoke/recommenders/recommender/test_newsrec_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import os
 import pytest
 
 try:
     from recommenders.models.newsrec.newsrec_utils import prepare_hparams
     from recommenders.models.deeprec.deeprec_utils import download_deeprec_resources
     from recommenders.models.newsrec.io.mind_iterator import MINDIterator
     from recommenders.models.newsrec.io.mind_all_iterator import MINDAllIterator
 except ImportError:
     pass  # disable error while collecting tests for non-gpu environments
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_news_iterator(mind_resource_path):
-    train_news_file = os.path.join(mind_resource_path, "train", r"news.tsv")
-    train_behaviors_file = os.path.join(mind_resource_path, "train", r"behaviors.tsv")
-    valid_news_file = os.path.join(mind_resource_path, "valid", r"news.tsv")
-    valid_behaviors_file = os.path.join(mind_resource_path, "valid", r"behaviors.tsv")
+    train_news_file = os.path.join(mind_resource_path, "train", "news.tsv")
+    train_behaviors_file = os.path.join(mind_resource_path, "train", "behaviors.tsv")
+    valid_news_file = os.path.join(mind_resource_path, "valid", "news.tsv")
+    valid_behaviors_file = os.path.join(mind_resource_path, "valid", "behaviors.tsv")
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"nrms.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "nrms.yaml")
 
     if not os.path.exists(train_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "train"),
             "MINDdemo_train.zip",
         )
     if not os.path.exists(valid_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "valid"),
             "MINDdemo_dev.zip",
         )
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
@@ -65,43 +65,42 @@
     assert test_iterator is not None
     for res in test_iterator.load_data_from_file(valid_news_file, valid_behaviors_file):
         assert isinstance(res, dict)
         assert len(res) == 5
         break
 
 
-@pytest.mark.smoke
 @pytest.mark.gpu
 def test_naml_iterator(mind_resource_path):
-    train_news_file = os.path.join(mind_resource_path, "train", r"news.tsv")
-    train_behaviors_file = os.path.join(mind_resource_path, "train", r"behaviors.tsv")
-    valid_news_file = os.path.join(mind_resource_path, "valid", r"news.tsv")
-    valid_behaviors_file = os.path.join(mind_resource_path, "valid", r"behaviors.tsv")
+    train_news_file = os.path.join(mind_resource_path, "train", "news.tsv")
+    train_behaviors_file = os.path.join(mind_resource_path, "train", "behaviors.tsv")
+    valid_news_file = os.path.join(mind_resource_path, "valid", "news.tsv")
+    valid_behaviors_file = os.path.join(mind_resource_path, "valid", "behaviors.tsv")
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding_all.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict_all.pkl")
     vertDict_file = os.path.join(mind_resource_path, "utils", "vert_dict.pkl")
     subvertDict_file = os.path.join(mind_resource_path, "utils", "subvert_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"naml.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "naml.yaml")
 
     if not os.path.exists(train_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "train"),
             "MINDdemo_train.zip",
         )
     if not os.path.exists(valid_news_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "valid"),
             "MINDdemo_dev.zip",
         )
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
```

### Comparing `recommenders-1.1.1/tests/unit/examples/test_notebooks_gpu.py` & `recommenders-1.2.0/tests/unit/examples/test_notebooks_gpu.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,75 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import os
 import pytest
 
-try:
-    import papermill as pm
-except ImportError:
-    pass  # disable error while collecting tests for non-notebook environments
-
 from recommenders.utils.gpu_utils import get_number_gpus
+from recommenders.utils.notebook_utils import execute_notebook
 
 
 @pytest.mark.notebooks
 @pytest.mark.gpu
 def test_gpu_vm():
     assert get_number_gpus() >= 1
 
 
 @pytest.mark.notebooks
 @pytest.mark.gpu
 def test_fastai(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["fastai"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(TOP_K=10, MOVIELENS_DATA_SIZE="mock100", EPOCHS=1),
     )
 
 
 @pytest.mark.notebooks
 @pytest.mark.gpu
 def test_ncf(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["ncf"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
             TOP_K=10, MOVIELENS_DATA_SIZE="mock100", EPOCHS=1, BATCH_SIZE=1024
         ),
     )
 
 
 @pytest.mark.notebooks
 @pytest.mark.gpu
 def test_ncf_deep_dive(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["ncf_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
             TOP_K=10, MOVIELENS_DATA_SIZE="mock100", EPOCHS=1, BATCH_SIZE=2048
         ),
     )
 
 
 @pytest.mark.notebooks
 @pytest.mark.gpu
 def test_xdeepfm(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["xdeepfm_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
-            EPOCHS_FOR_SYNTHETIC_RUN=1,
-            EPOCHS_FOR_CRITEO_RUN=1,
-            BATCH_SIZE_SYNTHETIC=128,
-            BATCH_SIZE_CRITEO=512,
+            EPOCHS=1,
+            BATCH_SIZE=1024,
         ),
     )
 
 
 @pytest.mark.notebooks
 @pytest.mark.gpu
 def test_wide_deep(notebooks, output_notebook, kernel_name, tmp):
@@ -88,15 +83,15 @@
         "STEPS": 1,
         "EVALUATE_WHILE_TRAINING": False,
         "MODEL_DIR": model_dir,
         "EXPORT_DIR_BASE": model_dir,
         "RATING_METRICS": ["rmse"],
         "RANKING_METRICS": ["ndcg_at_k"],
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
 
     # Test with different parameters
     model_dir = os.path.join(tmp, "wide_deep_1")
     os.mkdir(model_dir)
     params = {
@@ -105,22 +100,22 @@
         "ITEM_FEAT_COL": None,
         "EVALUATE_WHILE_TRAINING": True,
         "MODEL_DIR": model_dir,
         "EXPORT_DIR_BASE": model_dir,
         "RATING_METRICS": ["rsquared"],
         "RANKING_METRICS": ["map_at_k"],
     }
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path, output_notebook, kernel_name=kernel_name, parameters=params
     )
 
 
 @pytest.mark.notebooks
 @pytest.mark.gpu
 def test_dkn_quickstart(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["dkn_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(epochs=1, batch_size=500),
+        parameters=dict(EPOCHS=1, BATCH_SIZE=500, HISTORY_SIZE=5),
     )
```

### Comparing `recommenders-1.1.1/tests/unit/examples/test_notebooks_pyspark.py` & `recommenders-1.2.0/tests/unit/recommenders/utils/test_notebook_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,151 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import sys
 import pytest
+import nbclient
+from pathlib import Path
 
-try:
-    import papermill as pm
-except ImportError:
-    pass  # disable error while collecting tests for non-notebook environments
-
-from recommenders.utils.constants import (
-    DEFAULT_RATING_COL,
-    DEFAULT_USER_COL,
-    DEFAULT_ITEM_COL,
+from recommenders.utils.notebook_utils import (
+    is_jupyter,
+    is_databricks,
+    execute_notebook,
+    read_notebook,
+    _update_parameters,
 )
 
 
-# This is a flaky test that can fail unexpectedly
-@pytest.mark.flaky(reruns=5, reruns_delay=2)
-@pytest.mark.notebooks
-@pytest.mark.spark
-@pytest.mark.skipif(
-    sys.platform == "win32", reason="Takes 1087.56s in Windows, while in Linux 52.51s"
-)
-def test_als_pyspark_runs(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["als_pyspark"]
-    pm.execute_notebook(
-        notebook_path,
-        output_notebook,
-        kernel_name=kernel_name,
-        parameters=dict(
-            MOVIELENS_DATA_SIZE="mock100",
-            COL_USER=DEFAULT_USER_COL,
-            COL_ITEM=DEFAULT_ITEM_COL,
-            COL_RATING=DEFAULT_RATING_COL,
-        ),
-    )
+@pytest.fixture(scope="function")
+def notebook_types():
+    return Path(__file__).absolute().parent.joinpath("test_notebook_utils.ipynb")
 
 
-@pytest.mark.notebooks
-@pytest.mark.spark
-def test_data_split_runs(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["data_split"]
-    pm.execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
+@pytest.fixture(scope="function")
+def notebook_programmatic():
+    return (
+        Path(__file__)
+        .absolute()
+        .parent.joinpath("programmatic_notebook_execution.ipynb")
+    )
 
 
-# This is a flaky test that can fail unexpectedly
-@pytest.mark.flaky(reruns=5, reruns_delay=3)
 @pytest.mark.notebooks
-@pytest.mark.spark
-@pytest.mark.skipif(
-    sys.platform == "win32", reason="Takes 2764.50s in Windows, while in Linux 124.35s"
-)
-def test_als_deep_dive_runs(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["als_deep_dive"]
-    pm.execute_notebook(
-        notebook_path,
+def test_is_jupyter(notebook_types, output_notebook, kernel_name):
+    # Test on the terminal
+    assert is_jupyter() is False
+    assert is_databricks() is False
+
+    # Test on Jupyter notebook
+    execute_notebook(
+        notebook_types,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(
-            MOVIELENS_DATA_SIZE="mock100",
-            COL_USER=DEFAULT_USER_COL,
-            COL_ITEM=DEFAULT_ITEM_COL,
-            COL_RATING=DEFAULT_RATING_COL,
-        ),
     )
+    results = read_notebook(output_notebook)
+
+    assert results["is_jupyter"]
+    assert not results["is_databricks"]
 
 
-# This is a flaky test that can fail unexpectedly
-@pytest.mark.flaky(reruns=5, reruns_delay=3)
-@pytest.mark.notebooks
 @pytest.mark.spark
-@pytest.mark.skipif(
-    sys.platform == "win32", reason="Takes 583.75s in Windows, while in Linux 71.77s"
-)
-def test_evaluation_runs(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["evaluation"]
-    pm.execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
+@pytest.mark.notebooks
+@pytest.mark.skip(reason="TODO: Implement this")
+def test_is_databricks():
+    pass
 
 
-# This is a flaky test that can fail unexpectedly
-@pytest.mark.flaky(reruns=5, reruns_delay=2)
 @pytest.mark.notebooks
-@pytest.mark.spark
-def test_evaluation_diversity_runs(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["evaluation_diversity"]
-    pm.execute_notebook(
-        notebook_path,
+def test_update_parameters():
+    parameter_cell_source = '''
+# Integer
+TOP_K = 10
+# Float
+LEARNING_RATE = 0.001
+# String
+MOVIELENS_DATA_SIZE = "100k"
+# List
+RANKING_METRICS = [ evaluator.ndcg_at_k.__name__, evaluator.precision_at_k.__name__ ]
+# Boolean
+EVALUATE_WHILE_TRAINING = True
+'''
+
+    new_parameters = {
+        "MOVIELENS_DATA_SIZE": "1m",
+        "TOP_K": 1,
+        "EVALUATE_WHILE_TRAINING": False,
+        "RANKING_METRICS": ["ndcg_at_k", "precision_at_k"],
+        "LEARNING_RATE": 0.1,
+    }
+
+    new_cell_source = _update_parameters(parameter_cell_source, new_parameters)
+    assert new_cell_source == '''
+# Integer
+TOP_K = 1
+# Float
+LEARNING_RATE = 0.1
+# String
+MOVIELENS_DATA_SIZE = "1m"
+# List
+RANKING_METRICS = ['ndcg_at_k', 'precision_at_k']
+# Boolean
+EVALUATE_WHILE_TRAINING = False
+'''
+
+
+@pytest.mark.notebooks
+def test_notebook_execution(notebook_programmatic, output_notebook, kernel_name):
+    """Test that the notebook executes and returns the correct results without params."""
+    execute_notebook(
+        notebook_programmatic,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(
-            TOP_K=10,
-            MOVIELENS_DATA_SIZE="mock100",
-            COL_USER=DEFAULT_USER_COL,
-            COL_ITEM=DEFAULT_ITEM_COL,
-            COL_RATING=DEFAULT_RATING_COL,
-        ),
     )
 
+    results = read_notebook(output_notebook)
+    assert results["response1"] == 3
+    assert results["response2"] is True
+    assert results["response3"] == 7
+
 
-# This is a flaky test that can fail unexpectedly
-@pytest.mark.flaky(reruns=5, reruns_delay=2)
 @pytest.mark.notebooks
-@pytest.mark.spark
-@pytest.mark.skipif(
-    sys.platform == "win32", reason="Takes 2409.69s in Windows, while in Linux 138.30s"
+@pytest.mark.parametrize(
+    "parameters,expected_key,expected_value", [
+        (dict(a=6), "response1", 8),            # Test the correct results with integers
+        (dict(a=1.5), "response1", 3.5),        # Test the correct results with floats
+        (dict(b="M"), "response2", True),       # Test the correct results with strings
+        (dict(b="A"), "response2", "A"),        # Test the correct results with different strings
+        (dict(b="100k"), "response2", "100k"),  # Test the correct results with strings that have numbers
+        (dict(c=10), "response3", 12),          # Test the correct results with integers and a comment
+    ]
 )
-def test_spark_tuning(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["spark_tuning"]
-    pm.execute_notebook(
-        notebook_path,
+def test_notebook_execution_with_parameters(
+    notebook_programmatic,
+    output_notebook,
+    kernel_name,
+    parameters,
+    expected_key,
+    expected_value,    
+):
+    """Test that the notebook executes."""
+    execute_notebook(
+        notebook_programmatic,
         output_notebook,
         kernel_name=kernel_name,
-        parameters=dict(
-            MOVIELENS_DATA_SIZE="mock100",
-            NUMBER_CORES="1",
-            NUMBER_ITERATIONS=3,
-            SUBSET_RATIO=0.5,
-            RANK=[5, 10],
-            REG=[0.1, 0.01],
-        ),
+        parameters=parameters,
     )
 
+    results = read_notebook(output_notebook)
+    assert results[expected_key] == expected_value
+
 
 @pytest.mark.notebooks
-@pytest.mark.spark
-@pytest.mark.skipif(sys.platform == "win32", reason="Not implemented on Windows")
-def test_mmlspark_lightgbm_criteo_runs(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["mmlspark_lightgbm_criteo"]
-    pm.execute_notebook(
-        notebook_path,
-        output_notebook,
-        kernel_name=kernel_name,
-        parameters=dict(DATA_SIZE="sample", NUM_ITERATIONS=10),
-    )
+def test_notebook_execution_value_error_fails(
+    notebook_programmatic, output_notebook, kernel_name
+):
+    """Test that the notebook fails with a value error."""
+    with pytest.raises(nbclient.exceptions.CellExecutionError):
+        execute_notebook(
+            notebook_programmatic,
+            output_notebook,
+            kernel_name=kernel_name,
+            parameters=dict(b=1),
+        )
```

### Comparing `recommenders-1.1.1/tests/unit/examples/test_notebooks_python.py` & `recommenders-1.2.0/tests/unit/examples/test_notebooks_python.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,70 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import sys
 import pytest
 
-try:
-    import papermill as pm
-    import scrapbook as sb
-except ImportError:
-    pass  # disable error while collecting tests for non-notebook environments
+import recommenders
+from recommenders.utils.notebook_utils import execute_notebook, read_notebook
 
 
 TOL = 0.05
 ABS_TOL = 0.05
 
 
 @pytest.mark.notebooks
 def test_template_runs(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["template"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
-        parameters=dict(PM_VERSION=pm.__version__),
+        parameters=dict(RECOMMENDERS_VERSION=recommenders.__version__),
         kernel_name=kernel_name,
     )
-    nb = sb.read_notebook(output_notebook)
-    df = nb.papermill_dataframe
-    assert df.shape[0] == 2
-    check_version = df.loc[df["name"] == "checked_version", "value"].values[0]
-    assert check_version is True
+    results = read_notebook(output_notebook)
+
+    assert len(results) == 1
+    assert results["checked_version"]
 
 
 @pytest.mark.notebooks
 def test_sar_single_node_runs(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["sar_single_node"]
-    pm.execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
+    execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
 
 
 @pytest.mark.notebooks
 def test_sar_deep_dive_runs(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["sar_deep_dive"]
-    pm.execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
+    execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
 
 
 @pytest.mark.notebooks
 def test_baseline_deep_dive_runs(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["baseline_deep_dive"]
-    pm.execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
+    execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
 
 
 @pytest.mark.notebooks
 def test_surprise_deep_dive_runs(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["surprise_svd_deep_dive"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(MOVIELENS_DATA_SIZE="mock100"),
     )
 
 
 @pytest.mark.notebooks
-@pytest.mark.skip(reason="VW pip package has installation incompatibilities")
-def test_vw_deep_dive_runs(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["vowpal_wabbit_deep_dive"]
-    pm.execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
-
-
-@pytest.mark.notebooks
 def test_lightgbm(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["lightgbm_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(
             MAX_LEAF=32,
             MIN_DATA=20,
             NUM_OF_TREES=10,
@@ -82,39 +72,31 @@
             EARLY_STOPPING_ROUNDS=20,
             METRIC="auc",
         ),
     )
 
 
 @pytest.mark.notebooks
-@pytest.mark.skip(reason="Wikidata API is unstable")
-def test_wikidata_runs(notebooks, output_notebook, kernel_name, tmp):
-    notebook_path = notebooks["wikidata_knowledge_graph"]
-    MOVIELENS_SAMPLE_SIZE = 5
-    pm.execute_notebook(
-        notebook_path,
-        output_notebook,
-        kernel_name=kernel_name,
-        parameters=dict(
-            MOVIELENS_DATA_SIZE="100k",
-            MOVIELENS_SAMPLE=True,
-            MOVIELENS_SAMPLE_SIZE=MOVIELENS_SAMPLE_SIZE,
-        ),
-    )
+def test_cornac_deep_dive_runs(notebooks, output_notebook, kernel_name):
+    notebook_path = notebooks["cornac_bpr_deep_dive"]
+    execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
 
 
-@pytest.mark.experimental
 @pytest.mark.notebooks
+@pytest.mark.experimental
+@pytest.mark.skip(reason="rlrmc doesn't work with any officially released pymanopt package")
 def test_rlrmc_quickstart_runs(notebooks, output_notebook, kernel_name):
     notebook_path = notebooks["rlrmc_quickstart"]
-    pm.execute_notebook(
+    execute_notebook(
         notebook_path,
         output_notebook,
         kernel_name=kernel_name,
         parameters=dict(rank_parameter=2, MOVIELENS_DATA_SIZE="mock100"),
     )
 
 
 @pytest.mark.notebooks
-def test_cornac_deep_dive_runs(notebooks, output_notebook, kernel_name):
-    notebook_path = notebooks["cornac_bpr_deep_dive"]
-    pm.execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
+@pytest.mark.experimental
+@pytest.mark.skip(reason="VW pip package has installation incompatibilities")
+def test_vw_deep_dive_runs(notebooks, output_notebook, kernel_name):
+    notebook_path = notebooks["vowpal_wabbit_deep_dive"]
+    execute_notebook(notebook_path, output_notebook, kernel_name=kernel_name)
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/datasets/test_covid_utils.py` & `recommenders-1.2.0/tests/data_validation/recommenders/datasets/test_covid_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 from unittest.mock import patch
 import pytest
 from recommenders.datasets.covid_utils import (
     remove_duplicates,
     remove_nan,
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/datasets/test_dataset.py` & `recommenders-1.2.0/tests/unit/recommenders/datasets/test_download_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import pytest
 import requests
-from tempfile import TemporaryDirectory
 import logging
+from tempfile import TemporaryDirectory
+
 from recommenders.datasets.download_utils import maybe_download, download_path
 
 
 @pytest.fixture
 def files_fixtures():
-    file_url = "https://raw.githubusercontent.com/Microsoft/Recommenders/main/LICENSE"
+    file_url = (
+        "https://raw.githubusercontent.com/recommenders-team/recommenders/main/LICENSE"
+    )
     filepath = "license.txt"
     return file_url, filepath
 
 
 def test_maybe_download(files_fixtures):
     file_url, filepath = files_fixtures
     if os.path.exists(filepath):
         os.remove(filepath)
 
-    downloaded_filepath = maybe_download(file_url, "license.txt", expected_bytes=1162)
+    downloaded_filepath = maybe_download(file_url, "license.txt", expected_bytes=1212)
     assert os.path.exists(downloaded_filepath)
-    assert downloaded_filepath.split("/")[-1] == "license.txt"
+    assert os.path.basename(downloaded_filepath) == "license.txt"
 
 
 def test_maybe_download_wrong_bytes(caplog, files_fixtures):
     caplog.clear()
     caplog.set_level(logging.INFO)
 
     file_url, filepath = files_fixtures
@@ -46,15 +49,15 @@
     file_url, filepath = files_fixtures
     if os.path.exists(filepath):
         os.remove(filepath)
 
     downloaded_filepath = maybe_download(file_url, "license.txt")
     assert os.path.exists(downloaded_filepath)
     maybe_download(file_url, "license.txt")
-    assert "File ./license.txt already downloaded" in caplog.text
+    assert "File ." + os.path.sep + "license.txt already downloaded" in caplog.text
 
 
 def test_maybe_download_retry(caplog):
     caplog.clear()
     caplog.set_level(logging.INFO)
     with pytest.raises(requests.exceptions.HTTPError):
         maybe_download(
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/datasets/test_pandas_df_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/datasets/test_pandas_df_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+import os
 import numpy as np
 import pandas as pd
 import pytest
 from tempfile import TemporaryDirectory
-import os
 
 from recommenders.datasets.pandas_df_utils import (
     filter_by,
     LibffmConverter,
     has_same_base_dtype,
     has_columns,
     lru_cache_df,
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/datasets/test_python_splitter.py` & `recommenders-1.2.0/tests/unit/recommenders/datasets/test_python_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
+import pytest
 import pandas as pd
 import numpy as np
-import pytest
 
+from recommenders.utils.constants import (
+    DEFAULT_USER_COL,
+    DEFAULT_ITEM_COL,
+    DEFAULT_RATING_COL,
+    DEFAULT_TIMESTAMP_COL,
+)
 from recommenders.datasets.split_utils import (
     min_rating_filter_pandas,
     split_pandas_data_with_ratios,
 )
-
 from recommenders.datasets.python_splitters import (
     python_chrono_split,
     python_random_split,
     python_stratified_split,
     numpy_stratified_split,
 )
 
-from recommenders.utils.constants import (
-    DEFAULT_USER_COL,
-    DEFAULT_ITEM_COL,
-    DEFAULT_RATING_COL,
-    DEFAULT_TIMESTAMP_COL,
-)
-
 
 @pytest.fixture(scope="module")
 def test_specs():
     return {
         "number_of_rows": 1000,
         "seed": 123,
         "ratio": 0.6,
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/datasets/test_spark_splitter.py` & `recommenders-1.2.0/tests/unit/recommenders/datasets/test_spark_splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
+import pytest
 import numpy as np
 import pandas as pd
-import pytest
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
     DEFAULT_ITEM_COL,
     DEFAULT_RATING_COL,
     DEFAULT_TIMESTAMP_COL,
 )
 
@@ -44,14 +45,33 @@
                 DEFAULT_TIMESTAMP_COL: np.random.randint(1, 1000, NUM_ROWS)
                 + np.datetime64("2018-01-01"),
             }
         )
     )
 
 
+def _if_later(data1, data2):
+    """Helper function to test if records in data1 are earlier than that in data2.
+    Returns:
+        bool: True or False indicating if data1 is earlier than data2.
+    """
+
+    max_times = data1.groupBy(DEFAULT_USER_COL).agg(
+        F.max(DEFAULT_TIMESTAMP_COL).alias("max")
+    )
+    min_times = data2.groupBy(DEFAULT_USER_COL).agg(
+        F.min(DEFAULT_TIMESTAMP_COL).alias("min")
+    )
+    all_times = max_times.join(min_times, on=DEFAULT_USER_COL).select(
+        (F.col("max") <= F.col("min"))
+    )
+
+    return all([x[0] for x in all_times.collect()])
+
+
 @pytest.mark.spark
 def test_min_rating_filter(spark_dataset):
     dfs_user = min_rating_filter_spark(spark_dataset, min_rating=5, filter_by="user")
     dfs_item = min_rating_filter_spark(spark_dataset, min_rating=5, filter_by="item")
 
     user_rating_counts = [
         x["count"] >= 5 for x in dfs_user.groupBy(DEFAULT_USER_COL).count().collect()
@@ -186,26 +206,7 @@
     max_split0 = splits[0].agg(F.max(DEFAULT_TIMESTAMP_COL)).first()[0]
     min_split1 = splits[1].agg(F.min(DEFAULT_TIMESTAMP_COL)).first()[0]
     assert max_split0 <= min_split1
 
     max_split1 = splits[1].agg(F.max(DEFAULT_TIMESTAMP_COL)).first()[0]
     min_split2 = splits[2].agg(F.min(DEFAULT_TIMESTAMP_COL)).first()[0]
     assert max_split1 <= min_split2
-
-
-def _if_later(data1, data2):
-    """Helper function to test if records in data1 are earlier than that in data2.
-    Returns:
-        bool: True or False indicating if data1 is earlier than data2.
-    """
-
-    max_times = data1.groupBy(DEFAULT_USER_COL).agg(
-        F.max(DEFAULT_TIMESTAMP_COL).alias("max")
-    )
-    min_times = data2.groupBy(DEFAULT_USER_COL).agg(
-        F.min(DEFAULT_TIMESTAMP_COL).alias("min")
-    )
-    all_times = max_times.join(min_times, on=DEFAULT_USER_COL).select(
-        (F.col("max") <= F.col("min"))
-    )
-
-    return all([x[0] for x in all_times.collect()])
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/datasets/test_sparse.py` & `recommenders-1.2.0/tests/unit/recommenders/datasets/test_sparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import pandas as pd
 import numpy as np
 import pytest
 
 from recommenders.datasets.sparse import AffinityMatrix
@@ -76,15 +76,15 @@
 
     # here we eliminate the missing ratings to obtain a standard form of the df as that of real data.
     results = results[results.rating != 0]
 
     return results
 
 
-def test_df_to_sparse(test_specs, python_dataset):
+def test_df_to_sparse(python_dataset):
     # initialize the splitter
     header = {
         "col_user": DEFAULT_USER_COL,
         "col_item": DEFAULT_ITEM_COL,
         "col_rating": DEFAULT_RATING_COL,
     }
 
@@ -96,39 +96,39 @@
 
     # check that the generated matrix has the correct dimensions
     assert (X.shape[0] == python_dataset.userID.unique().shape[0]) & (
         X.shape[1] == python_dataset.itemID.unique().shape[0]
     )
 
 
-def test_sparse_to_df(test_specs, python_dataset):
+def test_sparse_to_df(python_dataset):
     # initialize the splitter
     header = {
         "col_user": DEFAULT_USER_COL,
         "col_item": DEFAULT_ITEM_COL,
         "col_rating": DEFAULT_RATING_COL,
     }
 
     # instantiate the the affinity matrix
     am = AffinityMatrix(df=python_dataset, **header)
 
     # generate the sparse matrix representation
     X, _, _ = am.gen_affinity_matrix()
 
     # use the inverse function to generate a pandas df from a sparse matrix ordered by userID
-    DF = am.map_back_sparse(X, kind="ratings")
+    df = am.map_back_sparse(X, kind="ratings")
 
     # tests: check that the two dataframes have the same elements in the same positions.
     assert (
-        DF.userID.values.all()
+        df.userID.values.all()
         == python_dataset.sort_values(by=["userID"]).userID.values.all()
     )
 
     assert (
-        DF.itemID.values.all()
+        df.itemID.values.all()
         == python_dataset.sort_values(by=["userID"]).itemID.values.all()
     )
 
     assert (
-        DF.rating.values.all()
+        df.rating.values.all()
         == python_dataset.sort_values(by=["userID"]).rating.values.all()
     )
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/datasets/test_wikidata.py` & `recommenders-1.2.0/tests/data_validation/recommenders/datasets/test_wikidata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import pytest
 
+import pytest
 
 from recommenders.datasets.wikidata import (
     find_wikidata_id,
     query_entity_links,
     read_linked_entities,
     query_entity_description,
 )
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/evaluation/test_python_evaluation.py` & `recommenders-1.2.0/tests/unit/recommenders/evaluation/test_python_evaluation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import numpy as np
 import pandas as pd
 import pytest
 from unittest.mock import Mock
 from sklearn.preprocessing import minmax_scale
-from pandas.util.testing import assert_frame_equal
+from pandas.testing import assert_frame_equal
 
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
     DEFAULT_ITEM_COL,
     DEFAULT_RATING_COL,
     DEFAULT_PREDICTION_COL,
 )
@@ -20,67 +21,36 @@
     merge_ranking_true_pred,
     rmse,
     mae,
     rsquared,
     exp_var,
     get_top_k_items,
     precision_at_k,
+    r_precision_at_k,
     recall_at_k,
     ndcg_at_k,
     map_at_k,
+    map,
     auc,
     logloss,
     user_diversity,
     diversity,
     historical_item_novelty,
     novelty,
     user_item_serendipity,
     user_serendipity,
     serendipity,
     catalog_coverage,
     distributional_coverage,
+    ColumnMismatchError,
+    ColumnTypeMismatchError,
 )
 
-TOL = 0.0001
-
-
-# fmt: off
-@pytest.fixture
-def rating_true():
-    return pd.DataFrame(
-        {
-            DEFAULT_USER_COL: [1, 2, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 1, 1],
-            DEFAULT_ITEM_COL: [3, 1, 4, 5, 6, 7, 2, 5, 6, 8, 9, 10, 11, 12, 13, 14, 1, 2],
-            DEFAULT_RATING_COL: [3, 5, 5, 3, 3, 1, 5, 5, 5, 4, 4, 3, 3, 3, 2, 1, 5, 4],
-        }
-    )
-
-
-@pytest.fixture
-def rating_pred():
-    return pd.DataFrame(
-        {
-            DEFAULT_USER_COL: [1, 2, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 1, 1],
-            DEFAULT_ITEM_COL: [12, 10, 3, 5, 11, 13, 4, 10, 7, 13, 1, 3, 5, 2, 11, 14, 3, 10],
-            DEFAULT_PREDICTION_COL: [12, 14, 13, 12, 11, 10, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 14, 13],
-            DEFAULT_RATING_COL: [3, 5, 5, 3, 3, 1, 5, 5, 5, 4, 4, 3, 3, 3, 2, 1, 5, 4],
-        }
-    )
-
 
-@pytest.fixture
-def rating_nohit():
-    return pd.DataFrame(
-        {
-            DEFAULT_USER_COL: [1, 2, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3, 1, 1],
-            DEFAULT_ITEM_COL: [100] * 18,
-            DEFAULT_PREDICTION_COL: [12, 14, 13, 12, 11, 10, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 14, 13],
-        }
-    )
-# fmt: on
+TOL = 0.0001
 
 
 @pytest.fixture
 def rating_true_binary(rating_true):
     # Convert true ratings to binary
     rating_true[DEFAULT_RATING_COL] = rating_true[DEFAULT_RATING_COL].apply(
         lambda x: 1.0 if x >= 3 else 0.0
@@ -94,20 +64,40 @@
     rating_pred[DEFAULT_PREDICTION_COL] = minmax_scale(
         rating_pred[DEFAULT_PREDICTION_COL].astype(float)
     )
     return rating_pred
 
 
 def test_column_dtypes_match(rating_true, rating_pred):
-    # Change data types of true and prediction data, and there should type error produced
-    rating_true[DEFAULT_USER_COL] = rating_true[DEFAULT_USER_COL].astype(str)
-    rating_true[DEFAULT_RATING_COL] = rating_true[DEFAULT_RATING_COL].astype(str)
+    # Check if _check_column_dtypes wraps the input function (i.e. returns the same output as the input function's)
+    mocked_fn = Mock(return_value=True)
+    assert _check_column_dtypes(mocked_fn)(
+        rating_true,
+        rating_pred,
+        col_user=DEFAULT_USER_COL,
+        col_item=DEFAULT_ITEM_COL,
+        col_rating=DEFAULT_RATING_COL,
+        col_prediction=DEFAULT_PREDICTION_COL,
+    )
 
-    expected_error = "Columns in provided DataFrames are not the same datatype"
-    with pytest.raises(ValueError, match=expected_error):
+    # Change data types of true and prediction data, and there should type mismatch error produced
+    rating_true[DEFAULT_USER_COL] = rating_true[DEFAULT_USER_COL].astype(str)
+    with pytest.raises(ColumnTypeMismatchError):
+        _check_column_dtypes(Mock())(
+            rating_true,
+            rating_pred,
+            col_user=DEFAULT_USER_COL,
+            col_item=DEFAULT_ITEM_COL,
+            col_rating=DEFAULT_RATING_COL,
+            col_prediction=DEFAULT_PREDICTION_COL,
+        )
+    
+    # Drop a column, and there should column mismatch error produced
+    rating_true.drop(DEFAULT_USER_COL, axis="columns", inplace=True)
+    with pytest.raises(ColumnMismatchError):
         _check_column_dtypes(Mock())(
             rating_true,
             rating_pred,
             col_user=DEFAULT_USER_COL,
             col_item=DEFAULT_ITEM_COL,
             col_rating=DEFAULT_RATING_COL,
             col_prediction=DEFAULT_PREDICTION_COL,
@@ -174,99 +164,124 @@
         )
         == 0
     )
     assert mae(rating_true, rating_pred) == pytest.approx(6.375, TOL)
 
 
 def test_python_rsquared(rating_true, rating_pred):
-    assert (
-        rsquared(
-            rating_true=rating_true,
-            rating_pred=rating_true,
-            col_prediction=DEFAULT_RATING_COL,
-        )
-        == pytest.approx(1.0, TOL)
-    )
+    assert rsquared(
+        rating_true=rating_true,
+        rating_pred=rating_true,
+        col_prediction=DEFAULT_RATING_COL,
+    ) == pytest.approx(1.0, TOL)
     assert rsquared(rating_true, rating_pred) == pytest.approx(-31.699029, TOL)
 
 
 def test_python_exp_var(rating_true, rating_pred):
-    assert (
-        exp_var(
-            rating_true=rating_true,
-            rating_pred=rating_true,
-            col_prediction=DEFAULT_RATING_COL,
-        )
-        == pytest.approx(1.0, TOL)
-    )
+    assert exp_var(
+        rating_true=rating_true,
+        rating_pred=rating_true,
+        col_prediction=DEFAULT_RATING_COL,
+    ) == pytest.approx(1.0, TOL)
     assert exp_var(rating_true, rating_pred) == pytest.approx(-6.4466, TOL)
 
 
 def test_get_top_k_items(rating_true):
     top_3_items_df = get_top_k_items(
         dataframe=rating_true,
         col_user=DEFAULT_USER_COL,
         col_rating=DEFAULT_RATING_COL,
         k=3,
     )
     top_3_user_true = pd.Series([1, 1, 1, 2, 2, 2, 3, 3, 3])
     top_3_rating_true = pd.Series([5, 4, 3, 5, 5, 3, 5, 5, 5])
     top_3_rank_true = pd.Series([1, 2, 3, 1, 2, 3, 1, 2, 3])
-    assert(top_3_items_df[DEFAULT_USER_COL].equals(top_3_user_true))
-    assert(top_3_items_df[DEFAULT_RATING_COL].equals(top_3_rating_true))
-    assert(top_3_items_df['rank'].equals(top_3_rank_true))
-    assert(top_3_items_df[DEFAULT_ITEM_COL][:3].equals(pd.Series([1, 2, 3])))
+    assert top_3_items_df[DEFAULT_USER_COL].equals(top_3_user_true)
+    assert top_3_items_df[DEFAULT_RATING_COL].equals(top_3_rating_true)
+    assert top_3_items_df["rank"].equals(top_3_rank_true)
+    assert top_3_items_df[DEFAULT_ITEM_COL][:3].equals(pd.Series([1, 2, 3]))
     # First two itemIDs of user 2. The scores are both 5, so any order is OK.
-    assert(set(top_3_items_df[DEFAULT_ITEM_COL][3:5]) == set([1, 4]))
+    assert set(top_3_items_df[DEFAULT_ITEM_COL][3:5]) == set([1, 4])
     # Third itemID of user 2. Both item 5 and 6 have a score of 3, so either one is OK.
-    assert(top_3_items_df[DEFAULT_ITEM_COL][5] in [5, 6])
+    assert top_3_items_df[DEFAULT_ITEM_COL][5] in [5, 6]
     # All itemIDs of user 3. All three items have a score of 5, so any order is OK.
-    assert(set(top_3_items_df[DEFAULT_ITEM_COL][6:]) == set([2, 5, 6]))
+    assert set(top_3_items_df[DEFAULT_ITEM_COL][6:]) == set([2, 5, 6])
 
 
 # Test get_top_k_items() when k is larger than the number of available items
 def test_get_top_k_items_largek(rating_true):
     top_6_items_df = get_top_k_items(
         dataframe=rating_true,
         col_user=DEFAULT_USER_COL,
         col_rating=DEFAULT_RATING_COL,
         k=6,
     )
     top_6_user_true = pd.Series([1, 1, 1, 2, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3])
     top_6_rating_true = pd.Series([5, 4, 3, 5, 5, 3, 3, 1, 5, 5, 5, 4, 4, 3])
     top_6_rank_true = pd.Series([1, 2, 3, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 6])
-    assert(top_6_items_df[DEFAULT_USER_COL].equals(top_6_user_true))
-    assert(top_6_items_df[DEFAULT_RATING_COL].equals(top_6_rating_true))
-    assert(top_6_items_df['rank'].equals(top_6_rank_true))
-    assert(top_6_items_df[DEFAULT_ITEM_COL][:3].equals(pd.Series([1, 2, 3])))
+    assert top_6_items_df[DEFAULT_USER_COL].equals(top_6_user_true)
+    assert top_6_items_df[DEFAULT_RATING_COL].equals(top_6_rating_true)
+    assert top_6_items_df["rank"].equals(top_6_rank_true)
+    assert top_6_items_df[DEFAULT_ITEM_COL][:3].equals(pd.Series([1, 2, 3]))
     # First two itemIDs of user 2. The scores are both 5, so any order is OK.
-    assert(set(top_6_items_df[DEFAULT_ITEM_COL][3:5]) == set([1, 4]))
+    assert set(top_6_items_df[DEFAULT_ITEM_COL][3:5]) == set([1, 4])
     # Third and fourth itemID of user 2. The scores are both 3, so any order is OK.
-    assert(set(top_6_items_df[DEFAULT_ITEM_COL][5:7]) == set([5, 6]))
-    assert(top_6_items_df[DEFAULT_ITEM_COL][7] == 7)
+    assert set(top_6_items_df[DEFAULT_ITEM_COL][5:7]) == set([5, 6])
+    assert top_6_items_df[DEFAULT_ITEM_COL][7] == 7
     # First three itemIDs of user 3. The scores are both 5, so any order is OK.
-    assert(set(top_6_items_df[DEFAULT_ITEM_COL][8:11]) == set([2, 5, 6]))
+    assert set(top_6_items_df[DEFAULT_ITEM_COL][8:11]) == set([2, 5, 6])
     # Fourth and fifth itemID of user 3. The scores are both 4, so any order is OK.
-    assert(set(top_6_items_df[DEFAULT_ITEM_COL][11:13]) == set([8, 9]))
+    assert set(top_6_items_df[DEFAULT_ITEM_COL][11:13]) == set([8, 9])
     # Sixth itemID of user 3. Item 10,11,12 have a score of 3, so either one is OK.
-    assert(top_6_items_df[DEFAULT_ITEM_COL][13] in [10, 11, 12])
+    assert top_6_items_df[DEFAULT_ITEM_COL][13] in [10, 11, 12]
 
 
 def test_python_ndcg_at_k(rating_true, rating_pred, rating_nohit):
+    assert ndcg_at_k(
+        rating_true=rating_true,
+        rating_pred=rating_true,
+        col_prediction=DEFAULT_RATING_COL,
+        k=10,
+    ) == pytest.approx(1.0, TOL)
+    assert ndcg_at_k(rating_true, rating_nohit, k=10) == 0.0
+    assert ndcg_at_k(rating_true, rating_pred, k=10) == pytest.approx(0.38172, TOL)
+
+    # Test raw relevance score and log2 discounting factor using wiki example
+    # See https://en.wikipedia.org/wiki/Discounted_cumulative_gain
+    df_true = pd.DataFrame(
+        {
+            DEFAULT_USER_COL: np.full(8, 0, dtype=int),
+            DEFAULT_ITEM_COL: np.arange(8),
+            DEFAULT_RATING_COL: np.asarray([3, 2, 3, 0, 1, 2, 3, 2]),
+        }
+    )
+    df_pred = pd.DataFrame(
+        {
+            DEFAULT_USER_COL: np.full(6, 0, dtype=int),
+            DEFAULT_ITEM_COL: np.arange(6),
+            DEFAULT_PREDICTION_COL: np.asarray([6, 5, 4, 3, 2, 1]),
+        }
+    )
+    assert ndcg_at_k(
+        df_true, df_pred, k=6, score_type="raw", discfun_type="log2"
+    ) == pytest.approx(0.785, TOL)
+
+
+def test_python_map(rating_true, rating_pred, rating_nohit):
     assert (
-        ndcg_at_k(
+        map(
             rating_true=rating_true,
             rating_pred=rating_true,
             col_prediction=DEFAULT_RATING_COL,
             k=10,
         )
-        == pytest.approx(1.0, TOL)
+        == 1
     )
-    assert ndcg_at_k(rating_true, rating_nohit, k=10) == 0.0
-    assert ndcg_at_k(rating_true, rating_pred, k=10) == pytest.approx(0.38172, TOL)
+    assert map(rating_true, rating_nohit, k=10) == 0.0
+    assert map(rating_true, rating_pred, k=10) == pytest.approx(0.23613, TOL)
 
 
 def test_python_map_at_k(rating_true, rating_pred, rating_nohit):
     assert (
         map_at_k(
             rating_true=rating_true,
             rating_pred=rating_true,
@@ -275,15 +290,15 @@
         )
         == 1
     )
     assert map_at_k(rating_true, rating_nohit, k=10) == 0.0
     assert map_at_k(rating_true, rating_pred, k=10) == pytest.approx(0.23613, TOL)
 
 
-def test_python_precision(rating_true, rating_pred, rating_nohit):
+def test_python_precision_at_k(rating_true, rating_pred, rating_nohit):
     assert (
         precision_at_k(
             rating_true=rating_true,
             rating_pred=rating_true,
             col_prediction=DEFAULT_RATING_COL,
             k=10,
         )
@@ -337,422 +352,367 @@
             col_prediction=DEFAULT_RATING_COL,
             k=5,
         )
         == 0.6
     )
 
 
-def test_python_recall(rating_true, rating_pred, rating_nohit):
-    assert (
-        recall_at_k(
-            rating_true=rating_true,
-            rating_pred=rating_true,
-            col_prediction=DEFAULT_RATING_COL,
-            k=10,
-        )
-        == pytest.approx(1, TOL)
-    )
+def test_python_recall_at_k(rating_true, rating_pred, rating_nohit):
+    assert recall_at_k(
+        rating_true=rating_true,
+        rating_pred=rating_true,
+        col_prediction=DEFAULT_RATING_COL,
+        k=10,
+    ) == pytest.approx(1, TOL)
     assert recall_at_k(rating_true, rating_nohit, k=10) == 0.0
     assert recall_at_k(rating_true, rating_pred, k=10) == pytest.approx(0.37777, TOL)
 
 
-def test_python_auc(rating_true_binary, rating_pred_binary):
-    assert (
-        auc(
-            rating_true=rating_true_binary,
-            rating_pred=rating_true_binary,
-            col_prediction=DEFAULT_RATING_COL,
-        )
-        == pytest.approx(1.0, TOL)
-    )
+def test_python_r_precision(rating_true, rating_pred, rating_nohit):
+    assert r_precision_at_k(
+        rating_true=rating_true,
+        rating_pred=rating_true,
+        col_prediction=DEFAULT_RATING_COL,
+        k=10,
+    ) == pytest.approx(1, TOL)
+    assert r_precision_at_k(rating_true, rating_nohit, k=5) == 0.0
+    assert r_precision_at_k(rating_true, rating_pred, k=3) == pytest.approx(0.21111, TOL)
+    assert r_precision_at_k(rating_true, rating_pred, k=5) == pytest.approx(0.24444, TOL)
+    # Equivalent to precision
+    assert r_precision_at_k(rating_true, rating_pred, k=10) == pytest.approx(0.37777, TOL)
 
-    assert (
-        auc(
-            rating_true=rating_true_binary,
-            rating_pred=rating_pred_binary,
-            col_rating=DEFAULT_RATING_COL,
-            col_prediction=DEFAULT_PREDICTION_COL,
-        )
-        == pytest.approx(0.75, TOL)
-    )
 
+def test_python_auc(rating_true_binary, rating_pred_binary):
+    assert auc(
+        rating_true=rating_true_binary,
+        rating_pred=rating_true_binary,
+        col_prediction=DEFAULT_RATING_COL,
+    ) == pytest.approx(1.0, TOL)
+
+    assert auc(
+        rating_true=rating_true_binary,
+        rating_pred=rating_pred_binary,
+        col_rating=DEFAULT_RATING_COL,
+        col_prediction=DEFAULT_PREDICTION_COL,
+    ) == pytest.approx(0.75, TOL)
 
-def test_python_logloss(rating_true_binary, rating_pred_binary):
-    assert (
-        logloss(
-            rating_true=rating_true_binary,
-            rating_pred=rating_true_binary,
-            col_prediction=DEFAULT_RATING_COL,
-        )
-        == pytest.approx(0, TOL)
-    )
 
-    assert (
-        logloss(
-            rating_true=rating_true_binary,
-            rating_pred=rating_pred_binary,
-            col_rating=DEFAULT_RATING_COL,
-            col_prediction=DEFAULT_PREDICTION_COL,
-        )
-        == pytest.approx(0.7835, TOL)
-    )
+def test_python_logloss(rating_true_binary, rating_pred_binary):
+    assert logloss(
+        rating_true=rating_true_binary,
+        rating_pred=rating_true_binary,
+        col_prediction=DEFAULT_RATING_COL,
+    ) == pytest.approx(0, TOL)
+
+    assert logloss(
+        rating_true=rating_true_binary,
+        rating_pred=rating_pred_binary,
+        col_rating=DEFAULT_RATING_COL,
+        col_prediction=DEFAULT_PREDICTION_COL,
+    ) == pytest.approx(0.7835, TOL)
 
 
 def test_python_errors(rating_true, rating_pred):
-    with pytest.raises(ValueError):
+    with pytest.raises(ColumnMismatchError):
         rmse(rating_true, rating_true, col_user="not_user")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ColumnMismatchError):
         mae(
             rating_pred,
             rating_pred,
             col_rating=DEFAULT_PREDICTION_COL,
             col_user="not_user",
         )
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ColumnMismatchError):
         rsquared(rating_true, rating_pred, col_item="not_item")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ColumnMismatchError):
         exp_var(
             rating_pred,
             rating_pred,
             col_rating=DEFAULT_PREDICTION_COL,
             col_item="not_item",
         )
 
-    with pytest.raises(ValueError):
-        precision_at_k(rating_true, rating_pred, col_rating="not_rating")
+    with pytest.raises(ColumnMismatchError):
+        precision_at_k(rating_true, rating_pred, col_prediction="not_prediction")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ColumnMismatchError):
         recall_at_k(rating_true, rating_pred, col_prediction="not_prediction")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ColumnMismatchError):
         ndcg_at_k(rating_true, rating_true, col_user="not_user")
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ColumnMismatchError):
         map_at_k(
             rating_pred,
             rating_pred,
             col_rating=DEFAULT_PREDICTION_COL,
             col_user="not_user",
         )
 
 
-# test diversity metrics
-@pytest.fixture(scope="module")
-def target_metrics():
-    return {
-        "c_coverage": pytest.approx(0.8, TOL),
-        "d_coverage": pytest.approx(1.9183, TOL),
-        "item_novelty": pd.DataFrame(
-            dict(ItemId=[1, 2, 3, 4, 5], item_novelty=[3.0, 3.0, 2.0, 1.41504, 3.0])
-        ),
-        "novelty": pytest.approx(2.83333, TOL),
-        "diversity": pytest.approx(0.43096, TOL),
-        "user_diversity": pd.DataFrame(
-            dict(UserId=[1, 2, 3], user_diversity=[0.29289, 1.0, 0.0])
-        ),
-        # diversity values when using item features to calculate item similarity
-        "diversity_item_feature_vector": pytest.approx(0.5000, TOL),
-        "user_diversity_item_feature_vector": pd.DataFrame(
-            dict(UserId=[1, 2, 3], user_diversity=[0.5000, 0.5000, 0.5000])
-        ),
-        "user_item_serendipity": pd.DataFrame(
-            dict(
-                UserId=[1, 1, 2, 2, 3, 3],
-                ItemId=[3, 5, 2, 5, 1, 2],
-                user_item_serendipity=[
-                    0.72783,
-                    0.0,
-                    0.71132,
-                    0.35777,
-                    0.80755,
-                    0.0,
-                ],
-            )
-        ),
-        "user_serendipity": pd.DataFrame(
-            dict(UserId=[1, 2, 3], user_serendipity=[0.363915, 0.53455, 0.403775])
-        ),
-        "serendipity": pytest.approx(0.43408, TOL),
-        # serendipity values when using item features to calculate item similarity
-        "user_item_serendipity_item_feature_vector": pd.DataFrame(
-            dict(
-                UserId=[1, 1, 2, 2, 3, 3],
-                ItemId=[3, 5, 2, 5, 1, 2],
-                user_item_serendipity=[
-                    0.5000,
-                    0.0,
-                    0.75,
-                    0.5000,
-                    0.6667,
-                    0.0,
-                ],
-            )
-        ),
-        "user_serendipity_item_feature_vector": pd.DataFrame(
-            dict(UserId=[1, 2, 3], user_serendipity=[0.2500, 0.625, 0.3333])
-        ),
-        "serendipity_item_feature_vector": pytest.approx(0.4028, TOL),
-    }
-
-
-@pytest.fixture(scope="module")
-def python_diversity_data():
-    train_df = pd.DataFrame(
-        {"UserId": [1, 1, 1, 2, 2, 3, 3, 3], "ItemId": [1, 2, 4, 3, 4, 3, 4, 5]}
-    )
-
-    reco_df = pd.DataFrame(
-        {
-            "UserId": [1, 1, 2, 2, 3, 3],
-            "ItemId": [3, 5, 2, 5, 1, 2],
-            "Relevance": [1, 0, 1, 1, 1, 0],
-        }
-    )
-
-    item_feature_df = pd.DataFrame(
-        {
-            "ItemId": [1, 2, 3, 4, 5],
-            "features": [
-                np.array([0.0, 1.0, 1.0, 0.0, 0.0], dtype=float),
-                np.array([0.0, 1.0, 0.0, 1.0, 0.0], dtype=float),
-                np.array([0.0, 0.0, 1.0, 1.0, 0.0], dtype=float),
-                np.array([0.0, 0.0, 1.0, 0.0, 1.0], dtype=float),
-                np.array([0.0, 0.0, 0.0, 1.0, 1.0], dtype=float),
-            ],
-        }
-    )
-    return train_df, reco_df, item_feature_df
-
-
-def test_catalog_coverage(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
+def test_catalog_coverage(diversity_data):
+    train_df, reco_df, _ = diversity_data
     c_coverage = catalog_coverage(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
-    assert c_coverage == target_metrics["c_coverage"]
+    assert c_coverage == pytest.approx(0.8, TOL)
 
 
-def test_distributional_coverage(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
+def test_distributional_coverage(diversity_data):
+    train_df, reco_df, _ = diversity_data
     d_coverage = distributional_coverage(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
-    assert d_coverage == target_metrics["d_coverage"]
+    assert d_coverage == pytest.approx(1.9183, TOL)
 
 
-def test_item_novelty(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
+def test_item_novelty(diversity_data):
+    train_df, reco_df, _ = diversity_data
     actual = historical_item_novelty(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
     assert_frame_equal(
-        target_metrics["item_novelty"], actual, check_exact=False, check_less_precise=4
+        pd.DataFrame(
+            dict(ItemId=[1, 2, 3, 4, 5], item_novelty=[3.0, 3.0, 2.0, 1.41504, 3.0])
+        ),
+        actual,
+        check_exact=False,
     )
     assert np.all(actual["item_novelty"].values >= 0)
     # Test that novelty is zero when data includes only one item
     train_df_new = train_df.loc[train_df["ItemId"] == 3]
     actual = historical_item_novelty(
         train_df=train_df_new, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
     assert actual["item_novelty"].values[0] == 0
 
 
-def test_novelty(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
-    actual = novelty(
+def test_novelty(diversity_data):
+    train_df, reco_df, _ = diversity_data
+    assert novelty(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
-    )
-    assert target_metrics["novelty"] == actual
-    assert actual >= 0
+    ) == pytest.approx(2.83333, TOL)
+
     # Test that novelty is zero when data includes only one item
     train_df_new = train_df.loc[train_df["ItemId"] == 3]
     reco_df_new = reco_df.loc[reco_df["ItemId"] == 3]
     assert (
         novelty(
             train_df=train_df_new,
             reco_df=reco_df_new,
             col_user="UserId",
             col_item="ItemId",
         )
         == 0
     )
 
 
-def test_user_diversity(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
+def test_user_diversity(diversity_data):
+    train_df, reco_df, _ = diversity_data
     actual = user_diversity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=None,
         item_sim_measure="item_cooccurrence_count",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance=None,
     )
     assert_frame_equal(
-        target_metrics["user_diversity"],
+        pd.DataFrame(
+            dict(UserId=[1, 2, 3], user_diversity=[0.29289, 1.0, 0.0])
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
-def test_diversity(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
-    assert target_metrics["diversity"] == diversity(
+def test_diversity(diversity_data):
+    train_df, reco_df, _ = diversity_data
+    assert diversity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=None,
         item_sim_measure="item_cooccurrence_count",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance=None,
-    )
+    ) == pytest.approx(0.43096, TOL)
 
 
-def test_user_item_serendipity(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
+def test_user_item_serendipity(diversity_data):
+    train_df, reco_df, _ = diversity_data
     actual = user_item_serendipity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=None,
         item_sim_measure="item_cooccurrence_count",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance="Relevance",
     )
     assert_frame_equal(
-        target_metrics["user_item_serendipity"],
+        pd.DataFrame(
+            dict(
+                UserId=[1, 1, 2, 2, 3, 3],
+                ItemId=[3, 5, 2, 5, 1, 2],
+                user_item_serendipity=[
+                    0.72783,
+                    0.0,
+                    0.71132,
+                    0.35777,
+                    0.80755,
+                    0.0,
+                ],
+            )
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
     )
 
 
-def test_user_serendipity(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
+def test_user_serendipity(diversity_data):
+    train_df, reco_df, _ = diversity_data
     actual = user_serendipity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=None,
         item_sim_measure="item_cooccurrence_count",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance="Relevance",
     )
     assert_frame_equal(
-        target_metrics["user_serendipity"],
+        pd.DataFrame(
+            dict(UserId=[1, 2, 3], user_serendipity=[0.363915, 0.53455, 0.403775])
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
     )
 
 
-def test_serendipity(python_diversity_data, target_metrics):
-    train_df, reco_df, _ = python_diversity_data
-    assert target_metrics["serendipity"] == serendipity(
+def test_serendipity(diversity_data):
+    train_df, reco_df, _ = diversity_data
+    assert serendipity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=None,
         item_sim_measure="item_cooccurrence_count",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance="Relevance",
-    )
+    ) == pytest.approx(0.43408, TOL)
 
 
-def test_user_diversity_item_feature_vector(python_diversity_data, target_metrics):
-    train_df, reco_df, item_feature_df = python_diversity_data
+def test_user_diversity_item_feature_vector(diversity_data):
+    train_df, reco_df, item_feature_df = diversity_data
     actual = user_diversity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance=None,
     )
     assert_frame_equal(
-        target_metrics["user_diversity_item_feature_vector"],
+        pd.DataFrame(
+            dict(UserId=[1, 2, 3], user_diversity=[0.5000, 0.5000, 0.5000])
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
     )
 
 
-def test_diversity_item_feature_vector(python_diversity_data, target_metrics):
-    train_df, reco_df, item_feature_df = python_diversity_data
-    assert target_metrics["diversity_item_feature_vector"] == diversity(
+def test_diversity_item_feature_vector(diversity_data):
+    train_df, reco_df, item_feature_df = diversity_data
+    assert diversity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance=None,
-    )
+    ) == pytest.approx(0.5000, TOL)
 
 
 def test_user_item_serendipity_item_feature_vector(
-    python_diversity_data, target_metrics
+    diversity_data,
 ):
-    train_df, reco_df, item_feature_df = python_diversity_data
+    train_df, reco_df, item_feature_df = diversity_data
     actual = user_item_serendipity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance="Relevance",
     )
     assert_frame_equal(
-        target_metrics["user_item_serendipity_item_feature_vector"],
+        pd.DataFrame(
+            dict(
+                UserId=[1, 1, 2, 2, 3, 3],
+                ItemId=[3, 5, 2, 5, 1, 2],
+                user_item_serendipity=[
+                    0.5000,
+                    0.0,
+                    0.75,
+                    0.5000,
+                    0.6667,
+                    0.0,
+                ],
+            )
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
-def test_user_serendipity_item_feature_vector(python_diversity_data, target_metrics):
-    train_df, reco_df, item_feature_df = python_diversity_data
+def test_user_serendipity_item_feature_vector(diversity_data):
+    train_df, reco_df, item_feature_df = diversity_data
     actual = user_serendipity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance="Relevance",
     )
     assert_frame_equal(
-        target_metrics["user_serendipity_item_feature_vector"],
+        pd.DataFrame(
+            dict(UserId=[1, 2, 3], user_serendipity=[0.2500, 0.625, 0.3333])
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
-def test_serendipity_item_feature_vector(python_diversity_data, target_metrics):
-    train_df, reco_df, item_feature_df = python_diversity_data
-    assert target_metrics["serendipity_item_feature_vector"] == serendipity(
+def test_serendipity_item_feature_vector(diversity_data):
+    train_df, reco_df, item_feature_df = diversity_data
+    assert serendipity(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
         col_sim="sim",
         col_relevance="Relevance",
-    )
+    ) == pytest.approx(0.4028, TOL)
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/evaluation/test_python_evaluation_time_performance.py` & `recommenders-1.2.0/tests/performance/recommenders/evaluation/test_python_evaluation_time_performance.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import numpy as np
 import pandas as pd
 import pytest
+import random
 from sklearn.preprocessing import minmax_scale
 
+from recommenders.utils.timer import Timer
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
     DEFAULT_ITEM_COL,
     DEFAULT_RATING_COL,
     DEFAULT_PREDICTION_COL,
     SEED,
 )
@@ -24,23 +26,21 @@
     precision_at_k,
     recall_at_k,
     ndcg_at_k,
     map_at_k,
     auc,
     logloss,
 )
-import random
-from recommenders.utils.timer import Timer
+
 
 random.seed(SEED)
-DATA_USER_NUM = 10000
+DATA_USER_NUM = 5000
 DATA_ITEM_NUM = DATA_USER_NUM * 2
 DATA_SAMPLE_NUM = DATA_USER_NUM * 1000
 DATA_RATING_MAX = 5
-
 TOL = 0.1
 
 
 # fmt: off
 @pytest.fixture
 def rating_true():
     return pd.DataFrame(
@@ -79,160 +79,156 @@
     rating_pred[DEFAULT_PREDICTION_COL] = minmax_scale(
         rating_pred[DEFAULT_PREDICTION_COL].astype(float)
     )
     return rating_pred
 
 
 # The following time thresholds are benchmarked on Azure
-# Standard_D14_v2 VM, with Intel(R) Xeon(R) CPU E5-2673 v3 @ 2.40GHz,
-# 16 cores, 112 GB RAM, 800 GB disk.
-# The thresholds are calculated by MEAN + 5 * STANDARD DEVIATION.
-
-
+# Standard_A8m_v2 with 8 vCPUs and 64 GiB memory.
 def test_merge_rating(rating_true, rating_pred):
     with Timer() as t:
         merge_rating_true_pred(
             rating_true,
             rating_pred,
             col_user=DEFAULT_USER_COL,
             col_item=DEFAULT_ITEM_COL,
             col_rating=DEFAULT_RATING_COL,
             col_prediction=DEFAULT_PREDICTION_COL,
         )
-    assert t.interval < 19.81252386 * (1 + TOL)
+    assert t.interval < 40 * (1 + TOL)
 
 
 def test_merge_ranking(rating_true, rating_pred):
     with Timer() as t:
         merge_ranking_true_pred(
             rating_true,
             rating_pred,
             col_user=DEFAULT_USER_COL,
             col_item=DEFAULT_ITEM_COL,
             col_rating=DEFAULT_RATING_COL,
             col_prediction=DEFAULT_PREDICTION_COL,
             relevancy_method="top_k",
         )
-    assert t.interval < 22.01327171 * (1 + TOL)
+    assert t.interval < 45 * (1 + TOL)
 
 
 def test_python_rmse(rating_true, rating_pred):
     with Timer() as t:
         rmse(
             rating_true=rating_true,
             rating_pred=rating_pred,
             col_prediction=DEFAULT_PREDICTION_COL,
         )
-    assert t.interval < 29.95031411 * (1 + TOL)
+    assert t.interval < 40 * (1 + TOL)
 
 
 def test_python_mae(rating_true, rating_pred):
     with Timer() as t:
         mae(
             rating_true=rating_true,
             rating_pred=rating_pred,
             col_prediction=DEFAULT_PREDICTION_COL,
         )
-    assert t.interval < 30.45756622 * (1 + TOL)
+    assert t.interval < 40 * (1 + TOL)
 
 
 def test_python_rsquared(rating_true, rating_pred):
     with Timer() as t:
         rsquared(
             rating_true=rating_true,
             rating_pred=rating_pred,
             col_prediction=DEFAULT_PREDICTION_COL,
         )
-    assert t.interval < 30.60572284 * (1 + TOL)
+    assert t.interval < 40 * (1 + TOL)
 
 
 def test_python_exp_var(rating_true, rating_pred):
     with Timer() as t:
         exp_var(
             rating_true=rating_true,
             rating_pred=rating_pred,
             col_prediction=DEFAULT_PREDICTION_COL,
         )
-    assert t.interval < 31.01451915 * (1 + TOL)
+    assert t.interval < 40 * (1 + TOL)
 
 
 def test_get_top_k_items(rating_true):
     with Timer() as t:
         get_top_k_items(
             dataframe=rating_true,
             col_user=DEFAULT_USER_COL,
             col_rating=DEFAULT_RATING_COL,
             k=10,
         )
-    assert t.interval < 3.90527593 * (1 + TOL)
+    assert t.interval < 10 * (1 + TOL)
 
 
 def test_get_top_k_items_largek(rating_true):
     with Timer() as t:
         get_top_k_items(
             dataframe=rating_true,
             col_user=DEFAULT_USER_COL,
             col_rating=DEFAULT_RATING_COL,
             k=1000,
         )
-    assert t.interval < 4.83998316 * (1 + TOL)
+    assert t.interval < 10 * (1 + TOL)
 
 
 def test_python_ndcg_at_k(rating_true, rating_pred):
     with Timer() as t:
         ndcg_at_k(
             rating_true=rating_true,
             rating_pred=rating_pred,
             col_prediction=DEFAULT_PREDICTION_COL,
             k=10,
         )
-    assert t.interval < 21.55627936 * (1 + TOL)
+    assert t.interval < 80 * (1 + TOL)
 
 
 def test_python_map_at_k(rating_true, rating_pred):
     with Timer() as t:
         map_at_k(
             rating_true=rating_true,
             rating_pred=rating_pred,
             col_prediction=DEFAULT_PREDICTION_COL,
             k=10,
         )
-    assert t.interval < 29.90376154 * (1 + TOL)
+    assert t.interval < 50 * (1 + TOL)
 
 
 def test_python_precision(rating_true, rating_pred):
     with Timer() as t:
         precision_at_k(rating_true, rating_pred, k=10)
-    assert t.interval < 29.95129834 * (1 + TOL)
+    assert t.interval < 50 * (1 + TOL)
 
 
 def test_python_recall(rating_true, rating_pred):
     with Timer() as t:
         recall_at_k(
             rating_true=rating_true,
             rating_pred=rating_pred,
             col_prediction=DEFAULT_PREDICTION_COL,
             k=10,
         )
-    assert t.interval < 30.29558967 * (1 + TOL)
+    assert t.interval < 50 * (1 + TOL)
 
 
 def test_python_auc(rating_true_binary, rating_pred_binary):
     with Timer() as t:
         auc(
             rating_true=rating_true_binary,
             rating_pred=rating_pred_binary,
             col_rating=DEFAULT_RATING_COL,
             col_prediction=DEFAULT_PREDICTION_COL,
         )
-    assert t.interval < 22.18870257 * (1 + TOL)
+    assert t.interval < 45 * (1 + TOL)
 
 
 def test_python_logloss(rating_true_binary, rating_pred_binary):
     with Timer() as t:
         logloss(
             rating_true=rating_true_binary,
             rating_pred=rating_pred_binary,
             col_rating=DEFAULT_RATING_COL,
             col_prediction=DEFAULT_PREDICTION_COL,
         )
-    assert t.interval < 32.91629787 * (1 + TOL)
+    assert t.interval < 45 * (1 + TOL)
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/evaluation/test_spark_evaluation.py` & `recommenders-1.2.0/tests/unit/recommenders/evaluation/test_spark_evaluation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,193 +1,62 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
+import pytest
 import numpy as np
 import pandas as pd
-import pytest
-from pandas.util.testing import assert_frame_equal
+from pandas.testing import assert_frame_equal
 
 from recommenders.evaluation.python_evaluation import (
     precision_at_k,
     recall_at_k,
     ndcg_at_k,
     map_at_k,
+    map,
 )
 
 try:
-    from pyspark.sql import Row
-    from pyspark.ml.linalg import Vectors, VectorUDT
-    from pyspark.sql.types import StructField, StructType, IntegerType
+    from pyspark.ml.functions import array_to_vector
+    from pyspark.sql.types import ArrayType, FloatType, IntegerType, StructField, StructType
     from recommenders.evaluation.spark_evaluation import (
         SparkDiversityEvaluation,
         SparkRankingEvaluation,
         SparkRatingEvaluation,
     )
 except ImportError:
     pass  # skip this import if we are in pure python environment
 
 
 TOL = 0.0001
 
 
-@pytest.fixture(scope="module")
-def target_metrics():
-    return {
-        "rmse": pytest.approx(7.254309, TOL),
-        "mae": pytest.approx(6.375, TOL),
-        "rsquared": pytest.approx(-31.699029, TOL),
-        "exp_var": pytest.approx(-6.4466, 0.01),
-        "ndcg": pytest.approx(0.38172, TOL),
-        "precision": pytest.approx(0.26666, TOL),
-        "map": pytest.approx(0.23613, TOL),
-        "recall": pytest.approx(0.37777, TOL),
-        "c_coverage": pytest.approx(0.8, TOL),
-        "d_coverage": pytest.approx(1.9183, TOL),
-        "item_novelty": pd.DataFrame(
-            dict(ItemId=[1, 2, 3, 4, 5], item_novelty=[3.0, 3.0, 2.0, 1.41504, 3.0])
-        ),
-        "novelty": pytest.approx(2.83333, TOL),
-        # diversity when using item co-occurrence count to calculate item similarity
-        "diversity": pytest.approx(0.43096, TOL),
-        "user_diversity": pd.DataFrame(
-            dict(UserId=[1, 2, 3], user_diversity=[0.29289, 1.0, 0.0])
-        ),
-        # diversity values when using item features to calculate item similarity
-        "diversity_item_feature_vector": pytest.approx(0.5000, TOL),
-        "user_diversity_item_feature_vector": pd.DataFrame(
-            dict(UserId=[1, 2, 3], user_diversity=[0.5000, 0.5000, 0.5000])
-        ),
-        "user_item_serendipity": pd.DataFrame(
-            dict(
-                UserId=[1, 1, 2, 2, 3, 3],
-                ItemId=[3, 5, 2, 5, 1, 2],
-                user_item_serendipity=[
-                    0.72783,
-                    0.0,
-                    0.71132,
-                    0.35777,
-                    0.80755,
-                    0.0,
-                ],
-            )
-        ),
-        "user_serendipity": pd.DataFrame(
-            dict(UserId=[1, 2, 3], user_serendipity=[0.363915, 0.53455, 0.403775])
-        ),
-        "serendipity": pytest.approx(0.43408, TOL),
-        # serendipity values when using item features to calculate item similarity
-        "user_item_serendipity_item_feature_vector": pd.DataFrame(
-            dict(
-                UserId=[1, 1, 2, 2, 3, 3],
-                ItemId=[3, 5, 2, 5, 1, 2],
-                user_item_serendipity=[
-                    0.5000,
-                    0.0,
-                    0.75,
-                    0.5000,
-                    0.6667,
-                    0.0,
-                ],
-            )
-        ),
-        "user_serendipity_item_feature_vector": pd.DataFrame(
-            dict(UserId=[1, 2, 3], user_serendipity=[0.2500, 0.625, 0.3333])
-        ),
-        "serendipity_item_feature_vector": pytest.approx(0.4028, TOL),
-    }
-
-
-@pytest.fixture(scope="module")
-def python_data():
-    rating_true = pd.DataFrame(
-        {
-            "userID": [1, 1, 1, 2, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3],
-            "itemID": [1, 2, 3, 1, 4, 5, 6, 7, 2, 5, 6, 8, 9, 10, 11, 12, 13, 14],
-            "rating": [5, 4, 3, 5, 5, 3, 3, 1, 5, 5, 5, 4, 4, 3, 3, 3, 2, 1],
-        }
-    )
-    rating_pred = pd.DataFrame(
-        {
-            "userID": [1, 1, 1, 2, 2, 2, 2, 2, 3, 3, 3, 3, 3, 3, 3, 3, 3, 3],
-            "itemID": [3, 10, 12, 10, 3, 5, 11, 13, 4, 10, 7, 13, 1, 3, 5, 2, 11, 14],
-            "prediction": [
-                14,
-                13,
-                12,
-                14,
-                13,
-                12,
-                11,
-                10,
-                14,
-                13,
-                12,
-                11,
-                10,
-                9,
-                8,
-                7,
-                6,
-                5,
-            ],
-        }
-    )
-    return rating_true, rating_pred
-
-
-@pytest.fixture(scope="module")
-def spark_data(python_data, spark):
-    rating_true, rating_pred = python_data
-
+@pytest.fixture
+def spark_data(rating_true, rating_pred, spark):
     df_true = spark.createDataFrame(rating_true)
     df_pred = spark.createDataFrame(rating_pred)
 
     return df_true, df_pred
 
 
-@pytest.fixture(scope="module")
-def spark_diversity_data(spark):
-    train_df = spark.createDataFrame(
-        [
-            Row(UserId=1, ItemId=1),
-            Row(UserId=1, ItemId=2),
-            Row(UserId=1, ItemId=4),
-            Row(UserId=2, ItemId=3),
-            Row(UserId=2, ItemId=4),
-            Row(UserId=3, ItemId=3),
-            Row(UserId=3, ItemId=4),
-            Row(UserId=3, ItemId=5),
-        ]
-    )
-    reco_df = spark.createDataFrame(
-        [
-            Row(UserId=1, ItemId=3, Relevance=1),
-            Row(UserId=1, ItemId=5, Relevance=0),
-            Row(UserId=2, ItemId=2, Relevance=1),
-            Row(UserId=2, ItemId=5, Relevance=1),
-            Row(UserId=3, ItemId=1, Relevance=1),
-            Row(UserId=3, ItemId=2, Relevance=0),
-        ]
-    )
-
+@pytest.fixture
+def spark_diversity_data(diversity_data, spark):
+    train_df, reco_df, item_feature_df = diversity_data
+    
+    train_df = spark.createDataFrame(train_df)
+    reco_df = spark.createDataFrame(reco_df)
+    item_feature_df["features"] = item_feature_df["features"].apply(lambda x: x.tolist())
     field = [
         StructField("ItemId", IntegerType(), True),
-        StructField("features", VectorUDT(), True),
+        StructField("features", ArrayType(FloatType()), True),
     ]
-    schema = StructType(field)
-    item_feature_df = spark.createDataFrame(
-        [
-            Row(ItemId=1, features=Vectors.sparse(5, [1, 2], [1.0, 1.0])),
-            Row(ItemId=2, features=Vectors.sparse(5, [1, 3], [1.0, 1.0])),
-            Row(ItemId=3, features=Vectors.sparse(5, [2, 3], [1.0, 1.0])),
-            Row(ItemId=4, features=Vectors.sparse(5, [2, 4], [1.0, 1.0])),
-            Row(ItemId=5, features=Vectors.sparse(5, [3, 4], [1.0, 1.0])),
-        ],
-        schema,
-    )
+    item_feature_df = spark.createDataFrame(item_feature_df, schema=StructType(field))
+    # Array[Float] to VectorUDT
+    item_feature_df = item_feature_df.withColumn("features", array_to_vector(item_feature_df["features"]))
+
     return train_df, reco_df, item_feature_df
 
 
 @pytest.mark.spark
 def test_init_spark(spark):
     assert spark is not None
 
@@ -196,444 +65,453 @@
 def test_init_spark_rating_eval(spark_data):
     df_true, df_pred = spark_data
     evaluator = SparkRatingEvaluation(df_true, df_pred)
     assert evaluator is not None
 
 
 @pytest.mark.spark
-def test_spark_rmse(spark_data, target_metrics):
+def test_spark_rmse(spark_data):
     df_true, df_pred = spark_data
 
-    evaluator1 = SparkRatingEvaluation(df_true, df_true, col_prediction="rating")
-    assert evaluator1.rmse() == 0
+    evaluator = SparkRatingEvaluation(df_true, df_true, col_prediction="rating")
+    assert evaluator.rmse() == 0
 
-    evaluator2 = SparkRatingEvaluation(df_true, df_pred)
-    assert evaluator2.rmse() == target_metrics["rmse"]
+    evaluator = SparkRatingEvaluation(df_true, df_pred)
+    assert evaluator.rmse() == pytest.approx(7.254309, TOL)
 
 
 @pytest.mark.spark
-def test_spark_mae(spark_data, target_metrics):
+def test_spark_mae(spark_data):
     df_true, df_pred = spark_data
 
-    evaluator1 = SparkRatingEvaluation(df_true, df_true, col_prediction="rating")
-    assert evaluator1.mae() == 0
+    evaluator = SparkRatingEvaluation(df_true, df_true, col_prediction="rating")
+    assert evaluator.mae() == 0
 
-    evaluator2 = SparkRatingEvaluation(df_true, df_pred)
-    assert evaluator2.mae() == target_metrics["mae"]
+    evaluator = SparkRatingEvaluation(df_true, df_pred)
+    assert evaluator.mae() == pytest.approx(6.375, TOL)
 
 
 @pytest.mark.spark
-def test_spark_rsquared(spark_data, target_metrics):
+def test_spark_rsquared(spark_data):
     df_true, df_pred = spark_data
 
-    evaluator1 = SparkRatingEvaluation(df_true, df_true, col_prediction="rating")
-    assert evaluator1.rsquared() == pytest.approx(1.0, TOL)
+    evaluator = SparkRatingEvaluation(df_true, df_true, col_prediction="rating")
+    assert evaluator.rsquared() == pytest.approx(1.0, TOL)
 
-    evaluator2 = SparkRatingEvaluation(df_true, df_pred)
-    assert evaluator2.rsquared() == target_metrics["rsquared"]
+    evaluator = SparkRatingEvaluation(df_true, df_pred)
+    assert evaluator.rsquared() == pytest.approx(-31.699029, TOL)
 
 
 @pytest.mark.spark
-def test_spark_exp_var(spark_data, target_metrics):
+def test_spark_exp_var(spark_data):
     df_true, df_pred = spark_data
 
-    evaluator1 = SparkRatingEvaluation(df_true, df_true, col_prediction="rating")
-    assert evaluator1.exp_var() == pytest.approx(1.0, TOL)
+    evaluator = SparkRatingEvaluation(df_true, df_true, col_prediction="rating")
+    assert evaluator.exp_var() == pytest.approx(1.0, TOL)
 
-    evaluator2 = SparkRatingEvaluation(df_true, df_pred)
-    assert evaluator2.exp_var() == target_metrics["exp_var"]
+    evaluator = SparkRatingEvaluation(df_true, df_pred)
+    assert evaluator.exp_var() == pytest.approx(-6.4466, TOL)
 
 
 @pytest.mark.spark
-def test_spark_recall(spark_data, target_metrics):
+def test_spark_recall_at_k(spark_data):
     df_true, df_pred = spark_data
 
     evaluator = SparkRankingEvaluation(df_true, df_pred)
-    assert evaluator.recall_at_k() == target_metrics["recall"]
+    assert evaluator.recall_at_k() == pytest.approx(0.37777, TOL)
 
-    evaluator1 = SparkRankingEvaluation(
+    evaluator = SparkRankingEvaluation(
         df_true, df_pred, relevancy_method="by_threshold", threshold=3.5
     )
-    assert evaluator1.recall_at_k() == target_metrics["recall"]
+    assert evaluator.recall_at_k() == pytest.approx(0.37777, TOL)
 
 
 @pytest.mark.spark
-def test_spark_precision(spark_data, target_metrics, spark):
+def test_spark_precision_at_k(spark_data, spark):
     df_true, df_pred = spark_data
 
     evaluator = SparkRankingEvaluation(df_true, df_pred, k=10)
-    assert evaluator.precision_at_k() == target_metrics["precision"]
+    assert evaluator.precision_at_k() == pytest.approx(0.26666, TOL)
 
-    evaluator1 = SparkRankingEvaluation(
+    evaluator = SparkRankingEvaluation(
         df_true, df_pred, relevancy_method="by_threshold", threshold=3.5
     )
-    assert evaluator1.precision_at_k() == target_metrics["precision"]
+    assert evaluator.precision_at_k() == pytest.approx(0.26666, TOL)
 
     # Check normalization
     single_user = pd.DataFrame(
         {"userID": [1, 1, 1], "itemID": [1, 2, 3], "rating": [5, 4, 3]}
     )
     df_single = spark.createDataFrame(single_user)
-    evaluator2 = SparkRankingEvaluation(
+    evaluator = SparkRankingEvaluation(
         df_single, df_single, k=3, col_prediction="rating"
     )
-    assert evaluator2.precision_at_k() == 1
+    assert evaluator.precision_at_k() == 1
 
     same_items = pd.DataFrame(
         {
             "userID": [1, 1, 1, 2, 2, 2],
             "itemID": [1, 2, 3, 1, 2, 3],
             "rating": [5, 4, 3, 5, 5, 3],
         }
     )
     df_same = spark.createDataFrame(same_items)
-    evaluator3 = SparkRankingEvaluation(df_same, df_same, k=3, col_prediction="rating")
-    assert evaluator3.precision_at_k() == 1
+    evaluator = SparkRankingEvaluation(df_same, df_same, k=3, col_prediction="rating")
+    assert evaluator.precision_at_k() == 1
 
     # Check that if the sample size is smaller than k, the maximum precision can not be 1
     # if we do precision@5 when there is only 3 items, we can get a maximum of 3/5.
-    evaluator4 = SparkRankingEvaluation(df_same, df_same, k=5, col_prediction="rating")
-    assert evaluator4.precision_at_k() == 0.6
+    evaluator = SparkRankingEvaluation(df_same, df_same, k=5, col_prediction="rating")
+    assert evaluator.precision_at_k() == 0.6
 
 
 @pytest.mark.spark
-def test_spark_ndcg(spark_data, target_metrics):
+def test_spark_ndcg_at_k(spark_data):
     df_true, df_pred = spark_data
 
-    evaluator0 = SparkRankingEvaluation(df_true, df_true, k=10, col_prediction="rating")
-    assert evaluator0.ndcg_at_k() == 1.0
+    evaluator = SparkRankingEvaluation(df_true, df_true, k=10, col_prediction="rating")
+    assert evaluator.ndcg_at_k() == 1.0
 
     evaluator = SparkRankingEvaluation(df_true, df_pred, k=10)
-    assert evaluator.ndcg_at_k() == target_metrics["ndcg"]
+    assert evaluator.ndcg_at_k() == pytest.approx(0.38172, TOL)
 
-    evaluator1 = SparkRankingEvaluation(
+    evaluator = SparkRankingEvaluation(
         df_true, df_pred, relevancy_method="by_threshold", threshold=3.5
     )
-    assert evaluator1.ndcg_at_k() == target_metrics["ndcg"]
+    assert evaluator.ndcg_at_k() == pytest.approx(0.38172, TOL)
 
 
 @pytest.mark.spark
-def test_spark_map(spark_data, target_metrics):
+def test_spark_map(spark_data):
     df_true, df_pred = spark_data
 
-    evaluator1 = SparkRankingEvaluation(
-        k=10, rating_true=df_true, rating_pred=df_true, col_prediction="rating"
-    )
-    assert evaluator1.map_at_k() == 1.0
+    evaluator = SparkRankingEvaluation(df_true, df_true, k=10, col_prediction="rating")
+    assert evaluator.map() == 1.0
 
     evaluator = SparkRankingEvaluation(df_true, df_pred, k=10)
-    assert evaluator.map_at_k() == target_metrics["map"]
+    assert evaluator.map() == pytest.approx(0.23613, TOL)
 
-    evaluator1 = SparkRankingEvaluation(
+    evaluator = SparkRankingEvaluation(
         df_true, df_pred, relevancy_method="by_threshold", threshold=3.5
     )
-    assert evaluator1.map_at_k() == target_metrics["map"]
+    assert evaluator.map() == pytest.approx(0.23613, TOL)
 
 
 @pytest.mark.spark
-def test_spark_python_match(python_data, spark):
-    # Test on the original data with k = 10.
-    df_true, df_pred = python_data
+def test_spark_map_at_k(spark_data):
+    df_true, df_pred = spark_data
 
-    dfs_true = spark.createDataFrame(df_true)
-    dfs_pred = spark.createDataFrame(df_pred)
+    evaluator = SparkRankingEvaluation(df_true, df_true, k=10, col_prediction="rating")
+    assert evaluator.map_at_k() == 1.0
 
-    eval_spark1 = SparkRankingEvaluation(dfs_true, dfs_pred, k=10)
+    evaluator = SparkRankingEvaluation(df_true, df_pred, k=10)
+    assert evaluator.map_at_k() == pytest.approx(0.23613, TOL)
 
-    assert recall_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark1.recall_at_k(), TOL
-    )
-    assert precision_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark1.precision_at_k(), TOL
-    )
-    assert ndcg_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark1.ndcg_at_k(), TOL
-    )
-    assert map_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark1.map_at_k(), TOL
+    evaluator = SparkRankingEvaluation(
+        df_true, df_pred, relevancy_method="by_threshold", threshold=3.5
     )
+    assert evaluator.map_at_k() == pytest.approx(0.23613, TOL)
 
-    # Test on the original data with k = 3.
-    dfs_true = spark.createDataFrame(df_true)
-    dfs_pred = spark.createDataFrame(df_pred)
-
-    eval_spark2 = SparkRankingEvaluation(dfs_true, dfs_pred, k=3)
-
-    assert recall_at_k(df_true, df_pred, k=3) == pytest.approx(
-        eval_spark2.recall_at_k(), TOL
-    )
-    assert precision_at_k(df_true, df_pred, k=3) == pytest.approx(
-        eval_spark2.precision_at_k(), TOL
-    )
-    assert ndcg_at_k(df_true, df_pred, k=3) == pytest.approx(
-        eval_spark2.ndcg_at_k(), TOL
-    )
-    assert map_at_k(df_true, df_pred, k=3) == pytest.approx(eval_spark2.map_at_k(), TOL)
 
-    # Remove the first row from the original data.
-    df_pred = df_pred[1:-1]
+@pytest.mark.spark
+@pytest.mark.parametrize(
+    "k,pred_start_row_i,user_id",
+    [
+        (10, 0, None),
+        (3, 0, None),   # Different k
+        (10, 0, None),  # Different pred
+        (10, 0, 3),     # Test with one user (userID == 3)
+    ]
+)
+def test_spark_python_match(rating_true, rating_pred, spark, k, pred_start_row_i, user_id):
+    df_true, df_pred = rating_true, rating_pred
+    df_pred = df_pred[pred_start_row_i:]
+    if user_id is not None:
+        df_pred = df_pred.loc[df_pred["userID"] == 3]
+        df_true = df_true.loc[df_true["userID"] == 3]
 
     dfs_true = spark.createDataFrame(df_true)
     dfs_pred = spark.createDataFrame(df_pred)
 
-    eval_spark3 = SparkRankingEvaluation(dfs_true, dfs_pred, k=10)
+    # Test on the original data with k = 10.
+    evaluator = SparkRankingEvaluation(dfs_true, dfs_pred, k=k)
 
-    assert recall_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark3.recall_at_k(), TOL
-    )
-    assert precision_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark3.precision_at_k(), TOL
+    assert recall_at_k(df_true, df_pred, k=k) == pytest.approx(
+        evaluator.recall_at_k(), TOL
     )
-    assert ndcg_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark3.ndcg_at_k(), TOL
+    assert precision_at_k(df_true, df_pred, k=k) == pytest.approx(
+        evaluator.precision_at_k(), TOL
     )
-    assert map_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark3.map_at_k(), TOL
+    assert ndcg_at_k(df_true, df_pred, k=k) == pytest.approx(
+        evaluator.ndcg_at_k(), TOL
     )
-
-    # Test with one user
-    df_pred = df_pred.loc[df_pred["userID"] == 3]
-    df_true = df_true.loc[df_true["userID"] == 3]
-
-    dfs_true = spark.createDataFrame(df_true)
-    dfs_pred = spark.createDataFrame(df_pred)
-
-    eval_spark4 = SparkRankingEvaluation(dfs_true, dfs_pred, k=10)
-
-    assert recall_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark4.recall_at_k(), TOL
-    )
-    assert precision_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark4.precision_at_k(), TOL
-    )
-    assert ndcg_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark4.ndcg_at_k(), TOL
+    assert map_at_k(df_true, df_pred, k=k) == pytest.approx(
+        evaluator.map_at_k(), TOL
     )
-    assert map_at_k(df_true, df_pred, k=10) == pytest.approx(
-        eval_spark4.map_at_k(), TOL
+    assert map(df_true, df_pred, k=k) == pytest.approx(
+        evaluator.map(), TOL
     )
 
 
 @pytest.mark.spark
-def test_catalog_coverage(spark_diversity_data, target_metrics):
+def test_catalog_coverage(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
     c_coverage = evaluator.catalog_coverage()
-    assert c_coverage == target_metrics["c_coverage"]
+    assert c_coverage == pytest.approx(0.8, TOL)
 
 
 @pytest.mark.spark
-def test_distributional_coverage(spark_diversity_data, target_metrics):
+def test_distributional_coverage(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
     d_coverage = evaluator.distributional_coverage()
-    assert d_coverage == target_metrics["d_coverage"]
+    assert d_coverage == pytest.approx(1.9183, TOL)
 
 
 @pytest.mark.spark
-def test_item_novelty(spark_diversity_data, target_metrics):
+def test_item_novelty(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
+
     evaluator = SparkDiversityEvaluation(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
     actual = evaluator.historical_item_novelty().toPandas()
     assert_frame_equal(
-        target_metrics["item_novelty"], actual, check_exact=False, check_less_precise=4
+        pd.DataFrame(
+            dict(ItemId=[1, 2, 3, 4, 5], item_novelty=[3.0, 3.0, 2.0, 1.41504, 3.0])
+        ),
+        actual,
+        check_exact=False,
+        atol=TOL,
     )
     assert np.all(actual["item_novelty"].values >= 0)
     # Test that novelty is zero when data includes only one item
     train_df_new = train_df.filter("ItemId == 3")
     evaluator = SparkDiversityEvaluation(
         train_df=train_df_new, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
     actual = evaluator.historical_item_novelty().toPandas()
     assert actual["item_novelty"].values[0] == 0
 
 
 @pytest.mark.spark
-def test_novelty(spark_diversity_data, target_metrics):
+def test_novelty(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
-    novelty = evaluator.novelty()
-    assert target_metrics["novelty"] == novelty
-    assert novelty >= 0
+    assert evaluator.novelty() == pytest.approx(2.83333, TOL)
+
     # Test that novelty is zero when data includes only one item
     train_df_new = train_df.filter("ItemId == 3")
     reco_df_new = reco_df.filter("ItemId == 3")
     evaluator = SparkDiversityEvaluation(
         train_df=train_df_new, reco_df=reco_df_new, col_user="UserId", col_item="ItemId"
     )
     assert evaluator.novelty() == 0
 
 
 @pytest.mark.spark
-def test_user_diversity(spark_diversity_data, target_metrics):
+def test_user_diversity(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
     actual = evaluator.user_diversity().toPandas()
     assert_frame_equal(
-        target_metrics["user_diversity"],
+        pd.DataFrame(
+            dict(UserId=[1, 2, 3], user_diversity=[0.29289, 1.0, 0.0])
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
 @pytest.mark.spark
-def test_diversity(spark_diversity_data, target_metrics):
+def test_diversity(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df, reco_df=reco_df, col_user="UserId", col_item="ItemId"
     )
-    assert target_metrics["diversity"] == evaluator.diversity()
+    assert evaluator.diversity() == pytest.approx(0.43096, TOL)
 
 
 @pytest.mark.spark
-def test_user_item_serendipity(spark_diversity_data, target_metrics):
+def test_user_item_serendipity(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df,
         reco_df=reco_df,
         col_user="UserId",
         col_item="ItemId",
         col_relevance="Relevance",
     )
     actual = evaluator.user_item_serendipity().toPandas()
     assert_frame_equal(
-        target_metrics["user_item_serendipity"],
+        pd.DataFrame(
+            dict(
+                UserId=[1, 1, 2, 2, 3, 3],
+                ItemId=[3, 5, 2, 5, 1, 2],
+                user_item_serendipity=[
+                    0.72783,
+                    0.0,
+                    0.71132,
+                    0.35777,
+                    0.80755,
+                    0.0,
+                ],
+            )
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
 @pytest.mark.spark
-def test_user_serendipity(spark_diversity_data, target_metrics):
+def test_user_serendipity(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df,
         reco_df=reco_df,
         col_user="UserId",
         col_item="ItemId",
         col_relevance="Relevance",
     )
     actual = evaluator.user_serendipity().toPandas()
     assert_frame_equal(
-        target_metrics["user_serendipity"],
+        pd.DataFrame(
+            dict(UserId=[1, 2, 3], user_serendipity=[0.363915, 0.53455, 0.403775])
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
 @pytest.mark.spark
-def test_serendipity(spark_diversity_data, target_metrics):
+def test_serendipity(spark_diversity_data):
     train_df, reco_df, _ = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df,
         reco_df=reco_df,
         col_user="UserId",
         col_item="ItemId",
         col_relevance="Relevance",
     )
-    assert target_metrics["serendipity"] == evaluator.serendipity()
+    assert evaluator.serendipity() == pytest.approx(0.43408, TOL)
 
 
 @pytest.mark.spark
-def test_user_diversity_item_feature_vector(spark_diversity_data, target_metrics):
+def test_user_diversity_item_feature_vector(spark_diversity_data):
     train_df, reco_df, item_feature_df = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
     )
     actual = evaluator.user_diversity().toPandas()
     assert_frame_equal(
-        target_metrics["user_diversity_item_feature_vector"],
+        pd.DataFrame(
+            dict(UserId=[1, 2, 3], user_diversity=[0.5000, 0.5000, 0.5000])
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
 @pytest.mark.spark
-def test_diversity_item_feature_vector(spark_diversity_data, target_metrics):
+def test_diversity_item_feature_vector(spark_diversity_data):
     train_df, reco_df, item_feature_df = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
     )
-    assert target_metrics["diversity_item_feature_vector"] == evaluator.diversity()
+    assert evaluator.diversity() == pytest.approx(0.5000, TOL)
 
 
 @pytest.mark.spark
 def test_user_item_serendipity_item_feature_vector(
-    spark_diversity_data, target_metrics
+    spark_diversity_data,
 ):
     train_df, reco_df, item_feature_df = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
         col_relevance="Relevance",
     )
     actual = evaluator.user_item_serendipity().toPandas()
     assert_frame_equal(
-        target_metrics["user_item_serendipity_item_feature_vector"],
+        pd.DataFrame(
+            dict(
+                UserId=[1, 1, 2, 2, 3, 3],
+                ItemId=[3, 5, 2, 5, 1, 2],
+                user_item_serendipity=[
+                    0.5000,
+                    0.0,
+                    0.75,
+                    0.5000,
+                    0.6667,
+                    0.0,
+                ],
+            )
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
 @pytest.mark.spark
-def test_user_serendipity_item_feature_vector(spark_diversity_data, target_metrics):
+def test_user_serendipity_item_feature_vector(spark_diversity_data):
     train_df, reco_df, item_feature_df = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
         col_relevance="Relevance",
     )
     actual = evaluator.user_serendipity().toPandas()
     assert_frame_equal(
-        target_metrics["user_serendipity_item_feature_vector"],
+        pd.DataFrame(
+            dict(UserId=[1, 2, 3], user_serendipity=[0.2500, 0.625, 0.3333])
+        ),
         actual,
         check_exact=False,
-        check_less_precise=4,
+        atol=TOL,
     )
 
 
 @pytest.mark.spark
-def test_serendipity_item_feature_vector(spark_diversity_data, target_metrics):
+def test_serendipity_item_feature_vector(spark_diversity_data):
     train_df, reco_df, item_feature_df = spark_diversity_data
     evaluator = SparkDiversityEvaluation(
         train_df=train_df,
         reco_df=reco_df,
         item_feature_df=item_feature_df,
         item_sim_measure="item_feature_vector",
         col_user="UserId",
         col_item="ItemId",
         col_relevance="Relevance",
     )
-    assert target_metrics["serendipity_item_feature_vector"] == evaluator.serendipity()
+    assert evaluator.serendipity() == pytest.approx(0.4028, TOL)
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_cornac_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_cornac_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
-import pandas as pd
 import pytest
+import pandas as pd
 import cornac
 
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
     DEFAULT_ITEM_COL,
     DEFAULT_RATING_COL,
 )
 from recommenders.models.cornac.cornac_utils import predict, predict_ranking
 from recommenders.evaluation.python_evaluation import mae, rmse, ndcg_at_k, recall_at_k
 
+
 TOL = 0.001
 
 
 @pytest.fixture
 def rating_true():
     return pd.DataFrame(
         {
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_deeprec_model.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_deeprec_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import pytest
+
 import os
+import pytest
+
 from recommenders.datasets import movielens
 from recommenders.datasets.amazon_reviews import (
     download_and_extract,
     data_preprocessing,
 )
 from recommenders.datasets.python_splitters import python_stratified_split
 
@@ -33,43 +35,23 @@
     from recommenders.models.deeprec.models.sequential.sum import SUMModel
     from recommenders.models.deeprec.models.xDeepFM import XDeepFMModel
 except ImportError:
     pass  # skip this import if we are in cpu environment
 
 
 @pytest.mark.gpu
-def test_xdeepfm_component_definition(deeprec_resource_path):
-    data_path = os.path.join(deeprec_resource_path, "xdeepfm")
-    yaml_file = os.path.join(data_path, "xDeepFM.yaml")
-
-    if not os.path.exists(yaml_file):
-        download_deeprec_resources(
-            "https://recodatasets.z20.web.core.windows.net/deeprec/",
-            data_path,
-            "xdeepfmresources.zip",
-        )
-
-    hparams = prepare_hparams(yaml_file)
-    model = XDeepFMModel(hparams, FFMTextIterator)
-
-    assert model.logit is not None
-    assert model.update is not None
-    assert model.iterator is not None
-
-
-@pytest.mark.gpu
 @pytest.fixture(scope="module")
 def dkn_files(deeprec_resource_path):
     data_path = os.path.join(deeprec_resource_path, "dkn")
     yaml_file = os.path.join(data_path, "dkn.yaml")
-    news_feature_file = os.path.join(data_path, r"doc_feature.txt")
-    user_history_file = os.path.join(data_path, r"user_history.txt")
-    wordEmb_file = os.path.join(data_path, r"word_embeddings_100.npy")
-    entityEmb_file = os.path.join(data_path, r"TransE_entity2vec_100.npy")
-    contextEmb_file = os.path.join(data_path, r"TransE_context2vec_100.npy")
+    news_feature_file = os.path.join(data_path, "doc_feature.txt")
+    user_history_file = os.path.join(data_path, "user_history.txt")
+    wordEmb_file = os.path.join(data_path, "word_embeddings_100.npy")
+    entityEmb_file = os.path.join(data_path, "TransE_entity2vec_100.npy")
+    contextEmb_file = os.path.join(data_path, "TransE_context2vec_100.npy")
 
     download_deeprec_resources(
         "https://recodatasets.z20.web.core.windows.net/deeprec/",
         data_path,
         "mind-demo.zip",
     )
     return (
@@ -80,14 +62,91 @@
         wordEmb_file,
         entityEmb_file,
         contextEmb_file,
     )
 
 
 @pytest.mark.gpu
+@pytest.fixture(scope="module")
+def sequential_files(deeprec_resource_path):
+    data_path = os.path.join(deeprec_resource_path, "slirec")
+    train_file = os.path.join(data_path, "train_data")
+    valid_file = os.path.join(data_path, "valid_data")
+    test_file = os.path.join(data_path, "test_data")
+    user_vocab = os.path.join(data_path, "user_vocab.pkl")
+    item_vocab = os.path.join(data_path, "item_vocab.pkl")
+    cate_vocab = os.path.join(data_path, "category_vocab.pkl")
+
+    reviews_name = "reviews_Movies_and_TV_5.json"
+    meta_name = "meta_Movies_and_TV.json"
+    reviews_file = os.path.join(data_path, reviews_name)
+    meta_file = os.path.join(data_path, meta_name)
+
+    # number of negative instances with a positive instance for validation
+    valid_num_ngs = 4
+    # number of negative instances with a positive instance for testing
+    test_num_ngs = 9
+    # sample a small item set for training and testing here for example
+    sample_rate = 0.01
+
+    input_files = [
+        reviews_file,
+        meta_file,
+        train_file,
+        valid_file,
+        test_file,
+        user_vocab,
+        item_vocab,
+        cate_vocab,
+    ]
+    download_and_extract(reviews_name, reviews_file)
+    download_and_extract(meta_name, meta_file)
+    data_preprocessing(
+        *input_files,
+        sample_rate=sample_rate,
+        valid_num_ngs=valid_num_ngs,
+        test_num_ngs=test_num_ngs
+    )
+
+    return (
+        data_path,
+        user_vocab,
+        item_vocab,
+        cate_vocab,
+    )
+
+
+@pytest.mark.gpu
+def test_xdeepfm_component_definition(deeprec_resource_path):
+    data_path = os.path.join(deeprec_resource_path, "xdeepfm")
+    yaml_file = os.path.join(data_path, "xDeepFM.yaml")
+
+    if not os.path.exists(yaml_file):
+        download_deeprec_resources(
+            "https://recodatasets.z20.web.core.windows.net/deeprec/",
+            data_path,
+            "xdeepfmresources.zip",
+        )
+
+    hparams = prepare_hparams(yaml_file)
+    model = XDeepFMModel(hparams, FFMTextIterator)
+
+    assert model.logit is not None
+    assert model.update is not None
+    assert model.iterator is not None
+    assert model.hparams is not None
+    assert model.hparams.model_type == "xDeepFM"
+    assert model.hparams.epochs == 50
+    assert model.hparams.batch_size == 128
+    assert model.hparams.learning_rate == 0.0005
+    assert model.hparams.loss == "log_loss"
+    assert model.hparams.optimizer == "adam"
+
+
+@pytest.mark.gpu
 def test_dkn_component_definition(dkn_files):
     # Load params from fixture
     (
         _,
         yaml_file,
         news_feature_file,
         user_history_file,
@@ -103,20 +162,26 @@
         user_history_file=user_history_file,
         wordEmb_file=wordEmb_file,
         entityEmb_file=entityEmb_file,
         contextEmb_file=contextEmb_file,
         epochs=1,
         learning_rate=0.0001,
     )
-    assert hparams is not None
 
     model = DKN(hparams, DKNTextIterator)
     assert model.logit is not None
     assert model.update is not None
     assert model.iterator is not None
+    assert model.hparams is not None
+    assert model.hparams.model_type == "dkn"
+    assert model.hparams.epochs == 1
+    assert model.hparams.batch_size == 100
+    assert model.hparams.learning_rate == 0.0001
+    assert model.hparams.loss == "log_loss"
+    assert model.hparams.optimizer == "adam"
 
 
 @pytest.mark.gpu
 def test_dkn_item2item_component_definition(dkn_files):
     # Load params from fixture
     (
         data_path,
@@ -139,73 +204,29 @@
         is_clip_norm=True,
         max_grad_norm=0.5,
         his_size=20,
         MODEL_DIR=os.path.join(data_path, "save_models"),
         use_entity=True,
         use_context=True,
     )
-    assert hparams is not None
 
     hparams.neg_num = 9
     model_item2item = DKNItem2Item(hparams, DKNItem2itemTextIterator)
     assert model_item2item.pred_logits is not None
     assert model_item2item.update is not None
     assert model_item2item.iterator is not None
-
-
-@pytest.mark.gpu
-@pytest.fixture(scope="module")
-def sequential_files(deeprec_resource_path):
-    data_path = os.path.join(deeprec_resource_path, "slirec")
-    train_file = os.path.join(data_path, r"train_data")
-    valid_file = os.path.join(data_path, r"valid_data")
-    test_file = os.path.join(data_path, r"test_data")
-    user_vocab = os.path.join(data_path, r"user_vocab.pkl")
-    item_vocab = os.path.join(data_path, r"item_vocab.pkl")
-    cate_vocab = os.path.join(data_path, r"category_vocab.pkl")
-
-    reviews_name = "reviews_Movies_and_TV_5.json"
-    meta_name = "meta_Movies_and_TV.json"
-    reviews_file = os.path.join(data_path, reviews_name)
-    meta_file = os.path.join(data_path, meta_name)
-    valid_num_ngs = (
-        4  # number of negative instances with a positive instance for validation
-    )
-    test_num_ngs = (
-        9  # number of negative instances with a positive instance for testing
-    )
-    sample_rate = (
-        0.01  # sample a small item set for training and testing here for example
-    )
-
-    input_files = [
-        reviews_file,
-        meta_file,
-        train_file,
-        valid_file,
-        test_file,
-        user_vocab,
-        item_vocab,
-        cate_vocab,
-    ]
-    download_and_extract(reviews_name, reviews_file)
-    download_and_extract(meta_name, meta_file)
-    data_preprocessing(
-        *input_files,
-        sample_rate=sample_rate,
-        valid_num_ngs=valid_num_ngs,
-        test_num_ngs=test_num_ngs
-    )
-
-    return (
-        data_path,
-        user_vocab,
-        item_vocab,
-        cate_vocab,
-    )
+    assert model_item2item.hparams is not None
+    assert model_item2item.hparams.model_type == "dkn"
+    assert model_item2item.hparams.epochs == 1
+    assert model_item2item.hparams.batch_size == 100
+    assert model_item2item.hparams.learning_rate == 0.0005
+    assert model_item2item.hparams.loss == "log_loss"
+    assert model_item2item.hparams.optimizer == "adam"
+    assert model_item2item.hparams.max_grad_norm == 0.5
+    assert model_item2item.hparams.his_size == 20
 
 
 @pytest.mark.gpu
 def test_slirec_component_definition(sequential_files, deeprec_config_path):
     yaml_file = os.path.join(deeprec_config_path, "sli_rec.yaml")
     data_path, user_vocab, item_vocab, cate_vocab = sequential_files
 
@@ -219,20 +240,30 @@
         MODEL_DIR=os.path.join(data_path, "model"),
         SUMMARIES_DIR=os.path.join(data_path, "summary"),
         user_vocab=user_vocab,
         item_vocab=item_vocab,
         cate_vocab=cate_vocab,
         need_sample=True,
     )
-    assert hparams is not None
 
     model = SLI_RECModel(hparams, SequentialIterator)
     assert model.logit is not None
     assert model.update is not None
     assert model.iterator is not None
+    assert model.hparams is not None
+    assert model.hparams.model_type == "sli_rec"
+    assert model.hparams.epochs == 1
+    assert model.hparams.batch_size == 400
+    assert model.hparams.learning_rate == 0.001
+    assert model.hparams.loss == "softmax"
+    assert model.hparams.optimizer == "adam"
+    assert model.hparams.train_num_ngs == 4
+    assert model.hparams.embed_l2 == 0.0
+    assert model.hparams.layer_l2 == 0.0
+    assert model.hparams.need_sample is True
 
 
 @pytest.mark.gpu
 def test_nextitnet_component_definition(sequential_files, deeprec_config_path):
     yaml_file_nextitnet = os.path.join(deeprec_config_path, "nextitnet.yaml")
     data_path, user_vocab, item_vocab, cate_vocab = sequential_files
 
@@ -247,20 +278,30 @@
         MODEL_DIR=os.path.join(data_path, "model"),
         SUMMARIES_DIR=os.path.join(data_path, "summary"),
         user_vocab=user_vocab,
         item_vocab=item_vocab,
         cate_vocab=cate_vocab,
         need_sample=True,
     )
-    assert hparams_nextitnet is not None
 
     model_nextitnet = NextItNetModel(hparams_nextitnet, NextItNetIterator)
     assert model_nextitnet.logit is not None
     assert model_nextitnet.update is not None
     assert model_nextitnet.iterator is not None
+    assert model_nextitnet.hparams is not None
+    assert model_nextitnet.hparams.model_type == "NextItNet"
+    assert model_nextitnet.hparams.epochs == 1
+    assert model_nextitnet.hparams.batch_size == 400
+    assert model_nextitnet.hparams.learning_rate == 0.001
+    assert model_nextitnet.hparams.loss == "softmax"
+    assert model_nextitnet.hparams.optimizer == "adam"
+    assert model_nextitnet.hparams.train_num_ngs == 4
+    assert model_nextitnet.hparams.embed_l2 == 0.0
+    assert model_nextitnet.hparams.layer_l2 == 0.0
+    assert model_nextitnet.hparams.need_sample is True
 
 
 @pytest.mark.gpu
 def test_sum_component_definition(sequential_files, deeprec_config_path):
     yaml_file_sum = os.path.join(deeprec_config_path, "sum.yaml")
     data_path, user_vocab, item_vocab, cate_vocab = sequential_files
 
@@ -275,37 +316,48 @@
         MODEL_DIR=os.path.join(data_path, "model"),
         SUMMARIES_DIR=os.path.join(data_path, "summary"),
         user_vocab=user_vocab,
         item_vocab=item_vocab,
         cate_vocab=cate_vocab,
         need_sample=True,
     )
-    assert hparams_sum is not None
 
     model_sum = SUMModel(hparams_sum, SequentialIterator)
     assert model_sum.logit is not None
     assert model_sum.update is not None
     assert model_sum.iterator is not None
+    assert model_sum.hparams is not None
+    assert model_sum.hparams.model_type == "SUM"
+    assert model_sum.hparams.epochs == 1
+    assert model_sum.hparams.batch_size == 400
+    assert model_sum.hparams.learning_rate == 0.001
+    assert model_sum.hparams.loss == "softmax"
+    assert model_sum.hparams.optimizer == "adam"
+    assert model_sum.hparams.train_num_ngs == 4
+    assert model_sum.hparams.embed_l2 == 0.0
+    assert model_sum.hparams.layer_l2 == 0.0
+    assert model_sum.hparams.need_sample is True
 
 
 @pytest.mark.gpu
 def test_lightgcn_component_definition(deeprec_config_path):
     yaml_file = os.path.join(deeprec_config_path, "lightgcn.yaml")
 
     df = movielens.load_pandas_df(size="100k")
     train, test = python_stratified_split(df, ratio=0.75)
 
     data = ImplicitCF(train=train, test=test)
 
-    embed_size = 64
-    hparams = prepare_hparams(yaml_file, embed_size=embed_size)
+    hparams = prepare_hparams(yaml_file, embed_size=64)
     model = LightGCN(hparams, data)
 
     assert model.norm_adj is not None
-    assert model.ua_embeddings.shape == [data.n_users, embed_size]
-    assert model.ia_embeddings.shape == [data.n_items, embed_size]
+    assert model.ua_embeddings.shape == [943, 64]
+    assert model.ia_embeddings.shape == [1682, 64]
     assert model.u_g_embeddings is not None
     assert model.pos_i_g_embeddings is not None
     assert model.neg_i_g_embeddings is not None
     assert model.batch_ratings is not None
     assert model.loss is not None
     assert model.opt is not None
+    assert model.batch_size == 1024
+    assert model.epochs == 1000
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_deeprec_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_deeprec_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import os
 import pytest
 
 try:
     from recommenders.models.deeprec.deeprec_utils import (
         prepare_hparams,
         download_deeprec_resources,
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_geoimc.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_geoimc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-try:
-    import collections
-    import pytest
-    import numpy as np
-    from scipy.sparse import csr_matrix
 
+import collections
+import pytest
+import numpy as np
+from scipy.sparse import csr_matrix
+
+try:
     from recommenders.models.geoimc.geoimc_data import DataPtr
     from recommenders.models.geoimc.geoimc_predict import Inferer
     from recommenders.models.geoimc.geoimc_algorithm import IMCProblem
     from recommenders.models.geoimc.geoimc_utils import (
         length_normalize,
         mean_center,
         reduce_dims,
     )
     from pymanopt.manifolds import Stiefel, SymmetricPositiveDefinite
 except:
-    pass    # skip if pymanopt not installed
+    pass  # skip if pymanopt not installed
+
 
 _IMC_TEST_DATA = [
     (
         csr_matrix(np.array([[1, 5, 3], [7, 2, 1]])),
         [
             np.array([[0, 6, 0, 5], [7, 1, 2, 1]]),
             np.array([[8, 8, 0, 8, 4], [7, 4, 3, 0, 7], [0, 6, 8, 7, 2]]),
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_lightfm_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_lightfm_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import pytest
 import itertools
 import numpy as np
 import pandas as pd
-from lightfm import LightFM, cross_validation
 from lightfm.data import Dataset
+from lightfm import LightFM, cross_validation
+
 from recommenders.models.lightfm.lightfm_utils import (
     track_model_metrics,
     similar_users,
     similar_items,
 )
 
+
 SEEDNO = 42
 TEST_PERCENTAGE = 0.25
 TEST_USER_ID = 2
 TEST_ITEM_ID = 1
 
 
 # note user and item ID need to be sequential for similar users and similar items to work
@@ -129,14 +132,15 @@
     train_interactions, test_interactions, item_features, user_features = interactions
     assert train_interactions.shape == (10, 10)
     assert test_interactions.shape == (10, 10)
     assert item_features.shape == (10, 19)
     assert user_features.shape == (10, 17)
 
 
+@pytest.mark.skip(reason="Flaky test")
 def test_fitting(fitting):
     output, _ = fitting
     assert output.shape == (4, 4)
     target = np.array(
         [
             [0, 0.10000000894069672, "train", "Precision"],
             [0, 0.10000000149011612, "test", "Precision"],
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_ncf_dataset.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_ncf_dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,64 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import os
 import pytest
 import pandas as pd
+
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
     DEFAULT_ITEM_COL,
     DEFAULT_RATING_COL,
     DEFAULT_TIMESTAMP_COL,
 )
 from recommenders.models.ncf.dataset import (
     DataFile,
     NegativeSampler,
     Dataset,
     EmptyFileException,
     MissingFieldsException,
     FileNotSortedException,
-    MissingUserException
+    MissingUserException,
 )
 
 
 @pytest.mark.gpu
 def test_datafile_init(dataset_ncf_files_sorted):
     train_path, _, _ = dataset_ncf_files_sorted
     train = pd.read_csv(train_path)
     users = train[DEFAULT_USER_COL].unique()
     items = train[DEFAULT_ITEM_COL].unique()
     datafile = DataFile(
-        train_path, DEFAULT_USER_COL, DEFAULT_ITEM_COL, DEFAULT_RATING_COL, col_test_batch=None, binary=True
+        train_path,
+        DEFAULT_USER_COL,
+        DEFAULT_ITEM_COL,
+        DEFAULT_RATING_COL,
+        col_test_batch=None,
+        binary=True,
     )
     assert set(datafile.users) == set(users)
     assert set(datafile.items) == set(items)
     assert set(datafile.user2id.keys()) == set(users)
     assert set(datafile.item2id.keys()) == set(items)
     assert len(set(datafile.user2id.values())) == len(users)
     assert len(set(datafile.item2id.values())) == len(items)
     assert datafile.data_len == train.shape[0]
 
     datafile_records = []
     with datafile as f:
         for line in f:
-            datafile_records.append({
-                DEFAULT_USER_COL: line[DEFAULT_USER_COL],
-                DEFAULT_ITEM_COL: line[DEFAULT_ITEM_COL],
-                DEFAULT_RATING_COL: line[DEFAULT_RATING_COL]
-            })
+            datafile_records.append(
+                {
+                    DEFAULT_USER_COL: line[DEFAULT_USER_COL],
+                    DEFAULT_ITEM_COL: line[DEFAULT_ITEM_COL],
+                    DEFAULT_RATING_COL: line[DEFAULT_RATING_COL],
+                }
+            )
     datafile_df = pd.DataFrame.from_records(datafile_records)
     assert datafile_df.shape[0] == train.shape[0]
 
     # test the data loaded from the file is the same as original data
     datafile_df = datafile_df.sort_values(by=[DEFAULT_USER_COL, DEFAULT_ITEM_COL])
     train = train.sort_values(by=[DEFAULT_USER_COL, DEFAULT_ITEM_COL])
     train[DEFAULT_RATING_COL] = train[DEFAULT_RATING_COL].apply(lambda x: float(x > 0))
@@ -64,59 +73,87 @@
         assert user_data[DEFAULT_USER_COL].iloc[0] == user
         with pytest.raises(MissingUserException):
             user_data == f.load_data(missing_user)
 
 
 @pytest.mark.gpu
 def test_datafile_init_unsorted(dataset_ncf_files_unsorted):
-    train_path, _, _= dataset_ncf_files_unsorted
+    train_path, _, _ = dataset_ncf_files_unsorted
     with pytest.raises(FileNotSortedException):
         datafile = DataFile(
-            train_path, DEFAULT_USER_COL, DEFAULT_ITEM_COL, DEFAULT_RATING_COL, col_test_batch=None, binary=True
+            train_path,
+            DEFAULT_USER_COL,
+            DEFAULT_ITEM_COL,
+            DEFAULT_RATING_COL,
+            col_test_batch=None,
+            binary=True,
         )
 
 
 @pytest.mark.gpu
 def test_datafile_init_empty(dataset_ncf_files_empty):
-    train_path, _, _= dataset_ncf_files_empty
+    train_path, _, _ = dataset_ncf_files_empty
     with pytest.raises(EmptyFileException):
         datafile = DataFile(
-            train_path, DEFAULT_USER_COL, DEFAULT_ITEM_COL, DEFAULT_RATING_COL, col_test_batch=None, binary=True
+            train_path,
+            DEFAULT_USER_COL,
+            DEFAULT_ITEM_COL,
+            DEFAULT_RATING_COL,
+            col_test_batch=None,
+            binary=True,
         )
 
 
 @pytest.mark.gpu
 def test_datafile_missing_column(dataset_ncf_files_missing_column):
-    train_path, _, _= dataset_ncf_files_missing_column
+    train_path, _, _ = dataset_ncf_files_missing_column
     with pytest.raises(MissingFieldsException):
         datafile = DataFile(
-            train_path, DEFAULT_USER_COL, DEFAULT_ITEM_COL, DEFAULT_RATING_COL, col_test_batch=None, binary=True
+            train_path,
+            DEFAULT_USER_COL,
+            DEFAULT_ITEM_COL,
+            DEFAULT_RATING_COL,
+            col_test_batch=None,
+            binary=True,
         )
 
 
 @pytest.mark.gpu
 def test_negative_sampler(caplog):
     user = 1
     n_samples = 3
     user_positive_item_pool = {1, 2}
     item_pool = {1, 2, 3, 4, 5}
     sample_with_replacement = False
-    sampler = NegativeSampler(user, n_samples, user_positive_item_pool, item_pool, sample_with_replacement)
+    sampler = NegativeSampler(
+        user, n_samples, user_positive_item_pool, item_pool, sample_with_replacement
+    )
     assert sampler.n_samples == 3
     samples = sampler.sample()
     assert set(samples) == item_pool.difference(user_positive_item_pool)
 
     # test sampler adjusts n_samples down if population is too small and that it raises a warning
     n_samples = 4
-    sampler = NegativeSampler(user, n_samples, user_positive_item_pool, item_pool, sample_with_replacement)
+    sampler = NegativeSampler(
+        user, n_samples, user_positive_item_pool, item_pool, sample_with_replacement
+    )
     assert sampler.n_samples == 3
-    assert "The population of negative items to sample from is too small for user 1" in caplog.text
+    assert (
+        "The population of negative items to sample from is too small for user 1"
+        in caplog.text
+    )
 
     # test sampling with replacement returns requested number of samples despite small population
-    sampler = NegativeSampler(user, n_samples, user_positive_item_pool, item_pool, sample_with_replacement=True)
+    sampler = NegativeSampler(
+        user,
+        n_samples,
+        user_positive_item_pool,
+        item_pool,
+        sample_with_replacement=True,
+    )
     assert sampler.n_samples == 4
     assert len(sampler.sample()) == n_samples
 
 
 @pytest.mark.gpu
 def test_train_loader(tmp_path, dataset_ncf_files_sorted):
     train_path, _, _ = dataset_ncf_files_sorted
@@ -135,25 +172,27 @@
 
     # test number of batches and data size is as expected after loading all training data
     full_data_len = train.shape[0] * 2
     batch_size = full_data_len // 10
     expected_batches = full_data_len // batch_size
     train_save_path = os.path.join(tmp_path, "train_full.csv")
     batch_records = []
-    for batch in dataset.train_loader(batch_size, shuffle_size=batch_size, yield_id=True, write_to=train_save_path):
+    for batch in dataset.train_loader(
+        batch_size, shuffle_size=batch_size, yield_id=True, write_to=train_save_path
+    ):
         assert type(batch[0][0]) == int
         assert type(batch[1][0]) == int
         assert type(batch[2][0]) == float
         batch_data = {
             DEFAULT_USER_COL: [dataset.id2user[user] for user in batch[0]],
             DEFAULT_ITEM_COL: [dataset.id2item[item] for item in batch[1]],
-            DEFAULT_RATING_COL: batch[2]
+            DEFAULT_RATING_COL: batch[2],
         }
         batch_records.append(pd.DataFrame(batch_data))
-    
+
     assert len(batch_records) == expected_batches
     train_loader_df = pd.concat(batch_records).reset_index(drop=True)
     assert train_loader_df.shape[0] == expected_batches * batch_size
     assert set(train_loader_df[DEFAULT_USER_COL]) == set(users)
     assert set(train_loader_df[DEFAULT_ITEM_COL]) == set(items)
 
     # test that data is successfully saved
@@ -166,29 +205,36 @@
 def test_test_loader(dataset_ncf_files_sorted):
     train_path, _, leave_one_out_test_path = dataset_ncf_files_sorted
     leave_one_out_test = pd.read_csv(leave_one_out_test_path)
     test_users = leave_one_out_test[DEFAULT_USER_COL].unique()
 
     n_neg = 1
     n_neg_test = 1
-    dataset = Dataset(train_path, test_file=leave_one_out_test_path, n_neg=n_neg, n_neg_test=n_neg_test)
+    dataset = Dataset(
+        train_path,
+        test_file=leave_one_out_test_path,
+        n_neg=n_neg,
+        n_neg_test=n_neg_test,
+    )
     assert set(dataset.test_full_datafile.users) == set(test_users)
 
     # test number of batches and data size is as expected after loading all test data
     expected_test_batches = leave_one_out_test.shape[0]
-    assert max(dataset.test_full_datafile.batch_indices_range) + 1 == expected_test_batches
+    assert (
+        max(dataset.test_full_datafile.batch_indices_range) + 1 == expected_test_batches
+    )
     batch_records = []
     for batch in dataset.test_loader(yield_id=True):
         assert type(batch[0][0]) == int
         assert type(batch[1][0]) == int
         assert type(batch[2][0]) == float
         batch_data = {
             DEFAULT_USER_COL: [dataset.id2user[user] for user in batch[0]],
             DEFAULT_ITEM_COL: [dataset.id2item[item] for item in batch[1]],
-            DEFAULT_RATING_COL: batch[2]
+            DEFAULT_RATING_COL: batch[2],
         }
         batch_records.append(pd.DataFrame(batch_data))
-    
+
     assert len(batch_records) == expected_test_batches
     test_loader_df = pd.concat(batch_records).reset_index(drop=True)
     assert test_loader_df.shape[0] == expected_test_batches * n_neg_test * 2
     assert set(test_loader_df[DEFAULT_USER_COL]) == set(test_users)
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_ncf_singlenode.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_ncf_singlenode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import os
 import shutil
+import pytest
 import numpy as np
 import pandas as pd
-import pytest
 
 try:
     from recommenders.models.ncf.ncf_singlenode import NCF
     from recommenders.models.ncf.dataset import Dataset
     from recommenders.utils.constants import (
         DEFAULT_USER_COL,
         DEFAULT_ITEM_COL,
@@ -144,28 +145,32 @@
     # TODO: test loading fc-concat
 
 
 @pytest.mark.gpu
 @pytest.mark.parametrize("model_type", ["NeuMF", "GMF", "MLP"])
 def test_fit(dataset_ncf_files_sorted, model_type):
     train_path, test_path, _ = dataset_ncf_files_sorted
-    data = Dataset(train_file=train_path, test_file=test_path, n_neg=N_NEG, n_neg_test=N_NEG_TEST)
+    data = Dataset(
+        train_file=train_path, test_file=test_path, n_neg=N_NEG, n_neg_test=N_NEG_TEST
+    )
     model = NCF(
         n_users=data.n_users, n_items=data.n_items, model_type=model_type, n_epochs=1
     )
     model.fit(data)
 
 
 @pytest.mark.gpu
 @pytest.mark.parametrize("model_type", ["NeuMF", "GMF", "MLP"])
 def test_predict(dataset_ncf_files_sorted, model_type):
     # test data format
     train_path, test_path, _ = dataset_ncf_files_sorted
     test = pd.read_csv(test_path)
-    data = Dataset(train_file=train_path, test_file=test_path, n_neg=N_NEG, n_neg_test=N_NEG_TEST)
+    data = Dataset(
+        train_file=train_path, test_file=test_path, n_neg=N_NEG, n_neg_test=N_NEG_TEST
+    )
     model = NCF(
         n_users=data.n_users, n_items=data.n_items, model_type=model_type, n_epochs=1
     )
     model.fit(data)
 
     test_users, test_items = list(test[DEFAULT_USER_COL]), list(test[DEFAULT_ITEM_COL])
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_newsrec_model.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_newsrec_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import pytest
 
 try:
     from recommenders.models.deeprec.deeprec_utils import download_deeprec_resources
@@ -18,19 +18,19 @@
 
 
 @pytest.mark.gpu
 def test_nrms_component_definition(mind_resource_path):
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"nrms.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "nrms.yaml")
 
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
@@ -50,19 +50,19 @@
 @pytest.mark.gpu
 def test_naml_component_definition(mind_resource_path):
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding_all.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict_all.pkl")
     vertDict_file = os.path.join(mind_resource_path, "utils", "vert_dict.pkl")
     subvertDict_file = os.path.join(mind_resource_path, "utils", "subvert_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"naml.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "naml.yaml")
 
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
@@ -82,19 +82,19 @@
 
 
 @pytest.mark.gpu
 def test_npa_component_definition(mind_resource_path):
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"npa.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "npa.yaml")
 
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "utils"),
             "MINDdemo_utils.zip",
         )
 
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
@@ -112,19 +112,19 @@
 
 
 @pytest.mark.gpu
 def test_lstur_component_definition(mind_resource_path):
     wordEmb_file = os.path.join(mind_resource_path, "utils", "embedding.npy")
     userDict_file = os.path.join(mind_resource_path, "utils", "uid2index.pkl")
     wordDict_file = os.path.join(mind_resource_path, "utils", "word_dict.pkl")
-    yaml_file = os.path.join(mind_resource_path, "utils", r"lstur.yaml")
+    yaml_file = os.path.join(mind_resource_path, "utils", "lstur.yaml")
 
     if not os.path.exists(yaml_file):
         download_deeprec_resources(
-            r"https://recodatasets.z20.web.core.windows.net/newsrec/",
+            "https://recodatasets.z20.web.core.windows.net/newsrec/",
             os.path.join(mind_resource_path, "mind", "utils"),
             "MINDdemo_utils.zip",
         )
     hparams = prepare_hparams(
         yaml_file,
         wordEmb_file=wordEmb_file,
         wordDict_file=wordDict_file,
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_newsrec_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_newsrec_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 import os
 import pytest
 
 try:
     from recommenders.models.deeprec.deeprec_utils import download_deeprec_resources
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_rbm.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_rbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import numpy as np
+
 import pytest
+import numpy as np
 
 try:
     from recommenders.models.rbm.rbm import RBM
 except ImportError:
     pass  # skip this import if we are in cpu environment
 
 
@@ -141,14 +142,15 @@
 
     # check that the multinomial distribution is normalized over the r classes for all users/items
     assert np.sum(pvh, axis=2) == pytest.approx(np.ones(Xtr.shape))
 
     # check that the sampled values of the visible units is in [0,r]
     assert check_sampled_values(v_sampled, r).all()
 
+
 @pytest.mark.gpu
 def test_save_load(init_rbm, affinity_matrix):
 
     # obtain the train/test set matrices
     Xtr, _ = affinity_matrix
 
     # initialize the model
@@ -201,8 +203,7 @@
     assert saved_model.learning_rate == original_model.learning_rate
     # standard deviation used to initialize the weight matrix from a normal distribution
     assert saved_model.stdv == original_model.stdv
     # sampling protocol used to increase the number of steps in Gibbs sampling
     assert saved_model.sampling_protocol == original_model.sampling_protocol
     # number of epochs after which the rmse is displayed
     assert saved_model.display_epoch == original_model.display_epoch
-
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_sar_singlenode.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_sar_singlenode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import itertools
+
 import json
 import pytest
+import itertools
 import numpy as np
 import pandas as pd
 from pandas.testing import assert_frame_equal
 
 from recommenders.utils.constants import DEFAULT_PREDICTION_COL
 from recommenders.models.sar import SAR
 
@@ -108,23 +109,21 @@
     )
 
     # Remove duplicates
     demo_usage_data = demo_usage_data.sort_values(
         header["col_timestamp"], ascending=False
     )
     demo_usage_data = demo_usage_data.drop_duplicates(
-        [header["col_user"], header["col_item"]],
-        keep="first"
+        [header["col_user"], header["col_item"]], keep="first"
     )
 
     model.fit(demo_usage_data)
 
     true_item_similarity = pd.read_csv(
-        sar_settings["FILE_DIR"] + "sim_" + file + str(threshold) + ".csv",
-        index_col=0
+        sar_settings["FILE_DIR"] + "sim_" + file + str(threshold) + ".csv", index_col=0
     )
     item2index = pd.Series(model.item2index)
     index = item2index[true_item_similarity.index]
     columns = item2index[true_item_similarity.columns]
 
     if similarity_type == "cooccurrence":
         test_item_similarity = pd.DataFrame(model.item_similarity.todense())
@@ -155,21 +154,24 @@
         time_decay_coefficient=30,
         time_now=time_now,
         **header
     )
     model.fit(demo_usage_data)
 
     true_user_affinity = pd.read_csv(
-        sar_settings["FILE_DIR"] + "user_aff.csv",
-        index_col=0
+        sar_settings["FILE_DIR"] + "user_aff.csv", index_col=0
+    )
+    sar_user_affinity = (
+        model.user_affinity[
+            model.user2index[sar_settings["TEST_USER_ID"]],
+            pd.Series(model.item2index)[true_user_affinity.columns],
+        ]
+        .toarray()
+        .flatten()
     )
-    sar_user_affinity = model.user_affinity[
-        model.user2index[sar_settings["TEST_USER_ID"]],
-        pd.Series(model.item2index)[true_user_affinity.columns]
-    ].toarray().flatten()
     assert np.allclose(
         true_user_affinity.astype("float64"),
         sar_user_affinity.astype("float64"),
         atol=sar_settings["ATOL"],
     )
 
     # Set time_now to 60 days later
@@ -180,25 +182,28 @@
         time_decay_coefficient=30,
         time_now=demo_usage_data[header["col_timestamp"]].max() + two_months,
         **header
     )
     model.fit(demo_usage_data)
 
     true_user_affinity = pd.read_csv(
-        sar_settings["FILE_DIR"] + "user_aff_2_months_later.csv",
-        index_col=0
+        sar_settings["FILE_DIR"] + "user_aff_2_months_later.csv", index_col=0
+    )
+    sar_user_affinity = (
+        model.user_affinity[
+            model.user2index[sar_settings["TEST_USER_ID"]],
+            pd.Series(model.item2index)[true_user_affinity.columns],
+        ]
+        .toarray()
+        .flatten()
     )
-    sar_user_affinity = model.user_affinity[
-        model.user2index[sar_settings["TEST_USER_ID"]],
-        pd.Series(model.item2index)[true_user_affinity.columns]
-    ].toarray().flatten()
     assert np.allclose(
         true_user_affinity.astype("float64"),
         sar_user_affinity.astype("float64"),
-        atol=sar_settings["ATOL"]
+        atol=sar_settings["ATOL"],
     )
 
 
 @pytest.mark.parametrize(
     "threshold,similarity_type,file",
     [
         (3, "cooccurrence", "count"),
@@ -222,15 +227,15 @@
         threshold=threshold,
         **header
     )
     model.fit(demo_usage_data)
 
     true_userpred = pd.read_csv(
         sar_settings["FILE_DIR"] + "userpred_" + file + str(threshold) + ".csv",
-        index_col=0
+        index_col=0,
     )
     test_results = model.recommend_k_items(
         demo_usage_data[
             demo_usage_data[header["col_user"]] == sar_settings["TEST_USER_ID"]
         ],
         top_k=10,
         sort_top_k=True,
@@ -242,15 +247,14 @@
     else:
         pd.testing.assert_frame_equal(
             test_results, true_userpred, atol=sar_settings["ATOL"]
         )
 
 
 def test_get_item_based_topk(header, pandas_dummy):
-
     sar = SAR(**header)
     sar.fit(pandas_dummy)
 
     # test with just items provided
     expected = pd.DataFrame(
         dict(UserId=[0, 0, 0], MovieId=[8, 7, 6], prediction=[2.0, 2.0, 2.0])
     )
@@ -291,15 +295,14 @@
         }
     )
     actual = sar.get_item_based_topk(items, top_k=3).set_index(["UserId", "MovieId"])
     assert_frame_equal(expected, actual, check_like=True)
 
 
 def test_get_popularity_based_topk(header):
-
     train_df = pd.DataFrame(
         {
             header["col_user"]: [1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 3, 4],
             header["col_item"]: [1, 4, 2, 1, 5, 4, 1, 4, 6, 3, 2, 4],
             header["col_rating"]: [1, 2, 3, 1, 2, 3, 1, 2, 3, 3, 3, 1],
         }
     )
@@ -374,15 +377,15 @@
     assert actual.shape == (2, 7)
     assert isinstance(actual, np.ndarray)
     assert np.isclose(expected, np.asarray(actual)).all()
 
 
 def test_match_similarity_type_from_json_file(header):
     # store parameters in json
-    params_str = json.dumps({'similarity_type': 'lift'})
+    params_str = json.dumps({"similarity_type": "lift"})
     # load parameters in json
     params = json.loads(params_str)
 
     params.update(header)
 
     model = SAR(**params)
 
@@ -401,29 +404,29 @@
 
 def test_dataset_with_duplicates(header):
     model = SAR(**header)
     train = pd.DataFrame(
         {
             header["col_user"]: [1, 1, 2, 2, 2],
             header["col_item"]: [1, 2, 1, 2, 2],
-            header["col_rating"]: [3.0, 4.0, 3.0, 4.0, 4.0]
+            header["col_rating"]: [3.0, 4.0, 3.0, 4.0, 4.0],
         }
     )
     with pytest.raises(ValueError):
         model.fit(train)
 
 
 def test_get_topk_most_similar_users(header):
     model = SAR(**header)
     # 1, 2, and 4 used the same items, but 1 and 2 have the same ratings also
     train = pd.DataFrame(
         {
             header["col_user"]: [1, 1, 2, 2, 3, 3, 3, 3, 4, 4],
             header["col_item"]: [1, 2, 1, 2, 3, 4, 5, 6, 1, 2],
-            header["col_rating"]: [3.0, 4.0, 3.0, 4.0, 3.0, 2.0, 1.0, 5.0, 5.0, 1.0]
+            header["col_rating"]: [3.0, 4.0, 3.0, 4.0, 3.0, 2.0, 1.0, 5.0, 5.0, 1.0],
         }
     )
     model.fit(train)
 
     similar_users = model.get_topk_most_similar_users(user=1, top_k=1)
     expected = pd.DataFrame(dict(UserId=[2], prediction=[25.0]))
     assert_frame_equal(expected, similar_users)
@@ -439,27 +442,27 @@
 
 def test_item_frequencies(header):
     model = SAR(**header)
     train = pd.DataFrame(
         {
             header["col_user"]: [1, 1, 2, 2, 3, 3, 3, 3, 4, 4],
             header["col_item"]: [1, 2, 1, 3, 3, 4, 5, 6, 1, 2],
-            header["col_rating"]: [3.0, 4.0, 5.0, 4.0, 3.0, 2.0, 1.0, 5.0, 1.0, 1.0]
+            header["col_rating"]: [3.0, 4.0, 5.0, 4.0, 3.0, 2.0, 1.0, 5.0, 1.0, 1.0],
         }
     )
     model.fit(train)
     assert model.item_frequencies[0] == 3
 
 
 def test_user_frequencies(header):
     model = SAR(**header)
     train = pd.DataFrame(
         {
             header["col_user"]: [1, 1, 2, 2, 3, 3, 3, 3, 4, 4],
             header["col_item"]: [1, 2, 1, 3, 3, 4, 5, 6, 1, 2],
-            header["col_rating"]: [3.0, 4.0, 5.0, 4.0, 3.0, 2.0, 1.0, 5.0, 1.0, 1.0]
+            header["col_rating"]: [3.0, 4.0, 5.0, 4.0, 3.0, 2.0, 1.0, 5.0, 1.0, 1.0],
         }
     )
     model.fit(train)
     # run this method once so that user frequencies are calculated
     model.get_popularity_based_topk(items=False)
     assert model.user_frequencies[0] == 2
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_sasrec_model.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_sasrec_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import pytest
+
 import os
+import pytest
 from collections import defaultdict
 
 try:
     from recommenders.models.sasrec.model import SASREC
     from recommenders.models.sasrec.ssept import SSEPT
     from recommenders.models.sasrec.sampler import WarpSampler
     from recommenders.models.sasrec.util import SASRecDataSet
 
     from recommenders.datasets.amazon_reviews import (
         download_and_extract,
         _reviews_preprocessing,
     )
-
 except ImportError:
     pass  # skip if in cpu environment
 
 
 @pytest.fixture()
 def model_parameters():
     params = {
@@ -176,15 +176,14 @@
     assert len(seq) == batch_size
     assert len(pos) == batch_size
     assert len(neg) == batch_size
 
 
 @pytest.mark.gpu
 def test_sasrec(model_parameters):
-
     params = model_parameters
 
     model = SASREC(
         item_num=params["itemnum"],
         seq_max_len=params["maxlen"],
         num_blocks=params["num_blocks"],
         embedding_dim=params["hidden_units"],
@@ -198,15 +197,14 @@
 
     assert model.encoder is not None
     assert model.item_embedding_layer is not None
 
 
 @pytest.mark.gpu
 def test_ssept(model_parameters):
-
     params = model_parameters
 
     model = SSEPT(
         item_num=params["itemnum"],
         user_num=params["usernum"],
         seq_max_len=params["maxlen"],
         num_blocks=params["num_blocks"],
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_surprise_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_surprise_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
-try:
-    import pandas as pd
-    import pytest
-    import surprise
-
-    from recommenders.utils.constants import (
-        DEFAULT_USER_COL,
-        DEFAULT_ITEM_COL,
-        DEFAULT_RATING_COL,
-    )
-    from recommenders.models.surprise.surprise_utils import (
-        predict,
-        compute_ranking_predictions,
-    )
-except:
-    pass    # skip if surprise not installed
+import pytest
+import pandas as pd
+import surprise
+
+from recommenders.utils.constants import (
+    DEFAULT_USER_COL,
+    DEFAULT_ITEM_COL,
+    DEFAULT_RATING_COL,
+)
+from recommenders.models.surprise.surprise_utils import (
+    predict,
+    compute_ranking_predictions,
+)
+
 
 TOL = 0.001
 
 
 @pytest.fixture
 def rating_true():
     return pd.DataFrame(
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_tfidf_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_tfidf_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import pytest
-from recommenders.models.tfidf.tfidf_utils import TfidfRecommender
-import pandas as pd
 import scipy
+import pandas as pd
+
+from recommenders.models.tfidf.tfidf_utils import TfidfRecommender
+
 
 CLEAN_COL = "cleaned_text"
 K = 2
 
 
 @pytest.fixture(scope="module")
 def df():
@@ -47,14 +50,28 @@
 
 
 @pytest.fixture(scope="module")
 def model():
     return TfidfRecommender(id_col="cord_uid", tokenization_method="scibert")
 
 
+@pytest.fixture(scope="module")
+def df_clean(model, df):
+    return model.clean_dataframe(df, ["abstract", "full_text"], new_col_name=CLEAN_COL)
+
+
+@pytest.fixture(scope="module")
+def model_fit(model, df_clean):
+    model_fit = TfidfRecommender(id_col="cord_uid", tokenization_method="scibert")
+    tf, vectors_tokenized = model_fit.tokenize_text(df_clean)
+    model_fit.fit(tf, vectors_tokenized)
+
+    return model_fit
+
+
 def test_init(model):
     assert model.id_col == "cord_uid"
     assert model.tokenization_method == "scibert"
 
 
 def test_clean_dataframe(model, df):
     df_clean = model.clean_dataframe(
@@ -65,39 +82,25 @@
     for idx, _ in df_clean.iterrows():
         s1 = str(df_clean[CLEAN_COL][idx])
         isalphanumeric.append(s1.replace(" ", "").isalnum())
 
     assert False not in isalphanumeric
 
 
-@pytest.fixture(scope="module")
-def df_clean(model, df):
-    return model.clean_dataframe(df, ["abstract", "full_text"], new_col_name=CLEAN_COL)
-
-
 def test_tokenize_text(model, df_clean):
     _, vectors_tokenized = model.tokenize_text(df_clean)
     assert True not in list(df_clean[CLEAN_COL] == vectors_tokenized)
 
 
 def test_fit(model, df_clean):
     tf, vectors_tokenized = model.tokenize_text(df_clean)
     model.fit(tf, vectors_tokenized)
     assert type(model.tfidf_matrix) == scipy.sparse.csr.csr_matrix
 
 
-@pytest.fixture(scope="module")
-def model_fit(model, df_clean):
-    model_fit = TfidfRecommender(id_col="cord_uid", tokenization_method="scibert")
-    tf, vectors_tokenized = model_fit.tokenize_text(df_clean)
-    model_fit.fit(tf, vectors_tokenized)
-
-    return model_fit
-
-
 def test_get_tokens(model_fit):
     tokens = model_fit.get_tokens()
     assert type(tokens) == dict
     assert type(list(tokens.keys())[0]) == str
 
 
 def test_get_stop_words(model_fit):
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_vowpal_wabbit.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_vowpal_wabbit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import os
 import pytest
 from unittest import mock
 import pandas as pd
 
 from recommenders.models.vowpal_wabbit.vw import VW
 
@@ -19,25 +20,25 @@
 @pytest.fixture(scope="function")
 def model():
     model = VW(col_user="user", col_item="item", col_prediction="prediction", q="ui")
     yield model
     del model
 
 
-@pytest.mark.vw
+@pytest.mark.experimental
 def test_vw_init_del():
     model = VW()
     tempdir = model.tempdir.name
     assert os.path.exists(tempdir)
 
     del model
     assert not os.path.exists(tempdir)
 
 
-@pytest.mark.vw
+@pytest.mark.experimental
 def test_to_vw_cmd():
     expected = [
         "vw",
         "-l",
         "0.1",
         "--l1",
         "0.2",
@@ -56,15 +57,15 @@
         quiet=False,
         rank=3,
         t=True,
     )
     assert VW.to_vw_cmd(params=params) == expected
 
 
-@pytest.mark.vw
+@pytest.mark.experimental
 def test_parse_train_cmd(model):
     expected = [
         "vw",
         "--loss_function",
         "logistic",
         "--oaa",
         "5",
@@ -73,15 +74,15 @@
         "-d",
         model.train_file,
     ]
     params = dict(loss_function="logistic", oaa=5, f="test", d="data", quiet=False)
     assert model.parse_train_params(params=params) == expected
 
 
-@pytest.mark.vw
+@pytest.mark.experimental
 def test_parse_test_cmd(model):
     expected = [
         "vw",
         "--loss_function",
         "logistic",
         "-d",
         model.test_file,
@@ -94,24 +95,24 @@
     ]
     params = dict(
         loss_function="logistic", i="test", oaa=5, d="data", test_only=True, quiet=True
     )
     assert model.parse_test_params(params=params) == expected
 
 
-@pytest.mark.vw
+@pytest.mark.experimental
 def test_to_vw_file(model, df):
     expected = ["1 0|user 1 |item 8", "5 1|user 3 |item 7", "3 2|user 2 |item 7"]
     model.to_vw_file(df, train=True)
     with open(model.train_file, "r") as f:
         assert f.read().splitlines() == expected
     del model
 
 
-@pytest.mark.vw
+@pytest.mark.experimental
 def test_fit_and_predict(model, df):
     # generate fake predictions
     with open(model.prediction_file, "w") as f:
         f.writelines(["1 0\n", "3 1\n", "5 2\n"])
 
     # patch subprocess call to vw
     with mock.patch(
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/models/test_wide_deep_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/models/test_wide_deep_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import os
 import pytest
 import pandas as pd
+
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
     DEFAULT_ITEM_COL,
     DEFAULT_RATING_COL,
 )
 
 try:
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/tuning/test_ncf_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/tuning/test_ncf_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-import pytest
+# Copyright (c) Recommenders contributors.
+# Licensed under the MIT License.
+
 
+import pytest
 from unittest.mock import Mock
 
 from recommenders.tuning.nni.ncf_utils import compute_test_results
 from recommenders.datasets.movielens import MockMovielensSchema
 
+
 DATA_SIZE = 1  # setting to 1 so all IDs are unique
 
 
 @pytest.fixture(scope="module")
 def mock_model():
     def mock_predict(*args, is_list=False):
-        """ Mock model predict method"""
+        """Mock model predict method"""
         if is_list:
             return [0] * DATA_SIZE
         else:
             return 0
 
     mock_model = Mock()
     mock_model.predict.side_effect = mock_predict
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/tuning/test_nni_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/tuning/test_nni_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import json
+
 import os
 import sys
-from tempfile import TemporaryDirectory
-from unittest.mock import patch
+import json
 import pytest
+from unittest.mock import patch
+from tempfile import TemporaryDirectory
 
 from recommenders.tuning.nni.nni_utils import (
     get_experiment_status,
     check_experiment_status,
     check_stopped,
     check_metrics_written,
     get_trials,
@@ -48,72 +49,78 @@
     return MockResponseTrials(content)
 
 
 def mock_exception():
     raise Exception()
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_get_experiment_status():
     content = "some_status"
     error = ""
     with patch(
         "requests.get", side_effect=lambda url: mocked_status_get(url, content, error)
     ):
         nni_status = get_experiment_status(NNI_STATUS_URL)
         assert nni_status["status"] == "some_status"
         assert nni_status["errors"] == [""]
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_experiment_status_done():
     content = "DONE"
     error = ""
     with patch(
         "requests.get", side_effect=lambda url: mocked_status_get(url, content, error)
     ):
         check_experiment_status(wait=0.1, max_retries=1)
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_experiment_status_tuner_no_more_trial():
     content = "TUNER_NO_MORE_TRIAL"
     error = ""
     with patch(
         "requests.get", side_effect=lambda url: mocked_status_get(url, content, error)
     ):
         check_experiment_status(wait=0.1, max_retries=1)
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_experiment_status_running():
     content = "RUNNING"
     error = ""
     with pytest.raises(TimeoutError) as excinfo:
         with patch(
             "requests.get",
             side_effect=lambda url: mocked_status_get(url, content, error),
         ):
             check_experiment_status(wait=0.1, max_retries=1)
     assert "check_experiment_status() timed out" == str(excinfo.value)
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_experiment_status_no_more_trial():
     content = "NO_MORE_TRIAL"
     error = ""
     with pytest.raises(TimeoutError) as excinfo:
         with patch(
             "requests.get",
             side_effect=lambda url: mocked_status_get(url, content, error),
         ):
             check_experiment_status(wait=0.1, max_retries=1)
     assert "check_experiment_status() timed out" == str(excinfo.value)
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_experiment_status_failed():
     content = "some_failed_status"
     error = "NNI_ERROR"
     with pytest.raises(RuntimeError) as excinfo:
         with patch(
             "requests.get",
@@ -122,51 +129,56 @@
             check_experiment_status(wait=0.1, max_retries=1)
     assert (
         "NNI experiment failed to complete with status some_failed_status - NNI_ERROR"
         == str(excinfo.value)
     )
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_stopped_timeout():
     content = "some_status"
     error = ""
     with pytest.raises(TimeoutError) as excinfo:
         with patch(
             "requests.get",
             side_effect=lambda url: mocked_status_get(url, content, error),
         ):
             check_stopped(wait=0.1, max_retries=1)
     assert "check_stopped() timed out" == str(excinfo.value)
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_stopped():
     with patch("requests.get", side_effect=mock_exception):
         check_stopped(wait=0.1, max_retries=1)
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_metrics_written():
     content = [{"finalMetricData": None}, {"finalMetricData": None}]
     with patch("requests.get", side_effect=lambda url: mocked_trials_get(url, content)):
         check_metrics_written(wait=0.1, max_retries=1)
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_check_metrics_written_timeout():
     content = [{"logPath": "/p"}, {"logPath": "/q"}]
     with pytest.raises(TimeoutError) as excinfo:
         with patch(
             "requests.get", side_effect=lambda url: mocked_trials_get(url, content)
         ):
             check_metrics_written(wait=0.1, max_retries=1)
     assert "check_metrics_written() timed out" == str(excinfo.value)
 
 
+@pytest.mark.experimental
 @pytest.mark.skipif(sys.platform == "win32", reason="nni not installable on windows")
 def test_get_trials():
     with TemporaryDirectory() as tmp_dir1, TemporaryDirectory() as tmp_dir2:
 
         mock_trials = [
             {
                 "finalMetricData": [
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/tuning/test_sweep.py` & `recommenders-1.2.0/tests/unit/recommenders/tuning/test_sweep.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
 import pytest
 
 from recommenders.tuning.parameter_sweep import generate_param_grid
 
 
 @pytest.fixture(scope="module")
 def parameter_dictionary():
-    params = {"param1": [1, 2, 3], "param2": [4, 5, 6], "param3": 1}
-
-    return params
+    return {"param1": [1, 2, 3], "param2": [4, 5, 6], "param3": 1}
 
 
 def test_param_sweep(parameter_dictionary):
     params_grid = generate_param_grid(parameter_dictionary)
 
     assert params_grid == [
         {"param1": 1, "param2": 4, "param3": 1},
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/utils/test_gpu_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/utils/test_gpu_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import sys
 import pytest
 
 try:
     import tensorflow as tf
     import torch
+    from recommenders.utils.gpu_utils import (
+        get_cuda_version,
+        get_cudnn_version,
+        get_gpu_info,
+        get_number_gpus,
+    )
 except ImportError:
     pass  # skip this import if we are in cpu environment
 
 
-from recommenders.utils.gpu_utils import (
-    get_cuda_version,
-    get_cudnn_version,
-    get_gpu_info,
-    get_number_gpus,
-)
-
-
 @pytest.mark.gpu
 def test_get_gpu_info():
     assert len(get_gpu_info()) >= 1
 
 
 @pytest.mark.gpu
 def test_get_number_gpus():
@@ -34,28 +33,30 @@
 def test_clear_memory_all_gpus():
     pass
 
 
 @pytest.mark.gpu
 @pytest.mark.skipif(sys.platform == "win32", reason="Not implemented on Windows")
 def test_get_cuda_version():
-    assert get_cuda_version() > "9.0.0"
+    assert int(get_cuda_version().split(".")[0]) > 9
 
 
 @pytest.mark.gpu
 def test_get_cudnn_version():
-    assert get_cudnn_version() > "7.0.0"
+    assert int(get_cudnn_version()[0]) > 7
 
 
 @pytest.mark.gpu
 def test_cudnn_enabled():
     assert torch.backends.cudnn.enabled == True
 
 
 @pytest.mark.gpu
+@pytest.mark.skip(reason="This function in TF is flaky")
 def test_tensorflow_gpu():
-    assert tf.test.is_gpu_available()
+    assert len(tf.config.list_physical_devices("GPU")) > 0
 
 
 @pytest.mark.gpu
+@pytest.mark.skip(reason="This function in PyTorch is flaky")
 def test_pytorch_gpu():
     assert torch.cuda.is_available()
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/utils/test_k8s_utils.py` & `recommenders-1.2.0/tests/integration/recommenders/utils/test_k8s_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 from recommenders.utils.k8s_utils import (
     qps_to_replicas,
     replicas_to_qps,
     nodes_to_replicas,
 )
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/utils/test_plot.py` & `recommenders-1.2.0/tests/unit/recommenders/utils/test_plot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
+
 import matplotlib
 import matplotlib.pyplot as plt
 from recommenders.utils.plot import line_graph
 
 matplotlib.use("Agg")
 
 
@@ -15,14 +16,16 @@
         values=[[1, 2, 3], [3, 2, 1]],
         labels=["Train", "Valid"],
         x_guides=[0, 1],
         x_name="Epoch",
         y_name="Accuracy",
         legend_loc="best",
     )
+    assert plt.gca().get_xlabel() == "Epoch"
+    assert plt.gca().get_ylabel() == "Accuracy"
     plt.close()
 
     # Single graph as a subplot
     line_graph(values=[1, 2, 3], labels="Train", subplot=(1, 1, 1))
     plt.close()
 
     # Single graph with x values
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/utils/test_python_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/utils/test_python_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
-import numpy as np
 import pytest
+import numpy as np
 
 from recommenders.utils.python_utils import (
     exponential_decay,
     jaccard,
     lift,
     get_top_k_scored_items,
     binarize,
     rescale,
 )
 
+
 TOL = 0.0001
 
 
 @pytest.fixture
 def target_matrices(scope="module"):
     J1 = np.array([[1.0, 0.0, 0.5], [0.0, 1.0, 0.33333], [0.5, 0.33333, 1.0]])
     J2 = np.array(
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/utils/test_tf_utils.py` & `recommenders-1.2.0/tests/unit/recommenders/utils/test_tf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
-import itertools
+
 import os
+import pytest
 import numpy as np
 import pandas as pd
-import pytest
+import itertools
+
 from recommenders.utils.constants import (
     DEFAULT_USER_COL,
     DEFAULT_ITEM_COL,
     DEFAULT_RATING_COL,
     SEED,
 )
 from recommenders.evaluation.python_evaluation import rmse
```

### Comparing `recommenders-1.1.1/tests/unit/recommenders/utils/test_timer.py` & `recommenders-1.2.0/tests/unit/recommenders/utils/test_timer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-# Copyright (c) Microsoft Corporation. All rights reserved.
+# Copyright (c) Recommenders contributors.
 # Licensed under the MIT License.
 
 
-import pytest
 import time
+import pytest
+
 from recommenders.utils.timer import Timer
 
 
 TOL = 0.03
 
 
 @pytest.fixture(scope="function")
```


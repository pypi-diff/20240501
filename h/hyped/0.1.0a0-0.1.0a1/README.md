# Comparing `tmp/hyped-0.1.0a0.tar.gz` & `tmp/hyped-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyped-0.1.0a0.tar", last modified: Mon Apr 15 20:16:14 2024, max compression
+gzip compressed data, was "hyped-0.1.0a1.tar", last modified: Wed May  1 14:22:00 2024, max compression
```

## Comparing `hyped-0.1.0a0.tar` & `hyped-0.1.0a1.tar`

### file list

```diff
@@ -1,177 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.176882 hyped-0.1.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.144881 hyped-0.1.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.148881 hyped-0.1.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-15 20:15:12.000000 hyped-0.1.0a0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-15 20:15:12.000000 hyped-0.1.0a0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-15 20:15:12.000000 hyped-0.1.0a0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-15 20:15:12.000000 hyped-0.1.0a0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-15 20:15:12.000000 hyped-0.1.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-15 20:15:12.000000 hyped-0.1.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 20:15:12.000000 hyped-0.1.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-15 20:16:14.176882 hyped-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-15 20:15:12.000000 hyped-0.1.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.152881 hyped-0.1.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 20:15:12.000000 hyped-0.1.0a0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 20:15:12.000000 hyped-0.1.0a0/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-15 20:15:12.000000 hyped-0.1.0a0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.152881 hyped-0.1.0a0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.152881 hyped-0.1.0a0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/docs/source/api/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-15 20:15:12.000000 hyped-0.1.0a0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-15 20:15:12.000000 hyped-0.1.0a0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-15 20:15:12.000000 hyped-0.1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-15 20:15:12.000000 hyped-0.1.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:16:14.176882 hyped-0.1.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.144881 hyped-0.1.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.152881 hyped-0.1.0a0/src/hyped/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-15 20:16:13.000000 hyped-0.1.0a0/src/hyped/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.152881 hyped-0.1.0a0/src/hyped/base/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/base/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/base/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/base/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.156881 hyped-0.1.0a0/src/hyped/common/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/common/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/common/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/common/feature_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    24044 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/common/feature_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/common/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.156881 hyped-0.1.0a0/src/hyped/data/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.156881 hyped-0.1.0a0/src/hyped/data/io/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.156881 hyped-0.1.0a0/src/hyped/data/io/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/io/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/io/datasets/cas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/io/datasets/typed_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.156881 hyped-0.1.0a0/src/hyped/data/io/writers/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/io/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/io/writers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/io/writers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/io/writers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.156881 hyped-0.1.0a0/src/hyped/data/processors/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13326 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.156881 hyped-0.1.0a0/src/hyped/data/processors/features/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/features/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/features/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/features/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.160881 hyped-0.1.0a0/src/hyped/data/processors/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/sequence/apply_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/sequence/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/sequence/extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/sequence/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/sequence/join_str_seq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.160881 hyped-0.1.0a0/src/hyped/data/processors/spans/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/spans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/spans/apply_idx_spans.py
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/spans/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/spans/from_bio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/spans/from_word_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/spans/idx_spans.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/spans/loc_to_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/spans/overlaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.160881 hyped-0.1.0a0/src/hyped/data/processors/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.160881 hyped-0.1.0a0/src/hyped/data/processors/statistics/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/sequence/disc_seq_val_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/sequence/seq_len_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/sequence/seq_val_hist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.164881 hyped-0.1.0a0/src/hyped/data/processors/statistics/value/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/value/disc_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/value/hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/statistics/value/mean_and_std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.164881 hyped-0.1.0a0/src/hyped/data/processors/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/taggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/taggers/bio.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/taggers/relex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.164881 hyped-0.1.0a0/src/hyped/data/processors/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-04-15 20:15:12.000000 hyped-0.1.0a0/src/hyped/data/processors/tokenizers/hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.176882 hyped-0.1.0a0/src/hyped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-15 20:16:14.000000 hyped-0.1.0a0/src/hyped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 20:16:14.000000 hyped-0.1.0a0/src/hyped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:16:14.000000 hyped-0.1.0a0/src/hyped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 20:16:14.000000 hyped-0.1.0a0/src/hyped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 20:16:14.000000 hyped-0.1.0a0/src/hyped.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.164881 hyped-0.1.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.164881 hyped-0.1.0a0/tests/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/base/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/base/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/base/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.164881 hyped-0.1.0a0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/common/test_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/common/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/common/test_feature_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    18093 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/common/test_feature_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/common/test_lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.168882 hyped-0.1.0a0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.168882 hyped-0.1.0a0/tests/data/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.168882 hyped-0.1.0a0/tests/data/io/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/io/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/io/datasets/test_cas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/io/datasets/test_typed_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.168882 hyped-0.1.0a0/tests/data/io/writers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/io/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/io/writers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/io/writers/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/io/writers/test_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.168882 hyped-0.1.0a0/tests/data/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.168882 hyped-0.1.0a0/tests/data/processors/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/features/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/features/test_flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/features/test_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.172881 hyped-0.1.0a0/tests/data/processors/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/sequence/test_apply_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/sequence/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/sequence/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/sequence/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/sequence/test_join_str_seq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.172881 hyped-0.1.0a0/tests/data/processors/spans/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/spans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/spans/test_apply_idx_spans.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/spans/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/spans/test_from_bio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/spans/test_from_word_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8264 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/spans/test_idx_spans.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/spans/test_loc_to_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/spans/test_overlaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.172881 hyped-0.1.0a0/tests/data/processors/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/statistics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/statistics/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/statistics/test_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.172881 hyped-0.1.0a0/tests/data/processors/statistics/value/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/statistics/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/statistics/value/test_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/statistics/value/test_mean_and_std.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.172881 hyped-0.1.0a0/tests/data/processors/taggers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/taggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/taggers/test_bio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/taggers/test_relex.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:16:14.176882 hyped-0.1.0a0/tests/data/processors/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/processors/tokenizers/test_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-15 20:15:12.000000 hyped-0.1.0a0/tests/data/test_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.692628 hyped-0.1.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.656629 hyped-0.1.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-01 14:21:33.000000 hyped-0.1.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-01 14:21:33.000000 hyped-0.1.0a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 14:21:33.000000 hyped-0.1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-01 14:22:00.692628 hyped-0.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-01 14:21:33.000000 hyped-0.1.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/add_ons.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/api/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/costum_data_processors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/feature_access.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-01 14:21:33.000000 hyped-0.1.0a1/docs/source/statistic_processors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-01 14:21:33.000000 hyped-0.1.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-01 14:21:33.000000 hyped-0.1.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:22:00.692628 hyped-0.1.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.656629 hyped-0.1.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.664629 hyped-0.1.0a1/src/hyped/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.668629 hyped-0.1.0a1/src/hyped/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/base/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.668629 hyped-0.1.0a1/src/hyped/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/feature_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/feature_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/common/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.668629 hyped-0.1.0a1/src/hyped/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.668629 hyped-0.1.0a1/src/hyped/data/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/io/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/datasets/cas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/datasets/typed_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/io/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/writers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/writers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/io/writers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21294 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/processors/features/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/features/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/features/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/features/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.672629 hyped-0.1.0a1/src/hyped/data/processors/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/apply_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/sequence/join_str_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/spans/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/apply_idx_spans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/from_bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/from_word_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/idx_spans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/loc_to_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/spans/overlaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/disc_seq_val_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/seq_len_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/seq_val_hist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/disc_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/statistics/value/mean_and_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/taggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/taggers/bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/taggers/relex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.676629 hyped-0.1.0a1/src/hyped/data/processors/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-05-01 14:21:33.000000 hyped-0.1.0a1/src/hyped/data/processors/tokenizers/hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/src/hyped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 14:22:00.000000 hyped-0.1.0a1/src/hyped.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/base/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/base/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/base/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_feature_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17355 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_feature_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/common/test_lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/data/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.680629 hyped-0.1.0a1/tests/hyped/data/io/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/datasets/test_cas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/datasets/test_typed_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.684629 hyped-0.1.0a1/tests/hyped/data/io/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/writers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/writers/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/io/writers/test_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.684629 hyped-0.1.0a1/tests/hyped/data/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.684629 hyped-0.1.0a1/tests/hyped/data/processors/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/features/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/features/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/features/test_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.684629 hyped-0.1.0a1/tests/hyped/data/processors/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_apply_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_join_str_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/spans/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_apply_idx_spans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_from_bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_from_word_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_idx_spans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_loc_to_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/spans/test_overlaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_disc_seq_val_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_seq_len_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/sequence/test_seq_val_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/test_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_disc_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_mean_and_std.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/taggers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/taggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/taggers/test_bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/taggers/test_relex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:22:00.688629 hyped-0.1.0a1/tests/hyped/data/processors/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/processors/tokenizers/test_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12943 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-01 14:21:33.000000 hyped-0.1.0a1/tests/hyped/data/test_pipe.py
```

### Comparing `hyped-0.1.0a0/.github/workflows/docs.yml` & `hyped-0.1.0a1/.github/workflows/docs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install -r requirements.txt
           python -m pip install -e .[docs]
 
       - name: Build Sphinx Documentation
         run: |
-          sphinx-apidoc -o docs/source/api src/
+          sphinx-apidoc -e -o docs/source/api src/hyped --tocfile hyped
           make -C docs html
 
       - name: Deploy to Github Pages
         uses: peaceiris/actions-gh-pages@v3
         with:
           publish_branch: gh-pages
           github_token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `hyped-0.1.0a0/.github/workflows/linting.yml` & `hyped-0.1.0a1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/.github/workflows/publish.yml` & `hyped-0.1.0a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/.gitignore` & `hyped-0.1.0a1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -143,8 +143,8 @@
 data
 docs/source/api/*
 !docs/source/api/.gitkeep
 src/hyped/__version__.py
 
 # explicitly unignore data directory
 !src/hyped/data
-!tests/data
+!tests/hyped/data
```

### Comparing `hyped-0.1.0a0/LICENSE` & `hyped-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/docs/Makefile` & `hyped-0.1.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/docs/make.bat` & `hyped-0.1.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/docs/source/conf.py` & `hyped-0.1.0a1/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # Include package path
 import os
 import sys
 
-sys.path.insert(0, os.path.abspath("../../src"))
+sys.path.insert(0, os.path.abspath("../../src/hyped"))
 
 
 # import all modules
 import hyped
+import hyped.__version__
 import hyped.data.graph
 import hyped.data.pipe
 import hyped.data.processors.base
 import hyped.data.processors.features.filter
 import hyped.data.processors.features.flatten
 import hyped.data.processors.features.format
 import hyped.data.processors.sequence.apply_mask
@@ -44,26 +45,25 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "hyped"
 copyright = "2024, open-hyped"
 author = "open-hyped"
-version = hyped.__version__
-release = hyped.__version__
+version = hyped.__version__.__version__
+release = hyped.__version__.__version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc"]
 
 templates_path = ["_templates"]
 exclude_patterns = []
 
-
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_rtd_theme"
 html_static_path = ["_static"]
 
 html_theme_options = {
```

### Comparing `hyped-0.1.0a0/src/hyped/base/auto.py` & `hyped-0.1.0a1/src/hyped/base/auto.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/base/config.py` & `hyped-0.1.0a1/src/hyped/base/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,19 +151,19 @@
 class BaseConfigurable(Generic[U], RegisterTypes, ABC):
     """Base class for configurable types.
 
     Configurable types define a `from_config` classmethod.
     Sub-types must implement this function.
     """
 
-    CONFIG_TYPE: None | type[BaseConfig] = None
+    CONFIG_TYPE: None | type[U] = None
 
     @classmethod
     @property
-    def generic_config_type(cls) -> type[BaseConfig]:
+    def generic_config_type(cls) -> type[U]:
         """Config Type specified by generic type var `U`.
 
         Get the generic configuration type of the configurable specified
         by the type variable `U`.
         """
         # get config class
         t = solve_typevar(cls, U)
@@ -173,15 +173,15 @@
                 "Configurable config type `%s` doesn't inherit from `%s`"
                 % (str(t), str(BaseConfig))
             )
         return t or BaseConfig
 
     @classmethod
     @property
-    def config_type(cls) -> type[BaseConfig]:
+    def config_type(cls) -> type[U]:
         """Get the (final) configuration type of the configurable.
 
         The final configuration type is specified by the `CONFIG_TYPE`
         class attribute. Falls back to the generic config type if the
         class attribute is not specified. Also checks that the concrete
         configuration type is valid, i.e. inherits the generic configuration
         type.
```

### Comparing `hyped-0.1.0a0/src/hyped/base/generic.py` & `hyped-0.1.0a1/src/hyped/base/generic.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/base/registry.py` & `hyped-0.1.0a1/src/hyped/base/registry.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/common/arrow.py` & `hyped-0.1.0a1/src/hyped/common/arrow.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/common/consumer.py` & `hyped-0.1.0a1/src/hyped/common/consumer.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/common/feature_checks.py` & `hyped-0.1.0a1/src/hyped/common/feature_checks.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/common/feature_key.py` & `hyped-0.1.0a1/src/hyped/common/feature_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Feature Key Module."""
 from __future__ import annotations
 
 from enum import Enum
 from itertools import chain
 from typing import Any, Iterable
 
+from datasets import Dataset
 from datasets.features.features import Features, FeatureType, Sequence
-from datasets.iterable_dataset import _batch_to_examples
-from pydantic import GetCoreSchemaHandler
+from datasets.iterable_dataset import _batch_to_examples, _examples_to_batch
+from pydantic import BaseModel, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 
 from .feature_checks import (
     check_feature_equals,
     get_sequence_feature,
     get_sequence_length,
     raise_feature_equals,
@@ -484,88 +485,243 @@
         """
         return map(
             FeatureKey.from_tuple,
             _iter_keys_in_features(features, max_depth, max_seq_len_to_unpack),
         )
 
 
-_FeatureKeyCollectionValue = (
-    FeatureKey
-    | list["_FeatureKeyCollectionValue"]
-    | dict[str, "_FeatureKeyCollectionValue"]
-)
+class Const(BaseModel):
+    """Constant Value Wrapper.
+
+    This wrapper is used to specify constant values in feature descriptions.
+
+    Consider the following example:
+
+    .. code-block: python
+
+        feature = Feature(
+            {
+                "const": Const("This is a constant value"),
+                "lookup": "feature"
+            }
+        )
+
+    Arguments:
+        value (str | int | float):
+            value
+    """
+
+    value: str | int | float
+
+    def __init__(self, value: str | int | float) -> None:
+        """Constructor."""
+        super(Const, self).__init__(value=value)
+
+    def __str__(self) -> str:
+        """String representation of the constant feature value."""
+        return "Const(%s)" % repr(self.value)
 
+    def __repr__(self) -> str:
+        """String representation of the constant feature value."""
+        return str(self)
+
+    @property
+    def ftype(self) -> Value:
+        """HuggingFace Datasets Feature Type of the constant value."""
+        return Dataset.from_dict({"feature": [self.value]}).features["feature"]
+
+
+class FeatureCollection(BaseModel):
+    """Feature Collection.
+
+    A Feature Collection is a more complex variant of a `FeatureKey`. Where a
+    feature key is only used to index a single feature, a `FeatureCollection`
+    can be used to build a complex collection of features on the fly.
+
+    Consider the following example:
 
-def _convert_to_feature_keys(
-    col: _FeatureKeyCollectionValue | str | tuple[str | int | slice],
-) -> _FeatureKeyCollectionValue:
-    """Internal helper function."""
-    if isinstance(col, dict):
-        return {k: _convert_to_feature_keys(v) for k, v in col.items()}
-    if isinstance(col, list):
-        return list(map(_convert_to_feature_keys, col))
-    if isinstance(col, tuple):
-        return FeatureKey.from_tuple(col)
-    if not isinstance(col, FeatureKey):
-        return FeatureKey(col)
-
-    raise ValueError()
-
-
-def _collect_from_example(
-    col: _FeatureKeyCollectionValue, example: dict[str, Any]
-) -> Any:
-    """Internal helper function."""
-    if isinstance(col, FeatureKey):
-        return col.index_example(example)
-    if isinstance(col, dict):
-        return {
-            key: _collect_from_example(val, example)
-            for key, val in col.items()
-        }
-    if isinstance(col, list):
-        return [_collect_from_example(x, example) for x in col]
-
-    raise ValueError()
-
-
-class FeatureKeyCollection(dict[str, _FeatureKeyCollectionValue]):
-    """Feature Key Collection.
-
-    Represents a (nested) collection of feature keys in the form of
-    a dictionary on the top-level but can include lists in nested
-    structures.
+    .. code-block: python
+
+        seq_feature = FeatureCollection(
+            [
+                FeatureKey("a"),
+                FeatureKey("b"),
+                FeatureKey("c")
+            ]
+        )
+
+        seq = seq_feature.index_example(...)
+
+    Arguments:
+        scheme (FeatureKey | list[FeatureCollection] | dict[str, FeatureCollection] | Const):
+            recipe of the feature, i.e. a specification on how to construct the feature
     """
 
-    def __init__(
-        self, collection: dict[str, _FeatureKeyCollectionValue] = {}
-    ) -> None:
-        """Instantiate new feature key collection.
+    scheme: FeatureKey | list[FeatureCollection] | dict[
+        str, FeatureCollection
+    ] | Const
+
+    def __init__(self, scheme: Any = None, **kwargs) -> None:
+        """Constructor."""
+        if len(kwargs) > 0:
+            scheme = kwargs
+
+        scheme = type(self)._parse_scheme(scheme)
+        super(FeatureCollection, self).__init__(scheme=scheme)
+
+    @classmethod
+    def _parse_scheme(cls, scheme: Any) -> FeatureCollection:
+        """Helper function used to parse a schema."""
+        if isinstance(scheme, dict):
+            return {key: FeatureCollection(val) for key, val in scheme.items()}
+        if isinstance(scheme, list):
+            return list(map(FeatureCollection, scheme))
+        if isinstance(scheme, (str, tuple)):
+            return FeatureKey(scheme)
+
+        return scheme
+
+    @property
+    def feature_keys(self) -> Iterable[FeatureKey]:
+        """Iterator over all feature keys listed in the collection."""
+        if isinstance(self.scheme, dict):
+            yield from chain.from_iterable(
+                val.feature_keys for val in self.scheme.values()
+            )
+        if isinstance(self.scheme, list):
+            yield from chain.from_iterable(
+                item.feature_keys for item in self.scheme
+            )
+        if isinstance(self.scheme, FeatureKey):
+            yield self.scheme
+
+    def index_features(self, features: Features) -> FeatureType:
+        """Index features.
+
+        Builds the features according to the specified scheme.
 
         Arguments:
-            collection (dict[str, _FeatureKeyCollectionValue]):
-                feature key collection
+            features (Features):
+                source feature mapping from which to build the features
+
+        Returns:
+            build_features (Features):
+                build dataset features matching the scheme
         """
-        dict.__init__(self, _convert_to_feature_keys(collection))
+        if isinstance(self.scheme, dict):
+            return Features(
+                {
+                    key: val.index_features(features)
+                    for key, val in self.scheme.items()
+                }
+            )
+        if isinstance(self.scheme, list):
+            assert len(self.scheme) > 0
+            # collect all features in specified in the list
+            collected_features = (
+                item.index_features(features) for item in self.scheme
+            )
+            f = next(collected_features)
+            # make sure the feature types match
+            for ff in collected_features:
+                if not check_feature_equals(f, ff):
+                    raise TypeError(
+                        "Expected all items of a sequence to be of the "
+                        "same feature type, got %s != %s" % (str(f), str(ff))
+                    )
+            return Sequence(f, length=len(self.scheme))
+        if isinstance(self.scheme, FeatureKey):
+            return self.scheme.index_features(features)
+        if isinstance(self.scheme, Const):
+            return self.scheme.ftype
+
+        raise TypeError
+
+    def index_example(self, example: dict[str, Any]) -> Any:
+        """Index example.
 
-    def __setitem__(self, idx: str, val: _FeatureKeyCollectionValue) -> None:
-        """Set value in collection.
+        Builds the feature sample from a given example according to the specified scheme.
 
         Arguments:
-            idx (str): string index key
-            val (_FeatureKeyCollectionValue): new value
+            example (dict[str, Any]):
+                example from which to build the feature
+
+        Returns:
+            build_sample (Any):
+                the sample build from the given example according to the scheme
         """
-        super(FeatureKeyCollection, self).__setitem__(
-            idx, _convert_to_feature_keys(val)
-        )
+        if isinstance(self.scheme, dict):
+            return {
+                key: val.index_example(example)
+                for key, val in self.scheme.items()
+            }
+        if isinstance(self.scheme, list):
+            return [item.index_example(example) for item in self.scheme]
+        if isinstance(self.scheme, FeatureKey):
+            return self.scheme.index_example(example)
+        if isinstance(self.scheme, Const):
+            return self.scheme.value
 
-    @classmethod
-    def from_feature_keys(
-        self, feature_keys: Iterable[FeatureKey]
-    ) -> FeatureKeyCollection:
+        raise TypeError
+
+    def index_batch(self, batch: dist[str, list[Any]]) -> list[Any]:
+        """Index Batch.
+
+        Builds the batch of feature samples from a given batch according
+        to the specified scheme.
+
+        Arguments:
+            batch (dict[str, list[Any]]):
+                batch from which to build the samples
+
+        Returns:
+            build_batch (list[Any]):
+                the batch build from the given batch according to the scheme
+        """
+        return list(map(self.index_example, _batch_to_examples(batch)))
+
+    def unpack(self) -> Any:
+        """Unpack the feature to a simple python object.
+
+        Returns:
+            scheme (Any):
+                the unpacked feature scheme in the form of simple nested
+                python objects, i.e. dictionaries and lists
+        """
+        if isinstance(self.scheme, dict):
+            return {key: val.unpack() for key, val in self.scheme.items()}
+        if isinstance(self.scheme, list):
+            return [item.unpack() for item in self.scheme]
+
+        return self.scheme
+
+    def __str__(self) -> str:
+        """String representation of the feature."""
+        return str(self.scheme)
+
+    def __repr__(self) -> str:
+        """String representation of the feature."""
+        return str(self)
+
+
+class FeatureDict(FeatureCollection):
+    """Feature Dictionary.
+
+    A special Feature Collection type guaranteed to be a dictionary on top-level
+    but can still contain nested sub-features.
+
+    Arguments:
+        scheme (dict[str, Feature]):
+            recipe of the feature, i.e. a specification on how to construct the feature
+    """
+
+    scheme: dict[str, FeatureCollection]
+
+    @staticmethod
+    def from_feature_keys(feature_keys: Iterable[FeatureKey]) -> FeatureDict:
         """Build a feature collection from a list of feature keys.
 
         The resulting feature collection matches the format of the
         feature keys, i.e. the feature keys apply to the collection.
 
         Take for example to following feature keys:
 
@@ -580,132 +736,48 @@
             feature_keys (Iterable[FeatureKey]):
                 iterable of feature keys to build a collection from
 
         Returns:
             collection (FeatureCollection):
                 resulting feature collection
         """
-        collection = FeatureKeyCollection()
-
+        feature = {}
         for key in feature_keys:
-            c = collection
+            c = feature
             # add all sub-entries
             for key_entry in key[:-1]:
                 if not isinstance(key_entry, str):
                     raise NotImplementedError()
                 if key_entry not in c:
                     c[key_entry] = {}
                 c = c[key_entry]
             # set key
             c[key[-1]] = key
 
-        return collection
-
-    def __str__(self) -> str:
-        """String representation of the feature key collection."""
-        return "FeatureKeyCollection(%s)" % str(dict(self))
-
-    def __repr__(self) -> str:
-        """String representation of the feature key collection."""
-        return str(self)
-
-    @classmethod
-    def __get_pydantic_core_schema__(
-        cls, source_type: Any, handler: GetCoreSchemaHandler
-    ) -> CoreSchema:
-        """Integrate feature key with pydantic."""
-        return core_schema.no_info_after_validator_function(cls, handler(dict))
-
-    @property
-    def feature_keys(self) -> Iterable[FeatureKey]:
-        """Iterator over all feature keys listed in the collection."""
-
-        def _iter_feature_keys(col: _FeatureKeyCollectionValue):
-            if isinstance(col, FeatureKey):
-                yield col
-            elif isinstance(col, dict):
-                yield from chain.from_iterable(
-                    map(_iter_feature_keys, col.values())
-                )
-            elif isinstance(col, list):
-                yield from chain.from_iterable(map(_iter_feature_keys, col))
-
-        yield from _iter_feature_keys(self)
-
-    def collect_features(self, features: Features) -> Features:
-        """Collect features.
-
-        Collect all features requested in the feature collection
-        and maintain the format of the collection.
-
-        Arguments:
-            features (Features):
-                source feature mapping from which to collect the requested
-                features
-
-        Returns:
-            collected_features (Features):
-                collected features in the format of the feature key collection
-        """
-
-        def _collect(v):
-            if isinstance(v, FeatureKey):
-                return v.index_features(features)
-            if isinstance(v, dict):
-                return FeatureKeyCollection.collect_features(v, features)
-            if isinstance(v, list):
-                assert len(v) > 0
-                # collect all features in specified in the list
-                collected_features = map(_collect, v)
-                f = next(collected_features)
-                # make sure the feature types match
-                for ff in collected_features:
-                    if not check_feature_equals(f, ff):
-                        raise TypeError(
-                            "Expected all items of a sequence to be of the "
-                            "same feature type, got %s != %s"
-                            % (str(f), str(ff))
-                        )
-                return Sequence(f, length=len(v))
-
-        return Features({key: _collect(val) for key, val in self.items()})
+        return FeatureDict(feature)
 
-    def collect_values(self, example: dict[str, Any]) -> dict[str, Any]:
-        """Collect Values.
+    def index_batch(self, batch: dist[str, list[Any]]) -> dict[str, list[Any]]:
+        """Index Batch.
 
-        Collect all values requested by the feature collection
-        and maintain the format of the collection.
+        Builds the batch of feature samples from a given batch according
+        to the specified scheme.
 
         Arguments:
-            example (dict[str, Any]):
-                example from which to collect the requested values
+            batch (dict[str, list[Any]]):
+                batch from which to build the samples
 
         Returns:
-            collected_values (dict[str, Any]):
-                collected values in the format of the feature key collection
+            build_batch (dict[str, list[Any]]):
+                the batch build from the given batch according to the scheme
         """
-        return _collect_from_example(self, example)
+        return _examples_to_batch(super(FeatureDict, self).index_batch(batch))
 
-    def collect_batch(
-        self, batch: dict[str, list[Any]]
-    ) -> dict[str, list[Any]]:
-        """Collect Batch.
+    def to_dict(self) -> dict[str, Any]:
+        """Convert to a python dictionary.
 
-        Collect all values from a batch of examples requested by the
-        feature collection and maintain the format of the collection.
-
-        Arguments:
-            batch (dict[str, list[Any]]):
-                example from which to collect the requested values
+        similar to `Feature.unpack` but is guaranteed to return a dictionary.
 
         Returns:
-            collected_values (dict[str, list[Any]]):
-                collected values in the format of the feature key collection
+            dict (dict[str, Any]):
+                feature scheme dictionary
         """
-        collected_batch = {key: [] for key in self.keys()}
-        for example in _batch_to_examples(batch):
-            for key, col in self.items():
-                collected_batch[key].append(
-                    _collect_from_example(col, example)
-                )
-
-        return collected_batch
+        return self.unpack()
```

### Comparing `hyped-0.1.0a0/src/hyped/common/lazy.py` & `hyped-0.1.0a1/src/hyped/common/lazy.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/graph.py` & `hyped-0.1.0a1/src/hyped/data/graph.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/io/datasets/__init__.py` & `hyped-0.1.0a1/src/hyped/data/io/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/io/datasets/cas.py` & `hyped-0.1.0a1/src/hyped/data/io/datasets/cas.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/io/datasets/typed_json.py` & `hyped-0.1.0a1/src/hyped/data/io/datasets/typed_json.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/io/writers/base.py` & `hyped-0.1.0a1/src/hyped/data/io/writers/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/io/writers/csv.py` & `hyped-0.1.0a1/src/hyped/data/io/writers/csv.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/io/writers/json.py` & `hyped-0.1.0a1/src/hyped/data/io/writers/json.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/pipe.py` & `hyped-0.1.0a1/src/hyped/data/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,14 @@
                 source dataset(s)
             **kwargs (dict[str, Any]):
                 arguments forwarded to datasets `.map` function
 
         Returns:
             out (datasets.Dataset|datasets.DatasetDict): processed dataset(s)
         """
-        # TODO: test this preparation logic
         # get the dataset features
         if isinstance(data, (datasets.Dataset, datasets.IterableDataset)):
             features = data.features
         elif isinstance(
             data, (datasets.DatasetDict, datasets.IterableDatasetDict)
         ):
             features = next(iter(data.values())).features
@@ -224,31 +223,30 @@
         elif not self.is_prepared:
             raise RuntimeError(
                 "Dataset features unknown, please manually prepare the data "
                 "pipe by calling the `.prepare` function with appropriate "
                 "features."
             )
 
-        # TODO: test this behavior
         # check if the data pipe contains and statistics that are expected
         # to be computed while running the data pipeline
         if (
             isinstance(data, (datasets.Dataset, datasets.DatasetDict))
             and any(isinstance(p, BaseDataStatistic) for p in self)
-            and not statistics_report_manager.is_empty
+            and not statistics_report_manager.is_empty()
         ):
             # load from cache file defaults to false
             kwargs["load_from_cache_file"] = kwargs.get(
                 "load_from_cache_file", False
             )
             # warn it dataset is loaded from cache
             if kwargs["load_from_cache_file"]:
                 warnings.warn(
                     "Loading map result from cache file will not compute "
-                    "statistics, set `load_from_cache_file` to False to avoid "
+                    "statistics, set `load_from_cache_file=False` to avoid "
                     "this behavior.",
                     UserWarning,
                 )
 
         # required settings
         kwargs["batched"] = True
         kwargs["with_indices"] = True
```

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/features/filter.py` & `hyped-0.1.0a1/src/hyped/data/processors/features/filter.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/features/flatten.py` & `hyped-0.1.0a1/src/hyped/data/processors/features/flatten.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Flatten Dataset Features Processor."""
 from datasets import Features
 from pydantic import Field
 
 from hyped.common.feature_key import (
+    FeatureDict,
     FeatureKey,
-    FeatureKeyCollection,
     _iter_keys_in_features,
 )
 from hyped.data.processors.features.format import (
     FormatFeatures,
     FormatFeaturesConfig,
 )
 
@@ -39,17 +39,15 @@
     """
 
     to_flatten: None | list[FeatureKey] = None
     delimiter: str = ":"
     depth: int = -1
     max_seq_length_to_unpack: int = 8
 
-    output_format: None | FeatureKeyCollection = Field(
-        default=None, init_var=False
-    )
+    output_format: None | FeatureDict = Field(default=None, init_var=False)
 
 
 class FlattenFeatures(FormatFeatures):
     """Flatten Dataset Features Processor.
 
     Similar to formatting features (see `hyped.data.processors.helpers.format`)
     but flattens nested features
@@ -81,22 +79,21 @@
         # in the feature mapping
         to_flatten = (
             self.config.to_flatten
             if self.config.to_flatten is not None
             else list(map(FeatureKey, features.keys()))
         )
 
-        collection = FeatureKeyCollection.from_feature_keys(to_flatten)
+        collection = FeatureDict.from_feature_keys(to_flatten).to_dict()
 
         for key in to_flatten:
             # get the feature to flatten
             feature = key.index_features(features)
 
-            # the key collection
-            # to add the flattened features into
+            # the key collection to add the flattened features into
             sub_collection = key[:-1].index_example(collection)
             assert key[-1] in sub_collection
             # flatten features
             flat_collection = {
                 self.config.delimiter.join(map(str, key[-1:] + k)): FeatureKey(
                     key + k
                 )
@@ -110,9 +107,9 @@
                     ),
                 )
             }
 
             sub_collection.pop(key[-1])
             sub_collection.update(flat_collection)
 
-        self.config.output_format = collection
+        self.config.output_format = FeatureDict(collection)
         return super(FlattenFeatures, self).map_features(features)
```

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/features/format.py` & `hyped-0.1.0a1/src/hyped/data/processors/features/format.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Format Dataset Features Data Processor."""
 
 from typing import Any, ClassVar
 
 from datasets import Features
 
-from hyped.common.feature_key import FeatureKeyCollection
+from hyped.common.feature_key import FeatureDict
 from hyped.data.processors.base import (
     BaseDataProcessor,
     BaseDataProcessorConfig,
 )
 
 
 class FormatFeaturesConfig(BaseDataProcessorConfig):
@@ -24,15 +24,15 @@
             of existing dataset features or paths (i.e. tuples) in case
             of nested features.
     """
 
     # include output format when parsing for required feature keys
     _IGNORE_KEYS_FROM_FIELDS: ClassVar[list[str]] = []
 
-    output_format: FeatureKeyCollection
+    output_format: FeatureDict
 
 
 class FormatFeatures(BaseDataProcessor[FormatFeaturesConfig]):
     """(Re-Format) Dataset Features Processor.
 
     Re-Formats Features of the dataset according to the
     mapping in the config.
```

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/sequence/apply_mask.py` & `hyped-0.1.0a1/src/hyped/data/processors/sequence/apply_mask.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/sequence/chunk.py` & `hyped-0.1.0a1/src/hyped/data/processors/sequence/chunk.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/sequence/extend.py` & `hyped-0.1.0a1/src/hyped/data/processors/sequence/extend.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/sequence/filter.py` & `hyped-0.1.0a1/src/hyped/data/processors/sequence/filter.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/sequence/join_str_seq.py` & `hyped-0.1.0a1/src/hyped/data/processors/sequence/join_str_seq.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/spans/apply_idx_spans.py` & `hyped-0.1.0a1/src/hyped/data/processors/spans/apply_idx_spans.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/spans/common.py` & `hyped-0.1.0a1/src/hyped/data/processors/spans/common.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/spans/from_bio.py` & `hyped-0.1.0a1/src/hyped/data/processors/spans/from_bio.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/spans/from_word_ids.py` & `hyped-0.1.0a1/src/hyped/data/processors/spans/from_word_ids.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/spans/idx_spans.py` & `hyped-0.1.0a1/src/hyped/data/processors/spans/idx_spans.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/spans/loc_to_glob.py` & `hyped-0.1.0a1/src/hyped/data/processors/spans/loc_to_glob.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/spans/overlaps.py` & `hyped-0.1.0a1/src/hyped/data/processors/spans/overlaps.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/statistics/base.py` & `hyped-0.1.0a1/src/hyped/data/processors/statistics/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/statistics/report.py` & `hyped-0.1.0a1/src/hyped/data/processors/statistics/report.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/statistics/sequence/disc_seq_val_hist.py` & `hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/disc_seq_val_hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     raise_feature_is_sequence,
 )
 from hyped.data.processors.statistics.value.disc_hist import (
     DiscreteHistogram,
     DiscreteHistogramConfig,
 )
 
-# TODO: write tests for sequence value histogram
-
 
 class DiscreteSequenceValueHistogramConfig(DiscreteHistogramConfig):
     """Discrete Sequence Value Histogram Data Statistic Config.
 
     Build a histogram of a given discrete sequence feature,
     e.g. ClassLabel or string.
```

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/statistics/sequence/seq_len_hist.py` & `hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/seq_len_hist.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     raise_feature_is_sequence,
 )
 from hyped.data.processors.statistics.value.hist import (
     Histogram,
     HistogramConfig,
 )
 
-# TODO: write tests for sequence length histogram
-
 
 class SequenceLengthHistogramConfig(HistogramConfig):
     """Sequence Length Histogram Data Statistic Config.
 
     Build a histogram over the lengths of a given sequence feature.
 
     Attributes:
@@ -42,19 +40,19 @@
     high: float = Field(default=0, init_var=False)
     num_bins: float = Field(default=0, init_var=False)
 
     def model_post_init(self, __context) -> None:
         """Initialize configuration."""
         # set values
         self.low = 0
-        self.high = self.num_bins = self.max_length
+        self.high = self.max_length
+        # +1 to accound for length zero
+        self.num_bins = self.max_length + 1
 
-        super(SequenceLengthHistogramConfig, self).__model_post_init__(
-            __context
-        )
+        super(SequenceLengthHistogramConfig, self).model_post_init(__context)
 
 
 class SequenceLengthHistogram(Histogram):
     """Sequence Length Histogram Data Statistic.
 
     Build a histogram over the lengths of a given sequence feature.
     """
```

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/statistics/sequence/seq_val_hist.py` & `hyped-0.1.0a1/src/hyped/data/processors/statistics/sequence/seq_val_hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 from hyped.common.feature_checks import raise_feature_is_sequence
 from hyped.data.processors.statistics.value.hist import (
     Histogram,
     HistogramConfig,
 )
 
-# TODO: write tests for sequence value histogram
-
 
 class SequenceValueHistogramConfig(HistogramConfig):
     """Sequence Value Histogram Data Statistic Config.
 
     Build a histogram of the values of a given sequence feature.
 
     Attributes:
```

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/statistics/value/disc_hist.py` & `hyped-0.1.0a1/src/hyped/data/processors/statistics/value/disc_hist.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 from hyped.common.feature_key import FeatureKey
 from hyped.data.processors.statistics.base import (
     BaseDataStatistic,
     BaseDataStatisticConfig,
 )
 from hyped.data.processors.statistics.report import StatisticsReportStorage
 
-# TODO: write tests for discrete sequence value histogram
-
 
 class DiscreteHistogramConfig(BaseDataStatisticConfig):
     """Discrete Histogram Data Statistic Config.
 
     Build a histogram of a given discrete value feature,
     e.g. ClassLabel or string.
 
@@ -45,24 +43,26 @@
     """Histogram Data Statistic.
 
     Build a histogram of a given discrete value feature,
     e.g. ClassLabel or string.
     """
 
     def _map_values(self, vals: list[Any]) -> list[Any]:
+        """Map values from indices to names in case of class label feature."""
         # get feature
         feature = self.config.feature_key.index_features(self.in_features)
         # check if feature is a class label
         if check_feature_equals(feature, ClassLabel):
             # map class ids to names
             return feature.int2str(vals)
 
         return vals
 
     def _compute_histogram(self, x: list[Any]) -> dict[Any, int]:
+        """Compute histogram from list of values."""
         return dict(Counter(self._map_values(x)))
 
     def initial_value(
         self, features: Features, manager: mp.Manager
     ) -> dict[Any, int]:
         """Initial histogram.
 
@@ -106,15 +106,15 @@
             examples (dict[str, list[Any]]): batch of examples
             index (list[int]): dataset indices of the batch of examples
             rank (int): execution process rank
 
         Returns:
             hist (dict[Any, str]): histogram of given batch of examples
         """
-        x = self.config.feature_key.index_features(examples)
+        x = self.config.feature_key.index_batch(examples)
         return self._compute_histogram(x)
 
     def compute(
         self,
         val: dict[Any, int],
         ext: dict[Any, int],
     ) -> dict[Any, int]:
```

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/statistics/value/hist.py` & `hyped-0.1.0a1/src/hyped/data/processors/statistics/value/hist.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/statistics/value/mean_and_std.py` & `hyped-0.1.0a1/src/hyped/data/processors/statistics/value/mean_and_std.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/taggers/bio.py` & `hyped-0.1.0a1/src/hyped/data/processors/taggers/bio.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/taggers/relex.py` & `hyped-0.1.0a1/src/hyped/data/processors/taggers/relex.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped/data/processors/tokenizers/hf.py` & `hyped-0.1.0a1/src/hyped/data/processors/tokenizers/hf.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/src/hyped.egg-info/SOURCES.txt` & `hyped-0.1.0a1/src/hyped.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 .gitignore
 .pre-commit-config.yaml
+CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 .github/workflows/docs.yml
 .github/workflows/linting.yml
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/build.sh
 docs/make.bat
+docs/source/add_ons.rst
 docs/source/conf.py
+docs/source/costum_data_processors.rst
+docs/source/feature_access.rst
+docs/source/getting_started.rst
 docs/source/index.rst
+docs/source/statistic_processors.rst
 docs/source/api/.gitkeep
-src/hyped/__init__.py
 src/hyped/__version__.py
 src/hyped.egg-info/PKG-INFO
 src/hyped.egg-info/SOURCES.txt
 src/hyped.egg-info/dependency_links.txt
 src/hyped.egg-info/requires.txt
 src/hyped.egg-info/top_level.txt
 src/hyped/base/__init__.py
@@ -76,61 +81,68 @@
 src/hyped/data/processors/statistics/value/mean_and_std.py
 src/hyped/data/processors/taggers/__init__.py
 src/hyped/data/processors/taggers/bio.py
 src/hyped/data/processors/taggers/relex.py
 src/hyped/data/processors/tokenizers/__init__.py
 src/hyped/data/processors/tokenizers/hf.py
 tests/__init__.py
-tests/base/__init__.py
-tests/base/test_config.py
-tests/base/test_generic.py
-tests/base/test_registry.py
-tests/common/__init__.py
-tests/common/test_arrow.py
-tests/common/test_consumer.py
-tests/common/test_feature_checks.py
-tests/common/test_feature_key.py
-tests/common/test_lazy.py
-tests/data/__init__.py
-tests/data/test_graph.py
-tests/data/test_pipe.py
-tests/data/io/__init__.py
-tests/data/io/datasets/__init__.py
-tests/data/io/datasets/test_cas.py
-tests/data/io/datasets/test_typed_json.py
-tests/data/io/writers/__init__.py
-tests/data/io/writers/base.py
-tests/data/io/writers/test_csv.py
-tests/data/io/writers/test_json.py
-tests/data/processors/__init__.py
-tests/data/processors/base.py
-tests/data/processors/test_base.py
-tests/data/processors/features/__init__.py
-tests/data/processors/features/test_filter.py
-tests/data/processors/features/test_flatten.py
-tests/data/processors/features/test_format.py
-tests/data/processors/sequence/__init__.py
-tests/data/processors/sequence/test_apply_mask.py
-tests/data/processors/sequence/test_chunk.py
-tests/data/processors/sequence/test_extend.py
-tests/data/processors/sequence/test_filter.py
-tests/data/processors/sequence/test_join_str_seq.py
-tests/data/processors/spans/__init__.py
-tests/data/processors/spans/test_apply_idx_spans.py
-tests/data/processors/spans/test_common.py
-tests/data/processors/spans/test_from_bio.py
-tests/data/processors/spans/test_from_word_ids.py
-tests/data/processors/spans/test_idx_spans.py
-tests/data/processors/spans/test_loc_to_glob.py
-tests/data/processors/spans/test_overlaps.py
-tests/data/processors/statistics/__init__.py
-tests/data/processors/statistics/base.py
-tests/data/processors/statistics/test_base.py
-tests/data/processors/statistics/test_report.py
-tests/data/processors/statistics/value/__init__.py
-tests/data/processors/statistics/value/test_hist.py
-tests/data/processors/statistics/value/test_mean_and_std.py
-tests/data/processors/taggers/__init__.py
-tests/data/processors/taggers/test_bio.py
-tests/data/processors/taggers/test_relex.py
-tests/data/processors/tokenizers/__init__.py
-tests/data/processors/tokenizers/test_hf.py
+tests/conftest.py
+tests/hyped/__init__.py
+tests/hyped/base/__init__.py
+tests/hyped/base/test_config.py
+tests/hyped/base/test_generic.py
+tests/hyped/base/test_registry.py
+tests/hyped/common/__init__.py
+tests/hyped/common/test_arrow.py
+tests/hyped/common/test_consumer.py
+tests/hyped/common/test_feature_checks.py
+tests/hyped/common/test_feature_key.py
+tests/hyped/common/test_lazy.py
+tests/hyped/data/__init__.py
+tests/hyped/data/test_graph.py
+tests/hyped/data/test_pipe.py
+tests/hyped/data/io/__init__.py
+tests/hyped/data/io/datasets/__init__.py
+tests/hyped/data/io/datasets/test_cas.py
+tests/hyped/data/io/datasets/test_typed_json.py
+tests/hyped/data/io/writers/__init__.py
+tests/hyped/data/io/writers/base.py
+tests/hyped/data/io/writers/test_csv.py
+tests/hyped/data/io/writers/test_json.py
+tests/hyped/data/processors/__init__.py
+tests/hyped/data/processors/base.py
+tests/hyped/data/processors/test_base.py
+tests/hyped/data/processors/features/__init__.py
+tests/hyped/data/processors/features/test_filter.py
+tests/hyped/data/processors/features/test_flatten.py
+tests/hyped/data/processors/features/test_format.py
+tests/hyped/data/processors/sequence/__init__.py
+tests/hyped/data/processors/sequence/test_apply_mask.py
+tests/hyped/data/processors/sequence/test_chunk.py
+tests/hyped/data/processors/sequence/test_extend.py
+tests/hyped/data/processors/sequence/test_filter.py
+tests/hyped/data/processors/sequence/test_join_str_seq.py
+tests/hyped/data/processors/spans/__init__.py
+tests/hyped/data/processors/spans/test_apply_idx_spans.py
+tests/hyped/data/processors/spans/test_common.py
+tests/hyped/data/processors/spans/test_from_bio.py
+tests/hyped/data/processors/spans/test_from_word_ids.py
+tests/hyped/data/processors/spans/test_idx_spans.py
+tests/hyped/data/processors/spans/test_loc_to_glob.py
+tests/hyped/data/processors/spans/test_overlaps.py
+tests/hyped/data/processors/statistics/__init__.py
+tests/hyped/data/processors/statistics/base.py
+tests/hyped/data/processors/statistics/test_base.py
+tests/hyped/data/processors/statistics/test_report.py
+tests/hyped/data/processors/statistics/sequence/__init__.py
+tests/hyped/data/processors/statistics/sequence/test_disc_seq_val_hist.py
+tests/hyped/data/processors/statistics/sequence/test_seq_len_hist.py
+tests/hyped/data/processors/statistics/sequence/test_seq_val_hist.py
+tests/hyped/data/processors/statistics/value/__init__.py
+tests/hyped/data/processors/statistics/value/test_disc_hist.py
+tests/hyped/data/processors/statistics/value/test_hist.py
+tests/hyped/data/processors/statistics/value/test_mean_and_std.py
+tests/hyped/data/processors/taggers/__init__.py
+tests/hyped/data/processors/taggers/test_bio.py
+tests/hyped/data/processors/taggers/test_relex.py
+tests/hyped/data/processors/tokenizers/__init__.py
+tests/hyped/data/processors/tokenizers/test_hf.py
```

### Comparing `hyped-0.1.0a0/tests/base/test_config.py` & `hyped-0.1.0a1/tests/hyped/base/test_config.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/base/test_generic.py` & `hyped-0.1.0a1/tests/hyped/base/test_generic.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/base/test_registry.py` & `hyped-0.1.0a1/tests/hyped/base/test_registry.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/common/test_arrow.py` & `hyped-0.1.0a1/tests/hyped/common/test_arrow.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/common/test_consumer.py` & `hyped-0.1.0a1/tests/hyped/common/test_consumer.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/common/test_feature_checks.py` & `hyped-0.1.0a1/tests/hyped/common/test_feature_checks.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/common/test_feature_key.py` & `hyped-0.1.0a1/tests/hyped/common/test_feature_key.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from contextlib import nullcontext
 
 import pytest
 from datasets import Features, Sequence, Value
 
 from hyped.common.feature_checks import check_feature_equals
-from hyped.common.feature_key import FeatureKey, FeatureKeyCollection
+from hyped.common.feature_key import FeatureDict, FeatureKey
 
 
 class TestFeatureKey(object):
     def test_basics(self):
         with pytest.raises(
             ValueError, match="First entry of a feature key must be a string"
         ):
@@ -367,164 +367,143 @@
     )
     def test_iter_keys_in_features(self, features, expected_keys):
         keys = list(FeatureKey.iter_keys_in_features(features))
         assert len(keys) == len(expected_keys)
         assert all(key in keys for key in expected_keys)
 
 
-class TestFeatureKeyCollection(object):
+class TestFeatureDict(object):
     def test_basics(self):
-        col = FeatureKeyCollection(
+        col = FeatureDict(
             {
                 "a": FeatureKey("a"),
                 "b": "b",
                 "c": ("x", "y"),
                 "d": [FeatureKey("a"), "b"],
                 "e": {"x": "x", "y": FeatureKey("y")},
             }
-        )
+        ).to_dict()
 
         assert isinstance(col["a"], FeatureKey)
         assert isinstance(col["b"], FeatureKey)
         assert isinstance(col["c"], FeatureKey)
         assert all(isinstance(k, FeatureKey) for k in col["d"])
         assert all(isinstance(k, FeatureKey) for k in col["e"].values())
 
-        col["x"] = "x"
-        col["y"] = ("x", "y")
-        col["z"] = ["x", "y"]
-        col["k"] = {"x": "x", "y": FeatureKey("y")}
-
-        assert isinstance(col["x"], FeatureKey)
-        assert isinstance(col["y"], FeatureKey)
-        assert all(isinstance(k, FeatureKey) for k in col["z"])
-        assert all(isinstance(k, FeatureKey) for k in col["k"].values())
-
     @pytest.mark.parametrize(
         "keys,expected_collection",
         [
-            ([FeatureKey("a")], FeatureKeyCollection({"a": FeatureKey("a")})),
+            ([FeatureKey("a")], FeatureDict({"a": FeatureKey("a")})),
             (
                 [FeatureKey("a"), FeatureKey("b")],
-                FeatureKeyCollection(
-                    {"a": FeatureKey("a"), "b": FeatureKey("b")}
-                ),
+                FeatureDict({"a": FeatureKey("a"), "b": FeatureKey("b")}),
             ),
             (
                 [FeatureKey("a", "b", "c"), FeatureKey("a", "x")],
-                FeatureKeyCollection(
+                FeatureDict(
                     {
                         "a": {
                             "b": {"c": FeatureKey("a", "b", "c")},
                             "x": FeatureKey("a", "x"),
                         },
                     }
                 ),
             ),
         ],
     )
     def test_from_features(self, keys, expected_collection):
-        assert (
-            FeatureKeyCollection.from_feature_keys(keys) == expected_collection
-        )
+        assert FeatureDict.from_feature_keys(keys) == expected_collection
 
     @pytest.mark.parametrize(
         "collection,expected_keys",
         [
-            (FeatureKeyCollection({"a": FeatureKey("a")}), [FeatureKey("a")]),
+            (FeatureDict({"a": FeatureKey("a")}), [FeatureKey("a")]),
             (
-                FeatureKeyCollection(
-                    {"a": FeatureKey("a"), "b": FeatureKey("b")}
-                ),
+                FeatureDict({"a": FeatureKey("a"), "b": FeatureKey("b")}),
                 [FeatureKey("a"), FeatureKey("b")],
             ),
             (
-                FeatureKeyCollection(
+                FeatureDict(
                     {
                         "a": FeatureKey("a"),
                         "b": {str(i): FeatureKey("b", i) for i in range(5)},
                     }
                 ),
                 [FeatureKey("a")] + [FeatureKey("b", i) for i in range(5)],
             ),
             (
-                FeatureKeyCollection(
+                FeatureDict(
                     {
                         "a": FeatureKey("a"),
                         "b": [FeatureKey("b", i) for i in range(5)],
                     }
                 ),
                 [FeatureKey("a")] + [FeatureKey("b", i) for i in range(5)],
             ),
         ],
     )
     def test_feature_keys(self, collection, expected_keys):
-        print(collection)
         keys = list(collection.feature_keys)
         assert len(keys) == len(expected_keys)
         assert all(key in keys for key in expected_keys)
 
     @pytest.mark.parametrize(
         "collection,features,expected_features",
         [
             (
-                FeatureKeyCollection({"a": FeatureKey("x")}),
+                FeatureDict({"a": FeatureKey("x")}),
                 Features({"x": Value("int32")}),
                 Features({"a": Value("int32")}),
             ),
             (
-                FeatureKeyCollection({"a": {"b": FeatureKey("x")}}),
+                FeatureDict({"a": {"b": FeatureKey("x")}}),
                 Features({"x": Value("int32")}),
                 Features({"a": {"b": Value("int32")}}),
             ),
             (
-                FeatureKeyCollection(
-                    {"a": [FeatureKey("x"), FeatureKey("y")]}
-                ),
+                FeatureDict({"a": [FeatureKey("x"), FeatureKey("y")]}),
                 Features({"x": Value("int32"), "y": Value("int32")}),
                 Features({"a": Sequence(Value("int32"), length=2)}),
             ),
         ],
     )
     def test_collect_features(self, collection, features, expected_features):
         assert check_feature_equals(
-            collection.collect_features(features), expected_features
+            collection.index_features(features), expected_features
         )
 
     @pytest.mark.parametrize(
         "collection,example,expected_values",
         [
-            (FeatureKeyCollection({"a": FeatureKey("x")}), {"x": 5}, {"a": 5}),
+            (FeatureDict({"a": FeatureKey("x")}), {"x": 5}, {"a": 5}),
             (
-                FeatureKeyCollection({"a": {"b": FeatureKey("x")}}),
+                FeatureDict({"a": {"b": FeatureKey("x")}}),
                 {"x": 5},
                 {"a": {"b": 5}},
             ),
             (
-                FeatureKeyCollection(
-                    {"a": [FeatureKey("x"), FeatureKey("y")]}
-                ),
+                FeatureDict({"a": [FeatureKey("x"), FeatureKey("y")]}),
                 {"x": 5, "y": 6},
                 {"a": [5, 6]},
             ),
         ],
     )
     def test_collect_values(self, collection, example, expected_values):
-        assert collection.collect_values(example) == expected_values
+        assert collection.index_example(example) == expected_values
 
     @pytest.mark.parametrize(
         "collection,batch,expected_values",
         [
             (
-                FeatureKeyCollection({"a": FeatureKey("x")}),
+                FeatureDict({"a": FeatureKey("x")}),
                 {"x": list(range(10))},
                 {"a": list(range(10))},
             ),
             (
-                FeatureKeyCollection({"a": {"b": FeatureKey("x")}}),
+                FeatureDict({"a": {"b": FeatureKey("x")}}),
                 {"x": list(range(10))},
                 {"a": [{"b": i} for i in range(10)]},
             ),
         ],
     )
     def test_collect_batch(self, collection, batch, expected_values):
-        assert collection.collect_batch(batch) == expected_values
+        assert collection.index_batch(batch) == expected_values
```

### Comparing `hyped-0.1.0a0/tests/common/test_lazy.py` & `hyped-0.1.0a1/tests/hyped/common/test_lazy.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/data/io/datasets/test_cas.py` & `hyped-0.1.0a1/tests/hyped/data/io/datasets/test_cas.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/data/io/datasets/test_typed_json.py` & `hyped-0.1.0a1/tests/hyped/data/io/datasets/test_typed_json.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/data/io/writers/base.py` & `hyped-0.1.0a1/tests/hyped/data/io/writers/base.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/data/io/writers/test_csv.py` & `hyped-0.1.0a1/tests/hyped/data/io/writers/test_csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datasets
 import pytest
 
 from hyped.data.io.writers.csv import CsvDatasetWriter
-from tests.data.io.writers.base import BaseTestDatasetWriter
+from tests.hyped.data.io.writers.base import BaseTestDatasetWriter
 
 
 class TestCsvDatasetWriter(BaseTestDatasetWriter):
     @pytest.fixture
     def writer(self, tmpdir, num_proc):
         return CsvDatasetWriter(
             save_dir=tmpdir, exist_ok=True, num_proc=num_proc
```

### Comparing `hyped-0.1.0a0/tests/data/io/writers/test_json.py` & `hyped-0.1.0a1/tests/hyped/data/io/writers/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datasets
 import pytest
 
 from hyped.data.io.writers.json import JsonDatasetWriter
-from tests.data.io.writers.base import BaseTestDatasetWriter
+from tests.hyped.data.io.writers.base import BaseTestDatasetWriter
 
 
 class TestJsonDatasetWriter(BaseTestDatasetWriter):
     @pytest.fixture
     def writer(self, tmpdir, num_proc):
         return JsonDatasetWriter(
             save_dir=tmpdir, exist_ok=True, num_proc=num_proc
```

### Comparing `hyped-0.1.0a0/tests/data/processors/base.py` & `hyped-0.1.0a1/tests/hyped/data/processors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,14 @@
         expected_out_features,
     ):
         # processor should be prepared at this point
         assert processor.is_prepared
 
         # check new and output features
         if expected_out_features is not None:
-            print(processor.new_features)
-            print(expected_out_features)
             assert processor.new_features == expected_out_features
 
             if processor.config.keep_input_features:
                 assert processor.out_features == (
                     in_features | expected_out_features
                 )
             else:
```

### Comparing `hyped-0.1.0a0/tests/data/processors/features/test_filter.py` & `hyped-0.1.0a1/tests/hyped/data/processors/features/test_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.features.filter import (
     FilterFeatures,
     FilterFeaturesConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 FEATURES = Features(
     {
         "X": Value("int32"),
         "Y": Sequence(Value("int32"), length=3),
         "A": {
             "x": Value("int32"),
```

### Comparing `hyped-0.1.0a0/tests/data/processors/features/test_flatten.py` & `hyped-0.1.0a1/tests/hyped/data/processors/features/test_flatten.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datasets import Features, Sequence, Value
 
 from hyped.common.feature_key import FeatureKey
 from hyped.data.processors.features.flatten import (
     FlattenFeatures,
     FlattenFeaturesConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class BaseTestFlattenFeatures(BaseTestDataProcessor):
     @pytest.fixture()
     def in_features(self):
         return Features(
             {
```

### Comparing `hyped-0.1.0a0/tests/data/processors/features/test_format.py` & `hyped-0.1.0a1/tests/hyped/data/processors/features/test_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datasets import Features, Sequence, Value
 
 from hyped.common.feature_key import FeatureKey
 from hyped.data.processors.features.format import (
     FormatFeatures,
     FormatFeaturesConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestFormatFeaturesConfig(object):
     def test_required_features(self):
         config = FormatFeaturesConfig(
             output_format={"new_X": "X", "new_Y": "Y"}
         )
```

### Comparing `hyped-0.1.0a0/tests/data/processors/sequence/test_apply_mask.py` & `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_apply_mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.sequence.apply_mask import (
     ApplyMask,
     ApplyMaskConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestApplyMask(BaseTestDataProcessor):
     @pytest.fixture
     def length(self):
         return 5
```

### Comparing `hyped-0.1.0a0/tests/data/processors/sequence/test_chunk.py` & `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_chunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.sequence.chunk import (
     ChunkSequence,
     ChunkSequenceConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestChunkSequence(BaseTestDataProcessor):
     @pytest.fixture(
         params=[
             {
                 # perfect chunk no overlap
```

### Comparing `hyped-0.1.0a0/tests/data/processors/sequence/test_extend.py` & `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_extend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.sequence.extend import (
     ExtendSequence,
     ExtendSequenceConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestExtendSequence(BaseTestDataProcessor):
     @pytest.fixture(
         params=[
             {
                 "feature": Value("int32"),
```

### Comparing `hyped-0.1.0a0/tests/data/processors/sequence/test_filter.py` & `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from datasets import ClassLabel, Features, Sequence, Value
 
 from hyped.data.processors.sequence.filter import (
     FilterSequence,
     FilterSequenceConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestFilterSequence(BaseTestDataProcessor):
     @pytest.fixture(
         params=[
             [int(i < 3) for i in range(10)],
             [int(i < 5) for i in range(10)],
```

### Comparing `hyped-0.1.0a0/tests/data/processors/sequence/test_join_str_seq.py` & `hyped-0.1.0a1/tests/hyped/data/processors/sequence/test_join_str_seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.sequence.join_str_seq import (
     JoinStringSequence,
     JoinStringSequenceConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestJoinStringSequence(BaseTestDataProcessor):
     @pytest.fixture(params=[" ", ",", " | "])
     def delimiter(self, request):
         return request.param
```

### Comparing `hyped-0.1.0a0/tests/data/processors/spans/test_apply_idx_spans.py` & `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_apply_idx_spans.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.spans.apply_idx_spans import (
     ApplyIndexSpans,
     ApplyIndexSpansConfig,
 )
 from hyped.data.processors.spans.common import SpansOutputs
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestApplyIndexSpans(BaseTestDataProcessor):
     @pytest.fixture(params=[True, False])
     def is_idx_spans_inclusive(self, request):
         return request.param
```

### Comparing `hyped-0.1.0a0/tests/data/processors/spans/test_common.py` & `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_common.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/data/processors/spans/test_from_bio.py` & `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_from_bio.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datasets import ClassLabel, Features, Sequence, Value
 
 from hyped.data.processors.spans.common import LabelledSpansOutputs
 from hyped.data.processors.spans.from_bio import (
     TokenSpansFromBioTags,
     TokenSpansFromBioTagsConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestTokenSpansFromBioTags(BaseTestDataProcessor):
     @pytest.fixture(
         params=[
             # basics
             [(3, 4, "X")],
```

### Comparing `hyped-0.1.0a0/tests/data/processors/spans/test_from_word_ids.py` & `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_from_word_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.spans.common import SpansOutputs
 from hyped.data.processors.spans.from_word_ids import (
     TokenSpansFromWordIds,
     TokenSpansFromWordIdsConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestTokenSpansFromWordIds(BaseTestDataProcessor):
     @pytest.fixture(
         params=[
             [(0, 5)],
             [(0, 5), (5, 10)],
```

### Comparing `hyped-0.1.0a0/tests/data/processors/spans/test_idx_spans.py` & `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_idx_spans.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.spans.common import SpansOutputs
 from hyped.data.processors.spans.idx_spans import (
     CoveredIndexSpans,
     CoveredIndexSpansConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestCoveredIndexSpansErrors(BaseTestDataProcessor):
     @pytest.fixture(
         params=[
             # invalid feature type
             {
```

### Comparing `hyped-0.1.0a0/tests/data/processors/spans/test_loc_to_glob.py` & `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_loc_to_glob.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.spans.common import SpansOutputs
 from hyped.data.processors.spans.loc_to_glob import (
     LocalToGlobalOffsets,
     LocalToGlobalOffsetsConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestLocalToGlobalOffsetsKeyErrors(BaseTestDataProcessor):
     @pytest.fixture
     def in_features(self):
         return Features(
             {
```

### Comparing `hyped-0.1.0a0/tests/data/processors/spans/test_overlaps.py` & `hyped-0.1.0a1/tests/hyped/data/processors/spans/test_overlaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.spans.common import SpansOutputs
 from hyped.data.processors.spans.overlaps import (
     ResolveSpanOverlaps,
     ResolveSpanOverlapsConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestResolveSpanOverlaps(BaseTestDataProcessor):
     @pytest.fixture(
         params=[
             [[], []],
             [[(2, 4), (5, 9)], [True, True]],
```

### Comparing `hyped-0.1.0a0/tests/data/processors/statistics/base.py` & `hyped-0.1.0a1/tests/hyped/data/processors/statistics/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 import pytest
 from datasets import Features
 
 from hyped.data.processors.statistics.base import BaseDataStatistic
 from hyped.data.processors.statistics.report import StatisticsReport
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class BaseTestDataStatistic(BaseTestDataProcessor):
     @pytest.fixture
     @abstractmethod
     def statistic(self, request) -> BaseDataStatistic:
         ...
```

### Comparing `hyped-0.1.0a0/tests/data/processors/statistics/test_base.py` & `hyped-0.1.0a1/tests/hyped/data/processors/statistics/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from datasets import Features, Value
 
 from hyped.data.processors.statistics.base import (
     BaseDataStatistic,
     BaseDataStatisticConfig,
 )
 from hyped.data.processors.statistics.report import StatisticsReport
-from tests.data.processors.statistics.base import BaseTestDataStatistic
-from tests.data.processors.statistics.test_report import is_lock_acquired
+from tests.hyped.data.processors.statistics.base import BaseTestDataStatistic
+from tests.hyped.data.processors.statistics.test_report import is_lock_acquired
 
 
 class ConstantStatisticConfig(BaseDataStatisticConfig):
     statistic_key: str = "constant"
     init_val: int = 0
     val: int = 1
```

### Comparing `hyped-0.1.0a0/tests/data/processors/statistics/test_report.py` & `hyped-0.1.0a1/tests/hyped/data/processors/statistics/test_report.py`

 * *Files identical despite different names*

### Comparing `hyped-0.1.0a0/tests/data/processors/statistics/value/test_hist.py` & `hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_hist.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytest
 from datasets import Features, Value
 
 from hyped.data.processors.statistics.value.hist import (
     Histogram,
     HistogramConfig,
 )
-from tests.data.processors.statistics.base import BaseTestDataStatistic
+from tests.hyped.data.processors.statistics.base import BaseTestDataStatistic
 
 
 class TestHistogram(BaseTestDataStatistic):
     @pytest.fixture
     def in_features(self):
         return Features({"A": Value("float64")})
```

### Comparing `hyped-0.1.0a0/tests/data/processors/statistics/value/test_mean_and_std.py` & `hyped-0.1.0a1/tests/hyped/data/processors/statistics/value/test_mean_and_std.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datasets import Features, Value
 
 from hyped.data.processors.statistics.value.mean_and_std import (
     MeanAndStd,
     MeanAndStdConfig,
     MeanAndStdTuple,
 )
-from tests.data.processors.statistics.base import BaseTestDataStatistic
+from tests.hyped.data.processors.statistics.base import BaseTestDataStatistic
 
 
 class TestMeanAndStd(BaseTestDataStatistic):
     @pytest.fixture
     def in_features(self):
         return Features({"A": Value("float64")})
```

### Comparing `hyped-0.1.0a0/tests/data/processors/taggers/test_bio.py` & `hyped-0.1.0a1/tests/hyped/data/processors/taggers/test_bio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from itertools import permutations
 
 import pytest
 from datasets import ClassLabel, Features, Sequence, Value
 
 from hyped.data.processors.taggers.bio import BioTagger, BioTaggerConfig
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestBioTagger(BaseTestDataProcessor):
     @pytest.fixture(params=[False, True])
     def is_span_inclusive(self, request):
         return request.param
```

### Comparing `hyped-0.1.0a0/tests/data/processors/taggers/test_relex.py` & `hyped-0.1.0a1/tests/hyped/data/processors/taggers/test_relex.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datasets import Features, Sequence, Value
 
 from hyped.data.processors.taggers.relex import (
     RelExTagger,
     RelExTaggerConfig,
     RelExTaggerOutputs,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 class TestRelExTagger(BaseTestDataProcessor):
     @pytest.fixture(
         params=[
             {
                 "input_sequence": [0, 1, 2, 3, 4, 5, 6, 7, 8],
```

### Comparing `hyped-0.1.0a0/tests/data/processors/tokenizers/test_hf.py` & `hyped-0.1.0a1/tests/hyped/data/processors/tokenizers/test_hf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datasets import Features, Sequence, Value
 from transformers import AutoTokenizer
 
 from hyped.data.processors.tokenizers.hf import (
     HuggingFaceTokenizer,
     HuggingFaceTokenizerConfig,
 )
-from tests.data.processors.base import BaseTestDataProcessor
+from tests.hyped.data.processors.base import BaseTestDataProcessor
 
 
 @pytest.fixture(params=["bert-base-uncased", "bert-base-german-cased"])
 def tokenizer(request):
     return request.param
```

### Comparing `hyped-0.1.0a0/tests/data/test_graph.py` & `hyped-0.1.0a1/tests/hyped/data/test_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,18 @@
                 # make sure node is connected to any input feature
                 assert max_length != -1
                 assert node_layers[node] == max_length
 
         # test if graph matches expected topology
         assert nx.is_isomorphic(G, graph)
 
+    def test_plot(self, G):
+        # hard to test but at least check for errors
+        G.plot()
+
 
 class TestSimplePath(BaseTestProcessGraph):
     @pytest.fixture
     def features(self) -> Features:
         return Features({"x": Value("int32")})
 
     @pytest.fixture
```

### Comparing `hyped-0.1.0a0/tests/data/test_pipe.py` & `hyped-0.1.0a1/tests/hyped/data/test_pipe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import datasets
 import pytest
 
 from hyped.data.pipe import DataPipe
-from tests.data.processors.test_base import (
+from hyped.data.processors.statistics.report import StatisticsReport
+from tests.hyped.data.processors.statistics.test_base import (
+    ConstantStatistic,
+    ConstantStatisticConfig,
+)
+from tests.hyped.data.processors.test_base import (
     ConstantDataProcessor,
     ConstantDataProcessorConfig,
 )
 
 
 @pytest.fixture
 def sample_data_pipe():
@@ -146,7 +151,55 @@
         assert all(k in ds.features for k in "XABC")
         assert all(x == ("example %i" % i) for i, x in enumerate(ds["X"]))
         assert all(a == "1" for a in ds["A"])
         assert all(a == "2" for a in ds["B"])
         assert all(a == "3" for a in ds["C"])
         # check features
         assert sample_data_pipe.out_features == ds.features
+
+    def test_warning_on_use_cache_and_statistic(self):
+        # create sample dataset
+        ds = datasets.Dataset.from_dict(
+            {"X": ["example %i" % i for i in range(1)]}
+        )
+
+        with StatisticsReport() as report:
+            # create data pipe containing a statistics processor
+            sample_data_pipe = DataPipe(
+                [ConstantStatistic(ConstantStatisticConfig(), report)]
+            )
+            # should not warn as the statistic is always computed
+            sample_data_pipe.apply(
+                ds, batch_size=1, load_from_cache_file=False
+            )
+
+        with StatisticsReport() as report:
+            # create data pipe containing a statistics processor
+            sample_data_pipe = DataPipe(
+                [ConstantStatistic(ConstantStatisticConfig(), report)]
+            )
+            # check for warning when statistic might not be computed
+            with pytest.warns(UserWarning):
+                sample_data_pipe.apply(
+                    ds, batch_size=1, load_from_cache_file=True
+                )
+
+    def test_error_on_missing_features(self, sample_data_pipe, tmp_path):
+        # create sample data file in json format
+        p = tmp_path / "data.json"
+        p.write_text('{"A": 0}')
+        # stream data from file
+        # datasets cannot infer the features when streaming from a file
+        ds = datasets.load_dataset(
+            "json", data_files=p.as_posix(), split="train", streaming=True
+        )
+        assert ds.features is None
+
+        # should lead to a runtime error as the pipe cannot be prepared
+        with pytest.raises(RuntimeError):
+            sample_data_pipe.apply(ds)
+
+        # need to be prepared manually
+        sample_data_pipe.prepare(
+            datasets.Features({"A": datasets.Value("int32")})
+        )
+        sample_data_pipe.apply(ds)
```


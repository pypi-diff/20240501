# Comparing `tmp/pyranges1-0.1.0.tar.gz` & `tmp/pyranges1-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyranges1-0.1.0.tar", last modified: Wed May  1 10:55:56 2024, max compression
+gzip compressed data, was "pyranges1-0.1.1.tar", last modified: Wed May  1 12:11:43 2024, max compression
```

## Comparing `pyranges1-0.1.0.tar` & `pyranges1-0.1.1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.314298 pyranges1-0.1.0/
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:52.545755 pyranges1-0.1.0/.github/
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:52.848362 pyranges1-0.1.0/.github/workflows/
--rw-r--r--   0 endbak01   (501) staff       (20)     1555 2024-05-01 07:23:12.000000 pyranges1-0.1.0/.github/workflows/build-book.yml
--rw-r--r--   0 endbak01   (501) staff       (20)      855 2024-05-01 07:23:12.000000 pyranges1-0.1.0/.github/workflows/build_and_upload_wheels.yml
--rw-r--r--   0 endbak01   (501) staff       (20)     1091 2024-05-01 07:23:12.000000 pyranges1-0.1.0/.github/workflows/check.yml
--rw-r--r--   0 endbak01   (501) staff       (20)      731 2024-05-01 07:23:12.000000 pyranges1-0.1.0/.github/workflows/run_hypothesis_tests.yml
--rw-r--r--   0 endbak01   (501) staff       (20)      270 2024-05-01 07:23:12.000000 pyranges1-0.1.0/.gitignore
--rw-r--r--   0 endbak01   (501) staff       (20)       54 2024-05-01 07:23:12.000000 pyranges1-0.1.0/CHANGELOG.txt
--rw-r--r--   0 endbak01   (501) staff       (20)     1063 2024-05-01 07:23:12.000000 pyranges1-0.1.0/LICENSE
--rw-r--r--   0 endbak01   (501) staff       (20)     4249 2024-05-01 10:55:56.310596 pyranges1-0.1.0/PKG-INFO
--rw-r--r--   0 endbak01   (501) staff       (20)     2319 2024-05-01 10:51:52.000000 pyranges1-0.1.0/README.md
--rwxr-xr-x   0 endbak01   (501) staff       (20)     2077 2024-05-01 07:23:12.000000 pyranges1-0.1.0/check_typing_linting_and_formatting.py
--rw-r--r--   0 endbak01   (501) staff       (20)      718 2024-05-01 07:23:12.000000 pyranges1-0.1.0/conftest.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:53.360806 pyranges1-0.1.0/docs/
--rw-r--r--   0 endbak01   (501) staff       (20)      634 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/Makefile
--rw-r--r--   0 endbak01   (501) staff       (20)      557 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/api_reference.rst
--rw-r--r--   0 endbak01   (501) staff       (20)     2487 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/conf.py
--rw-r--r--   0 endbak01   (501) staff       (20)    13159 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/developer_guide.rst
--rw-r--r--   0 endbak01   (501) staff       (20)      233 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/extension_orfs.rst
--rw-r--r--   0 endbak01   (501) staff       (20)      157 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/extension_seqs.rst
--rw-r--r--   0 endbak01   (501) staff       (20)      170 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/extension_stats.rst
--rw-r--r--   0 endbak01   (501) staff       (20)     8593 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/how_to_columns.rst
--rw-r--r--   0 endbak01   (501) staff       (20)    15830 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/how_to_create.rst
--rw-r--r--   0 endbak01   (501) staff       (20)    33827 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/how_to_genomic_ops.rst
--rw-r--r--   0 endbak01   (501) staff       (20)    11786 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/how_to_inspect.rst
--rw-r--r--   0 endbak01   (501) staff       (20)      246 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/how_to_pages.rst
--rw-r--r--   0 endbak01   (501) staff       (20)    21762 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/how_to_rows.rst
--rw-r--r--   0 endbak01   (501) staff       (20)     9979 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/how_to_sequences.rst
--rw-r--r--   0 endbak01   (501) staff       (20)     3737 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/how_to_write.rst
--rw-r--r--   0 endbak01   (501) staff       (20)     1633 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/index.rst
--rw-r--r--   0 endbak01   (501) staff       (20)      975 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/installation.rst
--rw-r--r--   0 endbak01   (501) staff       (20)      795 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/make.bat
--rw-r--r--   0 endbak01   (501) staff       (20)      227 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/pyranges_extensions.rst
--rw-r--r--   0 endbak01   (501) staff       (20)     2979 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/pyranges_module.rst
--rw-r--r--   0 endbak01   (501) staff       (20)      209 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/pyranges_objects.rst
--rw-r--r--   0 endbak01   (501) staff       (20)      271 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/range_frame.rst
--rw-r--r--   0 endbak01   (501) staff       (20)       38 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/requirements.txt
--rw-r--r--   0 endbak01   (501) staff       (20)     1191 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/todos.rst
--rw-r--r--   0 endbak01   (501) staff       (20)    46812 2024-05-01 07:23:12.000000 pyranges1-0.1.0/docs/tutorial.rst
--rw-r--r--   0 endbak01   (501) staff       (20)     2752 2024-05-01 10:52:41.000000 pyranges1-0.1.0/pyproject.toml
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:53.388774 pyranges1-0.1.0/pyranges/
--rw-r--r--   0 endbak01   (501) staff       (20)     1066 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/__init__.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:53.501968 pyranges1-0.1.0/pyranges/core/
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/__init__.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1672 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/empty.py
--rw-r--r--   0 endbak01   (501) staff       (20)    12623 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/example_data.py
--rw-r--r--   0 endbak01   (501) staff       (20)     5476 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/loci_getter.py
--rw-r--r--   0 endbak01   (501) staff       (20)     6200 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/multioverlap.py
--rw-r--r--   0 endbak01   (501) staff       (20)     5200 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/names.py
--rw-r--r--   0 endbak01   (501) staff       (20)     3424 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/options.py
--rw-r--r--   0 endbak01   (501) staff       (20)     9214 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/out.py
--rw-r--r--   0 endbak01   (501) staff       (20)     4957 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/parallelism.py
--rw-r--r--   0 endbak01   (501) staff       (20)    10009 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/pyranges_groupby.py
--rw-r--r--   0 endbak01   (501) staff       (20)     7223 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/pyranges_helpers.py
--rw-r--r--   0 endbak01   (501) staff       (20)   213034 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/pyranges_main.py
--rw-r--r--   0 endbak01   (501) staff       (20)     2845 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/random.py
--rw-r--r--   0 endbak01   (501) staff       (20)     7161 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/tostring.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1315 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/core/version.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:53.582936 pyranges1-0.1.0/pyranges/data/
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/__init__.py
--rw-r--r--   0 endbak01   (501) staff       (20)      327 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/aorta.bed
--rw-r--r--   0 endbak01   (501) staff       (20)      269 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/aorta2.bed
--rw-r--r--   0 endbak01   (501) staff       (20)   309369 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/chipseq.bed
--rw-r--r--   0 endbak01   (501) staff       (20)   309045 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/chipseq_background.bed
--rw-r--r--   0 endbak01   (501) staff       (20)      426 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/chromsizes.bed
--rw-r--r--   0 endbak01   (501) staff       (20)    28209 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/cpg.bed
--rw-r--r--   0 endbak01   (501) staff       (20)     4845 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/ensembl.gtf
--rw-r--r--   0 endbak01   (501) staff       (20)    35943 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/ensembl_human.gtf.gz
--rw-r--r--   0 endbak01   (501) staff       (20)    64417 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/exons.bed
--rw-r--r--   0 endbak01   (501) staff       (20)       69 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/f1.bed
--rw-r--r--   0 endbak01   (501) staff       (20)       30 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/f2.bed
--rw-r--r--   0 endbak01   (501) staff       (20)    81253 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/gencode_human.gtf.gz
--rw-r--r--   0 endbak01   (501) staff       (20)    55608 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/lamina.bed
--rw-r--r--   0 endbak01   (501) staff       (20)   387402 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/ncbi.fasta
--rw-r--r--   0 endbak01   (501) staff       (20)      220 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/ncbi.fasta.fai
--rw-r--r--   0 endbak01   (501) staff       (20)     3041 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/ncbi.gff.gz
--rw-r--r--   0 endbak01   (501) staff       (20)     1366 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/smaller.bam
--rw-r--r--   0 endbak01   (501) staff       (20)    62555 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/data/ucsc_human.bed.gz
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/docs
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:53.747952 pyranges1-0.1.0/pyranges/ext/
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/ext/__init__.py
--rw-r--r--   0 endbak01   (501) staff       (20)    30149 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/ext/orfs.py
--rw-r--r--   0 endbak01   (501) staff       (20)    13762 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/ext/seqs.py
--rw-r--r--   0 endbak01   (501) staff       (20)    27439 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/ext/stats.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:54.737687 pyranges1-0.1.0/pyranges/methods/
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/__init__.py
--rw-r--r--   0 endbak01   (501) staff       (20)     2197 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/boundaries.py
--rw-r--r--   0 endbak01   (501) staff       (20)      645 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/cluster.py
--rw-r--r--   0 endbak01   (501) staff       (20)      900 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/combine_positions.py
--rw-r--r--   0 endbak01   (501) staff       (20)     3407 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/concat.py
--rw-r--r--   0 endbak01   (501) staff       (20)     2114 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/coverage.py
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/itergrs.py
--rw-r--r--   0 endbak01   (501) staff       (20)     2483 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/join.py
--rw-r--r--   0 endbak01   (501) staff       (20)      365 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/max_disjoint.py
--rw-r--r--   0 endbak01   (501) staff       (20)      857 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/merge.py
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/merge_cluster.py
--rw-r--r--   0 endbak01   (501) staff       (20)     5349 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/nearest.py
--rw-r--r--   0 endbak01   (501) staff       (20)     3983 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/overlap.py
--rw-r--r--   0 endbak01   (501) staff       (20)      254 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/sort.py
--rw-r--r--   0 endbak01   (501) staff       (20)     3818 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/spliced_subsequence.py
--rw-r--r--   0 endbak01   (501) staff       (20)      952 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/split.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1349 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/statistics.py
--rw-r--r--   0 endbak01   (501) staff       (20)     3500 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/subsequence.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1229 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/subtraction.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1612 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/summary.py
--rw-r--r--   0 endbak01   (501) staff       (20)     4056 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/tile_genome.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1107 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/to_rle.py
--rw-r--r--   0 endbak01   (501) staff       (20)     2354 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/methods/windows.py
--rw-r--r--   0 endbak01   (501) staff       (20)       73 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/orfs.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:54.794372 pyranges1-0.1.0/pyranges/range_frame/
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/range_frame/__init__.py
--rw-r--r--   0 endbak01   (501) staff       (20)    12603 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/range_frame/range_frame.py
--rw-r--r--   0 endbak01   (501) staff       (20)     6741 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/range_frame/range_frame_validator.py
--rw-r--r--   0 endbak01   (501) staff       (20)    21738 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/readers.py
--rw-r--r--   0 endbak01   (501) staff       (20)      138 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/seqs.py
--rw-r--r--   0 endbak01   (501) staff       (20)      338 2024-05-01 07:23:12.000000 pyranges1-0.1.0/pyranges/stats.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.302981 pyranges1-0.1.0/pyranges1.egg-info/
--rw-r--r--   0 endbak01   (501) staff       (20)     4249 2024-05-01 10:55:52.000000 pyranges1-0.1.0/pyranges1.egg-info/PKG-INFO
--rw-r--r--   0 endbak01   (501) staff       (20)     3914 2024-05-01 10:55:52.000000 pyranges1-0.1.0/pyranges1.egg-info/SOURCES.txt
--rw-r--r--   0 endbak01   (501) staff       (20)        1 2024-05-01 10:55:52.000000 pyranges1-0.1.0/pyranges1.egg-info/dependency_links.txt
--rw-r--r--   0 endbak01   (501) staff       (20)      352 2024-05-01 10:55:52.000000 pyranges1-0.1.0/pyranges1.egg-info/requires.txt
--rw-r--r--   0 endbak01   (501) staff       (20)       25 2024-05-01 10:55:52.000000 pyranges1-0.1.0/pyranges1.egg-info/top_level.txt
--rw-r--r--   0 endbak01   (501) staff       (20)       38 2024-05-01 10:55:56.314589 pyranges1-0.1.0/setup.cfg
--rw-r--r--   0 endbak01   (501) staff       (20)      246 2024-05-01 07:23:12.000000 pyranges1-0.1.0/setup.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:55.189503 pyranges1-0.1.0/tests/
--rw-r--r--   0 endbak01   (501) staff       (20)    11164 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/.fuse_hidden0000017200000002
--rw-r--r--   0 endbak01   (501) staff       (20)     1820 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/helpers.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1890 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/hi
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:55.503864 pyranges1-0.1.0/tests/property_based/
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/property_based/__init__.py
--rw-r--r--   0 endbak01   (501) staff       (20)     7906 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/property_based/hypothesis_helper.py
--rw-r--r--   0 endbak01   (501) staff       (20)     9254 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/property_based/new.py
--rw-r--r--   0 endbak01   (501) staff       (20)    17767 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/property_based/test_binary.py
--rw-r--r--   0 endbak01   (501) staff       (20)     3413 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/property_based/test_do_not_error.py
--rw-r--r--   0 endbak01   (501) staff       (20)     9456 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/property_based/test_unary.py
--rw-r--r--   0 endbak01   (501) staff       (20)      312 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/run_doctest_tutorial_howto.py
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/test_calculate_frame.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1464 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/test_parallelism.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.045608 pyranges1-0.1.0/tests/unit/
--rw-r--r--   0 endbak01   (501) staff       (20)        1 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/__init__.py
--rw-r--r--   0 endbak01   (501) staff       (20)      534 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/chip_10.bed
--rw-r--r--   0 endbak01   (501) staff       (20)     2354 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/conftest.py
--rw-r--r--   0 endbak01   (501) staff       (20)       44 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/f1.bed
--rw-r--r--   0 endbak01   (501) staff       (20)       29 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/f2.bed
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.047411 pyranges1-0.1.0/tests/unit/getitem/
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/getitem/test_getitem.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1890 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/hi
--rw-r--r--   0 endbak01   (501) staff       (20)     6096 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/k_nearest.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.092209 pyranges1-0.1.0/tests/unit/new_position/
--rw-r--r--   0 endbak01   (501) staff       (20)      456 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/new_position/test_new_position.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.143440 pyranges1-0.1.0/tests/unit/out/
--rw-r--r--   0 endbak01   (501) staff       (20)      827 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/out/test_out.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.162281 pyranges1-0.1.0/tests/unit/spliced_subsequence/
--rw-r--r--   0 endbak01   (501) staff       (20)     2293 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/spliced_subsequence/test_spliced_subsequence.py
--rw-r--r--   0 endbak01   (501) staff       (20)      282 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/statistics.py
--rw-r--r--   0 endbak01   (501) staff       (20)      784 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/test_concat.py
--rw-r--r--   0 endbak01   (501) staff       (20)     1542 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/test_count_overlaps.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.292204 pyranges1-0.1.0/tests/unit/test_data/
--rw-r--r--   0 endbak01   (501) staff       (20)     4399 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/test_data/ensembl.gtf
--rw-r--r--   0 endbak01   (501) staff       (20)    71593 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/test_data/test_sorted.bam
--rw-r--r--   0 endbak01   (501) staff       (20)  1706448 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/test_data/test_sorted.bam.bai
--rw-r--r--   0 endbak01   (501) staff       (20)     1456 2024-05-01 07:23:12.000000 pyranges1-0.1.0/tests/unit/test_guessers.py
--rw-r--r--   0 endbak01   (501) staff       (20)     2090 2024-05-01 07:23:13.000000 pyranges1-0.1.0/tests/unit/test_join.py
--rw-r--r--   0 endbak01   (501) staff       (20)     6641 2024-05-01 07:23:13.000000 pyranges1-0.1.0/tests/unit/test_pandas_overrides.py
--rw-r--r--   0 endbak01   (501) staff       (20)      395 2024-05-01 07:23:13.000000 pyranges1-0.1.0/tests/unit/test_tostring.py
-drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:55:56.300595 pyranges1-0.1.0/tests/unit/unit/
--rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:13.000000 pyranges1-0.1.0/tests/unit/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.879408 pyranges1-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.847409 pyranges1-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.851409 pyranges1-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.github/workflows/all_checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.github/workflows/build_the_book.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.github/workflows/build_wheels_and_upload_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.github/workflows/hypothesis_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 12:11:38.000000 pyranges1-0.1.1/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 12:11:38.000000 pyranges1-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-01 12:11:43.879408 pyranges1-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-01 12:11:38.000000 pyranges1-0.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-01 12:11:38.000000 pyranges1-0.1.1/check_typing_linting_and_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-01 12:11:38.000000 pyranges1-0.1.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.855409 pyranges1-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/extension_orfs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/extension_seqs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/extension_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_columns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15830 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    33827 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_genomic_ops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_pages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_rows.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_sequences.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_write.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/pyranges_extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/pyranges_module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/pyranges_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/range_frame.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/todos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    46812 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.859408 pyranges1-0.1.1/pyranges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.859408 pyranges1-0.1.1/pyranges/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/loci_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/multioverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/pyranges_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/pyranges_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   213034 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/pyranges_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/tostring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.863409 pyranges1-0.1.1/pyranges/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/aorta.bed
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/aorta2.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   309369 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/chipseq.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   309045 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/chipseq_background.bed
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/chromsizes.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/cpg.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ensembl.gtf
+-rw-r--r--   0 runner    (1001) docker     (127)    35943 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ensembl_human.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    64417 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/exons.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/f1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/f2.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    81253 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/gencode_human.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    55608 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/lamina.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   387402 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ncbi.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ncbi.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ncbi.gff.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/smaller.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    62555 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ucsc_human.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/docs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.863409 pyranges1-0.1.1/pyranges/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/ext/orfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/ext/seqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27439 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/ext/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.867409 pyranges1-0.1.1/pyranges/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/combine_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/itergrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/max_disjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/merge_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/nearest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/spliced_subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/tile_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/to_rle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/orfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.867409 pyranges1-0.1.1/pyranges/range_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/range_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/range_frame/range_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/range_frame/range_frame_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/seqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/pyranges1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:11:43.879408 pyranges1-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-01 12:11:38.000000 pyranges1-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/.fuse_hidden0000017200000002
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/hi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/property_based/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/hypothesis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17767 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/test_do_not_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/run_doctest_tutorial_howto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/test_calculate_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/test_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/chip_10.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/f1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/f2.bed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/unit/getitem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/getitem/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/hi
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/k_nearest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/unit/new_position/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/new_position/test_new_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/tests/unit/out/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/out/test_out.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/tests/unit/spliced_subsequence/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/spliced_subsequence/test_spliced_subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_count_overlaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/tests/unit/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_data/ensembl.gtf
+-rw-r--r--   0 runner    (1001) docker     (127)    71593 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_data/test_sorted.bam
+-rw-r--r--   0 runner    (1001) docker     (127)  1706448 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_data/test_sorted.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_guessers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_pandas_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_tostring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/tests/unit/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/unit/__init__.py
```

### Comparing `pyranges1-0.1.0/.github/workflows/build-book.yml` & `pyranges1-0.1.1/.github/workflows/build_the_book.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/.github/workflows/build_and_upload_wheels.yml` & `pyranges1-0.1.1/.github/workflows/build_wheels_and_upload_to_pypi.yml`

 * *Files 17% similar despite different names*

```diff
@@ -25,11 +25,11 @@
           path: dist/*
 
       - name: Check metadata
         run: pipx run twine check dist/*
 
       - uses: pypa/gh-action-pypi-publish@v1.5.0
         with:
-          user: ${{ secrets.PYPI_USER }}
-          password: ${{ secrets.PYPI_PROD_PASSWORD }}
+          user: ${{ secrets.PYRANGES_1_PYPI_USER }}
+          password: ${{ secrets.PYRANGES_1_PYPI_PASSWORD }}
           verbose: true
           # To test: repository_url: https://test.pypi.org/legacy/
```

### Comparing `pyranges1-0.1.0/.github/workflows/check.yml` & `pyranges1-0.1.1/.github/workflows/all_checks.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/.github/workflows/run_hypothesis_tests.yml` & `pyranges1-0.1.1/.github/workflows/hypothesis_tests.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/LICENSE` & `pyranges1-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/PKG-INFO` & `pyranges1-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyranges1
-Version: 0.1.0
+Version: 0.1.1
 Summary: GenomicRanges for Python.
 Author-email: Endre Bakken Stovner <endbak@pm.me>
 License: MIT
 Project-URL: Homepage, http://github.com/pyranges/pyranges_1.x
 Keywords: bioinformatics,genomicranges,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
@@ -49,17 +49,19 @@
 Requires-Dist: pyranges[dev]; extra == "all"
 Requires-Dist: pyranges[docs]; extra == "all"
 
 # pyranges
 
 [![Coverage Status](https://img.shields.io/coveralls/github/biocore-ntnu/pyranges.svg)](https://coveralls.io/github/biocore-ntnu/pyranges?branch=master) [![hypothesis tested](graphs/hypothesis-tested-brightgreen.svg)](http://hypothesis.readthedocs.io/) [![PyPI version](https://badge.fury.io/py/pyranges.svg)](https://badge.fury.io/py/pyranges) [![MIT](https://img.shields.io/pypi/l/pyranges.svg?color=green)](https://opensource.org/licenses/MIT) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyranges.svg) [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pyranges/README.html)
 
-## Missing:
+## Install
 
-- to_bigwig: needs a rewrite of the pyrle module
+```bash
+pip install pyranges1
+```
 
 ## Introduction
 
 PyRanges is a Python library specifically designed for efficient and intuitive manipulation of genomics data,
 particularly genomic intervals (like genes, genomic features, or reads).
 The library is optimized for fast querying and manipulation of genomic annotations.
```

### Comparing `pyranges1-0.1.0/README.md` & `pyranges1-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # pyranges
 
 [![Coverage Status](https://img.shields.io/coveralls/github/biocore-ntnu/pyranges.svg)](https://coveralls.io/github/biocore-ntnu/pyranges?branch=master) [![hypothesis tested](graphs/hypothesis-tested-brightgreen.svg)](http://hypothesis.readthedocs.io/) [![PyPI version](https://badge.fury.io/py/pyranges.svg)](https://badge.fury.io/py/pyranges) [![MIT](https://img.shields.io/pypi/l/pyranges.svg?color=green)](https://opensource.org/licenses/MIT) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyranges.svg) [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pyranges/README.html)
 
-## Missing:
+## Install
 
-- to_bigwig: needs a rewrite of the pyrle module
+```bash
+pip install pyranges1
+```
 
 ## Introduction
 
 PyRanges is a Python library specifically designed for efficient and intuitive manipulation of genomics data,
 particularly genomic intervals (like genes, genomic features, or reads).
 The library is optimized for fast querying and manipulation of genomic annotations.
```

### Comparing `pyranges1-0.1.0/check_typing_linting_and_formatting.py` & `pyranges1-0.1.1/check_typing_linting_and_formatting.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/conftest.py` & `pyranges1-0.1.1/conftest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/Makefile` & `pyranges1-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/api_reference.rst` & `pyranges1-0.1.1/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/conf.py` & `pyranges1-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/developer_guide.rst` & `pyranges1-0.1.1/docs/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/how_to_columns.rst` & `pyranges1-0.1.1/docs/how_to_columns.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/how_to_create.rst` & `pyranges1-0.1.1/docs/how_to_create.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/how_to_genomic_ops.rst` & `pyranges1-0.1.1/docs/how_to_genomic_ops.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/how_to_inspect.rst` & `pyranges1-0.1.1/docs/how_to_inspect.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/how_to_rows.rst` & `pyranges1-0.1.1/docs/how_to_rows.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/how_to_sequences.rst` & `pyranges1-0.1.1/docs/how_to_sequences.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/how_to_write.rst` & `pyranges1-0.1.1/docs/how_to_write.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/index.rst` & `pyranges1-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/installation.rst` & `pyranges1-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/make.bat` & `pyranges1-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/pyranges_module.rst` & `pyranges1-0.1.1/docs/pyranges_module.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/todos.rst` & `pyranges1-0.1.1/docs/todos.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/docs/tutorial.rst` & `pyranges1-0.1.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyproject.toml` & `pyranges1-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "cython", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyranges1"
-version = "0.1.0"
+version = "0.1.1"
 description = "GenomicRanges for Python."
 requires-python = ">=3.11.0"
 readme = "README.md"
 authors = [{ name = "Endre Bakken Stovner", email = "endbak@pm.me" }]
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `pyranges1-0.1.0/pyranges/__init__.py` & `pyranges1-0.1.1/pyranges/__init__.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/empty.py` & `pyranges1-0.1.1/pyranges/core/empty.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/example_data.py` & `pyranges1-0.1.1/pyranges/core/example_data.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/loci_getter.py` & `pyranges1-0.1.1/pyranges/core/loci_getter.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/multioverlap.py` & `pyranges1-0.1.1/pyranges/core/multioverlap.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/names.py` & `pyranges1-0.1.1/pyranges/core/names.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/options.py` & `pyranges1-0.1.1/pyranges/core/options.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/out.py` & `pyranges1-0.1.1/pyranges/core/out.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/parallelism.py` & `pyranges1-0.1.1/pyranges/core/parallelism.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/pyranges_groupby.py` & `pyranges1-0.1.1/pyranges/core/pyranges_groupby.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/pyranges_helpers.py` & `pyranges1-0.1.1/pyranges/core/pyranges_helpers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/pyranges_main.py` & `pyranges1-0.1.1/pyranges/core/pyranges_main.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/random.py` & `pyranges1-0.1.1/pyranges/core/random.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/tostring.py` & `pyranges1-0.1.1/pyranges/core/tostring.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/core/version.py` & `pyranges1-0.1.1/pyranges/core/version.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/chipseq.bed` & `pyranges1-0.1.1/pyranges/data/chipseq.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/chipseq_background.bed` & `pyranges1-0.1.1/pyranges/data/chipseq_background.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/cpg.bed` & `pyranges1-0.1.1/pyranges/data/cpg.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/ensembl.gtf` & `pyranges1-0.1.1/pyranges/data/ensembl.gtf`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/ensembl_human.gtf.gz` & `pyranges1-0.1.1/pyranges/data/ensembl_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/exons.bed` & `pyranges1-0.1.1/pyranges/data/exons.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/gencode_human.gtf.gz` & `pyranges1-0.1.1/pyranges/data/gencode_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/lamina.bed` & `pyranges1-0.1.1/pyranges/data/lamina.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/ncbi.fasta` & `pyranges1-0.1.1/pyranges/data/ncbi.fasta`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/ncbi.gff.gz` & `pyranges1-0.1.1/pyranges/data/ncbi.gff.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/smaller.bam` & `pyranges1-0.1.1/pyranges/data/smaller.bam`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/data/ucsc_human.bed.gz` & `pyranges1-0.1.1/pyranges/data/ucsc_human.bed.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/ext/orfs.py` & `pyranges1-0.1.1/pyranges/ext/orfs.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/ext/seqs.py` & `pyranges1-0.1.1/pyranges/ext/seqs.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/ext/stats.py` & `pyranges1-0.1.1/pyranges/ext/stats.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/boundaries.py` & `pyranges1-0.1.1/pyranges/methods/boundaries.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/cluster.py` & `pyranges1-0.1.1/pyranges/methods/cluster.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/combine_positions.py` & `pyranges1-0.1.1/pyranges/methods/combine_positions.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/concat.py` & `pyranges1-0.1.1/pyranges/methods/concat.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/coverage.py` & `pyranges1-0.1.1/pyranges/methods/coverage.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/join.py` & `pyranges1-0.1.1/pyranges/methods/join.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/merge.py` & `pyranges1-0.1.1/pyranges/methods/merge.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/nearest.py` & `pyranges1-0.1.1/pyranges/methods/nearest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/overlap.py` & `pyranges1-0.1.1/pyranges/methods/overlap.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/spliced_subsequence.py` & `pyranges1-0.1.1/pyranges/methods/spliced_subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/split.py` & `pyranges1-0.1.1/pyranges/methods/split.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/statistics.py` & `pyranges1-0.1.1/pyranges/methods/statistics.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/subsequence.py` & `pyranges1-0.1.1/pyranges/methods/subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/subtraction.py` & `pyranges1-0.1.1/pyranges/methods/subtraction.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/summary.py` & `pyranges1-0.1.1/pyranges/methods/summary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/tile_genome.py` & `pyranges1-0.1.1/pyranges/methods/tile_genome.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/to_rle.py` & `pyranges1-0.1.1/pyranges/methods/to_rle.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/methods/windows.py` & `pyranges1-0.1.1/pyranges/methods/windows.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/range_frame/range_frame.py` & `pyranges1-0.1.1/pyranges/range_frame/range_frame.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/range_frame/range_frame_validator.py` & `pyranges1-0.1.1/pyranges/range_frame/range_frame_validator.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges/readers.py` & `pyranges1-0.1.1/pyranges/readers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/pyranges1.egg-info/PKG-INFO` & `pyranges1-0.1.1/pyranges1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyranges1
-Version: 0.1.0
+Version: 0.1.1
 Summary: GenomicRanges for Python.
 Author-email: Endre Bakken Stovner <endbak@pm.me>
 License: MIT
 Project-URL: Homepage, http://github.com/pyranges/pyranges_1.x
 Keywords: bioinformatics,genomicranges,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
@@ -49,17 +49,19 @@
 Requires-Dist: pyranges[dev]; extra == "all"
 Requires-Dist: pyranges[docs]; extra == "all"
 
 # pyranges
 
 [![Coverage Status](https://img.shields.io/coveralls/github/biocore-ntnu/pyranges.svg)](https://coveralls.io/github/biocore-ntnu/pyranges?branch=master) [![hypothesis tested](graphs/hypothesis-tested-brightgreen.svg)](http://hypothesis.readthedocs.io/) [![PyPI version](https://badge.fury.io/py/pyranges.svg)](https://badge.fury.io/py/pyranges) [![MIT](https://img.shields.io/pypi/l/pyranges.svg?color=green)](https://opensource.org/licenses/MIT) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyranges.svg) [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pyranges/README.html)
 
-## Missing:
+## Install
 
-- to_bigwig: needs a rewrite of the pyrle module
+```bash
+pip install pyranges1
+```
 
 ## Introduction
 
 PyRanges is a Python library specifically designed for efficient and intuitive manipulation of genomics data,
 particularly genomic intervals (like genes, genomic features, or reads).
 The library is optimized for fast querying and manipulation of genomic annotations.
```

### Comparing `pyranges1-0.1.0/pyranges1.egg-info/SOURCES.txt` & `pyranges1-0.1.1/pyranges1.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 CHANGELOG.txt
 LICENSE
 README.md
 check_typing_linting_and_formatting.py
 conftest.py
 pyproject.toml
 setup.py
-.github/workflows/build-book.yml
-.github/workflows/build_and_upload_wheels.yml
-.github/workflows/check.yml
-.github/workflows/run_hypothesis_tests.yml
+.github/workflows/all_checks.yml
+.github/workflows/build_the_book.yml
+.github/workflows/build_wheels_and_upload_to_pypi.yml
+.github/workflows/hypothesis_tests.yml
 docs/Makefile
 docs/api_reference.rst
 docs/conf.py
 docs/developer_guide.rst
 docs/extension_orfs.rst
 docs/extension_seqs.rst
 docs/extension_stats.rst
```

### Comparing `pyranges1-0.1.0/tests/.fuse_hidden0000017200000002` & `pyranges1-0.1.1/tests/.fuse_hidden0000017200000002`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/helpers.py` & `pyranges1-0.1.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/hi` & `pyranges1-0.1.1/tests/hi`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/property_based/hypothesis_helper.py` & `pyranges1-0.1.1/tests/property_based/hypothesis_helper.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/property_based/new.py` & `pyranges1-0.1.1/tests/property_based/new.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/property_based/test_binary.py` & `pyranges1-0.1.1/tests/property_based/test_binary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/property_based/test_do_not_error.py` & `pyranges1-0.1.1/tests/property_based/test_do_not_error.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/property_based/test_unary.py` & `pyranges1-0.1.1/tests/property_based/test_unary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/test_parallelism.py` & `pyranges1-0.1.1/tests/test_parallelism.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/chip_10.bed` & `pyranges1-0.1.1/tests/unit/chip_10.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/conftest.py` & `pyranges1-0.1.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/hi` & `pyranges1-0.1.1/tests/unit/hi`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/k_nearest.py` & `pyranges1-0.1.1/tests/unit/k_nearest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/out/test_out.py` & `pyranges1-0.1.1/tests/unit/out/test_out.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/spliced_subsequence/test_spliced_subsequence.py` & `pyranges1-0.1.1/tests/unit/spliced_subsequence/test_spliced_subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/test_concat.py` & `pyranges1-0.1.1/tests/unit/test_concat.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/test_count_overlaps.py` & `pyranges1-0.1.1/tests/unit/test_count_overlaps.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/test_data/ensembl.gtf` & `pyranges1-0.1.1/tests/unit/test_data/ensembl.gtf`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/test_data/test_sorted.bam` & `pyranges1-0.1.1/tests/unit/test_data/test_sorted.bam`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/test_data/test_sorted.bam.bai` & `pyranges1-0.1.1/tests/unit/test_data/test_sorted.bam.bai`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/test_guessers.py` & `pyranges1-0.1.1/tests/unit/test_guessers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/test_join.py` & `pyranges1-0.1.1/tests/unit/test_join.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.0/tests/unit/test_pandas_overrides.py` & `pyranges1-0.1.1/tests/unit/test_pandas_overrides.py`

 * *Files identical despite different names*


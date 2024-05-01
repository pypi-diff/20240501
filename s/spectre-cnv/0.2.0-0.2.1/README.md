# Comparing `tmp/spectre-cnv-0.2.0.tar.gz` & `tmp/spectre_cnv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectre-cnv-0.2.0.tar", last modified: Mon Mar 18 22:19:50 2024, max compression
+gzip compressed data, was "spectre_cnv-0.2.1.tar", last modified: Wed May  1 13:59:08 2024, max compression
```

## Comparing `spectre-cnv-0.2.0.tar` & `spectre_cnv-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.318524 spectre-cnv-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-03-18 22:19:50.318524 spectre-cnv-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-18 22:19:50.318524 spectre-cnv-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.310524 spectre-cnv-0.2.0/spectre/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.314524 spectre-cnv-0.2.0/spectre/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43950 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/breakpoint_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/call_cnv_AF.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/call_cnv_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/cnv_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/cnv_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/coverage_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    27584 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/analysis/snv_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.314524 spectre-cnv-0.2.0/spectre/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/classes/cnv_candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/classes/loh_candidate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.314524 spectre-cnv-0.2.0/spectre/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.314524 spectre-cnv-0.2.0/spectre/libs/unidip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/libs/unidip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/libs/unidip/dip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/libs/unidip/unidip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.314524 spectre-cnv-0.2.0/spectre/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/plots/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    34432 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/spectre.py
--rw-r--r--   0 runner    (1001) docker     (127)     7177 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/spectreCNV.py
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/spectreCNVPopulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.318524 spectre-cnv-0.2.0/spectre/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/OSUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/cnv_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/dataAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.318524 spectre-cnv-0.2.0/spectre/util/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/metadata/metadataCollector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/mosdepthReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/outputWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/timing_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)    12342 2024-03-18 22:19:41.000000 spectre-cnv-0.2.0/spectre/util/vcf_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:19:50.318524 spectre-cnv-0.2.0/spectre_cnv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-03-18 22:19:50.000000 spectre-cnv-0.2.0/spectre_cnv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-18 22:19:50.000000 spectre-cnv-0.2.0/spectre_cnv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 22:19:50.000000 spectre-cnv-0.2.0/spectre_cnv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-18 22:19:50.000000 spectre-cnv-0.2.0/spectre_cnv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-18 22:19:50.000000 spectre-cnv-0.2.0/spectre_cnv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-18 22:19:50.000000 spectre-cnv-0.2.0/spectre_cnv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.050674 spectre_cnv-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-01 13:59:08.050674 spectre_cnv-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-01 13:59:08.050674 spectre_cnv-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.042674 spectre_cnv-0.2.1/spectre/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.046674 spectre_cnv-0.2.1/spectre/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45786 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/breakpoint_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/call_cnv_AF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/call_cnv_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28745 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/cnv_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/cnv_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/coverage_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/analysis/snv_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.046674 spectre_cnv-0.2.1/spectre/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/classes/cnv_candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/classes/loh_candidate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.046674 spectre_cnv-0.2.1/spectre/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.046674 spectre_cnv-0.2.1/spectre/libs/unidip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/libs/unidip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/libs/unidip/dip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/libs/unidip/unidip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.046674 spectre_cnv-0.2.1/spectre/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/plots/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37004 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/spectre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/spectreCNV.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29283 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/spectreCNVPopulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.050674 spectre_cnv-0.2.1/spectre/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/OSUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/cnv_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/dataAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.050674 spectre_cnv-0.2.1/spectre/util/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/metadata/metadataCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/mosdepthReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13502 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/outputWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/timing_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-05-01 13:59:04.000000 spectre_cnv-0.2.1/spectre/util/vcf_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:59:08.050674 spectre_cnv-0.2.1/spectre_cnv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-01 13:59:08.000000 spectre_cnv-0.2.1/spectre_cnv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 13:59:08.000000 spectre_cnv-0.2.1/spectre_cnv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:59:08.000000 spectre_cnv-0.2.1/spectre_cnv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 13:59:08.000000 spectre_cnv-0.2.1/spectre_cnv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 13:59:08.000000 spectre_cnv-0.2.1/spectre_cnv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 13:59:08.000000 spectre_cnv-0.2.1/spectre_cnv.egg-info/top_level.txt
```

### Comparing `spectre-cnv-0.2.0/LICENSE` & `spectre_cnv-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/LICENSE.md` & `spectre_cnv-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/PKG-INFO` & `spectre_cnv-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: spectre-cnv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Long read copy number variation (CNV) caller
 Home-page: https://github.com/fritzsedlazeck/Spectre
 Author: Philippe Sanio
 Author-email: philippe.sanio@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
-Requires-Dist: pysam==0.22.0
-Requires-Dist: numpy==1.24.3
-Requires-Dist: pandas==2.0.1
-Requires-Dist: matplotlib==3.7.1
-Requires-Dist: scipy==1.10.1
+Requires-Dist: pysam>=0.22.0
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: pandas>=2.0.1
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: scipy>=1.10.1
 
 
 ![Spectre](./logo.png)
 # Spectre - Long read CNV caller
 Spectre is a long read copy number variation (CNV) caller. 
 Spectre is designed to detect large CNVs (>100kb) in a couple of minutes depending on your hardware.
 
@@ -26,20 +26,29 @@
 Additionally, Spectre can use the breakpoint (SNF) data from Sniffles to improve the CNV calling. However, it has to be converted to the SNFJ format using [snf2json](https://github.com/philippesanio/snf2json).
 
 
 The CNV output of Spectre is stored in three files, VCF, BED and .SPC which can be used in the population mode.
 
 Furthermore, Spectre offers a population mode, which can be used to search for CNV support in multiple samples. 
 Compared to other tools, Spectre searches not only in the final CNVs but also in CNV candidates which did not qualify for the final output of Spectre.
-## Required programs (conda)
+## Install Spectre
+Tested on **Python** version: **3.11** and **3.10**
 
 Install Spectre with Pip:
 ```bash
 pip install spectre-cnv
 ```
+Get the latest changes by building Spectre from source on your own and install it locally in your conda environment.
+```bash
+pip install build
+git clone https://github.com/fritzsedlazeck/Spectre.git
+cd ./Spectre
+python3 -m build
+pip install dist/spectre_cnv-<VERSION>.tar.gz # replace <VERSION> with e.g. 0.2.0
+```
 
 Setup a conda environment for Spectre (copy and paste the following commands)
 ```bash
 conda create -n spectre python=3.10 pysam==0.22.0 numpy==1.24.3 pandas==2.0.1 matplotlib==3.7.1 scipy==1.10.1 -y
 conda activate spectre
 ```
 Alternatively, you can use pip for installing the packages stored in the requirements txt
@@ -79,14 +88,15 @@
 - Reference genome (can be bgzip compressed)
 
 Optional
 - **MDR** file (if not already generated, Spectre will do that for you. You can also use the MDR file for every sample which has been aligned to the same reference genome)
 - VCF file containing SNV
 - SNF data from Sniffles (if parsed through [snf2json](https://github.com/philippesanio/snf2json))
 
+
 ## Run Spectre
 ### MDR file
 MDR files hold the information of N regions in the reference genome and restrict Spectre of using data from those regions. 
 We are providing sample MDR files for the reference genomes GRCh37 and GRCh38.
 
 If not provided, Spectre will generate a MDR file for you, which can take some time. 
 Thus, we highly recommend to generate a MDR file for your reference genome before running Spectre on multiple samples which have been aligned to the same reference.
@@ -112,22 +122,25 @@
   --coverage mosdepth/sampleid/mosdepth.regions.bed.gz \
   --sample-id sampleid \
   --output-dir sampleid_output_directory_path/ \
   --reference reference.fasta.gz
 ```
 ### Run Spectre with multiple samples
 Run Spectre with multiple samples:
->INFO: This will start the population mode automatically.
+>INFO: This will start the population mode automatically. All provided settings will be applied to all samples.
+
+>NOTE: If population flag is not set, Spectre will run in single sample mode. Thus, calculating only CNVs for the first sample. 
 
 ```bash
 spectre.py CNVCaller \
   --coverage mosdepth/sampleid-1/mosdepth.regions.bed.gz mosdepth/sampleid-2/mosdepth.regions.bed.gz \
   --sample-id sampleid-1 sampleid-2 \
   --output-dir sampleid_output_directory_path/ \
   --reference reference.fasta.gz
+  --population
 ```
 
 ### Population mode
 Run Spectre in population mode with two or more samples:
 >INFO: Spectre produces an intermediate file (.spc) which contains all calculated CNVs from a given samples. They are 
 > located in the output folder of given sample.
 
@@ -137,67 +150,79 @@
   --sample-id output_name \
   --output-dir sampleid_output_directory_path/
 ```
 
 
 ### Help
 ```
-Spectre:
+vcf_utils <command> [<args>]
+    Spectre:
         CNVCaller:
-            Required
+            [Required]
                 --coverage     Path to the coverage file from Mosdepth output. Expects the following files:
                                    <prefix>.regions.bed.gz
                                    <prefix>.regions.bed.gz.csi
-                               Can be one or more directories. Example:
+                               Can be one or more paths. However, providing multiple samples is only intended to
+                               work with the --population flag. Example:
                                     --coverage /path/md1.regions.gz /path/md2.regions.gz
-                --sample-id    Sample name/ID. Can be one or more ID. Example:
+                --sample-id    Sample name/ID. Can be one or more ID. However, providing multiple sample ids is only
+                               intended to work with the --population flag. Example:
                                     --sample-id id1 id2
                 --output-dir   Output directory
                 --reference    Reference sequence used for mapping (for N removal)
-            Optional, if missing it will be created
-                --metadata     Metadata file for Ns removal
-            Optional
+            [Optional, if missing it will be created]
+                --metadata     Metadata file for Ns removal (this will speed up Spectre massively if provided)
+                --n-size       Required amount of consecutive Ns to be considered an NRegion 
+                               in the reference sequence (Default = 5)
+
+            [Optional]
                 --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
-                --only-chr     Comma separated list of chromosomes to use
+                --only-chr     Comma separated list of chromosomes to use (e.g. chr1,chr2,chr3)
                 --ploidy       Set the ploidy for the analysis, useful for sex chromosomes (Default = 2)
                 --ploidy-chr   Comma separated list of key:value-pairs for individual chromosome ploidy control
                                (e.g. chrX:2,chrY:1) If chromosome is not specified, the default ploidy will be used.
-                --snv          VCF file containing the SNV for the same sample CNV want to be called
                 --snfj         Breakpoints from from Sniffle which has been converted from the SNF to the SNFJ format.
-                --n-size       Length of consecutive Ns (Default = 5)
+                               SNFJ files can be generated using the program snf2json.
                 --min-cnv-len  Minimum length of CNV (Default 100kb)
-                --cancer       Set this flag if the sample is cancer (Default = False)
-                --population   Runs the population mode on all provided samples
-                --threads      Amount of threads (This will boost performance if multiple samples are provided)
+                --snv          VCF file containing the SNV for the same sample CNV want to be called
+                --cancer       Set this flag if the sample is cancer (Default = False) This will disable some safety 
+                               checks, when determining the DEL and DUP thresholds. 
 
-                Coverage
+            [Optional, Coverage]
                 --sample-coverage-overwrite     Overwrites the calculated sample coverage, which is used to normalize
                                                 the coverage. e.g. a value of 30 equals to 30X coverage.
                 --disable-max-coverage          Disables the maximum coverage check. This will allow to call CNVs
 
-                LoH (requires --snv)
+            [Optional, LoH (requires --snv)]
                 --loh-min-snv-perkb             Minimum number of SNVs per kilobase for an LoH region (default=5)
                 --loh-min-snv-total             Minimum number of SNVs total for an LoH region (default=100)
                 --loh-min-region-size           Minimum size of a region for a LoH region (default=100000)
 
-
+                --population   Runs the population mode on all provided samples. It will apply all the provided
+                               configurations as well as the default population mode values to all samples.
+                --threads      Amount of threads (This will boost performance if multiple samples are provided)
         RemoveNs:
-            Required
+            [Required]
                 --reference    Reference genome used for mapping
                 --output-dir   Output dir
                 --output-file  Output file for results
-                --bin-size     Bin/Window size (same as Mosdepth)
-            Optional
-                --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
-                --n-size       Length of consecutive Ns (Default = 5)
-                --save-only    Will only save the metadata file and not show the results in screen (Default = False)
+            [Optional]
+                --n-size       Required amount of consecutive Ns to be considered an NRegion 
+                               in the reference sequence (Default = 5)
+                --save-only    Will only save the metadata file and not show the results on screen (Default = False)
 
         Population:
-            Required
-                --candidates   At least 2 candidate files (.spc or .vcf) which should be taken into consideration for the population mode.
-                --sample-id    Name of the output file
-                --output-dir   Output directory
-            Optional
-                --reference    Reference sequence (Required if VCF files are used!)
+            [Required]
+                --candidates   At least 2 .spc sample files which should be used in the population mode.
+                               (e.g. sample1.spc sample2.spc)
+                --sample-id    The name of the sample-id will be added accordingly at the output.
+                               (e.g. population_mode_<sample-id>.vcf.gz)
+                --output-dir   Path of the output directory
+            [Optional]
+                --reference    Reference sequence
+                --reciprocal-overlap        Minimum reciprocal overlap for supporting CNVs [0.0 - 1.0] (Default = 0.8)
+                --disable-quality-filter    Disables the quality filter for the population mode. Spectre will also
+                                            search for supporting CNVs in the .SPC files, which have not been reported
+                                            as final CNVs in the VCF and BED file.
         Version:
             version    Shows current version/build
 ```
```

### Comparing `spectre-cnv-0.2.0/README.md` & `spectre_cnv-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,29 @@
 Additionally, Spectre can use the breakpoint (SNF) data from Sniffles to improve the CNV calling. However, it has to be converted to the SNFJ format using [snf2json](https://github.com/philippesanio/snf2json).
 
 
 The CNV output of Spectre is stored in three files, VCF, BED and .SPC which can be used in the population mode.
 
 Furthermore, Spectre offers a population mode, which can be used to search for CNV support in multiple samples. 
 Compared to other tools, Spectre searches not only in the final CNVs but also in CNV candidates which did not qualify for the final output of Spectre.
-## Required programs (conda)
+## Install Spectre
+Tested on **Python** version: **3.11** and **3.10**
 
 Install Spectre with Pip:
 ```bash
 pip install spectre-cnv
 ```
+Get the latest changes by building Spectre from source on your own and install it locally in your conda environment.
+```bash
+pip install build
+git clone https://github.com/fritzsedlazeck/Spectre.git
+cd ./Spectre
+python3 -m build
+pip install dist/spectre_cnv-<VERSION>.tar.gz # replace <VERSION> with e.g. 0.2.0
+```
 
 Setup a conda environment for Spectre (copy and paste the following commands)
 ```bash
 conda create -n spectre python=3.10 pysam==0.22.0 numpy==1.24.3 pandas==2.0.1 matplotlib==3.7.1 scipy==1.10.1 -y
 conda activate spectre
 ```
 Alternatively, you can use pip for installing the packages stored in the requirements txt
@@ -62,14 +71,15 @@
 - Reference genome (can be bgzip compressed)
 
 Optional
 - **MDR** file (if not already generated, Spectre will do that for you. You can also use the MDR file for every sample which has been aligned to the same reference genome)
 - VCF file containing SNV
 - SNF data from Sniffles (if parsed through [snf2json](https://github.com/philippesanio/snf2json))
 
+
 ## Run Spectre
 ### MDR file
 MDR files hold the information of N regions in the reference genome and restrict Spectre of using data from those regions. 
 We are providing sample MDR files for the reference genomes GRCh37 and GRCh38.
 
 If not provided, Spectre will generate a MDR file for you, which can take some time. 
 Thus, we highly recommend to generate a MDR file for your reference genome before running Spectre on multiple samples which have been aligned to the same reference.
@@ -95,22 +105,25 @@
   --coverage mosdepth/sampleid/mosdepth.regions.bed.gz \
   --sample-id sampleid \
   --output-dir sampleid_output_directory_path/ \
   --reference reference.fasta.gz
 ```
 ### Run Spectre with multiple samples
 Run Spectre with multiple samples:
->INFO: This will start the population mode automatically.
+>INFO: This will start the population mode automatically. All provided settings will be applied to all samples.
+
+>NOTE: If population flag is not set, Spectre will run in single sample mode. Thus, calculating only CNVs for the first sample. 
 
 ```bash
 spectre.py CNVCaller \
   --coverage mosdepth/sampleid-1/mosdepth.regions.bed.gz mosdepth/sampleid-2/mosdepth.regions.bed.gz \
   --sample-id sampleid-1 sampleid-2 \
   --output-dir sampleid_output_directory_path/ \
   --reference reference.fasta.gz
+  --population
 ```
 
 ### Population mode
 Run Spectre in population mode with two or more samples:
 >INFO: Spectre produces an intermediate file (.spc) which contains all calculated CNVs from a given samples. They are 
 > located in the output folder of given sample.
 
@@ -120,67 +133,79 @@
   --sample-id output_name \
   --output-dir sampleid_output_directory_path/
 ```
 
 
 ### Help
 ```
-Spectre:
+vcf_utils <command> [<args>]
+    Spectre:
         CNVCaller:
-            Required
+            [Required]
                 --coverage     Path to the coverage file from Mosdepth output. Expects the following files:
                                    <prefix>.regions.bed.gz
                                    <prefix>.regions.bed.gz.csi
-                               Can be one or more directories. Example:
+                               Can be one or more paths. However, providing multiple samples is only intended to
+                               work with the --population flag. Example:
                                     --coverage /path/md1.regions.gz /path/md2.regions.gz
-                --sample-id    Sample name/ID. Can be one or more ID. Example:
+                --sample-id    Sample name/ID. Can be one or more ID. However, providing multiple sample ids is only
+                               intended to work with the --population flag. Example:
                                     --sample-id id1 id2
                 --output-dir   Output directory
                 --reference    Reference sequence used for mapping (for N removal)
-            Optional, if missing it will be created
-                --metadata     Metadata file for Ns removal
-            Optional
+            [Optional, if missing it will be created]
+                --metadata     Metadata file for Ns removal (this will speed up Spectre massively if provided)
+                --n-size       Required amount of consecutive Ns to be considered an NRegion 
+                               in the reference sequence (Default = 5)
+
+            [Optional]
                 --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
-                --only-chr     Comma separated list of chromosomes to use
+                --only-chr     Comma separated list of chromosomes to use (e.g. chr1,chr2,chr3)
                 --ploidy       Set the ploidy for the analysis, useful for sex chromosomes (Default = 2)
                 --ploidy-chr   Comma separated list of key:value-pairs for individual chromosome ploidy control
                                (e.g. chrX:2,chrY:1) If chromosome is not specified, the default ploidy will be used.
-                --snv          VCF file containing the SNV for the same sample CNV want to be called
                 --snfj         Breakpoints from from Sniffle which has been converted from the SNF to the SNFJ format.
-                --n-size       Length of consecutive Ns (Default = 5)
+                               SNFJ files can be generated using the program snf2json.
                 --min-cnv-len  Minimum length of CNV (Default 100kb)
-                --cancer       Set this flag if the sample is cancer (Default = False)
-                --population   Runs the population mode on all provided samples
-                --threads      Amount of threads (This will boost performance if multiple samples are provided)
+                --snv          VCF file containing the SNV for the same sample CNV want to be called
+                --cancer       Set this flag if the sample is cancer (Default = False) This will disable some safety 
+                               checks, when determining the DEL and DUP thresholds. 
 
-                Coverage
+            [Optional, Coverage]
                 --sample-coverage-overwrite     Overwrites the calculated sample coverage, which is used to normalize
                                                 the coverage. e.g. a value of 30 equals to 30X coverage.
                 --disable-max-coverage          Disables the maximum coverage check. This will allow to call CNVs
 
-                LoH (requires --snv)
+            [Optional, LoH (requires --snv)]
                 --loh-min-snv-perkb             Minimum number of SNVs per kilobase for an LoH region (default=5)
                 --loh-min-snv-total             Minimum number of SNVs total for an LoH region (default=100)
                 --loh-min-region-size           Minimum size of a region for a LoH region (default=100000)
 
-
+                --population   Runs the population mode on all provided samples. It will apply all the provided
+                               configurations as well as the default population mode values to all samples.
+                --threads      Amount of threads (This will boost performance if multiple samples are provided)
         RemoveNs:
-            Required
+            [Required]
                 --reference    Reference genome used for mapping
                 --output-dir   Output dir
                 --output-file  Output file for results
-                --bin-size     Bin/Window size (same as Mosdepth)
-            Optional
-                --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
-                --n-size       Length of consecutive Ns (Default = 5)
-                --save-only    Will only save the metadata file and not show the results in screen (Default = False)
+            [Optional]
+                --n-size       Required amount of consecutive Ns to be considered an NRegion 
+                               in the reference sequence (Default = 5)
+                --save-only    Will only save the metadata file and not show the results on screen (Default = False)
 
         Population:
-            Required
-                --candidates   At least 2 candidate files (.spc or .vcf) which should be taken into consideration for the population mode.
-                --sample-id    Name of the output file
-                --output-dir   Output directory
-            Optional
-                --reference    Reference sequence (Required if VCF files are used!)
+            [Required]
+                --candidates   At least 2 .spc sample files which should be used in the population mode.
+                               (e.g. sample1.spc sample2.spc)
+                --sample-id    The name of the sample-id will be added accordingly at the output.
+                               (e.g. population_mode_<sample-id>.vcf.gz)
+                --output-dir   Path of the output directory
+            [Optional]
+                --reference    Reference sequence
+                --reciprocal-overlap        Minimum reciprocal overlap for supporting CNVs [0.0 - 1.0] (Default = 0.8)
+                --disable-quality-filter    Disables the quality filter for the population mode. Spectre will also
+                                            search for supporting CNVs in the .SPC files, which have not been reported
+                                            as final CNVs in the VCF and BED file.
         Version:
             version    Shows current version/build
 ```
```

### Comparing `spectre-cnv-0.2.0/setup.cfg` & `spectre_cnv-0.2.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spectre-cnv"
-version = "0.2.0"
+version = "0.2.1"
 author = Philippe Sanio
 author_email = philippe.sanio@gmail.com
 description = "Long read copy number variation (CNV) caller"
 long_description = file: README.md
 long_description_content_type = text/markdown
 readme = "README.md"
 requires-python = ">=3.10"
@@ -12,19 +12,19 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 install_requires = 
-	pysam ==0.22.0,
-	numpy ==1.24.3,
-	pandas ==2.0.1,
-	matplotlib ==3.7.1,
-	scipy ==1.10.1
+	pysam >=0.22.0,
+	numpy >=1.24.3,
+	pandas >=2.0.1,
+	matplotlib >=3.7.1,
+	scipy >=1.10.1
 
 [options.entry_points]
 console_scripts = 
 	spectre = spectre.spectre:main
 
 [project.urls]
 Homepage = "https://github.com/fritzsedlazeck/spectre"
```

### Comparing `spectre-cnv-0.2.0/spectre/analysis/analysis.py` & `spectre_cnv-0.2.1/spectre/analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 
 import numpy as np
 import pandas as pd
 import pysam
 
 from spectre.analysis.breakpoint_analysis import Breakpoints
 from spectre.util import outputWriter
@@ -57,32 +58,52 @@
         self.intermediate_candidates_file_location = ""  # holds output path of serialized cnv object
         self.cnv_merged = {}  # use this for CNV call
         self.existing_cnv_ids = []  # holds all already used cnv IDs
         # cnv metrics
         self.cnv_metrics = None
         # snv data
         self.snv_derived_cn_neutral = None
+        self.snv_loh_raw = None
         self.snv_loh = None
         self.merged_candidates = None
         # output
         self.chromosome_names_out = None
+        # SNFJ
+        self.snfj_breakpoints = False
         # DEV
         self.min_chr_length = 1e6
         self.dist_min_overwrite = 10000  # 10kb TODO
         self.max_std_outlier_rm = self.spectre_args.dev_max_std_outlier_rm  # 5
         self.mosdepth_cov_genome_chr_diff = self.spectre_args.dev_mosdepth_cov_genome_chr_diff  # 0.10  # 10%
         self.lower_2n_threshold = self.spectre_args.dev_lower_2n_threshold  # overwritten after data_normalization call
         self.upper_2n_threshold = self.spectre_args.dev_upper_2n_threshold  # overwritten after data_normalization call
         self.cov_diff_threshold = self.spectre_args.dev_cov_diff_threshold  # 0.80
         self.dist_proportion = self.spectre_args.dev_dist_proportion  # 0.25
         self.candidate_final_threshold = self.spectre_args.min_cnv_len  # min_cnv_len #100000  # 100kb
         self.sample_coverage_overwrite = self.spectre_args.sample_coverage_overwrite  # sample_coverage_overwrite
         # TODO
         self.output_directory = spectre_args.out_dir
 
+    def pre_calculation_check(self):
+        min_cnv_len_check_smaller_threshold = False
+        min_cnv_len_greater_then_minimum = False
+        # check if min-cnv-len is smaller than 100KB
+        if self.spectre_args.min_cnv_len <= self.min_chr_length:
+            self.logger.warning(f"Minimum CNV length is smaller then {int(self.min_chr_length)} base pairs")
+            self.logger.warning(f"Expect trouble!")
+            min_cnv_len_check_smaller_threshold = True
+
+        if self.spectre_args.min_cnv_len <= self.dist_min_overwrite:
+            self.logger.error(f"Minimum CNV length must be greater then {int(self.dist_min_overwrite)} base pairs")
+            min_cnv_len_greater_then_minimum = False
+        else:
+            min_cnv_len_greater_then_minimum = True
+
+        return min_cnv_len_check_smaller_threshold and min_cnv_len_greater_then_minimum
+
     # Data normalization
     def data_normalization(self):
         """
         Normalize single chromosome bins
         """
         self.logger.debug(f'coverage file: {self.coverage_file}')
         if os.stat(self.coverage_file).st_size == 0:
@@ -90,14 +111,19 @@
 
         coverage_file_tabix = pysam.TabixFile(filename=self.coverage_file, index=f'{self.coverage_file}.csi')
 
         tmp_genome_wide_coverage_dict = {}
         tmp_genome_wide_position_dict = {}
         # load coverage data per chromosome
         for reference_chromosome in self.genome_info["chromosomes"]:
+            # Check if the chromosome is in the coverage file
+            if reference_chromosome not in coverage_file_tabix.contigs:
+                self.logger.warning(f"NO coverage data found for chromosome {reference_chromosome}")
+                continue
+
             # init
             tmp_positions = []
             tmp_coverage = []
 
             # load coverage data
             for tbx_line in coverage_file_tabix.fetch(reference_chromosome):
                 [reference_chromosome, start, _, coverage] = tbx_line.split("\t")
@@ -111,20 +137,30 @@
             if self.bin_size == 0:
                 self.bin_size = abs(self.positions[1] - self.positions[0])
                 self.logger.info(f"Determined bin size from Mosdepth coverage: {self.bin_size}")
                 # adjusting metadata according to bin size
                 fm = FastaRef()
                 self.metadata = fm.load_metadata(mdr_file_path=self.metadata_path,
                                                  blacklist_file_path=self.spectre_args.black_list,
-                                                 bin_size=self.bin_size)
+                                                 bin_size=int(self.bin_size))
+
+                if not self.pre_calculation_check():
+                    sys.exit(1)
+
             # remove n regions from coverage
             self.__remove_n_region_by_chromosome(reference_chromosome)
             # add coverage to the genome-wide coverage dict
             tmp_genome_wide_coverage_dict[reference_chromosome] = self.coverage
             tmp_genome_wide_position_dict[reference_chromosome] = self.positions
+        # abort if no coverage data was found across all chromosomes
+        if len(tmp_genome_wide_coverage_dict) == 0:
+            self.logger.error("No coverage data found for any chromosome in the reference sequence!")
+            self.logger.error("Please make sure that the the reference sequence and the coverage file have matching"
+                              " chromosome names.")
+            sys.exit(1)
 
         # Calculate the normalization statistics
         genome_wide_cov_values = [value for chrom_cov_values in tmp_genome_wide_coverage_dict.values() for value in
                                   chrom_cov_values]
 
         # Calculate the median of the values using numpy
         self.genome_wide_median = float(np.nanmedian(genome_wide_cov_values))
@@ -134,17 +170,20 @@
             self.genome_wide_median = self.sample_coverage_overwrite
         self.normalization_value = self.genome_wide_median
         self.genome_std = np.nanstd(genome_wide_cov_values)
 
         # check if the normalization value is within the expected range the range is plus minus 1 genome_std from the
         # normalization value
         if self.snv_derived_cn_neutral is not None:
-            if not (self.normalization_value - self.genome_std < self.snv_derived_cn_neutral["med"] < self.normalization_value + self.genome_std):
-                self.logger.warning(f'The median coverage value between the Mosdepth data and the SNV data are different!')
-                self.logger.warning(f'Coverage: Mosdepth: {self.normalization_value}X. SNV: {self.snv_derived_cn_neutral["med"]}X.')
+            if not (self.normalization_value - self.genome_std < self.snv_derived_cn_neutral[
+                "med"] < self.normalization_value + self.genome_std):
+                self.logger.warning(
+                    f'The median coverage value between the Mosdepth data and the SNV data are different!')
+                self.logger.warning(
+                    f'Coverage: Mosdepth: {self.normalization_value}X. SNV: {self.snv_derived_cn_neutral["med"]}X.')
                 self.logger.warning(f'Expect trouble!')
 
         # Apply normalization to the coverage data
         for reference_chromosome in self.spectre_args.only_chr_list:
             self.coverage = tmp_genome_wide_coverage_dict[reference_chromosome]
             self.positions = tmp_genome_wide_position_dict[reference_chromosome]
             cov_stats, norm_stats, cov_data = self.__normalization_and_statistics(reference_chromosome)
@@ -312,14 +351,15 @@
             cnv_call_list = self.clean_merged_candidates(cnv_call_list, 1.0)
             self.cnv_calls_list[each_chromosome] = cnv_call_list
         pass
 
     def check_snfj_breakpoints(self, snfspc_file):
         bp = Breakpoints(snfspc_file, self.as_dev)
         bp.correlate_cnvs_with_breakpoints(cnv_candidates=self.cnv_calls_list, bin_size=self.bin_size)
+        self.snfj_breakpoints = True
 
     # Candidate CNV merge by distance and CNV type
     def merge_candidates(self, candidates_cnv_list, chromosome_name):
         merged_candidates = []
         if len(candidates_cnv_list) > 1:
             dev_candidates_string = ""
             merge_rounds = 1
@@ -701,15 +741,15 @@
             bed_output_dev = outputWriter.BedOutput(f'{self.debug_dir}/raw-cnvs{self.sample_id}.bed.gz')
             bed_output_dev.make_bed(self.chromosome_names_out, self.raw_cnv_calls_list)
 
     def cnv_result_vcf(self, method=""):
         # TODO add LoH if self.snv_loh is not None
         # TODO modify make_vcf
         output_vcf = os.path.join(os.path.join(self.output_directory, f'{method}{self.sample_id}.vcf.gz'))
-        vcf_output = outputWriter.VCFOutput(output_vcf, self.genome_info)
+        vcf_output = outputWriter.VCFOutput(output_vcf, self.genome_info, self.snfj_breakpoints)
         vcf_output.make_vcf(self.chromosome_names_out, self.merged_candidates, self.sample_id)
 
     # Plots
     def coverage_plot(self):
         for each_chromosome in self.coverage_analysis.keys():
             plot_cnv = CoveragePlot()
             plot_cnv.file_prefix = f'{self.sample_id}_coverage_plot'
@@ -751,17 +791,17 @@
         intermediate_output_writer = outputWriter.IntermediateFile(self.output_directory)
         # genome_info = intermediate_output_writer.convert_candidates_to_dictionary(self.genome_info)
         cnv_calls_list_dict = intermediate_output_writer.convert_candidates_to_dictionary(self.cnv_calls_list)
         raw_cnv_calls_list_dict = intermediate_output_writer.convert_candidates_to_dictionary(self.raw_cnv_calls_list)
 
         # merge loh dict to  cnv calls dict
         if self.cnv_calls_list_af_filtered is not None:
-            loh_raw_cnv_calls_list_dict = intermediate_output_writer.convert_candidates_to_dictionary(self.snv_loh)
+            loh_raw_cnv_calls_list_dict = intermediate_output_writer.convert_candidates_to_dictionary(self.snv_loh_raw)
             loh_cnv_calls_list_dict = intermediate_output_writer.convert_candidates_to_dictionary(
-                self.cnv_calls_list_af_filtered)
+                self.snv_loh)
 
         analysis_dict = {
             "metadata": {"source": "spectre", "spectre_version": "0.2.alpha", "bin_size": int(self.bin_size),
                          "min_cn_len": int(self.candidate_final_threshold),
                          "normalization_value": float(self.normalization_value), "sample_id": self.sample_id},
             "genome_info": self.genome_info,
             "raw_cnvs": raw_cnv_calls_list_dict,
```

### Comparing `spectre-cnv-0.2.0/spectre/analysis/breakpoint_analysis.py` & `spectre_cnv-0.2.1/spectre/analysis/breakpoint_analysis.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/analysis/call_cnv_AF.py` & `spectre_cnv-0.2.1/spectre/analysis/call_cnv_AF.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,31 +68,32 @@
         upper_target_af = ((cn - dr) / cn)  # CN = 3 -> upper_target_af = 2/3
 
         if lower_target_af - slack < maf < lower_target_af + slack or \
             upper_target_af - slack < maf < upper_target_af + slack:
             return True
         return np.nan()
 
-    def af_cnv_call_region(self, cnv_candidates, snv_vcf):
+    def af_cnv_call_region(self, cnv_candidates, snv_vcf, af_tag):
         cnv_calls = {}
         vcf_file = pysam.VariantFile(snv_vcf)
         vcf_sample = list(vcf_file.header.samples).pop()  # only the first sample is used if a multisample is given
         for each_chromosome in cnv_candidates.keys():
             self.logger.debug(each_chromosome)
             cnv_calls[each_chromosome] = []
             for each_candidate in cnv_candidates[each_chromosome]:
                 genomic_region = f'{each_chromosome}:{each_candidate.start}-{each_candidate.end}'
                 # CN state == pliody is a FP as there is no copy number alteration
                 # NOTE: should we generalize it ot  cn_state == ploidy?
                 if each_candidate.cn_status == 2 and self.user_ploidy == 2:
                     self.logger.debug(f'FP,{genomic_region} => {each_candidate.cn_status},{each_candidate.type}')
                 else:
                     # AF is already a float
-                    af = np.nanmean([var_record.samples[vcf_sample]["AF"] for var_record in \
-                        vcf_file.fetch(region=genomic_region)])
+                    af = np.nanmean([var_record.samples[vcf_sample][af_tag] for var_record in \
+                        vcf_file.fetch(region=genomic_region) \
+                            if type(var_record.samples[vcf_sample][af_tag]) != tuple])
                     if self.af_cn_state_concordance(af, each_candidate.cn_status):
                         cnv_calls[each_chromosome].append(each_candidate)
                     else:
                         self.logger.debug(f'FP,{genomic_region} => {each_candidate.cn_status},{each_candidate.type},{af}')
         return cnv_calls
 
     def af_cn_state_concordance(self, af, cn_state):
```

### Comparing `spectre-cnv-0.2.0/spectre/analysis/call_cnv_coverage.py` & `spectre_cnv-0.2.1/spectre/analysis/call_cnv_coverage.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/analysis/cnv_metrics.py` & `spectre_cnv-0.2.1/spectre/analysis/cnv_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,15 +445,15 @@
                 self.logger.warning(f"Using fallback to threshold of: {del_threshold}")
             if dup_threshold > self.ploidy + 1:
                 self.logger.warning(
                     f"Estimated DUP threshold {dup_threshold} is over the allowed maximum threshold of {self.ploidy + 1}. ")
                 dup_threshold = self.ploidy + 1
                 self.logger.warning(f"Using fallback to threshold of: {dup_threshold}")
         return del_threshold, dup_threshold
-    def evaluate_cnvs(self, cnv_calls=None, refined_cnvs: bool = False) -> dict:
+    def evaluate_cnvs(self, refined_cnvs: bool = False) -> dict:
         """
         Evaluating all submitted CNV calls, by applying statistical tests. Optionally, plotting the location of the CNVs
         on the global coverage samples per chr.
         :return: Modified CNVCandidates
         """
         self.logger.debug("Evaluating all CNVs")
 
@@ -479,39 +479,39 @@
                     cnv_metrics_Z["cnv_call_mean"] = np.nanmean(cnv.cov)
 
                 cnv.statistics["z-score"] = {"statistics": cnv_metrics_Z["statistics"],
                                              "score": cnv_metrics_Z["score"],
                                              "pvalue": cnv_metrics_Z["pvalue"],
                                              "sample_score": cnv_metrics_Z["sample_score"]}
 
-                if self.as_dev and False:  # BUG line 385
-                    if not np.isnan(cnv_metrics_Z["cnv_call_mean"]):
-
-                        # pre check --> avoide div by 0
-                        if cnv_metrics_Z["cnv_call_mean"] == 0:
-                            x_index = 0
-                        else:
-                            if not np.isinf(cnv_metrics_Z["cnv_call_mean"]):
-                                x_index = int(cnv_metrics_Z["cnv_call_mean"] / width)
-                            else:
-                                x_index = int(x[-1])
-                        # check if out of bounds
-                        if x_index >= len(x):
-                            cnv_y = x[-1]
-                        else:
-                            cnv_y = int(x[x_index])
-                        cnv_y = int(cnv_y)
-                        annotation_endpoint_offset = 5 * (100 - x_index) * (
-                                1 - (cnv_y / 150)) + (max(x) / 10)  # np.random.randint(100,300)
-
-                        # Add
-                        ax.annotate(f"{cnv.id}", xy=(cnv_metrics_Z["cnv_call_mean"], cnv_y),
-                                    xytext=(cnv_metrics_Z["cnv_call_mean"], cnv_y + annotation_endpoint_offset),
-                                    rotation=60,
-                                    fontsize=12, arrowprops=dict(facecolor='green', shrink=0.05))
+                # if self.as_dev and False:  # BUG line 385
+                #     if not np.isnan(cnv_metrics_Z["cnv_call_mean"]):
+                #
+                #         # pre check --> avoide div by 0
+                #         if cnv_metrics_Z["cnv_call_mean"] == 0:
+                #             x_index = 0
+                #         else:
+                #             if not np.isinf(cnv_metrics_Z["cnv_call_mean"]):
+                #                 x_index = int(cnv_metrics_Z["cnv_call_mean"] / width)
+                #             else:
+                #                 x_index = int(x[-1])
+                #         # check if out of bounds
+                #         if x_index >= len(x):
+                #             cnv_y = x[-1]
+                #         else:
+                #             cnv_y = int(x[x_index])
+                #         cnv_y = int(cnv_y)
+                #         annotation_endpoint_offset = 5 * (100 - x_index) * (
+                #                 1 - (cnv_y / 150)) + (max(x) / 10)  # np.random.randint(100,300)
+                #
+                #         # Add
+                #         ax.annotate(f"{cnv.id}", xy=(cnv_metrics_Z["cnv_call_mean"], cnv_y),
+                #                     xytext=(cnv_metrics_Z["cnv_call_mean"], cnv_y + annotation_endpoint_offset),
+                #                     rotation=60,
+                #                     fontsize=12, arrowprops=dict(facecolor='green', shrink=0.05))
         if self.as_dev:
             self.logger.debug(f"Creating CNV distribution plot")
             fig, ax = plt.subplots()
             x, bins, p = ax.hist(self.df_coverage_candidate_no_excl_zone_random_samples['coverage'], bins=100,
                                  range=[0.0, 5.0])
             # FIXME: BUG -> AttributeError: 'silent_list' object has no attribute 'patches'
             # width = p.patches[0].get_width()
```

### Comparing `spectre-cnv-0.2.0/spectre/analysis/cnv_post_processing.py` & `spectre_cnv-0.2.1/spectre/analysis/cnv_post_processing.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/analysis/coverage_stats.py` & `spectre_cnv-0.2.1/spectre/analysis/coverage_stats.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/analysis/snv_analysis.py` & `spectre_cnv-0.2.1/spectre/analysis/snv_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pysam
 import numpy as np
 import math
 import os
 import sys
 from spectre.util import logger
+from collections import defaultdict
 import gzip
 import copy
 from spectre.classes.loh_candidate import LoHCandidate
 from spectre.libs.unidip.unidip import UniDip
 from spectre.util.vcf_parser import VCFParser
 from spectre.util.cnv_id import CNV_ID
 from spectre.analysis.call_cnv_AF import CNVCall as CNVAnalysisSNP
@@ -65,17 +66,17 @@
         # snv
         self.gt_tag="GT"
         self.dp_tag="DP"
         af="AF"    # Clair3
         vaf="VAF"  # DeepVariant
         header=self.snv_vcf.header.formats.keys()
         self.header_has_tags = self.gt_tag in header and self.dp_tag in header and (af in header or vaf in header)
-        self.logger.error("Not all tags needed are present in the SNV VCF file. Please remove the SNV file") if \
-            not self.header_has_tags else None
-        sys.exit(1)
+        if not self.header_has_tags:
+            self.logger.error("Not all tags needed are present in the SNV VCF file. Please remove the SNV file")
+            sys.exit(1)
         self.af_tag=af if af in header else vaf
         self.gt_het = (0, 1)
         self.gt_ref = (0, 0)
         self.gt_alt = (1, 1)
         # snv qual
         self.max_deviation_perfect_het_af = 0.12
         self.perfect_het_af = 0.5
@@ -123,18 +124,19 @@
         else:
             # something happened / possible error, use all
             self.cn_neutral_coverage_med = np.nanmedian(self.perfect_het_depth)
             self.cn_neutral_coverage_mean = np.nanmean(self.perfect_het_depth)
             self.cn_neutral_coverage_stdev = np.nanstd(self.perfect_het_depth)
 
     def het_dump(self):
-        het_dump_file = gzip.open(f'{self.spectre_args.out_dir}/debug/het_dump.txt.gz', 'wt')
-        for het in self.perfect_het_depth:
-            het_dump_file.write(f'{het}\n')
-        het_dump_file.close()
+        if self.spectre_args.as_dev:
+            het_dump_file = gzip.open(f'{self.spectre_args.out_dir}/debug/het_dump.txt.gz', 'wt')
+            for het in self.perfect_het_depth:
+                het_dump_file.write(f'{het}\n')
+            het_dump_file.close()
 
     def het_clean(self):
         # remove top 2% coverage
         p98 = np.percentile(np.array(self.perfect_het_depth), 98)
         self.logger.debug(f'p98 HET filter = {p98}')
         tmp = copy.deepcopy(self.perfect_het_depth)
         self.perfect_het_depth = []
@@ -144,26 +146,29 @@
         self.logger.debug(f'HET: {len(tmp)} |  p98 HET {len(self.perfect_het_depth)}')
 
     def _is_gt_het(self, snv):
         return snv[self.gt_tag] == self.gt_het
 
     def snv_nhet_chromosome(self):
         self.logger.debug(f'Het sites count per chromosome')
-        chr_het = {chro: 0 for chro in self.genome_info["chromosomes"]}
-        chr_alt = {chro: 0 for chro in self.genome_info["chromosomes"]}
-        chr_all = {chro: 0 for chro in self.genome_info["chromosomes"]}
-        cov_het = {chro: 0 for chro in self.genome_info["chromosomes"]}
+        chr_het = defaultdict(int)
+        chr_alt = defaultdict(int)
+        chr_all = defaultdict(int)
+        cov_het = defaultdict(int)
         # go to begginging of file
         self.snv_vcf.seek(0)
         for snv_record in self.snv_vcf.fetch():
             try:
                 [snv] = snv_record.samples.values()
             except ValueError:
                 [snv] = snv_record.samples.values()[0]
             chr_all[snv_record.chrom] += 1
+            # check for multiple AFs in snv
+            if type(snv[self.af_tag]) == tuple: 
+                continue
             if snv_record.qual > self.min_snv_qual and snv[self.dp_tag] > self.min_coverage_site:
                 # We only expect a single sample column in the VCF
                 # get only HET genotypes
                 if self._is_gt_het(snv):
                     if abs(self.perfect_het_af - snv[self.af_tag]) < self.max_deviation_perfect_het_af:
                         chr_het[snv_record.chrom] += 1
                         cov_het[snv_record.chrom] += snv[self.dp_tag]
@@ -204,14 +209,17 @@
         self.snv_vcf.seek(0)
         for snv_record in self.snv_vcf.fetch():
             # We only expect a single sample column in the VCF
             try:
                 [snv] = snv_record.samples.values()
             except ValueError:
                 [snv] = snv_record.samples.values()[0]
+            # check for multiple AFs in snv
+            if type(snv[self.af_tag]) == tuple: 
+                continue
             if use_chr_het_sites is not None:
                 if snv_record.chrom in use_chr_het_sites:
                     # Only high quality calls, threshold suggested by Medhat
                     if snv_record.qual > self.min_snv_qual:
                         # get only HET genotypes
                         if self._is_gt_het(snv):
                             if abs(self.perfect_het_af - snv[self.af_tag]) < self.max_deviation_perfect_het_af:
@@ -228,15 +236,15 @@
         if return_result:
             return self.cn_neutral_coverage_med
 
     def call_cnv_af_region(self, cnv_calls_list):
         cnv_by_af = CNVAnalysisSNP(genome_info=self.genome_info,
                                    user_args=self.spectre_args)
         self.logger.info("Calculating CNV events based on SNV data")
-        self.cnv_calls_list_af = cnv_by_af.af_cnv_call_region(cnv_calls_list, self.snv_file)
+        self.cnv_calls_list_af = cnv_by_af.af_cnv_call_region(cnv_calls_list, self.snv_file, self.af_tag)
 
     @staticmethod
     def get_score_sigmoid(lohc):
         # https://en.wikipedia.org/wiki/Logistic_function
         # x is the length of the give loh region
         x = lohc.size
         max_score = 60
@@ -271,14 +279,16 @@
                 # timitng per chr
                 dev_timing_chr = DevTiming(timing_process=f' {chro}', name=__name__)
                 dev_timing_chr.start()
                 for snv_record in self.snv_vcf.fetch(region=chro):
                     if snv_record.qual > self.min_snv_qual:
                         total_sites += 1
                         [snv] = snv_record.samples.values()
+                        if type(snv[self.af_tag]) == tuple: 
+                            continue
                         dp, gt, af = int(snv[self.dp_tag]), snv[self.gt_tag], float(snv[self.af_tag])
                         if gt == self.gt_alt:
                             loh_sites_count += 1
                             loh_per_cand += 1
                             sites_per_cand += 1
                             if not loh_candidates.is_init:
                                 loh_candidates.start_candidate_list(snv_record.contig, int(snv_record.pos),
@@ -493,42 +503,49 @@
         self.logger.info(f'Total number of loh candidates = {loh_pass + loh_fail["total"]}, after filtering:')
         self.logger.info(f'  PASS={loh_pass} | FAIL={loh_fail} | MIN_LEN={prety_min} MAX_LEN={prety_max}')
         # Dev timing ---------- #
         dev_timing.end()
         # -------------------- #
 
     def loh_dump(self, version=""):
-        dump_file = f'{self.spectre_args.out_dir}/debug/loh_dump{version}.tsv'
-        dump_file_bgz = f'{self.spectre_args.out_dir}/debug/loh_dump{version}.tsv.gz'
-        loh_dump_file = open(dump_file, 'w')
-        for lohc in self.loh_candidate_list:
-            loh_dump_file.write(f'{lohc.print(self.cn_neutral_coverage_med, self.ploidy)}\t' \
-                                f'{lohc.filter}\t{lohc.het_score}\t{np.round(lohc.gt_alt_prop, 3)}\n')
-        loh_dump_file.close()
-        pysam.tabix_compress(filename_in=dump_file, filename_out=dump_file_bgz, force=True)
-        pysam.tabix_index(filename=dump_file_bgz, force=True, preset="bed")
-        if os.path.isfile(dump_file_bgz) and os.stat(dump_file_bgz).st_size != 0:
-            os.remove(dump_file)
+        if self.spectre_args.as_dev:
+            dump_file = f'{self.spectre_args.out_dir}/debug/loh_dump{version}.tsv'
+            dump_file_bgz = f'{self.spectre_args.out_dir}/debug/loh_dump{version}.tsv.gz'
+            loh_dump_file = open(dump_file, 'w')
+            for lohc in self.loh_candidate_list:
+                loh_dump_file.write(f'{lohc.print(self.cn_neutral_coverage_med, self.ploidy)}\t' \
+                                    f'{lohc.filter}\t{lohc.het_score}\t{np.round(lohc.gt_alt_prop, 3)}\n')
+            loh_dump_file.close()
+            pysam.tabix_compress(filename_in=dump_file, filename_out=dump_file_bgz, force=True)
+            pysam.tabix_index(filename=dump_file_bgz, force=True, preset="bed")
+            if os.path.isfile(dump_file_bgz) and os.stat(dump_file_bgz).st_size != 0:
+                os.remove(dump_file)
 
     def loh_report(self):
         for lohc in self.loh_candidate_list:
             if lohc.loh_pass:
                 self.logger.debug(lohc.print(self.cn_neutral_coverage_med, self.ploidy))
 
-    def loh_pass_only(self):
+    def loh_pass_and_non_pass(self):
         pass_only = {}
+        fail_only = {}
         for chro in self.spectre_args.only_chr_list:
             if chro not in pass_only:
                 pass_only[chro] = []
+            if chro not in fail_only:
+                fail_only[chro] = []
         for lohc in self.loh_candidate_list:
             if lohc.loh_pass:
                 pass_only[lohc.chromosome].append(lohc)
+            else:
+                fail_only[lohc.chromosome].append(lohc)
         for chro in pass_only:
             self.logger.debug(f'LOH candidates pass {chro}:  {len(pass_only[chro])}')
-        return pass_only
+        return pass_only, fail_only
+
 
     def loh(self, existing_cnv_ids):
         #  > LoH candidates (quick)
         self.candidate_loh(existing_cnv_ids)
         #  > LoH debug
         # self.loh_dump(version="_v1")
         #  > LoH candidates merge
```

### Comparing `spectre-cnv-0.2.0/spectre/classes/cnv_candidate.py` & `spectre_cnv-0.2.1/spectre/classes/cnv_candidate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 
 class CNVCandidate(object):
-    def __init__(self, sample_origin="",bin_size=1000):
+    def __init__(self, sample_origin="", bin_size=1000):
         self.chromosome = ""
         self.start = 0
         self.end = 0
         self.size = 0
         self.bin_size = int(bin_size)
         self.pos = []
         self.cov = []
@@ -27,16 +27,18 @@
         self.het_score = float()  # makes sense from 0-1
         self.statistics = {}
         self.support_cnv_calls = {}
         self.sample_origin = sample_origin  # e.g. hg002
         self.merged_sample_references = set()
         # SV support from SNFJ data
         self.sv_support = False
+        # superseded by this candidate
+        self.merged_sample = False  # if this candidate is a merged candidate and has been superseded by another CNV
 
-    def push_candidates(self, chromosome, cnv_pos_cand_list, cnv_cov_cand_list, cnv_type ):
+    def push_candidates(self, chromosome, cnv_pos_cand_list, cnv_cov_cand_list, cnv_type):
         self.chromosome = chromosome
         self.pos = cnv_pos_cand_list
         self.start = int(self.pos[0])
         self.end = int(self.pos[-1])
         self.size = self.end - self.start
         self.size_kb = int((self.end - self.start) / self.bin_size)
         self.cov = cnv_cov_cand_list
@@ -61,15 +63,15 @@
         self.size_kb = int((self.end - self.start) / self.bin_size)
         self.median_cov_norm = np.nanmedian(self.cov)
         # self.raw_cov = list(self.raw_cov) + list(cnv_cand_raw_cov)
         self.median_raw_cov = self.median_cov_norm * self.normalization_value
         self.merged_sample_references.add(cnv_id)
         self.merged_sample_references |= cnv_merged_ids  # "|" joins sets
 
-    def add_scaffold_candidate(self, scaf_start:int, scaf_end:int, scaf_cov:list, scaf_pos:list):
+    def add_scaffold_candidate(self, scaf_start: int, scaf_end: int, scaf_cov: list, scaf_pos: list):
         # insert coverage and positions of scaffold into candidate between scaf_start and scaf_end in self.cov and self.pos
 
         # instert coverage
         self.cov = self.cov[:scaf_start] + scaf_cov + self.cov[scaf_end:]
         # insert positions
         self.pos = self.pos[:scaf_start] + scaf_pos + self.pos[scaf_end:]
 
@@ -90,31 +92,31 @@
             self.median_cov_norm = np.nanmedian(self.cov)
         else:
             self.median_cov_norm = 0.0
 
     def set_id(self, id: str):
         self.id = f"Spectre.{self.type}.{id}"
 
-    def reinitialize_candidate_values(self) -> None:
-        """
-        Used after loading data from .spc file
-        :return: None
-        """
-        self.cn_status = self.set_copy_number_status(self.cov)[0]  # set copy number status
-        self.median_coverage_candidates_merged()  # median of normalized coverage
-        self.merged_sample_references = set(self.merged_sample_references)  # convert list to set
-
     @staticmethod
     def set_copy_number_status(candidate_coverage):
         median_candidates_coverage = np.nanmedian(candidate_coverage)
         if median_candidates_coverage == np.inf or median_candidates_coverage == np.nan:
             return [2, 2.0]  # we are working with diploid data
             # one for regular signal ... inf can not be a valid CN state
         # copy number state is given by integer type conversion of the float value median coverage, e.g. 1.51-> 1
         return [int(round(median_candidates_coverage, 0)), median_candidates_coverage]
 
+    def get_number_of_merged_samples(self) -> int:
+        x = 0
+        # count number of samples in self.support_cnv_calls which have True as a value for merged_sample
+        for sample in self.support_cnv_calls:
+            for cnv in self.support_cnv_calls[sample]:
+                if cnv.merged_sample:
+                    x += 1
+        return x
+
     # functions required to use this object as a key in a dictionary
     def __hash__(self):
         return hash(self.id)
 
     def __eq__(self, other):
         return hash(self.id) == hash(other.id)
```

### Comparing `spectre-cnv-0.2.0/spectre/classes/loh_candidate.py` & `spectre_cnv-0.2.1/spectre/classes/loh_candidate.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/libs/unidip/dip.py` & `spectre_cnv-0.2.1/spectre/libs/unidip/dip.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/libs/unidip/unidip.py` & `spectre_cnv-0.2.1/spectre/libs/unidip/unidip.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/plots/plot.py` & `spectre_cnv-0.2.1/spectre/plots/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,10 +77,10 @@
         if bounds is not None:
             [upperb, lowerb] = bounds if len(bounds) == 2 else [np.NaN, np.NaN]
             self.main_plot.plot(np.array([1, stats.chromosome_len]), np.array([lowerb, lowerb]),
                                 linewidth='1', color="#dd3497")
             self.main_plot.plot(np.array([1, stats.chromosome_len]), np.array([upperb, upperb]),
                                 linewidth='1', color="#dd3497")
         self.figure.suptitle(f'{self.file_prefix} chromosome: {current_chromosome}')
-        self.figure.savefig(f'{self.output_directory}/debug/{self.file_prefix}_plot_cnv_{current_chromosome}.png', dpi=300)
-        self.logger.info(f'Plot saved: debug/{self.file_prefix}_plot_cnv_{current_chromosome}.png')
+        self.figure.savefig(f'{self.output_directory}/img/{self.file_prefix}_plot_cnv_{current_chromosome}.png', dpi=300)
+        self.logger.info(f'Plot saved: img/{self.file_prefix}_plot_cnv_{current_chromosome}.png')
         self.figure.clf()
```

### Comparing `spectre-cnv-0.2.0/spectre/spectre.py` & `spectre_cnv-0.2.1/spectre/spectre.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 import os
 import sys
+
 sys.dont_write_bytecode = True
 import argparse
 import pysam
 
 from builtins import float
 
 from spectre.util import logger
@@ -17,15 +18,15 @@
 class SpectreCallParam(object):
     def __init__(self):
         self.bin_size = 1  # in kb
         self.coverage_dir = ""
         self.sample_id = ""
         self.out_dir = ""
         self.reference = ""
-        self.metadata = ""
+        self.metadata_filename = ""
         self.snv = ""
         self.n_size = 5
         self.save_only = False  # this one is not updated as we need the return to occur
         self.black_list = ""
         self.only_chr_list = ""
         self.ploidy = 2
         self.ploidy_chr_list = ""
@@ -53,15 +54,15 @@
 
     def set_params_from_args(self, user_args):
         # self.bin_size = user_args.bin_size
         self.coverage_dir = user_args.coverage_dir
         self.sample_id = user_args.sample_id
         self.out_dir = user_args.output_dir
         self.reference = user_args.reference
-        self.metadata = user_args.metadata
+        self.metadata_filename = user_args.metadata_filename
         self.snv = user_args.snv_file
         self.snfj = user_args.snfj_file
         self.black_list = user_args.black_list_file
         self.only_chr_list = user_args.only_chr_list
         self.ploidy = user_args.ploidy
         self.ploidy_chr_list = user_args.ploidy_chr
         self.min_cnv_len = user_args.min_cnv_len
@@ -87,72 +88,72 @@
         # self.dev_candidate_final_threshold = user_args.candidate_final_threshold  # 100000  # 100kb
 
 
 class SpectreMetadataParam(object):
     def __init__(self):
         self.reference = ""
         self.bin_size = 1
-        self.metadata = ""
+        self.metadata_filename = ""
         self.out_dir = ""
         self.n_size = 5
         self.save_only = False
         self.as_dev = False
         self.black_list = ""
         self.call_from_console = False
 
     def set_params_from_args(self, user_args, metadata_from_console=False):
         self.reference = user_args.reference
-        # self.bin_size = user_args.bin_size
-        self.metadata = user_args.metadata
+        self.metadata_filename = user_args.metadata_filename
         self.out_dir = user_args.output_dir
         self.n_size = user_args.n_size
         self.save_only = user_args.save_only
-        self.black_list = user_args.black_list_file
         self.as_dev = user_args.as_dev
         self.call_from_console = metadata_from_console
 
     def set_params_from_spectre(self, user_spectre_args):
         self.reference = user_spectre_args.reference
         # self.bin_size = user_spectre_args.bin_size
-        self.metadata = user_spectre_args.metadata
+        self.metadata_filename = user_spectre_args.metadata_filename
         self.out_dir = user_spectre_args.out_dir
         self.n_size = user_spectre_args.n_size
         self.save_only = user_spectre_args.save_only
         self.black_list = user_spectre_args.black_list
         self.as_dev = user_spectre_args.as_dev
 
 
 class SpectrePopulationMode(object):
     def __init__(self):
         self.candidates = []
         self.sample_id = ""
         self.out_dir = ""
         self.reference = ""
         self.as_dev = False
+        self.disable_quality_filter = False
 
     def set_params_from_args(self, user_args):
         self.candidates = user_args.population_candidates
         self.sample_id = user_args.sample_id
         self.out_dir = user_args.output_dir
         self.reference = user_args.reference
+        self.disable_quality_filter = user_args.disable_quality_filter
         self.as_dev = user_args.as_dev
 
 
 def outside_spectre_worker(si: dict):
     worker = SpectreCNV(spectre_args=si["spectre_args"], mdr_file_path=si["mdr_file_path"],
                         coverage_filepath=si["coverage_filepath"], sample_id=si["sample_id"],
                         genome_info=si["genome_info"], debug_dir=si["debug_dir"])
     worker.cnv_call()
     return worker.cnv_analysis.intermediate_candidates_file_location
 
 
 class Spectre:
     def __init__(self, as_dev=False):
         # version
-        self.version = "0.2.0"
+        self.version = "0.2.1"
         # get a custom logger & set the logging level
         self.logger = logger.setup_log(__name__, as_dev)
 
         self.debug_dir = ""
         # for spectre cnv caller
         self.spectre_args = SpectreCallParam()
         self.sample_dir_list = []
@@ -183,83 +184,79 @@
         pysam_genome.close()
         self.logger.debug(f'genome: {genome_info["chromosomes"]}')
         self.genome = genome_info
 
     # TODO: we need to remove this and give the mdr metadata + blacklist in a single file
     def extact_metadata_from_reference(self) -> str:
         """
-        First step of Spectre, extract metadata from reference genome if no md file was provided
+        First step of Spectre, extract metadata from reference genome if no .mdr file was provided
         :return: path to the metadata file (optional)
         """
         # ----------- Metadata extraction from ref file  -----------
         self.metadata_args.out_dir = os.path.abspath(os.path.expanduser(self.metadata_args.out_dir))
 
         # Extract regions with Ns
         fasta_metadata = FastaRef(metadata_args=self.metadata_args)
         self.logger.info("Evaluate if a new .mdr file needs to be created")
 
         # Determine if a mdr file was given if not create one in the output directory
-        mdr_file_path = self.metadata_args.metadata if not self.metadata_args.call_from_console \
-            else f'{self.metadata_args.out_dir}/{self.metadata_args.metadata}'
+        mdr_file_path = self.metadata_args.metadata_filename if not self.metadata_args.call_from_console \
+            else f'{self.metadata_args.out_dir}/{self.metadata_args.metadata_filename}'
         # metadata parameter given?
         if mdr_file_path != "":
             mdr_file_path = os.path.abspath(os.path.expanduser(mdr_file_path))
         else:
             self.logger.info("Looking for default metadata.mdr in output directory")
             mdr_file_path = os.path.abspath(os.path.expanduser(f'{self.metadata_args.out_dir}/metadata.mdr'))
 
         # Check if mdr file exists
         if not os.path.exists(mdr_file_path):
             self.logger.info(f'No metadata file found in')
             self.logger.info(f'Extracting metadata from {self.metadata_args.reference}')
             fasta_metadata.get_n_regions(out_file_name=mdr_file_path)
         else:
-            self.logger.info(f'Using existing metadata file {self.metadata_args.metadata}')
+            self.logger.info(f'Using existing metadata file {self.metadata_args.metadata_filename}')
         return mdr_file_path
 
     # TODO: same here we need to remove this and give the mdr metadata + blacklist in a single file
     def meta_data_extraction(self):
         # ----------- Metadata extraction from ref file  -----------
         # self.metadata_args.as_dev  # Note: this is not used
         self.metadata_args.out_dir = os.path.abspath(os.path.expanduser(self.metadata_args.out_dir))
-        blacklist_data_bed = self.metadata_args.black_list  # bed format
+        # blacklist_data_bed = self.metadata_args.black_list  # bed format
         # Extract regions with Ns
         fasta_metadata = FastaRef(metadata_args=self.metadata_args)
         self.logger.info("Extraction of metadata is activated")
         # if "call_from_console" then the meta_data_report serves as output only,
         # otherwise as both
         default_metadata_name = f'{self.metadata_args.out_dir}/metadata.mdr'  # default
-        meta_data_report = self.metadata_args.metadata if not self.metadata_args.call_from_console \
-            else f'{self.metadata_args.out_dir}/{self.metadata_args.metadata}'
+        meta_data_report = self.metadata_args.metadata_filename if not self.metadata_args.call_from_console \
+            else f'{self.metadata_args.out_dir}/{self.metadata_args.metadata_filename}'
         # metadata parameter given?
         if meta_data_report != "":
             meta_data_report = os.path.abspath(os.path.expanduser(meta_data_report))
         else:
             self.logger.info("Looking for default metadata.mdr")
-            meta_data_report = os.path.abspath(os.path.expanduser(default_metadata_name))
-        # TODO metadata (.mdr) file does not exist
-        # TODO get true positions of Ns
+            if not os.path.exists(default_metadata_name):
+                meta_data_report = os.path.abspath(os.path.expanduser(default_metadata_name))
+                self.logger.info(f"Metadata file already exists at {meta_data_report}")
+
         if not os.path.exists(meta_data_report):
             self.logger.info(f'Extracting metadata from {self.metadata_args.reference}')
-            metadata_result = fasta_metadata.get_n_regions(out_file_name=meta_data_report)
-        else:
-            # TODO get true positions based on metadata (.mdr) file, shall only be called when computing the sample
-            self.logger.info(f'Extracting metadata from {meta_data_report}')
-            metadata_result = fasta_metadata.extract_n_regions_from_report(meta_data_report)
-
-        if self.metadata_args.black_list != "":
-            self.logger.debug("Using blacklist")
-            blacklist_results = fasta_metadata.extract_blacklisted_regions()
-            metadata_result = fasta_metadata.merge_metadata(metadata_result, blacklist_results)
-        # return metadata object (dict) after writing to file?
-        if self.metadata_args.save_only:
-            pass
-        else:
-            self.logger.debug("returned meta Object")
-            return metadata_result
+            fasta_metadata.get_n_regions(out_file_name=meta_data_report)
+        # else:
+        #     # TODO get true positions based on metadata (.mdr) file, shall only be called when computing the sample
+        #     self.logger.info(f'Extracting metadata from {meta_data_report}')
+        #     metadata_result = fasta_metadata.extract_n_regions_from_report(meta_data_report)
+        #
+        # if self.metadata_args.black_list != "":
+        #     self.logger.debug("Using blacklist")
+        #     blacklist_results = fasta_metadata.extract_blacklisted_regions()
+        #     metadata_result = fasta_metadata.merge_metadata(metadata_result, blacklist_results)
+        #     # fasta_metadata.write_combined_metadata_to_file(metadata_result, meta_data_report)
 
     def spectre_exe(self):
         # Parameters
         self.display_version()
         self.logger.info("Starting spectre")
 
         self.spectre_args.out_dir = os.path.abspath(os.path.expanduser(self.spectre_args.out_dir))
@@ -287,78 +284,93 @@
                     self.logger.error(f"Please use something like this: --ploidy-chr chr1:2,chr2:2,chrX:1,...")
                     sys.exit(1)
                 chr_name, ploidy = ploid_chr.split(":")
                 # check if chromosome is in reference genome if missing it will be added
                 if chr_name not in self.genome["chr_ploidy"].keys():
                     self.logger.warning(f"Chromosome {chr_name} not found in reference genome. Skipping {ploid_chr}!")
                     continue
-                self.genome["chr_ploidy"][chr_name] = int(ploidy)
+                # for ploidy values 1 and 2
+                new_ploidy = (1 / (int(ploidy) / self.spectre_args.ploidy)) * self.spectre_args.ploidy
+                self.genome["chr_ploidy"][chr_name] = int(new_ploidy)
 
         # Setting up directories
         if not os.path.exists(self.spectre_args.out_dir):
             os.makedirs(self.spectre_args.out_dir)
         # tmp dir
         if not os.path.exists(f'{self.spectre_args.out_dir}/tmp'):
             os.makedirs(f'{self.spectre_args.out_dir}/tmp')
 
+        # directory for cnv plots
+        if not os.path.exists(f'{self.spectre_args.out_dir}/img'):
+            os.makedirs(f'{self.spectre_args.out_dir}/img')
+
         if self.spectre_args.as_dev:
             self.debug_dir = f"{self.spectre_args.out_dir}/debug"
             if not os.path.exists(self.debug_dir):
                 os.makedirs(self.debug_dir)
         else:
             self.debug_dir = self.spectre_args.out_dir
 
         # Split for pop and single
         spectre_instructions = []
         for sample_id, coverage_dir in zip(self.spectre_args.sample_id, self.spectre_args.coverage_dir):
             coverage_dir = os.path.abspath(os.path.expanduser(coverage_dir))
-            instructions = {"spectre_args": self.spectre_args, "coverage_filepath": self.spectre_args.coverage_dir[0], "sample_id": sample_id,
+            instructions = {"spectre_args": self.spectre_args, "coverage_filepath": self.spectre_args.coverage_dir[0],
+                            "sample_id": sample_id,
                             "mdr_file_path": self.mdr_file_path, "genome_info": self.genome.copy(),
                             "debug_dir": self.debug_dir, "logger": self.logger
                             }
             spectre_instructions.append(instructions.copy())
 
         if self.spectre_args.run_population_mode:
             # Preparing spectre instructions for multiprocess
             spectre_instructions = []
             for sample_id, coverage_dir in zip(self.spectre_args.sample_id, self.spectre_args.coverage_dir):
                 coverage_dir = os.path.abspath(os.path.expanduser(coverage_dir))
-                instructions = {"spectre_args": self.spectre_args, "coverage_dir": coverage_dir, "sample_id": sample_id,
+                instructions = {"spectre_args": self.spectre_args, "coverage_filepath": coverage_dir,
+                                "sample_id": sample_id,
                                 "mdr_file_path": self.mdr_file_path, "genome_info": self.genome.copy(),
                                 "debug_dir": self.debug_dir, "logger": self.logger
                                 }
                 spectre_instructions.append(instructions.copy())
 
             # Distribute Samples over cores/threads
             with Pool(processes=self.spectre_args.threads) as pool:
                 results = pool.map(outside_spectre_worker, tuple(spectre_instructions))
             intermediate_file_paths = [x for x in results]
 
             if self.spectre_args.run_population_mode and len(intermediate_file_paths) > 1:
-                self.population_exe("population_file", intermediate_file_paths, self.spectre_args.out_dir, self.spectre_args.reference, self.spectre_args.as_dev)
+                self.population_exe("population_file", intermediate_file_paths, self.spectre_args.out_dir,
+                                    self.spectre_args.reference, self.spectre_args.as_dev)
         else:
+            instruction_0 = spectre_instructions[0]
+            if len(spectre_instructions) > 1:
+                self.logger.warning("You provided multiple samples but did not activate the population mode!")
+                self.logger.warning(f"Calling CNVs ONLY for sample: {instruction_0['sample_id']}")
+
+            spectre_main = SpectreCNV(spectre_args=instruction_0["spectre_args"],
+                                      mdr_file_path=instruction_0["mdr_file_path"],
+                                      coverage_filepath=instruction_0["coverage_filepath"],
+                                      sample_id=instruction_0["sample_id"],
+                                      genome_info=instruction_0["genome_info"], debug_dir=instruction_0["debug_dir"])
 
-            spectre_main = SpectreCNV(spectre_args=self.spectre_args,
-                                      mdr_file_path=self.mdr_file_path,
-                                      coverage_filepath=self.spectre_args.coverage_dir[0],
-                                      sample_id=self.spectre_args.sample_id[0],
-                                      genome_info=self.genome.copy(), debug_dir=self.debug_dir)
             spectre_main.cnv_call()
 
         self.logger.info("Spectre finished")
         # sys.exit(0)
 
     def population_exe(self, population_sample_name="", population_intermediate_files=None, outputdir="", reference="",
-                       as_dev=False):
+                       disable_quality_filter=False, as_dev=False):
         self.logger.info("Starting Spectre population mode")
         # Adjusting parameters
         sample_ids = self.population_args.sample_id if population_sample_name == "" else population_sample_name
         population_paths = self.population_args.candidates if not population_intermediate_files else population_intermediate_files
         output_dir = os.path.abspath(os.path.expanduser(self.population_args.out_dir)) if outputdir == "" else outputdir
         as_dev = self.population_args.as_dev if not as_dev else as_dev
+        disable_quality_filter = self.population_args.disable_quality_filter if not disable_quality_filter else disable_quality_filter
         reference = self.population_args.reference if not reference else reference
 
         # Required to load the genome information, if any other file format than .spc is provided
         if not any(".spc" in s for s in population_paths):
             if not self.genome:
                 self.make_genome_info(reference)
 
@@ -370,81 +382,95 @@
         if as_dev:
             debug_dir = f"{output_dir}/debug"
             if not os.path.exists(debug_dir):
                 os.makedirs(debug_dir)
 
         # Population mode setup
         __spectre_population_worker = SpectrePopulation(sample_id=sample_ids,
-                                                                             output_dir=output_dir,
-                                                                             reciprocal_overlap=0.2,
-                                                                             genome_info=self.genome)
+                                                        output_dir=output_dir,
+                                                        reciprocal_overlap=0.8,
+                                                        discard_quality_control=disable_quality_filter,
+                                                        genome_info=self.genome, as_dev=as_dev)
         __spectre_population_worker.load_files(population_paths)  # Loading files for population mode
         __spectre_population_worker.cnv_call_population()  # Starting the population CNV calculations
 
 
 # Arguments
 def get_arguments():
     spectre_help = """
     vcf_utils <command> [<args>]
     Spectre:
         CNVCaller:
-            Required
+            [Required]
                 --coverage     Path to the coverage file from Mosdepth output. Expects the following files:
                                    <prefix>.regions.bed.gz
                                    <prefix>.regions.bed.gz.csi
-                               Can be one or more directories. Example:
+                               Can be one or more paths. However, providing multiple samples is only intended to
+                               work with the --population flag. Example:
                                     --coverage /path/md1.regions.gz /path/md2.regions.gz
-                --sample-id    Sample name/ID. Can be one or more ID. Example:
+                --sample-id    Sample name/ID. Can be one or more ID. However, providing multiple sample ids is only
+                               intended to work with the --population flag. Example:
                                     --sample-id id1 id2
                 --output-dir   Output directory
                 --reference    Reference sequence used for mapping (for N removal)
-            Optional, if missing it will be created
-                --metadata     Metadata file for Ns removal
-            Optional
+            [Optional, if missing it will be created]
+                --metadata     Metadata file for Ns removal (this will speed up Spectre massively if provided)
+                --n-size       Required amount of consecutive Ns to be considered an NRegion 
+                               in the reference sequence (Default = 5)
+
+            [Optional]
                 --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
-                --only-chr     Comma separated list of chromosomes to use
+                --only-chr     Comma separated list of chromosomes to use (e.g. chr1,chr2,chr3)
                 --ploidy       Set the ploidy for the analysis, useful for sex chromosomes (Default = 2)
                 --ploidy-chr   Comma separated list of key:value-pairs for individual chromosome ploidy control
                                (e.g. chrX:2,chrY:1) If chromosome is not specified, the default ploidy will be used.
-                --snv          VCF file containing the SNV for the same sample CNV want to be called
                 --snfj         Breakpoints from from Sniffle which has been converted from the SNF to the SNFJ format.
-                --n-size       Length of consecutive Ns (Default = 5)
+                               SNFJ files can be generated using the program snf2json.
                 --min-cnv-len  Minimum length of CNV (Default 100kb)
-                --cancer       Set this flag if the sample is cancer (Default = False)
-                --population   Runs the population mode on all provided samples
-                --threads      Amount of threads (This will boost performance if multiple samples are provided)
+                --snv          VCF file containing the SNV for the same sample CNV want to be called
+                --cancer       Set this flag if the sample is cancer (Default = False) This will disable some safety 
+                               checks, when determining the DEL and DUP thresholds. 
 
-                Coverage
+            [Optional, Coverage]
                 --sample-coverage-overwrite     Overwrites the calculated sample coverage, which is used to normalize
                                                 the coverage. e.g. a value of 30 equals to 30X coverage.
                 --disable-max-coverage          Disables the maximum coverage check. This will allow to call CNVs
 
-                LoH (requires --snv)
+            [Optional, LoH (requires --snv)]
                 --loh-min-snv-perkb             Minimum number of SNVs per kilobase for an LoH region (default=5)
                 --loh-min-snv-total             Minimum number of SNVs total for an LoH region (default=100)
                 --loh-min-region-size           Minimum size of a region for a LoH region (default=100000)
 
-
+                --population   Runs the population mode on all provided samples. It will apply all the provided
+                               configurations as well as the default population mode values to all samples.
+                --threads      Amount of threads (This will boost performance if multiple samples are provided)
         RemoveNs:
-            Required
+            [Required]
                 --reference    Reference genome used for mapping
                 --output-dir   Output dir
                 --output-file  Output file for results
-            Optional
-                --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
-                --n-size       Length of consecutive Ns (Default = 5)
-                --save-only    Will only save the metadata file and not show the results in screen (Default = False)
+            [Optional]
+                --n-size       Required amount of consecutive Ns to be considered an NRegion 
+                               in the reference sequence (Default = 5)
+                --save-only    Will only save the metadata file and not show the results on screen (Default = False)
 
         Population:
-            Required
-                --candidates   At least 2 candidate files (.spc or .vcf) which should be taken into consideration for the population mode.
-                --sample-id    Name of the output file
-                --output-dir   Output directory
-            Optional
-                --reference    Reference sequence (Required if VCF files are used!)
+            [Required]
+                --candidates   At least 2 .spc sample files which should be used in the population mode.
+                               (e.g. sample1.spc sample2.spc)
+                --sample-id    The name of the sample-id will be added accordingly at the output.
+                               (e.g. population_mode_<sample-id>.vcf.gz)
+                --output-dir   Path of the output directory
+            [Optional]
+                --reference    Reference sequence
+                --reciprocal-overlap        Minimum reciprocal overlap for supporting variants (CNV or LOH) [0.0 - 1.0] 
+                                            (Default = 0.8)
+                --disable-quality-filter    Disables the quality filter for the population mode. Spectre will also
+                                            search for supporting CNVs in the .SPC files, which have not been reported
+                                            as final CNVs in the VCF and BED file.
         Version:
             version    Shows current version/build
     """
     parser = argparse.ArgumentParser(
         description="Spectre CNV caller",
         usage=spectre_help
     )
@@ -468,15 +494,16 @@
     subparser_cnv_caller.add_argument('-s', '--sample-id', type=str, required=True, dest='sample_id', default="",
                                       help='..., default = None', nargs='+')
     subparser_cnv_caller.add_argument('-d', '--output-dir', type=str, required=True, dest='output_dir', default=".",
                                       help='..., default = None')
     subparser_cnv_caller.add_argument('-r', '--reference', type=str, required=True, dest='reference', default="",
                                       help='..., default = None')
     # Optional, if missing will be created
-    subparser_cnv_caller.add_argument('-m', '--metadata', type=str, required=False, dest='metadata', default="",
+    subparser_cnv_caller.add_argument('-m', '--metadata', type=str, required=False, dest='metadata_filename',
+                                      default="",
                                       help='..., default = None')
     # Optional
     subparser_cnv_caller.add_argument('-v', '--snv', type=str, required=False, dest='snv_file', default="",
                                       help='...')
     subparser_cnv_caller.add_argument('-sj', '--snfj', type=str, required=False, dest='snfj_file', default="",
                                       help='...')
     subparser_cnv_caller.add_argument('-l', '--blacklist', type=str, required=False, dest='black_list_file',
@@ -504,23 +531,24 @@
                                       dest='disable_max_coverage', default=False, help='...s, default = False')
 
     subparser_cnv_caller.add_argument('-a', '--cancer', action='store_true', required=False, dest='is_cancer',
                                       default=False, help='..., default = False')
 
     # Loh
     subparser_cnv_caller.add_argument('-lohkb', '--loh-min-snv-perkb', type=int, required=False, default=10,
-                                      dest='loh_min_snv_perkb', help='..., default = 5')
-    subparser_cnv_caller.add_argument('-lohsnv', '--loh-min-snv-total', type=int, required=False, default=100,
-                                      dest='loh_min_snv_total', help='..., default = 50')
-    subparser_cnv_caller.add_argument('-lohsize', '--loh-min-region-size', type=float, required=False, default=100000.0,
-                                      dest='loh_min_region_size', help='..., default = 50000')
+                                      dest='loh_min_snv_perkb', help='default = 10')
+    subparser_cnv_caller.add_argument('-lohsnv', '--loh-min-snv-total', type=int, required=False, default=1000,
+                                      dest='loh_min_snv_total', help='default = 1000')
+    subparser_cnv_caller.add_argument('-lohsize', '--loh-min-region-size', type=float, required=False,
+                                      default=1000000.0,
+                                      dest='loh_min_region_size', help='default = 1Mb')
     subparser_cnv_caller.add_argument('-lohonly', '--loh-only', action='store_true', required=False, default=False,
-                                      dest='loh_only', help='')
+                                      dest='loh_only', help='Skips CNV calling, only outputs LOH')
     subparser_cnv_caller.add_argument('-cn', '--cn-neutral', type=float, required=False, default=0.0,
-                                      dest='cn_neutral', help='')
+                                      dest='cn_neutral', help='Overwithe the CN neutral value')
 
     # Dev
     subparser_cnv_caller.add_argument('-0', '--dev', action='store_true', required=False, dest='as_dev', default=False,
                                       help='dev, default = False')
     subparser_cnv_caller.add_argument('-01', '--dev-max-std-outlier-rm', type=int, required=False,
                                       dest='max_std_outlier_rm', default=5, help='..., default = 5')
     subparser_cnv_caller.add_argument('-02', '--mosdepth-cov-genome-chr-diff', type=float, required=False,
@@ -542,23 +570,22 @@
     metadata_help = "..."
     subparser_metadata = subparsers.add_parser("RemoveNs", help=metadata_help)
     # Required
     subparser_metadata.add_argument('-r', '--reference', type=str, required=True, dest='reference', default="",
                                     help='..., default = None')
     subparser_metadata.add_argument('-d', '--output-dir', type=str, required=True, dest='output_dir', default="",
                                     help='..., default = None')
-    subparser_metadata.add_argument('-f', '--output-file', type=str, required=True, dest='metadata', default="",
+    subparser_metadata.add_argument('-f', '--output-file', type=str, required=True, dest='metadata_filename',
+                                    default="",
                                     help='..., default = None')
     # Optional
     subparser_metadata.add_argument('-n', '--n-size', type=int, required=False, dest='n_size', default=5,
                                     help='..., default = 5')
     subparser_metadata.add_argument('-s', '--save-only', action='store_true', required=False, dest='save_only',
                                     default=False, help='save_only, default = False')
-    subparser_metadata.add_argument('-l', '--blacklist', type=str, required=False, dest='black_list_file', default="",
-                                    help='...')
     # Dev
     subparser_metadata.add_argument('-0', '--dev', action='store_true', required=False, dest='as_dev', default=False,
                                     help='dev, default = False')
 
     # ############################################################################################ #
     # Population mode
     cnv_population_help = "..."
@@ -566,20 +593,25 @@
     # Required
     subparser_cnv_population.add_argument('-c', '--candidates', type=str, required=True, dest='population_candidates',
                                           default="", help='..., default = None', nargs='+')
     subparser_cnv_population.add_argument('-s', '--sample-id', type=str, required=True, dest='sample_id', default="",
                                           help='..., default = None')
     subparser_cnv_population.add_argument('-d', '--output-dir', type=str, required=True, dest='output_dir', default=".",
                                           help='..., default = None')
+
     subparser_cnv_population.add_argument('-0', '--dev', action='store_true', required=False, dest='as_dev',
-                                          default=False,
-                                          help='dev, default = False')
+                                          default=False, help='dev, default = False')
     # Optional
     subparser_cnv_population.add_argument('-r', '--reference', type=str, required=False, dest='reference', default="",
                                           help='..., default = None')
+    subparser_cnv_population.add_argument('-ro', '--reciprocal-overlap', type=float, required=False,
+                                          dest='reciprocal_overlap', default=0.8, help='..., default = 0.8')
+
+    subparser_cnv_population.add_argument('-dqf', '--disable-quality-filter', action='store_true', required=False,
+                                          dest='disable_quality_filter', default=False,help='..., default = False')
 
     # ############################################################################################ #
     # Dev
     dev_help = "..."
     subparser_dev = subparsers.add_parser("dev", help=dev_help)
 
     # ############################################################################################ #
@@ -600,37 +632,31 @@
         sys.exit(1)
     # logger init
     main_logger = logger.setup_log(__name__, run_as_dev)
     # print Spectre input arguments
     main_logger.info(f"Spectre input: {command} {' '.join(sys.argv[2:])}")
     main_logger.debug(f'Debug output is enabled') if run_as_dev else None
     spectre_run = Spectre(run_as_dev)
-    min_bin_size = 100
     if command == "CNVCaller":
-        # logging.error("Bin size too small") if spectre_args.bin_size < min_bin_size else ""
         # ARGS:  bin_size, coverage_file_bed, sample_id, output_dir, reference="", metadata="", ...
         spectre_run.spectre_args.set_params_from_args(spectre_args)
         spectre_run.spectre_exe()
     elif command == "RemoveNs":
-        main_logger.error("Bin size too small") if spectre_args.bin_size < min_bin_size else ""
-        # ARGS:  reference_fas, output_dir, meta_data_report, bin_size=500, threshold=5
+        # ARGS:  reference_fas, output_dir, meta_data_report, threshold=5
         metadata_call_from_console = True
         spectre_run.metadata_args.set_params_from_args(spectre_args, metadata_call_from_console)
-        spectre_run.meta_data_extraction()
+        spectre_run.extact_metadata_from_reference()
+        # spectre_run.meta_data_extraction()
     elif command == "Population":
         main_logger.error("at least two candidates are required") if len(spectre_args.population_candidates) < 2 else ""
         spectre_run.population_args.set_params_from_args(spectre_args)
         spectre_run.population_exe()
-    elif command == "dev":
-        spectre_run.loh()
-        # spectre_run.display_version()
     elif command == "version":
         spectre_run.display_version()
     else:
-        # logging.error(f'No arguments provided.\n{spectre_help}')
+        print(spectre_help)
         pass
     sys.exit(0)
 
 
 if __name__ == '__main__':
     main()
-
```

### Comparing `spectre-cnv-0.2.0/spectre/spectreCNV.py` & `spectre_cnv-0.2.1/spectre/spectreCNV.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 
     def set_coverage_files(self, coverage_filepath):
         self.logger.info(
             f'Spectre calculating for: {str(coverage_filepath)}')  # and bin size: {self.spectre_args.bin_size}')
         self.get_coverage_dir_file(coverage_filepath)
         return coverage_filepath
 
+
     # MAIN analysis pipeline incluide CNV and SNV analysis (CN neutral and LoH)
     def cnv_call(self):
         # SNV analysis first, if SNV data exisist use it to get the CN neutral
         if self.spectre_args.snv != "":
             self.logger.info("Analysing CN neutral state from SNV data")
             self.logger.info("Cancer mode on") if self.spectre_args.is_cancer else None
             self.snv_analysis = SNVAnalysis(snv_file=self.spectre_args.snv, genome=self.genome_info,
@@ -106,15 +107,15 @@
             # Compare candidates to AF/SNV
             self.snv_analysis.call_cnv_af_region(self.cnv_analysis.cnv_calls_list)
             self.cnv_analysis.cnv_calls_list_af_filtered = self.snv_analysis.cnv_calls_list_af
             # LoH
             self.logger.info("Starting LOH")
             self.snv_analysis.loh(self.cnv_analysis.existing_cnv_ids)
             self.logger.info("Saving final LOH calls")
-            self.cnv_analysis.snv_loh = self.snv_analysis.loh_pass_only()
+            self.cnv_analysis.snv_loh, self.cnv_analysis.snv_loh_raw = self.snv_analysis.loh_pass_and_non_pass()
 
         # Check for breakpoints
         if self.spectre_args.snfj != "":
             self.logger.info("Checking breakpoints from the SNFJ file")
             self.cnv_analysis.check_snfj_breakpoints(self.spectre_args.snfj)
 
         # Make output files
```

### Comparing `spectre-cnv-0.2.0/spectre/util/OSUtil.py` & `spectre_cnv-0.2.1/spectre/util/OSUtil.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/util/cnv_id.py` & `spectre_cnv-0.2.1/spectre/util/cnv_id.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/util/dataAnalyzer.py` & `spectre_cnv-0.2.1/spectre/util/dataAnalyzer.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/util/metadata/metadataCollector.py` & `spectre_cnv-0.2.1/spectre/util/metadata/metadataCollector.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         chromosome_cnt = 0
         chromosome = ""
         # bin_size = self.metadata_args.bin_size
         self.output_file = out_file_name
         # assure abs paths
         reference = os.path.abspath(os.path.expanduser(self.metadata_args.reference))
         # DEL report_output_dir = os.path.abspath(os.path.expanduser(report_output_dir))
-        self.metadata_args.out_dir
+
         file_handler_fasta = open(reference, "r") if "gz" not in reference else gzip.open(reference, "rt")
         for raw_line in file_handler_fasta:
             line = raw_line.rstrip("\n")  # cut away the newline from line (\n)
             # check if line is not a comment or header
             if not (line[:1] == '>' or line[:1] == ';'):
                 for l in line:
                     char = l.upper()
@@ -83,25 +83,24 @@
                     self.logger.info(f'length: {str(chromosome_cnt)}\t{ref_dict[str(chromosome)]}')
                 chromosome = str(line[1:]).split(" ")[0]
                 ref_dict[str(chromosome)] = list()
                 self.logger.info(f'Reading {line}')
                 i = 0
                 j = 0
                 chromosome_cnt = 0
+        file_handler_fasta.close()
 
         self.__nList = ref_dict
         self.__nTo = j
         self.__cCnt = c_cnt
         self.__gCnt = g_cnt
         self.__aCnt = a_cnt
         self.__tCnt = t_cnt
+        # Get MDR statistics and write report
         self.__get_statistic_report()
-        # if not self.metadata_args.save_only:
-        #    return ref_dict
-        # return {}
 
     def extact_metadata_from_mdr(self, input_file: str, bin_size: int) -> dict:
         """
         Adjust the true N region positions according to the bin size.
         :param input_file: MDR file
         :param bin_size: bin size determined by looking at the positional gap in the mosdepth data.
         :return: Adjusted medata N regions.
@@ -189,28 +188,33 @@
                     cells = term.strip().split("\t")
                     if str(cells[1]) not in result:  # [1] = chromosome name
                         result[str(cells[1])] = []
                     result[str(cells[1])].append((cells[2], cells[3]))  # [2] start, [3] end
         return result
 
     def extract_blacklisted_regions(self, blacklist_file: str = "") -> dict:
+        """
+        Extracts the blacklisted regions and saves them as a dictionary if present.
+        :param blacklist_file: path/to/blacklist.bed
+        :return: dict
+        """
         result = dict()
-        if blacklist_file.__eq__(""):
-            path = os.path.abspath(os.path.expanduser(self.metadata_args.black_list))
-        else:
+        # Only try to read the blacklist if it is not provided
+        if blacklist_file != "":
             path = os.path.abspath(os.path.expanduser(blacklist_file))
-        with open(path, "r") as fp:
-            mm = mmap.mmap(fp.fileno(), 0, prot=mmap.PROT_READ)
-            for line in iter(mm.readline, b""):
-                # decode line and cut away last char from line (\n)
-                term = line.decode("utf-8")[:-1]
-                chrom, start, end = term.split("\t")[:3]
-                if str(chrom) not in result:
-                    result[str(chrom)] = []
-                result[str(chrom)].append((start, end))
+
+            with open(path, "r") as fp:
+                mm = mmap.mmap(fp.fileno(), 0, prot=mmap.PROT_READ)
+                for line in iter(mm.readline, b""):
+                    # decode line and cut away last char from line (\n)
+                    term = line.decode("utf-8")[:-1]
+                    chrom, start, end = term.split("\t")[:3]
+                    if str(chrom) not in result:
+                        result[str(chrom)] = []
+                    result[str(chrom)].append((start, end))
         return result
 
     @classmethod
     def merge_metadata(cls, m1: dict, m2: dict) -> dict:
         """
         Merges two dictionaries with the structure str:list
         :param m1: dict m1 with structure str:list
@@ -233,7 +237,8 @@
 
     def __write_report(self):
         self.logger.info(f"Writing MDR to: {os.path.join(self.metadata_args.out_dir, self.output_file)}")
         if not os.path.exists(self.metadata_args.out_dir):
             os.makedirs(self.metadata_args.out_dir)
         with open(os.path.join(self.metadata_args.out_dir, self.output_file), "w") as file:
             file.writelines(self.static_report)
+
```

### Comparing `spectre-cnv-0.2.0/spectre/util/mosdepthReader.py` & `spectre_cnv-0.2.1/spectre/util/mosdepthReader.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/util/outputWriter.py` & `spectre_cnv-0.2.1/spectre/util/outputWriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,19 +63,20 @@
             sample_format_list.append(":".join([str(s) for s in value]))
 
         return "\t".join([self.CHROM, str(self.POS), self.ID, self.REF, self.ALT, self.QUAL, self.FILTER,
                           self.INFO, self.FORMAT] + sample_format_list)
 
 
 class VCFOutput(object):
-    def __init__(self, output_file, genome_info):
+    def __init__(self, output_file, genome_info, sv_support: bool = False):
         self.supp_vec = {}
         self.output_vcf = output_file
         self.population_sample_ids = []
         self.genome_info = genome_info
+        self.sv_support = sv_support
         # example {'chromosomes': ['chr6'], 'chr_lengths': {'chr6': 170805979}}
 
     @staticmethod
     def id_generator(size=8, chars=string.ascii_uppercase + string.digits):
         return ''.join(random.choice(chars) for _ in range(size))
 
     def make_vcf_contigs(self):
@@ -101,22 +102,27 @@
                       'read and thus we cannot predict the full size.">'
                       ]
         # Add Info section
         vcf_header += ['##INFO=<ID=END,Number=1,Type=Integer,Description="End position of the structural variant">',
                        '##INFO=<ID=SVLEN,Number=1,Type=Integer,Description="Length of the SV">',
                        '##INFO=<ID=SVTYPE,Number=1,Type=String,Description="Type of copy number variant">',
                        '##INFO=<ID=CN,Number=1,Type=Integer,Description="Estimated copy number status">',
-                       '##INFO=<ID=SVSUPPORT,Number=1,Type=String,Description="SV support">']
+                       '##INFO=<ID=SVSUPPORT,Number=1,Type=String,Description="Indicator if a SV support was found in a provided SNFJ file">'
+                       ]
         if population_mode:
-            vcf_header += ['##INFO=<ID=SUPP_VEC,Number=1,Type=String,Description="Support vector">']
+            vcf_header += [
+                '##INFO=<ID=SUPPVEC,Number=1,Type=String,Description="Support vector for population variants">',
+                '##INFO=<ID=POPMERGENR,Number=1,Type=Integer,Description="Number of CNVs that have been merged '
+                'into this variant in the Spectre population mode">'
+                ]
 
         # Add Format section
         vcf_header += ['##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">',
                        '##FORMAT=<ID=HO,Number=2,Type=Float,Description="Homozygosity proportion">',
-                       '##FORMAT=<ID=GQ,Number=1,Type=Integer,Description="Genotype quality">',
+                       '##FORMAT=<ID=GQ,Number=1,Type=Float,Description="Genotype quality">',
                        '##FORMAT=<ID=DP,Number=2,Type=Float,Description="Read depth">',
                        '##FORMAT=<ID=ID,Number=1,Type=String,Description="Population ID of supporting CNV calls">'
                        ]
 
         if self.population_sample_ids:
             if population_mode:
                 s = f"##Spectre_population_samples={','.join(self.population_sample_ids)}"
@@ -147,50 +153,61 @@
                 vcf_line.POS = each_candidate.start
                 vcf_line.ID = each_candidate.id
                 vcf_line.ALT = self.set_svtype(each_candidate.type)
                 vcf_line.FILTER = each_candidate.filter
                 vcf_line.QUAL = str(each_candidate.quality)
                 vcf_line.INFO = f"END={each_candidate.end};SVLEN={each_candidate.size};SVTYPE={each_candidate.type};" \
                                 f"CN={each_candidate.cn_status};"
-                vcf_line.INFO += f"SVSUPPORT={'TRUE' if each_candidate.sv_support else 'FALSE'};"
+                if self.sv_support:
+                    vcf_line.INFO += f"SVSUPPORT={'TRUE' if each_candidate.sv_support else 'FALSE'};"
 
                 # checking if any other CNV through merging supported the given CNV
                 vcf_line.supp_vec = self.supp_vec.copy()
                 if not each_candidate.support_cnv_calls:
                     vcf_line.format_data = [each_candidate.gt, f'{round(each_candidate.het_score, 2)}',
                                             f"{int(each_candidate.statistics['z-score']['sample_score'])}",
-                                            f'{round(each_candidate.median_raw_cov,2)}']
+                                            f'{round(each_candidate.median_raw_cov, 2)}']
                 else:
                     vcf_line.format_data = []
                     vcf_line.FORMAT += ":ID"  # ADD ID tag in format as everything that is following are IDs
                     vcf_line.supp_vec = dict(
                         [(str(sample_key), 0) for sample_key in each_candidate.support_cnv_calls.keys()])
                     for sample_key, sample_value in each_candidate.support_cnv_calls.items():
                         if sample_value:
                             ids = []
                             scores = []
                             gts = []
-                            dps = [] # raw read depth
+                            dps = []  # raw read depth
                             # sample_id =""
                             for candidate in list(sample_value):
                                 ids.append(candidate.id)
-                                scores.append(candidate.statistics['z-score']['sample_score'])
+                                scores.append(np.float16(candidate.statistics['z-score']['sample_score']))
                                 gts.append(candidate.gt)
                                 # check if median_raw_cov exists
                                 if candidate.median_raw_cov:
                                     dps.append(candidate.median_raw_cov)
                             gt = Counter(gts).most_common(1)[0][0]
-                            score = np.mean(scores)
-                            dp = np.mean(dps)
-                            vcf_line.sample_format_data[sample_key] = [gt, "0.0", int(score),round(dp,2), ",".join(ids)]
+                            # check if scores or dps contains only nan values
+                            if all(np.isnan(x) for x in scores):
+                                score = np.nan
+                            else:
+                                score = np.nanmean(scores)
+
+                            if all(np.isnan(x) for x in dps):
+                                dp = np.nan
+                            else:
+                                dp = np.nanmean(dps)
+                            vcf_line.sample_format_data[sample_key] = [gt, "0.0", score, round(dp, 2), ",".join(ids)]
                             vcf_line.supp_vec[sample_key] = 1
                         else:
-                            vcf_line.sample_format_data[sample_key] = ["0/0", "0.0", 0, 0.0,"NULL"]
+                            vcf_line.sample_format_data[sample_key] = ["./.", "0.0", 0, 0.0, "NULL"]
                     # add support vector only if population mode is active
-                    vcf_line.INFO += ";SUPP_VEC=" + "".join([str(s) for s in vcf_line.supp_vec.values()])
+                    vcf_line.INFO += ";SUPPVEC=" + "".join([str(s) for s in vcf_line.supp_vec.values()])
+                    # add merged candidate number if population mode is active
+                    vcf_line.INFO += f";POPMERGENR={each_candidate.get_number_of_merged_samples()}"
                 vcf_lines.append(vcf_line.format_vcf_line())
         return "\n".join(vcf_lines)
 
     def make_vcf(self, chromosome_list, cnv_candidate_list, sample_id, population_sample_ids=None):
         # converting population sample ids from set to list
         if not population_sample_ids:
             population_sample_ids = [sample_id]
@@ -214,19 +231,20 @@
 
             # compress and index vcf file
             pysam.tabix_compress(filename_in=tmp_out + ".sort.tmp", filename_out=self.output_vcf, force=True)
             pysam.tabix_index(filename=self.output_vcf, force=True, preset="vcf")
 
         # clean up
         if os.path.isfile(self.output_vcf) and os.stat(self.output_vcf).st_size != 0:
-            os.remove(tmp_out) # remove the original unsorted vcf
+            os.remove(tmp_out)  # remove the original unsorted vcf
             # sorting file
             if os.path.exists(tmp_out + ".sort.tmp"):
                 os.remove(tmp_out + ".sort.tmp")
 
+
 class IntermediateFile(object):
     def __init__(self, output_dir: str, as_dev=False):
         self.output_dir = output_dir
         self.logger = logger.setup_log(__name__, as_dev)
 
     @staticmethod
     def convert_genome_info_to_dictionary(genome_info: dict):
@@ -238,15 +256,14 @@
     def convert_candidates_to_dictionary(candidates: dict):
         tmp_candidates_dict = dict([(key, []) for key in candidates.keys()])
         for key, candidates in candidates.items():
             tmp_candidates = []
             tmp_candidates_dict[key] = tmp_candidates
             for candidate in candidates:
                 tmp_dict = dict(candidate.__dict__)
-                tmp_dict = {k: v for k, v in tmp_dict.items() if v}
                 for key, value in tmp_dict.items():
                     if isinstance(value, set):
                         tmp_dict[key] = list(value)
                 #tmp_dict.pop('logger')
                 tmp_candidates.append(tmp_dict)
         return tmp_candidates_dict
```

### Comparing `spectre-cnv-0.2.0/spectre/util/timing_dev.py` & `spectre_cnv-0.2.1/spectre/util/timing_dev.py`

 * *Files identical despite different names*

### Comparing `spectre-cnv-0.2.0/spectre/util/vcf_parser.py` & `spectre_cnv-0.2.1/spectre/util/vcf_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,18 @@
                             af_index = format_.split(":").index("AF")
                             af = float(sample_.split(":")[af_index])
                             # self.logger.debug("like clair3")
                         except ValueError:
                             if format_.__contains__("VAF"):
                                 # pepper-margin-deepvariant
                                 af_index = format_.split(":").index("VAF")
-                                af = float(sample_.split(":")[af_index])
+                                try:
+                                    af = float(sample_.split(":")[af_index])
+                                except ValueError:
+                                    continue
                                 # self.logger.debug("like pepper-margin-deepvariant")
                             else:
                                 pass
                     elif info_.__contains__("AC"):
                         # longshot
                         ac = list(filter(lambda x: "AC" in x, info_.split(";")))[0].split("=")[1]
                         [ref_count, alt_count] = ac.split(",")
```

### Comparing `spectre-cnv-0.2.0/spectre_cnv.egg-info/PKG-INFO` & `spectre_cnv-0.2.1/spectre_cnv.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: spectre-cnv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Long read copy number variation (CNV) caller
 Home-page: https://github.com/fritzsedlazeck/Spectre
 Author: Philippe Sanio
 Author-email: philippe.sanio@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
-Requires-Dist: pysam==0.22.0
-Requires-Dist: numpy==1.24.3
-Requires-Dist: pandas==2.0.1
-Requires-Dist: matplotlib==3.7.1
-Requires-Dist: scipy==1.10.1
+Requires-Dist: pysam>=0.22.0
+Requires-Dist: numpy>=1.24.3
+Requires-Dist: pandas>=2.0.1
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: scipy>=1.10.1
 
 
 ![Spectre](./logo.png)
 # Spectre - Long read CNV caller
 Spectre is a long read copy number variation (CNV) caller. 
 Spectre is designed to detect large CNVs (>100kb) in a couple of minutes depending on your hardware.
 
@@ -26,20 +26,29 @@
 Additionally, Spectre can use the breakpoint (SNF) data from Sniffles to improve the CNV calling. However, it has to be converted to the SNFJ format using [snf2json](https://github.com/philippesanio/snf2json).
 
 
 The CNV output of Spectre is stored in three files, VCF, BED and .SPC which can be used in the population mode.
 
 Furthermore, Spectre offers a population mode, which can be used to search for CNV support in multiple samples. 
 Compared to other tools, Spectre searches not only in the final CNVs but also in CNV candidates which did not qualify for the final output of Spectre.
-## Required programs (conda)
+## Install Spectre
+Tested on **Python** version: **3.11** and **3.10**
 
 Install Spectre with Pip:
 ```bash
 pip install spectre-cnv
 ```
+Get the latest changes by building Spectre from source on your own and install it locally in your conda environment.
+```bash
+pip install build
+git clone https://github.com/fritzsedlazeck/Spectre.git
+cd ./Spectre
+python3 -m build
+pip install dist/spectre_cnv-<VERSION>.tar.gz # replace <VERSION> with e.g. 0.2.0
+```
 
 Setup a conda environment for Spectre (copy and paste the following commands)
 ```bash
 conda create -n spectre python=3.10 pysam==0.22.0 numpy==1.24.3 pandas==2.0.1 matplotlib==3.7.1 scipy==1.10.1 -y
 conda activate spectre
 ```
 Alternatively, you can use pip for installing the packages stored in the requirements txt
@@ -79,14 +88,15 @@
 - Reference genome (can be bgzip compressed)
 
 Optional
 - **MDR** file (if not already generated, Spectre will do that for you. You can also use the MDR file for every sample which has been aligned to the same reference genome)
 - VCF file containing SNV
 - SNF data from Sniffles (if parsed through [snf2json](https://github.com/philippesanio/snf2json))
 
+
 ## Run Spectre
 ### MDR file
 MDR files hold the information of N regions in the reference genome and restrict Spectre of using data from those regions. 
 We are providing sample MDR files for the reference genomes GRCh37 and GRCh38.
 
 If not provided, Spectre will generate a MDR file for you, which can take some time. 
 Thus, we highly recommend to generate a MDR file for your reference genome before running Spectre on multiple samples which have been aligned to the same reference.
@@ -112,22 +122,25 @@
   --coverage mosdepth/sampleid/mosdepth.regions.bed.gz \
   --sample-id sampleid \
   --output-dir sampleid_output_directory_path/ \
   --reference reference.fasta.gz
 ```
 ### Run Spectre with multiple samples
 Run Spectre with multiple samples:
->INFO: This will start the population mode automatically.
+>INFO: This will start the population mode automatically. All provided settings will be applied to all samples.
+
+>NOTE: If population flag is not set, Spectre will run in single sample mode. Thus, calculating only CNVs for the first sample. 
 
 ```bash
 spectre.py CNVCaller \
   --coverage mosdepth/sampleid-1/mosdepth.regions.bed.gz mosdepth/sampleid-2/mosdepth.regions.bed.gz \
   --sample-id sampleid-1 sampleid-2 \
   --output-dir sampleid_output_directory_path/ \
   --reference reference.fasta.gz
+  --population
 ```
 
 ### Population mode
 Run Spectre in population mode with two or more samples:
 >INFO: Spectre produces an intermediate file (.spc) which contains all calculated CNVs from a given samples. They are 
 > located in the output folder of given sample.
 
@@ -137,67 +150,79 @@
   --sample-id output_name \
   --output-dir sampleid_output_directory_path/
 ```
 
 
 ### Help
 ```
-Spectre:
+vcf_utils <command> [<args>]
+    Spectre:
         CNVCaller:
-            Required
+            [Required]
                 --coverage     Path to the coverage file from Mosdepth output. Expects the following files:
                                    <prefix>.regions.bed.gz
                                    <prefix>.regions.bed.gz.csi
-                               Can be one or more directories. Example:
+                               Can be one or more paths. However, providing multiple samples is only intended to
+                               work with the --population flag. Example:
                                     --coverage /path/md1.regions.gz /path/md2.regions.gz
-                --sample-id    Sample name/ID. Can be one or more ID. Example:
+                --sample-id    Sample name/ID. Can be one or more ID. However, providing multiple sample ids is only
+                               intended to work with the --population flag. Example:
                                     --sample-id id1 id2
                 --output-dir   Output directory
                 --reference    Reference sequence used for mapping (for N removal)
-            Optional, if missing it will be created
-                --metadata     Metadata file for Ns removal
-            Optional
+            [Optional, if missing it will be created]
+                --metadata     Metadata file for Ns removal (this will speed up Spectre massively if provided)
+                --n-size       Required amount of consecutive Ns to be considered an NRegion 
+                               in the reference sequence (Default = 5)
+
+            [Optional]
                 --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
-                --only-chr     Comma separated list of chromosomes to use
+                --only-chr     Comma separated list of chromosomes to use (e.g. chr1,chr2,chr3)
                 --ploidy       Set the ploidy for the analysis, useful for sex chromosomes (Default = 2)
                 --ploidy-chr   Comma separated list of key:value-pairs for individual chromosome ploidy control
                                (e.g. chrX:2,chrY:1) If chromosome is not specified, the default ploidy will be used.
-                --snv          VCF file containing the SNV for the same sample CNV want to be called
                 --snfj         Breakpoints from from Sniffle which has been converted from the SNF to the SNFJ format.
-                --n-size       Length of consecutive Ns (Default = 5)
+                               SNFJ files can be generated using the program snf2json.
                 --min-cnv-len  Minimum length of CNV (Default 100kb)
-                --cancer       Set this flag if the sample is cancer (Default = False)
-                --population   Runs the population mode on all provided samples
-                --threads      Amount of threads (This will boost performance if multiple samples are provided)
+                --snv          VCF file containing the SNV for the same sample CNV want to be called
+                --cancer       Set this flag if the sample is cancer (Default = False) This will disable some safety 
+                               checks, when determining the DEL and DUP thresholds. 
 
-                Coverage
+            [Optional, Coverage]
                 --sample-coverage-overwrite     Overwrites the calculated sample coverage, which is used to normalize
                                                 the coverage. e.g. a value of 30 equals to 30X coverage.
                 --disable-max-coverage          Disables the maximum coverage check. This will allow to call CNVs
 
-                LoH (requires --snv)
+            [Optional, LoH (requires --snv)]
                 --loh-min-snv-perkb             Minimum number of SNVs per kilobase for an LoH region (default=5)
                 --loh-min-snv-total             Minimum number of SNVs total for an LoH region (default=100)
                 --loh-min-region-size           Minimum size of a region for a LoH region (default=100000)
 
-
+                --population   Runs the population mode on all provided samples. It will apply all the provided
+                               configurations as well as the default population mode values to all samples.
+                --threads      Amount of threads (This will boost performance if multiple samples are provided)
         RemoveNs:
-            Required
+            [Required]
                 --reference    Reference genome used for mapping
                 --output-dir   Output dir
                 --output-file  Output file for results
-                --bin-size     Bin/Window size (same as Mosdepth)
-            Optional
-                --blacklist    Blacklist in bed format for sites that will be ignored (Default = "")
-                --n-size       Length of consecutive Ns (Default = 5)
-                --save-only    Will only save the metadata file and not show the results in screen (Default = False)
+            [Optional]
+                --n-size       Required amount of consecutive Ns to be considered an NRegion 
+                               in the reference sequence (Default = 5)
+                --save-only    Will only save the metadata file and not show the results on screen (Default = False)
 
         Population:
-            Required
-                --candidates   At least 2 candidate files (.spc or .vcf) which should be taken into consideration for the population mode.
-                --sample-id    Name of the output file
-                --output-dir   Output directory
-            Optional
-                --reference    Reference sequence (Required if VCF files are used!)
+            [Required]
+                --candidates   At least 2 .spc sample files which should be used in the population mode.
+                               (e.g. sample1.spc sample2.spc)
+                --sample-id    The name of the sample-id will be added accordingly at the output.
+                               (e.g. population_mode_<sample-id>.vcf.gz)
+                --output-dir   Path of the output directory
+            [Optional]
+                --reference    Reference sequence
+                --reciprocal-overlap        Minimum reciprocal overlap for supporting CNVs [0.0 - 1.0] (Default = 0.8)
+                --disable-quality-filter    Disables the quality filter for the population mode. Spectre will also
+                                            search for supporting CNVs in the .SPC files, which have not been reported
+                                            as final CNVs in the VCF and BED file.
         Version:
             version    Shows current version/build
 ```
```

### Comparing `spectre-cnv-0.2.0/spectre_cnv.egg-info/SOURCES.txt` & `spectre_cnv-0.2.1/spectre_cnv.egg-info/SOURCES.txt`

 * *Files identical despite different names*


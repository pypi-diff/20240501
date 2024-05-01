# Comparing `tmp/dataretrieval-1.0.7.tar.gz` & `tmp/dataretrieval-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataretrieval-1.0.7.tar", last modified: Sun Apr 28 16:10:07 2024, max compression
+gzip compressed data, was "dataretrieval-1.0.8.tar", last modified: Wed May  1 16:53:07 2024, max compression
```

## Comparing `dataretrieval-1.0.7.tar` & `dataretrieval-1.0.8.tar`

### file list

```diff
@@ -1,143 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.671178 dataretrieval-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.575177 dataretrieval-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.github/workflows/sphinx-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.575177 dataretrieval-1.0.7/.gitlab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/.gitlab/issue_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.gitlab/issue_templates/reviewer_checklist.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/.gitlab/merge_request_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.gitlab/merge_request_templates/reviewer_checklist.md
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/.prettierrc.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-28 16:10:07.671178 dataretrieval-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/code.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/dataretrieval/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/dataretrieval/codes/
--rwxr-xr-x   0 runner    (1001) docker     (127)       47 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/codes/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/codes/timezones.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/nadp.py
--rw-r--r--   0 runner    (1001) docker     (127)    18261 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/nldi.py
--rw-r--r--   0 runner    (1001) docker     (127)    51276 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/nwis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/streamstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/waterwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    15116 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/dataretrieval/wqp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.667178 dataretrieval-1.0.7/dataretrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 16:10:07.000000 dataretrieval-1.0.7/dataretrieval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.583177 dataretrieval-1.0.7/demos/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9869 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/NWIS_demo_1.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)    13027 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/R Python Vignette equivalents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.587177 dataretrieval-1.0.7/demos/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)   535225 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/datasets/peak_discharge_trends.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.587177 dataretrieval-1.0.7/demos/hydroshare/
--rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.587177 dataretrieval-1.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.587177 dataretrieval-1.0.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.591177 dataretrieval-1.0.7/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_DailyValues_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_GroundwaterLevels_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_Measurements_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_ParameterCodes_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_Peaks_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_Ratings_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_SiteInfo_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_SiteInventory_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_Statistics_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_UnitValues_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_WaterSamples_Examples.nblink
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/USGS_dataretrieval_WaterUse_Examples.nblink
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.591177 dataretrieval-1.0.7/docs/source/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)   535225 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/datasets/peak_discharge_trends.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/nwisdemo01.nblink
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/readme_examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/rvignettes.nblink
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/examples/siteinfo_examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.595177 dataretrieval-1.0.7/docs/source/meta/
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/meta/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/meta/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/meta/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.595177 dataretrieval-1.0.7/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/nadp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/nwis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/streamstats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/waterwatch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/reference/wqp.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.595177 dataretrieval-1.0.7/docs/source/userguide/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/userguide/dataportals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/userguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/docs/source/userguide/timeconventions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:10:07.671178 dataretrieval-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.595177 dataretrieval-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:10:07.667178 dataretrieval-1.0.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_basin.json
--rw-r--r--   0 runner    (1001) docker     (127)    26880 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_features_by_comid.json
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_features_by_feature_source_with_nav_mode.json
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_features_by_feature_source_without_nav_mode.json
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_features_by_lat_long.json
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_flowlines.json
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nldi_get_flowlines_by_comid.json
--rwxr-xr-x   0 runner    (1001) docker     (127)    22920 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/nwis_sites.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    48992 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/water_use_allegheny.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2485 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/water_use_national.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    14065 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterdata_measurements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterdata_pmcodes.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)  5998995 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterdata_qwdata.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    14869 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterservices_dv.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3221 2024-04-28 16:09:54.000000 dataretrieval-1.0.7/tests/data/waterservices_gwlevels.txt
--rwxr-xr-x   0 runner    (1001) docker     (127) 22180871 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_iv.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_peaks.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2323 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_ratings.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1447 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_site.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   198769 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/waterservices_stats.txt
--rw-r--r--   0 runner    (1001) docker     (127) 21772141 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_activities.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_activity_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1442378 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_detection_limits.txt
--rw-r--r--   0 runner    (1001) docker     (127)   436730 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_habitat_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_organizations.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1029205 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_project_weights.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28500 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_projects.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3155 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_results.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)  2276131 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/data/wqp_sites.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/nadp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/nldi_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/nwis_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22144 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/waterservices_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7787 2024-04-28 16:09:55.000000 dataretrieval-1.0.7/tests/wqp_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.873123 dataretrieval-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.781122 dataretrieval-1.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.785122 dataretrieval-1.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.github/workflows/sphinx-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.781122 dataretrieval-1.0.8/.gitlab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.785122 dataretrieval-1.0.8/.gitlab/issue_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.gitlab/issue_templates/reviewer_checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.785122 dataretrieval-1.0.8/.gitlab/merge_request_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.gitlab/merge_request_templates/reviewer_checklist.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-01 16:53:07.873123 dataretrieval-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/code.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.785122 dataretrieval-1.0.8/dataretrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 16:53:07.000000 dataretrieval-1.0.8/dataretrieval/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.789122 dataretrieval-1.0.8/dataretrieval/codes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       47 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/codes/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/codes/timezones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/nadp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18261 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/nldi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51276 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/streamstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/waterwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15116 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/dataretrieval/wqp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.869123 dataretrieval-1.0.8/dataretrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-01 16:53:07.000000 dataretrieval-1.0.8/dataretrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-01 16:53:07.000000 dataretrieval-1.0.8/dataretrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:53:07.000000 dataretrieval-1.0.8/dataretrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-01 16:53:07.000000 dataretrieval-1.0.8/dataretrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 16:53:07.000000 dataretrieval-1.0.8/dataretrieval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.789122 dataretrieval-1.0.8/demos/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9869 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/NWIS_demo_1.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13027 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/R Python Vignette equivalents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.789122 dataretrieval-1.0.8/demos/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)   535225 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/datasets/peak_discharge_trends.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.789122 dataretrieval-1.0.8/demos/hydroshare/
+-rw-r--r--   0 runner    (1001) docker     (127)     9236 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9860 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.793122 dataretrieval-1.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.793122 dataretrieval-1.0.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.793122 dataretrieval-1.0.8/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_DailyValues_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_GroundwaterLevels_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_Measurements_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_ParameterCodes_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_Peaks_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_Ratings_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_SiteInfo_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_SiteInventory_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_Statistics_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_UnitValues_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_WaterSamples_Examples.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/USGS_dataretrieval_WaterUse_Examples.nblink
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.793122 dataretrieval-1.0.8/docs/source/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)   535225 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/datasets/peak_discharge_trends.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/nwisdemo01.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/readme_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/rvignettes.nblink
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/examples/siteinfo_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.797122 dataretrieval-1.0.8/docs/source/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/meta/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/meta/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/meta/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.797122 dataretrieval-1.0.8/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/reference/nadp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/reference/nwis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/reference/streamstats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/reference/wqp.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.797122 dataretrieval-1.0.8/docs/source/userguide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/userguide/dataportals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/userguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/docs/source/userguide/timeconventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:53:07.873123 dataretrieval-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.801122 dataretrieval-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:53:07.865123 dataretrieval-1.0.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/nldi_get_basin.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26880 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/nldi_get_features_by_comid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/nldi_get_features_by_feature_source_with_nav_mode.json
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/nldi_get_features_by_feature_source_without_nav_mode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/nldi_get_features_by_lat_long.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/nldi_get_flowlines.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/nldi_get_flowlines_by_comid.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22920 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/nwis_sites.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48992 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/water_use_allegheny.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2485 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/water_use_national.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14065 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterdata_measurements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterdata_pmcodes.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)  5998995 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterdata_qwdata.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14869 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterservices_dv.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3221 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterservices_gwlevels.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127) 22180871 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterservices_iv.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterservices_peaks.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2323 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterservices_ratings.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1447 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterservices_site.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   198769 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/waterservices_stats.txt
+-rw-r--r--   0 runner    (1001) docker     (127) 21772141 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/wqp_activities.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/wqp_activity_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1442378 2024-05-01 16:52:55.000000 dataretrieval-1.0.8/tests/data/wqp_detection_limits.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   436730 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/data/wqp_habitat_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/data/wqp_organizations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1029205 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/data/wqp_project_weights.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28500 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/data/wqp_projects.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3155 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/data/wqp_results.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2276131 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/data/wqp_sites.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/nadp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/nldi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/nwis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22144 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/waterservices_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7787 2024-05-01 16:52:56.000000 dataretrieval-1.0.8/tests/wqp_test.py
```

### Comparing `dataretrieval-1.0.7/.github/workflows/python-package.yml` & `dataretrieval-1.0.8/.github/workflows/python-package.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Python package
 
 on:
   push:
+    branches: ['master']
   pull_request:
+    branches: ['master']
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest]
-        python-version: [3.8, 3.9, '3.10', 3.11]
+        python-version: [3.8, 3.9, '3.10', 3.11, 3.12]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `dataretrieval-1.0.7/.github/workflows/python-publish.yml` & `dataretrieval-1.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/.github/workflows/sphinx-docs.yml` & `dataretrieval-1.0.8/.github/workflows/sphinx-docs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         with:
           persist-credentials: false
       - name: Install dataretrieval, dependencies, and Sphinx then build docs
         shell: bash -l {0}
         run: |
           python -m pip install --upgrade pip
           pip install .[doc]
+          ipython kernel install --name "python3" --user
           sudo apt update -y && sudo apt install -y latexmk texlive-latex-recommended texlive-latex-extra texlive-fonts-recommended dvipng pandoc
           (cd docs && make docs)
           (cd docs && make html)
       - name: Debug
         run: |
           echo $REF
           echo $EVENT_NAME
```

### Comparing `dataretrieval-1.0.7/.gitignore` & `dataretrieval-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/.gitlab/issue_templates/reviewer_checklist.md` & `dataretrieval-1.0.8/.gitlab/issue_templates/reviewer_checklist.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/.gitlab/merge_request_templates/reviewer_checklist.md` & `dataretrieval-1.0.8/.gitlab/merge_request_templates/reviewer_checklist.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/.pre-commit-config.yaml` & `dataretrieval-1.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/CONTRIBUTING.md` & `dataretrieval-1.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/DISCLAIMER.md` & `dataretrieval-1.0.8/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/LICENSE.md` & `dataretrieval-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/PKG-INFO` & `dataretrieval-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataretrieval
-Version: 1.0.7
+Version: 1.0.8
 Summary: Discover and retrieve water data from U.S. federal hydrologic web services.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -64,17 +64,20 @@
 Requires-Dist: pytest>5.0.0; extra == "test"
 Requires-Dist: pytest-cov[all]; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: requests-mock; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: nbsphinx_link; extra == "doc"
+Requires-Dist: ipython; extra == "doc"
+Requires-Dist: ipykernel; extra == "doc"
+Requires-Dist: matplotlib; extra == "doc"
 Provides-Extra: nldi
 Requires-Dist: geopandas>=0.10; extra == "nldi"
 
 # dataretrieval: Download hydrologic data
 
 :warning: USGS data availability and format are changing on Water Quality Portal (WQP). Beginning in February 2024 data obtained from WQP legacy profiles will not include new USGS data or recent updates to existing data. 
 To view the status of changes in data availability and code functionality, visit: https://doi-usgs.github.io/dataRetrieval/articles/Status.html
```

### Comparing `dataretrieval-1.0.7/README.md` & `dataretrieval-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/code.json` & `dataretrieval-1.0.8/code.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/codes/states.py` & `dataretrieval-1.0.8/dataretrieval/codes/states.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/codes/timezones.py` & `dataretrieval-1.0.8/dataretrieval/codes/timezones.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/nadp.py` & `dataretrieval-1.0.8/dataretrieval/nadp.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/nldi.py` & `dataretrieval-1.0.8/dataretrieval/nldi.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/nwis.py` & `dataretrieval-1.0.8/dataretrieval/nwis.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/streamstats.py` & `dataretrieval-1.0.8/dataretrieval/streamstats.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/utils.py` & `dataretrieval-1.0.8/dataretrieval/utils.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/waterwatch.py` & `dataretrieval-1.0.8/dataretrieval/waterwatch.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval/wqp.py` & `dataretrieval-1.0.8/dataretrieval/wqp.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/dataretrieval.egg-info/PKG-INFO` & `dataretrieval-1.0.8/dataretrieval.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataretrieval
-Version: 1.0.7
+Version: 1.0.8
 Summary: Discover and retrieve water data from U.S. federal hydrologic web services.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -64,17 +64,20 @@
 Requires-Dist: pytest>5.0.0; extra == "test"
 Requires-Dist: pytest-cov[all]; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: requests-mock; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
-Requires-Dist: sphinx_rtd_theme; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: nbsphinx_link; extra == "doc"
+Requires-Dist: ipython; extra == "doc"
+Requires-Dist: ipykernel; extra == "doc"
+Requires-Dist: matplotlib; extra == "doc"
 Provides-Extra: nldi
 Requires-Dist: geopandas>=0.10; extra == "nldi"
 
 # dataretrieval: Download hydrologic data
 
 :warning: USGS data availability and format are changing on Water Quality Portal (WQP). Beginning in February 2024 data obtained from WQP legacy profiles will not include new USGS data or recent updates to existing data. 
 To view the status of changes in data availability and code functionality, visit: https://doi-usgs.github.io/dataRetrieval/articles/Status.html
```

### Comparing `dataretrieval-1.0.7/dataretrieval.egg-info/SOURCES.txt` & `dataretrieval-1.0.8/dataretrieval.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 docs/source/meta/installing.rst
 docs/source/meta/license.rst
 docs/source/reference/index.rst
 docs/source/reference/nadp.rst
 docs/source/reference/nwis.rst
 docs/source/reference/streamstats.rst
 docs/source/reference/utils.rst
-docs/source/reference/waterwatch.rst
 docs/source/reference/wqp.rst
 docs/source/userguide/dataportals.rst
 docs/source/userguide/index.rst
 docs/source/userguide/timeconventions.rst
 tests/__init__.py
 tests/nadp_test.py
 tests/nldi_test.py
```

### Comparing `dataretrieval-1.0.7/demos/NWIS_demo_1.ipynb` & `dataretrieval-1.0.8/demos/NWIS_demo_1.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/R Python Vignette equivalents.ipynb` & `dataretrieval-1.0.8/demos/R Python Vignette equivalents.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/datasets/peak_discharge_trends.csv` & `dataretrieval-1.0.8/demos/datasets/peak_discharge_trends.csv`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_DailyValues_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_GroundwaterLevels_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_Measurements_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_ParameterCodes_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_Peaks_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_Ratings_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_SiteInfo_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_SiteInventory_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_Statistics_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_UnitValues_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_WaterSamples_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb` & `dataretrieval-1.0.8/demos/hydroshare/USGS_dataretrieval_WaterUse_Examples.ipynb`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/Makefile` & `dataretrieval-1.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/conf.py` & `dataretrieval-1.0.8/docs/source/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # Since we aren't installing package here, we mock imports of the dependencies.
 
 # Relative paths so documentation can reference and include demos folder
 import os
@@ -28,15 +26,15 @@
     'sphinx.ext.autosummary',
     'sphinx.ext.napoleon',
     'sphinx.ext.todo',
     'sphinx.ext.coverage',
     'sphinx.ext.viewcode',
     'sphinx.ext.githubpages',
     'nbsphinx',
-    'nbsphinx_link'
+    'nbsphinx_link',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # suffix of source documents
 source_suffix = '.rst'
@@ -81,15 +79,15 @@
 
 # Autosummary / Automodapi settings
 autosummary_generate = True
 automodapi_inheritance_diagram = False
 autodoc_default_options = {
     'members': True,
     'inherited-members': False,
-    'private-members': True
+    'private-members': True,
 }
 
 # doctest
 doctest_global_setup = '''
 import dataretrieval
 import numpy as np
 import pandas as pd
@@ -104,25 +102,28 @@
 html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 
 html_theme_options = {
-    "logo_only": False,
-    "display_version": True,
+    'logo_only': False,
+    'display_version': True,
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # -- Options for linkcheck -------------------------------------------
 
 # Links to not "check" because they are problematic for the link checker
 linkcheck_ignore = [
     r'https://streamstats.usgs.gov/streamstatsservices/#/',
     r'https://www.waterqualitydata.us/public_srsnames/',
     r'https://waterqualitydata.us',
-    r'https://github.com/USGS-python/dataretrieval/tree/master/demos/hydroshare'
+    r'https://github.com/USGS-python/dataretrieval/tree/master/demos/hydroshare',
 ]
+
+# Some notebooks have warnings, which nbsphinx should ignore
+nbsphinx_allow_errors = True
```

### Comparing `dataretrieval-1.0.7/docs/source/examples/datasets/peak_discharge_trends.csv` & `dataretrieval-1.0.8/docs/source/examples/datasets/peak_discharge_trends.csv`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/examples/index.rst` & `dataretrieval-1.0.8/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/examples/readme_examples.rst` & `dataretrieval-1.0.8/docs/source/examples/readme_examples.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/examples/siteinfo_examples.rst` & `dataretrieval-1.0.8/docs/source/examples/siteinfo_examples.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/index.rst` & `dataretrieval-1.0.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/meta/contributing.rst` & `dataretrieval-1.0.8/docs/source/meta/contributing.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/meta/installing.rst` & `dataretrieval-1.0.8/docs/source/meta/installing.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/meta/license.rst` & `dataretrieval-1.0.8/docs/source/meta/license.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/docs/source/userguide/dataportals.rst` & `dataretrieval-1.0.8/docs/source/userguide/dataportals.rst`

 * *Files 22% similar despite different names*

```diff
@@ -17,11 +17,9 @@
 +-----------------------------------+---------------------------------------------------------------+
 | Mercury Deposition Network        | https://nadp.slh.wisc.edu/networks/mercury-deposition-network |
 +-----------------------------------+---------------------------------------------------------------+
 | Streamstats                       | https://streamstats.usgs.gov                                  |
 +-----------------------------------+---------------------------------------------------------------+
 | Water Quality Portal              | https://waterqualitydata.us                                   |
 +-----------------------------------+---------------------------------------------------------------+
-| WaterWatch                        | https://waterwatch.usgs.gov                                   |
-+-----------------------------------+---------------------------------------------------------------+
 | Water Services                    | https://waterservices.usgs.gov                                |
-+-----------------------------------+---------------------------------------------------------------+
++-----------------------------------+---------------------------------------------------------------+
```

### Comparing `dataretrieval-1.0.7/docs/source/userguide/timeconventions.rst` & `dataretrieval-1.0.8/docs/source/userguide/timeconventions.rst`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/pyproject.toml` & `dataretrieval-1.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -30,17 +30,20 @@
   "pytest-cov[all]",
   "coverage",
   "requests-mock",
   "flake8",
 ]
 doc = [
   "sphinx",
-  "sphinx_rtd_theme",
+  "sphinx-rtd-theme",
   "nbsphinx",
   "nbsphinx_link",
+  "ipython",
+  "ipykernel",
+  "matplotlib",
 ]
 nldi = [
   'geopandas>=0.10'
 ]
 
 [project.urls]
 homepage = "https://github.com/DOI-USGS/dataretrieval-python"
```

### Comparing `dataretrieval-1.0.7/tests/data/nldi_get_basin.json` & `dataretrieval-1.0.8/tests/data/nldi_get_basin.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/nldi_get_features_by_comid.json` & `dataretrieval-1.0.8/tests/data/nldi_get_features_by_comid.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/nldi_get_features_by_feature_source_with_nav_mode.json` & `dataretrieval-1.0.8/tests/data/nldi_get_features_by_feature_source_with_nav_mode.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/nldi_get_features_by_feature_source_without_nav_mode.json` & `dataretrieval-1.0.8/tests/data/nldi_get_features_by_feature_source_without_nav_mode.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/nldi_get_features_by_lat_long.json` & `dataretrieval-1.0.8/tests/data/nldi_get_features_by_lat_long.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/nldi_get_flowlines.json` & `dataretrieval-1.0.8/tests/data/nldi_get_flowlines.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/nldi_get_flowlines_by_comid.json` & `dataretrieval-1.0.8/tests/data/nldi_get_flowlines_by_comid.json`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/nwis_sites.txt` & `dataretrieval-1.0.8/tests/data/nwis_sites.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/water_use_allegheny.txt` & `dataretrieval-1.0.8/tests/data/water_use_allegheny.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/water_use_national.txt` & `dataretrieval-1.0.8/tests/data/water_use_national.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterdata_measurements.txt` & `dataretrieval-1.0.8/tests/data/waterdata_measurements.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterdata_qwdata.txt` & `dataretrieval-1.0.8/tests/data/waterdata_qwdata.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterservices_dv.txt` & `dataretrieval-1.0.8/tests/data/waterservices_dv.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterservices_gwlevels.txt` & `dataretrieval-1.0.8/tests/data/waterservices_gwlevels.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterservices_iv.txt` & `dataretrieval-1.0.8/tests/data/waterservices_iv.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterservices_peaks.txt` & `dataretrieval-1.0.8/tests/data/waterservices_peaks.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterservices_ratings.txt` & `dataretrieval-1.0.8/tests/data/waterservices_ratings.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterservices_site.txt` & `dataretrieval-1.0.8/tests/data/waterservices_site.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/waterservices_stats.txt` & `dataretrieval-1.0.8/tests/data/waterservices_stats.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_activities.txt` & `dataretrieval-1.0.8/tests/data/wqp_activities.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_activity_metrics.txt` & `dataretrieval-1.0.8/tests/data/wqp_activity_metrics.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_detection_limits.txt` & `dataretrieval-1.0.8/tests/data/wqp_detection_limits.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_habitat_metrics.txt` & `dataretrieval-1.0.8/tests/data/wqp_habitat_metrics.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_organizations.txt` & `dataretrieval-1.0.8/tests/data/wqp_organizations.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_project_weights.txt` & `dataretrieval-1.0.8/tests/data/wqp_project_weights.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_projects.txt` & `dataretrieval-1.0.8/tests/data/wqp_projects.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_results.txt` & `dataretrieval-1.0.8/tests/data/wqp_results.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/data/wqp_sites.txt` & `dataretrieval-1.0.8/tests/data/wqp_sites.txt`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/nadp_test.py` & `dataretrieval-1.0.8/tests/nadp_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/nldi_test.py` & `dataretrieval-1.0.8/tests/nldi_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/nwis_test.py` & `dataretrieval-1.0.8/tests/nwis_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/utils_test.py` & `dataretrieval-1.0.8/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/waterservices_test.py` & `dataretrieval-1.0.8/tests/waterservices_test.py`

 * *Files identical despite different names*

### Comparing `dataretrieval-1.0.7/tests/wqp_test.py` & `dataretrieval-1.0.8/tests/wqp_test.py`

 * *Files identical despite different names*


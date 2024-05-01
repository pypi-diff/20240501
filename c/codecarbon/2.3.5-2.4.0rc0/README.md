# Comparing `tmp/codecarbon-2.3.5.tar.gz` & `tmp/codecarbon-2.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecarbon-2.3.5.tar", last modified: Wed Apr 10 07:19:31 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `codecarbon-2.3.5.tar` & `codecarbon-2.4.0rc0.tar`

### file list

```diff
@@ -1,128 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.858790 codecarbon-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 07:19:23.000000 codecarbon-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-10 07:19:31.858790 codecarbon-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-10 07:19:23.000000 codecarbon-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.838790 codecarbon-2.3.5/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.838790 codecarbon-2.3.5/carbonserver/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.838790 codecarbon-2.3.5/carbonserver/carbonserver/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.838790 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/domain/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.842790 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.842790 codecarbon-2.3.5/carbonserver/carbonserver/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/database/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/carbonserver/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-10 07:19:23.000000 codecarbon-2.3.5/carbonserver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.842790 codecarbon-2.3.5/codecarbon/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.842790 codecarbon-2.3.5/codecarbon/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/powermetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/rapl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.834790 codecarbon-2.3.5/codecarbon/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/data/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/cloud/impact.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/data/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)    49665 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/hardware/cpu_power.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/data/private_infra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.846790 codecarbon-2.3.5/codecarbon/data/private_infra/2016/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0 runner    (1001) docker     (127)    49591 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (127)    46544 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/emissions_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.850790 codecarbon-2.3.5/codecarbon/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/geography.py
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/external/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.850790 codecarbon-2.3.5/codecarbon/prometheus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/prometheus/metric_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.850790 codecarbon-2.3.5/codecarbon/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.850790 codecarbon-2.3.5/codecarbon/viz/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    29734 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    29874 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/carbonboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28035 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-04-10 07:19:23.000000 codecarbon-2.3.5/codecarbon/viz/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.854790 codecarbon-2.3.5/codecarbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 07:19:31.000000 codecarbon-2.3.5/codecarbon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:19:31.858790 codecarbon-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-10 07:19:23.000000 codecarbon-2.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:19:31.854790 codecarbon-2.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_api_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_core_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_emissions_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_emissions_tracker_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_emissions_tracker_flush.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_geography.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_logging_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_powermetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_ram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_tracking_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/test_viz_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/testdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-10 07:19:23.000000 codecarbon-2.3.5/tests/testutils.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/_version.py
+-rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/emissions_tracker.py
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/input.py
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/cli/__init__.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/cli/cli_utils.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/__init__.py
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/api_client.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/cloud.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/co2_signal.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/config.py
+-rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/cpu.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/emissions.py
+-rw-r--r--   0        0        0    10300 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/gpu.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/measure.py
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/powermetrics.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/rapl.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/schemas.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/units.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/core/util.py
+-rw-r--r--   0        0        0   409749 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/canada_provinces.geojson
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/cloud/impact.csv
+-rw-r--r--   0        0        0    49714 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/hardware/cpu_power.csv
+-rw-r--r--   0        0        0    49131 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2023-07-07-22-40-48.png
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0        0        0    49591 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/our_world_in_data-2022_data.ipynb
+-rw-r--r--   0        0        0   420635 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/world_energy_mix.csv
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0        0        0    48072 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/global_energy_mix-old.json
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0        0        0    42145 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/01_get_world_carbon_intensity.ipynb
+-rw-r--r--   0        0        0    29597 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/02_convert_csv_to_json.ipynb
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/03_add_eu_data.ipynb
+-rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/data/private_infra/2020/eu-carbon-intensity-electricity.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/__init__.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/geography.py
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/hardware.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/logger.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/scheduler.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/external/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/prometheus/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/prometheus/metric_definitions.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/prometheus/prometheus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/__init__.py
+-rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/carbonboard.py
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0        0        0    28035 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/components.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0        0        0    25442 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0        0        0    29734 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0        0        0    29874 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/.gitignore
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/LICENSE
+-rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/README.md
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 codecarbon-2.4.0rc0/PKG-INFO
```

### Comparing `codecarbon-2.3.5/LICENSE` & `codecarbon-2.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/PKG-INFO` & `codecarbon-2.4.0rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: codecarbon
-Version: 2.3.5
+Version: 2.4.0rc0
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: arrow
+Requires-Dist: click
 Requires-Dist: pandas
-Requires-Dist: pynvml
-Requires-Dist: requests
+Requires-Dist: prometheus-client
 Requires-Dist: psutil
 Requires-Dist: py-cpuinfo
+Requires-Dist: pynvml
 Requires-Dist: rapidfuzz
-Requires-Dist: click
-Requires-Dist: prometheus_client
+Requires-Dist: requests
 Provides-Extra: viz
-Requires-Dist: dash; extra == "viz"
-Requires-Dist: dash_bootstrap_components<1.0.0; extra == "viz"
-Requires-Dist: fire; extra == "viz"
-Provides-Extra: dashboard
-Requires-Dist: dash>=2.2.0; extra == "dashboard"
-Requires-Dist: plotly>=5.6.0; extra == "dashboard"
-Requires-Dist: dash_bootstrap_components; extra == "dashboard"
+Requires-Dist: dash; extra == 'viz'
+Requires-Dist: dash-bootstrap-components<1.0.0; extra == 'viz'
+Requires-Dist: fire; extra == 'viz'
+Description-Content-Type: text/markdown
 
 ![banner](docs/edit/images/banner.png)
 
 Estimate and track carbon emissions from your computer, quantify and analyze their impact.
 
 [**Documentation**](https://mlco2.github.io/codecarbon)
```

### Comparing `codecarbon-2.3.5/README.md` & `codecarbon-2.4.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/cli/cli_utils.py` & `codecarbon-2.4.0rc0/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/cli/main.py` & `codecarbon-2.4.0rc0/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/api_client.py` & `codecarbon-2.4.0rc0/codecarbon/core/api_client.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/cloud.py` & `codecarbon-2.4.0rc0/codecarbon/core/cloud.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import requests
 
 from codecarbon.external.logger import logger
 
 
 def postprocess_gcp_cloud_metadata(cloud_metadata: Dict[str, Any]) -> Dict[str, Any]:
-    # type: (Dict[str, Any]) -> Dict[str, Any]
-
     # Attributes contains custom metadata and also contains Kubernetes config,
     # startup script and secrets, filter it out
     if "attributes" in cloud_metadata:
         del cloud_metadata["attributes"]
 
     return cloud_metadata
```

### Comparing `codecarbon-2.3.5/codecarbon/core/co2_signal.py` & `codecarbon-2.4.0rc0/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/config.py` & `codecarbon-2.4.0rc0/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/cpu.py` & `codecarbon-2.4.0rc0/codecarbon/core/cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/emissions.py` & `codecarbon-2.4.0rc0/codecarbon/core/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/gpu.py` & `codecarbon-2.4.0rc0/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/measure.py` & `codecarbon-2.4.0rc0/codecarbon/core/measure.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/powermetrics.py` & `codecarbon-2.4.0rc0/codecarbon/core/powermetrics.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/rapl.py` & `codecarbon-2.4.0rc0/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/schemas.py` & `codecarbon-2.4.0rc0/codecarbon/core/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/units.py` & `codecarbon-2.4.0rc0/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/core/util.py` & `codecarbon-2.4.0rc0/codecarbon/core/util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/data/cloud/impact.csv` & `codecarbon-2.4.0rc0/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.4.0rc0/codecarbon/data/hardware/cpu_power.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1365,14 +1365,15 @@
 Intel Core i5-11600,65
 Intel Core i5-11600K,125
 Intel Core i5-11600KF,125
 Intel Core i5-11600T,35
 Intel Core i5-2310,95
 Intel Core i5-2320,95
 Intel Core i5-2390T,35
+Intel Core i5-2400,95
 Intel Core i5-2405S,65
 Intel Core i5-2415M,35
 Intel Core i5-2430M,35
 Intel Core i5-2430M,35
 Intel Core i5-2435M,35
 Intel Core i5-2435M,35
 Intel Core i5-2467M,17
@@ -2158,7 +2159,8 @@
 Intel Xeon X5660,95
 Intel Xeon X5667,95
 Intel Xeon X5670,95
 Intel Xeon X5672,95
 Intel Xeon X5677,130
 Intel Xeon X5680,130
 Intel Xeon X5687,130
+Intel Xeon Silver 4208, 85
```

### Comparing `codecarbon-2.3.5/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.4.0rc0/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.4.0rc0/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/data/private_infra/global_energy_mix.json` & `codecarbon-2.4.0rc0/codecarbon/data/private_infra/global_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/emissions_tracker.py` & `codecarbon-2.4.0rc0/codecarbon/emissions_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,18 @@
         :param save_to_logger: Indicates if the emission artifacts should be written
                             to a dedicated logger, defaults to False.
         :param logging_logger: LoggerOutput object encapsulating a logging.logger
                             or a Google Cloud logger.
         :param save_to_prometheus: Indicates if the emission artifacts should be
                             pushed to prometheus, defaults to False.
         :param prometheus_url: url of the prometheus server, defaults to `localhost:9091`.
-        :param gpu_ids: User-specified known gpu ids to track, defaults to None.
+        :param gpu_ids: User-specified known gpu ids to track.
+                            Defaults to None, which means that all available gpus will be tracked.
+                            It needs to be a list of integers or a comma-separated string.
+                            Valid examples: [1, 3, 4] or "1,2".
         :param emissions_endpoint: Optional URL of http endpoint for sending emissions
                                    data.
         :param experiment_id: Id of the experiment.
         :param experiment_name: Label of the experiment
         :param co2_signal_api_token: API token for co2signal.com (requires sign-up for
                                      free beta)
         :param tracking_mode: One of "process" or "machine" in order to measure the
@@ -264,18 +267,24 @@
         self._conf["cpu_count"] = count_cpus()
         self._geo = None
         self._task_start_measurement_values = {}
         self._task_stop_measurement_values = {}
         self._tasks: Dict[str, Task] = {}
         self._active_task: Optional[str] = None
 
-        if isinstance(self._gpu_ids, str):
+        # If _gpu_ids is a string or a list of int, parse it to a list of ints
+        if isinstance(self._gpu_ids, str) or (
+            isinstance(self._gpu_ids, list)
+            and all(isinstance(gpu_id, int) for gpu_id in self._gpu_ids)
+        ):
             self._gpu_ids: List[int] = parse_gpu_ids(self._gpu_ids)
             self._conf["gpu_ids"] = self._gpu_ids
             self._conf["gpu_count"] = len(self._gpu_ids)
+        else:
+            logger.warn("Invalid gpu_ids format. Expected a string or a list of ints.")
 
         logger.info("[setup] RAM Tracking...")
         ram = RAM(tracking_mode=self._tracking_mode)
         self._conf["ram_total_size"] = ram.machine_memory_GB
         self._hardware: List[Union[RAM, CPU, GPU, AppleSiliconChip]] = [ram]
 
         # Hardware detection
```

### Comparing `codecarbon-2.3.5/codecarbon/external/geography.py` & `codecarbon-2.4.0rc0/codecarbon/external/geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/external/hardware.py` & `codecarbon-2.4.0rc0/codecarbon/external/hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/external/logger.py` & `codecarbon-2.4.0rc0/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/external/scheduler.py` & `codecarbon-2.4.0rc0/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/external/task.py` & `codecarbon-2.4.0rc0/codecarbon/external/task.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/input.py` & `codecarbon-2.4.0rc0/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/output.py` & `codecarbon-2.4.0rc0/codecarbon/output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/prometheus/metric_definitions.py` & `codecarbon-2.4.0rc0/codecarbon/prometheus/metric_definitions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/prometheus/prometheus.py` & `codecarbon-2.4.0rc0/codecarbon/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.4.0rc0/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.4.0rc0/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.4.0rc0/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/viz/carbonboard.py` & `codecarbon-2.4.0rc0/codecarbon/viz/carbonboard.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.4.0rc0/codecarbon/viz/carbonboard_on_api.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/viz/components.py` & `codecarbon-2.4.0rc0/codecarbon/viz/components.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.3.5/codecarbon/viz/data.py` & `codecarbon-2.4.0rc0/codecarbon/viz/data.py`

 * *Files identical despite different names*


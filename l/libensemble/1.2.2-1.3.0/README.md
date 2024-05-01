# Comparing `tmp/libensemble-1.2.2.tar.gz` & `tmp/libensemble-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libensemble-1.2.2.tar", last modified: Thu Mar 21 19:00:23 2024, max compression
+gzip compressed data, was "libensemble-1.3.0.tar", last modified: Wed May  1 20:34:28 2024, max compression
```

## Comparing `libensemble-1.2.2.tar` & `libensemble-1.3.0.tar`

### file list

```diff
@@ -1,675 +1,679 @@
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.256599 libensemble-1.2.2/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2093 2024-03-21 18:57:12.000000 libensemble-1.2.2/.flake8
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    34306 2024-03-21 18:57:12.000000 libensemble-1.2.2/CHANGELOG.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3115 2024-03-21 18:57:12.000000 libensemble-1.2.2/CONTRIBUTING.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1746 2024-03-21 18:57:12.000000 libensemble-1.2.2/LICENSE
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      401 2024-03-21 18:57:12.000000 libensemble-1.2.2/MANIFEST.in
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6704 2024-03-21 19:00:23.256599 libensemble-1.2.2/PKG-INFO
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5497 2024-03-21 18:57:12.000000 libensemble-1.2.2/README.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      269 2024-03-21 18:57:12.000000 libensemble-1.2.2/SUPPORT.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.172598 libensemble-1.2.2/docs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14887 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/FAQ.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      613 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/Makefile
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.172598 libensemble-1.2.2/docs/_static/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       53 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/_static/my_theme.css
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7847 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/advanced_installation.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      159 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/bibliography.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9787 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/conf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       33 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/contributing.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.172598 libensemble-1.2.2/docs/data_structures/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1711 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/data_structures/alloc_specs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      380 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/data_structures/data_structures.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      891 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/data_structures/exit_criteria.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3534 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/data_structures/gen_specs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    15530 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/data_structures/libE_specs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3126 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/data_structures/persis_info.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2959 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/data_structures/platform_specs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2575 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/data_structures/sim_specs.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.164598 libensemble-1.2.2/docs/dev_guide/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.172598 libensemble-1.2.2/docs/dev_guide/dev_API/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      366 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/developer_API.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      211 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/env_resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      326 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/history_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      187 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/manager_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       85 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/mpi_resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       87 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/node_resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      285 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      171 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/rset_resources_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      167 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/scheduler_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      164 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/worker_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      354 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/dev_API/worker_resources_module.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.172598 libensemble-1.2.2/docs/dev_guide/release_management/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      245 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/release_management/release_index.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.172598 libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      194 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1817 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/rel_conda.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      918 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/rel_github.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1162 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/rel_pypi.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4294 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/rel_spack.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3054 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/dev_guide/release_management/release_process.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.176598 libensemble-1.2.2/docs/examples/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1335 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/alloc_funcs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2076 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/aposmm.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2765 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/calling_scripts.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      626 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/examples_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      130 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/fd_param_finder.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      454 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/gen_funcs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      691 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/sampling.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1468 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/sim_funcs.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      534 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/surmise.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      709 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/tasmanian.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      177 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/examples/uniform_or_localopt.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.176598 libensemble-1.2.2/docs/executor/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      467 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/executor/balsam_2_executor.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      328 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/executor/ex_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2931 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/executor/executor.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1484 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/executor/mpi_executor.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7439 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/executor/overview.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.176598 libensemble-1.2.2/docs/function_guides/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5781 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/allocator.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4042 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/calc_status.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      668 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/function_guide_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8963 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/generator.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6232 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/history_array.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4076 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/sim_gen_alloc_api.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4230 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/simulator.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2151 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/work_dict.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2021 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/function_guides/worker_array.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2483 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/history_output_logging.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.184598 libensemble-1.2.2/docs/images/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    29290 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/adaptiveloop.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)  1001535 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/balsam2.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   295622 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/basic_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   189953 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/centralized_new_detailed.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   139065 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/diagram_with_persis.png
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.184598 libensemble-1.2.2/docs/images/diagram_xml/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5561 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/diagram_xml/adaptiveloop.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   707087 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/diagram_xml/balsam2.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    74050 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/diagram_xml/persis_add_worker.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    73798 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/diagram_xml/persis_wasted_node.xml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   171140 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/distributed_new_detailed.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   367100 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/funcxmodel.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   337602 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/gen_v_fail_or_cancel.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   244843 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/history_gen1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   244574 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/history_gen2.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    26836 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/history_init.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   205538 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/history_sim1.png
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    54153 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/libE_logo.png
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    66602 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/libE_logo_circle.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    32035 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/libE_logo_white.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6292 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/libEnsemble_Logo.svg
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    26268 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    31284 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   372562 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/localopt_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   250428 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/persis_add_worker.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   233756 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/persis_wasted_node.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   373798 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/sampling_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    34960 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/sinex.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    45757 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/variable_resources1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    48241 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/variable_resources2.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    41003 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/variable_resources3.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    43963 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/variable_resources_larger_rsets1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    46233 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/variable_resources_more_rsets1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    52608 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/variable_resources_persis_gen1.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    37856 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/images/variable_resources_sched_opts.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1091 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3022 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/introduction.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3502 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/introduction_latex.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1906 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/known_issues.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      794 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/latex_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      486 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/libe_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1810 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/nitpicky
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7330 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/overview_usecases.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.188598 libensemble-1.2.2/docs/platforms/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3598 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/aurora.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4787 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/bebop.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1958 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/example_scripts.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2167 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/frontier.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1951 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/improv.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6923 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/perlmutter.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9719 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/platforms_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3513 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/polaris.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2238 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/spock_crusher.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4724 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/srun.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7359 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/platforms/summit.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      679 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/posters.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      573 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/programming_libE.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      435 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/references.bib
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       30 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/release_notes.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      104 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/requirements.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.188598 libensemble-1.2.2/docs/resource_manager/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11481 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/resource_manager/overview.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1758 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/resource_manager/resource_detection.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      735 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/resource_manager/resources_index.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      783 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/resource_manager/scheduler_module.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      430 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/resource_manager/worker_resources.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3580 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/resource_manager/zero_resource_workers.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1788 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/rst_formatting_guidelines
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12567 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/running_libE.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.188598 libensemble-1.2.2/docs/tutorials/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12273 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/tutorials/aposmm_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11964 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/tutorials/calib_cancel_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    16420 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/tutorials/executor_forces_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11793 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/tutorials/forces_gpu_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12766 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/tutorials/local_sine_tutorial.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      153 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/tutorials/tutorials.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      904 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/utilities.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1723 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/welcome.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10302 2024-03-21 18:57:12.000000 libensemble-1.2.2/docs/xSDK_policy_compatibility.md
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.188598 libensemble-1.2.2/examples/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      856 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/README.rst
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.188598 libensemble-1.2.2/examples/alloc_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2318 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/alloc_funcs/fast_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3615 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/alloc_funcs/give_sim_work_first.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6374 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/alloc_funcs/start_only_persistent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4882 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/alloc_funcs/start_persistent_local_opt_gens.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.188598 libensemble-1.2.2/examples/calling_scripts/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.196598 libensemble-1.2.2/examples/calling_scripts/regression_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2379 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/common.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6038 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/optimizer.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.196598 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2496 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      694 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      500 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.196598 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      110 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/cleanup.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      918 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/exe.pl
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      474 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/findMin.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      692 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.pl
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2991 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      753 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/processexe.pl
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1696 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/runs.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       70 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/speed3d.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3666 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1762 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_1d_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4136 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_GPU_variable_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4145 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_GPU_variable_resources_multi_task.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3197 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_ensemble_platform_workdir.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1900 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2124 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3041 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_gpCAM.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2176 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_heffte.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2773 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_inverse_bayes_example.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4767 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3118 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4182 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4630 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_ibcdfo_pounders.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3309 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3604 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4040 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_pounders.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4711 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3446 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_blmvm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3051 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_nm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2990 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4996 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2771 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5473 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_gp.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4033 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4610 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5664 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5920 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_tasmanian.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3923 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3180 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_with_app_persistent_aposmm_tao_nm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5603 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/regression_tests/test_ytopt_heffte.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3974 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/run_libe_forces.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      977 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/run_libe_forces_from_yaml.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7559 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/calling_scripts/run_libensemble_on_warpx.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.196598 libensemble-1.2.2/examples/gen_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10615 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/gen_funcs/persistent_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6771 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/gen_funcs/sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4820 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/gen_funcs/uniform_or_localopt.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.200598 libensemble-1.2.2/examples/libE_submission_scripts/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      833 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/bebop_submit_slurm_central.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2803 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/bebop_submit_slurm_distrib.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      705 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/bridges_submit_slurm_central.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1541 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/cobalt_submit_mproc.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      939 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/edtb_submit_pbspro_central.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      307 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/submit_pbs_aurora.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      249 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/submit_pbs_polaris.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      258 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/submit_pbs_simple.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      367 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/submit_slurm_simple.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1279 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/libE_submission_scripts/summit_submit_mproc.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.200598 libensemble-1.2.2/examples/sim_funcs/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.200598 libensemble-1.2.2/examples/sim_funcs/branin/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/sim_funcs/branin/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      598 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/sim_funcs/branin/branin.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1124 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/sim_funcs/branin/branin_obj.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       71 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/sim_funcs/branin/known_minima_and_func_values
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11430 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/sim_funcs/chwirut1.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5320 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/sim_funcs/executor_hworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4108 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/sim_funcs/six_hump_camel.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.164598 libensemble-1.2.2/examples/tutorials/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.200598 libensemble-1.2.2/examples/tutorials/aposmm/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13701 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/aposmm/aposmm_tutorial_notebook.ipynb
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1814 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/aposmm/tutorial_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      632 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/aposmm/tutorial_six_hump_camel.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.200598 libensemble-1.2.2/examples/tutorials/forces_with_executor/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1787 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/forces_with_executor/build_forces.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13704 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/forces_with_executor/forces.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1276 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/forces_with_executor/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    22332 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/forces_with_executor/forces_tutorial_notebook.ipynb
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2436 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/forces_with_executor/run_libe_forces.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.200598 libensemble-1.2.2/examples/tutorials/images/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   295622 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/images/basic_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   372562 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/images/localopt_6hc.png
--rw-rw-r--   0 shudson   (1000) shudson   (1000)   373798 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/images/sampling_6hc.png
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.204598 libensemble-1.2.2/examples/tutorials/simple_sine/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      756 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/simple_sine/sine_gen.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      320 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/simple_sine/sine_sim.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11677 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2049 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/simple_sine/test_local_sine_tutorial.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1160 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/simple_sine/test_local_sine_tutorial_2.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2126 2024-03-21 18:57:12.000000 libensemble-1.2.2/examples/tutorials/simple_sine/test_local_sine_tutorial_3.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.204598 libensemble-1.2.2/install/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       93 2024-03-21 18:57:12.000000 libensemble-1.2.2/install/environment.yml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      731 2024-03-21 18:57:12.000000 libensemble-1.2.2/install/find_mpi.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      181 2024-03-21 18:57:12.000000 libensemble-1.2.2/install/gen_deps_environment.yml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       27 2024-03-21 18:57:12.000000 libensemble-1.2.2/install/misc_feature_requirements.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      156 2024-03-21 18:57:12.000000 libensemble-1.2.2/install/testing_requirements.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.204598 libensemble-1.2.2/libensemble/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      349 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/__init__.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.208598 libensemble-1.2.2/libensemble/alloc_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2318 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/fast_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6925 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/fast_alloc_and_pausing.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1439 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/give_pregenerated_work.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3615 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/give_sim_work_first.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3121 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/inverse_bayes_allocf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1783 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/only_one_gen_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3702 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/persistent_aposmm_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3195 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/start_fd_persistent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6374 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/start_only_persistent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4882 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/alloc_funcs/start_persistent_local_opt_gens.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.208598 libensemble-1.2.2/libensemble/comms/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/comms/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8664 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/comms/comms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7013 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/comms/logs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3766 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/comms/mpi.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3506 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/comms/tcp_mgr.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    18851 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/ensemble.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.208598 libensemble-1.2.2/libensemble/executors/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      444 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/executors/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    19970 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/executors/balsam_executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    26451 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/executors/executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14875 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/executors/mpi_executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    21782 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/executors/mpi_runner.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.212598 libensemble-1.2.2/libensemble/gen_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1335 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    24504 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/aposmm_localopt_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    33692 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10159 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_ax_multitask.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4945 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_fd_param_finder.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9388 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_gp.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9689 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_gpCAM.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1486 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_inverse_bayes.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10615 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9521 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_sampling_var_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8525 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_surmise_calib.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14491 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/persistent_tasmanian.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6771 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2242 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/surmise_calib_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4820 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/uniform_or_localopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2611 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/gen_funcs/ytopt_asktell.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10614 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/history.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    22223 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/libE.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1613 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/logger.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    25882 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/manager.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2314 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/message_numbers.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.212598 libensemble-1.2.2/libensemble/resources/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9334 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/env_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2380 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/gpu_detect.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9226 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/mpi_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6430 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/node_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10707 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/platforms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14275 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7728 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/rset_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    17877 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/scheduler.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14637 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/resources/worker_resources.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.216598 libensemble-1.2.2/libensemble/sim_funcs/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2552 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/borehole.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2052 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/borehole_kills.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.216598 libensemble-1.2.2/libensemble/sim_funcs/branin/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/branin/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      598 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/branin/branin.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1124 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/branin/branin_obj.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       71 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/branin/known_minima_and_func_values
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11430 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/chwirut1.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      353 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/comms_testing.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5320 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/executor_hworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      722 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/heffte.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      324 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/helloworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      422 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/inverse_bayes.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      673 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/mock_sim.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1337 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/noisy_vector_mapping.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      623 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/one_d_func.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      486 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/periodic_func.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2446 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/rosenbrock.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4185 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/run_line_check.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4108 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/six_hump_camel.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2767 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/surmise_test_function.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    11311 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/var_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1351 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/sim_funcs/ytopt_obj.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    19600 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/specs.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.216598 libensemble-1.2.2/libensemble/tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      643 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/__init__.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.228598 libensemble-1.2.2/libensemble/tests/functionality_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      457 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      538 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/1d_sampling.json
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      457 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/1d_sampling.toml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      445 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/1d_sampling.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2206 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/check_libE_stats.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       61 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/env_script_in.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1276 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      756 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/sine_gen.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      320 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/sine_sim.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1336 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_sampling_from_files.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2182 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_sampling_with_profile.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2201 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_splitcomm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2273 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_subcomm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2085 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_super_simple.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2710 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4861 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_GPU_gen_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2763 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1782 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_calc_exception.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2527 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_cancel_in_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2396 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_comms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2135 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_elapsed_time_abort.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2305 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_forces_tutorial.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2384 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_forces_tutorial_2.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3807 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3822 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_hworld_timeout.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2658 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_simple.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3025 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_fast_alloc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2049 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_local_sine_tutorial.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1160 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_local_sine_tutorial_2.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2126 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_local_sine_tutorial_3.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3164 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_comms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10236 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_gpu_settings.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3675 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_gpu_settings_env.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5288 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_gpu_settings_mock_nodes_multi_task.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13107 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4275 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_subnode.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5068 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4633 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6272 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5016 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1772 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_new_field.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3372 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_sampling_CUDA_variable_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2924 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_sim_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3590 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_gen_decides_stop.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3396 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2754 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_async.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2575 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_cancel.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2429 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_nonblocking.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3123 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_running_mean.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3338 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3516 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3736 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3267 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3490 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2167 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4043 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2404 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_input_dir_option.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4282 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_stats_output.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3186 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5461 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling_cancel.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4121 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling_one_residual_at_a_time.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3028 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling_then_persistent_localopt_runs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4164 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1973 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_worker_exceptions.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3163 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_workflow_dir.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4374 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_zero_resource_workers.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4653 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.232598 libensemble-1.2.2/libensemble/tests/regression_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2379 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/common.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6038 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/optimizer.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.232598 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2496 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      694 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      500 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.232598 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      110 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/cleanup.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      918 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/exe.pl
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      474 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/findMin.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      692 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.pl
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2991 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      753 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/processexe.pl
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1696 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/runs.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       70 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/speed3d.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3666 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1762 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_1d_sampling.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4136 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_GPU_variable_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4145 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_GPU_variable_resources_multi_task.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3197 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_ensemble_platform_workdir.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1900 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_evaluate_existing_sample.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2124 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_evaluate_mixed_sample.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3041 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_gpCAM.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2176 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_heffte.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2773 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_inverse_bayes_example.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4767 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3118 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_exception.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4182 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4630 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_ibcdfo_pounders.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3309 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3604 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4040 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_pounders.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4711 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3446 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_tao_blmvm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3051 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_tao_nm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2990 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4996 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2771 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_fd_param_finder.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5473 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_gp.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4033 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4610 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_surmise_calib.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5664 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_surmise_killsims.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5920 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_tasmanian.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3923 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_tasmanian_async.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3180 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_with_app_persistent_aposmm_tao_nm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5603 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/regression_tests/test_ytopt_heffte.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    27069 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/run-tests.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.232598 libensemble-1.2.2/libensemble/tests/scaling_tests/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.168598 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.236599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       60 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2056 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/define_apps.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1990 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7702 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2514 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/run_libe_forces_balsam.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2367 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/submit_libe_forces_remotely.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.236599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      290 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/clone.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      885 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/forces.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4822 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2554 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2482 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3974 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      977 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.236599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1787 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13704 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/forces.c
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.236599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      885 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5148 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4845 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      916 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/readme.md
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.236599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1697 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1934 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3435 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      224 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/submit_perlmutter.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.236599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1579 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      815 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3825 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/run_libe_forces.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.240599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_multi_app/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_multi_app/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1753 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_multi_app/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4632 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_multi_app/run_libe_forces.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      224 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_multi_app/submit_perlmutter.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.240599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_simple/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_simple/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1276 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1569 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_simple/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2436 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_simple/run_libe_forces.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.240599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       54 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/cleanup.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4700 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/forces_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      964 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/globus_compute_forces.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1293 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/readme.md
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      481 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/run_libe_forces_globus_compute.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.240599 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/submission_scripts/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      460 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/submission_scripts/submit_pbs_aurora.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      245 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/submission_scripts/submit_pbs_polaris.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      245 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/submission_scripts/submit_pbs_simple.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      363 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/submission_scripts/submit_slurm_simple.sh
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1370 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/forces/submission_scripts/summit_submit_mproc.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      148 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/note_moved_examples.md
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.240599 libensemble-1.2.2/libensemble/tests/scaling_tests/persistent_gp/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2947 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/persistent_gp/run_example.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.240599 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      853 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/all_machine_specs.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     4471 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/plot_results.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2503 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/read_sim_output.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1925 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/readme.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       44 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/requirements.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7559 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.240599 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/sim/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8355 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/sim/inputs
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1413 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/summit_submit_mproc.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3994 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/warpx_simf.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3284 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/write_sim_input.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.168598 libensemble-1.2.2/libensemble/tests/standalone_tests/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.240599 libensemble-1.2.2/libensemble/tests/standalone_tests/comms_test/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1823 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/comms_test/commtest.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      973 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/comms_test/readme.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.244598 libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)       84 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/build.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      663 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/burn_time.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4715 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/killtest.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2579 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/log.autotest.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2411 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/log.burn_time_test_with_top.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1814 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/readme.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1011 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/sleep_and_print.c
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.244598 libensemble-1.2.2/libensemble/tests/standalone_tests/mpi_launch_test/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      664 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/mpi_launch_test/create_mpi_jobs.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      311 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/mpi_launch_test/helloworld.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      747 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/mpi_launch_test/readme.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.244598 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.168598 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/outputs/
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.244598 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/outputs/frontier_2023.08.09-20.13.02/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      102 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/outputs/frontier_2023.08.09-20.13.02/time.out
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.244598 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/outputs/perlmutter_2023.08.09-17.14.02/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      106 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/outputs/perlmutter_2023.08.09-17.14.02/time.out
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1137 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/readme.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.244598 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/run/
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13705 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/run/forces.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      469 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/run/run_batches.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      930 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/run/run_timing_study.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      256 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/run/submit_frontier.sh
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      255 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/run/submit_perlmutter.sh
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.248599 libensemble-1.2.2/libensemble/tests/unit_tests/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      378 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      779 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/conftest.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      446 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/launch_busy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3129 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/setup.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.248599 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1359 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/borehole.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      210 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/c_startup.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      806 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/my_serialtask.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1166 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/my_simtask.c
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1247 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/my_simtask.f90
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       32 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/py_startup.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      723 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example.json
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      651 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example.toml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      551 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      551 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      535 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    20263 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_allocation_funcs_and_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3700 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_comms.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6740 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_ensemble.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    12526 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_env_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    32583 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_executor.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9719 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_executor_balsam.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    13363 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_executor_gpus.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    18078 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_history.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2238 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_launcher.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4066 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_loc_stack.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1733 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_manager_main.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4843 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_models.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5655 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_node_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6263 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_persistent_aposmm.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3452 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_platform.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    27445 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_resource_scheduler.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    39022 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_resources.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1499 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_scipy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8005 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_sim_dir_properties.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4335 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_task_funcs.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1534 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_timer.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4294 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests/test_ufunc_runners.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.252599 libensemble-1.2.2/libensemble/tests/unit_tests_logger/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests_logger/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3883 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests_logger/test_logger.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.252599 libensemble-1.2.2/libensemble/tests/unit_tests_mpi_import/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      779 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests_mpi_import/conftest.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7821 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests_mpi_import/test_libE_main.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.252599 libensemble-1.2.2/libensemble/tests/unit_tests_nompi/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests_nompi/.coveragerc
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      712 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests_nompi/conftest.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3022 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tests/unit_tests_nompi/test_aaa_comms.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.252599 libensemble-1.2.2/libensemble/tools/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      267 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tools/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    18581 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tools/alloc_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1717 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tools/fields_keys.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1368 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tools/forkable_pdb.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8949 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tools/parse_args.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4829 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tools/persistent_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     8633 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tools/test_support.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5769 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/tools/tools.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.252599 libensemble-1.2.2/libensemble/utils/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      102 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/__init__.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3254 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/launcher.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4964 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/loc_stack.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1558 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/misc.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     9741 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/output_directory.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4933 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/pydantic_bindings.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4937 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/runners.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     5012 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/specs_checkers.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2678 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/timer.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    10307 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/utils/validators.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       22 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/version.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    14504 2024-03-21 18:57:12.000000 libensemble-1.2.2/libensemble/worker.py
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.204598 libensemble-1.2.2/libensemble.egg-info/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     6704 2024-03-21 19:00:23.000000 libensemble-1.2.2/libensemble.egg-info/PKG-INFO
--rw-rw-r--   0 shudson   (1000) shudson   (1000)    30481 2024-03-21 19:00:23.000000 libensemble-1.2.2/libensemble.egg-info/SOURCES.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        1 2024-03-21 19:00:23.000000 libensemble-1.2.2/libensemble.egg-info/dependency_links.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)      170 2024-03-21 19:00:23.000000 libensemble-1.2.2/libensemble.egg-info/requires.txt
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       12 2024-03-21 19:00:23.000000 libensemble-1.2.2/libensemble.egg-info/top_level.txt
-drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-03-21 19:00:23.256599 libensemble-1.2.2/scripts/
--rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/__init__.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     2467 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/compare_npy.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     4549 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/liberegister
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     7194 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/libesubmit
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1632 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/plot_contours_and_history_points.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     3131 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/plot_libe_calcs_util_v_time.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     4169 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/plot_libe_histogram.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3709 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/plot_libe_tasks_util_v_time.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     2625 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/plot_pareto_3d.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1570 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/print_fields.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      839 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/print_npy.py
--rwxrwxr-x   0 shudson   (1000) shudson   (1000)      496 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/print_pickle.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     1745 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/process_history_to_make_chart.py
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     2224 2024-03-21 18:57:12.000000 libensemble-1.2.2/scripts/readme.rst
--rw-rw-r--   0 shudson   (1000) shudson   (1000)       38 2024-03-21 19:00:23.256599 libensemble-1.2.2/setup.cfg
--rw-rw-r--   0 shudson   (1000) shudson   (1000)     3713 2024-03-21 18:57:12.000000 libensemble-1.2.2/setup.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.414890 libensemble-1.3.0/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2093 2024-05-01 20:33:58.000000 libensemble-1.3.0/.flake8
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    35150 2024-05-01 20:33:58.000000 libensemble-1.3.0/CHANGELOG.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3115 2024-05-01 20:33:58.000000 libensemble-1.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1746 2024-05-01 20:33:58.000000 libensemble-1.3.0/LICENSE
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      401 2024-05-01 20:33:58.000000 libensemble-1.3.0/MANIFEST.in
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6842 2024-05-01 20:34:28.414890 libensemble-1.3.0/PKG-INFO
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5635 2024-05-01 20:33:58.000000 libensemble-1.3.0/README.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      269 2024-05-01 20:33:58.000000 libensemble-1.3.0/SUPPORT.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.342890 libensemble-1.3.0/docs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14887 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/FAQ.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      642 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/Makefile
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.342890 libensemble-1.3.0/docs/_static/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       53 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/_static/my_theme.css
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7847 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/advanced_installation.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      159 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/bibliography.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10028 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/conf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       33 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/contributing.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.342890 libensemble-1.3.0/docs/data_structures/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1711 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/data_structures/alloc_specs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      380 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/data_structures/data_structures.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      891 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/data_structures/exit_criteria.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3534 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/data_structures/gen_specs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    16102 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/data_structures/libE_specs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3161 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/data_structures/persis_info.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2959 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/data_structures/platform_specs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2575 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/data_structures/sim_specs.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.330890 libensemble-1.3.0/docs/dev_guide/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.342890 libensemble-1.3.0/docs/dev_guide/dev_API/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      366 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/developer_API.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      211 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/env_resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      326 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/history_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      187 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/manager_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       85 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/mpi_resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       87 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/node_resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      285 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      171 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/rset_resources_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      167 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/scheduler_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      164 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/worker_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      354 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/dev_API/worker_resources_module.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.342890 libensemble-1.3.0/docs/dev_guide/release_management/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      245 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/release_management/release_index.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.346890 libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      194 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1817 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/rel_conda.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      918 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/rel_github.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1162 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/rel_pypi.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4294 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/rel_spack.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3203 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/dev_guide/release_management/release_process.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.346890 libensemble-1.3.0/docs/examples/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1311 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/alloc_funcs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2076 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/aposmm.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2765 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/calling_scripts.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      626 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/examples_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      130 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/fd_param_finder.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      454 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/gen_funcs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      691 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/sampling.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1468 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/sim_funcs.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      534 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/surmise.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      709 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/tasmanian.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      177 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/examples/uniform_or_localopt.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.346890 libensemble-1.3.0/docs/executor/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      467 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/executor/balsam_2_executor.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      328 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/executor/ex_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2931 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/executor/executor.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1484 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/executor/mpi_executor.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7437 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/executor/overview.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.346890 libensemble-1.3.0/docs/function_guides/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5781 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/allocator.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4042 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/calc_status.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      668 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/function_guide_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8963 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/generator.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6232 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/history_array.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4076 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/sim_gen_alloc_api.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4230 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/simulator.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2151 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/work_dict.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2021 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/function_guides/worker_array.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2483 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/history_output_logging.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.354890 libensemble-1.3.0/docs/images/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    29290 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/adaptiveloop.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)  1001535 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/balsam2.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   295622 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/basic_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   189953 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/centralized_new_detailed.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   139065 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/diagram_with_persis.png
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.358890 libensemble-1.3.0/docs/images/diagram_xml/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5561 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/diagram_xml/adaptiveloop.xml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   707087 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/diagram_xml/balsam2.xml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    74050 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/diagram_xml/persis_add_worker.xml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    73798 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/diagram_xml/persis_wasted_node.xml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   171140 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/distributed_new_detailed.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   367100 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/funcxmodel.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   337602 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/gen_v_fail_or_cancel.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   244843 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/history_gen1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   244574 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/history_gen2.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    26836 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/history_init.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   205538 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/history_sim1.png
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    54153 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/libE_logo.png
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    66602 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/libE_logo_circle.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    32035 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/libE_logo_white.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6292 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/libEnsemble_Logo.svg
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    26268 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    31284 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   372562 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/localopt_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   250428 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/persis_add_worker.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   233756 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/persis_wasted_node.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   373798 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/sampling_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    34960 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/sinex.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    45757 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/variable_resources1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    48241 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/variable_resources2.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    41003 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/variable_resources3.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    43963 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/variable_resources_larger_rsets1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    46233 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/variable_resources_more_rsets1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    52608 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/variable_resources_persis_gen1.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    37856 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/images/variable_resources_sched_opts.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1091 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2885 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/introduction.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3404 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/introduction_latex.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1906 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/known_issues.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      794 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/latex_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      486 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/libe_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1810 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/nitpicky
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7328 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/overview_usecases.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.358890 libensemble-1.3.0/docs/platforms/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3598 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/aurora.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4787 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/bebop.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1958 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/example_scripts.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2167 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/frontier.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1951 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/improv.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6923 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/perlmutter.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9717 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/platforms_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3509 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/polaris.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2238 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/spock_crusher.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4724 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/srun.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7360 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/platforms/summit.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      679 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/posters.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      573 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/programming_libE.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      435 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/references.bib
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       30 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/release_notes.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      127 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/requirements.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.358890 libensemble-1.3.0/docs/resource_manager/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11481 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/resource_manager/overview.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1758 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/resource_manager/resource_detection.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      735 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/resource_manager/resources_index.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      783 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/resource_manager/scheduler_module.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      430 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/resource_manager/worker_resources.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3580 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/resource_manager/zero_resource_workers.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1788 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/rst_formatting_guidelines
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14073 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/running_libE.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1455 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/spelling_wordlist.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.358890 libensemble-1.3.0/docs/tutorials/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12273 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/tutorials/aposmm_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11964 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/tutorials/calib_cancel_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    17432 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/tutorials/executor_forces_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11793 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/tutorials/forces_gpu_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12766 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/tutorials/local_sine_tutorial.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      153 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/tutorials/tutorials.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      904 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/utilities.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1723 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/welcome.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10302 2024-05-01 20:33:58.000000 libensemble-1.3.0/docs/xSDK_policy_compatibility.md
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.358890 libensemble-1.3.0/examples/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      856 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/README.rst
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.358890 libensemble-1.3.0/examples/alloc_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2493 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/alloc_funcs/fast_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3761 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/alloc_funcs/give_sim_work_first.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6411 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/alloc_funcs/start_only_persistent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5105 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/alloc_funcs/start_persistent_local_opt_gens.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.358890 libensemble-1.3.0/examples/calling_scripts/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.362890 libensemble-1.3.0/examples/calling_scripts/regression_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2379 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/common.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6038 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/optimizer.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.366890 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2496 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      694 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      500 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.366890 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      110 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/cleanup.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      918 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/exe.pl
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      474 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/findMin.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      692 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.pl
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2991 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      753 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/processexe.pl
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1696 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/runs.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       70 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/speed3d.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3666 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1762 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_1d_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4136 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_GPU_variable_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4145 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_GPU_variable_resources_multi_task.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3121 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_ensemble_platform_workdir.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1900 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2170 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3041 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_gpCAM.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2176 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_heffte.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2773 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_inverse_bayes_example.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4767 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3118 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4182 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4630 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_ibcdfo_pounders.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3309 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3604 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4040 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_pounders.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4711 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3446 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_blmvm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3051 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_nm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2990 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4996 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2771 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5473 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_gp.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4033 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4610 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5664 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5920 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_tasmanian.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3923 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3180 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_with_app_persistent_aposmm_tao_nm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5603 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/regression_tests/test_ytopt_heffte.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3974 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/run_libe_forces.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      977 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/run_libe_forces_from_yaml.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7559 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/calling_scripts/run_libensemble_on_warpx.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.366890 libensemble-1.3.0/examples/gen_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10615 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/gen_funcs/persistent_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6769 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/gen_funcs/sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4820 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/gen_funcs/uniform_or_localopt.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.366890 libensemble-1.3.0/examples/libE_submission_scripts/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      833 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/bebop_submit_slurm_central.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2803 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/bebop_submit_slurm_distrib.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      705 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/bridges_submit_slurm_central.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1541 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/cobalt_submit_mproc.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      939 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/edtb_submit_pbspro_central.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      307 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/submit_pbs_aurora.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      249 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/submit_pbs_polaris.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      258 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/submit_pbs_simple.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      367 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/submit_slurm_simple.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1279 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/libE_submission_scripts/summit_submit_mproc.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.366890 libensemble-1.3.0/examples/sim_funcs/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.366890 libensemble-1.3.0/examples/sim_funcs/branin/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/sim_funcs/branin/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      598 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/sim_funcs/branin/branin.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1124 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/sim_funcs/branin/branin_obj.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       71 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/sim_funcs/branin/known_minima_and_func_values
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11430 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/sim_funcs/chwirut1.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5320 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/sim_funcs/executor_hworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4108 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/sim_funcs/six_hump_camel.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.334890 libensemble-1.3.0/examples/tutorials/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.370890 libensemble-1.3.0/examples/tutorials/aposmm/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    13701 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/aposmm/aposmm_tutorial_notebook.ipynb
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1814 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/aposmm/tutorial_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      632 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/aposmm/tutorial_six_hump_camel.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.370890 libensemble-1.3.0/examples/tutorials/forces_with_executor/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1787 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/forces_with_executor/build_forces.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13704 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/forces_with_executor/forces.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1276 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/forces_with_executor/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    22332 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/forces_with_executor/forces_tutorial_notebook.ipynb
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2436 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/forces_with_executor/run_libe_forces.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.370890 libensemble-1.3.0/examples/tutorials/images/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   295622 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/images/basic_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   372562 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/images/localopt_6hc.png
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)   373798 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/images/sampling_6hc.png
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.370890 libensemble-1.3.0/examples/tutorials/simple_sine/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      756 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/simple_sine/sine_gen.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      320 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/simple_sine/sine_sim.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11677 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2049 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/simple_sine/test_local_sine_tutorial.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1160 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/simple_sine/test_local_sine_tutorial_2.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2126 2024-05-01 20:33:58.000000 libensemble-1.3.0/examples/tutorials/simple_sine/test_local_sine_tutorial_3.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.370890 libensemble-1.3.0/install/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      731 2024-05-01 20:33:58.000000 libensemble-1.3.0/install/find_mpi.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      181 2024-05-01 20:33:58.000000 libensemble-1.3.0/install/gen_deps_environment.yml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       27 2024-05-01 20:33:58.000000 libensemble-1.3.0/install/misc_feature_requirements.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      156 2024-05-01 20:33:58.000000 libensemble-1.3.0/install/testing_requirements.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.374890 libensemble-1.3.0/libensemble/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      349 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/__init__.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.374890 libensemble-1.3.0/libensemble/alloc_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2493 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/fast_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7108 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/fast_alloc_and_pausing.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1456 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/give_pregenerated_work.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3761 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/give_sim_work_first.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3090 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/inverse_bayes_allocf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1934 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/only_one_gen_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3890 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/persistent_aposmm_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3175 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/start_fd_persistent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6411 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/start_only_persistent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5105 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/alloc_funcs/start_persistent_local_opt_gens.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.374890 libensemble-1.3.0/libensemble/comms/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/comms/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8656 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/comms/comms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7053 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/comms/logs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3766 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/comms/mpi.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3506 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/comms/tcp_mgr.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    18851 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/ensemble.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.378890 libensemble-1.3.0/libensemble/executors/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      444 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/executors/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    19970 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/executors/balsam_executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    26493 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/executors/executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14840 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/executors/mpi_executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    19209 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/executors/mpi_runner.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.378890 libensemble-1.3.0/libensemble/gen_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1335 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    24504 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/aposmm_localopt_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    33692 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10374 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_ax_multitask.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4945 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_fd_param_finder.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9388 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_gp.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9689 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_gpCAM.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1486 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_inverse_bayes.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10615 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9557 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_sampling_var_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8525 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_surmise_calib.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14490 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/persistent_tasmanian.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6769 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2242 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/surmise_calib_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4820 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/uniform_or_localopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2611 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/gen_funcs/ytopt_asktell.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10614 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/history.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    22556 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/libE.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1613 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/logger.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    27480 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/manager.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2314 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/message_numbers.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.378890 libensemble-1.3.0/libensemble/resources/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9334 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/env_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2380 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/gpu_detect.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9226 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/mpi_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6160 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/node_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10707 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/platforms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14275 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7727 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/rset_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    17901 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/scheduler.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14641 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/resources/worker_resources.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.382890 libensemble-1.3.0/libensemble/sim_funcs/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2552 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/borehole.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2052 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/borehole_kills.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.382890 libensemble-1.3.0/libensemble/sim_funcs/branin/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/branin/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      598 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/branin/branin.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1124 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/branin/branin_obj.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       71 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/branin/known_minima_and_func_values
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11430 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/chwirut1.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      353 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/comms_testing.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5320 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/executor_hworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      722 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/heffte.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      324 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/helloworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      422 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/inverse_bayes.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      673 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/mock_sim.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1337 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/noisy_vector_mapping.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      623 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/one_d_func.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      486 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/periodic_func.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2446 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/rosenbrock.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4231 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/run_line_check.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4108 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/six_hump_camel.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2767 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/surmise_test_function.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11311 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/var_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1351 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/sim_funcs/ytopt_obj.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    20337 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/specs.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.382890 libensemble-1.3.0/libensemble/tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      643 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/__init__.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.390890 libensemble-1.3.0/libensemble/tests/functionality_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      457 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      538 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/1d_sampling.json
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      457 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/1d_sampling.toml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      445 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/1d_sampling.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2272 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/check_libE_stats.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       61 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/env_script_in.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1276 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      756 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/sine_gen.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      320 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/sine_sim.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1336 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_sampling_from_files.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1958 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_sampling_no_comms_given.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2182 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_sampling_with_profile.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2201 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_splitcomm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2273 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_subcomm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2085 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_super_simple.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2710 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5153 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_GPU_gen_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2763 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1782 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_calc_exception.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2527 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_cancel_in_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2396 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_comms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2135 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_elapsed_time_abort.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2583 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_evaluate_existing_plus_gen.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2305 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_forces_tutorial.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2384 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_forces_tutorial_2.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3807 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3822 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_hworld_timeout.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2658 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_simple.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3025 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_fast_alloc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2049 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_local_sine_tutorial.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1160 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_local_sine_tutorial_2.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2126 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_local_sine_tutorial_3.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3164 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_comms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    10259 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_gpu_settings.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3675 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_gpu_settings_env.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5427 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_gpu_settings_mock_nodes_multi_task.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    13810 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4275 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_subnode.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5068 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4633 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6272 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5016 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1772 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_new_field.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3372 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_sampling_CUDA_variable_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2924 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_sim_uniform_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3590 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_gen_decides_stop.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3583 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2754 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_async.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2575 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_cancel.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2429 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_nonblocking.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3123 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_running_mean.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3338 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3516 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3736 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3267 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3490 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2167 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4043 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2404 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_input_dir_option.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4282 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_stats_output.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3186 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5461 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling_cancel.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4121 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling_one_residual_at_a_time.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3028 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling_then_persistent_localopt_runs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4164 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1973 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_worker_exceptions.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3163 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_workflow_dir.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4374 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_zero_resource_workers.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4653 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.394890 libensemble-1.3.0/libensemble/tests/regression_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      456 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2379 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/common.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6038 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/optimizer.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.394890 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2496 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      694 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      500 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/wrapper_obj_fun.m
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.398890 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      110 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/cleanup.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      918 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/exe.pl
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      474 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/findMin.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      692 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.pl
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2991 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      753 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/processexe.pl
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1696 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/runs.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       70 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/speed3d.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3666 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1762 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_1d_sampling.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4136 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_GPU_variable_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4145 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_GPU_variable_resources_multi_task.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3121 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_ensemble_platform_workdir.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1900 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_evaluate_existing_sample.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2170 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_evaluate_mixed_sample.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3041 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_gpCAM.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2176 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_heffte.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2773 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_inverse_bayes_example.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4767 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3118 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_exception.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4182 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4630 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_ibcdfo_pounders.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3309 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3604 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4040 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_pounders.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4711 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3446 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_tao_blmvm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3051 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_tao_nm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2990 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4996 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2771 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_fd_param_finder.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5473 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_gp.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4033 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4610 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_surmise_calib.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5664 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_surmise_killsims.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5920 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_tasmanian.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3923 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_tasmanian_async.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3180 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_with_app_persistent_aposmm_tao_nm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5603 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/regression_tests/test_ytopt_heffte.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    26960 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/run-tests.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.398890 libensemble-1.3.0/libensemble/tests/scaling_tests/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.334890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.398890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       60 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2056 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/define_apps.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1990 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7702 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2514 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/run_libe_forces_balsam.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2367 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/submit_libe_forces_remotely.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.398890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      290 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/clone.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      885 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/forces.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4822 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2554 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2482 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3974 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      977 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.398890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1787 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13704 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/forces.c
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.398890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      885 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5148 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4845 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      916 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/readme.md
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.398890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1697 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1934 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3435 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      224 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/submit_perlmutter.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.398890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1579 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      815 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3825 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/run_libe_forces.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.402890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_multi_app/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_multi_app/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1753 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_multi_app/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4632 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_multi_app/run_libe_forces.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      224 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_multi_app/submit_perlmutter.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.402890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_simple/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       52 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_simple/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1276 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1569 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_simple/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2436 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_simple/run_libe_forces.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.402890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       54 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/cleanup.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4700 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/forces_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      964 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/globus_compute_forces.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1293 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/readme.md
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      481 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/run_libe_forces_globus_compute.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.402890 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/submission_scripts/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      460 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/submission_scripts/submit_pbs_aurora.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      245 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/submission_scripts/submit_pbs_polaris.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      245 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/submission_scripts/submit_pbs_simple.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      363 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/submission_scripts/submit_slurm_simple.sh
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1370 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/forces/submission_scripts/summit_submit_mproc.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      148 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/note_moved_examples.md
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.402890 libensemble-1.3.0/libensemble/tests/scaling_tests/persistent_gp/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2947 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/persistent_gp/run_example.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.402890 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      853 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/all_machine_specs.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     4471 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/plot_results.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2503 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/read_sim_output.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1925 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/readme.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       44 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/requirements.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7559 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.402890 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/sim/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8355 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/sim/inputs
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1413 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/summit_submit_mproc.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3994 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/warpx_simf.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3284 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/write_sim_input.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.334890 libensemble-1.3.0/libensemble/tests/standalone_tests/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.406890 libensemble-1.3.0/libensemble/tests/standalone_tests/comms_test/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1823 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/comms_test/commtest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      973 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/comms_test/readme.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.406890 libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)       84 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/build.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      663 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/burn_time.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4715 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/killtest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2579 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/log.autotest.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2411 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/log.burn_time_test_with_top.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1814 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/readme.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1011 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/sleep_and_print.c
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.406890 libensemble-1.3.0/libensemble/tests/standalone_tests/mpi_launch_test/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      664 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/mpi_launch_test/create_mpi_jobs.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      311 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/mpi_launch_test/helloworld.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      747 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/mpi_launch_test/readme.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.406890 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.338890 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/outputs/
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.406890 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/outputs/frontier_2023.08.09-20.13.02/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      102 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/outputs/frontier_2023.08.09-20.13.02/time.out
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.406890 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/outputs/perlmutter_2023.08.09-17.14.02/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      106 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/outputs/perlmutter_2023.08.09-17.14.02/time.out
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1137 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/readme.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.406890 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/run/
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)    13705 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/run/forces.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      469 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/run/run_batches.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      930 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/run/run_timing_study.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      256 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/run/submit_frontier.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      255 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/run/submit_perlmutter.sh
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.410890 libensemble-1.3.0/libensemble/tests/unit_tests/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      378 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      779 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/conftest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       61 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/env_script_in.sh
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      446 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/launch_busy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3129 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/setup.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.410890 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1359 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/borehole.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      210 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/c_startup.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      806 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/my_serialtask.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1166 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/my_simtask.c
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1247 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/my_simtask.f90
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       32 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/py_startup.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      723 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example.json
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      651 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example.toml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      551 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      551 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      535 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    20315 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_allocation_funcs_and_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3700 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_comms.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6740 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_ensemble.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    12526 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_env_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    36710 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_executor.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9719 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_executor_balsam.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    13363 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_executor_gpus.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    18078 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_history.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2238 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_launcher.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4066 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_loc_stack.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1733 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_manager_main.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4843 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_models.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5664 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_node_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6263 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_persistent_aposmm.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3393 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_platform.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    27530 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_resource_scheduler.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    39022 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_resources.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1499 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_scipy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8005 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_sim_dir_properties.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4335 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_task_funcs.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1534 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_timer.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4246 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests/test_ufunc_runners.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.410890 libensemble-1.3.0/libensemble/tests/unit_tests_logger/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests_logger/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3883 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests_logger/test_logger.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.410890 libensemble-1.3.0/libensemble/tests/unit_tests_mpi_import/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests_mpi_import/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      779 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests_mpi_import/conftest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7821 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests_mpi_import/test_libE_main.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.410890 libensemble-1.3.0/libensemble/tests/unit_tests_nompi/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      404 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests_nompi/.coveragerc
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      712 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests_nompi/conftest.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3022 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tests/unit_tests_nompi/test_aaa_comms.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.414890 libensemble-1.3.0/libensemble/tools/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      267 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tools/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    18772 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tools/alloc_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1717 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tools/fields_keys.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1368 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tools/forkable_pdb.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9261 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tools/parse_args.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4829 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tools/persistent_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     8633 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tools/test_support.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5769 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/tools/tools.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.414890 libensemble-1.3.0/libensemble/utils/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      102 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/__init__.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3254 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/launcher.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4964 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/loc_stack.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2110 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/misc.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     9741 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/output_directory.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5008 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/pydantic_bindings.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3294 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/runners.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     5012 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/specs_checkers.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2678 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/timer.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    11120 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/utils/validators.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       22 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/version.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    14779 2024-05-01 20:33:58.000000 libensemble-1.3.0/libensemble/worker.py
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.374890 libensemble-1.3.0/libensemble.egg-info/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     6842 2024-05-01 20:34:28.000000 libensemble-1.3.0/libensemble.egg-info/PKG-INFO
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)    30728 2024-05-01 20:34:28.000000 libensemble-1.3.0/libensemble.egg-info/SOURCES.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        1 2024-05-01 20:34:28.000000 libensemble-1.3.0/libensemble.egg-info/dependency_links.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)      193 2024-05-01 20:34:28.000000 libensemble-1.3.0/libensemble.egg-info/requires.txt
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       12 2024-05-01 20:34:28.000000 libensemble-1.3.0/libensemble.egg-info/top_level.txt
+drwxrwxr-x   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:34:28.414890 libensemble-1.3.0/scripts/
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)        0 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/__init__.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     2467 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/compare_npy.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     4549 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/liberegister
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     7194 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/libesubmit
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1632 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/plot_contours_and_history_points.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     3131 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/plot_libe_calcs_util_v_time.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     4169 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/plot_libe_histogram.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3709 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/plot_libe_tasks_util_v_time.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     2625 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/plot_pareto_3d.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)     1570 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/print_fields.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      839 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/print_npy.py
+-rwxrwxr-x   0 shudson   (1000) shudson   (1000)      496 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/print_pickle.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     1745 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/process_history_to_make_chart.py
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     2224 2024-05-01 20:33:58.000000 libensemble-1.3.0/scripts/readme.rst
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)       38 2024-05-01 20:34:28.414890 libensemble-1.3.0/setup.cfg
+-rw-rw-r--   0 shudson   (1000) shudson   (1000)     3751 2024-05-01 20:33:58.000000 libensemble-1.3.0/setup.py
```

### Comparing `libensemble-1.2.2/.flake8` & `libensemble-1.3.0/.flake8`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/CHANGELOG.rst` & `libensemble-1.3.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,36 @@
 
 Below are the notes from all libEnsemble releases.
 
 GitHub issues are referenced, and can be viewed with hyperlinks on the `github releases page`_.
 
 .. _`github releases page`: https://github.com/Libensemble/libensemble/releases
 
+Release 1.3.0
+--------------
+
+:Date: May 01, 2024
+
+* Support generator running on the manager (on a thread). #1216/#1290
+  * Set `libE_specs["gen_on_manager"] = True`
+  * Then run with `nworkers` equal to the number of simulation workers.
+* Default to local comms when `nworkers` is supplied and no MPI runner is detected. #1169
+* Parse args defaults to **local** comms when `--nworkers` (or `-n`) is set on the command line. #1169
+
+:Note:
+
+* Tests were run on Linux and MacOS with Python versions 3.9, 3.10, 3.11, 3.12
+* Heterogeneous workflows tested on Frontier (OLCF), Polaris (ALCF), and Perlmutter (NERSC).
+* Note that tests have been recently run on Aurora (ALCF), but the system was unavailable at time of release.
+* Tests were also run on Bebop and Improv LCRC systems.
+
+:Known Issues:
+
+* See known issues section in the documentation.
+
 Release 1.2.2
 --------------
 
 :Date: March 21, 2024
 
 * Bugfix: Some `libE_specs` were not passed through correctly when added after ensemble initialization. #1264
 * `platform_specs` options are now merged with detected platforms, rather than replacing. #1265
@@ -199,15 +221,15 @@
 
 :Date: July 24, 2023
 
 * Fixes issues with workflow directories:
   * Ensure relative paths are interpreted from where libEnsemble is run. #1020
   * Create intermediate directories for workflow paths. #1017
 
-* Fixes issue where libEnsemble pre-initialized a shared multiprocssing queue. #1026
+* Fixes issue where libEnsemble pre-initialized a shared multiprocessing queue. #1026
 
 :Note:
 
 * Tested platforms include Linux, MacOS, Windows and major systems including Frontier (OLCF), Polaris (ALCF), Perlmutter (NERSC), Theta (ALCF) and Bebop. The major system tests ran heterogeneous workflows.
 
 :Known issues:
 
@@ -782,15 +804,15 @@
 * API change: persis_info now included as an argument to libE and is returned from libE instead of gen_info
 * Gen funcs: aposmm_logic module renamed to aposmm.
 * New example gen and allocation functions.
 * Updated Balsam launch script (with new Balsam workflow).
 * History is dumped to file on manager or worker exception and MPI aborted (with exit code 1). (#46)
 * Default logging level changed to DEBUG and redirected to file ensemble.log.
 * Added directory of standalone tests (comms, job kills, and nested MPI launches).
-* Improved and speeded up unit tests. (#68)
+* Improved and sped up unit tests. (#68)
 * Considerable documentation enhancements.
 
 :Known issues:
 
 * Open-MPI is not supported with direct MPI launches since nested MPI launches are not supported.
 
 Release 0.2.0
```

### Comparing `libensemble-1.2.2/CONTRIBUTING.rst` & `libensemble-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/LICENSE` & `libensemble-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/PKG-INFO` & `libensemble-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libensemble
-Version: 1.2.2
+Version: 1.3.0
 Summary: Library to coordinate the concurrent evaluation of dynamic ensembles of calculations
 Home-page: https://github.com/Libensemble/libensemble
 Author: Jeffrey Larson, Stephen Hudson, Stefan M. Wild, David Bindel and John-Luke Navarro
 Author-email: libensemble@lists.mcs.anl.gov
 License: BSD 3-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,50 +21,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 License-File: LICENSE
 
-.. image:: https://raw.githubusercontent.com/Libensemble/libensemble/main/docs/images/libE_logo.png
-   :align: center
-   :alt: libEnsemble
-
-|
-
-.. image:: https://img.shields.io/pypi/v/libensemble.svg?color=blue
-   :target: https://pypi.org/project/libensemble
-
-.. image:: https://img.shields.io/conda/v/conda-forge/libensemble?color=blue
-   :target: https://anaconda.org/conda-forge/libensemble
-
-.. image:: https://img.shields.io/spack/v/py-libensemble?color=blue
-   :target: https://packages.spack.io/package.html?name=py-libensemble
-
-|
-
-.. image:: https://github.com/Libensemble/libensemble/actions/workflows/extra.yml/badge.svg?branch=main
-   :target: https://github.com/Libensemble/libensemble/actions
-
-.. image:: https://codecov.io/github/Libensemble/libensemble/graph/badge.svg
-   :target: https://codecov.io/github/Libensemble/libensemble
-
-.. image:: https://readthedocs.org/projects/libensemble/badge/?maxAge=2592000
-   :target: https://libensemble.readthedocs.org/en/latest/
-   :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: black
+|libE_logo|
 
-.. image:: https://joss.theoj.org/papers/10.21105/joss.06031/status.svg
-   :target: https://doi.org/10.21105/joss.06031
-   :alt: JOSS Status
+|PyPI| |Conda| |Spack|
 
-|
+|Tests| |Coverage| |Docs| |Style| |JOSS|
 
 .. after_badges_rst_tag
 
 =====================================================================
 libEnsemble: A complete toolkit for dynamic ensembles of calculations
 =====================================================================
 
@@ -158,14 +127,37 @@
     volume  = {33},
     number  = {4},
     pages   = {977--988},
     year    = {2022},
     doi     = {10.1109/tpds.2021.3082815}
   }
 
+.. |libE_logo| image:: https://raw.githubusercontent.com/Libensemble/libensemble/main/docs/images/libE_logo.png
+   :align: middle
+   :alt: libEnsemble
+.. |PyPI| image:: https://img.shields.io/pypi/v/libensemble.svg?color=blue
+   :target: https://pypi.org/project/libensemble
+.. |Conda| image:: https://img.shields.io/conda/v/conda-forge/libensemble?color=blue
+   :target: https://anaconda.org/conda-forge/libensemble
+.. |Spack| image:: https://img.shields.io/spack/v/py-libensemble?color=blue
+   :target: https://packages.spack.io/package.html?name=py-libensemble
+.. |Tests| image:: https://github.com/Libensemble/libensemble/actions/workflows/extra.yml/badge.svg?branch=main
+   :target: https://github.com/Libensemble/libensemble/actions
+.. |Coverage| image:: https://codecov.io/github/Libensemble/libensemble/graph/badge.svg
+   :target: https://codecov.io/github/Libensemble/libensemble
+.. |Docs| image:: https://readthedocs.org/projects/libensemble/badge/?maxAge=2592000
+   :target: https://libensemble.readthedocs.org/en/latest/
+   :alt: Documentation Status
+.. |Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+.. |JOSS| image:: https://joss.theoj.org/papers/10.21105/joss.06031/status.svg
+   :target: https://doi.org/10.21105/joss.06031
+   :alt: JOSS Status
+
 .. _Community Examples repository: https://github.com/Libensemble/libe-community-examples
 .. _conda-forge: https://conda-forge.org/
 .. _Contributions: https://github.com/Libensemble/libensemble/blob/main/CONTRIBUTING.rst
 .. _docs: https://libensemble.readthedocs.io/en/main/advanced_installation.html
 .. _GitHub: https://github.com/Libensemble/libensemble
 .. _libEnsemble mailing list: https://lists.mcs.anl.gov/mailman/listinfo/libensemble
 .. _libEnsemble Slack page: https://libensemble.slack.com
```

### Comparing `libensemble-1.2.2/README.rst` & `libensemble-1.3.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,12 @@
-.. image:: https://raw.githubusercontent.com/Libensemble/libensemble/main/docs/images/libE_logo.png
-   :align: center
-   :alt: libEnsemble
-
-|
-
-.. image:: https://img.shields.io/pypi/v/libensemble.svg?color=blue
-   :target: https://pypi.org/project/libensemble
-
-.. image:: https://img.shields.io/conda/v/conda-forge/libensemble?color=blue
-   :target: https://anaconda.org/conda-forge/libensemble
-
-.. image:: https://img.shields.io/spack/v/py-libensemble?color=blue
-   :target: https://packages.spack.io/package.html?name=py-libensemble
-
-|
-
-.. image:: https://github.com/Libensemble/libensemble/actions/workflows/extra.yml/badge.svg?branch=main
-   :target: https://github.com/Libensemble/libensemble/actions
-
-.. image:: https://codecov.io/github/Libensemble/libensemble/graph/badge.svg
-   :target: https://codecov.io/github/Libensemble/libensemble
-
-.. image:: https://readthedocs.org/projects/libensemble/badge/?maxAge=2592000
-   :target: https://libensemble.readthedocs.org/en/latest/
-   :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: black
+|libE_logo|
 
-.. image:: https://joss.theoj.org/papers/10.21105/joss.06031/status.svg
-   :target: https://doi.org/10.21105/joss.06031
-   :alt: JOSS Status
+|PyPI| |Conda| |Spack|
 
-|
+|Tests| |Coverage| |Docs| |Style| |JOSS|
 
 .. after_badges_rst_tag
 
 =====================================================================
 libEnsemble: A complete toolkit for dynamic ensembles of calculations
 =====================================================================
 
@@ -131,14 +100,37 @@
     volume  = {33},
     number  = {4},
     pages   = {977--988},
     year    = {2022},
     doi     = {10.1109/tpds.2021.3082815}
   }
 
+.. |libE_logo| image:: https://raw.githubusercontent.com/Libensemble/libensemble/main/docs/images/libE_logo.png
+   :align: middle
+   :alt: libEnsemble
+.. |PyPI| image:: https://img.shields.io/pypi/v/libensemble.svg?color=blue
+   :target: https://pypi.org/project/libensemble
+.. |Conda| image:: https://img.shields.io/conda/v/conda-forge/libensemble?color=blue
+   :target: https://anaconda.org/conda-forge/libensemble
+.. |Spack| image:: https://img.shields.io/spack/v/py-libensemble?color=blue
+   :target: https://packages.spack.io/package.html?name=py-libensemble
+.. |Tests| image:: https://github.com/Libensemble/libensemble/actions/workflows/extra.yml/badge.svg?branch=main
+   :target: https://github.com/Libensemble/libensemble/actions
+.. |Coverage| image:: https://codecov.io/github/Libensemble/libensemble/graph/badge.svg
+   :target: https://codecov.io/github/Libensemble/libensemble
+.. |Docs| image:: https://readthedocs.org/projects/libensemble/badge/?maxAge=2592000
+   :target: https://libensemble.readthedocs.org/en/latest/
+   :alt: Documentation Status
+.. |Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+.. |JOSS| image:: https://joss.theoj.org/papers/10.21105/joss.06031/status.svg
+   :target: https://doi.org/10.21105/joss.06031
+   :alt: JOSS Status
+
 .. _Community Examples repository: https://github.com/Libensemble/libe-community-examples
 .. _conda-forge: https://conda-forge.org/
 .. _Contributions: https://github.com/Libensemble/libensemble/blob/main/CONTRIBUTING.rst
 .. _docs: https://libensemble.readthedocs.io/en/main/advanced_installation.html
 .. _GitHub: https://github.com/Libensemble/libensemble
 .. _libEnsemble mailing list: https://lists.mcs.anl.gov/mailman/listinfo/libensemble
 .. _libEnsemble Slack page: https://libensemble.slack.com
```

### Comparing `libensemble-1.2.2/docs/FAQ.rst` & `libensemble-1.3.0/docs/FAQ.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/Makefile` & `libensemble-1.3.0/docs/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
+#SPHINXOPTS    = -b spelling
 SPHINXOPTS    =
 SPHINXBUILD   = python3 -msphinx
 SPHINXPROJ    = libensemble
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
```

### Comparing `libensemble-1.2.2/docs/advanced_installation.rst` & `libensemble-1.3.0/docs/advanced_installation.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/conf.py` & `libensemble-1.3.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,25 +79,33 @@
 #
 needs_sphinx = "5.3"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
+    "sphinxcontrib.spelling",
     "sphinxcontrib.bibtex",
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     # 'sphinx.ext.autosectionlabel',
     "sphinx.ext.intersphinx",
     "sphinx.ext.imgconverter",
     "sphinx.ext.mathjax",
     "sphinxcontrib.autodoc_pydantic",
     "sphinx_design",
     "sphinx_copybutton",
 ]
+
+spelling_word_list_filename = "spelling_wordlist.txt"
+spelling_ignore_pypi_package_names = True
+spelling_ignore_acronyms = True
+spelling_ignore_python_builtins = True
+spelling_ignore_importable_modules = True
+
 bibtex_bibfiles = ["references.bib"]
 bibtex_default_style = "unsrt"
 # autosectionlabel_prefix_document = True
 # extensions = ['sphinx.ext.autodoc', 'sphinx.ext.napoleon', 'sphinx.ext.imgconverter']
 # breathe_projects = { "libEnsemble": "../code/src/xml/" }
 # breathe_default_project = "libEnsemble"
```

### Comparing `libensemble-1.2.2/docs/data_structures/alloc_specs.rst` & `libensemble-1.3.0/docs/data_structures/alloc_specs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/data_structures/exit_criteria.rst` & `libensemble-1.3.0/docs/data_structures/exit_criteria.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/data_structures/gen_specs.rst` & `libensemble-1.3.0/docs/data_structures/gen_specs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/data_structures/libE_specs.rst` & `libensemble-1.3.0/docs/data_structures/libE_specs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,23 @@
 
     .. tab-set::
 
         .. tab-item:: General
 
                 **comms** [str] = ``"mpi"``:
                     Manager/Worker communications mode: ``'mpi'``, ``'local'``, or ``'tcp'``.
+                    If ``nworkers`` is specified, then ``local`` comms will be used unless a
+                    parallel MPI environment is detected.
 
                 **nworkers** [int]:
-                    Number of worker processes in ``"local"`` or ``"tcp"``.
+                    Number of worker processes in ``"local"``, ``"threads"``, or ``"tcp"``.
+
+                **gen_on_manager** [bool] = False
+                    Instructs Manager process to run generator functions.
+                    This generator function can access/modify user objects by reference.
 
                 **mpi_comm** [MPI communicator] = ``MPI.COMM_WORLD``:
                     libEnsemble MPI communicator.
 
                 **dry_run** [bool] = ``False``:
                     Whether libEnsemble should immediately exit after validating all inputs.
 
@@ -47,14 +53,18 @@
                 **kill_canceled_sims** [bool] = ``False``:
                     Try to kill sims with ``cancel_requested`` set to ``True``.
                     If ``False``, the manager avoids this moderate overhead.
 
                 **disable_log_files** [bool] = ``False``:
                     Disable ``ensemble.log`` and ``libE_stats.txt`` log files.
 
+                **gen_workers** [list of ints]:
+                    List of workers that should run only generators. All other workers will run
+                    only simulator functions.
+
         .. tab-item:: Directories
 
             .. tab-set::
 
                 .. tab-item:: General
 
                     **use_workflow_dir** [bool] = ``False``:
```

### Comparing `libensemble-1.2.2/docs/data_structures/persis_info.rst` & `libensemble-1.3.0/docs/data_structures/persis_info.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,23 @@
       :emphasize-lines: 17
       :caption: libensemble/libensemble/gen_funcs/sampling.py
 
   .. tab-item:: Incrementing indexes or process counts
 
     .. literalinclude:: ../../libensemble/alloc_funcs/fast_alloc.py
        :linenos:
-       :start-at:     for wid in support.avail_worker_ids():
-       :end-before:         # Give sim work if possible
+       :start-at:     for wid in support.avail_worker_ids(gen_workers=False):
+       :end-before:         # Give gen work if possible
        :caption: libensemble/alloc_funcs/fast_alloc.py
 
   .. tab-item:: Tracking running generators
 
     .. literalinclude:: ../../libensemble/alloc_funcs/start_only_persistent.py
        :linenos:
-       :start-at:        avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=True)
+       :start-at:        avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=True, gen_workers=True)
        :end-before:    return Work, persis_info, 0
        :emphasize-lines: 18
        :caption: libensemble/alloc_funcs/start_only_persistent.py
 
   .. tab-item:: Allocation function triggers shutdown
 
     .. literalinclude:: ../../libensemble/alloc_funcs/start_only_persistent.py
```

### Comparing `libensemble-1.2.2/docs/data_structures/platform_specs.rst` & `libensemble-1.3.0/docs/data_structures/platform_specs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/data_structures/sim_specs.rst` & `libensemble-1.3.0/docs/data_structures/sim_specs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/rel_conda.rst` & `libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/rel_conda.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/rel_github.rst` & `libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/rel_github.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/rel_pypi.rst` & `libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/rel_pypi.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/dev_guide/release_management/release_platforms/rel_spack.rst` & `libensemble-1.3.0/docs/dev_guide/release_management/release_platforms/rel_spack.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/dev_guide/release_management/release_process.rst` & `libensemble-1.3.0/docs/dev_guide/release_management/release_process.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Release Process
 ===============
 
-A release
-can be undertaken only by a project administrator. A project administrator
-should have an administrator role on the libEnsemble GitHub, PyPI, and
-readthedocs pages.
+A release can be undertaken only by a project administrator. A project
+administrator should have an administrator role on the libEnsemble GitHub,
+PyPI, and readthedocs pages.
 
 Before release
 --------------
 
 - A GitHub issue is created with a checklist for the release.
 
 - A release branch should be taken off develop (or develop pulls controlled).
@@ -18,36 +17,42 @@
 
 - Version number is updated wherever it appears (and ``+dev`` suffix is removed)
   (in ``libensemble/version.py``).
 
 - Year in ``LICENSE`` is checked for correctness.
   (Note: The year generated in docs by ``docs/conf.py`` should be automatic).
 
-- ``setup.py`` and ``libensemble/__init__.py`` are checked to ensure all information is up to date.
+- ``setup.py`` and ``libensemble/__init__.py`` are checked to ensure all
+  information is up to date.
 
-- Update ``.wci.yml`` in root directory (version, date and any other information).
+- Update ``.wci.yml`` in root directory (version, date and any other
+  information).
 
-- ``MANIFEST.in`` is checked. Locally, try out ``python setup.py sdist`` and check created tarball.
-  contains correct files and directories for PyPI package.
-
-- Locally check that the example code in the README works with both local comms and mpi4py.
+- ``MANIFEST.in`` is checked. Locally, try out ``python setup.py sdist`` and
+  check the created tarball contains correct files and directories for PyPI
+  package.
 
 - Tests are run with source to be released (this may iterate):
 
   - On-line CI (GitHub Actions) tests must pass.
 
-  - Launch and verify extra tests: ``gh workflow run libEnsemble-complete-CI --ref branch_name``
+  - Launch and verify extra tests:
+    ``gh workflow run libEnsemble-complete-CI --ref branch_name``
 
-  - Scaling tests must be run on HPC platforms listed as supported in release notes.
-    Test variants by platform, launch mechanism, scale, and other factors can
-    be configured and exported by the libE-Templater_.
+  - Scaling tests must be run on HPC platforms listed as supported in release
+    notes. Test variants by platform, launch mechanism, scale, and other
+    factors can be configured and exported by the libE-Templater_.
 
   - Coverage must not have decreased unless there is a justifiable reason.
 
-  - Documentation must build and display correctly wherever hosted (currently readthedocs.com).
+  - Documentation must build and display correctly wherever hosted (currently
+    readthedocs.com).
+
+- Locally check that the example code in the README works with both local
+  comms and mpi4py.
 
 - Pull request from either the develop or release branch to main requesting
   one or more reviewers (including at least one other administrator).
 
 - Reviewer will check that all tests have passed and will then approve merge.
 
 During release
@@ -55,28 +60,35 @@
 
 An administrator will take the following steps.
 
 - Merge the pull request into main.
 
 - Once CI tests have passed on main:
 
-  - A GitHub release will be taken from the main (:ref:`github release<rel-github>`).
+  - A GitHub release will be taken from the main
+    (:ref:`github release<rel-github>`).
 
-  - A tarball (source distribution) will be uploaded to PyPI (:ref:`PyPI release<rel-pypi>`).
+  - A tarball (source distribution) will be uploaded to PyPI
+    (:ref:`PyPI release<rel-pypi>`).
 
   - The Conda package will be updated (:ref:`Conda release<rel-conda>`).
 
   - Spack package will be updated (:ref:`Spack release<rel-spack>`).
 
-- If the merge was made from a release branch (instead of develop), merge this branch into develop.
+- If the merge was made from a release branch (instead of develop), merge this
+  branch into develop.
 
-- Create a new commit on develop that appends ``+dev`` to the version number (wherever is appears).
+- Create a new commit on develop that appends ``+dev`` to the version number
+  (wherever is appears).
 
 After release
 -------------
 
-- Ensure all relevant GitHub issues are closed and moved to the *Done* column
-  on the kanban project board (inc. the release checklist).
+- Email the libEnsemble mailing list, and notify the `everyone` channel in the
+  libEnsemble Slack workspace with an announcement and quick summary of the
+  release.
 
-- Email libEnsemble mailing list, and notify the `everyone` channel in the libEnsemble Slack workspace.
+- Ensure all relevant GitHub issues are closed and moved to the *Done* column
+  on the kanban project board (inc. the release checklist). Those that were
+  already in *Done* should be archived.
 
 .. _libE-Templater: https://github.com/Libensemble/libE-templater
```

### Comparing `libensemble-1.2.2/docs/examples/alloc_funcs.rst` & `libensemble-1.3.0/docs/examples/alloc_funcs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 
    .. literalinclude:: ../../libensemble/alloc_funcs/start_only_persistent.py
       :language: python
       :linenos:
 
 start_persistent_local_opt_gens
 -------------------------------
-.. automodule:: libensemble.alloc_funcs.start_persistent_local_opt_gens
+.. automodule:: start_persistent_local_opt_gens
   :members:
   :undoc-members:
```

### Comparing `libensemble-1.2.2/docs/examples/aposmm.rst` & `libensemble-1.3.0/docs/examples/aposmm.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/examples/calling_scripts.rst` & `libensemble-1.3.0/docs/examples/calling_scripts.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/examples/examples_index.rst` & `libensemble-1.3.0/docs/examples/examples_index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/examples/sampling.rst` & `libensemble-1.3.0/docs/examples/sampling.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/examples/sim_funcs.rst` & `libensemble-1.3.0/docs/examples/sim_funcs.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/examples/surmise.rst` & `libensemble-1.3.0/docs/examples/surmise.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/examples/tasmanian.rst` & `libensemble-1.3.0/docs/examples/tasmanian.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/executor/executor.rst` & `libensemble-1.3.0/docs/executor/executor.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/executor/mpi_executor.rst` & `libensemble-1.3.0/docs/executor/mpi_executor.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/executor/overview.rst` & `libensemble-1.3.0/docs/executor/overview.rst`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 .. note::
     Applications or tasks submitted via the Balsam Executor are referred to as
     **"jobs"** within Balsam, including within Balsam's database and when
     describing the state of a completed submission.
 
 The ``MPIExecutor`` autodetects system criteria such as the appropriate MPI launcher
 and mechanisms to poll and kill tasks. It also has access to the resource manager,
-which partitions resources amongst workers, ensuring that runs utilize different
+which partitions resources among workers, ensuring that runs utilize different
 resources (e.g., nodes). Furthermore, the ``MPIExecutor`` offers resilience via the
 feature of re-launching tasks that fail to start because of system factors.
 
 Various back-end mechanisms may be used by the Executor to best interact
 with each system, including proxy launchers or task management systems such as
 Balsam_. Currently, these Executors launch at the application level within
 an existing resource pool. However, submissions to a batch scheduler may be
```

### Comparing `libensemble-1.2.2/docs/function_guides/allocator.rst` & `libensemble-1.3.0/docs/function_guides/allocator.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/function_guides/calc_status.rst` & `libensemble-1.3.0/docs/function_guides/calc_status.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/function_guides/function_guide_index.rst` & `libensemble-1.3.0/docs/function_guides/function_guide_index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/function_guides/generator.rst` & `libensemble-1.3.0/docs/function_guides/generator.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/function_guides/history_array.rst` & `libensemble-1.3.0/docs/function_guides/history_array.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/function_guides/sim_gen_alloc_api.rst` & `libensemble-1.3.0/docs/function_guides/sim_gen_alloc_api.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/function_guides/simulator.rst` & `libensemble-1.3.0/docs/function_guides/simulator.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/function_guides/work_dict.rst` & `libensemble-1.3.0/docs/function_guides/work_dict.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/function_guides/worker_array.rst` & `libensemble-1.3.0/docs/function_guides/worker_array.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/history_output_logging.rst` & `libensemble-1.3.0/docs/history_output_logging.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/adaptiveloop.png` & `libensemble-1.3.0/docs/images/adaptiveloop.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/balsam2.png` & `libensemble-1.3.0/docs/images/balsam2.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/basic_6hc.png` & `libensemble-1.3.0/docs/images/basic_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/centralized_new_detailed.png` & `libensemble-1.3.0/docs/images/centralized_new_detailed.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/diagram_with_persis.png` & `libensemble-1.3.0/docs/images/diagram_with_persis.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/diagram_xml/adaptiveloop.xml` & `libensemble-1.3.0/docs/images/diagram_xml/adaptiveloop.xml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/diagram_xml/balsam2.xml` & `libensemble-1.3.0/docs/images/diagram_xml/balsam2.xml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/diagram_xml/persis_add_worker.xml` & `libensemble-1.3.0/docs/images/diagram_xml/persis_add_worker.xml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/diagram_xml/persis_wasted_node.xml` & `libensemble-1.3.0/docs/images/diagram_xml/persis_wasted_node.xml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/distributed_new_detailed.png` & `libensemble-1.3.0/docs/images/distributed_new_detailed.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/funcxmodel.png` & `libensemble-1.3.0/docs/images/funcxmodel.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/gen_v_fail_or_cancel.png` & `libensemble-1.3.0/docs/images/gen_v_fail_or_cancel.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/history_gen1.png` & `libensemble-1.3.0/docs/images/history_gen1.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/history_gen2.png` & `libensemble-1.3.0/docs/images/history_gen2.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/history_init.png` & `libensemble-1.3.0/docs/images/history_init.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/history_sim1.png` & `libensemble-1.3.0/docs/images/history_sim1.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/libE_logo.png` & `libensemble-1.3.0/docs/images/libE_logo.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/libE_logo_circle.png` & `libensemble-1.3.0/docs/images/libE_logo_circle.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/libE_logo_white.png` & `libensemble-1.3.0/docs/images/libE_logo_white.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/libEnsemble_Logo.svg` & `libensemble-1.3.0/docs/images/libEnsemble_Logo.svg`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png` & `libensemble-1.3.0/docs/images/libe_opal_complete_v_killed_511w_2044sims_1030nodes.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png` & `libensemble-1.3.0/docs/images/libe_opal_util_v_time_511w_2044sims_1030nodes.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/localopt_6hc.png` & `libensemble-1.3.0/docs/images/localopt_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/persis_add_worker.png` & `libensemble-1.3.0/docs/images/persis_add_worker.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/persis_wasted_node.png` & `libensemble-1.3.0/docs/images/persis_wasted_node.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/sampling_6hc.png` & `libensemble-1.3.0/docs/images/sampling_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/sinex.png` & `libensemble-1.3.0/docs/images/sinex.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/variable_resources1.png` & `libensemble-1.3.0/docs/images/variable_resources1.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/variable_resources2.png` & `libensemble-1.3.0/docs/images/variable_resources2.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/variable_resources3.png` & `libensemble-1.3.0/docs/images/variable_resources3.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/variable_resources_larger_rsets1.png` & `libensemble-1.3.0/docs/images/variable_resources_larger_rsets1.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/variable_resources_more_rsets1.png` & `libensemble-1.3.0/docs/images/variable_resources_more_rsets1.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/variable_resources_persis_gen1.png` & `libensemble-1.3.0/docs/images/variable_resources_persis_gen1.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/images/variable_resources_sched_opts.png` & `libensemble-1.3.0/docs/images/variable_resources_sched_opts.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/index.rst` & `libensemble-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/introduction.rst` & `libensemble-1.3.0/docs/introduction.rst`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   - Tasmanian_ Toolkit for Adaptive Stochastic Modeling and Non-Intrusive ApproximatioN
   - VTMOP_ Fortran package for large-scale multiobjective multidisciplinary design optimization
 
   libEnsemble has also been used to coordinate many computationally expensive
   simulations. Select examples include:
 
   - OPAL_ Object Oriented Parallel Accelerator Library. (See this `IPAC manuscript`_.)
-  - WarpX_ Advanced electromagnetic particle-in-cell code. (See example `WarpX + libE scripts`_.)
+  - WarpX_ Advanced electromagnetic particle-in-cell code.
 
 .. _APOSMM: https://link.springer.com/article/10.1007/s12532-017-0131-4
 .. _Community Examples repository: https://github.com/Libensemble/libe-community-examples
 .. _DEAP: https://deap.readthedocs.io/en/master/overview.html
 .. _DFO-LS: https://github.com/numericalalgorithmsgroup/dfols
 .. _ECNoise: https://www.mcs.anl.gov/~wild/cnoise/
 .. _IPAC manuscript: https://doi.org/10.18429/JACoW-ICAP2018-SAPAF03
@@ -48,9 +48,8 @@
 .. _OPAL: http://amas.web.psi.ch/docs/opal/opal_user_guide-1.6.0.pdf
 .. _PETSc/TAO: http://www.mcs.anl.gov/petsc
 .. _scipy.optimize: https://docs.scipy.org/doc/scipy/reference/optimize.html
 .. _Surmise: https://surmise.readthedocs.io/en/latest/index.html
 .. _Tasmanian: https://tasmanian.ornl.gov/
 .. _user guide: https://libensemble.readthedocs.io/en/latest/programming_libE.html
 .. _VTMOP: https://github.com/Libensemble/libe-community-examples#vtmop
-.. _WarpX + libE scripts: https://warpx.readthedocs.io/en/latest/usage/workflows/libensemble.html
 .. _WarpX: https://warpx.readthedocs.io/en/latest/
```

### Comparing `libensemble-1.2.2/docs/introduction_latex.rst` & `libensemble-1.3.0/docs/introduction_latex.rst`

 * *Files 6% similar despite different names*

```diff
@@ -53,9 +53,8 @@
 .. _tarball: https://github.com/Libensemble/libensemble/releases/latest
 .. _Tasmanian: https://tasmanian.ornl.gov/
 .. _tomli: https://pypi.org/project/tomli/
 .. _tqdm: https://tqdm.github.io/
 .. _user guide: https://libensemble.readthedocs.io/en/latest/programming_libE.html
 .. _VTMOP: https://github.com/Libensemble/libe-community-examples#vtmop
 .. _WarpX: https://warpx.readthedocs.io/en/latest/
-.. _WarpX + libE scripts: https://warpx.readthedocs.io/en/latest/usage/workflows/libensemble.html
 .. _xsdk: https://xsdk.info
```

### Comparing `libensemble-1.2.2/docs/known_issues.rst` & `libensemble-1.3.0/docs/known_issues.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/latex_index.rst` & `libensemble-1.3.0/docs/latex_index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/nitpicky` & `libensemble-1.3.0/docs/nitpicky`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/overview_usecases.rst` & `libensemble-1.3.0/docs/overview_usecases.rst`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     functions may also be constructed to communicate directly with the manager,
     for example, to efficiently maintain and update data structures instead of
     communicating them between manager and worker. These calculations
     and the workers assigned to them are referred to as *persistent*.
 
   * **Resource Manager** libEnsemble has a built-in resource manager that can detect
     (or be provided with) a set of resources (e.g., a node-list). Resources are
-    divided up amongst workers (using *resource sets*) and can be dynamically
+    divided up among workers (using *resource sets*) and can be dynamically
     reassigned.
 
   * **Resource Set**: The smallest unit of resources that can be assigned (and
     dynamically reassigned) to workers. By default it is the provisioned resources
     divided by the number of workers (excluding any workers given in the
     ``zero_resource_workers`` libE_specs option). However, it can also be set
     directly by the ``num_resource_sets`` libE_specs option.
```

### Comparing `libensemble-1.2.2/docs/platforms/aurora.rst` & `libensemble-1.3.0/docs/platforms/aurora.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/platforms/bebop.rst` & `libensemble-1.3.0/docs/platforms/bebop.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/platforms/example_scripts.rst` & `libensemble-1.3.0/docs/platforms/example_scripts.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/platforms/frontier.rst` & `libensemble-1.3.0/docs/platforms/frontier.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/platforms/improv.rst` & `libensemble-1.3.0/docs/platforms/improv.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/platforms/perlmutter.rst` & `libensemble-1.3.0/docs/platforms/perlmutter.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/platforms/platforms_index.rst` & `libensemble-1.3.0/docs/platforms/platforms_index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     mpirun -np 5 python myscript.py
 
 or::
 
     python myscript.py --comms local --nworkers 4
 
 Either of these will run libEnsemble (inc. manager and 4 workers) on the first node. The remaining
-4 nodes will be divided amongst the workers for submitted applications. If the same run was
+4 nodes will be divided among the workers for submitted applications. If the same run was
 performed without ``libE_specs["dedicated_mode"]=True``, runs could be submitted to all 5 nodes. The number of workers
 can be modified to allow either multiple workers to map to each node or multiple nodes per worker.
 
 To launch libEnsemble distributed requires a less trivial libEnsemble run script.
 For example::
 
     mpirun -np 5 -ppn 1 python myscript.py
```

### Comparing `libensemble-1.2.2/docs/platforms/polaris.rst` & `libensemble-1.3.0/docs/platforms/polaris.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 Configuring Python and Installation
 -----------------------------------
 
 Python and libEnsemble are available on Polaris with the `conda` module. Load the
 ``conda`` module and activate the base environment::
 
-    module load conda
-    conda activate base
+    module use /soft/modulefiles
+    module load conda; conda activate
 
 This also gives you access to machine-optimized packages such as mpi4py_.
 
 To install further packages, including updating libEnsemble, you may either create
 a virtual environment on top of this (if just using ``pip install``) or clone the base
 environment (if you need ``conda install``). More details at `Python for Polaris`_.
 
@@ -97,8 +97,8 @@
 of this example is also available.
 
 .. _ALCF: https://www.alcf.anl.gov/
 .. _conda: https://conda.io/en/latest/
 .. _demonstration: https://youtu.be/Ff0dYYLQzoU
 .. _mpi4py: https://mpi4py.readthedocs.io/en/stable/
 .. _Polaris: https://www.alcf.anl.gov/polaris
-.. _Python for Polaris: https://www.alcf.anl.gov/support/user-guides/polaris/data-science-workflows/python/index.html
+.. _Python for Polaris: https://docs.alcf.anl.gov/polaris/data-science-workflows/python/
```

### Comparing `libensemble-1.2.2/docs/platforms/spock_crusher.rst` & `libensemble-1.3.0/docs/platforms/spock_crusher.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/platforms/srun.rst` & `libensemble-1.3.0/docs/platforms/srun.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/platforms/summit.rst` & `libensemble-1.3.0/docs/platforms/summit.rst`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     task = exctr.submit(app_name="mycode",
                         extra_args="-n 3 -a 1 -g 1 -c 1 --bind=packed:1 --smpiargs="-gpu""
                         app_args="-i input")
 
 The libEnsemble resource manager works out the resources available to each worker,
 but unlike some other systems, ``jsrun`` on Summit dynamically schedules runs to
 available slots across and within nodes. It can also queue tasks. This allows variable
-size runs to easily be handled on Summit. If oversubsciption to the `jsrun` system
+size runs to easily be handled on Summit. If oversubscription to the `jsrun` system
 is desired, then libEnsemble's resource manager can be disabled in the
 calling script via::
 
     libE_specs["disable_resource_manager"] = True
 
 In the above example, the task being submitted used three GPUs, which is half those
 available on a Summit node, and thus two such tasks may be allocated to each node
```

### Comparing `libensemble-1.2.2/docs/posters.rst` & `libensemble-1.3.0/docs/posters.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/programming_libE.rst` & `libensemble-1.3.0/docs/programming_libE.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/resource_manager/overview.rst` & `libensemble-1.3.0/docs/resource_manager/overview.rst`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 from the user.
 
 .. image:: ../images/variable_resources2.png
 
 .. image:: ../images/variable_resources3.png
 
 The particular nodes and slots assigned to each worker will be determined by the
-libEnsenble :doc:`built-in scheduler<scheduler_module>`, although users can provide
+libEnsemble :doc:`built-in scheduler<scheduler_module>`, although users can provide
 an alternative scheduler via the :doc:`allocation function<../function_guides/allocator>`.
 In short, the scheduler will prefer fitting simulations onto a node, and using
 even splits across nodes, if necessary.
 
 Accessing resources from the simulation function
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
```

### Comparing `libensemble-1.2.2/docs/resource_manager/resource_detection.rst` & `libensemble-1.3.0/docs/resource_manager/resource_detection.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/resource_manager/resources_index.rst` & `libensemble-1.3.0/docs/resource_manager/resources_index.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/resource_manager/scheduler_module.rst` & `libensemble-1.3.0/docs/resource_manager/scheduler_module.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/resource_manager/zero_resource_workers.rst` & `libensemble-1.3.0/docs/resource_manager/zero_resource_workers.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/rst_formatting_guidelines` & `libensemble-1.3.0/docs/rst_formatting_guidelines`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/running_libE.rst` & `libensemble-1.3.0/docs/running_libE.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 .. _running-libe:
 
 Running libEnsemble
 ===================
 
+Introduction
+------------
+
 libEnsemble runs with one manager and multiple workers. Each worker may run either
 a generator or simulator function (both are Python scripts). Generators
 determine the parameters/inputs for simulations. Simulator functions run and
 manage simulations, which often involve running a user application (see
 :doc:`Executor<executor/ex_index>`).
 
+.. note::
+    As of version 1.3.0, the generator can be run as a thread on the manager,
+    using the :ref:`libE_specs<datastruct-libe-specs>` option **gen_on_manager**.
+    When using this option, set the number of workers desired for running
+    simulations. See :ref:`Running generator on the manager<gen-on-manager>`
+    for more details.
+
 To use libEnsemble, you will need a calling script, which in turn will specify
 generator and simulator functions. Many :doc:`examples<examples/examples_index>`
 are available.
 
 There are currently three communication options for libEnsemble (determining how
 the Manager and Workers communicate). These are ``mpi``, ``local``, ``tcp``.
 The default is ``mpi``.
@@ -56,15 +66,15 @@
         Uses Python's built-in multiprocessing_ module.
         The ``comms`` type ``local`` and number of workers ``nworkers`` may
         be provided in :ref:`libE_specs<datastruct-libe-specs>`.
         Then run::
 
             python myscript.py
 
-        Or, if the script uses the :doc:`parse_args()<utilities>` function
+        Or, if the script uses the :meth:`parse_args<tools.parse_args>` function
         or an :class:`Ensemble<libensemble.ensemble.Ensemble>` object with ``Ensemble(parse_args=True)``,
         you can specify these on the command line::
 
             python myscript.py --comms local --nworkers N
 
         This will launch one manager and ``N`` workers.
 
@@ -94,32 +104,93 @@
         :class:`libE_specs<libensemble.specs.LibeSpecs>`, or on the command line
         if using an :class:`Ensemble<libensemble.ensemble.Ensemble>` object with
         ``Ensemble(parse_args=True)``,
 
         **Reverse-ssh interface**
 
         Set ``comms`` to ``ssh`` to launch workers on remote ssh-accessible systems. This
-        colocates workers, functions, and any applications. User
+        co-locates workers, functions, and any applications. User
         functions can also be persistent, unlike when launching remote functions via
         :ref:`Globus Compute<globus_compute_ref>`.
 
         The remote working directory and Python need to be specified. This may resemble::
 
             python myscript.py --comms ssh --workers machine1 machine2 --worker_pwd /home/workers --worker_python /home/.conda/.../python
 
         **Limitations of TCP mode**
 
         - There cannot be two calls to ``libE()`` or ``Ensemble.run()`` in the same script.
 
 Further Command Line Options
 ----------------------------
 
-See the **parse_args()** function in :doc:`Convenience Tools<utilities>` for
+See the :meth:`parse_args<tools.parse_args>` function in :doc:`Convenience Tools<utilities>` for
 further command line options.
 
+Persistent Workers
+------------------
+.. _persis_worker:
+
+In a regular (non-persistent) worker, the user's generator or simulation function is called
+whenever the worker receives work. A persistent worker is one that continues to run the
+generator or simulation function between work units, maintaining the local data environment.
+
+A common use-case consists of a persistent generator (such as :doc:`persistent_aposmm<examples/gen_funcs>`)
+that maintains optimization data while generating new simulation inputs. The persistent generator runs
+on a dedicated worker while in persistent mode. This requires an appropriate
+:doc:`allocation function<examples/alloc_funcs>` that will run the generator as persistent.
+
+When running with a persistent generator, it is important to remember that a worker will be dedicated
+to the generator and cannot run simulations. For example, the following run::
+
+    mpirun -np 3 python my_script.py
+
+starts one manager, one worker with a persistent generator, and one worker for running simulations.
+
+If this example was run as::
+
+    mpirun -np 2 python my_script.py
+
+No simulations will be able to run.
+
+.. _gen-on-manager:
+
+Running generator on the manager
+--------------------------------
+
+The majority of libEnsemble use cases run a single generator. The
+:ref:`libE_specs<datastruct-libe-specs>` option **gen_on_manager** will cause
+the generator function to run on a thread on the manager. This can run
+persistent user functions, sharing data structures with the manager, and avoids
+additional communication to a generator running on a worker. When using this
+option, the number of workers specified should be the (maximum) number of
+concurrent simulations.
+
+If modifying a workflow to use ``gen_on_manager`` consider the following.
+
+* Set ``nworkers`` to the number of workers desired for running simulations.
+* If using :meth:`add_unique_random_streams()<tools.add_unique_random_streams>`
+  to seed random streams, the default generator seed will be zero.
+* If you have a line like ``libE_specs["nresource_sets"] = nworkers -1``, this
+  line should be removed.
+* If the generator does use resources, ``nresource_sets`` can be increased as needed
+  so that the generator and all simulations are resourced.
+
+Environment Variables
+---------------------
+
+Environment variables required in your run environment can be set in your Python sim or gen function.
+For example::
+
+    os.environ["OMP_NUM_THREADS"] = 4
+
+set in your simulation script before the Executor *submit* command will export the setting
+to your run. For running a bash script in a sub environment when using the Executor, see
+the ``env_script`` option to the :doc:`MPI Executor<executor/mpi_executor>`.
+
 .. _liberegister:
 
 liberegister / libesubmit
 -------------------------
 
 Command-line utilities for preparing and launching libEnsemble workflows onto almost
 any machine and any scheduler, using a `PSI/J`_ Python implementation.
@@ -243,52 +314,14 @@
                         "launcher": null
                     }
                 }
 
         If libesubmit is run on a ``.json`` serialization from liberegister and can't find the
         specified calling script, it'll help search for matching candidate scripts.
 
-Persistent Workers
-------------------
-.. _persis_worker:
-
-In a regular (non-persistent) worker, the user's generator or simulation function is called
-whenever the worker receives work. A persistent worker is one that continues to run the
-generator or simulation function between work units, maintaining the local data environment.
-
-A common use-case consists of a persistent generator (such as :doc:`persistent_aposmm<examples/gen_funcs>`)
-that maintains optimization data while generating new simulation inputs. The persistent generator runs
-on a dedicated worker while in persistent mode. This requires an appropriate
-:doc:`allocation function<examples/alloc_funcs>` that will run the generator as persistent.
-
-When running with a persistent generator, it is important to remember that a worker will be dedicated
-to the generator and cannot run simulations. For example, the following run::
-
-    mpirun -np 3 python my_script.py
-
-starts one manager, one worker with a persistent generator, and one worker for running simulations.
-
-If this example was run as::
-
-    mpirun -np 2 python my_script.py
-
-No simulations will be able to run.
-
-Environment Variables
----------------------
-
-Environment variables required in your run environment can be set in your Python sim or gen function.
-For example::
-
-    os.environ["OMP_NUM_THREADS"] = 4
-
-set in your simulation script before the Executor *submit* command will export the setting
-to your run. For running a bash script in a sub environment when using the Executor, see
-the ``env_script`` option to the :doc:`MPI Executor<executor/mpi_executor>`.
-
 Further Run Information
 -----------------------
 
 For running on multi-node platforms and supercomputers, there are alternative ways to configure
 libEnsemble to resources. See the :doc:`Running on HPC Systems<platforms/platforms_index>`
 guide for more information, including some examples for specific systems.
```

### Comparing `libensemble-1.2.2/docs/tutorials/aposmm_tutorial.rst` & `libensemble-1.3.0/docs/tutorials/aposmm_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/tutorials/calib_cancel_tutorial.rst` & `libensemble-1.3.0/docs/tutorials/calib_cancel_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/tutorials/executor_forces_tutorial.rst` & `libensemble-1.3.0/docs/tutorials/executor_forces_tutorial.rst`

 * *Files 6% similar despite different names*

```diff
@@ -330,11 +330,47 @@
                         task.kill()
 
             if task.runtime > 60:
                 task.kill()
 
         ...
 
+Running the generator on the manager
+------------------------------------
+
+As of version 1.3.0, the generator can be run on a thread on the manager,
+using the :ref:`libE_specs<datastruct-libe-specs>` option **gen_on_manager**.
+
+Change the libE_specs as follows.
+
+   .. code-block:: python
+    :linenos:
+    :lineno-start: 28
+
+    nsim_workers = ensemble.nworkers
+
+    # Persistent gen does not need resources
+    ensemble.libE_specs = LibeSpecs(
+        gen_on_manager=True, sim_dirs_make=True, ensemble_dir_path="./test_executor_forces_tutorial"
+    )
+
+When running set ``nworkers`` to the number of workers desired for running simulations.
+E.g., Instead of:
+
+.. code-block:: bash
+
+    python run_libe_forces.py --comms local --nworkers 5
+
+use:
+
+.. code-block:: bash
+
+    python run_libe_forces.py --comms local --nworkers 4
+
+Note that as the generator random number seed will be zero instead of one, the checksum will change.
+
+For more information see :ref:`Running generator on the manager<gen-on-manager>`.
+
 .. _examples/tutorials/forces_with_executor: https://github.com/Libensemble/libensemble/tree/develop/examples/tutorials/forces_with_executor
 .. _forces_app: https://github.com/Libensemble/libensemble/tree/main/libensemble/tests/scaling_tests/forces/forces_app
 .. _forces_simple: https://github.com/Libensemble/libensemble/tree/main/libensemble/tests/scaling_tests/forces/forces_simple
 .. _GitHub: https://github.com/Libensemble/libensemble/issues
```

### Comparing `libensemble-1.2.2/docs/tutorials/forces_gpu_tutorial.rst` & `libensemble-1.3.0/docs/tutorials/forces_gpu_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/tutorials/local_sine_tutorial.rst` & `libensemble-1.3.0/docs/tutorials/local_sine_tutorial.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/utilities.rst` & `libensemble-1.3.0/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/welcome.rst` & `libensemble-1.3.0/docs/welcome.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/docs/xSDK_policy_compatibility.md` & `libensemble-1.3.0/docs/xSDK_policy_compatibility.md`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/README.rst` & `libensemble-1.3.0/examples/README.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/alloc_funcs/fast_alloc.py` & `libensemble-1.3.0/examples/alloc_funcs/fast_alloc.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,29 +28,30 @@
 
     support = AllocSupport(W, manage_resources, persis_info, libE_info)
 
     gen_count = support.count_gens()
     Work = {}
     gen_in = gen_specs.get("in", [])
 
-    for wid in support.avail_worker_ids():
+    # Give sim work if possible
+    for wid in support.avail_worker_ids(gen_workers=False):
         persis_info = support.skip_canceled_points(H, persis_info)
-
-        # Give sim work if possible
         if persis_info["next_to_give"] < len(H):
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], [persis_info["next_to_give"]], [])
             except InsufficientFreeResources:
                 break
             persis_info["next_to_give"] += 1
 
-        elif gen_count < user.get("num_active_gens", gen_count + 1):
-            # Give gen work
-            return_rows = range(len(H)) if gen_in else []
-            try:
-                Work[wid] = support.gen_work(wid, gen_in, return_rows, persis_info.get(wid))
-            except InsufficientFreeResources:
-                break
-            gen_count += 1
-            persis_info["total_gen_calls"] += 1
+    # Give gen work if possible
+    if persis_info["next_to_give"] >= len(H):
+        for wid in support.avail_worker_ids(gen_workers=True):
+            if wid not in Work and gen_count < user.get("num_active_gens", gen_count + 1):
+                return_rows = range(len(H)) if gen_in else []
+                try:
+                    Work[wid] = support.gen_work(wid, gen_in, return_rows, persis_info.get(wid))
+                except InsufficientFreeResources:
+                    break
+                gen_count += 1
+                persis_info["total_gen_calls"] += 1
 
     return Work, persis_info
```

### Comparing `libensemble-1.2.2/examples/alloc_funcs/give_sim_work_first.py` & `libensemble-1.3.0/examples/alloc_funcs/give_sim_work_first.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,23 +60,27 @@
 
     manage_resources = libE_info["use_resource_sets"]
     support = AllocSupport(W, manage_resources, persis_info, libE_info)
     gen_count = support.count_gens()
     Work = {}
 
     points_to_evaluate = ~H["sim_started"] & ~H["cancel_requested"]
-    for wid in support.avail_worker_ids():
-        if np.any(points_to_evaluate):
+
+    if np.any(points_to_evaluate):
+        for wid in support.avail_worker_ids(gen_workers=False):
             sim_ids_to_send = support.points_by_priority(H, points_avail=points_to_evaluate, batch=batch_give)
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], sim_ids_to_send, persis_info.get(wid))
             except InsufficientFreeResources:
                 break
             points_to_evaluate[sim_ids_to_send] = False
-        else:
+            if not np.any(points_to_evaluate):
+                break
+    else:
+        for wid in support.avail_worker_ids(gen_workers=True):
             # Allow at most num_active_gens active generator instances
             if gen_count >= user.get("num_active_gens", gen_count + 1):
                 break
 
             # Do not start gen instances in batch mode if workers still working
             if user.get("batch_mode") and not support.all_sim_ended(H):
                 break
```

### Comparing `libensemble-1.2.2/examples/alloc_funcs/start_only_persistent.py` & `libensemble-1.3.0/examples/alloc_funcs/start_only_persistent.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     persistent=True,
                     active_recv=active_recv_gen,
                 )
                 returned_but_not_given[point_ids] = False
 
     # Now the give_sim_work_first part
     points_to_evaluate = ~H["sim_started"] & ~H["cancel_requested"]
-    avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=False)
+    avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=False, gen_workers=False)
     if user.get("alt_type"):
         avail_workers = list(
             set(support.avail_worker_ids(persistent=False, zero_resource_workers=False))
             | set(support.avail_worker_ids(persistent=EVAL_SIM_TAG, zero_resource_workers=False))
         )
     for wid in avail_workers:
         if not np.any(points_to_evaluate):
@@ -111,15 +111,15 @@
         except InsufficientFreeResources:
             break
 
         points_to_evaluate[sim_ids_to_send] = False
 
     # Start persistent gens if no worker to give out. Uses zero_resource_workers if defined.
     if not np.any(points_to_evaluate):
-        avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=True)
+        avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=True, gen_workers=True)
 
         for wid in avail_workers:
             if gen_count < user.get("num_active_gens", 1):
                 # Finally, start a persistent generator as there is nothing else to do.
                 try:
                     Work[wid] = support.gen_work(
                         wid,
```

### Comparing `libensemble-1.2.2/examples/alloc_funcs/start_persistent_local_opt_gens.py` & `libensemble-1.3.0/examples/alloc_funcs/start_persistent_local_opt_gens.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         gen_inds = H["gen_worker"] == wid
         if support.all_sim_ended(H, gen_inds):
             last_time_pos = np.argmax(H["sim_started_time"][gen_inds])
             last_ind = np.nonzero(gen_inds)[0][last_time_pos]
             Work[wid] = support.gen_work(wid, gen_specs["persis_in"], last_ind, persis_info[wid], persistent=True)
             persis_info[wid]["run_order"].append(last_ind)
 
-    for wid in support.avail_worker_ids(persistent=False):
+    for wid in support.avail_worker_ids(persistent=False, gen_workers=True):
         # Find candidates to start local opt runs if a sample has been evaluated
         if np.any(np.logical_and(~H["local_pt"], H["sim_ended"], ~H["cancel_requested"])):
             n = len(H["x"][0])
             rk_c = extract_rk_c(gen_specs["user"], n)
             n_s = np.sum(~H["local_pt"])
             update_history_dist(H, n)
             starting_inds = decide_where_to_start_localopt(H, n, n_s, rk_c)
@@ -74,25 +74,29 @@
             except InsufficientFreeResources:
                 break
             H["started_run"][ind] = 1
             H["num_active_runs"][ind] += 1
             persis_info[wid]["run_order"] = [ind]
             gen_count += 1
 
-        elif np.any(points_to_evaluate):
+    if np.any(points_to_evaluate):
+        for wid in support.avail_worker_ids(persistent=False, gen_workers=False):
             # Perform sim evaluations from existing runs
             q_inds_logical = np.logical_and(points_to_evaluate, H["local_pt"])
             if not np.any(q_inds_logical):
                 q_inds_logical = points_to_evaluate
             sim_ids_to_send = np.nonzero(q_inds_logical)[0][0]  # oldest point
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], sim_ids_to_send, [])
             except InsufficientFreeResources:
                 break
             points_to_evaluate[sim_ids_to_send] = False
+            if not np.any(points_to_evaluate):
+                break
 
-        elif gen_count == 0 and not np.any(np.logical_and(W["active"] == EVAL_GEN_TAG, W["persis_state"] == 0)):
-            # Finally, generate points since there is nothing else to do (no resource sets req.)
-            Work[wid] = support.gen_work(wid, gen_specs.get("in", []), [], persis_info[wid], rset_team=[])
-            gen_count += 1
+    if gen_count == 0 and not np.any(np.logical_and(W["active"] == EVAL_GEN_TAG, W["persis_state"] == 0)):
+        # Finally, generate points since there is nothing else to do (no resource sets req.)
+        wid = support.avail_worker_ids(persistent=False, gen_workers=True)[0]
+        Work[wid] = support.gen_work(wid, gen_specs.get("in", []), [], persis_info[wid], rset_team=[])
+        gen_count += 1
 
     return Work, persis_info
```

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/common.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/common.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/optimizer.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/optimizer.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ECnoise.m`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/exe.pl` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/exe.pl`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.pl` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.pl`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/processexe.pl` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/processexe.pl`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/runs.sh` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/runs.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/support.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/support.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_1d_sampling.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_1d_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_GPU_variable_resources.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_GPU_variable_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_GPU_variable_resources_multi_task.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_GPU_variable_resources_multi_task.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_ensemble_platform_workdir.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_ensemble_platform_workdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import glob
 import os
 import re
+
 import numpy as np
 
+# Import libEnsemble items for this test
+from libensemble import Ensemble
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
 from libensemble.executors.mpi_executor import MPIExecutor
 from libensemble.gen_funcs.persistent_sampling_var_resources import uniform_sample as gen_f
-
-# Import libEnsemble items for this test
-from libensemble import Ensemble
 from libensemble.resources.platforms import PerlmutterGPU
 from libensemble.sim_funcs import six_hump_camel
 from libensemble.sim_funcs.var_resources import gpu_variable_resources as sim_f
 from libensemble.specs import LibeSpecs
 
-
 # from libensemble import logger
 # logger.set_level("DEBUG")  # For testing the test
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
     # Get paths for applications to run
     six_hump_camel_app = six_hump_camel.__file__
@@ -37,20 +36,21 @@
     # Ensure LIBE_PLATFORM environment variable is not set.
     if "LIBE_PLATFORM" in os.environ:
         del os.environ["LIBE_PLATFORM"]
 
     exctr = MPIExecutor()
     exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
 
-    ensemble = Ensemble(parse_args=True,
-                        executor=exctr,
-                        alloc_specs=alloc_specs,
-                        exit_criteria=exit_criteria,
-                        # libE_specs = LibeSpecs(use_workflow_dir=True, platform_specs=platform_specs),  # works
-                        )
+    ensemble = Ensemble(
+        parse_args=True,
+        executor=exctr,
+        alloc_specs=alloc_specs,
+        exit_criteria=exit_criteria,
+        # libE_specs = LibeSpecs(use_workflow_dir=True, platform_specs=platform_specs),  # works
+    )
 
     platform_specs = PerlmutterGPU()
     ensemble.libE_specs = LibeSpecs(
         num_resource_sets=ensemble.nworkers - 1,
         resource_info={"gpus_on_node": 4},
         use_workflow_dir=True,
         platform_specs=platform_specs,
@@ -79,13 +79,13 @@
     ensemble.run()
 
     if ensemble.is_manager:
         matching_dirs = glob.glob("workflow_*")
         assert matching_dirs, "No workflow dir found"
         most_recent_dir = max(matching_dirs, key=os.path.getctime)
         print(f"Checking ensemble.log in {most_recent_dir}")
-        file_path = file_path = os.path.join(most_recent_dir, 'ensemble.log')
+        file_path = file_path = os.path.join(most_recent_dir, "ensemble.log")
         if os.path.exists(file_path):  # an assert
-            with open(file_path, 'r') as file:
+            with open(file_path, "r") as file:
                 content = file.read()
                 pattern = r"Runline:\s+srun"
                 assert re.findall(pattern, content), "Incorrect MPI runner"
```

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_evaluate_existing_sample.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_evaluate_mixed_sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     H0["x"] = gen_borehole_input(samp)
     for i in range(500):
         H0["f"][i] = borehole_func(H0["x"][i])
     H0["sim_started"][:500] = True
     H0["sim_ended"][:500] = True
 
     sampling = Ensemble(parse_args=True)
+    sampling.libE_specs.gen_on_manager = True
     sampling.H0 = H0
     sampling.sim_specs = SimSpecs(sim_f=sim_f, inputs=["x"], out=[("f", float)])
     sampling.alloc_specs = AllocSpecs(alloc_f=alloc_f)
     sampling.exit_criteria = ExitCriteria(sim_max=len(H0))
     sampling.run()
 
     if sampling.is_manager:
```

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_gpCAM.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_gpCAM.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_heffte.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_heffte.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_inverse_bayes_example.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_inverse_bayes_example.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_dfols.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_exception.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_external_localopt.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_ibcdfo_pounders.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_ibcdfo_pounders.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_nlopt.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_periodic.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_pounders.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_pounders.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_scipy.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_blmvm.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_blmvm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_nm.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_tao_nm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_timeout.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_aposmm_with_grad.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_fd_param_finder.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_gp.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_gp.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_gp_multitask_ax.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_surmise_calib.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_surmise_killsims.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_tasmanian.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_tasmanian.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_persistent_tasmanian_async.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_with_app_persistent_aposmm_tao_nm.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_with_app_persistent_aposmm_tao_nm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/regression_tests/test_ytopt_heffte.py` & `libensemble-1.3.0/examples/calling_scripts/regression_tests/test_ytopt_heffte.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/run_libe_forces.py` & `libensemble-1.3.0/examples/calling_scripts/run_libe_forces.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/run_libe_forces_from_yaml.py` & `libensemble-1.3.0/examples/calling_scripts/run_libe_forces_from_yaml.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/calling_scripts/run_libensemble_on_warpx.py` & `libensemble-1.3.0/examples/calling_scripts/run_libensemble_on_warpx.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/gen_funcs/persistent_sampling.py` & `libensemble-1.3.0/examples/gen_funcs/persistent_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/gen_funcs/sampling.py` & `libensemble-1.3.0/examples/gen_funcs/sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,16 @@
     Generates ``gen_specs["user"]["gen_batch_size"]`` points uniformly over the domain
     defined by ``gen_specs["user"]["ub"]`` and ``gen_specs["user"]["lb"]``.
 
     Also randomly requests a different number of resource sets to be used in each evaluation.
 
     This generator is used to test/demonstrate setting of resource sets.
 
-    #.. seealso::
-        #`test_uniform_sampling_with_variable_resources.py <https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py>`_ # noqa
+    .. seealso::
+        `test_uniform_sampling_with_variable_resources.py <https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py>`_ # noqa
     """
 
     ub = gen_specs["user"]["ub"]
     lb = gen_specs["user"]["lb"]
     max_rsets = gen_specs["user"]["max_resource_sets"]
 
     n = len(lb)
```

### Comparing `libensemble-1.2.2/examples/gen_funcs/uniform_or_localopt.py` & `libensemble-1.3.0/examples/gen_funcs/uniform_or_localopt.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/libE_submission_scripts/bebop_submit_slurm_central.sh` & `libensemble-1.3.0/examples/libE_submission_scripts/bebop_submit_slurm_central.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/libE_submission_scripts/bebop_submit_slurm_distrib.sh` & `libensemble-1.3.0/examples/libE_submission_scripts/bebop_submit_slurm_distrib.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/libE_submission_scripts/bridges_submit_slurm_central.sh` & `libensemble-1.3.0/examples/libE_submission_scripts/bridges_submit_slurm_central.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/libE_submission_scripts/cobalt_submit_mproc.sh` & `libensemble-1.3.0/examples/libE_submission_scripts/cobalt_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/libE_submission_scripts/edtb_submit_pbspro_central.sh` & `libensemble-1.3.0/examples/libE_submission_scripts/edtb_submit_pbspro_central.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/libE_submission_scripts/summit_submit_mproc.sh` & `libensemble-1.3.0/examples/libE_submission_scripts/summit_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/sim_funcs/branin/branin.py` & `libensemble-1.3.0/examples/sim_funcs/branin/branin.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/sim_funcs/branin/branin_obj.py` & `libensemble-1.3.0/examples/sim_funcs/branin/branin_obj.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/sim_funcs/chwirut1.py` & `libensemble-1.3.0/examples/sim_funcs/chwirut1.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/sim_funcs/executor_hworld.py` & `libensemble-1.3.0/examples/sim_funcs/executor_hworld.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/sim_funcs/six_hump_camel.py` & `libensemble-1.3.0/examples/sim_funcs/six_hump_camel.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/aposmm/aposmm_tutorial_notebook.ipynb` & `libensemble-1.3.0/examples/tutorials/aposmm/aposmm_tutorial_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/aposmm/tutorial_aposmm.py` & `libensemble-1.3.0/examples/tutorials/aposmm/tutorial_aposmm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/aposmm/tutorial_six_hump_camel.py` & `libensemble-1.3.0/examples/tutorials/aposmm/tutorial_six_hump_camel.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/forces_with_executor/build_forces.sh` & `libensemble-1.3.0/examples/tutorials/forces_with_executor/build_forces.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/forces_with_executor/forces.c` & `libensemble-1.3.0/examples/tutorials/forces_with_executor/forces.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/forces_with_executor/forces_simf.py` & `libensemble-1.3.0/examples/tutorials/forces_with_executor/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/forces_with_executor/forces_tutorial_notebook.ipynb` & `libensemble-1.3.0/examples/tutorials/forces_with_executor/forces_tutorial_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/forces_with_executor/run_libe_forces.py` & `libensemble-1.3.0/examples/tutorials/forces_with_executor/run_libe_forces.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/images/basic_6hc.png` & `libensemble-1.3.0/examples/tutorials/images/basic_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/images/localopt_6hc.png` & `libensemble-1.3.0/examples/tutorials/images/localopt_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/images/sampling_6hc.png` & `libensemble-1.3.0/examples/tutorials/images/sampling_6hc.png`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/simple_sine/sine_gen.py` & `libensemble-1.3.0/examples/tutorials/simple_sine/sine_gen.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb` & `libensemble-1.3.0/examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/simple_sine/test_local_sine_tutorial.py` & `libensemble-1.3.0/examples/tutorials/simple_sine/test_local_sine_tutorial.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/simple_sine/test_local_sine_tutorial_2.py` & `libensemble-1.3.0/examples/tutorials/simple_sine/test_local_sine_tutorial_2.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/examples/tutorials/simple_sine/test_local_sine_tutorial_3.py` & `libensemble-1.3.0/examples/tutorials/simple_sine/test_local_sine_tutorial_3.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/install/find_mpi.py` & `libensemble-1.3.0/install/find_mpi.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/fast_alloc.py` & `libensemble-1.3.0/libensemble/alloc_funcs/fast_alloc.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,29 +28,30 @@
 
     support = AllocSupport(W, manage_resources, persis_info, libE_info)
 
     gen_count = support.count_gens()
     Work = {}
     gen_in = gen_specs.get("in", [])
 
-    for wid in support.avail_worker_ids():
+    # Give sim work if possible
+    for wid in support.avail_worker_ids(gen_workers=False):
         persis_info = support.skip_canceled_points(H, persis_info)
-
-        # Give sim work if possible
         if persis_info["next_to_give"] < len(H):
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], [persis_info["next_to_give"]], [])
             except InsufficientFreeResources:
                 break
             persis_info["next_to_give"] += 1
 
-        elif gen_count < user.get("num_active_gens", gen_count + 1):
-            # Give gen work
-            return_rows = range(len(H)) if gen_in else []
-            try:
-                Work[wid] = support.gen_work(wid, gen_in, return_rows, persis_info.get(wid))
-            except InsufficientFreeResources:
-                break
-            gen_count += 1
-            persis_info["total_gen_calls"] += 1
+    # Give gen work if possible
+    if persis_info["next_to_give"] >= len(H):
+        for wid in support.avail_worker_ids(gen_workers=True):
+            if wid not in Work and gen_count < user.get("num_active_gens", gen_count + 1):
+                return_rows = range(len(H)) if gen_in else []
+                try:
+                    Work[wid] = support.gen_work(wid, gen_in, return_rows, persis_info.get(wid))
+                except InsufficientFreeResources:
+                    break
+                gen_count += 1
+                persis_info["total_gen_calls"] += 1
 
     return Work, persis_info
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/fast_alloc_and_pausing.py` & `libensemble-1.3.0/libensemble/alloc_funcs/fast_alloc_and_pausing.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,18 @@
         # Something new is in the history.
         persis_info["need_to_give"].update(H["sim_id"][persis_info["H_len"] :].tolist())
         persis_info["H_len"] = len(H)
         persis_info["pt_ids"] = set(np.unique(H["pt_id"]))
         for pt_id in persis_info["pt_ids"]:
             persis_info["inds_of_pt_ids"][pt_id] = H["pt_id"] == pt_id
 
-    idle_workers = support.avail_worker_ids()
+    idle_sim_workers = support.avail_worker_ids(gen_workers=False)
+    idle_gen_workers = support.avail_worker_ids(gen_workers=True)
 
-    while len(idle_workers):
+    while len(idle_sim_workers):
         pt_ids_to_pause = set()
 
         # Find indices of H that are not yet given out to be evaluated
         if len(persis_info["need_to_give"]):
             # If "stop_on_NaN" is true and any f_i is a NaN, then pause
             # evaluations of other f_i, corresponding to the same pt_id
             if alloc_specs["user"].get("stop_on_NaNs"):
@@ -102,42 +103,46 @@
                 sim_ids_to_remove = np.in1d(H["pt_id"], list(pt_ids_to_pause))
                 H["paused"][sim_ids_to_remove] = True
 
                 persis_info["need_to_give"] = persis_info["need_to_give"].difference(np.where(sim_ids_to_remove)[0])
 
             if len(persis_info["need_to_give"]) != 0:
                 next_row = persis_info["need_to_give"].pop()
-                i = idle_workers[0]
+                i = idle_sim_workers[0]
                 try:
                     Work[i] = support.sim_work(i, H, sim_specs["in"], [next_row], [])
                 except InsufficientFreeResources:
                     persis_info["need_to_give"].add(next_row)
                     break
-                idle_workers = idle_workers[1:]
+                idle_sim_workers = idle_sim_workers[1:]
 
-        elif gen_count < alloc_specs["user"].get("num_active_gens", gen_count + 1):
+        else:
+            break
+
+    while len(idle_gen_workers):
+        if gen_count < alloc_specs["user"].get("num_active_gens", gen_count + 1):
             lw = persis_info["last_worker"]
 
             last_size = persis_info.get("last_size")
             if len(H):
                 # Don't give gen instances in batch mode if points are unfinished
                 if alloc_specs["user"].get("batch_mode") and not all(
                     np.logical_or(H["sim_ended"][last_size:], H["paused"][last_size:])
                 ):
                     break
 
             # Give gen work
-            i = idle_workers[0]
+            i = idle_gen_workers[0]
             try:
                 Work[i] = support.gen_work(i, gen_specs["in"], range(len(H)), persis_info[lw])
             except InsufficientFreeResources:
                 break
-            idle_workers = idle_workers[1:]
+            idle_gen_workers = idle_gen_workers[1:]
             gen_count += 1
             persis_info["total_gen_calls"] += 1
             persis_info["last_worker"] = i
             persis_info["last_size"] = len(H)
 
         elif gen_count >= alloc_specs["user"].get("num_active_gens", gen_count + 1):
-            idle_workers = []
+            idle_gen_workers = []
 
     return Work, persis_info
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/give_pregenerated_work.py` & `libensemble-1.3.0/libensemble/alloc_funcs/give_pregenerated_work.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     # Unless already defined, initialize next_to_give to be the first point in H
     persis_info["next_to_give"] = persis_info.get("next_to_give", 0)
 
     if persis_info["next_to_give"] >= len(H):
         return Work, persis_info, 1
 
-    for i in support.avail_worker_ids():
+    for i in support.avail_worker_ids(gen_workers=False):
         persis_info = support.skip_canceled_points(H, persis_info)
 
         # Give sim work
         try:
             Work[i] = support.sim_work(i, H, sim_specs["in"], [persis_info["next_to_give"]], [])
         except InsufficientFreeResources:
             break
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/give_sim_work_first.py` & `libensemble-1.3.0/libensemble/alloc_funcs/give_sim_work_first.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,23 +60,27 @@
 
     manage_resources = libE_info["use_resource_sets"]
     support = AllocSupport(W, manage_resources, persis_info, libE_info)
     gen_count = support.count_gens()
     Work = {}
 
     points_to_evaluate = ~H["sim_started"] & ~H["cancel_requested"]
-    for wid in support.avail_worker_ids():
-        if np.any(points_to_evaluate):
+
+    if np.any(points_to_evaluate):
+        for wid in support.avail_worker_ids(gen_workers=False):
             sim_ids_to_send = support.points_by_priority(H, points_avail=points_to_evaluate, batch=batch_give)
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], sim_ids_to_send, persis_info.get(wid))
             except InsufficientFreeResources:
                 break
             points_to_evaluate[sim_ids_to_send] = False
-        else:
+            if not np.any(points_to_evaluate):
+                break
+    else:
+        for wid in support.avail_worker_ids(gen_workers=True):
             # Allow at most num_active_gens active generator instances
             if gen_count >= user.get("num_active_gens", gen_count + 1):
                 break
 
             # Do not start gen instances in batch mode if workers still working
             if user.get("batch_mode") and not support.all_sim_ended(H):
                 break
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/inverse_bayes_allocf.py` & `libensemble-1.3.0/libensemble/alloc_funcs/inverse_bayes_allocf.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,29 +38,28 @@
                 n = gen_specs["user"]["subbatch_size"] * gen_specs["user"]["num_subbatches"]
                 k = H["batch"][-1]
                 H["weight"][(n * (k - 1)) : (n * k)] = H["weight"][(n * k) : (n * (k + 1))]
 
             Work[wid] = support.gen_work(wid, ["like"], inds_to_send_back, persis_info.get(wid), persistent=True)
 
     points_to_evaluate = ~H["sim_started"] & ~H["cancel_requested"]
-    for wid in support.avail_worker_ids(persistent=False):
-        if np.any(points_to_evaluate):
+    if np.any(points_to_evaluate):
+        for wid in support.avail_worker_ids(persistent=False, gen_workers=False):
+
             # perform sim evaluations (if any point hasn't been given).
             sim_subbatches = H["subbatch"][points_to_evaluate]
             sim_inds = sim_subbatches == np.min(sim_subbatches)
             sim_ids_to_send = np.nonzero(points_to_evaluate)[0][sim_inds]
 
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], sim_ids_to_send, [])
             except InsufficientFreeResources:
                 break
             points_to_evaluate[sim_ids_to_send] = False
-
-        elif gen_count == 0:
-            # Finally, generate points since there is nothing else to do.
-            try:
-                Work[wid] = support.gen_work(wid, gen_specs["in"], [], persis_info.get(wid), persistent=True)
-            except InsufficientFreeResources:
+            if not np.any(points_to_evaluate):
                 break
-            gen_count += 1
+
+    elif gen_count == 0:
+        wid = support.avail_worker_ids(persistent=False, gen_workers=True)[0]
+        Work[wid] = support.gen_work(wid, gen_specs["in"], [], persis_info.get(wid), persistent=True)
 
     return Work, persis_info
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/only_one_gen_alloc.py` & `libensemble-1.3.0/libensemble/alloc_funcs/only_one_gen_alloc.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,31 +17,34 @@
     manage_resources = libE_info["use_resource_sets"]
     support = AllocSupport(W, manage_resources, persis_info, libE_info)
 
     Work = {}
     gen_flag = True
     gen_in = gen_specs.get("in", [])
 
-    for wid in support.avail_worker_ids():
-        persis_info = support.skip_canceled_points(H, persis_info)
-
-        if persis_info["next_to_give"] < len(H):
+    if persis_info["next_to_give"] < len(H):
+        for wid in support.avail_worker_ids(gen_workers=False):
+            persis_info = support.skip_canceled_points(H, persis_info)
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], [persis_info["next_to_give"]], [])
             except InsufficientFreeResources:
                 break
             persis_info["next_to_give"] += 1
-
-        elif not support.test_any_gen() and gen_flag:
-            if not support.all_sim_ended(H):
+            if persis_info["next_to_give"] >= len(H):
                 break
 
-            # Give gen work
-            return_rows = range(len(H)) if gen_in else []
-            try:
-                Work[wid] = support.gen_work(wid, gen_in, return_rows, persis_info.get(wid))
-            except InsufficientFreeResources:
-                break
-            gen_flag = False
-            persis_info["total_gen_calls"] += 1
+    elif not support.test_any_gen() and gen_flag:
+        # Give gen work
+        return_rows = range(len(H)) if gen_in else []
+        wid = support.avail_worker_ids(gen_workers=True)[0]
+
+        if not support.all_sim_ended(H):
+            return Work, persis_info
+
+        try:
+            Work[wid] = support.gen_work(wid, gen_in, return_rows, persis_info.get(wid))
+        except InsufficientFreeResources:
+            return Work, persis_info
+        gen_flag = False
+        persis_info["total_gen_calls"] += 1
 
     return Work, persis_info
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/persistent_aposmm_alloc.py` & `libensemble-1.3.0/libensemble/alloc_funcs/persistent_aposmm_alloc.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,30 +49,34 @@
             if np.any(returned_but_not_given):
                 point_ids = np.where(returned_but_not_given)[0]
                 Work[wid] = support.gen_work(
                     wid, gen_specs["persis_in"], point_ids, persis_info.get(wid), persistent=True
                 )
                 returned_but_not_given[point_ids] = False
 
-    for wid in support.avail_worker_ids(persistent=False):
+    for wid in support.avail_worker_ids(persistent=False, gen_workers=False):
         persis_info = support.skip_canceled_points(H, persis_info)
 
         if persis_info["next_to_give"] < len(H):
             # perform sim evaluations (if they exist in History).
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], persis_info["next_to_give"], persis_info.get(wid))
             except InsufficientFreeResources:
                 break
             persis_info["next_to_give"] += 1
+            if persis_info["next_to_give"] >= len(H):
+                break
 
-        elif persis_info.get("gen_started") is None:
+    if persis_info.get("gen_started") is None:
+        for wid in support.avail_worker_ids(persistent=False, gen_workers=True):
             # Finally, call a persistent generator as there is nothing else to do.
             persis_info.get(wid)["nworkers"] = len(W)
             try:
                 Work[wid] = support.gen_work(
                     wid, gen_specs.get("in", []), range(len(H)), persis_info.get(wid), persistent=True
                 )
             except InsufficientFreeResources:
                 break
             persis_info["gen_started"] = True  # Must set after - in case break on resources
+            break
 
     return Work, persis_info
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/start_fd_persistent.py` & `libensemble-1.3.0/libensemble/alloc_funcs/start_fd_persistent.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,26 +45,25 @@
 
         if len(inds_to_send):
             Work[wid] = support.gen_work(
                 wid, gen_specs["persis_in"], inds_to_send, persis_info.get(wid), persistent=True
             )
 
     points_to_evaluate = ~H["sim_started"] & ~H["cancel_requested"]
-    for wid in support.avail_worker_ids(persistent=False):
-        if np.any(points_to_evaluate):
+    if np.any(points_to_evaluate):
+        for wid in support.avail_worker_ids(persistent=False, gen_workers=False):
             # perform sim evaluations (if they exist in History).
             sim_ids_to_send = np.nonzero(points_to_evaluate)[0][0]  # oldest point
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], sim_ids_to_send, persis_info.get(wid))
             except InsufficientFreeResources:
                 break
             points_to_evaluate[sim_ids_to_send] = False
-
-        elif gen_count == 0:
-            # Finally, call a persistent generator as there is nothing else to do.
-            try:
-                Work[wid] = support.gen_work(wid, gen_specs.get("in", []), [], persis_info.get(wid), persistent=True)
-            except InsufficientFreeResources:
+            if not np.any(points_to_evaluate):
                 break
-            gen_count += 1
+
+    if gen_count == 0:
+        wid = support.avail_worker_ids(persistent=False, gen_workers=True)[0]
+        Work[wid] = support.gen_work(wid, gen_specs.get("in", []), [], persis_info.get(wid), persistent=True)
+        gen_count += 1
 
     return Work, persis_info, 0
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/start_only_persistent.py` & `libensemble-1.3.0/libensemble/alloc_funcs/start_only_persistent.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     persistent=True,
                     active_recv=active_recv_gen,
                 )
                 returned_but_not_given[point_ids] = False
 
     # Now the give_sim_work_first part
     points_to_evaluate = ~H["sim_started"] & ~H["cancel_requested"]
-    avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=False)
+    avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=False, gen_workers=False)
     if user.get("alt_type"):
         avail_workers = list(
             set(support.avail_worker_ids(persistent=False, zero_resource_workers=False))
             | set(support.avail_worker_ids(persistent=EVAL_SIM_TAG, zero_resource_workers=False))
         )
     for wid in avail_workers:
         if not np.any(points_to_evaluate):
@@ -111,15 +111,15 @@
         except InsufficientFreeResources:
             break
 
         points_to_evaluate[sim_ids_to_send] = False
 
     # Start persistent gens if no worker to give out. Uses zero_resource_workers if defined.
     if not np.any(points_to_evaluate):
-        avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=True)
+        avail_workers = support.avail_worker_ids(persistent=False, zero_resource_workers=True, gen_workers=True)
 
         for wid in avail_workers:
             if gen_count < user.get("num_active_gens", 1):
                 # Finally, start a persistent generator as there is nothing else to do.
                 try:
                     Work[wid] = support.gen_work(
                         wid,
```

### Comparing `libensemble-1.2.2/libensemble/alloc_funcs/start_persistent_local_opt_gens.py` & `libensemble-1.3.0/libensemble/alloc_funcs/start_persistent_local_opt_gens.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         gen_inds = H["gen_worker"] == wid
         if support.all_sim_ended(H, gen_inds):
             last_time_pos = np.argmax(H["sim_started_time"][gen_inds])
             last_ind = np.nonzero(gen_inds)[0][last_time_pos]
             Work[wid] = support.gen_work(wid, gen_specs["persis_in"], last_ind, persis_info[wid], persistent=True)
             persis_info[wid]["run_order"].append(last_ind)
 
-    for wid in support.avail_worker_ids(persistent=False):
+    for wid in support.avail_worker_ids(persistent=False, gen_workers=True):
         # Find candidates to start local opt runs if a sample has been evaluated
         if np.any(np.logical_and(~H["local_pt"], H["sim_ended"], ~H["cancel_requested"])):
             n = len(H["x"][0])
             rk_c = extract_rk_c(gen_specs["user"], n)
             n_s = np.sum(~H["local_pt"])
             update_history_dist(H, n)
             starting_inds = decide_where_to_start_localopt(H, n, n_s, rk_c)
@@ -74,25 +74,29 @@
             except InsufficientFreeResources:
                 break
             H["started_run"][ind] = 1
             H["num_active_runs"][ind] += 1
             persis_info[wid]["run_order"] = [ind]
             gen_count += 1
 
-        elif np.any(points_to_evaluate):
+    if np.any(points_to_evaluate):
+        for wid in support.avail_worker_ids(persistent=False, gen_workers=False):
             # Perform sim evaluations from existing runs
             q_inds_logical = np.logical_and(points_to_evaluate, H["local_pt"])
             if not np.any(q_inds_logical):
                 q_inds_logical = points_to_evaluate
             sim_ids_to_send = np.nonzero(q_inds_logical)[0][0]  # oldest point
             try:
                 Work[wid] = support.sim_work(wid, H, sim_specs["in"], sim_ids_to_send, [])
             except InsufficientFreeResources:
                 break
             points_to_evaluate[sim_ids_to_send] = False
+            if not np.any(points_to_evaluate):
+                break
 
-        elif gen_count == 0 and not np.any(np.logical_and(W["active"] == EVAL_GEN_TAG, W["persis_state"] == 0)):
-            # Finally, generate points since there is nothing else to do (no resource sets req.)
-            Work[wid] = support.gen_work(wid, gen_specs.get("in", []), [], persis_info[wid], rset_team=[])
-            gen_count += 1
+    if gen_count == 0 and not np.any(np.logical_and(W["active"] == EVAL_GEN_TAG, W["persis_state"] == 0)):
+        # Finally, generate points since there is nothing else to do (no resource sets req.)
+        wid = support.avail_worker_ids(persistent=False, gen_workers=True)[0]
+        Work[wid] = support.gen_work(wid, gen_specs.get("in", []), [], persis_info[wid], rset_team=[])
+        gen_count += 1
 
     return Work, persis_info
```

### Comparing `libensemble-1.2.2/libensemble/comms/comms.py` & `libensemble-1.3.0/libensemble/comms/comms.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
     def mail_flag(self):
         """Check whether a message is ready for receipt."""
         return not self._inbox.empty()
 
 
 class QCommLocal(Comm):
-    def __init__(self, main, nworkers, *args, **kwargs):
+    def __init__(self, main, *args, **kwargs):
         self._result = None
         self._exception = None
         self._done = False
 
     def _is_result_msg(self, msg):
         """Return true if message indicates final result (and set result/except)."""
         if len(msg) and isinstance(msg[0], CommResult):
@@ -203,46 +203,49 @@
         if not self._done:
             raise Timeout()
         self.terminate(timeout=timeout)
         if self._exception is not None:
             raise RemoteException(self._exception.msg, self._exception.exc)
         return self._result
 
-    @staticmethod
-    def _qcomm_main(comm, main, *args, **kwargs):
-        """Main routine -- handles return values and exceptions."""
-        try:
-            _result = main(comm, *args, **kwargs)
-            comm.send(CommResult(_result))
-        except Exception as e:
-            comm.send(CommResultErr(str(e), format_exc()))
-            raise e
-
     @property
     def running(self):
         """Check if the thread/process is running."""
         return self.handle.is_alive()
 
     def __enter__(self):
         self.run()
         return self
 
     def __exit__(self, etype, value, traceback):
         self.handle.join()
 
 
+def _qcomm_main(comm, main, *args, **kwargs):
+    """Main routine -- handles return values and exceptions."""
+    try:
+        if not kwargs.get("user_function"):
+            _result = main(comm, *args, **kwargs)
+        else:
+            _result = main(*args)
+        comm.send(CommResult(_result))
+    except Exception as e:
+        comm.send(CommResultErr(str(e), format_exc()))
+        raise e
+
+
 class QCommThread(QCommLocal):
     """Launch a user function in a thread with an attached QComm."""
 
     def __init__(self, main, nworkers, *args, **kwargs):
         self.inbox = thread_queue.Queue()
         self.outbox = thread_queue.Queue()
-        super().__init__(self, main, nworkers, *args, **kwargs)
+        super().__init__(self, main, *args, **kwargs)
         comm = QComm(self.inbox, self.outbox, nworkers)
-        self.handle = Thread(target=QCommThread._qcomm_main, args=(comm, main) + args, kwargs=kwargs)
+        self.handle = Thread(target=_qcomm_main, args=(comm, main) + args, kwargs=kwargs)
 
     def terminate(self, timeout=None):
         """Terminate the thread.
 
         Threads can't easily be killed from the outside. It is possible to achieve such
         functionality, for example, with the `main` function periodically checking some
         variable/output to determine if the function should continue. This is not
@@ -256,17 +259,17 @@
 
 class QCommProcess(QCommLocal):
     """Launch a user function in a process with an attached QComm."""
 
     def __init__(self, main, nworkers, *args, **kwargs):
         self.inbox = Queue()
         self.outbox = Queue()
-        super().__init__(self, main, nworkers, *args, **kwargs)
+        super().__init__(self, main, *args, **kwargs)
         comm = QComm(self.inbox, self.outbox, nworkers)
-        self.handle = Process(target=QCommProcess._qcomm_main, args=(comm, main) + args, kwargs=kwargs)
+        self.handle = Process(target=_qcomm_main, args=(comm, main) + args, kwargs=kwargs)
 
     def terminate(self, timeout=None):
         """Terminate the process."""
         if self.running:
             self.handle.terminate()
         self.handle.join(timeout=timeout)
         if self.running:
```

### Comparing `libensemble-1.2.2/libensemble/comms/logs.py` & `libensemble-1.3.0/libensemble/comms/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,13 +199,14 @@
     # stat_logger = logging.getLogger(logconfig.stats_name)
 
     stat_logger.info(f"Starting ensemble at: {stat_timer.date_start}")
 
     def exit_logger():
         stat_timer.stop()
         stat_logger.info(f"Exiting ensemble at: {stat_timer.date_end} Time Taken: {stat_timer.elapsed}")
+        stat_logger.handlers[0].close()
 
         # If closing logs - each libE() call will log to a new file.
         # fh.close()
         # fhs.close()
 
     return exit_logger
```

### Comparing `libensemble-1.2.2/libensemble/comms/mpi.py` & `libensemble-1.3.0/libensemble/comms/mpi.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/comms/tcp_mgr.py` & `libensemble-1.3.0/libensemble/comms/tcp_mgr.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/ensemble.py` & `libensemble-1.3.0/libensemble/ensemble.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/executors/balsam_executor.py` & `libensemble-1.3.0/libensemble/executors/balsam_executor.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/executors/executor.py` & `libensemble-1.3.0/libensemble/executors/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,30 +225,31 @@
         """Check whether polling this task makes sense."""
         jassert(self.process is not None, f"task {self.name} has no process ID - check task has been launched")
         if self.finished:
             logger.debug(f"Polled task {self.name} has already finished. Not re-polling. Status is {self.state}")
             return False
         return True
 
-    def _set_complete(self, dry_run: bool = False) -> None:
+    def _set_complete(self) -> None:
         """Set task as complete"""
         self.finished = True
-        if dry_run:
+        if self.dry_run:
             self.success = True
             self.state = "FINISHED"
         else:
             self.calc_task_timing()
             self.errcode = self.process.returncode
             self.success = self.errcode == 0
             self.state = "FINISHED" if self.success else "FAILED"
             logger.info(f"Task {self.name} finished with errcode {self.errcode} ({self.state})")
 
     def poll(self) -> None:
         """Polls and updates the status attributes of the task"""
         if self.dry_run:
+            self._set_complete()
             return
 
         if not self._check_poll():
             return
 
         # Poll the task
         poll = self.process.poll()
@@ -270,14 +271,15 @@
         timeout: int or float,  Optional
             Time in seconds after which a TimeoutExpired exception is raised.
             If not set, then simply waits until completion.
             Note that the task is not automatically killed on timeout.
         """
 
         if self.dry_run:
+            self._set_complete()
             return
 
         if not self._check_poll():
             return
 
         # Wait on the task
         rc = launcher.wait(self.process, timeout)
@@ -627,15 +629,15 @@
             if task.state == "FINISHED":
                 calc_status = WORKER_DONE
             elif task.state == "FAILED_TO_START":
                 calc_status = TASK_FAILED_TO_START
             elif task.state == "FAILED":
                 calc_status = TASK_FAILED
             else:
-                logger.warning(f"Warning: Task {self.name} in unknown state {self.state}. Error code {self.errcode}")
+                logger.warning(f"Warning: Task {task.name} in unknown state {task.state}. Error code {task.errcode}")
 
         return calc_status
 
     def get_task(self, taskid: Union[str, int]) -> Optional[Task]:
         """Returns the task object for the supplied task ID"""
         task = next((j for j in self.list_of_tasks if j.id == taskid), None)
         if task is None:
@@ -663,15 +665,15 @@
                 self.last_task += 1
         return timing_msg
 
     def set_workerID(self, workerid) -> None:
         """Sets the worker ID for this executor"""
         self.workerID = workerid
 
-    def set_worker_info(self, comm, workerid=None) -> None:
+    def set_worker_info(self, comm=None, workerid=None) -> None:
         """Sets info for this executor"""
         self.workerID = workerid
         self.comm = comm
 
     def _check_app_exists(self, full_path: str) -> None:
         """Allows submit function to check if app exists and error if not"""
         if not os.path.isfile(full_path):
@@ -737,15 +739,15 @@
             app = self.get_app(app_name)
         elif calc_type is not None:
             app = self.default_app(calc_type)
         else:
             raise ExecutorException("Either app_name or calc_type must be set")
 
         default_workdir = os.getcwd()
-        task = Task(app, app_args, default_workdir, stdout, stderr, self.workerID)
+        task = Task(app, app_args, default_workdir, stdout, stderr, self.workerID, dry_run)
 
         if not dry_run:
             self._check_app_exists(task.app.full_path)
 
         runline = task.app.app_cmd.split()
         if task.app_args is not None:
             runline.extend(task.app_args.split())
@@ -784,15 +786,14 @@
     def poll(self, task: Task) -> None:
         """Polls the supplied task"""
         task.poll()
 
     def kill(self, task: Task) -> None:
         """Kills the supplied task"""
         jassert(isinstance(task, Task), "Invalid task has been provided")
-        task.poll()
         task.kill(self.wait_time)
 
     @staticmethod
     def _process_env_script(task, runline, env_script):
         """Merge users environment script with generated run-line"""
         sout_f = task.name + "_run.sh"
         p = Path(".")
```

### Comparing `libensemble-1.2.2/libensemble/executors/mpi_executor.py` & `libensemble-1.3.0/libensemble/executors/mpi_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 In order to create an MPI executor, the calling script should contain:
 
 .. code-block:: python
 
     exctr = MPIExecutor()
 
-The MPIExecutor will use system resource information supplied by the libEsnemble
+The MPIExecutor will use system resource information supplied by the libEnsemble
 resource manager when submitting tasks.
 
 """
 
 import logging
 import os
 import time
@@ -262,15 +262,15 @@
         wait_on_start: bool or int, Optional
             Whether to wait for task to be polled as RUNNING (or other
             active/end state) before continuing. If an integer N is supplied,
             wait at most N seconds.
 
         extra_args: str, Optional
             Additional command line arguments to supply to MPI runner. If
-            arguments are recognised as MPI resource configuration
+            arguments are recognized as MPI resource configuration
             (num_procs, num_nodes, procs_per_node) they will be used in
             resources determination unless also supplied in the direct
             options.
 
         auto_assign_gpus: bool, Optional
             Auto-assign GPUs available to this worker using either the method
             supplied in configuration or determined by detected environment.
@@ -310,15 +310,15 @@
             app = self.get_app(app_name)
         elif calc_type is not None:
             app = self.default_app(calc_type)
         else:
             raise ExecutorException("Either app_name or calc_type must be set")
 
         default_workdir = os.getcwd()
-        task = Task(app, app_args, default_workdir, stdout, stderr, self.workerID)
+        task = Task(app, app_args, default_workdir, stdout, stderr, self.workerID, dry_run)
 
         if not dry_run:
             self._check_app_exists(task.app.full_path)
 
         if stage_inout is not None:
             logger.warning("stage_inout option ignored in this " "executor - runs in-place")
 
@@ -367,17 +367,16 @@
 
         if env_script is not None:
             run_cmd = Executor._process_env_script(task, runline, env_script)
         else:
             run_cmd = runline
 
         if dry_run:
-            task.dry_run = True
             logger.info(f"Test (No submit) Runline: {' '.join(run_cmd)}")
-            task._set_complete(dry_run=True)
+            task._set_complete()
         else:
             # Set environment variables and launch task
             task._implement_env()
 
             # Launch Task
             self._launch_with_retries(task, sglaunch, wait_on_start, run_cmd)
```

### Comparing `libensemble-1.2.2/libensemble/executors/mpi_runner.py` & `libensemble-1.3.0/libensemble/executors/mpi_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self.arg_nprocs = ("--LIBE_NPROCS_ARG_EMPTY",)
         self.arg_nnodes = ("--LIBE_NNODES_ARG_EMPTY",)
         self.arg_ppn = ("--LIBE_PPN_ARG_EMPTY",)
         self.default_mpi_options = None
         self.default_gpu_args = None
         self.default_gpu_arg_type = None
         self.platform_info = platform_info
+        self.rm_rpn = False
 
     def _get_parser(self, p_args, nprocs, nnodes, ppn):
         """Parses MPI arguments from the provided string"""
         parser = argparse.ArgumentParser(description="Parse extra_args", allow_abbrev=False)
         parser.add_argument(*nprocs, type=int, dest="num_procs", default=None)
         parser.add_argument(*nnodes, type=int, dest="num_nodes", default=None)
         parser.add_argument(*ppn, type=int, dest="procs_per_node", default=None)
@@ -116,17 +117,16 @@
         else:
             extra_args = " ".join((extra_args, gpus_opt))
         return extra_args
 
     def _set_gpu_env_var(self, wresources, task, gpus_per_node, gpus_env):
         """Add GPU environment variable setting to the tasks environment"""
         jassert(wresources.matching_slots, f"Cannot assign CPUs/GPUs to non-matching slots per node {wresources.slots}")
-        if wresources.doihave_gpus():
-            slot_list = wresources.get_slots_as_string(multiplier=wresources.gpus_per_rset, limit=gpus_per_node)
-            task._add_to_env(gpus_env, slot_list)
+        slot_list = wresources.get_slots_as_string(multiplier=wresources.gpus_per_rset, limit=gpus_per_node)
+        task._add_to_env(gpus_env, slot_list)
 
     def _local_runner_set_gpus(self, task, wresources, extra_args, gpus_per_node, ppn):
         """Set default GPU setting for MPI runner"""
 
         arg_type = self.default_gpu_arg_type
         if arg_type is not None:
             gpu_value = gpus_per_node // ppn if arg_type == "option_gpus_per_task" else gpus_per_node
@@ -203,52 +203,50 @@
             return nprocs, nnodes, ppn, extra_args
 
         gpu_setting_type = "runner_default"
 
         if ppn is None:
             ppn = nprocs // nnodes
 
-        if self.platform_info is not None:
+        if self.platform_info:
             gpu_setting_type = self.platform_info.get("gpu_setting_type", gpu_setting_type)
 
         if gpu_setting_type == "runner_default":
             extra_args = self._local_runner_set_gpus(task, wresources, extra_args, gpus_per_node, ppn)
 
         elif gpu_setting_type in ["option_gpus_per_node", "option_gpus_per_task"]:
             gpu_value = gpus_per_node // ppn if gpu_setting_type == "option_gpus_per_task" else gpus_per_node
             gpu_setting_name = self.platform_info.get("gpu_setting_name", self._get_default_arg(gpu_setting_type))
             extra_args = self._set_gpu_cli_option(wresources, extra_args, gpu_setting_name, gpu_value)
 
-        elif gpu_setting_type == "env":
+        else:  # gpu_setting_type == "env":
             gpus_env = self.platform_info.get("gpu_setting_name", "CUDA_VISIBLE_DEVICES")
             self._set_gpu_env_var(wresources, task, gpus_per_node, gpus_env)
 
         return nprocs, nnodes, ppn, extra_args
 
     def _adjust_procs(self, nprocs, ppn, nnodes, ngpus, resources):
         """Adjust an invalid config"""
+
+        def adjust_resource(n_units, units_attr, units_name):
+            if n_units is not None and nnodes:
+                mod_n_units = n_units % nnodes
+                if mod_n_units != 0:
+                    try_n_units = n_units + (nnodes - mod_n_units)
+                    if try_n_units <= wresources.slot_count * getattr(wresources, units_attr) * nnodes:
+                        logger.info(
+                            f"Adjusted {units_name} to split evenly across nodes. From {n_units} to {try_n_units}"
+                        )
+                        return try_n_units
+            return n_units
+
         if resources is not None:
             wresources = resources.worker_resources
-            if ngpus is not None:
-                # When gen gives num_procs or num_gpus will have num_nodes
-                if nnodes:
-                    mod_gpus = ngpus % nnodes
-                    if mod_gpus != 0:
-                        try_gpus = ngpus + mod_gpus
-                        if try_gpus <= wresources.slot_count * wresources.gpus_per_rset * nnodes:
-                            oldng = ngpus
-                            ngpus = try_gpus
-                            logger.info(f"Adjusted ngpus to split evenly across nodes. From {oldng} to {ngpus}")
-            if nprocs is not None:
-                if nnodes:
-                    mod_cpus = nprocs % nnodes
-                    if mod_cpus != 0:
-                        oldnp = nprocs
-                        nprocs = nprocs + mod_cpus
-                        logger.info(f"Adjusted nprocs to split evenly across nodes. From {oldnp} to {nprocs}")
+            ngpus = adjust_resource(ngpus, "gpus_per_rset", "ngpus")
+            nprocs = adjust_resource(nprocs, "procs_per_rset", "nprocs")
         return nprocs, ngpus
 
     def get_mpi_specs(
         self,
         task,
         nprocs,
         nnodes,
@@ -292,14 +290,16 @@
             # if no_config_set, make match_procs_to_gpus default.
             if no_config_set:
                 match_procs_to_gpus = True
             nprocs, nnodes, ppn, extra_args = self._assign_gpus(
                 task, resources, nprocs, nnodes, ppn, ngpus, extra_args, match_procs_to_gpus
             )
 
+        rm_rpn = True if self.rm_rpn and ppn is None and nnodes is None else False
+
         hostlist = None
         if machinefile and not self.mfile_support:
             logger.warning(f"User machinefile ignored - not supported by {self.run_command}")
             machinefile = None
 
         if machinefile is None and resources is not None:
             nprocs, nnodes, ppn = mpi_resources.get_resources(resources, nprocs, nnodes, ppn, hyperthreads)
@@ -309,14 +309,17 @@
         else:
             nprocs, nnodes, ppn = mpi_resources.task_partition(nprocs, nnodes, ppn, machinefile)
 
         # Remove portable variable if in extra_args
         if extra_args:
             nprocs, nnodes, ppn = self._rm_replicated_args(nprocs, nnodes, ppn, p_args)
 
+        if rm_rpn:
+            ppn = None
+
         if self.default_mpi_options is not None:
             extra_args = self._append_to_extra_args(extra_args, self.default_mpi_options)
 
         return {
             "num_procs": nprocs,
             "num_nodes": nnodes,
             "procs_per_node": ppn,
@@ -334,14 +337,15 @@
         self.arg_nprocs = ("-n", "-np")
         self.arg_nnodes = ("--LIBE_NNODES_ARG_EMPTY",)
         self.arg_ppn = ("--ppn", "-ppn")
         self.default_mpi_options = None
         self.default_gpu_args = None
         self.default_gpu_arg_type = None
         self.platform_info = platform_info
+        self.rm_rpn = False
 
         self.mpi_command = [
             self.run_command,
             "--env {env}",
             "-machinefile {machinefile}",
             "-hosts {hostlist}",
             "-np {num_procs}",
@@ -358,14 +362,15 @@
         self.arg_nprocs = ("-n", "-np", "-c", "--n")
         self.arg_nnodes = ("--LIBE_NNODES_ARG_EMPTY",)
         self.arg_ppn = ("-npernode",)
         self.default_mpi_options = None
         self.default_gpu_args = None
         self.default_gpu_arg_type = None
         self.platform_info = platform_info
+        self.rm_rpn = False
         self.mpi_command = [
             self.run_command,
             "-x {env}",
             "-machinefile {machinefile}",
             "-host {hostlist}",
             "-np {num_procs}",
             "-npernode {procs_per_node}",
@@ -380,16 +385,15 @@
         """
         hostlist = None
         machinefile = None
         # Use machine files for Open-MPI
         # as "-host" requires entry for every rank
 
         machinefile = "machinefile_autogen"
-        if workerID is not None:
-            machinefile += f"_for_worker_{workerID}"
+        machinefile += f"_for_worker_{workerID}"
         machinefile += f"_task_{task.id}"
         mfile_created, nprocs, nnodes, ppn = mpi_resources.create_machinefile(
             resources, machinefile, nprocs, nnodes, ppn, hyperthreads
         )
         jassert(mfile_created, "Auto-creation of machinefile failed")
 
         return hostlist, machinefile
@@ -403,14 +407,15 @@
         self.arg_nprocs = ("-n",)
         self.arg_nnodes = ("--LIBE_NNODES_ARG_EMPTY",)
         self.arg_ppn = ("-N",)
         self.default_mpi_options = None
         self.default_gpu_args = None
         self.default_gpu_arg_type = None
         self.platform_info = platform_info
+        self.rm_rpn = False
         self.mpi_command = [
             self.run_command,
             "-e {env}",
             "-L {hostlist}",
             "-n {num_procs}",
             "-N {procs_per_node}",
             "{extra_args}",
@@ -425,14 +430,15 @@
         self.arg_nprocs = ("-n", "-np")
         self.arg_nnodes = ("--LIBE_NNODES_ARG_EMPTY",)
         self.arg_ppn = ("-cores",)
         self.default_mpi_options = None
         self.default_gpu_args = None
         self.default_gpu_arg_type = None
         self.platform_info = platform_info
+        self.rm_rpn = False
         self.mpi_command = [
             self.run_command,
             "-env {env}",
             "-n {num_procs}",
             "-cores {procs_per_node}",
             "{extra_args}",
         ]
@@ -445,16 +451,16 @@
         self.mfile_support = False
         self.arg_nprocs = ("-n", "--ntasks")
         self.arg_nnodes = ("-N", "--nodes")
         self.arg_ppn = ("--ntasks-per-node",)
         self.default_mpi_options = "--exact"
         self.default_gpu_arg_type = "option_gpus_per_task"
         self.default_gpu_args = {"option_gpus_per_task": "--gpus-per-task", "option_gpus_per_node": "--gpus-per-node"}
-
         self.platform_info = platform_info
+        self.rm_rpn = False
         self.mpi_command = [
             self.run_command,
             "-w {hostlist}",
             "--ntasks {num_procs}",
             "--nodes {num_nodes}",
             "--ntasks-per-node {procs_per_node}",
             "{extra_args}",
@@ -471,86 +477,12 @@
         self.arg_ppn = ("-r",)
         self.default_mpi_options = None
         self.default_gpu_arg_type = "option_gpus_per_task"
         self.default_gpu_args = {"option_gpus_per_task": "-g", "option_gpus_per_node": None}
 
         self.platform_info = platform_info
         self.mpi_command = [self.run_command, "-n {num_procs}", "-r {procs_per_node}", "{extra_args}"]
+        self.rm_rpn = True
 
-    def get_mpi_specs(
-        self,
-        task,
-        nprocs,
-        nnodes,
-        ppn,
-        ngpus,
-        machinefile,
-        hyperthreads,
-        extra_args,
-        auto_assign_gpus,
-        match_procs_to_gpus,
-        resources,
-        workerID,
-    ):
-        """Returns a dictionary with the MPI specifications for the runline.
-
-        This function takes user provided inputs and resource information and
-        uses these to determine the final MPI specifications. This may include
-        a host-list or machine file.
-
-        extra_args will be parsed if possible to extract MPI configuration.
-        Default arguments may be added, and GPU settings added to extra_args,
-        or to the task environment.
-        """
-
-        p_args = None
-
-        # Return auto_resource variables inc. extra_args additions
-        if extra_args:
-            nprocs, nnodes, ppn, p_args = self._parse_extra_args(
-                nprocs, nnodes, ppn, hyperthreads, extra_args=extra_args
-            )
-
-        # If no_config_set and auto_assign_gpus - make match_procs_to_gpus default.
-        no_config_set = not (nprocs or ppn)
-
-        if match_procs_to_gpus:
-            jassert(no_config_set, "match_procs_to_gpus is mutually exclusive with either of nprocs/ppn")
-        nprocs, ngpus = self._adjust_procs(nprocs, ppn, nnodes, ngpus, resources)
-
-        if auto_assign_gpus or ngpus is not None:
-            # if no_config_set, make match_procs_to_gpus default.
-            if no_config_set:
-                match_procs_to_gpus = True
-            nprocs, nnodes, ppn, extra_args = self._assign_gpus(
-                task, resources, nprocs, nnodes, ppn, ngpus, extra_args, match_procs_to_gpus
-            )
-
-        rm_rpn = True if ppn is None and nnodes is None else False
-
-        hostlist = None
-        if machinefile and not self.mfile_support:
-            logger.warning(f"User machinefile ignored - not supported by {self.run_command}")
-            machinefile = None
-        if machinefile is None and resources is not None:
-            nprocs, nnodes, ppn = mpi_resources.get_resources(resources, nprocs, nnodes, ppn, hyperthreads)
-        else:
-            nprocs, nnodes, ppn = mpi_resources.task_partition(nprocs, nnodes, ppn, machinefile)
-
-        # Remove portable variable if in extra_args
-        if extra_args:
-            nprocs, nnodes, ppn = self._rm_replicated_args(nprocs, nnodes, ppn, p_args)
-
-        if rm_rpn:
-            ppn = None
-
-        if self.default_mpi_options is not None:
-            extra_args = self._append_to_extra_args(extra_args, self.default_mpi_options)
-
-        return {
-            "num_procs": nprocs,
-            "num_nodes": nnodes,
-            "procs_per_node": ppn,
-            "extra_args": extra_args,
-            "machinefile": machinefile,
-            "hostlist": hostlist,
-        }
+    def express_spec(self, task, nprocs, nnodes, ppn, machinefile, hyperthreads, extra_args, resources, workerID):
+        """Returns None, None as jsrun uses neither hostlist or machinefile"""
+        return None, None
```

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/__init__.py` & `libensemble-1.3.0/libensemble/gen_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/aposmm_localopt_support.py` & `libensemble-1.3.0/libensemble/gen_funcs/aposmm_localopt_support.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_aposmm.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_aposmm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_ax_multitask.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_ax_multitask.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,26 @@
 from ax.core.generator_run import GeneratorRun
 from ax.core.multi_type_experiment import MultiTypeExperiment
 from ax.core.objective import Objective
 from ax.core.observation import ObservationFeatures
 from ax.core.optimization_config import OptimizationConfig
 from ax.core.parameter import ParameterType, RangeParameter
 from ax.core.search_space import SearchSpace
-from ax.modelbridge.factory import get_MTGP, get_sobol
+from ax.modelbridge.factory import get_sobol
 from ax.runners import SyntheticRunner
 from ax.storage.json_store.save import save_experiment
 from ax.storage.metric_registry import register_metric
 from ax.storage.runner_registry import register_runner
+from ax.utils.common.result import Ok
+
+try:
+    from ax.modelbridge.factory import get_MTGP
+except ImportError:
+    # For Ax >= 0.3.4
+    from ax.modelbridge.factory import get_MTGP_LEGACY as get_MTGP
 
 from libensemble.message_numbers import EVAL_GEN_TAG, FINISHED_PERSISTENT_GEN_TAG, PERSIS_STOP, STOP_TAG
 from libensemble.tools.persistent_support import PersistentSupport
 
 
 def persistent_gp_mt_ax_gen_f(H, persis_info, gen_specs, libE_info):
     """
@@ -241,15 +248,16 @@
                     "arm_name": arm_name,
                     "metric_name": self.name,
                     "trial_index": trial.index,
                     "mean": trial.run_metadata[arm_name]["f"],
                     "sem": 0.0,
                 }
             )
-        return Data(df=pd.DataFrame.from_records(records))
+        data = Data(df=pd.DataFrame.from_records(records))
+        return Ok(data)
 
 
 def max_utility_from_GP(n, m, gr, hifi_task):
     """
     High fidelity batches are constructed by selecting the maximum utility points
     from the low fidelity batch, after updating the model with the low fidelity results.
     This function selects the max utility points according to the MTGP
```

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_fd_param_finder.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_fd_param_finder.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_gp.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_gp.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_gpCAM.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_gpCAM.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_inverse_bayes.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_inverse_bayes.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_sampling.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_sampling_var_resources.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_sampling_var_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from libensemble.executors.executor import Executor
 from libensemble.message_numbers import EVAL_GEN_TAG, FINISHED_PERSISTENT_GEN_TAG, PERSIS_STOP, STOP_TAG
 from libensemble.tools.persistent_support import PersistentSupport
 from libensemble.tools.test_support import check_gpu_setting
 
 __all__ = [
     "uniform_sample",
+    "uniform_sample_with_var_gpus",
     "uniform_sample_with_procs_gpus",
     "uniform_sample_with_var_priorities",
     "uniform_sample_diff_simulations",
     "uniform_sample_with_sim_gen_resources",
 ]
```

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_surmise_calib.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_surmise_calib.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/persistent_tasmanian.py` & `libensemble-1.3.0/libensemble/gen_funcs/persistent_tasmanian.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 y_ptr += 1
         return out_ord
 
 
 def get_state(queued_pts, queued_ids, id_offset, new_points=np.array([]), completed_points=np.array([]), tol=1e-12):
     """
     Creates the data to be sent and updates the state arrays and scalars if new information
-    (new_points or compeleted_points) arrives. Ensures that the output state arrays remain sorted if
+    (new_points or completed_points) arrives. Ensures that the output state arrays remain sorted if
     the input state arrays are already sorted.
     """
     if new_points.size > 0:
         new_points_ord = np.lexsort(np.rot90(new_points))
         new_points_ids = id_offset + np.arange(new_points.shape[0])
         id_offset += new_points.shape[0]
         insert_idx = get_2D_insert_indices(queued_pts, new_points, y_ord=new_points_ord, tol=tol)
```

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/sampling.py` & `libensemble-1.3.0/libensemble/gen_funcs/sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,16 @@
     Generates ``gen_specs["user"]["gen_batch_size"]`` points uniformly over the domain
     defined by ``gen_specs["user"]["ub"]`` and ``gen_specs["user"]["lb"]``.
 
     Also randomly requests a different number of resource sets to be used in each evaluation.
 
     This generator is used to test/demonstrate setting of resource sets.
 
-    #.. seealso::
-        #`test_uniform_sampling_with_variable_resources.py <https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py>`_ # noqa
+    .. seealso::
+        `test_uniform_sampling_with_variable_resources.py <https://github.com/Libensemble/libensemble/blob/develop/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py>`_ # noqa
     """
 
     ub = gen_specs["user"]["ub"]
     lb = gen_specs["user"]["lb"]
     max_rsets = gen_specs["user"]["max_resource_sets"]
 
     n = len(lb)
```

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/surmise_calib_support.py` & `libensemble-1.3.0/libensemble/gen_funcs/surmise_calib_support.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/uniform_or_localopt.py` & `libensemble-1.3.0/libensemble/gen_funcs/uniform_or_localopt.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/gen_funcs/ytopt_asktell.py` & `libensemble-1.3.0/libensemble/gen_funcs/ytopt_asktell.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/history.py` & `libensemble-1.3.0/libensemble/history.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/libE.py` & `libensemble-1.3.0/libensemble/libE.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 """
 The libE module is the outer libEnsemble routine.
 
 This module sets up the manager and the team of workers, configured according
 to the contents of :ref:`libE_specs<datastruct-libe-specs>`. The manager/worker
-communications scheme used in libEnsemble is parsed from the ``comms`` key
-if present, with valid values being ``mpi``, ``local`` (for multiprocessing), or
-``tcp``. MPI is the default; if a communicator is specified, each call to this
-module will initiate manager/worker communications on a duplicate of that
+communications scheme used in libEnsemble is parsed from the ``comms`` key if
+present, with valid values being ``mpi``, ``local`` (for multiprocessing), or
+``tcp``.
+
+MPI is the default if ``nworkers`` is not given. However, if ``libE_specs["nworkers"]``
+is specified, then ``local`` comms will be used unless a parallel MPI environment
+is detected.
+
+For ``mpi`` comms, if a communicator is specified, each call to this module
+will initiate manager/worker communications on a duplicate of that
 communicator. Otherwise, a duplicate of ``COMM_WORLD`` will be used.
 
 In the vast majority of cases, programming with libEnsemble involves the creation
 of a *calling script*, a Python file where libEnsemble is parameterized via
 the various specification dictionaries (e.g. :ref:`libE_specs<datastruct-libe-specs>`,
-:ref:`sim_specs<datastruct-sim-specs>`, and :ref:`gen_specs<datastruct-gen-specs>`). The
-outer libEnsemble routine :meth:`libE()<libensemble.libE.libE>` is imported and called with such
-dictionaries to initiate libEnsemble. A simple calling script
+:ref:`sim_specs<datastruct-sim-specs>`, and :ref:`gen_specs<datastruct-gen-specs>`).
+The outer libEnsemble routine :meth:`libE()<libensemble.libE.libE>` is imported and
+called with such dictionaries to initiate libEnsemble. A simple calling script
 (from :doc:`the first tutorial<tutorials/local_sine_tutorial>`) may resemble:
 
 .. code-block:: python
     :linenos:
 
     import numpy as np
     from libensemble.libE import libE
@@ -382,14 +388,17 @@
     from libensemble.comms.mpi import MainMPIComm
 
     if not libE_specs["disable_log_files"]:
         exit_logger = manager_logging_config(specs=libE_specs)
     else:
         exit_logger = None
 
+    if libE_specs.get("nworkers"):
+        logger.manager_warning("*WARNING* 'mpi' comms is detected with 'nworkers'. nworkers will be ignored.\n")
+
     if isinstance(Executor.executor, MPIExecutor):
         if Executor.executor.mpi_runner_type == "openmpi":
             logger.manager_warning(
                 "WARNING: Nested MPI-workflow detected. User initialized both an MPI runtime and an MPI Executor.\n"
                 + "       Expect complications if using Open MPI."
                 + " An MPICH-derived MPI distribution is recommended for nested MPI workflows. \n"
             )
```

### Comparing `libensemble-1.2.2/libensemble/logger.py` & `libensemble-1.3.0/libensemble/logger.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/manager.py` & `libensemble-1.3.0/libensemble/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,33 +14,34 @@
 import traceback
 from typing import Any, Union
 
 import numpy as np
 import numpy.typing as npt
 from numpy.lib.recfunctions import repack_fields
 
-from libensemble.comms.comms import CommFinishedException
+from libensemble.comms.comms import CommFinishedException, QCommThread
+from libensemble.executors.executor import Executor
 from libensemble.message_numbers import (
     EVAL_GEN_TAG,
     EVAL_SIM_TAG,
     FINISHED_PERSISTENT_GEN_TAG,
     FINISHED_PERSISTENT_SIM_TAG,
     MAN_SIGNAL_FINISH,
     MAN_SIGNAL_KILL,
     PERSIS_STOP,
     STOP_TAG,
     calc_type_strings,
 )
 from libensemble.resources.resources import Resources
 from libensemble.tools.fields_keys import protected_libE_fields
 from libensemble.tools.tools import _PERSIS_RETURN_WARNING, _USER_CALC_DIR_WARNING
-from libensemble.utils.misc import extract_H_ranges
+from libensemble.utils.misc import _WorkerIndexer, extract_H_ranges
 from libensemble.utils.output_directory import EnsembleDirectory
 from libensemble.utils.timer import Timer
-from libensemble.worker import WorkerErrMsg
+from libensemble.worker import WorkerErrMsg, worker_main
 
 logger = logging.getLogger(__name__)
 # For debug messages - uncomment
 # logger.setLevel(logging.DEBUG)
 
 
 class ManagerException(Exception):
@@ -154,21 +155,44 @@
 
 
 class Manager:
     """Manager class for libensemble."""
 
     worker_dtype = [
         ("worker_id", int),
+        ("gen_worker", bool),
         ("active", int),
         ("persis_state", int),
-        ("active_recv", int),
+        ("active_recv", bool),
         ("gen_started_time", float),
         ("zero_resource_worker", bool),
     ]
 
+    def _run_additional_worker(self, hist, sim_specs, gen_specs, libE_specs):
+        dtypes = {
+            EVAL_SIM_TAG: repack_fields(hist.H[sim_specs["in"]]).dtype,
+            EVAL_GEN_TAG: repack_fields(hist.H[gen_specs["in"]]).dtype,
+        }
+        local_worker_comm = QCommThread(
+            worker_main,
+            len(self.wcomms),
+            sim_specs,
+            gen_specs,
+            libE_specs,
+            0,
+            False,
+            Resources.resources,
+            Executor.executor,
+        )
+        local_worker_comm.run()
+        local_worker_comm.send(0, dtypes)
+        if libE_specs.get("use_workflow_dir"):
+            local_worker_comm.send(0, libE_specs.get("workflow_dir_path"))
+        return local_worker_comm
+
     def __init__(
         self,
         hist,
         libE_specs: dict,
         alloc_specs: dict,
         sim_specs: dict,
         gen_specs: dict,
@@ -195,33 +219,49 @@
 
         dyn_keys = ("resource_sets", "num_procs", "num_gpus")
         dyn_keys_in_H = any(k in self.hist.H.dtype.names for k in dyn_keys)
         self.use_resource_sets = dyn_keys_in_H or self.libE_specs.get("num_resource_sets")
         self.gen_num_procs = libE_specs.get("gen_num_procs", 0)
         self.gen_num_gpus = libE_specs.get("gen_num_gpus", 0)
 
-        self.W = np.zeros(len(self.wcomms), dtype=Manager.worker_dtype)
-        self.W["worker_id"] = np.arange(len(self.wcomms)) + 1
         self.term_tests = [
             (2, "wallclock_max", self.term_test_wallclock),
             (1, "sim_max", self.term_test_sim_max),
             (1, "gen_max", self.term_test_gen_max),
             (1, "stop_val", self.term_test_stop_val),
         ]
 
+        gen_on_manager = self.libE_specs.get("gen_on_manager", False)
+
+        self.W = np.zeros(len(self.wcomms) + gen_on_manager, dtype=Manager.worker_dtype)
+        if gen_on_manager:
+            self.W["worker_id"] = np.arange(len(self.wcomms) + 1)  # [0, 1, 2, ...]
+            self.W[0]["gen_worker"] = True
+            local_worker_comm = self._run_additional_worker(hist, sim_specs, gen_specs, libE_specs)
+            self.wcomms = [local_worker_comm] + self.wcomms
+        else:
+            self.W["worker_id"] = np.arange(len(self.wcomms)) + 1  # [1, 2, 3, ...]
+
+        self.W = _WorkerIndexer(self.W, gen_on_manager)
+        self.wcomms = _WorkerIndexer(self.wcomms, gen_on_manager)
+
         temp_EnsembleDirectory = EnsembleDirectory(libE_specs=libE_specs)
         self.resources = Resources.resources
         self.scheduler_opts = self.libE_specs.get("scheduler_opts", {})
         if self.resources is not None:
             gresource = self.resources.glob_resources
             self.scheduler_opts = gresource.update_scheduler_opts(self.scheduler_opts)
             for wrk in self.W:
                 if wrk["worker_id"] in gresource.zero_resource_workers:
                     wrk["zero_resource_worker"] = True
 
+        for wrk in self.W:
+            if wrk["worker_id"] in self.libE_specs.get("gen_workers", []):
+                wrk["gen_worker"] = True
+
         try:
             temp_EnsembleDirectory.make_copyback()
         except AssertionError as e:  # Ensemble dir exists and isn't empty.
             logger.manager_warning(_USER_CALC_DIR_WARNING.format(temp_EnsembleDirectory.ensemble_dir))
             self._kill_workers()
             raise ManagerException(
                 "Manager errored on initialization",
@@ -261,15 +301,17 @@
         return 0
 
     # --- Low-level communication routines
 
     def _kill_workers(self) -> None:
         """Kills the workers"""
         for w in self.W["worker_id"]:
-            self.wcomms[w - 1].send(STOP_TAG, MAN_SIGNAL_FINISH)
+            self.wcomms[w].send(STOP_TAG, MAN_SIGNAL_FINISH)
+            if w == 0:
+                self.wcomms[0].result()
 
     # --- Checkpointing logic
 
     def _get_date_start_str(self) -> str:
         """Get timestamp for workflow start, for saving History"""
         date_start = self.date_start + "_"
         if platform.system() == "Windows":
@@ -315,23 +357,23 @@
         if self.libE_specs.get("save_every_k_gens"):
             self._save_every_k_gens(complete)
 
     # --- Handle outgoing messages to workers (work orders from alloc)
 
     def _check_work_order(self, Work: dict, w: int, force: bool = False) -> None:
         """Checks validity of an allocation function order"""
-        assert w != 0, "Can't send to worker 0; this is the manager."
-        if self.W[w - 1]["active_recv"]:
+        # assert w != 0, "Can't send to worker 0; this is the manager."
+        if self.W[w]["active_recv"]:
             assert "active_recv" in Work["libE_info"], (
                 "Messages to a worker in active_recv mode should have active_recv"
                 f"set to True in libE_info. Work['libE_info'] is {Work['libE_info']}"
             )
         else:
             if not force:
-                assert self.W[w - 1]["active"] == 0, (
+                assert not self.W[w]["active"], (
                     "Allocation function requested work be sent to worker %d, an already active worker." % w
                 )
         work_rows = Work["libE_info"]["H_rows"]
         if len(work_rows):
             work_fields = set(Work["H_fields"])
 
             assert len(work_fields), (
@@ -368,39 +410,40 @@
     def _send_work_order(self, Work: dict, w: int) -> None:
         """Sends an allocation function order to a worker"""
         logger.debug(f"Manager sending work unit to worker {w}")
 
         if self.resources:
             self._set_resources(Work, w)
 
-        self.wcomms[w - 1].send(Work["tag"], Work)
+        self.wcomms[w].send(Work["tag"], Work)
 
         if Work["tag"] == EVAL_GEN_TAG:
-            self.W[w - 1]["gen_started_time"] = time.time()
+            self.W[w]["gen_started_time"] = time.time()
 
         work_rows = Work["libE_info"]["H_rows"]
         work_name = calc_type_strings[Work["tag"]]
         logger.debug(f"Manager sending {work_name} work to worker {w}. Rows {extract_H_ranges(Work) or None}")
         if len(work_rows):
             new_dtype = [(name, self.hist.H.dtype.fields[name][0]) for name in Work["H_fields"]]
             H_to_be_sent = np.empty(len(work_rows), dtype=new_dtype)
             for i, row in enumerate(work_rows):
                 H_to_be_sent[i] = repack_fields(self.hist.H[Work["H_fields"]][row])
-            self.wcomms[w - 1].send(0, H_to_be_sent)
+
+            self.wcomms[w].send(0, H_to_be_sent)
 
     def _update_state_on_alloc(self, Work: dict, w: int):
         """Updates a workers' active/idle status following an allocation order"""
-        self.W[w - 1]["active"] = Work["tag"]
-        if "libE_info" in Work:
-            if "persistent" in Work["libE_info"]:
-                self.W[w - 1]["persis_state"] = Work["tag"]
-                if Work["libE_info"].get("active_recv", False):
-                    self.W[w - 1]["active_recv"] = Work["tag"]
-            else:
-                assert "active_recv" not in Work["libE_info"], "active_recv worker must also be persistent"
+
+        self.W[w]["active"] = Work["tag"]
+        if "persistent" in Work["libE_info"]:
+            self.W[w]["persis_state"] = Work["tag"]
+            if Work["libE_info"].get("active_recv", False):
+                self.W[w]["active_recv"] = True
+        else:
+            assert "active_recv" not in Work["libE_info"], "active_recv worker must also be persistent"
 
         work_rows = Work["libE_info"]["H_rows"]
         if Work["tag"] == EVAL_SIM_TAG:
             self.hist.update_history_x_out(work_rows, w, self.kill_canceled_sims)
         elif Work["tag"] == EVAL_GEN_TAG:
             self.hist.update_history_to_gen(work_rows)
 
@@ -413,74 +456,74 @@
         looped back over.
         """
         time.sleep(0.0001)  # Critical for multiprocessing performance
         new_stuff = True
         while new_stuff:
             new_stuff = False
             for w in self.W["worker_id"]:
-                if self.wcomms[w - 1].mail_flag():
+                if self.wcomms[w].mail_flag():
                     new_stuff = True
                     self._handle_msg_from_worker(persis_info, w)
 
         self._init_every_k_save()
         return persis_info
 
     def _update_state_on_worker_msg(self, persis_info: dict, D_recv: dict, w: int) -> None:
         """Updates history and worker info on worker message"""
         calc_type = D_recv["calc_type"]
         calc_status = D_recv["calc_status"]
 
         keep_state = D_recv["libE_info"].get("keep_state", False)
-        if w not in self.persis_pending and not self.W[w - 1]["active_recv"] and not keep_state:
-            self.W[w - 1]["active"] = 0
+        if w not in self.persis_pending and not self.W[w]["active_recv"] and not keep_state:
+            self.W[w]["active"] = 0
 
         if calc_status in [FINISHED_PERSISTENT_SIM_TAG, FINISHED_PERSISTENT_GEN_TAG]:
             final_data = D_recv.get("calc_out", None)
             if isinstance(final_data, np.ndarray):
                 if calc_status is FINISHED_PERSISTENT_GEN_TAG and self.libE_specs.get("use_persis_return_gen", False):
-                    self.hist.update_history_x_in(w, final_data, self.W[w - 1]["gen_started_time"])
+                    self.hist.update_history_x_in(w, final_data, self.W[w]["gen_started_time"])
                 elif calc_status is FINISHED_PERSISTENT_SIM_TAG and self.libE_specs.get("use_persis_return_sim", False):
                     self.hist.update_history_f(D_recv, self.kill_canceled_sims)
                 else:
                     logger.info(_PERSIS_RETURN_WARNING)
-            self.W[w - 1]["persis_state"] = 0
-            if self.W[w - 1]["active_recv"]:
-                self.W[w - 1]["active"] = 0
-                self.W[w - 1]["active_recv"] = 0
+            self.W[w]["persis_state"] = 0
+            if self.W[w]["active_recv"]:
+                self.W[w]["active"] = 0
+                self.W[w]["active_recv"] = False
             if w in self.persis_pending:
                 self.persis_pending.remove(w)
-                self.W[w - 1]["active"] = 0
+                self.W[w]["active"] = 0
             self._freeup_resources(w)
         else:
             if calc_type == EVAL_SIM_TAG:
                 self.hist.update_history_f(D_recv, self.kill_canceled_sims)
             if calc_type == EVAL_GEN_TAG:
-                self.hist.update_history_x_in(w, D_recv["calc_out"], self.W[w - 1]["gen_started_time"])
+                self.hist.update_history_x_in(w, D_recv["calc_out"], self.W[w]["gen_started_time"])
                 assert (
-                    len(D_recv["calc_out"]) or np.any(self.W["active"]) or self.W[w - 1]["persis_state"]
+                    len(D_recv["calc_out"]) or np.any(self.W["active"]) or self.W[w]["persis_state"]
                 ), "Gen must return work when is is the only thing active and not persistent."
             if "libE_info" in D_recv and "persistent" in D_recv["libE_info"]:
                 # Now a waiting, persistent worker
-                self.W[w - 1]["persis_state"] = calc_type
+                self.W[w]["persis_state"] = D_recv["calc_type"]
             else:
                 self._freeup_resources(w)
 
         if D_recv.get("persis_info"):
             persis_info[w].update(D_recv["persis_info"])
 
     def _handle_msg_from_worker(self, persis_info: dict, w: int) -> None:
         """Handles a message from worker w"""
         try:
-            msg = self.wcomms[w - 1].recv()
+            msg = self.wcomms[w].recv()
             tag, D_recv = msg
         except CommFinishedException:
             logger.debug(f"Finalizing message from Worker {w}")
             return
         if isinstance(D_recv, WorkerErrMsg):
-            self.W[w - 1]["active"] = 0
+            self.W[w]["active"] = 0
             logger.debug(f"Manager received exception from worker {w}")
             if not self.WorkerExc:
                 self.WorkerExc = True
                 self._kill_workers()
                 raise WorkerException(f"Received error message from worker {w}", D_recv.msg, D_recv.exc)
         elif isinstance(D_recv, logging.LogRecord):
             logger.debug(f"Manager received a log message from worker {w}")
@@ -505,15 +548,15 @@
 
             # Note that a return is still expected when running sims are killed
             if np.any(kill_sim):
                 logger.debug(f"Manager sending kill signals to H indices {kill_sim_rows}")
                 kill_ids = self.hist.H["sim_id"][kill_sim_rows]
                 kill_on_workers = self.hist.H["sim_worker"][kill_sim_rows]
                 for w in kill_on_workers:
-                    self.wcomms[w - 1].send(STOP_TAG, MAN_SIGNAL_KILL)
+                    self.wcomms[w].send(STOP_TAG, MAN_SIGNAL_KILL)
                     self.hist.H["kill_sent"][kill_ids] = True
 
     # --- Handle termination
 
     def _final_receive_and_kill(self, persis_info: dict) -> (dict, int, int):
         """
         Tries to receive from any active workers.
@@ -535,18 +578,18 @@
                         "tag": PERSIS_STOP,
                         "libE_info": {"persistent": True, "H_rows": rows_to_send},
                     }
                     self._check_work_order(work, w, force=True)
                     self._send_work_order(work, w)
                     self.hist.update_history_to_gen(rows_to_send)
                 else:
-                    self.wcomms[w - 1].send(PERSIS_STOP, MAN_SIGNAL_KILL)
-                if not self.W[w - 1]["active"]:
+                    self.wcomms[w].send(PERSIS_STOP, MAN_SIGNAL_KILL)
+                if not self.W[w]["active"]:
                     # Re-activate if necessary
-                    self.W[w - 1]["active"] = self.W[w - 1]["persis_state"]
+                    self.W[w]["active"] = self.W[w]["persis_state"]
                 self.persis_pending.append(w)
 
         exit_flag = 0
         while (any(self.W["active"]) or any(self.W["persis_state"])) and exit_flag == 0:
             persis_info = self._receive_from_workers(persis_info)
             if self.term_test(logged=False) == 2:
                 # Elapsed Wallclock has expired
@@ -581,14 +624,15 @@
             "scheduler_opts": self.scheduler_opts,
             "sim_started_count": self.hist.sim_started_count,
             "sim_ended_count": self.hist.sim_ended_count,
             "sim_max_given": self._sim_max_given(),
             "use_resource_sets": self.use_resource_sets,
             "gen_num_procs": self.gen_num_procs,
             "gen_num_gpus": self.gen_num_gpus,
+            "gen_on_manager": self.libE_specs.get("gen_on_manager", False),
         }
 
     def _alloc_work(self, H: npt.NDArray, persis_info: dict) -> dict:
         """
         Calls work allocation function from alloc_specs. Copies protected libE
         fields before the alloc_f call and ensures they weren't modified
         """
@@ -649,10 +693,11 @@
             raise LoggedException(e.args[0], e.args[1]) from None
         except Exception as e:
             logger.error(traceback.format_exc())
             raise LoggedException(e.args) from None
         finally:
             # Return persis_info, exit_flag, elapsed time
             result = self._final_receive_and_kill(persis_info)
+            self.wcomms = None
             sys.stdout.flush()
             sys.stderr.flush()
         return result
```

### Comparing `libensemble-1.2.2/libensemble/message_numbers.py` & `libensemble-1.3.0/libensemble/message_numbers.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/resources/env_resources.py` & `libensemble-1.3.0/libensemble/resources/env_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/resources/gpu_detect.py` & `libensemble-1.3.0/libensemble/resources/gpu_detect.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/resources/mpi_resources.py` & `libensemble-1.3.0/libensemble/resources/mpi_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/resources/node_resources.py` & `libensemble-1.3.0/libensemble/resources/node_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,52 +72,43 @@
         found_count = True
 
     if found_count:
         # Check all nodes have equal cores -  Not doing for other methods currently.
         if len(set(counter)) != 1:
             logger.warning(f"Detected compute nodes have different core counts: {set(counter)}")
 
-        physical_cores_avail_per_node = counter[0]
-        logical_cores_avail_per_node = counter[0]  # How to get SMT threads remotely
+        physical_cores_avail_per_node = min(counter)
+        logical_cores_avail_per_node = min(counter)  # How to get SMT threads remotely
         logger.warning("SMT currently not detected, returning physical cores only. Specify procs_per_node to override")
         return (physical_cores_avail_per_node, logical_cores_avail_per_node)
     else:
         return None
 
 
 def _cpu_info_complete(cores_info):
     """Returns true if cpu tuple/list entries have an integer value, else False"""
 
-    if cores_info is None:
-        return False
-
     for val in cores_info[:2]:
         if not isinstance(val, int):
             return False
     return True
 
 
 def _gpu_info_complete(cores_info):
     """Returns true if gpu tuple/list entries have an integer value, else False"""
 
-    if cores_info is None:
-        return False
-
     for val in cores_info[2:]:
         if not isinstance(val, int):
             return False
     return True
 
 
 def _complete_set(cores_info):
     """Returns True if all tuple/list entries have an integer value, else False"""
 
-    if cores_info is None:
-        return False
-
     for val in cores_info:
         if not isinstance(val, int):
             return False
     return True
 
 
 def _update_values(cores_info, cores_info_updates):
@@ -155,28 +146,25 @@
 
 
 def get_sub_node_resources(
     launcher: Optional[str] = None, remote_mode: bool = False, env_resources: Optional[EnvResources] = None
 ) -> Tuple[int, int, int]:
     """Returns logical and physical cores and GPUs per node as a tuple
 
-    First checks for known system values, then for environment values, and finally
-    for detected values. If remote_mode is True, then detection launches a job
-    via the MPI launcher.
+    First checks for environment values, and and then for detected values.
+    If remote_mode is True, then detection launches a job via the MPI launcher.
 
     Any value that is already valid, is not overwritten by successive stages.
 
     """
     cores_info = [None, None, None]
 
     # Check environment
-    if not _cpu_info_complete(cores_info):
-        cores_info[:2] = list(_get_cpu_resources_from_env(env_resources=env_resources) or [None, None])
-    if not _gpu_info_complete(cores_info):
-        cores_info[2] = get_gpus_from_env(env_resources=env_resources)
+    cores_info[:2] = list(_get_cpu_resources_from_env(env_resources=env_resources) or [None, None])
+    cores_info[2] = get_gpus_from_env(env_resources=env_resources)
     if _complete_set(cores_info):
         return tuple(cores_info)
 
     # Detection of cpu/gpu resources
     # If remote then launch probe, else detect locally
     if remote_mode:
         cores_info_str = _get_remote_resources(launcher=launcher)
```

### Comparing `libensemble-1.2.2/libensemble/resources/platforms.py` & `libensemble-1.3.0/libensemble/resources/platforms.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/resources/resources.py` & `libensemble-1.3.0/libensemble/resources/resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/resources/rset_resources.py` & `libensemble-1.3.0/libensemble/resources/rset_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class RSetResources:
     """A class that creates a fixed mapping of resource sets to the available resources.
 
     **Object Attributes:**
 
-    These are set on initialisation and include inherited.
+    These are set on initialization and include inherited.
     ``rsets`` below is used to abbreviate ``resource sets``.
 
     :ivar int num_workers: Total number of workers
     :ivar int num_workers_2assign2: The number of workers that will be assigned resource sets.
     :ivar int total_num_rsets: The total number of resource sets.
     :ivar list split_list: A list of lists, where each element is the list of nodes for a given rset.
     :ivar list local_rsets_list: A list over rsets, where each element is the number of rsets that share the node.
@@ -125,15 +125,15 @@
     def get_workers2assign2(num_workers, resources):
         """Returns workers to assign resources to"""
         zero_resource_list = resources.zero_resource_workers
         return num_workers - len(zero_resource_list)
 
     @staticmethod
     def even_assignment(nnodes, nworkers):
-        """Returns True if workers are evenly distributied to nodes, else False"""
+        """Returns True if workers are evenly distributed to nodes, else False"""
         try:
             return nnodes % nworkers == 0 or nworkers % nnodes == 0
         except ZeroDivisionError:
             logger.error("Either nworkers or nnodes is zero. Check that MPI ranks > 1")
             raise
 
     @staticmethod
```

### Comparing `libensemble-1.2.2/libensemble/resources/scheduler.py` & `libensemble-1.3.0/libensemble/resources/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         if self.avail_rsets_by_group is None:
             rsets = self.resources.rsets
             groups = np.unique(rsets["group"])
             self.avail_rsets_by_group = {}
             for g in groups:
                 self.avail_rsets_by_group[g] = []
             for ind, rset in enumerate(rsets):
-                if not rset["assigned"]:
+                if rset["assigned"] == -1:  # now default is -1.
                     g = rset["group"]
                     self.avail_rsets_by_group[g].append(ind)
         return self.avail_rsets_by_group
 
     def filter_for_rset_type(self, avail_rsets_by_group, use_gpus):
         """Return avail_rsets_by_group filtered by rset type (gpus/non-gpus/all)"""
```

### Comparing `libensemble-1.2.2/libensemble/resources/worker_resources.py` & `libensemble-1.3.0/libensemble/resources/worker_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.index_list = ResourceManager.get_index_list(
             self.num_workers,
             self.total_num_rsets,
             resources.zero_resource_workers,
         )
 
         self.rsets = np.zeros(self.total_num_rsets, dtype=ResourceManager.man_rset_dtype)
-        self.rsets["assigned"] = 0
+        self.rsets["assigned"] = -1
         for field in self.all_rsets.dtype.names:
             self.rsets[field] = self.all_rsets[field]
         self.num_groups = self.rsets["group"][-1]
 
         self.rsets_free = self.total_num_rsets
         self.gpu_rsets_free = self.total_num_gpu_rsets
         self.nongpu_rsets_free = self.total_num_nongpu_rsets
@@ -66,36 +66,36 @@
         self.even_groups = True if len(self.ngroups_by_size) == 1 else False
 
     def assign_rsets(self, rset_team, worker_id):
         """Mark the resource sets given by rset_team as assigned to worker_id"""
         if rset_team:
             rteam = self.rsets["assigned"][rset_team]
             for i, wid in enumerate(rteam):
-                if wid == 0:
+                if wid == -1:
                     self.rsets["assigned"][rset_team[i]] = worker_id
                     self.rsets_free -= 1
                     if self.rsets["gpus"][rset_team[i]]:
                         self.gpu_rsets_free -= 1
                     else:
                         self.nongpu_rsets_free -= 1
                 elif wid != worker_id:
                     ResourceManagerException(
                         f"Error: Attempting to assign rsets {rset_team}" f" already assigned to workers: {rteam}"
                     )
 
     def free_rsets(self, worker=None):
         """Free up assigned resource sets"""
         if worker is None:
-            self.rsets["assigned"] = 0
+            self.rsets["assigned"] = -1
             self.rsets_free = self.total_num_rsets
             self.gpu_rsets_free = self.total_num_gpu_rsets
             self.nongpu_rsets_free = self.total_num_nongpu_rsets
         else:
             rsets_to_free = np.where(self.rsets["assigned"] == worker)[0]
-            self.rsets["assigned"][rsets_to_free] = 0
+            self.rsets["assigned"][rsets_to_free] = -1
             self.rsets_free += len(rsets_to_free)
             self.gpu_rsets_free += np.count_nonzero(self.rsets["gpus"][rsets_to_free])
             self.nongpu_rsets_free += np.count_nonzero(~self.rsets["gpus"][rsets_to_free])
 
     @staticmethod
     def get_index_list(
         num_workers: int, num_rsets: int, zero_resource_list: List[Union[int, Any]]
```

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/borehole.py` & `libensemble-1.3.0/libensemble/sim_funcs/borehole.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/borehole_kills.py` & `libensemble-1.3.0/libensemble/sim_funcs/borehole_kills.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/branin/branin.py` & `libensemble-1.3.0/libensemble/sim_funcs/branin/branin.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/branin/branin_obj.py` & `libensemble-1.3.0/libensemble/sim_funcs/branin/branin_obj.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/chwirut1.py` & `libensemble-1.3.0/libensemble/sim_funcs/chwirut1.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/executor_hworld.py` & `libensemble-1.3.0/libensemble/sim_funcs/executor_hworld.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/heffte.py` & `libensemble-1.3.0/libensemble/sim_funcs/heffte.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/mock_sim.py` & `libensemble-1.3.0/libensemble/sim_funcs/mock_sim.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/noisy_vector_mapping.py` & `libensemble-1.3.0/libensemble/sim_funcs/noisy_vector_mapping.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/one_d_func.py` & `libensemble-1.3.0/libensemble/sim_funcs/one_d_func.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/rosenbrock.py` & `libensemble-1.3.0/libensemble/sim_funcs/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/run_line_check.py` & `libensemble-1.3.0/libensemble/sim_funcs/run_line_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     p_gens = sim_specs["user"].get("persis_gens", 0)
 
     for i, test in enumerate(test_list):
         task = exctr.submit(
             calc_type="sim",
             num_procs=test.get("nprocs", None),
             num_nodes=test.get("nnodes", None),
+            num_gpus=test.get("ngpus", None),
             procs_per_node=test.get("ppn", None),
             extra_args=test.get("e_args", None),
             app_args="--testid " + test.get("testid", None),
             stdout="out.txt",
             stderr="err.txt",
             hyperthreads=test.get("ht", None),
             dry_run=True,
```

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/six_hump_camel.py` & `libensemble-1.3.0/libensemble/sim_funcs/six_hump_camel.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/surmise_test_function.py` & `libensemble-1.3.0/libensemble/sim_funcs/surmise_test_function.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/var_resources.py` & `libensemble-1.3.0/libensemble/sim_funcs/var_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/sim_funcs/ytopt_obj.py` & `libensemble-1.3.0/libensemble/sim_funcs/ytopt_obj.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/specs.py` & `libensemble-1.3.0/libensemble/specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,19 @@
     globus_compute_endpoint: Optional[str] = ""
     """
     A Globus Compute (https://www.globus.org/compute) ID corresponding to an active endpoint on a remote system.
     libEnsemble's workers will submit simulator function instances to this endpoint instead of
     calling them locally.
     """
 
+    threaded: Optional[bool] = False
+    """
+    Instruct Worker process to launch user function to a thread.
+    """
+
     user: Optional[dict] = {}
     """
     A user-data dictionary to place bounds, constants, settings, or other parameters for customizing
     the simulator function.
     """
 
 
@@ -96,14 +101,19 @@
     globus_compute_endpoint: Optional[str] = ""
     """
     A Globus Compute (https://www.globus.org/compute) ID corresponding to an active endpoint on a remote system.
     libEnsemble's workers will submit generator function instances to this endpoint instead of
     calling them locally.
     """
 
+    threaded: Optional[bool] = False
+    """
+    Instruct Worker process to launch user function to a thread.
+    """
+
     user: Optional[dict] = {}
     """
     A user-data dictionary to place bounds, constants, settings, or other parameters for
     customizing the generator function
     """
 
 
@@ -153,18 +163,27 @@
 
 class LibeSpecs(BaseModel):
     """
     Specifications for configuring libEnsemble's runtime behavior.
     """
 
     comms: Optional[str] = "mpi"
-    """ Manager/Worker communications mode. ``'mpi'``, ``'local'``, ``'threads'``, or ``'tcp'`` """
+    """
+    Manager/Worker communications mode. ``'mpi'``, ``'local'``, ``'threads'``, or ``'tcp'``
+    If ``nworkers`` is specified, then ``local`` comms will be used unless a parallel MPI
+    environment is detected.
+    """
 
     nworkers: Optional[int] = 0
-    """ Number of worker processes in ``"local"`` or ``"tcp"``."""
+    """ Number of worker processes in ``"local"``, ``"threads"``, or ``"tcp"``."""
+
+    gen_on_manager: Optional[bool] = False
+    """ Instructs Manager process to run generator functions.
+    This generator function can access/modify user objects by reference.
+    """
 
     mpi_comm: Optional[Any] = None
     """ libEnsemble MPI communicator. Default: ``MPI.COMM_WORLD``"""
 
     dry_run: Optional[bool] = False
     """ Whether libEnsemble should immediately exit after validating all inputs. """
 
@@ -440,14 +459,20 @@
     zero_resource_workers: Optional[List[int]] = []
     """
     List of workers that require no resources. For when a fixed mapping of workers
     to resources is required. Otherwise, use ``num_resource_sets``.
     For use with supported allocation functions.
     """
 
+    gen_workers: Optional[List[int]] = []
+    """
+    List of workers that should only run generators. All other workers will only
+    run simulator functions.
+    """
+
     resource_info: Optional[dict] = {}
     """
     Resource information to override automatically detected resources.
     Allowed fields are given below in 'Overriding Resource Auto-detection'.
     Note that if ``disable_resource_manager`` is set then this option is ignored.
     """
```

### Comparing `libensemble-1.2.2/libensemble/tests/.coveragerc` & `libensemble-1.3.0/libensemble/tests/.coveragerc`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/1d_sampling.json` & `libensemble-1.3.0/libensemble/tests/functionality_tests/1d_sampling.json`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/check_libE_stats.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/check_libE_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """Iterate over rows in infile and check delimiters and datetime formats"""
     with open(infile) as f:
         total_cnt = 0
         for line in f:
             s_cnt = 0
             e_cnt = 0
             lst = line.split()
-            if lst[0] == "Manager":
+            if line.startswith("Manager     : Starting") or line.startswith("Manager     : Exiting"):
                 check_datetime(lst[5], lst[6])
                 continue
             for i, val in enumerate(lst):
                 if val == start:
                     s1 = lst[i + 1]
                     s2 = lst[i + 2]
                     check_datetime(s1, s2)
```

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/forces_simf.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/sine_gen.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/sine_gen.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_sampling_from_files.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_sampling_from_files.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_sampling_with_profile.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_sampling_with_profile.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_splitcomm.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_splitcomm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_subcomm.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_subcomm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_super_simple.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_super_simple.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_GPU_gen_resources.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_GPU_gen_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,34 +96,38 @@
         },
     }
 
     exit_criteria = {"sim_max": 20}
     libE_specs["resource_info"] = {"cores_on_node": (nworkers * 2, nworkers * 4), "gpus_on_node": nworkers}
 
     base_libE_specs = libE_specs.copy()
-    for run in range(5):
-        # reset
-        libE_specs = base_libE_specs.copy()
-        persis_info = add_unique_random_streams({}, nworkers + 1)
+    for gen_on_manager in [False, True]:
+        for run in range(5):
+            # reset
+            libE_specs = base_libE_specs.copy()
+            libE_specs["gen_on_manager"] = gen_on_manager
+            persis_info = add_unique_random_streams({}, nworkers + 1)
 
-        if run == 0:
-            libE_specs["gen_num_procs"] = 2
-        elif run == 1:
-            libE_specs["gen_num_gpus"] = 1
-        elif run == 2:
-            persis_info["gen_num_gpus"] = 1
-        elif run == 3:
-            # Two GPUs per resource set
-            libE_specs["resource_info"]["gpus_on_node"] = nworkers * 2
-            persis_info["gen_num_gpus"] = 1
-        elif run == 4:
-            # Two GPUs requested for gen
-            persis_info["gen_num_procs"] = 2
-            persis_info["gen_num_gpus"] = 2
-            gen_specs["user"]["max_procs"] = max(nworkers - 2, 1)
+            if run == 0:
+                libE_specs["gen_num_procs"] = 2
+            elif run == 1:
+                if gen_on_manager:
+                    print("SECOND LIBE CALL WITH GEN ON MANAGER")
+                libE_specs["gen_num_gpus"] = 1
+            elif run == 2:
+                persis_info["gen_num_gpus"] = 1
+            elif run == 3:
+                # Two GPUs per resource set
+                libE_specs["resource_info"]["gpus_on_node"] = nworkers * 2
+                persis_info["gen_num_gpus"] = 1
+            elif run == 4:
+                # Two GPUs requested for gen
+                persis_info["gen_num_procs"] = 2
+                persis_info["gen_num_gpus"] = 2
+                gen_specs["user"]["max_procs"] = max(nworkers - 2, 1)
 
-        # Perform the run
-        H, persis_info, flag = libE(
-            sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs, alloc_specs=alloc_specs
-        )
+            # Perform the run
+            H, persis_info, flag = libE(
+                sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs, alloc_specs=alloc_specs
+            )
 
 # All asserts are in gen and sim funcs
```

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_calc_exception.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_calc_exception.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_cancel_in_alloc.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_cancel_in_alloc.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_comms.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_comms.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_elapsed_time_abort.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_elapsed_time_abort.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_forces_tutorial.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_forces_tutorial.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_forces_tutorial_2.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_forces_tutorial_2.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_hworld_timeout.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_hworld_timeout.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_executor_simple.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_executor_simple.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_fast_alloc.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_fast_alloc.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_local_sine_tutorial.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_local_sine_tutorial.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_local_sine_tutorial_2.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_local_sine_tutorial_2.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_local_sine_tutorial_3.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_local_sine_tutorial_3.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_comms.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_comms.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_gpu_settings.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_gpu_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
 from libensemble.executors.mpi_executor import MPIExecutor
 from libensemble.gen_funcs.persistent_sampling_var_resources import uniform_sample as gen_f
 
 # Import libEnsemble items for this test
 from libensemble.libE import libE
-from libensemble.resources.platforms import Frontier, PerlmutterGPU, Platform, Polaris, Summit, Sunspot
+from libensemble.resources.platforms import Aurora, Frontier, PerlmutterGPU, Platform, Polaris, Summit
 from libensemble.sim_funcs import six_hump_camel
 from libensemble.sim_funcs.var_resources import gpu_variable_resources as sim_f
 from libensemble.tools import add_unique_random_streams, parse_args
 
 # from libensemble import logger
 # logger.set_level("DEBUG")  # For testing the test
 
@@ -109,15 +109,15 @@
     # Ensure LIBE_PLATFORM environment variable is not set.
     if "LIBE_PLATFORM" in os.environ:
         del os.environ["LIBE_PLATFORM"]
 
     # First set - use executor setting ------------------------------------------------------------
     libE_specs["resource_info"] = {"gpus_on_node": 4}  # Mock GPU system / remove to detect GPUs
 
-    for run_set in ["mpich", "openmpi", "aprun", "srun", "jsrun", "custom"]:
+    for run_set in ["mpich", "openmpi", "aprun", "srun", "jsrun", "msmpi", "custom"]:
         print(f"\nRunning GPU setting checks (via resource_info / custom_info) for {run_set} ------------- ")
         exctr = MPIExecutor(custom_info={"mpi_runner": run_set})
         exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
 
         # Reset persis_info. If has num_gens_started > 0 from alloc, will not runs any sims.
         persis_info = add_unique_random_streams({}, nworkers + 1)
 
@@ -134,15 +134,15 @@
         cores_per_node=64,
         logical_cores_per_node=128,
         gpus_per_node=8,
         gpu_setting_type="runner_default",
         scheduler_match_slots=False,
     )
 
-    for run_set in ["mpich", "openmpi", "aprun", "srun", "jsrun", "custom"]:
+    for run_set in ["mpich", "openmpi", "aprun", "srun", "jsrun", "msmpi", "custom"]:
         print(f"\nRunning GPU setting checks (via platform_specs class) for {run_set} ------------------- ")
         libE_specs["platform_specs"].mpi_runner = run_set
 
         print(f'{libE_specs["platform_specs"]=}')
 
         exctr = MPIExecutor()
         exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
@@ -171,15 +171,15 @@
         "cores_per_node": 64,
         "logical_cores_per_node": 128,
         "gpus_per_node": 8,
         "gpu_setting_type": "runner_default",
         "scheduler_match_slots": False,
     }
 
-    for run_set in ["mpich", "openmpi", "aprun", "srun", "jsrun", "custom"]:
+    for run_set in ["mpich", "openmpi", "aprun", "srun", "jsrun", "msmpi", "custom"]:
         print(f"\nRunning GPU setting checks (via platform_specs dict) for {run_set} ------------------- ")
         libE_specs["platform_specs"]["mpi_runner"] = run_set
 
         print(f'{libE_specs["platform_specs"]=}')
 
         exctr = MPIExecutor()
         exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
@@ -199,15 +199,15 @@
         H, _, flag = libE(
             sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs, alloc_specs=alloc_specs
         )
 
     del libE_specs["platform_specs"]
 
     # Fourth set - use platform setting ------------------------------------------------------------
-    for platform in ["summit", "crusher", "perlmutter_g", "polaris", "sunspot"]:
+    for platform in ["summit", "crusher", "perlmutter_g", "polaris", "aurora"]:
         print(f"\nRunning GPU setting checks (via known platform) for {platform} ------------------- ")
         libE_specs["platform"] = platform
 
         exctr = MPIExecutor()
         exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
 
         # Reset persis_info. If has num_gens_started > 0 from alloc, will not runs any sims.
@@ -217,15 +217,15 @@
         H, _, flag = libE(
             sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs, alloc_specs=alloc_specs
         )
 
         del libE_specs["platform"]
 
     # Fifth set - use platform environment setting -----------------------------------------------
-    for platform in ["summit", "crusher", "perlmutter_g", "polaris", "sunspot"]:
+    for platform in ["summit", "crusher", "perlmutter_g", "polaris", "aurora"]:
         print(f"\nRunning GPU setting checks (via known platform env. variable) for {platform} ----- ")
         os.environ["LIBE_PLATFORM"] = platform
 
         exctr = MPIExecutor()
         exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
 
         # Reset persis_info. If has num_gens_started > 0 from alloc, will not runs any sims.
@@ -235,15 +235,15 @@
         H, _, flag = libE(
             sim_specs, gen_specs, exit_criteria, persis_info, libE_specs=libE_specs, alloc_specs=alloc_specs
         )
 
         del os.environ["LIBE_PLATFORM"]
 
     # Sixth set - use platform_specs with known systems -------------------------------------------
-    for platform in [Summit, Frontier, PerlmutterGPU, Polaris, Sunspot]:
+    for platform in [Summit, Frontier, PerlmutterGPU, Polaris, Aurora]:
         print(f"\nRunning GPU setting checks (via known platform - platform_specs) for {platform} ------------------- ")
         libE_specs["platform_specs"] = platform()
 
         exctr = MPIExecutor()
         exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
 
         # Reset persis_info. If has num_gens_started > 0 from alloc, will not runs any sims.
```

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_gpu_settings_env.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_gpu_settings_env.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_gpu_settings_mock_nodes_multi_task.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_gpu_settings_mock_nodes_multi_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 
 Uses the dry_run option to test correct GPU settings for different mocked up systems.
 Test assertions are in the sim function via the check_gpu_setting function.
 
 The persistent generator creates simulations with variable resource requirements.
 
 Execute via one of the following commands (e.g. 5 workers):
-   mpiexec -np 6 python test_mpi_gpu_settings.py
-   python test_mpi_gpu_settings.py --comms local --nworkers 5
+   mpiexec -np 6 python test_mpi_gpu_settings_mock_nodes_multi_task.py
+   python test_mpi_gpu_settings_mock_nodes_multi_task.py --comms local --nworkers 5
 
 When running with the above command, the number of concurrent evaluations of
 the objective function will be 4, as one of the five workers will be the
 persistent generator.
 """
 
 # Do not change these lines - they are parsed by run-tests.sh
+# The 12 process (11 worker) run is necessary to test configurations that must be adjusted.
 # TESTSUITE_COMMS: mpi local
-# TESTSUITE_NPROCS: 3 6
+# TESTSUITE_NPROCS: 3 6 12
 
 import os
 import sys
 
 import numpy as np
 
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
```

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     if comms == "mpi":
         libE_specs["mpi_comm"].Barrier()
 
     # Mock up system
     custom_resources = {
         "cores_on_node": (16, 64),  # Tuple (physical cores, logical cores)
         "node_file": node_file,  # Name of file containing a node-list
+        "gpus_on_node": 4,  # For tests with ngpus
     }
     libE_specs["resource_info"] = custom_resources
 
     persis_info = add_unique_random_streams({}, nworkers + 1)
     exit_criteria = {"sim_max": nworkers * rounds}
 
     sim_specs = {
@@ -106,14 +107,17 @@
         {"testid": "ap2", "e_args": "-n 8 --xarg 1 -N 4"},  # parse extra_args
     ]
 
     # Note in a8: -n 8 is abbreviated form of --ntasks, this should be unaltered while --nodes is derived and inserted.
     eargs_srun = [
         {"testid": "sr1", "nprocs": 16, "e_args": "--xarg 1 --ntasks-per-node 16"},  # nprocs + parse extra_args
         {"testid": "sr2", "e_args": "-n 8 --xarg 1 --ntasks-per-node 4"},  # parse extra_args
+        {"testid": "sr3", "e_args": "--nodes 2 -n 8 --xarg 1 --ntasks-per-node 4"},
+        {"testid": "sr4", "ngpus": 8, "e_args": "--nodes 2 -n 8 --xarg 1 --ntasks-per-node 4"},
+        {"testid": "sr5", "ngpus": 8, "e_args": "-n 8 --xarg 1 --ntasks-per-node 4"}
     ]
 
     # Note for jsrun: proc = resource set. Awkward naming but this seems like the best solution.
     # Define extra_args as minimal relation of tasks/cores/gpus (one resource set), then n (nprocs) as multiplier.
     eargs_jsrun = [
         {"testid": "jsr1", "nprocs": 16, "e_args": "--xarg 1 -r 16"},  # nprocs + parse extra_args
         {"testid": "jsr2", "e_args": "-n 8 --xarg 1 -r 4"},  # parse extra_args
@@ -178,14 +182,17 @@
         "srun -w node-1,node-2 --ntasks 32 --nodes 2 --ntasks-per-node 16 --exact /path/to/fakeapp.x --testid base2",
         "srun -w node-1,node-2 --ntasks 32 --nodes 2 --ntasks-per-node 16 --xarg 1 --exact /path/to/fakeapp.x --testid base3",
         "srun -w node-1,node-2 --ntasks 128 --nodes 2 --ntasks-per-node 64 --xarg 1 --exact /path/to/fakeapp.x --testid base4",
         "srun -w node-1 --ntasks 16 --nodes 1 --ntasks-per-node 16 --xarg 1 --exact /path/to/fakeapp.x --testid base5",
         "srun -w node-1,node-2 --ntasks 16 --nodes 2 --ntasks-per-node 8 --xarg 1 --exact /path/to/fakeapp.x --testid base6",
         "srun -w node-1 --ntasks 16 --nodes 1 --xarg 1 --ntasks-per-node 16 --exact /path/to/fakeapp.x --testid sr1",
         "srun -w node-1,node-2 --nodes 2 -n 8 --xarg 1 --ntasks-per-node 4 --exact /path/to/fakeapp.x --testid sr2",
+        "srun -w node-1,node-2 --nodes 2 -n 8 --xarg 1 --ntasks-per-node 4 --exact /path/to/fakeapp.x --testid sr3",
+        "srun -w node-1,node-2 --nodes 2 -n 8 --xarg 1 --ntasks-per-node 4 --gpus-per-task 1 --exact /path/to/fakeapp.x --testid sr4",
+        "srun -w node-1,node-2 --nodes 2 -n 8 --xarg 1 --ntasks-per-node 4 --gpus-per-task 1 --exact /path/to/fakeapp.x --testid sr5",
     ]
 
     exp_jsrun = [
         "jsrun -n 2 -r 2 --xarg 1 /path/to/fakeapp.x --testid base1",
         "jsrun -n 32 /path/to/fakeapp.x --testid base2",
         "jsrun -n 32 --xarg 1 /path/to/fakeapp.x --testid base3",
         "jsrun -n 128 --xarg 1 /path/to/fakeapp.x --testid base4",
```

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_subnode.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_subnode.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_subnode_uneven.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_supernode_uneven.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_zrw_subnode_uneven.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_mpi_runners_zrw_supernode_uneven.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_new_field.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_new_field.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_sampling_CUDA_variable_resources.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_sampling_CUDA_variable_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_sim_uniform_sampling.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_sim_uniform_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_gen_decides_stop.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_gen_decides_stop.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     alloc_specs = {"alloc_f": alloc_f}
 
     exit_criteria = {"gen_max": num_batches * batch, "wallclock_max": 300}
 
     libE_specs["kill_canceled_sims"] = False
 
-    for run in range(3):
+    for run in range(5):
         persis_info = add_unique_random_streams({}, nworkers + 1)
         for i in persis_info:
             persis_info[i]["get_grad"] = True
 
         if run == 0:
             gen_specs["gen_f"] = gen_f1
         elif run == 1:
@@ -82,14 +82,19 @@
             gen_specs["out"] = [("x", float, (2 * m,)), ("obj_component", int)]
             gen_specs["user"]["num_components"] = m
             gen_specs["user"]["lb"] = np.arange(-2 * m - 1, -1)
             gen_specs["user"]["ub"] = np.arange(2 * m + 1, 1, -1)
             sim_specs["out"] = [("f_i", float), ("gradf_i", float, 2 * m)]
             sim_specs["in"] = ["x", "obj_component"]
             # sim_specs["out"] = [("f", float), ("grad", float, n)]
+        elif run == 3:
+            libE_specs["gen_on_manager"] = True
+        elif run == 4:
+            libE_specs["gen_on_manager"] = False
+            libE_specs["gen_workers"] = [2]
 
         # Perform the run
         H, persis_info, flag = libE(sim_specs, gen_specs, exit_criteria, persis_info, alloc_specs, libE_specs)
 
         if is_manager:
             assert len(np.unique(H["gen_ended_time"])) == num_batches
```

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_async.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_async.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_cancel.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_cancel.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_nonblocking.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_nonblocking.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_running_mean.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_persistent_uniform_sampling_running_mean.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_runlines_adaptive_workers.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_runlines_adaptive_workers_persistent_oversubscribe_rsets.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_dirs_per_calc.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_dirs_per_worker.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_dirs_with_exception.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_dirs_with_gen_dirs.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_sim_input_dir_option.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_sim_input_dir_option.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_stats_output.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_stats_output.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling_cancel.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling_cancel.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling_one_residual_at_a_time.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling_one_residual_at_a_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling_then_persistent_localopt_runs.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling_then_persistent_localopt_runs.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_uniform_sampling_with_variable_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_worker_exceptions.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_worker_exceptions.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_workflow_dir.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_workflow_dir.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_zero_resource_workers.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_zero_resource_workers.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py` & `libensemble-1.3.0/libensemble/tests/functionality_tests/test_zero_resource_workers_subnode.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/common.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/common.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/optimizer.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/optimizer.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m` & `libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ECnoise.m`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m` & `libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/call_matlab_octave_script.m`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/exe.pl` & `libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/exe.pl`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.pl` & `libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.pl`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/plopper.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/processexe.pl` & `libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/processexe.pl`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/runs.sh` & `libensemble-1.3.0/libensemble/tests/regression_tests/scripts_used_by_reg_tests/ytopt-libe-speed3d/runs.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/support.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/support.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_1d_sampling.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_1d_sampling.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_GPU_variable_resources.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_GPU_variable_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_GPU_variable_resources_multi_task.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_GPU_variable_resources_multi_task.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_ensemble_platform_workdir.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_ensemble_platform_workdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import glob
 import os
 import re
+
 import numpy as np
 
+# Import libEnsemble items for this test
+from libensemble import Ensemble
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens as alloc_f
 from libensemble.executors.mpi_executor import MPIExecutor
 from libensemble.gen_funcs.persistent_sampling_var_resources import uniform_sample as gen_f
-
-# Import libEnsemble items for this test
-from libensemble import Ensemble
 from libensemble.resources.platforms import PerlmutterGPU
 from libensemble.sim_funcs import six_hump_camel
 from libensemble.sim_funcs.var_resources import gpu_variable_resources as sim_f
 from libensemble.specs import LibeSpecs
 
-
 # from libensemble import logger
 # logger.set_level("DEBUG")  # For testing the test
 
 # Main block is necessary only when using local comms with spawn start method (default on macOS and Windows).
 if __name__ == "__main__":
     # Get paths for applications to run
     six_hump_camel_app = six_hump_camel.__file__
@@ -37,20 +36,21 @@
     # Ensure LIBE_PLATFORM environment variable is not set.
     if "LIBE_PLATFORM" in os.environ:
         del os.environ["LIBE_PLATFORM"]
 
     exctr = MPIExecutor()
     exctr.register_app(full_path=six_hump_camel_app, app_name="six_hump_camel")
 
-    ensemble = Ensemble(parse_args=True,
-                        executor=exctr,
-                        alloc_specs=alloc_specs,
-                        exit_criteria=exit_criteria,
-                        # libE_specs = LibeSpecs(use_workflow_dir=True, platform_specs=platform_specs),  # works
-                        )
+    ensemble = Ensemble(
+        parse_args=True,
+        executor=exctr,
+        alloc_specs=alloc_specs,
+        exit_criteria=exit_criteria,
+        # libE_specs = LibeSpecs(use_workflow_dir=True, platform_specs=platform_specs),  # works
+    )
 
     platform_specs = PerlmutterGPU()
     ensemble.libE_specs = LibeSpecs(
         num_resource_sets=ensemble.nworkers - 1,
         resource_info={"gpus_on_node": 4},
         use_workflow_dir=True,
         platform_specs=platform_specs,
@@ -79,13 +79,13 @@
     ensemble.run()
 
     if ensemble.is_manager:
         matching_dirs = glob.glob("workflow_*")
         assert matching_dirs, "No workflow dir found"
         most_recent_dir = max(matching_dirs, key=os.path.getctime)
         print(f"Checking ensemble.log in {most_recent_dir}")
-        file_path = file_path = os.path.join(most_recent_dir, 'ensemble.log')
+        file_path = file_path = os.path.join(most_recent_dir, "ensemble.log")
         if os.path.exists(file_path):  # an assert
-            with open(file_path, 'r') as file:
+            with open(file_path, "r") as file:
                 content = file.read()
                 pattern = r"Runline:\s+srun"
                 assert re.findall(pattern, content), "Incorrect MPI runner"
```

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_evaluate_existing_sample.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_evaluate_existing_sample.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_evaluate_mixed_sample.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_evaluate_mixed_sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     H0["x"] = gen_borehole_input(samp)
     for i in range(500):
         H0["f"][i] = borehole_func(H0["x"][i])
     H0["sim_started"][:500] = True
     H0["sim_ended"][:500] = True
 
     sampling = Ensemble(parse_args=True)
+    sampling.libE_specs.gen_on_manager = True
     sampling.H0 = H0
     sampling.sim_specs = SimSpecs(sim_f=sim_f, inputs=["x"], out=[("f", float)])
     sampling.alloc_specs = AllocSpecs(alloc_f=alloc_f)
     sampling.exit_criteria = ExitCriteria(sim_max=len(H0))
     sampling.run()
 
     if sampling.is_manager:
```

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_gpCAM.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_gpCAM.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_heffte.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_heffte.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_inverse_bayes_example.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_inverse_bayes_example.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_dfols.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_exception.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_exception.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_external_localopt.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_ibcdfo_pounders.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_ibcdfo_pounders.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_nlopt.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_periodic.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_pounders.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_pounders.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_scipy.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_tao_blmvm.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_tao_blmvm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_tao_nm.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_tao_nm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_timeout.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_aposmm_with_grad.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_fd_param_finder.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_fd_param_finder.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_gp.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_gp.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_gp_multitask_ax.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_surmise_calib.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_surmise_calib.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_surmise_killsims.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_surmise_killsims.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_tasmanian.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_tasmanian.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_persistent_tasmanian_async.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_persistent_tasmanian_async.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_with_app_persistent_aposmm_tao_nm.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_with_app_persistent_aposmm_tao_nm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/regression_tests/test_ytopt_heffte.py` & `libensemble-1.3.0/libensemble/tests/regression_tests/test_ytopt_heffte.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/run-tests.sh` & `libensemble-1.3.0/libensemble/tests/run-tests.sh`

 * *Files 4% similar despite different names*

```diff
@@ -602,17 +602,15 @@
       done #tests
     done #functionality/regression directories
     reg_end=$(current_time)
     reg_time=$(total_time $reg_start $reg_end)
 
     # ********* End Loop over regression tests *********
 
-    #Create Coverage Reports ----------------------------------------------
-
-    #Only if passed
+    # Only if passed
     if [ "$code" -eq "0" ]; then
 
       echo -e "\n..Moving output files to output dir"
 
       for DIR in $REG_TEST_SUBDIR $FUNC_TEST_SUBDIR
       do
         cd $ROOT_DIR/$DIR
@@ -623,59 +621,16 @@
 
         #sh - shld active_runs be prefixed for each job
         filelist=(*.$REG_TEST_OUTPUT_EXT);   [ -e ${filelist[0]} ] && mv *.$REG_TEST_OUTPUT_EXT output/
         filelist=(*.npy);                    [ -e ${filelist[0]} ] && mv *.npy output/
         filelist=(*active_runs.txt);         [ -e ${filelist[0]} ] && mv *active_runs.txt output/
 
       done
-      cd $ROOT_DIR
-
-      if [ "$RUN_COV_TESTS" = true ]; then
 
-        # Merge MPI coverage data for all ranks from regression tests and create xml report in sub-dir
-
-        for DIR in $REG_TEST_SUBDIR $FUNC_TEST_SUBDIR
-        do
-          cd $ROOT_DIR/$DIR
-
-          # Must combine all if in sep sub-dirs will copy to dir above
-          coverage combine .cov_reg_out* #Name of coverage data file must match that in .coveragerc in reg test dir.
-          coverage xml
-          echo -e "..Coverage xml written to dir $DIR/cov_reg/"
-
-        done
-        cd $ROOT_DIR
-
-        if [ "$RUN_UNIT_TESTS" = true ]; then
-
-          #Combine with unit test coverage at top-level
-          cd $ROOT_DIR/$COV_MERGE_DIR
-          cp $ROOT_DIR/$UNIT_TEST_SUBDIR/.cov_unit_out .
-          cp $ROOT_DIR/$UNIT_TEST_NOMPI_SUBDIR/.cov_unit_out2 .
-          cp $ROOT_DIR/$UNIT_TEST_LOGGER_SUBDIR/.cov_unit_out3 .
-          cp $ROOT_DIR/$REG_TEST_SUBDIR/.cov_reg_out .
-          cp $ROOT_DIR/$FUNC_TEST_SUBDIR/.cov_reg_out2 .
-
-          #coverage combine --rcfile=.coverage_merge.rc .cov_unit_out .cov_reg_out
-          coverage combine .cov_unit_out .cov_unit_out2 .cov_unit_out3 .cov_reg_out .cov_reg_out2 #Should create .cov_merge_out - see .coveragerc
-          coverage xml #Should create cov_merge/ dir
-          echo -e "..Combined Unit Test/Regression Test Coverage xml written to dir $COV_MERGE_DIR/cov_merge/"
-
-        else
-
-          # Still need to move reg cov results to COV_MERGE_DIR
-          cd $ROOT_DIR/$COV_MERGE_DIR
-          cp $ROOT_DIR/$REG_TEST_SUBDIR/.cov_reg_out .
-          cp $ROOT_DIR/$FUNC_TEST_SUBDIR/.cov_reg_out2 .
-
-          coverage combine .cov_reg_out .cov_reg_out2
-          coverage xml
-          echo -e "..Combined Regression Test Coverage xml written to dir $COV_MERGE_DIR/cov_merge/"
-        fi;
-      fi;
+      cd $ROOT_DIR
     fi;
 
     #All reg tests - summary ----------------------------------------------
     if [ "$code" -eq "0" ]; then
       echo
       #tput bold; tput setaf 2
 
@@ -707,14 +662,51 @@
       tput bold; tput setaf 1; echo -e "\nAbort $RUN_PREFIX: Regression tests failed (exit code $code)"; tput sgr 0
       echo
       exit $code
     fi;
 
   fi; #$RUN_REG_TESTS
 
+  #Create Coverage Reports ----------------------------------------------
+  cd $ROOT_DIR
+
+  if [ "$RUN_COV_TESTS" = true ]; then
+
+    # Merge MPI coverage data for all ranks from regression tests and create xml report in sub-dir
+    cd $ROOT_DIR/$COV_MERGE_DIR
+    cov_files=""
+
+    if [ "$RUN_UNIT_TESTS" = true ]; then
+      covfile="$ROOT_DIR/$UNIT_TEST_SUBDIR/.cov_unit_out"; [ -f ${covfile}  ] && cp $covfile .; cov_files="${cov_files} $covfile"
+      covfile="$ROOT_DIR/$UNIT_TEST_NOMPI_SUBDIR/.cov_unit_out2"; [ -f ${covfile}  ] && cp $covfile .; cov_files="${cov_files} $covfile"
+      covfile="$ROOT_DIR/$UNIT_TEST_LOGGER_SUBDIR/.cov_unit_out3"; [ -f ${covfile}  ] && cp $covfile .; cov_files="${cov_files} $covfile"
+      covfile="$ROOT_DIR/$UNIT_TEST_MPI_SUBDIR/.cov_unit_out4"; [ -f ${covfile}  ] && cp $covfile .; cov_files="${cov_files} $covfile"
+    fi;
+
+    if [ "$RUN_REG_TESTS" = true ]; then
+      for DIR in $REG_TEST_SUBDIR $FUNC_TEST_SUBDIR
+      do
+        cd $ROOT_DIR/$DIR
+        coverage combine .cov_reg_out* # Name of coverage data file must match that in .coveragerc in reg test dir.
+        coverage xml
+        echo -e "..Coverage xml written to dir $DIR/cov_reg/"
+      done
+      cd $ROOT_DIR/$COV_MERGE_DIR
+      covfile="$ROOT_DIR/$REG_TEST_SUBDIR/.cov_reg_out"; [ -f ${covfile}  ] && cp $covfile .; cov_files="${cov_files} $covfile"
+      covfile="$ROOT_DIR/$FUNC_TEST_SUBDIR/.cov_reg_out2"; [ -f ${covfile}  ] && cp $covfile .; cov_files="${cov_files} $covfile"
+    fi;
+
+    # Should create .cov_merge_out - see .coveragerc
+    if [ ! -z "cov_files" ]; then
+      coverage combine ${cov_files}
+      coverage xml # Should create cov_merge/ dir
+      echo -e "..Combined Test Coverage xml written to dir $COV_MERGE_DIR/cov_merge/"
+    fi;
+  fi;
+
   # Run Code standards Tests -----------------------------------------
   cd $ROOT_DIR
   if [ "$RUN_PEP_TESTS" = true ]; then
     tput bold; tput setaf 6
     echo -e "\n$RUN_PREFIX --$PYTHON_RUN: Running PEP tests - All python src below $PEP_SCOPE"
     tput sgr 0
     pytest --$PYTHON_PEP_STANDARD $ROOT_DIR/$PEP_SCOPE
```

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/define_apps.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/define_apps.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/forces_simf.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/readme.md` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/run_libe_forces_balsam.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/run_libe_forces_balsam.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/balsam_forces/submit_libe_forces_remotely.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/balsam_forces/submit_libe_forces_remotely.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/forces.yaml` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/forces.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/forces_support.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/readme.md` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_adv/run_libe_forces_from_yaml.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/build_forces.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/forces.c` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/forces.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/build_forces.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/mini_forces/mini_forces_AoS.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_app/readme.md` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_app/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/readme.md` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu/run_libe_forces.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/forces_simf.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/readme.md` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/run_libe_forces.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_gpu_var_resources/run_libe_forces.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_multi_app/forces_simf.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_multi_app/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_multi_app/run_libe_forces.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_multi_app/run_libe_forces.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_simple/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_simple/readme.md` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_simple/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/forces_simple/run_libe_forces.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/forces_simple/run_libe_forces.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/forces_simf.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/forces_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/globus_compute_forces.yaml` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/globus_compute_forces.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/globus_compute_forces/readme.md` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/globus_compute_forces/readme.md`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/forces/submission_scripts/summit_submit_mproc.sh` & `libensemble-1.3.0/libensemble/tests/scaling_tests/forces/submission_scripts/summit_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/persistent_gp/run_example.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/persistent_gp/run_example.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/all_machine_specs.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/all_machine_specs.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/plot_results.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/plot_results.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/read_sim_output.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/read_sim_output.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/readme.txt` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/run_libensemble_on_warpx.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/sim/inputs` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/sim/inputs`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/summit_submit_mproc.sh` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/summit_submit_mproc.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/warpx_simf.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/warpx_simf.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/scaling_tests/warpx/write_sim_input.py` & `libensemble-1.3.0/libensemble/tests/scaling_tests/warpx/write_sim_input.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/comms_test/commtest.py` & `libensemble-1.3.0/libensemble/tests/standalone_tests/comms_test/commtest.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/comms_test/readme.txt` & `libensemble-1.3.0/libensemble/tests/standalone_tests/comms_test/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/burn_time.c` & `libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/burn_time.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/killtest.py` & `libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/killtest.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/log.autotest.txt` & `libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/log.autotest.txt`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/log.burn_time_test_with_top.txt` & `libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/log.burn_time_test_with_top.txt`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/readme.txt` & `libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/kill_test/sleep_and_print.c` & `libensemble-1.3.0/libensemble/tests/standalone_tests/kill_test/sleep_and_print.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/mpi_launch_test/create_mpi_jobs.py` & `libensemble-1.3.0/libensemble/tests/standalone_tests/mpi_launch_test/create_mpi_jobs.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/mpi_launch_test/readme.txt` & `libensemble-1.3.0/libensemble/tests/standalone_tests/mpi_launch_test/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/readme.txt` & `libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/readme.txt`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/run/forces.c` & `libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/run/forces.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/standalone_tests/node_concurrency_test/run/run_timing_study.sh` & `libensemble-1.3.0/libensemble/tests/standalone_tests/node_concurrency_test/run/run_timing_study.sh`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/conftest.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/setup.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/setup.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/borehole.c` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/borehole.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/my_serialtask.c` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/my_serialtask.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/my_simtask.c` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/my_simtask.c`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/my_simtask.f90` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/my_simtask.f90`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example.json` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example.json`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example.toml` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example.toml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example.yaml` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml` & `libensemble-1.3.0/libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_allocation_funcs_and_support.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_allocation_funcs_and_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,33 @@
 from libensemble.history import History
 from libensemble.message_numbers import EVAL_GEN_TAG, EVAL_SIM_TAG
 from libensemble.resources.resources import Resources
 from libensemble.resources.scheduler import InsufficientResourcesError, ResourceScheduler
 from libensemble.tools import add_unique_random_streams
 from libensemble.tools.alloc_support import AllocException, AllocSupport
 from libensemble.tools.fields_keys import libE_fields
+from libensemble.utils.misc import _WorkerIndexer
 
 al = {"alloc_f": give_sim_work_first}
 libE_specs = {"comms": "local", "nworkers": 4}
 H0 = []
 
 W = np.array(
-    [(1, 0, 0, 0, False), (2, 0, 0, 0, False), (3, 0, 0, 0, False), (4, 0, 0, 0, False)],
+    [
+        (1, False, 0, 0, False, False),
+        (2, False, 0, 0, False, False),
+        (3, False, 0, 0, False, False),
+        (4, False, 0, 0, False, False),
+    ],
     dtype=[
         ("worker_id", "<i8"),
+        ("gen_worker", "?"),
         ("active", "<i8"),
         ("persis_state", "<i8"),
-        ("active_recv", "<i8"),
+        ("active_recv", "?"),
         ("zero_resource_worker", "?"),
     ],
 )
 
 fields = [("x", "<f8", 2), ("priority", "<f8")]
 H = np.zeros(5, dtype=libE_fields + fields)
 H[["gen_worker", "priority"]] = 1
@@ -95,60 +102,52 @@
 
 
 def test_als_worker_ids():
     als = AllocSupport(W, True)
     assert als.avail_worker_ids() == [1, 2, 3, 4], "avail_worker_ids() didn't return expected available worker list."
 
     W_ps = W.copy()
-    W_ps["persis_state"] = np.array([2, 0, 0, 0])
+    W_ps["persis_state"] = np.array([EVAL_GEN_TAG, 0, 0, 0])
     als = AllocSupport(W_ps, True)
-    assert als.avail_worker_ids(persistent=2) == [
+    assert als.avail_worker_ids(persistent=EVAL_GEN_TAG) == [
         1
     ], "avail_worker_ids() didn't return expected persistent worker list."
 
     W_ar = W.copy()
-    W_ar["active_recv"] = np.array([1, 0, 0, 0])
-    W_ar["persis_state"] = np.array([2, 0, 0, 0])
+    W_ar["active_recv"] = np.array([True, 0, 0, 0])
+    W_ar["persis_state"] = np.array([EVAL_GEN_TAG, 0, 0, 0])
     als = AllocSupport(W_ar, True)
-    assert als.avail_worker_ids(persistent=2, active_recv=True) == [
+    assert als.avail_worker_ids(persistent=EVAL_GEN_TAG, active_recv=True) == [
         1
     ], "avail_worker_ids() didn't return expected persistent worker list."
 
     flag = 1
     try:
         als.avail_worker_ids(active_recv=True)
     except AllocException:
         flag = 0
     assert flag == 0, "AllocSupport didn't error on invalid options for avail_worker_ids()"
 
-    W_ar = W.copy()
-    W_ar["active_recv"] = np.array([1, 0, 0, 0])
-    W_ar["persis_state"] = np.array([2, 0, 0, 0])
-    als = AllocSupport(W_ar, True)
-    assert als.avail_worker_ids(persistent=EVAL_GEN_TAG, active_recv=True) == [
-        1
-    ], "avail_worker_ids() didn't return expected persistent worker list."
-
     W_zrw = W.copy()
-    W_zrw["zero_resource_worker"] = np.array([1, 0, 0, 0])
+    W_zrw["zero_resource_worker"] = np.array([True, 0, 0, 0])
     als = AllocSupport(W_zrw, True)
     assert als.avail_worker_ids(zero_resource_workers=True) == [
         1
     ], "avail_worker_ids() didn't return expected zero resource worker list."
 
 
 def test_als_evaluate_gens():
     W_gens = W.copy()
-    W_gens["active"] = np.array([2, 0, 2, 0])
+    W_gens["active"] = np.array([EVAL_GEN_TAG, 0, EVAL_GEN_TAG, 0])
     als = AllocSupport(W_gens, True)
     assert als.count_gens() == 2, "count_gens() didn't return correct number of active generators"
 
     assert als.test_any_gen(), "test_any_gen() didn't return True on a generator worker being active."
 
-    W_gens["persis_state"] = np.array([2, 0, 0, 0])
+    W_gens["persis_state"] = np.array([EVAL_GEN_TAG, 0, 0, 0])
 
     assert (
         als.count_persis_gens() == 1
     ), "count_persis_gens() didn't return correct number of active persistent generators"
 
 
 def test_als_sim_work():
@@ -167,16 +166,17 @@
     ], "rset_team should not be defined if Resources hasn't been initialized?"
 
     assert all(
         [i in Work[1]["libE_info"]["H_rows"] for i in np.array([0, 1, 2, 3, 4])]
     ), "H_rows weren't assigned to libE_info correctly."
 
     W_ps = W.copy()
-    W_ps["persis_state"] = np.array([1, 0, 0, 0])
-    als = AllocSupport(W_ps, True)
+    W_ps["persis_state"] = np.array([EVAL_GEN_TAG, 0, 0, 0])
+    W_ps["zero_resource_worker"] = np.array([True, 0, 0, 0])
+    als = AllocSupport(_WorkerIndexer(W_ps, False), True)
     Work = {}
     Work[1] = als.sim_work(1, H, ["x"], np.array([0, 1, 2, 3, 4]), persis_info[1], persistent=True)
 
     assert not len(Work[1]["libE_info"]["rset_team"]), "Resource set should be empty for persistent workers."
 
     initialize_resources()
     als = AllocSupport(W, True)
@@ -204,16 +204,16 @@
     ], "rset_team should not be defined if Resources hasn't been initialized?"
 
     assert all(
         [i in Work[1]["libE_info"]["H_rows"] for i in range(0, 5)]
     ), "H_rows weren't assigned to libE_info correctly."
 
     W_ps = W.copy()
-    W_ps["persis_state"] = np.array([2, 0, 0, 0])
-    als = AllocSupport(W_ps, True)
+    W_ps["persis_state"] = np.array([EVAL_GEN_TAG, 0, 0, 0])
+    als = AllocSupport(_WorkerIndexer(W_ps, False), True)
     Work = {}
     Work[1] = als.gen_work(1, ["sim_id"], range(0, 5), persis_info[1], persistent=True)
 
     assert not len(Work[1]["libE_info"]["rset_team"]), "Resource set should be empty for persistent workers."
 
     initialize_resources()
     persis_info["gen_resources"] = 1
```

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_comms.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_comms.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_ensemble.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_env_resources.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_env_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_executor.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,47 @@
 import socket
 import sys
 import time
 
 import pytest
 
 from libensemble.executors.executor import NOT_STARTED_STATES, Executor, ExecutorException, TimeoutExpired
+from libensemble.message_numbers import STOP_TAG, TASK_FAILED, UNSET_TAG
 from libensemble.resources.mpi_resources import MPIResourcesException
 
 NCORES = 1
 build_sims = ["my_simtask.c", "my_serialtask.c", "c_startup.c"]
 
 sim_app = "simdir/my_simtask.x"
 serial_app = "simdir/my_serialtask.x"
 c_startup = "simdir/c_startup.x"
 py_startup = "simdir/py_startup.py"
 non_existent_app = "simdir/non_exist.x"
 
+UNKNOWN_SIGNAL = 2000
+
+
+class FakeCommTag:
+    def mail_flag(self):
+        return True
+
+    def recv(self):
+        return STOP_TAG + 10, 101
+
+
+class FakeCommSignal:
+    def mail_flag(self):
+        return True
+
+    def recv(self):
+        return STOP_TAG, UNKNOWN_SIGNAL
+
+    def push_to_buffer(self, mtag, man_signal):
+        pass
+
 
 def setup_module(module):
     if platform.system() != "Windows":
         import mpi4py
 
         mpi4py.rc.initialize = False
     try:
@@ -95,14 +117,15 @@
     """Set up serial Executor"""
     from libensemble.executors.executor import Executor
 
     exctr = Executor()
     exctr.add_platform_info()
     exctr.register_app(full_path=c_startup, app_name="c_startup")
     exctr.register_app(full_path=py_startup, app_name="py_startup")
+    exctr.register_app(full_path=py_startup, app_name="py_startup", precedent="python")
 
 
 def setup_executor_noapp():
     """Set up an MPI Executor but do not register application"""
     from libensemble.executors.mpi_executor import MPIExecutor
 
     exctr = MPIExecutor()
@@ -135,15 +158,15 @@
     from mpi4py import MPI
 
     return "Open MPI" in MPI.get_vendor()
 
 
 # -----------------------------------------------------------------------------
 # The following would typically be in the user sim_func.
-def polling_loop(exctr, task, timeout_sec=1, delay=0.05):
+def polling_loop(exctr, task, timeout_sec=2, delay=0.05):
     """Iterate over a loop, polling for an exit condition"""
     start = time.time()
 
     while time.time() - start < timeout_sec:
         time.sleep(delay)
 
         # Check output file for error.
@@ -230,14 +253,16 @@
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     task.wait()
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
     task.wait()  # Already complete
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
+    err_code = task.exception()
+    assert err_code == 0, f"Expected error code 0. Returned {err_code}"
 
 
 def test_launch_and_wait_no_platform():
     """Test of launching and waiting on task with no platform setup
 
     The MPI runner should be set on first call to executor.
     """
@@ -261,17 +286,17 @@
     setup_executor()
     exctr = Executor.executor
     cores = NCORES
     args_for_sim = "sleep 5"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     try:
         task.wait(timeout=0.5)
-    except TimeoutExpired:
+    except TimeoutExpired as e:
         print(task)
-        print(TimeoutExpired)
+        print(e)
         assert not task.finished, "task.finished should be False. Returned " + str(task.finished)
         task.kill()
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "USER_KILLED", "task.state should be USER_KILLED. Returned " + str(task.state)
 
 
 def test_launch_wait_on_start():
@@ -460,14 +485,20 @@
     # Testing no procs_per_node (shouldn't fail)
     task = exctr.submit(calc_type="sim", num_nodes=1, num_procs=2, app_args=args_for_sim)
     assert 1
     task = polling_loop(exctr, task, timeout_sec=4, delay=0.05)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
 
+    # Test with jsrun - does not support machinefiles
+    with pytest.raises(MPIResourcesException):
+        task = exctr.submit(
+            calc_type="sim", machinefile=machinefilename, app_args=args_for_sim, mpi_runner_type="jsrun"
+        )
+
 
 @pytest.mark.timeout(20)
 def test_doublekill():
     """Test attempt to kill already killed task.
 
     Kill should have no effect (except warning message) and should remain in state killed.
     """
@@ -642,14 +673,40 @@
     args_for_sim = "sleep 1.0 Fail"
     task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
     task = polling_loop(exctr, task, timeout_sec=3)
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FAILED", "task.state should be FAILED. Returned " + str(task.state)
 
 
+def test_task_failure_polling_loop_method():
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
+    setup_executor()
+    exctr = Executor.executor
+    cores = NCORES
+    args_for_sim = "sleep 1.0 Fail"
+    task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim)
+    calc_status = exctr.polling_loop(task)
+    assert task.finished, "task.finished should be True. Returned " + str(task.finished)
+    assert task.state == "FAILED", "task.state should be FAILED. Returned " + str(task.state)
+    assert calc_status == TASK_FAILED, f"calc_status should be {TASK_FAILED}"
+
+
+def test_task_unknown_state():
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
+    setup_executor()
+    exctr = Executor.executor
+    cores = NCORES
+    args_for_sim = "sleep 1.0"
+    task = exctr.submit(calc_type="sim", num_procs=cores, app_args=args_for_sim, dry_run=True)
+    task.state = "unknown"
+    calc_status = exctr.polling_loop(task)
+    assert task.finished, "task.finished should be True. Returned " + str(task.finished)
+    assert calc_status == UNSET_TAG, f"calc_status should be {UNSET_TAG}. Found {calc_status}"
+
+
 def test_retries_launch_fail():
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor_fakerunner()
     exctr = Executor.executor
     exctr.retry_delay_incr = 0.05
     cores = NCORES
     args_for_sim = "sleep 0"
@@ -727,24 +784,59 @@
     except ExecutorException as e:
         assert e.args[0] == "Application fake_app4 not found in registry"
         # Ordering of dictionary may vary
         # assert e.args[1] == "Registered applications: ['my_simtask.x', 'fake_app1', 'fake_app2']"
 
 
 def test_serial_exes():
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_serial_executor()
     exctr = Executor.executor
     args_for_sim = "sleep 0.1"
     task = exctr.submit(calc_type="sim", app_args=args_for_sim, wait_on_start=True)
     task.wait()
     assert task.finished, "task.finished should be True. Returned " + str(task.finished)
     assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
 
 
+def test_serial_exe_exception():
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
+    setup_serial_executor()
+    exctr = Executor.executor
+    with pytest.raises(ExecutorException):
+        exctr.submit()
+        pytest.fail("Expected exception")
+
+
+def test_serial_exe_env_script():
+    env_script_path = os.path.join(os.getcwd(), "./env_script_in.sh")
+    setup_serial_executor()
+    exctr = Executor.executor
+    args_for_sim = "sleep 0.1"
+    task = exctr.submit(calc_type="sim", app_args=args_for_sim, env_script=env_script_path)
+    task.wait()
+    # test env var should not exist here
+    assert "LIBE_TEST_SUB_ENV_VAR" not in os.environ
+
+
+def test_serial_exe_dryrun():
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
+    setup_serial_executor()
+    exctr = Executor.executor
+    exctr.set_gen_procs_gpus(libE_info={})
+    exctr.set_workerID(1)
+    args_for_sim = "sleep 0.1"
+    task = exctr.submit(calc_type="sim", app_args=args_for_sim, dry_run=True)
+    task.wait()
+    assert task.finished, "task.finished should be True. Returned " + str(task.finished)
+    assert task.state == "FINISHED", "task.state should be FINISHED. Returned " + str(task.state)
+
+
 def test_serial_startup_times():
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     setup_executor_startups()
     exctr = Executor.executor
 
     t1 = time.time()
     task = exctr.submit(app_name="c_startup")
     task.wait()
     stime = float(task.read_stdout())
@@ -802,14 +894,16 @@
     task.kill()
 
 
 def test_non_existent_app():
     """Tests exception on non-existent app"""
     from libensemble.executors.executor import Executor
 
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
+
     exctr = Executor()
 
     # Can register a non-existent app in case created as part of workflow.
     exctr.register_app(full_path=non_existent_app, app_name="nonexist")
 
     w_exctr = Executor.executor  # simulate on worker
 
@@ -821,14 +915,16 @@
         assert 0
 
 
 def test_non_existent_app_mpi():
     """Tests exception on non-existent app"""
     from libensemble.executors.mpi_executor import MPIExecutor
 
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
+
     exctr = MPIExecutor()
 
     # Can register a non-existent app in case created as part of workflow.
     exctr.register_app(full_path=non_existent_app, app_name="nonexist")
 
     w_exctr = Executor.executor  # simulate on worker
 
@@ -836,14 +932,31 @@
         w_exctr.submit(app_name="nonexist")
     except ExecutorException as e:
         assert e.args[0] == "Application does not exist simdir/non_exist.x"
     else:
         assert 0
 
 
+def test_man_signal_unrec_tag():
+    print(f"\nTest: {sys._getframe().f_code.co_name}\n")
+
+    setup_serial_executor()
+    exctr = Executor.executor
+
+    fake_comm1 = FakeCommTag()
+    exctr.comm = fake_comm1
+    man_signal = exctr.manager_poll()
+    assert man_signal is None, "manager_poll should have returned None"
+
+    fake_comm2 = FakeCommSignal()
+    exctr.comm = fake_comm2
+    man_signal = exctr.manager_poll()
+    assert man_signal == UNKNOWN_SIGNAL, f"manager_poll should have returned {UNKNOWN_SIGNAL}. Received {man_signal}"
+
+
 if __name__ == "__main__":
     setup_module(__file__)
     test_launch_and_poll()
     test_launch_and_wait()
     test_launch_and_wait_no_platform()
     test_launch_and_wait_timeout()
     test_launch_wait_on_start()
@@ -857,19 +970,25 @@
     test_finish_and_kill()
     test_launch_and_kill()
     test_launch_as_gen()
     test_launch_no_app()
     test_kill_task_with_no_submit()
     test_poll_task_with_no_submit()
     test_task_failure()
+    test_task_failure_polling_loop_method()
+    test_task_unknown_state()
     test_retries_launch_fail()
     test_retries_before_polling_loop_method()
     test_retries_run_fail()
     test_register_apps()
     test_serial_exes()
+    test_serial_exe_exception()
+    test_serial_exe_env_script()
+    test_serial_exe_dryrun()
     test_serial_startup_times()
     test_futures_interface()
     test_futures_interface_cancel()
     test_dry_run()
     test_non_existent_app()
     test_non_existent_app_mpi()
+    test_man_signal_unrec_tag()
     teardown_module(__file__)
```

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_executor_balsam.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_executor_balsam.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_executor_gpus.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_executor_gpus.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_history.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_history.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_launcher.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_loc_stack.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_loc_stack.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_manager_main.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_manager_main.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_models.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_models.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_node_resources.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_node_resources.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,80 +18,75 @@
 
 
 def teardown_function(function):
     print(f"teardown_function    function:{function.__name__}")
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = ""
 
 
+def setup_env_resources(target_resource):
+    """Set up environment resources"""
+    default_value = "THIS_ENV_VARIABLE_IS_DEF_NOT_SET"
+    resource_values = {
+        "nodelist_env_slurm": default_value,
+        "nodelist_env_cobalt": default_value,
+        "nodelist_env_pbs": default_value,
+        "nodelist_env_lsf": default_value,
+        "nodelist_env_lsf_shortform": default_value,
+    }
+    resource_values[target_resource] = "LIBE_RESOURCES_TEST_NODE_LIST"
+    env_resources = EnvResources(**resource_values)
+    return env_resources
+
+
 # Tests ========================================================================================
 
 
 def test_get_cpu_resources_from_env_empty():
     # Test empty call
     cores_info = node_resources._get_cpu_resources_from_env()
     assert cores_info is None, "cores_info should be None"
 
 
 def test_get_cpu_resources_from_env_lsf():
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = "batch5" + " g06n02" * 42
     exp_out = (42, 42)
-
-    env_resources1 = EnvResources(
-        nodelist_env_slurm="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_cobalt="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_lsf="LIBE_RESOURCES_TEST_NODE_LIST",
-        nodelist_env_lsf_shortform="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-    )
+    env_resources1 = setup_env_resources("nodelist_env_lsf")
     cores_info = node_resources._get_cpu_resources_from_env(env_resources=env_resources1)
     assert cores_info == exp_out, "cores_info returned does not match expected"
 
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = "batch5" + " g06n02" * 42 + " h21n18" * 42
-    env_resources2 = EnvResources(
-        nodelist_env_slurm="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_cobalt="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_lsf="LIBE_RESOURCES_TEST_NODE_LIST",
-        nodelist_env_lsf_shortform="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-    )
+    env_resources2 = setup_env_resources("nodelist_env_lsf")
     cores_info = node_resources._get_cpu_resources_from_env(env_resources=env_resources2)
     assert cores_info == exp_out, "cores_info returned does not match expected"
 
 
+def test_get_cpu_resources_from_env_lsf_diff_cores():
+    exp_out = (41, 41)
+    os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = "batch5" + " g06n02" * 42 + " h21n18" * 41
+    env_resources = setup_env_resources("nodelist_env_lsf")
+    cores_info = node_resources._get_cpu_resources_from_env(env_resources=env_resources)
+    assert cores_info == exp_out, "cores_info returned does not match expected"
+
+
 def test_get_cpu_resources_from_env_lsf_shortform():
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = "batch5 1 g06n02 42"
     exp_out = (42, 42)
-
-    env_resources1 = EnvResources(
-        nodelist_env_slurm="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_cobalt="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_lsf="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_lsf_shortform="LIBE_RESOURCES_TEST_NODE_LIST",
-    )
+    env_resources1 = setup_env_resources("nodelist_env_lsf_shortform")
     cores_info = node_resources._get_cpu_resources_from_env(env_resources=env_resources1)
     assert cores_info == exp_out, "cores_info returned does not match expected"
 
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = "batch5 1 g06n02 42 h21n18 42"
-    env_resources2 = EnvResources(
-        nodelist_env_slurm="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_cobalt="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_lsf="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_lsf_shortform="LIBE_RESOURCES_TEST_NODE_LIST",
-    )
+    env_resources2 = setup_env_resources("nodelist_env_lsf_shortform")
     cores_info = node_resources._get_cpu_resources_from_env(env_resources=env_resources2)
     assert cores_info == exp_out, "cores_info returned does not match expected"
 
 
 def test_get_cpu_resources_from_env_unknown_env():
     os.environ["LIBE_RESOURCES_TEST_NODE_LIST"] = "knl-[0009-0012]"
-    env_resources = EnvResources(
-        nodelist_env_slurm="LIBE_RESOURCES_TEST_NODE_LIST",
-        nodelist_env_cobalt="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_lsf="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-        nodelist_env_lsf_shortform="THIS_ENV_VARIABLE_IS_DEF_NOT_SET",
-    )
-
+    env_resources = setup_env_resources("nodelist_env_slurm")
     cores_info = node_resources._get_cpu_resources_from_env(env_resources=env_resources)
     assert cores_info is None, "cores_info should be None"
 
 
 def test_complete_set():
     assert not node_resources._complete_set([None, None, None])
     assert not node_resources._complete_set([2, None, 5])
@@ -123,20 +118,25 @@
 
 def test_update_from_str():
     result = node_resources._update_from_str([None, 2, 3], "11 12 13")
     assert result == [11, 12, 3], f"Unexpected result {result}"
     result = node_resources._update_from_str([1, 2, None], "11 12 13")
     assert result == [1, 2, 13], f"Unexpected result {result}"
 
+    # String is not an integer
+    result = node_resources._update_from_str([None, 2, 3], "Nope 12 13")
+    assert result == [None, 2, 3], f"Unexpected result {result}"
+
 
 if __name__ == "__main__":
     setup_standalone_run()
 
     test_get_cpu_resources_from_env_empty()
     test_get_cpu_resources_from_env_lsf()
+    test_get_cpu_resources_from_env_lsf_diff_cores()
     test_get_cpu_resources_from_env_lsf_shortform()
     test_get_cpu_resources_from_env_unknown_env()
     test_complete_set()
     test_cpu_info_complete()
     test_gpu_info_complete()
     test_update_values()
     test_update_from_str()
```

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_persistent_aposmm.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_persistent_aposmm.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_platform.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
+from libensemble.resources.platforms import Known_platforms, PlatformException, get_platform, known_system_detect
 from libensemble.utils.misc import specs_dump
-from libensemble.resources.platforms import PlatformException, get_platform, known_system_detect
-from libensemble.resources.platforms import Known_platforms
 
 my_spec = {
     "mpi_runner": "srun",
     "gpus_per_node": 4,
     "cores_per_node": 32,
 }
 
@@ -88,17 +87,15 @@
     name = known_system_detect(cmd=get_sys_cmd)
     platform_info = known_platforms[name]
     assert platform_info == summit_spec, f"Summit spec does not match expected ({platform_info})"
 
     # Try unknown system
     get_sys_cmd = "echo madeup.system"  # Overrides default "hostname -d"
     name = known_system_detect(cmd=get_sys_cmd)
-    assert (
-        name is None
-    ), f"Expected known_system_detect to return None ({name})"
+    assert name is None, f"Expected known_system_detect to return None ({name})"
 
 
 if __name__ == "__main__":
     test_platform_empty()
     test_unknown_platform()
     test_platform_known()
     test_platform_specs()
```

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_resource_scheduler.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_resource_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,48 +23,48 @@
         self.num_groups = num_groups
         self.rsets_per_node = self.total_num_rsets // num_groups
         self.gpu_rsets_per_node = min(gpus_per_node, self.rsets_per_node)
         self.nongpu_rsets_per_node = self.rsets_per_node - self.gpu_rsets_per_node
 
         self.even_groups = True
         self.rsets = np.zeros(self.total_num_rsets, dtype=MyResources.rset_dtype)
-        self.rsets["assigned"] = 0
+        self.rsets["assigned"] = -1
         for i in range(self.total_num_rsets):
             self.rsets["group"][i] = i // self.rsets_per_node
             self.rsets["slot"][i] = i % self.rsets_per_node
             self.rsets["gpus"][i] = self.rsets["slot"][i] < gpus_per_node
         self.rsets_free = self.total_num_rsets
         self.total_num_gpu_rsets = np.count_nonzero(self.rsets["gpus"])
         self.total_num_nongpu_rsets = np.count_nonzero(~self.rsets["gpus"])
 
         self.gpu_rsets_free = self.total_num_gpu_rsets
         self.nongpu_rsets_free = self.total_num_nongpu_rsets
 
     def free_rsets(self, worker=None):
         """Free up assigned resource sets"""
         if worker is None:
-            self.rsets["assigned"] = 0
+            self.rsets["assigned"] = -1
             self.rsets_free = self.total_num_rsets
         else:
             for rset, wid in enumerate(self.rsets["assigned"]):
                 if wid == worker:
-                    self.rsets["assigned"][rset] = 0
+                    self.rsets["assigned"][rset] = -1
                     self.rsets_free += 1
 
     def assign_rsets(self, rset_team, worker_id):
         """Mark the resource sets given by rset_team as assigned to worker_id"""
         if rset_team:
             self.rsets["assigned"][rset_team] = worker_id
             self.rsets_free -= len(rset_team)  # quick count
 
     # Special function for testing from a given starting point
     def fixed_assignment(self, assignment):
         """Set the given assignment along with other coupled information"""
         self.rsets["assigned"] = assignment
-        self.rsets_free = np.count_nonzero(self.rsets["assigned"] == 0)
+        self.rsets_free = np.count_nonzero(self.rsets["assigned"] == -1)
 
 
 def _fail_to_resource(sched, rsets, use_gpus=None):
     with pytest.raises(InsufficientFreeResources):
         rset_team = sched.assign_resources(rsets_req=rsets, use_gpus=use_gpus)
         pytest.fail(f"Expected InsufficientFreeResources. Found {rset_team}")
 
@@ -140,15 +140,15 @@
     del resources
 
 
 def test_cannot_split_quick_return():
     """Tests the quick return when splitting finds no free even gaps"""
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(6, 3)
-    resources.fixed_assignment(([1, 0, 0, 0, 3, 3]))
+    resources.fixed_assignment(([1, -1, -1, -1, 3, 3]))
     sched = ResourceScheduler(user_resources=resources)
     _fail_to_resource(sched, 3)
 
 
 def test_schedule_find_gaps_1node():
     """Tests assignment of rsets on one node.
 
@@ -173,15 +173,15 @@
             # Check not enough slots
             _fail_to_resource(sched, 4)
 
             rset_team = sched.assign_resources(rsets_req=2)
             assert rset_team == [5, 6]
 
             # Simulate resources freed up on return from worker
-            resources.fixed_assignment(([3, 3, 0, 0, 0, 4, 4, 0]))
+            resources.fixed_assignment(([3, 3, -1, -1, -1, 4, 4, -1]))
 
             # Create new scheduler to simulate new alloc call
             del sched
             rset_team = None
             sched = ResourceScheduler(user_resources=resources)
 
             rset_team = sched.assign_resources(rsets_req=4)
@@ -215,15 +215,15 @@
 
 def test_split_across_no_matching_slots():
     """Must split across - but no split2fit and no matching slots"""
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(6, 3)  # 3 nodes of 2 slots
 
     for split2fit in [False, True]:
-        resources.fixed_assignment(([0, 1, 1, 0, 0, 1]))
+        resources.fixed_assignment(([-1, 1, 1, -1, -1, 1]))
         sched_options = {"split2fit": split2fit}
         sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
         _fail_to_resource(sched, 3)
 
         sched.match_slots = False
         rset_team = sched.assign_resources(rsets_req=3)
         assert rset_team == [0, 3, 4], f"rset_team is {rset_team}."
@@ -325,18 +325,18 @@
 
 def test_try1node_findon_2nodes_matching_slots():
     """Tests finding gaps on two nodes with matching slots"""
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
 
     fixed_assignments = [
-        ([1, 1, 0, 0, 3, 3, 0, 0]),
-        ([0, 1, 0, 2, 0, 4, 0, 4]),
-        ([0, 1, 1, 0, 0, 2, 2, 0]),
-        ([1, 0, 1, 0, 3, 0, 3, 0]),
+        ([1, 1, -1, -1, 3, 3, -1, -1]),
+        ([-1, 1, -1, 2, -1, 4, -1, 4]),
+        ([-1, 1, 1, -1, -1, 2, 2, -1]),
+        ([1, -1, 1, -1, 3, -1, 3, -1]),
     ]
     exp_out = [[2, 3, 6, 7], [0, 2, 4, 6], [0, 3, 4, 7], [1, 3, 5, 7]]
 
     for i, assgn in enumerate(fixed_assignments):
         resources.fixed_assignment(assgn)
 
         # match_slots should make no difference
@@ -354,17 +354,17 @@
 
 def test_try1node_findon_2nodes_different_slots():
     """Tests finding gaps on two nodes with non-matching slots"""
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
 
     fixed_assignments = [
-        ([1, 1, 0, 0, 0, 2, 2, 0]),
-        ([1, 1, 0, 0, 0, 0, 3, 3]),
-        ([1, 0, 0, 1, 0, 3, 0, 3]),
+        ([1, 1, -1, -1, -1, 2, 2, -1]),
+        ([1, 1, -1, -1, -1, -1, 3, 3]),
+        ([1, -1, -1, 1, -1, 3, -1, 3]),
     ]
     exp_out = [[2, 3, 4, 7], [2, 3, 4, 5], [1, 2, 4, 6]]
 
     for i, assgn in enumerate(fixed_assignments):
         resources.fixed_assignment(assgn)
         sched = ResourceScheduler(user_resources=resources)
 
@@ -386,15 +386,15 @@
     del resources
 
 
 def test_try1node_findon_3nodes():
     """Tests finding gaps on two nodes as cannot fit on one due to others assigned"""
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(12, 3)
-    resources.fixed_assignment(([1, 1, 0, 0, 0, 2, 2, 0, 3, 0, 3, 3]))
+    resources.fixed_assignment(([1, 1, -1, -1, -1, 2, 2, -1, 3, -1, 3, 3]))
     sched = ResourceScheduler(user_resources=resources)
 
     # Default - with match_slots - cannot find a split with matching slots
     _fail_to_resource(sched, 3)
 
     # Can find non-matching slots across three nodes
     sched_options = {"match_slots": False}
@@ -440,15 +440,15 @@
     rset ID:     0  1  2  3  4  5   6  7  8  9  10 11   12 13 14 15 16 17
     slots ID:    0  1  2  3  4  5   0  1  2  3  4  5    0  1  2  3  4  5
     assigned:    0  1  0  0  0  0   0  0  0  0  0  0    0  0  0  0  0  0
 
     """
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(18, 3)
-    resources.fixed_assignment(([0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 3]))
+    resources.fixed_assignment(([-1, 1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, 3]))
     sched = ResourceScheduler(user_resources=resources)
 
     # Can't find 2 groups of 6 so find 3 groups of 4 - with matching slots.
     rset_team = sched.assign_resources(rsets_req=12)
     assert rset_team == [0, 2, 3, 4, 6, 8, 9, 10, 12, 14, 15, 16], f"rsets found {rset_team}"
 
     # Without matching slots, will find first available slots on each node.
@@ -483,28 +483,28 @@
     del resources
 
 
 def test_split2fit_even_required_fails():
     """Test tries one node then two, and both fail"""
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
-    resources.fixed_assignment(([1, 1, 1, 0, 2, 2, 0, 0]))
+    resources.fixed_assignment(([1, 1, 1, -1, 2, 2, -1, -1]))
 
     for match_slots in [False, True]:
         sched_options = {"match_slots": match_slots}
         sched = ResourceScheduler(user_resources=resources, sched_opts=sched_options)
         _fail_to_resource(sched, 4)
         assert sched.rsets_free == 3
 
 
 def test_split2fit_even_required_various():
     """Tests trying to fit to an non-even partition, and setting of local rsets_free"""
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(8, 2)
-    resources.fixed_assignment(([1, 1, 1, 0, 0, 0, 0, 0]))
+    resources.fixed_assignment(([1, 1, 1, -1, -1, -1, -1, -1]))
     sched = ResourceScheduler(user_resources=resources)
     assert sched.rsets_free == 5
 
     rset_team = sched.assign_resources(rsets_req=2)
     assert rset_team == [4, 5], f"rsets found {rset_team}"
     assert sched.rsets_free == 3
 
@@ -519,15 +519,15 @@
     assert sched.rsets_free == 1
 
 
 def test_try1node_findon_2_or_4nodes():
     """Tests splitting to fit. Needs 4 nodes if matching slots, else 2."""
     print(f"\nTest: {sys._getframe().f_code.co_name}\n")
     resources = MyResources(16, 4)
-    resources.fixed_assignment(([1, 1, 0, 1, 2, 2, 0, 0, 1, 0, 0, 1, 0, 4, 0, 4]))
+    resources.fixed_assignment(([1, 1, -1, 1, 2, 2, -1, -1, 1, -1, -1, 1, -1, 4, -1, 4]))
 
     sched = ResourceScheduler(user_resources=resources)
     rset_team = sched.assign_resources(rsets_req=4)
     assert rset_team == [2, 6, 10, 14], f"rsets found {rset_team}"
     del sched
     rset_team = None  # I think should always do between tests (esp if expected output is the same).
 
@@ -543,35 +543,35 @@
     rsets = resources.rsets
 
     # All slots filled
     rsets["assigned"] = 1
 
     # Now free up the one column
     col15 = rsets["slot"] == 15
-    rsets["assigned"][col15] = 0
+    rsets["assigned"][col15] = -1
 
     # Now make sure two rows (groups) with 8, but different slots
     free_row0 = (rsets["group"] == 0) & (rsets["slot"] < 8)
     free_row1 = (rsets["group"] == 1) & (rsets["slot"] >= 8)
 
     # Now make sure 4 rows of 4 exist (diff slots)
     free_row2 = (rsets["group"] == 2) & (rsets["slot"] < 4)
     free_row3 = (rsets["group"] == 3) & (rsets["slot"] >= 8) & (rsets["slot"] < 12)
 
     # Now make sure 8 rows of 2 exist (diff slots)
     # Free one slot each as last column already free
     free_strip = (rsets["group"] >= 12) & (rsets["slot"] == 3)
 
-    rsets["assigned"][free_row0] = 0
-    rsets["assigned"][free_row1] = 0
-    rsets["assigned"][free_row2] = 0
-    rsets["assigned"][free_row3] = 0
-    rsets["assigned"][free_strip] = 0
+    rsets["assigned"][free_row0] = -1
+    rsets["assigned"][free_row1] = -1
+    rsets["assigned"][free_row2] = -1
+    rsets["assigned"][free_row3] = -1
+    rsets["assigned"][free_strip] = -1
 
-    resources.free_rsets = np.count_nonzero(rsets["assigned"] == 0)
+    resources.free_rsets = np.count_nonzero(rsets["assigned"] == -1)
     # _print_assigned(resources)
 
 
 def test_large_match_slots():
     """Tests multiple match slots iterations
 
     Aim is try one of 16, then 2 of 8, then 4 or 4 and 8 or 2 then 16 of one.
```

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_resources.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_scipy.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_sim_dir_properties.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_sim_dir_properties.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_task_funcs.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_task_funcs.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_timer.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests/test_ufunc_runners.py` & `libensemble-1.3.0/libensemble/tests/unit_tests/test_ufunc_runners.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,127 @@
 import mock
 import numpy as np
 import pytest
 
 import libensemble.tests.unit_tests.setup as setup
-from libensemble.message_numbers import EVAL_GEN_TAG, EVAL_SIM_TAG
 from libensemble.tools.fields_keys import libE_fields
-from libensemble.utils.runners import Runners
+from libensemble.utils.runners import Runner
 
 
 def get_ufunc_args():
     sim_specs, gen_specs, exit_criteria = setup.make_criteria_and_specs_0()
 
     L = exit_criteria["sim_max"]
     H = np.zeros(L, dtype=list(set(libE_fields + sim_specs["out"] + gen_specs["out"])))
 
     H["sim_id"][-L:] = -1
     H["sim_started_time"][-L:] = np.inf
 
     sim_ids = np.zeros(1, dtype=int)
     Work = {
-        "tag": EVAL_SIM_TAG,
+        "tag": 1,
         "persis_info": {},
         "libE_info": {"H_rows": sim_ids},
         "H_fields": sim_specs["in"],
     }
     calc_in = H[Work["H_fields"]][Work["libE_info"]["H_rows"]]
     return calc_in, sim_specs, gen_specs
 
 
-@pytest.mark.extra
 def test_normal_runners():
     calc_in, sim_specs, gen_specs = get_ufunc_args()
 
-    runners = Runners(sim_specs, gen_specs)
-    assert (
-        not runners.has_globus_compute_sim and not runners.has_globus_compute_gen
+    simrunner = Runner(sim_specs)
+    genrunner = Runner(gen_specs)
+    assert not hasattr(simrunner, "globus_compute_executor") and not hasattr(
+        genrunner, "globus_compute_executor"
     ), "Globus Compute use should not be detected without setting endpoint fields"
 
-    ro = runners.make_runners()
-    assert all(
-        [i in ro for i in [EVAL_SIM_TAG, EVAL_GEN_TAG]]
-    ), "Both user function tags should be included in runners dictionary"
-
 
-@pytest.mark.extra
-def test_normal_no_gen():
+def test_thread_runners():
     calc_in, sim_specs, gen_specs = get_ufunc_args()
 
-    runners = Runners(sim_specs, {})
-    ro = runners.make_runners()
+    def tupilize(arg1, arg2):
+        return (arg1, arg2)
 
-    assert not ro[2], "generator function shouldn't be provided if not using gen_specs"
+    sim_specs["threaded"] = True  # TODO: undecided interface
+    sim_specs["sim_f"] = tupilize
+    persis_info = {"hello": "threads"}
+
+    simrunner = Runner(sim_specs)
+    result = simrunner._result(calc_in, persis_info, {})
+    assert result == (calc_in, persis_info)
+    assert hasattr(simrunner, "thread_handle")
+    simrunner.shutdown()
 
 
 @pytest.mark.extra
 def test_globus_compute_runner_init():
     calc_in, sim_specs, gen_specs = get_ufunc_args()
 
     sim_specs["globus_compute_endpoint"] = "1234"
 
     with mock.patch("globus_compute_sdk.Executor"):
-        runners = Runners(sim_specs, gen_specs)
+        runner = Runner(sim_specs)
 
-        assert (
-            runners.sim_globus_compute_executor is not None
+        assert hasattr(
+            runner, "globus_compute_executor"
         ), "Globus ComputeExecutor should have been instantiated when globus_compute_endpoint found in specs"
 
 
 @pytest.mark.extra
 def test_globus_compute_runner_pass():
     calc_in, sim_specs, gen_specs = get_ufunc_args()
 
     sim_specs["globus_compute_endpoint"] = "1234"
 
     with mock.patch("globus_compute_sdk.Executor"):
-        runners = Runners(sim_specs, gen_specs)
+        runner = Runner(sim_specs)
 
         #  Creating Mock Globus ComputeExecutor and Globus Compute future object - no exception
         globus_compute_mock = mock.Mock()
         globus_compute_future = mock.Mock()
         globus_compute_mock.submit_to_registered_function.return_value = globus_compute_future
         globus_compute_future.exception.return_value = None
         globus_compute_future.result.return_value = (True, True)
 
-        runners.sim_globus_compute_executor = globus_compute_mock
-        ro = runners.make_runners()
+        runner.globus_compute_executor = globus_compute_mock
+        runners = {1: runner.run}
 
         libE_info = {"H_rows": np.array([2, 3, 4]), "workerID": 1, "comm": "fakecomm"}
 
-        out, persis_info = ro[1](calc_in, {"libE_info": libE_info, "persis_info": {}, "tag": 1})
+        out, persis_info = runners[1](calc_in, {"libE_info": libE_info, "persis_info": {}, "tag": 1})
 
         assert all([out, persis_info]), "Globus Compute runner correctly returned results"
 
 
 @pytest.mark.extra
 def test_globus_compute_runner_fail():
     calc_in, sim_specs, gen_specs = get_ufunc_args()
 
     gen_specs["globus_compute_endpoint"] = "4321"
 
     with mock.patch("globus_compute_sdk.Executor"):
-        runners = Runners(sim_specs, gen_specs)
+        runner = Runner(gen_specs)
 
         #  Creating Mock Globus ComputeExecutor and Globus Compute future object - yes exception
         globus_compute_mock = mock.Mock()
         globus_compute_future = mock.Mock()
         globus_compute_mock.submit_to_registered_function.return_value = globus_compute_future
         globus_compute_future.exception.return_value = Exception
 
-        runners.gen_globus_compute_executor = globus_compute_mock
-        ro = runners.make_runners()
+        runner.globus_compute_executor = globus_compute_mock
+        runners = {2: runner.run}
 
         libE_info = {"H_rows": np.array([2, 3, 4]), "workerID": 1, "comm": "fakecomm"}
 
         with pytest.raises(Exception):
-            out, persis_info = ro[2](calc_in, {"libE_info": libE_info, "persis_info": {}, "tag": 2})
+            out, persis_info = runners[2](calc_in, {"libE_info": libE_info, "persis_info": {}, "tag": 2})
             pytest.fail("Expected exception")
 
 
 if __name__ == "__main__":
     test_normal_runners()
-    test_normal_no_gen()
+    test_thread_runners()
     test_globus_compute_runner_init()
     test_globus_compute_runner_pass()
     test_globus_compute_runner_fail()
```

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests_logger/test_logger.py` & `libensemble-1.3.0/libensemble/tests/unit_tests_logger/test_logger.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests_mpi_import/conftest.py` & `libensemble-1.3.0/libensemble/tests/unit_tests_mpi_import/conftest.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests_mpi_import/test_libE_main.py` & `libensemble-1.3.0/libensemble/tests/unit_tests_mpi_import/test_libE_main.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests_nompi/conftest.py` & `libensemble-1.3.0/libensemble/tests/unit_tests_nompi/conftest.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tests/unit_tests_nompi/test_aaa_comms.py` & `libensemble-1.3.0/libensemble/tests/unit_tests_nompi/test_aaa_comms.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tools/alloc_support.py` & `libensemble-1.3.0/libensemble/tools/alloc_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,32 +83,27 @@
                     return rset_team
                 except (InsufficientFreeResources, InsufficientResourcesError):
                     pass
 
             rset_team = self.sched.assign_resources(rsets_req, use_gpus, user_params)
         return rset_team
 
-    def avail_worker_ids(self, persistent=None, active_recv=False, zero_resource_workers=None):
+    def avail_worker_ids(self, persistent=None, active_recv=False, zero_resource_workers=None, gen_workers=None):
         """Returns available workers as a list of IDs, filtered by the given options.
 
         :param persistent: (Optional) Int. Only return workers with given ``persis_state`` (1=sim, 2=gen).
         :param active_recv: (Optional) Boolean. Only return workers with given active_recv state.
         :param zero_resource_workers: (Optional) Boolean. Only return workers that require no resources.
+        :param gen_workers: (Optional) Boolean. If True, return gen-only workers. If False, return all other workers.
         :returns: List of worker IDs.
 
         If there are no zero resource workers defined, then the ``zero_resource_workers`` argument will
         be ignored.
         """
 
-        def fltr(wrk, field, option):
-            """Filter by condition if supplied"""
-            if option is None:
-                return True
-            return wrk[field] == option
-
         # For abbrev.
         def fltr_persis():
             if persistent is None:
                 return True
             return wrk["persis_state"] == persistent
 
         def fltr_zrw():
@@ -117,34 +112,41 @@
                 return True
             return wrk["zero_resource_worker"] == zero_resource_workers
 
         def fltr_recving():
             if active_recv:
                 return wrk["active_recv"]
             else:
-                return not wrk["active"]
+                return wrk["active"] == 0
+
+        def fltr_gen_workers():
+            if no_gen_workers or gen_workers is None:
+                return True
+            return wrk["gen_worker"] == gen_workers
 
         if active_recv and not persistent:
             raise AllocException("Cannot ask for non-persistent active receive workers")
 
         # If there are no zero resource workers - then ignore zrw (i.e., use only if they exist)
         no_zrw = not any(self.W["zero_resource_worker"])
+        no_gen_workers = not any(self.W["gen_worker"])
+
         wrks = []
         for wrk in self.W:
-            if fltr_recving() and fltr_persis() and fltr_zrw():
+            if fltr_recving() and fltr_persis() and fltr_zrw() and fltr_gen_workers():
                 wrks.append(wrk["worker_id"])
         return wrks
 
     def count_gens(self):
         """Returns the number of active generators."""
-        return sum(self.W["active"] == EVAL_GEN_TAG)
+        return sum((self.W["active"] == EVAL_GEN_TAG))
 
     def test_any_gen(self):
         """Returns ``True`` if a generator worker is active."""
-        return any(self.W["active"] == EVAL_GEN_TAG)
+        return any((self.W["active"] == EVAL_GEN_TAG))
 
     def count_persis_gens(self):
         """Return the number of active persistent generators."""
         return sum(self.W["persis_state"] == EVAL_GEN_TAG)
 
     def _req_resources_sim(self, libE_info, user_params, H, H_rows):
         """Determine required resources for a sim work unit"""
@@ -197,15 +199,15 @@
                 num_rsets_req = max(num_rsets_req, num_rsets_req_for_gpus)
         return num_rsets_req, use_gpus
 
     def _update_rset_team(self, libE_info, wid, H=None, H_rows=None):
         """Add rset_team to libE_info."""
         if self.manage_resources and not libE_info.get("rset_team"):
             num_rsets_req = 0
-            if self.W[wid - 1]["persis_state"]:
+            if self.W[wid]["persis_state"]:
                 # Even if empty list, non-None rset_team stops manager giving default resources
                 libE_info["rset_team"] = []
                 return
             else:
                 user_params = []
                 # TODO - can't a gen have these (e.g. if have H0) - or if non-persistent
                 if H is not None and H_rows is not None:
@@ -268,15 +270,15 @@
 
         If ``rset_team`` is passed as an additional parameter, it will be honored, and assume that
         any resource checking has already been done. For example, passing ``rset_team=[]``, would
         ensure that no resources are assigned.
         """
         self._update_rset_team(libE_info, wid)
 
-        if not self.W[wid - 1]["persis_state"]:
+        if not self.W[wid]["persis_state"]:
             AllocSupport.gen_counter += 1  # Count total gens
             libE_info["gen_count"] = AllocSupport.gen_counter
 
         H_fields = AllocSupport._check_H_fields(H_fields)
         libE_info["H_rows"] = AllocSupport._check_H_rows(H_rows)
 
         work = {
```

### Comparing `libensemble-1.2.2/libensemble/tools/fields_keys.py` & `libensemble-1.3.0/libensemble/tools/fields_keys.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tools/forkable_pdb.py` & `libensemble-1.3.0/libensemble/tools/forkable_pdb.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tools/parse_args.py` & `libensemble-1.3.0/libensemble/tools/parse_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 parser = argparse.ArgumentParser(prog="test_...")
 
 parser.add_argument(
     "--comms",
     type=str,
     nargs="?",
     choices=["local", "threads", "tcp", "ssh", "client", "mpi"],
-    default="mpi",
     help="Type of communicator",
 )
-parser.add_argument("--nworkers", type=int, nargs="?", help="Number of local forked processes")
+parser.add_argument("-n", "--nworkers", type=int, nargs="?", help="Number of local forked processes")
 parser.add_argument(
     "--nsim_workers",
     type=int,
     nargs="?",
     help="Number of workers for sims. 1+ unresourced workers for a persistent generator will be added",
 )
 parser.add_argument("--nresource_sets", type=int, nargs="?", help="Number of resource sets")
@@ -181,31 +180,34 @@
                         [--worker_python [WORKER_PYTHON]]
                         [--tester_args [TESTER_ARGS [TESTER_ARGS ...]]]
 
         Note that running via an MPI runner uses the default 'mpi' comms, and '--nworkers'
         will be ignored. The number of processes are supplied via the MPI run line. One being
         the manager, and the rest are workers.
 
-        --comms,          Communications medium for manager and workers. Default is 'mpi'.
-        --nworkers,       (For 'local' or 'tcp' comms) Set number of workers.
+        --comms,          Communications medium for manager and workers.
+                          Default is 'local' if --nworkers is provided, otherwise  'mpi'.
+        --nworkers/-n,    (For 'local' or 'tcp' comms) Set number of workers.
         --nresource_sets, Explicitly set the number of resource sets. This sets
                           libE_specs["num_resource_sets"]. By default, resources will be
                           divided by workers (excluding zero_resource_workers).
         --nsim_workers,   (For 'local" or 'mpi' comms) A convenience option for cases with
                           persistent generators - sets the number of simulation workers.
                           If used with no other criteria, one additional worker for running a
                           generator will be added, and the number of resource sets will be assigned
                           the given value. If '--nworkers' has also been specified, will generate
                           enough additional workers to match the other criteria. If '--nresource_sets'
                           is also specified, will not override resource sets.
 
         Example command lines:
 
-        Run with 'local' comms and 4 workers
+        Run with 'local' comms and 4 workers (the following are equivalent).
         $ python calling_script --comms local --nworkers 4
+        $ python calling_script --nworkers 4
+        $ python calling_script -n 4
 
         Run with 'local' comms and 5 workers - one gen worker (no resources), and 4 sim workers.
         $ python calling_script --comms local --nsim_workers 4
 
         Run with 'local' comms with 4 workers and 8 resource sets. The extra resource sets will
         be used for larger simulations (using variable resource assignment).
         $ python calling_script --comms local --nresource_sets 8
@@ -224,14 +226,20 @@
 
     libE_specs: :obj:`dict`
         Settings and specifications for libEnsemble
         :doc:`(example)<data_structures/libE_specs>`
 
     """
     args, misc_args = parser.parse_known_args(sys.argv[1:])
+
+    # Assume local if nworkers is set.
+    if args.comms is None:
+        if args.nworkers is not None:
+            args.comms = "local"
+
     front_ends = {
         "mpi": _mpi_parse_args,
         "local": _local_parse_args,
         "threads": _local_parse_args,
         "tcp": _tcp_parse_args,
         "ssh": _ssh_parse_args,
         "client": _client_parse_args,
```

### Comparing `libensemble-1.2.2/libensemble/tools/persistent_support.py` & `libensemble-1.3.0/libensemble/tools/persistent_support.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tools/test_support.py` & `libensemble-1.3.0/libensemble/tools/test_support.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/tools/tools.py` & `libensemble-1.3.0/libensemble/tools/tools.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/utils/launcher.py` & `libensemble-1.3.0/libensemble/utils/launcher.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/utils/loc_stack.py` & `libensemble-1.3.0/libensemble/utils/loc_stack.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/utils/output_directory.py` & `libensemble-1.3.0/libensemble/utils/output_directory.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/utils/pydantic_bindings.py` & `libensemble-1.3.0/libensemble/utils/pydantic_bindings.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     check_provided_ufuncs,
     check_valid_comms_type,
     check_valid_in,
     check_valid_out,
     enable_save_H_when_every_K,
     genf_set_in_out_from_attrs,
     set_calc_dirs_on_input_dir,
+    set_default_comms,
     set_platform_specs_to_class,
     set_workflow_dir,
     simf_set_in_out_from_attrs,
 )
 
 if pydanticV1:
     from pydantic import BaseConfig
@@ -113,14 +114,15 @@
         __validators__={
             "check_valid_comms_type": check_valid_comms_type,
             "set_platform_specs_to_class": set_platform_specs_to_class,
             "check_input_dir_exists": check_input_dir_exists,
             "check_inputs_exist": check_inputs_exist,
             "check_any_workers_and_disable_rm_if_tcp": check_any_workers_and_disable_rm_if_tcp,
             "enable_save_H_when_every_K": enable_save_H_when_every_K,
+            "set_default_comms": set_default_comms,
             "set_workflow_dir": set_workflow_dir,
             "set_calc_dirs_on_input_dir": set_calc_dirs_on_input_dir,
         },
     )
 
     specs._EnsembleSpecs = create_model(
         "_EnsembleSpecs",
```

### Comparing `libensemble-1.2.2/libensemble/utils/specs_checkers.py` & `libensemble-1.3.0/libensemble/utils/specs_checkers.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/utils/timer.py` & `libensemble-1.3.0/libensemble/utils/timer.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/libensemble/utils/validators.py` & `libensemble-1.3.0/libensemble/utils/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from pathlib import Path
 from typing import Callable
 
 import numpy as np
 
 from libensemble.resources.platforms import Platform
 from libensemble.utils.misc import pydanticV1
@@ -17,14 +18,36 @@
 
 _UNRECOGNIZED_ERR = "Unrecognized field. Check closely for typos, or libEnsemble's docs"
 _UFUNC_INVALID_ERR = "Specified sim_f or gen_f is not callable. It should be a user function"
 _OUT_DTYPE_ERR = "unable to coerce into a NumPy dtype. It should be a list of 2-tuples or 3-tuples"
 _IN_INVALID_ERR = "value should be a list of field names (a list of strings)"
 
 
+def detect_comms_env():
+    """Return local or MPI comms based on env variables"""
+    mpi_vars = ["OMPI_COMM_WORLD_SIZE", "PMI_SIZE"]
+    comms_type = "local"
+    for var in mpi_vars:
+        value = os.getenv(var)
+        if value is not None:
+            if int(value) > 1:
+                comms_type = "mpi"
+                break
+    return comms_type
+
+
+def default_comms(values):
+    if "comms" not in values:
+        if values.get("nworkers") is not None:
+            values["comms"] = detect_comms_env()
+        else:
+            values["comms"] = "mpi"
+    return values
+
+
 def check_valid_out(cls, v):
     try:
         _ = np.dtype(v)
     except TypeError:
         raise ValueError(_OUT_DTYPE_ERR.format(v))
     else:
         return v
@@ -97,14 +120,18 @@
     check_mpi_runner_type = validator("mpi_runner")(check_mpi_runner_type)
 
     @root_validator
     def check_any_workers_and_disable_rm_if_tcp(cls, values):
         return _check_any_workers_and_disable_rm_if_tcp(values)
 
     @root_validator(pre=True)
+    def set_default_comms(cls, values):
+        return default_comms(values)
+
+    @root_validator(pre=True)
     def enable_save_H_when_every_K(cls, values):
         if "save_H_on_completion" not in values and (
             values.get("save_every_k_sims", 0) > 0 or values.get("save_every_k_gens", 0) > 0
         ):
             values["save_H_on_completion"] = True
         return values
 
@@ -191,14 +218,18 @@
     check_gpu_setting_type = field_validator("gpu_setting_type")(classmethod(check_gpu_setting_type))
     check_mpi_runner_type = field_validator("mpi_runner")(classmethod(check_mpi_runner_type))
 
     @model_validator(mode="after")
     def check_any_workers_and_disable_rm_if_tcp(self):
         return _check_any_workers_and_disable_rm_if_tcp(self)
 
+    @model_validator(mode="before")
+    def set_default_comms(cls, values):
+        return default_comms(values)
+
     @model_validator(mode="after")
     def enable_save_H_when_every_K(self):
         if not self.__dict__.get("save_H_on_completion") and (
             self.__dict__.get("save_every_k_sims", 0) > 0 or self.__dict__.get("save_every_k_gens", 0) > 0
         ):
             self.__dict__["save_H_on_completion"] = True
         return self
```

### Comparing `libensemble-1.2.2/libensemble/worker.py` & `libensemble-1.3.0/libensemble/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     calc_status_strings,
     calc_type_strings,
 )
 from libensemble.resources.resources import Resources
 from libensemble.utils.loc_stack import LocationStack
 from libensemble.utils.misc import extract_H_ranges
 from libensemble.utils.output_directory import EnsembleDirectory
-from libensemble.utils.runners import Runners
+from libensemble.utils.runners import Runner
 from libensemble.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 # To change logging level for just this module
 # logger.setLevel(logging.DEBUG)
 task_timing = False
 
@@ -93,15 +93,15 @@
     # Receive dtypes from manager
     _, dtypes = comm.recv()
 
     # Receive workflow dir from manager
     if libE_specs.get("use_workflow_dir"):
         _, libE_specs["workflow_dir_path"] = comm.recv()
 
-    workerID = workerID or comm.rank
+    workerID = workerID or getattr(comm, "rank", 0)
 
     # Initialize logging on comms
     if log_comm:
         worker_logging_config(comm, workerID)
 
     LS = LocationStack()
     LS.register_loc("workflow", Path(libE_specs.get("workflow_dir_path")))
@@ -162,18 +162,18 @@
     ) -> None:  # noqa: F821
         """Initializes new worker object"""
         self.comm = comm
         self.dtypes = dtypes
         self.workerID = workerID
         self.libE_specs = libE_specs
         self.stats_fmt = libE_specs.get("stats_fmt", {})
-
+        self.sim_runner = Runner(sim_specs)
+        self.gen_runner = Runner(gen_specs)
+        self.runners = {EVAL_SIM_TAG: self.sim_runner.run, EVAL_GEN_TAG: self.gen_runner.run}
         self.calc_iter = {EVAL_SIM_TAG: 0, EVAL_GEN_TAG: 0}
-        self.runners = Runners(sim_specs, gen_specs)
-        self._run_calc = self.runners.make_runners()
         Worker._set_executor(self.workerID, self.comm)
         Worker._set_resources(self.workerID, self.comm)
         self.EnsembleDirectory = EnsembleDirectory(libE_specs=libE_specs)
 
     @staticmethod
     def _set_gen_procs_gpus(libE_info, obj):
         if any(k in libE_info for k in ("num_procs", "num_gpus")):
@@ -252,15 +252,15 @@
 
         enum_desc, calc_id = self._extract_debug_data(calc_type, Work)
 
         timer = Timer()
 
         try:
             logger.debug(f"Starting {enum_desc}: {calc_id}")
-            calc = self._run_calc[calc_type]
+            calc = self.runners[calc_type]
             with timer:
                 if self.EnsembleDirectory.use_calc_dirs(calc_type):
                     loc_stack, calc_dir = self.EnsembleDirectory.prep_calc_dir(
                         Work,
                         self.calc_iter,
                         self.workerID,
                         calc_type,
@@ -408,9 +408,12 @@
                 self.comm.send(0, response)
 
         except Exception as e:
             self.comm.send(0, WorkerErrMsg(" ".join(format_exc_msg(type(e), e)).strip(), format_exc()))
         else:
             self.comm.kill_pending()
         finally:
-            self.runners.shutdown()
+            self.gen_runner.shutdown()
+            self.sim_runner.shutdown()
             self.EnsembleDirectory.copy_back()
+            if Executor.executor is not None:
+                Executor.executor.comm = None  # so Executor can be pickled upon further libE calls
```

### Comparing `libensemble-1.2.2/libensemble.egg-info/PKG-INFO` & `libensemble-1.3.0/libensemble.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libensemble
-Version: 1.2.2
+Version: 1.3.0
 Summary: Library to coordinate the concurrent evaluation of dynamic ensembles of calculations
 Home-page: https://github.com/Libensemble/libensemble
 Author: Jeffrey Larson, Stephen Hudson, Stefan M. Wild, David Bindel and John-Luke Navarro
 Author-email: libensemble@lists.mcs.anl.gov
 License: BSD 3-clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,50 +21,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 License-File: LICENSE
 
-.. image:: https://raw.githubusercontent.com/Libensemble/libensemble/main/docs/images/libE_logo.png
-   :align: center
-   :alt: libEnsemble
-
-|
-
-.. image:: https://img.shields.io/pypi/v/libensemble.svg?color=blue
-   :target: https://pypi.org/project/libensemble
-
-.. image:: https://img.shields.io/conda/v/conda-forge/libensemble?color=blue
-   :target: https://anaconda.org/conda-forge/libensemble
-
-.. image:: https://img.shields.io/spack/v/py-libensemble?color=blue
-   :target: https://packages.spack.io/package.html?name=py-libensemble
-
-|
-
-.. image:: https://github.com/Libensemble/libensemble/actions/workflows/extra.yml/badge.svg?branch=main
-   :target: https://github.com/Libensemble/libensemble/actions
-
-.. image:: https://codecov.io/github/Libensemble/libensemble/graph/badge.svg
-   :target: https://codecov.io/github/Libensemble/libensemble
-
-.. image:: https://readthedocs.org/projects/libensemble/badge/?maxAge=2592000
-   :target: https://libensemble.readthedocs.org/en/latest/
-   :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: black
+|libE_logo|
 
-.. image:: https://joss.theoj.org/papers/10.21105/joss.06031/status.svg
-   :target: https://doi.org/10.21105/joss.06031
-   :alt: JOSS Status
+|PyPI| |Conda| |Spack|
 
-|
+|Tests| |Coverage| |Docs| |Style| |JOSS|
 
 .. after_badges_rst_tag
 
 =====================================================================
 libEnsemble: A complete toolkit for dynamic ensembles of calculations
 =====================================================================
 
@@ -158,14 +127,37 @@
     volume  = {33},
     number  = {4},
     pages   = {977--988},
     year    = {2022},
     doi     = {10.1109/tpds.2021.3082815}
   }
 
+.. |libE_logo| image:: https://raw.githubusercontent.com/Libensemble/libensemble/main/docs/images/libE_logo.png
+   :align: middle
+   :alt: libEnsemble
+.. |PyPI| image:: https://img.shields.io/pypi/v/libensemble.svg?color=blue
+   :target: https://pypi.org/project/libensemble
+.. |Conda| image:: https://img.shields.io/conda/v/conda-forge/libensemble?color=blue
+   :target: https://anaconda.org/conda-forge/libensemble
+.. |Spack| image:: https://img.shields.io/spack/v/py-libensemble?color=blue
+   :target: https://packages.spack.io/package.html?name=py-libensemble
+.. |Tests| image:: https://github.com/Libensemble/libensemble/actions/workflows/extra.yml/badge.svg?branch=main
+   :target: https://github.com/Libensemble/libensemble/actions
+.. |Coverage| image:: https://codecov.io/github/Libensemble/libensemble/graph/badge.svg
+   :target: https://codecov.io/github/Libensemble/libensemble
+.. |Docs| image:: https://readthedocs.org/projects/libensemble/badge/?maxAge=2592000
+   :target: https://libensemble.readthedocs.org/en/latest/
+   :alt: Documentation Status
+.. |Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Code style: black
+.. |JOSS| image:: https://joss.theoj.org/papers/10.21105/joss.06031/status.svg
+   :target: https://doi.org/10.21105/joss.06031
+   :alt: JOSS Status
+
 .. _Community Examples repository: https://github.com/Libensemble/libe-community-examples
 .. _conda-forge: https://conda-forge.org/
 .. _Contributions: https://github.com/Libensemble/libensemble/blob/main/CONTRIBUTING.rst
 .. _docs: https://libensemble.readthedocs.io/en/main/advanced_installation.html
 .. _GitHub: https://github.com/Libensemble/libensemble
 .. _libEnsemble mailing list: https://lists.mcs.anl.gov/mailman/listinfo/libensemble
 .. _libEnsemble Slack page: https://libensemble.slack.com
```

### Comparing `libensemble-1.2.2/libensemble.egg-info/SOURCES.txt` & `libensemble-1.3.0/libensemble.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 docs/posters.rst
 docs/programming_libE.rst
 docs/references.bib
 docs/release_notes.rst
 docs/requirements.txt
 docs/rst_formatting_guidelines
 docs/running_libE.rst
+docs/spelling_wordlist.txt
 docs/utilities.rst
 docs/welcome.rst
 docs/xSDK_policy_compatibility.md
 docs/_static/my_theme.css
 docs/data_structures/alloc_specs.rst
 docs/data_structures/data_structures.rst
 docs/data_structures/exit_criteria.rst
@@ -227,15 +228,14 @@
 examples/tutorials/images/sampling_6hc.png
 examples/tutorials/simple_sine/sine_gen.py
 examples/tutorials/simple_sine/sine_sim.py
 examples/tutorials/simple_sine/sine_tutorial_notebook.ipynb
 examples/tutorials/simple_sine/test_local_sine_tutorial.py
 examples/tutorials/simple_sine/test_local_sine_tutorial_2.py
 examples/tutorials/simple_sine/test_local_sine_tutorial_3.py
-install/environment.yml
 install/find_mpi.py
 install/gen_deps_environment.yml
 install/misc_feature_requirements.txt
 install/testing_requirements.txt
 libensemble/__init__.py
 libensemble/ensemble.py
 libensemble/history.py
@@ -330,25 +330,27 @@
 libensemble/tests/functionality_tests/1d_sampling.yaml
 libensemble/tests/functionality_tests/check_libE_stats.py
 libensemble/tests/functionality_tests/env_script_in.sh
 libensemble/tests/functionality_tests/forces_simf.py
 libensemble/tests/functionality_tests/sine_gen.py
 libensemble/tests/functionality_tests/sine_sim.py
 libensemble/tests/functionality_tests/test_1d_sampling_from_files.py
+libensemble/tests/functionality_tests/test_1d_sampling_no_comms_given.py
 libensemble/tests/functionality_tests/test_1d_sampling_with_profile.py
 libensemble/tests/functionality_tests/test_1d_splitcomm.py
 libensemble/tests/functionality_tests/test_1d_subcomm.py
 libensemble/tests/functionality_tests/test_1d_super_simple.py
 libensemble/tests/functionality_tests/test_1d_uniform_sampling_with_comm_dup.py
 libensemble/tests/functionality_tests/test_GPU_gen_resources.py
 libensemble/tests/functionality_tests/test_active_persistent_worker_abort.py
 libensemble/tests/functionality_tests/test_calc_exception.py
 libensemble/tests/functionality_tests/test_cancel_in_alloc.py
 libensemble/tests/functionality_tests/test_comms.py
 libensemble/tests/functionality_tests/test_elapsed_time_abort.py
+libensemble/tests/functionality_tests/test_evaluate_existing_plus_gen.py
 libensemble/tests/functionality_tests/test_executor_forces_tutorial.py
 libensemble/tests/functionality_tests/test_executor_forces_tutorial_2.py
 libensemble/tests/functionality_tests/test_executor_hworld_pass_fail.py
 libensemble/tests/functionality_tests/test_executor_hworld_timeout.py
 libensemble/tests/functionality_tests/test_executor_simple.py
 libensemble/tests/functionality_tests/test_fast_alloc.py
 libensemble/tests/functionality_tests/test_local_sine_tutorial.py
@@ -515,14 +517,15 @@
 libensemble/tests/standalone_tests/node_concurrency_test/run/run_batches.sh
 libensemble/tests/standalone_tests/node_concurrency_test/run/run_timing_study.sh
 libensemble/tests/standalone_tests/node_concurrency_test/run/submit_frontier.sh
 libensemble/tests/standalone_tests/node_concurrency_test/run/submit_perlmutter.sh
 libensemble/tests/unit_tests/.coveragerc
 libensemble/tests/unit_tests/__init__.py
 libensemble/tests/unit_tests/conftest.py
+libensemble/tests/unit_tests/env_script_in.sh
 libensemble/tests/unit_tests/launch_busy.py
 libensemble/tests/unit_tests/setup.py
 libensemble/tests/unit_tests/test_allocation_funcs_and_support.py
 libensemble/tests/unit_tests/test_comms.py
 libensemble/tests/unit_tests/test_ensemble.py
 libensemble/tests/unit_tests/test_env_resources.py
 libensemble/tests/unit_tests/test_executor.py
@@ -552,14 +555,15 @@
 libensemble/tests/unit_tests/simdir/test_example.json
 libensemble/tests/unit_tests/simdir/test_example.toml
 libensemble/tests/unit_tests/simdir/test_example.yaml
 libensemble/tests/unit_tests/simdir/test_example_badfuncs_attribute.yaml
 libensemble/tests/unit_tests/simdir/test_example_badfuncs_notfound.yaml
 libensemble/tests/unit_tests_logger/.coveragerc
 libensemble/tests/unit_tests_logger/test_logger.py
+libensemble/tests/unit_tests_mpi_import/.coveragerc
 libensemble/tests/unit_tests_mpi_import/conftest.py
 libensemble/tests/unit_tests_mpi_import/test_libE_main.py
 libensemble/tests/unit_tests_nompi/.coveragerc
 libensemble/tests/unit_tests_nompi/conftest.py
 libensemble/tests/unit_tests_nompi/test_aaa_comms.py
 libensemble/tools/__init__.py
 libensemble/tools/alloc_support.py
```

### Comparing `libensemble-1.2.2/scripts/compare_npy.py` & `libensemble-1.3.0/scripts/compare_npy.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/liberegister` & `libensemble-1.3.0/scripts/liberegister`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/libesubmit` & `libensemble-1.3.0/scripts/libesubmit`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/plot_contours_and_history_points.py` & `libensemble-1.3.0/scripts/plot_contours_and_history_points.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/plot_libe_calcs_util_v_time.py` & `libensemble-1.3.0/scripts/plot_libe_calcs_util_v_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/plot_libe_histogram.py` & `libensemble-1.3.0/scripts/plot_libe_histogram.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/plot_libe_tasks_util_v_time.py` & `libensemble-1.3.0/scripts/plot_libe_tasks_util_v_time.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/plot_pareto_3d.py` & `libensemble-1.3.0/scripts/plot_pareto_3d.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/print_fields.py` & `libensemble-1.3.0/scripts/print_fields.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/print_npy.py` & `libensemble-1.3.0/scripts/print_npy.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/process_history_to_make_chart.py` & `libensemble-1.3.0/scripts/process_history_to_make_chart.py`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/scripts/readme.rst` & `libensemble-1.3.0/scripts/readme.rst`

 * *Files identical despite different names*

### Comparing `libensemble-1.2.2/setup.py` & `libensemble-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     extras_require={
         "docs": [
             "autodoc_pydantic",
             "sphinx<8",
             "sphinx_design",
             "sphinx_rtd_theme",
             "sphinxcontrib-bibtex",
+            "sphinxcontrib-spelling",
             "sphinx-copybutton",
         ],
     },
     scripts=[
         "scripts/liberegister",
         "scripts/libesubmit",
     ],
```


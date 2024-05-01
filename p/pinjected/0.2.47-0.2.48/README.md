# Comparing `tmp/pinjected-0.2.47.tar.gz` & `tmp/pinjected-0.2.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.47.tar", max compression
+gzip compressed data, was "pinjected-0.2.48.tar", max compression
```

## Comparing `pinjected-0.2.47.tar` & `pinjected-0.2.48.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.47/LICENSE
--rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.47/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.47/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.47/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.47/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.47/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.47/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5817 2024-04-24 10:38:38.128103 pinjected-0.2.47/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.47/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7345 2024-04-24 10:43:24.249513 pinjected-0.2.47/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.47/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.47/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.47/pinjected/di/decorators.py
--rw-r--r--   0        0        0    14786 2024-04-24 11:20:36.713957 pinjected-0.2.47/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.47/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.47/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.47/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.47/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.47/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.47/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.47/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.47/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.47/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.47/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.47/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.47/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.47/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.47/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.47/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.47/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.47/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.47/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.47/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.47/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.47/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.47/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.47/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.47/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.47/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.47/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.47/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.47/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.47/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.47/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31540 2024-04-16 12:32:23.061374 pinjected-0.2.47/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.47/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.47/pinjected/global_configs.py
--rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.47/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.47/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.47/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.47/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.47/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.47/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.47/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.47/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.47/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.47/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.47/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.47/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.47/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.47/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.47/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.47/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.47/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.47/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.47/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.47/pinjected/providable.py
--rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.47/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.47/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.47/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.47/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.47/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9550 2024-04-26 06:01:47.934871 pinjected-0.2.47/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.47/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.47/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.47/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.47/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.47/pinjected/test_package/child/module_with.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.47/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.47/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     7098 2024-04-24 11:49:45.241822 pinjected-0.2.47/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.47/pinjected/v2/di.py
--rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.47/pinjected/v2/keys.py
--rw-r--r--   0        0        0      507 2024-04-24 11:15:46.603608 pinjected-0.2.47/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0     9332 2024-04-24 11:45:09.926974 pinjected-0.2.47/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.47/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.47/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.47/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.47/pinjected/with_context.py
--rw-r--r--   0        0        0      656 2024-04-26 06:01:51.483841 pinjected-0.2.47/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.47/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.48/LICENSE
+-rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.48/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.48/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.48/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.48/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.48/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.48/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5817 2024-04-24 10:38:38.128103 pinjected-0.2.48/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.48/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7345 2024-04-24 10:43:24.249513 pinjected-0.2.48/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.48/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.48/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.48/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14583 2024-05-01 08:01:27.605626 pinjected-0.2.48/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.48/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.48/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.48/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.48/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.48/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.48/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.48/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.48/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.48/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.48/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.48/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.48/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.48/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.48/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.48/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.48/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.48/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.48/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.48/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.48/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.48/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.48/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.48/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.48/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.48/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.48/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15510 2024-05-01 08:01:27.611288 pinjected-0.2.48/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.48/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.48/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.48/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31540 2024-04-16 12:32:23.061374 pinjected-0.2.48/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.48/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.48/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.48/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.48/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.48/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.48/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.48/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.48/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.48/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.48/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.48/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.48/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.48/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.48/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.48/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.48/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.48/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.48/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.48/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.48/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.48/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.48/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.48/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.48/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.48/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.48/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.48/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9814 2024-05-01 08:00:14.710037 pinjected-0.2.48/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.48/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.48/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.48/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.48/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.48/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.48/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.48/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     7100 2024-05-01 08:00:27.078128 pinjected-0.2.48/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.48/pinjected/v2/di.py
+-rw-r--r--   0        0        0      524 2024-05-01 08:03:21.521914 pinjected-0.2.48/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      508 2024-05-01 08:00:14.705856 pinjected-0.2.48/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0    10541 2024-05-01 08:05:13.964304 pinjected-0.2.48/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.48/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.48/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.48/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.48/pinjected/with_context.py
+-rw-r--r--   0        0        0      656 2024-05-01 08:06:06.577458 pinjected-0.2.48/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.48/PKG-INFO
```

### Comparing `pinjected-0.2.47/LICENSE` & `pinjected-0.2.48/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/decoration.py` & `pinjected-0.2.48/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/demo.py` & `pinjected-0.2.48/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/app_designed.py` & `pinjected-0.2.48/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/app_injected.py` & `pinjected-0.2.48/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/applicative.py` & `pinjected-0.2.48/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/ast.py` & `pinjected-0.2.48/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/decorators.py` & `pinjected-0.2.48/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/design.py` & `pinjected-0.2.48/pinjected/di/design.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,38 +170,40 @@
         x = self
         for k, v in kwargs.items():
             if isinstance(v, type):
                 from loguru import logger
                 logger.warning(f"{k} is bound to class {v} with 'bind_instance' do you mean 'bind_class'?")
             x += Design({StrBindKey(k): BindInjected(Injected.pure(v))})
         return x
+    @staticmethod
+    def to_bind( tgt) -> IBind:
+        from loguru import logger
+        match tgt:
+            case IBind():
+                return tgt
+            case type():
+                return BindInjected(Injected.bind(tgt))
+            case EvaledInjected():
+                return ExprBind(tgt)
+            case DelegatedVar():
+                return ExprBind(tgt.eval())
+            case Injected():
+                return BindInjected(tgt)
+            case non_func if not callable(non_func):
+                logger.warning(f"{tgt}: non-callable or non-injected is passed to bind_provider. fixing automatically.")
+                return BindInjected(Injected.pure(non_func))
+            case func if callable(func):
+                return BindInjected(Injected.bind(func))
+            case _:
+                raise ValueError(f"cannot bind {tgt}")
 
     def bind_provider(self, **kwargs: Union[Callable, Injected]):
         bindings = dict()
         for k, v in kwargs.items():
-            # logger.info(f"binding provider:{k}=>{v}")
-            from loguru import logger
-            match v:
-                case type():
-                    # logger.warning(f"{k}->{v}: class is used for bind_provider. fixing automatically.")
-                    bindings[StrBindKey(k)] = BindInjected(Injected.bind(v))
-                case EvaledInjected():
-                    bindings[StrBindKey(k)] = ExprBind(v)
-                case DelegatedVar():
-                    bindings[StrBindKey(k)] = ExprBind(v.eval())
-                case Injected():
-                    bindings[StrBindKey(k)] = BindInjected(v)
-                case non_func if not callable(non_func):
-                    logger.warning(
-                        f"{k}->{v}: non-callable or non-injected is passed to bind_provider. fixing automatically.")
-                    bindings[StrBindKey(k)] = BindInjected(Injected.pure(v))
-                case func if callable(func):
-                    bindings[StrBindKey(k)] = BindInjected(Injected.bind(func))
-                case _:
-                    raise ValueError(f"cannot bind {k} to {v}")
+            bindings[StrBindKey(k)] = self.to_bind(v)
 
         return self + Design(
             bindings=bindings,
         )
 
     def add_metadata(self, **kwargs: "BindMetadata") -> "Design":
         res = self
```

### Comparing `pinjected-0.2.47/pinjected/di/designed.py` & `pinjected-0.2.48/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.48/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/graph.py` & `pinjected-0.2.48/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/injected.py` & `pinjected-0.2.48/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/injected_analysis.py` & `pinjected-0.2.48/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/modular_injected.py` & `pinjected-0.2.48/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/overload_experimental.py` & `pinjected-0.2.48/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/proxiable.py` & `pinjected-0.2.48/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/session.py` & `pinjected-0.2.48/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/sessioned.py` & `pinjected-0.2.48/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/static_proxy.py` & `pinjected-0.2.48/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.48/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/test_graph.py` & `pinjected-0.2.48/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/test_injected.py` & `pinjected-0.2.48/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/tools/add_overload.py` & `pinjected-0.2.48/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/di/util.py` & `pinjected-0.2.48/pinjected/di/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pinjected.di.design import Design
 from pinjected.di.injected import Injected, InjectedPure, InjectedFunction
 from pinjected.di.metadata.bind_metadata import BindMetadata
 from pinjected.di.metadata.location_data import CodeLocation, ModuleVarLocation
 from pinjected.di.monadic import getitem_opt
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.v2.binds import BindInjected
+from pinjected.v2.keys import StrBindKey, DestructorKey
 
 # is it possible to create a binding class which also has an ability to dynamically add..?
 # yes. actually.
 T = TypeVar("T")
 
 
 def rec_valmap(f, tgt: dict):
@@ -131,17 +132,17 @@
     if isinstance(f, type) and "self" in args:
         args.remove("self")
     return args
 
 
 def to_readable_name(o):
     match o:
-        case BindInjected(InjectedFunction(func, _),_):
+        case BindInjected(InjectedFunction(func, _), _):
             return func.__name__
-        case BindInjected(InjectedPure(value),_):
+        case BindInjected(InjectedPure(value), _):
             return value
         case any:
             return any
 
 
 def try_import_subject():
     try:
@@ -414,7 +415,20 @@
     """
     d = Design().bind_provider(**kwargs)
     return add_code_locations(d, kwargs, inspect.currentframe())
 
 
 def injecteds(**kwargs):
     return Design().bind_provider(**kwargs)
+
+
+def destructors(**kwargs):
+    """
+    registers destructors. using DestructorKey.
+    The values must be an async function that takes one argument.
+    """
+    res = instances()
+    for k, v in kwargs.items():
+        tgt = StrBindKey(k)
+        key = DestructorKey(tgt)
+        res += Design(bindings={key: Design.to_bind(v)})
+    return res
```

### Comparing `pinjected-0.2.47/pinjected/exceptions.py` & `pinjected-0.2.48/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.48/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.48/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/graph_inspection.py` & `pinjected-0.2.48/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/helper_structure.py` & `pinjected-0.2.48/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/helpers.py` & `pinjected-0.2.48/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.48/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.48/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/ide_supports/default_design.py` & `pinjected-0.2.48/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.48/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.48/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/main_impl.py` & `pinjected-0.2.48/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/maybe_patch.py` & `pinjected-0.2.48/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/module_helper.py` & `pinjected-0.2.48/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/module_inspector.py` & `pinjected-0.2.48/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/module_var_path.py` & `pinjected-0.2.48/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/notification.py` & `pinjected-0.2.48/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/nx_graph_util.py` & `pinjected-0.2.48/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/run_config_utils.py` & `pinjected-0.2.48/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/run_config_utils_v2.py` & `pinjected-0.2.48/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/run_helpers/config.py` & `pinjected-0.2.48/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.48/pinjected/run_helpers/run_injected.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,35 +118,42 @@
         if cmd == 'call':
             args = call_args or []
             kwargs = call_kwargs or {}
             var = Injected.ensure_injected(var).proxy
             logger.info(f"run_injected call with args:{args}, kwargs:{kwargs}")
 
             async def task():
-                _res = await design.to_resolver().provide(var(*args, **kwargs))
+                resolver = design.to_resolver()
+                _res = await resolver.provide(var(*args, **kwargs))
+
                 if isinstance(_res, Awaitable):
                     #logger.info(f"awaiting awaitable")
                     _res = await _res
                 if not return_result:
                     logger.info(f"run_injected call result:\n{_res}")
+                await resolver.destruct()
                 return _res
 
             res = asyncio.run(task())
         elif cmd == 'get':
             async def task():
-                _res = await design.to_resolver().provide(var)
+                resolver = design.to_resolver()
+                _res = await resolver.provide(var)
                 if isinstance(_res, Coroutine) or isinstance(_res, Awaitable):
                     _res = await _res
+                await resolver.destruct()
                 return _res
 
             res = asyncio.run(task())
             if not return_result:
                 logger.info(f"run_injected get result:\n{pformat(res)}")
         elif cmd == 'fire':
+            raise RuntimeError('fire is deprecated. use get.')
             return_result = True
+            resolver = design.to_resolver()
             res = design.provide(var)
             if isinstance(res, Coroutine):
                 res = asyncio.run(res)
             logger.info(f"run_injected fire result:\n{res}")
             if inspect.iscoroutinefunction(res) or (hasattr(res, '__is_async__') and res.__is_async__):
                 logger.info(f'{res} is a coroutine function, wrapping it with asyncio.run')
                 src = res
```

### Comparing `pinjected-0.2.47/pinjected/runnables.py` & `pinjected-0.2.48/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/test_package/__init__.py` & `pinjected-0.2.48/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/test_package/child/module1.py` & `pinjected-0.2.48/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/v2/ainjected.py` & `pinjected-0.2.48/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/v2/binds.py` & `pinjected-0.2.48/pinjected/v2/binds.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,7 +223,9 @@
     async def provide(self, cxt: ProvideContext, deps: Dict[IBindKey, Any]) -> T:
         data = self.src.provide(cxt, deps)
         return await self.async_f(data)
 
     @property
     def dependencies(self) -> set[IBindKey]:
         return self.src.dependencies
+
+
```

### Comparing `pinjected-0.2.47/pinjected/v2/di.py` & `pinjected-0.2.48/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pinjected/v2/resolver.py` & `pinjected-0.2.48/pinjected/v2/resolver.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from pinjected import Injected
 from pinjected.di.app_injected import await_awaitables, walk_replace, EvaledInjected
 from pinjected.di.ast import Expr, Object, Call, BiOp, UnaryOp, Attr, GetItem
 from pinjected.di.injected import extract_dependency
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.v2.binds import IBind, BindInjected
-from pinjected.v2.keys import IBindKey, StrBindKey
+from pinjected.v2.keys import IBindKey, StrBindKey, DestructorKey
 from pinjected.v2.provide_context import ProvideContext
 
 Providable = Union[str, IBindKey, Callable, IBind]
 
 
 class IScope(ABC):
     @abstractmethod
@@ -110,14 +110,16 @@
         )
         self.objects = {
             StrBindKey("__resolver__"): self,
             StrBindKey("__design__"): self.design
         }
         self.eval_memos = {}
         self.eval_locks = defaultdict(asyncio.Lock)
+        self.destruction_lock = asyncio.Lock()
+        self.destructed = False
 
     async def _optimize(self, expr: Expr):
         """
         this finds duplicated expr in the node and replace it with Cache Node.
         """
         return walk_replace(expr, lambda x: Cache(x))
 
@@ -240,14 +242,42 @@
 
     def to_blocking(self):
         return Resolver(self)
 
     def __getitem__(self, item):
         return self.provide(item)
 
+    async def destruct(self):
+        """
+        check objects and destruct them if they are destructable.
+        """
+
+        def a_destructor(f):
+            async def impl(tgt):
+                return f(tgt)
+
+            return impl
+
+        async with self.destruction_lock:
+            assert not self.destructed, "Resolver already destructed"
+            destructions = []
+            for k, v in list(self.objects.items()):
+                destruction_key = DestructorKey(k)
+                if destruction_key in self.design:
+                    destructor = await self[destruction_key]
+                    if not inspect.iscoroutinefunction(destructor):
+                        destructor = a_destructor(destructor)
+                    destructions.append(destructor(v))
+            logger.info(f"waiting for {len(destructions)} destructors to finish.")
+            results = await asyncio.gather(*destructions)
+            logger.success(f"all destructors finished with results:{results}")
+            self.destructed = True
+            logger.success(f"Resolver destructed")
+            return results
+
 
 @dataclass
 class Resolver:
     resolver: AsyncResolver
 
     def provide(self, tgt: Providable):
         return asyncio.run(self.resolver.provide(tgt))
```

### Comparing `pinjected-0.2.47/pinjected/visualize_di.py` & `pinjected-0.2.48/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.47/pyproject.toml` & `pinjected-0.2.48/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.47"
+version = "0.2.48"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.47/PKG-INFO` & `pinjected-0.2.48/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.47
+Version: 0.2.48
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/spark_frame-0.4.0.tar.gz` & `tmp/spark_frame-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_frame-0.4.0.tar", max compression
+gzip compressed data, was "spark_frame-0.5.0.tar", max compression
```

## Comparing `spark_frame-0.4.0.tar` & `spark_frame-0.5.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0    11357 2024-01-28 22:15:35.368355 spark_frame-0.4.0/LICENSE
--rw-r--r--   0        0        0    13007 2024-01-28 22:15:35.368355 spark_frame-0.4.0/README.md
--rw-r--r--   0        0        0     1843 2024-01-28 22:15:35.384355 spark_frame-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/__init__.py
--rw-r--r--   0        0        0      130 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/conf.py
--rw-r--r--   0        0        0      308 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/__init__.py
--rw-r--r--   0        0        0    35360 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/compare_dataframes_impl.py
--rw-r--r--   0        0        0      478 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/diff_format_options.py
--rw-r--r--   0        0        0    24153 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/diff_per_col.py
--rw-r--r--   0        0        0    32058 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/diff_result.py
--rw-r--r--   0        0        0    19087 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/diff_result_analyzer.py
--rw-r--r--   0        0        0      988 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/diff_result_summary.py
--rw-r--r--   0        0        0     2421 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/diff_stats.py
--rw-r--r--   0        0        0     2030 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/export.py
--rw-r--r--   0        0        0    10382 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/package.py
--rw-r--r--   0        0        0    10558 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/schema_diff.py
--rw-r--r--   0        0        0     1641 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_diff/special_characters.py
--rw-r--r--   0        0        0     9413 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/data_type_utils.py
--rw-r--r--   0        0        0        0 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/examples/__init__.py
--rw-r--r--   0        0        0     7776 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/examples/flatten_unflatten.py
--rw-r--r--   0        0        0     3900 2024-01-28 22:15:35.384355 spark_frame-0.4.0/spark_frame/examples/reference_nested.py
--rw-r--r--   0        0        0     7820 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/examples/working_with_json.py
--rw-r--r--   0        0        0    27192 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/examples/working_with_nested_data.py
--rw-r--r--   0        0        0      996 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/exceptions.py
--rw-r--r--   0        0        0     5527 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/field_utils.py
--rw-r--r--   0        0        0     7060 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/filesystem.py
--rw-r--r--   0        0        0      418 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/fp/README.md
--rw-r--r--   0        0        0      181 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/fp/__init__.py
--rw-r--r--   0        0        0     5547 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/fp/higher_order.py
--rw-r--r--   0        0        0     2506 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/fp/package.py
--rw-r--r--   0        0        0     2895 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/fp/printable_function.py
--rw-r--r--   0        0        0     5263 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/functions.py
--rw-r--r--   0        0        0      158 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/graph.py
--rw-r--r--   0        0        0        0 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/graph_impl/__init__.py
--rw-r--r--   0        0        0    20684 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/graph_impl/ascending_forest_traversal.py
--rw-r--r--   0        0        0      587 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested.py
--rw-r--r--   0        0        0      258 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_functions.py
--rw-r--r--   0        0        0        0 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_functions_impl/__init__.py
--rw-r--r--   0        0        0    13660 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_functions_impl/aggregate.py
--rw-r--r--   0        0        0     7895 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_functions_impl/average.py
--rw-r--r--   0        0        0     7257 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_functions_impl/sum.py
--rw-r--r--   0        0        0        0 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/__init__.py
--rw-r--r--   0        0        0     3571 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/fields.py
--rw-r--r--   0        0        0    46275 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/package.py
--rw-r--r--   0        0        0     3594 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/print_schema.py
--rw-r--r--   0        0        0     4094 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/schema_string.py
--rw-r--r--   0        0        0    10693 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/select_impl.py
--rw-r--r--   0        0        0     3550 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/unnest_all_fields.py
--rw-r--r--   0        0        0     3288 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/unnest_field.py
--rw-r--r--   0        0        0    10597 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/nested_impl/with_fields.py
--rw-r--r--   0        0        0        0 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/py.typed
--rw-r--r--   0        0        0     8338 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/schema_utils.py
--rw-r--r--   0        0        0     1404 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations.py
--rw-r--r--   0        0        0        0 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/__init__.py
--rw-r--r--   0        0        0    14527 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/analyze.py
--rw-r--r--   0        0        0     1503 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/analyze_aggs.py
--rw-r--r--   0        0        0     2947 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/convert_all_maps_to_arrays.py
--rw-r--r--   0        0        0     3134 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/flatten.py
--rw-r--r--   0        0        0     2429 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/flatten_all_arrays.py
--rw-r--r--   0        0        0     4791 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/harmonize_dataframes.py
--rw-r--r--   0        0        0    11105 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/parse_json_columns.py
--rw-r--r--   0        0        0     4115 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/sort_all_arrays.py
--rw-r--r--   0        0        0     4886 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/transform_all_field_names.py
--rw-r--r--   0        0        0     4292 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/transform_all_fields.py
--rw-r--r--   0        0        0     5175 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/unflatten.py
--rw-r--r--   0        0        0     1097 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/union_dataframes.py
--rw-r--r--   0        0        0     3882 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/unpivot.py
--rw-r--r--   0        0        0    10304 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/transformations_impl/with_generic_typed_struct.py
--rw-r--r--   0        0        0    15233 2024-01-28 22:15:35.388355 spark_frame-0.4.0/spark_frame/utils.py
--rw-r--r--   0        0        0    14065 1970-01-01 00:00:00.000000 spark_frame-0.4.0/setup.py
--rw-r--r--   0        0        0    13626 1970-01-01 00:00:00.000000 spark_frame-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 08:48:50.136915 spark_frame-0.5.0/LICENSE
+-rw-r--r--   0        0        0    14026 2024-05-01 08:48:50.136915 spark_frame-0.5.0/README.md
+-rw-r--r--   0        0        0     2711 2024-05-01 08:48:50.156915 spark_frame-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/conf.py
+-rw-r--r--   0        0        0      308 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/__init__.py
+-rw-r--r--   0        0        0    42984 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/compare_dataframes_impl.py
+-rw-r--r--   0        0        0      478 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/diff_format_options.py
+-rw-r--r--   0        0        0    30636 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/diff_per_col.py
+-rw-r--r--   0        0        0    35277 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/diff_result.py
+-rw-r--r--   0        0        0    22082 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/diff_result_analyzer.py
+-rw-r--r--   0        0        0     1010 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/diff_result_summary.py
+-rw-r--r--   0        0        0     2421 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/diff_stats.py
+-rw-r--r--   0        0        0     2468 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/export.py
+-rw-r--r--   0        0        0    11113 2024-05-01 08:48:50.156915 spark_frame-0.5.0/spark_frame/data_diff/package.py
+-rw-r--r--   0        0        0     2816 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/data_diff/sample.py
+-rw-r--r--   0        0        0    10558 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/data_diff/schema_diff.py
+-rw-r--r--   0        0        0     1641 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/data_diff/special_characters.py
+-rw-r--r--   0        0        0     9413 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/data_type_utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/examples/__init__.py
+-rw-r--r--   0        0        0     7776 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/examples/flatten_unflatten.py
+-rw-r--r--   0        0        0     3900 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/examples/reference_nested.py
+-rw-r--r--   0        0        0     7820 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/examples/working_with_json.py
+-rw-r--r--   0        0        0    27192 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/examples/working_with_nested_data.py
+-rw-r--r--   0        0        0      996 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/exceptions.py
+-rw-r--r--   0        0        0     7387 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/field_utils.py
+-rw-r--r--   0        0        0     7060 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/filesystem.py
+-rw-r--r--   0        0        0      418 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/fp/README.md
+-rw-r--r--   0        0        0      181 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/fp/__init__.py
+-rw-r--r--   0        0        0     5547 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/fp/higher_order.py
+-rw-r--r--   0        0        0     2506 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/fp/package.py
+-rw-r--r--   0        0        0     2895 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/fp/printable_function.py
+-rw-r--r--   0        0        0     6590 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/functions.py
+-rw-r--r--   0        0        0      158 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/graph.py
+-rw-r--r--   0        0        0        0 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/graph_impl/__init__.py
+-rw-r--r--   0        0        0    20684 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/graph_impl/ascending_forest_traversal.py
+-rw-r--r--   0        0        0      587 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested.py
+-rw-r--r--   0        0        0      258 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_functions.py
+-rw-r--r--   0        0        0        0 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_functions_impl/__init__.py
+-rw-r--r--   0        0        0    13660 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_functions_impl/aggregate.py
+-rw-r--r--   0        0        0     7895 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_functions_impl/average.py
+-rw-r--r--   0        0        0     7257 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_functions_impl/sum.py
+-rw-r--r--   0        0        0        0 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/__init__.py
+-rw-r--r--   0        0        0     3571 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/fields.py
+-rw-r--r--   0        0        0    46407 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/package.py
+-rw-r--r--   0        0        0     3594 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/print_schema.py
+-rw-r--r--   0        0        0     4094 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/schema_string.py
+-rw-r--r--   0        0        0    10693 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/select_impl.py
+-rw-r--r--   0        0        0     3553 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/unnest_all_fields.py
+-rw-r--r--   0        0        0     3288 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/unnest_field.py
+-rw-r--r--   0        0        0    10597 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/nested_impl/with_fields.py
+-rw-r--r--   0        0        0        0 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/py.typed
+-rw-r--r--   0        0        0     8338 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/schema_utils.py
+-rw-r--r--   0        0        0     1404 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/transformations.py
+-rw-r--r--   0        0        0        0 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/transformations_impl/__init__.py
+-rw-r--r--   0        0        0    14527 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/transformations_impl/analyze.py
+-rw-r--r--   0        0        0     1503 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/transformations_impl/analyze_aggs.py
+-rw-r--r--   0        0        0     2947 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/transformations_impl/convert_all_maps_to_arrays.py
+-rw-r--r--   0        0        0     3134 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/transformations_impl/flatten.py
+-rw-r--r--   0        0        0     2429 2024-05-01 08:48:50.160915 spark_frame-0.5.0/spark_frame/transformations_impl/flatten_all_arrays.py
+-rw-r--r--   0        0        0     4791 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/harmonize_dataframes.py
+-rw-r--r--   0        0        0    11261 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/parse_json_columns.py
+-rw-r--r--   0        0        0     4115 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/sort_all_arrays.py
+-rw-r--r--   0        0        0     4886 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/transform_all_field_names.py
+-rw-r--r--   0        0        0     4292 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/transform_all_fields.py
+-rw-r--r--   0        0        0     5335 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/unflatten.py
+-rw-r--r--   0        0        0     1097 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/union_dataframes.py
+-rw-r--r--   0        0        0     3882 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/unpivot.py
+-rw-r--r--   0        0        0    10304 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/transformations_impl/with_generic_typed_struct.py
+-rw-r--r--   0        0        0    15233 2024-05-01 08:48:50.164915 spark_frame-0.5.0/spark_frame/utils.py
+-rw-r--r--   0        0        0    15198 1970-01-01 00:00:00.000000 spark_frame-0.5.0/setup.py
+-rw-r--r--   0        0        0    14734 1970-01-01 00:00:00.000000 spark_frame-0.5.0/PKG-INFO
```

### Comparing `spark_frame-0.4.0/LICENSE` & `spark_frame-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/README.md` & `spark_frame-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,28 +61,35 @@
 ## Compatibilities and requirements
 
 
 This library does not depend on any other library.
 **Pyspark must be installed separately to use it.**
 It is compatible with the following versions:
 
-- Python: requires 3.8.1 or higher (tested against Python 3.9, 3.10 and 3.11)
-- Pyspark: requires 3.3.0 or higher
+- Python: requires 3.8.1 or higher (tested against Python 3.8, 3.9, 3.10, 3.11 and 3.12)
+- Pyspark: requires 3.3.0 or higher (tested against PySpark 3.3, 3.4 and 3.5)
 
 This library is tested against Windows, Mac and Linux.
 
+However, testing for the following combinations has been disabled, because they are failing:
+
+- PySpark 3.3 with Python >= 3.11
+- PySpark 3.4 with Python >= 3.12
+- PySpark 3.5 with Python 3.12 on Windows
+
 
 **Some features require extra libraries to be installed alongside this project.**
 **We chose to not include them as direct dependencies for security and flexibility reasons.**
 **This way, users who are not using these features don't need to worry about these dependencies.**
 
-| feature                                    |  Method                      | spark-frame's <br> version |     dependency required |
-|--------------------------------------------|------------------------------|----------------------------|------------------------:|
-| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | >= 0.4.0                   | data-diff-viewer==0.2.* |
-| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | < 0.4                      |                  jinja2 |
+| feature                                    |  Method                      | spark-frame's <br> version |               dependency required |
+|--------------------------------------------|------------------------------|----------------------------|----------------------------------:|
+| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | >= 0.5.0                   | data-diff-viewer==0.3.* (>=0.3.2) |
+| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | 0.4.*                      |           data-diff-viewer==0.2.* |
+| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | < 0.4                      |                            jinja2 |
 
 _Since version 0.4, the code used to generate HTML diff reports has been moved to 
 [data-diff-viewer](https://github.com/FurcyPin/data-diff-viewer) from the same author. 
 It comes with a dependency to [duckdb](https://github.com/duckdb/duckdb), 
 which is used to store the diff results and embed them in the HTML page._
 
 
@@ -99,14 +106,33 @@
 except the former runs on PySpark while the latter runs on BigQuery (obviously).
 I try to keep both projects consistent together, and will eventually port new developments made on 
 one project to the other one.
 
 
 # Changelog
 
+
+# v0.5.0
+
+**New features:**
+
+- data-diff:
+  - Full sample rows in data-diff: in the data-diff HTML report, you can now click on a most frequent 
+    value or change for a column and it will display the full content of a row where this change happens.
+    
+
+**Breaking Changes:**
+
+- data-diff:
+  - The names of the keys of the `DiffResult.diff_df_shards` dict have changed: 
+    All keys except the root key (`""`) have been appended a REPETITION_MARKER (`"!"`).
+    This will make future manipulations easier. This should not impact users as it is a very advanced mechanic. 
+
+
+
 # v0.4.0
 
 Fixes and improvements on data_diff.
 
 Improvements:
 - data-diff: 
   - Now supports complex data types. Declaring a repeated field (e.g. `"s!.id"` in join_cols will now explode the
@@ -119,15 +145,15 @@
 - added package `spark_frame.filesystem` that can be used to read and write files directly from the driver using
   the java FileSystem from Spark's JVM.
 
 **Breaking Changes:**
 - data-diff:
   - `spark_frame.data_diff.DataframeComparator` object has been removed. 
     Please use directly the method `spark_frame.data_diff.compare_dataframes`.
-  - package `spark_frame.data_diff.diff_results` has been renamed to `diff_results`.
+  - package `spark_frame.data_diff.diff_results` has been renamed to `diff_result`.
   - Generating HTML reports for data diff does not require jinja anymore, but it does now require the installation 
     of the library [data-diff-viewer](https://pypi.org/project/data-diff-viewer/), 
     please check the [Compatibilities and requirements](#compatibilities-and-requirements) 
     section to know which version to use.
   - The DiffResult object returned by the `compare_dataframes` method has evolved. In particular, the
     type of `diff_df_shards` changed from a single `DataFrame` to a `Dict[str, DataFrame]`.
   - `DiffFormatOptions.max_string_length` option has been removed
```

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/compare_dataframes_impl.py` & `spark_frame-0.5.0/spark_frame/data_diff/compare_dataframes_impl.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pyspark.sql.types import IntegerType, LongType, StringType
 
 from spark_frame import nested
 from spark_frame.data_diff.diff_result import DiffResult
 from spark_frame.data_diff.package import (
     EXISTS_COL_NAME,
     IS_EQUAL_COL_NAME,
+    SAMPLE_ID_COL_NAME,
     STRUCT_SEPARATOR_REPLACEMENT,
     canonize_col,
 )
 from spark_frame.data_diff.schema_diff import (
     DiffPrefix,
     SchemaDiffResult,
     diff_dataframe_schemas,
@@ -20,14 +21,15 @@
 from spark_frame.data_diff.special_characters import (
     _replace_special_characters,
     _replace_special_characters_from_col_names,
     _restore_special_characters,
 )
 from spark_frame.data_type_utils import is_repeated
 from spark_frame.exceptions import CombinatorialExplosionError, DataframeComparisonException
+from spark_frame.field_utils import has_same_or_higher_granularity
 from spark_frame.nested_impl.package import unnest_fields, validate_fields_exist
 from spark_frame.transformations import flatten
 from spark_frame.transformations_impl.convert_all_maps_to_arrays import (
     convert_all_maps_to_arrays,
 )
 from spark_frame.transformations_impl.harmonize_dataframes import harmonize_dataframes
 from spark_frame.transformations_impl.sort_all_arrays import sort_all_arrays
@@ -366,14 +368,15 @@
 
 
 def _build_diff_dataframe(
     left_df: DataFrame,
     right_df: DataFrame,
     column_names_diff: Dict[str, DiffPrefix],
     join_cols: List[str],
+    granularities: List[str],
 ) -> DataFrame:
     """Perform a column-by-column comparison between two DataFrames.
     The two DataFrames must have the same columns with the same ordering.
     The column `join_col` will be used to join the two DataFrames together.
     Then we build a new DataFrame with the `join_col` and for each column, a struct with three elements:
     - `left_value`: the value coming from the `left_df`
     - `right_value`: the value coming from the `right_df`
@@ -420,26 +423,26 @@
         |  4|  f|  3|  5|
         +---+---+---+---+
         <BLANKLINE>
         >>> from spark_frame.data_diff.schema_diff import _diff_dataframe_column_names
         >>> column_names_diff = _diff_dataframe_column_names(left_df.columns, right_df.columns)
         >>> column_names_diff
         {'id': ' ', 'c1': ' ', 'c2': ' ', 'c3': '-', 'c4': '+'}
-        >>> (_build_diff_dataframe(left_df, right_df, column_names_diff, ['id'])
+        >>> (_build_diff_dataframe(left_df, right_df, column_names_diff, join_cols=['id'], granularities=[""])
         ...     .withColumn('coalesced_id', f.expr('coalesce(id.left_value, id.right_value)'))
         ...     .orderBy('coalesced_id').drop('coalesced_id').show(truncate=False)
         ... ) # noqa: E501
-        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-        |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|
-        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-        |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{2, NULL, false, true, false}    |{NULL, 3, false, false, true}    |{true, true} |true        |
-        |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{3, NULL, false, true, false}    |{NULL, 4, false, false, true}    |{true, true} |false       |
-        |{3, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{4, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |
-        |{NULL, 4, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 5, false, false, true}    |{false, true}|false       |
-        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
+        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+        |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|__SAMPLE_ID__|
+        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+        |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{2, NULL, false, true, false}    |{NULL, 3, false, false, true}    |{true, true} |true        |[{"id":1}]   |
+        |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{3, NULL, false, true, false}    |{NULL, 4, false, false, true}    |{true, true} |false       |[{"id":2}]   |
+        |{3, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{4, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |[{"id":3}]   |
+        |{NULL, 4, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 5, false, false, true}    |{false, true}|false       |[{"id":4}]   |
+        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
         <BLANKLINE>
     """  # noqa: E501
     column_names_diff = {_replace_special_characters(col_name): diff for col_name, diff in column_names_diff.items()}
 
     left_df = left_df.withColumn(EXISTS_COL_NAME, f.lit(col=True))
     right_df = right_df.withColumn(EXISTS_COL_NAME, f.lit(col=True))
 
@@ -447,24 +450,28 @@
     diff = left_df.join(right_df, null_safe_join_clause, "full")
 
     left_df_fields = {field.name: field for field in left_df.schema.fields}
     right_df_fields = {field.name: field for field in right_df.schema.fields}
 
     def comparison_struct(col_name: str, diff_prefix: str) -> Column:
         if diff_prefix == DiffPrefix.ADDED:
-            left_col = f.lit(None)
+            # We use IF(true, None, right_df.col_name) to force
+            # the type of the NULL to be the same as right_df.col_name.
+            left_col = f.when(f.lit(col=True), f.lit(col=None)).otherwise(right_df[col_name])
             left_col_str = left_col
             exists_left = f.lit(col=False)
         else:
             left_col = left_df[col_name]
             left_col_str = canonize_col(left_col, left_df_fields[col_name])
             exists_left = f.coalesce(left_df[EXISTS_COL_NAME], f.lit(col=False))
 
         if diff_prefix == DiffPrefix.REMOVED:
-            right_col = f.lit(None)
+            # We use IF(true, None, left_df.col_name) to force
+            # the type of the NULL to be the same as left_df.col_name.
+            right_col = f.when(f.lit(col=True), f.lit(col=None)).otherwise(left_df[col_name])
             right_col_str = right_col
             exists_right = f.lit(col=False)
         else:
             right_col = right_df[col_name]
             right_col_str = canonize_col(right_col, right_df_fields[col_name])
             exists_right = f.coalesce(right_df[EXISTS_COL_NAME], f.lit(col=False))
 
@@ -491,19 +498,153 @@
         ],
         f.struct(
             f.coalesce(left_df[EXISTS_COL_NAME], f.lit(col=False)).alias("left_value"),
             f.coalesce(right_df[EXISTS_COL_NAME], f.lit(col=False)).alias("right_value"),
         ).alias(EXISTS_COL_NAME),
     )
 
+    diff_df = _add_is_equal_column(diff_df, column_names_diff)
+    diff_df = _add_join_cols_column(diff_df, join_cols, granularities)
+
+    return diff_df
+
+
+def _add_is_equal_column(diff_df: DataFrame, column_names_diff: Dict[str, DiffPrefix]) -> DataFrame:
+    """Add the __IS_EQUAL__ column to the diff_df"""
     row_is_equal = f.lit(col=True)
     for col_name, diff_prefix in column_names_diff.items():
         if diff_prefix == DiffPrefix.UNCHANGED and col_name in diff_df.columns:
             row_is_equal = row_is_equal & f.col(f"{col_name}.is_equal")
-    return diff_df.withColumn(IS_EQUAL_COL_NAME, row_is_equal)
+    diff_df = diff_df.withColumn(IS_EQUAL_COL_NAME, row_is_equal)
+    return diff_df
+
+
+def _get_join_cols_matching_key(join_cols: List[str], key: str) -> List[str]:
+    """
+    >>> join_cols = ["id", "s__ARRAY____STRUCT__id", "s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id"]
+    >>> _get_join_cols_matching_key(join_cols, "")
+    ['id']
+    >>> _get_join_cols_matching_key(join_cols, "other!")
+    []
+    >>> _get_join_cols_matching_key(join_cols, "s!")
+    ['id', 's__ARRAY____STRUCT__id']
+    >>> _get_join_cols_matching_key(join_cols, "s!.ss!")
+    ['id', 's__ARRAY____STRUCT__id', 's__ARRAY____STRUCT__ss__ARRAY____STRUCT__id']
+    """
+    join_cols = [_restore_special_characters(col) for col in join_cols]
+    join_cols = [
+        col
+        for col in join_cols
+        if has_same_or_higher_granularity(col, key) and any(has_same_or_higher_granularity(key, c) for c in join_cols)
+    ]
+    join_cols = [_replace_special_characters(col) for col in join_cols]
+    return join_cols
+
+
+def _build_key_col(join_cols: List[str]) -> Column:
+    key_col = f.to_json(
+        f.struct([f.coalesce(f.col(col)["left_value"], f.col(col)["right_value"]).alias(col) for col in join_cols]),
+    )
+    return key_col
+
+
+def _add_join_cols_column(diff_df: DataFrame, join_cols: List[str], common_keys: List[str]) -> DataFrame:
+    """Add the __SAMPLE_ID__ column to the diff_df
+
+    >>> from pyspark.sql import SparkSession
+    >>> spark = SparkSession.builder.appName("doctest").getOrCreate()
+
+    >>> diff_df = spark.sql(
+    ...     '''
+    ...     SELECT INLINE(ARRAY(
+    ...         STRUCT(
+    ...             STRUCT(1 as left_value, 1 as right_value) as id
+    ...         ),
+    ...         STRUCT(
+    ...             STRUCT(2 as left_value, NULL as right_value) as id
+    ...         ),
+    ...         STRUCT(
+    ...             STRUCT(NULL as left_value, 3 as right_value) as id
+    ...         )
+    ...     ))
+    ... ''',
+    ... )
+    >>> diff_df.show(truncate=False)
+    +---------+
+    |id       |
+    +---------+
+    |{1, 1}   |
+    |{2, NULL}|
+    |{NULL, 3}|
+    +---------+
+    <BLANKLINE>
+    >>> join_cols = ["id"]
+    >>> common_keys = [""]
+    >>> _add_join_cols_column(diff_df, join_cols, common_keys).show(truncate=False)
+    +---------+-------------+
+    |id       |__SAMPLE_ID__|
+    +---------+-------------+
+    |{1, 1}   |[{"id":1}]   |
+    |{2, NULL}|[{"id":2}]   |
+    |{NULL, 3}|[{"id":3}]   |
+    +---------+-------------+
+    <BLANKLINE>
+
+    >>> diff_df = spark.sql(
+    ...     '''
+    ...     SELECT INLINE(ARRAY(
+    ...         STRUCT(
+    ...             STRUCT(1 as left_value, 1 as right_value) as id,
+    ...             STRUCT(1 as left_value, 1 as right_value) as s__ARRAY____STRUCT__id,
+    ...             STRUCT(1 as left_value, 1 as right_value) as s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id
+    ...         ),
+    ...         STRUCT(
+    ...             STRUCT(1 as left_value, 1 as right_value) as id,
+    ...             STRUCT(2 as left_value, 2 as right_value) as s__ARRAY____STRUCT__id,
+    ...             STRUCT(1 as left_value, 1 as right_value) as s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id
+    ...         ),
+    ...         STRUCT(
+    ...             STRUCT(2 as left_value, 2 as right_value) as id,
+    ...             STRUCT(1 as left_value, 1 as right_value) as s__ARRAY____STRUCT__id,
+    ...             STRUCT(1 as left_value, 1 as right_value) as s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id
+    ...         ),
+    ...         STRUCT(
+    ...             STRUCT(2 as left_value, 2 as right_value) as id,
+    ...             STRUCT(1 as left_value, 1 as right_value) as s__ARRAY____STRUCT__id,
+    ...             STRUCT(2 as left_value, 2 as right_value) as s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id
+    ...         )
+    ...     ))
+    ... ''',
+    ... )
+    >>> diff_df.show(truncate=False)
+    +------+----------------------+-------------------------------------------+
+    |id    |s__ARRAY____STRUCT__id|s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id|
+    +------+----------------------+-------------------------------------------+
+    |{1, 1}|{1, 1}                |{1, 1}                                     |
+    |{1, 1}|{2, 2}                |{1, 1}                                     |
+    |{2, 2}|{1, 1}                |{1, 1}                                     |
+    |{2, 2}|{1, 1}                |{2, 2}                                     |
+    +------+----------------------+-------------------------------------------+
+    <BLANKLINE>
+    >>> join_cols = ["id", "s__ARRAY____STRUCT__id", "s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id"]
+    >>> common_keys = ["", "other!", "s!", "s!.ss!"]
+    >>> _add_join_cols_column(diff_df, join_cols, common_keys).show(truncate=False)
+    +------+----------------------+-------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
+    |id    |s__ARRAY____STRUCT__id|s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id|__SAMPLE_ID__                                                                                                                           |
+    +------+----------------------+-------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
+    |{1, 1}|{1, 1}                |{1, 1}                                     |[{"id":1}, {}, {"id":1,"s__ARRAY____STRUCT__id":1}, {"id":1,"s__ARRAY____STRUCT__id":1,"s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id":1}]|
+    |{1, 1}|{2, 2}                |{1, 1}                                     |[{"id":1}, {}, {"id":1,"s__ARRAY____STRUCT__id":2}, {"id":1,"s__ARRAY____STRUCT__id":2,"s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id":1}]|
+    |{2, 2}|{1, 1}                |{1, 1}                                     |[{"id":2}, {}, {"id":2,"s__ARRAY____STRUCT__id":1}, {"id":2,"s__ARRAY____STRUCT__id":1,"s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id":1}]|
+    |{2, 2}|{1, 1}                |{2, 2}                                     |[{"id":2}, {}, {"id":2,"s__ARRAY____STRUCT__id":1}, {"id":2,"s__ARRAY____STRUCT__id":1,"s__ARRAY____STRUCT__ss__ARRAY____STRUCT__id":2}]|
+    +------+----------------------+-------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
+    <BLANKLINE>
+    """  # noqa: E501
+    key_cols = [_build_key_col(_get_join_cols_matching_key(join_cols, key)) for key in common_keys]
+    diff_df = diff_df.withColumn(SAMPLE_ID_COL_NAME, f.array(key_cols))
+    return diff_df
 
 
 def _harmonize_and_normalize_dataframes(
     left_flat: DataFrame,
     right_flat: DataFrame,
     skip_make_dataframes_comparable: bool,
 ) -> Tuple[DataFrame, DataFrame]:
@@ -543,41 +684,36 @@
     )
     unnested_right_dfs = unnest_fields(
         right_df,
         right_fields_to_unnest,
         keep_fields=join_cols,
     )
 
-    common_keys = sorted(
+    granularities = sorted(
         set(unnested_left_dfs.keys()).intersection(set(unnested_right_dfs.keys())),
     )
 
-    def build_shard(key: str) -> DataFrame:
-        l_df = unnested_left_dfs[key]
-        r_df = unnested_right_dfs[key]
+    def build_shard(granularity: str) -> DataFrame:
+        l_df = unnested_left_dfs[granularity]
+        r_df = unnested_right_dfs[granularity]
         l_df = _replace_special_characters_from_col_names(l_df)
         r_df = _replace_special_characters_from_col_names(r_df)
         schema_diff_result = diff_dataframe_schemas(l_df, r_df, join_cols)
         new_join_cols = [_replace_special_characters(col) for col in join_cols]
         new_join_cols = [col for col in new_join_cols if col in l_df.columns]
         new_join_cols, self_join_growth_estimate = _get_join_cols(
             l_df,
             r_df,
             new_join_cols,
         )
         _check_join_cols(specified_join_cols, new_join_cols, self_join_growth_estimate)
-        diff_df = _build_diff_dataframe(
-            l_df,
-            r_df,
-            schema_diff_result.column_names_diff,
-            new_join_cols,
-        )
+        diff_df = _build_diff_dataframe(l_df, r_df, schema_diff_result.column_names_diff, new_join_cols, granularities)
         return diff_df
 
-    return {key: build_shard(key) for key in common_keys}
+    return {granularity: build_shard(granularity) for granularity in granularities}
 
 
 def compare_dataframes(
     left_df: DataFrame,
     right_df: DataFrame,
     join_cols: Optional[List[str]] = None,
 ) -> DiffResult:
@@ -759,15 +895,15 @@
         |my_array!.a|2    |1  |
         |my_array!.b|2    |2  |
         |my_array!.c|3    |2  |
         |my_array!.d|4    |3  |
         +-----------+-----+---+
         <BLANKLINE>
         ##############################################################
-        Granularity : my_array (5 rows)
+        Granularity : my_array! (5 rows)
         <BLANKLINE>
         Row count ok: 3 rows
         <BLANKLINE>
         1 (20.0%) rows are identical
         0 (0.0%) rows have changed
         2 (40.0%) rows are only in 'left'
         2 (40.0%) rows are only in 'right
```

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/diff_per_col.py` & `spark_frame-0.5.0/spark_frame/data_diff/diff_per_col.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,76 +50,79 @@
     """Pivot the top_per_col_state_df
 
     Examples:
 
         >>> from spark_frame.data_diff.diff_result import _get_test_diff_result
         >>> diff_result = _get_test_diff_result()
         >>> diff_result.top_per_col_state_df.show(100)
-        +-----------+-------------+----------+-----------+---+-------+
-        |column_name|        state|left_value|right_value| nb|row_num|
-        +-----------+-------------+----------+-----------+---+-------+
-        |         c1|    no_change|         b|          b|  3|      1|
-        |         c1|    no_change|         a|          a|  1|      2|
-        |         c1| only_in_left|         c|       NULL|  1|      1|
-        |         c1|only_in_right|      NULL|          f|  1|      1|
-        |         c2|      changed|         2|          4|  2|      1|
-        |         c2|      changed|         2|          3|  1|      2|
-        |         c2|    no_change|         1|          1|  1|      1|
-        |         c2| only_in_left|         3|       NULL|  1|      1|
-        |         c2|only_in_right|      NULL|          3|  1|      1|
-        |         c3| only_in_left|         1|       NULL|  2|      1|
-        |         c3| only_in_left|         2|       NULL|  2|      2|
-        |         c3| only_in_left|         3|       NULL|  1|      3|
-        |         c4|only_in_right|      NULL|          1|  2|      1|
-        |         c4|only_in_right|      NULL|          2|  2|      2|
-        |         c4|only_in_right|      NULL|          3|  1|      3|
-        |         id|    no_change|         1|          1|  1|      1|
-        |         id|    no_change|         2|          2|  1|      2|
-        |         id|    no_change|         3|          3|  1|      3|
-        |         id|    no_change|         4|          4|  1|      4|
-        |         id| only_in_left|         5|       NULL|  1|      1|
-        |         id|only_in_right|      NULL|          6|  1|      1|
-        +-----------+-------------+----------+-----------+---+-------+
+        +-----------+-------------+----------+-----------+---+-----------+-------+
+        |column_name|        state|left_value|right_value| nb| sample_ids|row_num|
+        +-----------+-------------+----------+-----------+---+-----------+-------+
+        |         c1|    no_change|         b|          b|  3|[{"id": 2}]|      1|
+        |         c1|    no_change|         a|          a|  1|[{"id": 1}]|      2|
+        |         c1| only_in_left|         c|       NULL|  1|[{"id": 5}]|      1|
+        |         c1|only_in_right|      NULL|          f|  1|[{"id": 6}]|      1|
+        |         c2|      changed|         2|          4|  2|[{"id": 3}]|      1|
+        |         c2|      changed|         2|          3|  1|[{"id": 2}]|      2|
+        |         c2|    no_change|         1|          1|  1|[{"id": 1}]|      1|
+        |         c2| only_in_left|         3|       NULL|  1|[{"id": 5}]|      1|
+        |         c2|only_in_right|      NULL|          3|  1|[{"id": 6}]|      1|
+        |         c3| only_in_left|         1|       NULL|  2|[{"id": 1}]|      1|
+        |         c3| only_in_left|         2|       NULL|  2|[{"id": 3}]|      2|
+        |         c3| only_in_left|         3|       NULL|  1|[{"id": 5}]|      3|
+        |         c4|only_in_right|      NULL|          1|  2|[{"id": 1}]|      1|
+        |         c4|only_in_right|      NULL|          2|  2|[{"id": 3}]|      2|
+        |         c4|only_in_right|      NULL|          3|  1|[{"id": 6}]|      3|
+        |         id|    no_change|         1|          1|  1|[{"id": 1}]|      1|
+        |         id|    no_change|         2|          2|  1|[{"id": 2}]|      2|
+        |         id|    no_change|         3|          3|  1|[{"id": 3}]|      3|
+        |         id|    no_change|         4|          4|  1|[{"id": 4}]|      4|
+        |         id| only_in_left|         5|       NULL|  1|[{"id": 5}]|      1|
+        |         id|only_in_right|      NULL|          6|  1|[{"id": 6}]|      1|
+        +-----------+-------------+----------+-----------+---+-----------+-------+
         <BLANKLINE>
 
         >>> _get_pivoted_df(diff_result.top_per_col_state_df, max_nb_rows_per_col_state=10).show(truncate=False)
-        +-----------+----------+----------------------+------------+--------------------------------------------+---------------+------------------------------------------+----------------+------------------------------------------+
-        |column_name|changed_nb|changed_diff          |no_change_nb|no_change_diff                              |only_in_left_nb|only_in_left_diff                         |only_in_right_nb|only_in_right_diff                        |
-        +-----------+----------+----------------------+------------+--------------------------------------------+---------------+------------------------------------------+----------------+------------------------------------------+
-        |c1         |NULL      |[]                    |4           |[{b, b, 3}, {a, a, 1}]                      |1              |[{c, NULL, 1}]                            |1               |[{NULL, f, 1}]                            |
-        |c4         |NULL      |[]                    |NULL        |[]                                          |NULL           |[]                                        |5               |[{NULL, 1, 2}, {NULL, 2, 2}, {NULL, 3, 1}]|
-        |c3         |NULL      |[]                    |NULL        |[]                                          |5              |[{1, NULL, 2}, {2, NULL, 2}, {3, NULL, 1}]|NULL            |[]                                        |
-        |c2         |3         |[{2, 4, 2}, {2, 3, 1}]|1           |[{1, 1, 1}]                                 |1              |[{3, NULL, 1}]                            |1               |[{NULL, 3, 1}]                            |
-        |id         |NULL      |[]                    |4           |[{1, 1, 1}, {2, 2, 1}, {3, 3, 1}, {4, 4, 1}]|1              |[{5, NULL, 1}]                            |1               |[{NULL, 6, 1}]                            |
-        +-----------+----------+----------------------+------------+--------------------------------------------+---------------+------------------------------------------+----------------+------------------------------------------+
+        +-----------+----------+------------------------------------------------+------------+------------------------------------------------------------------------------------------------+---------------+---------------------------------------------------------------------------------+----------------+---------------------------------------------------------------------------------+
+        |column_name|changed_nb|changed_diff                                    |no_change_nb|no_change_diff                                                                                  |only_in_left_nb|only_in_left_diff                                                                |only_in_right_nb|only_in_right_diff                                                               |
+        +-----------+----------+------------------------------------------------+------------+------------------------------------------------------------------------------------------------+---------------+---------------------------------------------------------------------------------+----------------+---------------------------------------------------------------------------------+
+        |c1         |NULL      |[]                                              |4           |[{b, b, 3, [{"id": 2}]}, {a, a, 1, [{"id": 1}]}]                                                |1              |[{c, NULL, 1, [{"id": 5}]}]                                                      |1               |[{NULL, f, 1, [{"id": 6}]}]                                                      |
+        |c4         |NULL      |[]                                              |NULL        |[]                                                                                              |NULL           |[]                                                                               |5               |[{NULL, 1, 2, [{"id": 1}]}, {NULL, 2, 2, [{"id": 3}]}, {NULL, 3, 1, [{"id": 6}]}]|
+        |c3         |NULL      |[]                                              |NULL        |[]                                                                                              |5              |[{1, NULL, 2, [{"id": 1}]}, {2, NULL, 2, [{"id": 3}]}, {3, NULL, 1, [{"id": 5}]}]|NULL            |[]                                                                               |
+        |c2         |3         |[{2, 4, 2, [{"id": 3}]}, {2, 3, 1, [{"id": 2}]}]|1           |[{1, 1, 1, [{"id": 1}]}]                                                                        |1              |[{3, NULL, 1, [{"id": 5}]}]                                                      |1               |[{NULL, 3, 1, [{"id": 6}]}]                                                      |
+        |id         |NULL      |[]                                              |4           |[{1, 1, 1, [{"id": 1}]}, {2, 2, 1, [{"id": 2}]}, {3, 3, 1, [{"id": 3}]}, {4, 4, 1, [{"id": 4}]}]|1              |[{5, NULL, 1, [{"id": 5}]}]                                                      |1               |[{NULL, 6, 1, [{"id": 6}]}]                                                      |
+        +-----------+----------+------------------------------------------------+------------+------------------------------------------------------------------------------------------------+---------------+---------------------------------------------------------------------------------+----------------+---------------------------------------------------------------------------------+
         <BLANKLINE>
     """  # noqa: E501
     pivoted_df = (
         top_per_col_state_df.groupBy("column_name")
         .pivot(
             "state",
             values=["changed", "no_change", "only_in_left", "only_in_right"],
         )
         .agg(
             f.sum("nb").alias("nb"),
             f.expr(
                 f"""
             ARRAY_AGG(
-                CASE WHEN row_num <= {max_nb_rows_per_col_state} THEN STRUCT(left_value, right_value, nb) END
+                CASE
+                    WHEN row_num <= {max_nb_rows_per_col_state}
+                    THEN STRUCT(left_value, right_value, nb, sample_ids)
+                END
             )""",
             ).alias("diff"),
         )
     )
     return pivoted_df
 
 
 def _format_diff_per_col_df(pivoted_df: DataFrame, col_df: DataFrame) -> DataFrame:
     """
 
-    Examples
+    Examples:
 
         >>> from spark_frame.data_diff.diff_result import _get_test_diff_result
         >>> diff_result = _get_test_diff_result()
         >>> spark = diff_result.top_per_col_state_df.sparkSession
         >>> columns = diff_result.schema_diff_result.column_names
         >>> col_df = _get_col_df(columns, spark)
         >>> pivoted_df = _get_pivoted_df(diff_result.top_per_col_state_df, max_nb_rows_per_col_state=10)
@@ -131,54 +134,58 @@
         |            1|         c1|
         |            2|         c2|
         |            3|         c3|
         |            4|         c4|
         +-------------+-----------+
         <BLANKLINE>
         >>> pivoted_df.show(truncate=False)
-        +-----------+----------+----------------------+------------+--------------------------------------------+---------------+------------------------------------------+----------------+------------------------------------------+
-        |column_name|changed_nb|changed_diff          |no_change_nb|no_change_diff                              |only_in_left_nb|only_in_left_diff                         |only_in_right_nb|only_in_right_diff                        |
-        +-----------+----------+----------------------+------------+--------------------------------------------+---------------+------------------------------------------+----------------+------------------------------------------+
-        |c1         |NULL      |[]                    |4           |[{b, b, 3}, {a, a, 1}]                      |1              |[{c, NULL, 1}]                            |1               |[{NULL, f, 1}]                            |
-        |c4         |NULL      |[]                    |NULL        |[]                                          |NULL           |[]                                        |5               |[{NULL, 1, 2}, {NULL, 2, 2}, {NULL, 3, 1}]|
-        |c3         |NULL      |[]                    |NULL        |[]                                          |5              |[{1, NULL, 2}, {2, NULL, 2}, {3, NULL, 1}]|NULL            |[]                                        |
-        |c2         |3         |[{2, 4, 2}, {2, 3, 1}]|1           |[{1, 1, 1}]                                 |1              |[{3, NULL, 1}]                            |1               |[{NULL, 3, 1}]                            |
-        |id         |NULL      |[]                    |4           |[{1, 1, 1}, {2, 2, 1}, {3, 3, 1}, {4, 4, 1}]|1              |[{5, NULL, 1}]                            |1               |[{NULL, 6, 1}]                            |
-        +-----------+----------+----------------------+------------+--------------------------------------------+---------------+------------------------------------------+----------------+------------------------------------------+
+        +-----------+----------+------------------------------------------------+------------+------------------------------------------------------------------------------------------------+---------------+---------------------------------------------------------------------------------+----------------+---------------------------------------------------------------------------------+
+        |column_name|changed_nb|changed_diff                                    |no_change_nb|no_change_diff                                                                                  |only_in_left_nb|only_in_left_diff                                                                |only_in_right_nb|only_in_right_diff                                                               |
+        +-----------+----------+------------------------------------------------+------------+------------------------------------------------------------------------------------------------+---------------+---------------------------------------------------------------------------------+----------------+---------------------------------------------------------------------------------+
+        |c1         |NULL      |[]                                              |4           |[{b, b, 3, [{"id": 2}]}, {a, a, 1, [{"id": 1}]}]                                                |1              |[{c, NULL, 1, [{"id": 5}]}]                                                      |1               |[{NULL, f, 1, [{"id": 6}]}]                                                      |
+        |c4         |NULL      |[]                                              |NULL        |[]                                                                                              |NULL           |[]                                                                               |5               |[{NULL, 1, 2, [{"id": 1}]}, {NULL, 2, 2, [{"id": 3}]}, {NULL, 3, 1, [{"id": 6}]}]|
+        |c3         |NULL      |[]                                              |NULL        |[]                                                                                              |5              |[{1, NULL, 2, [{"id": 1}]}, {2, NULL, 2, [{"id": 3}]}, {3, NULL, 1, [{"id": 5}]}]|NULL            |[]                                                                               |
+        |c2         |3         |[{2, 4, 2, [{"id": 3}]}, {2, 3, 1, [{"id": 2}]}]|1           |[{1, 1, 1, [{"id": 1}]}]                                                                        |1              |[{3, NULL, 1, [{"id": 5}]}]                                                      |1               |[{NULL, 3, 1, [{"id": 6}]}]                                                      |
+        |id         |NULL      |[]                                              |4           |[{1, 1, 1, [{"id": 1}]}, {2, 2, 1, [{"id": 2}]}, {3, 3, 1, [{"id": 3}]}, {4, 4, 1, [{"id": 4}]}]|1              |[{5, NULL, 1, [{"id": 5}]}]                                                      |1               |[{NULL, 6, 1, [{"id": 6}]}]                                                      |
+        +-----------+----------+------------------------------------------------+------------+------------------------------------------------------------------------------------------------+---------------+---------------------------------------------------------------------------------+----------------+---------------------------------------------------------------------------------+
         <BLANKLINE>
         >>> diff_per_col_df = _format_diff_per_col_df(pivoted_df, col_df)
         >>> nested.print_schema(diff_per_col_df)
         root
          |-- column_number: integer (nullable = true)
          |-- column_name: string (nullable = true)
          |-- counts.total: long (nullable = false)
          |-- counts.changed: long (nullable = false)
          |-- counts.no_change: long (nullable = false)
          |-- counts.only_in_left: long (nullable = false)
          |-- counts.only_in_right: long (nullable = false)
          |-- diff.changed!.left_value: string (nullable = true)
          |-- diff.changed!.right_value: string (nullable = true)
          |-- diff.changed!.nb: long (nullable = false)
+         |-- diff.changed!.sample_ids!: string (nullable = true)
          |-- diff.no_change!.value: string (nullable = true)
          |-- diff.no_change!.nb: long (nullable = false)
+         |-- diff.no_change!.sample_ids!: string (nullable = true)
          |-- diff.only_in_left!.value: string (nullable = true)
          |-- diff.only_in_left!.nb: long (nullable = false)
+         |-- diff.only_in_left!.sample_ids!: string (nullable = true)
          |-- diff.only_in_right!.value: string (nullable = true)
          |-- diff.only_in_right!.nb: long (nullable = false)
+         |-- diff.only_in_right!.sample_ids!: string (nullable = true)
         <BLANKLINE>
         >>> diff_per_col_df.show(truncate=False)
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |column_number|column_name|counts         |diff                                                      |
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1}, {2, 1}, {3, 1}, {4, 1}], [{5, 1}], [{6, 1}]}|
-        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{b, 3}, {a, 1}], [{c, 1}], [{f, 1}]}                |
-        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 4, 2}, {2, 3, 1}], [{1, 1}], [{3, 1}], [{3, 1}]}    |
-        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{1, 2}, {2, 2}, {3, 1}], []}                    |
-        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{1, 2}, {2, 2}, {3, 1}]}                    |
-        +-------------+-----------+---------------+----------------------------------------------------------+
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |column_number|column_name|counts         |diff                                                                                                                                    |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1, [{"id": 1}]}, {2, 1, [{"id": 2}]}, {3, 1, [{"id": 3}]}, {4, 1, [{"id": 4}]}], [{5, 1, [{"id": 5}]}], [{6, 1, [{"id": 6}]}]}|
+        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{b, 3, [{"id": 2}]}, {a, 1, [{"id": 1}]}], [{c, 1, [{"id": 5}]}], [{f, 1, [{"id": 6}]}]}                                          |
+        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 4, 2, [{"id": 3}]}, {2, 3, 1, [{"id": 2}]}], [{1, 1, [{"id": 1}]}], [{3, 1, [{"id": 5}]}], [{3, 1, [{"id": 6}]}]}                 |
+        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}, {3, 1, [{"id": 5}]}], []}                                                           |
+        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}, {3, 1, [{"id": 6}]}]}                                                           |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
         <BLANKLINE>
     """  # noqa: E501
     coalesced_df = col_df.join(pivoted_df, "column_name", "left").withColumns(
         {
             "changed_nb": f.coalesce(f.col("changed_nb"), f.lit(0)),
             "no_change_nb": f.coalesce(f.col("no_change_nb"), f.lit(0)),
             "only_in_left_nb": f.coalesce(f.col("only_in_left_nb"), f.lit(0)),
@@ -212,18 +219,21 @@
         {
             "column_number": None,
             "column_name": None,
             "counts": None,
             "diff.changed": None,
             "diff.no_change!.value": lambda s: s["left_value"],
             "diff.no_change!.nb": lambda s: s["nb"],
+            "diff.no_change!.sample_ids": lambda s: s["sample_ids"],
             "diff.only_in_left!.value": lambda s: s["left_value"],
             "diff.only_in_left!.nb": lambda s: s["nb"],
+            "diff.only_in_left!.sample_ids": lambda s: s["sample_ids"],
             "diff.only_in_right!.value": lambda s: s["right_value"],
             "diff.only_in_right!.nb": lambda s: s["nb"],
+            "diff.only_in_right!.sample_ids": lambda s: s["sample_ids"],
         },
     )
     return formatted_df
 
 
 @lru_cache()
 def _get_diff_per_col_df_with_cache(diff_result: "DiffResult", max_nb_rows_per_col_state: int) -> DataFrame:
@@ -281,51 +291,51 @@
             <BLANKLINE>
 
     Examples:
         >>> from spark_frame.data_diff.diff_result import _get_test_diff_result
         >>> diff_result = _get_test_diff_result()
         >>> diff_df = diff_result.diff_df_shards[""]
         >>> diff_df.show(truncate=False)
-        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-        |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|
-        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-        |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |
-        |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |
-        |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-        |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-        |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |
-        |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |
-        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
+        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+        |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|__SAMPLE_ID__|
+        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+        |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |[{"id": 1}]  |
+        |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |[{"id": 2}]  |
+        |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 3}]  |
+        |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 4}]  |
+        |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |[{"id": 5}]  |
+        |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |[{"id": 6}]  |
+        +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
         <BLANKLINE>
         >>> diff_result.top_per_col_state_df.show(100)
-        +-----------+-------------+----------+-----------+---+-------+
-        |column_name|        state|left_value|right_value| nb|row_num|
-        +-----------+-------------+----------+-----------+---+-------+
-        |         c1|    no_change|         b|          b|  3|      1|
-        |         c1|    no_change|         a|          a|  1|      2|
-        |         c1| only_in_left|         c|       NULL|  1|      1|
-        |         c1|only_in_right|      NULL|          f|  1|      1|
-        |         c2|      changed|         2|          4|  2|      1|
-        |         c2|      changed|         2|          3|  1|      2|
-        |         c2|    no_change|         1|          1|  1|      1|
-        |         c2| only_in_left|         3|       NULL|  1|      1|
-        |         c2|only_in_right|      NULL|          3|  1|      1|
-        |         c3| only_in_left|         1|       NULL|  2|      1|
-        |         c3| only_in_left|         2|       NULL|  2|      2|
-        |         c3| only_in_left|         3|       NULL|  1|      3|
-        |         c4|only_in_right|      NULL|          1|  2|      1|
-        |         c4|only_in_right|      NULL|          2|  2|      2|
-        |         c4|only_in_right|      NULL|          3|  1|      3|
-        |         id|    no_change|         1|          1|  1|      1|
-        |         id|    no_change|         2|          2|  1|      2|
-        |         id|    no_change|         3|          3|  1|      3|
-        |         id|    no_change|         4|          4|  1|      4|
-        |         id| only_in_left|         5|       NULL|  1|      1|
-        |         id|only_in_right|      NULL|          6|  1|      1|
-        +-----------+-------------+----------+-----------+---+-------+
+        +-----------+-------------+----------+-----------+---+-----------+-------+
+        |column_name|        state|left_value|right_value| nb| sample_ids|row_num|
+        +-----------+-------------+----------+-----------+---+-----------+-------+
+        |         c1|    no_change|         b|          b|  3|[{"id": 2}]|      1|
+        |         c1|    no_change|         a|          a|  1|[{"id": 1}]|      2|
+        |         c1| only_in_left|         c|       NULL|  1|[{"id": 5}]|      1|
+        |         c1|only_in_right|      NULL|          f|  1|[{"id": 6}]|      1|
+        |         c2|      changed|         2|          4|  2|[{"id": 3}]|      1|
+        |         c2|      changed|         2|          3|  1|[{"id": 2}]|      2|
+        |         c2|    no_change|         1|          1|  1|[{"id": 1}]|      1|
+        |         c2| only_in_left|         3|       NULL|  1|[{"id": 5}]|      1|
+        |         c2|only_in_right|      NULL|          3|  1|[{"id": 6}]|      1|
+        |         c3| only_in_left|         1|       NULL|  2|[{"id": 1}]|      1|
+        |         c3| only_in_left|         2|       NULL|  2|[{"id": 3}]|      2|
+        |         c3| only_in_left|         3|       NULL|  1|[{"id": 5}]|      3|
+        |         c4|only_in_right|      NULL|          1|  2|[{"id": 1}]|      1|
+        |         c4|only_in_right|      NULL|          2|  2|[{"id": 3}]|      2|
+        |         c4|only_in_right|      NULL|          3|  1|[{"id": 6}]|      3|
+        |         id|    no_change|         1|          1|  1|[{"id": 1}]|      1|
+        |         id|    no_change|         2|          2|  1|[{"id": 2}]|      2|
+        |         id|    no_change|         3|          3|  1|[{"id": 3}]|      3|
+        |         id|    no_change|         4|          4|  1|[{"id": 4}]|      4|
+        |         id| only_in_left|         5|       NULL|  1|[{"id": 5}]|      1|
+        |         id|only_in_right|      NULL|          6|  1|[{"id": 6}]|      1|
+        +-----------+-------------+----------+-----------+---+-----------+-------+
         <BLANKLINE>
 
         >>> diff_per_col_df = _get_diff_per_col_df(
         ...     diff_result.top_per_col_state_df,
         ...     diff_result.schema_diff_result.column_names,
         ...     max_nb_rows_per_col_state=10)
         >>> from spark_frame import nested
@@ -337,49 +347,53 @@
          |-- counts.changed: long (nullable = false)
          |-- counts.no_change: long (nullable = false)
          |-- counts.only_in_left: long (nullable = false)
          |-- counts.only_in_right: long (nullable = false)
          |-- diff.changed!.left_value: string (nullable = true)
          |-- diff.changed!.right_value: string (nullable = true)
          |-- diff.changed!.nb: long (nullable = false)
+         |-- diff.changed!.sample_ids!: string (nullable = true)
          |-- diff.no_change!.value: string (nullable = true)
          |-- diff.no_change!.nb: long (nullable = false)
+         |-- diff.no_change!.sample_ids!: string (nullable = true)
          |-- diff.only_in_left!.value: string (nullable = true)
          |-- diff.only_in_left!.nb: long (nullable = false)
+         |-- diff.only_in_left!.sample_ids!: string (nullable = true)
          |-- diff.only_in_right!.value: string (nullable = true)
          |-- diff.only_in_right!.nb: long (nullable = false)
+         |-- diff.only_in_right!.sample_ids!: string (nullable = true)
         <BLANKLINE>
         >>> diff_per_col_df.show(truncate=False)
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |column_number|column_name|counts         |diff                                                      |
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1}, {2, 1}, {3, 1}, {4, 1}], [{5, 1}], [{6, 1}]}|
-        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{b, 3}, {a, 1}], [{c, 1}], [{f, 1}]}                |
-        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 4, 2}, {2, 3, 1}], [{1, 1}], [{3, 1}], [{3, 1}]}    |
-        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{1, 2}, {2, 2}, {3, 1}], []}                    |
-        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{1, 2}, {2, 2}, {3, 1}]}                    |
-        +-------------+-----------+---------------+----------------------------------------------------------+
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |column_number|column_name|counts         |diff                                                                                                                                    |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1, [{"id": 1}]}, {2, 1, [{"id": 2}]}, {3, 1, [{"id": 3}]}, {4, 1, [{"id": 4}]}], [{5, 1, [{"id": 5}]}], [{6, 1, [{"id": 6}]}]}|
+        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{b, 3, [{"id": 2}]}, {a, 1, [{"id": 1}]}], [{c, 1, [{"id": 5}]}], [{f, 1, [{"id": 6}]}]}                                          |
+        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 4, 2, [{"id": 3}]}, {2, 3, 1, [{"id": 2}]}], [{1, 1, [{"id": 1}]}], [{3, 1, [{"id": 5}]}], [{3, 1, [{"id": 6}]}]}                 |
+        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}, {3, 1, [{"id": 5}]}], []}                                                           |
+        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}, {3, 1, [{"id": 6}]}]}                                                           |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
         <BLANKLINE>
 
         The following test demonstrates that the arrays in `diff`
         are not guaranteed to be sorted by decreasing frequency
         >>> _get_diff_per_col_df(
         ...     diff_result.top_per_col_state_df.orderBy("nb"),
         ...     diff_result.schema_diff_result.column_names,
         ...     max_nb_rows_per_col_state=10
         ... ).show(truncate=False)
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |column_number|column_name|counts         |diff                                                      |
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1}, {2, 1}, {3, 1}, {4, 1}], [{5, 1}], [{6, 1}]}|
-        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{a, 1}, {b, 3}], [{c, 1}], [{f, 1}]}                |
-        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 3, 1}, {2, 4, 2}], [{1, 1}], [{3, 1}], [{3, 1}]}    |
-        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{3, 1}, {1, 2}, {2, 2}], []}                    |
-        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{3, 1}, {1, 2}, {2, 2}]}                    |
-        +-------------+-----------+---------------+----------------------------------------------------------+
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |column_number|column_name|counts         |diff                                                                                                                                    |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1, [{"id": 1}]}, {2, 1, [{"id": 2}]}, {3, 1, [{"id": 3}]}, {4, 1, [{"id": 4}]}], [{5, 1, [{"id": 5}]}], [{6, 1, [{"id": 6}]}]}|
+        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{a, 1, [{"id": 1}]}, {b, 3, [{"id": 2}]}], [{c, 1, [{"id": 5}]}], [{f, 1, [{"id": 6}]}]}                                          |
+        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 3, 1, [{"id": 2}]}, {2, 4, 2, [{"id": 3}]}], [{1, 1, [{"id": 1}]}], [{3, 1, [{"id": 5}]}], [{3, 1, [{"id": 6}]}]}                 |
+        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{3, 1, [{"id": 5}]}, {1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}], []}                                                           |
+        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{3, 1, [{"id": 6}]}, {1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}]}                                                           |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
         <BLANKLINE>
     """  # noqa: E501
     spark = top_per_col_state_df.sparkSession
     pivoted_df = _get_pivoted_df(top_per_col_state_df, max_nb_rows_per_col_state)
     col_df = _get_col_df(columns, spark)
     df = _format_diff_per_col_df(pivoted_df, col_df)
     return df
```

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/diff_result.py` & `spark_frame-0.5.0/spark_frame/data_diff/diff_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,70 +11,76 @@
 from spark_frame.data_diff.diff_per_col import _get_diff_per_col_df_with_cache
 from spark_frame.data_diff.diff_stats import DiffStats
 from spark_frame.data_diff.export import export_html_diff_report
 from spark_frame.data_diff.package import (
     EXISTS_COL_NAME,
     IS_EQUAL_COL_NAME,
     PREDICATES,
+    SAMPLE_ID_COL_NAME,
     canonize_col,
 )
+from spark_frame.data_diff.sample import _get_sample_df_shards_with_cache
 from spark_frame.data_diff.schema_diff import DiffPrefix, SchemaDiffResult
 from spark_frame.data_diff.special_characters import _restore_special_characters_from_col
-from spark_frame.field_utils import substring_before_last_occurrence
+from spark_frame.field_utils import get_granularity
 from spark_frame.transformations import union_dataframes
 from spark_frame.utils import quote, strip_margin
 
 
 def _unpivot(diff_df: DataFrame) -> DataFrame:
     """Given a diff_df, builds an unpivoted version of it.
     All the values must be cast to STRING to make sure everything fits in the same column.
 
     Examples:
         >>> from spark_frame.data_diff.diff_result import _get_test_intersection_diff_df
         >>> diff_df = _get_test_intersection_diff_df()
         >>> diff_df.show(truncate=False)
-        +-------------------------+-------------------------+
-        |c1                       |c2                       |
-        +-------------------------+-------------------------+
-        |{a, d, false, true, true}|{1, 1, true, true, true} |
-        |{b, a, false, true, true}|{2, 4, false, true, true}|
-        +-------------------------+-------------------------+
+        +------------------------+-------------------------+-------------------------+-------------+
+        |id                      |c1                       |c2                       |__SAMPLE_ID__|
+        +------------------------+-------------------------+-------------------------+-------------+
+        |{1, 1, true, true, true}|{a, d, false, true, true}|{1, 1, true, true, true} |[{"id": 1}]  |
+        |{2, 2, true, true, true}|{a, d, false, true, true}|{2, 4, false, true, true}|[{"id": 2}]  |
+        +------------------------+-------------------------+-------------------------+-------------+
         <BLANKLINE>
-        >>> _unpivot(diff_df).orderBy('column_name').show(truncate=False)
-        +-----------+-------------------------+
-        |column_name|diff                     |
-        +-----------+-------------------------+
-        |c1         |{a, d, false, true, true}|
-        |c1         |{b, a, false, true, true}|
-        |c2         |{1, 1, true, true, true} |
-        |c2         |{2, 4, false, true, true}|
-        +-----------+-------------------------+
+        >>> _unpivot(diff_df).orderBy('column_name', 'diff').show(truncate=False)
+        +-----------+--------------------------------------+
+        |column_name|diff                                  |
+        +-----------+--------------------------------------+
+        |c1         |{a, d, false, true, true, [{"id": 1}]}|
+        |c1         |{a, d, false, true, true, [{"id": 2}]}|
+        |c2         |{1, 1, true, true, true, [{"id": 1}]} |
+        |c2         |{2, 4, false, true, true, [{"id": 2}]}|
+        |id         |{1, 1, true, true, true, [{"id": 1}]} |
+        |id         |{2, 2, true, true, true, [{"id": 2}]} |
+        +-----------+--------------------------------------+
         <BLANKLINE>
     """
 
     diff_df = diff_df.select(
         *[
             f.struct(
                 canonize_col(
-                    diff_df[field.name + ".left_value"],
+                    diff_df[quote(field.name) + ".left_value"],
                     cast(StructType, field.dataType).fields[0],
                 )
                 .cast("STRING")
                 .alias("left_value"),
                 canonize_col(
-                    diff_df[field.name + ".right_value"],
+                    diff_df[quote(field.name) + ".right_value"],
                     cast(StructType, field.dataType).fields[1],
                 )
                 .cast("STRING")
                 .alias("right_value"),
                 diff_df[quote(field.name) + ".is_equal"].alias("is_equal"),
                 diff_df[quote(field.name) + ".exists_left"].alias("exists_left"),
                 diff_df[quote(field.name) + ".exists_right"].alias("exists_right"),
+                diff_df[SAMPLE_ID_COL_NAME].alias("sample_ids"),
             ).alias(field.name)
             for field in diff_df.schema.fields
+            if field.name != SAMPLE_ID_COL_NAME
         ],
     )
 
     unpivoted_df = transformations.unpivot(
         diff_df,
         pivot_columns=[],
         key_alias="column_name",
@@ -135,24 +141,22 @@
 
     @property
     def is_ok(self) -> bool:
         return self.same_schema and self.same_data
 
     @cached_property
     def diff_stats_shards(self) -> Dict[str, DiffStats]:
-        return self._compute_diff_stats()
+        return self._compute_diff_stats_shards()
 
     @cached_property
     def top_per_col_state_df(self) -> DataFrame:
         def generate() -> Generator[DataFrame, None, None]:
             for key, diff_df in self.diff_df_shards.items():
                 keep_cols = [
-                    col_name
-                    for col_name in self.schema_diff_result.column_names
-                    if substring_before_last_occurrence(col_name, "!.") == key
+                    col_name for col_name in self.schema_diff_result.column_names if get_granularity(col_name) == key
                 ]
                 df = self._compute_top_per_col_state_df(diff_df)
                 yield df.where(f.col("column_name").isin(keep_cols))
 
         return union_dataframes(*generate()).localCheckpoint()
 
     def get_diff_per_col_df(self, max_nb_rows_per_col_state: int) -> DataFrame:
@@ -190,51 +194,51 @@
                  |-- diff.only_in_right!.nb: long (nullable = false)
                 <BLANKLINE>
 
         Examples:
             >>> from spark_frame.data_diff.diff_result import _get_test_diff_result
             >>> diff_result = _get_test_diff_result()
             >>> diff_result.diff_df_shards[''].show(truncate=False)
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-            |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-            |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |
-            |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |
-            |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-            |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-            |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |
-            |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+            |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|__SAMPLE_ID__|
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+            |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |[{"id": 1}]  |
+            |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |[{"id": 2}]  |
+            |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 3}]  |
+            |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 4}]  |
+            |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |[{"id": 5}]  |
+            |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |[{"id": 6}]  |
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
             <BLANKLINE>
             >>> diff_result.top_per_col_state_df.show(100)
-            +-----------+-------------+----------+-----------+---+-------+
-            |column_name|        state|left_value|right_value| nb|row_num|
-            +-----------+-------------+----------+-----------+---+-------+
-            |         c1|    no_change|         b|          b|  3|      1|
-            |         c1|    no_change|         a|          a|  1|      2|
-            |         c1| only_in_left|         c|       NULL|  1|      1|
-            |         c1|only_in_right|      NULL|          f|  1|      1|
-            |         c2|      changed|         2|          4|  2|      1|
-            |         c2|      changed|         2|          3|  1|      2|
-            |         c2|    no_change|         1|          1|  1|      1|
-            |         c2| only_in_left|         3|       NULL|  1|      1|
-            |         c2|only_in_right|      NULL|          3|  1|      1|
-            |         c3| only_in_left|         1|       NULL|  2|      1|
-            |         c3| only_in_left|         2|       NULL|  2|      2|
-            |         c3| only_in_left|         3|       NULL|  1|      3|
-            |         c4|only_in_right|      NULL|          1|  2|      1|
-            |         c4|only_in_right|      NULL|          2|  2|      2|
-            |         c4|only_in_right|      NULL|          3|  1|      3|
-            |         id|    no_change|         1|          1|  1|      1|
-            |         id|    no_change|         2|          2|  1|      2|
-            |         id|    no_change|         3|          3|  1|      3|
-            |         id|    no_change|         4|          4|  1|      4|
-            |         id| only_in_left|         5|       NULL|  1|      1|
-            |         id|only_in_right|      NULL|          6|  1|      1|
-            +-----------+-------------+----------+-----------+---+-------+
+            +-----------+-------------+----------+-----------+---+-----------+-------+
+            |column_name|        state|left_value|right_value| nb| sample_ids|row_num|
+            +-----------+-------------+----------+-----------+---+-----------+-------+
+            |         c1|    no_change|         b|          b|  3|[{"id": 2}]|      1|
+            |         c1|    no_change|         a|          a|  1|[{"id": 1}]|      2|
+            |         c1| only_in_left|         c|       NULL|  1|[{"id": 5}]|      1|
+            |         c1|only_in_right|      NULL|          f|  1|[{"id": 6}]|      1|
+            |         c2|      changed|         2|          4|  2|[{"id": 3}]|      1|
+            |         c2|      changed|         2|          3|  1|[{"id": 2}]|      2|
+            |         c2|    no_change|         1|          1|  1|[{"id": 1}]|      1|
+            |         c2| only_in_left|         3|       NULL|  1|[{"id": 5}]|      1|
+            |         c2|only_in_right|      NULL|          3|  1|[{"id": 6}]|      1|
+            |         c3| only_in_left|         1|       NULL|  2|[{"id": 1}]|      1|
+            |         c3| only_in_left|         2|       NULL|  2|[{"id": 3}]|      2|
+            |         c3| only_in_left|         3|       NULL|  1|[{"id": 5}]|      3|
+            |         c4|only_in_right|      NULL|          1|  2|[{"id": 1}]|      1|
+            |         c4|only_in_right|      NULL|          2|  2|[{"id": 3}]|      2|
+            |         c4|only_in_right|      NULL|          3|  1|[{"id": 6}]|      3|
+            |         id|    no_change|         1|          1|  1|[{"id": 1}]|      1|
+            |         id|    no_change|         2|          2|  1|[{"id": 2}]|      2|
+            |         id|    no_change|         3|          3|  1|[{"id": 3}]|      3|
+            |         id|    no_change|         4|          4|  1|[{"id": 4}]|      4|
+            |         id| only_in_left|         5|       NULL|  1|[{"id": 5}]|      1|
+            |         id|only_in_right|      NULL|          6|  1|[{"id": 6}]|      1|
+            +-----------+-------------+----------+-----------+---+-----------+-------+
             <BLANKLINE>
 
             >>> diff_per_col_df = diff_result.get_diff_per_col_df(max_nb_rows_per_col_state=10)
             >>> from spark_frame import nested
             >>> nested.print_schema(diff_per_col_df)
             root
              |-- column_number: integer (nullable = true)
@@ -243,35 +247,42 @@
              |-- counts.changed: long (nullable = false)
              |-- counts.no_change: long (nullable = false)
              |-- counts.only_in_left: long (nullable = false)
              |-- counts.only_in_right: long (nullable = false)
              |-- diff.changed!.left_value: string (nullable = true)
              |-- diff.changed!.right_value: string (nullable = true)
              |-- diff.changed!.nb: long (nullable = false)
+             |-- diff.changed!.sample_ids!: string (nullable = true)
              |-- diff.no_change!.value: string (nullable = true)
              |-- diff.no_change!.nb: long (nullable = false)
+             |-- diff.no_change!.sample_ids!: string (nullable = true)
              |-- diff.only_in_left!.value: string (nullable = true)
              |-- diff.only_in_left!.nb: long (nullable = false)
+             |-- diff.only_in_left!.sample_ids!: string (nullable = true)
              |-- diff.only_in_right!.value: string (nullable = true)
              |-- diff.only_in_right!.nb: long (nullable = false)
+             |-- diff.only_in_right!.sample_ids!: string (nullable = true)
             <BLANKLINE>
             >>> diff_per_col_df.show(truncate=False)
-            +-------------+-----------+---------------+----------------------------------------------------------+
-            |column_number|column_name|counts         |diff                                                      |
-            +-------------+-----------+---------------+----------------------------------------------------------+
-            |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1}, {2, 1}, {3, 1}, {4, 1}], [{5, 1}], [{6, 1}]}|
-            |1            |c1         |{6, 0, 4, 1, 1}|{[], [{b, 3}, {a, 1}], [{c, 1}], [{f, 1}]}                |
-            |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 4, 2}, {2, 3, 1}], [{1, 1}], [{3, 1}], [{3, 1}]}    |
-            |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{1, 2}, {2, 2}, {3, 1}], []}                    |
-            |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{1, 2}, {2, 2}, {3, 1}]}                    |
-            +-------------+-----------+---------------+----------------------------------------------------------+
+            +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+            |column_number|column_name|counts         |diff                                                                                                                                    |
+            +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+            |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1, [{"id": 1}]}, {2, 1, [{"id": 2}]}, {3, 1, [{"id": 3}]}, {4, 1, [{"id": 4}]}], [{5, 1, [{"id": 5}]}], [{6, 1, [{"id": 6}]}]}|
+            |1            |c1         |{6, 0, 4, 1, 1}|{[], [{b, 3, [{"id": 2}]}, {a, 1, [{"id": 1}]}], [{c, 1, [{"id": 5}]}], [{f, 1, [{"id": 6}]}]}                                          |
+            |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 4, 2, [{"id": 3}]}, {2, 3, 1, [{"id": 2}]}], [{1, 1, [{"id": 1}]}], [{3, 1, [{"id": 5}]}], [{3, 1, [{"id": 6}]}]}                 |
+            |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}, {3, 1, [{"id": 5}]}], []}                                                           |
+            |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}, {3, 1, [{"id": 6}]}]}                                                           |
+            +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
             <BLANKLINE>
         """  # noqa: E501
         return _get_diff_per_col_df_with_cache(self, max_nb_rows_per_col_state)
 
+    def get_sample_df_shards(self, max_nb_rows_per_col_state: int) -> List[DataFrame]:
+        return _get_sample_df_shards_with_cache(self, max_nb_rows_per_col_state)
+
     def _compute_diff_stats_shard(self, diff_df_shard: DataFrame) -> DiffStats:
         """Given a diff_df and its list of join_cols, return stats about the number of differing or missing rows
 
         >>> from spark_frame.data_diff.diff_result import _get_test_diff_result
         >>> diff_result = _get_test_diff_result()
         >>> diff_result.diff_df_shards[''].select('__EXISTS__', '__IS_EQUAL__').show()
         +-------------+------------+
@@ -281,15 +292,15 @@
         | {true, true}|       false|
         | {true, true}|       false|
         | {true, true}|       false|
         |{true, false}|       false|
         |{false, true}|       false|
         +-------------+------------+
         <BLANKLINE>
-        >>> diff_result._compute_diff_stats()['']
+        >>> diff_result._compute_diff_stats_shards()['']
         DiffStats(total=6, no_change=1, changed=3, in_left=5, in_right=5, only_in_left=1, only_in_right=1)
         """
         res_df = diff_df_shard.select(
             f.count(f.lit(1)).alias("total"),
             f.sum(
                 f.when(
                     PREDICATES.present_in_both & PREDICATES.row_is_equal,
@@ -320,15 +331,15 @@
             ),
         )
         res = res_df.collect()
         return DiffStats(
             **{k: (v if v is not None else 0) for k, v in res[0].asDict().items()},
         )
 
-    def _compute_diff_stats(self) -> Dict[str, DiffStats]:
+    def _compute_diff_stats_shards(self) -> Dict[str, DiffStats]:
         """Given a diff_df and its list of join_cols, return stats about the number of differing or missing rows
 
         >>> from spark_frame.data_diff.diff_result import _get_test_diff_result
         >>> diff_result = _get_test_diff_result()
         >>> diff_result.diff_df_shards[''].select('__EXISTS__', '__IS_EQUAL__').show()
         +-------------+------------+
         |   __EXISTS__|__IS_EQUAL__|
@@ -337,15 +348,15 @@
         | {true, true}|       false|
         | {true, true}|       false|
         | {true, true}|       false|
         |{true, false}|       false|
         |{false, true}|       false|
         +-------------+------------+
         <BLANKLINE>
-        >>> diff_result._compute_diff_stats()['']
+        >>> diff_result._compute_diff_stats_shards()['']
         DiffStats(total=6, no_change=1, changed=3, in_left=5, in_right=5, only_in_left=1, only_in_right=1)
         """
         return {
             key: self._compute_diff_stats_shard(diff_df_shard) for key, diff_df_shard in self.diff_df_shards.items()
         }
 
     def _compute_top_per_col_state_df(self, diff_df: DataFrame) -> DataFrame:
@@ -357,79 +368,81 @@
         - At most `max_nb_rows_per_col_state` per tuple (column_name, state). Rows with the highest "nb" are kept first.
 
         Examples:
             >>> from spark_frame.data_diff.diff_result import _get_test_diff_result
             >>> _diff_result = _get_test_diff_result()
             >>> diff_df = _diff_result.diff_df_shards['']
             >>> diff_df.show(truncate=False)
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-            |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-            |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |
-            |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |
-            |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-            |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-            |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |
-            |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+            |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|__SAMPLE_ID__|
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+            |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |[{"id": 1}]  |
+            |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |[{"id": 2}]  |
+            |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 3}]  |
+            |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 4}]  |
+            |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |[{"id": 5}]  |
+            |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |[{"id": 6}]  |
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
             <BLANKLINE>
             >>> (_diff_result._compute_top_per_col_state_df(diff_df)
             ...  .orderBy("column_name", "state", "left_value", "right_value")
             ... ).show(100)
-            +-----------+-------------+----------+-----------+---+-------+
-            |column_name|        state|left_value|right_value| nb|row_num|
-            +-----------+-------------+----------+-----------+---+-------+
-            |         c1|    no_change|         a|          a|  1|      2|
-            |         c1|    no_change|         b|          b|  3|      1|
-            |         c1| only_in_left|         c|       NULL|  1|      1|
-            |         c1|only_in_right|      NULL|          f|  1|      1|
-            |         c2|      changed|         2|          3|  1|      2|
-            |         c2|      changed|         2|          4|  2|      1|
-            |         c2|    no_change|         1|          1|  1|      1|
-            |         c2| only_in_left|         3|       NULL|  1|      1|
-            |         c2|only_in_right|      NULL|          3|  1|      1|
-            |         c3| only_in_left|         1|       NULL|  2|      1|
-            |         c3| only_in_left|         2|       NULL|  2|      2|
-            |         c3| only_in_left|         3|       NULL|  1|      3|
-            |         c4|only_in_right|      NULL|          1|  2|      1|
-            |         c4|only_in_right|      NULL|          2|  2|      2|
-            |         c4|only_in_right|      NULL|          3|  1|      3|
-            |         id|    no_change|         1|          1|  1|      1|
-            |         id|    no_change|         2|          2|  1|      2|
-            |         id|    no_change|         3|          3|  1|      3|
-            |         id|    no_change|         4|          4|  1|      4|
-            |         id| only_in_left|         5|       NULL|  1|      1|
-            |         id|only_in_right|      NULL|          6|  1|      1|
-            +-----------+-------------+----------+-----------+---+-------+
+            +-----------+-------------+----------+-----------+---+-----------+-------+
+            |column_name|        state|left_value|right_value| nb| sample_ids|row_num|
+            +-----------+-------------+----------+-----------+---+-----------+-------+
+            |         c1|    no_change|         a|          a|  1|[{"id": 1}]|      2|
+            |         c1|    no_change|         b|          b|  3|[{"id": 2}]|      1|
+            |         c1| only_in_left|         c|       NULL|  1|[{"id": 5}]|      1|
+            |         c1|only_in_right|      NULL|          f|  1|[{"id": 6}]|      1|
+            |         c2|      changed|         2|          3|  1|[{"id": 2}]|      2|
+            |         c2|      changed|         2|          4|  2|[{"id": 3}]|      1|
+            |         c2|    no_change|         1|          1|  1|[{"id": 1}]|      1|
+            |         c2| only_in_left|         3|       NULL|  1|[{"id": 5}]|      1|
+            |         c2|only_in_right|      NULL|          3|  1|[{"id": 6}]|      1|
+            |         c3| only_in_left|         1|       NULL|  2|[{"id": 1}]|      1|
+            |         c3| only_in_left|         2|       NULL|  2|[{"id": 3}]|      2|
+            |         c3| only_in_left|         3|       NULL|  1|[{"id": 5}]|      3|
+            |         c4|only_in_right|      NULL|          1|  2|[{"id": 1}]|      1|
+            |         c4|only_in_right|      NULL|          2|  2|[{"id": 3}]|      2|
+            |         c4|only_in_right|      NULL|          3|  1|[{"id": 6}]|      3|
+            |         id|    no_change|         1|          1|  1|[{"id": 1}]|      1|
+            |         id|    no_change|         2|          2|  1|[{"id": 2}]|      2|
+            |         id|    no_change|         3|          3|  1|[{"id": 3}]|      3|
+            |         id|    no_change|         4|          4|  1|[{"id": 4}]|      4|
+            |         id| only_in_left|         5|       NULL|  1|[{"id": 5}]|      1|
+            |         id|only_in_right|      NULL|          6|  1|[{"id": 6}]|      1|
+            +-----------+-------------+----------+-----------+---+-----------+-------+
             <BLANKLINE>
         """  # noqa: E501
-        unpivoted_diff_df = _unpivot(diff_df.drop(IS_EQUAL_COL_NAME, EXISTS_COL_NAME))
+        diff_df = diff_df.drop(IS_EQUAL_COL_NAME, EXISTS_COL_NAME)
+        unpivoted_diff_df = _unpivot(diff_df)
 
         only_in_left = f.col("diff")["exists_left"] & ~f.col("diff")["exists_right"]
         only_in_right = ~f.col("diff")["exists_left"] & f.col("diff")["exists_right"]
         exists_in_left_or_right = f.col("diff")["exists_left"] | f.col("diff")["exists_right"]
 
         df_1 = unpivoted_diff_df.select(
             "column_name",
             f.when(only_in_left, f.lit("only_in_left"))
             .when(only_in_right, f.lit("only_in_right"))
             .when(f.col("diff")["is_equal"], f.lit("no_change"))
             .otherwise(f.lit("changed"))
             .alias("state"),
             "diff.left_value",
             "diff.right_value",
+            "diff.sample_ids",
         ).where(exists_in_left_or_right)
         window = Window.partitionBy("column_name", "state").orderBy(
             f.col("nb").desc(),
             f.col("left_value"),
             f.col("right_value"),
         )
         df_2 = (
             df_1.groupBy("column_name", "state", "left_value", "right_value")
-            .agg(f.count(f.lit(1)).alias("nb"))
+            .agg(f.count(f.lit(1)).alias("nb"), f.first("sample_ids").alias("sample_ids"))
             .withColumn("row_num", f.row_number().over(window))
         )
         return df_2
 
     def display(
         self,
         show_examples: bool = False,
@@ -602,26 +615,34 @@
     from pyspark.sql import SparkSession
 
     spark = SparkSession.builder.appName("doctest").getOrCreate()
     diff_df = spark.sql(
         """
         SELECT INLINE(ARRAY(
             STRUCT(
+                STRUCT(1 as left_value, 1 as right_value, True as is_equal,
+                       True as exists_left, True as exists_right
+                ) as id,
                 STRUCT("a" as left_value, "d" as right_value, False as is_equal,
                        True as exists_left, True as exists_right
                 ) as c1,
                 STRUCT(1 as left_value, 1 as right_value, True as is_equal,
                        True as exists_left, True as exists_right
-                ) as c2
+                ) as c2,
+                ARRAY('{"id": 1}') as __SAMPLE_ID__
             ),
             STRUCT(
-                STRUCT("b" as left_value, "a" as right_value, False as is_equal,
+                STRUCT(2 as left_value, 2 as right_value, True as is_equal,
+                       True as exists_left, True as exists_right
+                ) as id,
+                STRUCT("a" as left_value, "d" as right_value, False as is_equal,
                        True as exists_left, True as exists_right
                 ) as c1,
                 STRUCT(2 as left_value, 4 as right_value, False as is_equal,
                        True as exists_left, True as exists_right
-                ) as c2
+                ) as c2,
+                ARRAY('{"id": 2}') as __SAMPLE_ID__
             )
         ))
     """,
     )
     return diff_df
```

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/diff_result_analyzer.py` & `spark_frame-0.5.0/spark_frame/data_diff/diff_result_analyzer.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,37 +57,37 @@
 
         Examples:
             >>> from spark_frame.data_diff.diff_result import _get_test_diff_result
             >>> diff_result = _get_test_diff_result()
             >>> analyzer = DiffResultAnalyzer(DiffFormatOptions(left_df_alias="before", right_df_alias="after"))
             >>> diff_df = diff_result.diff_df_shards[""]
             >>> diff_df.show(truncate=False)
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-            |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-            |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |
-            |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |
-            |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-            |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-            |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |
-            |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |
-            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+            |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|__SAMPLE_ID__|
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+            |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |[{"id": 1}]  |
+            |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |[{"id": 2}]  |
+            |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 3}]  |
+            |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 4}]  |
+            |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |[{"id": 5}]  |
+            |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |[{"id": 6}]  |
+            +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
             <BLANKLINE>
             >>> analyzer = DiffResultAnalyzer(DiffFormatOptions(left_df_alias="before", right_df_alias="after"))
             >>> diff_per_col_df = _get_test_diff_per_col_df()
             >>> diff_per_col_df.show(truncate=False)
-            +-------------+-----------+---------------+----------------------------------------------------------+
-            |column_number|column_name|counts         |diff                                                      |
-            +-------------+-----------+---------------+----------------------------------------------------------+
-            |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1}, {2, 1}, {3, 1}, {4, 1}], [{5, 1}], [{6, 1}]}|
-            |1            |c1         |{6, 0, 4, 1, 1}|{[], [{a, 1}, {b, 3}], [{c, 1}], [{f, 1}]}                |
-            |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 3, 1}, {2, 4, 2}], [{1, 1}], [{3, 1}], [{3, 1}]}    |
-            |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{3, 1}, {1, 2}, {2, 2}], []}                    |
-            |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{3, 1}, {1, 2}, {2, 2}]}                    |
-            +-------------+-----------+---------------+----------------------------------------------------------+
+            +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+            |column_number|column_name|counts         |diff                                                                                                                                    |
+            +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+            |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1, [{"id": 1}]}, {2, 1, [{"id": 2}]}, {3, 1, [{"id": 3}]}, {4, 1, [{"id": 4}]}], [{5, 1, [{"id": 5}]}], [{6, 1, [{"id": 6}]}]}|
+            |1            |c1         |{6, 0, 4, 1, 1}|{[], [{a, 1, [{"id": 1}]}, {b, 3, [{"id": 2}]}], [{c, 1, [{"id": 5}]}], [{f, 1, [{"id": 6}]}]}                                          |
+            |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 3, 1, [{"id": 2}]}, {2, 4, 2, [{"id": 3}]}], [{1, 1, [{"id": 1}]}], [{3, 1, [{"id": 5}]}], [{3, 1, [{"id": 6}]}]}                 |
+            |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{3, 1, [{"id": 5}]}, {1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}], []}                                                           |
+            |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{3, 1, [{"id": 6}]}, {1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}]}                                                           |
+            +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
             <BLANKLINE>
             >>> analyzer._display_diff_examples(diff_df, diff_per_col_df, join_cols = ['id'])
             Detailed examples :
             'c2' : 3 rows
             +---+----------+---------+
             | id|before__c2|after__c2|
             +---+----------+---------+
@@ -125,53 +125,57 @@
         we display examples of rows where this column changed, along with all the other columns
         that changed in this diff.
 
         Example:
 
         >>> diff_per_col_df = _get_test_diff_per_col_df()
         >>> diff_per_col_df.show(truncate=False)
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |column_number|column_name|counts         |diff                                                      |
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1}, {2, 1}, {3, 1}, {4, 1}], [{5, 1}], [{6, 1}]}|
-        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{a, 1}, {b, 3}], [{c, 1}], [{f, 1}]}                |
-        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 3, 1}, {2, 4, 2}], [{1, 1}], [{3, 1}], [{3, 1}]}    |
-        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{3, 1}, {1, 2}, {2, 2}], []}                    |
-        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{3, 1}, {1, 2}, {2, 2}]}                    |
-        +-------------+-----------+---------------+----------------------------------------------------------+
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |column_number|column_name|counts         |diff                                                                                                                                    |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1, [{"id": 1}]}, {2, 1, [{"id": 2}]}, {3, 1, [{"id": 3}]}, {4, 1, [{"id": 4}]}], [{5, 1, [{"id": 5}]}], [{6, 1, [{"id": 6}]}]}|
+        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{a, 1, [{"id": 1}]}, {b, 3, [{"id": 2}]}], [{c, 1, [{"id": 5}]}], [{f, 1, [{"id": 6}]}]}                                          |
+        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 3, 1, [{"id": 2}]}, {2, 4, 2, [{"id": 3}]}], [{1, 1, [{"id": 1}]}], [{3, 1, [{"id": 5}]}], [{3, 1, [{"id": 6}]}]}                 |
+        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{3, 1, [{"id": 5}]}, {1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}], []}                                                           |
+        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{3, 1, [{"id": 6}]}, {1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}]}                                                           |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
         <BLANKLINE>
         >>> from spark_frame import nested
         >>> nested.print_schema(diff_per_col_df)
         root
          |-- column_number: integer (nullable = true)
          |-- column_name: string (nullable = true)
          |-- counts.total: long (nullable = false)
          |-- counts.changed: long (nullable = false)
          |-- counts.no_change: long (nullable = false)
          |-- counts.only_in_left: long (nullable = false)
          |-- counts.only_in_right: long (nullable = false)
          |-- diff.changed!.left_value: string (nullable = true)
          |-- diff.changed!.right_value: string (nullable = true)
          |-- diff.changed!.nb: long (nullable = false)
+         |-- diff.changed!.sample_ids!: string (nullable = true)
          |-- diff.no_change!.value: string (nullable = true)
          |-- diff.no_change!.nb: long (nullable = false)
+         |-- diff.no_change!.sample_ids!: string (nullable = true)
          |-- diff.only_in_left!.value: string (nullable = true)
          |-- diff.only_in_left!.nb: long (nullable = false)
+         |-- diff.only_in_left!.sample_ids!: string (nullable = true)
          |-- diff.only_in_right!.value: string (nullable = true)
          |-- diff.only_in_right!.nb: long (nullable = false)
+         |-- diff.only_in_right!.sample_ids!: string (nullable = true)
         <BLANKLINE>
         >>> DiffResultAnalyzer._display_changed(diff_per_col_df)
         +-----------+-------------+----------+-----------+--------------+
         |column_name|total_nb_diff|left_value|right_value|nb_differences|
         +-----------+-------------+----------+-----------+--------------+
         |c2         |3            |2         |4          |2             |
         |c2         |3            |2         |3          |1             |
         +-----------+-------------+----------+-----------+--------------+
         <BLANKLINE>
-        """
+        """  # noqa: E501
         df = diff_per_col_df.where(_counts_changed_col() > 0)
         df = df.select(
             "column_name",
             _counts_changed_col().alias("total_nb_diff"),
             f.explode("diff.changed").alias("diff"),
         ).orderBy("column_number", f.desc(_diff_nb_col()))
         df = df.select(
@@ -195,43 +199,47 @@
         we display examples of rows where this column changed, along with all the other columns
         that changed in this diff.
 
         Example:
 
         >>> diff_per_col_df = _get_test_diff_per_col_df()
         >>> diff_per_col_df.show(truncate=False)
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |column_number|column_name|counts         |diff                                                      |
-        +-------------+-----------+---------------+----------------------------------------------------------+
-        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1}, {2, 1}, {3, 1}, {4, 1}], [{5, 1}], [{6, 1}]}|
-        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{a, 1}, {b, 3}], [{c, 1}], [{f, 1}]}                |
-        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 3, 1}, {2, 4, 2}], [{1, 1}], [{3, 1}], [{3, 1}]}    |
-        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{3, 1}, {1, 2}, {2, 2}], []}                    |
-        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{3, 1}, {1, 2}, {2, 2}]}                    |
-        +-------------+-----------+---------------+----------------------------------------------------------+
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |column_number|column_name|counts         |diff                                                                                                                                    |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
+        |0            |id         |{6, 0, 4, 1, 1}|{[], [{1, 1, [{"id": 1}]}, {2, 1, [{"id": 2}]}, {3, 1, [{"id": 3}]}, {4, 1, [{"id": 4}]}], [{5, 1, [{"id": 5}]}], [{6, 1, [{"id": 6}]}]}|
+        |1            |c1         |{6, 0, 4, 1, 1}|{[], [{a, 1, [{"id": 1}]}, {b, 3, [{"id": 2}]}], [{c, 1, [{"id": 5}]}], [{f, 1, [{"id": 6}]}]}                                          |
+        |2            |c2         |{6, 3, 1, 1, 1}|{[{2, 3, 1, [{"id": 2}]}, {2, 4, 2, [{"id": 3}]}], [{1, 1, [{"id": 1}]}], [{3, 1, [{"id": 5}]}], [{3, 1, [{"id": 6}]}]}                 |
+        |3            |c3         |{5, 0, 0, 5, 0}|{[], [], [{3, 1, [{"id": 5}]}, {1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}], []}                                                           |
+        |4            |c4         |{5, 0, 0, 0, 5}|{[], [], [], [{3, 1, [{"id": 6}]}, {1, 2, [{"id": 1}]}, {2, 2, [{"id": 3}]}]}                                                           |
+        +-------------+-----------+---------------+----------------------------------------------------------------------------------------------------------------------------------------+
         <BLANKLINE>
         >>> from spark_frame import nested
         >>> nested.print_schema(diff_per_col_df)
         root
          |-- column_number: integer (nullable = true)
          |-- column_name: string (nullable = true)
          |-- counts.total: long (nullable = false)
          |-- counts.changed: long (nullable = false)
          |-- counts.no_change: long (nullable = false)
          |-- counts.only_in_left: long (nullable = false)
          |-- counts.only_in_right: long (nullable = false)
          |-- diff.changed!.left_value: string (nullable = true)
          |-- diff.changed!.right_value: string (nullable = true)
          |-- diff.changed!.nb: long (nullable = false)
+         |-- diff.changed!.sample_ids!: string (nullable = true)
          |-- diff.no_change!.value: string (nullable = true)
          |-- diff.no_change!.nb: long (nullable = false)
+         |-- diff.no_change!.sample_ids!: string (nullable = true)
          |-- diff.only_in_left!.value: string (nullable = true)
          |-- diff.only_in_left!.nb: long (nullable = false)
+         |-- diff.only_in_left!.sample_ids!: string (nullable = true)
          |-- diff.only_in_right!.value: string (nullable = true)
          |-- diff.only_in_right!.nb: long (nullable = false)
+         |-- diff.only_in_right!.sample_ids!: string (nullable = true)
         <BLANKLINE>
         >>> DiffResultAnalyzer._display_only_in_left_or_right(diff_per_col_df, "left")
         +-----------+-----+---+
         |column_name|value|nb |
         +-----------+-----+---+
         |id         |5    |1  |
         |c1         |c    |1  |
@@ -250,15 +258,15 @@
         |c2         |3    |1  |
         |c4         |3    |1  |
         |c4         |1    |2  |
         |c4         |2    |2  |
         +-----------+-----+---+
         <BLANKLINE>
 
-        """
+        """  # noqa: E501
         df = diff_per_col_df.select(
             "column_name",
             f.explode(f"diff.only_in_{left_or_right}").alias("diff"),
         )
         df = df.select(
             "column_name",
             f.col("diff.value").alias("value"),
@@ -321,23 +329,26 @@
                 print(f"Most frequent values in '{right_df_alias}' for each column :")
                 self._display_only_in_left_or_right(diff_per_col_df, "right")
 
     def get_diff_result_summary(self, diff_result: DiffResult) -> DiffResultSummary:
         diff_per_col_df = diff_result.get_diff_per_col_df(
             max_nb_rows_per_col_state=self.diff_format_options.nb_top_values_kept_per_column,
         )
+        sample_df_shards = diff_result.get_sample_df_shards(
+            max_nb_rows_per_col_state=self.diff_format_options.nb_top_values_kept_per_column,
+        )
         summary = DiffResultSummary(
             left_df_alias=self.diff_format_options.left_df_alias,
             right_df_alias=self.diff_format_options.right_df_alias,
             diff_per_col_df=diff_per_col_df,
+            sample_df_shards=sample_df_shards,
             schema_diff_result=diff_result.schema_diff_result,
             join_cols=diff_result.join_cols,
             same_schema=diff_result.same_schema,
             same_data=diff_result.same_data,
-            is_ok=diff_result.is_ok,
             total_nb_rows=diff_result.total_nb_rows,
         )
         return summary
 
     def get_diff_per_col_df(
         self,
         diff_result: DiffResult,
```

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/diff_result_summary.py` & `spark_frame-0.5.0/spark_frame/data_diff/diff_result_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 
 
 @dataclass
 class DiffResultSummary:
     left_df_alias: str
     right_df_alias: str
     diff_per_col_df: DataFrame
+    sample_df_shards: List[DataFrame]
 
     schema_diff_result: SchemaDiffResult
     join_cols: List[str]
     same_schema: bool
     same_data: bool
-    is_ok: bool
     total_nb_rows: int
```

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/diff_stats.py` & `spark_frame-0.5.0/spark_frame/data_diff/diff_stats.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/export.py` & `spark_frame-0.5.0/spark_frame/data_diff/export.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,21 +10,29 @@
 
 def export_html_diff_report(
     diff_result_summary: DiffResultSummary,
     title: Optional[str],
     output_file_path: str,
     encoding: str,
 ) -> None:
-    load_external_module("data_diff_viewer", version_constraint="0.2.*")
+    load_external_module("data_diff_viewer", version_constraint="0.3.*")
     from data_diff_viewer import DiffSummary, generate_report_string
 
     with tempfile.TemporaryDirectory() as temp_dir:
         temp_dir_path = Path(temp_dir)
         diff_per_col_parquet_path = temp_dir_path / "diff_per_col"
-        diff_result_summary.diff_per_col_df.write.parquet(str(temp_dir_path / "diff_per_col"))
+        diff_per_col_parquet_glob_path = diff_per_col_parquet_path / "*.parquet"
+        diff_result_summary.diff_per_col_df.write.parquet(str(diff_per_col_parquet_path))
+
+        sample_parquet_glob_paths = []
+        for index, sample_df in enumerate(diff_result_summary.sample_df_shards):
+            sample_parquet_path = temp_dir_path / f"sample_{index}"
+            sample_parquet_glob_paths.append(sample_parquet_path / "*.parquet")
+            sample_df.write.parquet(str(sample_parquet_path))
+
         if title is None:
             report_title = f"{diff_result_summary.left_df_alias} vs {diff_result_summary.right_df_alias}"
         else:
             report_title = title
         column_names_diff = {k: v.value for k, v in diff_result_summary.schema_diff_result.column_names_diff.items()}
         diff_summary = DiffSummary(
             generated_with=f"{spark_frame.__name__}:{spark_frame.__version__}",
@@ -37,11 +45,12 @@
             same_data=diff_result_summary.same_data,
             total_nb_rows=diff_result_summary.total_nb_rows,
         )
         report = generate_report_string(
             report_title,
             diff_summary,
             temp_dir_path,
-            diff_per_col_parquet_path / "*.parquet",
+            diff_per_col_parquet_glob_path,
+            sample_parquet_glob_paths,
         )
         write_file(report, output_file_path, mode="overwrite", encoding=encoding)
         print(f"Report exported as {output_file_path}")
```

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/package.py` & `spark_frame-0.5.0/spark_frame/data_diff/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from pyspark.sql import Column, DataFrame
 from pyspark.sql import functions as f
 from pyspark.sql.types import StructField
 
 from spark_frame.data_type_utils import is_repeated
 
-MAGIC_HASH_COL_NAME = "__MAGIC_HASH__"
 EXISTS_COL_NAME = "__EXISTS__"
 IS_EQUAL_COL_NAME = "__IS_EQUAL__"
+SAMPLE_ID_COL_NAME = "__SAMPLE_ID__"
 STRUCT_SEPARATOR_REPLACEMENT = "__STRUCT__"
 REPETITION_MARKER_REPLACEMENT = "__ARRAY__"
 
 A = TypeVar("A")
 B = TypeVar("B")
 
 
@@ -62,32 +62,32 @@
 
     :param col: the SchemaField object
     :param schema_field: the parent DataFrame
     :return: a Column
     """
     if is_repeated(schema_field):
         col = f.when(~col.isNull(), f.to_json(col))
-    return col
+    return col.cast("STRING")
 
 
 @lru_cache
 def _get_test_diff_df() -> DataFrame:
     """
     >>> from spark_frame.data_diff.package import _get_test_diff_df
     >>> _get_test_diff_df().show(truncate=False)
-    +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-    |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|
-    +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
-    |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |
-    |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |
-    |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-    |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |
-    |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |
-    |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |
-    +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+
+    +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+    |id                           |c1                           |c2                           |c3                               |c4                               |__EXISTS__   |__IS_EQUAL__|__SAMPLE_ID__|
+    +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
+    |{1, 1, true, true, true}     |{a, a, true, true, true}     |{1, 1, true, true, true}     |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |true        |[{"id": 1}]  |
+    |{2, 2, true, true, true}     |{b, b, true, true, true}     |{2, 3, false, true, true}    |{1, NULL, false, true, false}    |{NULL, 1, false, false, true}    |{true, true} |false       |[{"id": 2}]  |
+    |{3, 3, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 3}]  |
+    |{4, 4, true, true, true}     |{b, b, true, true, true}     |{2, 4, false, true, true}    |{2, NULL, false, true, false}    |{NULL, 2, false, false, true}    |{true, true} |false       |[{"id": 4}]  |
+    |{5, NULL, false, true, false}|{c, NULL, false, true, false}|{3, NULL, false, true, false}|{3, NULL, false, true, false}    |{NULL, NULL, false, false, false}|{true, false}|false       |[{"id": 5}]  |
+    |{NULL, 6, false, false, true}|{NULL, f, false, false, true}|{NULL, 3, false, false, true}|{NULL, NULL, false, false, false}|{NULL, 3, false, false, true}    |{false, true}|false       |[{"id": 6}]  |
+    +-----------------------------+-----------------------------+-----------------------------+---------------------------------+---------------------------------+-------------+------------+-------------+
     <BLANKLINE>
     """  # noqa: E501
     from pyspark.sql import SparkSession
 
     spark = SparkSession.builder.appName("doctest").getOrCreate()
     diff_df = spark.sql(
         """
@@ -98,115 +98,121 @@
                 ) as id,
                 STRUCT("a" as left_value, "a" as right_value, True as is_equal,
                        True as exists_left, True as exists_right
                 ) as c1,
                 STRUCT(1 as left_value, 1 as right_value, True as is_equal,
                        True as exists_left, True as exists_right
                 ) as c2,
-                STRUCT(1 as left_value, NULL as right_value, False as is_equal,
+                STRUCT(1 as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        True as exists_left, False as exists_right
                 ) as c3,
-                STRUCT(NULL as left_value, 1 as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, 1 as right_value, False as is_equal,
                        False as exists_left, True as exists_right
                 ) as c4,
                 STRUCT(True as left_value, True as right_value) as __EXISTS__,
-                TRUE as __IS_EQUAL__
+                TRUE as __IS_EQUAL__,
+                ARRAY('{"id": 1}') as __SAMPLE_ID__
             ),
             STRUCT(
                 STRUCT(2 as left_value, 2 as right_value, True as is_equal,
                        True as exists_left, True as exists_right
                 ) as id,
                 STRUCT("b" as left_value, "b" as right_value, True as is_equal,
                        True as exists_left, True as exists_right
                 ) as c1,
                 STRUCT(2 as left_value, 3 as right_value, False as is_equal,
                        True as exists_left, True as exists_right
                 ) as c2,
-                STRUCT(1 as left_value, NULL as right_value, False as is_equal,
+                STRUCT(1 as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        True as exists_left, False as exists_right
                 ) as c3,
-                STRUCT(NULL as left_value, 1 as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, 1 as right_value, False as is_equal,
                        False as exists_left, True as exists_right
                 ) as c4,
                 STRUCT(True as left_value, True as right_value) as __EXISTS__,
-                FALSE as __IS_EQUAL__
+                FALSE as __IS_EQUAL__,
+                ARRAY('{"id": 2}') as __SAMPLE_ID__
             ),
             STRUCT(
                 STRUCT(3 as left_value, 3 as right_value, True as is_equal,
                        True as exists_left, True as exists_right
                 ) as id,
                 STRUCT("b" as left_value, "b" as right_value, True as is_equal,
                        True as exists_left, True as exists_right
                 ) as c1,
                 STRUCT(2 as left_value, 4 as right_value, False as is_equal,
                        True as exists_left, True as exists_right
                 ) as c2,
-                STRUCT(2 as left_value, NULL as right_value, False as is_equal,
+                STRUCT(2 as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        True as exists_left, False as exists_right
                 ) as c3,
-                STRUCT(NULL as left_value, 2 as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, 2 as right_value, False as is_equal,
                        False as exists_left, True as exists_right
                 ) as c4,
                 STRUCT(True as left_value, True as right_value) as __EXISTS__,
-                FALSE as __IS_EQUAL__
+                FALSE as __IS_EQUAL__,
+                ARRAY('{"id": 3}') as __SAMPLE_ID__
             ),
             STRUCT(
                 STRUCT(4 as left_value, 4 as right_value, True as is_equal,
                        True as exists_left, True as exists_right
                 ) as id,
                 STRUCT("b" as left_value, "b" as right_value, True as is_equal,
                        True as exists_left, True as exists_right
                 ) as c1,
                 STRUCT(2 as left_value, 4 as right_value, False as is_equal,
                        True as exists_left, True as exists_right
                 ) as c2,
-                STRUCT(2 as left_value, NULL as right_value, False as is_equal,
+                STRUCT(2 as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        True as exists_left, False as exists_right
                 ) as c3,
-                STRUCT(NULL as left_value, 2 as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, 2 as right_value, False as is_equal,
                        False as exists_left, True as exists_right
                 ) as c4,
                 STRUCT(True as left_value, True as right_value) as __EXISTS__,
-                FALSE as __IS_EQUAL__
+                FALSE as __IS_EQUAL__,
+                ARRAY('{"id": 4}') as __SAMPLE_ID__
             ),
             STRUCT(
-                STRUCT(5 as left_value, NULL as right_value, False as is_equal,
+                STRUCT(5 as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        True as exists_left, False as exists_right
                 ) as id,
-                STRUCT("c" as left_value, NULL as right_value, False as is_equal,
+                STRUCT("c" as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        True as exists_left, False as exists_right
                 ) as c1,
-                STRUCT(3 as left_value, NULL as right_value, False as is_equal,
+                STRUCT(3 as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        True as exists_left, False as exists_right
                 ) as c2,
-                STRUCT(3 as left_value, NULL as right_value, False as is_equal,
+                STRUCT(3 as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        True as exists_left, False as exists_right
                 ) as c3,
-                STRUCT(NULL as left_value, NULL as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        False as exists_left, False as exists_right
                 ) as c4,
                 STRUCT(True as left_value, False as right_value) as __EXISTS__,
-                FALSE as __IS_EQUAL__
+                FALSE as __IS_EQUAL__,
+                ARRAY('{"id": 5}') as __SAMPLE_ID__
             ),
             STRUCT(
-                STRUCT(NULL as left_value, 6 as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, 6 as right_value, False as is_equal,
                        False as exists_left, True as exists_right
                 ) as id,
-                STRUCT(NULL as left_value, "f" as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, "f" as right_value, False as is_equal,
                        False as exists_left, True as exists_right
                 ) as c1,
-                STRUCT(NULL as left_value, 3 as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, 3 as right_value, False as is_equal,
                        False as exists_left, True as exists_right
                 ) as c2,
-                STRUCT(NULL as left_value, NULL as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, CAST(NULL as INT) as right_value, False as is_equal,
                        False as exists_left, False as exists_right
                 ) as c3,
-                STRUCT(NULL as left_value, 3 as right_value, False as is_equal,
+                STRUCT(CAST(NULL as INT) as left_value, 3 as right_value, False as is_equal,
                        False as exists_left, True as exists_right
                 ) as c4,
                 STRUCT(False as left_value, True as right_value) as __EXISTS__,
-                FALSE as __IS_EQUAL__
+                FALSE as __IS_EQUAL__,
+                ARRAY('{"id": 6}') as __SAMPLE_ID__
             )
         ))
     """,
     )
     return diff_df
```

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/schema_diff.py` & `spark_frame-0.5.0/spark_frame/data_diff/schema_diff.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/data_diff/special_characters.py` & `spark_frame-0.5.0/spark_frame/data_diff/special_characters.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/data_type_utils.py` & `spark_frame-0.5.0/spark_frame/data_type_utils.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/examples/flatten_unflatten.py` & `spark_frame-0.5.0/spark_frame/examples/flatten_unflatten.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/examples/reference_nested.py` & `spark_frame-0.5.0/spark_frame/examples/reference_nested.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/examples/working_with_json.py` & `spark_frame-0.5.0/spark_frame/examples/working_with_json.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/examples/working_with_nested_data.py` & `spark_frame-0.5.0/spark_frame/examples/working_with_nested_data.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/exceptions.py` & `spark_frame-0.5.0/spark_frame/exceptions.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/field_utils.py` & `spark_frame-0.5.0/spark_frame/field_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -42,14 +42,38 @@
     >>> is_sub_field_or_equal_to_any("a", [])
     False
 
     """
     return any(is_sub_field_or_equal(sub_field, field) for field in fields)
 
 
+def get_granularity(field: str) -> str:
+    """Return True if `field` has the given granularity
+
+    >>> get_granularity("a")
+    ''
+    >>> get_granularity("s.z")
+    ''
+    >>> get_granularity("a!")
+    'a!'
+    >>> get_granularity("a!!")
+    'a!!'
+    >>> get_granularity("a!.b")
+    'a!'
+    >>> get_granularity("a!.b!.c")
+    'a!.b!'
+
+    """
+    granularity = substring_before_last_occurrence(field, "!")
+    if granularity == "":
+        return granularity
+    else:
+        return granularity + "!"
+
+
 def has_same_granularity(field: str, other_field: str) -> bool:
     """Return True if `field` is at the same granularity level as `other_field`
 
     >>> has_same_granularity("a", "a")
     True
     >>> has_same_granularity("a", "b")
     True
@@ -72,15 +96,15 @@
     False
     >>> has_same_granularity("a!.b", "a")
     False
     >>> has_same_granularity("a", "a!.b")
     False
 
     """
-    return field.split("!.")[:-1] == other_field.split("!.")[:-1]
+    return get_granularity(field) == get_granularity(other_field)
 
 
 def has_same_granularity_as_any(field: str, other_fields: List[str]) -> bool:
     """Return True if `field` is equal to or has the same parent as any field in `other_fields`
 
     >>> has_same_granularity_as_any("a", ["a", "b"])
     True
@@ -104,14 +128,58 @@
     >>> has_same_granularity_as_any("a", [])
     False
 
     """
     return any(has_same_granularity(field, other_field) for other_field in other_fields)
 
 
+def has_same_or_higher_granularity(field: str, other_field: str) -> bool:
+    """Return True if `field` is at the same granularity level as `other_field`
+
+    >>> has_same_or_higher_granularity("a", "")
+    True
+    >>> has_same_or_higher_granularity("s.z", "")
+    True
+    >>> has_same_or_higher_granularity("a!.b", "")
+    False
+    >>> has_same_or_higher_granularity("a!.b!.c", "")
+    False
+
+    >>> has_same_or_higher_granularity("a", "x!")
+    True
+    >>> has_same_or_higher_granularity("s.z", "x!")
+    True
+    >>> has_same_or_higher_granularity("a!.b", "x!")
+    False
+    >>> has_same_or_higher_granularity("a!.b!.c", "x!")
+    False
+
+    >>> has_same_or_higher_granularity("a", "a!")
+    True
+    >>> has_same_or_higher_granularity("s.z", "a!")
+    True
+    >>> has_same_or_higher_granularity("a!.b", "a!")
+    True
+    >>> has_same_or_higher_granularity("a!.b!.c", "a!")
+    False
+
+    >>> has_same_or_higher_granularity("a", "a!.b!")
+    True
+    >>> has_same_or_higher_granularity("s.z", "a!.b!")
+    True
+    >>> has_same_or_higher_granularity("a!.b", "a!.b!")
+    True
+    >>> has_same_or_higher_granularity("a!.s.z", "a!.b!")
+    True
+    >>> has_same_or_higher_granularity("a!.b!.c", "a!.b!")
+    True
+    """
+    return get_granularity(other_field).startswith(get_granularity(field))
+
+
 def is_sub_field(sub_field: str, field: str) -> bool:
     """Return True if `sub_field` is a sub-field of `field`, or is equal to `field`
 
     >>> is_sub_field("a", "a")
     True
     >>> is_sub_field("a", "b")
     False
@@ -120,14 +188,16 @@
     True
     >>> is_sub_field("a!.b", "a!")
     True
     >>> is_sub_field("a.b", "b")
     False
     >>> is_sub_field("a.b!", "a")
     False
+    >>> is_sub_field("a!.b", "a")
+    False
 
     >>> is_sub_field("a", "a.b")
     False
 
     >>> is_sub_field("a.b.c", "a.b")
     True
     >>> is_sub_field("a.b.c", "a")
```

### Comparing `spark_frame-0.4.0/spark_frame/filesystem.py` & `spark_frame-0.5.0/spark_frame/filesystem.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/fp/higher_order.py` & `spark_frame-0.5.0/spark_frame/fp/higher_order.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/fp/package.py` & `spark_frame-0.5.0/spark_frame/fp/package.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/fp/printable_function.py` & `spark_frame-0.5.0/spark_frame/fp/printable_function.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/functions.py` & `spark_frame-0.5.0/spark_frame/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,51 @@
 from typing import Union
 
 from pyspark.sql import Column
 from pyspark.sql import functions as f
 from pyspark.sql.types import DataType, StringType
 
-from spark_frame.utils import quote
+from spark_frame.exceptions import IllegalArgumentException
+from spark_frame.utils import StringOrColumn, assert_true, quote, str_to_col
+
+
+def array_union(*cols: StringOrColumn) -> Column:
+    """Collection function: returns an array of the elements in the union of all columns, without duplicates.
+
+    Args:
+        *cols: Columns or names of column of type ARRAY
+
+    Returns:
+        A Column expression containing the union of all arrays
+
+    Examples:
+        >>> from pyspark.sql import SparkSession
+        >>> spark = SparkSession.builder.appName("doctest").getOrCreate()
+        >>> df = spark.sql('SELECT ARRAY(1, 2) as c1, ARRAY(3, 4) as c2, ARRAY(5, 6) as c3')
+        >>> df.show()
+        +------+------+------+
+        |    c1|    c2|    c3|
+        +------+------+------+
+        |[1, 2]|[3, 4]|[5, 6]|
+        +------+------+------+
+        <BLANKLINE>
+        >>> df.select(array_union(df.c1, df.c2, df.c3).alias("c")).show()
+        +------------------+
+        |                 c|
+        +------------------+
+        |[1, 2, 3, 4, 5, 6]|
+        +------------------+
+        <BLANKLINE>
+    """
+    assert_true(len(cols) > 0, IllegalArgumentException("At least one column must be passed"))
+    columns = [str_to_col(col) for col in cols]
+    res = columns[0]
+    for col in columns[1:]:
+        res = f.array_union(res, col)
+    return res
 
 
 def empty_array(element_type: Union[DataType, str]) -> Column:
     """Create an empty Spark array column of the specified type.
     This is a workaround to the Spark method `typedLit` not being available in PySpark
 
     Args:
```

### Comparing `spark_frame-0.4.0/spark_frame/graph_impl/ascending_forest_traversal.py` & `spark_frame-0.5.0/spark_frame/graph_impl/ascending_forest_traversal.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested.py` & `spark_frame-0.5.0/spark_frame/nested.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_functions_impl/aggregate.py` & `spark_frame-0.5.0/spark_frame/nested_functions_impl/aggregate.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_functions_impl/average.py` & `spark_frame-0.5.0/spark_frame/nested_functions_impl/average.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_functions_impl/sum.py` & `spark_frame-0.5.0/spark_frame/nested_functions_impl/sum.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_impl/fields.py` & `spark_frame-0.5.0/spark_frame/nested_impl/fields.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_impl/package.py` & `spark_frame-0.5.0/spark_frame/nested_impl/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,41 +209,61 @@
         column_transformations: A `Dict(column_alias, column_transformation)`
 
     Returns:
         An ordered tree
 
     Examples:
         >>> _build_nested_struct_tree({
-        ...   "s!.c": PrintableFunction(lambda s: s["c"], 'trans_c') ,
-        ...   "s!.d": PrintableFunction(lambda s: s["d"].cast("DOUBLE"), 'trans_d'),
-        ... })
-        OrderedDict([('s', OrderedDict([('!', OrderedDict([('.', OrderedDict([('c', trans_c), ('d', trans_d)]))]))]))])
+        ...   "s!.c": "trans_c" ,
+        ...   "s!.d": "trans_d"
+        ... }) == OrderedDict(
+        ... [("s", OrderedDict([("!", OrderedDict([(".", OrderedDict([("c", "trans_c"), ("d", "trans_d")]))]))]))]
+        ... )
+        True
 
         >>> _build_nested_struct_tree({
-        ...   "e!!.c": PrintableFunction(lambda s: s["c"], 'trans_c') ,
-        ...   "e!!.d": PrintableFunction(lambda s: s["d"].cast("DOUBLE"), 'trans_d'),
-        ... })
-        OrderedDict([('e', OrderedDict([('!', OrderedDict([('!', OrderedDict([('.', OrderedDict([('c', trans_c), ('d', trans_d)]))]))]))]))])
+        ...   "e!!.c": "trans_c",
+        ...   "e!!.d": "trans_d",
+        ... }) == OrderedDict([
+        ...     ("e", OrderedDict([
+        ...         ("!", OrderedDict([
+        ...             ("!", OrderedDict([
+        ...                 (".", OrderedDict([
+        ...                     ("c", "trans_c"),
+        ...                     ("d", "trans_d")
+        ...                 ]))
+        ...             ]))
+        ...         ]))
+        ...     ]))
+        ... ])
+        True
 
         >>> _build_nested_struct_tree({
-        ...   "e!": PrintableFunction(lambda e: e.cast("DOUBLE"), 'trans_e')
-        ... })
-        OrderedDict([('e', OrderedDict([('!', trans_e)]))])
+        ...   "e!": "trans_e"
+        ... }) == OrderedDict([("e", OrderedDict([("!", "trans_e")]))])
+        True
 
         >>> _build_nested_struct_tree({
-        ...   "e!!": PrintableFunction(lambda e: e.cast("DOUBLE"), 'trans_e')
-        ... })
-        OrderedDict([('e', OrderedDict([('!', OrderedDict([('!', trans_e)]))]))])
+        ...   "e!!": "trans_e"
+        ... }) == OrderedDict([("e", OrderedDict([("!", OrderedDict([("!", "trans_e")]))]))])
+        True
 
         >>> _build_nested_struct_tree({
-        ...   "m1%key": PrintableFunction(lambda key : f.upper(key), 'trans_key'),
-        ...   "m1%value.a": PrintableFunction(lambda value : value["a"].cast("DOUBLE"), 'trans_value')
-        ... })
-        OrderedDict([('m1', OrderedDict([('%', OrderedDict([('%key', trans_key), ('%value', OrderedDict([('.', OrderedDict([('a', trans_value)]))]))]))]))])
-    """  # noqa: E501
+        ...   "m1%key": "trans_key",
+        ...   "m1%value.a": "trans_value"
+        ... }) == OrderedDict([
+        ...     ("m1", OrderedDict([
+        ...         ("%", OrderedDict([
+        ...             ("%key", "trans_key"),
+        ...             ("%value", OrderedDict([(".", OrderedDict([("a", "trans_value")]))]))
+        ...         ]))
+        ...     ]))
+        ... ])
+        True
+    """
 
     def rec_insert(
         node: OrderedTree,
         alias: str,
         column: Optional[AnyKindOfTransformation],
         is_map: bool = False,
     ) -> None:
@@ -838,24 +858,24 @@
 
 def _get_deepest_unnested_field(col_names: List[str]) -> str:
     """Given a list of field names, give the name of the deepest that has been unnested in that list.
 
     >>> _get_deepest_unnested_field(['id1', 'id2'])
     ''
     >>> _get_deepest_unnested_field(['id1', 'id2', 's1!.id'])
-    's1'
+    's1!'
     >>> _get_deepest_unnested_field(['id1', 'id2', 's1!.id', 's1!.ss!'])
-    's1!.ss'
+    's1!.ss!'
 
     """
     deepest = sorted(col_names, key=lambda s: s.count(REPETITION_MARKER))[-1]
     if deepest.count(REPETITION_MARKER) == 0:
         return ""
     else:
-        return substring_before_last_occurrence(deepest, REPETITION_MARKER)
+        return substring_before_last_occurrence(deepest, REPETITION_MARKER) + REPETITION_MARKER
 
 
 def _get_keep_columns_for_final_select(
     df: DataFrame,
     cols: List[Column],
     keep_columns_list: List[str],
 ) -> Generator[str, None, None]:
@@ -1032,77 +1052,77 @@
         +---+----+
         |  1| {7}|
         +---+----+
         <BLANKLINE>
         >>> for cols, res_df in unnest_fields(df, 's1!').items():
         ...     print(cols)
         ...     res_df.show(truncate=False)
-        s1
+        s1!
         +---------------------+
         |s1!                  |
         +---------------------+
         |{2, [{3, 4}], [5, 6]}|
         +---------------------+
         <BLANKLINE>
         >>> for cols, res_df in unnest_fields(df, 's1!.b!').items():
         ...     print(cols)
         ...     res_df.show(truncate=False)
-        s1!.b
+        s1!.b!
         +------+
         |s1!.b!|
         +------+
         |{3, 4}|
         +------+
         <BLANKLINE>
         >>> for cols, res_df in unnest_fields(df, 's1!.e!').items():
         ...     print(cols)
         ...     res_df.show(truncate=False)
-        s1!.e
+        s1!.e!
         +------+
         |s1!.e!|
         +------+
         |5     |
         |6     |
         +------+
         <BLANKLINE>
         >>> for cols, res_df in unnest_fields(df, 's1!.e').items():
         ...     print(cols)
         ...     res_df.show(truncate=False)
-        s1
+        s1!
         +------+
         |s1!.e |
         +------+
         |[5, 6]|
         +------+
         <BLANKLINE>
         >>> for cols, res_df in unnest_fields(df, ['s1!.b','s1!.e']).items():
         ...     print(cols)
         ...     res_df.show(truncate=False)
-        s1
+        s1!
         +--------+------+
         |s1!.b   |s1!.e |
         +--------+------+
         |[{3, 4}]|[5, 6]|
         +--------+------+
         <BLANKLINE>
         >>> for cols, res_df in unnest_fields(df, 's3!').items():
         ...     print(cols)
         ...     res_df.show(truncate=False)
-        s3
+        s3!
         +------+
         |s3!   |
         +------+
         |[1, 2]|
         |[3, 4]|
         +------+
         <BLANKLINE>
         >>> for cols, res_df in unnest_fields(df, 's3!!').items():
         ...     print(cols)
         ...     res_df.show(truncate=False)
-        s3!
+        s3!!
         +----+
         |s3!!|
         +----+
         |1   |
         |2   |
         |3   |
         |4   |
@@ -1115,47 +1135,47 @@
         <BLANKLINE>
         +---+------+
         |id |s2.f.g|
         +---+------+
         |1  |7     |
         +---+------+
         <BLANKLINE>
-        s1
+        s1!
         +---+-----+
         |id |s1!.a|
         +---+-----+
         |1  |2    |
         +---+-----+
         <BLANKLINE>
-        s1!.b
+        s1!.b!
         +---+--------+--------+
         |id |s1!.b!.c|s1!.b!.d|
         +---+--------+--------+
         |1  |3       |4       |
         +---+--------+--------+
         <BLANKLINE>
-        s1!.e
+        s1!.e!
         +---+------+
         |id |s1!.e!|
         +---+------+
         |1  |5     |
         |1  |6     |
         +---+------+
         <BLANKLINE>
-        s3!
+        s3!!
         +---+----+
         |id |s3!!|
         +---+----+
         |1  |1   |
         |1  |2   |
         |1  |3   |
         |1  |4   |
         +---+----+
         <BLANKLINE>
-        s4!
+        s4!!
         +---+------+------+
         |id |s4!!.e|s4!!.f|
         +---+------+------+
         |1  |1     |2     |
         |1  |3     |4     |
         +---+------+------+
         <BLANKLINE>
@@ -1167,47 +1187,47 @@
         <BLANKLINE>
         +---+------+
         |id |s2.f.g|
         +---+------+
         |1  |7     |
         +---+------+
         <BLANKLINE>
-        s1
+        s1!
         +----+-----+
         |s2.f|s1!.a|
         +----+-----+
         |{7} |2    |
         +----+-----+
         <BLANKLINE>
-        s1!.b
+        s1!.b!
         +----+--------+--------+
         |s2.f|s1!.b!.c|s1!.b!.d|
         +----+--------+--------+
         |{7} |3       |4       |
         +----+--------+--------+
         <BLANKLINE>
-        s1!.e
+        s1!.e!
         +----+------+
         |s2.f|s1!.e!|
         +----+------+
         |{7} |5     |
         |{7} |6     |
         +----+------+
         <BLANKLINE>
-        s3!
+        s3!!
         +----+----+
         |s2.f|s3!!|
         +----+----+
         |{7} |1   |
         |{7} |2   |
         |{7} |3   |
         |{7} |4   |
         +----+----+
         <BLANKLINE>
-        s4!
+        s4!!
         +----+------+------+
         |s2.f|s4!!.e|s4!!.f|
         +----+------+------+
         |{7} |1     |2     |
         |{7} |3     |4     |
         +----+------+------+
         <BLANKLINE>
@@ -1219,60 +1239,60 @@
         <BLANKLINE>
         +---+------+
         |id |s2.f.g|
         +---+------+
         |1  |7     |
         +---+------+
         <BLANKLINE>
-        s1
+        s1!
         +------+-----+
         |s2.f.g|s1!.a|
         +------+-----+
         |7     |2    |
         +------+-----+
         <BLANKLINE>
-        s1!.b
+        s1!.b!
         +------+--------+--------+
         |s2.f.g|s1!.b!.c|s1!.b!.d|
         +------+--------+--------+
         |7     |3       |4       |
         +------+--------+--------+
         <BLANKLINE>
-        s1!.e
+        s1!.e!
         +------+------+
         |s2.f.g|s1!.e!|
         +------+------+
         |7     |5     |
         |7     |6     |
         +------+------+
         <BLANKLINE>
-        s3!
+        s3!!
         +------+----+
         |s2.f.g|s3!!|
         +------+----+
         |7     |1   |
         |7     |2   |
         |7     |3   |
         |7     |4   |
         +------+----+
         <BLANKLINE>
-        s4!
+        s4!!
         +------+------+------+
         |s2.f.g|s4!!.e|s4!!.f|
         +------+------+------+
         |7     |1     |2     |
         |7     |3     |4     |
         +------+------+------+
         <BLANKLINE>
 
         Making sure keep_columns works with columns inside arrays of structs
         >>> for cols, res_df in unnest_fields(df, ['s1!.b!.c', 's1!.b!.d'], keep_fields=["s1!.a"]).items():
         ...     print(cols)
         ...     res_df.show(truncate=False)
-        s1!.b
+        s1!.b!
         +-----+--------+--------+
         |s1!.a|s1!.b!.c|s1!.b!.d|
         +-----+--------+--------+
         |2    |3       |4       |
         +-----+--------+--------+
         <BLANKLINE>
```

### Comparing `spark_frame-0.4.0/spark_frame/nested_impl/print_schema.py` & `spark_frame-0.5.0/spark_frame/nested_impl/print_schema.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_impl/schema_string.py` & `spark_frame-0.5.0/spark_frame/nested_impl/schema_string.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_impl/select_impl.py` & `spark_frame-0.5.0/spark_frame/nested_impl/select_impl.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_impl/unnest_all_fields.py` & `spark_frame-0.5.0/spark_frame/nested_impl/unnest_all_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,30 +67,30 @@
         <BLANKLINE>
         +---+----+
         | id|s1.a|
         +---+----+
         |  1|   2|
         +---+----+
         <BLANKLINE>
-        s2
+        s2!
         +---+-----+-----+
         | id|s2!.b|s2!.c|
         +---+-----+-----+
         |  1|    3|    4|
         +---+-----+-----+
         <BLANKLINE>
-        s2!.s3
+        s2!.s3!
         +---+---------+
         | id|s2!.s3!.d|
         +---+---------+
         |  1|        5|
         |  1|        6|
         +---+---------+
         <BLANKLINE>
-        s4
+        s4!
         +---+-----+-----+
         | id|s4!.e|s4!.f|
         +---+-----+-----+
         |  1|    7|    8|
         |  1|    9|   10|
         +---+-----+-----+
         <BLANKLINE>
```

### Comparing `spark_frame-0.4.0/spark_frame/nested_impl/unnest_field.py` & `spark_frame-0.5.0/spark_frame/nested_impl/unnest_field.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/nested_impl/with_fields.py` & `spark_frame-0.5.0/spark_frame/nested_impl/with_fields.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/schema_utils.py` & `spark_frame-0.5.0/spark_frame/schema_utils.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations.py` & `spark_frame-0.5.0/spark_frame/transformations.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/analyze.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/analyze.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/analyze_aggs.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/analyze_aggs.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/convert_all_maps_to_arrays.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/convert_all_maps_to_arrays.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/flatten.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/flatten.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/flatten_all_arrays.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/flatten_all_arrays.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/harmonize_dataframes.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/harmonize_dataframes.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/parse_json_columns.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/parse_json_columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,21 @@
     By default, the output columns will have the same name as the input columns, but if you want to keep the input
     columns you can pass a dict(input_col_name, output_col_name) to specify different output column names.
 
     Please be aware that automatic schema detection is not very robust, and while this method can be quite helpful
     for quick prototyping and data exploration, it is recommended to use a fixed schema and make sure the schema
     of the input json data is properly enforce, or at the very least use schema have a drift detection mechanism.
 
-    WARNING : when you use this method on a column that is inside a struct (e.g. column "a.b.c"),
-    instead of replacing that column it will create a new column outside the struct (e.g. "`a.b.c`") (See Example 2).
+    !!! warning
+        This method's performances are not optimal, has it has to perform a Python operation on the executor's side.
+
+    !!! warning
+        When you use this method on a column that is inside a struct (e.g. column "a.b.c"),
+        instead of replacing that column it will create a new column outside the struct (e.g. "`a.b.c`")
+        (See Example 2).
 
     Args:
         df: A Spark DataFrame
         columns: A column name, list of column names, or dict(column_name, parsed_column_name)
 
     Returns:
         A new DataFrame
```

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/sort_all_arrays.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/sort_all_arrays.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/transform_all_field_names.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/transform_all_field_names.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/transform_all_fields.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/transform_all_fields.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/unflatten.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/unflatten.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,29 @@
 from spark_frame.transformations_impl.flatten import flatten
 from spark_frame.utils import quote
 
 OrderedTree = Union["OrderedTree", Dict[str, "OrderedTree"]]  # type: ignore[misc]
 
 
 def _build_nested_struct_tree(columns: List[str], struct_separator: str) -> OrderedTree:
-    """Given a list of flattened column names and a separator
-
-    >>> _build_nested_struct_tree(["id", "s.a", "s.b.c", "s.b.d"], ".")
-    OrderedDict([('id', None), ('s', OrderedDict([('a', None), ('b', OrderedDict([('c', None), ('d', None)]))]))])
+    """
 
-    :param columns: Name of the flattened columns
-    :param struct_separator: Separator used in the column names for structs
-    :return:
+    Args:
+        columns: Name of the flattened columns
+        struct_separator: Separator used in the column names for structs
+
+    Returns:
+        an ordered tree structure
+
+    Tests:
+        Given a list of flattened column names and a separator, build a tree structure that represents these columns.
+        >>> _build_nested_struct_tree(["id", "s.a", "s.b.c", "s.b.d"], ".") == OrderedDict(
+        ...     [("id", None), ("s", OrderedDict([("a", None), ("b", OrderedDict([("c", None), ("d", None)]))]))]
+        ... )
+        True
     """
 
     def rec_insert(node: OrderedTree, col: str) -> None:
         if struct_separator in col:
             struct, subcol = col.split(struct_separator, 1)
             if struct not in node:
                 node[struct] = OrderedDict()
```

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/union_dataframes.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/union_dataframes.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/unpivot.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/unpivot.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/transformations_impl/with_generic_typed_struct.py` & `spark_frame-0.5.0/spark_frame/transformations_impl/with_generic_typed_struct.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/spark_frame/utils.py` & `spark_frame-0.5.0/spark_frame/utils.py`

 * *Files identical despite different names*

### Comparing `spark_frame-0.4.0/setup.py` & `spark_frame-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,28 @@
  'spark_frame.nested_functions_impl',
  'spark_frame.nested_impl',
  'spark_frame.transformations_impl']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['pip>=24.0.0,<25.0.0']
+
 setup_kwargs = {
     'name': 'spark-frame',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'A library containing various utility functions for playing with PySpark DataFrames',
-    'long_description': '# Spark-frame\n\n[![PyPI version](https://badge.fury.io/py/spark-frame.svg)](https://badge.fury.io/py/spark-frame)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spark-frame.svg)](https://pypi.org/project/spark-frame/)\n[![GitHub Build](https://img.shields.io/github/actions/workflow/status/FurcyPin/spark-frame/build_and_validate.yml?branch=main)](https://github.com/FurcyPin/spark-frame/actions)\n[![SonarCloud Coverage](https://sonarcloud.io/api/project_badges/measure?project=FurcyPin_spark-frame&metric=coverage)](https://sonarcloud.io/component_measures?id=FurcyPin_spark-frame&metric=coverage&view=list)\n[![SonarCloud Bugs](https://sonarcloud.io/api/project_badges/measure?project=FurcyPin_spark-frame&metric=bugs)](https://sonarcloud.io/component_measures?metric=reliability_rating&view=list&id=FurcyPin_spark-frame)\n[![SonarCloud Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=FurcyPin_spark-frame&metric=vulnerabilities)](https://sonarcloud.io/component_measures?metric=security_rating&view=list&id=FurcyPin_spark-frame)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/spark-frame)](https://pypi.org/project/spark-frame/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n## What is it ?\n\n**[Spark-frame](https://furcypin.github.io/spark-frame/) is a library that super-charges your Spark DataFrames!**\n\nIt brings several utility methods and transformation functions for PySpark DataFrames.\n\nHere is a quick list of the most exciting features :sunglasses:\n\n- `spark_frame.data_diff.compare_dataframes`: compare two SQL tables or DataFrames and generate an HTML report \n  to view the result. And yes, this is completely free, open source, and it works even with \n  complex data structures ! It also detects column reordering and can handle type changes.\n  [Go check it out :exclamation:](https://furcypin.github.io/spark-frame/use_cases/comparing_dataframes/)\n- `spark_frame.nested`: Did you ever thought manipulating complex data structures in SQL or Spark was a \n  nightmare :jack_o_lantern: ? You just found the solution ! The `nested` library  makes those manipulations much \n  cleaner and simpler. \n  [Get started over there :rocket:](https://furcypin.github.io/spark-frame/use_cases/working_with_nested_data/)\n- `spark_frame.transformations`: A wide collection of generic dataframe transformations.\n    - Ever wanted to apply a transformation to every field of a DataFrame depending on it\'s name or type ? \n      [Easy as pie :cake:](https://furcypin.github.io/spark-frame/reference/transformations/#spark_frame.transformations_impl.transform_all_fields.transform_all_fields)\n    - Ever wanted to rename every field of a DataFrame, including the deeply nested ones ? \n      [Done: :ok_hand:](https://furcypin.github.io/spark-frame/reference/transformations/#spark_frame.transformations_impl.transform_all_field_names.transform_all_field_names)\n    - Ever wanted to analyze the content of a DataFrame, \n      but [`DataFrame.describe()`](https://spark.apache.org/docs/3.1.1/api/python/reference/api/pyspark.sql.DataFrame.describe.html)\n      does not work with complex data types ? \n      [You\'re welcome :pray:](https://furcypin.github.io/spark-frame/reference/transformations/#spark_frame.transformations_impl.analyze.analyze)\n- `spark_frame.schema_utils`: Need to dump the schema of a DataFrame somewhere to be able to load it later ?\n     [We got you covered :thumbsup:](https://furcypin.github.io/spark-frame/reference/schema_utils/)\n- `spark_frame.graph.ascending_forest_traversal`: Need an algorithm that takes the adjacency matrix of a \n tree :deciduous_tree: (or forest) graph and associates each node to their corresponding root node ?\n But that other algorithm you tried went into an infinite loop ∞ because your graph isn\'t really a tree \n and occasionally contains cycles ? \n [Try this :evergreen_tree:](https://furcypin.github.io/spark-frame/reference/graph/#spark_frame.graph_impl.ascending_forest_traversal.ascending_forest_traversal)\n\n\n## Getting Started\n\nVisit the official Spark-frame website [documentation](https://furcypin.github.io/spark-frame/) \nfor [use cases examples](https://furcypin.github.io/spark-frame/use_cases/intro/) \nand [reference](https://furcypin.github.io/spark-frame/reference/functions/).\n\n## Installation\n\n[spark-frame is available on PyPi](https://pypi.org/project/spark-frame/).\n\n```bash\npip install spark-frame\n```\n\n## Compatibilities and requirements\n\n\nThis library does not depend on any other library.\n**Pyspark must be installed separately to use it.**\nIt is compatible with the following versions:\n\n- Python: requires 3.8.1 or higher (tested against Python 3.9, 3.10 and 3.11)\n- Pyspark: requires 3.3.0 or higher\n\nThis library is tested against Windows, Mac and Linux.\n\n\n**Some features require extra libraries to be installed alongside this project.**\n**We chose to not include them as direct dependencies for security and flexibility reasons.**\n**This way, users who are not using these features don\'t need to worry about these dependencies.**\n\n| feature                                    |  Method                      | spark-frame\'s <br> version |     dependency required |\n|--------------------------------------------|------------------------------|----------------------------|------------------------:|\n| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | >= 0.4.0                   | data-diff-viewer==0.2.* |\n| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | < 0.4                      |                  jinja2 |\n\n_Since version 0.4, the code used to generate HTML diff reports has been moved to \n[data-diff-viewer](https://github.com/FurcyPin/data-diff-viewer) from the same author. \nIt comes with a dependency to [duckdb](https://github.com/duckdb/duckdb), \nwhich is used to store the diff results and embed them in the HTML page._\n\n\n# Genesis of the project\n\nThese methods were initially part of the [karadoc](https://github.com/FurcyPin/karadoc) project \nused at [Younited](https://medium.com/younited-tech-blog), but they were fully independent from karadoc, \nso it made more sense to keep them as a standalone library.\n\nSeveral of these methods were my initial inspiration to make the cousin project\n[bigquery-frame](https://github.com/FurcyPin/bigquery-frame), which was first made to illustrate\nthis [blog article](https://medium.com/towards-data-science/sql-jinja-is-not-enough-why-we-need-dataframes-4d71a191936d).\nThis is why you will find similar methods in both `spark_frame` and `bigquery_frame`, \nexcept the former runs on PySpark while the latter runs on BigQuery (obviously).\nI try to keep both projects consistent together, and will eventually port new developments made on \none project to the other one.\n\n\n# Changelog\n\n# v0.4.0\n\nFixes and improvements on data_diff.\n\nImprovements:\n- data-diff: \n  - Now supports complex data types. Declaring a repeated field (e.g. `"s!.id"` in join_cols will now explode the\n    corresponding array and perform the diff on it).\n  - When columns are removed or renamed, they are now still displayed in the per-column diff report.\n  - Refactored and improved the HTML report: it is now fully standalone and can be opened without any \n    internet connection .\n  - Can now generate the HTML report directly on any remote file system accessible by Spark (e.g. "hdfs", "s3", etc.)\n  - A user-friendly error is now raised when one of the `join_cols` does not exist. \n- added package `spark_frame.filesystem` that can be used to read and write files directly from the driver using\n  the java FileSystem from Spark\'s JVM.\n\n**Breaking Changes:**\n- data-diff:\n  - `spark_frame.data_diff.DataframeComparator` object has been removed. \n    Please use directly the method `spark_frame.data_diff.compare_dataframes`.\n  - package `spark_frame.data_diff.diff_results` has been renamed to `diff_results`.\n  - Generating HTML reports for data diff does not require jinja anymore, but it does now require the installation \n    of the library [data-diff-viewer](https://pypi.org/project/data-diff-viewer/), \n    please check the [Compatibilities and requirements](#compatibilities-and-requirements) \n    section to know which version to use.\n  - The DiffResult object returned by the `compare_dataframes` method has evolved. In particular, the\n    type of `diff_df_shards` changed from a single `DataFrame` to a `Dict[str, DataFrame]`.\n  - `DiffFormatOptions.max_string_length` option has been removed\n  - `DiffFormatOptions.nb_diffed_rows` has been renamed to `nb_top_values_kept_per_column`\n  - `spark_frame.data_diff.compare_dataframes_impl.DataframeComparatorException` was replaced with\n    `spark_frame.exceptions.DataFrameComparisonException`\n  - `spark_frame.data_diff.compare_dataframes_impl.CombinatorialExplosionError` was replaced with\n    `spark_frame.exceptions.CombinatorialExplosionError`\n\nQA:\n- Spark: Added tests to ensure compatibility with Pyspark versions 3.3, 3.4 and 3.5\n- Replaced flake and isort with ruff\n\n# v0.3.2\n\nFixes and improvements on data_diff\n\n- Fix: automatic detection of join_col was sometimes selecting the wrong column\n- Visual improvements to HTML diff report:\n  - Name of columns used for join are now displayed in bold\n  - Total number of column is now displayed when the diff is ok\n  - Fix incorrect HTML diff display when one of the DataFrames is empty\n\n# v0.3.1\n\nFixes and improvements on data_diff\n\n- The `export_html_diff_report` method now accepts arguments to specify the path and encoding of the output html report. \n- Data-diff join now works correctly with null values\n- Visual improvements to HTML diff report\n\n\n# v0.3.0\n\nFixes and improvements on data_diff\n\n- Fixed incorrect diff results\n- Column values are not truncated at all, this was causing incorrect results. The possibility to limit the size \n  of the column values will be added back in a later version\n- Made sure that the most frequent values per column are now displayed by decreasing order of frequency\n\n\n# v0.2.0\n\nTwo new exciting features: *analyze* and *data_diff*. \nThey are still in experimental stage and will be improved in future releases.\n\n- Added a new transformation `spark_frame.transformations.analyze`.\n- Added new *data_diff* feature. Example:\n\n```python\nfrom pyspark.sql import DataFrame\nfrom spark_frame.data_diff import DataframeComparator\ndf1: DataFrame = ...\ndf2: DataFrame = ...\ndiff_result = DataframeComparator().compare_df(df1, df2) # Produces a DiffResult object\ndiff_result.display() # Print a diff report in the terminal\ndiff_result.export_to_html() # Generates a html diff report file named diff_report.html\n```\n\n\n# v0.1.1\n\n- Added a new transformation `spark_frame.transformations.flatten_all_arrays`.\n- Added support for multi-arg transformation to `nested.select` and `nested.with_fields` \n  With this feature, we can now access parent fields from higher levels\n  when applying a transformation. Example:\n  \n```\n>>> nested.print_schema(df)\n"""\nroot\n |-- id: integer (nullable = false)\n |-- s1!.average: integer (nullable = false)\n |-- s1!.values!: integer (nullable = false)\n"""\n>>> df.show(truncate=False)\n+---+--------------------------------------+\n|id |s1                                    |\n+---+--------------------------------------+\n|1  |[{2, [1, 2, 3]}, {3, [1, 2, 3, 4, 5]}]|\n+---+--------------------------------------+\n>>> new_df = df.transform(nested.with_fields, {\n>>>     "s1!.values!": lambda s1, value: value - s1["average"]  # This transformation takes 2 arguments\n>>> })\n+---+-----------------------------------------+\n|id |s1                                       |\n+---+-----------------------------------------+\n|1  |[{2, [-1, 0, 1]}, {3, [-2, -1, 0, 1, 2]}]|\n+---+-----------------------------------------+\n```\n\n# v0.1.0\n\n- Added a new _amazing_ module called `spark_frame.nested`, \n  which makes manipulation of nested data structure much easier!\n  Make sure to check out the [reference](https://furcypin.github.io/spark-frame/reference/nested/)\n  and the [use-cases](https://furcypin.github.io/spark-frame/use_cases/working_with_nested_data/).\n\n- Also added a new module called `spark_frame.nested_functions`,\n  which contains aggregation methods for nested data structures\n  ([See Reference](https://furcypin.github.io/spark-frame/reference/nested_functions/)).\n\n- New [transformations](https://furcypin.github.io/spark-frame/reference/transformations/):\n  - `spark_frame.transformations.transform_all_field_names`\n  - `spark_frame.transformations.transform_all_fields`\n  - `spark_frame.transformations.unnest_field`\n  - `spark_frame.transformations.unnest_all_fields`\n  - `spark_frame.transformations.union_dataframes`\n\n# v0.0.3\n\n- New transformation: `spark_frame.transformations.convert_all_maps_to_arrays`.\n- New transformation: `spark_frame.transformations.sort_all_arrays`.\n- New transformation: `spark_frame.transformations.harmonize_dataframes`.\n',
+    'long_description': '# Spark-frame\n\n[![PyPI version](https://badge.fury.io/py/spark-frame.svg)](https://badge.fury.io/py/spark-frame)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spark-frame.svg)](https://pypi.org/project/spark-frame/)\n[![GitHub Build](https://img.shields.io/github/actions/workflow/status/FurcyPin/spark-frame/build_and_validate.yml?branch=main)](https://github.com/FurcyPin/spark-frame/actions)\n[![SonarCloud Coverage](https://sonarcloud.io/api/project_badges/measure?project=FurcyPin_spark-frame&metric=coverage)](https://sonarcloud.io/component_measures?id=FurcyPin_spark-frame&metric=coverage&view=list)\n[![SonarCloud Bugs](https://sonarcloud.io/api/project_badges/measure?project=FurcyPin_spark-frame&metric=bugs)](https://sonarcloud.io/component_measures?metric=reliability_rating&view=list&id=FurcyPin_spark-frame)\n[![SonarCloud Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=FurcyPin_spark-frame&metric=vulnerabilities)](https://sonarcloud.io/component_measures?metric=security_rating&view=list&id=FurcyPin_spark-frame)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/spark-frame)](https://pypi.org/project/spark-frame/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n## What is it ?\n\n**[Spark-frame](https://furcypin.github.io/spark-frame/) is a library that super-charges your Spark DataFrames!**\n\nIt brings several utility methods and transformation functions for PySpark DataFrames.\n\nHere is a quick list of the most exciting features :sunglasses:\n\n- `spark_frame.data_diff.compare_dataframes`: compare two SQL tables or DataFrames and generate an HTML report \n  to view the result. And yes, this is completely free, open source, and it works even with \n  complex data structures ! It also detects column reordering and can handle type changes.\n  [Go check it out :exclamation:](https://furcypin.github.io/spark-frame/use_cases/comparing_dataframes/)\n- `spark_frame.nested`: Did you ever thought manipulating complex data structures in SQL or Spark was a \n  nightmare :jack_o_lantern: ? You just found the solution ! The `nested` library  makes those manipulations much \n  cleaner and simpler. \n  [Get started over there :rocket:](https://furcypin.github.io/spark-frame/use_cases/working_with_nested_data/)\n- `spark_frame.transformations`: A wide collection of generic dataframe transformations.\n    - Ever wanted to apply a transformation to every field of a DataFrame depending on it\'s name or type ? \n      [Easy as pie :cake:](https://furcypin.github.io/spark-frame/reference/transformations/#spark_frame.transformations_impl.transform_all_fields.transform_all_fields)\n    - Ever wanted to rename every field of a DataFrame, including the deeply nested ones ? \n      [Done: :ok_hand:](https://furcypin.github.io/spark-frame/reference/transformations/#spark_frame.transformations_impl.transform_all_field_names.transform_all_field_names)\n    - Ever wanted to analyze the content of a DataFrame, \n      but [`DataFrame.describe()`](https://spark.apache.org/docs/3.1.1/api/python/reference/api/pyspark.sql.DataFrame.describe.html)\n      does not work with complex data types ? \n      [You\'re welcome :pray:](https://furcypin.github.io/spark-frame/reference/transformations/#spark_frame.transformations_impl.analyze.analyze)\n- `spark_frame.schema_utils`: Need to dump the schema of a DataFrame somewhere to be able to load it later ?\n     [We got you covered :thumbsup:](https://furcypin.github.io/spark-frame/reference/schema_utils/)\n- `spark_frame.graph.ascending_forest_traversal`: Need an algorithm that takes the adjacency matrix of a \n tree :deciduous_tree: (or forest) graph and associates each node to their corresponding root node ?\n But that other algorithm you tried went into an infinite loop ∞ because your graph isn\'t really a tree \n and occasionally contains cycles ? \n [Try this :evergreen_tree:](https://furcypin.github.io/spark-frame/reference/graph/#spark_frame.graph_impl.ascending_forest_traversal.ascending_forest_traversal)\n\n\n## Getting Started\n\nVisit the official Spark-frame website [documentation](https://furcypin.github.io/spark-frame/) \nfor [use cases examples](https://furcypin.github.io/spark-frame/use_cases/intro/) \nand [reference](https://furcypin.github.io/spark-frame/reference/functions/).\n\n## Installation\n\n[spark-frame is available on PyPi](https://pypi.org/project/spark-frame/).\n\n```bash\npip install spark-frame\n```\n\n## Compatibilities and requirements\n\n\nThis library does not depend on any other library.\n**Pyspark must be installed separately to use it.**\nIt is compatible with the following versions:\n\n- Python: requires 3.8.1 or higher (tested against Python 3.8, 3.9, 3.10, 3.11 and 3.12)\n- Pyspark: requires 3.3.0 or higher (tested against PySpark 3.3, 3.4 and 3.5)\n\nThis library is tested against Windows, Mac and Linux.\n\nHowever, testing for the following combinations has been disabled, because they are failing:\n\n- PySpark 3.3 with Python >= 3.11\n- PySpark 3.4 with Python >= 3.12\n- PySpark 3.5 with Python 3.12 on Windows\n\n\n**Some features require extra libraries to be installed alongside this project.**\n**We chose to not include them as direct dependencies for security and flexibility reasons.**\n**This way, users who are not using these features don\'t need to worry about these dependencies.**\n\n| feature                                    |  Method                      | spark-frame\'s <br> version |               dependency required |\n|--------------------------------------------|------------------------------|----------------------------|----------------------------------:|\n| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | >= 0.5.0                   | data-diff-viewer==0.3.* (>=0.3.2) |\n| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | 0.4.*                      |           data-diff-viewer==0.2.* |\n| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | < 0.4                      |                            jinja2 |\n\n_Since version 0.4, the code used to generate HTML diff reports has been moved to \n[data-diff-viewer](https://github.com/FurcyPin/data-diff-viewer) from the same author. \nIt comes with a dependency to [duckdb](https://github.com/duckdb/duckdb), \nwhich is used to store the diff results and embed them in the HTML page._\n\n\n# Genesis of the project\n\nThese methods were initially part of the [karadoc](https://github.com/FurcyPin/karadoc) project \nused at [Younited](https://medium.com/younited-tech-blog), but they were fully independent from karadoc, \nso it made more sense to keep them as a standalone library.\n\nSeveral of these methods were my initial inspiration to make the cousin project\n[bigquery-frame](https://github.com/FurcyPin/bigquery-frame), which was first made to illustrate\nthis [blog article](https://medium.com/towards-data-science/sql-jinja-is-not-enough-why-we-need-dataframes-4d71a191936d).\nThis is why you will find similar methods in both `spark_frame` and `bigquery_frame`, \nexcept the former runs on PySpark while the latter runs on BigQuery (obviously).\nI try to keep both projects consistent together, and will eventually port new developments made on \none project to the other one.\n\n\n# Changelog\n\n\n# v0.5.0\n\n**New features:**\n\n- data-diff:\n  - Full sample rows in data-diff: in the data-diff HTML report, you can now click on a most frequent \n    value or change for a column and it will display the full content of a row where this change happens.\n    \n\n**Breaking Changes:**\n\n- data-diff:\n  - The names of the keys of the `DiffResult.diff_df_shards` dict have changed: \n    All keys except the root key (`""`) have been appended a REPETITION_MARKER (`"!"`).\n    This will make future manipulations easier. This should not impact users as it is a very advanced mechanic. \n\n\n\n# v0.4.0\n\nFixes and improvements on data_diff.\n\nImprovements:\n- data-diff: \n  - Now supports complex data types. Declaring a repeated field (e.g. `"s!.id"` in join_cols will now explode the\n    corresponding array and perform the diff on it).\n  - When columns are removed or renamed, they are now still displayed in the per-column diff report.\n  - Refactored and improved the HTML report: it is now fully standalone and can be opened without any \n    internet connection .\n  - Can now generate the HTML report directly on any remote file system accessible by Spark (e.g. "hdfs", "s3", etc.)\n  - A user-friendly error is now raised when one of the `join_cols` does not exist. \n- added package `spark_frame.filesystem` that can be used to read and write files directly from the driver using\n  the java FileSystem from Spark\'s JVM.\n\n**Breaking Changes:**\n- data-diff:\n  - `spark_frame.data_diff.DataframeComparator` object has been removed. \n    Please use directly the method `spark_frame.data_diff.compare_dataframes`.\n  - package `spark_frame.data_diff.diff_results` has been renamed to `diff_result`.\n  - Generating HTML reports for data diff does not require jinja anymore, but it does now require the installation \n    of the library [data-diff-viewer](https://pypi.org/project/data-diff-viewer/), \n    please check the [Compatibilities and requirements](#compatibilities-and-requirements) \n    section to know which version to use.\n  - The DiffResult object returned by the `compare_dataframes` method has evolved. In particular, the\n    type of `diff_df_shards` changed from a single `DataFrame` to a `Dict[str, DataFrame]`.\n  - `DiffFormatOptions.max_string_length` option has been removed\n  - `DiffFormatOptions.nb_diffed_rows` has been renamed to `nb_top_values_kept_per_column`\n  - `spark_frame.data_diff.compare_dataframes_impl.DataframeComparatorException` was replaced with\n    `spark_frame.exceptions.DataFrameComparisonException`\n  - `spark_frame.data_diff.compare_dataframes_impl.CombinatorialExplosionError` was replaced with\n    `spark_frame.exceptions.CombinatorialExplosionError`\n\nQA:\n- Spark: Added tests to ensure compatibility with Pyspark versions 3.3, 3.4 and 3.5\n- Replaced flake and isort with ruff\n\n# v0.3.2\n\nFixes and improvements on data_diff\n\n- Fix: automatic detection of join_col was sometimes selecting the wrong column\n- Visual improvements to HTML diff report:\n  - Name of columns used for join are now displayed in bold\n  - Total number of column is now displayed when the diff is ok\n  - Fix incorrect HTML diff display when one of the DataFrames is empty\n\n# v0.3.1\n\nFixes and improvements on data_diff\n\n- The `export_html_diff_report` method now accepts arguments to specify the path and encoding of the output html report. \n- Data-diff join now works correctly with null values\n- Visual improvements to HTML diff report\n\n\n# v0.3.0\n\nFixes and improvements on data_diff\n\n- Fixed incorrect diff results\n- Column values are not truncated at all, this was causing incorrect results. The possibility to limit the size \n  of the column values will be added back in a later version\n- Made sure that the most frequent values per column are now displayed by decreasing order of frequency\n\n\n# v0.2.0\n\nTwo new exciting features: *analyze* and *data_diff*. \nThey are still in experimental stage and will be improved in future releases.\n\n- Added a new transformation `spark_frame.transformations.analyze`.\n- Added new *data_diff* feature. Example:\n\n```python\nfrom pyspark.sql import DataFrame\nfrom spark_frame.data_diff import DataframeComparator\ndf1: DataFrame = ...\ndf2: DataFrame = ...\ndiff_result = DataframeComparator().compare_df(df1, df2) # Produces a DiffResult object\ndiff_result.display() # Print a diff report in the terminal\ndiff_result.export_to_html() # Generates a html diff report file named diff_report.html\n```\n\n\n# v0.1.1\n\n- Added a new transformation `spark_frame.transformations.flatten_all_arrays`.\n- Added support for multi-arg transformation to `nested.select` and `nested.with_fields` \n  With this feature, we can now access parent fields from higher levels\n  when applying a transformation. Example:\n  \n```\n>>> nested.print_schema(df)\n"""\nroot\n |-- id: integer (nullable = false)\n |-- s1!.average: integer (nullable = false)\n |-- s1!.values!: integer (nullable = false)\n"""\n>>> df.show(truncate=False)\n+---+--------------------------------------+\n|id |s1                                    |\n+---+--------------------------------------+\n|1  |[{2, [1, 2, 3]}, {3, [1, 2, 3, 4, 5]}]|\n+---+--------------------------------------+\n>>> new_df = df.transform(nested.with_fields, {\n>>>     "s1!.values!": lambda s1, value: value - s1["average"]  # This transformation takes 2 arguments\n>>> })\n+---+-----------------------------------------+\n|id |s1                                       |\n+---+-----------------------------------------+\n|1  |[{2, [-1, 0, 1]}, {3, [-2, -1, 0, 1, 2]}]|\n+---+-----------------------------------------+\n```\n\n# v0.1.0\n\n- Added a new _amazing_ module called `spark_frame.nested`, \n  which makes manipulation of nested data structure much easier!\n  Make sure to check out the [reference](https://furcypin.github.io/spark-frame/reference/nested/)\n  and the [use-cases](https://furcypin.github.io/spark-frame/use_cases/working_with_nested_data/).\n\n- Also added a new module called `spark_frame.nested_functions`,\n  which contains aggregation methods for nested data structures\n  ([See Reference](https://furcypin.github.io/spark-frame/reference/nested_functions/)).\n\n- New [transformations](https://furcypin.github.io/spark-frame/reference/transformations/):\n  - `spark_frame.transformations.transform_all_field_names`\n  - `spark_frame.transformations.transform_all_fields`\n  - `spark_frame.transformations.unnest_field`\n  - `spark_frame.transformations.unnest_all_fields`\n  - `spark_frame.transformations.union_dataframes`\n\n# v0.0.3\n\n- New transformation: `spark_frame.transformations.convert_all_maps_to_arrays`.\n- New transformation: `spark_frame.transformations.sort_all_arrays`.\n- New transformation: `spark_frame.transformations.harmonize_dataframes`.\n',
     'author': 'FurcyPin',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/FurcyPin/spark-frame',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8.1,<3.11',
+    'install_requires': install_requires,
+    'python_requires': '>=3.8.1,<3.13',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `spark_frame-0.4.0/PKG-INFO` & `spark_frame-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: spark-frame
-Version: 0.4.0
+Version: 0.5.0
 Summary: A library containing various utility functions for playing with PySpark DataFrames
 Home-page: https://github.com/FurcyPin/spark-frame
 License: Apache-2.0
 Keywords: Spark,PySpark,DataFrame
 Author: FurcyPin
-Requires-Python: >=3.8.1,<3.11
+Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pip (>=24.0.0,<25.0.0)
 Project-URL: Repository, https://github.com/FurcyPin/spark-frame
 Description-Content-Type: text/markdown
 
 # Spark-frame
 
 [![PyPI version](https://badge.fury.io/py/spark-frame.svg)](https://badge.fury.io/py/spark-frame)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spark-frame.svg)](https://pypi.org/project/spark-frame/)
@@ -77,28 +79,35 @@
 ## Compatibilities and requirements
 
 
 This library does not depend on any other library.
 **Pyspark must be installed separately to use it.**
 It is compatible with the following versions:
 
-- Python: requires 3.8.1 or higher (tested against Python 3.9, 3.10 and 3.11)
-- Pyspark: requires 3.3.0 or higher
+- Python: requires 3.8.1 or higher (tested against Python 3.8, 3.9, 3.10, 3.11 and 3.12)
+- Pyspark: requires 3.3.0 or higher (tested against PySpark 3.3, 3.4 and 3.5)
 
 This library is tested against Windows, Mac and Linux.
 
+However, testing for the following combinations has been disabled, because they are failing:
+
+- PySpark 3.3 with Python >= 3.11
+- PySpark 3.4 with Python >= 3.12
+- PySpark 3.5 with Python 3.12 on Windows
+
 
 **Some features require extra libraries to be installed alongside this project.**
 **We chose to not include them as direct dependencies for security and flexibility reasons.**
 **This way, users who are not using these features don't need to worry about these dependencies.**
 
-| feature                                    |  Method                      | spark-frame's <br> version |     dependency required |
-|--------------------------------------------|------------------------------|----------------------------|------------------------:|
-| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | >= 0.4.0                   | data-diff-viewer==0.2.* |
-| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | < 0.4                      |                  jinja2 |
+| feature                                    |  Method                      | spark-frame's <br> version |               dependency required |
+|--------------------------------------------|------------------------------|----------------------------|----------------------------------:|
+| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | >= 0.5.0                   | data-diff-viewer==0.3.* (>=0.3.2) |
+| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | 0.4.*                      |           data-diff-viewer==0.2.* |
+| Generating HTML <br> reports for data diff |  `DiffResult.export_to_html` | < 0.4                      |                            jinja2 |
 
 _Since version 0.4, the code used to generate HTML diff reports has been moved to 
 [data-diff-viewer](https://github.com/FurcyPin/data-diff-viewer) from the same author. 
 It comes with a dependency to [duckdb](https://github.com/duckdb/duckdb), 
 which is used to store the diff results and embed them in the HTML page._
 
 
@@ -115,14 +124,33 @@
 except the former runs on PySpark while the latter runs on BigQuery (obviously).
 I try to keep both projects consistent together, and will eventually port new developments made on 
 one project to the other one.
 
 
 # Changelog
 
+
+# v0.5.0
+
+**New features:**
+
+- data-diff:
+  - Full sample rows in data-diff: in the data-diff HTML report, you can now click on a most frequent 
+    value or change for a column and it will display the full content of a row where this change happens.
+    
+
+**Breaking Changes:**
+
+- data-diff:
+  - The names of the keys of the `DiffResult.diff_df_shards` dict have changed: 
+    All keys except the root key (`""`) have been appended a REPETITION_MARKER (`"!"`).
+    This will make future manipulations easier. This should not impact users as it is a very advanced mechanic. 
+
+
+
 # v0.4.0
 
 Fixes and improvements on data_diff.
 
 Improvements:
 - data-diff: 
   - Now supports complex data types. Declaring a repeated field (e.g. `"s!.id"` in join_cols will now explode the
@@ -135,15 +163,15 @@
 - added package `spark_frame.filesystem` that can be used to read and write files directly from the driver using
   the java FileSystem from Spark's JVM.
 
 **Breaking Changes:**
 - data-diff:
   - `spark_frame.data_diff.DataframeComparator` object has been removed. 
     Please use directly the method `spark_frame.data_diff.compare_dataframes`.
-  - package `spark_frame.data_diff.diff_results` has been renamed to `diff_results`.
+  - package `spark_frame.data_diff.diff_results` has been renamed to `diff_result`.
   - Generating HTML reports for data diff does not require jinja anymore, but it does now require the installation 
     of the library [data-diff-viewer](https://pypi.org/project/data-diff-viewer/), 
     please check the [Compatibilities and requirements](#compatibilities-and-requirements) 
     section to know which version to use.
   - The DiffResult object returned by the `compare_dataframes` method has evolved. In particular, the
     type of `diff_df_shards` changed from a single `DataFrame` to a `Dict[str, DataFrame]`.
   - `DiffFormatOptions.max_string_length` option has been removed
```


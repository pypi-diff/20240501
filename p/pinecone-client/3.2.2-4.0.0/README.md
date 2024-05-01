# Comparing `tmp/pinecone_client-3.2.2.tar.gz` & `tmp/pinecone_client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_client-3.2.2.tar", max compression
+gzip compressed data, was "pinecone_client-4.0.0.tar", max compression
```

## Comparing `pinecone_client-3.2.2.tar` & `pinecone_client-4.0.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    11356 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/LICENSE.txt
--rw-r--r--   0        0        0    14522 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/README.md
--rw-r--r--   0        0        0      394 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/__init__.py
--rw-r--r--   0        0        0        5 2024-03-29 23:30:20.301139 pinecone_client-3.2.2/pinecone/__version__
--rw-r--r--   0        0        0      199 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/config/__init__.py
--rw-r--r--   0        0        0     3228 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/config/config.py
--rw-r--r--   0        0        0     4258 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/config/openapi.py
--rw-r--r--   0        0        0      934 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/config/pinecone_config.py
--rw-r--r--   0        0        0       30 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/control/__init__.py
--rw-r--r--   0        0        0     1786 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/control/index_host_store.py
--rw-r--r--   0        0        0    24453 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/control/pinecone.py
--rw-r--r--   0        0        0        0 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/__init__.py
--rw-r--r--   0        0        0      907 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/client/__init__.py
--rw-r--r--   0        0        0      226 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/client/api/__init__.py
--rw-r--r--   0        0        0    44178 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/client/api/data_plane_api.py
--rw-r--r--   0        0        0    42885 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/client/api/manage_indexes_api.py
--rw-r--r--   0        0        0    37006 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/api_client.py
--rw-r--r--   0        0        0      556 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17137 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/configuration.py
--rw-r--r--   0        0        0     5270 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/__init__.py
--rw-r--r--   0        0        0    11433 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/collection_list.py
--rw-r--r--   0        0        0    13032 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/collection_model.py
--rw-r--r--   0        0        0    11527 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request.py
--rw-r--r--   0        0        0    11550 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request_spec.py
--rw-r--r--   0        0        0    12263 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request_spec_pod.py
--rw-r--r--   0        0        0    12063 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/create_collection_request.py
--rw-r--r--   0        0        0    13925 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/create_index_request.py
--rw-r--r--   0        0        0    12887 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/delete_request.py
--rw-r--r--   0        0        0    11726 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/describe_index_stats_request.py
--rw-r--r--   0        0        0    12925 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/describe_index_stats_response.py
--rw-r--r--   0        0        0    11746 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/error_response.py
--rw-r--r--   0        0        0    12829 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/error_response_error.py
--rw-r--r--   0        0        0    11910 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/fetch_response.py
--rw-r--r--   0        0        0    11363 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/index_list.py
--rw-r--r--   0        0        0    14018 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/index_model.py
--rw-r--r--   0        0        0    11695 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/index_model_spec.py
--rw-r--r--   0        0        0    11825 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/index_model_status.py
--rw-r--r--   0        0        0    11137 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/list_item.py
--rw-r--r--   0        0        0    12233 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/list_response.py
--rw-r--r--   0        0        0    11542 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/namespace_summary.py
--rw-r--r--   0        0        0    11153 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/pagination.py
--rw-r--r--   0        0        0    14766 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/pod_spec.py
--rw-r--r--   0        0        0    11495 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/pod_spec_metadata_config.py
--rw-r--r--   0        0        0    11358 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/protobuf_any.py
--rw-r--r--   0        0        0    12395 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/protobuf_null_value.py
--rw-r--r--   0        0        0    15451 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/query_request.py
--rw-r--r--   0        0        0    12553 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/query_response.py
--rw-r--r--   0        0        0    13170 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/query_vector.py
--rw-r--r--   0        0        0    11741 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/rpc_status.py
--rw-r--r--   0        0        0    12974 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/scored_vector.py
--rw-r--r--   0        0        0    12063 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/serverless_spec.py
--rw-r--r--   0        0        0    11731 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/single_query_results.py
--rw-r--r--   0        0        0    11533 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/sparse_values.py
--rw-r--r--   0        0        0    12778 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/update_request.py
--rw-r--r--   0        0        0    11918 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/upsert_request.py
--rw-r--r--   0        0        0    11280 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/upsert_response.py
--rw-r--r--   0        0        0    11275 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/usage.py
--rw-r--r--   0        0        0    12589 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/vector.py
--rw-r--r--   0        0        0    80537 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model_utils.py
--rw-r--r--   0        0        0     3104 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/models/__init__.py
--rw-r--r--   0        0        0    14204 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/rest.py
--rw-r--r--   0        0        0    76084 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2.py
--rw-r--r--   0        0        0    24258 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2.pyi
--rw-r--r--   0        0        0    14276 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0      291 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/__init__.py
--rw-r--r--   0        0        0     2125 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/errors.py
--rw-r--r--   0        0        0    27458 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/index.py
--rw-r--r--   0        0        0     1730 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/sparse_vector_factory.py
--rw-r--r--   0        0        0     2815 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/vector_factory.py
--rw-r--r--   0        0        0     4027 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/deprecation_warnings.py
--rw-r--r--   0        0        0     1033 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/exceptions.py
--rw-r--r--   0        0        0     1300 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/grpc/__init__.py
--rw-r--r--   0        0        0     5875 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/grpc/base.py
--rw-r--r--   0        0        0     1728 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/config.py
--rw-r--r--   0        0        0      961 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/future.py
--rw-r--r--   0        0        0    28020 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/index_grpc.py
--rw-r--r--   0        0        0     4166 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/pinecone.py
--rw-r--r--   0        0        0     3193 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/retry.py
--rw-r--r--   0        0        0     2000 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/sparse_values_factory.py
--rw-r--r--   0        0        0     2996 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/utils.py
--rw-r--r--   0        0        0     3841 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/vector_factory_grpc.py
--rw-r--r--   0        0        0      534 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/__init__.py
--rw-r--r--   0        0        0      277 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/collection_description.py
--rw-r--r--   0        0        0      852 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/collection_list.py
--rw-r--r--   0        0        0     1330 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/index_description.py
--rw-r--r--   0        0        0      718 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/index_list.py
--rw-r--r--   0        0        0      198 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/list_response.py
--rw-r--r--   0        0        0     2189 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/pod_spec.py
--rw-r--r--   0        0        0      164 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/serverless_spec.py
--rw-r--r--   0        0        0      348 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/__init__.py
--rw-r--r--   0        0        0      288 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/check_kwargs.py
--rw-r--r--   0        0        0      722 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/constants.py
--rw-r--r--   0        0        0      785 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/convert_to_list.py
--rw-r--r--   0        0        0      263 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/deprecation_notice.py
--rw-r--r--   0        0        0      750 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/error_handling.py
--rw-r--r--   0        0        0      193 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/fix_tuple_length.py
--rw-r--r--   0        0        0      206 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/normalize_host.py
--rw-r--r--   0        0        0      527 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/setup_openapi_client.py
--rw-r--r--   0        0        0     1011 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/user_agent.py
--rw-r--r--   0        0        0      157 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/version.py
--rw-r--r--   0        0        0     3295 2024-03-29 23:38:38.627886 pinecone_client-3.2.2/pyproject.toml
--rw-r--r--   0        0        0    16636 1970-01-01 00:00:00.000000 pinecone_client-3.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/LICENSE.txt
+-rw-r--r--   0        0        0    14522 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/README.md
+-rw-r--r--   0        0        0      394 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/__init__.py
+-rw-r--r--   0        0        0        5 2024-05-01 03:31:12.978757 pinecone_client-4.0.0/pinecone/__version__
+-rw-r--r--   0        0        0      199 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/config/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/config/config.py
+-rw-r--r--   0        0        0     4258 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/config/openapi.py
+-rw-r--r--   0        0        0      934 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/config/pinecone_config.py
+-rw-r--r--   0        0        0       30 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/control/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/control/index_host_store.py
+-rw-r--r--   0        0        0    24453 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/control/pinecone.py
+-rw-r--r--   0        0        0        0 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/core/__init__.py
+-rw-r--r--   0        0        0      907 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/core/client/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-01 03:31:12.906757 pinecone_client-4.0.0/pinecone/core/client/api/__init__.py
+-rw-r--r--   0        0        0    44178 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/api/data_plane_api.py
+-rw-r--r--   0        0        0    42885 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/api/manage_indexes_api.py
+-rw-r--r--   0        0        0    37006 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/api_client.py
+-rw-r--r--   0        0        0      556 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17137 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/configuration.py
+-rw-r--r--   0        0        0     5270 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11433 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/collection_list.py
+-rw-r--r--   0        0        0    13032 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/collection_model.py
+-rw-r--r--   0        0        0    11527 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request.py
+-rw-r--r--   0        0        0    11550 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request_spec.py
+-rw-r--r--   0        0        0    12263 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request_spec_pod.py
+-rw-r--r--   0        0        0    12063 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/create_collection_request.py
+-rw-r--r--   0        0        0    13925 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/create_index_request.py
+-rw-r--r--   0        0        0    12887 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/delete_request.py
+-rw-r--r--   0        0        0    11726 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/describe_index_stats_request.py
+-rw-r--r--   0        0        0    12925 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/describe_index_stats_response.py
+-rw-r--r--   0        0        0    11746 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/error_response.py
+-rw-r--r--   0        0        0    12829 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/error_response_error.py
+-rw-r--r--   0        0        0    11910 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/fetch_response.py
+-rw-r--r--   0        0        0    11363 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/index_list.py
+-rw-r--r--   0        0        0    14018 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/index_model.py
+-rw-r--r--   0        0        0    11695 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/index_model_spec.py
+-rw-r--r--   0        0        0    11825 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/index_model_status.py
+-rw-r--r--   0        0        0    11137 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/list_item.py
+-rw-r--r--   0        0        0    12233 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/list_response.py
+-rw-r--r--   0        0        0    11542 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/namespace_summary.py
+-rw-r--r--   0        0        0    11153 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/pagination.py
+-rw-r--r--   0        0        0    14766 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/pod_spec.py
+-rw-r--r--   0        0        0    11495 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/pod_spec_metadata_config.py
+-rw-r--r--   0        0        0    11358 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/protobuf_any.py
+-rw-r--r--   0        0        0    12395 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/protobuf_null_value.py
+-rw-r--r--   0        0        0    15451 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/query_request.py
+-rw-r--r--   0        0        0    12553 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/query_response.py
+-rw-r--r--   0        0        0    13170 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/query_vector.py
+-rw-r--r--   0        0        0    11741 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/rpc_status.py
+-rw-r--r--   0        0        0    12974 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/scored_vector.py
+-rw-r--r--   0        0        0    12063 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/serverless_spec.py
+-rw-r--r--   0        0        0    11731 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/single_query_results.py
+-rw-r--r--   0        0        0    11533 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/sparse_values.py
+-rw-r--r--   0        0        0    12778 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/update_request.py
+-rw-r--r--   0        0        0    11918 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/upsert_request.py
+-rw-r--r--   0        0        0    11280 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/upsert_response.py
+-rw-r--r--   0        0        0    11275 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/usage.py
+-rw-r--r--   0        0        0    12589 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model/vector.py
+-rw-r--r--   0        0        0    80537 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/model_utils.py
+-rw-r--r--   0        0        0     3104 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14204 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/client/rest.py
+-rw-r--r--   0        0        0    26761 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2.py
+-rw-r--r--   0        0        0    30075 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    14276 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0      291 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/data/__init__.py
+-rw-r--r--   0        0        0     2125 2024-05-01 03:31:12.910758 pinecone_client-4.0.0/pinecone/data/errors.py
+-rw-r--r--   0        0        0    27458 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/data/index.py
+-rw-r--r--   0        0        0     1730 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/data/sparse_vector_factory.py
+-rw-r--r--   0        0        0     2815 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/data/vector_factory.py
+-rw-r--r--   0        0        0     4027 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/deprecation_warnings.py
+-rw-r--r--   0        0        0     1033 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/exceptions.py
+-rw-r--r--   0        0        0     1300 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/__init__.py
+-rw-r--r--   0        0        0     5875 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/base.py
+-rw-r--r--   0        0        0     1728 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/config.py
+-rw-r--r--   0        0        0      961 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/future.py
+-rw-r--r--   0        0        0    28020 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/index_grpc.py
+-rw-r--r--   0        0        0     4166 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/pinecone.py
+-rw-r--r--   0        0        0     3193 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/retry.py
+-rw-r--r--   0        0        0     2000 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/sparse_values_factory.py
+-rw-r--r--   0        0        0     2996 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/utils.py
+-rw-r--r--   0        0        0     4220 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/grpc/vector_factory_grpc.py
+-rw-r--r--   0        0        0      534 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/collection_description.py
+-rw-r--r--   0        0        0      852 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/collection_list.py
+-rw-r--r--   0        0        0     1330 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/index_description.py
+-rw-r--r--   0        0        0      718 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/index_list.py
+-rw-r--r--   0        0        0      198 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/list_response.py
+-rw-r--r--   0        0        0     2189 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/pod_spec.py
+-rw-r--r--   0        0        0      164 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/models/serverless_spec.py
+-rw-r--r--   0        0        0      348 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/check_kwargs.py
+-rw-r--r--   0        0        0      722 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/constants.py
+-rw-r--r--   0        0        0      785 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/convert_to_list.py
+-rw-r--r--   0        0        0      263 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/deprecation_notice.py
+-rw-r--r--   0        0        0      750 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/error_handling.py
+-rw-r--r--   0        0        0      193 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/fix_tuple_length.py
+-rw-r--r--   0        0        0      206 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/normalize_host.py
+-rw-r--r--   0        0        0      527 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/setup_openapi_client.py
+-rw-r--r--   0        0        0     1011 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/user_agent.py
+-rw-r--r--   0        0        0      157 2024-05-01 03:31:12.914758 pinecone_client-4.0.0/pinecone/utils/version.py
+-rw-r--r--   0        0        0     3266 2024-05-01 03:40:20.894214 pinecone_client-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    16625 1970-01-01 00:00:00.000000 pinecone_client-4.0.0/PKG-INFO
```

### Comparing `pinecone_client-3.2.2/LICENSE.txt` & `pinecone_client-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/README.md` & `pinecone_client-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/config/config.py` & `pinecone_client-4.0.0/pinecone/config/config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/config/openapi.py` & `pinecone_client-4.0.0/pinecone/config/openapi.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/config/pinecone_config.py` & `pinecone_client-4.0.0/pinecone/config/pinecone_config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/control/index_host_store.py` & `pinecone_client-4.0.0/pinecone/control/index_host_store.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/control/pinecone.py` & `pinecone_client-4.0.0/pinecone/control/pinecone.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/__init__.py` & `pinecone_client-4.0.0/pinecone/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/api/data_plane_api.py` & `pinecone_client-4.0.0/pinecone/core/client/api/data_plane_api.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/api/manage_indexes_api.py` & `pinecone_client-4.0.0/pinecone/core/client/api/manage_indexes_api.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/api_client.py` & `pinecone_client-4.0.0/pinecone/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/apis/__init__.py` & `pinecone_client-4.0.0/pinecone/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/configuration.py` & `pinecone_client-4.0.0/pinecone/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/exceptions.py` & `pinecone_client-4.0.0/pinecone/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/collection_list.py` & `pinecone_client-4.0.0/pinecone/core/client/model/collection_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/collection_model.py` & `pinecone_client-4.0.0/pinecone/core/client/model/collection_model.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request.py` & `pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request_spec.py` & `pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request_spec_pod.py` & `pinecone_client-4.0.0/pinecone/core/client/model/configure_index_request_spec_pod.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/create_collection_request.py` & `pinecone_client-4.0.0/pinecone/core/client/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/create_index_request.py` & `pinecone_client-4.0.0/pinecone/core/client/model/create_index_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/delete_request.py` & `pinecone_client-4.0.0/pinecone/core/client/model/delete_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/describe_index_stats_request.py` & `pinecone_client-4.0.0/pinecone/core/client/model/describe_index_stats_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/describe_index_stats_response.py` & `pinecone_client-4.0.0/pinecone/core/client/model/describe_index_stats_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/error_response.py` & `pinecone_client-4.0.0/pinecone/core/client/model/error_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/error_response_error.py` & `pinecone_client-4.0.0/pinecone/core/client/model/error_response_error.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/fetch_response.py` & `pinecone_client-4.0.0/pinecone/core/client/model/fetch_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/index_list.py` & `pinecone_client-4.0.0/pinecone/core/client/model/index_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/index_model.py` & `pinecone_client-4.0.0/pinecone/core/client/model/index_model.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/index_model_spec.py` & `pinecone_client-4.0.0/pinecone/core/client/model/index_model_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/index_model_status.py` & `pinecone_client-4.0.0/pinecone/core/client/model/index_model_status.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/list_item.py` & `pinecone_client-4.0.0/pinecone/core/client/model/list_item.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/list_response.py` & `pinecone_client-4.0.0/pinecone/core/client/model/list_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/namespace_summary.py` & `pinecone_client-4.0.0/pinecone/core/client/model/namespace_summary.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/pagination.py` & `pinecone_client-4.0.0/pinecone/core/client/model/pagination.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/pod_spec.py` & `pinecone_client-4.0.0/pinecone/core/client/model/pod_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/pod_spec_metadata_config.py` & `pinecone_client-4.0.0/pinecone/core/client/model/pod_spec_metadata_config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/protobuf_any.py` & `pinecone_client-4.0.0/pinecone/core/client/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/protobuf_null_value.py` & `pinecone_client-4.0.0/pinecone/core/client/model/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/query_request.py` & `pinecone_client-4.0.0/pinecone/core/client/model/query_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/query_response.py` & `pinecone_client-4.0.0/pinecone/core/client/model/query_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/query_vector.py` & `pinecone_client-4.0.0/pinecone/core/client/model/query_vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/rpc_status.py` & `pinecone_client-4.0.0/pinecone/core/client/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/scored_vector.py` & `pinecone_client-4.0.0/pinecone/core/client/model/scored_vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/serverless_spec.py` & `pinecone_client-4.0.0/pinecone/core/client/model/serverless_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/single_query_results.py` & `pinecone_client-4.0.0/pinecone/core/client/model/single_query_results.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/sparse_values.py` & `pinecone_client-4.0.0/pinecone/core/client/model/sparse_values.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/update_request.py` & `pinecone_client-4.0.0/pinecone/core/client/model/update_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/upsert_request.py` & `pinecone_client-4.0.0/pinecone/core/client/model/upsert_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/upsert_response.py` & `pinecone_client-4.0.0/pinecone/core/client/model/upsert_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/usage.py` & `pinecone_client-4.0.0/pinecone/core/client/model/usage.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model/vector.py` & `pinecone_client-4.0.0/pinecone/core/client/model/vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/model_utils.py` & `pinecone_client-4.0.0/pinecone/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/models/__init__.py` & `pinecone_client-4.0.0/pinecone/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/client/rest.py` & `pinecone_client-4.0.0/pinecone/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2_grpc.py` & `pinecone_client-4.0.0/pinecone/core/grpc/protos/vector_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         raise NotImplementedError('Method not implemented!')
 
     def Fetch(self, request, context):
         """Fetch vectors
 
         The `fetch` operation looks up and returns vectors, by ID, from a single namespace. The returned vectors include the vector data and/or metadata.
 
-        For guidance and examples, see [Fetch data](https://docs.pinecone.io/reference/fetch).
+        For guidance and examples, see [Fetch data](https://docs.pinecone.io/docs/fetch-data).
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def List(self, request, context):
         """List vector IDs
@@ -117,15 +117,15 @@
         raise NotImplementedError('Method not implemented!')
 
     def Update(self, request, context):
         """Update a vector
 
         The `update` operation updates a vector in a namespace. If a value is included, it will overwrite the previous value. If a `set_metadata` is included, the values of the fields specified in it will be added or overwrite the previous value.
 
-        For guidance and examples, see [Update data](https://docs.pinecone.io/reference/update).
+        For guidance and examples, see [Update data](https://docs.pinecone.io/docs/update-data).
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DescribeIndexStats(self, request, context):
         """Get index stats
```

### Comparing `pinecone_client-3.2.2/pinecone/data/errors.py` & `pinecone_client-4.0.0/pinecone/data/errors.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/data/index.py` & `pinecone_client-4.0.0/pinecone/data/index.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/data/sparse_vector_factory.py` & `pinecone_client-4.0.0/pinecone/data/sparse_vector_factory.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/data/vector_factory.py` & `pinecone_client-4.0.0/pinecone/data/vector_factory.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/deprecation_warnings.py` & `pinecone_client-4.0.0/pinecone/deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/exceptions.py` & `pinecone_client-4.0.0/pinecone/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/__init__.py` & `pinecone_client-4.0.0/pinecone/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/base.py` & `pinecone_client-4.0.0/pinecone/grpc/base.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/config.py` & `pinecone_client-4.0.0/pinecone/grpc/config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/future.py` & `pinecone_client-4.0.0/pinecone/grpc/future.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/index_grpc.py` & `pinecone_client-4.0.0/pinecone/grpc/index_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/pinecone.py` & `pinecone_client-4.0.0/pinecone/grpc/pinecone.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/retry.py` & `pinecone_client-4.0.0/pinecone/grpc/retry.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/sparse_values_factory.py` & `pinecone_client-4.0.0/pinecone/grpc/sparse_values_factory.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/utils.py` & `pinecone_client-4.0.0/pinecone/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/grpc/vector_factory_grpc.py` & `pinecone_client-4.0.0/pinecone/grpc/vector_factory_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,10 +82,15 @@
                 raise MetadataDictionaryExpectedError(item)
         else:
             item["metadata"] = dict_to_proto_struct({})
 
         try:
             return GRPCVector(**item)
         except TypeError as e:
+            # Where possible raise a more specific error to the user.
+            vid = item.get("id")
+            if not isinstance(vid, bytes) and not isinstance(vid, str):
+                raise TypeError(f"Cannot set Vector.id to {vid}: {vid} has type {type(vid)}, "
+                                "but expected one of: (<class 'bytes'>, <class 'str'>) for field Vector.id")
             if not isinstance(item["values"], Iterable) or not isinstance(item["values"].__iter__().__next__(), numbers.Real):
                 raise TypeError(f"Column `values` is expected to be a list of floats")
             raise e
```

### Comparing `pinecone_client-3.2.2/pinecone/models/__init__.py` & `pinecone_client-4.0.0/pinecone/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/models/collection_list.py` & `pinecone_client-4.0.0/pinecone/models/collection_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/models/index_description.py` & `pinecone_client-4.0.0/pinecone/models/index_description.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/models/index_list.py` & `pinecone_client-4.0.0/pinecone/models/index_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/models/pod_spec.py` & `pinecone_client-4.0.0/pinecone/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/utils/constants.py` & `pinecone_client-4.0.0/pinecone/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/utils/convert_to_list.py` & `pinecone_client-4.0.0/pinecone/utils/convert_to_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/utils/error_handling.py` & `pinecone_client-4.0.0/pinecone/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/utils/setup_openapi_client.py` & `pinecone_client-4.0.0/pinecone/utils/setup_openapi_client.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pinecone/utils/user_agent.py` & `pinecone_client-4.0.0/pinecone/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.2/pyproject.toml` & `pinecone_client-4.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
 
 [tool.poetry]
 name = "pinecone-client"
-version = "3.2.2"
+version = "4.0.0"
 packages = [
     { include="pinecone", from="." },
 ]
 description = "Pinecone client and SDK"
 authors = ["Pinecone Systems, Inc. <support@pinecone.io>"]
 license = "Apache-2.0"
 readme = "README.md"
@@ -59,18 +59,18 @@
 # on latest but setting a broad range to have maximum
 # compatibility with libraries that may pin version.
 certifi = ">=2019.11.17"
 grpcio = [
   { version = ">=1.44.0", optional = true, python = "^3.8,<3.11" },
   { version = ">=1.59.0", optional = true, python = "^3.11" }
 ]
-grpc-gateway-protoc-gen-openapiv2 = { version = "0.1.0", optional = true }
 googleapis-common-protos = { version = ">=1.53.0", optional = true }
 lz4 = { version = ">=3.1.3", optional = true }
-protobuf = { version = "~=3.20.0", optional = true }
+protobuf = { version = "^4.25", optional = true }
+protoc-gen-openapiv2 = {version = "^0.0.1", optional = true }
 
 [tool.poetry.group.types]
 optional = true
 
 [tool.poetry.group.types.dependencies]
 mypy = "^1.6.1"
 types-urllib3 = "^1.26.25.14"
@@ -94,12 +94,12 @@
 pytest-cov = "2.10.1"
 pytest-mock = "3.6.1"
 pytest-timeout = "2.2.0"
 urllib3_mock = "0.3.3"
 responses = ">=0.8.1"
 
 [tool.poetry.extras]
-grpc = ["grpcio", "grpc-gateway-protoc-gen-openapiv2", "googleapis-common-protos", "lz4", "protobuf"]
+grpc = ["grpcio", "googleapis-common-protos", "lz4", "protobuf", "protoc-gen-openapiv2"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pinecone_client-3.2.2/PKG-INFO` & `pinecone_client-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-client
-Version: 3.2.2
+Version: 4.0.0
 Summary: Pinecone client and SDK
 Home-page: https://www.pinecone.io
 License: Apache-2.0
 Keywords: Pinecone,vector,database,cloud
 Author: Pinecone Systems, Inc.
 Author-email: support@pinecone.io
 Requires-Python: >=3.8,<4.0
@@ -25,19 +25,19 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: grpc
 Requires-Dist: certifi (>=2019.11.17)
 Requires-Dist: googleapis-common-protos (>=1.53.0) ; extra == "grpc"
-Requires-Dist: grpc-gateway-protoc-gen-openapiv2 (==0.1.0) ; extra == "grpc"
 Requires-Dist: grpcio (>=1.44.0) ; (python_version >= "3.8" and python_version < "3.11") and (extra == "grpc")
 Requires-Dist: grpcio (>=1.59.0) ; (python_version >= "3.11" and python_version < "4.0") and (extra == "grpc")
 Requires-Dist: lz4 (>=3.1.3) ; extra == "grpc"
-Requires-Dist: protobuf (>=3.20.0,<3.21.0) ; extra == "grpc"
+Requires-Dist: protobuf (>=4.25,<5.0) ; extra == "grpc"
+Requires-Dist: protoc-gen-openapiv2 (>=0.0.1,<0.0.2) ; extra == "grpc"
 Requires-Dist: tqdm (>=4.64.1)
 Requires-Dist: typing-extensions (>=3.7.4)
 Requires-Dist: urllib3 (>=1.26.0) ; python_version >= "3.8" and python_version < "3.12"
 Requires-Dist: urllib3 (>=1.26.5) ; python_version >= "3.12" and python_version < "4.0"
 Project-URL: Documentation, https://pinecone.io/docs
 Description-Content-Type: text/markdown
```


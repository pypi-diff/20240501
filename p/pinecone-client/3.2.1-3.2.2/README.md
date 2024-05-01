# Comparing `tmp/pinecone_client-3.2.1.tar.gz` & `tmp/pinecone_client-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_client-3.2.1.tar", max compression
+gzip compressed data, was "pinecone_client-3.2.2.tar", max compression
```

## Comparing `pinecone_client-3.2.1.tar` & `pinecone_client-3.2.2.tar`

### file list

```diff
@@ -1,100 +1,103 @@
--rw-r--r--   0        0        0    11356 2024-03-25 16:44:33.406969 pinecone_client-3.2.1/LICENSE.txt
--rw-r--r--   0        0        0    14522 2024-03-25 16:44:33.406969 pinecone_client-3.2.1/README.md
--rw-r--r--   0        0        0      394 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/__init__.py
--rw-r--r--   0        0        0        5 2024-03-25 16:44:33.482969 pinecone_client-3.2.1/pinecone/__version__
--rw-r--r--   0        0        0      199 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/config/__init__.py
--rw-r--r--   0        0        0     3228 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/config/config.py
--rw-r--r--   0        0        0     4626 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/config/openapi.py
--rw-r--r--   0        0        0      934 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/config/pinecone_config.py
--rw-r--r--   0        0        0       30 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/control/__init__.py
--rw-r--r--   0        0        0     1786 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/control/index_host_store.py
--rw-r--r--   0        0        0    24043 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/control/pinecone.py
--rw-r--r--   0        0        0        0 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/__init__.py
--rw-r--r--   0        0        0      907 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/__init__.py
--rw-r--r--   0        0        0      226 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/api/__init__.py
--rw-r--r--   0        0        0    44178 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/api/data_plane_api.py
--rw-r--r--   0        0        0    42885 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/api/manage_indexes_api.py
--rw-r--r--   0        0        0    37006 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/api_client.py
--rw-r--r--   0        0        0      556 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17137 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/configuration.py
--rw-r--r--   0        0        0     5270 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/__init__.py
--rw-r--r--   0        0        0    11433 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/collection_list.py
--rw-r--r--   0        0        0    13032 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/collection_model.py
--rw-r--r--   0        0        0    11527 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/configure_index_request.py
--rw-r--r--   0        0        0    11550 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/configure_index_request_spec.py
--rw-r--r--   0        0        0    12263 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/configure_index_request_spec_pod.py
--rw-r--r--   0        0        0    12063 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/create_collection_request.py
--rw-r--r--   0        0        0    13925 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/create_index_request.py
--rw-r--r--   0        0        0    12887 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/delete_request.py
--rw-r--r--   0        0        0    11726 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/describe_index_stats_request.py
--rw-r--r--   0        0        0    12925 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/describe_index_stats_response.py
--rw-r--r--   0        0        0    11746 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/error_response.py
--rw-r--r--   0        0        0    12829 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/error_response_error.py
--rw-r--r--   0        0        0    11910 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/fetch_response.py
--rw-r--r--   0        0        0    11363 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/index_list.py
--rw-r--r--   0        0        0    14018 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/index_model.py
--rw-r--r--   0        0        0    11695 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/index_model_spec.py
--rw-r--r--   0        0        0    11825 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/index_model_status.py
--rw-r--r--   0        0        0    11137 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/list_item.py
--rw-r--r--   0        0        0    12233 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/list_response.py
--rw-r--r--   0        0        0    11542 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/namespace_summary.py
--rw-r--r--   0        0        0    11153 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/pagination.py
--rw-r--r--   0        0        0    14766 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/pod_spec.py
--rw-r--r--   0        0        0    11495 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/pod_spec_metadata_config.py
--rw-r--r--   0        0        0    11358 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/protobuf_any.py
--rw-r--r--   0        0        0    12395 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/protobuf_null_value.py
--rw-r--r--   0        0        0    15451 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/query_request.py
--rw-r--r--   0        0        0    12553 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/query_response.py
--rw-r--r--   0        0        0    13170 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/query_vector.py
--rw-r--r--   0        0        0    11741 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/rpc_status.py
--rw-r--r--   0        0        0    12974 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/scored_vector.py
--rw-r--r--   0        0        0    12063 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/serverless_spec.py
--rw-r--r--   0        0        0    11731 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/single_query_results.py
--rw-r--r--   0        0        0    11533 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/sparse_values.py
--rw-r--r--   0        0        0    12778 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/update_request.py
--rw-r--r--   0        0        0    11918 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/upsert_request.py
--rw-r--r--   0        0        0    11280 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/upsert_response.py
--rw-r--r--   0        0        0    11275 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/usage.py
--rw-r--r--   0        0        0    12589 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model/vector.py
--rw-r--r--   0        0        0    80537 2024-03-25 16:44:33.410969 pinecone_client-3.2.1/pinecone/core/client/model_utils.py
--rw-r--r--   0        0        0     3104 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/core/client/models/__init__.py
--rw-r--r--   0        0        0    14204 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/core/client/rest.py
--rw-r--r--   0        0        0    76084 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/core/grpc/protos/vector_service_pb2.py
--rw-r--r--   0        0        0    24258 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/core/grpc/protos/vector_service_pb2.pyi
--rw-r--r--   0        0        0    14276 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0      299 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/data/__init__.py
--rw-r--r--   0        0        0    27458 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/data/index.py
--rw-r--r--   0        0        0     5329 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/data/vector_factory.py
--rw-r--r--   0        0        0     4027 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/deprecation_warnings.py
--rw-r--r--   0        0        0      874 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/exceptions.py
--rw-r--r--   0        0        0     1300 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/__init__.py
--rw-r--r--   0        0        0     5875 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/base.py
--rw-r--r--   0        0        0     1728 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/config.py
--rw-r--r--   0        0        0      961 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/future.py
--rw-r--r--   0        0        0    28020 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/index_grpc.py
--rw-r--r--   0        0        0     4166 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/pinecone.py
--rw-r--r--   0        0        0     3193 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/retry.py
--rw-r--r--   0        0        0     2996 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/utils.py
--rw-r--r--   0        0        0     5076 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/grpc/vector_factory_grpc.py
--rw-r--r--   0        0        0      534 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/models/__init__.py
--rw-r--r--   0        0        0      277 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/models/collection_description.py
--rw-r--r--   0        0        0      852 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/models/collection_list.py
--rw-r--r--   0        0        0     1330 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/models/index_description.py
--rw-r--r--   0        0        0      718 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/models/index_list.py
--rw-r--r--   0        0        0      198 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/models/list_response.py
--rw-r--r--   0        0        0     2189 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/models/pod_spec.py
--rw-r--r--   0        0        0      164 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/models/serverless_spec.py
--rw-r--r--   0        0        0      348 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/__init__.py
--rw-r--r--   0        0        0      288 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/check_kwargs.py
--rw-r--r--   0        0        0      722 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/constants.py
--rw-r--r--   0        0        0      247 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/convert_to_list.py
--rw-r--r--   0        0        0      263 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/deprecation_notice.py
--rw-r--r--   0        0        0      750 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/error_handling.py
--rw-r--r--   0        0        0      193 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/fix_tuple_length.py
--rw-r--r--   0        0        0      206 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/normalize_host.py
--rw-r--r--   0        0        0      527 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/setup_openapi_client.py
--rw-r--r--   0        0        0     1011 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/user_agent.py
--rw-r--r--   0        0        0      157 2024-03-25 16:44:33.414969 pinecone_client-3.2.1/pinecone/utils/version.py
--rw-r--r--   0        0        0     3295 2024-03-25 16:53:39.899256 pinecone_client-3.2.1/pyproject.toml
--rw-r--r--   0        0        0    16636 1970-01-01 00:00:00.000000 pinecone_client-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/LICENSE.txt
+-rw-r--r--   0        0        0    14522 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/README.md
+-rw-r--r--   0        0        0      394 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/__init__.py
+-rw-r--r--   0        0        0        5 2024-03-29 23:30:20.301139 pinecone_client-3.2.2/pinecone/__version__
+-rw-r--r--   0        0        0      199 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/config/__init__.py
+-rw-r--r--   0        0        0     3228 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/config/config.py
+-rw-r--r--   0        0        0     4258 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/config/openapi.py
+-rw-r--r--   0        0        0      934 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/config/pinecone_config.py
+-rw-r--r--   0        0        0       30 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/control/__init__.py
+-rw-r--r--   0        0        0     1786 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/control/index_host_store.py
+-rw-r--r--   0        0        0    24453 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/control/pinecone.py
+-rw-r--r--   0        0        0        0 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/__init__.py
+-rw-r--r--   0        0        0      907 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/client/__init__.py
+-rw-r--r--   0        0        0      226 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/client/api/__init__.py
+-rw-r--r--   0        0        0    44178 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/client/api/data_plane_api.py
+-rw-r--r--   0        0        0    42885 2024-03-29 23:30:20.233139 pinecone_client-3.2.2/pinecone/core/client/api/manage_indexes_api.py
+-rw-r--r--   0        0        0    37006 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/api_client.py
+-rw-r--r--   0        0        0      556 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17137 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/configuration.py
+-rw-r--r--   0        0        0     5270 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11433 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/collection_list.py
+-rw-r--r--   0        0        0    13032 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/collection_model.py
+-rw-r--r--   0        0        0    11527 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request.py
+-rw-r--r--   0        0        0    11550 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request_spec.py
+-rw-r--r--   0        0        0    12263 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request_spec_pod.py
+-rw-r--r--   0        0        0    12063 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/create_collection_request.py
+-rw-r--r--   0        0        0    13925 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/create_index_request.py
+-rw-r--r--   0        0        0    12887 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/delete_request.py
+-rw-r--r--   0        0        0    11726 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/describe_index_stats_request.py
+-rw-r--r--   0        0        0    12925 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/describe_index_stats_response.py
+-rw-r--r--   0        0        0    11746 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/error_response.py
+-rw-r--r--   0        0        0    12829 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/error_response_error.py
+-rw-r--r--   0        0        0    11910 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/fetch_response.py
+-rw-r--r--   0        0        0    11363 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/index_list.py
+-rw-r--r--   0        0        0    14018 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/index_model.py
+-rw-r--r--   0        0        0    11695 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/index_model_spec.py
+-rw-r--r--   0        0        0    11825 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/index_model_status.py
+-rw-r--r--   0        0        0    11137 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/list_item.py
+-rw-r--r--   0        0        0    12233 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/list_response.py
+-rw-r--r--   0        0        0    11542 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/namespace_summary.py
+-rw-r--r--   0        0        0    11153 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/pagination.py
+-rw-r--r--   0        0        0    14766 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/pod_spec.py
+-rw-r--r--   0        0        0    11495 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/pod_spec_metadata_config.py
+-rw-r--r--   0        0        0    11358 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/protobuf_any.py
+-rw-r--r--   0        0        0    12395 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/protobuf_null_value.py
+-rw-r--r--   0        0        0    15451 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/query_request.py
+-rw-r--r--   0        0        0    12553 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/query_response.py
+-rw-r--r--   0        0        0    13170 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/query_vector.py
+-rw-r--r--   0        0        0    11741 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/rpc_status.py
+-rw-r--r--   0        0        0    12974 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/scored_vector.py
+-rw-r--r--   0        0        0    12063 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/serverless_spec.py
+-rw-r--r--   0        0        0    11731 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/single_query_results.py
+-rw-r--r--   0        0        0    11533 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/sparse_values.py
+-rw-r--r--   0        0        0    12778 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/update_request.py
+-rw-r--r--   0        0        0    11918 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/upsert_request.py
+-rw-r--r--   0        0        0    11280 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/upsert_response.py
+-rw-r--r--   0        0        0    11275 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/usage.py
+-rw-r--r--   0        0        0    12589 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model/vector.py
+-rw-r--r--   0        0        0    80537 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/model_utils.py
+-rw-r--r--   0        0        0     3104 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14204 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/client/rest.py
+-rw-r--r--   0        0        0    76084 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2.py
+-rw-r--r--   0        0        0    24258 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    14276 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0      291 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/__init__.py
+-rw-r--r--   0        0        0     2125 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/errors.py
+-rw-r--r--   0        0        0    27458 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/index.py
+-rw-r--r--   0        0        0     1730 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/sparse_vector_factory.py
+-rw-r--r--   0        0        0     2815 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/data/vector_factory.py
+-rw-r--r--   0        0        0     4027 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/deprecation_warnings.py
+-rw-r--r--   0        0        0     1033 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/exceptions.py
+-rw-r--r--   0        0        0     1300 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/grpc/__init__.py
+-rw-r--r--   0        0        0     5875 2024-03-29 23:30:20.237139 pinecone_client-3.2.2/pinecone/grpc/base.py
+-rw-r--r--   0        0        0     1728 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/config.py
+-rw-r--r--   0        0        0      961 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/future.py
+-rw-r--r--   0        0        0    28020 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/index_grpc.py
+-rw-r--r--   0        0        0     4166 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/pinecone.py
+-rw-r--r--   0        0        0     3193 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/retry.py
+-rw-r--r--   0        0        0     2000 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/sparse_values_factory.py
+-rw-r--r--   0        0        0     2996 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/utils.py
+-rw-r--r--   0        0        0     3841 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/grpc/vector_factory_grpc.py
+-rw-r--r--   0        0        0      534 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/collection_description.py
+-rw-r--r--   0        0        0      852 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/collection_list.py
+-rw-r--r--   0        0        0     1330 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/index_description.py
+-rw-r--r--   0        0        0      718 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/index_list.py
+-rw-r--r--   0        0        0      198 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/list_response.py
+-rw-r--r--   0        0        0     2189 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/pod_spec.py
+-rw-r--r--   0        0        0      164 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/models/serverless_spec.py
+-rw-r--r--   0        0        0      348 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/__init__.py
+-rw-r--r--   0        0        0      288 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/check_kwargs.py
+-rw-r--r--   0        0        0      722 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/constants.py
+-rw-r--r--   0        0        0      785 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/convert_to_list.py
+-rw-r--r--   0        0        0      263 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/deprecation_notice.py
+-rw-r--r--   0        0        0      750 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/error_handling.py
+-rw-r--r--   0        0        0      193 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/fix_tuple_length.py
+-rw-r--r--   0        0        0      206 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/normalize_host.py
+-rw-r--r--   0        0        0      527 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/setup_openapi_client.py
+-rw-r--r--   0        0        0     1011 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/user_agent.py
+-rw-r--r--   0        0        0      157 2024-03-29 23:30:20.241139 pinecone_client-3.2.2/pinecone/utils/version.py
+-rw-r--r--   0        0        0     3295 2024-03-29 23:38:38.627886 pinecone_client-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0    16636 1970-01-01 00:00:00.000000 pinecone_client-3.2.2/PKG-INFO
```

### Comparing `pinecone_client-3.2.1/LICENSE.txt` & `pinecone_client-3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/README.md` & `pinecone_client-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/config/config.py` & `pinecone_client-3.2.2/pinecone/config/config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/config/openapi.py` & `pinecone_client-3.2.2/pinecone/config/openapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 from typing import List, Optional
 
 import certifi
 import socket
 import copy
-import warnings
 
 from urllib3.connection import HTTPConnection
 
 from pinecone.core.client.configuration import Configuration as OpenApiConfiguration
 
 TCP_KEEPINTVL = 60  # Sec
 TCP_KEEPIDLE = 300  # Sec
@@ -30,15 +29,14 @@
         '''
         Copy a user-supplied openapi configuration and update it with the user's api key and host. 
         If they have not specified other socket configuration, we will use the default values.
         We expect these objects are being passed mainly a vehicle for proxy configuration, so 
         we don't modify those settings.
         '''
         copied = copy.deepcopy(openapi_config)
-        warnings.warn("Passing openapi_config is deprecated and will be removed in a future release. Please pass settings such as proxy_url, proxy_headers, ssl_ca_certs, and ssl_verify directly to the Pinecone constructor as keyword arguments. See the README at https://github.com/pinecone-io/pinecone-python-client for examples.", DeprecationWarning)
 
         copied.api_key = {"ApiKeyAuth": api_key}
         copied.host = host
 
         # Set sensible defaults if the user hasn't set them
         if not copied.socket_options:
             copied.socket_options = cls._get_socket_options()
```

### Comparing `pinecone_client-3.2.1/pinecone/config/pinecone_config.py` & `pinecone_client-3.2.2/pinecone/config/pinecone_config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/control/index_host_store.py` & `pinecone_client-3.2.2/pinecone/control/index_host_store.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/control/pinecone.py` & `pinecone_client-3.2.2/pinecone/control/pinecone.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import warnings
 from typing import Optional, Dict, Any, Union, List, cast, NamedTuple
 
 from .index_host_store import IndexHostStore
 
 from pinecone.config import PineconeConfig, Config, ConfigBuilder
 
 from pinecone.core.client.api.manage_indexes_api import ManageIndexesApi
@@ -170,16 +171,14 @@
             ssl_ca_certs='path/to/cert-bundle.pem',
             ssl_verify=False
         )
 
         pc.list_indexes()
 
         ```
-        
-
         """
         if config:
             if not isinstance(config, Config):
                 raise TypeError("config must be of type pinecone.config.Config")
             else:
                 self.config = config
         else:
@@ -190,14 +189,17 @@
                 proxy_url=proxy_url,
                 proxy_headers=proxy_headers,
                 ssl_ca_certs=ssl_ca_certs,
                 ssl_verify=ssl_verify,
                 **kwargs
             )
 
+        if kwargs.get("openapi_config", None):
+            warnings.warn("Passing openapi_config is deprecated and will be removed in a future release. Please pass settings such as proxy_url, proxy_headers, ssl_ca_certs, and ssl_verify directly to the Pinecone constructor as keyword arguments. See the README at https://github.com/pinecone-io/pinecone-python-client for examples.", DeprecationWarning)
+
         self.openapi_config = ConfigBuilder.build_openapi_config(self.config, **kwargs)
         self.pool_threads = pool_threads
 
         if index_api:
             self.index_api = index_api
         else:
             self.index_api = setup_openapi_client(ManageIndexesApi, self.config, self.openapi_config, pool_threads)
```

### Comparing `pinecone_client-3.2.1/pinecone/core/client/__init__.py` & `pinecone_client-3.2.2/pinecone/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/api/data_plane_api.py` & `pinecone_client-3.2.2/pinecone/core/client/api/data_plane_api.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/api/manage_indexes_api.py` & `pinecone_client-3.2.2/pinecone/core/client/api/manage_indexes_api.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/api_client.py` & `pinecone_client-3.2.2/pinecone/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/apis/__init__.py` & `pinecone_client-3.2.2/pinecone/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/configuration.py` & `pinecone_client-3.2.2/pinecone/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/exceptions.py` & `pinecone_client-3.2.2/pinecone/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/collection_list.py` & `pinecone_client-3.2.2/pinecone/core/client/model/collection_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/collection_model.py` & `pinecone_client-3.2.2/pinecone/core/client/model/collection_model.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/configure_index_request.py` & `pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/configure_index_request_spec.py` & `pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/configure_index_request_spec_pod.py` & `pinecone_client-3.2.2/pinecone/core/client/model/configure_index_request_spec_pod.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/create_collection_request.py` & `pinecone_client-3.2.2/pinecone/core/client/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/create_index_request.py` & `pinecone_client-3.2.2/pinecone/core/client/model/create_index_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/delete_request.py` & `pinecone_client-3.2.2/pinecone/core/client/model/delete_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/describe_index_stats_request.py` & `pinecone_client-3.2.2/pinecone/core/client/model/describe_index_stats_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/describe_index_stats_response.py` & `pinecone_client-3.2.2/pinecone/core/client/model/describe_index_stats_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/error_response.py` & `pinecone_client-3.2.2/pinecone/core/client/model/error_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/error_response_error.py` & `pinecone_client-3.2.2/pinecone/core/client/model/error_response_error.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/fetch_response.py` & `pinecone_client-3.2.2/pinecone/core/client/model/fetch_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/index_list.py` & `pinecone_client-3.2.2/pinecone/core/client/model/index_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/index_model.py` & `pinecone_client-3.2.2/pinecone/core/client/model/index_model.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/index_model_spec.py` & `pinecone_client-3.2.2/pinecone/core/client/model/index_model_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/index_model_status.py` & `pinecone_client-3.2.2/pinecone/core/client/model/index_model_status.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/list_item.py` & `pinecone_client-3.2.2/pinecone/core/client/model/list_item.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/list_response.py` & `pinecone_client-3.2.2/pinecone/core/client/model/list_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/namespace_summary.py` & `pinecone_client-3.2.2/pinecone/core/client/model/namespace_summary.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/pagination.py` & `pinecone_client-3.2.2/pinecone/core/client/model/pagination.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/pod_spec.py` & `pinecone_client-3.2.2/pinecone/core/client/model/pod_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/pod_spec_metadata_config.py` & `pinecone_client-3.2.2/pinecone/core/client/model/pod_spec_metadata_config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/protobuf_any.py` & `pinecone_client-3.2.2/pinecone/core/client/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/protobuf_null_value.py` & `pinecone_client-3.2.2/pinecone/core/client/model/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/query_request.py` & `pinecone_client-3.2.2/pinecone/core/client/model/query_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/query_response.py` & `pinecone_client-3.2.2/pinecone/core/client/model/query_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/query_vector.py` & `pinecone_client-3.2.2/pinecone/core/client/model/query_vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/rpc_status.py` & `pinecone_client-3.2.2/pinecone/core/client/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/scored_vector.py` & `pinecone_client-3.2.2/pinecone/core/client/model/scored_vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/serverless_spec.py` & `pinecone_client-3.2.2/pinecone/core/client/model/serverless_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/single_query_results.py` & `pinecone_client-3.2.2/pinecone/core/client/model/single_query_results.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/sparse_values.py` & `pinecone_client-3.2.2/pinecone/core/client/model/sparse_values.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/update_request.py` & `pinecone_client-3.2.2/pinecone/core/client/model/update_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/upsert_request.py` & `pinecone_client-3.2.2/pinecone/core/client/model/upsert_request.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/upsert_response.py` & `pinecone_client-3.2.2/pinecone/core/client/model/upsert_response.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/usage.py` & `pinecone_client-3.2.2/pinecone/core/client/model/usage.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model/vector.py` & `pinecone_client-3.2.2/pinecone/core/client/model/vector.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/model_utils.py` & `pinecone_client-3.2.2/pinecone/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/models/__init__.py` & `pinecone_client-3.2.2/pinecone/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/client/rest.py` & `pinecone_client-3.2.2/pinecone/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/grpc/protos/vector_service_pb2.py` & `pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/grpc/protos/vector_service_pb2.pyi` & `pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/core/grpc/protos/vector_service_pb2_grpc.py` & `pinecone_client-3.2.2/pinecone/core/grpc/protos/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/data/index.py` & `pinecone_client-3.2.2/pinecone/data/index.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/deprecation_warnings.py` & `pinecone_client-3.2.2/pinecone/deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/grpc/__init__.py` & `pinecone_client-3.2.2/pinecone/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/grpc/base.py` & `pinecone_client-3.2.2/pinecone/grpc/base.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/grpc/config.py` & `pinecone_client-3.2.2/pinecone/grpc/config.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/grpc/future.py` & `pinecone_client-3.2.2/pinecone/grpc/future.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/grpc/index_grpc.py` & `pinecone_client-3.2.2/pinecone/grpc/index_grpc.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/grpc/pinecone.py` & `pinecone_client-3.2.2/pinecone/grpc/pinecone.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/grpc/retry.py` & `pinecone_client-3.2.2/pinecone/grpc/retry.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/grpc/utils.py` & `pinecone_client-3.2.2/pinecone/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/models/__init__.py` & `pinecone_client-3.2.2/pinecone/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/models/collection_list.py` & `pinecone_client-3.2.2/pinecone/models/collection_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/models/index_description.py` & `pinecone_client-3.2.2/pinecone/models/index_description.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/models/index_list.py` & `pinecone_client-3.2.2/pinecone/models/index_list.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/models/pod_spec.py` & `pinecone_client-3.2.2/pinecone/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/utils/constants.py` & `pinecone_client-3.2.2/pinecone/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/utils/error_handling.py` & `pinecone_client-3.2.2/pinecone/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/utils/setup_openapi_client.py` & `pinecone_client-3.2.2/pinecone/utils/setup_openapi_client.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pinecone/utils/user_agent.py` & `pinecone_client-3.2.2/pinecone/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `pinecone_client-3.2.1/pyproject.toml` & `pinecone_client-3.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
 
 [tool.poetry]
 name = "pinecone-client"
-version = "3.2.1"
+version = "3.2.2"
 packages = [
     { include="pinecone", from="." },
 ]
 description = "Pinecone client and SDK"
 authors = ["Pinecone Systems, Inc. <support@pinecone.io>"]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `pinecone_client-3.2.1/PKG-INFO` & `pinecone_client-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-client
-Version: 3.2.1
+Version: 3.2.2
 Summary: Pinecone client and SDK
 Home-page: https://www.pinecone.io
 License: Apache-2.0
 Keywords: Pinecone,vector,database,cloud
 Author: Pinecone Systems, Inc.
 Author-email: support@pinecone.io
 Requires-Python: >=3.8,<4.0
```


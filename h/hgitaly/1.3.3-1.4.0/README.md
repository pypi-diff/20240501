# Comparing `tmp/hgitaly-1.3.3.tar.gz` & `tmp/hgitaly-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgitaly-1.3.3.tar", last modified: Wed Mar 20 15:54:27 2024, max compression
+gzip compressed data, was "hgitaly-1.4.0.tar", last modified: Wed May  1 15:45:12 2024, max compression
```

## Comparing `hgitaly-1.3.3.tar` & `hgitaly-1.4.0.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.124352 hgitaly-1.3.3/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2022-07-07 20:49:19.000000 hgitaly-1.3.3/LICENSE
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2022-07-07 20:49:19.000000 hgitaly-1.3.3/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-03-20 15:54:27.123352 hgitaly-1.3.3/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15287 2024-02-14 14:38:06.000000 hgitaly-1.3.3/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.106352 hgitaly-1.3.3/hgext3rd/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgext3rd/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.106352 hgitaly-1.3.3/hgext3rd/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4418 2024-02-14 14:38:06.000000 hgitaly-1.3.3/hgext3rd/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1551 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgext3rd/hgitaly/revset.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.106352 hgitaly-1.3.3/hgext3rd/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgext3rd/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2021 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgext3rd/hgitaly/tests/test_revset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5392 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgext3rd/hgitaly/tests/test_serve.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.109352 hgitaly-1.3.3/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-03-20 15:33:52.000000 hgitaly-1.3.3/hgitaly/VERSION
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      361 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13506 2023-11-13 22:51:48.000000 hgitaly-1.3.3/hgitaly/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      744 2023-11-13 22:51:48.000000 hgitaly-1.3.3/hgitaly/changelog.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13280 2024-03-14 20:29:38.000000 hgitaly-1.3.3/hgitaly/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4209 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2749 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/feature.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      701 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/file_context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4495 2024-02-14 14:38:06.000000 hgitaly-1.3.3/hgitaly/git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6908 2023-11-13 22:51:48.000000 hgitaly-1.3.3/hgitaly/gitlab_ref.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.110352 hgitaly-1.3.3/hgitaly/license_detector/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4650 2023-11-21 17:47:45.000000 hgitaly-1.3.3/hgitaly/license_detector/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   270608 2023-11-21 17:47:45.000000 hgitaly-1.3.3/hgitaly/license_detector/spdx-licenses.json
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.111352 hgitaly-1.3.3/hgitaly/linguist/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6420 2023-11-13 22:51:48.000000 hgitaly-1.3.3/hgitaly/linguist/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   122122 2023-11-13 22:51:48.000000 hgitaly-1.3.3/hgitaly/linguist/languages.json
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1183 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/logging.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10350 2023-11-13 22:51:48.000000 hgitaly-1.3.3/hgitaly/manifest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9596 2024-02-14 14:38:06.000000 hgitaly-1.3.3/hgitaly/message.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1506 2024-03-14 20:29:38.000000 hgitaly-1.3.3/hgitaly/oid.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      953 2022-07-20 18:29:40.000000 hgitaly-1.3.3/hgitaly/pagination.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/path.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3252 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/peer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      711 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/procutil.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8872 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7891 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5689 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/revset.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.111352 hgitaly-1.3.3/hgitaly/server/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      417 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1683 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/address.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6087 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/server/mono.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7216 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/prefork.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.112352 hgitaly-1.3.3/hgitaly/server/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1256 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/tests/test_address.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3272 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/tests/test_mono.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6502 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/tests/test_prefork.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3704 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/tests/test_worker.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3748 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/server/worker.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.113352 hgitaly-1.3.3/hgitaly/service/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/service/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5013 2023-09-04 20:36:56.000000 hgitaly-1.3.3/hgitaly/service/blob.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    46333 2024-03-20 15:32:40.000000 hgitaly-1.3.3/hgitaly/service/commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25147 2024-02-14 14:38:06.000000 hgitaly-1.3.3/hgitaly/service/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2217 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/service/interceptors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1954 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/service/mercurial_changeset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16643 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/service/mercurial_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7480 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/service/mercurial_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9852 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/service/operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23474 2024-03-20 15:32:40.000000 hgitaly-1.3.3/hgitaly/service/ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    35623 2024-03-14 20:29:37.000000 hgitaly-1.3.3/hgitaly/service/repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      769 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/service/server.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.115352 hgitaly-1.3.3/hgitaly/service/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/service/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7380 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/service/tests/fixture.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4628 2023-09-04 20:36:56.000000 hgitaly-1.3.3/hgitaly/service/tests/test_blob.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    52626 2024-03-20 15:32:40.000000 hgitaly-1.3.3/hgitaly/service/tests/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2020 2023-11-14 22:18:49.000000 hgitaly-1.3.3/hgitaly/service/tests/test_default_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26417 2024-02-14 14:38:06.000000 hgitaly-1.3.3/hgitaly/service/tests/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2973 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/service/tests/test_mercurial_changeset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22959 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/service/tests/test_mercurial_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18968 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/service/tests/test_mercurial_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10594 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/service/tests/test_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22409 2024-03-20 15:32:40.000000 hgitaly-1.3.3/hgitaly/service/tests/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    49404 2024-03-14 20:29:37.000000 hgitaly-1.3.3/hgitaly/service/tests/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      721 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/service/tests/test_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17084 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1331 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/ssh.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5895 2024-02-14 14:38:06.000000 hgitaly-1.3.3/hgitaly/stream.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.118352 hgitaly-1.3.3/hgitaly/stub/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/stub/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9260 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/blob_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12934 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/stub/blob_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32146 2024-03-14 20:29:38.000000 hgitaly-1.3.3/hgitaly/stub/commit_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39150 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/commit_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13033 2024-03-14 20:29:38.000000 hgitaly-1.3.3/hgitaly/stub/diff_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12544 2024-03-14 20:29:38.000000 hgitaly-1.3.3/hgitaly/stub/diff_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6477 2024-03-14 20:29:38.000000 hgitaly-1.3.3/hgitaly/stub/errors_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/stub/errors_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2922 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/lint_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/stub/lint_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4218 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/mercurial_changeset_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2901 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/stub/mercurial_changeset_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7531 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/stub/mercurial_operations_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7995 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/stub/mercurial_operations_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11048 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/stub/mercurial_repository_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17065 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/stub/mercurial_repository_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29044 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/operations_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32883 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/operations_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    20829 2024-02-14 14:37:31.000000 hgitaly-1.3.3/hgitaly/stub/ref_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29202 2024-02-14 14:37:31.000000 hgitaly-1.3.3/hgitaly/stub/ref_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    47292 2024-03-14 20:29:38.000000 hgitaly-1.3.3/hgitaly/stub/repository_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    79381 2024-03-14 20:29:38.000000 hgitaly-1.3.3/hgitaly/stub/repository_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5080 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/server_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7231 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/server_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5996 2024-01-20 14:39:14.000000 hgitaly-1.3.3/hgitaly/stub/shared_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/stub/shared_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1653 2023-11-13 22:51:48.000000 hgitaly-1.3.3/hgitaly/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.119352 hgitaly-1.3.3/hgitaly/testing/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      317 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/testing/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1278 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/testing/bundle.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2828 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/testing/context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      901 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/testing/grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1147 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/testing/ssh.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3920 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/testing/sshd.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.119352 hgitaly-1.3.3/hgitaly/testing/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/testing/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1191 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/testing/tests/test_sshd.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.122352 hgitaly-1.3.3/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4609 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/tests/common.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9403 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3605 2024-02-14 14:38:06.000000 hgitaly-1.3.3/hgitaly/tests/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2024-02-13 21:06:34.000000 hgitaly-1.3.3/hgitaly/tests/test_errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_feature.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1439 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/tests/test_file_context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4599 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_gitlab_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1495 2023-11-21 17:47:45.000000 hgitaly-1.3.3/hgitaly/tests/test_license_detector.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1547 2023-11-21 17:47:45.000000 hgitaly-1.3.3/hgitaly/tests/test_linguist.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5582 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/tests/test_manifest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3374 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_messages.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1114 2022-07-07 20:49:19.000000 hgitaly-1.3.3/hgitaly/tests/test_oid.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1669 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_peer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      582 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      679 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_revset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10160 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/tests/test_servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1951 2024-02-14 14:38:06.000000 hgitaly-1.3.3/hgitaly/tests/test_stream.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1315 2023-07-26 15:42:21.000000 hgitaly-1.3.3/hgitaly/tests/test_tag.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24221 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/tests/test_workdir.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2017 2023-11-13 22:51:48.000000 hgitaly-1.3.3/hgitaly/util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14533 2024-01-20 11:36:48.000000 hgitaly-1.3.3/hgitaly/workdir.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.110352 hgitaly-1.3.3/hgitaly.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-03-20 15:54:27.000000 hgitaly-1.3.3/hgitaly.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4526 2024-03-20 15:54:27.000000 hgitaly-1.3.3/hgitaly.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-03-20 15:54:27.000000 hgitaly-1.3.3/hgitaly.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-03-20 15:54:27.000000 hgitaly-1.3.3/hgitaly.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2024-03-20 15:54:27.000000 hgitaly-1.3.3/hgitaly.egg-info/top_level.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-02-13 21:06:34.000000 hgitaly-1.3.3/install-requirements.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-03-20 15:54:27.124352 hgitaly-1.3.3/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      968 2023-11-21 17:46:05.000000 hgitaly-1.3.3/setup.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-03-20 15:54:27.123352 hgitaly-1.3.3/tests_with_gitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2437 2023-07-26 15:42:21.000000 hgitaly-1.3.3/tests_with_gitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23180 2024-02-13 21:06:34.000000 hgitaly-1.3.3/tests_with_gitaly/comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3545 2023-07-26 15:42:21.000000 hgitaly-1.3.3/tests_with_gitaly/conftest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2455 2023-07-26 15:42:21.000000 hgitaly-1.3.3/tests_with_gitaly/gitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1775 2023-07-26 15:42:21.000000 hgitaly-1.3.3/tests_with_gitaly/hgitaly_rhgitaly_comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2509 2024-03-14 20:29:37.000000 hgitaly-1.3.3/tests_with_gitaly/rhgitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    19479 2024-03-14 20:29:38.000000 hgitaly-1.3.3/tests_with_gitaly/test_blob_tree.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    31080 2024-03-14 20:29:38.000000 hgitaly-1.3.3/tests_with_gitaly/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3284 2023-07-26 15:42:21.000000 hgitaly-1.3.3/tests_with_gitaly/test_comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29596 2024-03-14 20:29:38.000000 hgitaly-1.3.3/tests_with_gitaly/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1371 2023-07-26 15:42:21.000000 hgitaly-1.3.3/tests_with_gitaly/test_gitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11653 2024-02-13 21:06:34.000000 hgitaly-1.3.3/tests_with_gitaly/test_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17745 2024-03-20 15:32:40.000000 hgitaly-1.3.3/tests_with_gitaly/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32102 2024-03-14 20:29:38.000000 hgitaly-1.3.3/tests_with_gitaly/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      941 2023-07-26 15:42:21.000000 hgitaly-1.3.3/tests_with_gitaly/test_rhgitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      820 2023-07-26 15:42:21.000000 hgitaly-1.3.3/tests_with_gitaly/test_server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.305377 hgitaly-1.4.0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2022-07-07 20:49:19.000000 hgitaly-1.4.0/LICENSE
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2022-07-07 20:49:19.000000 hgitaly-1.4.0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-01 15:45:12.305377 hgitaly-1.4.0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15287 2024-02-14 14:38:06.000000 hgitaly-1.4.0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.291377 hgitaly-1.4.0/hgext3rd/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgext3rd/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.291377 hgitaly-1.4.0/hgext3rd/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4418 2024-02-14 14:38:06.000000 hgitaly-1.4.0/hgext3rd/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1551 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgext3rd/hgitaly/revset.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.291377 hgitaly-1.4.0/hgext3rd/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgext3rd/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2021 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgext3rd/hgitaly/tests/test_revset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5392 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgext3rd/hgitaly/tests/test_serve.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.294377 hgitaly-1.4.0/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-05-01 15:43:00.000000 hgitaly-1.4.0/hgitaly/VERSION
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      361 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13506 2023-11-13 22:51:48.000000 hgitaly-1.4.0/hgitaly/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      744 2023-11-13 22:51:48.000000 hgitaly-1.4.0/hgitaly/changelog.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13280 2024-04-03 07:33:18.000000 hgitaly-1.4.0/hgitaly/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4209 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2749 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/feature.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      701 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/file_context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4495 2024-02-14 14:38:06.000000 hgitaly-1.4.0/hgitaly/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6908 2023-11-13 22:51:48.000000 hgitaly-1.4.0/hgitaly/gitlab_ref.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.294377 hgitaly-1.4.0/hgitaly/license_detector/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4650 2023-11-21 17:47:45.000000 hgitaly-1.4.0/hgitaly/license_detector/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   270608 2023-11-21 17:47:45.000000 hgitaly-1.4.0/hgitaly/license_detector/spdx-licenses.json
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.295377 hgitaly-1.4.0/hgitaly/linguist/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6420 2023-11-13 22:51:48.000000 hgitaly-1.4.0/hgitaly/linguist/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   122122 2023-11-13 22:51:48.000000 hgitaly-1.4.0/hgitaly/linguist/languages.json
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1183 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/logging.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10350 2023-11-13 22:51:48.000000 hgitaly-1.4.0/hgitaly/manifest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9596 2024-02-14 14:38:06.000000 hgitaly-1.4.0/hgitaly/message.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1506 2024-04-03 07:33:18.000000 hgitaly-1.4.0/hgitaly/oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      953 2022-07-20 18:29:40.000000 hgitaly-1.4.0/hgitaly/pagination.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/path.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3252 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/peer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      711 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/procutil.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8872 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7891 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5689 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/revset.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.295377 hgitaly-1.4.0/hgitaly/server/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      417 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1683 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/address.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6087 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/server/mono.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7216 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/prefork.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.295377 hgitaly-1.4.0/hgitaly/server/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1256 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/tests/test_address.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3272 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/tests/test_mono.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6502 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/tests/test_prefork.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3704 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/tests/test_worker.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3748 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/server/worker.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.297377 hgitaly-1.4.0/hgitaly/service/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/service/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5013 2023-09-04 20:36:56.000000 hgitaly-1.4.0/hgitaly/service/blob.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    46662 2024-05-01 15:41:47.000000 hgitaly-1.4.0/hgitaly/service/commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25147 2024-02-14 14:38:06.000000 hgitaly-1.4.0/hgitaly/service/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2217 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/service/interceptors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1954 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/service/mercurial_changeset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16868 2024-04-19 09:36:41.000000 hgitaly-1.4.0/hgitaly/service/mercurial_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7480 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/service/mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9852 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/service/operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23474 2024-04-03 07:33:18.000000 hgitaly-1.4.0/hgitaly/service/ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    35623 2024-03-14 20:29:37.000000 hgitaly-1.4.0/hgitaly/service/repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      769 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/service/server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.298377 hgitaly-1.4.0/hgitaly/service/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/service/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7380 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/service/tests/fixture.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4628 2023-09-04 20:36:56.000000 hgitaly-1.4.0/hgitaly/service/tests/test_blob.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    52689 2024-04-19 09:36:41.000000 hgitaly-1.4.0/hgitaly/service/tests/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2020 2023-11-14 22:18:49.000000 hgitaly-1.4.0/hgitaly/service/tests/test_default_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26417 2024-02-14 14:38:06.000000 hgitaly-1.4.0/hgitaly/service/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2973 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/service/tests/test_mercurial_changeset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22959 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/service/tests/test_mercurial_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18968 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/service/tests/test_mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10594 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/service/tests/test_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22409 2024-04-03 07:33:18.000000 hgitaly-1.4.0/hgitaly/service/tests/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    49404 2024-03-14 20:29:37.000000 hgitaly-1.4.0/hgitaly/service/tests/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      721 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/service/tests/test_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17084 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1331 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/ssh.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5895 2024-02-14 14:38:06.000000 hgitaly-1.4.0/hgitaly/stream.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.301377 hgitaly-1.4.0/hgitaly/stub/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/stub/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9342 2024-04-19 09:36:41.000000 hgitaly-1.4.0/hgitaly/stub/blob_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12934 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/stub/blob_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32146 2024-04-03 07:33:18.000000 hgitaly-1.4.0/hgitaly/stub/commit_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39150 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/stub/commit_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16478 2024-04-19 09:36:41.000000 hgitaly-1.4.0/hgitaly/stub/diff_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15634 2024-04-19 09:36:41.000000 hgitaly-1.4.0/hgitaly/stub/diff_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6477 2024-04-03 07:33:18.000000 hgitaly-1.4.0/hgitaly/stub/errors_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/stub/errors_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2922 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/stub/lint_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/stub/lint_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4218 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/stub/mercurial_changeset_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2901 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7531 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/stub/mercurial_operations_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7995 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/stub/mercurial_operations_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11048 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/stub/mercurial_repository_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17065 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/stub/mercurial_repository_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29658 2024-04-19 09:36:41.000000 hgitaly-1.4.0/hgitaly/stub/operations_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32883 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/stub/operations_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    20829 2024-02-14 14:37:31.000000 hgitaly-1.4.0/hgitaly/stub/ref_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29202 2024-02-14 14:37:31.000000 hgitaly-1.4.0/hgitaly/stub/ref_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    47292 2024-04-03 07:33:18.000000 hgitaly-1.4.0/hgitaly/stub/repository_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    79550 2024-04-19 09:36:41.000000 hgitaly-1.4.0/hgitaly/stub/repository_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5080 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/stub/server_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7231 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/stub/server_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5996 2024-01-20 14:39:14.000000 hgitaly-1.4.0/hgitaly/stub/shared_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/stub/shared_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1653 2023-11-13 22:51:48.000000 hgitaly-1.4.0/hgitaly/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.301377 hgitaly-1.4.0/hgitaly/testing/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      317 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/testing/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1278 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/testing/bundle.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2828 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/testing/context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      901 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/testing/grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1147 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/testing/ssh.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3920 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/testing/sshd.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.301377 hgitaly-1.4.0/hgitaly/testing/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/testing/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1191 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/testing/tests/test_sshd.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.303377 hgitaly-1.4.0/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4609 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/tests/common.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9403 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3605 2024-02-14 14:38:06.000000 hgitaly-1.4.0/hgitaly/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2024-02-13 21:06:34.000000 hgitaly-1.4.0/hgitaly/tests/test_errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_feature.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1439 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/tests/test_file_context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4599 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_gitlab_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1495 2023-11-21 17:47:45.000000 hgitaly-1.4.0/hgitaly/tests/test_license_detector.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1547 2023-11-21 17:47:45.000000 hgitaly-1.4.0/hgitaly/tests/test_linguist.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5582 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/tests/test_manifest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3374 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_messages.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1114 2022-07-07 20:49:19.000000 hgitaly-1.4.0/hgitaly/tests/test_oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1669 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_peer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      582 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      679 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_revset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10160 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/tests/test_servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1951 2024-02-14 14:38:06.000000 hgitaly-1.4.0/hgitaly/tests/test_stream.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1315 2023-07-26 15:42:21.000000 hgitaly-1.4.0/hgitaly/tests/test_tag.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24221 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/tests/test_workdir.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2017 2023-11-13 22:51:48.000000 hgitaly-1.4.0/hgitaly/util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14533 2024-01-20 11:36:48.000000 hgitaly-1.4.0/hgitaly/workdir.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.294377 hgitaly-1.4.0/hgitaly.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-01 15:45:12.000000 hgitaly-1.4.0/hgitaly.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4526 2024-05-01 15:45:12.000000 hgitaly-1.4.0/hgitaly.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-05-01 15:45:12.000000 hgitaly-1.4.0/hgitaly.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-01 15:45:12.000000 hgitaly-1.4.0/hgitaly.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2024-05-01 15:45:12.000000 hgitaly-1.4.0/hgitaly.egg-info/top_level.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-02-13 21:06:34.000000 hgitaly-1.4.0/install-requirements.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-05-01 15:45:12.305377 hgitaly-1.4.0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      968 2023-11-21 17:46:05.000000 hgitaly-1.4.0/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-01 15:45:12.305377 hgitaly-1.4.0/tests_with_gitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2437 2023-07-26 15:42:21.000000 hgitaly-1.4.0/tests_with_gitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23180 2024-02-13 21:06:34.000000 hgitaly-1.4.0/tests_with_gitaly/comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3545 2023-07-26 15:42:21.000000 hgitaly-1.4.0/tests_with_gitaly/conftest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2455 2023-07-26 15:42:21.000000 hgitaly-1.4.0/tests_with_gitaly/gitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1775 2023-07-26 15:42:21.000000 hgitaly-1.4.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2509 2024-03-14 20:29:37.000000 hgitaly-1.4.0/tests_with_gitaly/rhgitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    19479 2024-04-03 07:33:18.000000 hgitaly-1.4.0/tests_with_gitaly/test_blob_tree.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    31285 2024-05-01 15:41:47.000000 hgitaly-1.4.0/tests_with_gitaly/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3284 2023-07-26 15:42:21.000000 hgitaly-1.4.0/tests_with_gitaly/test_comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29596 2024-04-03 07:33:18.000000 hgitaly-1.4.0/tests_with_gitaly/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1371 2023-07-26 15:42:21.000000 hgitaly-1.4.0/tests_with_gitaly/test_gitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11653 2024-02-13 21:06:34.000000 hgitaly-1.4.0/tests_with_gitaly/test_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17745 2024-04-03 07:33:18.000000 hgitaly-1.4.0/tests_with_gitaly/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32102 2024-04-03 07:33:18.000000 hgitaly-1.4.0/tests_with_gitaly/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      941 2023-07-26 15:42:21.000000 hgitaly-1.4.0/tests_with_gitaly/test_rhgitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      820 2023-07-26 15:42:21.000000 hgitaly-1.4.0/tests_with_gitaly/test_server.py
```

### Comparing `hgitaly-1.3.3/LICENSE` & `hgitaly-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/PKG-INFO` & `hgitaly-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 1.3.3
+Version: 1.4.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Requires-Python: >=3.8
```

### Comparing `hgitaly-1.3.3/README.md` & `hgitaly-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgext3rd/hgitaly/__init__.py` & `hgitaly-1.4.0/hgext3rd/hgitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgext3rd/hgitaly/revset.py` & `hgitaly-1.4.0/hgext3rd/hgitaly/revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgext3rd/hgitaly/tests/test_revset.py` & `hgitaly-1.4.0/hgext3rd/hgitaly/tests/test_revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgext3rd/hgitaly/tests/test_serve.py` & `hgitaly-1.4.0/hgext3rd/hgitaly/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/branch.py` & `hgitaly-1.4.0/hgitaly/branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/changelog.py` & `hgitaly-1.4.0/hgitaly/changelog.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/diff.py` & `hgitaly-1.4.0/hgitaly/diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/errors.py` & `hgitaly-1.4.0/hgitaly/errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/feature.py` & `hgitaly-1.4.0/hgitaly/feature.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/file_context.py` & `hgitaly-1.4.0/hgitaly/file_context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/git.py` & `hgitaly-1.4.0/hgitaly/git.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/gitlab_ref.py` & `hgitaly-1.4.0/hgitaly/gitlab_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/license_detector/__init__.py` & `hgitaly-1.4.0/hgitaly/license_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/license_detector/spdx-licenses.json` & `hgitaly-1.4.0/hgitaly/license_detector/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/linguist/__init__.py` & `hgitaly-1.4.0/hgitaly/linguist/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/linguist/languages.json` & `hgitaly-1.4.0/hgitaly/linguist/languages.json`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/logging.py` & `hgitaly-1.4.0/hgitaly/logging.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/manifest.py` & `hgitaly-1.4.0/hgitaly/manifest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/message.py` & `hgitaly-1.4.0/hgitaly/message.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/oid.py` & `hgitaly-1.4.0/hgitaly/oid.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/pagination.py` & `hgitaly-1.4.0/hgitaly/pagination.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/path.py` & `hgitaly-1.4.0/hgitaly/path.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/peer.py` & `hgitaly-1.4.0/hgitaly/peer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/procutil.py` & `hgitaly-1.4.0/hgitaly/procutil.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/repository.py` & `hgitaly-1.4.0/hgitaly/repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/revision.py` & `hgitaly-1.4.0/hgitaly/revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/revset.py` & `hgitaly-1.4.0/hgitaly/revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/server/address.py` & `hgitaly-1.4.0/hgitaly/server/address.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/server/mono.py` & `hgitaly-1.4.0/hgitaly/server/mono.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/server/prefork.py` & `hgitaly-1.4.0/hgitaly/server/prefork.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/server/tests/test_address.py` & `hgitaly-1.4.0/hgitaly/server/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/server/tests/test_mono.py` & `hgitaly-1.4.0/hgitaly/server/tests/test_mono.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/server/tests/test_prefork.py` & `hgitaly-1.4.0/hgitaly/server/tests/test_prefork.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/server/tests/test_worker.py` & `hgitaly-1.4.0/hgitaly/server/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/server/worker.py` & `hgitaly-1.4.0/hgitaly/server/worker.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/blob.py` & `hgitaly-1.4.0/hgitaly/service/blob.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/commit.py` & `hgitaly-1.4.0/hgitaly/service/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     ListFilesResponse,
     FindCommitRequest,
     FindCommitResponse,
     CommitStatsRequest,
     CommitStatsResponse,
     FindAllCommitsRequest,
     FindAllCommitsResponse,
+    FindCommitsError,
     FindCommitsRequest,
     FindCommitsResponse,
     CommitLanguagesRequest,
     CommitLanguagesResponse,
     RawBlameError,
     RawBlameRequest,
     RawBlameResponse,
@@ -580,15 +581,17 @@
             pats = list(map(lambda p: repo.root + b'/' + p, pats))
 
         repo, opts = parse_find_commits_request_opts(request, context, repo)
 
         if request.revision and not opts[b'rev'][0]:
             logger.debug(
                 "Request %r, revision could not be found", req_log)
-            return FindCommitsResponse()
+            structured_abort(
+                context, StatusCode.NOT_FOUND, "commits not found",
+                FindCommitsError())
 
         walk_opts = logcmdutil.parseopts(repo.ui, pats, opts)
         revs, _ = logcmdutil.getrevs(repo, walk_opts)
 
         if request.offset > 0:
             revs = revs.slice(request.offset, len(revs))
 
@@ -596,14 +599,15 @@
             revs = repo.revs(b"sort(%ld, topo)", revs)
             if request.all:
                 revs = repo.revs(b"reverse(%ld)", revs)
 
         # investigation log for heptapod#1365
         if len(revs) == 0:
             logger.info("Empty commit list for walk_opts=%r", walk_opts)
+#            context.abort(StatusCode.NOT_FOUND, "commits not found")
 
         incl_ref_by = request.include_referenced_by
 
         with_short_stats = request.include_shortstat
         for chunk in chunked(revs):
             yield FindCommitsResponse(
                 commits=(message.commit(repo[rev],
@@ -1102,14 +1106,16 @@
 
     :param bytes path: subdir or file
     :param seen_from: changectx
     """
     if not path or path in (b'.', b'/', b'./'):
         # interpeted as a directory, this would be the repository root, which
         # all changesets change.
+        # TODO comment above is wrong, as empty changesets do exist!
+        # The question would be what Gitaly does in this case, if we care.
         return seen_from
 
     if literal_pathspec:
         match = GitLiteralPathSpec(path).match
     else:
         match = GitPathSpec(path).match
```

### Comparing `hgitaly-1.3.3/hgitaly/service/diff.py` & `hgitaly-1.4.0/hgitaly/service/diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/interceptors.py` & `hgitaly-1.4.0/hgitaly/service/interceptors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/mercurial_changeset.py` & `hgitaly-1.4.0/hgitaly/service/mercurial_changeset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/mercurial_operations.py` & `hgitaly-1.4.0/hgitaly/service/mercurial_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from mercurial.merge import merge
 from mercurial.mergestate import mergestate
 from mercurial.node import nullhex as NULL_NODE_HEX
 from mercurial.phases import (
     public as PUBLIC,
 )
+from mercurial import util as hgutil
 
 from heptapod.gitlab.branch import (
     NAMED_BRANCH_PREFIX,
     gitlab_branch_ref,
 )
 
 from .. import message
@@ -65,14 +66,15 @@
 from ..stub.shared_pb2 import (
     User,
 )
 from ..servicer import HGitalyServicer
 
 base_logger = logging.getLogger(__name__)
 
+MERCURIAL_VERSION = hgutil.versiontuple()
 MERGE_CONFLICTS_LABELS = [b'working copy', b'merge rev', b'common ancestor']
 
 
 class ConflictError(RuntimeError):
     """Raised by merge helpers and catched by service method"""
 
 
@@ -189,17 +191,22 @@
             context.abort(StatusCode.INVALID_ARGUMENT,
                           f"Changeset {node_id} not found")
         # it is essential that the censored file is not checked out.
         # normally, the repository should already be at the null revision,
         # but let's be really sure:
         self.repo_command(repo, context, 'update', NULL_NODE_HEX)
 
+        if MERCURIAL_VERSION >= (6, 7):
+            rev_arg = [changeset.rev()]  # hg>=6.7
+        else:
+            rev_arg = changeset.hex()  # hg<6.7
+
         self.repo_command(repo, context, 'censor',
                           b'/'.join((repo.root, request.file_path)),
-                          rev=changeset.hex(),
+                          rev=rev_arg,
                           tombstone=request.tombstone)
         return CensorResponse()
 
     def MergeBranch(self,
                     request: MergeBranchRequest,
                     context) -> MergeBranchResponse:
         logger = LoggerAdapter(base_logger, context)
```

### Comparing `hgitaly-1.3.3/hgitaly/service/mercurial_repository.py` & `hgitaly-1.4.0/hgitaly/service/mercurial_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/operations.py` & `hgitaly-1.4.0/hgitaly/service/operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/ref.py` & `hgitaly-1.4.0/hgitaly/service/ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/repository.py` & `hgitaly-1.4.0/hgitaly/service/repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/server.py` & `hgitaly-1.4.0/hgitaly/service/server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/fixture.py` & `hgitaly-1.4.0/hgitaly/service/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_blob.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_commit.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,20 +354,22 @@
     assert find_commits_ids(revision=b'4...1') == [sha4, sha3, sha2, sha1]
     assert find_commits_ids(revision=b'0..4') == [sha4, sha3, sha2]
     # use default branch if any of the side is omitted
     assert find_commits_ids(revision=b'...1') == [sha4, sha3, sha2, sha1]
     assert find_commits_ids(revision=b'1...') == [sha4, sha3, sha2, sha1]
     assert find_commits_ids(revision=b'0..') == [sha4, sha3, sha2]
     assert find_commits_ids(revision=b'..0') == []
-    # when revision does not exists
-    assert find_commits_ids(revision=b'does_not_exists') == []
-    assert find_commits_ids(revision=b'1234deadbeaf') == []
-    # special node ids
-    assert find_commits_ids(revision=b'ffffffff' * 5) == []
-    assert find_commits_ids(revision=b'ffffffff') == []
+    # when revision does not exists (including special Node IDs)
+    for rev in (b'does_not_exists',
+                b'1234deadbeaf',
+                b'ffffffff' * 5,
+                b'ffffffff'):
+        with pytest.raises(grpc.RpcError) as exc_info:
+            find_commits_ids(revision=rev)
+        assert exc_info.value.code() == grpc.StatusCode.NOT_FOUND
     # with all, return all the commits
     assert find_commits_ids(all=True) == [sha0, sha1, sha2, sha3, sha4]
     # with offset
     assert find_commits_ids(all=True, offset=2) == [sha2, sha3, sha4]
     # with skip_merges
     assert find_commits_ids(skip_merges=True) == [sha3, sha2, sha0]
     # with short stats
```

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_default_branch.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_default_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_diff.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_mercurial_changeset.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_mercurial_changeset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_mercurial_operations.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_mercurial_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_mercurial_repository.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_mercurial_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_operations.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_ref.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_repository_service.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_repository_service.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/service/tests/test_server.py` & `hgitaly-1.4.0/hgitaly/service/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/servicer.py` & `hgitaly-1.4.0/hgitaly/servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/ssh.py` & `hgitaly-1.4.0/hgitaly/ssh.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stream.py` & `hgitaly-1.4.0/hgitaly/stream.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/blob_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/blob_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import lint_pb2 as lint__pb2
 from . import shared_pb2 as shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nblob.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"Z\n\x0eGetBlobRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03oid\x18\x02 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\x03\":\n\x0fGetBlobResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0b\n\x03oid\x18\x03 \x01(\t\"\xbc\x01\n\x0fGetBlobsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12<\n\x0erevision_paths\x18\x02 \x03(\x0b\x32$.gitaly.GetBlobsRequest.RevisionPath\x12\r\n\x05limit\x18\x03 \x01(\x03\x1a.\n\x0cRevisionPath\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\x0c\"\xa1\x01\n\x10GetBlobsResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0b\n\x03oid\x18\x03 \x01(\t\x12\x14\n\x0cis_submodule\x18\x04 \x01(\x08\x12\x0c\n\x04mode\x18\x05 \x01(\x05\x12\x10\n\x08revision\x18\x06 \x01(\t\x12\x0c\n\x04path\x18\x07 \x01(\x0c\x12 \n\x04type\x18\x08 \x01(\x0e\x32\x12.gitaly.ObjectType\"\x8b\x01\n\x10ListBlobsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\t\x12\r\n\x05limit\x18\x03 \x01(\r\x12\x13\n\x0b\x62ytes_limit\x18\x04 \x01(\x03\x12\x12\n\nwith_paths\x18\x05 \x01(\x08\"\x81\x01\n\x11ListBlobsResponse\x12-\n\x05\x62lobs\x18\x01 \x03(\x0b\x32\x1e.gitaly.ListBlobsResponse.Blob\x1a=\n\x04\x42lob\x12\x0b\n\x03oid\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x12\x0c\n\x04path\x18\x04 \x01(\x0c\"g\n\x13ListAllBlobsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05limit\x18\x02 \x01(\r\x12\x13\n\x0b\x62ytes_limit\x18\x03 \x01(\x03\"y\n\x14ListAllBlobsResponse\x12\x30\n\x05\x62lobs\x18\x01 \x03(\x0b\x32!.gitaly.ListAllBlobsResponse.Blob\x1a/\n\x04\x42lob\x12\x0b\n\x03oid\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"5\n\nLFSPointer\x12\x0c\n\x04size\x18\x01 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0b\n\x03oid\x18\x03 \x01(\t\"W\n\x15GetLFSPointersRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08\x62lob_ids\x18\x02 \x03(\t\"B\n\x16GetLFSPointersResponse\x12(\n\x0clfs_pointers\x18\x01 \x03(\x0b\x32\x12.gitaly.LFSPointer\"h\n\x16ListLFSPointersRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\t\x12\r\n\x05limit\x18\x03 \x01(\x05\"C\n\x17ListLFSPointersResponse\x12(\n\x0clfs_pointers\x18\x01 \x03(\x0b\x32\x12.gitaly.LFSPointer\"X\n\x19ListAllLFSPointersRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05limit\x18\x03 \x01(\x05\"F\n\x1aListAllLFSPointersResponse\x12(\n\x0clfs_pointers\x18\x01 \x03(\x0b\x32\x12.gitaly.LFSPointer2\xdd\x04\n\x0b\x42lobService\x12\x44\n\x07GetBlob\x12\x16.gitaly.GetBlobRequest\x1a\x17.gitaly.GetBlobResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12G\n\x08GetBlobs\x12\x17.gitaly.GetBlobsRequest\x1a\x18.gitaly.GetBlobsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tListBlobs\x12\x18.gitaly.ListBlobsRequest\x1a\x19.gitaly.ListBlobsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12S\n\x0cListAllBlobs\x12\x1b.gitaly.ListAllBlobsRequest\x1a\x1c.gitaly.ListAllBlobsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12Y\n\x0eGetLFSPointers\x12\x1d.gitaly.GetLFSPointersRequest\x1a\x1e.gitaly.GetLFSPointersResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\\\n\x0fListLFSPointers\x12\x1e.gitaly.ListLFSPointersRequest\x1a\x1f.gitaly.ListLFSPointersResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x65\n\x12ListAllLFSPointers\x12!.gitaly.ListAllLFSPointersRequest\x1a\".gitaly.ListAllLFSPointersResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nblob.proto\x12\x06gitaly\x1a\nlint.proto\x1a\x0cshared.proto\"Z\n\x0eGetBlobRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x0b\n\x03oid\x18\x02 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\x03\":\n\x0fGetBlobResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0b\n\x03oid\x18\x03 \x01(\t\"\xbc\x01\n\x0fGetBlobsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12<\n\x0erevision_paths\x18\x02 \x03(\x0b\x32$.gitaly.GetBlobsRequest.RevisionPath\x12\r\n\x05limit\x18\x03 \x01(\x03\x1a.\n\x0cRevisionPath\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\x0c\"\xa1\x01\n\x10GetBlobsResponse\x12\x0c\n\x04size\x18\x01 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0b\n\x03oid\x18\x03 \x01(\t\x12\x14\n\x0cis_submodule\x18\x04 \x01(\x08\x12\x0c\n\x04mode\x18\x05 \x01(\x05\x12\x10\n\x08revision\x18\x06 \x01(\t\x12\x0c\n\x04path\x18\x07 \x01(\x0c\x12 \n\x04type\x18\x08 \x01(\x0e\x32\x12.gitaly.ObjectType\"\x8b\x01\n\x10ListBlobsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\t\x12\r\n\x05limit\x18\x03 \x01(\r\x12\x13\n\x0b\x62ytes_limit\x18\x04 \x01(\x03\x12\x12\n\nwith_paths\x18\x05 \x01(\x08\"\x81\x01\n\x11ListBlobsResponse\x12-\n\x05\x62lobs\x18\x01 \x03(\x0b\x32\x1e.gitaly.ListBlobsResponse.Blob\x1a=\n\x04\x42lob\x12\x0b\n\x03oid\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\x12\x0c\n\x04path\x18\x04 \x01(\x0c\"g\n\x13ListAllBlobsRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05limit\x18\x02 \x01(\r\x12\x13\n\x0b\x62ytes_limit\x18\x03 \x01(\x03\"y\n\x14ListAllBlobsResponse\x12\x30\n\x05\x62lobs\x18\x01 \x03(\x0b\x32!.gitaly.ListAllBlobsResponse.Blob\x1a/\n\x04\x42lob\x12\x0b\n\x03oid\x18\x01 \x01(\t\x12\x0c\n\x04size\x18\x02 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"Z\n\nLFSPointer\x12\x0c\n\x04size\x18\x01 \x01(\x03\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x0b\n\x03oid\x18\x03 \x01(\t\x12\x11\n\tfile_size\x18\x04 \x01(\x03\x12\x10\n\x08\x66ile_oid\x18\x05 \x01(\x0c\"W\n\x15GetLFSPointersRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08\x62lob_ids\x18\x02 \x03(\t\"B\n\x16GetLFSPointersResponse\x12(\n\x0clfs_pointers\x18\x01 \x03(\x0b\x32\x12.gitaly.LFSPointer\"h\n\x16ListLFSPointersRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x11\n\trevisions\x18\x02 \x03(\t\x12\r\n\x05limit\x18\x03 \x01(\x05\"C\n\x17ListLFSPointersResponse\x12(\n\x0clfs_pointers\x18\x01 \x03(\x0b\x32\x12.gitaly.LFSPointer\"X\n\x19ListAllLFSPointersRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05limit\x18\x03 \x01(\x05\"F\n\x1aListAllLFSPointersResponse\x12(\n\x0clfs_pointers\x18\x01 \x03(\x0b\x32\x12.gitaly.LFSPointer2\xdd\x04\n\x0b\x42lobService\x12\x44\n\x07GetBlob\x12\x16.gitaly.GetBlobRequest\x1a\x17.gitaly.GetBlobResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12G\n\x08GetBlobs\x12\x17.gitaly.GetBlobsRequest\x1a\x18.gitaly.GetBlobsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12J\n\tListBlobs\x12\x18.gitaly.ListBlobsRequest\x1a\x19.gitaly.ListBlobsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12S\n\x0cListAllBlobs\x12\x1b.gitaly.ListAllBlobsRequest\x1a\x1c.gitaly.ListAllBlobsResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12Y\n\x0eGetLFSPointers\x12\x1d.gitaly.GetLFSPointersRequest\x1a\x1e.gitaly.GetLFSPointersResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\\\n\x0fListLFSPointers\x12\x1e.gitaly.ListLFSPointersRequest\x1a\x1f.gitaly.ListLFSPointersResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x12\x65\n\x12ListAllLFSPointers\x12!.gitaly.ListAllLFSPointersRequest\x1a\".gitaly.ListAllLFSPointersResponse\"\x06\xfa\x97(\x02\x08\x02\x30\x01\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'blob_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -71,23 +71,23 @@
   _globals['_LISTALLBLOBSREQUEST']._serialized_start=829
   _globals['_LISTALLBLOBSREQUEST']._serialized_end=932
   _globals['_LISTALLBLOBSRESPONSE']._serialized_start=934
   _globals['_LISTALLBLOBSRESPONSE']._serialized_end=1055
   _globals['_LISTALLBLOBSRESPONSE_BLOB']._serialized_start=766
   _globals['_LISTALLBLOBSRESPONSE_BLOB']._serialized_end=813
   _globals['_LFSPOINTER']._serialized_start=1057
-  _globals['_LFSPOINTER']._serialized_end=1110
-  _globals['_GETLFSPOINTERSREQUEST']._serialized_start=1112
-  _globals['_GETLFSPOINTERSREQUEST']._serialized_end=1199
-  _globals['_GETLFSPOINTERSRESPONSE']._serialized_start=1201
-  _globals['_GETLFSPOINTERSRESPONSE']._serialized_end=1267
-  _globals['_LISTLFSPOINTERSREQUEST']._serialized_start=1269
-  _globals['_LISTLFSPOINTERSREQUEST']._serialized_end=1373
-  _globals['_LISTLFSPOINTERSRESPONSE']._serialized_start=1375
-  _globals['_LISTLFSPOINTERSRESPONSE']._serialized_end=1442
-  _globals['_LISTALLLFSPOINTERSREQUEST']._serialized_start=1444
-  _globals['_LISTALLLFSPOINTERSREQUEST']._serialized_end=1532
-  _globals['_LISTALLLFSPOINTERSRESPONSE']._serialized_start=1534
-  _globals['_LISTALLLFSPOINTERSRESPONSE']._serialized_end=1604
-  _globals['_BLOBSERVICE']._serialized_start=1607
-  _globals['_BLOBSERVICE']._serialized_end=2212
+  _globals['_LFSPOINTER']._serialized_end=1147
+  _globals['_GETLFSPOINTERSREQUEST']._serialized_start=1149
+  _globals['_GETLFSPOINTERSREQUEST']._serialized_end=1236
+  _globals['_GETLFSPOINTERSRESPONSE']._serialized_start=1238
+  _globals['_GETLFSPOINTERSRESPONSE']._serialized_end=1304
+  _globals['_LISTLFSPOINTERSREQUEST']._serialized_start=1306
+  _globals['_LISTLFSPOINTERSREQUEST']._serialized_end=1410
+  _globals['_LISTLFSPOINTERSRESPONSE']._serialized_start=1412
+  _globals['_LISTLFSPOINTERSRESPONSE']._serialized_end=1479
+  _globals['_LISTALLLFSPOINTERSREQUEST']._serialized_start=1481
+  _globals['_LISTALLLFSPOINTERSREQUEST']._serialized_end=1569
+  _globals['_LISTALLLFSPOINTERSRESPONSE']._serialized_start=1571
+  _globals['_LISTALLLFSPOINTERSRESPONSE']._serialized_end=1641
+  _globals['_BLOBSERVICE']._serialized_start=1644
+  _globals['_BLOBSERVICE']._serialized_end=2249
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hgitaly-1.3.3/hgitaly/stub/blob_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/blob_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/commit_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/commit_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/diff_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/diff_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,14 +47,24 @@
                 response_deserializer=diff__pb2.FindChangedPathsResponse.FromString,
                 )
         self.GetPatchID = channel.unary_unary(
                 '/gitaly.DiffService/GetPatchID',
                 request_serializer=diff__pb2.GetPatchIDRequest.SerializeToString,
                 response_deserializer=diff__pb2.GetPatchIDResponse.FromString,
                 )
+        self.RawRangeDiff = channel.unary_stream(
+                '/gitaly.DiffService/RawRangeDiff',
+                request_serializer=diff__pb2.RawRangeDiffRequest.SerializeToString,
+                response_deserializer=diff__pb2.RawRangeDiffResponse.FromString,
+                )
+        self.RangeDiff = channel.unary_stream(
+                '/gitaly.DiffService/RangeDiff',
+                request_serializer=diff__pb2.RangeDiffRequest.SerializeToString,
+                response_deserializer=diff__pb2.RangeDiffResponse.FromString,
+                )
 
 
 class DiffServiceServicer(object):
     """DiffService is a service which provides RPCs to inspect differences
     introduced between a set of commits.
     """
 
@@ -114,14 +124,28 @@
         whether diffs make the same change. Please refer to git-patch-id(1) for further information.
         If the difference between old and new change is empty then this RPC returns an error.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def RawRangeDiff(self, request, context):
+        """RawRangeDiff outputs the raw range diff data for a given range specification.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def RangeDiff(self, request, context):
+        """RangeDiff outputs the parsed commit pairs from range diff for a given range specification.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DiffServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CommitDiff': grpc.unary_stream_rpc_method_handler(
                     servicer.CommitDiff,
                     request_deserializer=diff__pb2.CommitDiffRequest.FromString,
                     response_serializer=diff__pb2.CommitDiffResponse.SerializeToString,
@@ -152,14 +176,24 @@
                     response_serializer=diff__pb2.FindChangedPathsResponse.SerializeToString,
             ),
             'GetPatchID': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPatchID,
                     request_deserializer=diff__pb2.GetPatchIDRequest.FromString,
                     response_serializer=diff__pb2.GetPatchIDResponse.SerializeToString,
             ),
+            'RawRangeDiff': grpc.unary_stream_rpc_method_handler(
+                    servicer.RawRangeDiff,
+                    request_deserializer=diff__pb2.RawRangeDiffRequest.FromString,
+                    response_serializer=diff__pb2.RawRangeDiffResponse.SerializeToString,
+            ),
+            'RangeDiff': grpc.unary_stream_rpc_method_handler(
+                    servicer.RangeDiff,
+                    request_deserializer=diff__pb2.RangeDiffRequest.FromString,
+                    response_serializer=diff__pb2.RangeDiffResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'gitaly.DiffService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -282,7 +316,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/gitaly.DiffService/GetPatchID',
             diff__pb2.GetPatchIDRequest.SerializeToString,
             diff__pb2.GetPatchIDResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RawRangeDiff(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/gitaly.DiffService/RawRangeDiff',
+            diff__pb2.RawRangeDiffRequest.SerializeToString,
+            diff__pb2.RawRangeDiffResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RangeDiff(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/gitaly.DiffService/RangeDiff',
+            diff__pb2.RangeDiffRequest.SerializeToString,
+            diff__pb2.RangeDiffResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `hgitaly-1.3.3/hgitaly/stub/errors_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/lint_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/lint_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/mercurial_changeset_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/mercurial_changeset_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/mercurial_changeset_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/mercurial_operations_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/mercurial_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/mercurial_operations_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/mercurial_operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/mercurial_repository_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/mercurial_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/mercurial_repository_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/mercurial_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/operations_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/operations_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from . import errors_pb2 as errors__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import lint_pb2 as lint__pb2
 from . import shared_pb2 as shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10operations.proto\x12\x06gitaly\x1a\x0c\x65rrors.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\nlint.proto\x1a\x0cshared.proto\"\x8d\x01\n\x17UserCreateBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x13\n\x0bstart_point\x18\x04 \x01(\x0c\"S\n\x18UserCreateBranchResponse\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.gitaly.BranchJ\x04\x08\x02\x10\x03R\x11pre_receive_error\"P\n\x15UserCreateBranchError\x12.\n\x0b\x63ustom_hook\x18\x01 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\x98\x01\n\x17UserUpdateBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x0e\n\x06newrev\x18\x04 \x01(\x0c\x12\x0e\n\x06oldrev\x18\x05 \x01(\x0c\"5\n\x18UserUpdateBranchResponse\x12\x19\n\x11pre_receive_error\x18\x01 \x01(\t\"\x92\x01\n\x17UserDeleteBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x18\n\x10\x65xpected_old_oid\x18\x04 \x01(\t\"3\n\x18UserDeleteBranchResponseJ\x04\x08\x01\x10\x02R\x11pre_receive_error\"\xbc\x01\n\x15UserDeleteBranchError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\x8c\x01\n\x14UserDeleteTagRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08tag_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x18\n\x10\x65xpected_old_oid\x18\x04 \x01(\t\"2\n\x15UserDeleteTagResponse\x12\x19\n\x11pre_receive_error\x18\x01 \x01(\t\"\xcb\x01\n\x14UserCreateTagRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08tag_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x17\n\x0ftarget_revision\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"X\n\x15UserCreateTagResponse\x12\x18\n\x03tag\x18\x01 \x01(\x0b\x32\x0b.gitaly.TagJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x06\x65xistsR\x11pre_receive_error\"\xf3\x01\n\x12UserCreateTagError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x38\n\x10reference_exists\x18\x04 \x01(\x0b\x32\x1c.gitaly.ReferenceExistsErrorH\x00\x42\x07\n\x05\x65rror\"\xee\x01\n\x16UserMergeBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tcommit_id\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x08 \x01(\t\x12\r\n\x05\x61pply\x18\x06 \x01(\x08\"\x81\x01\n\x17UserMergeBranchResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x34\n\rbranch_update\x18\x03 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdateJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x11pre_receive_error\"\xf1\x01\n\x14UserMergeBranchError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x34\n\x0emerge_conflict\x18\x04 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x42\x07\n\x05\x65rror\"\xae\x02\n\x15UserMergeToRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\nsource_sha\x18\x03 \x01(\t\x12\x12\n\x06\x62ranch\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\x12\n\ntarget_ref\x18\x05 \x01(\x0c\x12\x0f\n\x07message\x18\x06 \x01(\x0c\x12\x18\n\x10\x66irst_parent_ref\x18\x07 \x01(\x0c\x12\x1b\n\x0f\x61llow_conflicts\x18\x08 \x01(\x08\x42\x02\x18\x01\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"D\n\x16UserMergeToRefResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03R\x11pre_receive_error\"\xed\x01\n\x16UserRebaseToRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\nsource_sha\x18\x03 \x01(\t\x12\x12\n\ntarget_ref\x18\x05 \x01(\x0c\x12\x18\n\x10\x66irst_parent_ref\x18\x07 \x01(\x0c\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\",\n\x17UserRebaseToRefResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\"X\n\x15OperationBranchUpdate\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x14\n\x0crepo_created\x18\x02 \x01(\x08\x12\x16\n\x0e\x62ranch_created\x18\x03 \x01(\x08\"\x9c\x01\n\x13UserFFBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tcommit_id\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x18\n\x10\x65xpected_old_oid\x18\x05 \x01(\t\"g\n\x14UserFFBranchResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11pre_receive_error\x18\x02 \x01(\t\"\xcd\x02\n\x15UserCherryPickRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12!\n\x06\x63ommit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x06 \x01(\x0c\x12,\n\x10start_repository\x18\x07 \x01(\x0b\x32\x12.gitaly.Repository\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"\xb2\x01\n\x16UserCherryPickResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdateJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06R\x11\x63reate_tree_errorR\x0c\x63ommit_errorR\x11pre_receive_errorR\x16\x63reate_tree_error_code\"\x8f\x02\n\x13UserCherryPickError\x12:\n\x14\x63herry_pick_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12:\n\x16target_branch_diverged\x18\x02 \x01(\x0b\x32\x18.gitaly.NotAncestorErrorH\x00\x12\x45\n\x17\x63hanges_already_applied\x18\x03 \x01(\x0b\x32\".gitaly.ChangesAlreadyAppliedErrorH\x00\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x04 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x42\x07\n\x05\x65rror\"\xc9\x02\n\x11UserRevertRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12!\n\x06\x63ommit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x06 \x01(\x0c\x12,\n\x10start_repository\x18\x07 \x01(\x0b\x32\x12.gitaly.Repository\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"\x98\x02\n\x12UserRevertResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11\x63reate_tree_error\x18\x02 \x01(\t\x12\x14\n\x0c\x63ommit_error\x18\x03 \x01(\t\x12\x19\n\x11pre_receive_error\x18\x04 \x01(\t\x12J\n\x16\x63reate_tree_error_code\x18\x05 \x01(\x0e\x32*.gitaly.UserRevertResponse.CreateTreeError\"4\n\x0f\x43reateTreeError\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05\x45MPTY\x10\x01\x12\x0c\n\x08\x43ONFLICT\x10\x02\"\xa7\x02\n\x1bUserCommitFilesActionHeader\x12>\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32..gitaly.UserCommitFilesActionHeader.ActionType\x12\x11\n\tfile_path\x18\x02 \x01(\x0c\x12\x15\n\rprevious_path\x18\x03 \x01(\x0c\x12\x16\n\x0e\x62\x61se64_content\x18\x04 \x01(\x08\x12\x18\n\x10\x65xecute_filemode\x18\x05 \x01(\x08\x12\x15\n\rinfer_content\x18\x06 \x01(\x08\"U\n\nActionType\x12\n\n\x06\x43REATE\x10\x00\x12\x0e\n\nCREATE_DIR\x10\x01\x12\n\n\x06UPDATE\x10\x02\x12\x08\n\x04MOVE\x10\x03\x12\n\n\x06\x44\x45LETE\x10\x04\x12\t\n\x05\x43HMOD\x10\x05\"\x85\x01\n\x15UserCommitFilesAction\x12\x35\n\x06header\x18\x01 \x01(\x0b\x32#.gitaly.UserCommitFilesActionHeaderH\x00\x12\x11\n\x07\x63ontent\x18\x02 \x01(\x0cH\x00\x42\"\n user_commit_files_action_payload\"\x82\x03\n\x1cUserCommitFilesRequestHeader\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x13\n\x0b\x62ranch_name\x18\x03 \x01(\x0c\x12\x16\n\x0e\x63ommit_message\x18\x04 \x01(\x0c\x12\x1a\n\x12\x63ommit_author_name\x18\x05 \x01(\x0c\x12\x1b\n\x13\x63ommit_author_email\x18\x06 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x07 \x01(\x0c\x12,\n\x10start_repository\x18\x08 \x01(\x0b\x32\x12.gitaly.Repository\x12\r\n\x05\x66orce\x18\t \x01(\x08\x12\x11\n\tstart_sha\x18\n \x01(\t\x12-\n\ttimestamp\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x0c \x01(\t\"\xa6\x01\n\x16UserCommitFilesRequest\x12\x36\n\x06header\x18\x01 \x01(\x0b\x32$.gitaly.UserCommitFilesRequestHeaderH\x00\x12/\n\x06\x61\x63tion\x18\x02 \x01(\x0b\x32\x1d.gitaly.UserCommitFilesActionH\x00\x42#\n!user_commit_files_request_payload\"\x7f\n\x17UserCommitFilesResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x13\n\x0bindex_error\x18\x02 \x01(\t\x12\x19\n\x11pre_receive_error\x18\x03 \x01(\t\"\xad\x01\n\x14UserCommitFilesError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12*\n\x0cindex_update\x18\x02 \x01(\x0b\x32\x12.gitaly.IndexErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\xb8\x03\n\x1cUserRebaseConfirmableRequest\x12=\n\x06header\x18\x01 \x01(\x0b\x32+.gitaly.UserRebaseConfirmableRequest.HeaderH\x00\x12\x0f\n\x05\x61pply\x18\x02 \x01(\x08H\x00\x1a\x9c\x02\n\x06Header\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x15\n\trebase_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x12\n\nbranch_sha\x18\x05 \x01(\t\x12-\n\x11remote_repository\x18\x06 \x01(\x0b\x32\x12.gitaly.Repository\x12\x15\n\rremote_branch\x18\x07 \x01(\x0c\x12\x18\n\x10git_push_options\x18\x08 \x03(\t\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB)\n\'user_rebase_confirmable_request_payload\"\xa5\x01\n\x1dUserRebaseConfirmableResponse\x12\x14\n\nrebase_sha\x18\x01 \x01(\tH\x00\x12\x18\n\x0erebase_applied\x18\x02 \x01(\x08H\x00\x42*\n(user_rebase_confirmable_response_payloadJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05R\x11pre_receive_errorR\tgit_error\"\xfd\x01\n\x11UserSquashRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tstart_sha\x18\x05 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x06 \x01(\t\x12\x1c\n\x06\x61uthor\x18\x07 \x01(\x0b\x32\x0c.gitaly.User\x12\x16\n\x0e\x63ommit_message\x18\x08 \x01(\x0c\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05R\tsquash_id\"R\n\x12UserSquashResponse\x12\x12\n\nsquash_sha\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x11pre_receive_errorR\tgit_error\"\x8e\x01\n\x1aUserRebaseConfirmableError\x12\x35\n\x0frebase_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x02 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x42\x07\n\x05\x65rror\"\x8b\x01\n\x0fUserSquashError\x12\x38\n\x10resolve_revision\x18\x01 \x01(\x0b\x32\x1c.gitaly.ResolveRevisionErrorH\x00\x12\x35\n\x0frebase_conflict\x18\x02 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x42\x07\n\x05\x65rror\"\xbb\x02\n\x15UserApplyPatchRequest\x12\x36\n\x06header\x18\x01 \x01(\x0b\x32$.gitaly.UserApplyPatchRequest.HeaderH\x00\x12\x11\n\x07patches\x18\x02 \x01(\x0cH\x00\x1a\xb2\x01\n\x06Header\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x15\n\rtarget_branch\x18\x03 \x01(\x0c\x12-\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x05 \x01(\tB\"\n user_apply_patch_request_payload\"N\n\x16UserApplyPatchResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\"\xfe\x01\n\x1aUserUpdateSubmoduleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\ncommit_sha\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x11\n\tsubmodule\x18\x05 \x01(\x0c\x12\x16\n\x0e\x63ommit_message\x18\x06 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x08 \x01(\t\"\x9d\x01\n\x1bUserUpdateSubmoduleResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11pre_receive_error\x18\x02 \x01(\t\x12\x14\n\x0c\x63ommit_error\x18\x04 \x01(\tJ\x04\x08\x03\x10\x04R\x11\x63reate_tree_error2\xc9\x0b\n\x10OperationService\x12]\n\x10UserCreateBranch\x12\x1f.gitaly.UserCreateBranchRequest\x1a .gitaly.UserCreateBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10UserUpdateBranch\x12\x1f.gitaly.UserUpdateBranchRequest\x1a .gitaly.UserUpdateBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10UserDeleteBranch\x12\x1f.gitaly.UserDeleteBranchRequest\x1a .gitaly.UserDeleteBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rUserCreateTag\x12\x1c.gitaly.UserCreateTagRequest\x1a\x1d.gitaly.UserCreateTagResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rUserDeleteTag\x12\x1c.gitaly.UserDeleteTagRequest\x1a\x1d.gitaly.UserDeleteTagResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eUserMergeToRef\x12\x1d.gitaly.UserMergeToRefRequest\x1a\x1e.gitaly.UserMergeToRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12Z\n\x0fUserRebaseToRef\x12\x1e.gitaly.UserRebaseToRefRequest\x1a\x1f.gitaly.UserRebaseToRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12^\n\x0fUserMergeBranch\x12\x1e.gitaly.UserMergeBranchRequest\x1a\x1f.gitaly.UserMergeBranchResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x30\x01\x12Q\n\x0cUserFFBranch\x12\x1b.gitaly.UserFFBranchRequest\x1a\x1c.gitaly.UserFFBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eUserCherryPick\x12\x1d.gitaly.UserCherryPickRequest\x1a\x1e.gitaly.UserCherryPickResponse\"\x06\xfa\x97(\x02\x08\x01\x12\\\n\x0fUserCommitFiles\x12\x1e.gitaly.UserCommitFilesRequest\x1a\x1f.gitaly.UserCommitFilesResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12p\n\x15UserRebaseConfirmable\x12$.gitaly.UserRebaseConfirmableRequest\x1a%.gitaly.UserRebaseConfirmableResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x30\x01\x12K\n\nUserRevert\x12\x19.gitaly.UserRevertRequest\x1a\x1a.gitaly.UserRevertResponse\"\x06\xfa\x97(\x02\x08\x01\x12K\n\nUserSquash\x12\x19.gitaly.UserSquashRequest\x1a\x1a.gitaly.UserSquashResponse\"\x06\xfa\x97(\x02\x08\x01\x12Y\n\x0eUserApplyPatch\x12\x1d.gitaly.UserApplyPatchRequest\x1a\x1e.gitaly.UserApplyPatchResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12\x66\n\x13UserUpdateSubmodule\x12\".gitaly.UserUpdateSubmoduleRequest\x1a#.gitaly.UserUpdateSubmoduleResponse\"\x06\xfa\x97(\x02\x08\x01\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10operations.proto\x12\x06gitaly\x1a\x0c\x65rrors.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\nlint.proto\x1a\x0cshared.proto\"\x8d\x01\n\x17UserCreateBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x13\n\x0bstart_point\x18\x04 \x01(\x0c\"S\n\x18UserCreateBranchResponse\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.gitaly.BranchJ\x04\x08\x02\x10\x03R\x11pre_receive_error\"P\n\x15UserCreateBranchError\x12.\n\x0b\x63ustom_hook\x18\x01 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\x98\x01\n\x17UserUpdateBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x0e\n\x06newrev\x18\x04 \x01(\x0c\x12\x0e\n\x06oldrev\x18\x05 \x01(\x0c\"5\n\x18UserUpdateBranchResponse\x12\x19\n\x11pre_receive_error\x18\x01 \x01(\t\"\x92\x01\n\x17UserDeleteBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x18\n\x10\x65xpected_old_oid\x18\x04 \x01(\t\"3\n\x18UserDeleteBranchResponseJ\x04\x08\x01\x10\x02R\x11pre_receive_error\"\xbc\x01\n\x15UserDeleteBranchError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\x8c\x01\n\x14UserDeleteTagRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08tag_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x18\n\x10\x65xpected_old_oid\x18\x04 \x01(\t\"2\n\x15UserDeleteTagResponse\x12\x19\n\x11pre_receive_error\x18\x01 \x01(\t\"\xcb\x01\n\x14UserCreateTagRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x10\n\x08tag_name\x18\x02 \x01(\x0c\x12\x1a\n\x04user\x18\x03 \x01(\x0b\x32\x0c.gitaly.User\x12\x17\n\x0ftarget_revision\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"X\n\x15UserCreateTagResponse\x12\x18\n\x03tag\x18\x01 \x01(\x0b\x32\x0b.gitaly.TagJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x06\x65xistsR\x11pre_receive_error\"\xf3\x01\n\x12UserCreateTagError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x38\n\x10reference_exists\x18\x04 \x01(\x0b\x32\x1c.gitaly.ReferenceExistsErrorH\x00\x42\x07\n\x05\x65rror\"\xee\x01\n\x16UserMergeBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tcommit_id\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x08 \x01(\t\x12\r\n\x05\x61pply\x18\x06 \x01(\x08\"\x81\x01\n\x17UserMergeBranchResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x34\n\rbranch_update\x18\x03 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdateJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05R\x11pre_receive_error\"\xf1\x01\n\x14UserMergeBranchError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12\x38\n\x10reference_update\x18\x02 \x01(\x0b\x32\x1c.gitaly.ReferenceUpdateErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x34\n\x0emerge_conflict\x18\x04 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x42\x07\n\x05\x65rror\"\xae\x02\n\x15UserMergeToRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\nsource_sha\x18\x03 \x01(\t\x12\x12\n\x06\x62ranch\x18\x04 \x01(\x0c\x42\x02\x18\x01\x12\x12\n\ntarget_ref\x18\x05 \x01(\x0c\x12\x0f\n\x07message\x18\x06 \x01(\x0c\x12\x18\n\x10\x66irst_parent_ref\x18\x07 \x01(\x0c\x12\x1b\n\x0f\x61llow_conflicts\x18\x08 \x01(\x08\x42\x02\x18\x01\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"D\n\x16UserMergeToRefResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03R\x11pre_receive_error\"\xed\x01\n\x16UserRebaseToRefRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\nsource_sha\x18\x03 \x01(\t\x12\x12\n\ntarget_ref\x18\x05 \x01(\x0c\x12\x18\n\x10\x66irst_parent_ref\x18\x07 \x01(\x0c\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\",\n\x17UserRebaseToRefResponse\x12\x11\n\tcommit_id\x18\x01 \x01(\t\"X\n\x15OperationBranchUpdate\x12\x11\n\tcommit_id\x18\x01 \x01(\t\x12\x14\n\x0crepo_created\x18\x02 \x01(\x08\x12\x16\n\x0e\x62ranch_created\x18\x03 \x01(\x08\"\x9c\x01\n\x13UserFFBranchRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tcommit_id\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x18\n\x10\x65xpected_old_oid\x18\x05 \x01(\t\"g\n\x14UserFFBranchResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11pre_receive_error\x18\x02 \x01(\t\"\x86\x03\n\x15UserCherryPickRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12!\n\x06\x63ommit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x06 \x01(\x0c\x12,\n\x10start_repository\x18\x07 \x01(\x0b\x32\x12.gitaly.Repository\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\x12\x1a\n\x12\x63ommit_author_name\x18\x0b \x01(\x0c\x12\x1b\n\x13\x63ommit_author_email\x18\x0c \x01(\x0c\"\xb2\x01\n\x16UserCherryPickResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdateJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06R\x11\x63reate_tree_errorR\x0c\x63ommit_errorR\x11pre_receive_errorR\x16\x63reate_tree_error_code\"\x8f\x02\n\x13UserCherryPickError\x12:\n\x14\x63herry_pick_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12:\n\x16target_branch_diverged\x18\x02 \x01(\x0b\x32\x18.gitaly.NotAncestorErrorH\x00\x12\x45\n\x17\x63hanges_already_applied\x18\x03 \x01(\x0b\x32\".gitaly.ChangesAlreadyAppliedErrorH\x00\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x04 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x42\x07\n\x05\x65rror\"\xc9\x02\n\x11UserRevertRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12!\n\x06\x63ommit\x18\x03 \x01(\x0b\x32\x11.gitaly.GitCommit\x12\x13\n\x0b\x62ranch_name\x18\x04 \x01(\x0c\x12\x0f\n\x07message\x18\x05 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x06 \x01(\x0c\x12,\n\x10start_repository\x18\x07 \x01(\x0b\x32\x12.gitaly.Repository\x12\x0f\n\x07\x64ry_run\x18\x08 \x01(\x08\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\n \x01(\t\"\x98\x02\n\x12UserRevertResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11\x63reate_tree_error\x18\x02 \x01(\t\x12\x14\n\x0c\x63ommit_error\x18\x03 \x01(\t\x12\x19\n\x11pre_receive_error\x18\x04 \x01(\t\x12J\n\x16\x63reate_tree_error_code\x18\x05 \x01(\x0e\x32*.gitaly.UserRevertResponse.CreateTreeError\"4\n\x0f\x43reateTreeError\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05\x45MPTY\x10\x01\x12\x0c\n\x08\x43ONFLICT\x10\x02\"\xf9\x01\n\x0fUserRevertError\x12\x34\n\x0emerge_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12\x45\n\x17\x63hanges_already_applied\x18\x02 \x01(\x0b\x32\".gitaly.ChangesAlreadyAppliedErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x12\x30\n\x0cnot_ancestor\x18\x04 \x01(\x0b\x32\x18.gitaly.NotAncestorErrorH\x00\x42\x07\n\x05\x65rror\"\xa7\x02\n\x1bUserCommitFilesActionHeader\x12>\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32..gitaly.UserCommitFilesActionHeader.ActionType\x12\x11\n\tfile_path\x18\x02 \x01(\x0c\x12\x15\n\rprevious_path\x18\x03 \x01(\x0c\x12\x16\n\x0e\x62\x61se64_content\x18\x04 \x01(\x08\x12\x18\n\x10\x65xecute_filemode\x18\x05 \x01(\x08\x12\x15\n\rinfer_content\x18\x06 \x01(\x08\"U\n\nActionType\x12\n\n\x06\x43REATE\x10\x00\x12\x0e\n\nCREATE_DIR\x10\x01\x12\n\n\x06UPDATE\x10\x02\x12\x08\n\x04MOVE\x10\x03\x12\n\n\x06\x44\x45LETE\x10\x04\x12\t\n\x05\x43HMOD\x10\x05\"\x85\x01\n\x15UserCommitFilesAction\x12\x35\n\x06header\x18\x01 \x01(\x0b\x32#.gitaly.UserCommitFilesActionHeaderH\x00\x12\x11\n\x07\x63ontent\x18\x02 \x01(\x0cH\x00\x42\"\n user_commit_files_action_payload\"\x82\x03\n\x1cUserCommitFilesRequestHeader\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x13\n\x0b\x62ranch_name\x18\x03 \x01(\x0c\x12\x16\n\x0e\x63ommit_message\x18\x04 \x01(\x0c\x12\x1a\n\x12\x63ommit_author_name\x18\x05 \x01(\x0c\x12\x1b\n\x13\x63ommit_author_email\x18\x06 \x01(\x0c\x12\x19\n\x11start_branch_name\x18\x07 \x01(\x0c\x12,\n\x10start_repository\x18\x08 \x01(\x0b\x32\x12.gitaly.Repository\x12\r\n\x05\x66orce\x18\t \x01(\x08\x12\x11\n\tstart_sha\x18\n \x01(\t\x12-\n\ttimestamp\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x0c \x01(\t\"\xa6\x01\n\x16UserCommitFilesRequest\x12\x36\n\x06header\x18\x01 \x01(\x0b\x32$.gitaly.UserCommitFilesRequestHeaderH\x00\x12/\n\x06\x61\x63tion\x18\x02 \x01(\x0b\x32\x1d.gitaly.UserCommitFilesActionH\x00\x42#\n!user_commit_files_request_payload\"\x7f\n\x17UserCommitFilesResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x13\n\x0bindex_error\x18\x02 \x01(\t\x12\x19\n\x11pre_receive_error\x18\x03 \x01(\t\"\xad\x01\n\x14UserCommitFilesError\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x01 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x12*\n\x0cindex_update\x18\x02 \x01(\x0b\x32\x12.gitaly.IndexErrorH\x00\x12.\n\x0b\x63ustom_hook\x18\x03 \x01(\x0b\x32\x17.gitaly.CustomHookErrorH\x00\x42\x07\n\x05\x65rror\"\xb8\x03\n\x1cUserRebaseConfirmableRequest\x12=\n\x06header\x18\x01 \x01(\x0b\x32+.gitaly.UserRebaseConfirmableRequest.HeaderH\x00\x12\x0f\n\x05\x61pply\x18\x02 \x01(\x08H\x00\x1a\x9c\x02\n\x06Header\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x15\n\trebase_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x12\n\nbranch_sha\x18\x05 \x01(\t\x12-\n\x11remote_repository\x18\x06 \x01(\x0b\x32\x12.gitaly.Repository\x12\x15\n\rremote_branch\x18\x07 \x01(\x0c\x12\x18\n\x10git_push_options\x18\x08 \x03(\t\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampB)\n\'user_rebase_confirmable_request_payload\"\xa5\x01\n\x1dUserRebaseConfirmableResponse\x12\x14\n\nrebase_sha\x18\x01 \x01(\tH\x00\x12\x18\n\x0erebase_applied\x18\x02 \x01(\x08H\x00\x42*\n(user_rebase_confirmable_response_payloadJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05R\x11pre_receive_errorR\tgit_error\"\xfd\x01\n\x11UserSquashRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x11\n\tstart_sha\x18\x05 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x06 \x01(\t\x12\x1c\n\x06\x61uthor\x18\x07 \x01(\x0b\x32\x0c.gitaly.User\x12\x16\n\x0e\x63ommit_message\x18\x08 \x01(\x0c\x12-\n\ttimestamp\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05R\tsquash_id\"R\n\x12UserSquashResponse\x12\x12\n\nsquash_sha\x18\x01 \x01(\tJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x11pre_receive_errorR\tgit_error\"\x8e\x01\n\x1aUserRebaseConfirmableError\x12\x35\n\x0frebase_conflict\x18\x01 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x12\x30\n\x0c\x61\x63\x63\x65ss_check\x18\x02 \x01(\x0b\x32\x18.gitaly.AccessCheckErrorH\x00\x42\x07\n\x05\x65rror\"\x8b\x01\n\x0fUserSquashError\x12\x38\n\x10resolve_revision\x18\x01 \x01(\x0b\x32\x1c.gitaly.ResolveRevisionErrorH\x00\x12\x35\n\x0frebase_conflict\x18\x02 \x01(\x0b\x32\x1a.gitaly.MergeConflictErrorH\x00\x42\x07\n\x05\x65rror\"\xbb\x02\n\x15UserApplyPatchRequest\x12\x36\n\x06header\x18\x01 \x01(\x0b\x32$.gitaly.UserApplyPatchRequest.HeaderH\x00\x12\x11\n\x07patches\x18\x02 \x01(\x0cH\x00\x1a\xb2\x01\n\x06Header\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x15\n\rtarget_branch\x18\x03 \x01(\x0c\x12-\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x05 \x01(\tB\"\n user_apply_patch_request_payload\"N\n\x16UserApplyPatchResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\"\xfe\x01\n\x1aUserUpdateSubmoduleRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x1a\n\x04user\x18\x02 \x01(\x0b\x32\x0c.gitaly.User\x12\x12\n\ncommit_sha\x18\x03 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x04 \x01(\x0c\x12\x11\n\tsubmodule\x18\x05 \x01(\x0c\x12\x16\n\x0e\x63ommit_message\x18\x06 \x01(\x0c\x12-\n\ttimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x65xpected_old_oid\x18\x08 \x01(\t\"\x9d\x01\n\x1bUserUpdateSubmoduleResponse\x12\x34\n\rbranch_update\x18\x01 \x01(\x0b\x32\x1d.gitaly.OperationBranchUpdate\x12\x19\n\x11pre_receive_error\x18\x02 \x01(\t\x12\x14\n\x0c\x63ommit_error\x18\x04 \x01(\tJ\x04\x08\x03\x10\x04R\x11\x63reate_tree_error2\xc9\x0b\n\x10OperationService\x12]\n\x10UserCreateBranch\x12\x1f.gitaly.UserCreateBranchRequest\x1a .gitaly.UserCreateBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10UserUpdateBranch\x12\x1f.gitaly.UserUpdateBranchRequest\x1a .gitaly.UserUpdateBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12]\n\x10UserDeleteBranch\x12\x1f.gitaly.UserDeleteBranchRequest\x1a .gitaly.UserDeleteBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rUserCreateTag\x12\x1c.gitaly.UserCreateTagRequest\x1a\x1d.gitaly.UserCreateTagResponse\"\x06\xfa\x97(\x02\x08\x01\x12T\n\rUserDeleteTag\x12\x1c.gitaly.UserDeleteTagRequest\x1a\x1d.gitaly.UserDeleteTagResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eUserMergeToRef\x12\x1d.gitaly.UserMergeToRefRequest\x1a\x1e.gitaly.UserMergeToRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12Z\n\x0fUserRebaseToRef\x12\x1e.gitaly.UserRebaseToRefRequest\x1a\x1f.gitaly.UserRebaseToRefResponse\"\x06\xfa\x97(\x02\x08\x01\x12^\n\x0fUserMergeBranch\x12\x1e.gitaly.UserMergeBranchRequest\x1a\x1f.gitaly.UserMergeBranchResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x30\x01\x12Q\n\x0cUserFFBranch\x12\x1b.gitaly.UserFFBranchRequest\x1a\x1c.gitaly.UserFFBranchResponse\"\x06\xfa\x97(\x02\x08\x01\x12W\n\x0eUserCherryPick\x12\x1d.gitaly.UserCherryPickRequest\x1a\x1e.gitaly.UserCherryPickResponse\"\x06\xfa\x97(\x02\x08\x01\x12\\\n\x0fUserCommitFiles\x12\x1e.gitaly.UserCommitFilesRequest\x1a\x1f.gitaly.UserCommitFilesResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12p\n\x15UserRebaseConfirmable\x12$.gitaly.UserRebaseConfirmableRequest\x1a%.gitaly.UserRebaseConfirmableResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x30\x01\x12K\n\nUserRevert\x12\x19.gitaly.UserRevertRequest\x1a\x1a.gitaly.UserRevertResponse\"\x06\xfa\x97(\x02\x08\x01\x12K\n\nUserSquash\x12\x19.gitaly.UserSquashRequest\x1a\x1a.gitaly.UserSquashResponse\"\x06\xfa\x97(\x02\x08\x01\x12Y\n\x0eUserApplyPatch\x12\x1d.gitaly.UserApplyPatchRequest\x1a\x1e.gitaly.UserApplyPatchResponse\"\x06\xfa\x97(\x02\x08\x01(\x01\x12\x66\n\x13UserUpdateSubmodule\x12\".gitaly.UserUpdateSubmoduleRequest\x1a#.gitaly.UserUpdateSubmoduleResponse\"\x06\xfa\x97(\x02\x08\x01\x42\x34Z2gitlab.com/gitlab-org/gitaly/v16/proto/go/gitalypbb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'operations_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -139,59 +139,61 @@
   _globals['_OPERATIONBRANCHUPDATE']._serialized_start=3030
   _globals['_OPERATIONBRANCHUPDATE']._serialized_end=3118
   _globals['_USERFFBRANCHREQUEST']._serialized_start=3121
   _globals['_USERFFBRANCHREQUEST']._serialized_end=3277
   _globals['_USERFFBRANCHRESPONSE']._serialized_start=3279
   _globals['_USERFFBRANCHRESPONSE']._serialized_end=3382
   _globals['_USERCHERRYPICKREQUEST']._serialized_start=3385
-  _globals['_USERCHERRYPICKREQUEST']._serialized_end=3718
-  _globals['_USERCHERRYPICKRESPONSE']._serialized_start=3721
-  _globals['_USERCHERRYPICKRESPONSE']._serialized_end=3899
-  _globals['_USERCHERRYPICKERROR']._serialized_start=3902
-  _globals['_USERCHERRYPICKERROR']._serialized_end=4173
-  _globals['_USERREVERTREQUEST']._serialized_start=4176
-  _globals['_USERREVERTREQUEST']._serialized_end=4505
-  _globals['_USERREVERTRESPONSE']._serialized_start=4508
-  _globals['_USERREVERTRESPONSE']._serialized_end=4788
-  _globals['_USERREVERTRESPONSE_CREATETREEERROR']._serialized_start=4736
-  _globals['_USERREVERTRESPONSE_CREATETREEERROR']._serialized_end=4788
-  _globals['_USERCOMMITFILESACTIONHEADER']._serialized_start=4791
-  _globals['_USERCOMMITFILESACTIONHEADER']._serialized_end=5086
-  _globals['_USERCOMMITFILESACTIONHEADER_ACTIONTYPE']._serialized_start=5001
-  _globals['_USERCOMMITFILESACTIONHEADER_ACTIONTYPE']._serialized_end=5086
-  _globals['_USERCOMMITFILESACTION']._serialized_start=5089
-  _globals['_USERCOMMITFILESACTION']._serialized_end=5222
-  _globals['_USERCOMMITFILESREQUESTHEADER']._serialized_start=5225
-  _globals['_USERCOMMITFILESREQUESTHEADER']._serialized_end=5611
-  _globals['_USERCOMMITFILESREQUEST']._serialized_start=5614
-  _globals['_USERCOMMITFILESREQUEST']._serialized_end=5780
-  _globals['_USERCOMMITFILESRESPONSE']._serialized_start=5782
-  _globals['_USERCOMMITFILESRESPONSE']._serialized_end=5909
-  _globals['_USERCOMMITFILESERROR']._serialized_start=5912
-  _globals['_USERCOMMITFILESERROR']._serialized_end=6085
-  _globals['_USERREBASECONFIRMABLEREQUEST']._serialized_start=6088
-  _globals['_USERREBASECONFIRMABLEREQUEST']._serialized_end=6528
-  _globals['_USERREBASECONFIRMABLEREQUEST_HEADER']._serialized_start=6201
-  _globals['_USERREBASECONFIRMABLEREQUEST_HEADER']._serialized_end=6485
-  _globals['_USERREBASECONFIRMABLERESPONSE']._serialized_start=6531
-  _globals['_USERREBASECONFIRMABLERESPONSE']._serialized_end=6696
-  _globals['_USERSQUASHREQUEST']._serialized_start=6699
-  _globals['_USERSQUASHREQUEST']._serialized_end=6952
-  _globals['_USERSQUASHRESPONSE']._serialized_start=6954
-  _globals['_USERSQUASHRESPONSE']._serialized_end=7036
-  _globals['_USERREBASECONFIRMABLEERROR']._serialized_start=7039
-  _globals['_USERREBASECONFIRMABLEERROR']._serialized_end=7181
-  _globals['_USERSQUASHERROR']._serialized_start=7184
-  _globals['_USERSQUASHERROR']._serialized_end=7323
-  _globals['_USERAPPLYPATCHREQUEST']._serialized_start=7326
-  _globals['_USERAPPLYPATCHREQUEST']._serialized_end=7641
-  _globals['_USERAPPLYPATCHREQUEST_HEADER']._serialized_start=7427
-  _globals['_USERAPPLYPATCHREQUEST_HEADER']._serialized_end=7605
-  _globals['_USERAPPLYPATCHRESPONSE']._serialized_start=7643
-  _globals['_USERAPPLYPATCHRESPONSE']._serialized_end=7721
-  _globals['_USERUPDATESUBMODULEREQUEST']._serialized_start=7724
-  _globals['_USERUPDATESUBMODULEREQUEST']._serialized_end=7978
-  _globals['_USERUPDATESUBMODULERESPONSE']._serialized_start=7981
-  _globals['_USERUPDATESUBMODULERESPONSE']._serialized_end=8138
-  _globals['_OPERATIONSERVICE']._serialized_start=8141
-  _globals['_OPERATIONSERVICE']._serialized_end=9622
+  _globals['_USERCHERRYPICKREQUEST']._serialized_end=3775
+  _globals['_USERCHERRYPICKRESPONSE']._serialized_start=3778
+  _globals['_USERCHERRYPICKRESPONSE']._serialized_end=3956
+  _globals['_USERCHERRYPICKERROR']._serialized_start=3959
+  _globals['_USERCHERRYPICKERROR']._serialized_end=4230
+  _globals['_USERREVERTREQUEST']._serialized_start=4233
+  _globals['_USERREVERTREQUEST']._serialized_end=4562
+  _globals['_USERREVERTRESPONSE']._serialized_start=4565
+  _globals['_USERREVERTRESPONSE']._serialized_end=4845
+  _globals['_USERREVERTRESPONSE_CREATETREEERROR']._serialized_start=4793
+  _globals['_USERREVERTRESPONSE_CREATETREEERROR']._serialized_end=4845
+  _globals['_USERREVERTERROR']._serialized_start=4848
+  _globals['_USERREVERTERROR']._serialized_end=5097
+  _globals['_USERCOMMITFILESACTIONHEADER']._serialized_start=5100
+  _globals['_USERCOMMITFILESACTIONHEADER']._serialized_end=5395
+  _globals['_USERCOMMITFILESACTIONHEADER_ACTIONTYPE']._serialized_start=5310
+  _globals['_USERCOMMITFILESACTIONHEADER_ACTIONTYPE']._serialized_end=5395
+  _globals['_USERCOMMITFILESACTION']._serialized_start=5398
+  _globals['_USERCOMMITFILESACTION']._serialized_end=5531
+  _globals['_USERCOMMITFILESREQUESTHEADER']._serialized_start=5534
+  _globals['_USERCOMMITFILESREQUESTHEADER']._serialized_end=5920
+  _globals['_USERCOMMITFILESREQUEST']._serialized_start=5923
+  _globals['_USERCOMMITFILESREQUEST']._serialized_end=6089
+  _globals['_USERCOMMITFILESRESPONSE']._serialized_start=6091
+  _globals['_USERCOMMITFILESRESPONSE']._serialized_end=6218
+  _globals['_USERCOMMITFILESERROR']._serialized_start=6221
+  _globals['_USERCOMMITFILESERROR']._serialized_end=6394
+  _globals['_USERREBASECONFIRMABLEREQUEST']._serialized_start=6397
+  _globals['_USERREBASECONFIRMABLEREQUEST']._serialized_end=6837
+  _globals['_USERREBASECONFIRMABLEREQUEST_HEADER']._serialized_start=6510
+  _globals['_USERREBASECONFIRMABLEREQUEST_HEADER']._serialized_end=6794
+  _globals['_USERREBASECONFIRMABLERESPONSE']._serialized_start=6840
+  _globals['_USERREBASECONFIRMABLERESPONSE']._serialized_end=7005
+  _globals['_USERSQUASHREQUEST']._serialized_start=7008
+  _globals['_USERSQUASHREQUEST']._serialized_end=7261
+  _globals['_USERSQUASHRESPONSE']._serialized_start=7263
+  _globals['_USERSQUASHRESPONSE']._serialized_end=7345
+  _globals['_USERREBASECONFIRMABLEERROR']._serialized_start=7348
+  _globals['_USERREBASECONFIRMABLEERROR']._serialized_end=7490
+  _globals['_USERSQUASHERROR']._serialized_start=7493
+  _globals['_USERSQUASHERROR']._serialized_end=7632
+  _globals['_USERAPPLYPATCHREQUEST']._serialized_start=7635
+  _globals['_USERAPPLYPATCHREQUEST']._serialized_end=7950
+  _globals['_USERAPPLYPATCHREQUEST_HEADER']._serialized_start=7736
+  _globals['_USERAPPLYPATCHREQUEST_HEADER']._serialized_end=7914
+  _globals['_USERAPPLYPATCHRESPONSE']._serialized_start=7952
+  _globals['_USERAPPLYPATCHRESPONSE']._serialized_end=8030
+  _globals['_USERUPDATESUBMODULEREQUEST']._serialized_start=8033
+  _globals['_USERUPDATESUBMODULEREQUEST']._serialized_end=8287
+  _globals['_USERUPDATESUBMODULERESPONSE']._serialized_start=8290
+  _globals['_USERUPDATESUBMODULERESPONSE']._serialized_end=8447
+  _globals['_OPERATIONSERVICE']._serialized_start=8450
+  _globals['_OPERATIONSERVICE']._serialized_end=9931
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hgitaly-1.3.3/hgitaly/stub/operations_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/ref_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/ref_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/ref_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/repository_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/repository_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/repository_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/repository_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,16 @@
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def WriteRef(self, request, context):
         """WriteRef creates or updates a ref in a repository to point to a new value.
+        If the request contains object revisions that do not exist in the repository, the RPC returns
+        the NOT_FOUND code with the ReferenceNotFoundError detail.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def FindMergeBase(self, request, context):
         """FindMergeBase returns the best common ancestor between two or more commits. Consult the man
```

### Comparing `hgitaly-1.3.3/hgitaly/stub/server_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/server_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/server_pb2_grpc.py` & `hgitaly-1.4.0/hgitaly/stub/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/stub/shared_pb2.py` & `hgitaly-1.4.0/hgitaly/stub/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tag.py` & `hgitaly-1.4.0/hgitaly/tag.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/testing/bundle.py` & `hgitaly-1.4.0/hgitaly/testing/bundle.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/testing/context.py` & `hgitaly-1.4.0/hgitaly/testing/context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/testing/grpc.py` & `hgitaly-1.4.0/hgitaly/testing/grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/testing/ssh.py` & `hgitaly-1.4.0/hgitaly/testing/ssh.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/testing/sshd.py` & `hgitaly-1.4.0/hgitaly/testing/sshd.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/testing/tests/test_sshd.py` & `hgitaly-1.4.0/hgitaly/testing/tests/test_sshd.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/common.py` & `hgitaly-1.4.0/hgitaly/tests/common.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_branch.py` & `hgitaly-1.4.0/hgitaly/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_diff.py` & `hgitaly-1.4.0/hgitaly/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_errors.py` & `hgitaly-1.4.0/hgitaly/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_feature.py` & `hgitaly-1.4.0/hgitaly/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_file_context.py` & `hgitaly-1.4.0/hgitaly/tests/test_file_context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_gitlab_ref.py` & `hgitaly-1.4.0/hgitaly/tests/test_gitlab_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_license_detector.py` & `hgitaly-1.4.0/hgitaly/tests/test_license_detector.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_linguist.py` & `hgitaly-1.4.0/hgitaly/tests/test_linguist.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_manifest.py` & `hgitaly-1.4.0/hgitaly/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_messages.py` & `hgitaly-1.4.0/hgitaly/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_oid.py` & `hgitaly-1.4.0/hgitaly/tests/test_oid.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_peer.py` & `hgitaly-1.4.0/hgitaly/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_repository.py` & `hgitaly-1.4.0/hgitaly/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_revision.py` & `hgitaly-1.4.0/hgitaly/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_revset.py` & `hgitaly-1.4.0/hgitaly/tests/test_revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_servicer.py` & `hgitaly-1.4.0/hgitaly/tests/test_servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_stream.py` & `hgitaly-1.4.0/hgitaly/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_tag.py` & `hgitaly-1.4.0/hgitaly/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/tests/test_workdir.py` & `hgitaly-1.4.0/hgitaly/tests/test_workdir.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/util.py` & `hgitaly-1.4.0/hgitaly/util.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly/workdir.py` & `hgitaly-1.4.0/hgitaly/workdir.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/hgitaly.egg-info/PKG-INFO` & `hgitaly-1.4.0/hgitaly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 1.3.3
+Version: 1.4.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Requires-Python: >=3.8
```

### Comparing `hgitaly-1.3.3/hgitaly.egg-info/SOURCES.txt` & `hgitaly-1.4.0/hgitaly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/setup.py` & `hgitaly-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/__init__.py` & `hgitaly-1.4.0/tests_with_gitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/comparison.py` & `hgitaly-1.4.0/tests_with_gitaly/comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/conftest.py` & `hgitaly-1.4.0/tests_with_gitaly/conftest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/gitaly.py` & `hgitaly-1.4.0/tests_with_gitaly/gitaly.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/hgitaly_rhgitaly_comparison.py` & `hgitaly-1.4.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/rhgitaly.py` & `hgitaly-1.4.0/tests_with_gitaly/rhgitaly.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_blob_tree.py` & `hgitaly-1.4.0/tests_with_gitaly/test_blob_tree.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_commit.py` & `hgitaly-1.4.0/tests_with_gitaly/test_commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 )
 if skip_comparison_tests():  # pragma no cover
     pytestmark = pytest.mark.skip
 
 parametrize = pytest.mark.parametrize
 
 
-def test_compare_last_commit_for(gitaly_comparison):
-    fixture = gitaly_comparison
+@parametrize('hg_server', ('hgitaly', 'rhgitaly'))
+def test_compare_last_commit_for(gitaly_rhgitaly_comparison, hg_server):
+    fixture = gitaly_rhgitaly_comparison
     git_repo = fixture.git_repo
 
     wrapper = fixture.hg_repo_wrapper
     ctx0 = wrapper.write_commit('foo', message="Some foo")
     git_shas = {
         ctx0.hex(): git_repo.branches()[b'branch/default']['sha'],
     }
@@ -107,14 +108,15 @@
     # exist (let's not depend on Gitaly accepting symbolic revisions, here)
     assert_compare_errors(revision=b'be0123ef' * 5, path=b'sub')
 
     def lcfp_norm(rpc_helper, response, **kw):
         normalize_commit_message(response.commit)
 
     rpc_helper = fixture.rpc_helper(stub_cls=CommitServiceStub,
+                                    hg_server=hg_server,
                                     method_name='LastCommitForPath',
                                     request_cls=LastCommitForPathRequest,
                                     request_sha_attrs=['revision'],
                                     response_sha_attrs=[
                                         'commit.id',
                                         'commit.parent_ids[]',
                                         ],
@@ -396,16 +398,17 @@
     def sorted_comparison():
         orig = rpc_helper.sorted
         rpc_helper.sorted = True
         yield
         rpc_helper.sorted = orig
 
     assert_compare = rpc_helper.assert_compare
+    assert_compare_errors = rpc_helper.assert_compare_errors
 
-    assert_compare(revision=b'HEAD')
+    assert_compare_errors(revision=b'HEAD')
     fixture.invalidate()  # for the hg->git map
 
     # set_default_gitlab_branch(wrapper.repo, b'branch/default')
     # prepare repo as:
     #
     #   @    4 (branch/default) merge with stable
     #   |\
```

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_comparison.py` & `hgitaly-1.4.0/tests_with_gitaly/test_comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_diff.py` & `hgitaly-1.4.0/tests_with_gitaly/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_gitaly_server.py` & `hgitaly-1.4.0/tests_with_gitaly/test_gitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_operations.py` & `hgitaly-1.4.0/tests_with_gitaly/test_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_ref.py` & `hgitaly-1.4.0/tests_with_gitaly/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_repository_service.py` & `hgitaly-1.4.0/tests_with_gitaly/test_repository_service.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_rhgitaly_server.py` & `hgitaly-1.4.0/tests_with_gitaly/test_rhgitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.3.3/tests_with_gitaly/test_server.py` & `hgitaly-1.4.0/tests_with_gitaly/test_server.py`

 * *Files identical despite different names*


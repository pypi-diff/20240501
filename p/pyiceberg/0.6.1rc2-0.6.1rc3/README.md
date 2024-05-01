# Comparing `tmp/pyiceberg-0.6.1rc2.tar.gz` & `tmp/pyiceberg-0.6.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiceberg-0.6.1rc2.tar", max compression
+gzip compressed data, was "pyiceberg-0.6.1rc3.tar", max compression
```

## Comparing `pyiceberg-0.6.1rc2.tar` & `pyiceberg-0.6.1rc3.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0    12548 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/LICENSE
--rw-r--r--   0        0        0     2567 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/Makefile
--rw-r--r--   0        0        0      251 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/NOTICE
--rw-r--r--   0        0        0     1218 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/README.md
--rw-r--r--   0        0        0     2196 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/build-module.py
--rw-r--r--   0        0        0       43 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/dev/.rat-excludes
--rw-r--r--   0        0        0     2856 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/dev/Dockerfile
--rwxr-xr-x   0        0        0     2529 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/dev/check-license
--rw-r--r--   0        0        0     1018 2024-04-16 03:08:56.497691 pyiceberg-0.6.1rc2/dev/docker-compose-azurite.yml
--rw-r--r--   0        0        0     1061 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/docker-compose-gcs-server.yml
--rw-r--r--   0        0        0     2851 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/docker-compose-integration.yml
--rw-r--r--   0        0        0     1626 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/docker-compose.yml
--rwxr-xr-x   0        0        0      912 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/entrypoint.sh
--rw-r--r--   0        0        0     1584 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/hive/Dockerfile
--rw-r--r--   0        0        0     1756 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/hive/core-site.xml
--rw-r--r--   0        0        0    11857 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/provision.py
--rwxr-xr-x   0        0        0     1198 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/run-azurite.sh
--rw-r--r--   0        0        0     1218 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/run-gcs-server.sh
--rwxr-xr-x   0        0        0     1194 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/run-minio.sh
--rw-r--r--   0        0        0     1895 2024-04-16 03:08:56.501691 pyiceberg-0.6.1rc2/dev/spark-defaults.conf
--rw-r--r--   0        0        0      808 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/__init__.py
--rw-r--r--   0        0        0     1685 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/__init__.py
--rw-r--r--   0        0        0     1621 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/bzip2.py
--rw-r--r--   0        0        0     1115 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/codec.py
--rw-r--r--   0        0        0     1416 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/deflate.py
--rw-r--r--   0        0        0     2702 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/snappy_codec.py
--rw-r--r--   0        0        0     2075 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/zstandard_codec.py
--rw-r--r--   0        0        0     6025 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/decoder.py
--rw-r--r--   0        0        0     1985 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/decoder_basic.c
--rw-r--r--   0        0        0     1811 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/decoder_fast.pyi
--rw-r--r--   0        0        0     6360 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/decoder_fast.pyx
--rw-r--r--   0        0        0     2904 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/encoder.py
--rw-r--r--   0        0        0     9396 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/file.py
--rw-r--r--   0        0        0    16716 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/reader.py
--rw-r--r--   0        0        0    20003 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/resolver.py
--rw-r--r--   0        0        0     6564 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/avro/writer.py
--rw-r--r--   0        0        0    25005 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/catalog/__init__.py
--rw-r--r--   0        0        0    31800 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/catalog/dynamodb.py
--rw-r--r--   0        0        0    28827 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/catalog/glue.py
--rw-r--r--   0        0        0    25030 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/catalog/hive.py
--rw-r--r--   0        0        0     3583 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/catalog/noop.py
--rw-r--r--   0        0        0    26345 2024-04-16 03:08:56.509691 pyiceberg-0.6.1rc2/pyiceberg/catalog/rest.py
--rw-r--r--   0        0        0    27936 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/catalog/sql.py
--rw-r--r--   0        0        0      785 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/cli/__init__.py
--rw-r--r--   0        0        0    14432 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/cli/console.py
--rw-r--r--   0        0        0     8772 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/cli/output.py
--rw-r--r--   0        0        0    10197 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/conversions.py
--rw-r--r--   0        0        0     3085 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/exceptions.py
--rw-r--r--   0        0        0    30164 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/expressions/__init__.py
--rw-r--r--   0        0        0    23158 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/expressions/literals.py
--rw-r--r--   0        0        0     7761 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/expressions/parser.py
--rw-r--r--   0        0        0    55613 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/expressions/visitors.py
--rw-r--r--   0        0        0    11628 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/io/__init__.py
--rw-r--r--   0        0        0    12121 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/io/fsspec.py
--rw-r--r--   0        0        0    70712 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/io/pyarrow.py
--rw-r--r--   0        0        0    36875 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/manifest.py
--rw-r--r--   0        0        0     8250 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/partitioning.py
--rw-r--r--   0        0        0      826 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/py.typed
--rw-r--r--   0        0        0    61024 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/schema.py
--rw-r--r--   0        0        0     4964 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/serializers.py
--rw-r--r--   0        0        0   100442 2024-04-16 03:08:56.513691 pyiceberg-0.6.1rc2/pyiceberg/table/__init__.py
--rw-r--r--   0        0        0    20318 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/table/metadata.py
--rw-r--r--   0        0        0     6891 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/table/name_mapping.py
--rw-r--r--   0        0        0     2460 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/table/refs.py
--rw-r--r--   0        0        0    14702 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/table/snapshots.py
--rw-r--r--   0        0        0     6892 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/table/sorting.py
--rw-r--r--   0        0        0    27363 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/transforms.py
--rw-r--r--   0        0        0     7322 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/typedef.py
--rw-r--r--   0        0        0    23492 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/types.py
--rw-r--r--   0        0        0      785 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/__init__.py
--rw-r--r--   0        0        0     3243 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/bin_packing.py
--rw-r--r--   0        0        0     1552 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/concurrent.py
--rw-r--r--   0        0        0     7219 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/config.py
--rw-r--r--   0        0        0     7022 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/datetime.py
--rw-r--r--   0        0        0     4348 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/decimal.py
--rw-r--r--   0        0        0     1829 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/deprecated.py
--rw-r--r--   0        0        0     2349 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/lazydict.py
--rw-r--r--   0        0        0     1405 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/parsing.py
--rw-r--r--   0        0        0    23395 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/schema_conversion.py
--rw-r--r--   0        0        0     2141 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/singleton.py
--rw-r--r--   0        0        0     1856 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/pyiceberg/utils/truncate.py
--rw-r--r--   0        0        0    18191 2024-04-16 03:09:03.817631 pyiceberg-0.6.1rc2/pyproject.toml
--rw-r--r--   0        0        0     7525 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/avro/test_decoder.py
--rw-r--r--   0        0        0     3632 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/avro/test_encoder.py
--rw-r--r--   0        0        0    12572 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/avro/test_file.py
--rw-r--r--   0        0        0    15572 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/avro/test_reader.py
--rw-r--r--   0        0        0    12594 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/avro/test_resolver.py
--rw-r--r--   0        0        0     5939 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/avro/test_writer.py
--rw-r--r--   0        0        0    11602 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/catalog/integration_test_dynamodb.py
--rw-r--r--   0        0        0    19459 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/catalog/integration_test_glue.py
--rw-r--r--   0        0        0    26374 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/catalog/test_base.py
--rw-r--r--   0        0        0    24772 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/catalog/test_dynamodb.py
--rw-r--r--   0        0        0    29880 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/catalog/test_glue.py
--rw-r--r--   0        0        0    38624 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/catalog/test_hive.py
--rw-r--r--   0        0        0    30584 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/catalog/test_rest.py
--rw-r--r--   0        0        0    31465 2024-04-16 03:08:56.517691 pyiceberg-0.6.1rc2/tests/catalog/test_sql.py
--rw-r--r--   0        0        0    36737 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/cli/test_console.py
--rw-r--r--   0        0        0      799 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/cli/test_output.py
--rw-r--r--   0        0        0    79787 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/conftest.py
--rw-r--r--   0        0        0    45204 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/expressions/test_evaluator.py
--rw-r--r--   0        0        0    44013 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/expressions/test_expressions.py
--rw-r--r--   0        0        0    27381 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/expressions/test_literals.py
--rw-r--r--   0        0        0     7048 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/expressions/test_parser.py
--rw-r--r--   0        0        0    12446 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/expressions/test_projection.py
--rw-r--r--   0        0        0    63987 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/expressions/test_visitors.py
--rw-r--r--   0        0        0    21345 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/integration/test_reads.py
--rw-r--r--   0        0        0     4856 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/integration/test_rest_manifest.py
--rw-r--r--   0        0        0    94266 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/integration/test_rest_schema.py
--rw-r--r--   0        0        0    26887 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/integration/test_writes.py
--rw-r--r--   0        0        0    27032 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/io/test_fsspec.py
--rw-r--r--   0        0        0    11532 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/io/test_io.py
--rw-r--r--   0        0        0    59346 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/io/test_pyarrow.py
--rw-r--r--   0        0        0    27462 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/io/test_pyarrow_stats.py
--rw-r--r--   0        0        0    19085 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/io/test_pyarrow_visitor.py
--rw-r--r--   0        0        0    40869 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/table/test_init.py
--rw-r--r--   0        0        0    32589 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/table/test_metadata.py
--rw-r--r--   0        0        0     8861 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/table/test_name_mapping.py
--rw-r--r--   0        0        0     5474 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/table/test_partitioning.py
--rw-r--r--   0        0        0     3282 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/table/test_refs.py
--rw-r--r--   0        0        0    10093 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/table/test_snapshots.py
--rw-r--r--   0        0        0     4111 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/table/test_sorting.py
--rw-r--r--   0        0        0    22756 2024-04-16 03:08:56.521690 pyiceberg-0.6.1rc2/tests/test_conversions.py
--rw-r--r--   0        0        0    61584 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/test_schema.py
--rw-r--r--   0        0        0     2336 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/test_serializers.py
--rw-r--r--   0        0        0    35991 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/test_transforms.py
--rw-r--r--   0        0        0     2567 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/test_typedef.py
--rw-r--r--   0        0        0    18815 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/test_types.py
--rw-r--r--   0        0        0     1113 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/test_version.py
--rw-r--r--   0        0        0     2725 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_bin_packing.py
--rw-r--r--   0        0        0     1720 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_concurrent.py
--rw-r--r--   0        0        0     3622 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_config.py
--rw-r--r--   0        0        0     2551 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1705 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_decimal.py
--rw-r--r--   0        0        0     1354 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_deprecated.py
--rw-r--r--   0        0        0     1198 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_lazydict.py
--rw-r--r--   0        0        0    19020 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_manifest.py
--rw-r--r--   0        0        0    13077 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_schema_conversion.py
--rw-r--r--   0        0        0     1334 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_singleton.py
--rw-r--r--   0        0        0     1319 2024-04-16 03:08:56.525690 pyiceberg-0.6.1rc2/tests/utils/test_truncate.py
--rw-r--r--   0        0        0    74745 2024-04-16 03:08:56.529690 pyiceberg-0.6.1rc2/vendor/fb303/FacebookService.py
--rw-r--r--   0        0        0      853 2024-04-16 03:08:56.529690 pyiceberg-0.6.1rc2/vendor/fb303/__init__.py
--rw-r--r--   0        0        0      943 2024-04-16 03:08:56.529690 pyiceberg-0.6.1rc2/vendor/fb303/constants.py
--rw-r--r--   0        0        0     1549 2024-04-16 03:08:56.529690 pyiceberg-0.6.1rc2/vendor/fb303/ttypes.py
--rw-r--r--   0        0        0  2241478 2024-04-16 03:08:56.533690 pyiceberg-0.6.1rc2/vendor/hive_metastore/ThriftHiveMetastore.py
--rw-r--r--   0        0        0      856 2024-04-16 03:08:56.533690 pyiceberg-0.6.1rc2/vendor/hive_metastore/__init__.py
--rw-r--r--   0        0        0     2401 2024-04-16 03:08:56.533690 pyiceberg-0.6.1rc2/vendor/hive_metastore/constants.py
--rw-r--r--   0        0        0  1354270 2024-04-16 03:08:56.537690 pyiceberg-0.6.1rc2/vendor/hive_metastore/ttypes.py
--rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 pyiceberg-0.6.1rc2/PKG-INFO
+-rw-r--r--   0        0        0    12548 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/LICENSE
+-rw-r--r--   0        0        0     2567 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/Makefile
+-rw-r--r--   0        0        0      251 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/NOTICE
+-rw-r--r--   0        0        0     1218 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/README.md
+-rw-r--r--   0        0        0     2196 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/build-module.py
+-rw-r--r--   0        0        0       43 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/.rat-excludes
+-rw-r--r--   0        0        0     2856 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/Dockerfile
+-rwxr-xr-x   0        0        0     2529 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/check-license
+-rw-r--r--   0        0        0     1018 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/docker-compose-azurite.yml
+-rw-r--r--   0        0        0     1061 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/docker-compose-gcs-server.yml
+-rw-r--r--   0        0        0     2851 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/docker-compose-integration.yml
+-rw-r--r--   0        0        0     1626 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/docker-compose.yml
+-rwxr-xr-x   0        0        0      912 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/entrypoint.sh
+-rw-r--r--   0        0        0     1584 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/hive/Dockerfile
+-rw-r--r--   0        0        0     1756 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/hive/core-site.xml
+-rw-r--r--   0        0        0    11857 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/provision.py
+-rwxr-xr-x   0        0        0     1198 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/run-azurite.sh
+-rw-r--r--   0        0        0     1218 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/run-gcs-server.sh
+-rwxr-xr-x   0        0        0     1194 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/run-minio.sh
+-rw-r--r--   0        0        0     1895 2024-04-18 06:48:15.845155 pyiceberg-0.6.1rc3/dev/spark-defaults.conf
+-rw-r--r--   0        0        0      808 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/__init__.py
+-rw-r--r--   0        0        0     1685 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/__init__.py
+-rw-r--r--   0        0        0     1621 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/bzip2.py
+-rw-r--r--   0        0        0     1115 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/codec.py
+-rw-r--r--   0        0        0     1416 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/deflate.py
+-rw-r--r--   0        0        0     2702 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/snappy_codec.py
+-rw-r--r--   0        0        0     2075 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/zstandard_codec.py
+-rw-r--r--   0        0        0     6025 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/decoder.py
+-rw-r--r--   0        0        0     1985 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/decoder_basic.c
+-rw-r--r--   0        0        0     1811 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/decoder_fast.pyi
+-rw-r--r--   0        0        0     6360 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/decoder_fast.pyx
+-rw-r--r--   0        0        0     2904 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/encoder.py
+-rw-r--r--   0        0        0     9396 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/file.py
+-rw-r--r--   0        0        0    16716 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/reader.py
+-rw-r--r--   0        0        0    20003 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/resolver.py
+-rw-r--r--   0        0        0     6564 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/avro/writer.py
+-rw-r--r--   0        0        0    25005 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/catalog/__init__.py
+-rw-r--r--   0        0        0    31800 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/catalog/dynamodb.py
+-rw-r--r--   0        0        0    28827 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/catalog/glue.py
+-rw-r--r--   0        0        0    25030 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/catalog/hive.py
+-rw-r--r--   0        0        0     3583 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/catalog/noop.py
+-rw-r--r--   0        0        0    26345 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/catalog/rest.py
+-rw-r--r--   0        0        0    27936 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/catalog/sql.py
+-rw-r--r--   0        0        0      785 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/cli/__init__.py
+-rw-r--r--   0        0        0    14432 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/cli/console.py
+-rw-r--r--   0        0        0     8772 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/cli/output.py
+-rw-r--r--   0        0        0    10197 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/conversions.py
+-rw-r--r--   0        0        0     3085 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/exceptions.py
+-rw-r--r--   0        0        0    30164 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/expressions/__init__.py
+-rw-r--r--   0        0        0    23158 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/expressions/literals.py
+-rw-r--r--   0        0        0     7761 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/expressions/parser.py
+-rw-r--r--   0        0        0    55613 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/expressions/visitors.py
+-rw-r--r--   0        0        0    11628 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/io/__init__.py
+-rw-r--r--   0        0        0    12121 2024-04-18 06:48:15.857155 pyiceberg-0.6.1rc3/pyiceberg/io/fsspec.py
+-rw-r--r--   0        0        0    70712 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/io/pyarrow.py
+-rw-r--r--   0        0        0    36875 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/manifest.py
+-rw-r--r--   0        0        0     8250 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/partitioning.py
+-rw-r--r--   0        0        0      826 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/py.typed
+-rw-r--r--   0        0        0    61024 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/schema.py
+-rw-r--r--   0        0        0     4964 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/serializers.py
+-rw-r--r--   0        0        0   100442 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/table/__init__.py
+-rw-r--r--   0        0        0    20318 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/table/metadata.py
+-rw-r--r--   0        0        0     6891 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/table/name_mapping.py
+-rw-r--r--   0        0        0     2460 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/table/refs.py
+-rw-r--r--   0        0        0    14702 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/table/snapshots.py
+-rw-r--r--   0        0        0     6892 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/table/sorting.py
+-rw-r--r--   0        0        0    27363 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/transforms.py
+-rw-r--r--   0        0        0     7322 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/typedef.py
+-rw-r--r--   0        0        0    23492 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/types.py
+-rw-r--r--   0        0        0      785 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/__init__.py
+-rw-r--r--   0        0        0     3243 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/bin_packing.py
+-rw-r--r--   0        0        0     1552 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/concurrent.py
+-rw-r--r--   0        0        0     7219 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/config.py
+-rw-r--r--   0        0        0     7022 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/datetime.py
+-rw-r--r--   0        0        0     4348 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/decimal.py
+-rw-r--r--   0        0        0     1829 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/deprecated.py
+-rw-r--r--   0        0        0     2349 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/lazydict.py
+-rw-r--r--   0        0        0     1405 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/parsing.py
+-rw-r--r--   0        0        0    23395 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/schema_conversion.py
+-rw-r--r--   0        0        0     2141 2024-04-18 06:48:15.861156 pyiceberg-0.6.1rc3/pyiceberg/utils/singleton.py
+-rw-r--r--   0        0        0     1856 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/pyiceberg/utils/truncate.py
+-rw-r--r--   0        0        0    18211 2024-04-18 06:48:24.345210 pyiceberg-0.6.1rc3/pyproject.toml
+-rw-r--r--   0        0        0     7525 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/avro/test_decoder.py
+-rw-r--r--   0        0        0     3632 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/avro/test_encoder.py
+-rw-r--r--   0        0        0    12572 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/avro/test_file.py
+-rw-r--r--   0        0        0    15572 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/avro/test_reader.py
+-rw-r--r--   0        0        0    12594 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/avro/test_resolver.py
+-rw-r--r--   0        0        0     5939 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/avro/test_writer.py
+-rw-r--r--   0        0        0    11602 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/catalog/integration_test_dynamodb.py
+-rw-r--r--   0        0        0    19459 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/catalog/integration_test_glue.py
+-rw-r--r--   0        0        0    26374 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/catalog/test_base.py
+-rw-r--r--   0        0        0    24772 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/catalog/test_dynamodb.py
+-rw-r--r--   0        0        0    29880 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/catalog/test_glue.py
+-rw-r--r--   0        0        0    38624 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/catalog/test_hive.py
+-rw-r--r--   0        0        0    30584 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/catalog/test_rest.py
+-rw-r--r--   0        0        0    31465 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/catalog/test_sql.py
+-rw-r--r--   0        0        0    36737 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/cli/test_console.py
+-rw-r--r--   0        0        0      799 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/cli/test_output.py
+-rw-r--r--   0        0        0    79787 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/conftest.py
+-rw-r--r--   0        0        0    45204 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/expressions/test_evaluator.py
+-rw-r--r--   0        0        0    44013 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/expressions/test_expressions.py
+-rw-r--r--   0        0        0    27381 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/expressions/test_literals.py
+-rw-r--r--   0        0        0     7048 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/expressions/test_parser.py
+-rw-r--r--   0        0        0    12446 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/expressions/test_projection.py
+-rw-r--r--   0        0        0    63987 2024-04-18 06:48:15.865156 pyiceberg-0.6.1rc3/tests/expressions/test_visitors.py
+-rw-r--r--   0        0        0    21345 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/integration/test_reads.py
+-rw-r--r--   0        0        0     4856 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/integration/test_rest_manifest.py
+-rw-r--r--   0        0        0    94266 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/integration/test_rest_schema.py
+-rw-r--r--   0        0        0    26887 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/integration/test_writes.py
+-rw-r--r--   0        0        0    27032 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/io/test_fsspec.py
+-rw-r--r--   0        0        0    11532 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/io/test_io.py
+-rw-r--r--   0        0        0    59346 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/io/test_pyarrow.py
+-rw-r--r--   0        0        0    27462 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/io/test_pyarrow_stats.py
+-rw-r--r--   0        0        0    19085 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/io/test_pyarrow_visitor.py
+-rw-r--r--   0        0        0    40869 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/table/test_init.py
+-rw-r--r--   0        0        0    32589 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/table/test_metadata.py
+-rw-r--r--   0        0        0     8861 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/table/test_name_mapping.py
+-rw-r--r--   0        0        0     5474 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/table/test_partitioning.py
+-rw-r--r--   0        0        0     3282 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/table/test_refs.py
+-rw-r--r--   0        0        0    10093 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/table/test_snapshots.py
+-rw-r--r--   0        0        0     4111 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/table/test_sorting.py
+-rw-r--r--   0        0        0    22756 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/test_conversions.py
+-rw-r--r--   0        0        0    61584 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/test_schema.py
+-rw-r--r--   0        0        0     2336 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/test_serializers.py
+-rw-r--r--   0        0        0    35991 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/test_transforms.py
+-rw-r--r--   0        0        0     2567 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/test_typedef.py
+-rw-r--r--   0        0        0    18815 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/test_types.py
+-rw-r--r--   0        0        0     1113 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/test_version.py
+-rw-r--r--   0        0        0     2725 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/utils/test_bin_packing.py
+-rw-r--r--   0        0        0     1720 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/utils/test_concurrent.py
+-rw-r--r--   0        0        0     3622 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/utils/test_config.py
+-rw-r--r--   0        0        0     2551 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1705 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/utils/test_decimal.py
+-rw-r--r--   0        0        0     1354 2024-04-18 06:48:15.869156 pyiceberg-0.6.1rc3/tests/utils/test_deprecated.py
+-rw-r--r--   0        0        0     1198 2024-04-18 06:48:15.873156 pyiceberg-0.6.1rc3/tests/utils/test_lazydict.py
+-rw-r--r--   0        0        0    19020 2024-04-18 06:48:15.873156 pyiceberg-0.6.1rc3/tests/utils/test_manifest.py
+-rw-r--r--   0        0        0    13077 2024-04-18 06:48:15.873156 pyiceberg-0.6.1rc3/tests/utils/test_schema_conversion.py
+-rw-r--r--   0        0        0     1334 2024-04-18 06:48:15.873156 pyiceberg-0.6.1rc3/tests/utils/test_singleton.py
+-rw-r--r--   0        0        0     1319 2024-04-18 06:48:15.873156 pyiceberg-0.6.1rc3/tests/utils/test_truncate.py
+-rw-r--r--   0        0        0    74745 2024-04-18 06:48:15.877156 pyiceberg-0.6.1rc3/vendor/fb303/FacebookService.py
+-rw-r--r--   0        0        0      853 2024-04-18 06:48:15.877156 pyiceberg-0.6.1rc3/vendor/fb303/__init__.py
+-rw-r--r--   0        0        0      943 2024-04-18 06:48:15.877156 pyiceberg-0.6.1rc3/vendor/fb303/constants.py
+-rw-r--r--   0        0        0     1549 2024-04-18 06:48:15.877156 pyiceberg-0.6.1rc3/vendor/fb303/ttypes.py
+-rw-r--r--   0        0        0  2241478 2024-04-18 06:48:15.881156 pyiceberg-0.6.1rc3/vendor/hive_metastore/ThriftHiveMetastore.py
+-rw-r--r--   0        0        0      856 2024-04-18 06:48:15.881156 pyiceberg-0.6.1rc3/vendor/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     2401 2024-04-18 06:48:15.881156 pyiceberg-0.6.1rc3/vendor/hive_metastore/constants.py
+-rw-r--r--   0        0        0  1354270 2024-04-18 06:48:15.881156 pyiceberg-0.6.1rc3/vendor/hive_metastore/ttypes.py
+-rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 pyiceberg-0.6.1rc3/PKG-INFO
```

### Comparing `pyiceberg-0.6.1rc2/LICENSE` & `pyiceberg-0.6.1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/Makefile` & `pyiceberg-0.6.1rc3/Makefile`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/README.md` & `pyiceberg-0.6.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/build-module.py` & `pyiceberg-0.6.1rc3/build-module.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/Dockerfile` & `pyiceberg-0.6.1rc3/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/check-license` & `pyiceberg-0.6.1rc3/dev/check-license`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/docker-compose-azurite.yml` & `pyiceberg-0.6.1rc3/dev/docker-compose-azurite.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/docker-compose-gcs-server.yml` & `pyiceberg-0.6.1rc3/dev/docker-compose-gcs-server.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/docker-compose-integration.yml` & `pyiceberg-0.6.1rc3/dev/docker-compose-integration.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/docker-compose.yml` & `pyiceberg-0.6.1rc3/dev/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/entrypoint.sh` & `pyiceberg-0.6.1rc3/dev/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/hive/Dockerfile` & `pyiceberg-0.6.1rc3/dev/hive/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/hive/core-site.xml` & `pyiceberg-0.6.1rc3/dev/hive/core-site.xml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/provision.py` & `pyiceberg-0.6.1rc3/dev/provision.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/run-azurite.sh` & `pyiceberg-0.6.1rc3/dev/run-azurite.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/run-gcs-server.sh` & `pyiceberg-0.6.1rc3/dev/run-gcs-server.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/run-minio.sh` & `pyiceberg-0.6.1rc3/dev/run-minio.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/dev/spark-defaults.conf` & `pyiceberg-0.6.1rc3/dev/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/bzip2.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/bzip2.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/codec.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/deflate.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/deflate.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/snappy_codec.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/snappy_codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/codecs/zstandard_codec.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/codecs/zstandard_codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/decoder.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/decoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/decoder_basic.c` & `pyiceberg-0.6.1rc3/pyiceberg/avro/decoder_basic.c`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/decoder_fast.pyi` & `pyiceberg-0.6.1rc3/pyiceberg/avro/decoder_fast.pyi`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/decoder_fast.pyx` & `pyiceberg-0.6.1rc3/pyiceberg/avro/decoder_fast.pyx`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/encoder.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/encoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/file.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/file.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/reader.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/reader.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/resolver.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/resolver.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/avro/writer.py` & `pyiceberg-0.6.1rc3/pyiceberg/avro/writer.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/catalog/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/catalog/dynamodb.py` & `pyiceberg-0.6.1rc3/pyiceberg/catalog/dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/catalog/glue.py` & `pyiceberg-0.6.1rc3/pyiceberg/catalog/glue.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/catalog/hive.py` & `pyiceberg-0.6.1rc3/pyiceberg/catalog/hive.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/catalog/noop.py` & `pyiceberg-0.6.1rc3/pyiceberg/catalog/noop.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/catalog/rest.py` & `pyiceberg-0.6.1rc3/pyiceberg/catalog/rest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/catalog/sql.py` & `pyiceberg-0.6.1rc3/pyiceberg/catalog/sql.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/cli/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/cli/console.py` & `pyiceberg-0.6.1rc3/pyiceberg/cli/console.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/cli/output.py` & `pyiceberg-0.6.1rc3/pyiceberg/cli/output.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/conversions.py` & `pyiceberg-0.6.1rc3/pyiceberg/conversions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/exceptions.py` & `pyiceberg-0.6.1rc3/pyiceberg/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/expressions/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/expressions/literals.py` & `pyiceberg-0.6.1rc3/pyiceberg/expressions/literals.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/expressions/parser.py` & `pyiceberg-0.6.1rc3/pyiceberg/expressions/parser.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/expressions/visitors.py` & `pyiceberg-0.6.1rc3/pyiceberg/expressions/visitors.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/io/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/io/fsspec.py` & `pyiceberg-0.6.1rc3/pyiceberg/io/fsspec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/io/pyarrow.py` & `pyiceberg-0.6.1rc3/pyiceberg/io/pyarrow.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/manifest.py` & `pyiceberg-0.6.1rc3/pyiceberg/manifest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/partitioning.py` & `pyiceberg-0.6.1rc3/pyiceberg/partitioning.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/py.typed` & `pyiceberg-0.6.1rc3/pyiceberg/py.typed`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/schema.py` & `pyiceberg-0.6.1rc3/pyiceberg/schema.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/serializers.py` & `pyiceberg-0.6.1rc3/pyiceberg/serializers.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/table/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/table/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/table/metadata.py` & `pyiceberg-0.6.1rc3/pyiceberg/table/metadata.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/table/name_mapping.py` & `pyiceberg-0.6.1rc3/pyiceberg/table/name_mapping.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/table/refs.py` & `pyiceberg-0.6.1rc3/pyiceberg/table/refs.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/table/snapshots.py` & `pyiceberg-0.6.1rc3/pyiceberg/table/snapshots.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/table/sorting.py` & `pyiceberg-0.6.1rc3/pyiceberg/table/sorting.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/transforms.py` & `pyiceberg-0.6.1rc3/pyiceberg/transforms.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/typedef.py` & `pyiceberg-0.6.1rc3/pyiceberg/typedef.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/types.py` & `pyiceberg-0.6.1rc3/pyiceberg/types.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/__init__.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/bin_packing.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/bin_packing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/concurrent.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/config.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/config.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/datetime.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/decimal.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/decimal.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/deprecated.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/lazydict.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/lazydict.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/parsing.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/schema_conversion.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/schema_conversion.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/singleton.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyiceberg/utils/truncate.py` & `pyiceberg-0.6.1rc3/pyiceberg/utils/truncate.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/pyproject.toml` & `pyiceberg-0.6.1rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.poetry]
 name = "pyiceberg"
-version = "0.6.1rc2"
+version = "0.6.1rc3"
 readme = "README.md"
 homepage = "https://py.iceberg.apache.org/"
 repository = "https://github.com/apache/iceberg-python"
 description = "Apache Iceberg is an open table format for huge analytic datasets"
 authors = ["Apache Software Foundation <dev@iceberg.apache.org>"]
 license = "Apache License 2.0"
 classifiers = [
@@ -81,14 +81,15 @@
 coverage = { version = "^7.4.1", extras = ["toml"] }
 requests-mock = "1.11.0"
 moto = { version = "^5.0.1", extras = ["server"] }
 typing-extensions = "4.9.0"
 pytest-mock = "3.12.0"
 pyspark = "3.5.0"
 cython = "3.0.8"
+docutils = "!=0.21"
 
 [[tool.mypy.overrides]]
 module = "pytest_mock.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "pyarrow.*"
```

### Comparing `pyiceberg-0.6.1rc2/tests/avro/test_decoder.py` & `pyiceberg-0.6.1rc3/tests/avro/test_decoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/avro/test_encoder.py` & `pyiceberg-0.6.1rc3/tests/avro/test_encoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/avro/test_file.py` & `pyiceberg-0.6.1rc3/tests/avro/test_file.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/avro/test_reader.py` & `pyiceberg-0.6.1rc3/tests/avro/test_reader.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/avro/test_resolver.py` & `pyiceberg-0.6.1rc3/tests/avro/test_resolver.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/avro/test_writer.py` & `pyiceberg-0.6.1rc3/tests/avro/test_writer.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/catalog/integration_test_dynamodb.py` & `pyiceberg-0.6.1rc3/tests/catalog/integration_test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/catalog/integration_test_glue.py` & `pyiceberg-0.6.1rc3/tests/catalog/integration_test_glue.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/catalog/test_base.py` & `pyiceberg-0.6.1rc3/tests/catalog/test_base.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/catalog/test_dynamodb.py` & `pyiceberg-0.6.1rc3/tests/catalog/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/catalog/test_glue.py` & `pyiceberg-0.6.1rc3/tests/catalog/test_glue.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/catalog/test_hive.py` & `pyiceberg-0.6.1rc3/tests/catalog/test_hive.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/catalog/test_rest.py` & `pyiceberg-0.6.1rc3/tests/catalog/test_rest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/catalog/test_sql.py` & `pyiceberg-0.6.1rc3/tests/catalog/test_sql.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/cli/test_console.py` & `pyiceberg-0.6.1rc3/tests/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/cli/test_output.py` & `pyiceberg-0.6.1rc3/tests/cli/test_output.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/conftest.py` & `pyiceberg-0.6.1rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/expressions/test_evaluator.py` & `pyiceberg-0.6.1rc3/tests/expressions/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/expressions/test_expressions.py` & `pyiceberg-0.6.1rc3/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/expressions/test_literals.py` & `pyiceberg-0.6.1rc3/tests/expressions/test_literals.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/expressions/test_parser.py` & `pyiceberg-0.6.1rc3/tests/expressions/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/expressions/test_projection.py` & `pyiceberg-0.6.1rc3/tests/expressions/test_projection.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/expressions/test_visitors.py` & `pyiceberg-0.6.1rc3/tests/expressions/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/integration/test_reads.py` & `pyiceberg-0.6.1rc3/tests/integration/test_reads.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/integration/test_rest_manifest.py` & `pyiceberg-0.6.1rc3/tests/integration/test_rest_manifest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/integration/test_rest_schema.py` & `pyiceberg-0.6.1rc3/tests/integration/test_rest_schema.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/integration/test_writes.py` & `pyiceberg-0.6.1rc3/tests/integration/test_writes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/io/test_fsspec.py` & `pyiceberg-0.6.1rc3/tests/io/test_fsspec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/io/test_io.py` & `pyiceberg-0.6.1rc3/tests/io/test_io.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/io/test_pyarrow.py` & `pyiceberg-0.6.1rc3/tests/io/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/io/test_pyarrow_stats.py` & `pyiceberg-0.6.1rc3/tests/io/test_pyarrow_stats.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/io/test_pyarrow_visitor.py` & `pyiceberg-0.6.1rc3/tests/io/test_pyarrow_visitor.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/table/test_init.py` & `pyiceberg-0.6.1rc3/tests/table/test_init.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/table/test_metadata.py` & `pyiceberg-0.6.1rc3/tests/table/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/table/test_name_mapping.py` & `pyiceberg-0.6.1rc3/tests/table/test_name_mapping.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/table/test_partitioning.py` & `pyiceberg-0.6.1rc3/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/table/test_refs.py` & `pyiceberg-0.6.1rc3/tests/table/test_refs.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/table/test_snapshots.py` & `pyiceberg-0.6.1rc3/tests/table/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/table/test_sorting.py` & `pyiceberg-0.6.1rc3/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/test_conversions.py` & `pyiceberg-0.6.1rc3/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/test_schema.py` & `pyiceberg-0.6.1rc3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/test_serializers.py` & `pyiceberg-0.6.1rc3/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/test_transforms.py` & `pyiceberg-0.6.1rc3/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/test_typedef.py` & `pyiceberg-0.6.1rc3/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/test_types.py` & `pyiceberg-0.6.1rc3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/test_version.py` & `pyiceberg-0.6.1rc3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_bin_packing.py` & `pyiceberg-0.6.1rc3/tests/utils/test_bin_packing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_concurrent.py` & `pyiceberg-0.6.1rc3/tests/utils/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_config.py` & `pyiceberg-0.6.1rc3/tests/utils/test_config.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_datetime.py` & `pyiceberg-0.6.1rc3/tests/utils/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_decimal.py` & `pyiceberg-0.6.1rc3/tests/utils/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_deprecated.py` & `pyiceberg-0.6.1rc3/tests/utils/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_lazydict.py` & `pyiceberg-0.6.1rc3/tests/utils/test_lazydict.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_manifest.py` & `pyiceberg-0.6.1rc3/tests/utils/test_manifest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_schema_conversion.py` & `pyiceberg-0.6.1rc3/tests/utils/test_schema_conversion.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_singleton.py` & `pyiceberg-0.6.1rc3/tests/utils/test_singleton.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/tests/utils/test_truncate.py` & `pyiceberg-0.6.1rc3/tests/utils/test_truncate.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/vendor/fb303/FacebookService.py` & `pyiceberg-0.6.1rc3/vendor/fb303/FacebookService.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/vendor/fb303/__init__.py` & `pyiceberg-0.6.1rc3/vendor/fb303/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/vendor/fb303/constants.py` & `pyiceberg-0.6.1rc3/vendor/fb303/constants.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/vendor/fb303/ttypes.py` & `pyiceberg-0.6.1rc3/vendor/fb303/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/vendor/hive_metastore/ThriftHiveMetastore.py` & `pyiceberg-0.6.1rc3/vendor/hive_metastore/ThriftHiveMetastore.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/vendor/hive_metastore/__init__.py` & `pyiceberg-0.6.1rc3/vendor/hive_metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/vendor/hive_metastore/constants.py` & `pyiceberg-0.6.1rc3/vendor/hive_metastore/constants.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/vendor/hive_metastore/ttypes.py` & `pyiceberg-0.6.1rc3/vendor/hive_metastore/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.6.1rc2/PKG-INFO` & `pyiceberg-0.6.1rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiceberg
-Version: 0.6.1rc2
+Version: 0.6.1rc3
 Summary: Apache Iceberg is an open table format for huge analytic datasets
 Home-page: https://py.iceberg.apache.org/
 License: Apache-2.0
 Author: Apache Software Foundation
 Author-email: dev@iceberg.apache.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


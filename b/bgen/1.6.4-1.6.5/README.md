# Comparing `tmp/bgen-1.6.4.tar.gz` & `tmp/bgen-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgen-1.6.4.tar", last modified: Mon Mar 11 21:03:26 2024, max compression
+gzip compressed data, was "bgen-1.6.5.tar", last modified: Wed May  1 18:59:47 2024, max compression
```

## Comparing `bgen-1.6.4.tar` & `bgen-1.6.5.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.706168 bgen-1.6.4/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-03-11 21:02:59.000000 bgen-1.6.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-11 21:02:59.000000 bgen-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-03-11 21:03:26.706168 bgen-1.6.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     6402 2024-03-11 21:02:59.000000 bgen-1.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-11 21:02:59.000000 bgen-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 21:03:26.706168 bgen-1.6.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-03-11 21:02:59.000000 bgen-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.686167 bgen-1.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.690167 bgen-1.6.4/src/bgen/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-11 21:02:59.000000 bgen-1.6.4/src/bgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-03-11 21:02:59.000000 bgen-1.6.4/src/bgen/index.py
--rw-r--r--   0 runner    (1001) docker     (127)  1644794 2024-03-11 21:03:25.000000 bgen-1.6.4/src/bgen/reader.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-03-11 21:02:59.000000 bgen-1.6.4/src/bgen/reader.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1327180 2024-03-11 21:03:26.000000 bgen-1.6.4/src/bgen/writer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-03-11 21:02:59.000000 bgen-1.6.4/src/bgen/writer.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.690167 bgen-1.6.4/src/bgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-03-11 21:03:26.000000 bgen-1.6.4/src/bgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-11 21:03:26.000000 bgen-1.6.4/src/bgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 21:03:26.000000 bgen-1.6.4/src/bgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-11 21:03:26.000000 bgen-1.6.4/src/bgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-11 21:03:26.000000 bgen-1.6.4/src/bgen.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    35199 2024-03-11 21:02:59.000000 bgen-1.6.4/src/genotypes.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     2005 2024-03-11 21:02:59.000000 bgen-1.6.4/src/genotypes.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     1343 2024-03-11 21:02:59.000000 bgen-1.6.4/src/header.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)      527 2024-03-11 21:02:59.000000 bgen-1.6.4/src/header.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     3372 2024-03-11 21:02:59.000000 bgen-1.6.4/src/reader.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-03-11 21:02:59.000000 bgen-1.6.4/src/reader.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     2303 2024-03-11 21:02:59.000000 bgen-1.6.4/src/samples.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-03-11 21:02:59.000000 bgen-1.6.4/src/samples.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     6535 2024-03-11 21:02:59.000000 bgen-1.6.4/src/utils.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)      527 2024-03-11 21:02:59.000000 bgen-1.6.4/src/utils.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     4116 2024-03-11 21:02:59.000000 bgen-1.6.4/src/variant.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-03-11 21:02:59.000000 bgen-1.6.4/src/variant.h
--rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-03-11 21:02:59.000000 bgen-1.6.4/src/writer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-11 21:02:59.000000 bgen-1.6.4/src/writer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.682167 bgen-1.6.4/src/zstd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.690167 bgen-1.6.4/src/zstd/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.694167 bgen-1.6.4/src/zstd/lib/common/
--rw-r--r--   0 runner    (1001) docker     (127)    18345 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/compiler.h
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/cpu.h
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/debug.c
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/debug.h
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/error_private.c
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/error_private.h
--rw-r--r--   0 runner    (1001) docker     (127)    33031 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/fse.h
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    19952 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/huf.h
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/mem.h
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/pool.c
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/pool.h
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/threading.c
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/threading.h
--rw-r--r--   0 runner    (1001) docker     (127)    29099 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/zstd_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/zstd_errors.h
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/common/zstd_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.698167 bgen-1.6.4/src/zstd/lib/compress/
--rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/hist.c
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/hist.h
--rw-r--r--   0 runner    (1001) docker     (127)    32772 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)   172484 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)    40937 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_compress_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_compress_literals.c
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_compress_literals.h
--rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_compress_sequences.c
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_compress_sequences.h
--rw-r--r--   0 runner    (1001) docker     (127)    19166 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_cwksp.h
--rw-r--r--   0 runner    (1001) docker     (127)    25278 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_double_fast.c
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_double_fast.h
--rw-r--r--   0 runner    (1001) docker     (127)    21936 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_fast.c
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_fast.h
--rw-r--r--   0 runner    (1001) docker     (127)    51720 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_lazy.c
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_lazy.h
--rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_ldm.c
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_ldm.h
--rw-r--r--   0 runner    (1001) docker     (127)    57582 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_opt.c
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstd_opt.h
--rw-r--r--   0 runner    (1001) docker     (127)    92625 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstdmt_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/compress/zstdmt_compress.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.698167 bgen-1.6.4/src/zstd/lib/decompress/
--rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/decompress/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/decompress/zstd_ddict.c
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/decompress/zstd_ddict.h
--rw-r--r--   0 runner    (1001) docker     (127)    72690 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/decompress/zstd_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    56849 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/decompress/zstd_decompress_block.c
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/decompress/zstd_decompress_block.h
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/decompress/zstd_decompress_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.702168 bgen-1.6.4/src/zstd/lib/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/deprecated/zbuff.h
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/deprecated/zbuff_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/deprecated/zbuff_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/deprecated/zbuff_decompress.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.702168 bgen-1.6.4/src/zstd/lib/dictBuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    42155 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/dictBuilder/cover.c
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/dictBuilder/cover.h
--rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/dictBuilder/divsufsort.c
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/dictBuilder/divsufsort.h
--rw-r--r--   0 runner    (1001) docker     (127)    28051 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/dictBuilder/fastcover.c
--rw-r--r--   0 runner    (1001) docker     (127)    43760 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/dictBuilder/zdict.c
--rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/dictBuilder/zdict.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:03:26.706168 bgen-1.6.4/src/zstd/lib/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_legacy.h
--rw-r--r--   0 runner    (1001) docker     (127)    71259 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v01.c
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v01.h
--rw-r--r--   0 runner    (1001) docker     (127)   128019 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v02.c
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v02.h
--rw-r--r--   0 runner    (1001) docker     (127)   114139 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v03.c
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v03.h
--rw-r--r--   0 runner    (1001) docker     (127)   135210 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v04.c
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v04.h
--rw-r--r--   0 runner    (1001) docker     (127)   156397 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v05.c
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v05.h
--rw-r--r--   0 runner    (1001) docker     (127)   166025 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v06.c
--rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v06.h
--rw-r--r--   0 runner    (1001) docker     (127)   185004 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v07.c
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/legacy/zstd_v07.h
--rw-r--r--   0 runner    (1001) docker     (127)   119972 2024-03-11 21:03:04.000000 bgen-1.6.4/src/zstd/lib/zstd.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.333150 bgen-1.6.5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1053 2024-05-01 18:59:19.000000 bgen-1.6.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 18:59:19.000000 bgen-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-01 18:59:47.333150 bgen-1.6.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6402 2024-05-01 18:59:19.000000 bgen-1.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 18:59:19.000000 bgen-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:59:47.333150 bgen-1.6.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-05-01 18:59:19.000000 bgen-1.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.317150 bgen-1.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.321150 bgen-1.6.5/src/bgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 18:59:19.000000 bgen-1.6.5/src/bgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-01 18:59:19.000000 bgen-1.6.5/src/bgen/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1646457 2024-05-01 18:59:46.000000 bgen-1.6.5/src/bgen/reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19691 2024-05-01 18:59:19.000000 bgen-1.6.5/src/bgen/reader.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1327999 2024-05-01 18:59:47.000000 bgen-1.6.5/src/bgen/writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-01 18:59:19.000000 bgen-1.6.5/src/bgen/writer.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.321150 bgen-1.6.5/src/bgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-01 18:59:47.000000 bgen-1.6.5/src/bgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-01 18:59:47.000000 bgen-1.6.5/src/bgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:59:47.000000 bgen-1.6.5/src/bgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 18:59:47.000000 bgen-1.6.5/src/bgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 18:59:47.000000 bgen-1.6.5/src/bgen.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35199 2024-05-01 18:59:19.000000 bgen-1.6.5/src/genotypes.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2005 2024-05-01 18:59:19.000000 bgen-1.6.5/src/genotypes.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1343 2024-05-01 18:59:19.000000 bgen-1.6.5/src/header.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      527 2024-05-01 18:59:19.000000 bgen-1.6.5/src/header.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3529 2024-05-01 18:59:19.000000 bgen-1.6.5/src/reader.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-05-01 18:59:19.000000 bgen-1.6.5/src/reader.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2303 2024-05-01 18:59:19.000000 bgen-1.6.5/src/samples.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-05-01 18:59:19.000000 bgen-1.6.5/src/samples.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6535 2024-05-01 18:59:19.000000 bgen-1.6.5/src/utils.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      527 2024-05-01 18:59:19.000000 bgen-1.6.5/src/utils.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4116 2024-05-01 18:59:19.000000 bgen-1.6.5/src/variant.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-01 18:59:19.000000 bgen-1.6.5/src/variant.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-05-01 18:59:19.000000 bgen-1.6.5/src/writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-01 18:59:19.000000 bgen-1.6.5/src/writer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.313150 bgen-1.6.5/src/zstd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.321150 bgen-1.6.5/src/zstd/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.325150 bgen-1.6.5/src/zstd/lib/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    18345 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/debug.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/debug.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/error_private.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33031 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/fse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19952 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/huf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/mem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/pool.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/pool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/threading.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/threading.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29099 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/zstd_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/zstd_errors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/common/zstd_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.329150 bgen-1.6.5/src/zstd/lib/compress/
+-rw-r--r--   0 runner    (1001) docker     (127)    27542 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/hist.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/hist.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32772 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)   172484 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    40937 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_compress_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_compress_literals.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_compress_literals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19037 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_compress_sequences.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_compress_sequences.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19166 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_cwksp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25278 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_double_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_double_fast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21936 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_fast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    51720 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_lazy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_lazy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_ldm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_ldm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57582 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_opt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstd_opt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    92625 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstdmt_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/compress/zstdmt_compress.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.329150 bgen-1.6.5/src/zstd/lib/decompress/
+-rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/decompress/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/decompress/zstd_ddict.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/decompress/zstd_ddict.h
+-rw-r--r--   0 runner    (1001) docker     (127)    72690 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/decompress/zstd_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    56849 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/decompress/zstd_decompress_block.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/decompress/zstd_decompress_block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/decompress/zstd_decompress_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.329150 bgen-1.6.5/src/zstd/lib/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/deprecated/zbuff.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/deprecated/zbuff_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/deprecated/zbuff_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/deprecated/zbuff_decompress.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.333150 bgen-1.6.5/src/zstd/lib/dictBuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    42155 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/dictBuilder/cover.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/dictBuilder/cover.h
+-rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/dictBuilder/divsufsort.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/dictBuilder/divsufsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28051 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/dictBuilder/fastcover.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43760 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/dictBuilder/zdict.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/dictBuilder/zdict.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:59:47.333150 bgen-1.6.5/src/zstd/lib/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_legacy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    71259 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v01.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v01.h
+-rw-r--r--   0 runner    (1001) docker     (127)   128019 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v02.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v02.h
+-rw-r--r--   0 runner    (1001) docker     (127)   114139 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v03.h
+-rw-r--r--   0 runner    (1001) docker     (127)   135210 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v04.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v04.h
+-rw-r--r--   0 runner    (1001) docker     (127)   156397 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v05.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v05.h
+-rw-r--r--   0 runner    (1001) docker     (127)   166025 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v06.h
+-rw-r--r--   0 runner    (1001) docker     (127)   185004 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v07.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/legacy/zstd_v07.h
+-rw-r--r--   0 runner    (1001) docker     (127)   119972 2024-05-01 18:59:22.000000 bgen-1.6.5/src/zstd/lib/zstd.h
```

### Comparing `bgen-1.6.4/LICENSE.txt` & `bgen-1.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/PKG-INFO` & `bgen-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgen
-Version: 1.6.4
+Version: 1.6.5
 Summary: Package for loading data from bgen files
 Home-page: https://github.com/jeremymcrae/bgen
 Author: Jeremy McRae
 Author-email: jmcrae@illumina.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `bgen-1.6.4/README.md` & `bgen-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/setup.py` & `bgen-1.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         language='c++'),
     ])
 
 setup(name='bgen',
     description='Package for loading data from bgen files',
     long_description=io.open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
-    version='1.6.4',
+    version='1.6.5',
     author='Jeremy McRae',
     author_email='jmcrae@illumina.com',
     license="MIT",
     url='https://github.com/jeremymcrae/bgen',
     packages=['bgen'],
     package_dir={'': 'src'},
     install_requires=[
```

### Comparing `bgen-1.6.4/src/bgen/index.py` & `bgen-1.6.5/src/bgen/index.py`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/bgen/reader.cpp` & `bgen-1.6.5/src/bgen/reader.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "src/header.h",
             "src/reader.h",
@@ -15,51 +15,51 @@
             "-I/usr/include",
             "-O2",
             "-mavx",
             "-mavx2"
         ],
         "extra_objects": [
             "src/zstd/lib/common/entropy_common.o",
-            "src/zstd/lib/common/debug.o",
-            "src/zstd/lib/common/error_private.o",
-            "src/zstd/lib/common/zstd_common.o",
-            "src/zstd/lib/common/fse_decompress.o",
             "src/zstd/lib/common/threading.o",
             "src/zstd/lib/common/xxhash.o",
+            "src/zstd/lib/common/zstd_common.o",
+            "src/zstd/lib/common/fse_decompress.o",
+            "src/zstd/lib/common/debug.o",
             "src/zstd/lib/common/pool.o",
-            "src/zstd/lib/compress/hist.o",
-            "src/zstd/lib/compress/zstd_compress_sequences.o",
+            "src/zstd/lib/common/error_private.o",
             "src/zstd/lib/compress/zstd_opt.o",
-            "src/zstd/lib/compress/zstd_double_fast.o",
             "src/zstd/lib/compress/fse_compress.o",
-            "src/zstd/lib/compress/zstd_ldm.o",
-            "src/zstd/lib/compress/zstd_fast.o",
+            "src/zstd/lib/compress/hist.o",
             "src/zstd/lib/compress/zstd_compress_literals.o",
-            "src/zstd/lib/compress/zstd_compress.o",
+            "src/zstd/lib/compress/huf_compress.o",
             "src/zstd/lib/compress/zstd_lazy.o",
             "src/zstd/lib/compress/zstdmt_compress.o",
-            "src/zstd/lib/compress/huf_compress.o",
-            "src/zstd/lib/decompress/zstd_decompress.o",
-            "src/zstd/lib/decompress/huf_decompress.o",
+            "src/zstd/lib/compress/zstd_double_fast.o",
+            "src/zstd/lib/compress/zstd_fast.o",
+            "src/zstd/lib/compress/zstd_ldm.o",
+            "src/zstd/lib/compress/zstd_compress_sequences.o",
+            "src/zstd/lib/compress/zstd_compress.o",
             "src/zstd/lib/decompress/zstd_decompress_block.o",
+            "src/zstd/lib/decompress/huf_decompress.o",
+            "src/zstd/lib/decompress/zstd_decompress.o",
             "src/zstd/lib/decompress/zstd_ddict.o",
+            "src/zstd/lib/dictBuilder/fastcover.o",
             "src/zstd/lib/dictBuilder/zdict.o",
             "src/zstd/lib/dictBuilder/divsufsort.o",
             "src/zstd/lib/dictBuilder/cover.o",
-            "src/zstd/lib/dictBuilder/fastcover.o",
             "src/zstd/lib/deprecated/zbuff_compress.o",
-            "src/zstd/lib/deprecated/zbuff_decompress.o",
             "src/zstd/lib/deprecated/zbuff_common.o",
+            "src/zstd/lib/deprecated/zbuff_decompress.o",
+            "src/zstd/lib/legacy/zstd_v04.o",
+            "src/zstd/lib/legacy/zstd_v07.o",
+            "src/zstd/lib/legacy/zstd_v01.o",
             "src/zstd/lib/legacy/zstd_v03.o",
             "src/zstd/lib/legacy/zstd_v06.o",
-            "src/zstd/lib/legacy/zstd_v07.o",
             "src/zstd/lib/legacy/zstd_v02.o",
-            "src/zstd/lib/legacy/zstd_v05.o",
-            "src/zstd/lib/legacy/zstd_v01.o",
-            "src/zstd/lib/legacy/zstd_v04.o"
+            "src/zstd/lib/legacy/zstd_v05.o"
         ],
         "include_dirs": [
             "src",
             "src/zstd/lib",
             "src/zlib"
         ],
         "language": "c++",
@@ -101,18 +101,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -196,14 +196,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -257,14 +259,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -318,60 +322,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -454,14 +481,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -26562,34 +26592,56 @@
  */
   }
 
   /* "bgen/reader.pyx":475
  *               self.thisptr.fsize)
  * 
  *       if not self.delay_parsing:             # <<<<<<<<<<<<<<
- *           idx = [i for i, x in enumerate(self.rsids) if x == rsid]
+ *           idx = [i for i, x in enumerate(self.rsids()) if x == rsid]
  *           if len(idx) == 0:
  */
   __pyx_t_1 = (!(__pyx_v_self->delay_parsing != 0));
   if (__pyx_t_1) {
 
     /* "bgen/reader.pyx":476
  * 
  *       if not self.delay_parsing:
- *           idx = [i for i, x in enumerate(self.rsids) if x == rsid]             # <<<<<<<<<<<<<<
+ *           idx = [i for i, x in enumerate(self.rsids()) if x == rsid]             # <<<<<<<<<<<<<<
  *           if len(idx) == 0:
  *               raise ValueError(f'cannot find variant match for {rsid}')
  */
     { /* enter inner scope */
       __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 476, __pyx_L8_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_int_0);
       __pyx_t_7 = __pyx_int_0;
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_rsids); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 476, __pyx_L8_error)
-      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_rsids); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 476, __pyx_L8_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_2 = NULL;
+      __pyx_t_5 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_2)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_2);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_5 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 476, __pyx_L8_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      }
       if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
         __pyx_t_3 = __pyx_t_4; __Pyx_INCREF(__pyx_t_3);
         __pyx_t_8 = 0;
         __pyx_t_9 = NULL;
       } else {
         __pyx_t_8 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 476, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_3);
@@ -26667,25 +26719,25 @@
       __pyx_L13_exit_scope:;
     } /* exit inner scope */
     __pyx_v_idx = ((PyObject*)__pyx_t_6);
     __pyx_t_6 = 0;
 
     /* "bgen/reader.pyx":477
  *       if not self.delay_parsing:
- *           idx = [i for i, x in enumerate(self.rsids) if x == rsid]
+ *           idx = [i for i, x in enumerate(self.rsids()) if x == rsid]
  *           if len(idx) == 0:             # <<<<<<<<<<<<<<
  *               raise ValueError(f'cannot find variant match for {rsid}')
  *           elif len(idx) > 1:
  */
     __pyx_t_8 = __Pyx_PyList_GET_SIZE(__pyx_v_idx); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 477, __pyx_L1_error)
     __pyx_t_1 = (__pyx_t_8 == 0);
     if (unlikely(__pyx_t_1)) {
 
       /* "bgen/reader.pyx":478
- *           idx = [i for i, x in enumerate(self.rsids) if x == rsid]
+ *           idx = [i for i, x in enumerate(self.rsids()) if x == rsid]
  *           if len(idx) == 0:
  *               raise ValueError(f'cannot find variant match for {rsid}')             # <<<<<<<<<<<<<<
  *           elif len(idx) > 1:
  *               raise ValueError(f'multiple variant matches for {rsid}')
  */
       __pyx_t_6 = __Pyx_PyObject_FormatSimple(__pyx_v_rsid, __pyx_empty_unicode); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 478, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
@@ -26697,15 +26749,15 @@
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(1, 478, __pyx_L1_error)
 
       /* "bgen/reader.pyx":477
  *       if not self.delay_parsing:
- *           idx = [i for i, x in enumerate(self.rsids) if x == rsid]
+ *           idx = [i for i, x in enumerate(self.rsids()) if x == rsid]
  *           if len(idx) == 0:             # <<<<<<<<<<<<<<
  *               raise ValueError(f'cannot find variant match for {rsid}')
  *           elif len(idx) > 1:
  */
     }
 
     /* "bgen/reader.pyx":479
@@ -26761,15 +26813,15 @@
     __pyx_t_6 = 0;
     goto __pyx_L0;
 
     /* "bgen/reader.pyx":475
  *               self.thisptr.fsize)
  * 
  *       if not self.delay_parsing:             # <<<<<<<<<<<<<<
- *           idx = [i for i, x in enumerate(self.rsids) if x == rsid]
+ *           idx = [i for i, x in enumerate(self.rsids()) if x == rsid]
  *           if len(idx) == 0:
  */
   }
 
   /* "bgen/reader.pyx":483
  *           return self[idx]
  * 
@@ -29631,24 +29683,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_4bgen_6reader___pyx_scope_struct__fetch *__pyx_freelist_4bgen_6reader___pyx_scope_struct__fetch[8];
 static int __pyx_freecount_4bgen_6reader___pyx_scope_struct__fetch = 0;
+#endif
 
 static PyObject *__pyx_tp_new_4bgen_6reader___pyx_scope_struct__fetch(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_4bgen_6reader___pyx_scope_struct__fetch > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_4bgen_6reader___pyx_scope_struct__fetch)))) {
     o = (PyObject*)__pyx_freelist_4bgen_6reader___pyx_scope_struct__fetch[--__pyx_freecount_4bgen_6reader___pyx_scope_struct__fetch];
     memset(o, 0, sizeof(struct __pyx_obj_4bgen_6reader___pyx_scope_struct__fetch));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -29672,15 +29726,15 @@
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_chrom);
   Py_CLEAR(p->__pyx_v_offset);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_start);
   Py_CLEAR(p->__pyx_v_stop);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_4bgen_6reader___pyx_scope_struct__fetch < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_4bgen_6reader___pyx_scope_struct__fetch)))) {
     __pyx_freelist_4bgen_6reader___pyx_scope_struct__fetch[__pyx_freecount_4bgen_6reader___pyx_scope_struct__fetch++] = ((struct __pyx_obj_4bgen_6reader___pyx_scope_struct__fetch *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
```

### Comparing `bgen-1.6.4/src/bgen/reader.pyx` & `bgen-1.6.5/src/bgen/reader.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,15 @@
       if self.index:
           offset = self.index.offset_by_rsid(rsid)
           return BgenVar(self.handle, offset, self.thisptr.header.layout,
               self.thisptr.header.compression, self.thisptr.header.nsamples,
               self.thisptr.fsize)
       
       if not self.delay_parsing:
-          idx = [i for i, x in enumerate(self.rsids) if x == rsid]
+          idx = [i for i, x in enumerate(self.rsids()) if x == rsid]
           if len(idx) == 0:
               raise ValueError(f'cannot find variant match for {rsid}')
           elif len(idx) > 1:
               raise ValueError(f'multiple variant matches for {rsid}')
           return self[idx]
       
       raise ValueError("can't get variant without fully loading the bgen, or indexing")
```

### Comparing `bgen-1.6.4/src/bgen/writer.cpp` & `bgen-1.6.5/src/bgen/writer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "src/genotypes.h",
             "src/writer.h"
@@ -12,51 +12,51 @@
             "-I/usr/include",
             "-O2",
             "-mavx",
             "-mavx2"
         ],
         "extra_objects": [
             "src/zstd/lib/common/entropy_common.o",
-            "src/zstd/lib/common/debug.o",
-            "src/zstd/lib/common/error_private.o",
-            "src/zstd/lib/common/zstd_common.o",
-            "src/zstd/lib/common/fse_decompress.o",
             "src/zstd/lib/common/threading.o",
             "src/zstd/lib/common/xxhash.o",
+            "src/zstd/lib/common/zstd_common.o",
+            "src/zstd/lib/common/fse_decompress.o",
+            "src/zstd/lib/common/debug.o",
             "src/zstd/lib/common/pool.o",
-            "src/zstd/lib/compress/hist.o",
-            "src/zstd/lib/compress/zstd_compress_sequences.o",
+            "src/zstd/lib/common/error_private.o",
             "src/zstd/lib/compress/zstd_opt.o",
-            "src/zstd/lib/compress/zstd_double_fast.o",
             "src/zstd/lib/compress/fse_compress.o",
-            "src/zstd/lib/compress/zstd_ldm.o",
-            "src/zstd/lib/compress/zstd_fast.o",
+            "src/zstd/lib/compress/hist.o",
             "src/zstd/lib/compress/zstd_compress_literals.o",
-            "src/zstd/lib/compress/zstd_compress.o",
+            "src/zstd/lib/compress/huf_compress.o",
             "src/zstd/lib/compress/zstd_lazy.o",
             "src/zstd/lib/compress/zstdmt_compress.o",
-            "src/zstd/lib/compress/huf_compress.o",
-            "src/zstd/lib/decompress/zstd_decompress.o",
-            "src/zstd/lib/decompress/huf_decompress.o",
+            "src/zstd/lib/compress/zstd_double_fast.o",
+            "src/zstd/lib/compress/zstd_fast.o",
+            "src/zstd/lib/compress/zstd_ldm.o",
+            "src/zstd/lib/compress/zstd_compress_sequences.o",
+            "src/zstd/lib/compress/zstd_compress.o",
             "src/zstd/lib/decompress/zstd_decompress_block.o",
+            "src/zstd/lib/decompress/huf_decompress.o",
+            "src/zstd/lib/decompress/zstd_decompress.o",
             "src/zstd/lib/decompress/zstd_ddict.o",
+            "src/zstd/lib/dictBuilder/fastcover.o",
             "src/zstd/lib/dictBuilder/zdict.o",
             "src/zstd/lib/dictBuilder/divsufsort.o",
             "src/zstd/lib/dictBuilder/cover.o",
-            "src/zstd/lib/dictBuilder/fastcover.o",
             "src/zstd/lib/deprecated/zbuff_compress.o",
-            "src/zstd/lib/deprecated/zbuff_decompress.o",
             "src/zstd/lib/deprecated/zbuff_common.o",
+            "src/zstd/lib/deprecated/zbuff_decompress.o",
+            "src/zstd/lib/legacy/zstd_v04.o",
+            "src/zstd/lib/legacy/zstd_v07.o",
+            "src/zstd/lib/legacy/zstd_v01.o",
             "src/zstd/lib/legacy/zstd_v03.o",
             "src/zstd/lib/legacy/zstd_v06.o",
-            "src/zstd/lib/legacy/zstd_v07.o",
             "src/zstd/lib/legacy/zstd_v02.o",
-            "src/zstd/lib/legacy/zstd_v05.o",
-            "src/zstd/lib/legacy/zstd_v01.o",
-            "src/zstd/lib/legacy/zstd_v04.o"
+            "src/zstd/lib/legacy/zstd_v05.o"
         ],
         "include_dirs": [
             "src",
             "src/zstd/lib",
             "src/zlib"
         ],
         "language": "c++",
@@ -95,18 +95,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -190,14 +190,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -251,14 +253,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -312,60 +316,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -448,14 +475,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -19007,15 +19037,15 @@
   return __pyx_r;
 }
 
 /* "bgen/writer.pyx":55
  *     ''' class to automatically index bgen files as they are being constructed
  *     '''
  *     def __init__(self, bgen_path):             # <<<<<<<<<<<<<<
- *         index_path = Path(str(bgen_path + '.bgi'))
+ *         index_path = Path(str(bgen_path) + '.bgi')
  *         if index_path.exists():
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4bgen_6writer_7Indexer_1__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -19140,23 +19170,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
   /* "bgen/writer.pyx":56
  *     '''
  *     def __init__(self, bgen_path):
- *         index_path = Path(str(bgen_path + '.bgi'))             # <<<<<<<<<<<<<<
+ *         index_path = Path(str(bgen_path) + '.bgi')             # <<<<<<<<<<<<<<
  *         if index_path.exists():
  *             index_path.unlink()
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Path); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Add(__pyx_v_bgen_path, __pyx_kp_u_bgi); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Str(__pyx_v_bgen_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_kp_u_bgi); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -19179,15 +19209,15 @@
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_index_path = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "bgen/writer.pyx":57
  *     def __init__(self, bgen_path):
- *         index_path = Path(str(bgen_path + '.bgi'))
+ *         index_path = Path(str(bgen_path) + '.bgi')
  *         if index_path.exists():             # <<<<<<<<<<<<<<
  *             index_path.unlink()
  *         self.conn = sqlite3.connect(index_path)
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_path, __pyx_n_s_exists); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
@@ -19213,15 +19243,15 @@
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
 
     /* "bgen/writer.pyx":58
- *         index_path = Path(str(bgen_path + '.bgi'))
+ *         index_path = Path(str(bgen_path) + '.bgi')
  *         if index_path.exists():
  *             index_path.unlink()             # <<<<<<<<<<<<<<
  *         self.conn = sqlite3.connect(index_path)
  *         self.cur = self.conn.cursor()
  */
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_index_path, __pyx_n_s_unlink); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
@@ -19247,15 +19277,15 @@
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "bgen/writer.pyx":57
  *     def __init__(self, bgen_path):
- *         index_path = Path(str(bgen_path + '.bgi'))
+ *         index_path = Path(str(bgen_path) + '.bgi')
  *         if index_path.exists():             # <<<<<<<<<<<<<<
  *             index_path.unlink()
  *         self.conn = sqlite3.connect(index_path)
  */
   }
 
   /* "bgen/writer.pyx":59
@@ -19365,15 +19395,15 @@
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "bgen/writer.pyx":55
  *     ''' class to automatically index bgen files as they are being constructed
  *     '''
  *     def __init__(self, bgen_path):             # <<<<<<<<<<<<<<
- *         index_path = Path(str(bgen_path + '.bgi'))
+ *         index_path = Path(str(bgen_path) + '.bgi')
  *         if index_path.exists():
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -24868,15 +24898,15 @@
   __Pyx_GIVEREF(__pyx_tuple__23);
   __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "bgen/writer.pyx":55
  *     ''' class to automatically index bgen files as they are being constructed
  *     '''
  *     def __init__(self, bgen_path):             # <<<<<<<<<<<<<<
- *         index_path = Path(str(bgen_path + '.bgi'))
+ *         index_path = Path(str(bgen_path) + '.bgi')
  *         if index_path.exists():
  */
   __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_bgen_path, __pyx_n_s_index_path); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
   __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_bgen_writer_pyx, __pyx_n_s_init, 55, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 55, __pyx_L1_error)
 
@@ -26157,15 +26187,15 @@
   __pyx_t_4 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Indexer, __pyx_n_s_Indexer, (PyObject *) NULL, __pyx_n_s_bgen_writer, __pyx_kp_s_class_to_automatically_index_bg); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
   /* "bgen/writer.pyx":55
  *     ''' class to automatically index bgen files as they are being constructed
  *     '''
  *     def __init__(self, bgen_path):             # <<<<<<<<<<<<<<
- *         index_path = Path(str(bgen_path + '.bgi'))
+ *         index_path = Path(str(bgen_path) + '.bgi')
  *         if index_path.exists():
  */
   __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4bgen_6writer_7Indexer_1__init__, 0, __pyx_n_s_Indexer___init, NULL, __pyx_n_s_bgen_writer, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_init, __pyx_t_7) < 0) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
```

### Comparing `bgen-1.6.4/src/bgen/writer.pyx` & `bgen-1.6.5/src/bgen/writer.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                          uint32_t min_ploidy, uint32_t max_ploidy,
                          bool phased, uint8_t bit_depth) except +
 
 class Indexer:
     ''' class to automatically index bgen files as they are being constructed
     '''
     def __init__(self, bgen_path):
-        index_path = Path(str(bgen_path + '.bgi'))
+        index_path = Path(str(bgen_path) + '.bgi')
         if index_path.exists():
             index_path.unlink()
         self.conn = sqlite3.connect(index_path)
         self.cur = self.conn.cursor()
         self.create_tables()
     
     def create_tables(self):
```

### Comparing `bgen-1.6.4/src/bgen.egg-info/PKG-INFO` & `bgen-1.6.5/src/bgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgen
-Version: 1.6.4
+Version: 1.6.5
 Summary: Package for loading data from bgen files
 Home-page: https://github.com/jeremymcrae/bgen
 Author: Jeremy McRae
 Author-email: jmcrae@illumina.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `bgen-1.6.4/src/bgen.egg-info/SOURCES.txt` & `bgen-1.6.5/src/bgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/genotypes.cpp` & `bgen-1.6.5/src/genotypes.cpp`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/genotypes.h` & `bgen-1.6.5/src/genotypes.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/header.cpp` & `bgen-1.6.5/src/header.cpp`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/header.h` & `bgen-1.6.5/src/header.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/reader.cpp` & `bgen-1.6.5/src/reader.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,17 @@
   Variant var(&handle, offset, header.layout, header.compression, header.nsamples, fsize);
   offset = var.next_variant_offset;
   return var;
 }
 
 /// load all variants into memory at once
 void CppBgenReader::parse_all_variants() {
+  if (variants.size() == header.nvariants) {
+    return;
+  }
   offset = header.offset + 4;
   variants.clear();
   variants.resize(header.nvariants);
   int idx = 0;
   while (true) {
     try {
       variants[idx] = next_var();
@@ -75,41 +78,45 @@
   // and sort the variants again afterward
   std::sort(variants.begin(), variants.end(),
           [] (Variant const& a, Variant const& b) { return a.pos < b.pos; });
 }
 
 /// get all the IDs for the variants in the bgen file
 std::vector<std::string> CppBgenReader::varids() {
+  parse_all_variants();
   std::vector<std::string> varid(variants.size());
   for (std::uint32_t x=0; x<variants.size(); x++) {
     varid[x] = variants[x].varid;
   }
   return varid;
 }
 
 /// get all the rsIDs for the variants in the bgen file
 std::vector<std::string> CppBgenReader::rsids() {
+  parse_all_variants();
   std::vector<std::string> rsid(variants.size());
   for (std::uint32_t x=0; x<variants.size(); x++) {
     rsid[x] = variants[x].rsid;
   }
   return rsid;
 }
 
 /// get all the chroms for the variants in the bgen file
 std::vector<std::string> CppBgenReader::chroms() {
+  parse_all_variants();
   std::vector<std::string> chrom(variants.size());
   for (std::uint32_t x=0; x<variants.size(); x++) {
     chrom[x] = variants[x].chrom;
   }
   return chrom;
 }
 
 /// get all the positions for the variants in the bgen file
 std::vector<std::uint32_t> CppBgenReader::positions() {
+  parse_all_variants();
   std::vector<std::uint32_t> position(variants.size());
   for (std::uint32_t x=0; x<variants.size(); x++) {
     position[x] = variants[x].pos;
   }
   return position;
 }
```

### Comparing `bgen-1.6.4/src/reader.h` & `bgen-1.6.5/src/reader.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/samples.cpp` & `bgen-1.6.5/src/samples.cpp`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/utils.cpp` & `bgen-1.6.5/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/utils.h` & `bgen-1.6.5/src/utils.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/variant.cpp` & `bgen-1.6.5/src/variant.cpp`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/variant.h` & `bgen-1.6.5/src/variant.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/writer.cpp` & `bgen-1.6.5/src/writer.cpp`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/writer.h` & `bgen-1.6.5/src/writer.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/bitstream.h` & `bgen-1.6.5/src/zstd/lib/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/compiler.h` & `bgen-1.6.5/src/zstd/lib/common/compiler.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/cpu.h` & `bgen-1.6.5/src/zstd/lib/common/cpu.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/debug.c` & `bgen-1.6.5/src/zstd/lib/common/debug.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/debug.h` & `bgen-1.6.5/src/zstd/lib/common/debug.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/entropy_common.c` & `bgen-1.6.5/src/zstd/lib/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/error_private.c` & `bgen-1.6.5/src/zstd/lib/common/error_private.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/error_private.h` & `bgen-1.6.5/src/zstd/lib/common/error_private.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/fse.h` & `bgen-1.6.5/src/zstd/lib/common/fse.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/fse_decompress.c` & `bgen-1.6.5/src/zstd/lib/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/huf.h` & `bgen-1.6.5/src/zstd/lib/common/huf.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/mem.h` & `bgen-1.6.5/src/zstd/lib/common/mem.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/pool.c` & `bgen-1.6.5/src/zstd/lib/common/pool.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/pool.h` & `bgen-1.6.5/src/zstd/lib/common/pool.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/threading.c` & `bgen-1.6.5/src/zstd/lib/common/threading.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/threading.h` & `bgen-1.6.5/src/zstd/lib/common/threading.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/xxhash.c` & `bgen-1.6.5/src/zstd/lib/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/xxhash.h` & `bgen-1.6.5/src/zstd/lib/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/zstd_common.c` & `bgen-1.6.5/src/zstd/lib/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/zstd_errors.h` & `bgen-1.6.5/src/zstd/lib/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/common/zstd_internal.h` & `bgen-1.6.5/src/zstd/lib/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/fse_compress.c` & `bgen-1.6.5/src/zstd/lib/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/hist.c` & `bgen-1.6.5/src/zstd/lib/compress/hist.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/hist.h` & `bgen-1.6.5/src/zstd/lib/compress/hist.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/huf_compress.c` & `bgen-1.6.5/src/zstd/lib/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_compress.c` & `bgen-1.6.5/src/zstd/lib/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_compress_internal.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_compress_literals.c` & `bgen-1.6.5/src/zstd/lib/compress/zstd_compress_literals.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_compress_literals.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_compress_literals.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_compress_sequences.c` & `bgen-1.6.5/src/zstd/lib/compress/zstd_compress_sequences.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_compress_sequences.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_compress_sequences.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_cwksp.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_cwksp.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_double_fast.c` & `bgen-1.6.5/src/zstd/lib/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_double_fast.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_fast.c` & `bgen-1.6.5/src/zstd/lib/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_fast.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_lazy.c` & `bgen-1.6.5/src/zstd/lib/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_lazy.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_ldm.c` & `bgen-1.6.5/src/zstd/lib/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_ldm.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_opt.c` & `bgen-1.6.5/src/zstd/lib/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstd_opt.h` & `bgen-1.6.5/src/zstd/lib/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstdmt_compress.c` & `bgen-1.6.5/src/zstd/lib/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/compress/zstdmt_compress.h` & `bgen-1.6.5/src/zstd/lib/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/decompress/huf_decompress.c` & `bgen-1.6.5/src/zstd/lib/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/decompress/zstd_ddict.c` & `bgen-1.6.5/src/zstd/lib/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/decompress/zstd_ddict.h` & `bgen-1.6.5/src/zstd/lib/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/decompress/zstd_decompress.c` & `bgen-1.6.5/src/zstd/lib/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/decompress/zstd_decompress_block.c` & `bgen-1.6.5/src/zstd/lib/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/decompress/zstd_decompress_block.h` & `bgen-1.6.5/src/zstd/lib/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/decompress/zstd_decompress_internal.h` & `bgen-1.6.5/src/zstd/lib/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/deprecated/zbuff.h` & `bgen-1.6.5/src/zstd/lib/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/deprecated/zbuff_common.c` & `bgen-1.6.5/src/zstd/lib/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/deprecated/zbuff_compress.c` & `bgen-1.6.5/src/zstd/lib/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/deprecated/zbuff_decompress.c` & `bgen-1.6.5/src/zstd/lib/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/dictBuilder/cover.c` & `bgen-1.6.5/src/zstd/lib/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/dictBuilder/cover.h` & `bgen-1.6.5/src/zstd/lib/dictBuilder/cover.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/dictBuilder/divsufsort.c` & `bgen-1.6.5/src/zstd/lib/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/dictBuilder/divsufsort.h` & `bgen-1.6.5/src/zstd/lib/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/dictBuilder/fastcover.c` & `bgen-1.6.5/src/zstd/lib/dictBuilder/fastcover.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/dictBuilder/zdict.c` & `bgen-1.6.5/src/zstd/lib/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/dictBuilder/zdict.h` & `bgen-1.6.5/src/zstd/lib/dictBuilder/zdict.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_legacy.h` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v01.c` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v01.h` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v02.c` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v02.h` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v03.c` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v03.h` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v04.c` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v04.h` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v05.c` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v05.h` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v06.c` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v06.h` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v07.c` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/legacy/zstd_v07.h` & `bgen-1.6.5/src/zstd/lib/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `bgen-1.6.4/src/zstd/lib/zstd.h` & `bgen-1.6.5/src/zstd/lib/zstd.h`

 * *Files identical despite different names*


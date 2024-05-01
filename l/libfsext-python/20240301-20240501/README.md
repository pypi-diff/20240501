# Comparing `tmp/libfsext-python-20240301.tar.gz` & `tmp/libfsext-python-20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfsext-python-20240301.tar", last modified: Sat Mar  2 14:06:27 2024, max compression
+gzip compressed data, was "libfsext-python-20240501.tar", last modified: Wed May  1 05:52:27 2024, max compression
```

## Comparing `libfsext-python-20240301.tar` & `libfsext-python-20240501.tar`

### file list

```diff
@@ -1,914 +1,914 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:26.000000 libfsext-20240301/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:24.000000 libfsext-20240301/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33624 2024-03-02 13:26:29.000000 libfsext-20240301/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-03-02 13:26:10.000000 libfsext-20240301/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-01 12:22:51.000000 libfsext-20240301/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-02 13:26:28.000000 libfsext-20240301/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-01 12:22:51.000000 libfsext-20240301/NEWS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2443 2024-03-02 13:26:46.000000 libfsext-20240301/libfsext.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-02 13:26:29.000000 libfsext-20240301/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:24.000000 libfsext-20240301/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29839 2024-03-02 13:26:29.000000 libfsext-20240301/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 13:26:13.000000 libfsext-20240301/libfguid/libfguid_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      712 2024-03-01 12:22:51.000000 libfsext-20240301/libfsext.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:21.000000 libfsext-20240301/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:06:33.000000 libfsext-20240301/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:06:32.000000 libfsext-20240301/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:06:32.000000 libfsext-20240301/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:06:32.000000 libfsext-20240301/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30359 2023-12-03 09:06:33.000000 libfsext-20240301/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:06:32.000000 libfsext-20240301/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:06:32.000000 libfsext-20240301/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:06:32.000000 libfsext-20240301/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:06:33.000000 libfsext-20240301/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-02 13:26:23.000000 libfsext-20240301/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-02 13:26:23.000000 libfsext-20240301/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:06:33.000000 libfsext-20240301/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:06:32.000000 libfsext-20240301/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:06:33.000000 libfsext-20240301/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-02 13:26:22.000000 libfsext-20240301/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:06:32.000000 libfsext-20240301/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:06:33.000000 libfsext-20240301/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:06:32.000000 libfsext-20240301/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-02 13:26:23.000000 libfsext-20240301/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:06:32.000000 libfsext-20240301/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:06:32.000000 libfsext-20240301/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-02 13:26:22.000000 libfsext-20240301/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:06:32.000000 libfsext-20240301/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:06:32.000000 libfsext-20240301/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 09:06:32.000000 libfsext-20240301/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:06:33.000000 libfsext-20240301/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:06:33.000000 libfsext-20240301/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:06:33.000000 libfsext-20240301/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:22.000000 libfsext-20240301/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      474 2024-03-01 12:22:51.000000 libfsext-20240301/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30141 2024-03-01 12:22:54.000000 libfsext-20240301/include/libfsext.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:22.000000 libfsext-20240301/include/libfsext/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2220 2024-03-01 12:22:54.000000 libfsext-20240301/include/libfsext/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2218 2024-03-02 13:26:46.000000 libfsext-20240301/include/libfsext/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5032 2024-03-01 12:22:54.000000 libfsext-20240301/include/libfsext/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4901 2024-03-02 13:26:46.000000 libfsext-20240301/include/libfsext/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-01 12:22:54.000000 libfsext-20240301/include/libfsext/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-03-01 12:22:54.000000 libfsext-20240301/include/libfsext/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-01 12:22:54.000000 libfsext-20240301/include/libfsext/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-03-02 13:26:46.000000 libfsext-20240301/include/libfsext/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-03-01 12:22:54.000000 libfsext-20240301/include/libfsext/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28385 2024-03-02 13:26:28.000000 libfsext-20240301/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30141 2024-03-02 13:26:46.000000 libfsext-20240301/include/libfsext.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:22.000000 libfsext-20240301/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-01 12:22:54.000000 libfsext-20240301/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-01 12:22:54.000000 libfsext-20240301/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-01 12:22:54.000000 libfsext-20240301/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-01 12:22:54.000000 libfsext-20240301/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-01 12:22:54.000000 libfsext-20240301/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-01 12:22:54.000000 libfsext-20240301/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-01 12:22:54.000000 libfsext-20240301/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-01 12:22:51.000000 libfsext-20240301/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-01 12:22:54.000000 libfsext-20240301/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-03-02 13:26:46.000000 libfsext-20240301/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17849 2024-03-02 13:26:28.000000 libfsext-20240301/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18894 2024-03-02 13:26:46.000000 libfsext-20240301/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-01 12:22:54.000000 libfsext-20240301/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-01 12:22:54.000000 libfsext-20240301/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-01 12:22:54.000000 libfsext-20240301/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25392 2024-03-02 13:26:28.000000 libfsext-20240301/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:22.000000 libfsext-20240301/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30395 2024-03-02 13:26:29.000000 libfsext-20240301/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-02 13:26:02.000000 libfsext-20240301/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:24.000000 libfsext-20240301/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30868 2024-03-02 13:26:29.000000 libfsext-20240301/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-03-02 13:26:09.000000 libfsext-20240301/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2303 2023-12-03 09:06:05.000000 libfsext-20240301/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:24.000000 libfsext-20240301/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33854 2024-03-02 13:26:28.000000 libfsext-20240301/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-03-02 13:25:57.000000 libfsext-20240301/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:06:05.000000 libfsext-20240301/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-02 13:26:28.000000 libfsext-20240301/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:21.000000 libfsext-20240301/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/libfsext-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-03-01 12:22:57.000000 libfsext-20240301/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:21.000000 libfsext-20240301/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2147 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-03-02 13:26:46.000000 libfsext-20240301/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/libfsext-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/libfsext.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-03-01 12:22:51.000000 libfsext-20240301/dpkg/libfsext-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-03-02 13:26:46.000000 libfsext-20240301/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-01 12:22:51.000000 libfsext-20240301/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1974914 2024-03-02 13:26:27.000000 libfsext-20240301/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-02 13:26:28.000000 libfsext-20240301/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-02 13:26:28.000000 libfsext-20240301/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsextinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7282 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsextinfo/fsextinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5732 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_notify/fsext_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsextmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7669 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsextmount/fsextmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_attribute_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5924 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_attribute_values/fsext_test_attribute_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_superblock/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6322 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_superblock/fsext_test_superblock.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5645 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_error/fsext_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_bitmap/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_bitmap/fsext_test_bitmap.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_block_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6343 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_block_data_handle/fsext_test_block_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_extent/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5894 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_extent/fsext_test_extent.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_inode_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5909 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_inode_table/fsext_test_inode_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6164 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_tools_info_handle/fsext_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2207 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_extents_footer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5918 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_extents_footer/fsext_test_extents_footer.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_inode/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5891 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_inode/fsext_test_inode.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_directory_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5921 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_directory_entry/fsext_test_directory_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6307 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_block/fsext_test_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/pyfsext/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6871 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/pyfsext/pyfsext.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5903 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_io_handle/fsext_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_directory/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6319 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_directory/fsext_test_directory.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_tools_signal/fsext_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_extended_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_extended_attribute/fsext_test_extended_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_extent_index/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5912 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_extent_index/fsext_test_extent_index.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6557 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_volume/fsext_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_block_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6495 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_block_vector/fsext_test_block_vector.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44724 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libfsext.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_buffer_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_buffer_data_handle/fsext_test_buffer_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_tools_output/fsext_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_file_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5906 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_file_entry/fsext_test_file_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_group_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6340 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_group_descriptor/fsext_test_group_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libfsext/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12069 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libfsext/libfsext.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_extents_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5918 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_extents_header/fsext_test_extents_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_checksum/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5657 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_checksum/fsext_test_checksum.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/fsext_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6560 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/fsext_test_support/fsext_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24567 2024-03-02 13:26:29.000000 libfsext-20240301/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:27.000000 libfsext-20240301/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-03-02 08:06:55.000000 libfsext-20240301/msvscpp/libfdatetime/libfdatetime.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-03-01 12:22:54.000000 libfsext-20240301/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:23.000000 libfsext-20240301/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31159 2024-03-02 13:26:29.000000 libfsext-20240301/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-03-02 13:26:01.000000 libfsext-20240301/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      546 2024-03-01 12:23:44.000000 libfsext-20240301/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:25.000000 libfsext-20240301/pyfsext/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3525 2024-03-01 12:23:58.000000 libfsext-20240301/pyfsext/pyfsext_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7362 2024-03-01 12:23:58.000000 libfsext-20240301/pyfsext/pyfsext_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3486 2024-03-01 12:23:58.000000 libfsext-20240301/pyfsext/pyfsext_extended_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2023-12-03 09:06:33.000000 libfsext-20240301/pyfsext/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_libfsext.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2634 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_extended_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28440 2024-03-01 12:23:58.000000 libfsext-20240301/pyfsext/pyfsext_extended_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_file_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15994 2024-03-01 12:23:58.000000 libfsext-20240301/pyfsext/pyfsext.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76680 2024-03-01 12:23:58.000000 libfsext-20240301/pyfsext/pyfsext_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47874 2024-03-02 13:26:29.000000 libfsext-20240301/pyfsext/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9890 2024-03-01 12:23:58.000000 libfsext-20240301/pyfsext/pyfsext_extended_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34943 2024-03-01 12:23:58.000000 libfsext-20240301/pyfsext/pyfsext_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9439 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_file_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-03-01 12:22:56.000000 libfsext-20240301/pyfsext/pyfsext_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-02 13:26:28.000000 libfsext-20240301/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:22.000000 libfsext-20240301/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32843 2024-03-02 13:26:28.000000 libfsext-20240301/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 13:25:58.000000 libfsext-20240301/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-01 12:22:51.000000 libfsext-20240301/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-03-01 12:22:51.000000 libfsext-20240301/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-02 13:26:28.000000 libfsext-20240301/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-01 12:22:51.000000 libfsext-20240301/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-03-01 12:22:51.000000 libfsext-20240301/acinclude.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:25.000000 libfsext-20240301/fsexttools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36321 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3061 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37913 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4994 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3297 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/digest_hash.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30757 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4361 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1590 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2023-12-03 09:06:31.000000 libfsext-20240301/fsexttools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22158 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    80949 2024-03-02 11:35:17.000000 libfsext-20240301/fsexttools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3661 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15493 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/fsextmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10875 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/fsextinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3324 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19354 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libfsext.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34985 2024-03-02 13:26:28.000000 libfsext-20240301/fsexttools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1244 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/digest_hash.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2024-03-01 12:22:56.000000 libfsext-20240301/fsexttools/fsexttools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3050 2024-03-01 12:23:58.000000 libfsext-20240301/fsexttools/mount_fuse.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:06:05.000000 libfsext-20240301/config.rpath
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3488 2024-03-01 12:22:51.000000 libfsext-20240301/libfsext.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:22.000000 libfsext-20240301/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33249 2024-03-02 13:26:29.000000 libfsext-20240301/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-02 13:26:08.000000 libfsext-20240301/libcthreads/libcthreads_queue.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:25.000000 libfsext-20240301/libfsext/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8529 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_bitmap.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_block_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2179 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_inode_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12002 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1799 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_bitmap.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10228 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extent.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7821 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17086 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_attribute_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1819 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_attributes_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24275 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_directory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7795 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1670 2024-03-02 08:04:55.000000 libfsext-20240301/libfsext/libfsext_checksum.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2740 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_group_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_block_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1089 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19758 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_group_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2695 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/fsext_extents.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3193 2024-03-02 07:52:13.000000 libfsext-20240301/libfsext/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6039 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extent_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3103 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_attribute_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14856 2024-03-02 11:48:44.000000 libfsext-20240301/libfsext/fsext_superblock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22186 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_data_blocks.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2024-03-02 08:26:52.000000 libfsext-20240301/libfsext/libfsext_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2125 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extent.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4899 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_block_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2233 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_data_blocks.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4774 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extents_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9425 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6407 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extents_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3001 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_directory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18271 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extent_index.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36220 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extended_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extents_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   120345 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52454 2024-03-02 12:38:10.000000 libfsext-20240301/libfsext/libfsext_superblock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8391 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_block_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3812 2024-03-02 13:26:46.000000 libfsext-20240301/libfsext/libfsext_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1832 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   103891 2024-03-02 13:04:03.000000 libfsext-20240301/libfsext/libfsext_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66405 2024-03-02 13:09:07.000000 libfsext-20240301/libfsext/libfsext_inode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_block_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2709 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/fsext_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2195 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extents.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6994 2024-03-02 11:47:47.000000 libfsext-20240301/libfsext/libfsext_superblock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2202 2024-03-02 11:48:03.000000 libfsext-20240301/libfsext/libfsext_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10968 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_block_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extended_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8716 2024-03-02 12:06:13.000000 libfsext-20240301/libfsext/fsext_inode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18929 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extents.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23037 2024-03-02 11:35:42.000000 libfsext-20240301/libfsext/libfsext_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3814 2024-03-02 11:46:14.000000 libfsext-20240301/libfsext/libfsext_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4711 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/fsext_group_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40370 2024-03-02 13:26:29.000000 libfsext-20240301/libfsext/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6042 2024-03-02 11:57:20.000000 libfsext-20240301/libfsext/libfsext_inode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_buffer_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2024-03-02 13:26:46.000000 libfsext-20240301/libfsext/libfsext.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14079 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_attributes_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2868 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10147 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_inode_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/fsext_directory_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1659 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_extents_footer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1879 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3299 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_directory_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3804 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5241 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-01 12:22:55.000000 libfsext-20240301/libfsext/libfsext_unused.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-02 13:26:29.000000 libfsext-20240301/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:24.000000 libfsext-20240301/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30437 2024-03-02 13:26:29.000000 libfsext-20240301/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-03-02 13:26:05.000000 libfsext-20240301/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1058 2024-03-01 13:58:36.000000 libfsext-20240301/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:26.000000 libfsext-20240301/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3235 2024-03-01 12:22:57.000000 libfsext-20240301/manuals/fsextinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      190 2023-12-03 09:06:33.000000 libfsext-20240301/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2024-03-01 12:22:57.000000 libfsext-20240301/manuals/fsextmount.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27394 2024-03-02 13:26:29.000000 libfsext-20240301/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14808 2024-03-01 12:22:57.000000 libfsext-20240301/manuals/libfsext.3
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:26.000000 libfsext-20240301/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_libfsext.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9650 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_extents_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21176 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_attribute_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16235 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4261 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2663 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_inode_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4275 2024-03-02 08:28:19.000000 libfsext-20240301/tests/fsext_test_checksum.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4076 2024-03-01 12:23:58.000000 libfsext-20240301/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15297 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16666 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_block_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15726 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22091 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_superblock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24871 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12428 2024-03-02 08:06:37.000000 libfsext-20240301/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4052 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_extended_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38388 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6551 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_group_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11536 2024-03-01 12:23:58.000000 libfsext-20240301/tests/pyfsext_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41056 2024-03-02 11:58:48.000000 libfsext-20240301/tests/fsext_test_inode.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-01 12:22:57.000000 libfsext-20240301/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4086 2024-03-01 12:22:57.000000 libfsext-20240301/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6297 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_extents_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20513 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_bitmap.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_extent_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32914 2024-03-02 11:59:38.000000 libfsext-20240301/tests/fsext_test_directory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1997 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-01 12:22:57.000000 libfsext-20240301/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13376 2024-03-01 12:23:44.000000 libfsext-20240301/tests/fsext_test_extent.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20898 2024-03-02 11:59:20.000000 libfsext-20240301/tests/fsext_test_block_vector.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3348 2024-03-01 12:22:57.000000 libfsext-20240301/tests/test_fsextinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    79024 2024-03-02 13:26:29.000000 libfsext-20240301/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5706 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2800 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3464 2024-03-01 12:23:58.000000 libfsext-20240301/tests/pyfsext_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-01 12:22:57.000000 libfsext-20240301/tests/fsext_test_unused.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4326 2024-03-02 08:06:46.000000 libfsext-20240301/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:26.000000 libfsext-20240301/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3661 2024-03-01 12:22:56.000000 libfsext-20240301/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2024 2023-12-03 09:06:06.000000 libfsext-20240301/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-03-01 12:22:56.000000 libfsext-20240301/ossfuzz/ossfuzz_libfsext.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-03-01 12:22:56.000000 libfsext-20240301/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5555 2024-03-01 12:22:56.000000 libfsext-20240301/ossfuzz/file_entry_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-03-01 12:22:56.000000 libfsext-20240301/ossfuzz/extended_attribute_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36747 2024-03-02 13:26:29.000000 libfsext-20240301/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-02 13:26:22.000000 libfsext-20240301/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:25.000000 libfsext-20240301/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32969 2024-03-02 13:26:29.000000 libfsext-20240301/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-03-02 13:26:14.000000 libfsext-20240301/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:23.000000 libfsext-20240301/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31217 2024-03-02 13:26:29.000000 libfsext-20240301/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-03-02 13:26:06.000000 libfsext-20240301/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:26.000000 libfsext-20240301/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:06:33.000000 libfsext-20240301/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:06:33.000000 libfsext-20240301/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:06:33.000000 libfsext-20240301/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:06:33.000000 libfsext-20240301/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:06:33.000000 libfsext-20240301/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:06:33.000000 libfsext-20240301/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:06:33.000000 libfsext-20240301/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:06:33.000000 libfsext-20240301/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:06:33.000000 libfsext-20240301/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-03-02 13:26:46.000000 libfsext-20240301/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:06:33.000000 libfsext-20240301/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:06:33.000000 libfsext-20240301/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:23.000000 libfsext-20240301/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53961 2024-03-02 13:26:29.000000 libfsext-20240301/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-02 13:26:17.000000 libfsext-20240301/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41467 2024-03-02 13:26:28.000000 libfsext-20240301/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:22.000000 libfsext-20240301/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30271 2024-03-02 13:26:29.000000 libfsext-20240301/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-02 13:26:04.000000 libfsext-20240301/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:22.000000 libfsext-20240301/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-02 13:26:00.000000 libfsext-20240301/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-02 13:26:00.000000 libfsext-20240301/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-02 13:25:59.000000 libfsext-20240301/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29784 2024-03-02 13:26:28.000000 libfsext-20240301/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-02 14:06:24.000000 libfsext-20240301/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33010 2024-03-02 13:26:29.000000 libfsext-20240301/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-03-02 13:26:12.000000 libfsext-20240301/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56884 2024-03-02 13:26:25.000000 libfsext-20240301/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8065 2024-03-01 12:22:51.000000 libfsext-20240301/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-03-02 14:06:27.845226 libfsext-20240301/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34244 2024-05-01 04:28:17.000000 libfsext-20240501/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-01 04:27:57.000000 libfsext-20240501/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-01 03:55:41.000000 libfsext-20240501/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-01 04:28:17.000000 libfsext-20240501/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 03:55:41.000000 libfsext-20240501/NEWS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2445 2024-05-01 04:28:38.000000 libfsext-20240501/libfsext.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-01 04:28:17.000000 libfsext-20240501/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30045 2024-05-01 04:28:17.000000 libfsext-20240501/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 04:27:59.000000 libfsext-20240501/libfguid/libfguid_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      712 2024-05-01 03:55:41.000000 libfsext-20240501/libfsext.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:23.000000 libfsext-20240501/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:06:32.000000 libfsext-20240501/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:06:32.000000 libfsext-20240501/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:06:32.000000 libfsext-20240501/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:06:32.000000 libfsext-20240501/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:06:32.000000 libfsext-20240501/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-01 03:55:49.000000 libfsext-20240501/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-01 04:28:11.000000 libfsext-20240501/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-01 04:28:11.000000 libfsext-20240501/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:06:32.000000 libfsext-20240501/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-01 04:28:10.000000 libfsext-20240501/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:06:32.000000 libfsext-20240501/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:06:32.000000 libfsext-20240501/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-01 04:28:11.000000 libfsext-20240501/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:06:32.000000 libfsext-20240501/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:06:32.000000 libfsext-20240501/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-01 04:28:10.000000 libfsext-20240501/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:06:32.000000 libfsext-20240501/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-01 03:55:49.000000 libfsext-20240501/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:06:33.000000 libfsext-20240501/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-01 03:55:49.000000 libfsext-20240501/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-01 03:55:49.000000 libfsext-20240501/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      425 2024-05-01 04:01:29.000000 libfsext-20240501/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30141 2024-05-01 03:55:44.000000 libfsext-20240501/include/libfsext.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/include/libfsext/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2220 2024-05-01 03:55:44.000000 libfsext-20240501/include/libfsext/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2218 2024-05-01 04:28:37.000000 libfsext-20240501/include/libfsext/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5032 2024-05-01 03:55:44.000000 libfsext-20240501/include/libfsext/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4901 2024-05-01 04:28:37.000000 libfsext-20240501/include/libfsext/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 03:55:44.000000 libfsext-20240501/include/libfsext/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-05-01 03:55:44.000000 libfsext-20240501/include/libfsext/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 03:55:44.000000 libfsext-20240501/include/libfsext/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-05-01 04:28:37.000000 libfsext-20240501/include/libfsext/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-05-01 03:55:44.000000 libfsext-20240501/include/libfsext/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28421 2024-05-01 04:28:17.000000 libfsext-20240501/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30141 2024-05-01 04:28:37.000000 libfsext-20240501/include/libfsext.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-01 03:55:44.000000 libfsext-20240501/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-01 03:55:44.000000 libfsext-20240501/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-01 03:55:44.000000 libfsext-20240501/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-01 03:55:44.000000 libfsext-20240501/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-01 03:55:44.000000 libfsext-20240501/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-01 03:55:44.000000 libfsext-20240501/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-01 03:55:44.000000 libfsext-20240501/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-01 04:01:29.000000 libfsext-20240501/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-01 03:55:44.000000 libfsext-20240501/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-05-01 04:28:38.000000 libfsext-20240501/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17932 2024-05-01 04:28:16.000000 libfsext-20240501/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18983 2024-05-01 04:28:38.000000 libfsext-20240501/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-01 03:55:44.000000 libfsext-20240501/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-01 03:55:44.000000 libfsext-20240501/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-01 03:55:44.000000 libfsext-20240501/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25455 2024-05-01 04:28:17.000000 libfsext-20240501/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30653 2024-05-01 04:28:17.000000 libfsext-20240501/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-01 04:27:47.000000 libfsext-20240501/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31162 2024-05-01 04:28:17.000000 libfsext-20240501/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-01 04:27:55.000000 libfsext-20240501/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2111 2024-05-01 04:03:39.000000 libfsext-20240501/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34505 2024-05-01 04:28:17.000000 libfsext-20240501/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-01 04:27:39.000000 libfsext-20240501/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:06:05.000000 libfsext-20240501/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-01 04:28:17.000000 libfsext-20240501/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:23.000000 libfsext-20240501/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/libfsext-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-05-01 03:55:49.000000 libfsext-20240501/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:23.000000 libfsext-20240501/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2147 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-05-01 04:28:38.000000 libfsext-20240501/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/libfsext-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/libfsext.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-01 03:55:41.000000 libfsext-20240501/dpkg/libfsext-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-05-01 04:28:38.000000 libfsext-20240501/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-01 03:55:41.000000 libfsext-20240501/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1990719 2024-05-01 04:28:15.000000 libfsext-20240501/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-01 04:28:17.000000 libfsext-20240501/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-01 04:28:17.000000 libfsext-20240501/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsextinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7282 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/fsextinfo/fsextinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5732 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_notify/fsext_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsextmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7669 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/fsextmount/fsextmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_attribute_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5924 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_attribute_values/fsext_test_attribute_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_superblock/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6322 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_superblock/fsext_test_superblock.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5645 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_error/fsext_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_bitmap/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_bitmap/fsext_test_bitmap.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_block_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6343 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_block_data_handle/fsext_test_block_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_extent/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5894 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_extent/fsext_test_extent.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_inode_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5909 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_inode_table/fsext_test_inode_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6164 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_tools_info_handle/fsext_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2178 2024-05-01 04:02:56.000000 libfsext-20240501/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_extents_footer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5918 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_extents_footer/fsext_test_extents_footer.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_inode/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5891 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_inode/fsext_test_inode.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_directory_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5921 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_directory_entry/fsext_test_directory_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6307 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_block/fsext_test_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/pyfsext/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6871 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/pyfsext/pyfsext.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5903 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_io_handle/fsext_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_directory/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6319 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_directory/fsext_test_directory.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_tools_signal/fsext_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_extended_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_extended_attribute/fsext_test_extended_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_extent_index/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5912 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_extent_index/fsext_test_extent_index.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6557 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_volume/fsext_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_block_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6495 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_block_vector/fsext_test_block_vector.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44724 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/libfsext.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_buffer_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_buffer_data_handle/fsext_test_buffer_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_tools_output/fsext_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_file_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5906 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_file_entry/fsext_test_file_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_group_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6340 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_group_descriptor/fsext_test_group_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libfsext/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12069 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libfsext/libfsext.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_extents_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5918 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_extents_header/fsext_test_extents_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_checksum/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5657 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_checksum/fsext_test_checksum.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/fsext_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6560 2024-05-01 03:56:31.000000 libfsext-20240501/msvscpp/fsext_test_support/fsext_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24623 2024-05-01 04:28:17.000000 libfsext-20240501/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-05-01 03:56:12.000000 libfsext-20240501/msvscpp/libfdatetime/libfdatetime.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-05-01 03:55:44.000000 libfsext-20240501/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31486 2024-05-01 04:28:17.000000 libfsext-20240501/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-01 04:27:46.000000 libfsext-20240501/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      546 2024-05-01 03:57:04.000000 libfsext-20240501/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/pyfsext/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3525 2024-05-01 03:57:04.000000 libfsext-20240501/pyfsext/pyfsext_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7362 2024-05-01 03:57:04.000000 libfsext-20240501/pyfsext/pyfsext_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3486 2024-05-01 03:57:04.000000 libfsext-20240501/pyfsext/pyfsext_extended_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1311 2024-05-01 04:02:42.000000 libfsext-20240501/pyfsext/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_libfsext.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2634 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_extended_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28413 2024-05-01 03:57:04.000000 libfsext-20240501/pyfsext/pyfsext_extended_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_file_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15994 2024-05-01 03:57:04.000000 libfsext-20240501/pyfsext/pyfsext.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76653 2024-05-01 03:57:04.000000 libfsext-20240501/pyfsext/pyfsext_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48484 2024-05-01 04:28:17.000000 libfsext-20240501/pyfsext/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9890 2024-05-01 03:57:04.000000 libfsext-20240501/pyfsext/pyfsext_extended_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34943 2024-05-01 03:57:04.000000 libfsext-20240501/pyfsext/pyfsext_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9439 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_file_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-05-01 03:55:47.000000 libfsext-20240501/pyfsext/pyfsext_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-01 04:28:17.000000 libfsext-20240501/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-05-01 04:28:17.000000 libfsext-20240501/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 04:27:41.000000 libfsext-20240501/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-01 03:55:41.000000 libfsext-20240501/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-05-01 03:55:41.000000 libfsext-20240501/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-01 04:28:17.000000 libfsext-20240501/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-01 03:55:41.000000 libfsext-20240501/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-05-01 03:55:41.000000 libfsext-20240501/acinclude.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/fsexttools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36321 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3061 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37913 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4994 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3297 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/digest_hash.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30757 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4361 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1590 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2557 2024-05-01 04:02:21.000000 libfsext-20240501/fsexttools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22158 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    80949 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3661 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15493 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/fsextmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10875 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/fsextinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3324 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19354 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libfsext.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35513 2024-05-01 04:28:17.000000 libfsext-20240501/fsexttools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1244 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/digest_hash.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2024-05-01 03:55:47.000000 libfsext-20240501/fsexttools/fsexttools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3050 2024-05-01 03:57:04.000000 libfsext-20240501/fsexttools/mount_fuse.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:06:05.000000 libfsext-20240501/config.rpath
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3488 2024-05-01 03:55:41.000000 libfsext-20240501/libfsext.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33838 2024-05-01 04:28:17.000000 libfsext-20240501/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-01 04:27:53.000000 libfsext-20240501/libcthreads/libcthreads_queue.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/libfsext/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8529 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_bitmap.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_block_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2179 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_inode_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12002 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1799 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_bitmap.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10228 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extent.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7821 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17086 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_attribute_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1819 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_attributes_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24275 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_directory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7795 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1670 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_checksum.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2787 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_group_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_block_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1089 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22610 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_group_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2695 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/fsext_extents.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-05-01 04:02:12.000000 libfsext-20240501/libfsext/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6039 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extent_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3103 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_attribute_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14856 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/fsext_superblock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22186 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_data_blocks.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2125 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extent.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4899 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_block_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2233 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_data_blocks.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4774 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extents_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9425 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6407 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extents_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3001 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_directory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18271 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extent_index.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36220 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extended_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extents_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   120345 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52454 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_superblock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8391 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_block_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3812 2024-05-01 04:28:37.000000 libfsext-20240501/libfsext/libfsext_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1832 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   103953 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66410 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_inode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_block_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2709 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/fsext_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2195 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extents.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6994 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_superblock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2202 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10968 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_block_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extended_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8716 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/fsext_inode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18929 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extents.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23037 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3814 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4711 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/fsext_group_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41767 2024-05-01 04:28:17.000000 libfsext-20240501/libfsext/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6061 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_inode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_buffer_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1087 2024-05-01 04:28:38.000000 libfsext-20240501/libfsext/libfsext.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14079 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_attributes_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2868 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10147 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_inode_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/fsext_directory_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1659 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_extents_footer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1879 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3299 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_directory_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3804 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5241 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 03:55:46.000000 libfsext-20240501/libfsext/libfsext_unused.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-01 04:28:17.000000 libfsext-20240501/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30684 2024-05-01 04:28:17.000000 libfsext-20240501/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-01 04:27:50.000000 libfsext-20240501/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1058 2024-03-01 13:58:36.000000 libfsext-20240501/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3235 2024-05-01 03:55:49.000000 libfsext-20240501/manuals/fsextinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      161 2024-05-01 04:01:58.000000 libfsext-20240501/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2024-05-01 03:55:49.000000 libfsext-20240501/manuals/fsextmount.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27450 2024-05-01 04:28:17.000000 libfsext-20240501/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14808 2024-05-01 03:55:49.000000 libfsext-20240501/manuals/libfsext.3
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_libfsext.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9650 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_extents_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21176 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_attribute_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16235 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4261 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2663 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_inode_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4275 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_checksum.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4045 2024-05-01 04:00:17.000000 libfsext-20240501/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15297 2024-05-01 03:55:49.000000 libfsext-20240501/tests/fsext_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16666 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_block_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-05-01 03:55:49.000000 libfsext-20240501/tests/fsext_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15726 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22091 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_superblock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24871 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12445 2024-05-01 04:09:49.000000 libfsext-20240501/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4052 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_extended_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38388 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6551 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_group_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11536 2024-05-01 03:57:04.000000 libfsext-20240501/tests/pyfsext_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40916 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_inode.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 03:55:48.000000 libfsext-20240501/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4415 2024-05-01 03:55:48.000000 libfsext-20240501/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6297 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_extents_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20513 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_bitmap.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_extent_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32886 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_directory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1997 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-01 03:55:48.000000 libfsext-20240501/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13376 2024-05-01 03:56:31.000000 libfsext-20240501/tests/fsext_test_extent.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20870 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_block_vector.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3317 2024-05-01 03:55:48.000000 libfsext-20240501/tests/test_fsextinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    80694 2024-05-01 04:28:18.000000 libfsext-20240501/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-05-01 03:55:49.000000 libfsext-20240501/tests/fsext_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5706 2024-05-01 03:55:49.000000 libfsext-20240501/tests/fsext_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2800 2024-05-01 03:55:48.000000 libfsext-20240501/tests/fsext_test_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3464 2024-05-01 03:57:04.000000 libfsext-20240501/tests/pyfsext_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 03:55:49.000000 libfsext-20240501/tests/fsext_test_unused.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4295 2024-05-01 03:59:59.000000 libfsext-20240501/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:26.000000 libfsext-20240501/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3661 2024-05-01 03:55:46.000000 libfsext-20240501/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2020 2024-05-01 04:01:41.000000 libfsext-20240501/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-05-01 03:55:46.000000 libfsext-20240501/ossfuzz/ossfuzz_libfsext.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-01 03:55:46.000000 libfsext-20240501/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5555 2024-05-01 03:55:46.000000 libfsext-20240501/ossfuzz/file_entry_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-05-01 03:55:46.000000 libfsext-20240501/ossfuzz/extended_attribute_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36956 2024-05-01 04:28:17.000000 libfsext-20240501/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-01 04:28:10.000000 libfsext-20240501/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33549 2024-05-01 04:28:17.000000 libfsext-20240501/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-01 04:28:01.000000 libfsext-20240501/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31581 2024-05-01 04:28:17.000000 libfsext-20240501/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-01 04:27:52.000000 libfsext-20240501/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:06:33.000000 libfsext-20240501/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:06:33.000000 libfsext-20240501/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:06:33.000000 libfsext-20240501/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:06:33.000000 libfsext-20240501/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:06:33.000000 libfsext-20240501/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:06:33.000000 libfsext-20240501/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:06:33.000000 libfsext-20240501/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:06:33.000000 libfsext-20240501/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:06:33.000000 libfsext-20240501/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-05-01 04:28:37.000000 libfsext-20240501/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:06:33.000000 libfsext-20240501/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:06:33.000000 libfsext-20240501/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57165 2024-05-01 04:28:17.000000 libfsext-20240501/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-01 04:28:05.000000 libfsext-20240501/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41405 2024-05-01 04:28:17.000000 libfsext-20240501/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30522 2024-05-01 04:28:17.000000 libfsext-20240501/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-01 04:27:49.000000 libfsext-20240501/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:24.000000 libfsext-20240501/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 04:27:43.000000 libfsext-20240501/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29989 2024-05-01 04:28:17.000000 libfsext-20240501/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 05:52:25.000000 libfsext-20240501/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33573 2024-05-01 04:28:17.000000 libfsext-20240501/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-05-01 04:27:58.000000 libfsext-20240501/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56884 2024-05-01 04:28:13.000000 libfsext-20240501/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8065 2024-05-01 03:55:41.000000 libfsext-20240501/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-05-01 05:52:27.011720 libfsext-20240501/PKG-INFO
```

### Comparing `libfsext-20240301/libfdata/libfdata_error.h` & `libfsext-20240501/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_area.c` & `libfsext-20240501/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_stream.h` & `libfsext-20240501/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_cache.h` & `libfsext-20240501/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_range_list.c` & `libfsext-20240501/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_mapped_range.c` & `libfsext-20240501/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_libcerror.h` & `libfsext-20240501/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_definitions.h` & `libfsext-20240501/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libfsext-20240301/libfdata/libfdata_list.c` & `libfsext-20240501/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_libcdata.h` & `libfsext-20240501/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_list.h` & `libfsext-20240501/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_list_element.h` & `libfsext-20240501/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/Makefile.am` & `libfsext-20240501/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libfsext-20240301/libfdata/libfdata_libcnotify.h` & `libfsext-20240501/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_extern.h` & `libfsext-20240501/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_notify.c` & `libfsext-20240501/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_cache.c` & `libfsext-20240501/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_stream.c` & `libfsext-20240501/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_unused.h` & `libfsext-20240501/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_range.h` & `libfsext-20240501/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_area.h` & `libfsext-20240501/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_error.c` & `libfsext-20240501/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_support.h` & `libfsext-20240501/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_range.c` & `libfsext-20240501/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_mapped_range.h` & `libfsext-20240501/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_support.c` & `libfsext-20240501/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_list_element.c` & `libfsext-20240501/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_segments_array.c` & `libfsext-20240501/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_types.h` & `libfsext-20240501/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_notify.h` & `libfsext-20240501/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_range_list.h` & `libfsext-20240501/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_segments_array.h` & `libfsext-20240501/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/Makefile.in` & `libfsext-20240501/libfdata/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -485,14 +485,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -553,16 +555,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -586,15 +588,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -806,24 +809,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -919,17 +937,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libfdata/libfdata_vector.c` & `libfsext-20240501/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_libfcache.h` & `libfsext-20240501/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdata/libfdata_vector.h` & `libfsext-20240501/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/COPYING` & `libfsext-20240501/COPYING`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/install-sh` & `libfsext-20240501/install-sh`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext.spec` & `libfsext-20240501/libfsext.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfsext
-Version: 20240301
+Version: 20240501
 Release: 1
 Summary: Library to support the Extended File System (ext) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfsext
               
@@ -36,16 +36,16 @@
 
 %description -n libfsext-python3
 Python 3 bindings for libfsext
 
 %package -n libfsext-tools
 Summary: Several tools for reading Extended File System (ext) volumes
 Group: Applications/System
-Requires: libfsext = %{version}-%{release} openssl fuse-libs 
-BuildRequires: openssl-devel fuse-devel 
+Requires: libfsext = %{version}-%{release} openssl fuse3-libs 
+BuildRequires: openssl-devel fuse3-devel 
 
 %description -n libfsext-tools
 Several tools for reading Extended File System (ext) volumes
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libfsext-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sat Mar  2 2024 Joachim Metz <joachim.metz@gmail.com> 20240301-1
+* Wed May  1 2024 Joachim Metz <joachim.metz@gmail.com> 20240501-1
 - Auto-generated
```

### Comparing `libfsext-20240301/depcomp` & `libfsext-20240501/depcomp`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_error.c` & `libfsext-20240501/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_support.h` & `libfsext-20240501/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_identifier.h` & `libfsext-20240501/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_libcerror.h` & `libfsext-20240501/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/Makefile.am` & `libfsext-20240501/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libfsext-20240301/libfguid/libfguid_unused.h` & `libfsext-20240501/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_extern.h` & `libfsext-20240501/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_types.h` & `libfsext-20240501/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_identifier.c` & `libfsext-20240501/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_support.c` & `libfsext-20240501/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfguid/libfguid_definitions.h` & `libfsext-20240501/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libfsext-20240301/libfguid/Makefile.in` & `libfsext-20240501/libfguid/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -529,30 +531,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -754,24 +757,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -857,17 +865,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libfguid/libfguid_error.h` & `libfsext-20240501/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext.pc.in` & `libfsext-20240501/libfsext.pc.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/libcfile.m4` & `libfsext-20240501/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/libfdatetime.m4` & `libfsext-20240501/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/tests.m4` & `libfsext-20240501/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/libcpath.m4` & `libfsext-20240501/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/lib-prefix.m4` & `libfsext-20240501/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/progtest.m4` & `libfsext-20240501/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/libuna.m4` & `libfsext-20240501/m4/libuna.m4`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -239,14 +241,44 @@
         AC_CHECK_LIB(
           una,
           libuna_unicode_character_copy_to_byte_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_unicode_character_size_to_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_unicode_character_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_unicode_character_copy_to_utf7_stream,
           [ac_cv_libuna_dummy=yes],
@@ -908,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -939,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/gettext.m4` & `libfsext-20240501/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/lib-ld.m4` & `libfsext-20240501/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/libclocale.m4` & `libfsext-20240501/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/libcdata.m4` & `libfsext-20240501/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/libcsplit.m4` & `libfsext-20240501/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/common.m4` & `libfsext-20240501/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libfsext-20240301/m4/libcthreads.m4` & `libfsext-20240501/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libfsext-20240301/m4/ltversion.m4` & `libfsext-20240501/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/ltsugar.m4` & `libfsext-20240501/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/libfdata.m4` & `libfsext-20240501/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/host-cpu-c-abi.m4` & `libfsext-20240501/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/libfuse.m4` & `libfsext-20240501/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libfsext-20240301/m4/libtool.m4` & `libfsext-20240501/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/po.m4` & `libfsext-20240501/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/libcerror.m4` & `libfsext-20240501/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/libcnotify.m4` & `libfsext-20240501/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/libfguid.m4` & `libfsext-20240501/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libfsext-20240301/m4/libbfio.m4` & `libfsext-20240501/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/libhmac.m4` & `libfsext-20240501/m4/libhmac.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libhmac required headers and functions
 dnl
-dnl Version: 20200104
+dnl Version: 20240413
 
 dnl Function to detect if libhmac is available
 dnl ac_libhmac_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBHMAC_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno],
     [ac_cv_libhmac=no],
     [ac_cv_libhmac=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libhmac which returns "yes" and --with-libhmac= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect],
+      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libhmac"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libhmac}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libhmac}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libhmac],
           [1])
@@ -161,16 +163,17 @@
           hmac,
           libhmac_sha512_free,
           [ac_cv_libhmac_dummy=yes],
           [ac_cv_libhmac=no])
 
         ac_cv_libhmac_LIBADD="-lhmac"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_libhmac" != xyes],
+      [test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libhmac in directory: $ac_cv_with_libhmac],
         [1])
       ])
     ])
 
   AS_IF(
@@ -240,15 +243,15 @@
     [ac_cv_libhmac_sha256=$ac_cv_libcrypto_sha256])
 
   AS_IF(
     [test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno],
     [ac_cv_libhmac_sha512=local],
     [ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512])
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
   ])
 
 dnl Function to detect how to enable libhmac
 AC_DEFUN([AX_LIBHMAC_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/intlmacosx.m4` & `libfsext-20240501/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/lt~obsolete.m4` & `libfsext-20240501/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/lib-link.m4` & `libfsext-20240501/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/iconv.m4` & `libfsext-20240501/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/ltoptions.m4` & `libfsext-20240501/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/nls.m4` & `libfsext-20240501/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/python.m4` & `libfsext-20240501/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libfsext-20240301/m4/libcrypto.m4` & `libfsext-20240501/m4/libcrypto.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcrypto required headers and functions
 dnl
-dnl Version: 20231007
+dnl Version: 20240308
 
 dnl Function to detect whether openssl/evp.h can be used in combination with zlib.h
 AC_DEFUN([AX_LIBCRYPTO_CHECK_OPENSSL_EVP_ZLIB_COMPATIBILE],
   [AC_CACHE_CHECK(
     [if openssl/evp.h can be used in combination with zlib.h],
     [ac_cv_openssl_evp_zlib_compatible],
     [AC_LANG_PUSH(C)
@@ -619,16 +619,18 @@
 
 dnl Function to detect if libcrypto (openssl) dependencies are available
 AC_DEFUN([AX_LIBCRYPTO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno],
     [ac_cv_libcrypto=no],
     [dnl Check if the directory provided as parameter exists
+    dnl For both --with-openssl which returns "yes" and --with-openssl= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect],
+      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_openssl"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_openssl],
           [1])
```

### Comparing `libfsext-20240301/m4/types.m4` & `libfsext-20240501/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/m4/libfcache.m4` & `libfsext-20240501/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libfsext-20240301/m4/pthread.m4` & `libfsext-20240501/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libfsext-20240301/include/libfsext.h.in` & `libfsext-20240501/include/libfsext.h.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/libfsext/definitions.h.in` & `libfsext-20240501/include/libfsext/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/libfsext/definitions.h` & `libfsext-20240501/include/libfsext/definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFSEXT_DEFINITIONS_H )
 #define _LIBFSEXT_DEFINITIONS_H
 
 #include <libfsext/types.h>
 
-#define LIBFSEXT_VERSION			20240301
+#define LIBFSEXT_VERSION			20240501
 
 /* The version string
  */
-#define LIBFSEXT_VERSION_STRING			"20240301"
+#define LIBFSEXT_VERSION_STRING			"20240501"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSEXT_ACCESS_FLAGS
```

### Comparing `libfsext-20240301/include/libfsext/types.h.in` & `libfsext-20240501/include/libfsext/types.h.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/libfsext/types.h` & `libfsext-20240501/include/libfsext/types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/libfsext/features.h.in` & `libfsext-20240501/include/libfsext/features.h.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/libfsext/error.h` & `libfsext-20240501/include/libfsext/error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/libfsext/extern.h` & `libfsext-20240501/include/libfsext/extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/libfsext/features.h` & `libfsext-20240501/include/libfsext/features.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/libfsext/codepage.h` & `libfsext-20240501/include/libfsext/codepage.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/include/Makefile.in` & `libfsext-20240501/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -451,14 +451,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -535,15 +537,20 @@
 
 EXTRA_DIST = \
 	libfsext.h.in \
 	libfsext/definitions.h.in \
 	libfsext/features.h.in \
 	libfsext/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsext.h \
+	libfsext/definitions.h \
+	libfsext/features.h \
+	libfsext/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -740,23 +747,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -838,17 +847,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfsext.h
-	-rm -f libfsext/definitions.h
-	-rm -f libfsext/features.h
-	-rm -f libfsext/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/include/libfsext.h` & `libfsext-20240501/include/libfsext.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/config_borlandc.h` & `libfsext-20240501/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/file_stream.h` & `libfsext-20240501/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/memory.h` & `libfsext-20240501/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/byte_stream.h` & `libfsext-20240501/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/common.h` & `libfsext-20240501/common/common.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/config_winapi.h` & `libfsext-20240501/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/system_string.h` & `libfsext-20240501/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/types.h.in` & `libfsext-20240501/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/types.h` & `libfsext-20240501/common/types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/config.h.in` & `libfsext-20240501/common/config.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -239,14 +239,17 @@
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 #undef HAVE_LIBFGUID_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the `hmac' library (-lhmac). */
 #undef HAVE_LIBHMAC
 
 /* Define to 1 if you have the <libhmac.h> header file. */
 #undef HAVE_LIBHMAC_H
 
 /* Define to 1 if you have the <libintl.h> header file. */
```

### Comparing `libfsext-20240301/common/config.h` & `libfsext-20240501/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,18 @@
 /* Define to 1 if you have the `fguid' library (-lfguid). */
 /* #undef HAVE_LIBFGUID */
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 /* #undef HAVE_LIBFGUID_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the `hmac' library (-lhmac). */
 /* #undef HAVE_LIBHMAC */
 
 /* Define to 1 if you have the <libhmac.h> header file. */
 /* #undef HAVE_LIBHMAC_H */
 
@@ -589,24 +592,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfsext"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfsext 20240301"
+#define PACKAGE_STRING "libfsext 20240501"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfsext"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240301"
+#define PACKAGE_VERSION "20240501"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -627,15 +630,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240301"
+#define VERSION "20240501"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfsext-20240301/common/wide_string.h` & `libfsext-20240501/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/narrow_string.h` & `libfsext-20240501/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/config_msc.h` & `libfsext-20240501/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/common/Makefile.in` & `libfsext-20240501/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -421,14 +421,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -488,15 +490,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -504,15 +508,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -680,23 +687,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -776,15 +785,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/libclocale/libclocale_wide_string.c` & `libfsext-20240501/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/libclocale_support.h` & `libfsext-20240501/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/Makefile.am` & `libfsext-20240501/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libfsext-20240301/libclocale/libclocale_definitions.h` & `libfsext-20240501/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libfsext-20240301/libclocale/libclocale_unused.h` & `libfsext-20240501/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/libclocale_libcerror.h` & `libfsext-20240501/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/libclocale_locale.h` & `libfsext-20240501/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/libclocale_support.c` & `libfsext-20240501/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/libclocale_codepage.c` & `libfsext-20240501/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/libclocale_locale.c` & `libfsext-20240501/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/Makefile.in` & `libfsext-20240501/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -465,14 +465,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -534,30 +536,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -760,24 +763,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -864,17 +873,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libclocale/libclocale_extern.h` & `libfsext-20240501/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/libclocale_wide_string.h` & `libfsext-20240501/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libclocale/libclocale_codepage.h` & `libfsext-20240501/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_libcdata.h` & `libfsext-20240501/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_types.h` & `libfsext-20240501/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_cache_value.c` & `libfsext-20240501/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_unused.h` & `libfsext-20240501/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/Makefile.am` & `libfsext-20240501/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libfsext-20240301/libfcache/libfcache_support.h` & `libfsext-20240501/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_error.h` & `libfsext-20240501/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_support.c` & `libfsext-20240501/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_cache.h` & `libfsext-20240501/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_error.c` & `libfsext-20240501/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_libcerror.h` & `libfsext-20240501/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_date_time.c` & `libfsext-20240501/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_extern.h` & `libfsext-20240501/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_cache_value.h` & `libfsext-20240501/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/Makefile.in` & `libfsext-20240501/libfcache/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -468,14 +468,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -557,15 +559,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -769,24 +772,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -874,17 +884,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libfcache/libfcache_date_time.h` & `libfsext-20240501/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfcache/libfcache_definitions.h` & `libfsext-20240501/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libfsext-20240301/libfcache/libfcache_cache.c` & `libfsext-20240501/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/Makefile.am` & `libfsext-20240501/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -60,16 +60,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libfsext.pc \
+	libfsext.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfsext.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -92,19 +99,7 @@
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfsext && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfsext.pc
-	-rm -f libfsext.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfsext-20240301/libbfio/libbfio_file_range.h` & `libfsext-20240501/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file_range_io_handle.c` & `libfsext-20240501/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_support.c` & `libfsext-20240501/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_libcpath.h` & `libfsext-20240501/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_error.h` & `libfsext-20240501/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_libclocale.h` & `libfsext-20240501/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_error.c` & `libfsext-20240501/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_libuna.h` & `libfsext-20240501/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file_io_handle.h` & `libfsext-20240501/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file_pool.h` & `libfsext-20240501/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file_range.c` & `libfsext-20240501/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_types.h` & `libfsext-20240501/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_unused.h` & `libfsext-20240501/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_libcdata.h` & `libfsext-20240501/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file.h` & `libfsext-20240501/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/Makefile.am` & `libfsext-20240501/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libfsext-20240301/libbfio/libbfio_libcfile.h` & `libfsext-20240501/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_definitions.h` & `libfsext-20240501/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libfsext-20240301/libbfio/libbfio_codepage.h` & `libfsext-20240501/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file_io_handle.c` & `libfsext-20240501/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_support.h` & `libfsext-20240501/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_memory_range.h` & `libfsext-20240501/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file_pool.c` & `libfsext-20240501/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file_range_io_handle.h` & `libfsext-20240501/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_libcthreads.h` & `libfsext-20240501/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_system_string.h` & `libfsext-20240501/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_memory_range_io_handle.c` & `libfsext-20240501/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_handle.c` & `libfsext-20240501/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_file.c` & `libfsext-20240501/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_handle.h` & `libfsext-20240501/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_memory_range.c` & `libfsext-20240501/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_pool.c` & `libfsext-20240501/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_libcerror.h` & `libfsext-20240501/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/Makefile.in` & `libfsext-20240501/libbfio/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -486,14 +486,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -554,16 +556,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -594,15 +596,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -813,24 +816,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -899,14 +916,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -917,23 +936,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/libbfio/libbfio_system_string.c` & `libfsext-20240501/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_memory_range_io_handle.h` & `libfsext-20240501/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_extern.h` & `libfsext-20240501/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/libbfio/libbfio_pool.h` & `libfsext-20240501/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsext-20240301/config.guess` & `libfsext-20240501/config.guess`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/dpkg/copyright` & `libfsext-20240501/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/dpkg/control` & `libfsext-20240501/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/dpkg/rules` & `libfsext-20240501/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/COPYING.LESSER` & `libfsext-20240501/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/configure` & `libfsext-20240501/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfsext 20240301.
+# Generated by GNU Autoconf 2.71 for libfsext 20240501.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfsext'
 PACKAGE_TARNAME='libfsext'
-PACKAGE_VERSION='20240301'
-PACKAGE_STRING='libfsext 20240301'
+PACKAGE_VERSION='20240501'
+PACKAGE_STRING='libfsext 20240501'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfsext.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 ax_libhmac_spec_build_requires
 ax_libhmac_spec_requires
 ax_libhmac_pc_libs_private
 LIBHMAC_LIBADD
 LIBHMAC_CPPFLAGS
 HAVE_LOCAL_LIBHMAC_FALSE
 HAVE_LOCAL_LIBHMAC_TRUE
@@ -1129,14 +1131,16 @@
 libfdatetime_LIBS
 libfguid_CFLAGS
 libfguid_LIBS
 libhmac_CFLAGS
 libhmac_LIBS
 openssl_CFLAGS
 openssl_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1679,15 +1683,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfsext 20240301 to adapt to many kinds of systems.
+\`configure' configures libfsext 20240501 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1750,15 +1754,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfsext 20240301:";;
+     short | recursive ) echo "Configuration of libfsext 20240501:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1949,14 +1953,17 @@
               C compiler flags for libhmac, overriding pkg-config
   libhmac_LIBS
               linker flags for libhmac, overriding pkg-config
   openssl_CFLAGS
               C compiler flags for openssl, overriding pkg-config
   openssl_LIBS
               linker flags for openssl, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -2019,15 +2026,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfsext configure 20240301
+libfsext configure 20240501
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2740,15 +2747,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfsext $as_me 20240301, which was
+It was created by libfsext $as_me 20240501, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4229,15 +4236,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfsext'
- VERSION='20240301'
+ VERSION='20240501'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23824,15 +23831,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24323,15 +24330,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24473,15 +24481,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24575,15 +24583,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26215,15 +26223,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26277,47 +26285,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26351,15 +26364,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26393,15 +26406,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26436,15 +26449,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26478,15 +26491,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26520,15 +26533,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26562,15 +26575,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26604,15 +26617,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26647,15 +26660,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26689,15 +26702,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26731,15 +26744,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26773,15 +26786,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26815,15 +26828,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26858,15 +26871,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26900,15 +26913,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26942,15 +26955,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26984,15 +26997,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27026,15 +27039,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27069,67 +27082,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27217,15 +27239,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30996,15 +31018,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31029,15 +31052,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31107,15 +31130,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31662,15 +31685,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31826,15 +31850,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31904,15 +31928,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32362,15 +32386,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32425,15 +32450,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32503,15 +32528,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33226,15 +33251,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33259,15 +33285,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33337,15 +33363,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -34844,14 +34870,266 @@
 if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf7_stream in -luna" >&5
 printf %s "checking for libuna_unicode_character_copy_from_utf7_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -40295,15 +40573,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40328,15 +40607,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40406,15 +40685,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41595,15 +41874,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -41917,15 +42197,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -41995,15 +42275,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -42800,15 +43080,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42998,15 +43279,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43076,15 +43357,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45194,15 +45475,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45227,15 +45509,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45305,15 +45587,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46225,15 +46507,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46326,15 +46609,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46404,15 +46687,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49692,15 +49975,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49725,15 +50009,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -49803,15 +50087,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -53247,15 +53531,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -53280,15 +53565,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53358,15 +53643,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -53940,15 +54225,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -53973,15 +54259,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -54292,16 +54578,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -54464,15 +54754,15 @@
 printf "%s\n" "$ac_cv_with_libhmac" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno
 then :
   ac_cv_libhmac=no
 else $as_nop
   ac_cv_libhmac=check
-        if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect
+                if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   if test -d "$ac_cv_with_libhmac"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libhmac}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libhmac}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -55470,15 +55760,16 @@
 fi
 
 
         ac_cv_libhmac_LIBADD="-lhmac"
 fi
 
 fi
-    if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_libhmac" != xyes
+
+    if test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libhmac in directory: $ac_cv_with_libhmac
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -55584,15 +55875,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -59770,15 +60061,15 @@
   if test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno
 then :
   ac_cv_libhmac_sha512=local
 else $as_nop
   ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512
 fi
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBHMAC 1" >>confdefs.h
@@ -59843,33 +60134,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
 
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
+
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
+fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
+
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -59937,51 +60302,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -60144,45 +60568,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -60350,29 +60767,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -60403,14 +60840,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -60418,14 +60861,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -61351,15 +61802,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfsext $as_me 20240301, which was
+This file was extended by libfsext $as_me 20240501, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -61419,15 +61870,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfsext config.status 20240301
+libfsext config.status 20240501
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfsext-20240301/compile` & `libfsext-20240501/compile`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/missing` & `libfsext-20240501/missing`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libfdata/libfdata.vcproj` & `libfsext-20240501/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsextinfo/fsextinfo.vcproj` & `libfsext-20240501/msvscpp/fsextinfo/fsextinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_notify/fsext_test_notify.vcproj` & `libfsext-20240501/msvscpp/fsext_test_notify/fsext_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsextmount/fsextmount.vcproj` & `libfsext-20240501/msvscpp/fsextmount/fsextmount.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_attribute_values/fsext_test_attribute_values.vcproj` & `libfsext-20240501/msvscpp/fsext_test_attribute_values/fsext_test_attribute_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_superblock/fsext_test_superblock.vcproj` & `libfsext-20240501/msvscpp/fsext_test_superblock/fsext_test_superblock.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_error/fsext_test_error.vcproj` & `libfsext-20240501/msvscpp/fsext_test_error/fsext_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_bitmap/fsext_test_bitmap.vcproj` & `libfsext-20240501/msvscpp/fsext_test_bitmap/fsext_test_bitmap.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_block_data_handle/fsext_test_block_data_handle.vcproj` & `libfsext-20240501/msvscpp/fsext_test_block_data_handle/fsext_test_block_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libfguid/libfguid.vcproj` & `libfsext-20240501/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_extent/fsext_test_extent.vcproj` & `libfsext-20240501/msvscpp/fsext_test_extent/fsext_test_extent.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libclocale/libclocale.vcproj` & `libfsext-20240501/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_inode_table/fsext_test_inode_table.vcproj` & `libfsext-20240501/msvscpp/fsext_test_inode_table/fsext_test_inode_table.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_tools_info_handle/fsext_test_tools_info_handle.vcproj` & `libfsext-20240501/msvscpp/fsext_test_tools_info_handle/fsext_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libfcache/libfcache.vcproj` & `libfsext-20240501/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/Makefile.am` & `libfsext-20240501/msvscpp/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -46,13 +46,11 @@
 	libuna/libuna.vcproj \
 	pyfsext/pyfsext.vcproj \
 	libfsext.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfsext-20240301/msvscpp/libbfio/libbfio.vcproj` & `libfsext-20240501/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_extents_footer/fsext_test_extents_footer.vcproj` & `libfsext-20240501/msvscpp/fsext_test_extents_footer/fsext_test_extents_footer.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_inode/fsext_test_inode.vcproj` & `libfsext-20240501/msvscpp/fsext_test_inode/fsext_test_inode.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_directory_entry/fsext_test_directory_entry.vcproj` & `libfsext-20240501/msvscpp/fsext_test_directory_entry/fsext_test_directory_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libcfile/libcfile.vcproj` & `libfsext-20240501/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_block/fsext_test_block.vcproj` & `libfsext-20240501/msvscpp/fsext_test_block/fsext_test_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/pyfsext/pyfsext.vcproj` & `libfsext-20240501/msvscpp/pyfsext/pyfsext.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_io_handle/fsext_test_io_handle.vcproj` & `libfsext-20240501/msvscpp/fsext_test_io_handle/fsext_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_directory/fsext_test_directory.vcproj` & `libfsext-20240501/msvscpp/fsext_test_directory/fsext_test_directory.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libcdata/libcdata.vcproj` & `libfsext-20240501/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_tools_signal/fsext_test_tools_signal.vcproj` & `libfsext-20240501/msvscpp/fsext_test_tools_signal/fsext_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_extended_attribute/fsext_test_extended_attribute.vcproj` & `libfsext-20240501/msvscpp/fsext_test_extended_attribute/fsext_test_extended_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_extent_index/fsext_test_extent_index.vcproj` & `libfsext-20240501/msvscpp/fsext_test_extent_index/fsext_test_extent_index.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_volume/fsext_test_volume.vcproj` & `libfsext-20240501/msvscpp/fsext_test_volume/fsext_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_block_vector/fsext_test_block_vector.vcproj` & `libfsext-20240501/msvscpp/fsext_test_block_vector/fsext_test_block_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libfsext.sln` & `libfsext-20240501/msvscpp/libfsext.sln`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_buffer_data_handle/fsext_test_buffer_data_handle.vcproj` & `libfsext-20240501/msvscpp/fsext_test_buffer_data_handle/fsext_test_buffer_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_tools_output/fsext_test_tools_output.vcproj` & `libfsext-20240501/msvscpp/fsext_test_tools_output/fsext_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_file_entry/fsext_test_file_entry.vcproj` & `libfsext-20240501/msvscpp/fsext_test_file_entry/fsext_test_file_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libcthreads/libcthreads.vcproj` & `libfsext-20240501/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_group_descriptor/fsext_test_group_descriptor.vcproj` & `libfsext-20240501/msvscpp/fsext_test_group_descriptor/fsext_test_group_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libfsext/libfsext.vcproj` & `libfsext-20240501/msvscpp/libfsext/libfsext.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libcpath/libcpath.vcproj` & `libfsext-20240501/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_extents_header/fsext_test_extents_header.vcproj` & `libfsext-20240501/msvscpp/fsext_test_extents_header/fsext_test_extents_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libhmac/libhmac.vcproj` & `libfsext-20240501/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libcsplit/libcsplit.vcproj` & `libfsext-20240501/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_checksum/fsext_test_checksum.vcproj` & `libfsext-20240501/msvscpp/fsext_test_checksum/fsext_test_checksum.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/fsext_test_support/fsext_test_support.vcproj` & `libfsext-20240501/msvscpp/fsext_test_support/fsext_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libuna/libuna.vcproj` & `libfsext-20240501/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/Makefile.in` & `libfsext-20240501/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -403,14 +403,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -522,15 +524,16 @@
 	libuna/libuna.vcproj \
 	pyfsext/pyfsext.vcproj \
 	libfsext.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -634,23 +637,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -729,13 +734,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/msvscpp/libcnotify/libcnotify.vcproj` & `libfsext-20240501/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libcerror/libcerror.vcproj` & `libfsext-20240501/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfsext-20240501/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_extern.h` & `libfsext-20240501/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_support.h` & `libfsext-20240501/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_unused.h` & `libfsext-20240501/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_notify.h` & `libfsext-20240501/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_support.c` & `libfsext-20240501/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_types.h` & `libfsext-20240501/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/Makefile.am` & `libfsext-20240501/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libfsext-20240301/libcfile/libcfile_notify.c` & `libfsext-20240501/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_system_string.h` & `libfsext-20240501/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_file.h` & `libfsext-20240501/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_libcnotify.h` & `libfsext-20240501/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_system_string.c` & `libfsext-20240501/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_error.h` & `libfsext-20240501/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_libcerror.h` & `libfsext-20240501/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_file.c` & `libfsext-20240501/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_libclocale.h` & `libfsext-20240501/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_winapi.h` & `libfsext-20240501/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/Makefile.in` & `libfsext-20240501/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -468,14 +468,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -560,15 +562,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -773,24 +776,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -879,17 +890,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libcfile/libcfile_error.c` & `libfsext-20240501/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_libuna.h` & `libfsext-20240501/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_winapi.c` & `libfsext-20240501/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcfile/libcfile_definitions.h` & `libfsext-20240501/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libfsext-20240301/README` & `libfsext-20240501/README`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_error.c` & `libfsext-20240501/pyfsext/pyfsext_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_volume.h` & `libfsext-20240501/pyfsext/pyfsext_volume.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_file_entry.h` & `libfsext-20240501/pyfsext/pyfsext_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_extended_attribute.h` & `libfsext-20240501/pyfsext/pyfsext_extended_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_integer.c` & `libfsext-20240501/pyfsext/pyfsext_integer.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_datetime.h` & `libfsext-20240501/pyfsext/pyfsext_datetime.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_libcerror.h` & `libfsext-20240501/pyfsext/pyfsext_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_python.h` & `libfsext-20240501/pyfsext/pyfsext_python.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/Makefile.am` & `libfsext-20240501/pyfsext/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -43,14 +43,11 @@
 	@LIBBFIO_LIBADD@
 
 pyfsext_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfsext_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f setup.py
-	-rm -f Makefile
-
```

### Comparing `libfsext-20240301/pyfsext/pyfsext_libfsext.h` & `libfsext-20240501/pyfsext/pyfsext_libfsext.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_integer.h` & `libfsext-20240501/pyfsext/pyfsext_integer.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_extended_attributes.h` & `libfsext-20240501/pyfsext/pyfsext_extended_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_extended_attribute.c` & `libfsext-20240501/pyfsext/pyfsext_extended_attribute.c`

 * *Files 1% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 	  "get_name() -> Unicode string\n"
 	  "\n"
 	  "Retrieves the name." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyfsext_extended_attribute_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyfsext_extended_attribute_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyfsext_extended_attribute_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -70,15 +70,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset within the data." },
 
 	{ "read",
 	  (PyCFunction) pyfsext_extended_attribute_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "seek",
 	  (PyCFunction) pyfsext_extended_attribute_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libfsext-20240301/pyfsext/pyfsext_file_object_io_handle.c` & `libfsext-20240501/pyfsext/pyfsext_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_unused.h` & `libfsext-20240501/pyfsext/pyfsext_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_file_entries.h` & `libfsext-20240501/pyfsext/pyfsext_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext.h` & `libfsext-20240501/pyfsext/pyfsext.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_file_object_io_handle.h` & `libfsext-20240501/pyfsext/pyfsext_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext.c` & `libfsext-20240501/pyfsext/pyfsext.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_libbfio.h` & `libfsext-20240501/pyfsext/pyfsext_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_file_entry.c` & `libfsext-20240501/pyfsext/pyfsext_file_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -222,22 +222,22 @@
 	  "get_sub_file_entry_by_name(name) -> Object or None\n"
 	  "\n"
 	  "Retrieves the sub file entry for an UTF-8 encoded name specified by the name." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyfsext_file_entry_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at the current offset." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyfsext_file_entry_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyfsext_file_entry_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -250,15 +250,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset of the data." },
 
 	{ "read",
 	  (PyCFunction) pyfsext_file_entry_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at the current offset." },
 
 	{ "seek",
 	  (PyCFunction) pyfsext_file_entry_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libfsext-20240301/pyfsext/pyfsext_datetime.c` & `libfsext-20240501/pyfsext/pyfsext_datetime.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/Makefile.in` & `libfsext-20240501/pyfsext/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -512,14 +512,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -580,16 +582,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -623,15 +625,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyfsext_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfsext_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -937,24 +940,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_error.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_extended_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_extended_attributes.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_file_entries.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_file_entry.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_integer.Plo
+	-rm -f ./$(DEPDIR)/pyfsext_la-pyfsext_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1048,14 +1063,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f setup.py
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/pyfsext/pyfsext_extended_attributes.c` & `libfsext-20240501/pyfsext/pyfsext_extended_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_volume.c` & `libfsext-20240501/pyfsext/pyfsext_volume.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_file_entries.c` & `libfsext-20240501/pyfsext/pyfsext_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/pyfsext/pyfsext_error.h` & `libfsext-20240501/pyfsext/pyfsext_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/INSTALL` & `libfsext-20240501/INSTALL`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_list_element.h` & `libfsext-20240501/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_array.h` & `libfsext-20240501/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_definitions.h` & `libfsext-20240501/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libfsext-20240301/libcdata/libcdata_libcerror.h` & `libfsext-20240501/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_unused.h` & `libfsext-20240501/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_btree.h` & `libfsext-20240501/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_btree.c` & `libfsext-20240501/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_support.c` & `libfsext-20240501/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_list.c` & `libfsext-20240501/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_extern.h` & `libfsext-20240501/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_list.h` & `libfsext-20240501/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_btree_values_list.h` & `libfsext-20240501/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/Makefile.am` & `libfsext-20240501/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libfsext-20240301/libcdata/libcdata_btree_node.h` & `libfsext-20240501/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_range_list_value.h` & `libfsext-20240501/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_range_list.h` & `libfsext-20240501/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_range_list.c` & `libfsext-20240501/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_array.c` & `libfsext-20240501/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_list_element.c` & `libfsext-20240501/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_libcthreads.h` & `libfsext-20240501/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_tree_node.h` & `libfsext-20240501/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_error.h` & `libfsext-20240501/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_types.h` & `libfsext-20240501/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_btree_node.c` & `libfsext-20240501/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_tree_node.c` & `libfsext-20240501/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_support.h` & `libfsext-20240501/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/Makefile.in` & `libfsext-20240501/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -482,14 +482,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -550,16 +552,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -576,15 +578,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -794,24 +797,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -905,17 +921,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libcdata/libcdata_range_list_value.c` & `libfsext-20240501/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_btree_values_list.c` & `libfsext-20240501/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcdata/libcdata_error.c` & `libfsext-20240501/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/config.sub` & `libfsext-20240501/config.sub`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/setup.py` & `libfsext-20240501/setup.py`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/acinclude.m4` & `libfsext-20240501/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libclocale.h` & `libfsext-20240501/fsexttools/fsexttools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_dokan.c` & `libfsext-20240501/fsexttools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_file_system.h` & `libfsext-20240501/fsexttools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_fuse.c` & `libfsext-20240501/fsexttools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/info_handle.h` & `libfsext-20240501/fsexttools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_signal.h` & `libfsext-20240501/fsexttools/fsexttools_signal.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_dokan.h` & `libfsext-20240501/fsexttools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libcerror.h` & `libfsext-20240501/fsexttools/fsexttools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/digest_hash.c` & `libfsext-20240501/fsexttools/digest_hash.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_file_system.c` & `libfsext-20240501/fsexttools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libcpath.h` & `libfsext-20240501/fsexttools/fsexttools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libfcache.h` & `libfsext-20240501/fsexttools/fsexttools_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_output.c` & `libfsext-20240501/fsexttools/fsexttools_output.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libfdata.h` & `libfsext-20240501/fsexttools/fsexttools_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/Makefile.am` & `libfsext-20240501/fsexttools/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -96,17 +96,15 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsext/libfsext.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on fsextinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fsextinfo_SOURCES)
```

### Comparing `libfsext-20240301/fsexttools/fsexttools_libhmac.h` & `libfsext-20240501/fsexttools/fsexttools_libhmac.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_file_entry.c` & `libfsext-20240501/fsexttools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/info_handle.c` & `libfsext-20240501/fsexttools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libuna.h` & `libfsext-20240501/fsexttools/fsexttools_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_file_entry.h` & `libfsext-20240501/fsexttools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libfdatetime.h` & `libfsext-20240501/fsexttools/fsexttools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsextmount.c` & `libfsext-20240501/fsexttools/fsextmount.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_output.h` & `libfsext-20240501/fsexttools/fsexttools_output.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsextinfo.c` & `libfsext-20240501/fsexttools/fsextinfo.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_handle.h` & `libfsext-20240501/fsexttools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libbfio.h` & `libfsext-20240501/fsexttools/fsexttools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_getopt.h` & `libfsext-20240501/fsexttools/fsexttools_getopt.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_unused.h` & `libfsext-20240501/fsexttools/fsexttools_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libcnotify.h` & `libfsext-20240501/fsexttools/fsexttools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_handle.c` & `libfsext-20240501/fsexttools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libfsext.h` & `libfsext-20240501/fsexttools/fsexttools_libfsext.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_getopt.c` & `libfsext-20240501/fsexttools/fsexttools_getopt.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_i18n.h` & `libfsext-20240501/fsexttools/fsexttools_i18n.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/Makefile.in` & `libfsext-20240501/fsexttools/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -469,14 +469,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -537,16 +539,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -633,15 +635,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsext/libfsext.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -898,23 +901,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/digest_hash.Po
+	-rm -f ./$(DEPDIR)/fsextinfo.Po
+	-rm -f ./$(DEPDIR)/fsextmount.Po
+	-rm -f ./$(DEPDIR)/fsexttools_getopt.Po
+	-rm -f ./$(DEPDIR)/fsexttools_output.Po
+	-rm -f ./$(DEPDIR)/fsexttools_signal.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1009,17 +1026,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on fsextinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fsextinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/fsexttools/digest_hash.h` & `libfsext-20240501/fsexttools/digest_hash.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_signal.c` & `libfsext-20240501/fsexttools/fsexttools_signal.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/fsexttools_libfguid.h` & `libfsext-20240501/fsexttools/fsexttools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/fsexttools/mount_fuse.h` & `libfsext-20240501/fsexttools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/config.rpath` & `libfsext-20240501/config.rpath`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext.spec.in` & `libfsext-20240501/libfsext.spec.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_thread.h` & `libfsext-20240501/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_read_write_lock.h` & `libfsext-20240501/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_thread.c` & `libfsext-20240501/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_thread_pool.h` & `libfsext-20240501/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_support.h` & `libfsext-20240501/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_lock.h` & `libfsext-20240501/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_unused.h` & `libfsext-20240501/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_lock.c` & `libfsext-20240501/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_condition.h` & `libfsext-20240501/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_repeating_thread.h` & `libfsext-20240501/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/Makefile.am` & `libfsext-20240501/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libfsext-20240301/libcthreads/libcthreads_support.c` & `libfsext-20240501/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_mutex.c` & `libfsext-20240501/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_queue.c` & `libfsext-20240501/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_mutex.h` & `libfsext-20240501/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_types.h` & `libfsext-20240501/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_thread_attributes.h` & `libfsext-20240501/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_condition.c` & `libfsext-20240501/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_error.c` & `libfsext-20240501/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_read_write_lock.c` & `libfsext-20240501/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_libcerror.h` & `libfsext-20240501/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_definitions.h` & `libfsext-20240501/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libfsext-20240301/libcthreads/libcthreads_thread_pool.c` & `libfsext-20240501/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_error.h` & `libfsext-20240501/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_thread_attributes.c` & `libfsext-20240501/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_extern.h` & `libfsext-20240501/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/libcthreads_repeating_thread.c` & `libfsext-20240501/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcthreads/Makefile.in` & `libfsext-20240501/libcthreads/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -486,14 +486,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -554,16 +556,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -578,15 +580,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -796,24 +799,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -907,17 +923,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libcthreads/libcthreads_queue.h` & `libfsext-20240501/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_bitmap.c` & `libfsext-20240501/libfsext/libfsext_bitmap.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_notify.c` & `libfsext-20240501/libfsext/libfsext_notify.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_block_vector.h` & `libfsext-20240501/libfsext/libfsext_block_vector.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_inode_table.h` & `libfsext-20240501/libfsext/libfsext_inode_table.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_file_entry.h` & `libfsext-20240501/libfsext/libfsext_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_bitmap.h` & `libfsext-20240501/libfsext/libfsext_bitmap.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extent.c` & `libfsext-20240501/libfsext/libfsext_extent.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_buffer_data_handle.c` & `libfsext-20240501/libfsext/libfsext_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_attribute_values.c` & `libfsext-20240501/libfsext/libfsext_attribute_values.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libuna.h` & `libfsext-20240501/libfsext/libfsext_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_attributes_block.h` & `libfsext-20240501/libfsext/libfsext_attributes_block.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libcerror.h` & `libfsext-20240501/libfsext/libfsext_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libfdata.h` & `libfsext-20240501/libfsext/libfsext_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_directory.c` & `libfsext-20240501/libfsext/libfsext_directory.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_volume.h` & `libfsext-20240501/libfsext/libfsext_volume.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_checksum.h` & `libfsext-20240501/libfsext/libfsext_checksum.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_support.h` & `libfsext-20240501/libfsext/libfsext_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libclocale.h` & `libfsext-20240501/libfsext/libfsext_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_error.h` & `libfsext-20240501/libfsext/libfsext_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_group_descriptor.h` & `libfsext-20240501/libfsext/libfsext_group_descriptor.h`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 extern "C" {
 #endif
 
 typedef struct libfsext_group_descriptor libfsext_group_descriptor_t;
 
 struct libfsext_group_descriptor
 {
+	/* Group number
+	 */
+	uint32_t group_number;
+
 	/* Block bitmap block number
 	 */
 	uint64_t block_bitmap_block_number;
 
 	/* Inode bitmap block number
 	 */
 	uint64_t inode_bitmap_block_number;
```

### Comparing `libfsext-20240301/libfsext/libfsext_block_data_handle.h` & `libfsext-20240501/libfsext/libfsext_block_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext.rc.in` & `libfsext-20240501/libfsext/libfsext.rc.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_error.c` & `libfsext-20240501/libfsext/libfsext_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_group_descriptor.c` & `libfsext-20240501/libfsext/libfsext_group_descriptor.c`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
  */
 
 #include <common.h>
 #include <byte_stream.h>
 #include <memory.h>
 #include <types.h>
 
+#include "libfsext_checksum.h"
 #include "libfsext_definitions.h"
 #include "libfsext_group_descriptor.h"
 #include "libfsext_io_handle.h"
 #include "libfsext_libbfio.h"
 #include "libfsext_libcerror.h"
 #include "libfsext_libcnotify.h"
 
@@ -142,22 +143,24 @@
 int libfsext_group_descriptor_read_data(
      libfsext_group_descriptor_t *group_descriptor,
      libfsext_io_handle_t *io_handle,
      const uint8_t *data,
      size_t data_size,
      libcerror_error_t **error )
 {
+	uint8_t checksum_data[ 4 ];
+	uint8_t empty_checksum_data[ 2 ]  = { 0, 0 };
+
 	static char *function             = "libfsext_group_descriptor_read_data";
 	size_t group_descriptor_data_size = 0;
 	uint64_t value_64bit              = 0;
+	uint32_t calculated_checksum      = 0;
+	uint32_t stored_checksum          = 0;
 	uint32_t value_32bit              = 0;
-
-#if defined( HAVE_DEBUG_OUTPUT )
 	uint16_t value_16bit              = 0;
-#endif
 
 	if( group_descriptor == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -327,14 +330,20 @@
 		 ( (fsext_group_descriptor_ext4_t *) data )->inode_bitmap_checksum_lower,
 		 group_descriptor->inode_bitmap_checksum );
 
 		byte_stream_copy_to_uint16_little_endian(
 		 ( (fsext_group_descriptor_ext4_t *) data )->number_of_unused_inodes_lower,
 		 group_descriptor->number_of_unused_inodes );
 
+		byte_stream_copy_to_uint16_little_endian(
+		 ( (fsext_group_descriptor_ext4_t *) data )->checksum,
+		 value_16bit );
+
+		stored_checksum = value_16bit;
+
 #if defined( HAVE_DEBUG_OUTPUT )
 		if( libcnotify_verbose != 0 )
 		{
 			libcnotify_printf(
 			 "%s: block bitmap block number (lower)\t\t: %" PRIu64 "\n",
 			 function,
 			 group_descriptor->block_bitmap_block_number );
@@ -583,29 +592,131 @@
 			 group_descriptor->number_of_directories );
 
 			libcnotify_printf(
 			 "%s: number of unused inodes\t\t\t: %" PRIu32 "\n",
 			 function,
 			 group_descriptor->number_of_unused_inodes );
 
-			libcnotify_printf(
-			 "%s: block bitmap checksum\t\t\t: 0x%04" PRIx32 "\n",
-			 function,
-			 group_descriptor->block_bitmap_checksum );
+			if( ( io_handle->read_only_compatible_features_flags & LIBFSEXT_READ_ONLY_COMPATIBLE_FEATURES_FLAG_METADATA_CHECKSUM ) != 0 )
+			{
+				libcnotify_printf(
+				 "%s: block bitmap checksum\t\t\t: 0x%08" PRIx32 "\n",
+				 function,
+				 group_descriptor->block_bitmap_checksum );
 
-			libcnotify_printf(
-			 "%s: inode bitmap checksum\t\t\t: 0x%04" PRIx32 "\n",
-			 function,
-			 group_descriptor->inode_bitmap_checksum );
+				libcnotify_printf(
+				 "%s: inode bitmap checksum\t\t\t: 0x%08" PRIx32 "\n",
+				 function,
+				 group_descriptor->inode_bitmap_checksum );
+			}
+			else
+			{
+				libcnotify_printf(
+				 "%s: block bitmap checksum\t\t\t: 0x%04" PRIx32 "\n",
+				 function,
+				 group_descriptor->block_bitmap_checksum );
 
+				libcnotify_printf(
+				 "%s: inode bitmap checksum\t\t\t: 0x%04" PRIx32 "\n",
+				 function,
+				 group_descriptor->inode_bitmap_checksum );
+			}
 			libcnotify_printf(
 			 "\n" );
 		}
 #endif /* defined( HAVE_DEBUG_OUTPUT ) */
 	}
+/* TODO add support for crc16 checksum */
+	if( ( io_handle->read_only_compatible_features_flags & LIBFSEXT_READ_ONLY_COMPATIBLE_FEATURES_FLAG_METADATA_CHECKSUM ) != 0 )
+	{
+		byte_stream_copy_from_uint32_little_endian(
+		 checksum_data,
+		 group_descriptor->group_number );
+
+		if( libfsext_checksum_calculate_crc32(
+		     &calculated_checksum,
+		     checksum_data,
+		     4,
+		     io_handle->metadata_checksum_seed,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+			 "%s: unable to calculate CRC-32.",
+			 function );
+
+			return( -1 );
+		}
+		if( libfsext_checksum_calculate_crc32(
+		     &calculated_checksum,
+		     data,
+		     30,
+		     calculated_checksum,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+			 "%s: unable to calculate CRC-32.",
+			 function );
+
+			return( -1 );
+		}
+		if( libfsext_checksum_calculate_crc32(
+		     &calculated_checksum,
+		     empty_checksum_data,
+		     2,
+		     calculated_checksum,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+			 "%s: unable to calculate CRC-32.",
+			 function );
+
+			return( -1 );
+		}
+		if( libfsext_checksum_calculate_crc32(
+		     &calculated_checksum,
+		     &( data[ 32 ] ),
+		     data_size - 32,
+		     calculated_checksum,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+			 "%s: unable to calculate CRC-32.",
+			 function );
+
+			return( -1 );
+		}
+		calculated_checksum = ( 0xffffffffUL - calculated_checksum ) & 0x0000ffffUL;
+
+		if( ( stored_checksum != 0 )
+		 && ( stored_checksum != calculated_checksum ) )
+		{
+#if defined( HAVE_DEBUG_OUTPUT )
+			if( libcnotify_verbose != 0 )
+			{
+				libcnotify_printf(
+				 "%s: mismatch in checksum ( 0x%08" PRIx32 " != 0x%08" PRIx32 " ).\n",
+				 function,
+				 stored_checksum,
+				 calculated_checksum );
+			}
+#endif
+		}
+	}
 	return( 1 );
 }
 
 /* Reads the group descriptor from a Basic File IO (bfio) handle
  * Returns 1 if successful or -1 on error
  */
 int libfsext_group_descriptor_read_file_io_handle(
```

### Comparing `libfsext-20240301/libfsext/fsext_extents.h` & `libfsext-20240501/libfsext/fsext_extents.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/Makefile.am` & `libfsext-20240501/libfsext/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -93,21 +93,19 @@
 libfsext_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfsext_definitions.h.in \
 	libfsext.rc \
 	libfsext.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsext_definitions.h \
+	libfsext.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfsext_definitions.h
-	-rm -f libfsext.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfsext ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfsext_la_SOURCES)
```

### Comparing `libfsext-20240301/libfsext/libfsext_extern.h` & `libfsext-20240501/libfsext/libfsext_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extent_index.c` & `libfsext-20240501/libfsext/libfsext_extent_index.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_attribute_values.h` & `libfsext-20240501/libfsext/libfsext_attribute_values.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/fsext_superblock.h` & `libfsext-20240501/libfsext/fsext_superblock.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_data_blocks.c` & `libfsext-20240501/libfsext/libfsext_data_blocks.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_checksum.c` & `libfsext-20240501/libfsext/libfsext_checksum.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extent.h` & `libfsext-20240501/libfsext/libfsext_extent.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libfcache.h` & `libfsext-20240501/libfsext/libfsext_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_block_data_handle.c` & `libfsext-20240501/libfsext/libfsext_block_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_data_blocks.h` & `libfsext-20240501/libfsext/libfsext_data_blocks.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extents_footer.c` & `libfsext-20240501/libfsext/libfsext_extents_footer.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_support.c` & `libfsext-20240501/libfsext/libfsext_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extents_header.c` & `libfsext-20240501/libfsext/libfsext_extents_header.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libcnotify.h` & `libfsext-20240501/libfsext/libfsext_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_directory.h` & `libfsext-20240501/libfsext/libfsext_directory.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libfguid.h` & `libfsext-20240501/libfsext/libfsext_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_directory_entry.c` & `libfsext-20240501/libfsext/libfsext_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extent_index.h` & `libfsext-20240501/libfsext/libfsext_extent_index.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extended_attribute.c` & `libfsext-20240501/libfsext/libfsext_extended_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extents_header.h` & `libfsext-20240501/libfsext/libfsext_extents_header.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_file_entry.c` & `libfsext-20240501/libfsext/libfsext_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_superblock.c` & `libfsext-20240501/libfsext/libfsext_superblock.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_block_vector.c` & `libfsext-20240501/libfsext/libfsext_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_definitions.h` & `libfsext-20240501/libfsext/libfsext_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBFSEXT )
 #include <libfsext/definitions.h>
 
 /* The definitions in <libfsext/definitions.h> are copied here
  * for local use of libfsext
  */
 #else
-#define LIBFSEXT_VERSION						20240301
+#define LIBFSEXT_VERSION						20240501
 
 /* The version string
  */
-#define LIBFSEXT_VERSION_STRING						"20240301"
+#define LIBFSEXT_VERSION_STRING						"20240501"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSEXT_ACCESS_FLAGS
```

### Comparing `libfsext-20240301/libfsext/libfsext.c` & `libfsext-20240501/libfsext/libfsext.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_volume.c` & `libfsext-20240501/libfsext/libfsext_volume.c`

 * *Files 0% similar despite different names*

```diff
@@ -1417,14 +1417,16 @@
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
 					 "%s: unable to create group descriptor.",
 					 function );
 
 					goto on_error;
 				}
+				group_descriptor->group_number = group_descriptor_index;
+
 				if( libfsext_group_descriptor_read_file_io_handle(
 				     group_descriptor,
 				     internal_volume->io_handle,
 				     file_io_handle,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
```

### Comparing `libfsext-20240301/libfsext/libfsext_inode.c` & `libfsext-20240501/libfsext/libfsext_inode.c`

 * *Files 1% similar despite different names*

```diff
@@ -402,15 +402,14 @@
 
 /* Reads the inode data
  * Returns 1 if successful or -1 on error
  */
 int libfsext_inode_read_data(
      libfsext_inode_t *inode,
      libfsext_io_handle_t *io_handle,
-     uint32_t inode_number,
      const uint8_t *data,
      size_t data_size,
      libcerror_error_t **error )
 {
 	uint8_t checksum_data[ 4 ];
 	uint8_t empty_checksum_data[ 2 ]     = { 0, 0 };
 
@@ -1516,15 +1515,15 @@
 	}
 #endif /* defined( HAVE_DEBUG_OUTPUT ) */
 
 	if( ( io_handle->read_only_compatible_features_flags & LIBFSEXT_READ_ONLY_COMPATIBLE_FEATURES_FLAG_METADATA_CHECKSUM ) != 0 )
 	{
 		byte_stream_copy_from_uint32_little_endian(
 		 checksum_data,
-		 inode_number + 1 );
+		 inode->inode_number );
 
 		if( libfsext_checksum_calculate_crc32(
 		     &calculated_checksum,
 		     checksum_data,
 		     4,
 		     io_handle->metadata_checksum_seed,
 		     error ) != 1 )
@@ -2558,15 +2557,15 @@
 	static char *function   = "libfsext_inode_read_element_data";
 	ssize_t read_count      = 0;
 
 	LIBFSEXT_UNREFERENCED_PARAMETER( element_data_file_index )
 	LIBFSEXT_UNREFERENCED_PARAMETER( element_flags )
 	LIBFSEXT_UNREFERENCED_PARAMETER( read_flags )
 
-	if( (uint64_t) element_index > (uint64_t) UINT32_MAX )
+	if( (uint64_t) element_index > (uint64_t) ( UINT32_MAX - 1 ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 		 "%s: element index value out of bounds.",
 		 function );
@@ -2638,18 +2637,19 @@
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
 		 "%s: unable to create inode.",
 		 function );
 
 		goto on_error;
 	}
+	inode->inode_number = (uint32_t) element_index + 1;
+
 	if( libfsext_inode_read_data(
 	     inode,
 	     io_handle,
-	     (uint32_t) element_index,
 	     data,
 	     (size_t) element_data_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_IO,
```

### Comparing `libfsext-20240301/libfsext/libfsext_notify.h` & `libfsext-20240501/libfsext/libfsext_notify.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_block_stream.h` & `libfsext-20240501/libfsext/libfsext_block_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/fsext_attributes.h` & `libfsext-20240501/libfsext/fsext_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extents.h` & `libfsext-20240501/libfsext/libfsext_extents.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_superblock.h` & `libfsext-20240501/libfsext/libfsext_superblock.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_io_handle.h` & `libfsext-20240501/libfsext/libfsext_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_block_stream.c` & `libfsext-20240501/libfsext/libfsext_block_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extended_attribute.h` & `libfsext-20240501/libfsext/libfsext_extended_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/fsext_inode.h` & `libfsext-20240501/libfsext/fsext_inode.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extents.c` & `libfsext-20240501/libfsext/libfsext_extents.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libcdata.h` & `libfsext-20240501/libfsext/libfsext_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_debug.c` & `libfsext-20240501/libfsext/libfsext_debug.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_definitions.h.in` & `libfsext-20240501/libfsext/libfsext_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/fsext_group_descriptor.h` & `libfsext-20240501/libfsext/fsext_group_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libfdatetime.h` & `libfsext-20240501/libfsext/libfsext_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/Makefile.in` & `libfsext-20240501/libfsext/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -525,14 +525,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -593,16 +595,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -689,15 +691,18 @@
 
 libfsext_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfsext_definitions.h.in \
 	libfsext.rc \
 	libfsext.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsext_definitions.h \
+	libfsext.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -957,24 +962,56 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfsext.Plo
+	-rm -f ./$(DEPDIR)/libfsext_attribute_values.Plo
+	-rm -f ./$(DEPDIR)/libfsext_attributes_block.Plo
+	-rm -f ./$(DEPDIR)/libfsext_bitmap.Plo
+	-rm -f ./$(DEPDIR)/libfsext_block.Plo
+	-rm -f ./$(DEPDIR)/libfsext_block_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsext_block_stream.Plo
+	-rm -f ./$(DEPDIR)/libfsext_block_vector.Plo
+	-rm -f ./$(DEPDIR)/libfsext_buffer_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsext_checksum.Plo
+	-rm -f ./$(DEPDIR)/libfsext_data_blocks.Plo
+	-rm -f ./$(DEPDIR)/libfsext_debug.Plo
+	-rm -f ./$(DEPDIR)/libfsext_directory.Plo
+	-rm -f ./$(DEPDIR)/libfsext_directory_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsext_error.Plo
+	-rm -f ./$(DEPDIR)/libfsext_extended_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsext_extent.Plo
+	-rm -f ./$(DEPDIR)/libfsext_extent_index.Plo
+	-rm -f ./$(DEPDIR)/libfsext_extents.Plo
+	-rm -f ./$(DEPDIR)/libfsext_extents_footer.Plo
+	-rm -f ./$(DEPDIR)/libfsext_extents_header.Plo
+	-rm -f ./$(DEPDIR)/libfsext_file_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsext_group_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfsext_inode.Plo
+	-rm -f ./$(DEPDIR)/libfsext_inode_table.Plo
+	-rm -f ./$(DEPDIR)/libfsext_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsext_notify.Plo
+	-rm -f ./$(DEPDIR)/libfsext_superblock.Plo
+	-rm -f ./$(DEPDIR)/libfsext_support.Plo
+	-rm -f ./$(DEPDIR)/libfsext_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1087,19 +1124,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfsext_definitions.h
-	-rm -f libfsext.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfsext ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfsext_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libfsext/libfsext_inode.h` & `libfsext-20240501/libfsext/libfsext_inode.h`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 extern "C" {
 #endif
 
 typedef struct libfsext_inode libfsext_inode_t;
 
 struct libfsext_inode
 {
+	/* Inode number
+	 */
+	uint32_t inode_number;
+
 	/* File mode
 	 */
 	uint16_t file_mode;
 
 	/* Data size
 	 */
 	uint64_t data_size;
@@ -150,15 +154,14 @@
      libfsext_inode_t **destination_inode,
      libfsext_inode_t *source_inode,
      libcerror_error_t **error );
 
 int libfsext_inode_read_data(
      libfsext_inode_t *inode,
      libfsext_io_handle_t *io_handle,
-     uint32_t inode_number,
      const uint8_t *data,
      size_t data_size,
      libcerror_error_t **error );
 
 int libfsext_inode_read_data_reference(
      libfsext_inode_t *inode,
      libfsext_io_handle_t *io_handle,
```

### Comparing `libfsext-20240301/libfsext/libfsext_buffer_data_handle.h` & `libfsext-20240501/libfsext/libfsext_buffer_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_block.h` & `libfsext-20240501/libfsext/libfsext_block.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext.rc` & `libfsext-20240501/libfsext/libfsext.rc`

 * *Files 11% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support the Extended File System (ext) format\0"
-      VALUE "FileVersion",		"20240301" "\0"
+      VALUE "FileVersion",		"20240501" "\0"
       VALUE "InternalName",		"libfsext.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfsext.dll\0"
       VALUE "ProductName",		"libfsext\0"
-      VALUE "ProductVersion",		"20240301" "\0"
+      VALUE "ProductVersion",		"20240501" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfsext/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfsext-20240301/libfsext/libfsext_attributes_block.c` & `libfsext-20240501/libfsext/libfsext_attributes_block.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_debug.h` & `libfsext-20240501/libfsext/libfsext_debug.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_inode_table.c` & `libfsext-20240501/libfsext/libfsext_inode_table.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/fsext_directory_entry.h` & `libfsext-20240501/libfsext/fsext_directory_entry.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libcthreads.h` & `libfsext-20240501/libfsext/libfsext_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_extents_footer.h` & `libfsext-20240501/libfsext/libfsext_extents_footer.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_types.h` & `libfsext-20240501/libfsext/libfsext_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_directory_entry.h` & `libfsext-20240501/libfsext/libfsext_directory_entry.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_io_handle.c` & `libfsext-20240501/libfsext/libfsext_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_libbfio.h` & `libfsext-20240501/libfsext/libfsext_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_block.c` & `libfsext-20240501/libfsext/libfsext_block.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfsext/libfsext_unused.h` & `libfsext-20240501/libfsext/libfsext_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/test-driver` & `libfsext-20240501/test-driver`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_support.c` & `libfsext-20240501/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_libcerror.h` & `libfsext-20240501/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_definitions.h` & `libfsext-20240501/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libfsext-20240301/libcpath/Makefile.am` & `libfsext-20240501/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libfsext-20240301/libcpath/libcpath_error.c` & `libfsext-20240501/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_extern.h` & `libfsext-20240501/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_system_string.h` & `libfsext-20240501/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_support.h` & `libfsext-20240501/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_libcsplit.h` & `libfsext-20240501/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_system_string.c` & `libfsext-20240501/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_libclocale.h` & `libfsext-20240501/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_error.h` & `libfsext-20240501/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/Makefile.in` & `libfsext-20240501/libcpath/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -462,14 +462,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -530,16 +532,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -551,15 +553,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -762,24 +765,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -866,17 +875,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libcpath/libcpath_libuna.h` & `libfsext-20240501/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_unused.h` & `libfsext-20240501/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_path.c` & `libfsext-20240501/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcpath/libcpath_path.h` & `libfsext-20240501/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/ChangeLog` & `libfsext-20240501/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/manuals/fsextinfo.1` & `libfsext-20240501/manuals/fsextinfo.1`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/manuals/fsextmount.1` & `libfsext-20240501/manuals/fsextmount.1`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/manuals/Makefile.in` & `libfsext-20240501/manuals/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -435,14 +435,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -512,15 +514,16 @@
 	libfsext.3
 
 EXTRA_DIST = \
 	fsextinfo.1 \
 	fsextmount.1 \
 	libfsext.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -713,23 +716,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -811,13 +816,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/manuals/libfsext.3` & `libfsext-20240501/manuals/libfsext.3`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_libfsext.h` & `libfsext-20240501/tests/fsext_test_libfsext.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_extents_header.c` & `libfsext-20240501/tests/fsext_test_extents_header.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_attribute_values.c` & `libfsext-20240501/tests/fsext_test_attribute_values.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_block.c` & `libfsext-20240501/tests/fsext_test_block.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_memory.h` & `libfsext-20240501/tests/fsext_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_file_entry.c` & `libfsext-20240501/tests/fsext_test_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_inode_table.c` & `libfsext-20240501/tests/fsext_test_inode_table.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_checksum.c` & `libfsext-20240501/tests/fsext_test_checksum.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/test_tools.sh` & `libfsext-20240501/tests/test_tools.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libfsext-20240301/tests/fsext_test_support.c` & `libfsext-20240501/tests/fsext_test_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_block_data_handle.c` & `libfsext-20240501/tests/fsext_test_block_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_tools_signal.c` & `libfsext-20240501/tests/fsext_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_functions.c` & `libfsext-20240501/tests/fsext_test_functions.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_io_handle.c` & `libfsext-20240501/tests/fsext_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_superblock.c` & `libfsext-20240501/tests/fsext_test_superblock.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_directory_entry.c` & `libfsext-20240501/tests/fsext_test_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/Makefile.am` & `libfsext-20240501/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -519,13 +519,12 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsext/libfsext.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@PTHREAD_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libfsext-20240301/tests/fsext_test_extended_attribute.c` & `libfsext-20240501/tests/fsext_test_extended_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_volume.c` & `libfsext-20240501/tests/fsext_test_volume.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_error.c` & `libfsext-20240501/tests/fsext_test_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_macros.h` & `libfsext-20240501/tests/fsext_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_group_descriptor.c` & `libfsext-20240501/tests/fsext_test_group_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/pyfsext_test_volume.py` & `libfsext-20240501/tests/pyfsext_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_libfdata.h` & `libfsext-20240501/tests/fsext_test_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_libuna.h` & `libfsext-20240501/tests/fsext_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_inode.c` & `libfsext-20240501/tests/fsext_test_inode.c`

 * *Files 0% similar despite different names*

```diff
@@ -757,15 +757,14 @@
 	 */
 	io_handle->format_version = 3;
 	io_handle->inode_size     = 0;
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data1,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -777,15 +776,14 @@
 
 	io_handle->format_version = 4;
 	io_handle->inode_size     = 128;
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data2,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -797,15 +795,14 @@
 
 	io_handle->format_version = 4;
 	io_handle->inode_size     = 128;
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data3,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -822,15 +819,14 @@
 
 	io_handle->format_version = 2;
 	io_handle->inode_size     = 0;
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data4,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -849,15 +845,14 @@
 	 */
 	io_handle->format_version = 3;
 	io_handle->inode_size     = 0;
 
 	result = libfsext_inode_read_data(
 	          NULL,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data1,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -869,15 +864,14 @@
 
 	libcerror_error_free(
 	 &error );
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          NULL,
-	          0,
 	          fsext_test_inode_data1,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -889,15 +883,14 @@
 
 	libcerror_error_free(
 	 &error );
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          NULL,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -909,15 +902,14 @@
 
 	libcerror_error_free(
 	 &error );
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data1,
 	          (size_t) SSIZE_MAX + 1,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -929,15 +921,14 @@
 
 	libcerror_error_free(
 	 &error );
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data1,
 	          0,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -2077,15 +2068,14 @@
 	FSEXT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data3,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
```

### Comparing `libfsext-20240301/tests/test_python_module.sh` & `libfsext-20240501/tests/test_python_module.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="volume";
 OPTION_SETS=("offset");
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libfsext";
+PYTHON_MODULE="pyfsext";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfsext_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfsext_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyfsext");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libfsext-20240301/tests/fsext_test_getopt.c` & `libfsext-20240501/tests/fsext_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_extents_footer.c` & `libfsext-20240501/tests/fsext_test_extents_footer.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_bitmap.c` & `libfsext-20240501/tests/fsext_test_bitmap.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_extent_index.c` & `libfsext-20240501/tests/fsext_test_extent_index.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_directory.c` & `libfsext-20240501/tests/fsext_test_directory.c`

 * *Files 0% similar despite different names*

```diff
@@ -466,15 +466,14 @@
 	FSEXT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data1,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -1063,15 +1062,14 @@
 	FSEXT_TEST_ASSERT_IS_NULL(
 	 "error",
 	 error );
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data1,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
```

### Comparing `libfsext-20240301/tests/fsext_test_functions.h` & `libfsext-20240501/tests/fsext_test_functions.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_libbfio.h` & `libfsext-20240501/tests/fsext_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/test_runner.sh` & `libfsext-20240501/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_extent.c` & `libfsext-20240501/tests/fsext_test_extent.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_notify.c` & `libfsext-20240501/tests/fsext_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_block_vector.c` & `libfsext-20240501/tests/fsext_test_block_vector.c`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
 
 	io_handle->format_version = 3;
 	io_handle->inode_size     = 0;
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data1,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
@@ -465,15 +464,14 @@
 
 	io_handle->format_version = 3;
 	io_handle->inode_size     = 0;
 
 	result = libfsext_inode_read_data(
 	          inode,
 	          io_handle,
-	          0,
 	          fsext_test_inode_data1,
 	          128,
 	          &error );
 
 	FSEXT_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
```

### Comparing `libfsext-20240301/tests/test_fsextinfo.sh` & `libfsext-20240501/tests/test_fsextinfo.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("fsextinfo" "fsextinfo_fs");
 OPTIONS_PER_PROFILE=("" "-H");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libfsext-20240301/tests/fsext_test_libfcache.h` & `libfsext-20240501/tests/fsext_test_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_libclocale.h` & `libfsext-20240501/tests/fsext_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_libcnotify.h` & `libfsext-20240501/tests/fsext_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_getopt.h` & `libfsext-20240501/tests/fsext_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/Makefile.in` & `libfsext-20240501/tests/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -882,14 +882,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -951,16 +953,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1442,16 +1444,18 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsext/libfsext.la \
 	@LIBCTHREADS_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@PTHREAD_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1997,24 +2001,60 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../fsexttools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../fsexttools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../fsexttools/$(DEPDIR)/digest_hash.Po
+	-rm -f ../fsexttools/$(DEPDIR)/fsexttools_output.Po
+	-rm -f ../fsexttools/$(DEPDIR)/fsexttools_signal.Po
+	-rm -f ../fsexttools/$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/fsext_test_attribute_values.Po
+	-rm -f ./$(DEPDIR)/fsext_test_bitmap.Po
+	-rm -f ./$(DEPDIR)/fsext_test_block.Po
+	-rm -f ./$(DEPDIR)/fsext_test_block_data_handle.Po
+	-rm -f ./$(DEPDIR)/fsext_test_block_vector.Po
+	-rm -f ./$(DEPDIR)/fsext_test_buffer_data_handle.Po
+	-rm -f ./$(DEPDIR)/fsext_test_checksum.Po
+	-rm -f ./$(DEPDIR)/fsext_test_directory.Po
+	-rm -f ./$(DEPDIR)/fsext_test_directory_entry.Po
+	-rm -f ./$(DEPDIR)/fsext_test_error.Po
+	-rm -f ./$(DEPDIR)/fsext_test_extended_attribute.Po
+	-rm -f ./$(DEPDIR)/fsext_test_extent.Po
+	-rm -f ./$(DEPDIR)/fsext_test_extent_index.Po
+	-rm -f ./$(DEPDIR)/fsext_test_extents_footer.Po
+	-rm -f ./$(DEPDIR)/fsext_test_extents_header.Po
+	-rm -f ./$(DEPDIR)/fsext_test_file_entry.Po
+	-rm -f ./$(DEPDIR)/fsext_test_functions.Po
+	-rm -f ./$(DEPDIR)/fsext_test_getopt.Po
+	-rm -f ./$(DEPDIR)/fsext_test_group_descriptor.Po
+	-rm -f ./$(DEPDIR)/fsext_test_inode.Po
+	-rm -f ./$(DEPDIR)/fsext_test_inode_table.Po
+	-rm -f ./$(DEPDIR)/fsext_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/fsext_test_memory.Po
+	-rm -f ./$(DEPDIR)/fsext_test_notify.Po
+	-rm -f ./$(DEPDIR)/fsext_test_superblock.Po
+	-rm -f ./$(DEPDIR)/fsext_test_support.Po
+	-rm -f ./$(DEPDIR)/fsext_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/fsext_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/fsext_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/fsext_test_volume.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2131,13 +2171,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/tests/fsext_test_tools_output.c` & `libfsext-20240501/tests/fsext_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_tools_info_handle.c` & `libfsext-20240501/tests/fsext_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_libcerror.h` & `libfsext-20240501/tests/fsext_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_memory.c` & `libfsext-20240501/tests/fsext_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_buffer_data_handle.c` & `libfsext-20240501/tests/fsext_test_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/pyfsext_test_support.py` & `libfsext-20240501/tests/pyfsext_test_support.py`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/fsext_test_unused.h` & `libfsext-20240501/tests/fsext_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/tests/test_library.sh` & `libfsext-20240501/tests/test_library.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="attribute_values bitmap block block_data_handle block_vector buffer_data_handle checksum directory directory_entry error extended_attribute extent extent_index extents_footer extents_header file_entry group_descriptor inode inode_table io_handle notify superblock";
 LIBRARY_TESTS_WITH_INPUT="support volume";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libfsext-20240301/ossfuzz/volume_fuzzer.cc` & `libfsext-20240501/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/ossfuzz/Makefile.am` & `libfsext-20240501/ossfuzz/Makefile.am`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -67,20 +67,18 @@
 	../libfsext/libfsext.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on extended_attribute_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(extended_attribute_fuzzer_SOURCES)
 	@echo "Running splint on file_entry_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_entry_fuzzer_SOURCES)
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libfsext-20240301/ossfuzz/ossfuzz_libfsext.h` & `libfsext-20240501/ossfuzz/ossfuzz_libfsext.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/ossfuzz/ossfuzz_libbfio.h` & `libfsext-20240501/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/ossfuzz/file_entry_fuzzer.cc` & `libfsext-20240501/ossfuzz/file_entry_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/ossfuzz/extended_attribute_fuzzer.cc` & `libfsext-20240501/ossfuzz/extended_attribute_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/ossfuzz/Makefile.in` & `libfsext-20240501/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -496,14 +496,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -564,16 +566,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -629,15 +631,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfsext/libfsext.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -889,23 +892,28 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/extended_attribute_fuzzer.Po
+	-rm -f ./$(DEPDIR)/file_entry_fuzzer.Po
+	-rm -f ./$(DEPDIR)/volume_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -991,17 +999,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on extended_attribute_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(extended_attribute_fuzzer_SOURCES)
 	@echo "Running splint on file_entry_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_entry_fuzzer_SOURCES)
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libfsext-20240301/ltmain.sh` & `libfsext-20240501/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha1_context.c` & `libfsext-20240501/libhmac/libhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha224.h` & `libfsext-20240501/libhmac/libhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha512_context.c` & `libfsext-20240501/libhmac/libhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_extern.h` & `libfsext-20240501/libhmac/libhmac_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_md5.c` & `libfsext-20240501/libhmac/libhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_md5.h` & `libfsext-20240501/libhmac/libhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_error.h` & `libfsext-20240501/libhmac/libhmac_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_types.h` & `libfsext-20240501/libhmac/libhmac_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_byte_stream.h` & `libfsext-20240501/libhmac/libhmac_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha512.c` & `libfsext-20240501/libhmac/libhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha256_context.c` & `libfsext-20240501/libhmac/libhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha224.c` & `libfsext-20240501/libhmac/libhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_definitions.h` & `libfsext-20240501/libhmac/libhmac_definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBHMAC )
 #include <libhmac/definitions.h>
 
 /* The definitions in <libhmac/definitions.h> are copied here
  * for local use of libhmac
  */
 #else
-#define LIBHMAC_VERSION			20240129
+#define LIBHMAC_VERSION			20240417
 
 /* The libhmac version string
  */
-#define LIBHMAC_VERSION_STRING		"20240129"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libfsext-20240301/libhmac/libhmac_unused.h` & `libfsext-20240501/libhmac/libhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha1.h` & `libfsext-20240501/libhmac/libhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha256_context.h` & `libfsext-20240501/libhmac/libhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/Makefile.am` & `libfsext-20240501/libhmac/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBHMAC
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libhmac.la
 
 libhmac_la_SOURCES = \
@@ -25,19 +25,17 @@
 	libhmac_sha512.c libhmac_sha512.h \
 	libhmac_sha512_context.c libhmac_sha512_context.h \
 	libhmac_support.c libhmac_support.h \
 	libhmac_types.h \
 	libhmac_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
```

### Comparing `libfsext-20240301/libhmac/libhmac_sha224_context.c` & `libfsext-20240501/libhmac/libhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_md5_context.h` & `libfsext-20240501/libhmac/libhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha256.c` & `libfsext-20240501/libhmac/libhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha1_context.h` & `libfsext-20240501/libhmac/libhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_libcerror.h` & `libfsext-20240501/libhmac/libhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_error.c` & `libfsext-20240501/libhmac/libhmac_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_support.h` & `libfsext-20240501/libhmac/libhmac_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/Makefile.in` & `libfsext-20240501/libhmac/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -485,14 +485,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -553,16 +555,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBHMAC_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCRYPTO_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBHMAC_TRUE@noinst_LTLIBRARIES = libhmac.la
 @HAVE_LOCAL_LIBHMAC_TRUE@libhmac_la_SOURCES = \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_byte_stream.h \
@@ -580,15 +582,16 @@
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha256_context.c libhmac_sha256_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512.c libhmac_sha512.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512_context.c libhmac_sha512_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_support.c libhmac_support.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_types.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -799,24 +802,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libhmac_error.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -911,17 +928,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libhmac/libhmac_sha256.h` & `libfsext-20240501/libhmac/libhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha224_context.h` & `libfsext-20240501/libhmac/libhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha512_context.h` & `libfsext-20240501/libhmac/libhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha512.h` & `libfsext-20240501/libhmac/libhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_support.c` & `libfsext-20240501/libhmac/libhmac_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_sha1.c` & `libfsext-20240501/libhmac/libhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libhmac/libhmac_md5_context.c` & `libfsext-20240501/libhmac/libhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_narrow_string.c` & `libfsext-20240501/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_definitions.h` & `libfsext-20240501/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libfsext-20240301/libcsplit/libcsplit_types.h` & `libfsext-20240501/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_wide_split_string.c` & `libfsext-20240501/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_support.h` & `libfsext-20240501/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/Makefile.am` & `libfsext-20240501/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libfsext-20240301/libcsplit/libcsplit_libcerror.h` & `libfsext-20240501/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_wide_string.c` & `libfsext-20240501/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_unused.h` & `libfsext-20240501/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_wide_split_string.h` & `libfsext-20240501/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_error.c` & `libfsext-20240501/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_narrow_split_string.c` & `libfsext-20240501/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_extern.h` & `libfsext-20240501/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_error.h` & `libfsext-20240501/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_support.c` & `libfsext-20240501/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_wide_string.h` & `libfsext-20240501/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/Makefile.in` & `libfsext-20240501/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -472,14 +472,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -540,16 +542,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -558,15 +560,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -771,24 +774,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -877,17 +888,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libcsplit/libcsplit_narrow_split_string.h` & `libfsext-20240501/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcsplit/libcsplit_narrow_string.h` & `libfsext-20240501/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/po/remove-potcdate.sin` & `libfsext-20240501/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/po/Makefile.in.in` & `libfsext-20240501/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/po/en@quot.header` & `libfsext-20240501/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/po/en@boldquot.header` & `libfsext-20240501/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/po/insert-header.sin` & `libfsext-20240501/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/po/Makevars` & `libfsext-20240501/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/po/Makevars.in` & `libfsext-20240501/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/po/Rules-quot` & `libfsext-20240501/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1251.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf16_string.c` & `libfsext-20240501/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_base16_stream.c` & `libfsext-20240501/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf8_stream.h` & `libfsext-20240501/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_2.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_932.c` & `libfsext-20240501/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_dingbats.h` & `libfsext-20240501/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf8_string.c` & `libfsext-20240501/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_base64_stream.c` & `libfsext-20240501/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_error.h` & `libfsext-20240501/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_turkish.h` & `libfsext-20240501/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_unicode_character.c` & `libfsext-20240501/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_gaelic.c` & `libfsext-20240501/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_arabic.h` & `libfsext-20240501/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_thai.c` & `libfsext-20240501/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_874.h` & `libfsext-20240501/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_15.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf8_string.h` & `libfsext-20240501/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_16.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1255.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf7_stream.c` & `libfsext-20240501/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_byte_stream.h` & `libfsext-20240501/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_koi8_u.c` & `libfsext-20240501/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_unused.h` & `libfsext-20240501/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_6.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_14.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_base64_stream.h` & `libfsext-20240501/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_error.c` & `libfsext-20240501/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_centraleurroman.h` & `libfsext-20240501/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_romanian.c` & `libfsext-20240501/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_6.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_9.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_russian.h` & `libfsext-20240501/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_dingbats.c` & `libfsext-20240501/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_15.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_936.c` & `libfsext-20240501/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_croatian.h` & `libfsext-20240501/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_scsu.h` & `libfsext-20240501/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/Makefile.am` & `libfsext-20240501/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libfsext-20240301/libuna/libuna_utf32_stream.c` & `libfsext-20240501/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_936.h` & `libfsext-20240501/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_10.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_roman.c` & `libfsext-20240501/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf7_stream.h` & `libfsext-20240501/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_3.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_thai.h` & `libfsext-20240501/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_farsi.h` & `libfsext-20240501/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_ukrainian.c` & `libfsext-20240501/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_inuit.c` & `libfsext-20240501/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_932.h` & `libfsext-20240501/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_874.c` & `libfsext-20240501/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_5.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_10.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_definitions.h` & `libfsext-20240501/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libfsext-20240301/libuna/libuna_url_stream.h` & `libfsext-20240501/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_icelandic.h` & `libfsext-20240501/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_koi8_u.h` & `libfsext-20240501/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf16_stream.c` & `libfsext-20240501/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1253.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_4.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_greek.c` & `libfsext-20240501/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_libcerror.h` & `libfsext-20240501/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_centraleurroman.c` & `libfsext-20240501/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1254.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_13.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_7.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1255.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_unicode_character.h` & `libfsext-20240501/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_8.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_13.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_949.h` & `libfsext-20240501/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_cyrillic.c` & `libfsext-20240501/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_celtic.c` & `libfsext-20240501/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_support.h` & `libfsext-20240501/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_4.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_949.c` & `libfsext-20240501/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf16_stream.h` & `libfsext-20240501/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_symbol.c` & `libfsext-20240501/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_roman.h` & `libfsext-20240501/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1257.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1254.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_950.c` & `libfsext-20240501/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_extern.h` & `libfsext-20240501/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1256.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_types.h` & `libfsext-20240501/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_base32_stream.h` & `libfsext-20240501/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1253.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_16.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf8_stream.c` & `libfsext-20240501/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1250.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_2.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_support.c` & `libfsext-20240501/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_koi8_r.c` & `libfsext-20240501/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_5.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf16_string.h` & `libfsext-20240501/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf32_string.c` & `libfsext-20240501/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_icelandic.c` & `libfsext-20240501/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1256.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf32_string.h` & `libfsext-20240501/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_romanian.h` & `libfsext-20240501/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_8.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_koi8_r.h` & `libfsext-20240501/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_cyrillic.h` & `libfsext-20240501/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_arabic.c` & `libfsext-20240501/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_croatian.c` & `libfsext-20240501/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_9.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_greek.h` & `libfsext-20240501/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1258.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_7.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/Makefile.in` & `libfsext-20240501/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -640,14 +640,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -708,16 +710,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -783,15 +785,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1053,24 +1056,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1216,17 +1284,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_3.c` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1250.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_scsu.c` & `libfsext-20240501/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1252.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_turkish.c` & `libfsext-20240501/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_ukrainian.h` & `libfsext-20240501/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_russian.c` & `libfsext-20240501/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1258.c` & `libfsext-20240501/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_celtic.h` & `libfsext-20240501/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_byte_stream.c` & `libfsext-20240501/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_gaelic.h` & `libfsext-20240501/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_utf32_stream.h` & `libfsext-20240501/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_symbol.h` & `libfsext-20240501/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1257.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_inuit.h` & `libfsext-20240501/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_mac_farsi.c` & `libfsext-20240501/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_950.h` & `libfsext-20240501/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_url_stream.c` & `libfsext-20240501/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1251.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_windows_1252.h` & `libfsext-20240501/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_codepage_iso_8859_14.h` & `libfsext-20240501/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_base16_stream.h` & `libfsext-20240501/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libuna/libuna_base32_stream.c` & `libfsext-20240501/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/Makefile.in` & `libfsext-20240501/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -522,14 +522,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -654,16 +656,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libfsext.pc \
+	libfsext.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfsext.pc
 
 all: all-recursive
 
@@ -1080,23 +1089,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1207,22 +1219,10 @@
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfsext && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfsext.pc
-	-rm -f libfsext.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsext-20240301/libcnotify/libcnotify_definitions.h` & `libfsext-20240501/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libfsext-20240301/libcnotify/libcnotify_extern.h` & `libfsext-20240501/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/libcnotify_support.c` & `libfsext-20240501/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/libcnotify_stream.h` & `libfsext-20240501/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/Makefile.am` & `libfsext-20240501/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libfsext-20240301/libcnotify/libcnotify_unused.h` & `libfsext-20240501/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/libcnotify_verbose.h` & `libfsext-20240501/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/libcnotify_print.h` & `libfsext-20240501/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/libcnotify_stream.c` & `libfsext-20240501/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/libcnotify_support.h` & `libfsext-20240501/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/libcnotify_verbose.c` & `libfsext-20240501/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/Makefile.in` & `libfsext-20240501/libcnotify/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -464,14 +464,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -532,30 +534,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -758,24 +761,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -862,17 +871,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libcnotify/libcnotify_libcerror.h` & `libfsext-20240501/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcnotify/libcnotify_print.c` & `libfsext-20240501/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/libcerror_system.c` & `libfsext-20240501/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/libcerror_error.c` & `libfsext-20240501/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/libcerror_extern.h` & `libfsext-20240501/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/Makefile.am` & `libfsext-20240501/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libfsext-20240301/libcerror/libcerror_types.h` & `libfsext-20240501/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/libcerror_support.h` & `libfsext-20240501/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/libcerror_error.h` & `libfsext-20240501/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/libcerror_system.h` & `libfsext-20240501/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/libcerror_definitions.h` & `libfsext-20240501/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libfsext-20240301/libcerror/libcerror_support.c` & `libfsext-20240501/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/libcerror_unused.h` & `libfsext-20240501/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libcerror/Makefile.in` & `libfsext-20240501/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -529,28 +531,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -752,24 +755,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -855,17 +863,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_floatingtime.h` & `libfsext-20240501/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_nsf_timedate.c` & `libfsext-20240501/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_error.h` & `libfsext-20240501/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_floatingtime.c` & `libfsext-20240501/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_support.h` & `libfsext-20240501/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_hfs_time.h` & `libfsext-20240501/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_definitions.h` & `libfsext-20240501/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_hfs_time.c` & `libfsext-20240501/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/Makefile.am` & `libfsext-20240501/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_filetime.c` & `libfsext-20240501/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_systemtime.h` & `libfsext-20240501/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_extern.h` & `libfsext-20240501/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_posix_time.c` & `libfsext-20240501/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_unused.h` & `libfsext-20240501/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_fat_date_time.h` & `libfsext-20240501/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_systemtime.c` & `libfsext-20240501/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_nsf_timedate.h` & `libfsext-20240501/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_libcerror.h` & `libfsext-20240501/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_support.c` & `libfsext-20240501/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_error.c` & `libfsext-20240501/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_posix_time.h` & `libfsext-20240501/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_date_time_values.h` & `libfsext-20240501/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_filetime.h` & `libfsext-20240501/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_date_time_values.c` & `libfsext-20240501/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_types.h` & `libfsext-20240501/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/libfdatetime/Makefile.in` & `libfsext-20240501/libfdatetime/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -483,14 +483,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -551,16 +553,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -573,15 +575,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -790,24 +793,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -900,17 +915,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsext-20240301/libfdatetime/libfdatetime_fat_date_time.c` & `libfsext-20240501/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/aclocal.m4` & `libfsext-20240501/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfsext-20240301/configure.ac` & `libfsext-20240501/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfsext],
- [20240301],
+ [20240501],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfsext.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

